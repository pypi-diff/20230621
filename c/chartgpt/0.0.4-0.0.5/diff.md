# Comparing `tmp/chartgpt-0.0.4.tar.gz` & `tmp/chartgpt-0.0.5.tar.gz`

## Comparing `chartgpt-0.0.4.tar` & `chartgpt-0.0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 chartgpt-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 chartgpt-0.0.4/mkdocs.yml
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 chartgpt-0.0.4/requirements.txt
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 chartgpt-0.0.4/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 chartgpt-0.0.4/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 chartgpt-0.0.4/.github/workflows/test.yml
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 chartgpt-0.0.4/chartgpt/__init__.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 chartgpt-0.0.4/chartgpt/__main__.py
--rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 chartgpt-0.0.4/chartgpt/chartgpt.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 chartgpt-0.0.4/chartgpt/constants.py
--rw-r--r--   0        0        0     4544 2020-02-02 00:00:00.000000 chartgpt-0.0.4/chartgpt/llm.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 chartgpt-0.0.4/chartgpt/prompts/base.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 chartgpt-0.0.4/chartgpt/prompts/generate_python_code.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 chartgpt-0.0.4/docs/api-generated.md
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 chartgpt-0.0.4/docs/index.md
--rw-r--r--   0        0        0    80099 2020-02-02 00:00:00.000000 chartgpt-0.0.4/docs/assets/chart.png
--rw-r--r--   0        0        0   925601 2020-02-02 00:00:00.000000 chartgpt-0.0.4/docs/assets/dash.png
--rw-r--r--   0        0        0   746570 2020-02-02 00:00:00.000000 chartgpt-0.0.4/docs/assets/notebook.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chartgpt-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 chartgpt-0.0.4/tests/test_run_code.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 chartgpt-0.0.4/.gitignore
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 chartgpt-0.0.4/LICENSE
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 chartgpt-0.0.4/README.md
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 chartgpt-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 chartgpt-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 chartgpt-0.0.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 chartgpt-0.0.5/mkdocs.yml
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 chartgpt-0.0.5/requirements.txt
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 chartgpt-0.0.5/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 chartgpt-0.0.5/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 chartgpt-0.0.5/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 chartgpt-0.0.5/chartgpt/__init__.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 chartgpt-0.0.5/chartgpt/__main__.py
+-rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 chartgpt-0.0.5/chartgpt/chartgpt.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 chartgpt-0.0.5/chartgpt/constants.py
+-rw-r--r--   0        0        0     4544 2020-02-02 00:00:00.000000 chartgpt-0.0.5/chartgpt/llm.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 chartgpt-0.0.5/chartgpt/prompts/base.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 chartgpt-0.0.5/chartgpt/prompts/generate_python_code.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 chartgpt-0.0.5/docs/api-generated.md
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 chartgpt-0.0.5/docs/index.md
+-rw-r--r--   0        0        0    80099 2020-02-02 00:00:00.000000 chartgpt-0.0.5/docs/assets/chart.png
+-rw-r--r--   0        0        0   925601 2020-02-02 00:00:00.000000 chartgpt-0.0.5/docs/assets/dash.png
+-rw-r--r--   0        0        0   746570 2020-02-02 00:00:00.000000 chartgpt-0.0.5/docs/assets/notebook.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chartgpt-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 chartgpt-0.0.5/tests/test_run_code.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 chartgpt-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 chartgpt-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 chartgpt-0.0.5/README.md
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 chartgpt-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 chartgpt-0.0.5/PKG-INFO
```

### Comparing `chartgpt-0.0.4/.pre-commit-config.yaml` & `chartgpt-0.0.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `chartgpt-0.0.4/mkdocs.yml` & `chartgpt-0.0.5/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `chartgpt-0.0.4/.devcontainer/devcontainer.json` & `chartgpt-0.0.5/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `chartgpt-0.0.4/.github/workflows/publish.yml` & `chartgpt-0.0.5/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `chartgpt-0.0.4/.github/workflows/test.yml` & `chartgpt-0.0.5/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `chartgpt-0.0.4/chartgpt/__init__.py` & `chartgpt-0.0.5/chartgpt/__init__.py`

 * *Files identical despite different names*

### Comparing `chartgpt-0.0.4/chartgpt/chartgpt.py` & `chartgpt-0.0.5/chartgpt/chartgpt.py`

 * *Files identical despite different names*

### Comparing `chartgpt-0.0.4/chartgpt/constants.py` & `chartgpt-0.0.5/chartgpt/constants.py`

 * *Files identical despite different names*

### Comparing `chartgpt-0.0.4/chartgpt/llm.py` & `chartgpt-0.0.5/chartgpt/llm.py`

 * *Files identical despite different names*

### Comparing `chartgpt-0.0.4/chartgpt/prompts/base.py` & `chartgpt-0.0.5/chartgpt/prompts/base.py`

 * *Files identical despite different names*

### Comparing `chartgpt-0.0.4/chartgpt/prompts/generate_python_code.py` & `chartgpt-0.0.5/chartgpt/prompts/generate_python_code.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 When asked about the data, your response must include a python code that uses the \
 library Plotly to make a chart using the dataframe `df`. If necessary, you can filter \
 the dataframe `df`. You can use any chart type you want.
 Using the provided dataframe, df, return the python code and make sure to prefix the \
 requested python code with {START_CODE_TAG} exactly and suffix the code with \
 {END_CODE_TAG} exactly to get the answer to the following question:
+{user_prompt}
 """
 
     def __init__(self, **kwargs):
         super().__init__(
             today_date=date.today(),
             START_CODE_TAG=START_CODE_TAG,
             END_CODE_TAG=END_CODE_TAG,
```

### Comparing `chartgpt-0.0.4/docs/index.md` & `chartgpt-0.0.5/docs/index.md`

 * *Files identical despite different names*

### Comparing `chartgpt-0.0.4/docs/assets/chart.png` & `chartgpt-0.0.5/docs/assets/chart.png`

 * *Files identical despite different names*

### Comparing `chartgpt-0.0.4/docs/assets/dash.png` & `chartgpt-0.0.5/docs/assets/dash.png`

 * *Files identical despite different names*

### Comparing `chartgpt-0.0.4/docs/assets/notebook.png` & `chartgpt-0.0.5/docs/assets/notebook.png`

 * *Files identical despite different names*

### Comparing `chartgpt-0.0.4/tests/test_run_code.py` & `chartgpt-0.0.5/tests/test_run_code.py`

 * *Files identical despite different names*

### Comparing `chartgpt-0.0.4/LICENSE` & `chartgpt-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `chartgpt-0.0.4/README.md` & `chartgpt-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `chartgpt-0.0.4/pyproject.toml` & `chartgpt-0.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "chartgpt"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Elie Brosset", email="eliebrosset@gmail.com" },
 ]
 description = "ChartGPT is a library for generating charts from text"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `chartgpt-0.0.4/PKG-INFO` & `chartgpt-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chartgpt
-Version: 0.0.4
+Version: 0.0.5
 Summary: ChartGPT is a library for generating charts from text
 Project-URL: Homepage, https://github.com/chatgpt/chart
 Author-email: Elie Brosset <eliebrosset@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

