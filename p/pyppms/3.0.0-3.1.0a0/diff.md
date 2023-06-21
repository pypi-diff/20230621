# Comparing `tmp/pyppms-3.0.0.tar.gz` & `tmp/pyppms-3.1.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyppms-3.0.0.tar", max compression
+gzip compressed data, was "pyppms-3.1.0a0.tar", max compression
```

## Comparing `pyppms-3.0.0.tar` & `pyppms-3.1.0a0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     2942 2022-04-20 07:35:38.348949 pyppms-3.0.0/README.md
--rw-r--r--   0        0        0     1146 2023-06-20 11:18:22.862069 pyppms-3.0.0/pyproject.toml
--rw-r--r--   0        0        0      231 2023-04-26 16:03:26.526029 pyppms-3.0.0/src/pyppms/__init__.py
--rw-r--r--   0        0        0     5593 2023-06-20 11:17:40.005575 pyppms-3.0.0/src/pyppms/booking.py
--rw-r--r--   0        0        0     7035 2023-06-20 11:17:40.005575 pyppms-3.0.0/src/pyppms/common.py
--rw-r--r--   0        0        0    46975 2023-06-20 11:17:40.009575 pyppms-3.0.0/src/pyppms/ppms.py
--rw-r--r--   0        0        0     3944 2023-06-20 11:17:40.009575 pyppms-3.0.0/src/pyppms/system.py
--rw-r--r--   0        0        0     2270 2023-06-20 11:17:40.009575 pyppms-3.0.0/src/pyppms/user.py
--rw-r--r--   0        0        0     3776 1970-01-01 00:00:00.000000 pyppms-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2942 2022-04-20 07:35:38.348949 pyppms-3.1.0a0/README.md
+-rw-r--r--   0        0        0     1148 2023-06-20 11:54:30.827850 pyppms-3.1.0a0/pyproject.toml
+-rw-r--r--   0        0        0      231 2023-04-26 16:03:26.526029 pyppms-3.1.0a0/src/pyppms/__init__.py
+-rw-r--r--   0        0        0     5657 2023-06-20 11:50:46.845568 pyppms-3.1.0a0/src/pyppms/booking.py
+-rw-r--r--   0        0        0     7551 2023-06-20 11:40:07.471530 pyppms-3.1.0a0/src/pyppms/common.py
+-rw-r--r--   0        0        0    47070 2023-06-20 11:53:20.255126 pyppms-3.1.0a0/src/pyppms/ppms.py
+-rw-r--r--   0        0        0     3944 2023-06-20 11:17:40.009575 pyppms-3.1.0a0/src/pyppms/system.py
+-rw-r--r--   0        0        0     2270 2023-06-20 11:17:40.009575 pyppms-3.1.0a0/src/pyppms/user.py
+-rw-r--r--   0        0        0     3778 1970-01-01 00:00:00.000000 pyppms-3.1.0a0/PKG-INFO
```

### Comparing `pyppms-3.0.0/README.md` & `pyppms-3.1.0a0/README.md`

 * *Files identical despite different names*

### Comparing `pyppms-3.0.0/pyproject.toml` & `pyppms-3.1.0a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 description = "A Python package to communicate with Stratocore's PUMAPI."
 name = "pyppms"
-version = "3.0.0"
+version = "3.1.0a0"
 
 license = "GPLv3"
 
 authors = [
   "Niko Ehrenfeuchter <nikolaus.ehrenfeuchter@unibas.ch>",
   "Laurent Guerard <laurent.guerard@unibas.ch>",
 ]
```

### Comparing `pyppms-3.0.0/src/pyppms/booking.py` & `pyppms-3.1.0a0/src/pyppms/booking.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Module representing bookings / reservations in PPMS."""
 
 from datetime import datetime
 
 from loguru import logger as log
 
-from .common import time_rel_to_abs
+from .common import time_rel_to_abs, fmt_time
 
 
 class PpmsBooking:
 
     """Object representing a booking (reservation) in PPMS.
 
     Attributes
@@ -118,15 +118,15 @@
         start = date.replace(
             hour=int(time_str.split(":")[0]),
             minute=int(time_str.split(":")[1]),
             second=0,
             microsecond=0,
         )
         self.starttime = start
-        log.debug("New starttime: {}", self)
+        log.trace("New starttime: {}", self)
 
     def endtime_fromstr(self, time_str, date=None):
         """Change the ending time and / or day of a booking.
 
         Parameters
         ----------
         time_str : str
@@ -140,28 +140,35 @@
         end = date.replace(
             hour=int(time_str.split(":")[0]),
             minute=int(time_str.split(":")[1]),
             second=0,
             microsecond=0,
         )
         self.endtime = end
-        log.debug("New endtime: {}", self)
+        log.trace("New endtime: {}", self)
 
     def __str__(self):
-        def fmt_time(time):
-            # in case a booking was created from a "nextbooking" response it will not
-            # have the `endtime` attribute set, so treat this separately:
-            if time is None:
-                return "===UNDEFINED==="
-            return datetime.strftime(time, "%Y-%m-%d %H:%M")
-
         msg = (
             f"PpmsBooking(username=[{self.username}], "
             f"system_id=[{self.system_id}], "
             f"starttime=[{fmt_time(self.starttime)}], "
             f"endtime=[{fmt_time(self.endtime)}]"
         )
         if self.session:
             msg += f", session=[{self.session}]"
         msg += ")"
 
         return msg
+
+    @property
+    def desc(self):
+        """Format a "short" description of the object.
+
+        Returns
+        -------
+        str
+            A string containing `username`, `system_id` and the booking times.
+        """
+        return (
+            f"{self.username}@{self.system_id} "
+            f"[{fmt_time(self.starttime)} -- {fmt_time(self.endtime)}]"
+        )
```

### Comparing `pyppms-3.0.0/src/pyppms/common.py` & `pyppms-3.1.0a0/src/pyppms/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -194,7 +194,27 @@
     -------
     datetime
         The absolute time point as a datetime object.
     """
     now = datetime.now().replace(second=0, microsecond=0)
     abstime = now + timedelta(minutes=int(minutes_from_now))
     return abstime
+
+
+def fmt_time(time):
+    """Format a `datetime` or `None` object to string.
+
+    This is useful to apply it to booking times as they might be `None` e.g. in
+    case they have been created from a "nextbooking" response.
+
+    Parameters
+    ----------
+    time : datetime.datetime or None
+
+    Returns
+    -------
+    str
+        The formatted time, or a specific string in case the input was `None`.
+    """
+    if time is None:
+        return "===UNDEFINED==="
+    return datetime.strftime(time, "%Y-%m-%d %H:%M")
```

### Comparing `pyppms-3.0.0/src/pyppms/ppms.py` & `pyppms-3.1.0a0/src/pyppms/ppms.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
             "Attempting authentication against {} with key [{}...{}]",
             self.url,
             self.api_key[:2],
             self.api_key[-2:],
         )
         self.status["auth_state"] = "attempting"
         response = self.request("auth")
-        log.debug(f"Authenticate response: {response.text}")
+        log.trace(f"Authenticate response: {response.text}")
         self.status["auth_response"] = response.text
         self.status["auth_httpstatus"] = response.status_code
 
         # NOTE: an unauthorized request has already been caught be the request() method
         # above. Our legacy code was additionally testing for 'error' in the response
         # text - however, it is unclear if PUMAPI ever returns this:
         if "error" in response.text.lower():
@@ -162,16 +162,19 @@
             msg = (
                 f"Authenticating against {self.url} with key "
                 f"[{self.api_key[:2]}...{self.api_key[-2:]}] FAILED!"
             )
             log.error(msg)
             raise requests.exceptions.ConnectionError(msg)
 
-        log.info(f"Authentication succeeded, response=[{response.text}]")
-        log.debug(f"HTTP Status: {response.status_code}")
+        log.info(
+            "Authentication succeeded, response=[{}], http_status=[{}]",
+            response.text,
+            response.status_code,
+        )
         self.status["auth_state"] = "good"
 
     def request(self, action, parameters={}, skip_cache=False):
         """Generic method to submit a request to PPMS and return the result.
 
         This convenience method deals with adding the API key to a given
         request, submitting it to the PUMAPI and checking the response for some
@@ -245,22 +248,22 @@
         str
             The full path to a file name identified by all parameters of the
             request (except credentials like 'apikey').
         """
         action = req_data["action"]
 
         if self.cache_users_only and action != "getuser":
-            log.debug(f"NOT caching '{action}' (cache_users_only is set)")
+            log.trace(f"NOT caching '{action}' (cache_users_only is set)")
             return None
 
         intercept_dir = os.path.join(self.cache_path, action)
         if create_dir and not os.path.exists(intercept_dir):  # pragma: no cover
             try:
                 os.makedirs(intercept_dir)
-                log.debug(f"Created dir to store response: {intercept_dir}")
+                log.trace(f"Created dir to store response: {intercept_dir}")
             except Exception as err:  # pylint: disable-msg=broad-except
                 log.warning(f"Failed creating [{intercept_dir}]: {err}")
                 return None
 
         signature = ""
         # different python versions are returning dict items in different order, so
         # simply iterating over them will not always produce the same result - hence we
@@ -312,15 +315,18 @@
 
         intercept_file = self.__interception_path(req_data, create_dir=False)
         if not intercept_file or not os.path.exists(intercept_file):  # pragma: no cover
             raise LookupError(f"No cache hit for [{intercept_file}]")
 
         with open(intercept_file, "r", encoding="utf-8") as infile:
             text = infile.read()
-        log.debug(f"Read intercepted response text from [{intercept_file}]")
+        log.debug(
+            "Read intercepted response text from [{}]",
+            intercept_file[len(str(self.cache_path)) :],
+        )
 
         status_code = 200
         status_file = os.path.splitext(intercept_file)[0] + "_status-code.txt"
         if os.path.exists(status_file):
             with open(status_file, "r", encoding="utf-8") as infile:
                 status_code = infile.read()
             log.debug(f"Read intercepted response status code from [{status_file}]")
@@ -698,28 +704,28 @@
             loc_desc,
             name_contains,
         )
         system_ids = []
         systems = self.get_systems()
         for sys_id, system in systems.items():
             if loc.lower() not in str(system.localisation).lower():
-                log.debug(
+                log.trace(
                     "System [{}] location ({}) is NOT matching ({}), ignoring",
                     system.name,
                     system.localisation,
                     loc,
                 )
                 continue
 
             # log.debug('System [{}] is matching location [{}], checking if '
             #           'the name is matching any of the valid pattern {}',
             #           system.name, loc, name_contains)
             for valid_name in name_contains:
                 if valid_name in system.name:
-                    log.debug("System [{}] matches all criteria", system.name)
+                    log.trace("System [{}] matches all criteria", system.name)
                     system_ids.append(sys_id)
                     break
 
             # if sys_id not in system_ids:
             #     log.debug('System [{}] does NOT match a valid name: {}',
             #               system.name, name_contains)
```

### Comparing `pyppms-3.0.0/src/pyppms/system.py` & `pyppms-3.1.0a0/src/pyppms/system.py`

 * *Files identical despite different names*

### Comparing `pyppms-3.0.0/src/pyppms/user.py` & `pyppms-3.1.0a0/src/pyppms/user.py`

 * *Files identical despite different names*

### Comparing `pyppms-3.0.0/PKG-INFO` & `pyppms-3.1.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyppms
-Version: 3.0.0
+Version: 3.1.0a0
 Summary: A Python package to communicate with Stratocore's PUMAPI.
 Home-page: https://pypi.org/project/pyppms/
 License: GPLv3
 Keywords: ppms,pumapi,booking-system,reservation-system
 Author: Niko Ehrenfeuchter
 Author-email: nikolaus.ehrenfeuchter@unibas.ch
 Requires-Python: >=3.9,<4.0
```

