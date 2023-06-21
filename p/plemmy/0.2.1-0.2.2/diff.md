# Comparing `tmp/plemmy-0.2.1.tar.gz` & `tmp/plemmy-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plemmy-0.2.1.tar", last modified: Wed Jun 21 05:08:33 2023, max compression
+gzip compressed data, was "plemmy-0.2.2.tar", last modified: Wed Jun 21 17:46:16 2023, max compression
```

## Comparing `plemmy-0.2.1.tar` & `plemmy-0.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 05:08:33.829477 plemmy-0.2.1/
--rw-rw-rw-   0        0        0    11367 2023-06-20 00:43:37.000000 plemmy-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     2048 2023-06-21 05:08:33.829477 plemmy-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1675 2023-06-21 04:32:59.000000 plemmy-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-21 05:08:33.804471 plemmy-0.2.1/plemmy/
--rw-rw-rw-   0        0        0      140 2023-06-20 00:36:09.000000 plemmy-0.2.1/plemmy/__init__.py
--rw-rw-rw-   0        0        0    30133 2023-06-21 05:08:17.000000 plemmy-0.2.1/plemmy/lemmyhttp.py
--rw-rw-rw-   0        0        0     1539 2023-06-21 05:08:17.000000 plemmy-0.2.1/plemmy/utils.py
--rw-rw-rw-   0        0        0      120 2023-06-21 05:08:17.000000 plemmy-0.2.1/plemmy/version.py
-drwxrwxrwx   0        0        0        0 2023-06-21 05:08:33.828477 plemmy-0.2.1/plemmy.egg-info/
--rw-rw-rw-   0        0        0     2048 2023-06-21 05:08:33.000000 plemmy-0.2.1/plemmy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2023-06-21 05:08:33.000000 plemmy-0.2.1/plemmy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 05:08:33.000000 plemmy-0.2.1/plemmy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-21 05:08:33.000000 plemmy-0.2.1/plemmy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       17 2023-06-21 05:08:33.000000 plemmy-0.2.1/plemmy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-21 05:08:33.000000 plemmy-0.2.1/plemmy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-21 05:08:33.829477 plemmy-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      878 2023-06-20 00:48:06.000000 plemmy-0.2.1/setup.py
+drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-06-21 17:46:16.201411 plemmy-0.2.2/
+-rw-r--r--   0 tjkessler   (501) staff       (20)    11367 2023-06-20 19:47:16.000000 plemmy-0.2.2/LICENSE
+-rw-r--r--   0 tjkessler   (501) staff       (20)     1961 2023-06-21 17:46:16.201255 plemmy-0.2.2/PKG-INFO
+-rw-r--r--   0 tjkessler   (501) staff       (20)     1675 2023-06-20 22:25:52.000000 plemmy-0.2.2/README.md
+drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-06-21 17:46:16.200144 plemmy-0.2.2/plemmy/
+-rw-r--r--   0 tjkessler   (501) staff       (20)      140 2023-06-20 19:47:16.000000 plemmy-0.2.2/plemmy/__init__.py
+-rw-r--r--   0 tjkessler   (501) staff       (20)    30174 2023-06-21 17:41:59.000000 plemmy-0.2.2/plemmy/lemmyhttp.py
+-rw-r--r--   0 tjkessler   (501) staff       (20)     1592 2023-06-21 17:42:05.000000 plemmy-0.2.2/plemmy/utils.py
+-rw-r--r--   0 tjkessler   (501) staff       (20)      120 2023-06-21 17:41:42.000000 plemmy-0.2.2/plemmy/version.py
+drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-06-21 17:46:16.201024 plemmy-0.2.2/plemmy.egg-info/
+-rw-r--r--   0 tjkessler   (501) staff       (20)     1961 2023-06-21 17:46:16.000000 plemmy-0.2.2/plemmy.egg-info/PKG-INFO
+-rw-r--r--   0 tjkessler   (501) staff       (20)      277 2023-06-21 17:46:16.000000 plemmy-0.2.2/plemmy.egg-info/SOURCES.txt
+-rw-r--r--   0 tjkessler   (501) staff       (20)        1 2023-06-21 17:46:16.000000 plemmy-0.2.2/plemmy.egg-info/dependency_links.txt
+-rw-r--r--   0 tjkessler   (501) staff       (20)        1 2023-06-21 17:46:16.000000 plemmy-0.2.2/plemmy.egg-info/not-zip-safe
+-rw-r--r--   0 tjkessler   (501) staff       (20)       17 2023-06-21 17:46:16.000000 plemmy-0.2.2/plemmy.egg-info/requires.txt
+-rw-r--r--   0 tjkessler   (501) staff       (20)        7 2023-06-21 17:46:16.000000 plemmy-0.2.2/plemmy.egg-info/top_level.txt
+-rw-r--r--   0 tjkessler   (501) staff       (20)       38 2023-06-21 17:46:16.201457 plemmy-0.2.2/setup.cfg
+-rw-r--r--   0 tjkessler   (501) staff       (20)      878 2023-06-20 19:47:16.000000 plemmy-0.2.2/setup.py
```

### Comparing `plemmy-0.2.1/LICENSE` & `plemmy-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `plemmy-0.2.1/PKG-INFO` & `plemmy-0.2.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,67 +1,53 @@
-Metadata-Version: 2.1
-Name: plemmy
-Version: 0.2.1
-Summary: Python API for LemmyHttp
-Home-page: https://github.com/tjkessler/plemmy
-Author: Travis Kessler
-Author-email: travis.j.kessler@gmail.com
-License: Apache License 2.0
-Platform: UNKNOWN
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
-
-
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
```

### Comparing `plemmy-0.2.1/README.md` & `plemmy-0.2.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: plemmy
+Version: 0.2.2
+Summary: Python API for LemmyHttp
+Home-page: https://github.com/tjkessler/plemmy
+Author: Travis Kessler
+Author-email: travis.j.kessler@gmail.com
+License: Apache License 2.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Plemmy: a Python package for accessing the Lemmy API
 
 <img src="img/plemmy.png" alt="drawing" width="325"/>
 
 [![GitHub version](https://badge.fury.io/gh/tjkessler%2Fplemmy.svg)](https://badge.fury.io/gh/tjkessler%2Fplemmy)
 [![PyPI version](https://badge.fury.io/py/plemmy.svg)](https://badge.fury.io/py/plemmy)
 [![GitHub license](https://img.shields.io/badge/license-Apache-blue.svg)](https://raw.githubusercontent.com/tjkessler/plemmy/master/LICENSE.txt)
```

### Comparing `plemmy-0.2.1/plemmy/lemmyhttp.py` & `plemmy-0.2.2/plemmy/lemmyhttp.py`

 * *Files 0% similar despite different names*

```diff
@@ -331,15 +331,16 @@
                            self._headers, form)
 
     def get_community(self, id: int = None,
                       name: str = None) -> requests.Response:
 
         form = create_form(locals())
         form["auth"] = self.key
-        return get_handler(f"{self._api_url}/community", self._headers, form)
+        return get_handler(f"{self._api_url}/community", self._headers,
+                           None, params=form)
 
     def get_modlog(self, type_: str, community_id: int = None,
                    limit: int = None, mod_person_id: int = None,
                    other_person_id: int = None,
                    page: int = None) -> requests.Response:
 
         form = create_form(locals())
```

### Comparing `plemmy-0.2.1/plemmy/utils.py` & `plemmy-0.2.2/plemmy/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,19 +24,20 @@
     except requests.exceptions.RequestException as ex:
         logger.error(f"PUT error: {ex}\n\nURL: {url}" +
                      f"\nheaders: {headers}\njson: {json}")
         return None
     return re
 
 
-def get_handler(url: str, headers: dict, json: dict) -> requests.Response:
+def get_handler(url: str, headers: dict, json: dict,
+                params: dict = None) -> requests.Response:
 
     logger = logging.getLogger(__name__)
     try:
-        re = requests.get(url, headers=headers, json=json)
+        re = requests.get(url, headers=headers, json=json, params=params)
         logger.debug(f"Code: {re.status_code}")
     except requests.exceptions.RequestException as ex:
         logger.error(f"GET error: {ex}\n\nURL: {url}" +
                      f"\nheaders: {headers}\njson: {json}")
         return None
     return re
```

### Comparing `plemmy-0.2.1/plemmy.egg-info/PKG-INFO` & `plemmy-0.2.2/plemmy.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,64 @@
-Metadata-Version: 2.1
-Name: plemmy
-Version: 0.2.1
-Summary: Python API for LemmyHttp
-Home-page: https://github.com/tjkessler/plemmy
-Author: Travis Kessler
-Author-email: travis.j.kessler@gmail.com
-License: Apache License 2.0
-Platform: UNKNOWN
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
-
-
+Metadata-Version: 2.1
+Name: plemmy
+Version: 0.2.2
+Summary: Python API for LemmyHttp
+Home-page: https://github.com/tjkessler/plemmy
+Author: Travis Kessler
+Author-email: travis.j.kessler@gmail.com
+License: Apache License 2.0
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
```

### Comparing `plemmy-0.2.1/setup.py` & `plemmy-0.2.2/setup.py`

 * *Files identical despite different names*

