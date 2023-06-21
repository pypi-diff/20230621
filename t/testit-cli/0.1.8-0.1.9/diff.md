# Comparing `tmp/testit-cli-0.1.8.tar.gz` & `tmp/testit-cli-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testit-cli-0.1.8.tar", last modified: Wed Jun  7 14:56:29 2023, max compression
+gzip compressed data, was "testit-cli-0.1.9.tar", last modified: Wed Jun 21 11:00:59 2023, max compression
```

## Comparing `testit-cli-0.1.8.tar` & `testit-cli-0.1.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:56:29.096231 testit-cli-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-07 14:56:19.000000 testit-cli-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-07 14:56:29.096231 testit-cli-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-07 14:56:19.000000 testit-cli-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 14:56:29.096231 testit-cli-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-07 14:56:19.000000 testit-cli-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:56:29.092231 testit-cli-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:56:29.096231 testit-cli-0.1.8/src/testit_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 14:56:19.000000 testit-cli-0.1.8/src/testit_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-07 14:56:19.000000 testit-cli-0.1.8/src/testit_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-06-07 14:56:19.000000 testit-cli-0.1.8/src/testit_cli/apiclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-06-07 14:56:19.000000 testit-cli-0.1.8/src/testit_cli/args_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-06-07 14:56:19.000000 testit-cli-0.1.8/src/testit_cli/configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-07 14:56:19.000000 testit-cli-0.1.8/src/testit_cli/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-06-07 14:56:19.000000 testit-cli-0.1.8/src/testit_cli/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-07 14:56:19.000000 testit-cli-0.1.8/src/testit_cli/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:56:29.096231 testit-cli-0.1.8/src/testit_cli/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 14:56:19.000000 testit-cli-0.1.8/src/testit_cli/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-07 14:56:19.000000 testit-cli-0.1.8/src/testit_cli/models/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-07 14:56:19.000000 testit-cli-0.1.8/src/testit_cli/models/mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-07 14:56:19.000000 testit-cli-0.1.8/src/testit_cli/models/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-07 14:56:19.000000 testit-cli-0.1.8/src/testit_cli/models/testcase.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-07 14:56:19.000000 testit-cli-0.1.8/src/testit_cli/models/testrun.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-06-07 14:56:19.000000 testit-cli-0.1.8/src/testit_cli/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-06-07 14:56:19.000000 testit-cli-0.1.8/src/testit_cli/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:56:29.096231 testit-cli-0.1.8/src/testit_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-07 14:56:29.000000 testit-cli-0.1.8/src/testit_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-07 14:56:29.000000 testit-cli-0.1.8/src/testit_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 14:56:29.000000 testit-cli-0.1.8/src/testit_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-07 14:56:29.000000 testit-cli-0.1.8/src/testit_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-07 14:56:29.000000 testit-cli-0.1.8/src/testit_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-07 14:56:29.000000 testit-cli-0.1.8/src/testit_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:00:59.654245 testit-cli-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-21 11:00:45.000000 testit-cli-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-21 11:00:59.654245 testit-cli-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-21 11:00:45.000000 testit-cli-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 11:00:59.654245 testit-cli-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-21 11:00:45.000000 testit-cli-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:00:59.646245 testit-cli-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:00:59.650245 testit-cli-0.1.9/src/testit_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 11:00:45.000000 testit-cli-0.1.9/src/testit_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-21 11:00:45.000000 testit-cli-0.1.9/src/testit_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-06-21 11:00:45.000000 testit-cli-0.1.9/src/testit_cli/apiclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-06-21 11:00:45.000000 testit-cli-0.1.9/src/testit_cli/args_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-06-21 11:00:45.000000 testit-cli-0.1.9/src/testit_cli/configurator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-21 11:00:45.000000 testit-cli-0.1.9/src/testit_cli/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-06-21 11:00:45.000000 testit-cli-0.1.9/src/testit_cli/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-21 11:00:45.000000 testit-cli-0.1.9/src/testit_cli/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:00:59.654245 testit-cli-0.1.9/src/testit_cli/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 11:00:45.000000 testit-cli-0.1.9/src/testit_cli/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-21 11:00:45.000000 testit-cli-0.1.9/src/testit_cli/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-21 11:00:45.000000 testit-cli-0.1.9/src/testit_cli/models/mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-21 11:00:45.000000 testit-cli-0.1.9/src/testit_cli/models/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-21 11:00:45.000000 testit-cli-0.1.9/src/testit_cli/models/testcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-21 11:00:45.000000 testit-cli-0.1.9/src/testit_cli/models/testrun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-06-21 11:00:45.000000 testit-cli-0.1.9/src/testit_cli/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-06-21 11:00:45.000000 testit-cli-0.1.9/src/testit_cli/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:00:59.654245 testit-cli-0.1.9/src/testit_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-21 11:00:59.000000 testit-cli-0.1.9/src/testit_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-21 11:00:59.000000 testit-cli-0.1.9/src/testit_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 11:00:59.000000 testit-cli-0.1.9/src/testit_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-21 11:00:59.000000 testit-cli-0.1.9/src/testit_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-21 11:00:59.000000 testit-cli-0.1.9/src/testit_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-21 11:00:59.000000 testit-cli-0.1.9/src/testit_cli.egg-info/top_level.txt
```

### Comparing `testit-cli-0.1.8/LICENSE` & `testit-cli-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `testit-cli-0.1.8/PKG-INFO` & `testit-cli-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-cli
-Version: 0.1.8
+Version: 0.1.9
 Summary: This tool is the command line wrapper of Test IT allowing you to upload the test results in real time to Test IT
 Home-page: https://pypi.org/project/testit/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `testit-cli-0.1.8/setup.py` & `testit-cli-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='testit-cli',
-    version='0.1.8',
+    version='0.1.9',
     description='This tool is the command line wrapper of Test IT allowing you to upload the test results in real time '
                 'to Test IT',
     long_description=open('README.md', "r").read(),
     long_description_content_type="text/markdown",
     url='https://pypi.org/project/testit/',
     author='Integration team',
     author_email='integrations@testit.software',
```

### Comparing `testit-cli-0.1.8/src/testit_cli/__main__.py` & `testit-cli-0.1.9/src/testit_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `testit-cli-0.1.8/src/testit_cli/apiclient.py` & `testit-cli-0.1.9/src/testit_cli/apiclient.py`

 * *Files identical despite different names*

### Comparing `testit-cli-0.1.8/src/testit_cli/args_parser.py` & `testit-cli-0.1.9/src/testit_cli/args_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,27 +18,28 @@
             description="""This tool is the command line wrapper of Test IT
                      allowing you to upload the test results in real time to Test IT""",
         )
 
     def parse_args(self):
         """Function parses commandline arguments and returns config."""
         args = self.parser.parse_args()
-        if sys.argv[0].split("\\")[-1] == "testit":
+        if len(sys.argv) == 1:
             self.parser.print_help()
             sys.exit(0)
         return Config(
             Mode(args.mode),
             args.url,
             args.token,
             args.project_id,
             args.configuration_id,
             args.testrun_id,
             args.testrun_name,
             args.separator,
             args.namespace,
+            args.classname,
             args.results,
             args.debug,
             args.output,
         )
 
     def __add_args(self):
         self.parser.add_argument(
@@ -112,14 +113,22 @@
             "--namespace",
             action="store",
             dest="namespace",
             metavar="NameSpace01",
             help="Set namespace",
         )
         self.parser.add_argument(
+            "-cn",
+            "--classname",
+            action="store",
+            dest="classname",
+            metavar="ClassName01",
+            help="Set classname",
+        )
+        self.parser.add_argument(
             "-r",
             "--results",
             action="store",
             dest="results",
             metavar="DIR",
             default=None,
             help="Set directory with results file",
```

### Comparing `testit-cli-0.1.8/src/testit_cli/configurator.py` & `testit-cli-0.1.9/src/testit_cli/configurator.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,18 @@
         """Function returns separator."""
         return self.__config.separator
 
     def get_namespace(self):
         """Function returns namespace."""
         return self.__config.namespace
 
+    def get_classname(self):
+        """Function returns classname."""
+        return self.__config.classname
+
     def get_mode(self):
         """Function returns mode."""
         return self.__config.mode
 
     def get_output(self):
         """Function returns output file path."""
         return self.__config.output
```

### Comparing `testit-cli-0.1.8/src/testit_cli/converter.py` & `testit-cli-0.1.9/src/testit_cli/converter.py`

 * *Files identical despite different names*

### Comparing `testit-cli-0.1.8/src/testit_cli/importer.py` & `testit-cli-0.1.9/src/testit_cli/importer.py`

 * *Files identical despite different names*

### Comparing `testit-cli-0.1.8/src/testit_cli/models/testcase.py` & `testit-cli-0.1.9/src/testit_cli/models/testcase.py`

 * *Files identical despite different names*

### Comparing `testit-cli-0.1.8/src/testit_cli/parser.py` & `testit-cli-0.1.9/src/testit_cli/parser.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,38 +9,43 @@
 
 
 class Parser:
     def __init__(self, config: Configurator):
         self.__path_to_results = config.get_path()
         self.__separator = config.get_separator()
         self.__namespace = config.get_namespace()
+        self.__classname = config.get_classname()
 
     def read_file(self):  # noqa: C901
         results = []
         files = self.__get_files()
 
         for file in files:
 
             xml = minidom.parse(file)
             testcases = xml.getElementsByTagName("testcase")
 
             for elem in testcases:
                 name = elem.attributes["name"].value
                 duration = float(elem.attributes["time"].value) * 1000 if "time" in elem.attributes else 0
+                name_space = "namespace"
+                class_name = "classname"
 
                 if self.__separator is not None and self.__separator in elem.attributes["classname"].value:
                     class_name = elem.attributes["classname"].value.split(self.__separator)[-1]
                     name_space = elem.attributes["classname"].value[:-(len(class_name) + 1)]
-                else:
+                elif "classname" in elem.attributes:
                     class_name = elem.attributes["classname"].value
-                    name_space = "namespace"
 
                 if self.__namespace is not None:
                     name_space = self.__namespace
 
+                if self.__classname is not None:
+                    class_name = self.__classname
+
                 testcase = TestCase(name, name_space, class_name, duration)
 
                 if elem.childNodes is not None:
                     for child in elem.childNodes:
                         if child.nodeName == "error" or child.nodeName == "failure":
                             if "message" in child.attributes:
                                 testcase.set_message(child.attributes["message"].value)
```

### Comparing `testit-cli-0.1.8/src/testit_cli/service.py` & `testit-cli-0.1.9/src/testit_cli/service.py`

 * *Files identical despite different names*

### Comparing `testit-cli-0.1.8/src/testit_cli.egg-info/PKG-INFO` & `testit-cli-0.1.9/src/testit_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-cli
-Version: 0.1.8
+Version: 0.1.9
 Summary: This tool is the command line wrapper of Test IT allowing you to upload the test results in real time to Test IT
 Home-page: https://pypi.org/project/testit/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `testit-cli-0.1.8/src/testit_cli.egg-info/SOURCES.txt` & `testit-cli-0.1.9/src/testit_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

