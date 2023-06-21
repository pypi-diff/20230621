# Comparing `tmp/wiliot-api-4.1.2.tar.gz` & `tmp/wiliot-api-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiliot-api-4.1.2.tar", last modified: Thu May 11 23:02:51 2023, max compression
+gzip compressed data, was "wiliot-api-4.2.0.tar", last modified: Wed Jun 21 08:03:46 2023, max compression
```

## Comparing `wiliot-api-4.1.2.tar` & `wiliot-api-4.2.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-11 23:02:51.754939 wiliot-api-4.1.2/
--rw-rw-rw-   0 root         (0) root         (0)       96 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     5159 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     3397 2023-05-11 23:02:51.754939 wiliot-api-4.1.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2891 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)     7163 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)      328 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-11 23:02:51.754939 wiliot-api-4.1.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1685 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/unittests.dockerfile
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-11 23:02:51.750939 wiliot-api-4.1.2/wiliot_api/
--rw-rw-rw-   0 root         (0) root         (0)     4293 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/wiliot_api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11124 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/wiliot_api/api_client.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-11 23:02:51.754939 wiliot-api-4.1.2/wiliot_api/edge/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/wiliot_api/edge/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13640 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/wiliot_api/edge/edge.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-11 23:02:51.754939 wiliot-api-4.1.2/wiliot_api/edge/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/wiliot_api/edge/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5799 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/wiliot_api/edge/examples/edge_api.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-11 23:02:51.754939 wiliot-api-4.1.2/wiliot_api/manufacturing/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/wiliot_api/manufacturing/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-11 23:02:51.754939 wiliot-api-4.1.2/wiliot_api/manufacturing/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/wiliot_api/manufacturing/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5327 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/wiliot_api/manufacturing/examples/mannufacturing_api.py
--rw-rw-rw-   0 root         (0) root         (0)    14095 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/wiliot_api/manufacturing/manufacturing.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-11 23:02:51.754939 wiliot-api-4.1.2/wiliot_api/platform/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/wiliot_api/platform/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-11 23:02:51.754939 wiliot-api-4.1.2/wiliot_api/platform/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/wiliot_api/platform/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5899 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/wiliot_api/platform/examples/platform_api.py
--rw-rw-rw-   0 root         (0) root         (0)    35660 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/wiliot_api/platform/platform.py
--rw-rw-rw-   0 root         (0) root         (0)     3075 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/wiliot_api/platform/platform_models.py
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/wiliot_api/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-11 23:02:51.754939 wiliot-api-4.1.2/wiliot_api/security/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/wiliot_api/security/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7223 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/wiliot_api/security/security.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-11 23:02:51.754939 wiliot-api-4.1.2/wiliot_api/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/wiliot_api/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2042 2023-05-11 23:02:35.000000 wiliot-api-4.1.2/wiliot_api/utils/get_version.py
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-05-11 23:02:51.000000 wiliot-api-4.1.2/wiliot_api/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-11 23:02:51.754939 wiliot-api-4.1.2/wiliot_api.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     3397 2023-05-11 23:02:51.000000 wiliot-api-4.1.2/wiliot_api.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1030 2023-05-11 23:02:51.000000 wiliot-api-4.1.2/wiliot_api.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-11 23:02:51.000000 wiliot-api-4.1.2/wiliot_api.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-11 23:02:51.000000 wiliot-api-4.1.2/wiliot_api.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-05-11 23:02:51.000000 wiliot-api-4.1.2/wiliot_api.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       11 2023-05-11 23:02:51.000000 wiliot-api-4.1.2/wiliot_api.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 08:03:46.910452 wiliot-api-4.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)       96 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     5159 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     3825 2023-06-21 08:03:46.910452 wiliot-api-4.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3319 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     8440 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)      328 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-21 08:03:46.910452 wiliot-api-4.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1685 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/unittests.dockerfile
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 08:03:46.906452 wiliot-api-4.2.0/wiliot_api/
+-rw-rw-rw-   0 root         (0) root         (0)     4293 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/wiliot_api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11109 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/wiliot_api/api_client.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 08:03:46.910452 wiliot-api-4.2.0/wiliot_api/edge/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/wiliot_api/edge/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15211 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/wiliot_api/edge/edge.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 08:03:46.910452 wiliot-api-4.2.0/wiliot_api/edge/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/wiliot_api/edge/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5799 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/wiliot_api/edge/examples/edge_api.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 08:03:46.910452 wiliot-api-4.2.0/wiliot_api/manufacturing/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/wiliot_api/manufacturing/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 08:03:46.910452 wiliot-api-4.2.0/wiliot_api/manufacturing/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/wiliot_api/manufacturing/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5327 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/wiliot_api/manufacturing/examples/mannufacturing_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    14099 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/wiliot_api/manufacturing/manufacturing.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 08:03:46.910452 wiliot-api-4.2.0/wiliot_api/platform/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/wiliot_api/platform/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 08:03:46.910452 wiliot-api-4.2.0/wiliot_api/platform/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/wiliot_api/platform/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5899 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/wiliot_api/platform/examples/platform_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    35610 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/wiliot_api/platform/platform.py
+-rw-rw-rw-   0 root         (0) root         (0)     3075 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/wiliot_api/platform/platform_models.py
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/wiliot_api/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 08:03:46.910452 wiliot-api-4.2.0/wiliot_api/security/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/wiliot_api/security/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7223 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/wiliot_api/security/security.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 08:03:46.910452 wiliot-api-4.2.0/wiliot_api/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/wiliot_api/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2042 2023-06-21 08:03:30.000000 wiliot-api-4.2.0/wiliot_api/utils/get_version.py
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-06-21 08:03:46.000000 wiliot-api-4.2.0/wiliot_api/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 08:03:46.910452 wiliot-api-4.2.0/wiliot_api.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     3825 2023-06-21 08:03:46.000000 wiliot-api-4.2.0/wiliot_api.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1030 2023-06-21 08:03:46.000000 wiliot-api-4.2.0/wiliot_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-21 08:03:46.000000 wiliot-api-4.2.0/wiliot_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-21 08:03:46.000000 wiliot-api-4.2.0/wiliot_api.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-06-21 08:03:46.000000 wiliot-api-4.2.0/wiliot_api.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       11 2023-06-21 08:03:46.000000 wiliot-api-4.2.0/wiliot_api.egg-info/top_level.txt
```

### Comparing `wiliot-api-4.1.2/LICENSE` & `wiliot-api-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.1.2/PKG-INFO` & `wiliot-api-4.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiliot-api
-Version: 4.1.2
+Version: 4.2.0
 Summary: A library for interacting with Wiliot's private Cloud API
 Home-page: UNKNOWN
 Author: Wiliot
 Author-email: support@wiliot.com
 License: MIT
 Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
 Platform: UNKNOWN
@@ -57,14 +57,22 @@
 * [platform](wiliot_api/platform/examples)
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
+Version 4.2.0:
+-----------------
+* Changed API URLs to support new cloud environment
+* Added support for pulling paginated bridge and gateway lists (when an owner has more than 100 bridges/gateways)
+* Added a function to update multiple bridges' configuration in one call
+* Removed GATEWAY as an association type for location - not supported by the platform
+* Requiring at least one pixel to be provided when creating an asset
+
 Version 4.1.2:
 -----------------
 * Changed additional functions use the metadataFetch API to support larger returned data sets:
     * Get Locations
     * Get zones
     * Get location associations
     * Get zone associations
```

### Comparing `wiliot-api-4.1.2/README.md` & `wiliot-api-4.2.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -40,14 +40,22 @@
 * [platform](wiliot_api/platform/examples)
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
+Version 4.2.0:
+-----------------
+* Changed API URLs to support new cloud environment
+* Added support for pulling paginated bridge and gateway lists (when an owner has more than 100 bridges/gateways)
+* Added a function to update multiple bridges' configuration in one call
+* Removed GATEWAY as an association type for location - not supported by the platform
+* Requiring at least one pixel to be provided when creating an asset
+
 Version 4.1.2:
 -----------------
 * Changed additional functions use the metadataFetch API to support larger returned data sets:
     * Get Locations
     * Get zones
     * Get location associations
     * Get zone associations
```

### Comparing `wiliot-api-4.1.2/bitbucket-pipelines.yml` & `wiliot-api-4.2.0/bitbucket-pipelines.yml`

 * *Files 13% similar despite different names*

```diff
@@ -82,14 +82,37 @@
             - python3 setup.py sdist bdist_wheel
             #update version.py with new minor version and build number (first step is done by setup as well- but we want to add build number as well):
             - echo "__version__ = '$version'" > wiliot_api/version.py
             - echo "build_number = '$BITBUCKET_BUILD_NUMBER'" >> wiliot_api/version.py
             - aws codeartifact login --tool twine --domain wiliot-cloud --domain-owner 142654642153 --repository pypi
             - twine upload --repository codeartifact dist/*
 
+    publish-full-version-into-new-codearfact:
+      - step:
+          name: Build and publish full version py-wilot into codeartifact
+          image:
+            name: 096303741971.dkr.ecr.us-east-2.amazonaws.com/ci:0.0.1-alpine
+            aws:
+              access-key: $CLOUD_AWS_ACCESS_KEY_ID
+              secret-key: $CLOUD_AWS_SECRET_ACCESS_KEY
+          script:
+            - pip3 install setuptools_scm wheel twine
+            - pip3 install gitpython
+            # get updated version number:
+            - version="`python3 wiliot_api/utils/get_version.py`"
+            # update minor version:
+            - python3 setup.py sdist bdist_wheel
+            #update version.py with new minor version and build number (first step is done by setup as well- but we want to add build number as well):
+            - echo "__version__ = '$version'" > wiliot_api/version.py
+            - echo "build_number = '$BITBUCKET_BUILD_NUMBER'" >> wiliot_api/version.py
+            - export AWS_ACCESS_KEY_ID=$CLOUD_AWS_ACCESS_KEY_ID AWS_SECRET_ACCESS_KEY=$CLOUD_AWS_SECRET_ACCESS_KEY
+            - aws codeartifact login --region us-east-2 --tool twine --domain wiliot-cloud --domain-owner 096303741971 --repository pypi
+            - twine upload --repository codeartifact dist/*
+
+
     publish-slim-version-into-pypi:
       - step:
           name: Build and publish slim version py-wilot into pypi
           <<: *wiliot-ci-image
           script:
             - pip3 install setuptools_scm
             - pip3 install gitpython
```

### Comparing `wiliot-api-4.1.2/setup.py` & `wiliot-api-4.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.1.2/wiliot_api/__init__.py` & `wiliot-api-4.2.0/wiliot_api/__init__.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.1.2/wiliot_api/api_client.py` & `wiliot-api-4.2.0/wiliot_api/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,26 +68,26 @@
 
 class WiliotCloudError(Exception):
     pass
 
 
 class Client:
     def __init__(self, oauth_username=None, oauth_password=None, api_key=None,
-                 env='', api_version='v1', log_file=None, logger_=None):
+                 env='prod', api_version='v1', log_file=None, logger_=None):
         # The caller must provide either a set of oauth username abd password or an API key
         if api_key is None and (oauth_password is None or oauth_username is None):
             raise Exception('Provide either an API key or a username and password')
         
-        self.env = env + "/" if env != '' and env != 'prod' else ''
+        self.env = env
         self.api_version = api_version
         self.headers = {
             "accept": "application/json",
             "Content-Type": "application/json"
         }
-        self.auth_obj = security.WiliotAuthentication(base_path=f"https://api.wiliot.com/{self.env}{self.api_version}/",
+        self.auth_obj = security.WiliotAuthentication(base_path=f"https://api.us-east-2.{self.env}.wiliot.cloud/{self.api_version}/",
                                                       oauth_username=oauth_username,
                                                       oauth_password=oauth_password,
                                                       api_key=api_key)
         self.headers["Authorization"] = self.auth_obj.get_token()
         if logger_ is None:
             self.logger = logging.getLogger()
             self.logger.setLevel(log_level)
@@ -101,15 +101,15 @@
                 self.handler = logging.StreamHandler()
             self.handler.setLevel(log_level)
             formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
             self.handler.setFormatter(formatter)
             self.logger.addHandler(self.handler)
 
     def _get_base_url(self, override_client_path=None, override_api_version=None):
-        api_path = f"https://api.wiliot.com/{self.env}{self.api_version if override_api_version is None else override_api_version}/"
+        api_path = f"https://api.us-east-2.{self.env}.wiliot.cloud/{self.api_version if override_api_version is None else override_api_version}/"
         base_url = api_path + self.client_path if override_client_path is None else api_path + override_client_path
         return base_url
 
     def _renew_token(self):
         if self.auth_obj.token_expired():
             self.headers["Authorization"] = self.auth_obj.get_token()
```

### Comparing `wiliot-api-4.1.2/wiliot_api/edge/edge.py` & `wiliot-api-4.2.0/wiliot_api/edge/edge.py`

 * *Files 7% similar despite different names*

```diff
@@ -71,28 +71,35 @@
 
 class BridgeAction(Enum):
     BLINK_LED = 'blinkBridgeLed'
     REBOOT = 'rebootBridge'
 
 
 class EdgeClient(Client):
-    def __init__(self, api_key, owner_id, env='', log_file=None, logger_=None):
+    def __init__(self, api_key, owner_id, env='prod', log_file=None, logger_=None):
         self.client_path = f"owner/{owner_id}/".format(owner_id=owner_id)
         self.owner_id = owner_id
         super().__init__(api_key=api_key, env=env, log_file=log_file, logger_=logger_)
 
     def get_gateways(self):
         """
         Get a list of gateways owned by the owner
         :return: A list of gateways
         """
         path = "gateway"
-        response = self._get(path)
-        res = response.get("data", [])
-        return res
+        params = {}
+        all_gateways = []
+        while True:
+            response = self._get(path, params=params)
+            all_gateways += response["data"]
+            if response.get("meta", {}).get("hasNext"):
+                params['cursor'] = response["meta"]["cursor"]
+            else:
+                break
+        return all_gateways
 
     def get_gateway(self, gateway_id):
         """
         Get a gateway's details including the applications it's associated with
         :param gateway_id:
         :return: A dictionary containing the information returned by the API
         """
@@ -210,20 +217,27 @@
         :return: A list of bridges
         """
         path = "bridge"
         params = {}
         if online is not None:
             params['online'] = online
         try:
-            res = self._get(path, params=params)
-            bridges = res["data"]
-            if gateway_id is not None:
-                bridges = [b for b in bridges if any([c["connected"] and c["gatewayId"] == gateway_id for c
-                                                      in b["connections"]])]
-            return bridges
+            all_bridges = []
+            while True:
+                res = self._get(path, params=params)
+                bridges = res["data"]
+                if gateway_id is not None:
+                    bridges = [b for b in bridges if any([c["connected"] and c["gatewayId"] == gateway_id for c
+                                                          in b["connections"]])]
+                all_bridges += bridges
+                if res.get("meta", {}).get("hasNext"):
+                    params["cursor"] = res["meta"]["cursor"]
+                else:
+                    break
+            return all_bridges
         except WiliotCloudError:
             raise
 
     def get_bridge(self, bridge_id):
         """
         Get information about a specific bridge
         :param bridge_id: String - the ID of the bridge to get information about
@@ -286,14 +300,36 @@
             res = self._put(path, payload)
             return res["message"].lower().find("updated bridge success") != -1
         except WiliotCloudError as e:
             print("Failed to update bridge configuration")
             raise WiliotCloudError(
                 "Failed to update bridge configuration. Received the following error: {}".format(e.args[0]))
 
+    def update_bridges_configuration(self, bridge_ids, config={}):
+        """
+        Update multiple bridges' configuration
+        :param bridge_ids: A list of bridge IDs
+        :param config: A dictionary of configuration keys and values
+        :return: True if the configuration update was received successfully. Note, that this is not an indication
+        that a bridge's configuration was updated. To verify that configuration has been updated read the bridge
+        configuration and compare to the requested values
+        """
+        path = "bridge"
+        payload = {
+            "config": config,
+            "ids": bridge_ids
+        }
+        try:
+            res = self._put(path, payload)
+            return res["message"].lower().find("updated success") != -1
+        except WiliotCloudError as e:
+            print("Failed to update bridges' configuration")
+            raise WiliotCloudError(
+                "Failed to update bridges' configuration. Received the following error: {}".format(e.args[0]))
+
     def send_action_to_bridge(self, bridge_id, action):
         """
         Send an action to a bridge
         :param bridge_id: String - the ID of the bridge to send the action to
         :param action: BridgeAction
         :return: True if the cloud successfully sent the action to the bridge, False otherwise
         """
```

### Comparing `wiliot-api-4.1.2/wiliot_api/edge/examples/edge_api.py` & `wiliot-api-4.2.0/wiliot_api/edge/examples/edge_api.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.1.2/wiliot_api/manufacturing/examples/mannufacturing_api.py` & `wiliot-api-4.2.0/wiliot_api/manufacturing/examples/mannufacturing_api.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.1.2/wiliot_api/manufacturing/manufacturing.py` & `wiliot-api-4.2.0/wiliot_api/manufacturing/manufacturing.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 from wiliot_api.api_client import Client, WiliotCloudError
 import datetime
 from uuid import uuid4
 import jwt
 
 
 class ManufacturingClient(Client):
-    def __init__(self, oauth_username=None, oauth_password=None, api_key=None, env='', log_file=None, logger_=None):
+    def __init__(self, oauth_username=None, oauth_password=None, api_key=None, env='prod', log_file=None, logger_=None):
         self.client_path = "manufacturing/"
         super().__init__(oauth_username=oauth_username,
                          oauth_password=oauth_password, api_key=api_key, env=env, log_file=log_file, logger_=logger_)
     
     # Pixel Ownership Change functions
     
     def change_pixel_owner_by_range(self, from_owner_id, to_owner_id, from_pixel_id, to_pixel_id):
```

### Comparing `wiliot-api-4.1.2/wiliot_api/platform/examples/platform_api.py` & `wiliot-api-4.2.0/wiliot_api/platform/examples/platform_api.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.1.2/wiliot_api/platform/platform.py` & `wiliot-api-4.2.0/wiliot_api/platform/platform.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,19 +101,18 @@
 class ZoneAssociationType(Enum):
     BRIDGE = 'bridge'
     TAG = 'tag'
 
 
 class LocationAssociationType(Enum):
     BRIDGE = 'bridge'
-    GATEWAY = 'gateway'
 
 
 class PlatformClient(Client):
-    def __init__(self, api_key, owner_id, env='', log_file=None, logger_=None):
+    def __init__(self, api_key, owner_id, env='prod', log_file=None, logger_=None):
         self.client_path = "traceability/owner/{owner_id}/".format(owner_id=owner_id)
         self.owner_id = owner_id
         super().__init__(api_key=api_key, env=env, log_file=log_file, logger_=logger_)
 
     # Tag calls
 
     def get_pixels(self, limit=None, next=None):
@@ -218,25 +217,25 @@
 
         try:
             return res["data"]["assets"]["page"][0]
         except IndexError:
             raise AssetNotFound
 
     def create_asset(self,
-                     name, category_id, asset_id=None,
-                     pixels=[], status=None):
+                     name, category_id, pixels, asset_id=None,
+                     status=None):
         """
         Create an asset, and optionally assign pixels
         :param name: String - required - A name for the asset (required)
         :param category_id: String - required - the type of asset
-        :param asset_id: String - optional. If not provided an asset ID will be generated automatically
-        :param pixels: List - optional - of dictionaries for asset pixels. Each item should be a dictionary with the
+        :param pixels: List - required - of dictionaries for asset pixels. Each item should be a dictionary with the
         following keys:
          > tagId: string
          > role: Enum: TagRole
+        :param asset_id: String - optional. If not provided an asset ID will be generated automatically
         :param status: String - optional - A status
         :return: The created asset if successful
         """
         assert isinstance(pixels, list), "Expecting a list of strings for pixels_ids"
         path = "/asset"
         payload = {
             "id": asset_id,
@@ -310,15 +309,15 @@
         Disassociate a pixel from an asset
         :param asset_id: String - required - the ID of the asset to disassociate the pixel from
         :param pixel_id: String - required - the ID of the pixel to disassociate from the asset
         :return: True if disassociation was successful.
         """
         path = f"asset/{asset_id}/tag/{pixel_id}"
         try:
-            res = self._delete(path, payload={}, override_api_version="v2")
+            res = self._delete(path, payload={})
             return res['message'].lower().find("success") != -1
         except WiliotCloudError as e:
             print("Failed to associate pixel to asset")
             raise e
 
     # Asset Label calls
```

### Comparing `wiliot-api-4.1.2/wiliot_api/platform/platform_models.py` & `wiliot-api-4.2.0/wiliot_api/platform/platform_models.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.1.2/wiliot_api/security/security.py` & `wiliot-api-4.2.0/wiliot_api/security/security.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.1.2/wiliot_api/utils/get_version.py` & `wiliot-api-4.2.0/wiliot_api/utils/get_version.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.1.2/wiliot_api.egg-info/PKG-INFO` & `wiliot-api-4.2.0/wiliot_api.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiliot-api
-Version: 4.1.2
+Version: 4.2.0
 Summary: A library for interacting with Wiliot's private Cloud API
 Home-page: UNKNOWN
 Author: Wiliot
 Author-email: support@wiliot.com
 License: MIT
 Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
 Platform: UNKNOWN
@@ -57,14 +57,22 @@
 * [platform](wiliot_api/platform/examples)
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
+Version 4.2.0:
+-----------------
+* Changed API URLs to support new cloud environment
+* Added support for pulling paginated bridge and gateway lists (when an owner has more than 100 bridges/gateways)
+* Added a function to update multiple bridges' configuration in one call
+* Removed GATEWAY as an association type for location - not supported by the platform
+* Requiring at least one pixel to be provided when creating an asset
+
 Version 4.1.2:
 -----------------
 * Changed additional functions use the metadataFetch API to support larger returned data sets:
     * Get Locations
     * Get zones
     * Get location associations
     * Get zone associations
```

### Comparing `wiliot-api-4.1.2/wiliot_api.egg-info/SOURCES.txt` & `wiliot-api-4.2.0/wiliot_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

