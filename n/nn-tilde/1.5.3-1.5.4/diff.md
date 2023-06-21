# Comparing `tmp/nn_tilde-1.5.3.tar.gz` & `tmp/nn_tilde-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nn_tilde-1.5.3.tar", last modified: Tue Jun  6 13:42:08 2023, max compression
+gzip compressed data, was "nn_tilde-1.5.4.tar", last modified: Wed Jun 21 15:41:59 2023, max compression
```

## Comparing `nn_tilde-1.5.3.tar` & `nn_tilde-1.5.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:42:08.853924 nn_tilde-1.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)    19916 2023-06-06 13:40:18.000000 nn_tilde-1.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-06 13:40:18.000000 nn_tilde-1.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9871 2023-06-06 13:42:08.853924 nn_tilde-1.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9676 2023-06-06 13:40:18.000000 nn_tilde-1.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:42:08.853924 nn_tilde-1.5.3/nn_tilde.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9871 2023-06-06 13:42:08.000000 nn_tilde-1.5.3/nn_tilde.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-06 13:42:08.000000 nn_tilde-1.5.3/nn_tilde.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 13:42:08.000000 nn_tilde-1.5.3/nn_tilde.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-06 13:42:08.000000 nn_tilde-1.5.3/nn_tilde.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-06 13:42:08.000000 nn_tilde-1.5.3/nn_tilde.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:42:08.853924 nn_tilde-1.5.3/python_tools/
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-06-06 13:40:18.000000 nn_tilde-1.5.3/python_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-06 13:40:18.000000 nn_tilde-1.5.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 13:42:08.853924 nn_tilde-1.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-06 13:40:18.000000 nn_tilde-1.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:41:59.972024 nn_tilde-1.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    19916 2023-06-21 15:39:52.000000 nn_tilde-1.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-21 15:39:52.000000 nn_tilde-1.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10235 2023-06-21 15:41:59.972024 nn_tilde-1.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10048 2023-06-21 15:39:52.000000 nn_tilde-1.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:41:59.972024 nn_tilde-1.5.4/nn_tilde.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10235 2023-06-21 15:41:59.000000 nn_tilde-1.5.4/nn_tilde.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-21 15:41:59.000000 nn_tilde-1.5.4/nn_tilde.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 15:41:59.000000 nn_tilde-1.5.4/nn_tilde.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-21 15:41:59.000000 nn_tilde-1.5.4/nn_tilde.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-21 15:41:59.000000 nn_tilde-1.5.4/nn_tilde.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:41:59.972024 nn_tilde-1.5.4/python_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-06-21 15:39:52.000000 nn_tilde-1.5.4/python_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-21 15:39:52.000000 nn_tilde-1.5.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 15:41:59.972024 nn_tilde-1.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-21 15:39:52.000000 nn_tilde-1.5.4/setup.py
```

### Comparing `nn_tilde-1.5.3/LICENSE` & `nn_tilde-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nn_tilde-1.5.3/PKG-INFO` & `nn_tilde-1.5.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nn_tilde
-Version: 1.5.3
+Version: 1.5.4
 Summary: Set of tools to create nn_tilde compatible models.
 Author: Antoine CAILLON
 Author-email: caillon@ircam.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -211,7 +211,17 @@
 While nn~ can be compiled and used on Raspberry Pi, you may have to consider using lighter deep learning models. We currently only support 64bit OS.
 
 Install nn~ for PureData using
 
 ```bash
 curl -s https://raw.githubusercontent.com/acids-ircam/nn_tilde/master/install/raspberrypi.sh | bash
 ```
+
+# Funding
+
+This work is led at IRCAM, and has been funded by the following projects
+
+* [ANR MakiMono](https://acids.ircam.fr/course/makimono/)
+* [ACTOR](https://www.actorproject.org/)
+* [DAFNE+](https://dafneplus.eu/) N° 101061548
+
+<img src="https://ec.europa.eu/regional_policy/images/information-sources/logo-download-center/eu_co_funded_en.jpg" width=200px/>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nn_tilde Version: 1.5.3 Summary: Set of tools to
+Metadata-Version: 2.1 Name: nn_tilde Version: 1.5.4 Summary: Set of tools to
 create nn_tilde compatible models. Author: Antoine CAILLON Author-email:
 caillon@ircam.fr Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
 License-File: LICENSE ![banner](https://github.com/acids-ircam/nn_tilde/raw/
 master/assets/banner.png) # Demonstration video [![RAVE x nn~](http://
 img.youtube.com/vi/dMZs04TzxUI/mqdefault.jpg)](https://www.youtube.com/
@@ -116,8 +116,12 @@
 Install Visual Studio and the C++ tools - Run the following commands: ```bash
 git clone https://github.com/acids-ircam/nn_tilde --recurse-submodules cd
 nn_tilde mkdir build cd build cmake ..\src -A x64 -DCMAKE_PREFIX_PATH="" cmake
 --build . --config Release ``` ## Raspberry Pi While nn~ can be compiled and
 used on Raspberry Pi, you may have to consider using lighter deep learning
 models. We currently only support 64bit OS. Install nn~Â for PureData using
 ```bash curl -s https://raw.githubusercontent.com/acids-ircam/nn_tilde/master/
-install/raspberrypi.sh | bash ```
+install/raspberrypi.sh | bash ``` # Funding This work is led at IRCAM, and has
+been funded by the following projects * [ANR MakiMono](https://acids.ircam.fr/
+course/makimono/) * [ACTOR](https://www.actorproject.org/) * [DAFNE+](https://
+dafneplus.eu/) NÂ° 101061548 [https://ec.europa.eu/regional_policy/images/
+information-sources/logo-download-center/eu_co_funded_en.jpg]
```

### Comparing `nn_tilde-1.5.3/README.md` & `nn_tilde-1.5.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -198,7 +198,17 @@
 While nn~ can be compiled and used on Raspberry Pi, you may have to consider using lighter deep learning models. We currently only support 64bit OS.
 
 Install nn~ for PureData using
 
 ```bash
 curl -s https://raw.githubusercontent.com/acids-ircam/nn_tilde/master/install/raspberrypi.sh | bash
 ```
+
+# Funding
+
+This work is led at IRCAM, and has been funded by the following projects
+
+* [ANR MakiMono](https://acids.ircam.fr/course/makimono/)
+* [ACTOR](https://www.actorproject.org/)
+* [DAFNE+](https://dafneplus.eu/) N° 101061548
+
+<img src="https://ec.europa.eu/regional_policy/images/information-sources/logo-download-center/eu_co_funded_en.jpg" width=200px/>
```

#### html2text {}

```diff
@@ -111,8 +111,12 @@
 Install Visual Studio and the C++ tools - Run the following commands: ```bash
 git clone https://github.com/acids-ircam/nn_tilde --recurse-submodules cd
 nn_tilde mkdir build cd build cmake ..\src -A x64 -DCMAKE_PREFIX_PATH="" cmake
 --build . --config Release ``` ## Raspberry Pi While nn~ can be compiled and
 used on Raspberry Pi, you may have to consider using lighter deep learning
 models. We currently only support 64bit OS. Install nn~Â for PureData using
 ```bash curl -s https://raw.githubusercontent.com/acids-ircam/nn_tilde/master/
-install/raspberrypi.sh | bash ```
+install/raspberrypi.sh | bash ``` # Funding This work is led at IRCAM, and has
+been funded by the following projects * [ANR MakiMono](https://acids.ircam.fr/
+course/makimono/) * [ACTOR](https://www.actorproject.org/) * [DAFNE+](https://
+dafneplus.eu/) NÂ° 101061548 [https://ec.europa.eu/regional_policy/images/
+information-sources/logo-download-center/eu_co_funded_en.jpg]
```

### Comparing `nn_tilde-1.5.3/nn_tilde.egg-info/PKG-INFO` & `nn_tilde-1.5.4/nn_tilde.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nn-tilde
-Version: 1.5.3
+Version: 1.5.4
 Summary: Set of tools to create nn_tilde compatible models.
 Author: Antoine CAILLON
 Author-email: caillon@ircam.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -211,7 +211,17 @@
 While nn~ can be compiled and used on Raspberry Pi, you may have to consider using lighter deep learning models. We currently only support 64bit OS.
 
 Install nn~ for PureData using
 
 ```bash
 curl -s https://raw.githubusercontent.com/acids-ircam/nn_tilde/master/install/raspberrypi.sh | bash
 ```
+
+# Funding
+
+This work is led at IRCAM, and has been funded by the following projects
+
+* [ANR MakiMono](https://acids.ircam.fr/course/makimono/)
+* [ACTOR](https://www.actorproject.org/)
+* [DAFNE+](https://dafneplus.eu/) N° 101061548
+
+<img src="https://ec.europa.eu/regional_policy/images/information-sources/logo-download-center/eu_co_funded_en.jpg" width=200px/>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nn-tilde Version: 1.5.3 Summary: Set of tools to
+Metadata-Version: 2.1 Name: nn-tilde Version: 1.5.4 Summary: Set of tools to
 create nn_tilde compatible models. Author: Antoine CAILLON Author-email:
 caillon@ircam.fr Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
 License-File: LICENSE ![banner](https://github.com/acids-ircam/nn_tilde/raw/
 master/assets/banner.png) # Demonstration video [![RAVE x nn~](http://
 img.youtube.com/vi/dMZs04TzxUI/mqdefault.jpg)](https://www.youtube.com/
@@ -116,8 +116,12 @@
 Install Visual Studio and the C++ tools - Run the following commands: ```bash
 git clone https://github.com/acids-ircam/nn_tilde --recurse-submodules cd
 nn_tilde mkdir build cd build cmake ..\src -A x64 -DCMAKE_PREFIX_PATH="" cmake
 --build . --config Release ``` ## Raspberry Pi While nn~ can be compiled and
 used on Raspberry Pi, you may have to consider using lighter deep learning
 models. We currently only support 64bit OS. Install nn~Â for PureData using
 ```bash curl -s https://raw.githubusercontent.com/acids-ircam/nn_tilde/master/
-install/raspberrypi.sh | bash ```
+install/raspberrypi.sh | bash ``` # Funding This work is led at IRCAM, and has
+been funded by the following projects * [ANR MakiMono](https://acids.ircam.fr/
+course/makimono/) * [ACTOR](https://www.actorproject.org/) * [DAFNE+](https://
+dafneplus.eu/) NÂ° 101061548 [https://ec.europa.eu/regional_policy/images/
+information-sources/logo-download-center/eu_co_funded_en.jpg]
```

### Comparing `nn_tilde-1.5.3/python_tools/__init__.py` & `nn_tilde-1.5.4/python_tools/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,14 +89,16 @@
                     f"Wrong number of output channels for method \"{method_name}\", "
                     f"expected {out_channels} got {y.shape[1]}"))
             if y.shape[2] != test_buffer_size // out_ratio:
                 raise ValueError(
                     (f"Wrong output length for method \"{method_name}\", "
                      f"expected {test_buffer_size//out_ratio} "
                      f"got {y.shape[2]}"))
+            if y.dtype != torch.float:
+                raise ValueError(f"Output tensor must be of type float, got {y.dtype}")
 
             if cc.MAX_BATCH_SIZE > 1:
                 logging.info(f"Testing method {method_name} with mc.nn~ API")
                 x = torch.zeros(4, in_channels, test_buffer_size // in_ratio)
                 y = getattr(self, method_name)(x)
 
                 if len(y.shape) != 3:
```

### Comparing `nn_tilde-1.5.3/setup.py` & `nn_tilde-1.5.4/setup.py`

 * *Files identical despite different names*

