# Comparing `tmp/filedata-0.2.2.tar.gz` & `tmp/filedata-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filedata-0.2.2.tar", last modified: Wed Jun 21 01:08:30 2023, max compression
+gzip compressed data, was "filedata-0.2.3.tar", last modified: Wed Jun 21 03:25:51 2023, max compression
```

## Comparing `filedata-0.2.2.tar` & `filedata-0.2.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 01:08:30.626152 filedata-0.2.2/
--rwxrwxrwx   0 root         (0) root         (0)      107 2023-06-21 00:08:49.000000 filedata-0.2.2/MANIFEST.in
--rwxrwxrwx   0 root         (0) root         (0)      490 2023-06-21 01:08:30.626152 filedata-0.2.2/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)       57 2023-06-21 00:08:49.000000 filedata-0.2.2/README.rst
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 01:08:30.344731 filedata-0.2.2/filedata/
--rwxrwxrwx   0 root         (0) root         (0)       22 2023-06-21 01:07:14.000000 filedata-0.2.2/filedata/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      841 2023-06-21 00:08:49.000000 filedata-0.2.2/filedata/config.py
--rwxrwxrwx   0 root         (0) root         (0)     3399 2023-06-21 00:08:49.000000 filedata-0.2.2/filedata/file.py
--rwxrwxrwx   0 root         (0) root         (0)     2895 2023-06-21 00:08:49.000000 filedata-0.2.2/filedata/html.py
--rwxrwxrwx   0 root         (0) root         (0)     6466 2023-06-21 00:08:49.000000 filedata-0.2.2/filedata/image.py
--rwxrwxrwx   0 root         (0) root         (0)      801 2023-06-21 00:08:49.000000 filedata-0.2.2/filedata/pdf.py
--rwxrwxrwx   0 root         (0) root         (0)     1198 2023-06-21 00:08:49.000000 filedata-0.2.2/filedata/retry.py
--rwxrwxrwx   0 root         (0) root         (0)      624 2023-06-21 01:07:06.000000 filedata-0.2.2/filedata/text.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 01:08:30.516776 filedata-0.2.2/filedata/text_algo/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 00:11:15.000000 filedata-0.2.2/filedata/text_algo/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2939 2023-06-21 01:03:57.000000 filedata-0.2.2/filedata/text_algo/ac.py
--rwxrwxrwx   0 root         (0) root         (0)       94 2023-06-21 00:08:49.000000 filedata-0.2.2/filedata/time.py
--rwxrwxrwx   0 root         (0) root         (0)      466 2023-06-21 00:08:49.000000 filedata-0.2.2/filedata/utils.py
--rwxrwxrwx   0 root         (0) root         (0)      252 2023-06-21 00:08:49.000000 filedata-0.2.2/filedata/video.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 01:08:30.454276 filedata-0.2.2/filedata.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      490 2023-06-21 01:08:29.000000 filedata-0.2.2/filedata.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      578 2023-06-21 01:08:30.000000 filedata-0.2.2/filedata.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-21 01:08:29.000000 filedata-0.2.2/filedata.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-21 01:08:29.000000 filedata-0.2.2/filedata.egg-info/not-zip-safe
--rwxrwxrwx   0 root         (0) root         (0)      124 2023-06-21 01:08:29.000000 filedata-0.2.2/filedata.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       15 2023-06-21 01:08:29.000000 filedata-0.2.2/filedata.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 01:08:30.532401 filedata-0.2.2/requirements/
--rwxrwxrwx   0 root         (0) root         (0)       18 2023-06-21 00:08:49.000000 filedata-0.2.2/requirements/test.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-06-21 01:08:30.626152 filedata-0.2.2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1549 2023-06-21 00:08:49.000000 filedata-0.2.2/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 01:08:30.563651 filedata-0.2.2/tests/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 00:08:49.000000 filedata-0.2.2/tests/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 01:08:30.594901 filedata-0.2.2/tests/test_text_algo/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 00:58:58.000000 filedata-0.2.2/tests/test_text_algo/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      841 2023-06-21 01:06:46.000000 filedata-0.2.2/tests/test_text_algo/test_ac.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 03:25:51.970338 filedata-0.2.3/
+-rwxrwxrwx   0 root         (0) root         (0)      107 2023-06-21 00:08:49.000000 filedata-0.2.3/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)      490 2023-06-21 03:25:51.970338 filedata-0.2.3/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)       57 2023-06-21 00:08:49.000000 filedata-0.2.3/README.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 03:25:51.439215 filedata-0.2.3/filedata/
+-rwxrwxrwx   0 root         (0) root         (0)       22 2023-06-21 03:10:15.000000 filedata-0.2.3/filedata/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      841 2023-06-21 00:08:49.000000 filedata-0.2.3/filedata/config.py
+-rwxrwxrwx   0 root         (0) root         (0)     3399 2023-06-21 00:08:49.000000 filedata-0.2.3/filedata/file.py
+-rwxrwxrwx   0 root         (0) root         (0)     2895 2023-06-21 00:08:49.000000 filedata-0.2.3/filedata/html.py
+-rwxrwxrwx   0 root         (0) root         (0)     6466 2023-06-21 00:08:49.000000 filedata-0.2.3/filedata/image.py
+-rwxrwxrwx   0 root         (0) root         (0)      801 2023-06-21 00:08:49.000000 filedata-0.2.3/filedata/pdf.py
+-rwxrwxrwx   0 root         (0) root         (0)     1198 2023-06-21 00:08:49.000000 filedata-0.2.3/filedata/retry.py
+-rwxrwxrwx   0 root         (0) root         (0)      624 2023-06-21 01:07:06.000000 filedata-0.2.3/filedata/text.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 03:25:51.783080 filedata-0.2.3/filedata/text_algo/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 00:11:15.000000 filedata-0.2.3/filedata/text_algo/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4274 2023-06-21 03:21:30.000000 filedata-0.2.3/filedata/text_algo/ac.py
+-rwxrwxrwx   0 root         (0) root         (0)       94 2023-06-21 00:08:49.000000 filedata-0.2.3/filedata/time.py
+-rwxrwxrwx   0 root         (0) root         (0)      466 2023-06-21 00:08:49.000000 filedata-0.2.3/filedata/utils.py
+-rwxrwxrwx   0 root         (0) root         (0)      252 2023-06-21 00:08:49.000000 filedata-0.2.3/filedata/video.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 03:25:51.704922 filedata-0.2.3/filedata.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      490 2023-06-21 03:25:50.000000 filedata-0.2.3/filedata.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      578 2023-06-21 03:25:51.000000 filedata-0.2.3/filedata.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-21 03:25:50.000000 filedata-0.2.3/filedata.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-21 01:08:29.000000 filedata-0.2.3/filedata.egg-info/not-zip-safe
+-rwxrwxrwx   0 root         (0) root         (0)      124 2023-06-21 03:25:50.000000 filedata-0.2.3/filedata.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       15 2023-06-21 03:25:50.000000 filedata-0.2.3/filedata.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 03:25:51.814346 filedata-0.2.3/requirements/
+-rwxrwxrwx   0 root         (0) root         (0)       18 2023-06-21 00:08:49.000000 filedata-0.2.3/requirements/test.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-06-21 03:25:51.970338 filedata-0.2.3/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1549 2023-06-21 00:08:49.000000 filedata-0.2.3/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 03:25:51.845596 filedata-0.2.3/tests/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 00:08:49.000000 filedata-0.2.3/tests/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 03:25:51.939338 filedata-0.2.3/tests/test_text_algo/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 00:58:58.000000 filedata-0.2.3/tests/test_text_algo/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1292 2023-06-21 03:06:06.000000 filedata-0.2.3/tests/test_text_algo/test_ac.py
```

### Comparing `filedata-0.2.2/filedata/config.py` & `filedata-0.2.3/filedata/config.py`

 * *Files identical despite different names*

### Comparing `filedata-0.2.2/filedata/file.py` & `filedata-0.2.3/filedata/file.py`

 * *Files identical despite different names*

### Comparing `filedata-0.2.2/filedata/html.py` & `filedata-0.2.3/filedata/html.py`

 * *Files identical despite different names*

### Comparing `filedata-0.2.2/filedata/image.py` & `filedata-0.2.3/filedata/image.py`

 * *Files identical despite different names*

### Comparing `filedata-0.2.2/filedata/pdf.py` & `filedata-0.2.3/filedata/pdf.py`

 * *Files identical despite different names*

### Comparing `filedata-0.2.2/filedata/retry.py` & `filedata-0.2.3/filedata/retry.py`

 * *Files identical despite different names*

### Comparing `filedata-0.2.2/filedata/text.py` & `filedata-0.2.3/filedata/text.py`

 * *Files identical despite different names*

### Comparing `filedata-0.2.2/filedata.egg-info/SOURCES.txt` & `filedata-0.2.3/filedata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `filedata-0.2.2/setup.py` & `filedata-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `filedata-0.2.2/tests/test_text_algo/test_ac.py` & `filedata-0.2.3/tests/test_text_algo/test_ac.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,7 +21,20 @@
     ac = ACAutomaton(words)
     result = ac.find_all(content)
 
     assert len(result) == 7
     for r in result:
         assert r.word in words
         assert content[r.position[0]:r.position[1]] == r.word
+
+
+def test_find_all_from_segments():
+    words = ['软件测试', '软件测试方案', '软件']
+    segments = ['这是', '一个', '软件测试', '方案', '，', '可以', '用来', '做', '应用软件', '测试']
+
+    ac = ACAutomaton(words)
+    result = ac.find_all_from_segments(segments)
+
+    assert len(result) == 2
+    for r in result:
+        assert r.word in words
+        assert ''.join(segments[r.position[0]:r.position[1]]) == r.word
```

