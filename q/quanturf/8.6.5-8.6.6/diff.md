# Comparing `tmp/quanturf-8.6.5.tar.gz` & `tmp/quanturf-8.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quanturf-8.6.5.tar", last modified: Mon Jun 12 14:18:53 2023, max compression
+gzip compressed data, was "quanturf-8.6.6.tar", last modified: Wed Jun 21 06:58:06 2023, max compression
```

## Comparing `quanturf-8.6.5.tar` & `quanturf-8.6.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 aayush    (1000) aayush    (1000)        0 2023-06-12 14:18:53.780182 quanturf-8.6.5/
--rw-r--r--   0 aayush    (1000) aayush    (1000)    35149 2023-05-29 13:06:01.000000 quanturf-8.6.5/LICENCE.txt
--rw-r--r--   0 aayush    (1000) aayush    (1000)      780 2023-06-12 14:18:53.780182 quanturf-8.6.5/PKG-INFO
--rw-r--r--   0 aayush    (1000) aayush    (1000)     6705 2023-05-29 13:06:01.000000 quanturf-8.6.5/README.md
-drwxr-xr-x   0 aayush    (1000) aayush    (1000)        0 2023-06-12 14:18:53.780182 quanturf-8.6.5/quanturf/
--rw-r--r--   0 aayush    (1000) aayush    (1000)        0 2023-05-29 13:06:01.000000 quanturf-8.6.5/quanturf/__init__.py
--rw-r--r--   0 aayush    (1000) aayush    (1000)     2055 2023-06-12 14:15:03.000000 quanturf-8.6.5/quanturf/__main__.py
--rw-r--r--   0 aayush    (1000) aayush    (1000)      157 2023-06-12 14:15:03.000000 quanturf-8.6.5/quanturf/config.yaml
--rw-r--r--   0 aayush    (1000) aayush    (1000)    29725 2023-06-12 14:15:03.000000 quanturf-8.6.5/quanturf/jupyter_notebook_config.py
--rw-r--r--   0 aayush    (1000) aayush    (1000)     3674 2023-06-12 14:15:03.000000 quanturf-8.6.5/quanturf/quanturf.ipynb
-drwxr-xr-x   0 aayush    (1000) aayush    (1000)        0 2023-06-12 14:18:53.780182 quanturf-8.6.5/quanturf.egg-info/
--rw-r--r--   0 aayush    (1000) aayush    (1000)      780 2023-06-12 14:18:53.000000 quanturf-8.6.5/quanturf.egg-info/PKG-INFO
--rw-r--r--   0 aayush    (1000) aayush    (1000)      358 2023-06-12 14:18:53.000000 quanturf-8.6.5/quanturf.egg-info/SOURCES.txt
--rw-r--r--   0 aayush    (1000) aayush    (1000)        1 2023-06-12 14:18:53.000000 quanturf-8.6.5/quanturf.egg-info/dependency_links.txt
--rw-r--r--   0 aayush    (1000) aayush    (1000)       52 2023-06-12 14:18:53.000000 quanturf-8.6.5/quanturf.egg-info/entry_points.txt
--rw-r--r--   0 aayush    (1000) aayush    (1000)       75 2023-06-12 14:18:53.000000 quanturf-8.6.5/quanturf.egg-info/requires.txt
--rw-r--r--   0 aayush    (1000) aayush    (1000)        9 2023-06-12 14:18:53.000000 quanturf-8.6.5/quanturf.egg-info/top_level.txt
--rw-r--r--   0 aayush    (1000) aayush    (1000)       38 2023-06-12 14:18:53.780182 quanturf-8.6.5/setup.cfg
--rw-r--r--   0 aayush    (1000) aayush    (1000)     2518 2023-06-12 14:17:25.000000 quanturf-8.6.5/setup.py
--rw-r--r--   0 aayush    (1000) aayush    (1000)      329 2023-05-29 13:19:34.000000 quanturf-8.6.5/version.py
+drwxr-xr-x   0 aayush    (1000) aayush    (1000)        0 2023-06-21 06:58:06.821087 quanturf-8.6.6/
+-rw-r--r--   0 aayush    (1000) aayush    (1000)    35149 2023-05-29 13:06:01.000000 quanturf-8.6.6/LICENCE.txt
+-rw-r--r--   0 aayush    (1000) aayush    (1000)      780 2023-06-21 06:58:06.821087 quanturf-8.6.6/PKG-INFO
+-rw-r--r--   0 aayush    (1000) aayush    (1000)     6705 2023-05-29 13:06:01.000000 quanturf-8.6.6/README.md
+drwxr-xr-x   0 aayush    (1000) aayush    (1000)        0 2023-06-21 06:58:06.820087 quanturf-8.6.6/quanturf/
+-rw-r--r--   0 aayush    (1000) aayush    (1000)        0 2023-05-29 13:06:01.000000 quanturf-8.6.6/quanturf/__init__.py
+-rw-r--r--   0 aayush    (1000) aayush    (1000)     2081 2023-06-21 06:55:35.000000 quanturf-8.6.6/quanturf/__main__.py
+-rw-r--r--   0 aayush    (1000) aayush    (1000)      157 2023-06-12 14:15:03.000000 quanturf-8.6.6/quanturf/config.yaml
+-rw-r--r--   0 aayush    (1000) aayush    (1000)    29725 2023-06-12 14:15:03.000000 quanturf-8.6.6/quanturf/jupyter_notebook_config.py
+-rw-r--r--   0 aayush    (1000) aayush    (1000)     3674 2023-06-12 14:15:03.000000 quanturf-8.6.6/quanturf/quanturf.ipynb
+drwxr-xr-x   0 aayush    (1000) aayush    (1000)        0 2023-06-21 06:58:06.821087 quanturf-8.6.6/quanturf.egg-info/
+-rw-r--r--   0 aayush    (1000) aayush    (1000)      780 2023-06-21 06:58:06.000000 quanturf-8.6.6/quanturf.egg-info/PKG-INFO
+-rw-r--r--   0 aayush    (1000) aayush    (1000)      358 2023-06-21 06:58:06.000000 quanturf-8.6.6/quanturf.egg-info/SOURCES.txt
+-rw-r--r--   0 aayush    (1000) aayush    (1000)        1 2023-06-21 06:58:06.000000 quanturf-8.6.6/quanturf.egg-info/dependency_links.txt
+-rw-r--r--   0 aayush    (1000) aayush    (1000)       52 2023-06-21 06:58:06.000000 quanturf-8.6.6/quanturf.egg-info/entry_points.txt
+-rw-r--r--   0 aayush    (1000) aayush    (1000)       75 2023-06-21 06:58:06.000000 quanturf-8.6.6/quanturf.egg-info/requires.txt
+-rw-r--r--   0 aayush    (1000) aayush    (1000)        9 2023-06-21 06:58:06.000000 quanturf-8.6.6/quanturf.egg-info/top_level.txt
+-rw-r--r--   0 aayush    (1000) aayush    (1000)       38 2023-06-21 06:58:06.821087 quanturf-8.6.6/setup.cfg
+-rw-r--r--   0 aayush    (1000) aayush    (1000)     2238 2023-06-21 06:55:35.000000 quanturf-8.6.6/setup.py
+-rw-r--r--   0 aayush    (1000) aayush    (1000)      329 2023-05-29 13:19:34.000000 quanturf-8.6.6/version.py
```

### Comparing `quanturf-8.6.5/LICENCE.txt` & `quanturf-8.6.6/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `quanturf-8.6.5/PKG-INFO` & `quanturf-8.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quanturf
-Version: 8.6.5
+Version: 8.6.6
 Summary: REMOTE_USER Authenticator: An Authenticator for Jupyterhub to read user information from HTTP request headers, as when running behind an authenticating proxy.
 Home-page: https://github.com/Quanturf/quanturf_pypi_package.git
 Author: Quanturf
 Author-email: quanturf.finance@gmail.com
 License: GPLv3
 Keywords: Interactive,Interpreter,Shell,Web
 Platform: Linux
```

### Comparing `quanturf-8.6.5/README.md` & `quanturf-8.6.6/README.md`

 * *Files identical despite different names*

### Comparing `quanturf-8.6.5/quanturf/__main__.py` & `quanturf-8.6.6/quanturf/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,21 +45,21 @@
         str_out = ' '.join(str_out)
         env_dir = os.path.normpath(os.path.join(str_out, "quanturf"))
         os.environ['JUPYTER_APP_LAUNCHER_PATH'] = env_dir
 
         filename = os.path.join(str_out, "quanturf","jupyter_notebook_config.py")
         filename2 = filename.replace(os.sep, '/')
         print("filename2: ", filename2)
-        os.system("jupyter lab --config=" + filename2)
+        os.system("jupyter lab --ip=0.0.0.0 --config=" + filename2)
 
     if len(out) >= 2:
         str_out = out[1]
         env_dir = os.path.normpath(os.path.join(str_out, "quanturf"))
         os.environ['JUPYTER_APP_LAUNCHER_PATH'] = env_dir
 
         filename = os.path.join(str_out, "quanturf","jupyter_notebook_config.py")
         filename2 = filename.replace(os.sep, '/')
-        os.system("jupyter lab --config=" + filename2)
+        os.system("jupyter lab --ip=0.0.0.0 --config=" + filename2)
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `quanturf-8.6.5/quanturf/jupyter_notebook_config.py` & `quanturf-8.6.6/quanturf/jupyter_notebook_config.py`

 * *Files identical despite different names*

### Comparing `quanturf-8.6.5/quanturf/quanturf.ipynb` & `quanturf-8.6.6/quanturf/quanturf.ipynb`

 * *Files identical despite different names*

### Comparing `quanturf-8.6.5/quanturf.egg-info/PKG-INFO` & `quanturf-8.6.6/quanturf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quanturf
-Version: 8.6.5
+Version: 8.6.6
 Summary: REMOTE_USER Authenticator: An Authenticator for Jupyterhub to read user information from HTTP request headers, as when running behind an authenticating proxy.
 Home-page: https://github.com/Quanturf/quanturf_pypi_package.git
 Author: Quanturf
 Author-email: quanturf.finance@gmail.com
 License: GPLv3
 Keywords: Interactive,Interpreter,Shell,Web
 Platform: Linux
```

### Comparing `quanturf-8.6.5/setup.py` & `quanturf-8.6.6/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 version_ns = {}
 with open(pjoin(here, 'version.py')) as f:
     exec(f.read(), {}, version_ns)
 
 setup_args = dict(
     name='quanturf',
     packages=['quanturf'],
-    version="8.6.5",
+    version="8.6.6",
     description="""REMOTE_USER Authenticator: An Authenticator for Jupyterhub to read user information from HTTP request headers, as when running behind an authenticating proxy.""",
     long_description="",
     author="Quanturf",
     author_email="quanturf.finance@gmail.com",
     url="https://github.com/Quanturf/quanturf_pypi_package.git",
     license="GPLv3",
     platforms="Linux, Mac OS X",
@@ -42,22 +42,14 @@
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
     ],
     package_data={'': [
         'quanturf.ipynb',
-        'download_data.ipynb',
-        'golden_cross.ipynb',
-        'MACD.ipynb',
-        'mlp_model.ipynb',
-        'RSI.ipynb',
-        'BarraFactorModel_FactorBased.ipynb',
-        'RelativeStrengthIndex(RSI)_Indicator.ipynb',
-        'StochasticOscillator_Indicators.ipynb',
         'config.yaml'
     ]},
     include_package_data=True,
     data_files=[('.', ['version.py'])],
     # scripts=['bin/run_quanturf'],
     entry_points={
         "console_scripts": [
```

