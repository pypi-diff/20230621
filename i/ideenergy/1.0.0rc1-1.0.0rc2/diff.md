# Comparing `tmp/ideenergy-1.0.0rc1.tar.gz` & `tmp/ideenergy-1.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ideenergy-1.0.0rc1.tar", last modified: Fri Oct 21 18:30:43 2022, max compression
+gzip compressed data, was "ideenergy-1.0.0rc2.tar", last modified: Mon Jan  2 16:57:36 2023, max compression
```

## Comparing `ideenergy-1.0.0rc1.tar` & `ideenergy-1.0.0rc2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 18:30:43.791932 ideenergy-1.0.0rc1/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-10-21 18:30:33.000000 ideenergy-1.0.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1240 2022-10-21 18:30:43.791932 ideenergy-1.0.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      711 2022-10-21 18:30:33.000000 ideenergy-1.0.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 18:30:43.791932 ideenergy-1.0.0rc1/ideenergy/
--rw-r--r--   0 runner    (1001) docker     (121)     4330 2022-10-21 18:30:33.000000 ideenergy-1.0.0rc1/ideenergy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      887 2022-10-21 18:30:33.000000 ideenergy-1.0.0rc1/ideenergy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3433 2022-10-21 18:30:33.000000 ideenergy-1.0.0rc1/ideenergy/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    13763 2022-10-21 18:30:33.000000 ideenergy-1.0.0rc1/ideenergy/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     1778 2022-10-21 18:30:33.000000 ideenergy-1.0.0rc1/ideenergy/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (121)     2257 2022-10-21 18:30:33.000000 ideenergy-1.0.0rc1/ideenergy/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 18:30:43.791932 ideenergy-1.0.0rc1/ideenergy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1240 2022-10-21 18:30:43.000000 ideenergy-1.0.0rc1/ideenergy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      362 2022-10-21 18:30:43.000000 ideenergy-1.0.0rc1/ideenergy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-21 18:30:43.000000 ideenergy-1.0.0rc1/ideenergy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-10-21 18:30:43.000000 ideenergy-1.0.0rc1/ideenergy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-10-21 18:30:43.000000 ideenergy-1.0.0rc1/ideenergy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-10-21 18:30:43.000000 ideenergy-1.0.0rc1/ideenergy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-10-21 18:30:33.000000 ideenergy-1.0.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      858 2022-10-21 18:30:43.791932 ideenergy-1.0.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 16:57:36.260704 ideenergy-1.0.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-01-02 16:57:26.000000 ideenergy-1.0.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-01-02 16:57:36.260704 ideenergy-1.0.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-01-02 16:57:26.000000 ideenergy-1.0.0rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 16:57:36.256704 ideenergy-1.0.0rc2/ideenergy/
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-01-02 16:57:26.000000 ideenergy-1.0.0rc2/ideenergy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-01-02 16:57:26.000000 ideenergy-1.0.0rc2/ideenergy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-01-02 16:57:26.000000 ideenergy-1.0.0rc2/ideenergy/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13763 2023-01-02 16:57:26.000000 ideenergy-1.0.0rc2/ideenergy/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-01-02 16:57:26.000000 ideenergy-1.0.0rc2/ideenergy/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-01-02 16:57:26.000000 ideenergy-1.0.0rc2/ideenergy/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 16:57:36.260704 ideenergy-1.0.0rc2/ideenergy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-01-02 16:57:36.000000 ideenergy-1.0.0rc2/ideenergy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-02 16:57:36.000000 ideenergy-1.0.0rc2/ideenergy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-02 16:57:36.000000 ideenergy-1.0.0rc2/ideenergy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-01-02 16:57:36.000000 ideenergy-1.0.0rc2/ideenergy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-01-02 16:57:36.000000 ideenergy-1.0.0rc2/ideenergy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-02 16:57:36.000000 ideenergy-1.0.0rc2/ideenergy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-01-02 16:57:26.000000 ideenergy-1.0.0rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-01-02 16:57:36.260704 ideenergy-1.0.0rc2/setup.cfg
```

### Comparing `ideenergy-1.0.0rc1/LICENSE` & `ideenergy-1.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `ideenergy-1.0.0rc1/PKG-INFO` & `ideenergy-1.0.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ideenergy
-Version: 1.0.0rc1
+Version: 1.0.0rc2
 Summary: Interface to i-de.es energy data
 Home-page: https://github.com/ldotlopez/ideenergy
 Author: Luis López
 Author-email: luis@cuarentaydos.com
 Project-URL: Bug Tracker, https://github.com/ldotlopez/ideenergy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ideenergy-1.0.0rc1/README.md` & `ideenergy-1.0.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `ideenergy-1.0.0rc1/ideenergy/__init__.py` & `ideenergy-1.0.0rc2/ideenergy/__init__.py`

 * *Files identical despite different names*

### Comparing `ideenergy-1.0.0rc1/ideenergy/__main__.py` & `ideenergy-1.0.0rc2/ideenergy/__main__.py`

 * *Files identical despite different names*

### Comparing `ideenergy-1.0.0rc1/ideenergy/cli.py` & `ideenergy-1.0.0rc2/ideenergy/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,20 +88,20 @@
 
     session = await get_session()
     client = Client(
         username=username, password=password, session=session, logger=logger
     )
 
     try:
-        data = await _main()
+        if data := await _main():
+            print(pprint.pformat(data))
 
     except RequestFailedError as e:
         print(f"Request failed: {e}", file=sys.stderr)
         await session.close()
-        return
+        sys.ext(1)
 
-    print(pprint.pformat(data))
     await session.close()
 
 
 if __name__ == "__main__":
     asyncio.run(main())
```

### Comparing `ideenergy-1.0.0rc1/ideenergy/client.py` & `ideenergy-1.0.0rc2/ideenergy/client.py`

 * *Files identical despite different names*

### Comparing `ideenergy-1.0.0rc1/ideenergy/mqtt.py` & `ideenergy-1.0.0rc2/ideenergy/mqtt.py`

 * *Files identical despite different names*

### Comparing `ideenergy-1.0.0rc1/ideenergy/parsers.py` & `ideenergy-1.0.0rc2/ideenergy/parsers.py`

 * *Files identical despite different names*

### Comparing `ideenergy-1.0.0rc1/ideenergy.egg-info/PKG-INFO` & `ideenergy-1.0.0rc2/ideenergy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ideenergy
-Version: 1.0.0rc1
+Version: 1.0.0rc2
 Summary: Interface to i-de.es energy data
 Home-page: https://github.com/ldotlopez/ideenergy
 Author: Luis López
 Author-email: luis@cuarentaydos.com
 Project-URL: Bug Tracker, https://github.com/ldotlopez/ideenergy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ideenergy-1.0.0rc1/setup.cfg` & `ideenergy-1.0.0rc2/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ideenergy
-version = 1.0.0-rc1
+version = 1.0.0-rc2
 author = Luis López
 author_email = luis@cuarentaydos.com
 description = Interface to i-de.es energy data
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ldotlopez/ideenergy
 project_urls = 
@@ -16,19 +16,18 @@
 
 [options]
 package_dir = 
 	ideenergy = ideenergy
 packages = find:
 python_requires = >=3.9
 install_requires = 
-	aiohttp
-	attrs == 21.2.0
+	aiohttp>=3.8.0, <4
 
 [options.extras_require]
-mqtt = paho-mqtt >= 1.6.1
+mqtt = paho-mqtt >= 1.6.1, <2
 
 [options.packages.find]
 where = 
 
 [options.entry_points]
 console_scripts = 
 	ideenergy = ideenergy.cli:main
```

