# Comparing `tmp/ladok3-3.8.tar.gz` & `tmp/ladok3-3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ladok3-3.8.tar", max compression
+gzip compressed data, was "ladok3-3.9.tar", max compression
```

## Comparing `ladok3-3.8.tar` & `ladok3-3.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1155 2023-02-09 10:24:29.151703 ladok3-3.8/LICENSE
--rw-r--r--   0        0        0     6677 2022-10-25 12:52:56.416560 ladok3-3.8/README.md
--rw-r--r--   0        0        0      980 2023-02-09 10:25:13.624003 ladok3-3.8/doc/Makefile
--rw-r--r--   0        0        0      173 2022-10-25 09:48:40.909030 ladok3-3.8/doc/abstract.tex
--rw-r--r--   0        0        0     3723 2023-02-09 10:24:29.155703 ladok3-3.8/doc/ladok3.tex
--rw-r--r--   0        0        0     1160 2022-10-25 09:48:40.917030 ladok3-3.8/doc/preamble.tex
--rw-r--r--   0        0        0     3276 2022-10-25 09:54:49.529819 ladok3-3.8/makefiles/doc.mk
--rw-r--r--   0        0        0     1326 2022-10-20 12:02:01.907186 ladok3-3.8/makefiles/exam.mk
--rw-r--r--   0        0        0       66 2022-10-20 12:02:01.903186 ladok3-3.8/makefiles/haskell.mk
--rw-r--r--   0        0        0      820 2022-10-20 12:02:01.907186 ladok3-3.8/makefiles/miun.course.mk
--rw-r--r--   0        0        0     6206 2022-10-20 12:02:01.903186 ladok3-3.8/makefiles/miun.depend.mk
--rw-r--r--   0        0        0      664 2022-10-20 12:02:01.903186 ladok3-3.8/makefiles/miun.docs.mk
--rw-r--r--   0        0        0      611 2022-10-20 12:02:01.903186 ladok3-3.8/makefiles/miun.port.mk
--rw-r--r--   0        0        0      709 2022-10-20 12:02:01.903186 ladok3-3.8/makefiles/miun.pub.mk
--rw-r--r--   0        0        0     2880 2022-10-20 12:02:01.907186 ladok3-3.8/makefiles/noweb.mk
--rw-r--r--   0        0        0     2363 2022-10-20 12:02:01.907186 ladok3-3.8/makefiles/pkg.mk
--rw-r--r--   0        0        0     1225 2022-10-20 12:02:01.907186 ladok3-3.8/makefiles/portability.mk
--rw-r--r--   0        0        0     4827 2022-10-25 09:54:49.533819 ladok3-3.8/makefiles/pub.mk
--rw-r--r--   0        0        0     2321 2022-10-20 12:02:01.903186 ladok3-3.8/makefiles/results.mk
--rw-r--r--   0        0        0      421 2022-10-20 12:02:01.903186 ladok3-3.8/makefiles/subdir.mk
--rw-r--r--   0        0        0     6376 2022-10-25 09:54:49.533819 ladok3-3.8/makefiles/tex.mk
--rw-r--r--   0        0        0     2536 2022-10-20 12:02:01.903186 ladok3-3.8/makefiles/transform.mk
--rw-r--r--   0        0        0     1766 2023-06-08 20:55:19.256631 ladok3-3.8/pyproject.toml
--rw-r--r--   0        0        0       81 2022-10-25 12:52:56.440560 ladok3-3.8/src/ladok3/.gitignore
--rw-r--r--   0        0        0      557 2023-02-09 10:24:29.155703 ladok3-3.8/src/ladok3/Makefile
--rw-r--r--   0        0        0    43238 2023-02-09 19:44:21.886639 ladok3-3.8/src/ladok3/api.nw
--rw-r--r--   0        0        0    20472 2023-03-24 09:13:29.004895 ladok3-3.8/src/ladok3/cli.nw
--rw-r--r--   0        0        0    11785 2023-03-24 10:51:01.801680 ladok3-3.8/src/ladok3/data.nw
--rw-r--r--   0        0        0    50144 2023-06-08 19:44:13.018284 ladok3-3.8/src/ladok3/ladok3.nw
--rw-r--r--   0        0        0     8461 2023-06-08 20:34:03.363626 ladok3-3.8/src/ladok3/report.nw
--rw-r--r--   0        0        0     3747 2023-06-08 20:54:19.896194 ladok3-3.8/src/ladok3/student.nw
--rw-r--r--   0        0        0   180333 2023-02-09 19:28:11.895452 ladok3-3.8/src/ladok3/undoc.nw
--rw-r--r--   0        0        0     8098 1970-01-01 00:00:00.000000 ladok3-3.8/PKG-INFO
+-rw-r--r--   0        0        0     1155 2023-02-09 10:24:29.151703 ladok3-3.9/LICENSE
+-rw-r--r--   0        0        0     6677 2022-10-25 12:52:56.416560 ladok3-3.9/README.md
+-rw-r--r--   0        0        0      980 2023-02-09 10:25:13.624003 ladok3-3.9/doc/Makefile
+-rw-r--r--   0        0        0      173 2022-10-25 09:48:40.909030 ladok3-3.9/doc/abstract.tex
+-rw-r--r--   0        0        0     3723 2023-02-09 10:24:29.155703 ladok3-3.9/doc/ladok3.tex
+-rw-r--r--   0        0        0     1160 2022-10-25 09:48:40.917030 ladok3-3.9/doc/preamble.tex
+-rw-r--r--   0        0        0     3276 2022-10-25 09:54:49.529819 ladok3-3.9/makefiles/doc.mk
+-rw-r--r--   0        0        0     1326 2022-10-20 12:02:01.907186 ladok3-3.9/makefiles/exam.mk
+-rw-r--r--   0        0        0       66 2022-10-20 12:02:01.903186 ladok3-3.9/makefiles/haskell.mk
+-rw-r--r--   0        0        0      820 2022-10-20 12:02:01.907186 ladok3-3.9/makefiles/miun.course.mk
+-rw-r--r--   0        0        0     6206 2022-10-20 12:02:01.903186 ladok3-3.9/makefiles/miun.depend.mk
+-rw-r--r--   0        0        0      664 2022-10-20 12:02:01.903186 ladok3-3.9/makefiles/miun.docs.mk
+-rw-r--r--   0        0        0      611 2022-10-20 12:02:01.903186 ladok3-3.9/makefiles/miun.port.mk
+-rw-r--r--   0        0        0      709 2022-10-20 12:02:01.903186 ladok3-3.9/makefiles/miun.pub.mk
+-rw-r--r--   0        0        0     2912 2023-06-09 13:33:51.987944 ladok3-3.9/makefiles/noweb.mk
+-rw-r--r--   0        0        0     2363 2023-06-09 13:33:51.611939 ladok3-3.9/makefiles/pkg.mk
+-rw-r--r--   0        0        0     1225 2023-06-09 13:33:51.971944 ladok3-3.9/makefiles/portability.mk
+-rw-r--r--   0        0        0     4827 2023-06-09 13:33:51.579938 ladok3-3.9/makefiles/pub.mk
+-rw-r--r--   0        0        0     2321 2022-10-20 12:02:01.903186 ladok3-3.9/makefiles/results.mk
+-rw-r--r--   0        0        0      421 2022-10-20 12:02:01.903186 ladok3-3.9/makefiles/subdir.mk
+-rw-r--r--   0        0        0     6376 2023-06-09 13:33:51.979944 ladok3-3.9/makefiles/tex.mk
+-rw-r--r--   0        0        0     2536 2022-10-20 12:02:01.903186 ladok3-3.9/makefiles/transform.mk
+-rw-r--r--   0        0        0     1766 2023-06-21 18:26:12.197504 ladok3-3.9/pyproject.toml
+-rw-r--r--   0        0        0       81 2022-10-25 12:52:56.440560 ladok3-3.9/src/ladok3/.gitignore
+-rw-r--r--   0        0        0      557 2023-02-09 10:24:29.155703 ladok3-3.9/src/ladok3/Makefile
+-rw-r--r--   0        0        0    43238 2023-02-09 19:44:21.886639 ladok3-3.9/src/ladok3/api.nw
+-rw-r--r--   0        0        0    20641 2023-06-21 18:24:44.772562 ladok3-3.9/src/ladok3/cli.nw
+-rw-r--r--   0        0        0    11785 2023-03-24 10:51:01.801680 ladok3-3.9/src/ladok3/data.nw
+-rw-r--r--   0        0        0    50144 2023-06-08 19:44:13.018284 ladok3-3.9/src/ladok3/ladok3.nw
+-rw-r--r--   0        0        0     8461 2023-06-08 20:34:03.363626 ladok3-3.9/src/ladok3/report.nw
+-rw-r--r--   0        0        0     3747 2023-06-08 20:54:19.896194 ladok3-3.9/src/ladok3/student.nw
+-rw-r--r--   0        0        0   180333 2023-02-09 19:28:11.895452 ladok3-3.9/src/ladok3/undoc.nw
+-rw-r--r--   0        0        0     8098 1970-01-01 00:00:00.000000 ladok3-3.9/PKG-INFO
```

### Comparing `ladok3-3.8/LICENSE` & `ladok3-3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ladok3-3.8/README.md` & `ladok3-3.9/README.md`

 * *Files identical despite different names*

### Comparing `ladok3-3.8/doc/Makefile` & `ladok3-3.9/doc/Makefile`

 * *Files identical despite different names*

### Comparing `ladok3-3.8/doc/ladok3.tex` & `ladok3-3.9/doc/ladok3.tex`

 * *Files identical despite different names*

### Comparing `ladok3-3.8/doc/preamble.tex` & `ladok3-3.9/doc/preamble.tex`

 * *Files identical despite different names*

### Comparing `ladok3-3.8/makefiles/doc.mk` & `ladok3-3.9/makefiles/doc.mk`

 * *Files identical despite different names*

### Comparing `ladok3-3.8/makefiles/exam.mk` & `ladok3-3.9/makefiles/exam.mk`

 * *Files identical despite different names*

### Comparing `ladok3-3.8/makefiles/miun.course.mk` & `ladok3-3.9/makefiles/miun.course.mk`

 * *Files identical despite different names*

### Comparing `ladok3-3.8/makefiles/miun.depend.mk` & `ladok3-3.9/makefiles/miun.depend.mk`

 * *Files identical despite different names*

### Comparing `ladok3-3.8/makefiles/miun.docs.mk` & `ladok3-3.9/makefiles/miun.docs.mk`

 * *Files identical despite different names*

### Comparing `ladok3-3.8/makefiles/miun.port.mk` & `ladok3-3.9/makefiles/miun.port.mk`

 * *Files identical despite different names*

### Comparing `ladok3-3.8/makefiles/miun.pub.mk` & `ladok3-3.9/makefiles/miun.pub.mk`

 * *Files identical despite different names*

### Comparing `ladok3-3.8/makefiles/noweb.mk` & `ladok3-3.9/makefiles/noweb.mk`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ifndef NOWEB_MK
 NOWEB_MK = true
 
 NOWEAVE.tex?=       noweave ${NOWEAVEFLAGS.tex} $< > $@
-NOWEAVEFLAGS.tex?=  -x -n -delay -t2
+NOWEAVEFLAGS.tex?=  ${NOWEAVEFLAGS} -x -n -delay -t2
 NOWEAVE.pdf?=       \
   noweave ${NOWEAVEFLAGS.pdf} $< > ${@:.pdf=.tex} && \
   latexmk -pdf ${@:.pdf=.tex}
-NOWEAVEFLAGS.pdf?=  -x -t2
+NOWEAVEFLAGS.pdf?=  ${NOWEAVEFLAGS} -x -t2
 NOTANGLEFLAGS?=
 NOTANGLE?=      notangle ${NOTANGLEFLAGS} -R$(notdir $@) $(filter %.nw,$^) | \
                   ${CPIF} $@
 CPIF?=          cpif
 NOWEB_SUFFIXES+=    .c .cc .cpp .cxx
 NOTANGLEFLAGS.c?=   -L
 NOTANGLE.c?=        notangle ${NOTANGLEFLAGS.c} -R$(notdir $@) \
```

### Comparing `ladok3-3.8/makefiles/pkg.mk` & `ladok3-3.9/makefiles/pkg.mk`

 * *Files identical despite different names*

### Comparing `ladok3-3.8/makefiles/portability.mk` & `ladok3-3.9/makefiles/portability.mk`

 * *Files identical despite different names*

### Comparing `ladok3-3.8/makefiles/pub.mk` & `ladok3-3.9/makefiles/pub.mk`

 * *Files identical despite different names*

### Comparing `ladok3-3.8/makefiles/results.mk` & `ladok3-3.9/makefiles/results.mk`

 * *Files identical despite different names*

### Comparing `ladok3-3.8/makefiles/tex.mk` & `ladok3-3.9/makefiles/tex.mk`

 * *Files identical despite different names*

### Comparing `ladok3-3.8/makefiles/transform.mk` & `ladok3-3.9/makefiles/transform.mk`

 * *Files identical despite different names*

### Comparing `ladok3-3.8/pyproject.toml` & `ladok3-3.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ladok3"
-version = "3.8"
+version = "3.9"
 description = "Python wrapper and CLI for the LADOK3 REST API."
 authors = [
   "Daniel Bosk <dbosk@kth.se>",
   "Alexander Baltatzis",
   "Gerald Q. Maguire Jr"
 ]
 license = "MIT"
```

### Comparing `ladok3-3.8/src/ladok3/Makefile` & `ladok3-3.9/src/ladok3/Makefile`

 * *Files identical despite different names*

### Comparing `ladok3-3.8/src/ladok3/api.nw` & `ladok3-3.9/src/ladok3/api.nw`

 * *Files identical despite different names*

### Comparing `ladok3-3.8/src/ladok3/cli.nw` & `ladok3-3.9/src/ladok3/cli.nw`

 * *Files 2% similar despite different names*

```diff
@@ -284,15 +284,17 @@
 The rest we don't need to do much about, merely point out the possibilities to 
 the user.
 <<login description>>=
 Manages the user's LADOK login credentials. There are three ways to supply the 
 login credentials, in order of priority:
 
 1) Through the system keyring: Just run `ladok login` and you'll be asked to 
-   enter the credentials and they will be stored in the keyring.
+   enter the credentials and they will be stored in the keyring. Note that for 
+   this to work on the WSL platform (and possibly on Windows), you need to 
+   install the `keyrings.alt` package: `python3 -m pip install keyrings.alt`.
 
 2) Through the environment: Just set the environment variables
 
   a) LADOK_INST, the name of the institution, e.g. KTH Royal Institute of 
   Technology;
   b) LADOK_VARS, a colon-separated list of environment variables, similarly to 
   what's done in `ladok login` --- most don't need this, but can rather set
```

### Comparing `ladok3-3.8/src/ladok3/data.nw` & `ladok3-3.9/src/ladok3/data.nw`

 * *Files identical despite different names*

### Comparing `ladok3-3.8/src/ladok3/ladok3.nw` & `ladok3-3.9/src/ladok3/ladok3.nw`

 * *Files identical despite different names*

### Comparing `ladok3-3.8/src/ladok3/report.nw` & `ladok3-3.9/src/ladok3/report.nw`

 * *Files identical despite different names*

### Comparing `ladok3-3.8/src/ladok3/student.nw` & `ladok3-3.9/src/ladok3/student.nw`

 * *Files identical despite different names*

### Comparing `ladok3-3.8/src/ladok3/undoc.nw` & `ladok3-3.9/src/ladok3/undoc.nw`

 * *Files identical despite different names*

### Comparing `ladok3-3.8/PKG-INFO` & `ladok3-3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ladok3
-Version: 3.8
+Version: 3.9
 Summary: Python wrapper and CLI for the LADOK3 REST API.
 Home-page: https://github.com/dbosk/ladok3
 License: MIT
 Keywords: ladok3,ladok
 Author: Daniel Bosk
 Author-email: dbosk@kth.se
 Requires-Python: >=3.8,<4.0
```

