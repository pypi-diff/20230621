# Comparing `tmp/prelude-cli-1.2.5.tar.gz` & `tmp/prelude-cli-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prelude-cli-1.2.5.tar", last modified: Thu Jun 15 14:40:17 2023, max compression
+gzip compressed data, was "prelude-cli-1.2.6.tar", last modified: Wed Jun 21 21:01:30 2023, max compression
```

## Comparing `prelude-cli-1.2.5.tar` & `prelude-cli-1.2.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-15 14:40:17.097532 prelude-cli-1.2.5/
--rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-cli-1.2.5/LICENSE
--rw-r--r--   0 pack       (501) staff       (20)       31 2023-01-24 13:01:01.000000 prelude-cli-1.2.5/MANIFEST.in
--rw-r--r--   0 pack       (501) staff       (20)      832 2023-06-15 14:40:17.097576 prelude-cli-1.2.5/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      391 2023-03-01 15:58:44.000000 prelude-cli-1.2.5/README.md
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-15 14:40:17.094597 prelude-cli-1.2.5/prelude_cli/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.2.5/prelude_cli/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)      775 2023-05-02 14:19:17.000000 prelude-cli-1.2.5/prelude_cli/cli.py
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-05-03 13:30:52.000000 prelude-cli-1.2.5/prelude_cli/spinner.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-15 14:40:17.095378 prelude-cli-1.2.5/prelude_cli/templates/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.2.5/prelude_cli/templates/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)      249 2023-06-01 16:01:25.000000 prelude-cli-1.2.5/prelude_cli/templates/template.go
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-15 14:40:17.097311 prelude-cli-1.2.5/prelude_cli/views/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.2.5/prelude_cli/views/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     4036 2023-06-06 22:22:58.000000 prelude-cli-1.2.5/prelude_cli/views/build.py
--rw-r--r--   0 pack       (501) staff       (20)      552 2023-02-08 14:42:44.000000 prelude-cli-1.2.5/prelude_cli/views/configure.py
--rw-r--r--   0 pack       (501) staff       (20)     7956 2023-06-12 21:16:47.000000 prelude-cli-1.2.5/prelude_cli/views/detect.py
--rw-r--r--   0 pack       (501) staff       (20)     3895 2023-06-12 21:16:47.000000 prelude-cli-1.2.5/prelude_cli/views/iam.py
--rw-r--r--   0 pack       (501) staff       (20)     2279 2023-05-18 19:30:30.000000 prelude-cli-1.2.5/prelude_cli/views/partner.py
--rw-r--r--   0 pack       (501) staff       (20)     1139 2023-05-03 13:30:52.000000 prelude-cli-1.2.5/prelude_cli/views/shared.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-15 14:40:17.095201 prelude-cli-1.2.5/prelude_cli.egg-info/
--rw-r--r--   0 pack       (501) staff       (20)      832 2023-06-15 14:40:17.000000 prelude-cli-1.2.5/prelude_cli.egg-info/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      598 2023-06-15 14:40:17.000000 prelude-cli-1.2.5/prelude_cli.egg-info/SOURCES.txt
--rw-r--r--   0 pack       (501) staff       (20)        1 2023-06-15 14:40:17.000000 prelude-cli-1.2.5/prelude_cli.egg-info/dependency_links.txt
--rw-r--r--   0 pack       (501) staff       (20)       48 2023-06-15 14:40:17.000000 prelude-cli-1.2.5/prelude_cli.egg-info/entry_points.txt
--rw-r--r--   0 pack       (501) staff       (20)       32 2023-06-15 14:40:17.000000 prelude-cli-1.2.5/prelude_cli.egg-info/requires.txt
--rw-r--r--   0 pack       (501) staff       (20)       12 2023-06-15 14:40:17.000000 prelude-cli-1.2.5/prelude_cli.egg-info/top_level.txt
--rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-cli-1.2.5/pyproject.toml
--rw-r--r--   0 pack       (501) staff       (20)      663 2023-06-15 14:40:17.097787 prelude-cli-1.2.5/setup.cfg
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-21 21:01:30.321853 prelude-cli-1.2.6/
+-rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-cli-1.2.6/LICENSE
+-rw-r--r--   0 pack       (501) staff       (20)       31 2023-01-24 13:01:01.000000 prelude-cli-1.2.6/MANIFEST.in
+-rw-r--r--   0 pack       (501) staff       (20)      832 2023-06-21 21:01:30.321897 prelude-cli-1.2.6/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      391 2023-03-01 15:58:44.000000 prelude-cli-1.2.6/README.md
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-21 21:01:30.318972 prelude-cli-1.2.6/prelude_cli/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.2.6/prelude_cli/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)      775 2023-05-02 14:19:17.000000 prelude-cli-1.2.6/prelude_cli/cli.py
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-05-03 13:30:52.000000 prelude-cli-1.2.6/prelude_cli/spinner.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-21 21:01:30.319836 prelude-cli-1.2.6/prelude_cli/templates/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.2.6/prelude_cli/templates/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)      249 2023-06-01 16:01:25.000000 prelude-cli-1.2.6/prelude_cli/templates/template.go
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-21 21:01:30.321648 prelude-cli-1.2.6/prelude_cli/views/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.2.6/prelude_cli/views/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     3997 2023-06-21 16:09:59.000000 prelude-cli-1.2.6/prelude_cli/views/build.py
+-rw-r--r--   0 pack       (501) staff       (20)      552 2023-02-08 14:42:44.000000 prelude-cli-1.2.6/prelude_cli/views/configure.py
+-rw-r--r--   0 pack       (501) staff       (20)     7956 2023-06-12 21:16:47.000000 prelude-cli-1.2.6/prelude_cli/views/detect.py
+-rw-r--r--   0 pack       (501) staff       (20)     3895 2023-06-12 21:16:47.000000 prelude-cli-1.2.6/prelude_cli/views/iam.py
+-rw-r--r--   0 pack       (501) staff       (20)     2279 2023-05-18 19:30:30.000000 prelude-cli-1.2.6/prelude_cli/views/partner.py
+-rw-r--r--   0 pack       (501) staff       (20)     1139 2023-05-03 13:30:52.000000 prelude-cli-1.2.6/prelude_cli/views/shared.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-21 21:01:30.319656 prelude-cli-1.2.6/prelude_cli.egg-info/
+-rw-r--r--   0 pack       (501) staff       (20)      832 2023-06-21 21:01:30.000000 prelude-cli-1.2.6/prelude_cli.egg-info/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      598 2023-06-21 21:01:30.000000 prelude-cli-1.2.6/prelude_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 pack       (501) staff       (20)        1 2023-06-21 21:01:30.000000 prelude-cli-1.2.6/prelude_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 pack       (501) staff       (20)       48 2023-06-21 21:01:30.000000 prelude-cli-1.2.6/prelude_cli.egg-info/entry_points.txt
+-rw-r--r--   0 pack       (501) staff       (20)       32 2023-06-21 21:01:30.000000 prelude-cli-1.2.6/prelude_cli.egg-info/requires.txt
+-rw-r--r--   0 pack       (501) staff       (20)       12 2023-06-21 21:01:30.000000 prelude-cli-1.2.6/prelude_cli.egg-info/top_level.txt
+-rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-cli-1.2.6/pyproject.toml
+-rw-r--r--   0 pack       (501) staff       (20)      663 2023-06-21 21:01:30.322104 prelude-cli-1.2.6/setup.cfg
```

### Comparing `prelude-cli-1.2.5/LICENSE` & `prelude-cli-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.2.5/PKG-INFO` & `prelude-cli-1.2.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-cli
-Version: 1.2.5
+Version: 1.2.6
 Summary: For interacting with the Prelude SDK
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-cli-1.2.5/prelude_cli/cli.py` & `prelude-cli-1.2.6/prelude_cli/cli.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.2.5/prelude_cli/views/build.py` & `prelude-cli-1.2.6/prelude_cli/views/build.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,26 +21,26 @@
     """ Custom security tests """
     ctx.obj = BuildController(account=ctx.obj)
 
 
 @build.command('create-test')
 @click.argument('name')
 @click.option('-u', '--unit', required=True, help='unit identifier', type=str)
-@click.option('-a', '--advisory', help='alert identifier [CVE ID, Advisory ID, etc]', default=None, type=str)
 @click.option('-t', '--test', help='test identifier', default=None, type=str)
+@click.option('-a', '--advisory', default=None, hidden=True, type=str)
 @click.pass_obj
 @handle_api_error
-def create_test(controller, name, unit, advisory, test):
+def create_test(controller, name, unit, test, advisory):
     """ Create or update a security test """
     with Spinner():
         t = controller.create_test(
             name=name,
             unit=unit,
-            advisory=advisory,
-            test_id=test
+            test_id=test,
+            advisory=advisory
         )
 
     if not test:
         basename = f'{t["id"]}.go'
         template = pkg_resources.read_text(templates, 'template.go')
         template = template.replace('$ID', t['id'])
         template = template.replace('$NAME', name)
```

### Comparing `prelude-cli-1.2.5/prelude_cli/views/configure.py` & `prelude-cli-1.2.6/prelude_cli/views/configure.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.2.5/prelude_cli/views/detect.py` & `prelude-cli-1.2.6/prelude_cli/views/detect.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.2.5/prelude_cli/views/iam.py` & `prelude-cli-1.2.6/prelude_cli/views/iam.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.2.5/prelude_cli/views/partner.py` & `prelude-cli-1.2.6/prelude_cli/views/partner.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.2.5/prelude_cli/views/shared.py` & `prelude-cli-1.2.6/prelude_cli/views/shared.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.2.5/prelude_cli.egg-info/PKG-INFO` & `prelude-cli-1.2.6/prelude_cli.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-cli
-Version: 1.2.5
+Version: 1.2.6
 Summary: For interacting with the Prelude SDK
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-cli-1.2.5/prelude_cli.egg-info/SOURCES.txt` & `prelude-cli-1.2.6/prelude_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.2.5/setup.cfg` & `prelude-cli-1.2.6/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = prelude-cli
-version = 1.2.5
+version = 1.2.6
 author = Prelude Research
 author_email = support@preludesecurity.com
 description = For interacting with the Prelude SDK
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/preludeorg
 classifiers = 
@@ -13,15 +13,15 @@
 	Operating System :: OS Independent
 
 [options]
 packages = find:
 include_package_data = True
 python_requires = >=3.8
 install_requires = 
-	prelude-sdk == 1.2.5
+	prelude-sdk == 1.2.6
 	click > 8
 	rich
 
 [options.entry_points]
 console_scripts = 
 	prelude = prelude_cli.cli:cli
```

