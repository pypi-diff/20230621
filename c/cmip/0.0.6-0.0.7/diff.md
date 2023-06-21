# Comparing `tmp/cmip-0.0.6.tar.gz` & `tmp/cmip-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmip-0.0.6.tar", last modified: Wed Apr 19 10:30:50 2023, max compression
+gzip compressed data, was "cmip-0.0.7.tar", last modified: Wed Jun 21 06:31:09 2023, max compression
```

## Comparing `cmip-0.0.6.tar` & `cmip-0.0.7.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 10:30:50.541176 cmip-0.0.6/
--rw-rw-rw-   0        0        0     1083 2022-10-27 04:31:09.000000 cmip-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     1120 2023-04-19 10:30:50.540175 cmip-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      738 2023-04-17 02:51:43.000000 cmip-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 10:30:50.504080 cmip-0.0.6/cmip/
--rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.6/cmip/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 10:30:50.512839 cmip-0.0.6/cmip/data/
--rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.6/cmip/data/ad.txt
--rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.6/cmip/data/chinese_frequency.tsv
--rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.6/cmip/data/letter_mapping.txt
--rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.6/cmip/data/pinyin.txt
-drwxrwxrwx   0        0        0        0 2023-04-19 10:30:50.515841 cmip-0.0.6/cmip/gibberish/
--rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.6/cmip/gibberish/__init__.py
--rw-rw-rw-   0        0        0     2560 2022-10-27 04:31:09.000000 cmip-0.0.6/cmip/gibberish/gibberish.py
-drwxrwxrwx   0        0        0        0 2023-04-19 10:30:50.517845 cmip-0.0.6/cmip/image/
--rw-rw-rw-   0        0        0     1347 2022-10-27 04:31:09.000000 cmip-0.0.6/cmip/image/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 10:30:50.523840 cmip-0.0.6/cmip/text/
--rw-rw-rw-   0        0        0     2886 2023-04-19 10:30:05.000000 cmip-0.0.6/cmip/text/__init__.py
--rw-rw-rw-   0        0        0     5071 2022-12-15 09:16:49.000000 cmip-0.0.6/cmip/text/ac_automation.py
--rw-rw-rw-   0        0        0     1755 2022-10-27 04:31:09.000000 cmip-0.0.6/cmip/text/normalize.py
--rw-rw-rw-   0        0        0      555 2022-10-27 04:31:09.000000 cmip-0.0.6/cmip/text/similarity.py
--rw-rw-rw-   0        0        0     2403 2022-10-28 01:23:10.000000 cmip-0.0.6/cmip/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-19 10:30:50.532837 cmip-0.0.6/cmip/web/
--rw-rw-rw-   0        0        0      482 2022-10-27 09:02:47.000000 cmip-0.0.6/cmip/web/__init__.py
--rw-rw-rw-   0        0        0    33944 2023-03-03 05:43:41.000000 cmip-0.0.6/cmip/web/html.py
--rw-rw-rw-   0        0        0     7136 2022-10-27 04:31:09.000000 cmip-0.0.6/cmip/web/simhash_utils.py
--rw-rw-rw-   0        0        0      777 2022-10-27 04:31:09.000000 cmip-0.0.6/cmip/web/utils.py
--rw-rw-rw-   0        0        0     3445 2023-04-17 02:42:39.000000 cmip-0.0.6/cmip/web/web_scraping.py
-drwxrwxrwx   0        0        0        0 2023-04-19 10:30:50.537175 cmip-0.0.6/cmip/word_discover/
--rw-rw-rw-   0        0        0      163 2022-10-27 04:31:09.000000 cmip-0.0.6/cmip/word_discover/__init__.py
--rw-rw-rw-   0        0        0     1864 2022-10-27 04:31:09.000000 cmip-0.0.6/cmip/word_discover/ngram.py
--rw-rw-rw-   0        0        0     7008 2022-10-27 04:31:09.000000 cmip-0.0.6/cmip/word_discover/word_discover.py
-drwxrwxrwx   0        0        0        0 2023-04-19 10:30:50.509837 cmip-0.0.6/cmip.egg-info/
--rw-rw-rw-   0        0        0     1120 2023-04-19 10:30:50.000000 cmip-0.0.6/cmip.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      715 2023-04-19 10:30:50.000000 cmip-0.0.6/cmip.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 10:30:50.000000 cmip-0.0.6/cmip.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-04-19 10:30:50.000000 cmip-0.0.6/cmip.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-19 10:30:50.000000 cmip-0.0.6/cmip.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 10:30:50.541176 cmip-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      742 2023-04-19 10:29:33.000000 cmip-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-19 10:30:50.539174 cmip-0.0.6/test/
--rw-rw-rw-   0        0        0        0 2022-12-09 06:53:07.000000 cmip-0.0.6/test/__init__.py
--rw-rw-rw-   0        0        0     1415 2022-12-15 09:05:59.000000 cmip-0.0.6/test/test_ac_automation.py
+drwxrwxrwx   0        0        0        0 2023-06-21 06:31:09.558127 cmip-0.0.7/
+-rw-rw-rw-   0        0        0     1083 2022-10-27 04:31:09.000000 cmip-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     1120 2023-06-21 06:31:09.556116 cmip-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      738 2023-04-17 02:51:43.000000 cmip-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-21 06:31:09.487398 cmip-0.0.7/cmip/
+-rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.7/cmip/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 06:31:09.511391 cmip-0.0.7/cmip/data/
+-rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.7/cmip/data/ad.txt
+-rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.7/cmip/data/chinese_frequency.tsv
+-rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.7/cmip/data/letter_mapping.txt
+-rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.7/cmip/data/pinyin.txt
+drwxrwxrwx   0        0        0        0 2023-06-21 06:31:09.516385 cmip-0.0.7/cmip/gibberish/
+-rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.7/cmip/gibberish/__init__.py
+-rw-rw-rw-   0        0        0     2560 2022-10-27 04:31:09.000000 cmip-0.0.7/cmip/gibberish/gibberish.py
+drwxrwxrwx   0        0        0        0 2023-06-21 06:31:09.518389 cmip-0.0.7/cmip/image/
+-rw-rw-rw-   0        0        0     1347 2022-10-27 04:31:09.000000 cmip-0.0.7/cmip/image/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 06:31:09.531387 cmip-0.0.7/cmip/text/
+-rw-rw-rw-   0        0        0     2886 2023-04-19 10:30:05.000000 cmip-0.0.7/cmip/text/__init__.py
+-rw-rw-rw-   0        0        0     5071 2022-12-15 09:16:49.000000 cmip-0.0.7/cmip/text/ac_automation.py
+-rw-rw-rw-   0        0        0     1755 2022-10-27 04:31:09.000000 cmip-0.0.7/cmip/text/normalize.py
+-rw-rw-rw-   0        0        0      555 2022-10-27 04:31:09.000000 cmip-0.0.7/cmip/text/similarity.py
+-rw-rw-rw-   0        0        0     2403 2022-10-28 01:23:10.000000 cmip-0.0.7/cmip/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-21 06:31:09.544627 cmip-0.0.7/cmip/web/
+-rw-rw-rw-   0        0        0      482 2022-10-27 09:02:47.000000 cmip-0.0.7/cmip/web/__init__.py
+-rw-rw-rw-   0        0        0    33944 2023-03-03 05:43:41.000000 cmip-0.0.7/cmip/web/html.py
+-rw-rw-rw-   0        0        0     7136 2022-10-27 04:31:09.000000 cmip-0.0.7/cmip/web/simhash_utils.py
+-rw-rw-rw-   0        0        0      837 2023-06-21 06:26:43.000000 cmip-0.0.7/cmip/web/utils.py
+-rw-rw-rw-   0        0        0     3864 2023-06-21 06:27:40.000000 cmip-0.0.7/cmip/web/web_scraping.py
+drwxrwxrwx   0        0        0        0 2023-06-21 06:31:09.549522 cmip-0.0.7/cmip/word_discover/
+-rw-rw-rw-   0        0        0      163 2022-10-27 04:31:09.000000 cmip-0.0.7/cmip/word_discover/__init__.py
+-rw-rw-rw-   0        0        0     1864 2022-10-27 04:31:09.000000 cmip-0.0.7/cmip/word_discover/ngram.py
+-rw-rw-rw-   0        0        0     7008 2022-10-27 04:31:09.000000 cmip-0.0.7/cmip/word_discover/word_discover.py
+drwxrwxrwx   0        0        0        0 2023-06-21 06:31:09.500386 cmip-0.0.7/cmip.egg-info/
+-rw-rw-rw-   0        0        0     1120 2023-06-21 06:31:09.000000 cmip-0.0.7/cmip.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      715 2023-06-21 06:31:09.000000 cmip-0.0.7/cmip.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 06:31:09.000000 cmip-0.0.7/cmip.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-06-21 06:31:09.000000 cmip-0.0.7/cmip.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-21 06:31:09.000000 cmip-0.0.7/cmip.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 06:31:09.559108 cmip-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      742 2023-06-21 06:29:49.000000 cmip-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 06:31:09.553108 cmip-0.0.7/test/
+-rw-rw-rw-   0        0        0        0 2022-12-09 06:53:07.000000 cmip-0.0.7/test/__init__.py
+-rw-rw-rw-   0        0        0     1415 2022-12-15 09:05:59.000000 cmip-0.0.7/test/test_ac_automation.py
```

### Comparing `cmip-0.0.6/LICENSE` & `cmip-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cmip-0.0.6/PKG-INFO` & `cmip-0.0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmip
-Version: 0.0.6
+Version: 0.0.7
 Summary: An efficient information processing program.
 Home-page: https://github.com/mikuh/cmip
 Author: geb
 Author-email: 853934146@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `cmip-0.0.6/README.md` & `cmip-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `cmip-0.0.6/cmip/gibberish/gibberish.py` & `cmip-0.0.7/cmip/gibberish/gibberish.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.6/cmip/image/__init__.py` & `cmip-0.0.7/cmip/image/__init__.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.6/cmip/text/__init__.py` & `cmip-0.0.7/cmip/text/__init__.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.6/cmip/text/ac_automation.py` & `cmip-0.0.7/cmip/text/ac_automation.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.6/cmip/text/normalize.py` & `cmip-0.0.7/cmip/text/normalize.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.6/cmip/text/similarity.py` & `cmip-0.0.7/cmip/text/similarity.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.6/cmip/utils.py` & `cmip-0.0.7/cmip/utils.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.6/cmip/web/html.py` & `cmip-0.0.7/cmip/web/html.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.6/cmip/web/simhash_utils.py` & `cmip-0.0.7/cmip/web/simhash_utils.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.6/cmip/web/utils.py` & `cmip-0.0.7/cmip/web/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 
 def is_valid_url(url: str) -> str:
     return validators.url(url)
 
 
 def url2domain(url: str) -> str:
     if validators.url(url):
-        return urlparse(url).netloc.lower().strip('.')
+        return urlparse(url).hostname.lower().strip('.')
+        # return urlparse(url).netloc.lower().strip('.')
 
 
 def top_domain(domain: str) -> str:
     parts = domain.lower().split(".")
     if len(parts) > 1:
         if parts[-2] in {'com', 'edu', 'net', 'org', 'co'}:
             return '.'.join(parts[-3:])
```

### Comparing `cmip-0.0.6/cmip/web/web_scraping.py` & `cmip-0.0.7/cmip/web/web_scraping.py`

 * *Files 24% similar despite different names*

```diff
@@ -74,13 +74,22 @@
             print(f"Error in main: {e}")
         finally:
             await semaphore.acquire()
             await browser.close()
 
 
 if __name__ == "__main__":
-    urls = [
-        "https://baidu.com",
-        "https://qq.com",
-        # ...更多的URL
-    ]
-    asyncio.run(web_scraping(urls))
+    # urls = [
+    #     "https://baidu.com:443",
+    #     "https://qq.com",
+    #     # ...更多的URL
+    # ]
+    # asyncio.run(web_scraping(urls))
+    # import validators
+    from urllib.parse import urlparse
+    # if validators.url("http://dlsbbjb--com--02396907a64d3.wsipv6.com"):
+    #     print("miao")
+    # print(urlparse("http://dlsbbjb--com--02396907a64d3.wsipv6.com").netloc.lower().strip('.'))
+    # print(url2domain("http://dlsbbjb--com--02396907a64d3.wsipv6.com"))
+
+
+    print(url2domain("https://www.baidu.com:8000/asdasdasd"))
```

### Comparing `cmip-0.0.6/cmip/word_discover/ngram.py` & `cmip-0.0.7/cmip/word_discover/ngram.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.6/cmip/word_discover/word_discover.py` & `cmip-0.0.7/cmip/word_discover/word_discover.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.6/cmip.egg-info/PKG-INFO` & `cmip-0.0.7/cmip.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmip
-Version: 0.0.6
+Version: 0.0.7
 Summary: An efficient information processing program.
 Home-page: https://github.com/mikuh/cmip
 Author: geb
 Author-email: 853934146@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `cmip-0.0.6/cmip.egg-info/SOURCES.txt` & `cmip-0.0.7/cmip.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cmip-0.0.6/setup.py` & `cmip-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="cmip",
-    version="0.0.6",
+    version="0.0.7",
     author="geb",
     author_email="853934146@qq.com",
     description="An efficient information processing program.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mikuh/cmip",
     packages=setuptools.find_packages(),
```

### Comparing `cmip-0.0.6/test/test_ac_automation.py` & `cmip-0.0.7/test/test_ac_automation.py`

 * *Files identical despite different names*

