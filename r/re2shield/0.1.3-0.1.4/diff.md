# Comparing `tmp/re2shield-0.1.3.tar.gz` & `tmp/re2shield-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "re2shield-0.1.3.tar", last modified: Mon Jun 19 09:26:41 2023, max compression
+gzip compressed data, was "re2shield-0.1.4.tar", last modified: Wed Jun 21 01:59:48 2023, max compression
```

## Comparing `re2shield-0.1.3.tar` & `re2shield-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:26:41.776641 re2shield-0.1.3/
--rw-r--r--   0 root         (0) root         (0)     5510 2023-06-19 09:26:41.776641 re2shield-0.1.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4276 2023-06-19 09:23:22.000000 re2shield-0.1.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:26:41.775642 re2shield-0.1.3/re2shield/
--rw-r--r--   0 root         (0) root         (0)       43 2023-06-19 09:06:53.000000 re2shield-0.1.3/re2shield/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2379 2023-06-19 09:12:42.000000 re2shield-0.1.3/re2shield/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:26:41.776641 re2shield-0.1.3/re2shield.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5510 2023-06-19 09:26:41.000000 re2shield-0.1.3/re2shield.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      259 2023-06-19 09:26:41.000000 re2shield-0.1.3/re2shield.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 09:26:41.000000 re2shield-0.1.3/re2shield.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-06-19 09:26:41.000000 re2shield-0.1.3/re2shield.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-19 09:26:41.000000 re2shield-0.1.3/re2shield.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-19 09:26:41.776641 re2shield-0.1.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      859 2023-06-19 09:08:11.000000 re2shield-0.1.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:26:41.776641 re2shield-0.1.3/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 09:06:53.000000 re2shield-0.1.3/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      965 2023-06-19 09:24:22.000000 re2shield-0.1.3/tests/test_core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 01:59:48.025787 re2shield-0.1.4/
+-rw-r--r--   0 root         (0) root         (0)     5434 2023-06-21 01:59:48.025787 re2shield-0.1.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4192 2023-06-21 01:56:03.000000 re2shield-0.1.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 01:59:48.024787 re2shield-0.1.4/re2shield/
+-rw-r--r--   0 root         (0) root         (0)       43 2023-06-20 07:41:51.000000 re2shield-0.1.4/re2shield/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2019 2023-06-21 01:40:32.000000 re2shield-0.1.4/re2shield/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 01:59:48.025787 re2shield-0.1.4/re2shield.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5434 2023-06-21 01:59:47.000000 re2shield-0.1.4/re2shield.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      259 2023-06-21 01:59:48.000000 re2shield-0.1.4/re2shield.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 01:59:47.000000 re2shield-0.1.4/re2shield.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-06-21 01:59:47.000000 re2shield-0.1.4/re2shield.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-21 01:59:47.000000 re2shield-0.1.4/re2shield.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-21 01:59:48.025787 re2shield-0.1.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      859 2023-06-21 01:21:27.000000 re2shield-0.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 01:59:48.025787 re2shield-0.1.4/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 07:41:51.000000 re2shield-0.1.4/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      865 2023-06-21 01:41:12.000000 re2shield-0.1.4/tests/test_core.py
```

### Comparing `re2shield-0.1.3/PKG-INFO` & `re2shield-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: re2shield
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python library that provides a convenient interface for compiling and matching regular expression patterns using the re2 library.
 Home-page: https://github.com/Npc-coder/re2shield
 Author: mkCha
 Author-email: dxsaq0@gmail.com
 License: UNKNOWN
 Description: # re2shield
         `re2shield` is a Python library that provides a shield for working with regular expressions using the `re2` module. 
@@ -36,18 +36,20 @@
         ```shell
         git clone https://github.com/Npc-coder/re2shield.git
         cd re2shield
         pip install .
         ```
         
         ## Updates
-        ### Version 0.1.3
-        - Added the ability to count the number of patterns in the Re2ShieldDatabase. You can now print the Re2Shield object to see the number of compiled patterns.
-        - Added an 'overwrite' option to the compile method in Re2Shield. If 'overwrite' is False (default), new patterns are added to the existing ones. If 'overwrite' is True, new patterns replace the existing ones.
-        - Enhanced ID duplication check. Now it checks for ID duplication not only among the new patterns but also between the new patterns and the existing ones in the database. If a duplicate ID is found and 'overwrite' is False, a ValueError is raised.
+        ### Version 0.1.4
+        - Simplified the interface for compiling patterns. Now the compile method only requires a list of regular expressions. It automatically assigns a unique ID to each pattern, starting from 0 and incrementing for each new pattern.
+        - Removed the flags parameter from the compile method, as it was not necessary for the functionality of the library.
+        Improved the load function to correctly set the id_counter for the loaded Re2Shield object, ensuring that new patterns compiled after loading will have unique IDs.
+        - Removed the unnecessary ID duplication check in the compile method, as the new automatic ID assignment guarantees uniqueness.
+        
         Please refer to the [Usage](#usage) section for examples of how to use these new features.
         
         ## Usage
         ### Importing the Library
         Here is a simple example demonstrating how to use re2shield:
         
         ```python
@@ -59,21 +61,20 @@
             # Load patterns from file
             try:
                 db = re2shield.load('patterns.pkl')
                 print(db)  # Prints the number of patterns in the database
             except FileNotFoundError:
                 # If pattern file doesn't exist, compile the patterns
                 patterns = [
-                    (r'\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,}\b', 1, None),
-                    (r'\b\d{3}[-.\s]??\d{3}[-.\s]??\d{4}\b', 2, None),
-                    (r'\d+', 3, None)
+                    r'\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,}\b',
+                    r'\b\d{3}[-.\s]??\d{3}[-.\s]??\d{4}\b',
+                    r'\d+'
                 ]
         
-                expressions, ids, flags = zip(*patterns)
-                db.compile(expressions=expressions, ids=ids, flags=flags, overwrite=False)
+                db.compile(expressions=patterns, overwrite=False)
                 print(db)  # Prints the number of patterns in the database
                 db.dump('patterns.pkl')
         
             # Find patterns in text
             def match_handler(id, from_, to, flags, context):
                 print(f"Match found for pattern {id} from {from_} to {to}: {context}")
```

### Comparing `re2shield-0.1.3/README.md` & `re2shield-0.1.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -28,18 +28,20 @@
 ```shell
 git clone https://github.com/Npc-coder/re2shield.git
 cd re2shield
 pip install .
 ```
 
 ## Updates
-### Version 0.1.3
-- Added the ability to count the number of patterns in the Re2ShieldDatabase. You can now print the Re2Shield object to see the number of compiled patterns.
-- Added an 'overwrite' option to the compile method in Re2Shield. If 'overwrite' is False (default), new patterns are added to the existing ones. If 'overwrite' is True, new patterns replace the existing ones.
-- Enhanced ID duplication check. Now it checks for ID duplication not only among the new patterns but also between the new patterns and the existing ones in the database. If a duplicate ID is found and 'overwrite' is False, a ValueError is raised.
+### Version 0.1.4
+- Simplified the interface for compiling patterns. Now the compile method only requires a list of regular expressions. It automatically assigns a unique ID to each pattern, starting from 0 and incrementing for each new pattern.
+- Removed the flags parameter from the compile method, as it was not necessary for the functionality of the library.
+Improved the load function to correctly set the id_counter for the loaded Re2Shield object, ensuring that new patterns compiled after loading will have unique IDs.
+- Removed the unnecessary ID duplication check in the compile method, as the new automatic ID assignment guarantees uniqueness.
+
 Please refer to the [Usage](#usage) section for examples of how to use these new features.
 
 ## Usage
 ### Importing the Library
 Here is a simple example demonstrating how to use re2shield:
 
 ```python
@@ -51,21 +53,20 @@
     # Load patterns from file
     try:
         db = re2shield.load('patterns.pkl')
         print(db)  # Prints the number of patterns in the database
     except FileNotFoundError:
         # If pattern file doesn't exist, compile the patterns
         patterns = [
-            (r'\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,}\b', 1, None),
-            (r'\b\d{3}[-.\s]??\d{3}[-.\s]??\d{4}\b', 2, None),
-            (r'\d+', 3, None)
+            r'\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,}\b',
+            r'\b\d{3}[-.\s]??\d{3}[-.\s]??\d{4}\b',
+            r'\d+'
         ]
 
-        expressions, ids, flags = zip(*patterns)
-        db.compile(expressions=expressions, ids=ids, flags=flags, overwrite=False)
+        db.compile(expressions=patterns, overwrite=False)
         print(db)  # Prints the number of patterns in the database
         db.dump('patterns.pkl')
 
     # Find patterns in text
     def match_handler(id, from_, to, flags, context):
         print(f"Match found for pattern {id} from {from_} to {to}: {context}")
```

### Comparing `re2shield-0.1.3/re2shield/core.py` & `re2shield-0.1.4/re2shield/core.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,39 +14,31 @@
 
     def count_patterns(self):
         return len(self.re2_patterns)
 
 class Re2Shield:
     def __init__(self):
         self.db = None
+        self.id_counter = 0
 
     def __str__(self):
         if self.db is not None:
-            return f"Re2Shield Database with {self.db.count_patterns()} patterns."
+            return f"Database with {self.db.count_patterns()} patterns."
         else:
-            return "Re2Shield Database is not compiled."
-
-    def compile(self, expressions, ids, flags, overwrite=False):
-        if len(expressions) != len(ids) != len(flags):
-            raise ValueError("All parameters should have the same length")
-
-        re2_patterns = {}
-        raw_patterns = {}
-        if not overwrite and self.db is not None:
-            re2_patterns = self.db.re2_patterns.copy()
-            raw_patterns = self.db.raw_patterns.copy()
-
-        for id, expr, flag in zip(ids, expressions, flags):
-            if id in re2_patterns:
-                raise ValueError(f"ID {id} already exists in the database. To overwrite, set overwrite=True.")
-            re2_patterns[id] = re2.compile(expr, flag)
-            raw_patterns[id] = (expr, flag)
-
-        self.db = Re2ShieldDatabase(re2_patterns, raw_patterns)
+            return "Database is not compiled."
 
+    def compile(self, expressions, overwrite=False):
+        if overwrite or self.db is None:
+            self.db = Re2ShieldDatabase({}, {})
+            self.id_counter = 0
+
+        for expr in expressions:
+            self.db.re2_patterns[self.id_counter] = re2.compile(expr)
+            self.db.raw_patterns[self.id_counter] = expr
+            self.id_counter += 1
 
     def dump(self, file_path):
         if self.db is not None:
             with open(file_path, 'wb') as f:
                 pickle.dump(self.db.raw_patterns, f)
         else:
             raise ValueError("No compiled database found. Please compile patterns first.")
@@ -58,11 +50,12 @@
             raise ValueError("No compiled database found. Please compile patterns first.")
 
 Database = Re2Shield
 
 def load(file_path):
     with open(file_path, 'rb') as f:
         raw_patterns = pickle.load(f)
-        re2_patterns = {id: re2.compile(expr, flag) for id, (expr, flag) in raw_patterns.items()}
+        re2_patterns = {id: re2.compile(expr) for id, expr in raw_patterns.items()}
     re2_shield = Re2Shield()
     re2_shield.db = Re2ShieldDatabase(re2_patterns, raw_patterns)
-    return re2_shield
+    re2_shield.id_counter = max(raw_patterns.keys()) + 1
+    return re2_shield
```

### Comparing `re2shield-0.1.3/re2shield.egg-info/PKG-INFO` & `re2shield-0.1.4/re2shield.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: re2shield
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python library that provides a convenient interface for compiling and matching regular expression patterns using the re2 library.
 Home-page: https://github.com/Npc-coder/re2shield
 Author: mkCha
 Author-email: dxsaq0@gmail.com
 License: UNKNOWN
 Description: # re2shield
         `re2shield` is a Python library that provides a shield for working with regular expressions using the `re2` module. 
@@ -36,18 +36,20 @@
         ```shell
         git clone https://github.com/Npc-coder/re2shield.git
         cd re2shield
         pip install .
         ```
         
         ## Updates
-        ### Version 0.1.3
-        - Added the ability to count the number of patterns in the Re2ShieldDatabase. You can now print the Re2Shield object to see the number of compiled patterns.
-        - Added an 'overwrite' option to the compile method in Re2Shield. If 'overwrite' is False (default), new patterns are added to the existing ones. If 'overwrite' is True, new patterns replace the existing ones.
-        - Enhanced ID duplication check. Now it checks for ID duplication not only among the new patterns but also between the new patterns and the existing ones in the database. If a duplicate ID is found and 'overwrite' is False, a ValueError is raised.
+        ### Version 0.1.4
+        - Simplified the interface for compiling patterns. Now the compile method only requires a list of regular expressions. It automatically assigns a unique ID to each pattern, starting from 0 and incrementing for each new pattern.
+        - Removed the flags parameter from the compile method, as it was not necessary for the functionality of the library.
+        Improved the load function to correctly set the id_counter for the loaded Re2Shield object, ensuring that new patterns compiled after loading will have unique IDs.
+        - Removed the unnecessary ID duplication check in the compile method, as the new automatic ID assignment guarantees uniqueness.
+        
         Please refer to the [Usage](#usage) section for examples of how to use these new features.
         
         ## Usage
         ### Importing the Library
         Here is a simple example demonstrating how to use re2shield:
         
         ```python
@@ -59,21 +61,20 @@
             # Load patterns from file
             try:
                 db = re2shield.load('patterns.pkl')
                 print(db)  # Prints the number of patterns in the database
             except FileNotFoundError:
                 # If pattern file doesn't exist, compile the patterns
                 patterns = [
-                    (r'\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,}\b', 1, None),
-                    (r'\b\d{3}[-.\s]??\d{3}[-.\s]??\d{4}\b', 2, None),
-                    (r'\d+', 3, None)
+                    r'\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,}\b',
+                    r'\b\d{3}[-.\s]??\d{3}[-.\s]??\d{4}\b',
+                    r'\d+'
                 ]
         
-                expressions, ids, flags = zip(*patterns)
-                db.compile(expressions=expressions, ids=ids, flags=flags, overwrite=False)
+                db.compile(expressions=patterns, overwrite=False)
                 print(db)  # Prints the number of patterns in the database
                 db.dump('patterns.pkl')
         
             # Find patterns in text
             def match_handler(id, from_, to, flags, context):
                 print(f"Match found for pattern {id} from {from_} to {to}: {context}")
```

### Comparing `re2shield-0.1.3/setup.py` & `re2shield-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='re2shield',
-    version='0.1.3',
+    version='0.1.4',
     url='https://github.com/Npc-coder/re2shield',  # Replace with your own GitHub project URL
     author='mkCha',
     author_email='dxsaq0@gmail.com',
     description='A Python library that provides a convenient interface for compiling and matching regular expression patterns using the re2 library.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

### Comparing `re2shield-0.1.3/tests/test_core.py` & `re2shield-0.1.4/tests/test_core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import re2shield
 
 if __name__ == "__main__":
     db = re2shield.Database()
 
     # Load patterns from file
     try:
-        db = re2shield.load('patterns.db')
+        db = re2shield.load('./patterns.db')
         print(db)  # Prints the number of patterns in the database
     except FileNotFoundError:
         # If pattern file doesn't exist, compile the patterns
         patterns = [
-            (r'\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,}\b', 1, None),
-            (r'\b\d{3}[-.\s]??\d{3}[-.\s]??\d{4}\b', 2, None),
-            (r'\d+', 3, None)
+            r'\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,}\b',
+            r'\b\d{3}[-.\s]??\d{3}[-.\s]??\d{4}\b',
+            r'\d+'
         ]
 
-        expressions, ids, flags = zip(*patterns)
-        db.compile(expressions=expressions, ids=ids, flags=flags, overwrite=False)
+        db.compile(expressions=patterns, overwrite=False)
+
         print(db)  # Prints the number of patterns in the database
         db.dump('patterns.db')
 
     # Find patterns in text
     def match_handler(id, from_, to, flags, context):
         print(f"Match found for pattern {id} from {from_} to {to}: {context}")
 
     db.scan('test@ex12ample12.com', match_handler)
+
```

