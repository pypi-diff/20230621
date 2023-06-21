# Comparing `tmp/ibmcloudant-0.4.2.tar.gz` & `tmp/ibmcloudant-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibmcloudant-0.4.2.tar", last modified: Wed May 24 10:03:03 2023, max compression
+gzip compressed data, was "ibmcloudant-0.4.3.tar", last modified: Wed Jun 21 09:05:03 2023, max compression
```

## Comparing `ibmcloudant-0.4.2.tar` & `ibmcloudant-0.4.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-24 10:03:03.466310 ibmcloudant-0.4.2/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11357 2023-05-24 09:52:04.000000 ibmcloudant-0.4.2/LICENSE
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       70 2023-05-24 09:52:04.000000 ibmcloudant-0.4.2/MANIFEST.in
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    27205 2023-05-24 10:03:03.466310 ibmcloudant-0.4.2/PKG-INFO
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    26203 2023-05-24 09:54:50.000000 ibmcloudant-0.4.2/README.md
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-24 10:03:03.466310 ibmcloudant-0.4.2/ibmcloudant/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1596 2023-05-24 09:52:04.000000 ibmcloudant-0.4.2/ibmcloudant/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     6630 2023-05-24 09:52:04.000000 ibmcloudant-0.4.2/ibmcloudant/cloudant_base_service.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)   746253 2023-05-24 09:52:04.000000 ibmcloudant-0.4.2/ibmcloudant/cloudant_v1.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1811 2023-05-24 09:52:04.000000 ibmcloudant-0.4.2/ibmcloudant/common.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3396 2023-05-24 09:52:04.000000 ibmcloudant-0.4.2/ibmcloudant/couchdb_session_authenticator.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1543 2023-05-24 09:52:04.000000 ibmcloudant-0.4.2/ibmcloudant/couchdb_session_get_authenticator_patch.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3609 2023-05-24 09:52:04.000000 ibmcloudant-0.4.2/ibmcloudant/couchdb_session_token_manager.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      655 2023-05-24 09:54:50.000000 ibmcloudant-0.4.2/ibmcloudant/version.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-24 10:03:03.466310 ibmcloudant-0.4.2/ibmcloudant.egg-info/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    27205 2023-05-24 10:03:03.000000 ibmcloudant-0.4.2/ibmcloudant.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      558 2023-05-24 10:03:03.000000 ibmcloudant-0.4.2/ibmcloudant.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-05-24 10:03:03.000000 ibmcloudant-0.4.2/ibmcloudant.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       97 2023-05-24 10:03:03.000000 ibmcloudant-0.4.2/ibmcloudant.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       12 2023-05-24 10:03:03.000000 ibmcloudant-0.4.2/ibmcloudant.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-05-24 09:52:24.000000 ibmcloudant-0.4.2/ibmcloudant.egg-info/zip-safe
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      231 2023-05-24 09:52:04.000000 ibmcloudant-0.4.2/requirements-dev.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      135 2023-05-24 09:52:04.000000 ibmcloudant-0.4.2/requirements.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       38 2023-05-24 10:03:03.466310 ibmcloudant-0.4.2/setup.cfg
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3435 2023-05-24 09:54:50.000000 ibmcloudant-0.4.2/setup.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 09:05:03.647334 ibmcloudant-0.4.3/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11357 2023-06-21 08:48:37.000000 ibmcloudant-0.4.3/LICENSE
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       70 2023-06-21 08:48:37.000000 ibmcloudant-0.4.3/MANIFEST.in
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    27205 2023-06-21 09:05:03.647334 ibmcloudant-0.4.3/PKG-INFO
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    26203 2023-06-21 08:51:22.000000 ibmcloudant-0.4.3/README.md
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 09:05:03.643335 ibmcloudant-0.4.3/ibmcloudant/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1596 2023-06-21 08:48:37.000000 ibmcloudant-0.4.3/ibmcloudant/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     6630 2023-06-21 08:48:37.000000 ibmcloudant-0.4.3/ibmcloudant/cloudant_base_service.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)   746253 2023-06-21 08:48:37.000000 ibmcloudant-0.4.3/ibmcloudant/cloudant_v1.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1811 2023-06-21 08:48:37.000000 ibmcloudant-0.4.3/ibmcloudant/common.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3396 2023-06-21 08:48:37.000000 ibmcloudant-0.4.3/ibmcloudant/couchdb_session_authenticator.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1543 2023-06-21 08:48:37.000000 ibmcloudant-0.4.3/ibmcloudant/couchdb_session_get_authenticator_patch.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3609 2023-06-21 08:48:37.000000 ibmcloudant-0.4.3/ibmcloudant/couchdb_session_token_manager.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      655 2023-06-21 08:51:22.000000 ibmcloudant-0.4.3/ibmcloudant/version.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 09:05:03.647334 ibmcloudant-0.4.3/ibmcloudant.egg-info/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    27205 2023-06-21 09:05:03.000000 ibmcloudant-0.4.3/ibmcloudant.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      558 2023-06-21 09:05:03.000000 ibmcloudant-0.4.3/ibmcloudant.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-06-21 09:05:03.000000 ibmcloudant-0.4.3/ibmcloudant.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       97 2023-06-21 09:05:03.000000 ibmcloudant-0.4.3/ibmcloudant.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       12 2023-06-21 09:05:03.000000 ibmcloudant-0.4.3/ibmcloudant.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-06-21 08:48:57.000000 ibmcloudant-0.4.3/ibmcloudant.egg-info/zip-safe
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      180 2023-06-21 08:48:37.000000 ibmcloudant-0.4.3/requirements-dev.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      135 2023-06-21 08:48:37.000000 ibmcloudant-0.4.3/requirements.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       38 2023-06-21 09:05:03.647334 ibmcloudant-0.4.3/setup.cfg
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3435 2023-06-21 08:51:22.000000 ibmcloudant-0.4.3/setup.py
```

### Comparing `ibmcloudant-0.4.2/LICENSE` & `ibmcloudant-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ibmcloudant-0.4.2/PKG-INFO` & `ibmcloudant-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibmcloudant
-Version: 0.4.2
+Version: 0.4.3
 Summary: Python client library for IBM Cloudant
 Home-page: https://github.com/IBM/cloudant-python-sdk
 Author: IBM
 Author-email: cldtsdks@us.ibm.com
 License: Apache 2.0
 Keywords: ibmcloudant
 Classifier: Programming Language :: Python
@@ -23,15 +23,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Build Status](https://github.com/IBM/cloudant-python-sdk/actions/workflows/test.yml/badge.svg?branch=main&event=push)](https://github.com/IBM/cloudant-python-sdk/actions/workflows/test.yml)
 [![Release](https://img.shields.io/github/v/release/IBM/cloudant-python-sdk?include_prereleases&sort=semver)](https://github.com/IBM/cloudant-python-sdk/releases/latest)
 [![Docs](https://img.shields.io/static/v1?label=Pydoc&message=latest&color=blue)](https://ibm.github.io/cloudant-python-sdk/)
 
-# IBM Cloudant Python SDK Version 0.4.2
+# IBM Cloudant Python SDK Version 0.4.3
 
 IBM Cloudant Python SDK is a client library that interacts with the
 [IBM Cloudant APIs](https://cloud.ibm.com/apidocs/cloudant?code=python).
 
 Disclaimer: This library is still a 0.x release. We do consider this
 library production-ready and capable, but there are still some
 limitations we’re working to resolve, and refinements we want to
@@ -123,21 +123,21 @@
 - Python 3.7 or above.
 
 ## Installation
 
 To install, use `pip` or `easy_install`:
 
 ```bash
-pip install --upgrade "ibmcloudant>=0.4.2"
+pip install --upgrade "ibmcloudant>=0.4.3"
 ```
 
 or
 
 ```bash
-easy_install --upgrade "ibmcloudant>=0.4.2"
+easy_install --upgrade "ibmcloudant>=0.4.3"
 ```
 
 ## Authentication
 
 [service-credentials]: https://cloud.ibm.com/docs/Cloudant?topic=Cloudant-locating-your-service-credentials
 [cloud-IAM-mgmt]: https://cloud.ibm.com/docs/Cloudant?topic=Cloudant-managing-access-for-cloudant#introduction-iam-ai
 [couch-cookie-auth]: https://docs.couchdb.org/en/stable/api/server/authn.html#cookie-authentication
```

### Comparing `ibmcloudant-0.4.2/README.md` & `ibmcloudant-0.4.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [![Build Status](https://github.com/IBM/cloudant-python-sdk/actions/workflows/test.yml/badge.svg?branch=main&event=push)](https://github.com/IBM/cloudant-python-sdk/actions/workflows/test.yml)
 [![Release](https://img.shields.io/github/v/release/IBM/cloudant-python-sdk?include_prereleases&sort=semver)](https://github.com/IBM/cloudant-python-sdk/releases/latest)
 [![Docs](https://img.shields.io/static/v1?label=Pydoc&message=latest&color=blue)](https://ibm.github.io/cloudant-python-sdk/)
 
-# IBM Cloudant Python SDK Version 0.4.2
+# IBM Cloudant Python SDK Version 0.4.3
 
 IBM Cloudant Python SDK is a client library that interacts with the
 [IBM Cloudant APIs](https://cloud.ibm.com/apidocs/cloudant?code=python).
 
 Disclaimer: This library is still a 0.x release. We do consider this
 library production-ready and capable, but there are still some
 limitations we’re working to resolve, and refinements we want to
@@ -98,21 +98,21 @@
 - Python 3.7 or above.
 
 ## Installation
 
 To install, use `pip` or `easy_install`:
 
 ```bash
-pip install --upgrade "ibmcloudant>=0.4.2"
+pip install --upgrade "ibmcloudant>=0.4.3"
 ```
 
 or
 
 ```bash
-easy_install --upgrade "ibmcloudant>=0.4.2"
+easy_install --upgrade "ibmcloudant>=0.4.3"
 ```
 
 ## Authentication
 
 [service-credentials]: https://cloud.ibm.com/docs/Cloudant?topic=Cloudant-locating-your-service-credentials
 [cloud-IAM-mgmt]: https://cloud.ibm.com/docs/Cloudant?topic=Cloudant-managing-access-for-cloudant#introduction-iam-ai
 [couch-cookie-auth]: https://docs.couchdb.org/en/stable/api/server/authn.html#cookie-authentication
```

### Comparing `ibmcloudant-0.4.2/ibmcloudant/__init__.py` & `ibmcloudant-0.4.3/ibmcloudant/__init__.py`

 * *Files identical despite different names*

### Comparing `ibmcloudant-0.4.2/ibmcloudant/cloudant_base_service.py` & `ibmcloudant-0.4.3/ibmcloudant/cloudant_base_service.py`

 * *Files identical despite different names*

### Comparing `ibmcloudant-0.4.2/ibmcloudant/cloudant_v1.py` & `ibmcloudant-0.4.3/ibmcloudant/cloudant_v1.py`

 * *Files identical despite different names*

### Comparing `ibmcloudant-0.4.2/ibmcloudant/common.py` & `ibmcloudant-0.4.3/ibmcloudant/common.py`

 * *Files identical despite different names*

### Comparing `ibmcloudant-0.4.2/ibmcloudant/couchdb_session_authenticator.py` & `ibmcloudant-0.4.3/ibmcloudant/couchdb_session_authenticator.py`

 * *Files identical despite different names*

### Comparing `ibmcloudant-0.4.2/ibmcloudant/couchdb_session_get_authenticator_patch.py` & `ibmcloudant-0.4.3/ibmcloudant/couchdb_session_get_authenticator_patch.py`

 * *Files identical despite different names*

### Comparing `ibmcloudant-0.4.2/ibmcloudant/couchdb_session_token_manager.py` & `ibmcloudant-0.4.3/ibmcloudant/couchdb_session_token_manager.py`

 * *Files identical despite different names*

### Comparing `ibmcloudant-0.4.2/ibmcloudant/version.py` & `ibmcloudant-0.4.3/ibmcloudant/version.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Version of ibmcloudant
 """
-__version__ = '0.4.2'
+__version__ = '0.4.3'
```

### Comparing `ibmcloudant-0.4.2/ibmcloudant.egg-info/PKG-INFO` & `ibmcloudant-0.4.3/ibmcloudant.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibmcloudant
-Version: 0.4.2
+Version: 0.4.3
 Summary: Python client library for IBM Cloudant
 Home-page: https://github.com/IBM/cloudant-python-sdk
 Author: IBM
 Author-email: cldtsdks@us.ibm.com
 License: Apache 2.0
 Keywords: ibmcloudant
 Classifier: Programming Language :: Python
@@ -23,15 +23,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Build Status](https://github.com/IBM/cloudant-python-sdk/actions/workflows/test.yml/badge.svg?branch=main&event=push)](https://github.com/IBM/cloudant-python-sdk/actions/workflows/test.yml)
 [![Release](https://img.shields.io/github/v/release/IBM/cloudant-python-sdk?include_prereleases&sort=semver)](https://github.com/IBM/cloudant-python-sdk/releases/latest)
 [![Docs](https://img.shields.io/static/v1?label=Pydoc&message=latest&color=blue)](https://ibm.github.io/cloudant-python-sdk/)
 
-# IBM Cloudant Python SDK Version 0.4.2
+# IBM Cloudant Python SDK Version 0.4.3
 
 IBM Cloudant Python SDK is a client library that interacts with the
 [IBM Cloudant APIs](https://cloud.ibm.com/apidocs/cloudant?code=python).
 
 Disclaimer: This library is still a 0.x release. We do consider this
 library production-ready and capable, but there are still some
 limitations we’re working to resolve, and refinements we want to
@@ -123,21 +123,21 @@
 - Python 3.7 or above.
 
 ## Installation
 
 To install, use `pip` or `easy_install`:
 
 ```bash
-pip install --upgrade "ibmcloudant>=0.4.2"
+pip install --upgrade "ibmcloudant>=0.4.3"
 ```
 
 or
 
 ```bash
-easy_install --upgrade "ibmcloudant>=0.4.2"
+easy_install --upgrade "ibmcloudant>=0.4.3"
 ```
 
 ## Authentication
 
 [service-credentials]: https://cloud.ibm.com/docs/Cloudant?topic=Cloudant-locating-your-service-credentials
 [cloud-IAM-mgmt]: https://cloud.ibm.com/docs/Cloudant?topic=Cloudant-managing-access-for-cloudant#introduction-iam-ai
 [couch-cookie-auth]: https://docs.couchdb.org/en/stable/api/server/authn.html#cookie-authentication
```

### Comparing `ibmcloudant-0.4.2/ibmcloudant.egg-info/SOURCES.txt` & `ibmcloudant-0.4.3/ibmcloudant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ibmcloudant-0.4.2/setup.py` & `ibmcloudant-0.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 from setuptools import setup
 from setuptools.command.test import test as TestCommand
 import os
 import sys
 import pkg_resources
 
-__version__ = '0.4.2'
+__version__ = '0.4.3'
 PACKAGE_NAME = 'ibmcloudant'
 PACKAGE_DESC = 'Python client library for IBM Cloudant'
 
 with open('requirements.txt') as f:
     install_requires = [str(req) for req in pkg_resources.parse_requirements(f)]
 with open('requirements-dev.txt') as f:
     tests_require = [str(req) for req in pkg_resources.parse_requirements(f)]
```

