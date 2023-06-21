# Comparing `tmp/sk_report_generator-0.0.1.tar.gz` & `tmp/sk_report_generator-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sk_report_generator-0.0.1.tar", last modified: Mon Jun 12 06:01:19 2023, max compression
+gzip compressed data, was "sk_report_generator-0.0.2.tar", last modified: Wed Jun 21 13:07:12 2023, max compression
```

## Comparing `sk_report_generator-0.0.1.tar` & `sk_report_generator-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 06:01:19.762533 sk_report_generator-0.0.1/
--rw-rw-rw-   0        0        0     1055 2023-06-08 17:52:35.000000 sk_report_generator-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     3186 2023-06-12 06:01:19.762533 sk_report_generator-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2750 2023-06-12 05:59:22.000000 sk_report_generator-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-12 06:01:19.762533 sk_report_generator-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      756 2023-06-12 06:00:48.000000 sk_report_generator-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-12 06:01:19.653158 sk_report_generator-0.0.1/sk_report_generator/
--rw-rw-rw-   0        0        0        2 2023-06-12 02:41:47.000000 sk_report_generator-0.0.1/sk_report_generator/__init__.py
--rw-rw-rw-   0        0        0     1580 2023-06-12 03:49:15.000000 sk_report_generator-0.0.1/sk_report_generator/report_generator.py
--rw-rw-rw-   0        0        0     4243 2023-06-12 03:45:23.000000 sk_report_generator-0.0.1/sk_report_generator/test_generator.py
-drwxrwxrwx   0        0        0        0 2023-06-12 06:01:19.762533 sk_report_generator-0.0.1/sk_report_generator.egg-info/
--rw-rw-rw-   0        0        0     3186 2023-06-12 06:01:19.000000 sk_report_generator-0.0.1/sk_report_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      354 2023-06-12 06:01:19.000000 sk_report_generator-0.0.1/sk_report_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 06:01:19.000000 sk_report_generator-0.0.1/sk_report_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-12 06:01:19.000000 sk_report_generator-0.0.1/sk_report_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-06-12 06:01:19.000000 sk_report_generator-0.0.1/sk_report_generator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-21 13:07:12.802759 sk_report_generator-0.0.2/
+-rw-rw-rw-   0        0        0     1055 2023-06-18 09:14:44.000000 sk_report_generator-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     3186 2023-06-21 13:07:12.797506 sk_report_generator-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2750 2023-06-18 09:14:44.000000 sk_report_generator-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-21 13:07:12.802759 sk_report_generator-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      756 2023-06-21 13:07:10.000000 sk_report_generator-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 13:07:12.724999 sk_report_generator-0.0.2/sk_report_generator/
+-rw-rw-rw-   0        0        0       10 2023-06-21 08:07:09.000000 sk_report_generator-0.0.2/sk_report_generator/__init__.py
+-rw-rw-rw-   0        0        0      376 2023-06-21 08:07:09.000000 sk_report_generator-0.0.2/sk_report_generator/base.py
+-rw-rw-rw-   0        0        0      918 2023-06-21 08:07:09.000000 sk_report_generator-0.0.2/sk_report_generator/report_generator.py
+drwxrwxrwx   0        0        0        0 2023-06-21 13:07:12.792469 sk_report_generator-0.0.2/sk_report_generator/reporter/
+-rw-rw-rw-   0        0        0       10 2023-06-21 08:07:09.000000 sk_report_generator-0.0.2/sk_report_generator/reporter/__init__.py
+-rw-rw-rw-   0        0        0      468 2023-06-21 08:07:09.000000 sk_report_generator-0.0.2/sk_report_generator/reporter/default.py
+-rw-rw-rw-   0        0        0      998 2023-06-21 10:17:38.000000 sk_report_generator-0.0.2/sk_report_generator/reporter/format.py
+-rw-rw-rw-   0        0        0     1180 2023-06-21 08:07:09.000000 sk_report_generator-0.0.2/sk_report_generator/reporter/matrix.py
+-rw-rw-rw-   0        0        0     1880 2023-06-21 08:07:09.000000 sk_report_generator-0.0.2/sk_report_generator/reporter/script_evaluate.py
+-rw-rw-rw-   0        0        0      835 2023-06-21 08:07:09.000000 sk_report_generator-0.0.2/sk_report_generator/reporter/variable.py
+-rw-rw-rw-   0        0        0      256 2023-06-21 08:07:09.000000 sk_report_generator-0.0.2/sk_report_generator/test.py
+-rw-rw-rw-   0        0        0     4287 2023-06-21 10:14:30.000000 sk_report_generator-0.0.2/sk_report_generator/test_generator.py
+drwxrwxrwx   0        0        0        0 2023-06-21 13:07:12.777243 sk_report_generator-0.0.2/sk_report_generator.egg-info/
+-rw-rw-rw-   0        0        0     3186 2023-06-21 13:07:12.000000 sk_report_generator-0.0.2/sk_report_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      658 2023-06-21 13:07:12.000000 sk_report_generator-0.0.2/sk_report_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 13:07:12.000000 sk_report_generator-0.0.2/sk_report_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-21 13:07:12.000000 sk_report_generator-0.0.2/sk_report_generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-06-21 13:07:12.000000 sk_report_generator-0.0.2/sk_report_generator.egg-info/top_level.txt
```

### Comparing `sk_report_generator-0.0.1/LICENSE.txt` & `sk_report_generator-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sk_report_generator-0.0.1/PKG-INFO` & `sk_report_generator-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sk_report_generator
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple Reporting program
 Author: gkibria
 Author-email: gkibria121@gmail.com
 Keywords: python,report generator
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sk_report_generator-0.0.1/README.md` & `sk_report_generator-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sk_report_generator-0.0.1/setup.py` & `sk_report_generator-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='sk_report_generator',
-    version='0.0.1',
+    version='0.0.2',
     description='A simple Reporting program',
     author='gkibria',
     long_description=long_description,
     long_description_content_type="text/markdown",  # Specify the content type as Markdown
     author_email='gkibria121@gmail.com',
     packages=find_packages(),
     install_requires=['regex'],
```

### Comparing `sk_report_generator-0.0.1/sk_report_generator/test_generator.py` & `sk_report_generator-0.0.2/sk_report_generator/test_generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,32 +4,32 @@
 
 class ReportGeneratorTest(unittest.TestCase):
     def setUp(self):
         self.report_generator = ReportGenerator()
 
     def test_generate_report(self):
 
-        template = 'Rohim has {{$x:.2f}} taka and Korim has $y taka. They have $xy taka. The can get $var taka. They need $var2 taka and $yx'
+        template = 'Rohim has {{$x:.2f}} taka and Korim has {{$y}} taka. They have {{$xy}} taka. The can get {{$var}} taka. They need {{$var2}} taka and {{$yx}}'
         data = {'$x': '3.00000099999999', '$y': '3.0', '$var': '460.0', '$var2': '6.00000099999999', '$xy': '12.00000199999998', '$yx': '18.00000299999997'}
         expected_output = 'Rohim has 3.00 taka and Korim has 3.0 taka. They have 12.00000199999998 taka. The can get 460.0 taka. They need 6.00000099999999 taka and 18.00000299999997'
 
         output = self.report_generator.generate_report(template, data)
 
         self.assertEqual(output, expected_output)
 
     def test_generate_report2(self):
         # Test case 1: Basic substitution
-        template = 'Hello, {{$name}}!'
+        template = 'Hello, {{$name.value()}}!'
         data = {'$name': 'John'}
         expected_output = 'Hello, John!'
         output = self.report_generator.generate_report(template, data)
         self.assertEqual(output, expected_output)
 
         # Test case 2: Formatting and multiple substitutions
-        template = 'Total amount: $total_amount. Discount: {{$discount:.2f}}%. Final amount: $final_amount.'
+        template = 'Total amount: {{$total_amount}}. Discount: {{$discount:.2f}}%. Final amount: {{$final_amount}}.'
         data = {'$total_amount': '1000', '$discount': '15.5', '$final_amount': '845.00'}
         expected_output = 'Total amount: 1000. Discount: 15.50%. Final amount: 845.00.'
         output = self.report_generator.generate_report(template, data)
         self.assertEqual(output, expected_output)
 
         # Test case 3: Substitution not present in data
         template = 'Hello, {{$name}}!'
@@ -50,15 +50,15 @@
         template = 'The answer is {{$number}}.'
         data = {'$number': 42}
         expected_output = 'The answer is 42.'
         output = self.report_generator.generate_report(template, data)
         self.assertEqual(output, expected_output)
 
         # Test case 2: Substitution with string value
-        template = 'The color is {{$color}}.'
+        template = 'The color is {{$color.value()}}.'
         data = {'$color': 'blue'}
         expected_output = 'The color is blue.'
         output = self.report_generator.generate_report(template, data)
         self.assertEqual(output, expected_output)
 
         # Test case 3: Substitution with float value and custom format
         template = 'The price is ${{ $price:.2f }}.'
```

### Comparing `sk_report_generator-0.0.1/sk_report_generator.egg-info/PKG-INFO` & `sk_report_generator-0.0.2/sk_report_generator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sk-report-generator
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple Reporting program
 Author: gkibria
 Author-email: gkibria121@gmail.com
 Keywords: python,report generator
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

