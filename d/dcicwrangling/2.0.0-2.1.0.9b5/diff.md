# Comparing `tmp/dcicwrangling-2.0.0.tar.gz` & `tmp/dcicwrangling-2.1.0.9b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicwrangling-2.0.0.tar", max compression
+gzip compressed data, was "dcicwrangling-2.1.0.9b5.tar", max compression
```

## Comparing `dcicwrangling-2.0.0.tar` & `dcicwrangling-2.1.0.9b5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     2044 2023-02-03 19:58:01.952773 dcicwrangling-2.0.0/README.md
--rw-r--r--   0        0        0      803 2023-02-03 19:58:01.960774 dcicwrangling-2.0.0/pyproject.toml
--rw-r--r--   0        0        0    31604 2023-02-03 19:58:01.960774 dcicwrangling-2.0.0/scripts/GAM_fastq_accession2filename.txt.gz
--rw-r--r--   0        0        0        0 2023-02-03 19:58:01.960774 dcicwrangling-2.0.0/scripts/__init__.py
--rw-r--r--   0        0        0      127 2023-02-03 19:58:01.960774 dcicwrangling-2.0.0/scripts/_version.py
--rw-r--r--   0        0        0     1621 2023-02-03 19:58:01.960774 dcicwrangling-2.0.0/scripts/cp_files2diffbucket.py
--rw-r--r--   0        0        0     1344 2023-02-03 19:58:01.960774 dcicwrangling-2.0.0/scripts/empty_patch_items.py
--rw-r--r--   0        0        0     6547 2023-02-03 19:58:01.960774 dcicwrangling-2.0.0/scripts/generate_wfr_from_pf.py
--rw-r--r--   0        0        0    25996 2023-02-03 19:58:01.960774 dcicwrangling-2.0.0/scripts/geo2fdn.py
--rw-r--r--   0        0        0      849 2023-02-03 19:58:01.960774 dcicwrangling-2.0.0/scripts/get_item_ids_from_search.py
--rw-r--r--   0        0        0     3481 2023-02-03 19:58:01.960774 dcicwrangling-2.0.0/scripts/get_linked_item_ids.py
--rw-r--r--   0        0        0     3013 2023-02-03 19:58:01.960774 dcicwrangling-2.0.0/scripts/item_fetcher.py
--rw-r--r--   0        0        0     8362 2023-02-03 19:58:01.960774 dcicwrangling-2.0.0/scripts/item_loader.py
--rw-r--r--   0        0        0     8454 2023-02-03 19:58:01.960774 dcicwrangling-2.0.0/scripts/load_items_json.py
--rw-r--r--   0        0        0     3684 2023-02-03 19:58:01.960774 dcicwrangling-2.0.0/scripts/ontology_term_loader.py
--rw-r--r--   0        0        0     7386 2023-02-03 19:58:01.960774 dcicwrangling-2.0.0/scripts/parse_damid_pf.py
--rw-r--r--   0        0        0     2334 2023-02-03 19:58:01.960774 dcicwrangling-2.0.0/scripts/patch_field_for_many_items.py
--rw-r--r--   0        0        0     2132 2023-02-03 19:58:01.960774 dcicwrangling-2.0.0/scripts/pfs2opfs.py
--rw-r--r--   0        0        0     1835 2023-02-03 19:58:01.960774 dcicwrangling-2.0.0/scripts/quick_patcher.py
--rw-r--r--   0        0        0     5789 2023-02-03 19:58:01.960774 dcicwrangling-2.0.0/scripts/rxiv2ja.py
--rw-r--r--   0        0        0     5285 2023-02-03 19:58:01.960774 dcicwrangling-2.0.0/scripts/tag_release_freeze.py
--rw-r--r--   0        0        0     3086 2023-02-03 19:58:01.960774 dcicwrangling-2.0.0/scripts/tagger.py
--rw-r--r--   0        0        0     3030 1970-01-01 00:00:00.000000 dcicwrangling-2.0.0/setup.py
--rw-r--r--   0        0        0     2765 1970-01-01 00:00:00.000000 dcicwrangling-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2044 2023-06-21 15:54:37.538415 dcicwrangling-2.1.0.9b5/README.md
+-rw-r--r--   0        0        0      807 2023-06-21 15:54:37.542415 dcicwrangling-2.1.0.9b5/pyproject.toml
+-rw-r--r--   0        0        0    31604 2023-06-21 15:54:37.542415 dcicwrangling-2.1.0.9b5/scripts/GAM_fastq_accession2filename.txt.gz
+-rw-r--r--   0        0        0        0 2023-06-21 15:54:37.542415 dcicwrangling-2.1.0.9b5/scripts/__init__.py
+-rw-r--r--   0        0        0      127 2023-06-21 15:54:37.542415 dcicwrangling-2.1.0.9b5/scripts/_version.py
+-rw-r--r--   0        0        0     1621 2023-06-21 15:54:37.542415 dcicwrangling-2.1.0.9b5/scripts/cp_files2diffbucket.py
+-rw-r--r--   0        0        0     1344 2023-06-21 15:54:37.542415 dcicwrangling-2.1.0.9b5/scripts/empty_patch_items.py
+-rw-r--r--   0        0        0     6547 2023-06-21 15:54:37.542415 dcicwrangling-2.1.0.9b5/scripts/generate_wfr_from_pf.py
+-rw-r--r--   0        0        0    25996 2023-06-21 15:54:37.542415 dcicwrangling-2.1.0.9b5/scripts/geo2fdn.py
+-rw-r--r--   0        0        0      849 2023-06-21 15:54:37.542415 dcicwrangling-2.1.0.9b5/scripts/get_item_ids_from_search.py
+-rw-r--r--   0        0        0     3481 2023-06-21 15:54:37.542415 dcicwrangling-2.1.0.9b5/scripts/get_linked_item_ids.py
+-rw-r--r--   0        0        0     3013 2023-06-21 15:54:37.542415 dcicwrangling-2.1.0.9b5/scripts/item_fetcher.py
+-rw-r--r--   0        0        0     8362 2023-06-21 15:54:37.542415 dcicwrangling-2.1.0.9b5/scripts/item_loader.py
+-rw-r--r--   0        0        0     8454 2023-06-21 15:54:37.542415 dcicwrangling-2.1.0.9b5/scripts/load_items_json.py
+-rw-r--r--   0        0        0     3684 2023-06-21 15:54:37.542415 dcicwrangling-2.1.0.9b5/scripts/ontology_term_loader.py
+-rw-r--r--   0        0        0     7386 2023-06-21 15:54:37.542415 dcicwrangling-2.1.0.9b5/scripts/parse_damid_pf.py
+-rw-r--r--   0        0        0     2334 2023-06-21 15:54:37.542415 dcicwrangling-2.1.0.9b5/scripts/patch_field_for_many_items.py
+-rw-r--r--   0        0        0     2132 2023-06-21 15:54:37.542415 dcicwrangling-2.1.0.9b5/scripts/pfs2opfs.py
+-rw-r--r--   0        0        0     1835 2023-06-21 15:54:37.542415 dcicwrangling-2.1.0.9b5/scripts/quick_patcher.py
+-rw-r--r--   0        0        0     5789 2023-06-21 15:54:37.542415 dcicwrangling-2.1.0.9b5/scripts/rxiv2ja.py
+-rw-r--r--   0        0        0     5285 2023-06-21 15:54:37.542415 dcicwrangling-2.1.0.9b5/scripts/tag_release_freeze.py
+-rw-r--r--   0        0        0     3086 2023-06-21 15:54:37.542415 dcicwrangling-2.1.0.9b5/scripts/tagger.py
+-rw-r--r--   0        0        0     3034 1970-01-01 00:00:00.000000 dcicwrangling-2.1.0.9b5/setup.py
+-rw-r--r--   0        0        0     2769 1970-01-01 00:00:00.000000 dcicwrangling-2.1.0.9b5/PKG-INFO
```

### Comparing `dcicwrangling-2.0.0/README.md` & `dcicwrangling-2.1.0.9b5/README.md`

 * *Files identical despite different names*

### Comparing `dcicwrangling-2.0.0/pyproject.toml` & `dcicwrangling-2.1.0.9b5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "dcicwrangling"
-version = "2.0.0"
+version = "2.1.0.9b5"
 description = "Scripts and Jupyter notebooks for 4DN wrangling"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/4dn-dcic/dcicwrangling"
 repository = "https://github.com/4dn-dcic/dcicwrangling"
 packages = [{ include="scripts", from="." }]
 
 [tool.poetry.dependencies]
 python = ">=3.7.1, <3.9"
-dcicutils = "^6.8.0"
+dcicutils = "^7.4.0"
 openpyxl = "^3.0.9"
 Biopython = "1.76"
 GEOparse = "^2.0.1"
 jupyterlab = "3.2.8"
 
 [tool.poetry.dev-dependencies]
 pytest = ">=4.5.0"
```

### Comparing `dcicwrangling-2.0.0/scripts/GAM_fastq_accession2filename.txt.gz` & `dcicwrangling-2.1.0.9b5/scripts/GAM_fastq_accession2filename.txt.gz`

 * *Files identical despite different names*

### Comparing `dcicwrangling-2.0.0/scripts/cp_files2diffbucket.py` & `dcicwrangling-2.1.0.9b5/scripts/cp_files2diffbucket.py`

 * *Files identical despite different names*

### Comparing `dcicwrangling-2.0.0/scripts/empty_patch_items.py` & `dcicwrangling-2.1.0.9b5/scripts/empty_patch_items.py`

 * *Files identical despite different names*

### Comparing `dcicwrangling-2.0.0/scripts/generate_wfr_from_pf.py` & `dcicwrangling-2.1.0.9b5/scripts/generate_wfr_from_pf.py`

 * *Files identical despite different names*

### Comparing `dcicwrangling-2.0.0/scripts/geo2fdn.py` & `dcicwrangling-2.1.0.9b5/scripts/geo2fdn.py`

 * *Files identical despite different names*

### Comparing `dcicwrangling-2.0.0/scripts/get_item_ids_from_search.py` & `dcicwrangling-2.1.0.9b5/scripts/get_item_ids_from_search.py`

 * *Files identical despite different names*

### Comparing `dcicwrangling-2.0.0/scripts/get_linked_item_ids.py` & `dcicwrangling-2.1.0.9b5/scripts/get_linked_item_ids.py`

 * *Files identical despite different names*

### Comparing `dcicwrangling-2.0.0/scripts/item_fetcher.py` & `dcicwrangling-2.1.0.9b5/scripts/item_fetcher.py`

 * *Files identical despite different names*

### Comparing `dcicwrangling-2.0.0/scripts/item_loader.py` & `dcicwrangling-2.1.0.9b5/scripts/item_loader.py`

 * *Files identical despite different names*

### Comparing `dcicwrangling-2.0.0/scripts/load_items_json.py` & `dcicwrangling-2.1.0.9b5/scripts/load_items_json.py`

 * *Files identical despite different names*

### Comparing `dcicwrangling-2.0.0/scripts/ontology_term_loader.py` & `dcicwrangling-2.1.0.9b5/scripts/ontology_term_loader.py`

 * *Files identical despite different names*

### Comparing `dcicwrangling-2.0.0/scripts/parse_damid_pf.py` & `dcicwrangling-2.1.0.9b5/scripts/parse_damid_pf.py`

 * *Files identical despite different names*

### Comparing `dcicwrangling-2.0.0/scripts/patch_field_for_many_items.py` & `dcicwrangling-2.1.0.9b5/scripts/patch_field_for_many_items.py`

 * *Files identical despite different names*

### Comparing `dcicwrangling-2.0.0/scripts/pfs2opfs.py` & `dcicwrangling-2.1.0.9b5/scripts/pfs2opfs.py`

 * *Files identical despite different names*

### Comparing `dcicwrangling-2.0.0/scripts/quick_patcher.py` & `dcicwrangling-2.1.0.9b5/scripts/quick_patcher.py`

 * *Files identical despite different names*

### Comparing `dcicwrangling-2.0.0/scripts/rxiv2ja.py` & `dcicwrangling-2.1.0.9b5/scripts/rxiv2ja.py`

 * *Files identical despite different names*

### Comparing `dcicwrangling-2.0.0/scripts/tag_release_freeze.py` & `dcicwrangling-2.1.0.9b5/scripts/tag_release_freeze.py`

 * *Files identical despite different names*

### Comparing `dcicwrangling-2.0.0/scripts/tagger.py` & `dcicwrangling-2.1.0.9b5/scripts/tagger.py`

 * *Files identical despite different names*

### Comparing `dcicwrangling-2.0.0/setup.py` & `dcicwrangling-2.1.0.9b5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['Biopython==1.76',
  'GEOparse>=2.0.1,<3.0.0',
- 'dcicutils>=6.8.0,<7.0.0',
+ 'dcicutils>=7.4.0,<8.0.0',
  'jupyterlab==3.2.8',
  'openpyxl>=3.0.9,<4.0.0']
 
 entry_points = \
 {'console_scripts': ['fetch-items = scripts.item_fetcher:main']}
 
 setup_kwargs = {
     'name': 'dcicwrangling',
-    'version': '2.0.0',
+    'version': '2.1.0.9b5',
     'description': 'Scripts and Jupyter notebooks for 4DN wrangling',
     'long_description': "# DCIC-wrangling\n\nThis is a collection of scripts and Jupyter notebooks that can be helpful when performing many data wrangling tasks.  Most of the tools are specific to 4DN Nucleome wrangling needs, however may be modified to be more generally useful for certain tasks.\n\n## Install\n\nPackaged with `poetry` can be installed using `make`, `poetry` or `pip`.\n\nFrom the dcicwrangling directory - `make build`\n\nIf you already have poetry installed - `poetry install`\n\nOr to pip install from PyPi - `pip install dcicwrangling`\n\nAll dependencies are installed by default - if for some reason you don't want to install `pytest` packages or `invoke` (used to launch notebooks) you can do `poetry install --no-dev` - not recommended.\n\n## Usage\n\n### Jupyter notebooks\nThere are a collection of commonly used jupyter notebooks in the `notebooks/useful_notebooks` directory.  You can start a jupyter notebook server locally using `invoke notebook` from the top level directory.  This should launch the server and open a browser page where the notebooks can be accessed.\n\n**IMPORTANT!** - You should create your own folder in the `notebooks` directory named `Yourname_scripts`.  This folder is where you should create, access and run your notebooks.  If you want to start with one of the notebooks in the useful_notebooks directory please create a copy and move it to your own folder.  This keeps the repository clean and organized.  Please **DO NOT** run notebooks in the useful_notebooks directory and commit the results to the repository.\n\n### Scripts\n\nThe scripts directory contains some useful command line scripts.  They can be run from the top level directory using `python scripts/script_name --options`.  Using `--help` shows available options.  In general, modified versions and bespoke scripts should not be committed to the repository - or alternatively committed to a separate non-master branch.\n\nAs scripts are developed and refined `tool.poetry.scripts` directives can be added to facilitate script usage - see `pyproject.toml` file example.\n",
     'author': '4DN-DCIC Team',
     'author_email': 'support@4dnucleome.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/4dn-dcic/dcicwrangling',
```

### Comparing `dcicwrangling-2.0.0/PKG-INFO` & `dcicwrangling-2.1.0.9b5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: dcicwrangling
-Version: 2.0.0
+Version: 2.1.0.9b5
 Summary: Scripts and Jupyter notebooks for 4DN wrangling
 Home-page: https://github.com/4dn-dcic/dcicwrangling
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7.1,<3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Dist: Biopython (==1.76)
 Requires-Dist: GEOparse (>=2.0.1,<3.0.0)
-Requires-Dist: dcicutils (>=6.8.0,<7.0.0)
+Requires-Dist: dcicutils (>=7.4.0,<8.0.0)
 Requires-Dist: jupyterlab (==3.2.8)
 Requires-Dist: openpyxl (>=3.0.9,<4.0.0)
 Project-URL: Repository, https://github.com/4dn-dcic/dcicwrangling
 Description-Content-Type: text/markdown
 
 # DCIC-wrangling
```

