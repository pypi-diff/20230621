# Comparing `tmp/pipcontrol-1.1.0.tar.gz` & `tmp/pipcontrol-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipcontrol-1.1.0.tar", last modified: Sun Feb 26 02:39:43 2023, max compression
+gzip compressed data, was "pipcontrol-1.2.0.tar", last modified: Wed Jun 21 06:05:51 2023, max compression
```

## Comparing `pipcontrol-1.1.0.tar` & `pipcontrol-1.2.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 mingoolee   (501) staff       (20)        0 2023-02-26 02:39:43.245828 pipcontrol-1.1.0/
--rw-r--r--   0 mingoolee   (501) staff       (20)     1211 2023-02-26 02:39:43.245898 pipcontrol-1.1.0/PKG-INFO
--rw-r--r--   0 mingoolee   (501) staff       (20)      563 2023-02-26 02:38:59.000000 pipcontrol-1.1.0/README.md
-drwxr-xr-x   0 mingoolee   (501) staff       (20)        0 2023-02-26 02:39:43.244762 pipcontrol-1.1.0/pipcontrol/
--rw-r--r--   0 mingoolee   (501) staff       (20)     1123 2023-02-26 02:11:55.000000 pipcontrol-1.1.0/pipcontrol/__init__.py
--rw-r--r--   0 mingoolee   (501) staff       (20)     3639 2023-02-26 02:38:32.000000 pipcontrol-1.1.0/pipcontrol/pipcontrol.py
-drwxr-xr-x   0 mingoolee   (501) staff       (20)        0 2023-02-26 02:39:43.245699 pipcontrol-1.1.0/pipcontrol.egg-info/
--rw-r--r--   0 mingoolee   (501) staff       (20)     1211 2023-02-26 02:39:43.000000 pipcontrol-1.1.0/pipcontrol.egg-info/PKG-INFO
--rw-r--r--   0 mingoolee   (501) staff       (20)      245 2023-02-26 02:39:43.000000 pipcontrol-1.1.0/pipcontrol.egg-info/SOURCES.txt
--rw-r--r--   0 mingoolee   (501) staff       (20)        1 2023-02-26 02:39:43.000000 pipcontrol-1.1.0/pipcontrol.egg-info/dependency_links.txt
--rw-r--r--   0 mingoolee   (501) staff       (20)        1 2023-02-26 02:28:14.000000 pipcontrol-1.1.0/pipcontrol.egg-info/not-zip-safe
--rw-r--r--   0 mingoolee   (501) staff       (20)       11 2023-02-26 02:39:43.000000 pipcontrol-1.1.0/pipcontrol.egg-info/top_level.txt
--rw-r--r--   0 mingoolee   (501) staff       (20)       79 2023-02-26 02:39:43.246137 pipcontrol-1.1.0/setup.cfg
--rw-r--r--   0 mingoolee   (501) staff       (20)     1622 2023-02-26 02:38:14.000000 pipcontrol-1.1.0/setup.py
+drwxr-xr-x   0 mingoolee   (501) staff       (20)        0 2023-06-21 06:05:51.003334 pipcontrol-1.2.0/
+-rw-r--r--   0 mingoolee   (501) staff       (20)     1799 2023-06-21 06:05:51.003393 pipcontrol-1.2.0/PKG-INFO
+-rw-r--r--   0 mingoolee   (501) staff       (20)     1140 2023-06-21 06:04:24.000000 pipcontrol-1.2.0/README.md
+drwxr-xr-x   0 mingoolee   (501) staff       (20)        0 2023-06-21 06:05:51.002427 pipcontrol-1.2.0/pipcontrol/
+-rw-r--r--   0 mingoolee   (501) staff       (20)     1123 2023-02-27 05:09:04.000000 pipcontrol-1.2.0/pipcontrol/__init__.py
+-rw-r--r--   0 mingoolee   (501) staff       (20)    10454 2023-06-21 06:05:26.000000 pipcontrol-1.2.0/pipcontrol/pipcontrol.py
+-rw-r--r--   0 mingoolee   (501) staff       (20)      166 2023-06-21 03:03:34.000000 pipcontrol-1.2.0/pipcontrol/test.py
+drwxr-xr-x   0 mingoolee   (501) staff       (20)        0 2023-06-21 06:05:51.003217 pipcontrol-1.2.0/pipcontrol.egg-info/
+-rw-r--r--   0 mingoolee   (501) staff       (20)     1799 2023-06-21 06:05:50.000000 pipcontrol-1.2.0/pipcontrol.egg-info/PKG-INFO
+-rw-r--r--   0 mingoolee   (501) staff       (20)      264 2023-06-21 06:05:50.000000 pipcontrol-1.2.0/pipcontrol.egg-info/SOURCES.txt
+-rw-r--r--   0 mingoolee   (501) staff       (20)        1 2023-06-21 06:05:50.000000 pipcontrol-1.2.0/pipcontrol.egg-info/dependency_links.txt
+-rw-r--r--   0 mingoolee   (501) staff       (20)        1 2023-06-21 06:05:50.000000 pipcontrol-1.2.0/pipcontrol.egg-info/not-zip-safe
+-rw-r--r--   0 mingoolee   (501) staff       (20)       11 2023-06-21 06:05:50.000000 pipcontrol-1.2.0/pipcontrol.egg-info/top_level.txt
+-rw-r--r--   0 mingoolee   (501) staff       (20)       79 2023-06-21 06:05:51.003615 pipcontrol-1.2.0/setup.cfg
+-rw-r--r--   0 mingoolee   (501) staff       (20)     1633 2023-06-21 02:58:10.000000 pipcontrol-1.2.0/setup.py
```

### Comparing `pipcontrol-1.1.0/pipcontrol/__init__.py` & `pipcontrol-1.2.0/pipcontrol/__init__.py`

 * *Files identical despite different names*

### Comparing `pipcontrol-1.1.0/setup.py` & `pipcontrol-1.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="pipcontrol",
-    version="1.1.0",
-    description="pip module automation",
+    version="1.2.0",
+    description="control pip module in python code",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Mingoo Lee",
     author_email="labovming@gmail.com",
     keyword=["python", "package", "install", "update", "uninstall", "pip", "pip3", "requirements"],
     python_requires=">=3.8",
     zip_safe=False,
@@ -22,15 +22,15 @@
     url="https://github.com/labov/pipcontrol",
     packages=setuptools.find_packages(),
     classifiers=[
         # How mature is this project? Common values are
         #   3 - Alpha
         #   4 - Beta
         #   5 - Production/Stable
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 4 - Beta",
         # Indicate who your project is intended for
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
         "Topic :: Software Development :: Libraries :: Python Modules",
         # Pick your license as you wish (should match "license" above)
         "License :: OSI Approved :: MIT License",
         # Specify the Python versions you support here. In particular, ensure
```

