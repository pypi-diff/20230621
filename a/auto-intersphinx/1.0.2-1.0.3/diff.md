# Comparing `tmp/auto-intersphinx-1.0.2.tar.gz` & `tmp/auto-intersphinx-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-intersphinx-1.0.2.tar", last modified: Tue Feb 28 17:56:07 2023, max compression
+gzip compressed data, was "auto-intersphinx-1.0.3.tar", last modified: Wed Jun 21 17:18:04 2023, max compression
```

## Comparing `auto-intersphinx-1.0.2.tar` & `auto-intersphinx-1.0.3.tar`

### file list

```diff
@@ -1,43 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 17:56:07.628673 auto-intersphinx-1.0.2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 17:56:07.620673 auto-intersphinx-1.0.2/LICENSES/
--rw-rw-rw-   0 root         (0) root         (0)     1459 2023-02-10 16:38:45.000000 auto-intersphinx-1.0.2/LICENSES/BSD-3-Clause.txt
--rw-rw-rw-   0 root         (0) root         (0)      271 2023-02-11 14:40:40.000000 auto-intersphinx-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2184 2023-02-28 17:56:07.628673 auto-intersphinx-1.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1193 2023-02-28 17:53:15.000000 auto-intersphinx-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 17:56:07.624673 auto-intersphinx-1.0.2/doc/
--rw-rw-rw-   0 root         (0) root         (0)      393 2023-02-10 16:38:45.000000 auto-intersphinx-1.0.2/doc/api.rst
--rw-rw-rw-   0 root         (0) root         (0)     1442 2023-02-10 16:38:45.000000 auto-intersphinx-1.0.2/doc/cli.rst
--rw-rw-rw-   0 root         (0) root         (0)      800 2023-02-10 16:38:45.000000 auto-intersphinx-1.0.2/doc/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      881 2023-02-28 17:39:45.000000 auto-intersphinx-1.0.2/doc/install.rst
--rw-rw-rw-   0 root         (0) root         (0)      786 2023-02-10 16:38:45.000000 auto-intersphinx-1.0.2/doc/links.rst
--rw-rw-rw-   0 root         (0) root         (0)    11995 2023-02-10 16:38:45.000000 auto-intersphinx-1.0.2/doc/usage.rst
--rw-rw-rw-   0 root         (0) root         (0)     2016 2023-02-28 17:53:15.000000 auto-intersphinx-1.0.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-28 17:56:07.628673 auto-intersphinx-1.0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      169 2023-02-10 16:38:45.000000 auto-intersphinx-1.0.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 17:56:07.620673 auto-intersphinx-1.0.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 17:56:07.624673 auto-intersphinx-1.0.2/src/auto_intersphinx/
--rw-rw-rw-   0 root         (0) root         (0)    11585 2023-02-10 16:42:55.000000 auto-intersphinx-1.0.2/src/auto_intersphinx/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    40034 2023-02-16 09:08:24.000000 auto-intersphinx-1.0.2/src/auto_intersphinx/catalog.json
--rw-rw-rw-   0 root         (0) root         (0)    24725 2023-02-10 16:42:55.000000 auto-intersphinx-1.0.2/src/auto_intersphinx/catalog.py
--rw-rw-rw-   0 root         (0) root         (0)     6304 2023-02-10 16:42:55.000000 auto-intersphinx-1.0.2/src/auto_intersphinx/check_packages.py
--rw-rw-rw-   0 root         (0) root         (0)      900 2023-02-10 16:42:55.000000 auto-intersphinx-1.0.2/src/auto_intersphinx/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1930 2023-02-10 16:42:55.000000 auto-intersphinx-1.0.2/src/auto_intersphinx/dump_objects.py
--rw-rw-rw-   0 root         (0) root         (0)     6438 2023-02-16 13:01:18.000000 auto-intersphinx-1.0.2/src/auto_intersphinx/update_catalog.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 17:56:07.624673 auto-intersphinx-1.0.2/src/auto_intersphinx.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2184 2023-02-28 17:56:07.000000 auto-intersphinx-1.0.2/src/auto_intersphinx.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      904 2023-02-28 17:56:07.000000 auto-intersphinx-1.0.2/src/auto_intersphinx.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-28 17:56:07.000000 auto-intersphinx-1.0.2/src/auto_intersphinx.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-02-28 17:56:07.000000 auto-intersphinx-1.0.2/src/auto_intersphinx.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      180 2023-02-28 17:56:07.000000 auto-intersphinx-1.0.2/src/auto_intersphinx.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-02-28 17:56:07.000000 auto-intersphinx-1.0.2/src/auto_intersphinx.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-28 17:56:07.000000 auto-intersphinx-1.0.2/src/auto_intersphinx.egg-info/zip-safe
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 17:56:07.628673 auto-intersphinx-1.0.2/tests/
--rw-rw-rw-   0 root         (0) root         (0)      177 2023-02-10 16:38:45.000000 auto-intersphinx-1.0.2/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      354 2023-02-10 16:42:55.000000 auto-intersphinx-1.0.2/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 17:56:07.628673 auto-intersphinx-1.0.2/tests/data/
--rw-rw-rw-   0 root         (0) root         (0)     1241 2023-02-10 16:38:45.000000 auto-intersphinx-1.0.2/tests/data/catalog.json
--rw-rw-rw-   0 root         (0) root         (0)      167 2023-02-10 16:38:45.000000 auto-intersphinx-1.0.2/tests/data/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     8318 2023-02-10 16:38:45.000000 auto-intersphinx-1.0.2/tests/test_auto_intersphinx.py
--rw-rw-rw-   0 root         (0) root         (0)     4675 2023-02-10 16:38:45.000000 auto-intersphinx-1.0.2/tests/test_check_packages.py
--rw-rw-rw-   0 root         (0) root         (0)      793 2023-02-10 16:38:45.000000 auto-intersphinx-1.0.2/tests/test_dump_objects.py
--rw-rw-rw-   0 root         (0) root         (0)     7718 2023-02-10 16:38:45.000000 auto-intersphinx-1.0.2/tests/test_update_catalog.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 17:18:04.359602 auto-intersphinx-1.0.3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 17:18:04.351602 auto-intersphinx-1.0.3/LICENSES/
+-rw-rw-rw-   0 root         (0) root         (0)     1459 2023-06-21 16:53:48.000000 auto-intersphinx-1.0.3/LICENSES/BSD-3-Clause.txt
+-rw-rw-rw-   0 root         (0) root         (0)      270 2023-06-21 16:53:48.000000 auto-intersphinx-1.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2184 2023-06-21 17:18:04.359602 auto-intersphinx-1.0.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1193 2023-06-21 17:13:08.000000 auto-intersphinx-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 17:18:04.355602 auto-intersphinx-1.0.3/doc/
+-rw-rw-rw-   0 root         (0) root         (0)      393 2023-06-21 16:53:48.000000 auto-intersphinx-1.0.3/doc/api.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1442 2023-06-21 16:53:48.000000 auto-intersphinx-1.0.3/doc/cli.rst
+-rw-rw-rw-   0 root         (0) root         (0)      800 2023-06-21 16:53:48.000000 auto-intersphinx-1.0.3/doc/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      881 2023-06-21 16:53:48.000000 auto-intersphinx-1.0.3/doc/install.rst
+-rw-rw-rw-   0 root         (0) root         (0)      786 2023-06-21 16:53:48.000000 auto-intersphinx-1.0.3/doc/links.rst
+-rw-rw-rw-   0 root         (0) root         (0)    11995 2023-06-21 16:53:48.000000 auto-intersphinx-1.0.3/doc/usage.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2016 2023-06-21 17:13:08.000000 auto-intersphinx-1.0.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-21 17:18:04.359602 auto-intersphinx-1.0.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      169 2023-06-21 16:53:48.000000 auto-intersphinx-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 17:18:04.351602 auto-intersphinx-1.0.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 17:18:04.355602 auto-intersphinx-1.0.3/src/auto_intersphinx/
+-rw-rw-rw-   0 root         (0) root         (0)    11585 2023-06-21 16:53:48.000000 auto-intersphinx-1.0.3/src/auto_intersphinx/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    40377 2023-06-21 16:53:48.000000 auto-intersphinx-1.0.3/src/auto_intersphinx/catalog.json
+-rw-rw-rw-   0 root         (0) root         (0)    24725 2023-06-21 16:53:48.000000 auto-intersphinx-1.0.3/src/auto_intersphinx/catalog.py
+-rw-rw-rw-   0 root         (0) root         (0)     6304 2023-06-21 16:53:48.000000 auto-intersphinx-1.0.3/src/auto_intersphinx/check_packages.py
+-rw-rw-rw-   0 root         (0) root         (0)      900 2023-06-21 16:53:48.000000 auto-intersphinx-1.0.3/src/auto_intersphinx/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1930 2023-06-21 16:53:48.000000 auto-intersphinx-1.0.3/src/auto_intersphinx/dump_objects.py
+-rw-rw-rw-   0 root         (0) root         (0)     6438 2023-06-21 16:53:48.000000 auto-intersphinx-1.0.3/src/auto_intersphinx/update_catalog.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 17:18:04.355602 auto-intersphinx-1.0.3/src/auto_intersphinx.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2184 2023-06-21 17:18:04.000000 auto-intersphinx-1.0.3/src/auto_intersphinx.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      886 2023-06-21 17:18:04.000000 auto-intersphinx-1.0.3/src/auto_intersphinx.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 17:18:04.000000 auto-intersphinx-1.0.3/src/auto_intersphinx.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-06-21 17:18:04.000000 auto-intersphinx-1.0.3/src/auto_intersphinx.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      180 2023-06-21 17:18:04.000000 auto-intersphinx-1.0.3/src/auto_intersphinx.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-06-21 17:18:04.000000 auto-intersphinx-1.0.3/src/auto_intersphinx.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 17:18:04.000000 auto-intersphinx-1.0.3/src/auto_intersphinx.egg-info/zip-safe
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 17:18:04.359602 auto-intersphinx-1.0.3/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      354 2023-06-21 16:53:48.000000 auto-intersphinx-1.0.3/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 17:18:04.359602 auto-intersphinx-1.0.3/tests/data/
+-rw-rw-rw-   0 root         (0) root         (0)     1241 2023-06-21 16:53:48.000000 auto-intersphinx-1.0.3/tests/data/catalog.json
+-rw-rw-rw-   0 root         (0) root         (0)      167 2023-06-21 16:53:48.000000 auto-intersphinx-1.0.3/tests/data/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     8318 2023-06-21 16:53:48.000000 auto-intersphinx-1.0.3/tests/test_auto_intersphinx.py
+-rw-rw-rw-   0 root         (0) root         (0)     4675 2023-06-21 16:53:48.000000 auto-intersphinx-1.0.3/tests/test_check_packages.py
+-rw-rw-rw-   0 root         (0) root         (0)      793 2023-06-21 16:53:48.000000 auto-intersphinx-1.0.3/tests/test_dump_objects.py
+-rw-rw-rw-   0 root         (0) root         (0)     7718 2023-06-21 16:53:48.000000 auto-intersphinx-1.0.3/tests/test_update_catalog.py
```

### Comparing `auto-intersphinx-1.0.2/LICENSES/BSD-3-Clause.txt` & `auto-intersphinx-1.0.3/LICENSES/BSD-3-Clause.txt`

 * *Files identical despite different names*

### Comparing `auto-intersphinx-1.0.2/PKG-INFO` & `auto-intersphinx-1.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: auto-intersphinx
-Version: 1.0.2
+Version: 1.0.3
 Summary: Automatic links direct project dependencies to the intersphinx catalog
 Author-email: Andre Anjos <andre.anjos@idiap.ch>
 License: BSD 3-Clause License
-Project-URL: documentation, https://auto-intersphinx.readthedocs.io/en/v1.0.2/
+Project-URL: documentation, https://auto-intersphinx.readthedocs.io/en/v1.0.3/
 Project-URL: homepage, https://pypi.org/project/auto-intersphinx
 Project-URL: repository, https://gitlab.idiap.ch/software/auto-intersphinx
 Project-URL: changelog, https://gitlab.idiap.ch/software/auto-intersphinx/-/releases
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -23,17 +23,17 @@
 
 <!--
 SPDX-FileCopyrightText: Copyright © 2022 Idiap Research Institute <contact@idiap.ch>
 
 SPDX-License-Identifier: BSD-3-Clause
 -->
 
-[![latest-docs](https://img.shields.io/badge/docs-v1.0.2-orange.svg)](https://auto-intersphinx.readthedocs.io/en/v1.0.2/)
-[![build](https://gitlab.idiap.ch/software/auto-intersphinx/badges/v1.0.2/pipeline.svg)](https://gitlab.idiap.ch/software/auto-intersphinx/commits/v1.0.2)
-[![coverage](https://gitlab.idiap.ch/software/auto-intersphinx/badges/v1.0.2/coverage.svg)](https://www.idiap.ch/software/biosignal/docs/software/auto-intersphinx/v1.0.2/coverage/index.html)
+[![latest-docs](https://img.shields.io/badge/docs-v1.0.3-orange.svg)](https://auto-intersphinx.readthedocs.io/en/v1.0.3/)
+[![build](https://gitlab.idiap.ch/software/auto-intersphinx/badges/v1.0.3/pipeline.svg)](https://gitlab.idiap.ch/software/auto-intersphinx/commits/v1.0.3)
+[![coverage](https://gitlab.idiap.ch/software/auto-intersphinx/badges/v1.0.3/coverage.svg)](https://www.idiap.ch/software/biosignal/docs/software/auto-intersphinx/v1.0.3/coverage/index.html)
 [![repository](https://img.shields.io/badge/gitlab-project-0000c0.svg)](https://gitlab.idiap.ch/software/auto-intersphinx)
 
 # Automatically Links Package Documentation from Their Names
 
 This package contains a [Sphinx](https://www.sphinx-doc.org/) plugin that can
 fill
 [intersphinx](https://www.sphinx-doc.org/en/main/usage/extensions/intersphinx.html)
```

### Comparing `auto-intersphinx-1.0.2/README.md` & `auto-intersphinx-1.0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
 SPDX-FileCopyrightText: Copyright © 2022 Idiap Research Institute <contact@idiap.ch>
 
 SPDX-License-Identifier: BSD-3-Clause
 -->
 
-[![latest-docs](https://img.shields.io/badge/docs-v1.0.2-orange.svg)](https://auto-intersphinx.readthedocs.io/en/v1.0.2/)
-[![build](https://gitlab.idiap.ch/software/auto-intersphinx/badges/v1.0.2/pipeline.svg)](https://gitlab.idiap.ch/software/auto-intersphinx/commits/v1.0.2)
-[![coverage](https://gitlab.idiap.ch/software/auto-intersphinx/badges/v1.0.2/coverage.svg)](https://www.idiap.ch/software/biosignal/docs/software/auto-intersphinx/v1.0.2/coverage/index.html)
+[![latest-docs](https://img.shields.io/badge/docs-v1.0.3-orange.svg)](https://auto-intersphinx.readthedocs.io/en/v1.0.3/)
+[![build](https://gitlab.idiap.ch/software/auto-intersphinx/badges/v1.0.3/pipeline.svg)](https://gitlab.idiap.ch/software/auto-intersphinx/commits/v1.0.3)
+[![coverage](https://gitlab.idiap.ch/software/auto-intersphinx/badges/v1.0.3/coverage.svg)](https://www.idiap.ch/software/biosignal/docs/software/auto-intersphinx/v1.0.3/coverage/index.html)
 [![repository](https://img.shields.io/badge/gitlab-project-0000c0.svg)](https://gitlab.idiap.ch/software/auto-intersphinx)
 
 # Automatically Links Package Documentation from Their Names
 
 This package contains a [Sphinx](https://www.sphinx-doc.org/) plugin that can
 fill
 [intersphinx](https://www.sphinx-doc.org/en/main/usage/extensions/intersphinx.html)
```

### Comparing `auto-intersphinx-1.0.2/doc/cli.rst` & `auto-intersphinx-1.0.3/doc/cli.rst`

 * *Files identical despite different names*

### Comparing `auto-intersphinx-1.0.2/doc/index.rst` & `auto-intersphinx-1.0.3/doc/index.rst`

 * *Files identical despite different names*

### Comparing `auto-intersphinx-1.0.2/doc/install.rst` & `auto-intersphinx-1.0.3/doc/install.rst`

 * *Files identical despite different names*

### Comparing `auto-intersphinx-1.0.2/doc/links.rst` & `auto-intersphinx-1.0.3/doc/links.rst`

 * *Files identical despite different names*

### Comparing `auto-intersphinx-1.0.2/doc/usage.rst` & `auto-intersphinx-1.0.3/doc/usage.rst`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 online searching for those cross-references.  Here is the rough algorithm,
 performed for each entry in the ``auto_intersphinx_packages`` list:
 
 1. If an intersphinx_ URL for the given package on the user catalog, that is
    used prioritarily, and the ``intersphinx_mapping`` for that package is
    filled and the algorithm continues with the next package.
 2. Else, we check the built-in catalog, distributed with auto-intersphinx.  If
-   an URL for teh package is found there, then we fill-in
+   an URL for the package is found there, then we fill-in
    ``intersphinx_mapping`` and continue.
 3. Else, we check the current Python environment, searching for the package
    metadata and attached documentation URLs the project may declare.  Many
    projects declare their Sphinx_ documents this way.  If an URL is found, it
    is checked for an ``objects.inv`` file existing there (not downloaded at
    this point), and if that exists, it added to the user catalog, allowing it
    to be added to the ``intersphinx_mapping``.  If successful, the algorithm
@@ -210,15 +210,15 @@
 ==================
 
 To update an existing catalog, use the command-line application
 :ref:`auto_intersphinx.cli.update_catalog`:
 
 .. code-block:: sh
 
-   auto-intersphinx-update-catalog -vvv --self --catalog=catalog.json
+   auto-intersphinx update-catalog -vvv --self --catalog=catalog.json
 
 This will read the current information available in the existing catalog, and
 will search the sources once more for updated information.  Naturally, packages
 with no sources (empty ``sources``) entries, will **not** be updated.
 
 
 Browsing for Documentation
@@ -226,15 +226,15 @@
 
 You may ask the command-line application
 :ref:`auto_intersphinx.cli.check_packages` to display where documentation
 information may be found for a package.  For example:
 
 .. code-block:: sh
 
-   $ auto-intersphinx-check-packages numpy
+   $ auto-intersphinx check-packages numpy
    Found numpy in builtin catalog:
    | {
    |   "latest": "https://numpy.org/devdocs/",
    |   "stable": "https://numpy.org/doc/stable/",
    |   "1.23.4": "https://numpy.org/doc/1.23/",
    |   "1.23.x": "https://numpy.org/doc/1.23/",
    |   "1.22.x": "https://numpy.org/doc/1.22/",
```

### Comparing `auto-intersphinx-1.0.2/pyproject.toml` & `auto-intersphinx-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build-system]
     requires = ["setuptools>=61.0.0", "wheel"]
     build-backend = "setuptools.build_meta"
 
 [project]
 name = "auto-intersphinx"
-version = "1.0.2"
+version = "1.0.3"
 requires-python = ">=3.9"
 description = "Automatic links direct project dependencies to the intersphinx catalog"
 readme = "README.md"
 license = {text = "BSD 3-Clause License"}
 authors = [
   {name = "Andre Anjos", email = "andre.anjos@idiap.ch"},
 ]
@@ -29,15 +29,15 @@
     "sphinx",
     "packaging",
     "requests",
     "lxml",
 ]
 
 [project.urls]
-documentation = "https://auto-intersphinx.readthedocs.io/en/v1.0.2/"
+documentation = "https://auto-intersphinx.readthedocs.io/en/v1.0.3/"
 homepage = "https://pypi.org/project/auto-intersphinx"
 repository = "https://gitlab.idiap.ch/software/auto-intersphinx"
 changelog = "https://gitlab.idiap.ch/software/auto-intersphinx/-/releases"
 
 [project.optional-dependencies]
 qa = ["pre-commit"]
 doc = [
```

### Comparing `auto-intersphinx-1.0.2/src/auto_intersphinx/__init__.py` & `auto-intersphinx-1.0.3/src/auto_intersphinx/__init__.py`

 * *Files identical despite different names*

### Comparing `auto-intersphinx-1.0.2/src/auto_intersphinx/catalog.json` & `auto-intersphinx-1.0.3/src/auto_intersphinx/catalog.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9833131067961164%*

 * *Differences: {"'lightning'": "OrderedDict([('versions', OrderedDict([('latest', "*

 * *                "'https://lightning.ai/docs/pytorch/latest/'), ('stable', "*

 * *                "'https://lightning.ai/docs/pytorch/stable/'), ('2.0.2', "*

 * *                "'https://lightning.ai/docs/pytorch/2.0.2/'), ('2.0.1', "*

 * *                "'https://lightning.ai/docs/pytorch/2.0.1/'), ('2.0.0', "*

 * *                "'https://lightning.ai/docs/pytorch/2.0.0/')])), ('sources', OrderedDict())])",*

 * * "'pytorch-lightning'": "{'versions': {'latest': […]*

```diff
@@ -293,14 +293,24 @@
             "2.11.x": "https://jinja.palletsprojects.com/en/2.11.x/",
             "2.9.x": "https://jinja.palletsprojects.com/en/2.9.x/",
             "3.0.x": "https://jinja.palletsprojects.com/en/3.0.x/",
             "3.1.x": "https://jinja.palletsprojects.com/en/3.1.x/",
             "latest": "https://jinja.palletsprojects.com/en/latest/"
         }
     },
+    "lightning": {
+        "sources": {},
+        "versions": {
+            "2.0.0": "https://lightning.ai/docs/pytorch/2.0.0/",
+            "2.0.1": "https://lightning.ai/docs/pytorch/2.0.1/",
+            "2.0.2": "https://lightning.ai/docs/pytorch/2.0.2/",
+            "latest": "https://lightning.ai/docs/pytorch/latest/",
+            "stable": "https://lightning.ai/docs/pytorch/stable/"
+        }
+    },
     "matplotlib": {
         "sources": {},
         "versions": {
             "stable": "https://matplotlib.org/stable/"
         }
     },
     "mne": {
@@ -591,16 +601,16 @@
             "1.8.4": "https://pytorch-lightning.readthedocs.io/en/1.8.4/",
             "1.8.5": "https://pytorch-lightning.readthedocs.io/en/1.8.5/",
             "1.8.6": "https://pytorch-lightning.readthedocs.io/en/1.8.6/",
             "1.9.0": "https://pytorch-lightning.readthedocs.io/en/1.9.0/",
             "1.9.1": "https://pytorch-lightning.readthedocs.io/en/1.9.1/",
             "1.9.2": "https://pytorch-lightning.readthedocs.io/en/1.9.2/",
             "future-structure": "https://pytorch-lightning.readthedocs.io/en/future-structure/",
-            "latest": "https://pytorch-lightning.readthedocs.io/en/latest/",
-            "stable": "https://pytorch-lightning.readthedocs.io/en/stable/"
+            "latest": "https://lightning.ai/docs/pytorch/latest/",
+            "stable": "https://lightning.ai/docs/pytorch/stable/"
         }
     },
     "pyyaml": {
         "sources": {},
         "versions": {}
     },
     "pyzmq": {
```

### Comparing `auto-intersphinx-1.0.2/src/auto_intersphinx/catalog.py` & `auto-intersphinx-1.0.3/src/auto_intersphinx/catalog.py`

 * *Files identical despite different names*

### Comparing `auto-intersphinx-1.0.2/src/auto_intersphinx/check_packages.py` & `auto-intersphinx-1.0.3/src/auto_intersphinx/check_packages.py`

 * *Files identical despite different names*

### Comparing `auto-intersphinx-1.0.2/src/auto_intersphinx/cli.py` & `auto-intersphinx-1.0.3/src/auto_intersphinx/cli.py`

 * *Files identical despite different names*

### Comparing `auto-intersphinx-1.0.2/src/auto_intersphinx/dump_objects.py` & `auto-intersphinx-1.0.3/src/auto_intersphinx/dump_objects.py`

 * *Files identical despite different names*

### Comparing `auto-intersphinx-1.0.2/src/auto_intersphinx/update_catalog.py` & `auto-intersphinx-1.0.3/src/auto_intersphinx/update_catalog.py`

 * *Files identical despite different names*

### Comparing `auto-intersphinx-1.0.2/src/auto_intersphinx.egg-info/PKG-INFO` & `auto-intersphinx-1.0.3/src/auto_intersphinx.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: auto-intersphinx
-Version: 1.0.2
+Version: 1.0.3
 Summary: Automatic links direct project dependencies to the intersphinx catalog
 Author-email: Andre Anjos <andre.anjos@idiap.ch>
 License: BSD 3-Clause License
-Project-URL: documentation, https://auto-intersphinx.readthedocs.io/en/v1.0.2/
+Project-URL: documentation, https://auto-intersphinx.readthedocs.io/en/v1.0.3/
 Project-URL: homepage, https://pypi.org/project/auto-intersphinx
 Project-URL: repository, https://gitlab.idiap.ch/software/auto-intersphinx
 Project-URL: changelog, https://gitlab.idiap.ch/software/auto-intersphinx/-/releases
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -23,17 +23,17 @@
 
 <!--
 SPDX-FileCopyrightText: Copyright © 2022 Idiap Research Institute <contact@idiap.ch>
 
 SPDX-License-Identifier: BSD-3-Clause
 -->
 
-[![latest-docs](https://img.shields.io/badge/docs-v1.0.2-orange.svg)](https://auto-intersphinx.readthedocs.io/en/v1.0.2/)
-[![build](https://gitlab.idiap.ch/software/auto-intersphinx/badges/v1.0.2/pipeline.svg)](https://gitlab.idiap.ch/software/auto-intersphinx/commits/v1.0.2)
-[![coverage](https://gitlab.idiap.ch/software/auto-intersphinx/badges/v1.0.2/coverage.svg)](https://www.idiap.ch/software/biosignal/docs/software/auto-intersphinx/v1.0.2/coverage/index.html)
+[![latest-docs](https://img.shields.io/badge/docs-v1.0.3-orange.svg)](https://auto-intersphinx.readthedocs.io/en/v1.0.3/)
+[![build](https://gitlab.idiap.ch/software/auto-intersphinx/badges/v1.0.3/pipeline.svg)](https://gitlab.idiap.ch/software/auto-intersphinx/commits/v1.0.3)
+[![coverage](https://gitlab.idiap.ch/software/auto-intersphinx/badges/v1.0.3/coverage.svg)](https://www.idiap.ch/software/biosignal/docs/software/auto-intersphinx/v1.0.3/coverage/index.html)
 [![repository](https://img.shields.io/badge/gitlab-project-0000c0.svg)](https://gitlab.idiap.ch/software/auto-intersphinx)
 
 # Automatically Links Package Documentation from Their Names
 
 This package contains a [Sphinx](https://www.sphinx-doc.org/) plugin that can
 fill
 [intersphinx](https://www.sphinx-doc.org/en/main/usage/extensions/intersphinx.html)
```

### Comparing `auto-intersphinx-1.0.2/src/auto_intersphinx.egg-info/SOURCES.txt` & `auto-intersphinx-1.0.3/src/auto_intersphinx.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 src/auto_intersphinx.egg-info/PKG-INFO
 src/auto_intersphinx.egg-info/SOURCES.txt
 src/auto_intersphinx.egg-info/dependency_links.txt
 src/auto_intersphinx.egg-info/entry_points.txt
 src/auto_intersphinx.egg-info/requires.txt
 src/auto_intersphinx.egg-info/top_level.txt
 src/auto_intersphinx.egg-info/zip-safe
-tests/__init__.py
 tests/conftest.py
 tests/test_auto_intersphinx.py
 tests/test_check_packages.py
 tests/test_dump_objects.py
 tests/test_update_catalog.py
 tests/data/catalog.json
 tests/data/requirements.txt
```

### Comparing `auto-intersphinx-1.0.2/tests/data/catalog.json` & `auto-intersphinx-1.0.3/tests/data/catalog.json`

 * *Files identical despite different names*

### Comparing `auto-intersphinx-1.0.2/tests/test_auto_intersphinx.py` & `auto-intersphinx-1.0.3/tests/test_auto_intersphinx.py`

 * *Files identical despite different names*

### Comparing `auto-intersphinx-1.0.2/tests/test_check_packages.py` & `auto-intersphinx-1.0.3/tests/test_check_packages.py`

 * *Files identical despite different names*

### Comparing `auto-intersphinx-1.0.2/tests/test_dump_objects.py` & `auto-intersphinx-1.0.3/tests/test_dump_objects.py`

 * *Files identical despite different names*

### Comparing `auto-intersphinx-1.0.2/tests/test_update_catalog.py` & `auto-intersphinx-1.0.3/tests/test_update_catalog.py`

 * *Files identical despite different names*

