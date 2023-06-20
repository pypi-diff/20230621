# Comparing `tmp/robocorp_storage-0.1.0.tar.gz` & `tmp/robocorp_storage-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_storage-0.1.0.tar", max compression
+gzip compressed data, was "robocorp_storage-0.1.1.tar", max compression
```

## Comparing `robocorp_storage-0.1.0.tar` & `robocorp_storage-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      388 2023-06-19 16:18:13.338583 robocorp_storage-0.1.0/README.md
--rw-r--r--   0        0        0      635 2023-06-19 16:18:13.339305 robocorp_storage-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5408 2023-06-19 16:18:13.339455 robocorp_storage-0.1.0/src/robocorp/storage/__init__.py
--rw-r--r--   0        0        0     6538 2023-06-19 16:18:13.339559 robocorp_storage-0.1.0/src/robocorp/storage/_requests.py
--rw-r--r--   0        0        0     1487 2023-06-19 16:18:13.339675 robocorp_storage-0.1.0/src/robocorp/storage/_storage.py
--rw-r--r--   0        0        0     1260 2023-06-19 16:18:13.339779 robocorp_storage-0.1.0/src/robocorp/storage/_utils.py
--rw-r--r--   0        0        0        0 2023-06-19 16:18:13.339813 robocorp_storage-0.1.0/src/robocorp/storage/py.typed
--rw-r--r--   0        0        0      893 1970-01-01 00:00:00.000000 robocorp_storage-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      388 2023-06-20 23:01:39.204147 robocorp_storage-0.1.1/README.md
+-rw-r--r--   0        0        0      801 2023-06-20 23:01:39.204147 robocorp_storage-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5317 2023-06-20 23:01:39.204147 robocorp_storage-0.1.1/src/robocorp/storage/__init__.py
+-rw-r--r--   0        0        0     6642 2023-06-20 23:01:39.204147 robocorp_storage-0.1.1/src/robocorp/storage/_requests.py
+-rw-r--r--   0        0        0     1759 2023-06-20 23:01:39.204147 robocorp_storage-0.1.1/src/robocorp/storage/_storage.py
+-rw-r--r--   0        0        0     1203 2023-06-20 23:01:39.204147 robocorp_storage-0.1.1/src/robocorp/storage/_utils.py
+-rw-r--r--   0        0        0        0 2023-06-20 23:01:39.204147 robocorp_storage-0.1.1/src/robocorp/storage/py.typed
+-rw-r--r--   0        0        0     1255 1970-01-01 00:00:00.000000 robocorp_storage-0.1.1/PKG-INFO
```

### Comparing `robocorp_storage-0.1.0/src/robocorp/storage/__init__.py` & `robocorp_storage-0.1.1/src/robocorp/storage/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,169 +1,172 @@
+import functools
 import logging
 import random
 import time
-from typing import List, Optional, cast
+from typing import List, cast
+
+import requests
 
 from ._requests import RequestsHTTPError
-from ._storage import Asset, AssetMeta, AssetNotFound
+from ._storage import Asset, AssetMeta, AssetNotFound, AssetUploadFailed
 from ._storage import get_assets_client as _get_assets_client
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 version_info = [int(x) for x in __version__.split(".")]
 
 LOGGER = logging.getLogger(__name__)
 
 
+def _handle_missing_asset(response: requests.Response, *, name: str, asset_id: str):
+    assets_client = _get_assets_client()
+    try:
+        assets_client.handle_error(response)
+    except RequestsHTTPError as exc:
+        if exc.status_code == 404:
+            # NOTE(cmin764): Any `404 Not Found` error won't be retried and will
+            #  bubble-up from the first request.
+            message = f"Asset {name!r} with id {asset_id!r} not found"
+            raise AssetNotFound(
+                message, status_code=exc.status_code, status_message=exc.status_message
+            ) from exc
+        else:
+            raise exc
+
+
 def list_assets() -> List[AssetMeta]:
     """List all the existing assets.
 
     Returns:
         A list of assets where each asset is a dictionary with fields like 'id' and
-        'name'.
+        'name'
     """
     assets_client = _get_assets_client()
     assets = assets_client.get("").json()
-    LOGGER.info("Found %d assets.", len(assets))
+    LOGGER.debug("Retrieved %d assets", len(assets))
     return assets
 
 
 def _retrieve_asset_id(name: str) -> str:
     for asset in list_assets():
         if asset["name"] == name:
             asset_id = asset["id"]
-            LOGGER.debug("Found existing asset %r with ID: %s", name, asset_id)
+            LOGGER.debug("Found existing asset %r with id: %s", name, asset_id)
             return asset_id
 
-    LOGGER.warning("No asset with name %r found, assuming ID.", name)
+    LOGGER.warning("No asset with name %r found, assuming id", name)
     return name
 
 
-def _get_asset(name: str, raise_if_missing: bool = True) -> Optional[Asset]:
-    assets_client = _get_assets_client()
+def _get_asset(name: str) -> Asset:
     asset_id = _retrieve_asset_id(name)
-    exception = None
-
-    def _handle_error(resp):
-        # NOTE(cmin764): The API will return 404 if the asset can't be found on the
-        #  server, therefore don't let this raise, nor retry given this custom handler.
-        nonlocal exception
-        try:
-            assets_client.handle_error(resp)
-        except RequestsHTTPError as exc:
-            if exc.status_code == 404:
-                exception = exc
-            else:
-                raise
 
-    LOGGER.debug("Retrieving asset %r with resulted ID %r.", name, asset_id)
+    assets_client = _get_assets_client()
+    _handle_error = functools.partial(
+        _handle_missing_asset, name=name, asset_id=asset_id
+    )
     response = assets_client.get(asset_id, _handle_error=_handle_error)
-    if response.ok:
-        return cast(Asset, response.json())
-
-    message = f"asset with name {name!r} and resulted ID {asset_id!r} couldn't be found"
-    if raise_if_missing:
-        raise AssetNotFound(message) from exception
-
-    LOGGER.warning("%s%s!", message[0].upper(), message[1:])
-    return None
+    return cast(Asset, response.json())
 
 
 def get_asset(name: str) -> str:
-    """Get the asset's value by providing its `name`.
+    """Get an asset's value by providing its `name`.
 
     Args:
-        name: Name of the asset to fetch.
+        name: Name of the asset
 
     Returns:
-        The previously set value of this asset. (empty if it was never set)
+        The previously set value of this asset, or empty string if not set
 
     Raises:
-        AssetNotFound: When the queried asset doesn't exist.
+        AssetNotFound: Asset with given name does not exist
     """
-    LOGGER.info("Retrieving asset %r.", name)
-    payload = _get_asset(name)["payload"]  # type: ignore
+    LOGGER.info("Retrieving asset: %r", name)
+    payload = _get_asset(name)["payload"]
     if payload["type"] == "empty":
-        LOGGER.warning("Asset %r has no value set!", name)
+        LOGGER.warning("Asset %r has no value set", name)
         return ""
 
     assets_client = _get_assets_client()
     url = payload["url"]
     return assets_client.get(url, headers={}).text
 
 
-def _create_asset(name: str):
-    LOGGER.debug("Creating new asset with name %r.", name)
+def _create_asset(name: str) -> Asset:
+    LOGGER.debug("Creating new asset with name: %r", name)
     assets_client = _get_assets_client()
     body = {"name": name}
     return assets_client.post("", json=body).json()
 
 
 def set_asset(name: str, value: str, wait: bool = True):
-    """Sets/Creates an asset named `name` with the provided `value`.
+    """Creates or updates an asset named `name` with the provided `value`.
 
     Args:
-        name: Name of the existing or new asset to create. (if missing)
-        value: The new value set within the asset.
-        wait: Blocks until the new value is reflected within the asset.
+        name: Name of the existing or new asset to create (if missing)
+        value: The new value to set within the asset
+        wait: Wait for value to be set successfully
 
     Raises:
-        AssetNotFound: When the queried asset doesn't exist.
+        AssetUploadFailed: Unexpected error while uploading the asset
     """
-    existing_asset = _get_asset(name, raise_if_missing=False)
-    if existing_asset:
-        asset_id = existing_asset["id"]
-        LOGGER.debug("Updating already existing asset with ID %r.", asset_id)
-    else:
+    try:
+        asset_id = _get_asset(name)["id"]
+        LOGGER.debug("Updating existing asset with id: %r", asset_id)
+    except AssetNotFound:
         asset_id = _create_asset(name)["id"]
-        LOGGER.debug("Updating newly created asset with ID %r.", asset_id)
+        LOGGER.debug("Created new asset with id: %r", asset_id)
 
     assets_client = _get_assets_client()
     body = {"content_type": "text/plain"}
     upload_data = assets_client.post(f"{asset_id}/upload", json=body).json()
     assets_client.put(upload_data["upload_url"], data=value, headers={})
 
-    if wait:
-        LOGGER.info(
-            "Waiting for the sent value to be set successfully in the %r asset...", name
-        )
-        upload_url = f"{asset_id}/uploads/{upload_data['id']}"
-        while True:
-            upload_data = assets_client.get(upload_url).json()
-            status = upload_data["status"]
-            if status == "pending":
-                sleep_time = round(random.uniform(0, 1), 2)
-                LOGGER.debug("Asset upload still pending, sleeping %.2f...", sleep_time)
-                time.sleep(sleep_time)
-                continue
-            elif status == "completed":
-                break
-            elif status == "failed":
-                raise ValueError(
-                    f"asset {name!r} upload failed with {upload_data['reason']!r}"
-                )
-            else:
-                raise TypeError(f"asset {name!r} got invalid status {status!r}")
+    if not wait:
+        return
+
+    LOGGER.info("Waiting for asset %r value to update successfully", name)
+    upload_url = f"{asset_id}/uploads/{upload_data['id']}"
+    while True:
+        upload_data = assets_client.get(upload_url).json()
+        status = upload_data["status"]
+        if status == "pending":
+            sleep_time = round(random.uniform(0, 1), 2)
+            LOGGER.debug("Asset upload still pending, sleeping %.2f...", sleep_time)
+            time.sleep(sleep_time)
+            continue
+        elif status == "completed":
+            break
+        elif status == "failed":
+            reason = upload_data["reason"]
+            raise AssetUploadFailed(f"Asset {name!r} upload failed: {reason}")
+        else:
+            raise AssetUploadFailed(f"Asset {name!r} got invalid status: {status}")
 
-    LOGGER.info("Asset with name %r set successfully.", name)
+    LOGGER.info("Asset %r set successfully", name)
 
 
 def delete_asset(name: str):
     """Delete an asset by providing its `name`.
 
     Args:
-        name: Name of the asset to delete.
+        name: Name of the asset to delete
 
     Raises:
-        AssetNotFound: When the queried asset doesn't exist.
+        AssetNotFound: Asset with the given name does not exist
     """
-    LOGGER.info("Deleting asset %r.", name)
+    LOGGER.info("Deleting asset: %r", name)
+    asset_id = _retrieve_asset_id(name)
     assets_client = _get_assets_client()
-    assets_client.delete(_get_asset(name)["id"])  # type: ignore
+    _handle_error = functools.partial(
+        _handle_missing_asset, name=name, asset_id=asset_id
+    )
+    assets_client.delete(asset_id, _handle_error=_handle_error)
 
 
 __all__ = [
     "AssetNotFound",
-    "list_assets",
+    "AssetUploadFailed",
+    "delete_asset",
     "get_asset",
+    "list_assets",
     "set_asset",
-    "delete_asset",
 ]
```

### Comparing `robocorp_storage-0.1.0/src/robocorp/storage/_requests.py` & `robocorp_storage-0.1.1/src/robocorp/storage/_requests.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,25 +23,26 @@
 def _needs_retry(exc: BaseException) -> bool:
     # Don't retry on some specific error codes or messages.
 
     # https://www.restapitutorial.com/httpstatuscodes.html
     # 400 - payload is bad and needs to be changed
     # 401 - missing auth bearer token
     # 403 - auth is in place, but not allowed (insufficient privileges)
+    # 404 - resource does not exist
     # 409 - payload not good for the affected resource
-    no_retry_codes = [400, 401, 403, 409]
+    no_retry_codes = [400, 401, 403, 404, 409]
 
     if isinstance(exc, RequestsHTTPError):
         if exc.status_code in no_retry_codes:
             return False
 
         if exc.status_code == 429:
-            # We hit the rate limiter, so sleep extra.
-            seconds = random.uniform(1, 3)
-            LOGGER.warning("Rate limit hit, sleeping: %fs", seconds)
+            # We hit the rate limiter, so sleep extra before retrying.
+            seconds = round(random.uniform(1, 3), 2)
+            LOGGER.warning("Rate limit hit, sleeping %.2fs...", seconds)
             time.sleep(seconds)
 
     return True
 
 
 def _before_sleep_log():
     log_method = LOGGER.log
@@ -57,15 +58,19 @@
     return before_sleep_log(LOGGER, logging.DEBUG, exc_info=True)
 
 
 class RequestsHTTPError(HTTPError):
     """Custom `requests` HTTP error with status code and message."""
 
     def __init__(
-        self, *args, status_code: int = 0, status_message: str = "Error", **kwargs
+        self,
+        *args,
+        status_code: int = 0,
+        status_message: str = "Error",
+        **kwargs,
     ):
         super().__init__(*args, **kwargs)
 
         self.status_code = status_code
         self.status_message = status_message
```

### Comparing `robocorp_storage-0.1.0/src/robocorp/storage/_storage.py` & `robocorp_storage-0.1.1/src/robocorp/storage/_storage.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,48 @@
 import logging
+import sys
 from functools import lru_cache
-from typing import Dict, Optional, TypedDict
+from typing import Dict, Optional
 
-from ._requests import Requests
+from ._requests import Requests, RequestsHTTPError
 from ._utils import RequiresEnv, url_join
 
-LOGGER = logging.getLogger(__name__)
+if sys.version_info >= (3, 8):
+    from typing import TypedDict
+else:
+    from typing_extensions import TypedDict
+
 
+LOGGER = logging.getLogger(__name__)
 
 AssetMeta = Dict[str, str]
 Payload = TypedDict(
-    "Payload", {"type": str, "content_type": Optional[str], "url": Optional[str]}
+    "Payload",
+    {
+        "type": str,
+        "content_type": Optional[str],
+        "url": Optional[str],
+    },
 )
 Asset = TypedDict(
     "Asset",
     {
         "id": str,
         "name": str,
         "payload": Payload,
     },
 )
 
 
-class AssetNotFound(KeyError):
-    """Raised when the queried asset couldn't be found."""
+class AssetNotFound(RequestsHTTPError):
+    """No asset with given name/id found."""
+
+
+class AssetUploadFailed(RuntimeError):
+    """There was an unexpected error while uploading an asset."""
 
 
 @lru_cache(maxsize=1)
 def get_assets_client():
     """Creates and returns an API client based on the injected env vars in CR."""
     requires_env = RequiresEnv(
         "Asset Storage feature can be used with Control Room only"
```

### Comparing `robocorp_storage-0.1.0/src/robocorp/storage/_utils.py` & `robocorp_storage-0.1.1/src/robocorp/storage/_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import functools
 import os
 import urllib.parse as urlparse
-from typing import Any, Optional
+from typing import Any
 
 # Sentinel value for undefined arguments.
 UNDEFINED = object()
 
 
 def required_env(name: str, default: Any = UNDEFINED) -> str:
     """Load required environment variable.
 
     Args:
-        name: Name of the requested environment variable.
+        name: Name of the requested environment variable
         default: Value to return if no such env var is found, otherwise `KeyError` is
-            raised.
+            raised
     """
     val = os.getenv(name, default)
     if val is UNDEFINED:
         raise KeyError(f"Missing required environment variable: {name}")
     return val
 
 
@@ -31,16 +31,13 @@
     def __call__(self, *args, **kwargs):
         try:
             return required_env(*args, **kwargs)
         except Exception as exc:
             raise self._exception from exc
 
 
-def url_join(*parts: str) -> Optional[str]:
-    """Join parts of URL and handle missing/duplicate slashes."""
-    if not parts:
-        return None
-
+def url_join(*parts: str) -> str:
+    """Join parts into a URL and handle missing/duplicate slashes."""
     url = ""
     for part in parts:
         url = urlparse.urljoin(url, part.strip("/") + "/")
     return url
```

### Comparing `robocorp_storage-0.1.0/PKG-INFO` & `robocorp_storage-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 Metadata-Version: 2.1
 Name: robocorp-storage
-Version: 0.1.0
+Version: 0.1.1
 Summary: Robocorp Asset Storage library
+Home-page: https://github.com/robocorp/robo/
+License: Apache-2.0
 Author: Cosmin P.
 Author-email: cosmin@robocorp.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: tenacity (>=8.0.1,<9.0.0)
+Requires-Dist: typing-extensions (>=4.6.3,<5.0.0) ; python_version < "3.8"
+Project-URL: Repository, https://github.com/robocorp/robo/
 Description-Content-Type: text/markdown
 
 # Robocorp Control Room Asset Storage API library
 
 `robocorp-storage` is a library which provides read and write access to the
 *Asset Storage* in Robocorp **Control Room**.
```

