# Comparing `tmp/EntityNormalizer-0.1.0.post2.tar.gz` & `tmp/EntityNormalizer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EntityNormalizer-0.1.0.post2.tar", last modified: Mon Jun 19 04:52:07 2023, max compression
+gzip compressed data, was "EntityNormalizer-0.2.0.tar", last modified: Wed Jun 21 02:34:36 2023, max compression
```

## Comparing `EntityNormalizer-0.1.0.post2.tar` & `EntityNormalizer-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,19 @@
-drwxr-xr-x   0 gabriel-he   (501) staff       (20)        0 2023-06-19 04:52:07.237644 EntityNormalizer-0.1.0.post2/
-drwxr-xr-x   0 gabriel-he   (501) staff       (20)        0 2023-06-19 04:52:07.237017 EntityNormalizer-0.1.0.post2/EntityNormalizer/
--rw-r--r--   0 gabriel-he   (501) staff       (20)     2388 2023-06-14 01:47:35.000000 EntityNormalizer-0.1.0.post2/EntityNormalizer/__init__.py
-drwxr-xr-x   0 gabriel-he   (501) staff       (20)        0 2023-06-19 04:52:07.237541 EntityNormalizer-0.1.0.post2/EntityNormalizer.egg-info/
--rw-r--r--   0 gabriel-he   (501) staff       (20)     2682 2023-06-19 04:52:07.000000 EntityNormalizer-0.1.0.post2/EntityNormalizer.egg-info/PKG-INFO
--rw-r--r--   0 gabriel-he   (501) staff       (20)      268 2023-06-19 04:52:07.000000 EntityNormalizer-0.1.0.post2/EntityNormalizer.egg-info/SOURCES.txt
--rw-r--r--   0 gabriel-he   (501) staff       (20)        1 2023-06-19 04:52:07.000000 EntityNormalizer-0.1.0.post2/EntityNormalizer.egg-info/dependency_links.txt
--rw-r--r--   0 gabriel-he   (501) staff       (20)       26 2023-06-19 04:52:07.000000 EntityNormalizer-0.1.0.post2/EntityNormalizer.egg-info/requires.txt
--rw-r--r--   0 gabriel-he   (501) staff       (20)       17 2023-06-19 04:52:07.000000 EntityNormalizer-0.1.0.post2/EntityNormalizer.egg-info/top_level.txt
--rw-r--r--   0 gabriel-he   (501) staff       (20)     1061 2023-06-19 04:28:05.000000 EntityNormalizer-0.1.0.post2/LICENSE.txt
--rw-r--r--   0 gabriel-he   (501) staff       (20)     2682 2023-06-19 04:52:07.237712 EntityNormalizer-0.1.0.post2/PKG-INFO
--rw-r--r--   0 gabriel-he   (501) staff       (20)     2285 2023-06-19 04:40:59.000000 EntityNormalizer-0.1.0.post2/README.md
--rw-r--r--   0 gabriel-he   (501) staff       (20)      160 2023-06-19 04:52:07.237890 EntityNormalizer-0.1.0.post2/setup.cfg
--rw-r--r--   0 gabriel-he   (501) staff       (20)      545 2023-06-19 04:52:02.000000 EntityNormalizer-0.1.0.post2/setup.py
+drwxr-xr-x   0 gabriel-he   (501) staff       (20)        0 2023-06-21 02:34:36.155138 EntityNormalizer-0.2.0/
+drwxr-xr-x   0 gabriel-he   (501) staff       (20)        0 2023-06-21 02:34:36.153879 EntityNormalizer-0.2.0/EntityNormalizer/
+-rw-r--r--   0 gabriel-he   (501) staff       (20)      840 2023-06-21 02:34:07.000000 EntityNormalizer-0.2.0/EntityNormalizer/Dictionaries.py
+-rw-r--r--   0 gabriel-he   (501) staff       (20)     2388 2023-06-14 01:47:35.000000 EntityNormalizer-0.2.0/EntityNormalizer/__init__.py
+drwxr-xr-x   0 gabriel-he   (501) staff       (20)        0 2023-06-21 02:34:36.154964 EntityNormalizer-0.2.0/EntityNormalizer/resources/
+-rw-r--r--   0 gabriel-he   (501) staff       (20)   200050 2023-06-21 02:34:07.000000 EntityNormalizer-0.2.0/EntityNormalizer/resources/MedDic-CANCER-ADE-JA_202306.csv
+-rw-r--r--   0 gabriel-he   (501) staff       (20)    52151 2023-06-21 02:34:07.000000 EntityNormalizer-0.2.0/EntityNormalizer/resources/MedDic-CANCER-DRUG-JA_202306.csv
+drwxr-xr-x   0 gabriel-he   (501) staff       (20)        0 2023-06-21 02:34:36.154563 EntityNormalizer-0.2.0/EntityNormalizer.egg-info/
+-rw-r--r--   0 gabriel-he   (501) staff       (20)     4031 2023-06-21 02:34:36.000000 EntityNormalizer-0.2.0/EntityNormalizer.egg-info/PKG-INFO
+-rw-r--r--   0 gabriel-he   (501) staff       (20)      432 2023-06-21 02:34:36.000000 EntityNormalizer-0.2.0/EntityNormalizer.egg-info/SOURCES.txt
+-rw-r--r--   0 gabriel-he   (501) staff       (20)        1 2023-06-21 02:34:36.000000 EntityNormalizer-0.2.0/EntityNormalizer.egg-info/dependency_links.txt
+-rw-r--r--   0 gabriel-he   (501) staff       (20)       26 2023-06-21 02:34:36.000000 EntityNormalizer-0.2.0/EntityNormalizer.egg-info/requires.txt
+-rw-r--r--   0 gabriel-he   (501) staff       (20)       17 2023-06-21 02:34:36.000000 EntityNormalizer-0.2.0/EntityNormalizer.egg-info/top_level.txt
+-rw-r--r--   0 gabriel-he   (501) staff       (20)     1061 2023-06-19 04:28:05.000000 EntityNormalizer-0.2.0/LICENSE.txt
+-rw-r--r--   0 gabriel-he   (501) staff       (20)       36 2023-06-21 02:34:07.000000 EntityNormalizer-0.2.0/MANIFEST.in
+-rw-r--r--   0 gabriel-he   (501) staff       (20)     4031 2023-06-21 02:34:36.155210 EntityNormalizer-0.2.0/PKG-INFO
+-rw-r--r--   0 gabriel-he   (501) staff       (20)     3640 2023-06-21 02:34:07.000000 EntityNormalizer-0.2.0/README.md
+-rw-r--r--   0 gabriel-he   (501) staff       (20)      160 2023-06-21 02:34:36.155428 EntityNormalizer-0.2.0/setup.cfg
+-rw-r--r--   0 gabriel-he   (501) staff       (20)      574 2023-06-21 02:34:07.000000 EntityNormalizer-0.2.0/setup.py
```

### Comparing `EntityNormalizer-0.1.0.post2/EntityNormalizer/__init__.py` & `EntityNormalizer-0.2.0/EntityNormalizer/__init__.py`

 * *Files identical despite different names*

### Comparing `EntityNormalizer-0.1.0.post2/EntityNormalizer.egg-info/PKG-INFO` & `EntityNormalizer-0.2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,23 @@
-Metadata-Version: 2.1
-Name: EntityNormalizer
-Version: 0.1.0.post2
-Summary: Library for normalizing entities based on a dictionary
-Home-page: https://github.com/sociocom/EntityNormalizer
-Download-URL: https://github.com/sociocom/EntityNormalizer/archive/refs/tags/0.1.0.tar.gz
-Author: Gabriel Herman Bernardim Andrade
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # Entity Normalizer
 
 Python tool for normalizing entities based on a dictionary.
 
 ## Usage
 
 This tool can be used as:
-- a *command line tool*, by cloning this repository and running `pip install .` under the root of this source; then you can run`main.py` with the required parameters to process your entity-listed file.
+- a *command line tool*, by cloning this repository and running `pip install .` under the root of this source; 
+then you can run`main.py` with the required parameters to process your entity-listed file.
 - a *Python package* , by installing the package using `pip install EntityNormalizer`
 
 ### Input and output
   
 The input file must contain one entity per line. 
 The output file will contain the normalized entities, again, one per line.  
-The dicitory file must be a comma-separated table file, i.e., `csv`.
+The dictionary file must be a comma-separated table file, i.e., `csv`.
 
 If the entity does not produce any match in the dictionary, it will be normalized to `[NO_MATCH]`. 
 If the entity is found in the dictionary but the normalization is empty, it will be normalized to `[NO_NORM_FOUND]`.  
   
 ----
   
 ### Command line usage
@@ -43,27 +33,67 @@
 - `target`: Normalization column from dictionary [Required]
 - `matching_threshold`: Threshold of string similarity for the normalization to be accepted (default: 50) [Optional]
 - `index`: Use column indexes instead of names [Optional]
   
 #### Example
 
 - With column names:  
+
     `python main.py data/input.txt data/output.txt data/dictionary.csv surface_form_col normalization_col --matching_threshold 50`
-- With integer column indexes: 
+- With integer column indexes:
+
     `python main.py data/input.txt data/output.txt data/dictionary.csv --index source 0 target 2 --matching_threshold 80`
 
 ---
 
  ### Python package usage
-After instalation,  the `normalized` function can be invoked with the dicitonary and a `list` of entities to produce a `list` of normalized entities.
+After installation,  the `normalize` function can be invoked with the dicitonary and a `list` of entities to produce a `list` of normalized entities.
 
 #### Example
 ```python
 from EntityNormalizer import EntityDictionary, normalize
 
-entities  =  [entity1, entity2, entity3]
+entities = ['entity1', 'entity2', 'entity3']
 
-normalization_dictionary  = EntityDictionary('data/dictionary.csv',  'surface_forms',  'normalizations')
-normalized  = normalize(entities,  normalization_dictionary,  matching_threshold=70)
+normalization_dictionary = EntityDictionary('data/dictionary.csv', 'surface_forms', 'normalizations')
+normalized = normalize(entities, normalization_dictionary, matching_threshold=70)
 
 print(normalized)
 ```
+
+## Bundled dictionaries
+
+This library comes with a set of bundled dictionaries, which can be found under the `resources` folder:
+
+- MedDic-CANCER-ADE-JA
+- MedDic-CANCER-DRUG-JA
+
+These are a set of Japanese medical dictionaries developed with normalization of concepts normally found during the
+analysis of adverse events caused by anticancer drugs. Please refer to 
+[this page](https://sociocom.naist.jp/meddic-cancer-ja/) for mor information.
+
+There are convenient classes for loading these dictionaries, which can be accessed with the `Dictionaries` module:
+
+```python
+from EntityNormalizer import Dictionaries, normalize
+
+entities = ['entity1', 'entity2', 'entity3']
+
+# Load the dictionaries
+cancer_ade = Dictionaries.MedDicCancerADE()
+cancer_drug = Dictionaries.MedDicCancerDrug()
+
+# Use the dictionaries
+normalized_ade = normalize(entities, cancer_ade, matching_threshold=70)
+normalized_drug = normalize(entities, cancer_drug, matching_threshold=70)
+```
+
+Both dictionaries use the columns `出現形` (Surface form) and `[細分類]` (Sub-classification) as source and target
+columns, respectively. 
+
+This can be altered by passing the referring parameter when creating the dictionary:
+
+```python
+from EntityNormalizer import Dictionaries
+
+cancer_ade = Dictionaries.MedDicCancerADE(source_column='customColumn', target_column='customColumn2')
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `EntityNormalizer-0.1.0.post2/LICENSE.txt` & `EntityNormalizer-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `EntityNormalizer-0.1.0.post2/PKG-INFO` & `EntityNormalizer-0.2.0/EntityNormalizer.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: EntityNormalizer
-Version: 0.1.0.post2
+Version: 0.2.0
 Summary: Library for normalizing entities based on a dictionary
 Home-page: https://github.com/sociocom/EntityNormalizer
-Download-URL: https://github.com/sociocom/EntityNormalizer/archive/refs/tags/0.1.0.tar.gz
+Download-URL: https://github.com/sociocom/EntityNormalizer/archive/refs/tags/0.2.0.tar.gz
 Author: Gabriel Herman Bernardim Andrade
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Entity Normalizer
 
 Python tool for normalizing entities based on a dictionary.
 
 ## Usage
 
 This tool can be used as:
-- a *command line tool*, by cloning this repository and running `pip install .` under the root of this source; then you can run`main.py` with the required parameters to process your entity-listed file.
+- a *command line tool*, by cloning this repository and running `pip install .` under the root of this source; 
+then you can run`main.py` with the required parameters to process your entity-listed file.
 - a *Python package* , by installing the package using `pip install EntityNormalizer`
 
 ### Input and output
   
 The input file must contain one entity per line. 
 The output file will contain the normalized entities, again, one per line.  
-The dicitory file must be a comma-separated table file, i.e., `csv`.
+The dictionary file must be a comma-separated table file, i.e., `csv`.
 
 If the entity does not produce any match in the dictionary, it will be normalized to `[NO_MATCH]`. 
 If the entity is found in the dictionary but the normalization is empty, it will be normalized to `[NO_NORM_FOUND]`.  
   
 ----
   
 ### Command line usage
@@ -43,27 +44,67 @@
 - `target`: Normalization column from dictionary [Required]
 - `matching_threshold`: Threshold of string similarity for the normalization to be accepted (default: 50) [Optional]
 - `index`: Use column indexes instead of names [Optional]
   
 #### Example
 
 - With column names:  
+
     `python main.py data/input.txt data/output.txt data/dictionary.csv surface_form_col normalization_col --matching_threshold 50`
-- With integer column indexes: 
+- With integer column indexes:
+
     `python main.py data/input.txt data/output.txt data/dictionary.csv --index source 0 target 2 --matching_threshold 80`
 
 ---
 
  ### Python package usage
-After instalation,  the `normalized` function can be invoked with the dicitonary and a `list` of entities to produce a `list` of normalized entities.
+After installation,  the `normalize` function can be invoked with the dicitonary and a `list` of entities to produce a `list` of normalized entities.
 
 #### Example
 ```python
 from EntityNormalizer import EntityDictionary, normalize
 
-entities  =  [entity1, entity2, entity3]
+entities = ['entity1', 'entity2', 'entity3']
 
-normalization_dictionary  = EntityDictionary('data/dictionary.csv',  'surface_forms',  'normalizations')
-normalized  = normalize(entities,  normalization_dictionary,  matching_threshold=70)
+normalization_dictionary = EntityDictionary('data/dictionary.csv', 'surface_forms', 'normalizations')
+normalized = normalize(entities, normalization_dictionary, matching_threshold=70)
 
 print(normalized)
 ```
+
+## Bundled dictionaries
+
+This library comes with a set of bundled dictionaries, which can be found under the `resources` folder:
+
+- MedDic-CANCER-ADE-JA
+- MedDic-CANCER-DRUG-JA
+
+These are a set of Japanese medical dictionaries developed with normalization of concepts normally found during the
+analysis of adverse events caused by anticancer drugs. Please refer to 
+[this page](https://sociocom.naist.jp/meddic-cancer-ja/) for mor information.
+
+There are convenient classes for loading these dictionaries, which can be accessed with the `Dictionaries` module:
+
+```python
+from EntityNormalizer import Dictionaries, normalize
+
+entities = ['entity1', 'entity2', 'entity3']
+
+# Load the dictionaries
+cancer_ade = Dictionaries.MedDicCancerADE()
+cancer_drug = Dictionaries.MedDicCancerDrug()
+
+# Use the dictionaries
+normalized_ade = normalize(entities, cancer_ade, matching_threshold=70)
+normalized_drug = normalize(entities, cancer_drug, matching_threshold=70)
+```
+
+Both dictionaries use the columns `出現形` (Surface form) and `[細分類]` (Sub-classification) as source and target
+columns, respectively. 
+
+This can be altered by passing the referring parameter when creating the dictionary:
+
+```python
+from EntityNormalizer import Dictionaries
+
+cancer_ade = Dictionaries.MedDicCancerADE(source_column='customColumn', target_column='customColumn2')
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `EntityNormalizer-0.1.0.post2/setup.py` & `EntityNormalizer-0.2.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from setuptools import find_packages, setup
 setup(
     name='EntityNormalizer',
     packages=find_packages(),
-    version='0.1.0-2',
+    version='0.2.0',
     description='Library for normalizing entities based on a dictionary',
     author='Gabriel Herman Bernardim Andrade',
     license='MIT',
     readme='README.md',
     url='https://github.com/sociocom/EntityNormalizer',
-    download_url='https://github.com/sociocom/EntityNormalizer/archive/refs/tags/0.1.0.tar.gz',
+    download_url='https://github.com/sociocom/EntityNormalizer/archive/refs/tags/0.2.0.tar.gz',
+    include_package_data=True,
     py_modules=['EntityNormalizer'],
     install_requires=['pandas', 'rapidfuzz', 'mojimoji'],
 )
```

