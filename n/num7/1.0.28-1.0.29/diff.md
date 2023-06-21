# Comparing `tmp/num7-1.0.28.tar.gz` & `tmp/num7-1.0.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "num7-1.0.28.tar", last modified: Sat May 13 12:17:22 2023, max compression
+gzip compressed data, was "num7-1.0.29.tar", last modified: Wed Jun 21 07:09:51 2023, max compression
```

## Comparing `num7-1.0.28.tar` & `num7-1.0.29.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 12:17:22.087031 num7-1.0.28/
--rw-rw-rw-   0        0        0     1076 2023-02-24 11:37:18.000000 num7-1.0.28/LICENSE.txt
--rw-rw-rw-   0        0        0    20208 2023-05-13 12:17:22.083068 num7-1.0.28/PKG-INFO
--rw-rw-rw-   0        0        0    19720 2023-02-24 10:01:58.000000 num7-1.0.28/README.md
--rw-rw-rw-   0        0        0       42 2023-05-13 12:17:22.087031 num7-1.0.28/setup.cfg
--rw-rw-rw-   0        0        0      743 2023-05-13 12:12:12.000000 num7-1.0.28/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-13 12:17:22.063141 num7-1.0.28/src/
-drwxrwxrwx   0        0        0        0 2023-05-13 12:17:22.081726 num7-1.0.28/src/num7.egg-info/
--rw-rw-rw-   0        0        0    20208 2023-05-13 12:17:21.000000 num7-1.0.28/src/num7.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      170 2023-05-13 12:17:21.000000 num7-1.0.28/src/num7.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 12:17:21.000000 num7-1.0.28/src/num7.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-05-13 12:17:21.000000 num7-1.0.28/src/num7.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    62483 2023-05-13 12:07:09.000000 num7-1.0.28/src/num7.py
+drwxrwxrwx   0        0        0        0 2023-06-21 07:09:51.056674 num7-1.0.29/
+-rw-rw-rw-   0        0        0     1076 2023-02-24 11:37:18.000000 num7-1.0.29/LICENSE.txt
+-rw-rw-rw-   0        0        0    20208 2023-06-21 07:09:51.056674 num7-1.0.29/PKG-INFO
+-rw-rw-rw-   0        0        0    19720 2023-02-24 10:01:58.000000 num7-1.0.29/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-21 07:09:51.056674 num7-1.0.29/setup.cfg
+-rw-rw-rw-   0        0        0      743 2023-06-21 06:59:56.000000 num7-1.0.29/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 07:09:51.042151 num7-1.0.29/src/
+drwxrwxrwx   0        0        0        0 2023-06-21 07:09:51.051686 num7-1.0.29/src/num7.egg-info/
+-rw-rw-rw-   0        0        0    20208 2023-06-21 07:09:50.000000 num7-1.0.29/src/num7.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      170 2023-06-21 07:09:50.000000 num7-1.0.29/src/num7.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 07:09:50.000000 num7-1.0.29/src/num7.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-06-21 07:09:50.000000 num7-1.0.29/src/num7.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    62600 2023-06-20 17:50:32.000000 num7-1.0.29/src/num7.py
```

### Comparing `num7-1.0.28/LICENSE.txt` & `num7-1.0.29/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `num7-1.0.28/PKG-INFO` & `num7-1.0.29/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: num7
-Version: 1.0.28
+Version: 1.0.29
 Summary: Num - SUPREME PRECISION GENERAL PURPOSE ARITHMETIC-LOGIC DECIMAL CLASS
 Home-page: https://github.com/giocip/num7
 Author: giocip
 Author-email: giocip7@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `num7-1.0.28/README.md` & `num7-1.0.29/README.md`

 * *Files identical despite different names*

### Comparing `num7-1.0.28/setup.py` & `num7-1.0.29/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(name='num7',
-	  version='1.0.28',
+	  version='1.0.29',
 	  description='Num - SUPREME PRECISION GENERAL PURPOSE ARITHMETIC-LOGIC DECIMAL CLASS',
       long_description=long_description,
       long_description_content_type='text/markdown',
 	  py_modules=['num7'],
 	  package_dir={'': 'src'},
 	  url='https://github.com/giocip/num7',
 	  author='giocip',
```

### Comparing `num7-1.0.28/src/num7.egg-info/PKG-INFO` & `num7-1.0.29/src/num7.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: num7
-Version: 1.0.28
+Version: 1.0.29
 Summary: Num - SUPREME PRECISION GENERAL PURPOSE ARITHMETIC-LOGIC DECIMAL CLASS
 Home-page: https://github.com/giocip/num7
 Author: giocip
 Author-email: giocip7@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `num7-1.0.28/src/num7.py` & `num7-1.0.29/src/num7.py`

 * *Files 1% similar despite different names*

```diff
@@ -968,14 +968,16 @@
         return Num(self).__pow__(Num(e))        
     
     def __pow__(self, e) -> 'Num': #argument e mandatory,  
         ''' (**) overloading power binary operator and used by built-in function pow() '''
         if type(e) != int and type(e) != Num:
             raise ValueError("Num.__pow__ => type not valid:", e)            																			 
         if type(e) == int or type(e) == Num and e.is_numint():            
+            if self == Num('0.0') and e == 0:
+                raise ValueError("Num.__pow__ => undetermined:", e) 
             if e < 0:
                 b = i = Num('1.0') / self #
                 e = -e
                 while e > 1:
                     b *= i
                     e -= 1
             else:
```

