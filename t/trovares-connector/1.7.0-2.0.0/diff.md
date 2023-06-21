# Comparing `tmp/trovares_connector-1.7.0.tar.gz` & `tmp/trovares_connector-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trovares_connector-1.7.0.tar", last modified: Wed Feb 22 23:24:50 2023, max compression
+gzip compressed data, was "trovares_connector-2.0.0.tar", last modified: Wed Jun 21 20:19:27 2023, max compression
```

## Comparing `trovares_connector-1.7.0.tar` & `trovares_connector-2.0.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 snapcore  (1000) snapcore  (1000)        0 2023-02-22 23:24:50.925944 trovares_connector-1.7.0/
-drwxr-xr-x   0 snapcore  (1000) snapcore  (1000)        0 2023-02-22 23:24:50.915912 trovares_connector-1.7.0/.github/
-drwxr-xr-x   0 snapcore  (1000) snapcore  (1000)        0 2023-02-22 23:24:50.919256 trovares_connector-1.7.0/.github/workflows/
--rw-r--r--   0 snapcore  (1000) snapcore  (1000)     3813 2023-02-22 22:54:17.000000 trovares_connector-1.7.0/.github/workflows/pytest.yml
--rw-r--r--   0 snapcore  (1000) snapcore  (1000)     2008 2023-02-22 22:00:55.000000 trovares_connector-1.7.0/.github/workflows/sphinx.yml
--rw-r--r--   0 snapcore  (1000) snapcore  (1000)     1799 2022-06-10 18:44:24.000000 trovares_connector-1.7.0/.gitignore
--rw-r--r--   0 snapcore  (1000) snapcore  (1000)    11357 2022-06-10 18:44:24.000000 trovares_connector-1.7.0/LICENSE
--rw-r--r--   0 snapcore  (1000) snapcore  (1000)     4954 2023-02-22 23:24:50.925944 trovares_connector-1.7.0/PKG-INFO
--rw-r--r--   0 snapcore  (1000) snapcore  (1000)     3761 2022-07-29 23:20:09.000000 trovares_connector-1.7.0/README.md
--rw-r--r--   0 snapcore  (1000) snapcore  (1000)     2600 2023-02-22 22:00:55.000000 trovares_connector-1.7.0/RELEASE.rst
-drwxr-xr-x   0 snapcore  (1000) snapcore  (1000)        0 2023-02-22 23:24:50.919256 trovares_connector-1.7.0/docs/
--rw-r--r--   0 snapcore  (1000) snapcore  (1000)      788 2022-06-23 20:10:30.000000 trovares_connector-1.7.0/docs/Makefile
--rw-r--r--   0 snapcore  (1000) snapcore  (1000)      134 2023-02-22 22:49:17.000000 trovares_connector-1.7.0/docs/requirements.txt
-drwxr-xr-x   0 snapcore  (1000) snapcore  (1000)        0 2023-02-22 23:24:50.919256 trovares_connector-1.7.0/docs/source/
--rw-r--r--   0 snapcore  (1000) snapcore  (1000)     5799 2023-02-22 22:26:12.000000 trovares_connector-1.7.0/docs/source/conf.py
--rw-r--r--   0 snapcore  (1000) snapcore  (1000)    10324 2023-02-22 22:00:55.000000 trovares_connector-1.7.0/docs/source/index.rst
--rw-r--r--   0 snapcore  (1000) snapcore  (1000)      840 2023-02-22 22:00:55.000000 trovares_connector-1.7.0/pyproject.toml
-drwxr-xr-x   0 snapcore  (1000) snapcore  (1000)        0 2023-02-22 23:24:50.919256 trovares_connector-1.7.0/scripts/
--rwxr-xr-x   0 snapcore  (1000) snapcore  (1000)      927 2023-02-22 22:00:55.000000 trovares_connector-1.7.0/scripts/build-documentation.sh
--rwxr-xr-x   0 snapcore  (1000) snapcore  (1000)      877 2023-02-22 22:00:55.000000 trovares_connector-1.7.0/scripts/install.sh
--rw-r--r--   0 snapcore  (1000) snapcore  (1000)     1341 2023-02-22 23:24:50.929288 trovares_connector-1.7.0/setup.cfg
-drwxr-xr-x   0 snapcore  (1000) snapcore  (1000)        0 2023-02-22 23:24:50.919256 trovares_connector-1.7.0/src/
-drwxr-xr-x   0 snapcore  (1000) snapcore  (1000)        0 2023-02-22 23:24:50.922600 trovares_connector-1.7.0/src/trovares_connector/
--rw-r--r--   0 snapcore  (1000) snapcore  (1000)     1122 2023-02-22 22:00:55.000000 trovares_connector-1.7.0/src/trovares_connector/__init__.py
--rw-r--r--   0 snapcore  (1000) snapcore  (1000)     3830 2023-02-22 22:00:55.000000 trovares_connector-1.7.0/src/trovares_connector/common.py
-drwxr-xr-x   0 snapcore  (1000) snapcore  (1000)        0 2023-02-22 23:24:50.922600 trovares_connector-1.7.0/src/trovares_connector/neo4j_connector/
--rw-r--r--   0 snapcore  (1000) snapcore  (1000)      892 2023-02-22 22:00:55.000000 trovares_connector-1.7.0/src/trovares_connector/neo4j_connector/__init__.py
-drwxr-xr-x   0 snapcore  (1000) snapcore  (1000)        0 2023-02-22 23:24:50.925944 trovares_connector-1.7.0/src/trovares_connector/neo4j_connector/frontend/
--rw-r--r--   0 snapcore  (1000) snapcore  (1000)    51440 2022-07-29 16:26:40.000000 trovares_connector-1.7.0/src/trovares_connector/neo4j_connector/frontend/CypherLexer.py
--rw-r--r--   0 snapcore  (1000) snapcore  (1000)    32534 2022-07-29 16:26:40.000000 trovares_connector-1.7.0/src/trovares_connector/neo4j_connector/frontend/CypherListener.py
--rw-r--r--   0 snapcore  (1000) snapcore  (1000)   384928 2022-07-29 16:26:40.000000 trovares_connector-1.7.0/src/trovares_connector/neo4j_connector/frontend/CypherParser.py
--rw-r--r--   0 snapcore  (1000) snapcore  (1000)    19195 2022-07-29 16:26:40.000000 trovares_connector-1.7.0/src/trovares_connector/neo4j_connector/frontend/CypherVisitor.py
--rw-r--r--   0 snapcore  (1000) snapcore  (1000)        0 2022-07-29 16:26:40.000000 trovares_connector-1.7.0/src/trovares_connector/neo4j_connector/frontend/__init__.py
--rw-r--r--   0 snapcore  (1000) snapcore  (1000)    68000 2023-02-22 22:00:55.000000 trovares_connector-1.7.0/src/trovares_connector/neo4j_connector/neo4j_connector.py
--rw-r--r--   0 snapcore  (1000) snapcore  (1000)    14916 2023-02-22 22:00:55.000000 trovares_connector-1.7.0/src/trovares_connector/neo4j_connector/query_translator.py
--rw-r--r--   0 snapcore  (1000) snapcore  (1000)    29025 2023-02-22 22:00:55.000000 trovares_connector-1.7.0/src/trovares_connector/odbc.py
-drwxr-xr-x   0 snapcore  (1000) snapcore  (1000)        0 2023-02-22 23:24:50.922600 trovares_connector-1.7.0/src/trovares_connector.egg-info/
--rw-r--r--   0 snapcore  (1000) snapcore  (1000)     4954 2023-02-22 23:24:50.000000 trovares_connector-1.7.0/src/trovares_connector.egg-info/PKG-INFO
--rw-r--r--   0 snapcore  (1000) snapcore  (1000)     1158 2023-02-22 23:24:50.000000 trovares_connector-1.7.0/src/trovares_connector.egg-info/SOURCES.txt
--rw-r--r--   0 snapcore  (1000) snapcore  (1000)        1 2023-02-22 23:24:50.000000 trovares_connector-1.7.0/src/trovares_connector.egg-info/dependency_links.txt
--rw-r--r--   0 snapcore  (1000) snapcore  (1000)      102 2023-02-22 23:24:50.000000 trovares_connector-1.7.0/src/trovares_connector.egg-info/requires.txt
--rw-r--r--   0 snapcore  (1000) snapcore  (1000)       19 2023-02-22 23:24:50.000000 trovares_connector-1.7.0/src/trovares_connector.egg-info/top_level.txt
-drwxr-xr-x   0 snapcore  (1000) snapcore  (1000)        0 2023-02-22 23:24:50.925944 trovares_connector-1.7.0/test/
--rw-r--r--   0 snapcore  (1000) snapcore  (1000)        0 2022-07-06 00:04:24.000000 trovares_connector-1.7.0/test/conftest.py
--rw-r--r--   0 snapcore  (1000) snapcore  (1000)      394 2022-06-15 19:18:05.000000 trovares_connector-1.7.0/test/test_admin.py
--rw-r--r--   0 snapcore  (1000) snapcore  (1000)    35380 2023-02-22 22:00:55.000000 trovares_connector-1.7.0/test/test_neo4j_connector.py
--rw-r--r--   0 snapcore  (1000) snapcore  (1000)    20715 2023-02-22 22:00:55.000000 trovares_connector-1.7.0/test/test_odbc_connector.py
+drwxr-xr-x   0 snapcore  (1000) snapcore  (1000)        0 2023-06-21 20:19:27.655439 trovares_connector-2.0.0/
+drwxr-xr-x   0 snapcore  (1000) snapcore  (1000)        0 2023-06-21 20:19:27.618751 trovares_connector-2.0.0/.github/
+drwxr-xr-x   0 snapcore  (1000) snapcore  (1000)        0 2023-06-21 20:19:27.625422 trovares_connector-2.0.0/.github/workflows/
+-rw-r--r--   0 snapcore  (1000) snapcore  (1000)     3813 2023-02-22 22:54:17.000000 trovares_connector-2.0.0/.github/workflows/pytest.yml
+-rw-r--r--   0 snapcore  (1000) snapcore  (1000)     2008 2023-02-22 22:00:55.000000 trovares_connector-2.0.0/.github/workflows/sphinx.yml
+-rw-r--r--   0 snapcore  (1000) snapcore  (1000)     1799 2022-06-10 18:44:24.000000 trovares_connector-2.0.0/.gitignore
+-rw-r--r--   0 snapcore  (1000) snapcore  (1000)    11357 2022-06-10 18:44:24.000000 trovares_connector-2.0.0/LICENSE
+-rw-r--r--   0 snapcore  (1000) snapcore  (1000)     4964 2023-06-21 20:19:27.655439 trovares_connector-2.0.0/PKG-INFO
+-rw-r--r--   0 snapcore  (1000) snapcore  (1000)     3771 2023-03-02 19:53:38.000000 trovares_connector-2.0.0/README.md
+-rw-r--r--   0 snapcore  (1000) snapcore  (1000)     2732 2023-06-21 20:18:29.000000 trovares_connector-2.0.0/RELEASE.rst
+drwxr-xr-x   0 snapcore  (1000) snapcore  (1000)        0 2023-06-21 20:19:27.628757 trovares_connector-2.0.0/docs/
+-rw-r--r--   0 snapcore  (1000) snapcore  (1000)      788 2022-06-23 20:10:30.000000 trovares_connector-2.0.0/docs/Makefile
+-rw-r--r--   0 snapcore  (1000) snapcore  (1000)      134 2023-02-22 22:49:17.000000 trovares_connector-2.0.0/docs/requirements.txt
+drwxr-xr-x   0 snapcore  (1000) snapcore  (1000)        0 2023-06-21 20:19:27.632092 trovares_connector-2.0.0/docs/source/
+-rw-r--r--   0 snapcore  (1000) snapcore  (1000)     5799 2023-06-21 20:18:29.000000 trovares_connector-2.0.0/docs/source/conf.py
+-rw-r--r--   0 snapcore  (1000) snapcore  (1000)    10951 2023-03-02 19:13:08.000000 trovares_connector-2.0.0/docs/source/index.rst
+-rw-r--r--   0 snapcore  (1000) snapcore  (1000)      840 2023-02-22 22:00:55.000000 trovares_connector-2.0.0/pyproject.toml
+drwxr-xr-x   0 snapcore  (1000) snapcore  (1000)        0 2023-06-21 20:19:27.632092 trovares_connector-2.0.0/scripts/
+-rwxr-xr-x   0 snapcore  (1000) snapcore  (1000)      927 2023-02-22 22:00:55.000000 trovares_connector-2.0.0/scripts/build-documentation.sh
+-rwxr-xr-x   0 snapcore  (1000) snapcore  (1000)      877 2023-02-22 22:00:55.000000 trovares_connector-2.0.0/scripts/install.sh
+-rw-r--r--   0 snapcore  (1000) snapcore  (1000)     1341 2023-06-21 20:19:27.658775 trovares_connector-2.0.0/setup.cfg
+drwxr-xr-x   0 snapcore  (1000) snapcore  (1000)        0 2023-06-21 20:19:27.625422 trovares_connector-2.0.0/src/
+drwxr-xr-x   0 snapcore  (1000) snapcore  (1000)        0 2023-06-21 20:19:27.642098 trovares_connector-2.0.0/src/trovares_connector/
+-rw-r--r--   0 snapcore  (1000) snapcore  (1000)     1122 2023-02-22 22:00:55.000000 trovares_connector-2.0.0/src/trovares_connector/__init__.py
+-rw-r--r--   0 snapcore  (1000) snapcore  (1000)     3830 2023-02-22 22:00:55.000000 trovares_connector-2.0.0/src/trovares_connector/common.py
+drwxr-xr-x   0 snapcore  (1000) snapcore  (1000)        0 2023-06-21 20:19:27.645434 trovares_connector-2.0.0/src/trovares_connector/neo4j_connector/
+-rw-r--r--   0 snapcore  (1000) snapcore  (1000)      892 2023-02-22 22:00:55.000000 trovares_connector-2.0.0/src/trovares_connector/neo4j_connector/__init__.py
+drwxr-xr-x   0 snapcore  (1000) snapcore  (1000)        0 2023-06-21 20:19:27.655439 trovares_connector-2.0.0/src/trovares_connector/neo4j_connector/frontend/
+-rw-r--r--   0 snapcore  (1000) snapcore  (1000)    51440 2022-07-29 16:26:40.000000 trovares_connector-2.0.0/src/trovares_connector/neo4j_connector/frontend/CypherLexer.py
+-rw-r--r--   0 snapcore  (1000) snapcore  (1000)    32534 2022-07-29 16:26:40.000000 trovares_connector-2.0.0/src/trovares_connector/neo4j_connector/frontend/CypherListener.py
+-rw-r--r--   0 snapcore  (1000) snapcore  (1000)   384928 2022-07-29 16:26:40.000000 trovares_connector-2.0.0/src/trovares_connector/neo4j_connector/frontend/CypherParser.py
+-rw-r--r--   0 snapcore  (1000) snapcore  (1000)    19195 2022-07-29 16:26:40.000000 trovares_connector-2.0.0/src/trovares_connector/neo4j_connector/frontend/CypherVisitor.py
+-rw-r--r--   0 snapcore  (1000) snapcore  (1000)        0 2022-07-29 16:26:40.000000 trovares_connector-2.0.0/src/trovares_connector/neo4j_connector/frontend/__init__.py
+-rw-r--r--   0 snapcore  (1000) snapcore  (1000)    67978 2023-06-21 20:18:29.000000 trovares_connector-2.0.0/src/trovares_connector/neo4j_connector/neo4j_connector.py
+-rw-r--r--   0 snapcore  (1000) snapcore  (1000)    14916 2023-02-22 22:00:55.000000 trovares_connector-2.0.0/src/trovares_connector/neo4j_connector/query_translator.py
+-rw-r--r--   0 snapcore  (1000) snapcore  (1000)    29049 2023-06-21 20:18:29.000000 trovares_connector-2.0.0/src/trovares_connector/odbc.py
+drwxr-xr-x   0 snapcore  (1000) snapcore  (1000)        0 2023-06-21 20:19:27.642098 trovares_connector-2.0.0/src/trovares_connector.egg-info/
+-rw-r--r--   0 snapcore  (1000) snapcore  (1000)     4964 2023-06-21 20:19:27.000000 trovares_connector-2.0.0/src/trovares_connector.egg-info/PKG-INFO
+-rw-r--r--   0 snapcore  (1000) snapcore  (1000)     1158 2023-06-21 20:19:27.000000 trovares_connector-2.0.0/src/trovares_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 snapcore  (1000) snapcore  (1000)        1 2023-06-21 20:19:27.000000 trovares_connector-2.0.0/src/trovares_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 snapcore  (1000) snapcore  (1000)      102 2023-06-21 20:19:27.000000 trovares_connector-2.0.0/src/trovares_connector.egg-info/requires.txt
+-rw-r--r--   0 snapcore  (1000) snapcore  (1000)       19 2023-06-21 20:19:27.000000 trovares_connector-2.0.0/src/trovares_connector.egg-info/top_level.txt
+drwxr-xr-x   0 snapcore  (1000) snapcore  (1000)        0 2023-06-21 20:19:27.655439 trovares_connector-2.0.0/test/
+-rw-r--r--   0 snapcore  (1000) snapcore  (1000)        0 2022-07-06 00:04:24.000000 trovares_connector-2.0.0/test/conftest.py
+-rw-r--r--   0 snapcore  (1000) snapcore  (1000)      394 2022-06-15 19:18:05.000000 trovares_connector-2.0.0/test/test_admin.py
+-rw-r--r--   0 snapcore  (1000) snapcore  (1000)    35040 2023-06-21 20:18:29.000000 trovares_connector-2.0.0/test/test_neo4j_connector.py
+-rw-r--r--   0 snapcore  (1000) snapcore  (1000)    20265 2023-06-21 20:18:29.000000 trovares_connector-2.0.0/test/test_odbc_connector.py
```

### Comparing `trovares_connector-1.7.0/.github/workflows/pytest.yml` & `trovares_connector-2.0.0/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `trovares_connector-1.7.0/.github/workflows/sphinx.yml` & `trovares_connector-2.0.0/.github/workflows/sphinx.yml`

 * *Files identical despite different names*

### Comparing `trovares_connector-1.7.0/.gitignore` & `trovares_connector-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `trovares_connector-1.7.0/LICENSE` & `trovares_connector-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trovares_connector-1.7.0/PKG-INFO` & `trovares_connector-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trovares_connector
-Version: 1.7.0
+Version: 2.0.0
 Summary: Connecting the Trovares xGT graph analytics engine to other applications.
 Home-page: http://www.trovares.com/
 Author: Trovares, Inc.
 Author-email: support@trovares.com
 License: apache2
 Project-URL: Documentation, https://trovares.github.io/trovares_connector/
 Project-URL: Repository, https://github.com/trovares/trovares_connector
@@ -33,15 +33,15 @@
 [![Pypi Versions](https://img.shields.io/pypi/pyversions/trovares_connector)](https://pypi.python.org/pypi/trovares_connector)
 [![License](https://img.shields.io/github/license/trovares/trovares_connector)](https://github.com/trovares/trovares_connector/blob/main/LICENSE)
 [![Twitter Follow](https://img.shields.io/twitter/follow/TrovaresxGT)](https://twitter.com/TrovaresxGT)
 
 This Python package is for connecting the Trovares xGT graph analytics engine to other applications.
 Trovares xGT can [significantly speedup Neo4j queries](https://www.trovares.com/trovaresvneo4j).
 
-The default connector provided is for Neo4j.
+The default connector provided is for Neo4j or AuraDB.
 The package also provides an optional ODBC connector for connecting to databases or applications that support ODBC.
 Information about the ODBC connector can be found [in the documentation](https://trovares.github.io/trovares_connector/odbc). 
 
 <table>
   <tr>
     <td><b>Homepage:</b></td>
     <td><a href="https://www.trovares.com">trovares.com</a></td>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: trovares_connector Version: 1.7.0 Summary:
+Metadata-Version: 2.1 Name: trovares_connector Version: 2.0.0 Summary:
 Connecting the Trovares xGT graph analytics engine to other applications. Home-
 page: http://www.trovares.com/ Author: Trovares, Inc. Author-email:
 support@trovares.com License: apache2 Project-URL: Documentation, https://
 trovares.github.io/trovares_connector/ Project-URL: Repository, https://
 github.com/trovares/trovares_connector Project-URL: Changelog, https://
 github.com/trovares/trovares_connector/blob/main/RELEASE.rst Keywords: Neo4j
 Trovares xGT cypher ODBC database Classifier: Development Status :: 5 -
@@ -22,17 +22,17 @@
 pyversions/trovares_connector)](https://pypi.python.org/pypi/
 trovares_connector) [![License](https://img.shields.io/github/license/trovares/
 trovares_connector)](https://github.com/trovares/trovares_connector/blob/main/
 LICENSE) [![Twitter Follow](https://img.shields.io/twitter/follow/TrovaresxGT)]
 (https://twitter.com/TrovaresxGT) This Python package is for connecting the
 Trovares xGT graph analytics engine to other applications. Trovares xGT can
 [significantly speedup Neo4j queries](https://www.trovares.com/trovaresvneo4j).
-The default connector provided is for Neo4j. The package also provides an
-optional ODBC connector for connecting to databases or applications that
-support ODBC. Information about the ODBC connector can be found [in the
+The default connector provided is for Neo4j or AuraDB. The package also
+provides an optional ODBC connector for connecting to databases or applications
+that support ODBC. Information about the ODBC connector can be found [in the
 documentation](https://trovares.github.io/trovares_connector/odbc).
 Homepage:      trovares.com
 Documentation: trovares.github.io/trovares_connector
 General Help:  github.com/trovares/trovares_connector/discussions
 ## Requirements - [Neo4j Python](https://pypi.org/project/neo4j/) - [xGT
 Python](https://pypi.org/project/xgt/) - [Pyarrow](https://pypi.org/project/
 pyarrow/) - [Trovares xGT](https://www.trovares.com) ## Installation You can
```

### Comparing `trovares_connector-1.7.0/README.md` & `trovares_connector-2.0.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [![Pypi Versions](https://img.shields.io/pypi/pyversions/trovares_connector)](https://pypi.python.org/pypi/trovares_connector)
 [![License](https://img.shields.io/github/license/trovares/trovares_connector)](https://github.com/trovares/trovares_connector/blob/main/LICENSE)
 [![Twitter Follow](https://img.shields.io/twitter/follow/TrovaresxGT)](https://twitter.com/TrovaresxGT)
 
 This Python package is for connecting the Trovares xGT graph analytics engine to other applications.
 Trovares xGT can [significantly speedup Neo4j queries](https://www.trovares.com/trovaresvneo4j).
 
-The default connector provided is for Neo4j.
+The default connector provided is for Neo4j or AuraDB.
 The package also provides an optional ODBC connector for connecting to databases or applications that support ODBC.
 Information about the ODBC connector can be found [in the documentation](https://trovares.github.io/trovares_connector/odbc). 
 
 <table>
   <tr>
     <td><b>Homepage:</b></td>
     <td><a href="https://www.trovares.com">trovares.com</a></td>
```

#### html2text {}

```diff
@@ -6,17 +6,17 @@
 pyversions/trovares_connector)](https://pypi.python.org/pypi/
 trovares_connector) [![License](https://img.shields.io/github/license/trovares/
 trovares_connector)](https://github.com/trovares/trovares_connector/blob/main/
 LICENSE) [![Twitter Follow](https://img.shields.io/twitter/follow/TrovaresxGT)]
 (https://twitter.com/TrovaresxGT) This Python package is for connecting the
 Trovares xGT graph analytics engine to other applications. Trovares xGT can
 [significantly speedup Neo4j queries](https://www.trovares.com/trovaresvneo4j).
-The default connector provided is for Neo4j. The package also provides an
-optional ODBC connector for connecting to databases or applications that
-support ODBC. Information about the ODBC connector can be found [in the
+The default connector provided is for Neo4j or AuraDB. The package also
+provides an optional ODBC connector for connecting to databases or applications
+that support ODBC. Information about the ODBC connector can be found [in the
 documentation](https://trovares.github.io/trovares_connector/odbc).
 Homepage:      trovares.com
 Documentation: trovares.github.io/trovares_connector
 General Help:  github.com/trovares/trovares_connector/discussions
 ## Requirements - [Neo4j Python](https://pypi.org/project/neo4j/) - [xGT
 Python](https://pypi.org/project/xgt/) - [Pyarrow](https://pypi.org/project/
 pyarrow/) - [Trovares xGT](https://www.trovares.com) ## Installation You can
```

### Comparing `trovares_connector-1.7.0/RELEASE.rst` & `trovares_connector-2.0.0/RELEASE.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 Release Notes
 =============
 
+2.0.0 (06-14-2023)
+------------------
+
+Changed
+^^^^^^^
+  - Require xGT 1.14.
+
+Fixed
+^^^^^
+  - Warnings about deprecated functions.
+
 1.7.0 (02-22-2023)
 ------------------
 
 New Features
 ^^^^^^^^^^^^
   - Added SAP driver that supports downloading from SAP ASE.
```

### Comparing `trovares_connector-1.7.0/docs/Makefile` & `trovares_connector-2.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `trovares_connector-1.7.0/docs/source/conf.py` & `trovares_connector-2.0.0/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 # -- Project information -----------------------------------------------------
 
 project = 'trovares_connector'
 copyright = '2022-2023, Trovares, Inc.'
 author = 'trovares.com'
 
 # The full version, including alpha/beta/rc tags
-release = '1.7.0'
+release = '2.0.0'
 
 # -- General configuration ---------------------------------------------------
 
 # Sphinx extensions. These are Python module names that will be imported.
 extensions = [
   'sphinx.ext.autodoc',
   'sphinx.ext.autosummary',
```

### Comparing `trovares_connector-1.7.0/docs/source/index.rst` & `trovares_connector-2.0.0/docs/source/index.rst`

 * *Files 8% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 Trovares xGT can `significantly speedup Neo4j queries <https://www.trovares.com/trovaresvneo4j>`_.
 
 The connector `source code <http://github.com/trovares/trovares_connector/>`_ is available on github.
 
 A basic guide is provided below.
 For a quick start see :ref:`quick_start`.
 
-The default connector provided is for connecting to Neo4j.
+The default connector provided is for connecting to Neo4j or AuraDB.
 The package also provides an optional :ref:`odbc` for connecting to databases or applications that support ODBC.
 
 Installation
 ------------
 
 You can install this python package by executing this command:
 
@@ -154,14 +154,30 @@
 
 In addition the unlabeled nodes in Neo4j are named '' and this can be used to map these to a custom xGT type:
 
 .. code-block:: python
 
    conn.transfer_to_xgt(vertices=[('', 'my_empty_type')])
 
+Connecting to AuraDB
+^^^^^^^^^^^^^^^^^^^^
+The connector can connect to AuraDB instances by setting the hostname and appropriate protocol:
+
+.. code-block:: python
+
+   import xgt
+   from trovares_connector import Neo4jConnector, Neo4jDriver
+   from neo4j import GraphDatabase
+
+   xgt_server = xgt.Connection()
+   xgt_server.set_default_namespace('neo4j')
+   # The protocol would be the part before ://. Usually this is neo4j+s.
+   neo4j_server = Neo4jDriver(protocol='neo4j+s', hostname='hostname <something like ashdjs43.databases.neo4j.io>', auth=('neo4j', 'foo'))
+   conn = Neo4jConnector(xgt_server, neo4j_server)
+
 
 Using various Neo4j drivers
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 The connector supports passing a trovares_connector.Neo4jDriver, neo4j.BoltDriver, or a neo4j.Neo4jDriver.
 The Trovares Neo4jDriver provides support for connecting to the Neo4j server through a combination of choices such as http, arrow, bolt, or other drivers.
 These additional drivers can provide much faster performance than the default neo4j.Neo4jDriver, but may require the optional components as explained in :ref:`requirements`.
```

### Comparing `trovares_connector-1.7.0/pyproject.toml` & `trovares_connector-2.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `trovares_connector-1.7.0/scripts/build-documentation.sh` & `trovares_connector-2.0.0/scripts/build-documentation.sh`

 * *Files identical despite different names*

### Comparing `trovares_connector-1.7.0/scripts/install.sh` & `trovares_connector-2.0.0/scripts/install.sh`

 * *Files identical despite different names*

### Comparing `trovares_connector-1.7.0/setup.cfg` & `trovares_connector-2.0.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trovares_connector
-version = 1.7.0
+version = 2.0.0
 author = Trovares, Inc.
 author_email = support@trovares.com
 description = Connecting the Trovares xGT graph analytics engine to other applications.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = apache2
 url = http://www.trovares.com/
@@ -29,15 +29,15 @@
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.7
 install_requires = 
 	neo4j>=4.4.1
-	xgt>=1.10.1
+	xgt>=1.14.0
 	pyarrow>=7.0.0
 	antlr4-python3-runtime>=4.10
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
```

### Comparing `trovares_connector-1.7.0/src/trovares_connector/__init__.py` & `trovares_connector-2.0.0/src/trovares_connector/__init__.py`

 * *Files identical despite different names*

### Comparing `trovares_connector-1.7.0/src/trovares_connector/common.py` & `trovares_connector-2.0.0/src/trovares_connector/common.py`

 * *Files identical despite different names*

### Comparing `trovares_connector-1.7.0/src/trovares_connector/neo4j_connector/__init__.py` & `trovares_connector-2.0.0/src/trovares_connector/neo4j_connector/__init__.py`

 * *Files identical despite different names*

### Comparing `trovares_connector-1.7.0/src/trovares_connector/neo4j_connector/frontend/CypherLexer.py` & `trovares_connector-2.0.0/src/trovares_connector/neo4j_connector/frontend/CypherLexer.py`

 * *Files identical despite different names*

### Comparing `trovares_connector-1.7.0/src/trovares_connector/neo4j_connector/frontend/CypherListener.py` & `trovares_connector-2.0.0/src/trovares_connector/neo4j_connector/frontend/CypherListener.py`

 * *Files identical despite different names*

### Comparing `trovares_connector-1.7.0/src/trovares_connector/neo4j_connector/frontend/CypherParser.py` & `trovares_connector-2.0.0/src/trovares_connector/neo4j_connector/frontend/CypherParser.py`

 * *Files identical despite different names*

### Comparing `trovares_connector-1.7.0/src/trovares_connector/neo4j_connector/frontend/CypherVisitor.py` & `trovares_connector-2.0.0/src/trovares_connector/neo4j_connector/frontend/CypherVisitor.py`

 * *Files identical despite different names*

### Comparing `trovares_connector-1.7.0/src/trovares_connector/neo4j_connector/neo4j_connector.py` & `trovares_connector-2.0.0/src/trovares_connector/neo4j_connector/neo4j_connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -591,15 +591,15 @@
         for vertex, schema in xgt_schemas['vertices'].items():
             table_schema = schema['schema']
             key = schema['key']
             create_frame = True
             vname = schema['xgt_name']
             if append:
                 try:
-                    frame = self._xgt_server.get_vertex_frame(vname)
+                    frame = self._xgt_server.get_frame(vname)
                     if frame.schema != table_schema:
                         raise ValueError(
                             f"Vertex Frame {vname} has a schema {frame.schema}"
                             + f" that is incompatible with Neo4j: {table_schema}"
                         )
                     create_frame = False
                 except:
@@ -813,26 +813,26 @@
         -------
             None
         """
         xgt_server = self._xgt_server
         if namespace == None:
             namespace = self._default_namespace
         if vertices == None and edges == None:
-            vertices = [frame.name for frame in xgt_server.get_vertex_frames(namespace=namespace)]
-            edges = [frame.name for frame in xgt_server.get_edge_frames(namespace=namespace)]
+            vertices = [frame.name for frame in xgt_server.get_frames(namespace=namespace, frame_type='vertex')]
+            edges = [frame.name for frame in xgt_server.get_frames(namespace=namespace, frame_type='edge')]
             namespace = None
         elif vertices == None:
             vertices = []
         elif edges == None:
             edges = []
 
         id_neo4j_map = { }
 
         for edge in edges:
-            edge_frame = xgt_server.get_edge_frame(edge)
+            edge_frame = xgt_server.get_frame(edge)
             vertices.append(edge_frame.source_name)
             vertices.append(edge_frame.target_name)
 
         def convert(value):
             if value is None:
                 return 'Null'
             elif isinstance(value, str):
@@ -871,24 +871,24 @@
 
         count_map = { }
         estimated_counts = 0
         for vertex in vertices:
             if vertex in count_map:
                 continue
             count_map[vertex] = True
-            estimated_counts += xgt_server.get_vertex_frame(vertex).num_rows
+            estimated_counts += xgt_server.get_frame(vertex).num_rows
         for edge in edges:
-            estimated_counts += xgt_server.get_edge_frame(edge).num_rows
+            estimated_counts += xgt_server.get_frame(edge).num_rows
 
         with ProgressDisplay(estimated_counts) as progress_bar:
             for vertex in vertices:
                 if vertex in id_neo4j_map:
                     continue
                 id_neo4j_map[vertex] = { }
-                vertex_frame = xgt_server.get_vertex_frame(vertex)
+                vertex_frame = xgt_server.get_frame(vertex)
                 create_string = 'create (a:' + vertex + '{{{0}}}) return ID(a)'
 
                 schema = vertex_frame.schema
                 reader = self.__arrow_reader(vertex)
 
                 labels = [val[0] for val in schema]
 
@@ -918,19 +918,19 @@
                                 progress_bar.show_progress(1)
                             tx.commit()
                             tx.close()
                         except StopIteration:
                             break
 
             for edge in edges:
-                edge_frame = xgt_server.get_edge_frame(edge)
+                edge_frame = xgt_server.get_frame(edge)
                 source = edge_frame.source_name
                 target = edge_frame.target_name
-                source_frame = xgt_server.get_vertex_frame(source)
-                target_frame = xgt_server.get_vertex_frame(target)
+                source_frame = xgt_server.get_frame(source)
+                target_frame = xgt_server.get_frame(target)
                 source_map = id_neo4j_map[source]
                 target_map = id_neo4j_map[target]
                 create_string = 'match (a:' + source + '), (b:' + target + ') where ID(a) = {0} and ID(b) = {1} create (a)-[:' + edge + '{{{2}}}]->(b)'
 
                 schema = edge_frame.schema
                 reader = self.__arrow_reader(edge)
                 labels = [val[0] for val in schema]
```

### Comparing `trovares_connector-1.7.0/src/trovares_connector/neo4j_connector/query_translator.py` & `trovares_connector-2.0.0/src/trovares_connector/neo4j_connector/query_translator.py`

 * *Files identical despite different names*

### Comparing `trovares_connector-1.7.0/src/trovares_connector/odbc.py` & `trovares_connector-2.0.0/src/trovares_connector/odbc.py`

 * *Files 0% similar despite different names*

```diff
@@ -501,17 +501,17 @@
         """
         if isinstance(self._driver, OracleODBCDriver):
             raise XgtNotImplementedError("Oracle not supported for transferring to.")
         xgt_server = self._xgt_server
         if namespace == None:
             namespace = self._default_namespace
         if vertices == None and edges == None and tables == None:
-            vertices = [(frame.name, frame.name) for frame in xgt_server.get_vertex_frames(namespace=namespace)]
-            edges = [(frame.name, frame.name) for frame in xgt_server.get_edge_frames(namespace=namespace)]
-            tables = [(frame.name, frame.name) for frame in xgt_server.get_table_frames(namespace=namespace)]
+            vertices = [(frame.name, frame.name) for frame in xgt_server.get_frames(namespace=namespace, frame_type='vertex')]
+            edges = [(frame.name, frame.name) for frame in xgt_server.get_frames(namespace=namespace, frame_type='edge')]
+            tables = [(frame.name, frame.name) for frame in xgt_server.get_frames(namespace=namespace, frame_type='table')]
             namespace = None
         if vertices == None:
             vertices = []
         if edges == None:
             edges = []
         if tables == None:
             tables = []
@@ -535,19 +535,19 @@
                 final_tables.append((table, table))
             else:
                 final_tables.append(table)
 
         estimate = 0
 
         for vertex in final_vertices:
-            estimate += xgt_server.get_vertex_frame(vertex[0]).num_rows
+            estimate += xgt_server.get_frame(vertex[0]).num_rows
         for edge in final_edges:
-            estimate += xgt_server.get_edge_frame(edge[0]).num_rows
+            estimate += xgt_server.get_frame(edge[0]).num_rows
         for table in final_tables:
-            estimate += xgt_server.get_table_frame(table[0]).num_rows
+            estimate += xgt_server.get_frame(table[0]).num_rows
 
         with ProgressDisplay(estimate) as progress_bar:
             for table in final_vertices + final_edges + final_tables:
                 frame, table = table
                 reader = self.__arrow_reader(frame)
                 batch_reader = reader.to_reader()
```

### Comparing `trovares_connector-1.7.0/src/trovares_connector.egg-info/PKG-INFO` & `trovares_connector-2.0.0/src/trovares_connector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trovares-connector
-Version: 1.7.0
+Version: 2.0.0
 Summary: Connecting the Trovares xGT graph analytics engine to other applications.
 Home-page: http://www.trovares.com/
 Author: Trovares, Inc.
 Author-email: support@trovares.com
 License: apache2
 Project-URL: Documentation, https://trovares.github.io/trovares_connector/
 Project-URL: Repository, https://github.com/trovares/trovares_connector
@@ -33,15 +33,15 @@
 [![Pypi Versions](https://img.shields.io/pypi/pyversions/trovares_connector)](https://pypi.python.org/pypi/trovares_connector)
 [![License](https://img.shields.io/github/license/trovares/trovares_connector)](https://github.com/trovares/trovares_connector/blob/main/LICENSE)
 [![Twitter Follow](https://img.shields.io/twitter/follow/TrovaresxGT)](https://twitter.com/TrovaresxGT)
 
 This Python package is for connecting the Trovares xGT graph analytics engine to other applications.
 Trovares xGT can [significantly speedup Neo4j queries](https://www.trovares.com/trovaresvneo4j).
 
-The default connector provided is for Neo4j.
+The default connector provided is for Neo4j or AuraDB.
 The package also provides an optional ODBC connector for connecting to databases or applications that support ODBC.
 Information about the ODBC connector can be found [in the documentation](https://trovares.github.io/trovares_connector/odbc). 
 
 <table>
   <tr>
     <td><b>Homepage:</b></td>
     <td><a href="https://www.trovares.com">trovares.com</a></td>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: trovares-connector Version: 1.7.0 Summary:
+Metadata-Version: 2.1 Name: trovares-connector Version: 2.0.0 Summary:
 Connecting the Trovares xGT graph analytics engine to other applications. Home-
 page: http://www.trovares.com/ Author: Trovares, Inc. Author-email:
 support@trovares.com License: apache2 Project-URL: Documentation, https://
 trovares.github.io/trovares_connector/ Project-URL: Repository, https://
 github.com/trovares/trovares_connector Project-URL: Changelog, https://
 github.com/trovares/trovares_connector/blob/main/RELEASE.rst Keywords: Neo4j
 Trovares xGT cypher ODBC database Classifier: Development Status :: 5 -
@@ -22,17 +22,17 @@
 pyversions/trovares_connector)](https://pypi.python.org/pypi/
 trovares_connector) [![License](https://img.shields.io/github/license/trovares/
 trovares_connector)](https://github.com/trovares/trovares_connector/blob/main/
 LICENSE) [![Twitter Follow](https://img.shields.io/twitter/follow/TrovaresxGT)]
 (https://twitter.com/TrovaresxGT) This Python package is for connecting the
 Trovares xGT graph analytics engine to other applications. Trovares xGT can
 [significantly speedup Neo4j queries](https://www.trovares.com/trovaresvneo4j).
-The default connector provided is for Neo4j. The package also provides an
-optional ODBC connector for connecting to databases or applications that
-support ODBC. Information about the ODBC connector can be found [in the
+The default connector provided is for Neo4j or AuraDB. The package also
+provides an optional ODBC connector for connecting to databases or applications
+that support ODBC. Information about the ODBC connector can be found [in the
 documentation](https://trovares.github.io/trovares_connector/odbc).
 Homepage:      trovares.com
 Documentation: trovares.github.io/trovares_connector
 General Help:  github.com/trovares/trovares_connector/discussions
 ## Requirements - [Neo4j Python](https://pypi.org/project/neo4j/) - [xGT
 Python](https://pypi.org/project/xgt/) - [Pyarrow](https://pypi.org/project/
 pyarrow/) - [Trovares xGT](https://www.trovares.com) ## Installation You can
```

### Comparing `trovares_connector-1.7.0/src/trovares_connector.egg-info/SOURCES.txt` & `trovares_connector-2.0.0/src/trovares_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trovares_connector-1.7.0/test/test_neo4j_connector.py` & `trovares_connector-2.0.0/test/test_neo4j_connector.py`

 * *Files 9% similar despite different names*

```diff
@@ -230,43 +230,43 @@
     xgt_schema = c.get_xgt_schemas(vertices=['Node'])
     c.create_xgt_schemas(xgt_schema)
     for vertex, schema in xgt_schema['vertices'].items():
       table_schema = schema['schema']
       attributes = {_:t for _, t in table_schema}
       print(f"\nAttributes: {attributes}")
     c.copy_data_to_xgt(xgt_schema)
-    node_frame = self.xgt.get_vertex_frame('Node')
+    node_frame = self.xgt.get_frame('Node')
     assert node_frame.num_rows == 1
 
   def test_transfer_node_working_types_bolt(self):
     self._populate_node_working_types_bolt()
     c = self.conn
     xgt_schema = c.get_xgt_schemas(vertices=['Node'])
     c.create_xgt_schemas(xgt_schema)
     for vertex, schema in xgt_schema['vertices'].items():
       table_schema = schema['schema']
       attributes = {_:t for _, *t  in table_schema}
       print(f"\nAttributes: {attributes}")
     c.copy_data_to_xgt(xgt_schema)
-    node_frame = self.xgt.get_vertex_frame('Node')
+    node_frame = self.xgt.get_frame('Node')
     assert node_frame.num_rows == 3
     print(node_frame.get_data())
 
   def test_transfer_nodes_to_neo4j(self):
     self._populate_node_working_types_bolt()
     c = self.conn
     c.transfer_to_xgt(vertices=['Node'])
-    node_frame = self.xgt.get_vertex_frame('Node')
+    node_frame = self.xgt.get_frame('Node')
     assert node_frame.num_rows == 3
     expected = [row[1:] for row in node_frame.get_data()]
     self.neo4j_driver.query("MATCH (n) DETACH DELETE n").finalize()
     c.transfer_to_neo4j(vertices=['Node'])
     self.xgt.drop_frame("Node")
     c.transfer_to_xgt(vertices=['Node'])
-    node_frame = self.xgt.get_vertex_frame('Node')
+    node_frame = self.xgt.get_frame('Node')
     assert node_frame.num_rows == 3
     result = [row[1:] for row in node_frame.get_data()]
     # The column ordering can change when uploading to neo4j
     # So we just need to verify the None rows are correct
     # and the same elements are in the row with data, but with a different order.
     expected_pos = 0
     result_pos = 0
@@ -281,26 +281,26 @@
             assert expected[i].count(None) == len(expected[i])
     self.assertCountEqual(expected[expected_pos], result[result_pos])
 
   def test_transfer_edges_to_neo4j(self):
     self._populate_relationship_working_types_bolt()
     c = self.conn
     c.transfer_to_xgt(edges=['Relationship'])
-    node_frame = self.xgt.get_vertex_frame('Node')
-    edge_frame = self.xgt.get_edge_frame('Relationship')
+    node_frame = self.xgt.get_frame('Node')
+    edge_frame = self.xgt.get_frame('Relationship')
     assert edge_frame.num_rows == 3
     node_expected = [row[1:] for row in node_frame.get_data()]
     edge_expected = [row[2:] for row in edge_frame.get_data()]
     self.neo4j_driver.query("MATCH (n) DETACH DELETE n").finalize()
     c.transfer_to_neo4j(edges=['Relationship'])
     self.xgt.drop_frame("Relationship")
     self.xgt.drop_frame("Node")
     c.transfer_to_xgt(edges=['Relationship'])
-    node_frame = self.xgt.get_vertex_frame('Node')
-    edge_frame = self.xgt.get_edge_frame('Relationship')
+    node_frame = self.xgt.get_frame('Node')
+    edge_frame = self.xgt.get_frame('Relationship')
     assert edge_frame.num_rows == 3
     node_result = [row[1:] for row in node_frame.get_data()]
     edge_result = [row[2:] for row in edge_frame.get_data()]
     self.assertCountEqual(node_expected, node_result)
     # The column ordering can change when uploading to neo4j
     # So we just need to verify the None rows are correct
     # and the same elements are in the row with data, but with a different order.
@@ -319,67 +319,67 @@
 
   def test_transfer_relationship_working_types_bolt(self):
     self._populate_relationship_working_types_bolt()
     c = self.conn
     xgt_schema = c.get_xgt_schemas(vertices=['Node'], edges=['Relationship'])
     c.create_xgt_schemas(xgt_schema)
     c.copy_data_to_xgt(xgt_schema)
-    edge_frame = self.xgt.get_edge_frame('Relationship')
+    edge_frame = self.xgt.get_frame('Relationship')
     assert edge_frame.num_rows == 3
     print(edge_frame.get_data())
     self.xgt.drop_frame("Relationship")
 
   def test_transfer_relationship_working_types_bolt_map(self):
     self._populate_relationship_working_types_bolt()
     c = self.conn
     xgt_schema = c.get_xgt_schemas(vertices=[('Node', 'n')], edges=[('Relationship', 'r')])
     c.create_xgt_schemas(xgt_schema)
     c.copy_data_to_xgt(xgt_schema)
-    node_frame = self.xgt.get_vertex_frame('n')
-    edge_frame = self.xgt.get_edge_frame('r')
+    node_frame = self.xgt.get_frame('n')
+    edge_frame = self.xgt.get_frame('r')
     assert node_frame.num_rows == 6
     assert edge_frame.num_rows == 3
     print(edge_frame.get_data())
     self.xgt.drop_frame('r')
 
   def test_transfer_relationship_without_vertex_bolt(self):
     self._populate_relationship_working_types_bolt()
     c = self.conn
     xgt_schema = c.get_xgt_schemas(edges=['Relationship'])
     c.create_xgt_schemas(xgt_schema)
     c.copy_data_to_xgt(xgt_schema)
-    node_frame = self.xgt.get_vertex_frame('Node')
-    edge_frame = self.xgt.get_edge_frame('Relationship')
+    node_frame = self.xgt.get_frame('Node')
+    edge_frame = self.xgt.get_frame('Relationship')
     assert node_frame.num_rows == 6
     assert edge_frame.num_rows == 3
     assert node_frame.get_data(length=1)[0][1] == 1
     self.xgt.drop_frame("Relationship")
 
   def test_transfer_relationship_without_vertex_bolt_two_phase(self):
     self._populate_relationship_working_types_bolt()
     c = self.conn
     c.transfer_to_xgt(vertices=['Node'])
     xgt_schema = c.get_xgt_schemas(edges=['Relationship'], import_edge_nodes=False)
     c.create_xgt_schemas(xgt_schema, append=True)
     c.copy_data_to_xgt(xgt_schema)
-    node_frame = self.xgt.get_vertex_frame('Node')
-    edge_frame = self.xgt.get_edge_frame('Relationship')
+    node_frame = self.xgt.get_frame('Node')
+    edge_frame = self.xgt.get_frame('Relationship')
     assert node_frame.num_rows == 6
     assert edge_frame.num_rows == 3
     assert node_frame.get_data(length=1)[0][1] == 1
     self.xgt.drop_frame("Relationship")
 
   def test_transfer_everything_bolt(self):
     self._populate_relationship_working_types_bolt()
     c = self.conn
     xgt_schema = c.get_xgt_schemas()
     c.create_xgt_schemas(xgt_schema)
     c.copy_data_to_xgt(xgt_schema)
-    node_frame = self.xgt.get_vertex_frame('Node')
-    edge_frame = self.xgt.get_edge_frame('Relationship')
+    node_frame = self.xgt.get_frame('Node')
+    edge_frame = self.xgt.get_frame('Relationship')
     assert node_frame.num_rows == 6
     assert edge_frame.num_rows == 3
     self.xgt.drop_frame("Relationship")
 
   def test_append(self):
     c = self.conn
     self.neo4j_driver.query(
@@ -390,69 +390,69 @@
     c.copy_data_to_xgt(xgt_schema)
     c.create_xgt_schemas(xgt_schema, append=True)
 
     self.neo4j_driver.query("MATCH (n) DETACH DELETE n").finalize()
     self.neo4j_driver.query(
         'CREATE (:Node{int: 344, str: "string"})').finalize()
     c.copy_data_to_xgt(xgt_schema)
-    node_frame = self.xgt.get_vertex_frame('Node')
+    node_frame = self.xgt.get_frame('Node')
     assert node_frame.num_rows == 2
 
     c.create_xgt_schemas(xgt_schema, append=False)
-    node_frame = self.xgt.get_vertex_frame('Node')
+    node_frame = self.xgt.get_frame('Node')
     assert node_frame.num_rows == 0
 
   def test_dropping(self):
     c = self.conn
     self.neo4j_driver.query(
         'CREATE (:Node{})-[:Relationship]->(:Node{})').finalize()
     xgt_schema1 = c.get_xgt_schemas(vertices=['Node'], edges=['Relationship'])
     xgt_schema2 = c.get_xgt_schemas(vertices=['Node'])
 
     c.create_xgt_schemas(xgt_schema1)
-    self.xgt.get_vertex_frame('Node')
-    self.xgt.get_edge_frame('Relationship')
+    self.xgt.get_frame('Node')
+    self.xgt.get_frame('Relationship')
 
     c.create_xgt_schemas(xgt_schema1)
-    self.xgt.get_vertex_frame('Node')
-    self.xgt.get_edge_frame('Relationship')
+    self.xgt.get_frame('Node')
+    self.xgt.get_frame('Relationship')
 
     with self.assertRaises(xgt.XgtFrameDependencyError):
         c.create_xgt_schemas(xgt_schema2)
     c.create_xgt_schemas(xgt_schema2, force=True)
-    self.xgt.get_vertex_frame('Node')
+    self.xgt.get_frame('Node')
     with self.assertRaises(xgt.XgtNameError):
-        self.xgt.get_edge_frame('Relationship')
+        self.xgt.get_frame('Relationship')
 
   def test_multiple_node_labels_to(self):
     c = self.conn
     self.neo4j_driver.query(
         'CREATE (:Node1{})-[:Relationship{}]->(:Node1{}), (:Node1{})-[:Relationship{}]->(:Node2{})').finalize()
     schema = c.get_xgt_schemas(vertices=['Node1', 'Node2'], edges=['Relationship'])
     c.create_xgt_schemas(schema)
     c.copy_data_to_xgt(schema)
 
-    node_frame = self.xgt.get_edge_frame('Node1_Relationship_Node1')
+    node_frame = self.xgt.get_frame('Node1_Relationship_Node1')
     assert node_frame.num_rows == 1
-    node_frame = self.xgt.get_edge_frame('Node1_Relationship_Node2')
+    node_frame = self.xgt.get_frame('Node1_Relationship_Node2')
     assert node_frame.num_rows == 1
     self.xgt.drop_frame("Node1_Relationship_Node1")
     self.xgt.drop_frame("Node1_Relationship_Node2")
 
   def test_multiple_node_labels_from(self):
     c = self.conn
     self.neo4j_driver.query(
         'CREATE (:Node1{})-[:Relationship{}]->(:Node1{}), (:Node2{})-[:Relationship{}]->(:Node1{})').finalize()
     schema = c.get_xgt_schemas(vertices=['Node1', 'Node2'], edges=['Relationship'])
     c.create_xgt_schemas(schema)
     c.copy_data_to_xgt(schema)
 
-    node_frame = self.xgt.get_edge_frame('Node1_Relationship_Node1')
+    node_frame = self.xgt.get_frame('Node1_Relationship_Node1')
     assert node_frame.num_rows == 1
-    node_frame = self.xgt.get_edge_frame('Node2_Relationship_Node1')
+    node_frame = self.xgt.get_frame('Node2_Relationship_Node1')
     assert node_frame.num_rows == 1
     self.xgt.drop_frame("Node1_Relationship_Node1")
     self.xgt.drop_frame("Node2_Relationship_Node1")
 
   def test_multiple_property_types_vertex_negative(self):
     c = self.conn
     self.neo4j_driver.query(
@@ -496,121 +496,121 @@
     with self.assertRaises(xgt.XgtNameError):
         c.transfer_to_neo4j(edges=['cars'])
 
   def test_empty_labels(self):
     c = self.conn
     self.neo4j_driver.query('CREATE ()').finalize()
     c.transfer_to_xgt(vertices=[''])
-    node_frame = self.xgt.get_vertex_frame('unlabeled')
+    node_frame = self.xgt.get_frame('unlabeled')
     assert node_frame.num_rows == 1
 
   def test_map_empty_labels(self):
     c = self.conn
     self.neo4j_driver.query('CREATE ()').finalize()
     c.transfer_to_xgt(vertices=[('', 'custom_name')])
-    node_frame = self.xgt.get_vertex_frame('custom_name')
+    node_frame = self.xgt.get_frame('custom_name')
     assert node_frame.num_rows == 1
     with self.assertRaises(xgt.XgtNameError):
-        node_frame = self.xgt.get_vertex_frame('unlabeled')
+        node_frame = self.xgt.get_frame('unlabeled')
 
   def test_empty_labels_schema(self):
     c = self.conn
     self.neo4j_driver.query('CREATE ({int:2})').finalize()
     c.transfer_to_xgt(vertices=[''])
-    node_frame = self.xgt.get_vertex_frame('unlabeled')
+    node_frame = self.xgt.get_frame('unlabeled')
     res = self.xgt.run_job('match (v) return v.int')
     assert node_frame.num_rows == 1
     assert res.get_data()[0][0] == 2
     self.neo4j_driver.query("MATCH (n) DETACH DELETE n").finalize()
     self.neo4j_driver.query('CREATE ({str:"bbb"})').finalize()
     c.transfer_to_xgt(vertices=[''])
-    node_frame = self.xgt.get_vertex_frame('unlabeled')
+    node_frame = self.xgt.get_frame('unlabeled')
     res = self.xgt.run_job('match (v) return v.str')
     assert node_frame.num_rows == 1
     assert res.get_data()[0][0] == "bbb"
 
   def test_edge_empty_labels(self):
     c = self.conn
     self.neo4j_driver.query(
         'CREATE ()-[:e1]->(), (:Node)-[:e2]->(), ()-[:e3]->(:Node)').finalize()
     c.transfer_to_xgt(edges=['e1', 'e2', 'e3'])
-    node_frame = self.xgt.get_edge_frame('e1')
+    node_frame = self.xgt.get_frame('e1')
     assert node_frame.num_rows == 1
-    node_frame = self.xgt.get_edge_frame('e2')
+    node_frame = self.xgt.get_frame('e2')
     assert node_frame.num_rows == 1
-    node_frame = self.xgt.get_edge_frame('e3')
+    node_frame = self.xgt.get_frame('e3')
     assert node_frame.num_rows == 1
-    node_frame = self.xgt.get_vertex_frame('unlabeled')
+    node_frame = self.xgt.get_frame('unlabeled')
     assert node_frame.num_rows == 4
-    node_frame = self.xgt.get_vertex_frame('Node')
+    node_frame = self.xgt.get_frame('Node')
     assert node_frame.num_rows == 2
 
   def test_edge_empty_labels_schema(self):
     c = self.conn
     self.neo4j_driver.query(
         'CREATE ()-[:e1]->({int:1}), (:Node)-[:e2]->({str:"aaa"}), ({bool:True})-[:e3]->(:Node)').finalize()
     c.transfer_to_xgt(edges=['e1', 'e2', 'e3'])
-    node_frame = self.xgt.get_edge_frame('e1')
+    node_frame = self.xgt.get_frame('e1')
     res = self.xgt.run_job('match ()-[:e1]->(v) return v.int')
     assert node_frame.num_rows == 1
     assert res.get_data()[0][0] == 1
-    node_frame = self.xgt.get_edge_frame('e2')
+    node_frame = self.xgt.get_frame('e2')
     res = self.xgt.run_job('match ()-[:e2]->(v) return v.str')
     assert node_frame.num_rows == 1
     assert res.get_data()[0][0] == "aaa"
-    node_frame = self.xgt.get_edge_frame('e3')
+    node_frame = self.xgt.get_frame('e3')
     res = self.xgt.run_job('match (v)-[:e3]->() return v.bool')
     assert node_frame.num_rows == 1
     assert res.get_data()[0][0] == True
-    node_frame = self.xgt.get_vertex_frame('unlabeled')
+    node_frame = self.xgt.get_frame('unlabeled')
     assert node_frame.num_rows == 4
-    node_frame = self.xgt.get_vertex_frame('Node')
+    node_frame = self.xgt.get_frame('Node')
     assert node_frame.num_rows == 2
 
   def test_map_edge_empty_labels(self):
     c = self.conn
     self.neo4j_driver.query(
         'CREATE ()-[:e1]->(), (:Node)-[:e2]->(), ()-[:e3]->(:Node)').finalize()
     c.transfer_to_xgt(vertices=[('', 'custom_empty'), ('Node', 'custom_Node')], edges=[('e1', 'edge1'), ('e2', 'edge2'), 'e3'])
-    node_frame = self.xgt.get_edge_frame('edge1')
+    node_frame = self.xgt.get_frame('edge1')
     assert node_frame.num_rows == 1
-    node_frame = self.xgt.get_edge_frame('edge2')
+    node_frame = self.xgt.get_frame('edge2')
     assert node_frame.num_rows == 1
-    node_frame = self.xgt.get_edge_frame('e3')
+    node_frame = self.xgt.get_frame('e3')
     assert node_frame.num_rows == 1
-    node_frame = self.xgt.get_vertex_frame('custom_empty')
+    node_frame = self.xgt.get_frame('custom_empty')
     assert node_frame.num_rows == 4
-    node_frame = self.xgt.get_vertex_frame('custom_Node')
+    node_frame = self.xgt.get_frame('custom_Node')
     assert node_frame.num_rows == 2
     with self.assertRaises(xgt.XgtNameError):
-        node_frame = self.xgt.get_vertex_frame('unlabeled')
+        node_frame = self.xgt.get_frame('unlabeled')
     with self.assertRaises(xgt.XgtNameError):
-        node_frame = self.xgt.get_vertex_frame('Node')
+        node_frame = self.xgt.get_frame('Node')
 
   def test_edge_empty_labels_schema_no_implicit(self):
     c = self.conn
     self.neo4j_driver.query(
         'CREATE ()-[:e1]->({int:1}), (:Node)-[:e2]->({str:"aaa"}), ({bool:True})-[:e3]->(:Node)').finalize()
     c.transfer_to_xgt(vertices=['', 'Node'])
     c.transfer_to_xgt(edges=['e1', 'e2', 'e3'], append=True, import_edge_nodes=False)
-    node_frame = self.xgt.get_edge_frame('e1')
+    node_frame = self.xgt.get_frame('e1')
     res = self.xgt.run_job('match ()-[:e1]->(v) return v.int')
     assert node_frame.num_rows == 1
     assert res.get_data()[0][0] == 1
-    node_frame = self.xgt.get_edge_frame('e2')
+    node_frame = self.xgt.get_frame('e2')
     res = self.xgt.run_job('match ()-[:e2]->(v) return v.str')
     assert node_frame.num_rows == 1
     assert res.get_data()[0][0] == "aaa"
-    node_frame = self.xgt.get_edge_frame('e3')
+    node_frame = self.xgt.get_frame('e3')
     res = self.xgt.run_job('match (v)-[:e3]->() return v.bool')
     assert node_frame.num_rows == 1
     assert res.get_data()[0][0] == True
-    node_frame = self.xgt.get_vertex_frame('unlabeled')
+    node_frame = self.xgt.get_frame('unlabeled')
     assert node_frame.num_rows == 4
-    node_frame = self.xgt.get_vertex_frame('Node')
+    node_frame = self.xgt.get_frame('Node')
     assert node_frame.num_rows == 2
 
   def test_query_translator_loop_data(self):
     self.neo4j_driver.query("create (a:Node{int:1})-[b:EDGE{int:1}]->(a)").finalize()
     query = "match(a) return a"
     assert query == self.conn.translate_query(query)
     query = "match(a:Node) return a"
```

### Comparing `trovares_connector-1.7.0/test/test_odbc_connector.py` & `trovares_connector-2.0.0/test/test_odbc_connector.py`

 * *Files 9% similar despite different names*

```diff
@@ -70,136 +70,136 @@
                    "TestDatetime DATETIME, TestTimestamp TIMESTAMP NULL, TestTime TIME, TestYear YEAR)")
     cursor.execute("INSERT INTO test VALUES (True, 32, 5000, 1.7, 1.98, 'vdxs', 'String', 1.78976, '1989-05-06', '1986-05-06 12:56:34', "
                    "'1989-05-06 12:56:34', '12:56:34', 1999)")
     cursor.execute("INSERT INTO test VALUES (NULL, NULL, NULL, NULL, NULL, NULL, NULL, NULL, NULL, NULL, NULL, NULL, NULL)")
     self.odbc_driver.commit()
 
     self.conn.transfer_to_xgt(tables = ['test'])
-    assert self.xgt.get_table_frame('test').num_rows == 2
-    print(self.xgt.get_table_frame('test').get_data())
+    assert self.xgt.get_frame('test').num_rows == 2
+    print(self.xgt.get_frame('test').get_data())
 
   def test_rename(self):
     cursor = self.odbc_driver.cursor()
     cursor.execute("CREATE TABLE test (Value1 INT, Value2 INT, Value3 varchar(255))")
     cursor.execute("INSERT INTO test VALUES (0, 0, 'hello')")
     self.odbc_driver.commit()
 
     self.conn.transfer_to_xgt(tables = [('test','test1')])
-    assert self.xgt.get_table_frame('test1').num_rows == 1
-    print(self.xgt.get_table_frame('test1').get_data())
+    assert self.xgt.get_frame('test1').num_rows == 1
+    print(self.xgt.get_frame('test1').get_data())
 
     self.conn.transfer_to_xgt(tables = [('test', {'frame' : 'test2'})])
-    assert self.xgt.get_table_frame('test2').num_rows == 1
-    print(self.xgt.get_table_frame('test2').get_data())
+    assert self.xgt.get_frame('test2').num_rows == 1
+    print(self.xgt.get_frame('test2').get_data())
 
   def test_vertex(self):
     cursor = self.odbc_driver.cursor()
     cursor.execute("CREATE TABLE test (Value1 INT, Value2 INT, Value3 varchar(255))")
     cursor.execute("INSERT INTO test VALUES (0, 0, 'hola')")
     cursor.execute("INSERT INTO test VALUES (1, 0, 'adios')")
     self.odbc_driver.commit()
 
     self.conn.transfer_to_xgt(tables = [('test', (0,))])
-    assert self.xgt.get_vertex_frame('test').num_rows == 2
-    print(self.xgt.get_vertex_frame('test').get_data())
+    assert self.xgt.get_frame('test').num_rows == 2
+    print(self.xgt.get_frame('test').get_data())
 
     self.conn.transfer_to_xgt(tables = [('test','test1', (0,))])
-    assert self.xgt.get_vertex_frame('test1').num_rows == 2
-    print(self.xgt.get_vertex_frame('test1').get_data())
+    assert self.xgt.get_frame('test1').num_rows == 2
+    print(self.xgt.get_frame('test1').get_data())
 
     self.conn.transfer_to_xgt(tables = [('test','test2', ('Value1',))])
-    assert self.xgt.get_vertex_frame('test2').num_rows == 2
-    print(self.xgt.get_vertex_frame('test2').get_data())
+    assert self.xgt.get_frame('test2').num_rows == 2
+    print(self.xgt.get_frame('test2').get_data())
 
     self.conn.transfer_to_xgt(tables = [('test', {'frame' : 'test3', 'key' : 0 } )])
-    assert self.xgt.get_vertex_frame('test3').num_rows == 2
-    print(self.xgt.get_vertex_frame('test3').get_data())
+    assert self.xgt.get_frame('test3').num_rows == 2
+    print(self.xgt.get_frame('test3').get_data())
 
     self.conn.transfer_to_xgt(tables = [('test', {'frame' : 'test4', 'key' : 'Value1' } )])
-    assert self.xgt.get_vertex_frame('test4').num_rows == 2
-    print(self.xgt.get_vertex_frame('test4').get_data())
+    assert self.xgt.get_frame('test4').num_rows == 2
+    print(self.xgt.get_frame('test4').get_data())
 
   def test_edge(self):
     cursor = self.odbc_driver.cursor()
     cursor.execute("CREATE TABLE test (Value1 INT, Value2 INT, Value3 varchar(255))")
     cursor.execute("INSERT INTO test VALUES (0, 0, 'hola')")
     cursor.execute("INSERT INTO test VALUES (1, 0, 'adios')")
     self.odbc_driver.commit()
 
     self.conn.transfer_to_xgt(tables = [('test', ('Vertex', 'Vertex', 0, 1))], easy_edges=True)
-    assert self.xgt.get_edge_frame('test').num_rows == 2
-    print(self.xgt.get_edge_frame('test').get_data())
+    assert self.xgt.get_frame('test').num_rows == 2
+    print(self.xgt.get_frame('test').get_data())
 
     self.conn.transfer_to_xgt(tables = [('test','test1', ('Vertex', 'Vertex', 0, 1))])
-    assert self.xgt.get_edge_frame('test1').num_rows == 2
-    print(self.xgt.get_edge_frame('test1').get_data())
+    assert self.xgt.get_frame('test1').num_rows == 2
+    print(self.xgt.get_frame('test1').get_data())
 
     self.conn.transfer_to_xgt(tables = [('test', 'Vertex1', (0,)), ('test','test2', ('Vertex1', 'Vertex1', 'Value1', 'Value2'))])
-    assert self.xgt.get_edge_frame('test2').num_rows == 2
-    print(self.xgt.get_edge_frame('test2').get_data())
+    assert self.xgt.get_frame('test2').num_rows == 2
+    print(self.xgt.get_frame('test2').get_data())
 
     self.conn.transfer_to_xgt(tables = [('test', {'frame' : 'test3', 'source' : 'Vertex', 'target' : 'Vertex', 'source_key' : 0, 'target_key' : 1 } )])
-    assert self.xgt.get_edge_frame('test3').num_rows == 2
-    print(self.xgt.get_edge_frame('test3').get_data())
+    assert self.xgt.get_frame('test3').num_rows == 2
+    print(self.xgt.get_frame('test3').get_data())
 
     self.conn.transfer_to_xgt(tables = [('test', {'frame' : 'test4', 'source' : 'Vertex', 'target' : 'Vertex', 'source_key' : 'Value1', 'target_key' : 'Value2' } )])
-    assert self.xgt.get_edge_frame('test4').num_rows == 2
-    print(self.xgt.get_edge_frame('test4').get_data())
+    assert self.xgt.get_frame('test4').num_rows == 2
+    print(self.xgt.get_frame('test4').get_data())
 
   def test_append(self):
     cursor = self.odbc_driver.cursor()
     cursor.execute("CREATE TABLE test (Value1 INT, Value2 INT, Value3 varchar(255))")
     cursor.execute("INSERT INTO test VALUES (0, 0, 'hola')")
     self.odbc_driver.commit()
 
     self.conn.transfer_to_xgt(tables = [('test', ('Vertex', 'Vertex', 0, 1))], easy_edges=True)
-    assert self.xgt.get_edge_frame('test').num_rows == 1
-    print(self.xgt.get_edge_frame('test').get_data())
+    assert self.xgt.get_frame('test').num_rows == 1
+    print(self.xgt.get_frame('test').get_data())
 
     cursor.execute("DROP TABLE IF EXISTS test")
     cursor.execute("CREATE TABLE test (Value1 INT, Value2 INT, Value3 varchar(255))")
     cursor.execute("INSERT INTO test VALUES (1, 0, 'adios')")
     self.odbc_driver.commit()
     self.conn.transfer_to_xgt(tables = [('test', ('Vertex', 'Vertex', 0, 1))], append=True)
-    assert self.xgt.get_edge_frame('test').num_rows == 2
-    print(self.xgt.get_edge_frame('test').get_data())
+    assert self.xgt.get_frame('test').num_rows == 2
+    print(self.xgt.get_frame('test').get_data())
 
   def test_dropping(self):
     c = self.conn
     cursor = self.odbc_driver.cursor()
     cursor.execute("CREATE TABLE Node (id INT)")
     cursor.execute("INSERT INTO Node VALUES (0)")
     cursor.execute("CREATE TABLE Relationship (Value1 INT, Value2 INT, Value3 varchar(255))")
     cursor.execute("INSERT INTO Relationship VALUES (0, 0, 'hola')")
     self.odbc_driver.commit()
 
     xgt_schema1 = self.conn.get_xgt_schemas(tables = [('Node', (0,)), ('Relationship', ('Node', 'Node', 0, 1))])
     xgt_schema2 = self.conn.get_xgt_schemas(tables = [('Node', (0,))])
 
     c.create_xgt_schemas(xgt_schema1)
-    self.xgt.get_vertex_frame('Node')
-    self.xgt.get_edge_frame('Relationship')
+    self.xgt.get_frame('Node')
+    self.xgt.get_frame('Relationship')
 
     c.create_xgt_schemas(xgt_schema1)
-    self.xgt.get_vertex_frame('Node')
-    self.xgt.get_edge_frame('Relationship')
+    self.xgt.get_frame('Node')
+    self.xgt.get_frame('Relationship')
 
     with self.assertRaises(xgt.XgtFrameDependencyError):
         c.create_xgt_schemas(xgt_schema2)
     c.create_xgt_schemas(xgt_schema2, force = True)
-    self.xgt.get_vertex_frame('Node')
+    self.xgt.get_frame('Node')
     with self.assertRaises(xgt.XgtNameError):
-        self.xgt.get_edge_frame('Relationship')
+        self.xgt.get_frame('Relationship')
 
   def test_transfer_no_data(self):
     c = self.conn
     cursor = self.odbc_driver.cursor()
     cursor.execute("CREATE TABLE Node (id INT)")
     self.conn.transfer_to_xgt(tables = [('Node', (0,))])
-    assert self.xgt.get_vertex_frame('Node').num_rows == 0
+    assert self.xgt.get_frame('Node').num_rows == 0
 
   def test_transfer_to_odbc(self):
     cursor = self.odbc_driver.cursor()
     create_statement = """CREATE TABLE test (TestBool BOOL, TestInt INT, TestBigInt BIGINT, TestFloat FLOAT(24), TestDouble FLOAT(53),
                        TestFixedString char(5), TestString varchar(255), TestDecimal DECIMAL(10, 6), TestDate DATE,
                        TestDateTime DATETIME, TestTimestamp TIMESTAMP NULL, TestTime TIME, TestYear YEAR)"""
     cursor.execute(create_statement)
@@ -209,16 +209,16 @@
     self.odbc_driver.commit()
 
     self.conn.transfer_to_xgt(tables = ['test'])
     cursor.execute("DROP TABLE IF EXISTS test")
     cursor.execute(create_statement)
     self.conn.transfer_to_odbc(tables = ['test'])
     self.conn.transfer_to_xgt(tables = ['test'])
-    assert self.xgt.get_table_frame('test').num_rows == 2
-    print(self.xgt.get_table_frame('test').get_data())
+    assert self.xgt.get_frame('test').num_rows == 2
+    print(self.xgt.get_frame('test').get_data())
 
   def test_transfer_to_odbc_rename(self):
     cursor = self.odbc_driver.cursor()
     create_statement = """CREATE TABLE test (TestBool BOOL, TestInt INT, TestBigInt BIGINT, TestFloat FLOAT(24), TestDouble FLOAT(53),
                        TestFixedString char(5), TestString varchar(255), TestDecimal DECIMAL(10, 6), TestDate DATE,
                        TestDateTime DATETIME, TestTimestamp TIMESTAMP NULL, TestTime TIME, TestYear YEAR)"""
     cursor.execute(create_statement)
@@ -227,16 +227,16 @@
     self.odbc_driver.commit()
 
     self.conn.transfer_to_xgt(tables = [('test', 'test1')])
     cursor.execute("DROP TABLE IF EXISTS test")
     cursor.execute(create_statement)
     self.conn.transfer_to_odbc(tables = [('test1', 'test')])
     self.conn.transfer_to_xgt(tables = ['test'])
-    assert self.xgt.get_table_frame('test').num_rows == 1
-    print(self.xgt.get_table_frame('test').get_data())
+    assert self.xgt.get_frame('test').num_rows == 1
+    print(self.xgt.get_frame('test').get_data())
 
   def test_transfer_to_odbc_vertex(self):
     cursor = self.odbc_driver.cursor()
     create_statement = """CREATE TABLE test (TestBool BOOL, TestInt INT, TestBigInt BIGINT, TestFloat FLOAT(24), TestDouble FLOAT(53),
                        TestFixedString char(5), TestString varchar(255), TestDecimal DECIMAL(10, 6), TestDate DATE,
                        TestDateTime DATETIME, TestTimestamp TIMESTAMP NULL, TestTime TIME, TestYear YEAR)"""
     cursor.execute(create_statement)
@@ -245,16 +245,16 @@
     self.odbc_driver.commit()
 
     self.conn.transfer_to_xgt(tables = [('test', (0,))])
     cursor.execute("DROP TABLE IF EXISTS test")
     cursor.execute(create_statement)
     self.conn.transfer_to_odbc(vertices = ['test'])
     self.conn.transfer_to_xgt(tables = [('test', (0,))])
-    assert self.xgt.get_vertex_frame('test').num_rows == 1
-    print(self.xgt.get_vertex_frame('test').get_data())
+    assert self.xgt.get_frame('test').num_rows == 1
+    print(self.xgt.get_frame('test').get_data())
 
   def test_transfer_to_odbc_vertex_rename(self):
     cursor = self.odbc_driver.cursor()
     create_statement = """CREATE TABLE test (TestBool BOOL, TestInt INT, TestBigInt BIGINT, TestFloat FLOAT(24), TestDouble FLOAT(53),
                        TestFixedString char(5), TestString varchar(255), TestDecimal DECIMAL(10, 6), TestDate DATE,
                        TestDateTime DATETIME, TestTimestamp TIMESTAMP NULL, TestTime TIME, TestYear YEAR)"""
     cursor.execute(create_statement)
@@ -263,16 +263,16 @@
     self.odbc_driver.commit()
 
     self.conn.transfer_to_xgt(tables = [('test', 'test1', (0,))])
     cursor.execute("DROP TABLE IF EXISTS test")
     cursor.execute(create_statement)
     self.conn.transfer_to_odbc(vertices = [('test1', 'test')])
     self.conn.transfer_to_xgt(tables = [('test', (0,))])
-    assert self.xgt.get_vertex_frame('test').num_rows == 1
-    print(self.xgt.get_vertex_frame('test').get_data())
+    assert self.xgt.get_frame('test').num_rows == 1
+    print(self.xgt.get_frame('test').get_data())
 
   def test_transfer_to_odbc_edges(self):
     cursor = self.odbc_driver.cursor()
     create_statement = """CREATE TABLE test (TestBool BOOL, TestInt INT, TestBigInt BIGINT, TestFloat FLOAT(24), TestDouble FLOAT(53),
                        TestFixedString char(5), TestString varchar(255), TestDecimal DECIMAL(10, 6), TestDate DATE,
                        TestDateTime DATETIME, TestTimestamp TIMESTAMP NULL, TestTime TIME, TestYear YEAR)"""
     cursor.execute(create_statement)
@@ -281,16 +281,16 @@
     self.odbc_driver.commit()
 
     self.conn.transfer_to_xgt(tables = [('test', ('Vertex1', 'Vertex2', 1, 2))], easy_edges = True)
     cursor.execute("DROP TABLE IF EXISTS test")
     cursor.execute(create_statement)
     self.conn.transfer_to_odbc(edges = ['test'])
     self.conn.transfer_to_xgt(tables = [('test', ('Vertex1', 'Vertex2', 1, 2))], easy_edges = True)
-    assert self.xgt.get_edge_frame('test').num_rows == 1
-    print(self.xgt.get_edge_frame('test').get_data())
+    assert self.xgt.get_frame('test').num_rows == 1
+    print(self.xgt.get_frame('test').get_data())
 
   def test_transfer_to_odbc_edges_rename(self):
     cursor = self.odbc_driver.cursor()
     create_statement = """CREATE TABLE test (TestBool BOOL, TestInt INT, TestBigInt BIGINT, TestFloat FLOAT(24), TestDouble FLOAT(53),
                        TestFixedString char(5), TestString varchar(255), TestDecimal DECIMAL(10, 6), TestDate DATE,
                        TestDateTime DATETIME, TestTimestamp TIMESTAMP NULL, TestTime TIME, TestYear YEAR)"""
     cursor.execute(create_statement)
@@ -299,103 +299,103 @@
     self.odbc_driver.commit()
 
     self.conn.transfer_to_xgt(tables=[('test', 'test1', ('Vertex1', 'Vertex2', 1, 2))], easy_edges = True)
     cursor.execute("DROP TABLE IF EXISTS test")
     cursor.execute(create_statement)
     self.conn.transfer_to_odbc(edges = [('test1', 'test')])
     self.conn.transfer_to_xgt(tables = [('test', ('Vertex1', 'Vertex2', 1, 2))], easy_edges = True, force = True)
-    assert self.xgt.get_edge_frame('test').num_rows == 1
-    print(self.xgt.get_edge_frame('test').get_data())
+    assert self.xgt.get_frame('test').num_rows == 1
+    print(self.xgt.get_frame('test').get_data())
 
   def test_transfer_query(self):
     cursor = self.odbc_driver.cursor()
     cursor.execute("CREATE TABLE test (TestBool BOOL, TestInt INT, TestBigInt BIGINT, TestFloat FLOAT(24), TestDouble FLOAT(53), "
                    "TestFixedString char(5), TestString varchar(255), TestDecimal DECIMAL(10, 6), TestDate DATE, "
                    "TestDatetime DATETIME, TestTimestamp TIMESTAMP NULL, TestTime TIME, TestYear YEAR)")
     cursor.execute("INSERT INTO test VALUES (True, 32, 5000, 1.7, 1.98, 'vdxs', 'String', 1.78976, '1989-05-06', '1986-05-06 12:56:34', "
                    "'1989-05-06 12:56:34', '12:56:34', 1999)")
     cursor.execute("INSERT INTO test VALUES (NULL, NULL, NULL, NULL, NULL, NULL, NULL, NULL, NULL, NULL, NULL, NULL, NULL)")
     self.odbc_driver.commit()
 
     self.conn.transfer_query_to_xgt("SELECT * FROM test", mapping = 'my_test')
-    assert self.xgt.get_table_frame('my_test').num_rows == 2
-    print(self.xgt.get_table_frame('my_test').get_data())
+    assert self.xgt.get_frame('my_test').num_rows == 2
+    print(self.xgt.get_frame('my_test').get_data())
 
   def test_vertex_query(self):
     cursor = self.odbc_driver.cursor()
     cursor.execute("CREATE TABLE test (Value1 INT, Value2 INT, Value3 varchar(255))")
     cursor.execute("INSERT INTO test VALUES (0, 0, 'hola')")
     cursor.execute("INSERT INTO test VALUES (1, 0, 'adios')")
     self.odbc_driver.commit()
 
     self.conn.transfer_query_to_xgt("SELECT * FROM test", mapping = ('test', (0,)))
-    assert self.xgt.get_vertex_frame('test').num_rows == 2
-    print(self.xgt.get_vertex_frame('test').get_data())
+    assert self.xgt.get_frame('test').num_rows == 2
+    print(self.xgt.get_frame('test').get_data())
 
     self.conn.transfer_query_to_xgt("SELECT * FROM test", mapping = ('test1', (0,)))
-    assert self.xgt.get_vertex_frame('test1').num_rows == 2
-    print(self.xgt.get_vertex_frame('test1').get_data())
+    assert self.xgt.get_frame('test1').num_rows == 2
+    print(self.xgt.get_frame('test1').get_data())
 
     self.conn.transfer_query_to_xgt("SELECT * FROM test", mapping = ('test2', ('Value1',)))
-    assert self.xgt.get_vertex_frame('test2').num_rows == 2
-    print(self.xgt.get_vertex_frame('test2').get_data())
+    assert self.xgt.get_frame('test2').num_rows == 2
+    print(self.xgt.get_frame('test2').get_data())
 
     self.conn.transfer_query_to_xgt("SELECT * FROM test", mapping = ('test', {'frame' : 'test3', 'key' : 0 } ))
-    assert self.xgt.get_vertex_frame('test3').num_rows == 2
-    print(self.xgt.get_vertex_frame('test3').get_data())
+    assert self.xgt.get_frame('test3').num_rows == 2
+    print(self.xgt.get_frame('test3').get_data())
 
     self.conn.transfer_query_to_xgt("SELECT * FROM test", mapping = ('test', {'frame' : 'test4', 'key' : 'Value1' } ))
-    assert self.xgt.get_vertex_frame('test4').num_rows == 2
-    print(self.xgt.get_vertex_frame('test4').get_data())
+    assert self.xgt.get_frame('test4').num_rows == 2
+    print(self.xgt.get_frame('test4').get_data())
 
   def test_edge_query(self):
     cursor = self.odbc_driver.cursor()
     cursor.execute("CREATE TABLE test (Value1 INT, Value2 INT, Value3 varchar(255))")
     cursor.execute("INSERT INTO test VALUES (0, 0, 'hola')")
     cursor.execute("INSERT INTO test VALUES (1, 0, 'adios')")
     self.odbc_driver.commit()
 
     self.conn.transfer_query_to_xgt("SELECT * FROM test", mapping = ('test', ('Vertex', 'Vertex', 0, 1)), easy_edges=True)
-    assert self.xgt.get_edge_frame('test').num_rows == 2
-    print(self.xgt.get_edge_frame('test').get_data())
+    assert self.xgt.get_frame('test').num_rows == 2
+    print(self.xgt.get_frame('test').get_data())
 
     self.conn.transfer_query_to_xgt("SELECT * FROM test", mapping = ('test1', ('Vertex', 'Vertex', 0, 1)))
-    assert self.xgt.get_edge_frame('test1').num_rows == 2
-    print(self.xgt.get_edge_frame('test1').get_data())
+    assert self.xgt.get_frame('test1').num_rows == 2
+    print(self.xgt.get_frame('test1').get_data())
 
     self.conn.transfer_query_to_xgt("SELECT * FROM test", mapping = ('Vertex1', (0,)))
     self.conn.transfer_query_to_xgt("SELECT * FROM test", mapping = ('test', 'test2', ('Vertex1', 'Vertex1', 'Value1', 'Value2')))
-    assert self.xgt.get_edge_frame('test2').num_rows == 2
-    print(self.xgt.get_edge_frame('test2').get_data())
+    assert self.xgt.get_frame('test2').num_rows == 2
+    print(self.xgt.get_frame('test2').get_data())
 
     self.conn.transfer_query_to_xgt("SELECT * FROM test", mapping = ('test', {'frame' : 'test3', 'source' : 'Vertex', 'target' : 'Vertex', 'source_key' : 0, 'target_key' : 1 }))
-    assert self.xgt.get_edge_frame('test3').num_rows == 2
-    print(self.xgt.get_edge_frame('test3').get_data())
+    assert self.xgt.get_frame('test3').num_rows == 2
+    print(self.xgt.get_frame('test3').get_data())
 
     self.conn.transfer_query_to_xgt("SELECT * FROM test", mapping = ('test', {'frame' : 'test4', 'source' : 'Vertex', 'target' : 'Vertex', 'source_key' : 'Value1', 'target_key' : 'Value2' }))
-    assert self.xgt.get_edge_frame('test4').num_rows == 2
-    print(self.xgt.get_edge_frame('test4').get_data())
+    assert self.xgt.get_frame('test4').num_rows == 2
+    print(self.xgt.get_frame('test4').get_data())
 
   def test_append_query(self):
     cursor = self.odbc_driver.cursor()
     cursor.execute("CREATE TABLE test (Value1 INT, Value2 INT, Value3 varchar(255))")
     cursor.execute("INSERT INTO test VALUES (0, 0, 'hola')")
     self.odbc_driver.commit()
 
     self.conn.transfer_query_to_xgt("SELECT * FROM test", mapping = ('test', ('Vertex', 'Vertex', 0, 1)), easy_edges=True)
-    assert self.xgt.get_edge_frame('test').num_rows == 1
-    print(self.xgt.get_edge_frame('test').get_data())
+    assert self.xgt.get_frame('test').num_rows == 1
+    print(self.xgt.get_frame('test').get_data())
 
     cursor.execute("DROP TABLE IF EXISTS test")
     cursor.execute("CREATE TABLE test (Value1 INT, Value2 INT, Value3 varchar(255))")
     cursor.execute("INSERT INTO test VALUES (1, 0, 'adios')")
     self.odbc_driver.commit()
     self.conn.transfer_query_to_xgt("SELECT * FROM test", mapping = ('test', ('Vertex', 'Vertex', 0, 1)), append=True)
-    assert self.xgt.get_edge_frame('test').num_rows == 2
-    print(self.xgt.get_edge_frame('test').get_data())
+    assert self.xgt.get_frame('test').num_rows == 2
+    print(self.xgt.get_frame('test').get_data())
 
   def test_transfer_no_data_query(self):
     c = self.conn
     cursor = self.odbc_driver.cursor()
     cursor.execute("CREATE TABLE Node (id INT)")
     self.conn.transfer_query_to_xgt("SELECT * FROM Node", mapping = ('Node', (0,)))
-    assert self.xgt.get_vertex_frame('Node').num_rows == 0
+    assert self.xgt.get_frame('Node').num_rows == 0
```

