# Comparing `tmp/setuptools_dso-2.8a1.tar.gz` & `tmp/setuptools_dso-2.9a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/setuptools_dso-2.8a1.tar", last modified: Tue May  2 20:00:31 2023, max compression
+gzip compressed data, was "dist/setuptools_dso-2.9a1.tar", last modified: Wed Jun 21 18:43:40 2023, max compression
```

## Comparing `setuptools_dso-2.8a1.tar` & `setuptools_dso-2.9a1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:00:31.000000 setuptools_dso-2.8a1/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-02 20:00:17.000000 setuptools_dso-2.8a1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-02 20:00:17.000000 setuptools_dso-2.8a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-02 20:00:17.000000 setuptools_dso-2.8a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-02 20:00:31.000000 setuptools_dso-2.8a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-02 20:00:17.000000 setuptools_dso-2.8a1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-02 20:00:17.000000 setuptools_dso-2.8a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-02 20:00:31.000000 setuptools_dso-2.8a1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1357 2023-05-02 20:00:17.000000 setuptools_dso-2.8a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:00:31.000000 setuptools_dso-2.8a1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:00:31.000000 setuptools_dso-2.8a1/src/setuptools_dso/
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-05-02 20:00:17.000000 setuptools_dso-2.8a1/src/setuptools_dso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-05-02 20:00:17.000000 setuptools_dso-2.8a1/src/setuptools_dso/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)    26488 2023-05-02 20:00:17.000000 setuptools_dso-2.8a1/src/setuptools_dso/dsocmd.py
--rw-r--r--   0 runner    (1001) docker     (123)    16544 2023-05-02 20:00:17.000000 setuptools_dso-2.8a1/src/setuptools_dso/probe.py
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-05-02 20:00:17.000000 setuptools_dso-2.8a1/src/setuptools_dso/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:00:31.000000 setuptools_dso-2.8a1/src/setuptools_dso/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:00:17.000000 setuptools_dso-2.8a1/src/setuptools_dso/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-02 20:00:17.000000 setuptools_dso-2.8a1/src/setuptools_dso/test/test_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-02 20:00:17.000000 setuptools_dso-2.8a1/src/setuptools_dso/test/test_probe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:00:31.000000 setuptools_dso-2.8a1/src/setuptools_dso.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-02 20:00:31.000000 setuptools_dso-2.8a1/src/setuptools_dso.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-02 20:00:31.000000 setuptools_dso-2.8a1/src/setuptools_dso.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 20:00:31.000000 setuptools_dso-2.8a1/src/setuptools_dso.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-02 20:00:31.000000 setuptools_dso-2.8a1/src/setuptools_dso.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-02 20:00:31.000000 setuptools_dso-2.8a1/src/setuptools_dso.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:43:40.000000 setuptools_dso-2.9a1/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-21 18:43:24.000000 setuptools_dso-2.9a1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-21 18:43:24.000000 setuptools_dso-2.9a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-21 18:43:24.000000 setuptools_dso-2.9a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-21 18:43:40.000000 setuptools_dso-2.9a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-21 18:43:24.000000 setuptools_dso-2.9a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-21 18:43:24.000000 setuptools_dso-2.9a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-21 18:43:40.000000 setuptools_dso-2.9a1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1357 2023-06-21 18:43:24.000000 setuptools_dso-2.9a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:43:40.000000 setuptools_dso-2.9a1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:43:40.000000 setuptools_dso-2.9a1/src/setuptools_dso/
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-06-21 18:43:24.000000 setuptools_dso-2.9a1/src/setuptools_dso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-06-21 18:43:24.000000 setuptools_dso-2.9a1/src/setuptools_dso/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26488 2023-06-21 18:43:24.000000 setuptools_dso-2.9a1/src/setuptools_dso/dsocmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17335 2023-06-21 18:43:24.000000 setuptools_dso-2.9a1/src/setuptools_dso/probe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-06-21 18:43:24.000000 setuptools_dso-2.9a1/src/setuptools_dso/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:43:40.000000 setuptools_dso-2.9a1/src/setuptools_dso/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 18:43:24.000000 setuptools_dso-2.9a1/src/setuptools_dso/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-21 18:43:24.000000 setuptools_dso-2.9a1/src/setuptools_dso/test/test_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-06-21 18:43:24.000000 setuptools_dso-2.9a1/src/setuptools_dso/test/test_probe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:43:40.000000 setuptools_dso-2.9a1/src/setuptools_dso.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-21 18:43:39.000000 setuptools_dso-2.9a1/src/setuptools_dso.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-21 18:43:39.000000 setuptools_dso-2.9a1/src/setuptools_dso.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 18:43:39.000000 setuptools_dso-2.9a1/src/setuptools_dso.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-21 18:43:39.000000 setuptools_dso-2.9a1/src/setuptools_dso.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-21 18:43:39.000000 setuptools_dso-2.9a1/src/setuptools_dso.egg-info/top_level.txt
```

### Comparing `setuptools_dso-2.8a1/LICENSE` & `setuptools_dso-2.9a1/LICENSE`

 * *Files identical despite different names*

### Comparing `setuptools_dso-2.8a1/PKG-INFO` & `setuptools_dso-2.9a1/src/setuptools_dso.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: setuptools_dso
-Version: 2.8a1
+Name: setuptools-dso
+Version: 2.9a1
 Summary: setuptools extension to build non-python shared libraries
 Home-page: https://github.com/mdavidsaver/setuptools_dso
 Author: Michael Davidsaver
 Author-email: mdavidsaver@gmail.com
 License: BSD
 Project-URL: Documentation, https://mdavidsaver.github.io/setuptools_dso
 Project-URL: Release Notes, https://mdavidsaver.github.io/setuptools_dso/releasenotes.html
```

### Comparing `setuptools_dso-2.8a1/README.md` & `setuptools_dso-2.9a1/README.md`

 * *Files identical despite different names*

### Comparing `setuptools_dso-2.8a1/setup.py` & `setuptools_dso-2.9a1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as F:
     long_description = F.read()
 
 setup(
     name='setuptools_dso',
-    version="2.8a1",
+    version="2.9a1",
     description="setuptools extension to build non-python shared libraries",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/mdavidsaver/setuptools_dso',
     project_urls={
         'Documentation':'https://mdavidsaver.github.io/setuptools_dso',
         'Release Notes':'https://mdavidsaver.github.io/setuptools_dso/releasenotes.html',
```

### Comparing `setuptools_dso-2.8a1/src/setuptools_dso/__init__.py` & `setuptools_dso-2.9a1/src/setuptools_dso/__init__.py`

 * *Files identical despite different names*

### Comparing `setuptools_dso-2.8a1/src/setuptools_dso/compiler.py` & `setuptools_dso-2.9a1/src/setuptools_dso/compiler.py`

 * *Files identical despite different names*

### Comparing `setuptools_dso-2.8a1/src/setuptools_dso/dsocmd.py` & `setuptools_dso-2.9a1/src/setuptools_dso/dsocmd.py`

 * *Files identical despite different names*

### Comparing `setuptools_dso-2.8a1/src/setuptools_dso/probe.py` & `setuptools_dso-2.9a1/src/setuptools_dso/probe.py`

 * *Files 12% similar despite different names*

```diff
@@ -240,70 +240,86 @@
             ''
         ]
 
         ret = self.try_compile('\n'.join(src), **kws)
         log.info('Probe Member %s::%s -> %s', struct, member, 'Present' if ret else 'Absent')
         return ret
 
-    def eval_macros(self, macros, headers=None, define_macros=None, **kws):
+    def eval_macros(self, macros, headers=None, define_macros=None, language='c', **kws):
         """Expand C/C++ preprocessor macros.
 
         For undefined macros, None is returned.
         For defined macros a string is returned.
         When evaluating multiple macros, the order of the macros argument is preserved
         in the OrderedDict which is returned.
 
         :returns: An OrderedDict mapping to string (if defined) or None (if not defined)
         :param str|list macros: A macro name string, or a list of such strings
         :param list headers: List of headers to include during all test compilations
         :param list define_macros: Extra macro definitions.
+        :param str language: Source code language: 'c' or 'c++'  (Added in 2.9)
         :param list include_dirs: Extra directories to search for headers
         :param list extra_preargs: Extra arguments to pass to the compiler
         :param list extra_postargs: Extra arguments to pass to the compiler
         """
         if isinstance(macros, str):
             macros = [macros]
 
-        srcname = os.path.join(self.tempdir, self._source_name('eval_macros_in', **kws))
-        outname = os.path.join(self.tempdir, self._source_name('eval_macros_out', **kws))
+        srcname = os.path.join(self.tempdir, self._source_name('eval_macros_in', language=language, **kws))
+        outname = os.path.join(self.tempdir, self._source_name('eval_macros_out', language=language, **kws))
 
         define_macros = self.define_macros + list(define_macros or [])
         src = ['#include <%s>'%h for h in self.headers+list(headers or ())]
 
         for macro in macros:
             src.append('''
 #if defined({macro})
-void D_{macro} = |||{macro}|||;
+void D_{macro} = |||{macro}|||; void X_{macro};
 #else
-void U_{macro} = ||||||;
+void U_{macro} = ||||||; void X_{macro};
 #endif /* {macro} */
 '''.format(macro=macro))
 
         src = '\n'.join(src)
 
         with open(srcname, 'w') as F:
             F.write(src)
 
         self.compiler.preprocess(srcname, outname, macros=define_macros, **kws)
 
         with open(outname, 'r') as F:
             out = F.read()
 
-        defs = {}
-
-        for M in re.finditer(r'void ([DU])_([a-zA-Z_][a-zA-Z0-9_]*) = \|\|\|(.*?)\|\|\|;', out, re.MULTILINE):
-            du, name, val = M.groups()
+        # Various pre-processor implementations are inconsistent about
+        # what "debris" is emitted in the output.
+        # eg. GCC strips C/C++ comments, while MSVC leaves them in.
+
+        # remove pre-processor directive lines
+        out = re.sub(r'^\s*#[^\n\r]*$', '', out, 0, re.MULTILINE)
+        # remove c++ line comments
+        out = re.sub(r'^//[^\n\r]*$', '', out, 0, re.MULTILINE)
+        # remove C comments
+        out = re.sub(r'/\*.*?\*/', '', out, 0, re.MULTILINE|re.DOTALL)
+
+        defs = OrderedDict()
+
+        for name in macros:
+            pat = r'.*void ([DU])_%(name)s = \|\|\|(.*?)\|\|\|; void X_%(name)s;.*'%{'name':name}
+            M = re.match(pat, out, re.MULTILINE|re.DOTALL)
+            if M is None:
+                raise RuntimeError("In %r\nFailed to find match for %r using %r"%(out, name, pat))
+            du, val = M.groups()
             if du=='D':
-                defs[name] = val
+                defs[name] = val.strip()
             elif du=='U':
                 defs[name] = None
             else:
                 raise ValueError("Logic error {0!r} : {1!r}".format(M, M.groups()) )
 
-        return OrderedDict([(name, defs[name]) for name in macros]) # will error in some def was extracted
+        return defs
 
     @property
     def info(self):
         """Inspect toolchain
 
         :returns: A :py:class:`probe.ToolchainInfo`
         """
```

### Comparing `setuptools_dso-2.8a1/src/setuptools_dso/runtime.py` & `setuptools_dso-2.9a1/src/setuptools_dso/runtime.py`

 * *Files identical despite different names*

### Comparing `setuptools_dso-2.8a1/src/setuptools_dso/test/test_probe.py` & `setuptools_dso-2.9a1/src/setuptools_dso/test/test_probe.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,16 +46,26 @@
             ('NOVAL', ' '),
             ('MAGIC', '42'),
             ('HELLO', '"hello world"'),
             ('MULTILINE', 'this is a test'),
         ])
 
     def test_predef(self):
-        gnuc, clang, msc_ver = self.probe.eval_macros(['__GNUC__', '__clang__', '_MSC_VER'])
-        self.assertTrue(gnuc or clang or msc_ver)
+        # self ID for supported compilers
+        defs = self.probe.eval_macros(['__GNUC__', '__clang__', '_MSC_VER'])
+        self.assertTrue(any(defs.values()), str(defs))
+
+    def test_cxx(self):
+        defs = self.probe.eval_macros([
+            # ID for known C++ stdlib implementations
+            '__GLIBCXX__',     # g++
+            '_CPPLIB_VER',     # Dinkumware (aka. MSVC)
+            '_LIBCPP_VERSION', # clang
+        ], headers=['string'], language='c++')
+        self.assertTrue(any(defs.values()), str(defs))
 
     def test_info(self):
         info = self.probe.info
         print("Raw Macros", info._raw_macros)
         print("Info", info)
 
         self.assertIn(info.compiler, ('clang', 'gcc', 'msvc'))
```

### Comparing `setuptools_dso-2.8a1/src/setuptools_dso.egg-info/PKG-INFO` & `setuptools_dso-2.9a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: setuptools-dso
-Version: 2.8a1
+Name: setuptools_dso
+Version: 2.9a1
 Summary: setuptools extension to build non-python shared libraries
 Home-page: https://github.com/mdavidsaver/setuptools_dso
 Author: Michael Davidsaver
 Author-email: mdavidsaver@gmail.com
 License: BSD
 Project-URL: Documentation, https://mdavidsaver.github.io/setuptools_dso
 Project-URL: Release Notes, https://mdavidsaver.github.io/setuptools_dso/releasenotes.html
```

### Comparing `setuptools_dso-2.8a1/src/setuptools_dso.egg-info/SOURCES.txt` & `setuptools_dso-2.9a1/src/setuptools_dso.egg-info/SOURCES.txt`

 * *Files identical despite different names*

