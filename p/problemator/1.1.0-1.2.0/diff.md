# Comparing `tmp/problemator-1.1.0.tar.gz` & `tmp/problemator-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "problemator-1.1.0.tar", last modified: Mon May 29 19:51:56 2023, max compression
+gzip compressed data, was "problemator-1.2.0.tar", last modified: Wed Jun 21 17:28:58 2023, max compression
```

## Comparing `problemator-1.1.0.tar` & `problemator-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 19:51:56.891997 problemator-1.1.0/
--rw-rw-rw-   0        0        0     1080 2023-05-29 19:44:03.000000 problemator-1.1.0/LICENSE
--rw-rw-rw-   0        0        0       34 2022-04-12 16:05:18.000000 problemator-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1499 2023-05-29 19:51:56.891997 problemator-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      926 2023-05-29 19:50:56.000000 problemator-1.1.0/README.MD
-drwxrwxrwx   0        0        0        0 2023-05-29 19:51:56.889006 problemator-1.1.0/problemator/
--rw-rw-rw-   0        0        0       36 2023-05-29 19:50:54.000000 problemator-1.1.0/problemator/__init__.py
--rw-rw-rw-   0        0        0     2580 2023-05-29 19:50:53.000000 problemator-1.1.0/problemator/problemator.py
-drwxrwxrwx   0        0        0        0 2023-05-29 19:51:56.891997 problemator-1.1.0/problemator.egg-info/
--rw-rw-rw-   0        0        0     1499 2023-05-29 19:51:56.000000 problemator-1.1.0/problemator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2023-05-29 19:51:56.000000 problemator-1.1.0/problemator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 19:51:56.000000 problemator-1.1.0/problemator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-05-29 19:51:56.000000 problemator-1.1.0/problemator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-29 19:51:56.000000 problemator-1.1.0/problemator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-29 19:51:56.891997 problemator-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      892 2023-05-29 19:51:21.000000 problemator-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 17:28:58.398655 problemator-1.2.0/
+-rw-rw-rw-   0        0        0     1080 2023-05-29 19:44:03.000000 problemator-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0       34 2022-04-12 16:05:18.000000 problemator-1.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1549 2023-06-21 17:28:58.398655 problemator-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      976 2023-06-21 17:28:28.000000 problemator-1.2.0/README.MD
+drwxrwxrwx   0        0        0        0 2023-06-21 17:28:58.395663 problemator-1.2.0/problemator/
+-rw-rw-rw-   0        0        0       36 2023-05-29 19:50:54.000000 problemator-1.2.0/problemator/__init__.py
+-rw-rw-rw-   0        0        0     3826 2023-06-21 17:27:06.000000 problemator-1.2.0/problemator/problemator.py
+drwxrwxrwx   0        0        0        0 2023-06-21 17:28:58.397658 problemator-1.2.0/problemator.egg-info/
+-rw-rw-rw-   0        0        0     1549 2023-06-21 17:28:58.000000 problemator-1.2.0/problemator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2023-06-21 17:28:58.000000 problemator-1.2.0/problemator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 17:28:58.000000 problemator-1.2.0/problemator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-06-21 17:28:58.000000 problemator-1.2.0/problemator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-21 17:28:58.000000 problemator-1.2.0/problemator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 17:28:58.398655 problemator-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      892 2023-06-21 17:27:30.000000 problemator-1.2.0/setup.py
```

### Comparing `problemator-1.1.0/LICENSE` & `problemator-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `problemator-1.1.0/PKG-INFO` & `problemator-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: problemator
-Version: 1.1.0
+Version: 1.2.0
 Summary: WolframAlpha's Unlimited AI-generated practice problems and answers API wrapper.
 Home-page: https://github.com/DedInc/problemator
 Author: Maehdakvan
 Author-email: visitanimation@google.com
 Project-URL: Bug Tracker, https://github.com/DedInc/problemator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -35,10 +35,11 @@
 
 print(problem['text'])  # Text of the problem
 print(problem['image'])  # Image of the problem
 print(problem['difficulty'])  # Difficulty of the problem
 
 result = p.check_problem(problem, 'x+5')  # Check problem, where x+5 - answer
 print(result['correct'])  # True or False
+print(result['attempt'])  # Image of the Attempt
 print(result['hint'])  # Image of the Hint
 print(result['solution'])  # Image of the Solution
 ```
```

### Comparing `problemator-1.1.0/README.MD` & `problemator-1.2.0/README.MD`

 * *Files 4% similar despite different names*

```diff
@@ -20,10 +20,11 @@
 
 print(problem['text'])  # Text of the problem
 print(problem['image'])  # Image of the problem
 print(problem['difficulty'])  # Difficulty of the problem
 
 result = p.check_problem(problem, 'x+5')  # Check problem, where x+5 - answer
 print(result['correct'])  # True or False
+print(result['attempt'])  # Image of the Attempt
 print(result['hint'])  # Image of the Hint
 print(result['solution'])  # Image of the Solution
 ```
```

### Comparing `problemator-1.1.0/problemator/problemator.py` & `problemator-1.2.0/problemator/problemator.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,50 +4,95 @@
 
 
 class Problemator:
     def __init__(self):
         self.categories = {}
         self.load_session()
 
-    def search_categories(self, cats):
-        for c in cats:
-            if 'Subcategories' in c:
-                self.search_categories(c['Subcategories'])
-            else:
-                self.categories[c['LinkTo']] = len(self.categories)
+    def convert_categories(self, categories_dict, id_counter=0):
+        converted_data = {}
 
-    def get_category(self, id):
-        for cat in self.categories.keys():
-            if self.categories[cat] == id:
-                return cat
+        for category in categories_dict:
+            category_name = category['Display']
+            subcategories = category.get('Subcategories', [])
+
+            if subcategories:
+                converted_subcategories, id_counter = self.convert_categories(subcategories, id_counter)
+                converted_data[category_name] = converted_subcategories
+            else:
+                linkto_id = category.get('LinkTo')
+                if linkto_id is not None:
+                    converted_data[category_name] = {'name': linkto_id, 'id': id_counter}
+                    id_counter += 1
+                else:
+                    continue
+
+        return converted_data, id_counter
+
+    def get_category(self, id, categories=None):
+        if categories is None:
+            categories = self.categories
+
+        for cat, value in categories.items():
+            if isinstance(value, dict):
+                if 'id' in value and value['id'] == id:
+                    return value['name']
+
+                subcategory_result = self.get_category(id, value)
+                if subcategory_result:
+                    return subcategory_result
 
     def load_session(self):
         self.s = Session()
         self.s.headers['User-Agent'] = generate_user_agent()
         self.s.headers['Accept'] = 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9'
         self.s.headers['Accept-Encoding'] = 'gzip, deflate, br'
         self.s.headers['Accept-Language'] = 'ru-RU,ru;q=0.9,kk-KZ;q=0.8,kk;q=0.7,en-US;q=0.6,en;q=0.5'
 
         r = self.s.get('https://www.wolframalpha.com/input/wpg/categories.jsp?load=true').json()
-        self.search_categories(r['Categories']['Categories'])
+        self.categories, _ = self.convert_categories(r['Categories']['Categories'])
         self.API = r['domain']
 
     def check_problem(self, problem, answer):
         lvl = problem['difficulty']
         pid = problem['id']
         machine = problem['machine']
         for c in problem['session']:
             cookie = create_cookie(name=c['name'], value=c['value'], domain=c['domain'])
             self.s.cookies.set_cookie(cookie)
-        r = self.s.get(f'{self.API}/input/wpg/checkanswer.jsp?attempt=1&difficulty={lvl}&load=true&problemID={pid}&query={answer}&s={machine}&type=InputField').json()
-        return {'correct': r['correct'], 'hint': r['hint'], 'solution': r['solution']}
+
+        url = f'{self.API}/input/wpg/checkanswer.jsp'
+
+        params = {
+            'attempt': 1,
+            'difficulty': lvl,
+            'load': 'true',
+            'problemID': pid,
+            'query': answer,
+            's': machine,
+            'type': 'InputField'
+        }
+
+        r = self.s.get(url, params=params).json()
+        return {'correct': r['correct'], 'hint': r['hint'], 'solution': r['solution'], 'attempt': r['attempt']}
 
     def generate_problem(self, lvl=0, type='IntegerAddition'):
         lvl = {0: 'Beginner', 1: 'Intermediate', 2: 'Advanced'}[lvl]
-        r = self.s.get(f'{self.API}/input/wpg/problem.jsp?count=1&difficulty={lvl}&load=1&type={type}').json()
+
+        url = f'{self.API}/input/wpg/problem.jsp'
+
+        params = {
+            'count': 1,
+            'difficulty': lvl,
+            'load': 'true',
+            'type': type
+        }
+
+        r = self.s.get(url, params=params).json()
+
         problems = r['problems']
         machine = r['machine']
         cookies = []
         for c in self.s.cookies:
             if c.name == 'JSESSIONID':
                 cookies.append({'name': c.name, 'value': c.value, 'domain': c.domain})
         problem = problems[0]
```

### Comparing `problemator-1.1.0/problemator.egg-info/PKG-INFO` & `problemator-1.2.0/problemator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: problemator
-Version: 1.1.0
+Version: 1.2.0
 Summary: WolframAlpha's Unlimited AI-generated practice problems and answers API wrapper.
 Home-page: https://github.com/DedInc/problemator
 Author: Maehdakvan
 Author-email: visitanimation@google.com
 Project-URL: Bug Tracker, https://github.com/DedInc/problemator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -35,10 +35,11 @@
 
 print(problem['text'])  # Text of the problem
 print(problem['image'])  # Image of the problem
 print(problem['difficulty'])  # Difficulty of the problem
 
 result = p.check_problem(problem, 'x+5')  # Check problem, where x+5 - answer
 print(result['correct'])  # True or False
+print(result['attempt'])  # Image of the Attempt
 print(result['hint'])  # Image of the Hint
 print(result['solution'])  # Image of the Solution
 ```
```

### Comparing `problemator-1.1.0/setup.py` & `problemator-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="problemator",
-    version="1.1.0",
+    version="1.2.0",
     author="Maehdakvan",
     author_email="visitanimation@google.com",
     description="WolframAlpha's Unlimited AI-generated practice problems and answers API wrapper.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/DedInc/problemator",
     project_urls={
```

