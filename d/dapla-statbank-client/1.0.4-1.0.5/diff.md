# Comparing `tmp/dapla_statbank_client-1.0.4.tar.gz` & `tmp/dapla_statbank_client-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dapla_statbank_client-1.0.4.tar", max compression
+gzip compressed data, was "dapla_statbank_client-1.0.5.tar", max compression
```

## Comparing `dapla_statbank_client-1.0.4.tar` & `dapla_statbank_client-1.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1074 2023-05-08 06:04:34.724356 dapla_statbank_client-1.0.4/LICENSE
--rw-r--r--   0        0        0     9087 2023-05-08 06:04:34.724356 dapla_statbank_client-1.0.4/README.md
--rw-r--r--   0        0        0     1119 2023-05-08 06:04:56.424735 dapla_statbank_client-1.0.4/pyproject.toml
--rw-r--r--   0        0        0      206 2023-05-08 06:04:56.424735 dapla_statbank_client-1.0.4/statbank/__init__.py
--rw-r--r--   0        0        0     5651 2023-05-08 06:04:34.724356 dapla_statbank_client-1.0.4/statbank/apidata.py
--rw-r--r--   0        0        0     3668 2023-05-08 06:04:34.724356 dapla_statbank_client-1.0.4/statbank/auth.py
--rw-r--r--   0        0        0    17571 2023-05-08 06:04:34.724356 dapla_statbank_client-1.0.4/statbank/client.py
--rw-r--r--   0        0        0    13617 2023-05-08 06:04:34.724356 dapla_statbank_client-1.0.4/statbank/transfer.py
--rw-r--r--   0        0        0    13722 2023-05-08 06:04:34.728356 dapla_statbank_client-1.0.4/statbank/uttrekk.py
--rw-r--r--   0        0        0    14153 2023-05-08 06:04:34.728356 dapla_statbank_client-1.0.4/statbank/uttrekk_validations.py
--rw-r--r--   0        0        0     9786 1970-01-01 00:00:00.000000 dapla_statbank_client-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-21 06:28:23.912741 dapla_statbank_client-1.0.5/LICENSE
+-rw-r--r--   0        0        0     9274 2023-06-21 06:28:44.577244 dapla_statbank_client-1.0.5/README.md
+-rw-r--r--   0        0        0     1119 2023-06-21 06:28:44.577244 dapla_statbank_client-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0      206 2023-06-21 06:28:44.581244 dapla_statbank_client-1.0.5/statbank/__init__.py
+-rw-r--r--   0        0        0     5651 2023-06-21 06:28:23.916741 dapla_statbank_client-1.0.5/statbank/apidata.py
+-rw-r--r--   0        0        0     3668 2023-06-21 06:28:23.916741 dapla_statbank_client-1.0.5/statbank/auth.py
+-rw-r--r--   0        0        0    17571 2023-06-21 06:28:23.916741 dapla_statbank_client-1.0.5/statbank/client.py
+-rw-r--r--   0        0        0    13617 2023-06-21 06:28:23.916741 dapla_statbank_client-1.0.5/statbank/transfer.py
+-rw-r--r--   0        0        0    15368 2023-06-21 06:28:44.581244 dapla_statbank_client-1.0.5/statbank/uttrekk.py
+-rw-r--r--   0        0        0    14290 2023-06-21 06:28:44.581244 dapla_statbank_client-1.0.5/statbank/uttrekk_validations.py
+-rw-r--r--   0        0        0     9973 1970-01-01 00:00:00.000000 dapla_statbank_client-1.0.5/PKG-INFO
```

### Comparing `dapla_statbank_client-1.0.4/LICENSE` & `dapla_statbank_client-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dapla_statbank_client-1.0.4/README.md` & `dapla_statbank_client-1.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -126,15 +126,16 @@
 filbesk_06339_new = stat_client.read_description_json("path.json")
 ```
 Some deeper data-structures, like the dataframes in the transfer will not be serialized and stored with the transfer-object in its json.
 
 ---
 
 ### Version history
-- 1.0.3 Fixing bug where empty codelists stops description initialization, Updating pyjstat to 2.4.0, changing imports to absolute from package root
+- 1.0.5 Making transferdata_template smarter, were it can take a bunch of dataframes and incorporate them in the returned dict. Trying to support columntype "internasjonal rapportering".
+- 1.0.4 Fixing bug where empty codelists stops description initialization, Updating pyjstat to 2.4.0, changing imports to absolute from package root
 - 1.0.2 Doc-string style cleanup, a check on username and password on client init, changes to time and display of time, demo notebooks cleaned
 - 1.0.0 Finished going through initial issues, less complaining from verify on floats
 - 0.0.11 Statbank people wanted a user-agent-requesst-header to differentiate test from prod
 - 0.0.9 After further user-testing and requests
 - 0.0.5 Still some parameter issues
 - 0.0.4 More test coverage, some bugs fixed in rounding checks and parameter-passing
 - 0.0.3 Removed batches, stripping uttrekk from transfer, rounding function on uttrekk, data required in as a dict of dataframes, with "deltabell-navn". Tableid now works to transfer to instead of only "hovedtabellnavn"
```

### Comparing `dapla_statbank_client-1.0.4/pyproject.toml` & `dapla_statbank_client-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dapla-statbank-client"
-version = "1.0.4"
+version = "1.0.5"
 description = "Handles data transfer Statbank <-> Dapla for Statistics Norway"
 authors = ["Statistics Norway", "Carl F. Corneil <cfc@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "statbank"}]
 
 [tool.poetry.dependencies]
```

### Comparing `dapla_statbank_client-1.0.4/statbank/apidata.py` & `dapla_statbank_client-1.0.5/statbank/apidata.py`

 * *Files identical despite different names*

### Comparing `dapla_statbank_client-1.0.4/statbank/auth.py` & `dapla_statbank_client-1.0.5/statbank/auth.py`

 * *Files identical despite different names*

### Comparing `dapla_statbank_client-1.0.4/statbank/client.py` & `dapla_statbank_client-1.0.5/statbank/client.py`

 * *Files identical despite different names*

### Comparing `dapla_statbank_client-1.0.4/statbank/transfer.py` & `dapla_statbank_client-1.0.5/statbank/transfer.py`

 * *Files identical despite different names*

### Comparing `dapla_statbank_client-1.0.4/statbank/uttrekk.py` & `dapla_statbank_client-1.0.5/statbank/uttrekk.py`

 * *Files 8% similar despite different names*

```diff
@@ -100,14 +100,16 @@
         for i, deltabell in enumerate(self.variables):
             variabel_text += f"""\nDeltabell (DataFrame) nummer {i+1}:
                 {deltabell["deltabell"]}
                 """
             variables = [*deltabell["variabler"], *deltabell["statistikkvariabler"]]
             if "null_prikk_missing" in deltabell.keys():
                 variables += deltabell["null_prikk_missing"]
+            if "internasjonal_rapportering" in deltabell.keys():
+                variables += deltabell["internasjonal_rapportering"]
             variabel_text += f"Antall kolonner: {len(variables)}"
             for i, variabel in enumerate(variables):
                 variabel_text += f"\n\tKolonne {i+1}: "
                 if "Kodeliste_text" in variabel.keys():
                     variabel_text += variabel["Kodeliste_text"]
                 elif "Text" in variabel.keys():
                     variabel_text += variabel["Text"]
@@ -128,27 +130,55 @@
 
     def __repr__(self):
         return (
             'StatbankUttrekksBeskrivelse(tableid="'
             + f'{self.tableid}", loaduser="{self.loaduser}")'
         )
 
-    def transferdata_template(self) -> dict:
+    def transferdata_template(self, *dfs: list[pd.DataFrame] | pd.DataFrame) -> dict:
         """Get the shape the data should have to name the "deltabeller".
         If we didnt use a dictionary we would have to rely on the order of a list of "deltabeller".
-        Instead we chose to explicitly name the deltabller in this package.
+        Instead we chose to explicitly name the deltabller in this package, and make you check this after creation.
+
+        Parameters
+        -------
+        dfs: if provided, will try to use pandas dataframes sent in to populate the dict returned by the method.
+            Send in one dataframe, several, a list of dataframes or similar.
+            ORDER IS IMPORTANT make sure the result is what you expect.
 
         Returns
         -------
-        A dictionary with correct keys, but placeholders for where the dataframes should go.
+        A dictionary with correct keys, but placeholders for where the dataframes should go if no Dataframes are passed.
+        A dict of dataframes as values if a list of Dataframes are sent in, or dataframes as individual parameters.
         """
-        template = {k: f"df{i}" for i, (k, v) in enumerate(self.subtables.items())}
+
+        # If sending in a list, unwrap one layer
+        if not isinstance(dfs[0], pd.DataFrame) and len(dfs) == 1:
+            dfs = dfs[0]
+        if dfs:
+            if not all([isinstance(df, pd.DataFrame) for df in dfs]):
+                raise TypeError(
+                    "All elements sent in to transferdata_template must be pandas dataframes."
+                )
+            if not len(dfs) == len(self.subtables):
+                raise KeyError(
+                    "Number of dataframes in must match the number of subtables."
+                )
+
+        if dfs:
+            template = {k: dfs[i] for i, k in enumerate(self.subtables.keys())}
+        else:
+            template = {k: f"df{i}" for i, k in enumerate(self.subtables.keys())}
+
         print("{")
         for k, v in template.items():
-            print(f'"{k}" : {v},')
+            if isinstance(v, pd.DataFrame):
+                print(f'"{k}" : Dataframe with column-names: {v.columns}')
+            else:
+                print(f'"{k}" : {v},')
         print("}")
         return template
 
     def to_json(self, path: str = "") -> dict:
         """Store a copy of the current state of the uttrekk-object as a json.
         If path is provided, tries to write to it,
         otherwise will return a json-string for you to handle like you wish.
@@ -312,15 +342,18 @@
         self.tablename = self.filbeskrivelse["Huvudtabell"]
         self.subtables = {
             x["Filnavn"]: x["Filtext"] for x in self.filbeskrivelse["DeltabellTitler"]
         }
         self.variables = self.filbeskrivelse["deltabller"]
         self.codelists = {}
         if "kodelister" in self.filbeskrivelse.keys():
-            for kodeliste in self.filbeskrivelse["kodelister"]:
+            kodelister = self.filbeskrivelse["kodelister"]
+            if "IRkodelister" in self.filbeskrivelse.keys():
+                kodelister = {**kodelister, **self.filbeskrivelse["IRkodelister"]}
+            for kodeliste in kodelister:
                 new_kodeliste = {}
                 for kode in kodeliste["koder"]:
                     new_kodeliste[kode["kode"]] = kode["text"]
                 self.codelists[kodeliste["kodeliste"]] = {"koder": new_kodeliste}
                 remain_keys = list(kodeliste.keys())
                 remain_keys.remove("koder")
                 remain_keys.remove("kodeliste")
```

### Comparing `dapla_statbank_client-1.0.4/statbank/uttrekk_validations.py` & `dapla_statbank_client-1.0.5/statbank/uttrekk_validations.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,20 +19,22 @@
         for deltabell_num, deltabell in enumerate(self.variables):
             deltabell_navn = deltabell["deltabell"]
             col_num = len(deltabell["variabler"]) + len(
                 deltabell["statistikkvariabler"]
             )  # Mangler prikke-kolonner?
             if "null_prikk_missing" in deltabell.keys():
                 col_num += len(deltabell["null_prikk_missing"])
+            if "internasjonal_rapportering" in deltabell.keys():
+                col_num += len(deltabell["internasjonal_rapportering"])
             if len(data[deltabell_navn].columns) != col_num:
                 validation_errors[f"col_count_data_{deltabell_num}"] = ValueError(
                     f"""
-                    EXPECTING {col_num} COLUMNS IN DATFRAME NUMBER
-                    {deltabell_num}: {deltabell_navn}
-                    ONLY FOUND {len(data[deltabell_navn].columns)}
+                    EXPECTING {col_num} COLUMNS IN DATAFRAME NUMBER {deltabell_num}:
+                    {deltabell_navn}
+                    BUT FOUND {len(data[deltabell_navn].columns)}
                     """
                 )
         for k in validation_errors.keys():
             if "col_count_data" in k:
                 if printing:
                     print(validation_errors[k])
                 break
```

### Comparing `dapla_statbank_client-1.0.4/PKG-INFO` & `dapla_statbank_client-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dapla-statbank-client
-Version: 1.0.4
+Version: 1.0.5
 Summary: Handles data transfer Statbank <-> Dapla for Statistics Norway
 License: MIT
 Author: Statistics Norway
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -145,15 +145,16 @@
 filbesk_06339_new = stat_client.read_description_json("path.json")
 ```
 Some deeper data-structures, like the dataframes in the transfer will not be serialized and stored with the transfer-object in its json.
 
 ---
 
 ### Version history
-- 1.0.3 Fixing bug where empty codelists stops description initialization, Updating pyjstat to 2.4.0, changing imports to absolute from package root
+- 1.0.5 Making transferdata_template smarter, were it can take a bunch of dataframes and incorporate them in the returned dict. Trying to support columntype "internasjonal rapportering".
+- 1.0.4 Fixing bug where empty codelists stops description initialization, Updating pyjstat to 2.4.0, changing imports to absolute from package root
 - 1.0.2 Doc-string style cleanup, a check on username and password on client init, changes to time and display of time, demo notebooks cleaned
 - 1.0.0 Finished going through initial issues, less complaining from verify on floats
 - 0.0.11 Statbank people wanted a user-agent-requesst-header to differentiate test from prod
 - 0.0.9 After further user-testing and requests
 - 0.0.5 Still some parameter issues
 - 0.0.4 More test coverage, some bugs fixed in rounding checks and parameter-passing
 - 0.0.3 Removed batches, stripping uttrekk from transfer, rounding function on uttrekk, data required in as a dict of dataframes, with "deltabell-navn". Tableid now works to transfer to instead of only "hovedtabellnavn"
```

