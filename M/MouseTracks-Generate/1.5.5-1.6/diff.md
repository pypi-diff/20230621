# Comparing `tmp/MouseTracks_Generate-1.5.5.tar.gz` & `tmp/MouseTracks_Generate-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MouseTracks_Generate-1.5.5.tar", last modified: Tue Jun 20 13:39:29 2023, max compression
+gzip compressed data, was "MouseTracks_Generate-1.6.tar", last modified: Wed Jun 21 05:15:44 2023, max compression
```

## Comparing `MouseTracks_Generate-1.5.5.tar` & `MouseTracks_Generate-1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 13:39:29.670794 MouseTracks_Generate-1.5.5/
--rw-rw-rw-   0        0        0     1068 2023-06-20 02:28:28.000000 MouseTracks_Generate-1.5.5/LICENCE
--rw-rw-rw-   0        0        0       90 2023-06-20 05:44:42.000000 MouseTracks_Generate-1.5.5/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-06-20 13:39:29.639539 MouseTracks_Generate-1.5.5/MouseTracks_Generate/
--rw-rw-rw-   0        0        0      161 2023-06-20 13:05:06.000000 MouseTracks_Generate-1.5.5/MouseTracks_Generate/__init__.py
--rw-rw-rw-   0        0        0     5522 2023-06-20 13:29:42.000000 MouseTracks_Generate-1.5.5/MouseTracks_Generate/generate.py
--rw-rw-rw-   0        0        0    80957 2023-06-08 02:12:28.000000 MouseTracks_Generate-1.5.5/MouseTracks_Generate/length_analysis.csv
--rw-rw-rw-   0        0        0   149928 2023-06-20 02:41:13.000000 MouseTracks_Generate-1.5.5/MouseTracks_Generate/model2.h5
-drwxrwxrwx   0        0        0        0 2023-06-20 13:39:29.655157 MouseTracks_Generate-1.5.5/MouseTracks_Generate.egg-info/
--rw-rw-rw-   0        0        0      275 2023-06-20 13:39:29.000000 MouseTracks_Generate-1.5.5/MouseTracks_Generate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      385 2023-06-20 13:39:29.000000 MouseTracks_Generate-1.5.5/MouseTracks_Generate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 13:39:29.000000 MouseTracks_Generate-1.5.5/MouseTracks_Generate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-06-20 13:39:29.000000 MouseTracks_Generate-1.5.5/MouseTracks_Generate.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-20 13:39:29.000000 MouseTracks_Generate-1.5.5/MouseTracks_Generate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      275 2023-06-20 13:39:29.670794 MouseTracks_Generate-1.5.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-20 13:39:29.670794 MouseTracks_Generate-1.5.5/setup.cfg
--rw-rw-rw-   0        0        0      630 2023-06-20 13:39:13.000000 MouseTracks_Generate-1.5.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 05:15:44.360983 MouseTracks_Generate-1.6/
+-rw-rw-rw-   0        0        0     1068 2023-06-20 02:28:28.000000 MouseTracks_Generate-1.6/LICENCE
+-rw-rw-rw-   0        0        0       90 2023-06-20 05:44:42.000000 MouseTracks_Generate-1.6/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-06-21 05:15:44.342985 MouseTracks_Generate-1.6/MouseTracks_Generate/
+-rw-rw-rw-   0        0        0      161 2023-06-20 13:05:06.000000 MouseTracks_Generate-1.6/MouseTracks_Generate/__init__.py
+-rw-rw-rw-   0        0        0     5712 2023-06-21 05:13:39.000000 MouseTracks_Generate-1.6/MouseTracks_Generate/generate.py
+-rw-rw-rw-   0        0        0    80957 2023-06-08 02:12:28.000000 MouseTracks_Generate-1.6/MouseTracks_Generate/length_analysis.csv
+-rw-rw-rw-   0        0        0   149928 2023-06-20 02:41:13.000000 MouseTracks_Generate-1.6/MouseTracks_Generate/model2.h5
+drwxrwxrwx   0        0        0        0 2023-06-21 05:15:44.355980 MouseTracks_Generate-1.6/MouseTracks_Generate.egg-info/
+-rw-rw-rw-   0        0        0      273 2023-06-21 05:15:44.000000 MouseTracks_Generate-1.6/MouseTracks_Generate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2023-06-21 05:15:44.000000 MouseTracks_Generate-1.6/MouseTracks_Generate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 05:15:44.000000 MouseTracks_Generate-1.6/MouseTracks_Generate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-06-21 05:15:44.000000 MouseTracks_Generate-1.6/MouseTracks_Generate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-21 05:15:44.000000 MouseTracks_Generate-1.6/MouseTracks_Generate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      273 2023-06-21 05:15:44.359981 MouseTracks_Generate-1.6/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-21 05:15:44.361983 MouseTracks_Generate-1.6/setup.cfg
+-rw-rw-rw-   0        0        0      628 2023-06-21 05:14:47.000000 MouseTracks_Generate-1.6/setup.py
```

### Comparing `MouseTracks_Generate-1.5.5/LICENCE` & `MouseTracks_Generate-1.6/LICENCE`

 * *Files identical despite different names*

### Comparing `MouseTracks_Generate-1.5.5/MouseTracks_Generate/generate.py` & `MouseTracks_Generate-1.6/MouseTracks_Generate/generate.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,18 @@
 
 
 def get_length(startx ,starty, stopx, stopy):
     dx = abs(stopx - startx)
     dy = abs(stopy - starty)
     distance = int(math.sqrt(dx**2 + dy**2))
     length = int(fx(distance))
-    length = random.randint(length-10, length+10)
+    if length <= 118:
+        length = random.randint(length-10, length+10)
+    else:
+        length = 128
     return length
 
 
 def create_actions(startx, starty, stopx, stopy):
     length = get_length(startx, starty, stopx, stopy)
 
     x1 = startx
@@ -80,16 +83,22 @@
         y1.append(y1[-1] + j)
     x1 = x1[0:length]
     y1 = y1[0:length]
     dx1 = dx1[0:length]
     dy1 = dy1[0:length]
     x1_end = x1[-1]
     y1_end = y1[-1]
-    rate_x = (stopx - startx) / (x1_end - startx)
-    rate_y = (stopy - starty) / (y1_end - starty)
+    if x1_end - startx == 0:
+        rate_x = 0
+    else:
+        rate_x = (stopx - startx) / (x1_end - startx)
+    if y1_end - starty == 0:
+        rate_y = 0
+    else:
+        rate_y = (stopy - starty) / (y1_end - starty)
 
     x = x1
     y = y1
     for k in range(length):
         x[k] = int((x1[k] - startx) * rate_x + startx)
         y[k] = int((y1[k] - starty) * rate_y + starty)
```

### Comparing `MouseTracks_Generate-1.5.5/MouseTracks_Generate/length_analysis.csv` & `MouseTracks_Generate-1.6/MouseTracks_Generate/length_analysis.csv`

 * *Files identical despite different names*

### Comparing `MouseTracks_Generate-1.5.5/MouseTracks_Generate/model2.h5` & `MouseTracks_Generate-1.6/MouseTracks_Generate/model2.h5`

 * *Files identical despite different names*

### Comparing `MouseTracks_Generate-1.5.5/setup.py` & `MouseTracks_Generate-1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('readme.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='MouseTracks_Generate',
-    version='1.5.5',
+    version='1.6',
     author='momo',
     long_description=long_description,
     include_package_data=True,
     packages=setuptools.find_packages(),
     install_requires=[
         'pandas',
         'numpy',
```

