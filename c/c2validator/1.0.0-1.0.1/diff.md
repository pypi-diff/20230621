# Comparing `tmp/c2validator-1.0.0.tar.gz` & `tmp/c2validator-1.0.1.tar.gz`

## Comparing `c2validator-1.0.0.tar` & `c2validator-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,17 @@
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 c2validator-1.0.0/pytest.ini
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c2validator-1.0.0/src/__init__.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 c2validator-1.0.0/src/c2validator/__init__.py
--rw-r--r--   0        0        0     8416 2020-02-02 00:00:00.000000 c2validator-1.0.0/src/c2validator/validator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c2validator-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 c2validator-1.0.0/tests/tests_cpf_and_cnpj_generator.py
--rw-r--r--   0        0        0     7404 2020-02-02 00:00:00.000000 c2validator-1.0.0/tests/tests_cpf_and_cnpj_validator.py
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 c2validator-1.0.0/tests/tests_validaor_and_generator_base.py
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 c2validator-1.0.0/tests/tests_validator_and_generator_base.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 c2validator-1.0.0/.gitignore
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 c2validator-1.0.0/LICENSE
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 c2validator-1.0.0/README.md
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 c2validator-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 c2validator-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 c2validator-1.0.1/pytest.ini
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 c2validator-1.0.1/requirements.txt
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 c2validator-1.0.1/c2validator/__init__.py
+-rw-r--r--   0        0        0     8038 2020-02-02 00:00:00.000000 c2validator-1.0.1/c2validator/validator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c2validator-1.0.1/src/__init__.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 c2validator-1.0.1/src/c2validator/__init__.py
+-rw-r--r--   0        0        0     8416 2020-02-02 00:00:00.000000 c2validator-1.0.1/src/c2validator/validator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c2validator-1.0.1/tests/__init__.py
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 c2validator-1.0.1/tests/tests_cpf_and_cnpj_generator.py
+-rw-r--r--   0        0        0     7404 2020-02-02 00:00:00.000000 c2validator-1.0.1/tests/tests_cpf_and_cnpj_validator.py
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 c2validator-1.0.1/tests/tests_validaor_and_generator_base.py
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 c2validator-1.0.1/tests/tests_validator_and_generator_base.py
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 c2validator-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 c2validator-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 c2validator-1.0.1/README.md
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 c2validator-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 c2validator-1.0.1/PKG-INFO
```

### Comparing `c2validator-1.0.0/src/c2validator/validator.py` & `c2validator-1.0.1/src/c2validator/validator.py`

 * *Files identical despite different names*

### Comparing `c2validator-1.0.0/tests/tests_cpf_and_cnpj_generator.py` & `c2validator-1.0.1/tests/tests_cpf_and_cnpj_generator.py`

 * *Files identical despite different names*

### Comparing `c2validator-1.0.0/tests/tests_cpf_and_cnpj_validator.py` & `c2validator-1.0.1/tests/tests_cpf_and_cnpj_validator.py`

 * *Files identical despite different names*

### Comparing `c2validator-1.0.0/tests/tests_validaor_and_generator_base.py` & `c2validator-1.0.1/tests/tests_validaor_and_generator_base.py`

 * *Files identical despite different names*

### Comparing `c2validator-1.0.0/tests/tests_validator_and_generator_base.py` & `c2validator-1.0.1/tests/tests_validator_and_generator_base.py`

 * *Files identical despite different names*

### Comparing `c2validator-1.0.0/.gitignore` & `c2validator-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `c2validator-1.0.0/LICENSE` & `c2validator-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `c2validator-1.0.0/README.md` & `c2validator-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -18,34 +18,34 @@
 True
 ```
 
 
 This is semple.
 If CPF or CNPJ is invalid, the return we will `False`.
 
-If the value contains letters symbols or punctuation, a private __clean() method will clean the data before validate.
+If the value contains letters, symbols or punctuation, a private __clean() method will clean the data before validate.
 
 ```
 >>> import c2validator as c2
 >>> 
->>> cpf = c2.validate('725.849abc.240//-21') 
+>>> cpf = c2.validate('725.849.240-21') 
 >>> cpf.is_valid()
 True
 ```
 
 ## Returning a clean value
 When the CPF or CNPJ is valid, you can use the formatted() method.
 This method returns the value without symbols, letters or punctuation.
 But, if you need a formatted data with punctuation, you can use
 formatted(punctuation=True).
 
 ```
 >>> import c2validator as c2
 >>> 
->>> cpf = c2.validate('725.849abc.240//-21') 
+>>> cpf = c2.validate('725.849.240-21') 
 >>> cpf.is_valid()
 True
 >>> cpf.formatted()
 '72584924021'
 >>> cpf.formatted(punctuation=True) 
 '725.849.240-21'
 ```
```

### Comparing `c2validator-1.0.0/pyproject.toml` & `c2validator-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "c2validator"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Guilherme Costa", email="guilherme.partic@gmail.com" },
 ]
 description = "This package validate and generate CPF and CNPJ for tests"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `c2validator-1.0.0/PKG-INFO` & `c2validator-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c2validator
-Version: 1.0.0
+Version: 1.0.1
 Summary: This package validate and generate CPF and CNPJ for tests
 Project-URL: Homepage, https://github.com/devguilhermecosta/c2validator
 Project-URL: Bug Tracker, https://github.com/devguilhermecosta/c2validator/issues
 Author-email: Guilherme Costa <guilherme.partic@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -32,34 +32,34 @@
 True
 ```
 
 
 This is semple.
 If CPF or CNPJ is invalid, the return we will `False`.
 
-If the value contains letters symbols or punctuation, a private __clean() method will clean the data before validate.
+If the value contains letters, symbols or punctuation, a private __clean() method will clean the data before validate.
 
 ```
 >>> import c2validator as c2
 >>> 
->>> cpf = c2.validate('725.849abc.240//-21') 
+>>> cpf = c2.validate('725.849.240-21') 
 >>> cpf.is_valid()
 True
 ```
 
 ## Returning a clean value
 When the CPF or CNPJ is valid, you can use the formatted() method.
 This method returns the value without symbols, letters or punctuation.
 But, if you need a formatted data with punctuation, you can use
 formatted(punctuation=True).
 
 ```
 >>> import c2validator as c2
 >>> 
->>> cpf = c2.validate('725.849abc.240//-21') 
+>>> cpf = c2.validate('725.849.240-21') 
 >>> cpf.is_valid()
 True
 >>> cpf.formatted()
 '72584924021'
 >>> cpf.formatted(punctuation=True) 
 '725.849.240-21'
 ```
```

