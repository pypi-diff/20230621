# Comparing `tmp/pgb_broker_utils-0.2.8.tar.gz` & `tmp/pgb_broker_utils-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/troyraen/Documents/broker/repo2/broker/broker_utils/dist/tmpc50kfxwt/pgb_broker_utils-0.2.8.tar", last modified: Tue Aug  3 22:31:53 2021, max compression
+gzip compressed data, was "/Users/troyraen/Documents/broker/repo2/broker/broker_utils/dist/tmpjj9e9bgu/pgb_broker_utils-0.2.9.tar", last modified: Sat Aug  7 16:42:35 2021, max compression
```

## Comparing `pgb_broker_utils-0.2.8.tar` & `pgb_broker_utils-0.2.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 troyraen   (501) staff       (20)        0 2021-08-03 22:31:53.000000 pgb_broker_utils-0.2.8/
--rw-r--r--   0 troyraen   (501) staff       (20)    34515 2021-07-14 03:28:29.000000 pgb_broker_utils-0.2.8/LICENSE.txt
--rw-r--r--   0 troyraen   (501) staff       (20)       25 2021-08-03 22:31:41.000000 pgb_broker_utils-0.2.8/MANIFEST.in
--rw-r--r--   0 troyraen   (501) staff       (20)     1173 2021-08-03 22:31:53.000000 pgb_broker_utils-0.2.8/PKG-INFO
--rw-r--r--   0 troyraen   (501) staff       (20)      404 2021-07-14 03:28:29.000000 pgb_broker_utils-0.2.8/README.md
-drwxr-xr-x   0 troyraen   (501) staff       (20)        0 2021-08-03 22:31:53.000000 pgb_broker_utils-0.2.8/broker_utils/
--rw-r--r--   0 troyraen   (501) staff       (20)      186 2021-07-14 03:28:29.000000 pgb_broker_utils-0.2.8/broker_utils/__init__.py
--rw-r--r--   0 troyraen   (501) staff       (20)     4417 2021-08-02 20:58:38.000000 pgb_broker_utils-0.2.8/broker_utils/beam_transforms.py
--rw-r--r--   0 troyraen   (501) staff       (20)    11779 2021-08-03 22:26:36.000000 pgb_broker_utils-0.2.8/broker_utils/consumer_sim.py
--rw-r--r--   0 troyraen   (501) staff       (20)     1982 2021-07-14 03:28:29.000000 pgb_broker_utils-0.2.8/broker_utils/data_utils.py
--rw-r--r--   0 troyraen   (501) staff       (20)     2837 2021-07-14 03:28:29.000000 pgb_broker_utils-0.2.8/broker_utils/gcp_utils.py
--rw-r--r--   0 troyraen   (501) staff       (20)     1750 2021-07-14 03:28:29.000000 pgb_broker_utils-0.2.8/broker_utils/schema_maps.py
-drwxr-xr-x   0 troyraen   (501) staff       (20)        0 2021-08-03 22:31:53.000000 pgb_broker_utils-0.2.8/pgb_broker_utils.egg-info/
--rw-r--r--   0 troyraen   (501) staff       (20)     1173 2021-08-03 22:31:53.000000 pgb_broker_utils-0.2.8/pgb_broker_utils.egg-info/PKG-INFO
--rw-r--r--   0 troyraen   (501) staff       (20)      425 2021-08-03 22:31:53.000000 pgb_broker_utils-0.2.8/pgb_broker_utils.egg-info/SOURCES.txt
--rw-r--r--   0 troyraen   (501) staff       (20)        1 2021-08-03 22:31:53.000000 pgb_broker_utils-0.2.8/pgb_broker_utils.egg-info/dependency_links.txt
--rw-r--r--   0 troyraen   (501) staff       (20)      155 2021-08-03 22:31:53.000000 pgb_broker_utils-0.2.8/pgb_broker_utils.egg-info/requires.txt
--rw-r--r--   0 troyraen   (501) staff       (20)       13 2021-08-03 22:31:53.000000 pgb_broker_utils-0.2.8/pgb_broker_utils.egg-info/top_level.txt
--rw-r--r--   0 troyraen   (501) staff       (20)      196 2021-07-14 03:28:29.000000 pgb_broker_utils-0.2.8/requirements.txt
--rw-r--r--   0 troyraen   (501) staff       (20)       38 2021-08-03 22:31:53.000000 pgb_broker_utils-0.2.8/setup.cfg
--rw-r--r--   0 troyraen   (501) staff       (20)     2457 2021-08-03 22:30:28.000000 pgb_broker_utils-0.2.8/setup.py
+drwxr-xr-x   0 troyraen   (501) staff       (20)        0 2021-08-07 16:42:35.000000 pgb_broker_utils-0.2.9/
+-rw-r--r--   0 troyraen   (501) staff       (20)    34515 2021-08-04 00:04:29.000000 pgb_broker_utils-0.2.9/LICENSE.txt
+-rw-r--r--   0 troyraen   (501) staff       (20)       25 2021-08-04 00:04:29.000000 pgb_broker_utils-0.2.9/MANIFEST.in
+-rw-r--r--   0 troyraen   (501) staff       (20)     1173 2021-08-07 16:42:35.000000 pgb_broker_utils-0.2.9/PKG-INFO
+-rw-r--r--   0 troyraen   (501) staff       (20)      404 2021-08-04 00:04:29.000000 pgb_broker_utils-0.2.9/README.md
+drwxr-xr-x   0 troyraen   (501) staff       (20)        0 2021-08-07 16:42:35.000000 pgb_broker_utils-0.2.9/broker_utils/
+-rw-r--r--   0 troyraen   (501) staff       (20)      186 2021-08-04 00:04:29.000000 pgb_broker_utils-0.2.9/broker_utils/__init__.py
+-rw-r--r--   0 troyraen   (501) staff       (20)     4417 2021-08-04 00:04:29.000000 pgb_broker_utils-0.2.9/broker_utils/beam_transforms.py
+-rw-r--r--   0 troyraen   (501) staff       (20)    11779 2021-08-04 00:04:29.000000 pgb_broker_utils-0.2.9/broker_utils/consumer_sim.py
+-rw-r--r--   0 troyraen   (501) staff       (20)     1982 2021-08-04 00:04:29.000000 pgb_broker_utils-0.2.9/broker_utils/data_utils.py
+-rw-r--r--   0 troyraen   (501) staff       (20)     8239 2021-08-06 20:34:09.000000 pgb_broker_utils-0.2.9/broker_utils/gcp_utils.py
+-rw-r--r--   0 troyraen   (501) staff       (20)     1750 2021-08-04 00:04:29.000000 pgb_broker_utils-0.2.9/broker_utils/schema_maps.py
+drwxr-xr-x   0 troyraen   (501) staff       (20)        0 2021-08-07 16:42:35.000000 pgb_broker_utils-0.2.9/pgb_broker_utils.egg-info/
+-rw-r--r--   0 troyraen   (501) staff       (20)     1173 2021-08-07 16:42:35.000000 pgb_broker_utils-0.2.9/pgb_broker_utils.egg-info/PKG-INFO
+-rw-r--r--   0 troyraen   (501) staff       (20)      425 2021-08-07 16:42:35.000000 pgb_broker_utils-0.2.9/pgb_broker_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 troyraen   (501) staff       (20)        1 2021-08-07 16:42:35.000000 pgb_broker_utils-0.2.9/pgb_broker_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 troyraen   (501) staff       (20)      155 2021-08-07 16:42:35.000000 pgb_broker_utils-0.2.9/pgb_broker_utils.egg-info/requires.txt
+-rw-r--r--   0 troyraen   (501) staff       (20)       13 2021-08-07 16:42:35.000000 pgb_broker_utils-0.2.9/pgb_broker_utils.egg-info/top_level.txt
+-rw-r--r--   0 troyraen   (501) staff       (20)      196 2021-08-04 00:04:29.000000 pgb_broker_utils-0.2.9/requirements.txt
+-rw-r--r--   0 troyraen   (501) staff       (20)       38 2021-08-07 16:42:35.000000 pgb_broker_utils-0.2.9/setup.cfg
+-rw-r--r--   0 troyraen   (501) staff       (20)     2457 2021-08-06 20:08:13.000000 pgb_broker_utils-0.2.9/setup.py
```

### Comparing `pgb_broker_utils-0.2.8/LICENSE.txt` & `pgb_broker_utils-0.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pgb_broker_utils-0.2.8/PKG-INFO` & `pgb_broker_utils-0.2.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgb_broker_utils
-Version: 0.2.8
+Version: 0.2.9
 Summary: Tools used by the Pitt-Google astronomical alert broker.
 Home-page: https://github.com/mwvgroup/Pitt-Google-Broker
 Author: Troy Raen
 Author-email: troy.raen@pitt.edu
 License: UNKNOWN
 Keywords: astronomy,alert broker
 Platform: UNKNOWN
```

### Comparing `pgb_broker_utils-0.2.8/broker_utils/beam_transforms.py` & `pgb_broker_utils-0.2.9/broker_utils/beam_transforms.py`

 * *Files identical despite different names*

### Comparing `pgb_broker_utils-0.2.8/broker_utils/consumer_sim.py` & `pgb_broker_utils-0.2.9/broker_utils/consumer_sim.py`

 * *Files identical despite different names*

### Comparing `pgb_broker_utils-0.2.8/broker_utils/data_utils.py` & `pgb_broker_utils-0.2.9/broker_utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `pgb_broker_utils-0.2.8/broker_utils/schema_maps.py` & `pgb_broker_utils-0.2.9/broker_utils/schema_maps.py`

 * *Files identical despite different names*

### Comparing `pgb_broker_utils-0.2.8/pgb_broker_utils.egg-info/PKG-INFO` & `pgb_broker_utils-0.2.9/pgb_broker_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgb-broker-utils
-Version: 0.2.8
+Version: 0.2.9
 Summary: Tools used by the Pitt-Google astronomical alert broker.
 Home-page: https://github.com/mwvgroup/Pitt-Google-Broker
 Author: Troy Raen
 Author-email: troy.raen@pitt.edu
 License: UNKNOWN
 Keywords: astronomy,alert broker
 Platform: UNKNOWN
```

### Comparing `pgb_broker_utils-0.2.8/setup.py` & `pgb_broker_utils-0.2.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='pgb_broker_utils',  # Required
-    version='0.2.8',  # Required
+    version='0.2.9',  # Required
     description='Tools used by the Pitt-Google astronomical alert broker.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering :: Astronomy',
```

