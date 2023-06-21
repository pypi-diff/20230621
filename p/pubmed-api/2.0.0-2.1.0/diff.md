# Comparing `tmp/pubmed_api-2.0.0.tar.gz` & `tmp/pubmed_api-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pubmed_api-2.0.0.tar", last modified: Sun Apr  2 06:30:26 2023, max compression
+gzip compressed data, was "pubmed_api-2.1.0.tar", last modified: Wed Jun 21 11:27:26 2023, max compression
```

## Comparing `pubmed_api-2.0.0.tar` & `pubmed_api-2.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 shivam    (1000) shivam    (1000)        0 2023-04-02 06:30:26.807339 pubmed_api-2.0.0/
--rwxrwxrwx   0 shivam    (1000) shivam    (1000)     1069 2023-04-01 05:58:28.000000 pubmed_api-2.0.0/LICENSE.md
--rwxrwxrwx   0 shivam    (1000) shivam    (1000)     4053 2023-04-02 06:30:26.806981 pubmed_api-2.0.0/PKG-INFO
--rwxrwxrwx   0 shivam    (1000) shivam    (1000)     3746 2023-04-01 05:31:37.000000 pubmed_api-2.0.0/README.md
-drwxrwxrwx   0 shivam    (1000) shivam    (1000)        0 2023-04-02 06:30:26.775919 pubmed_api-2.0.0/pubmed_api/
--rwxrwxrwx   0 shivam    (1000) shivam    (1000)        0 2023-03-28 06:54:15.000000 pubmed_api-2.0.0/pubmed_api/__init__.py
--rwxrwxrwx   0 shivam    (1000) shivam    (1000)     3524 2023-03-28 07:53:50.000000 pubmed_api-2.0.0/pubmed_api/api.py
--rwxrwxrwx   0 shivam    (1000) shivam    (1000)     1259 2023-03-28 07:53:50.000000 pubmed_api-2.0.0/pubmed_api/pubmed.py
-drwxrwxrwx   0 shivam    (1000) shivam    (1000)        0 2023-04-02 06:30:26.805956 pubmed_api-2.0.0/pubmed_api.egg-info/
--rwxrwxrwx   0 shivam    (1000) shivam    (1000)     4053 2023-04-02 06:30:26.000000 pubmed_api-2.0.0/pubmed_api.egg-info/PKG-INFO
--rwxrwxrwx   0 shivam    (1000) shivam    (1000)      290 2023-04-02 06:30:26.000000 pubmed_api-2.0.0/pubmed_api.egg-info/SOURCES.txt
--rwxrwxrwx   0 shivam    (1000) shivam    (1000)        1 2023-04-02 06:30:26.000000 pubmed_api-2.0.0/pubmed_api.egg-info/dependency_links.txt
--rwxrwxrwx   0 shivam    (1000) shivam    (1000)       19 2023-04-02 06:30:26.000000 pubmed_api-2.0.0/pubmed_api.egg-info/requires.txt
--rwxrwxrwx   0 shivam    (1000) shivam    (1000)       11 2023-04-02 06:30:26.000000 pubmed_api-2.0.0/pubmed_api.egg-info/top_level.txt
--rwxrwxrwx   0 shivam    (1000) shivam    (1000)       80 2023-04-01 05:50:02.000000 pubmed_api-2.0.0/pyproject.toml
--rwxrwxrwx   0 shivam    (1000) shivam    (1000)       38 2023-04-02 06:30:26.807429 pubmed_api-2.0.0/setup.cfg
--rwxrwxrwx   0 shivam    (1000) shivam    (1000)      573 2023-04-02 06:30:08.000000 pubmed_api-2.0.0/setup.py
-drwxrwxrwx   0 shivam    (1000) shivam    (1000)        0 2023-04-02 06:30:26.806450 pubmed_api-2.0.0/tests/
--rwxrwxrwx   0 shivam    (1000) shivam    (1000)     3364 2023-03-28 08:09:22.000000 pubmed_api-2.0.0/tests/tests.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 11:27:26.858010 pubmed_api-2.1.0/
+-rwxrwxrwx   0 root         (0) root         (0)     1069 2023-04-01 05:58:28.000000 pubmed_api-2.1.0/LICENSE.md
+-rwxrwxrwx   0 root         (0) root         (0)     4053 2023-06-21 11:27:26.857751 pubmed_api-2.1.0/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     3746 2023-04-01 05:31:37.000000 pubmed_api-2.1.0/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 11:27:26.818198 pubmed_api-2.1.0/pubmed_api/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-03-28 06:54:15.000000 pubmed_api-2.1.0/pubmed_api/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3790 2023-06-21 11:16:56.000000 pubmed_api-2.1.0/pubmed_api/api.py
+-rwxrwxrwx   0 root         (0) root         (0)     1259 2023-06-20 15:27:15.000000 pubmed_api-2.1.0/pubmed_api/pubmed.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 11:27:26.827563 pubmed_api-2.1.0/pubmed_api.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     4053 2023-06-21 11:27:26.000000 pubmed_api-2.1.0/pubmed_api.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      290 2023-06-21 11:27:26.000000 pubmed_api-2.1.0/pubmed_api.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-21 11:27:26.000000 pubmed_api-2.1.0/pubmed_api.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       19 2023-06-21 11:27:26.000000 pubmed_api-2.1.0/pubmed_api.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       11 2023-06-21 11:27:26.000000 pubmed_api-2.1.0/pubmed_api.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       80 2023-04-01 05:50:02.000000 pubmed_api-2.1.0/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-06-21 11:27:26.858152 pubmed_api-2.1.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      573 2023-06-21 11:26:06.000000 pubmed_api-2.1.0/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 11:27:26.827986 pubmed_api-2.1.0/tests/
+-rwxrwxrwx   0 root         (0) root         (0)     3364 2023-03-28 08:09:22.000000 pubmed_api-2.1.0/tests/tests.py
```

### Comparing `pubmed_api-2.0.0/LICENSE.md` & `pubmed_api-2.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pubmed_api-2.0.0/PKG-INFO` & `pubmed_api-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pubmed_api
-Version: 2.0.0
+Version: 2.1.0
 Summary: Runs PubMed search strings over pubmed API using a batch logic
 Home-page: https://github.com/shivam221098/pubmed-api-v1
 Author: Shivam Singh
 Author-email: shivam221098@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `pubmed_api-2.0.0/README.md` & `pubmed_api-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pubmed_api-2.0.0/pubmed_api/api.py` & `pubmed_api-2.1.0/pubmed_api/api.py`

 * *Files 13% similar despite different names*

```diff
@@ -39,19 +39,23 @@
         return self
 
     def __str__(self):
         return f"Count: {self.record_count}, PMID Count: {len(self.pmids)}"
 
 
 class Params:
+    __YEARS_DIFFERENCE__ = 11  # date filter will be applied for last 'n' years
+
     def __init__(
             self,
             term: str,
     ):
-        self.__term = term
+        self.__term = f"{term} AND " \
+                      f"({datetime.now().year - self.__YEARS_DIFFERENCE__}/01/01[Date - Create] : " \
+                      f"{datetime.now().year}/12/31[Date - Create])"
         self.__retstart = 0
         self.__uid_start = 1
         self.__uid_end = None
 
     @property
     def uid_start(self):
         return self.__uid_start
@@ -74,15 +78,15 @@
             return {
                 "term": self.__term,
                 "retmax": 9999,
                 "retstart": 0,
                 "sort": "pub_date"
             }
         return {
-            "term": self.__term + f" AND {self.uid_start}:{self.uid_end}[UID]",
+            "term": self.__term + f" AND ({self.uid_start}:{self.uid_end}[UID])",
             "retmax": 9999,
             "retstart": 0
         }
 
 
 class API(Session):
     __BASE_ESEARCH_URL__ = "https://eutils.ncbi.nlm.nih.gov/entrez/eutils/esearch.fcgi"
```

### Comparing `pubmed_api-2.0.0/pubmed_api/pubmed.py` & `pubmed_api-2.1.0/pubmed_api/pubmed.py`

 * *Files identical despite different names*

### Comparing `pubmed_api-2.0.0/pubmed_api.egg-info/PKG-INFO` & `pubmed_api-2.1.0/pubmed_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pubmed-api
-Version: 2.0.0
+Version: 2.1.0
 Summary: Runs PubMed search strings over pubmed API using a batch logic
 Home-page: https://github.com/shivam221098/pubmed-api-v1
 Author: Shivam Singh
 Author-email: shivam221098@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `pubmed_api-2.0.0/setup.py` & `pubmed_api-2.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r", encoding="utf-8") as file:
     long_description = file.read()
 
 
 setuptools.setup(
     name="pubmed_api",
-    version="2.0.0",
+    version="2.1.0",
     author="Shivam Singh",
     author_email="shivam221098@gmail.com",
     description="Runs PubMed search strings over pubmed API using a batch logic",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/shivam221098/pubmed-api-v1",
     packages=["pubmed_api"],
```

### Comparing `pubmed_api-2.0.0/tests/tests.py` & `pubmed_api-2.1.0/tests/tests.py`

 * *Files identical despite different names*

