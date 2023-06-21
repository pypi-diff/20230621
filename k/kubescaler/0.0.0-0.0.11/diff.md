# Comparing `tmp/kubescaler-0.0.0.tar.gz` & `tmp/kubescaler-0.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kubescaler-0.0.0.tar", last modified: Wed May 24 06:53:52 2023, max compression
+gzip compressed data, was "kubescaler-0.0.11.tar", last modified: Wed Jun 21 21:22:39 2023, max compression
```

## Comparing `kubescaler-0.0.0.tar` & `kubescaler-0.0.11.tar`

### file list

```diff
@@ -1,32 +1,37 @@
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-24 06:53:52.561457 kubescaler-0.0.0/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      498 2023-05-24 04:09:38.000000 kubescaler-0.0.0/COPYRIGHT
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1108 2023-05-24 04:09:38.000000 kubescaler-0.0.0/LICENSE
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      317 2023-05-24 04:15:45.000000 kubescaler-0.0.0/MANIFEST.in
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1167 2023-05-24 04:09:38.000000 kubescaler-0.0.0/NOTICE
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3240 2023-05-24 06:53:52.561457 kubescaler-0.0.0/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2389 2023-05-24 04:56:10.000000 kubescaler-0.0.0/README.md
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-24 06:53:52.561457 kubescaler-0.0.0/kubescaler/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       83 2023-05-24 04:51:49.000000 kubescaler-0.0.0/kubescaler/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2190 2023-05-24 04:47:55.000000 kubescaler-0.0.0/kubescaler/cluster.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1570 2023-05-24 04:37:00.000000 kubescaler-0.0.0/kubescaler/decorators.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      524 2023-05-24 04:39:56.000000 kubescaler-0.0.0/kubescaler/defaults.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6105 2023-05-24 04:39:20.000000 kubescaler-0.0.0/kubescaler/logger.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-24 06:53:52.561457 kubescaler-0.0.0/kubescaler/scaler/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       30 2023-05-24 04:51:40.000000 kubescaler-0.0.0/kubescaler/scaler/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    10080 2023-05-24 06:17:17.000000 kubescaler-0.0.0/kubescaler/scaler/google.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-24 06:53:52.561457 kubescaler-0.0.0/kubescaler/utils/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      429 2023-05-24 06:14:50.000000 kubescaler-0.0.0/kubescaler/utils/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5085 2023-05-24 04:38:51.000000 kubescaler-0.0.0/kubescaler/utils/fileio.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1456 2023-05-24 04:38:11.000000 kubescaler-0.0.0/kubescaler/utils/misc.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2615 2023-05-24 04:37:51.000000 kubescaler-0.0.0/kubescaler/utils/terminal.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1303 2023-05-24 04:36:48.000000 kubescaler-0.0.0/kubescaler/version.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-24 06:53:52.561457 kubescaler-0.0.0/kubescaler.egg-info/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3240 2023-05-24 06:53:52.000000 kubescaler-0.0.0/kubescaler.egg-info/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      586 2023-05-24 06:53:52.000000 kubescaler-0.0.0/kubescaler.egg-info/SOURCES.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-05-24 06:53:52.000000 kubescaler-0.0.0/kubescaler.egg-info/dependency_links.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-05-24 05:01:47.000000 kubescaler-0.0.0/kubescaler.egg-info/not-zip-safe
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      142 2023-05-24 06:53:52.000000 kubescaler-0.0.0/kubescaler.egg-info/requires.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       11 2023-05-24 06:53:52.000000 kubescaler-0.0.0/kubescaler.egg-info/top_level.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      132 2023-05-24 04:09:39.000000 kubescaler-0.0.0/pyproject.toml
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      225 2023-05-24 06:53:52.565457 kubescaler-0.0.0/setup.cfg
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3582 2023-05-24 04:57:06.000000 kubescaler-0.0.0/setup.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-21 21:22:39.094038 kubescaler-0.0.11/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      498 2023-05-24 04:09:38.000000 kubescaler-0.0.11/COPYRIGHT
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1108 2023-05-24 04:09:38.000000 kubescaler-0.0.11/LICENSE
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      317 2023-05-24 04:15:45.000000 kubescaler-0.0.11/MANIFEST.in
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1167 2023-05-24 04:09:38.000000 kubescaler-0.0.11/NOTICE
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3372 2023-06-21 21:22:39.094038 kubescaler-0.0.11/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2512 2023-05-25 18:09:11.000000 kubescaler-0.0.11/README.md
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-21 21:22:39.090038 kubescaler-0.0.11/kubescaler/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       43 2023-05-25 18:09:11.000000 kubescaler-0.0.11/kubescaler/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2370 2023-05-25 18:09:11.000000 kubescaler-0.0.11/kubescaler/cluster.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1755 2023-05-25 18:09:11.000000 kubescaler-0.0.11/kubescaler/decorators.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      604 2023-05-25 18:09:11.000000 kubescaler-0.0.11/kubescaler/defaults.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6105 2023-05-24 04:39:20.000000 kubescaler-0.0.11/kubescaler/logger.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-21 21:22:39.090038 kubescaler-0.0.11/kubescaler/scaler/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       59 2023-05-25 18:09:11.000000 kubescaler-0.0.11/kubescaler/scaler/__init__.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-21 21:22:39.094038 kubescaler-0.0.11/kubescaler/scaler/aws/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       32 2023-05-25 18:09:11.000000 kubescaler-0.0.11/kubescaler/scaler/aws/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1103 2023-05-25 18:09:11.000000 kubescaler-0.0.11/kubescaler/scaler/aws/ami.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    22082 2023-05-25 18:09:11.000000 kubescaler-0.0.11/kubescaler/scaler/aws/cluster.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1316 2023-05-25 18:09:11.000000 kubescaler-0.0.11/kubescaler/scaler/aws/template.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    11961 2023-06-21 21:22:35.000000 kubescaler-0.0.11/kubescaler/scaler/google.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-21 21:22:39.094038 kubescaler-0.0.11/kubescaler/utils/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      399 2023-05-25 18:09:11.000000 kubescaler-0.0.11/kubescaler/utils/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5085 2023-05-25 18:09:11.000000 kubescaler-0.0.11/kubescaler/utils/fileio.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1456 2023-05-24 04:38:11.000000 kubescaler-0.0.11/kubescaler/utils/misc.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      912 2023-05-25 18:09:11.000000 kubescaler-0.0.11/kubescaler/utils/terminal.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1414 2023-06-21 21:22:35.000000 kubescaler-0.0.11/kubescaler/version.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-21 21:22:39.090038 kubescaler-0.0.11/kubescaler.egg-info/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3372 2023-06-21 21:22:38.000000 kubescaler-0.0.11/kubescaler.egg-info/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      716 2023-06-21 21:22:39.000000 kubescaler-0.0.11/kubescaler.egg-info/SOURCES.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-06-21 21:22:38.000000 kubescaler-0.0.11/kubescaler.egg-info/dependency_links.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-05-24 05:01:47.000000 kubescaler-0.0.11/kubescaler.egg-info/not-zip-safe
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      228 2023-06-21 21:22:38.000000 kubescaler-0.0.11/kubescaler.egg-info/requires.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       11 2023-06-21 21:22:38.000000 kubescaler-0.0.11/kubescaler.egg-info/top_level.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      132 2023-05-24 04:09:39.000000 kubescaler-0.0.11/pyproject.toml
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      294 2023-06-21 21:22:39.094038 kubescaler-0.0.11/setup.cfg
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3582 2023-05-24 04:57:06.000000 kubescaler-0.0.11/setup.py
```

### Comparing `kubescaler-0.0.0/LICENSE` & `kubescaler-0.0.11/LICENSE`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.0/NOTICE` & `kubescaler-0.0.11/NOTICE`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.0/PKG-INFO` & `kubescaler-0.0.11/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: kubescaler
-Version: 0.0.0
+Version: 0.0.11
 Summary: Helper classes for scaling Kubernetes clusters
 Home-page: https://github.com/converged-computing/kubescaler
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
-Keywords: Kubernetes,elasticity,scaling
+Keywords: Kubernetes,elasticity,scaling,EKS,GKE
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
@@ -38,15 +38,15 @@
 </a>
 
 This is a set of helper Python classes that make it easy to add elasticity, or scaling
 up and down, of your Kubernetes clusters in Python. We currently have support for the clouds
 we use, namely:
 
 - Google (GKE)
-- Amazon (EKS) (under development)
+- Amazon (EKS)
 
 🚧️ **under development** 🚧️
 
 This tool is under development and is not ready for production use. Documentation
 and examples coming soon!
 
 ## 😁️ Contributors 😁️
@@ -66,14 +66,19 @@
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
 
+## TODO
+
+ - fix up GKE scale function to only be one function, we don't need to reset max and min again
+ - run experiments for scaling on EKS
+
 ## License
 
 HPCIC DevTools is distributed under the terms of the MIT license.
 All new contributions must be made under this license.
 
 See [LICENSE](https://github.com/converged-computing/kubescaler/blob/main/LICENSE),
 [COPYRIGHT](https://github.com/converged-computing/kubescaler/blob/main/COPYRIGHT), and
```

#### html2text {}

```diff
@@ -1,32 +1,34 @@
-Metadata-Version: 2.1 Name: kubescaler Version: 0.0.0 Summary: Helper classes
+Metadata-Version: 2.1 Name: kubescaler Version: 0.0.11 Summary: Helper classes
 for scaling Kubernetes clusters Home-page: https://github.com/converged-
 computing/kubescaler Author: Vanessa Sochat Author-email:
 vsoch@users.noreply.github.com Maintainer: Vanessa Sochat License: LICENSE
-Keywords: Kubernetes,elasticity,scaling Platform: UNKNOWN Classifier: Intended
-Audience :: Science/Research Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License Classifier: Programming
-Language :: Python Classifier: Topic :: Software Development Classifier: Topic
-:: Scientific/Engineering Classifier: Operating System :: Unix Classifier:
-Programming Language :: Python :: 3.8 Description-Content-Type: text/markdown
-Provides-Extra: all Provides-Extra: google Provides-Extra: aws License-File:
-LICENSE License-File: NOTICE # KubeScaler > Make your Kubernetes cluster YUGE!
-Or Smol. :)  [![All Contributors](https://img.shields.io/badge/
-all_contributors-1-orange.svg?style=flat-square)](#contributors-)  [![PyPI]
-(https://img.shields.io/pypi/v/kubescaler)](https://pypi.org/project/
-kubescaler/) [KubeScaler_Logo] This is a set of helper Python classes that make
-it easy to add elasticity, or scaling up and down, of your Kubernetes clusters
-in Python. We currently have support for the clouds we use, namely: - Google
-(GKE) - Amazon (EKS) (under development) ð§ï¸ **under development** ð§ï¸
+Keywords: Kubernetes,elasticity,scaling,EKS,GKE Platform: UNKNOWN Classifier:
+Intended Audience :: Science/Research Classifier: Intended Audience ::
+Developers Classifier: License :: OSI Approved :: MIT License Classifier:
+Programming Language :: Python Classifier: Topic :: Software Development
+Classifier: Topic :: Scientific/Engineering Classifier: Operating System ::
+Unix Classifier: Programming Language :: Python :: 3.8 Description-Content-
+Type: text/markdown Provides-Extra: all Provides-Extra: google Provides-Extra:
+aws License-File: LICENSE License-File: NOTICE # KubeScaler > Make your
+Kubernetes cluster YUGE! Or Smol. :)  [![All Contributors](https://
+img.shields.io/badge/all_contributors-1-orange.svg?style=flat-square)]
+(#contributors-)  [![PyPI](https://img.shields.io/pypi/v/kubescaler)](https://
+pypi.org/project/kubescaler/) [KubeScaler_Logo] This is a set of helper Python
+classes that make it easy to add elasticity, or scaling up and down, of your
+Kubernetes clusters in Python. We currently have support for the clouds we use,
+namely: - Google (GKE) - Amazon (EKS) ð§ï¸ **under development** ð§ï¸
 This tool is under development and is not ready for production use.
 Documentation and examples coming soon! ## ðï¸ Contributors ðï¸ We use
 the [all-contributors](https://github.com/all-contributors/all-contributors)
 tool to generate a contributors graphic below.
 [Vanessasaurus]
  Vanessasaurus
      ð»
-   ## License HPCIC DevTools is distributed under the terms of the MIT license.
-All new contributions must be made under this license. See [LICENSE](https://
+   ## TODO - fix up GKE scale function to only be one function, we don't need
+to reset max and min again - run experiments for scaling on EKS ## License
+HPCIC DevTools is distributed under the terms of the MIT license. All new
+contributions must be made under this license. See [LICENSE](https://
 github.com/converged-computing/kubescaler/blob/main/LICENSE), [COPYRIGHT]
 (https://github.com/converged-computing/kubescaler/blob/main/COPYRIGHT), and
 [NOTICE](https://github.com/converged-computing/kubescaler/blob/main/NOTICE)
 for details. SPDX-License-Identifier: (MIT) LLNL-CODE- 842614
```

### Comparing `kubescaler-0.0.0/README.md` & `kubescaler-0.0.11/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 </a>
 
 This is a set of helper Python classes that make it easy to add elasticity, or scaling
 up and down, of your Kubernetes clusters in Python. We currently have support for the clouds
 we use, namely:
 
 - Google (GKE)
-- Amazon (EKS) (under development)
+- Amazon (EKS)
 
 🚧️ **under development** 🚧️
 
 This tool is under development and is not ready for production use. Documentation
 and examples coming soon!
 
 ## 😁️ Contributors 😁️
@@ -40,14 +40,19 @@
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
 
+## TODO
+
+ - fix up GKE scale function to only be one function, we don't need to reset max and min again
+ - run experiments for scaling on EKS
+
 ## License
 
 HPCIC DevTools is distributed under the terms of the MIT license.
 All new contributions must be made under this license.
 
 See [LICENSE](https://github.com/converged-computing/kubescaler/blob/main/LICENSE),
 [COPYRIGHT](https://github.com/converged-computing/kubescaler/blob/main/COPYRIGHT), and
```

#### html2text {}

```diff
@@ -1,21 +1,23 @@
 # KubeScaler > Make your Kubernetes cluster YUGE! Or Smol. :)  [![All
 Contributors](https://img.shields.io/badge/all_contributors-1-
 orange.svg?style=flat-square)](#contributors-)  [![PyPI](https://
 img.shields.io/pypi/v/kubescaler)](https://pypi.org/project/kubescaler/)
 [KubeScaler_Logo] This is a set of helper Python classes that make it easy to
 add elasticity, or scaling up and down, of your Kubernetes clusters in Python.
 We currently have support for the clouds we use, namely: - Google (GKE) -
-Amazon (EKS) (under development) ð§ï¸ **under development** ð§ï¸ This
-tool is under development and is not ready for production use. Documentation
-and examples coming soon! ## ðï¸ Contributors ðï¸ We use the [all-
-contributors](https://github.com/all-contributors/all-contributors) tool to
-generate a contributors graphic below.
+Amazon (EKS) ð§ï¸ **under development** ð§ï¸ This tool is under
+development and is not ready for production use. Documentation and examples
+coming soon! ## ðï¸ Contributors ðï¸ We use the [all-contributors]
+(https://github.com/all-contributors/all-contributors) tool to generate a
+contributors graphic below.
 [Vanessasaurus]
  Vanessasaurus
      ð»
-   ## License HPCIC DevTools is distributed under the terms of the MIT license.
-All new contributions must be made under this license. See [LICENSE](https://
+   ## TODO - fix up GKE scale function to only be one function, we don't need
+to reset max and min again - run experiments for scaling on EKS ## License
+HPCIC DevTools is distributed under the terms of the MIT license. All new
+contributions must be made under this license. See [LICENSE](https://
 github.com/converged-computing/kubescaler/blob/main/LICENSE), [COPYRIGHT]
 (https://github.com/converged-computing/kubescaler/blob/main/COPYRIGHT), and
 [NOTICE](https://github.com/converged-computing/kubescaler/blob/main/NOTICE)
 for details. SPDX-License-Identifier: (MIT) LLNL-CODE- 842614
```

### Comparing `kubescaler-0.0.0/kubescaler/decorators.py` & `kubescaler-0.0.11/kubescaler/decorators.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright 2022-2023 Lawrence Livermore National Security, LLC and other
 # HPCIC DevTools Developers. See the top-level COPYRIGHT file for details.
 #
 # SPDX-License-Identifier: (MIT)
 
-from functools import partial, update_wrapper
 import time
+from functools import partial, update_wrapper
+
 
 class timed:
     """
     Time the runtime of a function, add to times
     """
 
     def __init__(self, func):
@@ -16,14 +17,18 @@
         self.func = func
 
     def __get__(self, obj, objtype):
         return partial(self.__call__, obj)
 
     def __call__(self, cls, *args, **kwargs):
         name = self.func.__name__
+
+        # If it's not create or delete cluster we need the node count
+        if name not in ["create_cluster", "delete_cluster"]:
+            name = f"{name}-size-{cls.node_count}"
         start = time.time()
         res = self.func(cls, *args, **kwargs)
         end = time.time()
         cls.times[name] = round(end - start, 3)
         return res
 
 
@@ -49,8 +54,8 @@
             try:
                 return self.func(cls, *args, **kwargs)
             except Exception as e:
                 sleep = timeout + 3**attempt
                 print(f"Retrying in {sleep} seconds - error: {e}")
                 time.sleep(sleep)
                 attempt += 1
-        return self.func(cls, *args, **kwargs)
+        return self.func(cls, *args, **kwargs)
```

### Comparing `kubescaler-0.0.0/kubescaler/defaults.py` & `kubescaler-0.0.11/kubescaler/defaults.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,9 +9,12 @@
 
 install_dir = utils.get_installdir()
 reps = {"$install_dir": install_dir, "$root_dir": os.path.dirname(install_dir)}
 
 # User home
 userhome = os.path.expanduser("~/.kubescaler")
 
+# Default Kubernetes version (aws doesn't have 1.27)
+kubernetes_version = 1.27
+
 # The default GitHub registry with recipes (for docgen)
 github_url = "https://github.com/converged-computing/kubescaler"
```

### Comparing `kubescaler-0.0.0/kubescaler/logger.py` & `kubescaler-0.0.11/kubescaler/logger.py`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.0/kubescaler/scaler/google.py` & `kubescaler-0.0.11/kubescaler/scaler/google.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,71 @@
-from google.cloud import container_v1
-from google.api_core.exceptions import NotFound
-from kubescaler.decorators import timed, retry
-from kubescaler.cluster import Cluster
+# Copyright 2023 Lawrence Livermore National Security, LLC and other
+# HPCIC DevTools Developers. See the top-level COPYRIGHT file for details.
+#
+# SPDX-License-Identifier: (MIT)
+
+import base64
+import sys
+import tempfile
 import time
 
+from kubernetes import client as kubernetes_client
+
+from kubescaler.cluster import Cluster
+from kubescaler.decorators import retry, timed
+
+try:
+    import google.auth
+    import google.auth.transport.requests
+    from google.api_core.exceptions import NotFound
+    from google.cloud import container_v1
+except ImportError:
+    sys.exit("Please pip install kubescaler[google]")
+
+
 class GKECluster(Cluster):
     """
     A scaler for a Google Kubernetes Engine (GKE) cluster
     """
+
+    default_region = "us-central1-a"
+
     def __init__(
         self,
         project,
-        *args,
-        machine_type="c2-standard-8",
         machine_type_memory_gb=32,
         machine_type_vcpu=8,
-        region="us-central1-a",
-        **kwargs
+        **kwargs,
     ):
         """
         A simple class to control creating a cluster
         """
-        super().__init__(*args, **kwargs)
+        super().__init__(**kwargs)
 
         # This client we can use to interact with Google Cloud GKE
         # https://github.com/googleapis/python-container/blob/main/google/cloud/container_v1/services/cluster_manager/client.py#L96
         print("⭐️ Creating global cluster manager client...")
         self.client = container_v1.ClusterManagerClient()
         self.project = project
-        self.region = region
-        self.machine_type = machine_type
+        self.machine_type = self.machine_type or "c2-standard-8"
         self.machine_type_vcpu = machine_type_vcpu
         self.machine_type_memory_gb = machine_type_memory_gb
+        self.tags = self.tags or ["kubescaler-cluster"]
+        self.configuration = None
 
     @timed
     def delete_cluster(self):
         """
         Delete the cluster
         """
         request = container_v1.DeleteClusterRequest(name=self.cluster_name)
         # Make the request, and check until deleted!
         self.client.delete_cluster(request=request)
+        self.configuration = None
         self.wait_for_delete()
-        # TODO we need a wait for create too!
 
     @property
     def zone(self):
         """
         The region is the zone minus the last letter!
         """
         return self.region.rsplit("-", 1)[0]
@@ -72,15 +91,17 @@
         """
         return self.scale(count, count, count + 1, pool_name=pool_name)
 
     def scale_down(self, count, pool_name="default-pool"):
         """
         Make a request to scale the cluster
         """
-        return self.scale(count, max(count - 1, 0), count, pool_name=pool_name)
+        return self.scale(
+            count, max(count - 1, self.min_nodes), count, pool_name=pool_name
+        )
 
     def scale(self, count, min_count, max_count, pool_name="default-pool"):
         """
         Make a request to scale the cluster
         """
         node_pool_name = f"{self.cluster_name}/nodePools/{pool_name}"
 
@@ -136,14 +157,47 @@
             # metadata = {"startup-script": my_startup_script,
             #            "user-data": my_user_data}
         )
         print("\n🥣️ cluster node_config")
         print(node_config)
         return node_config
 
+    def get_k8s_client(self):
+        """
+        Get a client to use to interact with the cluster, either corev1.api
+        or the kubernetes api client.
+
+        https://github.com/googleapis/python-container/issues/6
+        """
+        request = {"name": self.cluster_name}
+        response = self.client.get_cluster(request=request)
+        creds, projects = google.auth.default(
+            scopes=["https://www.googleapis.com/auth/cloud-platform"]
+        )
+        auth_req = google.auth.transport.requests.Request()
+        creds.refresh(auth_req)
+
+        # Save the configuration for advanced users to user later
+        if not self.configuration:
+            configuration = kubernetes_client.Configuration()
+            configuration.host = f"https://{response.endpoint}"
+            with tempfile.NamedTemporaryFile(delete=False) as ca_cert:
+                ca_cert.write(
+                    base64.b64decode(response.master_auth.cluster_ca_certificate)
+                )
+                configuration.ssl_ca_cert = ca_cert.name
+            configuration.api_key_prefix["authorization"] = "Bearer"
+            configuration.api_key["authorization"] = creds.token
+            self.configuration = configuration
+
+        # This has .api_client for just the api client
+        return kubernetes_client.CoreV1Api(
+            kubernetes_client.ApiClient(self.configuration)
+        )
+
     @property
     def cluster(self):
         """
         Get the cluster proto with our defaults
         """
         # Design our initial cluster!
         # https://github.com/googleapis/python-container/blob/main/google/cloud/container_v1/types/cluster_service.py#LL2119C1-L2124C1
```

### Comparing `kubescaler-0.0.0/kubescaler/utils/fileio.py` & `kubescaler-0.0.11/kubescaler/utils/fileio.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,14 @@
     except OSError as e:
         if e.errno == errno.EEXIST and os.path.isdir(path):
             pass
         else:
             logger.exit("Error creating path %s, exiting." % path)
 
 
-
 def get_tmpfile(tmpdir=None, prefix="kubescaler-"):
     """
     Get a temporary file with an optional prefix.
     """
 
     # First priority for the base goes to the user requested.
     tmpdir = tempfile.gettempdir()
@@ -145,15 +144,15 @@
     if os.path.exists(destination) and force is True:
         os.remove(destination)
 
     shutil.copyfile(source, destination)
     return destination
 
 
-def write_file(filename, content, mode="w", exec=False):
+def write_file(content, filename, mode="w", exec=False):
     """
     Write content to a filename
     """
     with open(filename, mode) as filey:
         filey.writelines(content)
     if exec:
         st = os.stat(filename)
@@ -209,8 +208,8 @@
     return content
 
 
 def read_json(filename, mode="r"):
     """
     Read a json file to a dictionary.
     """
-    return json.loads(read_file(filename))
+    return json.loads(read_file(filename))
```

### Comparing `kubescaler-0.0.0/kubescaler/utils/misc.py` & `kubescaler-0.0.11/kubescaler/utils/misc.py`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.0/kubescaler/version.py` & `kubescaler-0.0.11/kubescaler/version.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 # Copyright 2023 Lawrence Livermore National Security, LLC and other
 # HPCIC DevTools Developers. See the top-level COPYRIGHT file for details.
 #
 # SPDX-License-Identifier: (MIT)
 
-__version__ = "0.0.0"
+__version__ = "0.0.11"
 AUTHOR = "Vanessa Sochat"
 EMAIL = "vsoch@users.noreply.github.com"
 NAME = "kubescaler"
 PACKAGE_URL = "https://github.com/converged-computing/kubescaler"
-KEYWORDS = "Kubernetes, elasticity, scaling"
+KEYWORDS = "Kubernetes, elasticity, scaling, EKS, GKE"
 DESCRIPTION = "Helper classes for scaling Kubernetes clusters"
 LICENSE = "LICENSE"
 
 ################################################################################
 # Global requirements
 
 # Since we assume wanting Singularity and lmod, we require spython and Jinja2
 
 INSTALL_REQUIRES = (
     ("ruamel.yaml", {"min_version": None}),
     ("jsonschema", {"min_version": None}),
+    ("kubernetes", {"min_version": None}),
 )
 
-AWS_REQUIRES = (("boto3", {"min_version": None}),)
+AWS_REQUIRES = (
+    ("awscli", {"min_version": None}),
+    ("boto3", {"min_version": None}),
+)
 
 # Prefer discovery clients - more control
 GOOGLE_CLOUD_REQUIRES = (
-#    ("google-auth", {"min_version": None}),
     ("google-cloud-container", {"min_version": None}),
+    ("google-api-python-client", {"min_version": None}),
 )
 
 TESTS_REQUIRES = (("pytest", {"min_version": "4.6.2"}),)
 
 ################################################################################
 # Submodule Requirements (versions that include database)
```

### Comparing `kubescaler-0.0.0/kubescaler.egg-info/PKG-INFO` & `kubescaler-0.0.11/kubescaler.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: kubescaler
-Version: 0.0.0
+Version: 0.0.11
 Summary: Helper classes for scaling Kubernetes clusters
 Home-page: https://github.com/converged-computing/kubescaler
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
-Keywords: Kubernetes,elasticity,scaling
+Keywords: Kubernetes,elasticity,scaling,EKS,GKE
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
@@ -38,15 +38,15 @@
 </a>
 
 This is a set of helper Python classes that make it easy to add elasticity, or scaling
 up and down, of your Kubernetes clusters in Python. We currently have support for the clouds
 we use, namely:
 
 - Google (GKE)
-- Amazon (EKS) (under development)
+- Amazon (EKS)
 
 🚧️ **under development** 🚧️
 
 This tool is under development and is not ready for production use. Documentation
 and examples coming soon!
 
 ## 😁️ Contributors 😁️
@@ -66,14 +66,19 @@
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
 
+## TODO
+
+ - fix up GKE scale function to only be one function, we don't need to reset max and min again
+ - run experiments for scaling on EKS
+
 ## License
 
 HPCIC DevTools is distributed under the terms of the MIT license.
 All new contributions must be made under this license.
 
 See [LICENSE](https://github.com/converged-computing/kubescaler/blob/main/LICENSE),
 [COPYRIGHT](https://github.com/converged-computing/kubescaler/blob/main/COPYRIGHT), and
```

#### html2text {}

```diff
@@ -1,32 +1,34 @@
-Metadata-Version: 2.1 Name: kubescaler Version: 0.0.0 Summary: Helper classes
+Metadata-Version: 2.1 Name: kubescaler Version: 0.0.11 Summary: Helper classes
 for scaling Kubernetes clusters Home-page: https://github.com/converged-
 computing/kubescaler Author: Vanessa Sochat Author-email:
 vsoch@users.noreply.github.com Maintainer: Vanessa Sochat License: LICENSE
-Keywords: Kubernetes,elasticity,scaling Platform: UNKNOWN Classifier: Intended
-Audience :: Science/Research Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License Classifier: Programming
-Language :: Python Classifier: Topic :: Software Development Classifier: Topic
-:: Scientific/Engineering Classifier: Operating System :: Unix Classifier:
-Programming Language :: Python :: 3.8 Description-Content-Type: text/markdown
-Provides-Extra: all Provides-Extra: google Provides-Extra: aws License-File:
-LICENSE License-File: NOTICE # KubeScaler > Make your Kubernetes cluster YUGE!
-Or Smol. :)  [![All Contributors](https://img.shields.io/badge/
-all_contributors-1-orange.svg?style=flat-square)](#contributors-)  [![PyPI]
-(https://img.shields.io/pypi/v/kubescaler)](https://pypi.org/project/
-kubescaler/) [KubeScaler_Logo] This is a set of helper Python classes that make
-it easy to add elasticity, or scaling up and down, of your Kubernetes clusters
-in Python. We currently have support for the clouds we use, namely: - Google
-(GKE) - Amazon (EKS) (under development) ð§ï¸ **under development** ð§ï¸
+Keywords: Kubernetes,elasticity,scaling,EKS,GKE Platform: UNKNOWN Classifier:
+Intended Audience :: Science/Research Classifier: Intended Audience ::
+Developers Classifier: License :: OSI Approved :: MIT License Classifier:
+Programming Language :: Python Classifier: Topic :: Software Development
+Classifier: Topic :: Scientific/Engineering Classifier: Operating System ::
+Unix Classifier: Programming Language :: Python :: 3.8 Description-Content-
+Type: text/markdown Provides-Extra: all Provides-Extra: google Provides-Extra:
+aws License-File: LICENSE License-File: NOTICE # KubeScaler > Make your
+Kubernetes cluster YUGE! Or Smol. :)  [![All Contributors](https://
+img.shields.io/badge/all_contributors-1-orange.svg?style=flat-square)]
+(#contributors-)  [![PyPI](https://img.shields.io/pypi/v/kubescaler)](https://
+pypi.org/project/kubescaler/) [KubeScaler_Logo] This is a set of helper Python
+classes that make it easy to add elasticity, or scaling up and down, of your
+Kubernetes clusters in Python. We currently have support for the clouds we use,
+namely: - Google (GKE) - Amazon (EKS) ð§ï¸ **under development** ð§ï¸
 This tool is under development and is not ready for production use.
 Documentation and examples coming soon! ## ðï¸ Contributors ðï¸ We use
 the [all-contributors](https://github.com/all-contributors/all-contributors)
 tool to generate a contributors graphic below.
 [Vanessasaurus]
  Vanessasaurus
      ð»
-   ## License HPCIC DevTools is distributed under the terms of the MIT license.
-All new contributions must be made under this license. See [LICENSE](https://
+   ## TODO - fix up GKE scale function to only be one function, we don't need
+to reset max and min again - run experiments for scaling on EKS ## License
+HPCIC DevTools is distributed under the terms of the MIT license. All new
+contributions must be made under this license. See [LICENSE](https://
 github.com/converged-computing/kubescaler/blob/main/LICENSE), [COPYRIGHT]
 (https://github.com/converged-computing/kubescaler/blob/main/COPYRIGHT), and
 [NOTICE](https://github.com/converged-computing/kubescaler/blob/main/NOTICE)
 for details. SPDX-License-Identifier: (MIT) LLNL-CODE- 842614
```

### Comparing `kubescaler-0.0.0/kubescaler.egg-info/SOURCES.txt` & `kubescaler-0.0.11/kubescaler.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -16,11 +16,15 @@
 kubescaler.egg-info/SOURCES.txt
 kubescaler.egg-info/dependency_links.txt
 kubescaler.egg-info/not-zip-safe
 kubescaler.egg-info/requires.txt
 kubescaler.egg-info/top_level.txt
 kubescaler/scaler/__init__.py
 kubescaler/scaler/google.py
+kubescaler/scaler/aws/__init__.py
+kubescaler/scaler/aws/ami.py
+kubescaler/scaler/aws/cluster.py
+kubescaler/scaler/aws/template.py
 kubescaler/utils/__init__.py
 kubescaler/utils/fileio.py
 kubescaler/utils/misc.py
 kubescaler/utils/terminal.py
```

### Comparing `kubescaler-0.0.0/setup.py` & `kubescaler-0.0.11/setup.py`

 * *Files identical despite different names*

