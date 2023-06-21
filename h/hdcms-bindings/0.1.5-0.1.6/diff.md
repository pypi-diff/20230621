# Comparing `tmp/hdcms-bindings-0.1.5.tar.gz` & `tmp/hdcms-bindings-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdcms-bindings-0.1.5.tar", last modified: Tue Jun 20 08:57:22 2023, max compression
+gzip compressed data, was "hdcms-bindings-0.1.6.tar", last modified: Wed Jun 21 00:06:23 2023, max compression
```

## Comparing `hdcms-bindings-0.1.5.tar` & `hdcms-bindings-0.1.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 jason      (502) staff       (20)        0 2023-06-20 08:57:22.225489 hdcms-bindings-0.1.5/
--rw-r--r--   0 jason      (502) staff       (20)     1830 2023-01-22 19:56:08.000000 hdcms-bindings-0.1.5/LICENSE
--rw-r--r--   0 jason      (502) staff       (20)      146 2023-02-03 06:05:56.000000 hdcms-bindings-0.1.5/MANIFEST.in
--rw-r--r--   0 jason      (502) staff       (20)     5514 2023-06-20 08:57:22.225317 hdcms-bindings-0.1.5/PKG-INFO
--rw-r--r--   0 jason      (502) staff       (20)     3037 2023-06-20 08:56:33.000000 hdcms-bindings-0.1.5/README.md
-drwxr-xr-x   0 jason      (502) staff       (20)        0 2023-06-20 08:57:22.222332 hdcms-bindings-0.1.5/hdcms-c/
-drwxr-xr-x   0 jason      (502) staff       (20)        0 2023-06-20 08:57:22.223699 hdcms-bindings-0.1.5/hdcms-c/src/
--rw-r--r--   0 jason      (502) staff       (20)      882 2023-02-03 05:04:03.000000 hdcms-bindings-0.1.5/hdcms-c/src/fixwindows.h
--rw-r--r--   0 jason      (502) staff       (20)    10239 2023-06-18 17:14:08.000000 hdcms-bindings-0.1.5/hdcms-c/src/main.c
--rw-r--r--   0 jason      (502) staff       (20)       48 2023-02-03 05:04:03.000000 hdcms-bindings-0.1.5/hdcms-c/src/main.h
-drwxr-xr-x   0 jason      (502) staff       (20)        0 2023-06-20 08:57:22.224525 hdcms-bindings-0.1.5/hdcms-c/src/util/
--rw-r--r--   0 jason      (502) staff       (20)    20530 2023-06-20 08:03:24.000000 hdcms-bindings-0.1.5/hdcms-c/src/util/array.c
--rw-r--r--   0 jason      (502) staff       (20)     9226 2023-06-17 22:57:37.000000 hdcms-bindings-0.1.5/hdcms-c/src/util/array.h
--rw-r--r--   0 jason      (502) staff       (20)     4318 2023-06-20 08:03:24.000000 hdcms-bindings-0.1.5/hdcms-c/src/util/bin.c
--rw-r--r--   0 jason      (502) staff       (20)     2880 2023-06-18 17:14:08.000000 hdcms-bindings-0.1.5/hdcms-c/src/util/bin.h
--rw-r--r--   0 jason      (502) staff       (20)     8646 2023-06-18 17:14:08.000000 hdcms-bindings-0.1.5/hdcms-c/src/util/peak.c
--rw-r--r--   0 jason      (502) staff       (20)     5701 2023-06-17 22:57:37.000000 hdcms-bindings-0.1.5/hdcms-c/src/util/peak.h
-drwxr-xr-x   0 jason      (502) staff       (20)        0 2023-06-20 08:57:22.225144 hdcms-bindings-0.1.5/hdcms_bindings.egg-info/
--rw-r--r--   0 jason      (502) staff       (20)     5514 2023-06-20 08:57:22.000000 hdcms-bindings-0.1.5/hdcms_bindings.egg-info/PKG-INFO
--rw-r--r--   0 jason      (502) staff       (20)      421 2023-06-20 08:57:22.000000 hdcms-bindings-0.1.5/hdcms_bindings.egg-info/SOURCES.txt
--rw-r--r--   0 jason      (502) staff       (20)        1 2023-06-20 08:57:22.000000 hdcms-bindings-0.1.5/hdcms_bindings.egg-info/dependency_links.txt
--rw-r--r--   0 jason      (502) staff       (20)       15 2023-06-20 08:57:22.000000 hdcms-bindings-0.1.5/hdcms_bindings.egg-info/top_level.txt
--rw-r--r--   0 jason      (502) staff       (20)      538 2023-06-20 08:56:42.000000 hdcms-bindings-0.1.5/pyproject.toml
--rw-r--r--   0 jason      (502) staff       (20)     9415 2023-06-20 08:54:44.000000 hdcms-bindings-0.1.5/python.c
--rw-r--r--   0 jason      (502) staff       (20)       38 2023-06-20 08:57:22.225528 hdcms-bindings-0.1.5/setup.cfg
--rw-r--r--   0 jason      (502) staff       (20)      590 2023-02-03 06:07:14.000000 hdcms-bindings-0.1.5/setup.py
+drwxr-xr-x   0 jason      (502) staff       (20)        0 2023-06-21 00:06:23.312436 hdcms-bindings-0.1.6/
+-rw-r--r--   0 jason      (502) staff       (20)     1830 2023-01-22 19:56:08.000000 hdcms-bindings-0.1.6/LICENSE
+-rw-r--r--   0 jason      (502) staff       (20)      146 2023-02-03 06:05:56.000000 hdcms-bindings-0.1.6/MANIFEST.in
+-rw-r--r--   0 jason      (502) staff       (20)     5530 2023-06-21 00:06:23.312268 hdcms-bindings-0.1.6/PKG-INFO
+-rw-r--r--   0 jason      (502) staff       (20)     3053 2023-06-21 00:06:16.000000 hdcms-bindings-0.1.6/README.md
+drwxr-xr-x   0 jason      (502) staff       (20)        0 2023-06-21 00:06:23.299867 hdcms-bindings-0.1.6/hdcms-c/
+drwxr-xr-x   0 jason      (502) staff       (20)        0 2023-06-21 00:06:23.303650 hdcms-bindings-0.1.6/hdcms-c/src/
+-rw-r--r--   0 jason      (502) staff       (20)      882 2023-02-03 05:04:03.000000 hdcms-bindings-0.1.6/hdcms-c/src/fixwindows.h
+-rw-r--r--   0 jason      (502) staff       (20)    10313 2023-06-20 23:47:59.000000 hdcms-bindings-0.1.6/hdcms-c/src/main.c
+-rw-r--r--   0 jason      (502) staff       (20)       48 2023-02-03 05:04:03.000000 hdcms-bindings-0.1.6/hdcms-c/src/main.h
+drwxr-xr-x   0 jason      (502) staff       (20)        0 2023-06-21 00:06:23.306730 hdcms-bindings-0.1.6/hdcms-c/src/util/
+-rw-r--r--   0 jason      (502) staff       (20)    20530 2023-06-20 08:03:24.000000 hdcms-bindings-0.1.6/hdcms-c/src/util/array.c
+-rw-r--r--   0 jason      (502) staff       (20)     9226 2023-06-17 22:57:37.000000 hdcms-bindings-0.1.6/hdcms-c/src/util/array.h
+-rw-r--r--   0 jason      (502) staff       (20)     4318 2023-06-20 08:03:24.000000 hdcms-bindings-0.1.6/hdcms-c/src/util/bin.c
+-rw-r--r--   0 jason      (502) staff       (20)     2880 2023-06-18 17:14:08.000000 hdcms-bindings-0.1.6/hdcms-c/src/util/bin.h
+-rw-r--r--   0 jason      (502) staff       (20)     8646 2023-06-20 23:51:42.000000 hdcms-bindings-0.1.6/hdcms-c/src/util/peak.c
+-rw-r--r--   0 jason      (502) staff       (20)     5701 2023-06-17 22:57:37.000000 hdcms-bindings-0.1.6/hdcms-c/src/util/peak.h
+drwxr-xr-x   0 jason      (502) staff       (20)        0 2023-06-21 00:06:23.312048 hdcms-bindings-0.1.6/hdcms_bindings.egg-info/
+-rw-r--r--   0 jason      (502) staff       (20)     5530 2023-06-21 00:06:23.000000 hdcms-bindings-0.1.6/hdcms_bindings.egg-info/PKG-INFO
+-rw-r--r--   0 jason      (502) staff       (20)      421 2023-06-21 00:06:23.000000 hdcms-bindings-0.1.6/hdcms_bindings.egg-info/SOURCES.txt
+-rw-r--r--   0 jason      (502) staff       (20)        1 2023-06-21 00:06:23.000000 hdcms-bindings-0.1.6/hdcms_bindings.egg-info/dependency_links.txt
+-rw-r--r--   0 jason      (502) staff       (20)       15 2023-06-21 00:06:23.000000 hdcms-bindings-0.1.6/hdcms_bindings.egg-info/top_level.txt
+-rw-r--r--   0 jason      (502) staff       (20)      538 2023-06-21 00:06:03.000000 hdcms-bindings-0.1.6/pyproject.toml
+-rw-r--r--   0 jason      (502) staff       (20)     9465 2023-06-21 00:05:56.000000 hdcms-bindings-0.1.6/python.c
+-rw-r--r--   0 jason      (502) staff       (20)       38 2023-06-21 00:06:23.312482 hdcms-bindings-0.1.6/setup.cfg
+-rw-r--r--   0 jason      (502) staff       (20)      590 2023-02-03 06:07:14.000000 hdcms-bindings-0.1.6/setup.py
```

### Comparing `hdcms-bindings-0.1.5/LICENSE` & `hdcms-bindings-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hdcms-bindings-0.1.5/PKG-INFO` & `hdcms-bindings-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdcms-bindings
-Version: 0.1.5
+Version: 0.1.6
 Summary: This package wraps the C functions in hdcms
 Author: Arun Moorthy
 Author-email: Jason Eveleth <hdcms@jasoneveleth.com>
 License: NIST-developed software is provided by NIST as a public service. You may use,
         copy, and distribute copies of the software in any medium, provided that you
         keep intact this entire notice. You may improve, modify, and create derivative
         works of the software or any portion of the software, and you may copy and
@@ -87,14 +87,16 @@
 https://docs.python.org/3/extending/extending.html#building-arbitrary-values
 https://numpy.org/doc/stable/user/c-info.how-to-extend.html
 https://numpy.org/doc/stable/reference/c-api/array.html#c.PyArray_SimpleNew
 https://numpy.org/doc/stable/reference/c-api/dtype.html
 
 # Changelog
 
+0.1.6 Add xtol
+
 0.1.5 Update start, stop, num_bins, and scaling for both 1d and 2d
 
 0.1.4 Rename package (setup.py has the import name, which must match the c lib symbols)
 
 0.1.3 Rename package for real for real
 
 0.1.2 Rename package for real (broken)
```

### Comparing `hdcms-bindings-0.1.5/README.md` & `hdcms-bindings-0.1.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,16 @@
 https://docs.python.org/3/extending/extending.html#building-arbitrary-values
 https://numpy.org/doc/stable/user/c-info.how-to-extend.html
 https://numpy.org/doc/stable/reference/c-api/array.html#c.PyArray_SimpleNew
 https://numpy.org/doc/stable/reference/c-api/dtype.html
 
 # Changelog
 
+0.1.6 Add xtol
+
 0.1.5 Update start, stop, num_bins, and scaling for both 1d and 2d
 
 0.1.4 Rename package (setup.py has the import name, which must match the c lib symbols)
 
 0.1.3 Rename package for real for real
 
 0.1.2 Rename package for real (broken)
```

### Comparing `hdcms-bindings-0.1.5/hdcms-c/src/fixwindows.h` & `hdcms-bindings-0.1.6/hdcms-c/src/fixwindows.h`

 * *Files identical despite different names*

### Comparing `hdcms-bindings-0.1.5/hdcms-c/src/main.c` & `hdcms-bindings-0.1.6/hdcms-c/src/main.c`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         return false;
     }
     close(fd);
     return true;
 }
 
 static struct matrix
-filenames_to_stats(char *str, int mflag, double start, double end, double num_bins, char scaling)
+filenames_to_stats(char *str, int mflag, double start, double end, double num_bins, char scaling, double xtol)
 {
     struct matarray arr = matarr_zeros(2);
 
     char *path;
     size_t i;
     for (i = 0; (path = find_token(&str, " ,\n\t")); i++) {
         if ((size_t)i == arr.length) { // resize
@@ -94,16 +94,19 @@
         matarr_set(arr, i, m);
     }
     arr.length = i; // wastes some of the malloc'd mem but that's okay
     struct matrix stats;
     if (mflag == ONED) {
         stats = bin_stat_1D(arr, start, end, num_bins);
     } else if (mflag == TWOD) {
-        size_t n = matarr_get(arr, 0).len1; // >= longest possible length
-        stats = peak_stat(arr, n, inf);
+        size_t n = 0;
+        for (size_t i = 0; i < arr.length; i++) {
+            n += matarr_get(arr, i).len1;
+        }
+        stats = peak_stat(arr, n, xtol);
     } else {
         printf("\n");
         usage();
     }
     matarr_free(arr);
     return stats;
 }
@@ -123,23 +126,23 @@
     rewind(fileptr);            // Jump back to the beginning of the file
 
     buffer = malloc(len + 1);            // Enough memory for the file (and NUL)
     fread(buffer, len, 1, fileptr);      // Read in the entire file
     fclose(fileptr);                     // Close the file
     buffer[len] = '\0';                  // NUL terminate the string
 
-    struct matrix stats = filenames_to_stats(buffer, mflag, 0, 900. * (8999. / 9000.), 9000., 'm');
+    struct matrix stats = filenames_to_stats(buffer, mflag, 0, 900. * (8999. / 9000.), 9000., 'm', inf);
     free(buffer);
     matarr_set(arr, i, stats);
 }
 
 static void
 list_option(char *str, struct matarray arr, const size_t i)
 {
-    struct matrix stats = filenames_to_stats(str, mflag, 0, 900. * (8999. / 9000.), 9000., 'm');
+    struct matrix stats = filenames_to_stats(str, mflag, 0, 900. * (8999. / 9000.), 9000., 'm', inf);
     matarr_set(arr, i, stats);
 }
 
 static void
 print_comparison(const struct matrix m)
 {
     printf("╭────┬");
```

### Comparing `hdcms-bindings-0.1.5/hdcms-c/src/util/array.c` & `hdcms-bindings-0.1.6/hdcms-c/src/util/array.c`

 * *Files identical despite different names*

### Comparing `hdcms-bindings-0.1.5/hdcms-c/src/util/array.h` & `hdcms-bindings-0.1.6/hdcms-c/src/util/array.h`

 * *Files identical despite different names*

### Comparing `hdcms-bindings-0.1.5/hdcms-c/src/util/bin.c` & `hdcms-bindings-0.1.6/hdcms-c/src/util/bin.c`

 * *Files identical despite different names*

### Comparing `hdcms-bindings-0.1.5/hdcms-c/src/util/bin.h` & `hdcms-bindings-0.1.6/hdcms-c/src/util/bin.h`

 * *Files identical despite different names*

### Comparing `hdcms-bindings-0.1.5/hdcms-c/src/util/peak.c` & `hdcms-bindings-0.1.6/hdcms-c/src/util/peak.c`

 * *Files identical despite different names*

### Comparing `hdcms-bindings-0.1.5/hdcms-c/src/util/peak.h` & `hdcms-bindings-0.1.6/hdcms-c/src/util/peak.h`

 * *Files identical despite different names*

### Comparing `hdcms-bindings-0.1.5/hdcms_bindings.egg-info/PKG-INFO` & `hdcms-bindings-0.1.6/hdcms_bindings.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdcms-bindings
-Version: 0.1.5
+Version: 0.1.6
 Summary: This package wraps the C functions in hdcms
 Author: Arun Moorthy
 Author-email: Jason Eveleth <hdcms@jasoneveleth.com>
 License: NIST-developed software is provided by NIST as a public service. You may use,
         copy, and distribute copies of the software in any medium, provided that you
         keep intact this entire notice. You may improve, modify, and create derivative
         works of the software or any portion of the software, and you may copy and
@@ -87,14 +87,16 @@
 https://docs.python.org/3/extending/extending.html#building-arbitrary-values
 https://numpy.org/doc/stable/user/c-info.how-to-extend.html
 https://numpy.org/doc/stable/reference/c-api/array.html#c.PyArray_SimpleNew
 https://numpy.org/doc/stable/reference/c-api/dtype.html
 
 # Changelog
 
+0.1.6 Add xtol
+
 0.1.5 Update start, stop, num_bins, and scaling for both 1d and 2d
 
 0.1.4 Rename package (setup.py has the import name, which must match the c lib symbols)
 
 0.1.3 Rename package for real for real
 
 0.1.2 Rename package for real (broken)
```

### Comparing `hdcms-bindings-0.1.5/pyproject.toml` & `hdcms-bindings-0.1.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "numpy", "toml"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hdcms-bindings"
-version = "0.1.5"
+version = "0.1.6"
 description = "This package wraps the C functions in hdcms"
 authors = [
     {name="Jason Eveleth", email="hdcms@jasoneveleth.com"},
     {name="Arun Moorthy"},
 ]
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `hdcms-bindings-0.1.5/python.c` & `hdcms-bindings-0.1.6/python.c`

 * *Files 2% similar despite different names*

```diff
@@ -88,38 +88,39 @@
         PyErr_SetString(PyExc_RuntimeError, "failed to parse args (in C)");
         return NULL;
     }
 
     int len = strlen(str) + 1;
     char *copy = safe_calloc(len, 1);
     strncpy(copy, str, len);
-    struct matrix m = filenames_to_stats(copy, ONED, start, end, num_bins, scaling[0]);
+    struct matrix m = filenames_to_stats(copy, ONED, start, end, num_bins, scaling[0], inf);
 
     assert(m.is_owner);
 
     return mat_to_pyobject(m);
 }
 
 static PyObject*
 filenames_to_stats_2d_cfunc(PyObject *dummy, PyObject *args, PyObject *kwargs)
 {
-    static char *kwlist[] = {"filenames", "scaling", NULL};
+    static char *kwlist[] = {"filenames", "scaling", "xtol", NULL};
 
     const char *str;
     const char *scaling = "m";
-    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "s|s", kwlist, &str, &scaling)) {
+    double xtol = inf;
+    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "s|sd", kwlist, &str, &scaling, &xtol)) {
         PyErr_SetString(PyExc_RuntimeError, "failed to parse args (in C)");
         return NULL;
     }
 
     int len = strlen(str) + 1;
     char *copy = safe_calloc(len, 1);
     strncpy(copy, str, len);
     // we can pass dummy values since they will be singored by the mflag
-    struct matrix m = filenames_to_stats(copy, TWOD, 0, 0, 0, scaling[0]);
+    struct matrix m = filenames_to_stats(copy, TWOD, 0, 0, 0, scaling[0], xtol);
 
     assert(m.is_owner);
 
     return mat_to_pyobject(m);
 }
 
 static PyObject*
```

### Comparing `hdcms-bindings-0.1.5/setup.py` & `hdcms-bindings-0.1.6/setup.py`

 * *Files identical despite different names*

