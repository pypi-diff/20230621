# Comparing `tmp/Telexy.MARS-1.23.623.tar.gz` & `tmp/Telexy.MARS-1.23.624.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Telexy.MARS-1.23.623.tar", last modified: Wed Jun 21 00:44:15 2023, max compression
+gzip compressed data, was "Telexy.MARS-1.23.624.tar", last modified: Wed Jun 21 03:21:32 2023, max compression
```

## Comparing `Telexy.MARS-1.23.623.tar` & `Telexy.MARS-1.23.624.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 00:44:15.440959 Telexy.MARS-1.23.623/
--rw-rw-rw-   0        0        0     1076 2023-03-15 22:01:12.000000 Telexy.MARS-1.23.623/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-06-21 00:44:15.425442 Telexy.MARS-1.23.623/MARS/
--rw-rw-rw-   0        0        0     1010 2023-06-21 00:21:13.000000 Telexy.MARS-1.23.623/MARS/MARS.py
--rw-rw-rw-   0        0        0     1859 2023-06-20 23:59:15.000000 Telexy.MARS-1.23.623/MARS/MARSRegistry.py
--rw-rw-rw-   0        0        0        0 2023-06-21 00:43:26.000000 Telexy.MARS-1.23.623/MARS/__init__.py
--rw-rw-rw-   0        0        0      478 2023-06-21 00:44:15.438959 Telexy.MARS-1.23.623/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-21 00:44:15.437957 Telexy.MARS-1.23.623/Telexy.MARS.egg-info/
--rw-rw-rw-   0        0        0      478 2023-06-21 00:44:15.000000 Telexy.MARS-1.23.623/Telexy.MARS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-06-21 00:44:15.000000 Telexy.MARS-1.23.623/Telexy.MARS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 00:44:15.000000 Telexy.MARS-1.23.623/Telexy.MARS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-06-21 00:44:15.000000 Telexy.MARS-1.23.623/Telexy.MARS.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-21 00:44:15.000000 Telexy.MARS-1.23.623/Telexy.MARS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-21 00:44:15.440959 Telexy.MARS-1.23.623/setup.cfg
--rw-rw-rw-   0        0        0     1445 2023-06-21 00:43:33.000000 Telexy.MARS-1.23.623/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:21:32.041847 Telexy.MARS-1.23.624/
+-rw-rw-rw-   0        0        0     1076 2023-03-15 22:01:12.000000 Telexy.MARS-1.23.624/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-06-21 03:21:32.031836 Telexy.MARS-1.23.624/MARS/
+-rw-rw-rw-   0        0        0       23 2023-06-21 03:20:36.000000 Telexy.MARS-1.23.624/MARS/__init__.py
+-rw-rw-rw-   0        0        0      879 2023-06-21 03:20:52.000000 Telexy.MARS-1.23.624/MARS/__main__.py
+-rw-rw-rw-   0        0        0     1859 2023-06-20 23:59:15.000000 Telexy.MARS-1.23.624/MARS/registry.py
+-rw-rw-rw-   0        0        0      478 2023-06-21 03:21:32.040844 Telexy.MARS-1.23.624/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-21 03:21:32.039844 Telexy.MARS-1.23.624/Telexy.MARS.egg-info/
+-rw-rw-rw-   0        0        0      478 2023-06-21 03:21:31.000000 Telexy.MARS-1.23.624/Telexy.MARS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-06-21 03:21:31.000000 Telexy.MARS-1.23.624/Telexy.MARS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 03:21:31.000000 Telexy.MARS-1.23.624/Telexy.MARS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-06-21 03:21:31.000000 Telexy.MARS-1.23.624/Telexy.MARS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-21 03:21:31.000000 Telexy.MARS-1.23.624/Telexy.MARS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 03:21:32.041847 Telexy.MARS-1.23.624/setup.cfg
+-rw-rw-rw-   0        0        0     1429 2023-06-21 03:21:29.000000 Telexy.MARS-1.23.624/setup.py
```

### Comparing `Telexy.MARS-1.23.623/LICENSE.txt` & `Telexy.MARS-1.23.624/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Telexy.MARS-1.23.623/MARS/MARS.py` & `Telexy.MARS-1.23.624/MARS/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 import cherrypy
-from registration import *
+from registry import *
 
 @cherrypy.expose
 class MARS(object):
 
     def __init__(self, keys, values):
         for(key, value) in zip(keys, values):
             self.__dict__[key] = value
 
 
-if __name__ == '__main__':
     
-    #fusePlugin = MARSApplicationRegistryPlugin("FuseApi", "Fuse", "Telexy.DS.Fuse")
-    #register(fusePlugin)
+#fusePlugin = MARSApplicationRegistryPlugin("FuseApi", "Fuse", "Telexy.DS.Fuse")
+#register(fusePlugin)
 
-    conf = {
-        '/': {
-        }
+conf = {
+    '/': {
     }
+}
 
-    cherrypy.config.update({
-        'server.socket_host' : '0.0.0.0',
-        'server.socket_port' : 8080
-    })
-
-    #retrieve registered plug ins and instantiate them
-    regItems = getRegisteredPlugins()
-    paths = []
-    instances = []
-    for i in regItems:
-        # get paths
-        paths.append(i.applicationPath)
-        # create instance
-        inst = i.instantiate()
-        # append instance
-        instances.append(inst)
-        # retrieve configurations
-        conf['/' + i.applicationPath] = inst.configuration()
+cherrypy.config.update({
+    'server.socket_host' : '0.0.0.0',
+    'server.socket_port' : 8080
+})
+
+#retrieve registered plug ins and instantiate them
+regItems = getRegisteredPlugins()
+paths = []
+instances = []
+for i in regItems:
+    # get paths
+    paths.append(i.applicationPath)
+    # create instance
+    inst = i.instantiate()
+    # append instance
+    instances.append(inst)
+    # retrieve configurations
+    conf['/' + i.applicationPath] = inst.configuration()
 
-    webapp = MARS(paths, instances)
+webapp = MARS(paths, instances)
 
-    cherrypy.quickstart(webapp, '/', conf)
+cherrypy.quickstart(webapp, '/', conf)
```

### Comparing `Telexy.MARS-1.23.623/MARS/MARSRegistry.py` & `Telexy.MARS-1.23.624/MARS/registry.py`

 * *Files identical despite different names*

### Comparing `Telexy.MARS-1.23.623/setup.py` & `Telexy.MARS-1.23.624/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="Telexy.MARS",                     # This is the name of the package
-    version="1.23.623",                        # The initial release version
+    version="1.23.624",                        # The initial release version
     author="Telexy",                     # Full name of the author
     author_email="support@telexy.com", # Full email of author
     description="MARS Inference server",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],                                      # Information to filter the project on PyPi website
     python_requires='>=3.10',                # Minimum version requirement of the package
-    py_modules=["MARS", "MARSRegistry"],             # Name of the python package
+    py_modules=["MARS"],             # Name of the python package
     #package_dir={'':'/Telexy'},     # Directory of the source code of the package
     install_requires=['jsonpickle', "cherrypy"]                     # Install other dependencies if any
 )
```

