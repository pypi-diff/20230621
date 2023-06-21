# Comparing `tmp/plemmy-0.2.0.tar.gz` & `tmp/plemmy-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plemmy-0.2.0.tar", last modified: Tue Jun 20 22:26:54 2023, max compression
+gzip compressed data, was "plemmy-0.2.1.tar", last modified: Wed Jun 21 05:08:33 2023, max compression
```

## Comparing `plemmy-0.2.0.tar` & `plemmy-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-06-20 22:26:54.350271 plemmy-0.2.0/
--rw-r--r--   0 tjkessler   (501) staff       (20)    11367 2023-06-20 19:47:16.000000 plemmy-0.2.0/LICENSE
--rw-r--r--   0 tjkessler   (501) staff       (20)     1961 2023-06-20 22:26:54.350098 plemmy-0.2.0/PKG-INFO
--rw-r--r--   0 tjkessler   (501) staff       (20)     1675 2023-06-20 22:25:52.000000 plemmy-0.2.0/README.md
-drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-06-20 22:26:54.348959 plemmy-0.2.0/plemmy/
--rw-r--r--   0 tjkessler   (501) staff       (20)      140 2023-06-20 19:47:16.000000 plemmy-0.2.0/plemmy/__init__.py
--rw-r--r--   0 tjkessler   (501) staff       (20)    42043 2023-06-20 22:25:52.000000 plemmy-0.2.0/plemmy/lemmyhttp.py
--rw-r--r--   0 tjkessler   (501) staff       (20)     1395 2023-06-20 19:47:16.000000 plemmy-0.2.0/plemmy/utils.py
--rw-r--r--   0 tjkessler   (501) staff       (20)      120 2023-06-20 22:25:52.000000 plemmy-0.2.0/plemmy/version.py
-drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-06-20 22:26:54.349872 plemmy-0.2.0/plemmy.egg-info/
--rw-r--r--   0 tjkessler   (501) staff       (20)     1961 2023-06-20 22:26:54.000000 plemmy-0.2.0/plemmy.egg-info/PKG-INFO
--rw-r--r--   0 tjkessler   (501) staff       (20)      277 2023-06-20 22:26:54.000000 plemmy-0.2.0/plemmy.egg-info/SOURCES.txt
--rw-r--r--   0 tjkessler   (501) staff       (20)        1 2023-06-20 22:26:54.000000 plemmy-0.2.0/plemmy.egg-info/dependency_links.txt
--rw-r--r--   0 tjkessler   (501) staff       (20)        1 2023-06-20 22:26:54.000000 plemmy-0.2.0/plemmy.egg-info/not-zip-safe
--rw-r--r--   0 tjkessler   (501) staff       (20)       17 2023-06-20 22:26:54.000000 plemmy-0.2.0/plemmy.egg-info/requires.txt
--rw-r--r--   0 tjkessler   (501) staff       (20)        7 2023-06-20 22:26:54.000000 plemmy-0.2.0/plemmy.egg-info/top_level.txt
--rw-r--r--   0 tjkessler   (501) staff       (20)       38 2023-06-20 22:26:54.350320 plemmy-0.2.0/setup.cfg
--rw-r--r--   0 tjkessler   (501) staff       (20)      878 2023-06-20 19:47:16.000000 plemmy-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 05:08:33.829477 plemmy-0.2.1/
+-rw-rw-rw-   0        0        0    11367 2023-06-20 00:43:37.000000 plemmy-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     2048 2023-06-21 05:08:33.829477 plemmy-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1675 2023-06-21 04:32:59.000000 plemmy-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-21 05:08:33.804471 plemmy-0.2.1/plemmy/
+-rw-rw-rw-   0        0        0      140 2023-06-20 00:36:09.000000 plemmy-0.2.1/plemmy/__init__.py
+-rw-rw-rw-   0        0        0    30133 2023-06-21 05:08:17.000000 plemmy-0.2.1/plemmy/lemmyhttp.py
+-rw-rw-rw-   0        0        0     1539 2023-06-21 05:08:17.000000 plemmy-0.2.1/plemmy/utils.py
+-rw-rw-rw-   0        0        0      120 2023-06-21 05:08:17.000000 plemmy-0.2.1/plemmy/version.py
+drwxrwxrwx   0        0        0        0 2023-06-21 05:08:33.828477 plemmy-0.2.1/plemmy.egg-info/
+-rw-rw-rw-   0        0        0     2048 2023-06-21 05:08:33.000000 plemmy-0.2.1/plemmy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2023-06-21 05:08:33.000000 plemmy-0.2.1/plemmy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 05:08:33.000000 plemmy-0.2.1/plemmy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-21 05:08:33.000000 plemmy-0.2.1/plemmy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       17 2023-06-21 05:08:33.000000 plemmy-0.2.1/plemmy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-21 05:08:33.000000 plemmy-0.2.1/plemmy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 05:08:33.829477 plemmy-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      878 2023-06-20 00:48:06.000000 plemmy-0.2.1/setup.py
```

### Comparing `plemmy-0.2.0/LICENSE` & `plemmy-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `plemmy-0.2.0/PKG-INFO` & `plemmy-0.2.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: plemmy
-Version: 0.2.0
-Summary: Python API for LemmyHttp
-Home-page: https://github.com/tjkessler/plemmy
-Author: Travis Kessler
-Author-email: travis.j.kessler@gmail.com
-License: Apache License 2.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Plemmy: a Python package for accessing the Lemmy API
 
 <img src="img/plemmy.png" alt="drawing" width="325"/>
 
 [![GitHub version](https://badge.fury.io/gh/tjkessler%2Fplemmy.svg)](https://badge.fury.io/gh/tjkessler%2Fplemmy)
 [![PyPI version](https://badge.fury.io/py/plemmy.svg)](https://badge.fury.io/py/plemmy)
 [![GitHub license](https://img.shields.io/badge/license-Apache-blue.svg)](https://raw.githubusercontent.com/tjkessler/plemmy/master/LICENSE.txt)
```

### Comparing `plemmy-0.2.0/README.md` & `plemmy-0.2.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,67 @@
-# Plemmy: a Python package for accessing the Lemmy API
-
-<img src="img/plemmy.png" alt="drawing" width="325"/>
-
-[![GitHub version](https://badge.fury.io/gh/tjkessler%2Fplemmy.svg)](https://badge.fury.io/gh/tjkessler%2Fplemmy)
-[![PyPI version](https://badge.fury.io/py/plemmy.svg)](https://badge.fury.io/py/plemmy)
-[![GitHub license](https://img.shields.io/badge/license-Apache-blue.svg)](https://raw.githubusercontent.com/tjkessler/plemmy/master/LICENSE.txt)
-
-Plemmy allows you to interact with any Lemmy instance using Python and the [LemmyHttp API](https://join-lemmy.org/api/classes/LemmyHttp.html).
-
-**WARNING:** Plemmy is still in development and needs testing!
-
-## Installation ##
-
-For the most up-to-date version of Plemmy, clone and install from the repository:
-
-```
-git clone https://github.com/tjkessler/plemmy
-cd plemmy
-python setup.py install
-```
-
-A PyPI repository is periodically updated:
-
-```
-pip install plemmy
-```
-
-## Basic usage ##
-
-Interact with a Lemmy instance using the _LemmyHttp_ object:
-
-```python
-from plemmy import LemmyHttp
-
-# create object for Lemmy.ml
-srv = LemmyHttp("https://lemmy.ml")
-
-# log in to Lemmy.ml
-srv.login("<username_or_email>", "<password>")
-
-# make a comment
-srv.create_comment("Hello from plemmy!", post_id)
-
-# create a post
-srv.create_post(community_id, "New post's title", body="Body text", url="https://a.link.to.share")
-```
-
-Full documentation is on its way, but in the meantime check out our source code.
-
-## Reporting issues, making contributions, etc. ##
-
-Don't hesitate to report a bug or unexpected results! Want to contribute? Make a pull request. Contact [@tjkessler](https://github.com/tjkessler) with any questions.
+Metadata-Version: 2.1
+Name: plemmy
+Version: 0.2.1
+Summary: Python API for LemmyHttp
+Home-page: https://github.com/tjkessler/plemmy
+Author: Travis Kessler
+Author-email: travis.j.kessler@gmail.com
+License: Apache License 2.0
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Plemmy: a Python package for accessing the Lemmy API
+
+<img src="img/plemmy.png" alt="drawing" width="325"/>
+
+[![GitHub version](https://badge.fury.io/gh/tjkessler%2Fplemmy.svg)](https://badge.fury.io/gh/tjkessler%2Fplemmy)
+[![PyPI version](https://badge.fury.io/py/plemmy.svg)](https://badge.fury.io/py/plemmy)
+[![GitHub license](https://img.shields.io/badge/license-Apache-blue.svg)](https://raw.githubusercontent.com/tjkessler/plemmy/master/LICENSE.txt)
+
+Plemmy allows you to interact with any Lemmy instance using Python and the [LemmyHttp API](https://join-lemmy.org/api/classes/LemmyHttp.html).
+
+**WARNING:** Plemmy is still in development and needs testing!
+
+## Installation ##
+
+For the most up-to-date version of Plemmy, clone and install from the repository:
+
+```
+git clone https://github.com/tjkessler/plemmy
+cd plemmy
+python setup.py install
+```
+
+A PyPI repository is periodically updated:
+
+```
+pip install plemmy
+```
+
+## Basic usage ##
+
+Interact with a Lemmy instance using the _LemmyHttp_ object:
+
+```python
+from plemmy import LemmyHttp
+
+# create object for Lemmy.ml
+srv = LemmyHttp("https://lemmy.ml")
+
+# log in to Lemmy.ml
+srv.login("<username_or_email>", "<password>")
+
+# make a comment
+srv.create_comment("Hello from plemmy!", post_id)
+
+# create a post
+srv.create_post(community_id, "New post's title", body="Body text", url="https://a.link.to.share")
+```
+
+Full documentation is on its way, but in the meantime check out our source code.
+
+## Reporting issues, making contributions, etc. ##
+
+Don't hesitate to report a bug or unexpected results! Want to contribute? Make a pull request. Contact [@tjkessler](https://github.com/tjkessler) with any questions.
+
+
```

### Comparing `plemmy-0.2.0/plemmy/utils.py` & `plemmy-0.2.1/plemmy/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -35,7 +35,13 @@
         re = requests.get(url, headers=headers, json=json)
         logger.debug(f"Code: {re.status_code}")
     except requests.exceptions.RequestException as ex:
         logger.error(f"GET error: {ex}\n\nURL: {url}" +
                      f"\nheaders: {headers}\njson: {json}")
         return None
     return re
+
+
+def create_form(arguments: dict) -> dict:
+
+    return {k: v for k, v in arguments.items()
+            if v is not None and k != "self"}
```

### Comparing `plemmy-0.2.0/plemmy.egg-info/PKG-INFO` & `plemmy-0.2.1/plemmy.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,64 +1,67 @@
-Metadata-Version: 2.1
-Name: plemmy
-Version: 0.2.0
-Summary: Python API for LemmyHttp
-Home-page: https://github.com/tjkessler/plemmy
-Author: Travis Kessler
-Author-email: travis.j.kessler@gmail.com
-License: Apache License 2.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Plemmy: a Python package for accessing the Lemmy API
-
-<img src="img/plemmy.png" alt="drawing" width="325"/>
-
-[![GitHub version](https://badge.fury.io/gh/tjkessler%2Fplemmy.svg)](https://badge.fury.io/gh/tjkessler%2Fplemmy)
-[![PyPI version](https://badge.fury.io/py/plemmy.svg)](https://badge.fury.io/py/plemmy)
-[![GitHub license](https://img.shields.io/badge/license-Apache-blue.svg)](https://raw.githubusercontent.com/tjkessler/plemmy/master/LICENSE.txt)
-
-Plemmy allows you to interact with any Lemmy instance using Python and the [LemmyHttp API](https://join-lemmy.org/api/classes/LemmyHttp.html).
-
-**WARNING:** Plemmy is still in development and needs testing!
-
-## Installation ##
-
-For the most up-to-date version of Plemmy, clone and install from the repository:
-
-```
-git clone https://github.com/tjkessler/plemmy
-cd plemmy
-python setup.py install
-```
-
-A PyPI repository is periodically updated:
-
-```
-pip install plemmy
-```
-
-## Basic usage ##
-
-Interact with a Lemmy instance using the _LemmyHttp_ object:
-
-```python
-from plemmy import LemmyHttp
-
-# create object for Lemmy.ml
-srv = LemmyHttp("https://lemmy.ml")
-
-# log in to Lemmy.ml
-srv.login("<username_or_email>", "<password>")
-
-# make a comment
-srv.create_comment("Hello from plemmy!", post_id)
-
-# create a post
-srv.create_post(community_id, "New post's title", body="Body text", url="https://a.link.to.share")
-```
-
-Full documentation is on its way, but in the meantime check out our source code.
-
-## Reporting issues, making contributions, etc. ##
-
-Don't hesitate to report a bug or unexpected results! Want to contribute? Make a pull request. Contact [@tjkessler](https://github.com/tjkessler) with any questions.
+Metadata-Version: 2.1
+Name: plemmy
+Version: 0.2.1
+Summary: Python API for LemmyHttp
+Home-page: https://github.com/tjkessler/plemmy
+Author: Travis Kessler
+Author-email: travis.j.kessler@gmail.com
+License: Apache License 2.0
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Plemmy: a Python package for accessing the Lemmy API
+
+<img src="img/plemmy.png" alt="drawing" width="325"/>
+
+[![GitHub version](https://badge.fury.io/gh/tjkessler%2Fplemmy.svg)](https://badge.fury.io/gh/tjkessler%2Fplemmy)
+[![PyPI version](https://badge.fury.io/py/plemmy.svg)](https://badge.fury.io/py/plemmy)
+[![GitHub license](https://img.shields.io/badge/license-Apache-blue.svg)](https://raw.githubusercontent.com/tjkessler/plemmy/master/LICENSE.txt)
+
+Plemmy allows you to interact with any Lemmy instance using Python and the [LemmyHttp API](https://join-lemmy.org/api/classes/LemmyHttp.html).
+
+**WARNING:** Plemmy is still in development and needs testing!
+
+## Installation ##
+
+For the most up-to-date version of Plemmy, clone and install from the repository:
+
+```
+git clone https://github.com/tjkessler/plemmy
+cd plemmy
+python setup.py install
+```
+
+A PyPI repository is periodically updated:
+
+```
+pip install plemmy
+```
+
+## Basic usage ##
+
+Interact with a Lemmy instance using the _LemmyHttp_ object:
+
+```python
+from plemmy import LemmyHttp
+
+# create object for Lemmy.ml
+srv = LemmyHttp("https://lemmy.ml")
+
+# log in to Lemmy.ml
+srv.login("<username_or_email>", "<password>")
+
+# make a comment
+srv.create_comment("Hello from plemmy!", post_id)
+
+# create a post
+srv.create_post(community_id, "New post's title", body="Body text", url="https://a.link.to.share")
+```
+
+Full documentation is on its way, but in the meantime check out our source code.
+
+## Reporting issues, making contributions, etc. ##
+
+Don't hesitate to report a bug or unexpected results! Want to contribute? Make a pull request. Contact [@tjkessler](https://github.com/tjkessler) with any questions.
+
+
```

### Comparing `plemmy-0.2.0/setup.py` & `plemmy-0.2.1/setup.py`

 * *Files identical despite different names*

