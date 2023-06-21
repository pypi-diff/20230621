# Comparing `tmp/frontegg-2.1.4.tar.gz` & `tmp/frontegg-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frontegg-2.1.4.tar", max compression
+gzip compressed data, was "frontegg-2.1.6.tar", max compression
```

## Comparing `frontegg-2.1.4.tar` & `frontegg-2.1.6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1065 2022-10-13 14:59:50.240636 frontegg-2.1.4/LICENSE
--rw-r--r--   0        0        0      406 2023-02-02 10:01:16.057919 frontegg-2.1.4/README-PYPI.rst
--rw-r--r--   0        0        0      213 2022-12-11 12:48:40.494240 frontegg-2.1.4/frontegg/__init__.py
--rw-r--r--   0        0        0      243 2022-12-11 12:48:40.494450 frontegg-2.1.4/frontegg/common/__init__.py
--rw-r--r--   0        0        0      489 2023-02-02 10:01:22.637222 frontegg-2.1.4/frontegg/common/cache/cache_manager.py
--rw-r--r--   0        0        0     1206 2023-02-02 10:01:22.637491 frontegg-2.1.4/frontegg/common/cache/local_cache_manager.py
--rw-r--r--   0        0        0     1147 2023-02-02 10:01:22.637710 frontegg-2.1.4/frontegg/common/cache/redis_cache_manager.py
--rw-r--r--   0        0        0      202 2022-12-11 12:48:40.494652 frontegg-2.1.4/frontegg/common/clients/__init__.py
--rw-r--r--   0        0        0     1738 2022-12-11 12:48:40.494799 frontegg-2.1.4/frontegg/common/clients/audits_client.py
--rw-r--r--   0        0        0     3232 2022-12-11 12:48:40.494939 frontegg-2.1.4/frontegg/common/clients/http_client.py
--rw-r--r--   0        0        0     4338 2023-05-16 15:25:53.376931 frontegg-2.1.4/frontegg/common/clients/token_resolvers/access_token_resolver.py
--rw-r--r--   0        0        0      702 2023-02-02 10:01:22.638337 frontegg-2.1.4/frontegg/common/clients/token_resolvers/access_token_services/base_access_token_service.py
--rw-r--r--   0        0        0     2658 2023-05-16 15:25:53.377590 frontegg-2.1.4/frontegg/common/clients/token_resolvers/access_token_services/cache_services/cache_access_token_service.py
--rw-r--r--   0        0        0      985 2023-02-02 10:01:22.638891 frontegg-2.1.4/frontegg/common/clients/token_resolvers/access_token_services/cache_services/cache_tenant_access_token_service.py
--rw-r--r--   0        0        0      989 2023-02-02 10:01:22.639121 frontegg-2.1.4/frontegg/common/clients/token_resolvers/access_token_services/cache_services/cache_user_access_token_service.py
--rw-r--r--   0        0        0     1626 2023-02-02 10:01:22.639423 frontegg-2.1.4/frontegg/common/clients/token_resolvers/access_token_services/services/access_token_service.py
--rw-r--r--   0        0        0     1328 2023-02-02 10:01:22.639638 frontegg-2.1.4/frontegg/common/clients/token_resolvers/access_token_services/services/tenant_access_token_service.py
--rw-r--r--   0        0        0     1202 2023-02-02 10:01:22.639846 frontegg-2.1.4/frontegg/common/clients/token_resolvers/access_token_services/services/user_access_token_service.py
--rw-r--r--   0        0        0      968 2023-02-02 10:01:22.640079 frontegg-2.1.4/frontegg/common/clients/token_resolvers/authorization_header_resolver.py
--rw-r--r--   0        0        0     3563 2023-02-02 10:01:22.640311 frontegg-2.1.4/frontegg/common/clients/token_resolvers/token_resolver.py
--rw-r--r--   0        0        0     1352 2023-02-02 10:01:22.640525 frontegg-2.1.4/frontegg/common/clients/types.py
--rw-r--r--   0        0        0     1712 2022-12-11 12:48:40.495077 frontegg-2.1.4/frontegg/common/frontegg_authenticator.py
--rw-r--r--   0        0        0      351 2022-12-11 12:48:40.495204 frontegg-2.1.4/frontegg/common/frontegg_config.py
--rw-r--r--   0        0        0     1518 2023-05-16 15:29:09.508464 frontegg-2.1.4/frontegg/common/frontegg_context.py
--rw-r--r--   0        0        0     4225 2023-02-02 10:01:22.641738 frontegg-2.1.4/frontegg/common/identity_mixin.py
--rw-r--r--   0        0        0      250 2023-02-02 10:01:22.642005 frontegg-2.1.4/frontegg/common/package_utils.py
--rw-r--r--   0        0        0     4247 2023-03-22 13:04:42.099164 frontegg-2.1.4/frontegg/fastapi/README.md
--rw-r--r--   0        0        0       53 2022-10-13 14:59:50.242552 frontegg-2.1.4/frontegg/fastapi/__init__.py
--rw-r--r--   0        0        0     1620 2023-03-22 13:04:42.099816 frontegg-2.1.4/frontegg/fastapi/frontegg.py
--rw-r--r--   0        0        0      152 2022-12-11 12:48:40.497018 frontegg-2.1.4/frontegg/fastapi/secure_access/__init__.py
--rw-r--r--   0        0        0     4689 2023-05-16 15:29:09.509024 frontegg-2.1.4/frontegg/fastapi/secure_access/frontegg_security.py
--rw-r--r--   0        0        0     4164 2023-03-22 13:04:42.101047 frontegg-2.1.4/frontegg/flask/README.md
--rw-r--r--   0        0        0       53 2022-12-11 12:48:40.497924 frontegg-2.1.4/frontegg/flask/__init__.py
--rw-r--r--   0        0        0     1620 2023-03-22 13:04:42.101711 frontegg-2.1.4/frontegg/flask/frontegg.py
--rw-r--r--   0        0        0       86 2022-12-11 12:48:40.498654 frontegg-2.1.4/frontegg/flask/secure_access/__init__.py
--rw-r--r--   0        0        0     1820 2023-02-02 10:01:22.644681 frontegg-2.1.4/frontegg/flask/secure_access/with_authentication.py
--rw-r--r--   0        0        0      589 2022-12-11 12:48:40.499555 frontegg-2.1.4/frontegg/helpers/exceptions.py
--rw-r--r--   0        0        0     1669 2023-03-22 13:05:39.187041 frontegg-2.1.4/frontegg/helpers/frontegg_urls.py
--rw-r--r--   0        0        0      295 2022-10-13 14:59:50.243962 frontegg-2.1.4/frontegg/helpers/logger.py
--rw-r--r--   0        0        0      984 2022-12-11 12:48:40.500433 frontegg-2.1.4/frontegg/helpers/retry.py
--rw-r--r--   0        0        0     1582 2023-05-16 15:36:46.754671 frontegg-2.1.4/pyproject.toml
--rw-r--r--   0        0        0     1907 1970-01-01 00:00:00.000000 frontegg-2.1.4/setup.py
--rw-r--r--   0        0        0     1997 1970-01-01 00:00:00.000000 frontegg-2.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-10-13 14:59:50.240636 frontegg-2.1.6/LICENSE
+-rw-r--r--   0        0        0      406 2023-02-02 10:01:16.057919 frontegg-2.1.6/README-PYPI.rst
+-rw-r--r--   0        0        0      213 2023-06-18 07:04:25.922682 frontegg-2.1.6/frontegg/__init__.py
+-rw-r--r--   0        0        0      243 2023-06-18 07:04:25.923013 frontegg-2.1.6/frontegg/common/__init__.py
+-rw-r--r--   0        0        0      489 2023-06-18 07:04:25.923620 frontegg-2.1.6/frontegg/common/cache/cache_manager.py
+-rw-r--r--   0        0        0     1206 2023-06-18 07:04:25.924185 frontegg-2.1.6/frontegg/common/cache/local_cache_manager.py
+-rw-r--r--   0        0        0     1147 2023-06-18 07:04:25.924616 frontegg-2.1.6/frontegg/common/cache/redis_cache_manager.py
+-rw-r--r--   0        0        0      202 2023-06-18 07:04:25.925034 frontegg-2.1.6/frontegg/common/clients/__init__.py
+-rw-r--r--   0        0        0     1738 2023-06-18 07:04:25.925303 frontegg-2.1.6/frontegg/common/clients/audits_client.py
+-rw-r--r--   0        0        0     3506 2023-06-18 07:04:30.572278 frontegg-2.1.6/frontegg/common/clients/http_client.py
+-rw-r--r--   0        0        0     4338 2023-06-18 07:04:25.925865 frontegg-2.1.6/frontegg/common/clients/token_resolvers/access_token_resolver.py
+-rw-r--r--   0        0        0      702 2023-06-18 07:04:25.926270 frontegg-2.1.6/frontegg/common/clients/token_resolvers/access_token_services/base_access_token_service.py
+-rw-r--r--   0        0        0     2658 2023-06-18 07:04:25.926655 frontegg-2.1.6/frontegg/common/clients/token_resolvers/access_token_services/cache_services/cache_access_token_service.py
+-rw-r--r--   0        0        0      985 2023-06-18 07:04:25.926997 frontegg-2.1.6/frontegg/common/clients/token_resolvers/access_token_services/cache_services/cache_tenant_access_token_service.py
+-rw-r--r--   0        0        0      989 2023-06-18 07:04:25.927373 frontegg-2.1.6/frontegg/common/clients/token_resolvers/access_token_services/cache_services/cache_user_access_token_service.py
+-rw-r--r--   0        0        0     1801 2023-06-18 07:04:30.572728 frontegg-2.1.6/frontegg/common/clients/token_resolvers/access_token_services/services/access_token_service.py
+-rw-r--r--   0        0        0     1328 2023-06-18 07:04:25.928029 frontegg-2.1.6/frontegg/common/clients/token_resolvers/access_token_services/services/tenant_access_token_service.py
+-rw-r--r--   0        0        0     1238 2023-06-18 07:04:30.573137 frontegg-2.1.6/frontegg/common/clients/token_resolvers/access_token_services/services/user_access_token_service.py
+-rw-r--r--   0        0        0      968 2023-06-18 07:04:25.928568 frontegg-2.1.6/frontegg/common/clients/token_resolvers/authorization_header_resolver.py
+-rw-r--r--   0        0        0     3563 2023-06-18 07:04:25.928882 frontegg-2.1.6/frontegg/common/clients/token_resolvers/token_resolver.py
+-rw-r--r--   0        0        0     1382 2023-06-21 11:15:20.617134 frontegg-2.1.6/frontegg/common/clients/types.py
+-rw-r--r--   0        0        0     1736 2023-06-21 11:15:20.617810 frontegg-2.1.6/frontegg/common/frontegg_authenticator.py
+-rw-r--r--   0        0        0      351 2023-06-18 07:04:25.929610 frontegg-2.1.6/frontegg/common/frontegg_config.py
+-rw-r--r--   0        0        0     1518 2023-06-18 07:04:25.929880 frontegg-2.1.6/frontegg/common/frontegg_context.py
+-rw-r--r--   0        0        0     4236 2023-06-18 07:04:30.573772 frontegg-2.1.6/frontegg/common/identity_mixin.py
+-rw-r--r--   0        0        0      250 2023-06-18 07:04:25.930276 frontegg-2.1.6/frontegg/common/package_utils.py
+-rw-r--r--   0        0        0     4247 2023-06-18 07:04:25.930800 frontegg-2.1.6/frontegg/fastapi/README.md
+-rw-r--r--   0        0        0       53 2022-10-13 14:59:50.242552 frontegg-2.1.6/frontegg/fastapi/__init__.py
+-rw-r--r--   0        0        0     1620 2023-06-18 07:04:25.931185 frontegg-2.1.6/frontegg/fastapi/frontegg.py
+-rw-r--r--   0        0        0      152 2023-06-18 07:04:25.931640 frontegg-2.1.6/frontegg/fastapi/secure_access/__init__.py
+-rw-r--r--   0        0        0     4747 2023-06-21 11:15:20.618482 frontegg-2.1.6/frontegg/fastapi/secure_access/frontegg_security.py
+-rw-r--r--   0        0        0     4164 2023-06-18 07:04:25.932334 frontegg-2.1.6/frontegg/flask/README.md
+-rw-r--r--   0        0        0       53 2023-06-18 07:04:25.932620 frontegg-2.1.6/frontegg/flask/__init__.py
+-rw-r--r--   0        0        0     1620 2023-06-18 07:04:25.932999 frontegg-2.1.6/frontegg/flask/frontegg.py
+-rw-r--r--   0        0        0       86 2023-06-18 07:04:25.933554 frontegg-2.1.6/frontegg/flask/secure_access/__init__.py
+-rw-r--r--   0        0        0     1820 2023-06-18 07:04:25.933948 frontegg-2.1.6/frontegg/flask/secure_access/with_authentication.py
+-rw-r--r--   0        0        0      589 2023-06-18 07:04:25.934422 frontegg-2.1.6/frontegg/helpers/exceptions.py
+-rw-r--r--   0        0        0     1669 2023-06-18 07:04:25.934917 frontegg-2.1.6/frontegg/helpers/frontegg_urls.py
+-rw-r--r--   0        0        0      295 2022-10-13 14:59:50.243962 frontegg-2.1.6/frontegg/helpers/logger.py
+-rw-r--r--   0        0        0      984 2023-06-18 07:04:25.935451 frontegg-2.1.6/frontegg/helpers/retry.py
+-rw-r--r--   0        0        0     1582 2023-06-21 11:23:25.405797 frontegg-2.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1907 1970-01-01 00:00:00.000000 frontegg-2.1.6/setup.py
+-rw-r--r--   0        0        0     1997 1970-01-01 00:00:00.000000 frontegg-2.1.6/PKG-INFO
```

### Comparing `frontegg-2.1.4/LICENSE` & `frontegg-2.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.4/frontegg/common/cache/local_cache_manager.py` & `frontegg-2.1.6/frontegg/common/cache/local_cache_manager.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.4/frontegg/common/cache/redis_cache_manager.py` & `frontegg-2.1.6/frontegg/common/cache/redis_cache_manager.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.4/frontegg/common/clients/audits_client.py` & `frontegg-2.1.6/frontegg/common/clients/audits_client.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.4/frontegg/common/clients/http_client.py` & `frontegg-2.1.6/frontegg/common/clients/http_client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,15 @@
+import os
 from typing import Optional
 from requests import session, Response
 from ..frontegg_authenticator import FronteggAuthenticator
 from urllib.parse import urljoin
 
+timeout_in_seconds = os.environ.get('FRONTEGG_HTTP_TIMEOUT_IN_SECONDS') or '3'
+timeout_in_seconds = int(timeout_in_seconds)
 
 def merge(first: dict, second: dict):
     return {**first, **second}
 
 
 def combineUrl(base_url: str, endpoint: str):
     return urljoin(base_url, endpoint)
@@ -42,58 +45,58 @@
             params: Optional[dict] = None,
             tenant_id: Optional[str] = None,
             host: Optional[str] = None,
             headers: Optional[dict] = {}) -> Response:
         self.__prepare_auth_headers()
         new_headers = prepare_headers(tenant_id, host, headers)
 
-        return self.client.get(combineUrl(self.base_url, url), params=params, headers=new_headers)
+        return self.client.get(combineUrl(self.base_url, url), params=params, headers=new_headers, timeout=timeout_in_seconds)
 
     def post(self,
              data,
              url: str = '',
              tenant_id: Optional[str] = None,
              host: Optional[str] = None,
              headers: Optional[dict] = {}
              ) -> Response:
         self.__prepare_auth_headers()
 
         new_headers = prepare_headers(tenant_id, host, headers)
-        return self.client.post(combineUrl(self.base_url, url), json=data, headers=new_headers)
+        return self.client.post(combineUrl(self.base_url, url), json=data, headers=new_headers, timeout=timeout_in_seconds)
 
     def put(self,
             data,
             url: str = '',
             tenant_id: Optional[str] = None,
             host: Optional[str] = None,
             headers: Optional[dict] = {}
             ) -> Response:
         self.__prepare_auth_headers()
 
         new_headers = prepare_headers(tenant_id, host, headers)
-        return self.client.put(combineUrl(self.base_url, url), json=data, headers=new_headers)
+        return self.client.put(combineUrl(self.base_url, url), json=data, headers=new_headers, timeout=timeout_in_seconds)
 
     def delete(self,
                url: str = '',
                tenant_id: Optional[str] = None,
                host: Optional[str] = None,
                headers: Optional[dict] = {}
                ) -> Response:
         self.__prepare_auth_headers()
 
         new_headers = prepare_headers(tenant_id, host, headers)
-        return self.client.delete(combineUrl(self.base_url, url), headers=new_headers)
+        return self.client.delete(combineUrl(self.base_url, url), headers=new_headers, timeout=timeout_in_seconds)
 
     def patch(self,
               data,
               url: str = '',
               tenant_id: Optional[str] = None,
               host: Optional[str] = None,
               headers: Optional[dict] = {}
               ) -> Response:
         self.__prepare_auth_headers()
 
         new_headers = prepare_headers(tenant_id, host, headers)
-        return self.client.patch(combineUrl(self.base_url, url), json=data, headers=new_headers)
+        return self.client.patch(combineUrl(self.base_url, url), json=data, headers=new_headers, timeout=timeout_in_seconds)
 
 
 __all__ = 'HttpClient'
```

### Comparing `frontegg-2.1.4/frontegg/common/clients/token_resolvers/access_token_resolver.py` & `frontegg-2.1.6/frontegg/common/clients/token_resolvers/access_token_resolver.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.4/frontegg/common/clients/token_resolvers/access_token_services/base_access_token_service.py` & `frontegg-2.1.6/frontegg/common/clients/token_resolvers/access_token_services/base_access_token_service.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.4/frontegg/common/clients/token_resolvers/access_token_services/cache_services/cache_access_token_service.py` & `frontegg-2.1.6/frontegg/common/clients/token_resolvers/access_token_services/cache_services/cache_access_token_service.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.4/frontegg/common/clients/token_resolvers/access_token_services/cache_services/cache_tenant_access_token_service.py` & `frontegg-2.1.6/frontegg/common/clients/token_resolvers/access_token_services/cache_services/cache_tenant_access_token_service.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.4/frontegg/common/clients/token_resolvers/access_token_services/cache_services/cache_user_access_token_service.py` & `frontegg-2.1.6/frontegg/common/clients/token_resolvers/access_token_services/cache_services/cache_user_access_token_service.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.4/frontegg/common/clients/token_resolvers/access_token_services/services/access_token_service.py` & `frontegg-2.1.6/frontegg/common/clients/token_resolvers/access_token_services/services/access_token_service.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import abc
 import json
 from typing import List, TypeVar, Union
 from frontegg.common.clients.types import IAccessToken, IEntityWithRoles, TokenTypes
 from frontegg.helpers.exceptions import UnauthenticatedException
+from frontegg.helpers.logger import logger
 from frontegg.common.clients.token_resolvers.access_token_services.base_access_token_service import \
     BaseAccessTokenService
 
 T = TypeVar('T', bound=IAccessToken)
 
 
 class AccessTokenService(abc.ABC, BaseAccessTokenService[T]):
@@ -14,23 +15,25 @@
         self.type = type
 
     def get_entity(self, entity: T) -> IEntityWithRoles:
         try:
             data = self.get_entity_from_identity(entity)
             return data
         except Exception as e:
+            logger.exception('Failed to get entity from identity')
             if self.__is_api_tokens_disabled(e):
-                raise FailedToAuthenticateException()
+                raise UnauthenticatedException()
 
             raise e
 
     def get_active_access_token_ids(self) -> List[str]:
         try:
             return self.get_active_access_token_ids_from_identity()
         except Exception as e:
+            logger.exception('Failed to get active access token ids')
             if self.__is_api_tokens_disabled(e):
                 raise UnauthenticatedException()
 
             raise e
 
     @abc.abstractmethod
     def get_entity_from_identity(self, entity: T) -> IEntityWithRoles:
```

### Comparing `frontegg-2.1.4/frontegg/common/clients/token_resolvers/access_token_services/services/tenant_access_token_service.py` & `frontegg-2.1.6/frontegg/common/clients/token_resolvers/access_token_services/services/tenant_access_token_service.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.4/frontegg/common/clients/token_resolvers/access_token_services/services/user_access_token_service.py` & `frontegg-2.1.6/frontegg/common/clients/token_resolvers/access_token_services/services/user_access_token_service.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,10 +17,11 @@
         data = response.json()
 
         return {**entity, 'roles': data.get('roles'), 'permissions': data.get('permissions')}
 
     def get_active_access_token_ids_from_identity(self) -> List[str]:
         response = self.client.get(
             urljoin(frontegg_urls.identity_service['base_url'], 'resources/vendor-only/users/access-tokens/v1/active'))
+        response.raise_for_status()
         data = response.json()
 
         return data
```

### Comparing `frontegg-2.1.4/frontegg/common/clients/token_resolvers/authorization_header_resolver.py` & `frontegg-2.1.6/frontegg/common/clients/token_resolvers/authorization_header_resolver.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.4/frontegg/common/clients/token_resolvers/token_resolver.py` & `frontegg-2.1.6/frontegg/common/clients/token_resolvers/token_resolver.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.4/frontegg/common/clients/types.py` & `frontegg-2.1.6/frontegg/common/clients/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     metadata: Dict[str, any]
     userId: str
     name: Optional[str] = None
     email: Optional[str] = None
     email_verified: Optional[bool] = None
     invisible: Optional[bool] = None
     tenantId: str
+    superUser: Optional[bool]
 
 
 class IAccessToken(IEntity):
     type: Union[TokenTypes.TenantAccessToken.value, TokenTypes.UserAccessToken.value]
 
 
 class ITenantAccessToken(IAccessToken):
```

### Comparing `frontegg-2.1.4/frontegg/common/frontegg_authenticator.py` & `frontegg-2.1.6/frontegg/common/frontegg_authenticator.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,18 +28,18 @@
         body = {
             'clientId': self.client_id,
             'secret': self.api_key
         }
         logger.info('Will refresh vendor token')
         auth_url = frontegg_urls.authentication_service['authenticate_vendor']
 
-        auth_response = self.vendor_session_request.post(auth_url, json=body)
+        auth_response = self.vendor_session_request.post(auth_url, json=body, timeout=3)
         auth_response.raise_for_status()
         logger.info('Got a new vendor token from frontegg')
         response_body = auth_response.json()
         self.__access_token = response_body['token']
         self.__access_token_expiration = calcTokenExpiration(response_body['expiresIn'])
-        self.vendor_session_request.headers.update({'x-access-token': self.__access_token})
+        self.vendor_session_request.headers.update({'x-access-token': self.__access_token}, timeout='3')
         logger.info('New vendor token was set successfully')
 
 
 def calcTokenExpiration(expiration): return arrow.utcnow().shift(seconds=expiration * 0.8)
```

### Comparing `frontegg-2.1.4/frontegg/common/frontegg_context.py` & `frontegg-2.1.6/frontegg/common/frontegg_context.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.4/frontegg/common/identity_mixin.py` & `frontegg-2.1.6/frontegg/common/identity_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         logger.error('failed to get public key in all retries')
 
     def fetch_public_key(self) -> str:
         if self.__authenticator.should_refresh_vendor_token:
             self.__authenticator.refresh_vendor_token()
 
         response = self.__authenticator.vendor_session_request.get(
-            frontegg_urls.identity_service['vendor_config'])
+            frontegg_urls.identity_service['vendor_config'], timeout=3)
         response.raise_for_status()
         data = response.json()
         return data.get('publicKey')
 
     def validate_identity_on_token(
             self,
             token,
```

### Comparing `frontegg-2.1.4/frontegg/fastapi/README.md` & `frontegg-2.1.6/frontegg/fastapi/README.md`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.4/frontegg/fastapi/frontegg.py` & `frontegg-2.1.6/frontegg/fastapi/frontegg.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.4/frontegg/fastapi/secure_access/frontegg_security.py` & `frontegg-2.1.6/frontegg/fastapi/secure_access/frontegg_security.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     # User token fields - all fields must be optional in order to support API tokens
     metadata: Optional[Dict[str, Any]]
     name: Optional[str]
     email: Optional[str]
     email_verified: Optional[bool]
     tenant_ids: Optional[List[str]] = Field(alias='tenantIds', default_factory=list)
     profile_picture_url: Optional[str] = Field(alias='profilePictureUrl')
+    super_user: Optional[bool] = Field(alias='superUser')
 
     # API Token fields - all fields must be optional in order to support user tokens
     created_by_user_id: Optional[str] = Field(alias='createdByUserId')
 
     def has_permissions(self, permissions: List[str]) -> bool:
         return bool(permissions) and all(p in self.permissions for p in permissions)
```

### Comparing `frontegg-2.1.4/frontegg/flask/README.md` & `frontegg-2.1.6/frontegg/flask/README.md`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.4/frontegg/flask/frontegg.py` & `frontegg-2.1.6/frontegg/flask/frontegg.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.4/frontegg/flask/secure_access/with_authentication.py` & `frontegg-2.1.6/frontegg/flask/secure_access/with_authentication.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.4/frontegg/helpers/exceptions.py` & `frontegg-2.1.6/frontegg/helpers/exceptions.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.4/frontegg/helpers/frontegg_urls.py` & `frontegg-2.1.6/frontegg/helpers/frontegg_urls.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.4/frontegg/helpers/retry.py` & `frontegg-2.1.6/frontegg/helpers/retry.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.4/pyproject.toml` & `frontegg-2.1.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "frontegg"
-version = "2.1.4"
+version = "2.1.6"
 description = "Frontegg is a web platform where SaaS companies can set up their fully managed, scalable and brand aware - SaaS features and integrate them into their SaaS portals in up to 5 lines of code."
 homepage = "https://frontegg.com/"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
```

### Comparing `frontegg-2.1.4/setup.py` & `frontegg-2.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
  'typing-extensions>=4.4.0,<5.0.0']
 
 extras_require = \
 {'fastapi': ['fastapi'], 'flask': ['flask>=1.0,<2.0']}
 
 setup_kwargs = {
     'name': 'frontegg',
-    'version': '2.1.4',
+    'version': '2.1.6',
     'description': 'Frontegg is a web platform where SaaS companies can set up their fully managed, scalable and brand aware - SaaS features and integrate them into their SaaS portals in up to 5 lines of code.',
     'long_description': '.. image:: https://fronteggstuff.blob.core.windows.net/frongegg-logos/logo-transparent.png\n   :alt: Frontegg\n\nFrontegg is a web platform where SaaS companies can set up their fully managed, scalable and brand aware - SaaS features and integrate them into their SaaS portals in up to 5 lines of code.\n\nFor more information and usage you can visit the `github repo <https://github.com/frontegg/python-sdk>`_.',
     'author': 'Frontegg LTD',
     'author_email': 'hello@frontegg.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://frontegg.com/',
```

### Comparing `frontegg-2.1.4/PKG-INFO` & `frontegg-2.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frontegg
-Version: 2.1.4
+Version: 2.1.6
 Summary: Frontegg is a web platform where SaaS companies can set up their fully managed, scalable and brand aware - SaaS features and integrate them into their SaaS portals in up to 5 lines of code.
 Home-page: https://frontegg.com/
 Author: Frontegg LTD
 Author-email: hello@frontegg.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
```

