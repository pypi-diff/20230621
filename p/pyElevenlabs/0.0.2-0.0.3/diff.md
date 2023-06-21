# Comparing `tmp/pyElevenlabs-0.0.2.tar.gz` & `tmp/pyElevenlabs-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyElevenlabs-0.0.2.tar", last modified: Fri Feb 10 13:26:22 2023, max compression
+gzip compressed data, was "pyElevenlabs-0.0.3.tar", last modified: Wed Jun 21 19:14:30 2023, max compression
```

## Comparing `pyElevenlabs-0.0.2.tar` & `pyElevenlabs-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-02-10 13:26:22.516634 pyElevenlabs-0.0.2/
--rw-rw-rw-   0        0        0     1088 2023-02-10 12:17:21.000000 pyElevenlabs-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1102 2023-02-10 13:26:22.514634 pyElevenlabs-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      560 2023-02-10 12:26:24.000000 pyElevenlabs-0.0.2/README.md
--rw-rw-rw-   0        0        0      609 2023-02-10 13:25:33.000000 pyElevenlabs-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-10 13:26:22.517633 pyElevenlabs-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-02-10 13:26:22.346641 pyElevenlabs-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-02-10 13:26:22.421632 pyElevenlabs-0.0.2/src/pyElevenlabs/
--rw-rw-rw-   0        0        0        0 2023-02-10 11:44:02.000000 pyElevenlabs-0.0.2/src/pyElevenlabs/__init__.py
--rw-rw-rw-   0        0        0      507 2023-02-10 13:25:29.000000 pyElevenlabs-0.0.2/src/pyElevenlabs/pyElevenlabs.py
--rw-rw-rw-   0        0        0      382 2023-02-10 12:20:26.000000 pyElevenlabs-0.0.2/src/pyElevenlabs/test.py
-drwxrwxrwx   0        0        0        0 2023-02-10 13:26:22.503641 pyElevenlabs-0.0.2/src/pyElevenlabs.egg-info/
--rw-rw-rw-   0        0        0     1102 2023-02-10 13:26:22.000000 pyElevenlabs-0.0.2/src/pyElevenlabs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-02-10 13:26:22.000000 pyElevenlabs-0.0.2/src/pyElevenlabs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-10 13:26:22.000000 pyElevenlabs-0.0.2/src/pyElevenlabs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-02-10 13:26:22.000000 pyElevenlabs-0.0.2/src/pyElevenlabs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:14:30.128648 pyElevenlabs-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-21 19:14:19.000000 pyElevenlabs-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-21 19:14:30.128648 pyElevenlabs-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-21 19:14:19.000000 pyElevenlabs-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-21 19:14:19.000000 pyElevenlabs-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 19:14:30.128648 pyElevenlabs-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:14:30.128648 pyElevenlabs-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:14:30.128648 pyElevenlabs-0.0.3/src/pyElevenlabs/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-21 19:14:19.000000 pyElevenlabs-0.0.3/src/pyElevenlabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-21 19:14:19.000000 pyElevenlabs-0.0.3/src/pyElevenlabs/pyElevenlabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-21 19:14:19.000000 pyElevenlabs-0.0.3/src/pyElevenlabs/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:14:30.128648 pyElevenlabs-0.0.3/src/pyElevenlabs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-21 19:14:30.000000 pyElevenlabs-0.0.3/src/pyElevenlabs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-21 19:14:30.000000 pyElevenlabs-0.0.3/src/pyElevenlabs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 19:14:30.000000 pyElevenlabs-0.0.3/src/pyElevenlabs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-21 19:14:30.000000 pyElevenlabs-0.0.3/src/pyElevenlabs.egg-info/top_level.txt
```

### Comparing `pyElevenlabs-0.0.2/LICENSE` & `pyElevenlabs-0.0.3/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) [year] [fullname]
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) [year] [fullname]
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `pyElevenlabs-0.0.2/PKG-INFO` & `pyElevenlabs-0.0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1
-Name: pyElevenlabs
-Version: 0.0.2
-Summary: Python wrapper for the ElevenLabs API
-Author-email: Philip Lawall <philip@lawall.me>
-Project-URL: Homepage, https://github.com/philiplawall/pyElevenLabs
-Project-URL: Bug Tracker, https://github.com/philiplawall/pyElevenLabs/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Python wrapper for Elevenlabs API
-
-This is a python wrapper for the Elevenlabs API ([LINK](https://beta.elevenlabs.io/))
-
-Currently only supports calling the text-to-speech endpoint.
-Needs a api_key and voice_id to work. Api Key is available in your Profile. Voice Id is available [here](https://api.elevenlabs.io/v1/voices).
-
----
-
-This package and repository is no way affiliated with Elevenlabs. Please ssend all support requests related to this python package to this Issue Tracker: [Issues](https://github.com/philiplawall/pyElevenlabs/issues)
+Metadata-Version: 2.1
+Name: pyElevenlabs
+Version: 0.0.3
+Summary: Python wrapper for the ElevenLabs API
+Author-email: Philip Lawall <philip@lawall.me>
+Project-URL: Homepage, https://github.com/philiplawall/pyElevenLabs
+Project-URL: Bug Tracker, https://github.com/philiplawall/pyElevenLabs/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Python wrapper for Elevenlabs API
+
+This is a python wrapper for the Elevenlabs API ([LINK](https://beta.elevenlabs.io/))
+
+Currently only supports calling the text-to-speech endpoint.
+Needs a api_key and voice_id to work. Api Key is available in your Profile. Voice Id is available [here](https://api.elevenlabs.io/v1/voices).
+
+---
+
+This package and repository is no way affiliated with Elevenlabs. Please ssend all support requests related to this python package to this Issue Tracker: [Issues](https://github.com/philiplawall/pyElevenlabs/issues)
```

### Comparing `pyElevenlabs-0.0.2/README.md` & `pyElevenlabs-0.0.3/README.md`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# Python wrapper for Elevenlabs API
-
-This is a python wrapper for the Elevenlabs API ([LINK](https://beta.elevenlabs.io/))
-
-Currently only supports calling the text-to-speech endpoint.
-Needs a api_key and voice_id to work. Api Key is available in your Profile. Voice Id is available [here](https://api.elevenlabs.io/v1/voices).
-
----
-
-This package and repository is no way affiliated with Elevenlabs. Please ssend all support requests related to this python package to this Issue Tracker: [Issues](https://github.com/philiplawall/pyElevenlabs/issues)
+# Python wrapper for Elevenlabs API
+
+This is a python wrapper for the Elevenlabs API ([LINK](https://beta.elevenlabs.io/))
+
+Currently only supports calling the text-to-speech endpoint.
+Needs a api_key and voice_id to work. Api Key is available in your Profile. Voice Id is available [here](https://api.elevenlabs.io/v1/voices).
+
+---
+
+This package and repository is no way affiliated with Elevenlabs. Please ssend all support requests related to this python package to this Issue Tracker: [Issues](https://github.com/philiplawall/pyElevenlabs/issues)
```

### Comparing `pyElevenlabs-0.0.2/pyproject.toml` & `pyElevenlabs-0.0.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-[build-system]
-requires = ["setuptools"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "pyElevenlabs"
-version = "0.0.2"
-authors = [
-  { name="Philip Lawall", email="philip@lawall.me" }
-]
-description = "Python wrapper for the ElevenLabs API"
-readme = "README.md"
-requires-python = ">=3.6"
-classifiers = [
-  "Programming Language :: Python :: 3",
-  "License :: OSI Approved :: MIT License",
-  "Operating System :: OS Independent",
-]
-
-[project.urls]
-"Homepage" = "https://github.com/philiplawall/pyElevenLabs"
-"Bug Tracker" = "https://github.com/philiplawall/pyElevenLabs/issues"
+[build-system]
+requires = ["setuptools"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "pyElevenlabs"
+version = "0.0.3"
+authors = [
+  { name="Philip Lawall", email="philip@lawall.me" }
+]
+description = "Python wrapper for the ElevenLabs API"
+readme = "README.md"
+requires-python = ">=3.6"
+classifiers = [
+  "Programming Language :: Python :: 3",
+  "License :: OSI Approved :: MIT License",
+  "Operating System :: OS Independent",
+]
+
+[project.urls]
+"Homepage" = "https://github.com/philiplawall/pyElevenLabs"
+"Bug Tracker" = "https://github.com/philiplawall/pyElevenLabs/issues"
```

### Comparing `pyElevenlabs-0.0.2/src/pyElevenlabs.egg-info/PKG-INFO` & `pyElevenlabs-0.0.3/src/pyElevenlabs.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1
-Name: pyElevenlabs
-Version: 0.0.2
-Summary: Python wrapper for the ElevenLabs API
-Author-email: Philip Lawall <philip@lawall.me>
-Project-URL: Homepage, https://github.com/philiplawall/pyElevenLabs
-Project-URL: Bug Tracker, https://github.com/philiplawall/pyElevenLabs/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Python wrapper for Elevenlabs API
-
-This is a python wrapper for the Elevenlabs API ([LINK](https://beta.elevenlabs.io/))
-
-Currently only supports calling the text-to-speech endpoint.
-Needs a api_key and voice_id to work. Api Key is available in your Profile. Voice Id is available [here](https://api.elevenlabs.io/v1/voices).
-
----
-
-This package and repository is no way affiliated with Elevenlabs. Please ssend all support requests related to this python package to this Issue Tracker: [Issues](https://github.com/philiplawall/pyElevenlabs/issues)
+Metadata-Version: 2.1
+Name: pyElevenlabs
+Version: 0.0.3
+Summary: Python wrapper for the ElevenLabs API
+Author-email: Philip Lawall <philip@lawall.me>
+Project-URL: Homepage, https://github.com/philiplawall/pyElevenLabs
+Project-URL: Bug Tracker, https://github.com/philiplawall/pyElevenLabs/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Python wrapper for Elevenlabs API
+
+This is a python wrapper for the Elevenlabs API ([LINK](https://beta.elevenlabs.io/))
+
+Currently only supports calling the text-to-speech endpoint.
+Needs a api_key and voice_id to work. Api Key is available in your Profile. Voice Id is available [here](https://api.elevenlabs.io/v1/voices).
+
+---
+
+This package and repository is no way affiliated with Elevenlabs. Please ssend all support requests related to this python package to this Issue Tracker: [Issues](https://github.com/philiplawall/pyElevenlabs/issues)
```

