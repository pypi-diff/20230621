# Comparing `tmp/Paymob-Toolbox-0.0.1.tar.gz` & `tmp/Paymob-Toolbox-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Paymob-Toolbox-0.0.1.tar", last modified: Tue Jun 20 21:50:07 2023, max compression
+gzip compressed data, was "Paymob-Toolbox-0.0.2.tar", last modified: Wed Jun 21 10:59:10 2023, max compression
```

## Comparing `Paymob-Toolbox-0.0.1.tar` & `Paymob-Toolbox-0.0.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:50:07.260247 Paymob-Toolbox-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-06-20 21:50:07.260247 Paymob-Toolbox-0.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:50:07.244246 Paymob-Toolbox-0.0.1/Paymob_Toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-06-20 21:50:07.000000 Paymob-Toolbox-0.0.1/Paymob_Toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-20 21:50:07.000000 Paymob-Toolbox-0.0.1/Paymob_Toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 21:50:07.000000 Paymob-Toolbox-0.0.1/Paymob_Toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-20 21:50:07.000000 Paymob-Toolbox-0.0.1/Paymob_Toolbox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5733 2023-06-20 21:49:59.000000 Paymob-Toolbox-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:50:07.248246 Paymob-Toolbox-0.0.1/paymob/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:49:59.000000 Paymob-Toolbox-0.0.1/paymob/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:50:07.248246 Paymob-Toolbox-0.0.1/paymob/accept/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-20 21:49:59.000000 Paymob-Toolbox-0.0.1/paymob/accept/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16749 2023-06-20 21:49:59.000000 Paymob-Toolbox-0.0.1/paymob/accept/accept_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:50:07.252246 Paymob-Toolbox-0.0.1/paymob/accept/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-20 21:49:59.000000 Paymob-Toolbox-0.0.1/paymob/accept/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-20 21:49:59.000000 Paymob-Toolbox-0.0.1/paymob/accept/callbacks/card_token_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-20 21:49:59.000000 Paymob-Toolbox-0.0.1/paymob/accept/callbacks/delivery_status_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-20 21:49:59.000000 Paymob-Toolbox-0.0.1/paymob/accept/callbacks/generic_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-20 21:49:59.000000 Paymob-Toolbox-0.0.1/paymob/accept/callbacks/transaction_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-20 21:49:59.000000 Paymob-Toolbox-0.0.1/paymob/accept/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-06-20 21:49:59.000000 Paymob-Toolbox-0.0.1/paymob/accept/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-20 21:49:59.000000 Paymob-Toolbox-0.0.1/paymob/accept/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:50:07.256247 Paymob-Toolbox-0.0.1/paymob/accept/data_classes/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-20 21:49:59.000000 Paymob-Toolbox-0.0.1/paymob/accept/data_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-20 21:49:59.000000 Paymob-Toolbox-0.0.1/paymob/accept/data_classes/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-20 21:49:59.000000 Paymob-Toolbox-0.0.1/paymob/accept/data_classes/merchant.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-20 21:49:59.000000 Paymob-Toolbox-0.0.1/paymob/accept/data_classes/order.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-20 21:49:59.000000 Paymob-Toolbox-0.0.1/paymob/accept/data_classes/order_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-20 21:49:59.000000 Paymob-Toolbox-0.0.1/paymob/accept/data_classes/payment_key_claims.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-20 21:49:59.000000 Paymob-Toolbox-0.0.1/paymob/accept/data_classes/shipping_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-20 21:49:59.000000 Paymob-Toolbox-0.0.1/paymob/accept/data_classes/source_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-20 21:49:59.000000 Paymob-Toolbox-0.0.1/paymob/accept/data_classes/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-20 21:49:59.000000 Paymob-Toolbox-0.0.1/paymob/accept/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-06-20 21:49:59.000000 Paymob-Toolbox-0.0.1/paymob/accept/hmac_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-20 21:49:59.000000 Paymob-Toolbox-0.0.1/paymob/accept/response_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-06-20 21:49:59.000000 Paymob-Toolbox-0.0.1/paymob/accept/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-20 21:49:59.000000 Paymob-Toolbox-0.0.1/paymob/accept/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:50:07.256247 Paymob-Toolbox-0.0.1/paymob/data_classes/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-20 21:49:59.000000 Paymob-Toolbox-0.0.1/paymob/data_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-20 21:49:59.000000 Paymob-Toolbox-0.0.1/paymob/data_classes/response_feedback_dataclass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:50:07.256247 Paymob-Toolbox-0.0.1/paymob/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-20 21:49:59.000000 Paymob-Toolbox-0.0.1/paymob/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-20 21:49:59.000000 Paymob-Toolbox-0.0.1/paymob/utils/class_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-20 21:49:59.000000 Paymob-Toolbox-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 21:50:07.260247 Paymob-Toolbox-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-20 21:50:05.000000 Paymob-Toolbox-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:50:07.256247 Paymob-Toolbox-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:49:59.000000 Paymob-Toolbox-0.0.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:50:07.260247 Paymob-Toolbox-0.0.1/tests/accept/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:49:59.000000 Paymob-Toolbox-0.0.1/tests/accept/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-06-20 21:49:59.000000 Paymob-Toolbox-0.0.1/tests/accept/test_accept_utils_class.py
--rw-r--r--   0 runner    (1001) docker     (123)    18188 2023-06-20 21:49:59.000000 Paymob-Toolbox-0.0.1/tests/accept/test_hmac_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-20 21:49:59.000000 Paymob-Toolbox-0.0.1/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:59:10.270818 Paymob-Toolbox-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-06-21 10:59:10.270818 Paymob-Toolbox-0.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:59:10.266818 Paymob-Toolbox-0.0.2/Paymob_Toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-06-21 10:59:10.000000 Paymob-Toolbox-0.0.2/Paymob_Toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-21 10:59:10.000000 Paymob-Toolbox-0.0.2/Paymob_Toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 10:59:10.000000 Paymob-Toolbox-0.0.2/Paymob_Toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-21 10:59:10.000000 Paymob-Toolbox-0.0.2/Paymob_Toolbox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5733 2023-06-21 10:59:04.000000 Paymob-Toolbox-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:59:10.266818 Paymob-Toolbox-0.0.2/paymob/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 10:59:04.000000 Paymob-Toolbox-0.0.2/paymob/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:59:10.270818 Paymob-Toolbox-0.0.2/paymob/accept/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-21 10:59:04.000000 Paymob-Toolbox-0.0.2/paymob/accept/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16749 2023-06-21 10:59:04.000000 Paymob-Toolbox-0.0.2/paymob/accept/accept_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:59:10.270818 Paymob-Toolbox-0.0.2/paymob/accept/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-21 10:59:04.000000 Paymob-Toolbox-0.0.2/paymob/accept/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-21 10:59:04.000000 Paymob-Toolbox-0.0.2/paymob/accept/callbacks/card_token_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-21 10:59:04.000000 Paymob-Toolbox-0.0.2/paymob/accept/callbacks/delivery_status_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-21 10:59:04.000000 Paymob-Toolbox-0.0.2/paymob/accept/callbacks/generic_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-21 10:59:04.000000 Paymob-Toolbox-0.0.2/paymob/accept/callbacks/transaction_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-21 10:59:04.000000 Paymob-Toolbox-0.0.2/paymob/accept/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-06-21 10:59:04.000000 Paymob-Toolbox-0.0.2/paymob/accept/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-21 10:59:04.000000 Paymob-Toolbox-0.0.2/paymob/accept/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:59:10.270818 Paymob-Toolbox-0.0.2/paymob/accept/data_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-21 10:59:04.000000 Paymob-Toolbox-0.0.2/paymob/accept/data_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-21 10:59:04.000000 Paymob-Toolbox-0.0.2/paymob/accept/data_classes/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-21 10:59:04.000000 Paymob-Toolbox-0.0.2/paymob/accept/data_classes/merchant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-21 10:59:04.000000 Paymob-Toolbox-0.0.2/paymob/accept/data_classes/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-21 10:59:04.000000 Paymob-Toolbox-0.0.2/paymob/accept/data_classes/order_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-21 10:59:04.000000 Paymob-Toolbox-0.0.2/paymob/accept/data_classes/payment_key_claims.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-21 10:59:04.000000 Paymob-Toolbox-0.0.2/paymob/accept/data_classes/shipping_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-21 10:59:04.000000 Paymob-Toolbox-0.0.2/paymob/accept/data_classes/source_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-21 10:59:04.000000 Paymob-Toolbox-0.0.2/paymob/accept/data_classes/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-21 10:59:04.000000 Paymob-Toolbox-0.0.2/paymob/accept/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-06-21 10:59:04.000000 Paymob-Toolbox-0.0.2/paymob/accept/hmac_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-21 10:59:04.000000 Paymob-Toolbox-0.0.2/paymob/accept/response_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-06-21 10:59:04.000000 Paymob-Toolbox-0.0.2/paymob/accept/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-21 10:59:04.000000 Paymob-Toolbox-0.0.2/paymob/accept/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:59:10.270818 Paymob-Toolbox-0.0.2/paymob/data_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-21 10:59:04.000000 Paymob-Toolbox-0.0.2/paymob/data_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-21 10:59:04.000000 Paymob-Toolbox-0.0.2/paymob/data_classes/response_feedback_dataclass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:59:10.270818 Paymob-Toolbox-0.0.2/paymob/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-21 10:59:04.000000 Paymob-Toolbox-0.0.2/paymob/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-21 10:59:04.000000 Paymob-Toolbox-0.0.2/paymob/utils/class_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-21 10:59:04.000000 Paymob-Toolbox-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 10:59:10.270818 Paymob-Toolbox-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-21 10:59:09.000000 Paymob-Toolbox-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:59:10.270818 Paymob-Toolbox-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 10:59:04.000000 Paymob-Toolbox-0.0.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 10:59:10.270818 Paymob-Toolbox-0.0.2/tests/accept/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 10:59:04.000000 Paymob-Toolbox-0.0.2/tests/accept/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-06-21 10:59:04.000000 Paymob-Toolbox-0.0.2/tests/accept/test_accept_utils_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18188 2023-06-21 10:59:04.000000 Paymob-Toolbox-0.0.2/tests/accept/test_hmac_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-21 10:59:04.000000 Paymob-Toolbox-0.0.2/tests/utils.py
```

### Comparing `Paymob-Toolbox-0.0.1/PKG-INFO` & `Paymob-Toolbox-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Paymob-Toolbox
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple Python package that provides convenient access to the Paymob APIs from applications written in the Python language.
 Home-page: https://github.com/muhammedattif/Paymob
 Author: DjangoFam Team
 Author-email: mahmoud.nasser.abdulhamed11@gmail.com
 License: UNKNOWN
 Keywords: pypi,paymob,payment,python
 Platform: UNKNOWN
```

### Comparing `Paymob-Toolbox-0.0.1/Paymob_Toolbox.egg-info/PKG-INFO` & `Paymob-Toolbox-0.0.2/Paymob_Toolbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Paymob-Toolbox
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple Python package that provides convenient access to the Paymob APIs from applications written in the Python language.
 Home-page: https://github.com/muhammedattif/Paymob
 Author: DjangoFam Team
 Author-email: mahmoud.nasser.abdulhamed11@gmail.com
 License: UNKNOWN
 Keywords: pypi,paymob,payment,python
 Platform: UNKNOWN
```

### Comparing `Paymob-Toolbox-0.0.1/Paymob_Toolbox.egg-info/SOURCES.txt` & `Paymob-Toolbox-0.0.2/Paymob_Toolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Paymob-Toolbox-0.0.1/README.md` & `Paymob-Toolbox-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `Paymob-Toolbox-0.0.1/paymob/accept/accept_client.py` & `Paymob-Toolbox-0.0.2/paymob/accept/accept_client.py`

 * *Files identical despite different names*

### Comparing `Paymob-Toolbox-0.0.1/paymob/accept/callbacks/generic_callback.py` & `Paymob-Toolbox-0.0.2/paymob/accept/callbacks/generic_callback.py`

 * *Files identical despite different names*

### Comparing `Paymob-Toolbox-0.0.1/paymob/accept/config.py` & `Paymob-Toolbox-0.0.2/paymob/accept/config.py`

 * *Files identical despite different names*

### Comparing `Paymob-Toolbox-0.0.1/paymob/accept/connection.py` & `Paymob-Toolbox-0.0.2/paymob/accept/connection.py`

 * *Files identical despite different names*

### Comparing `Paymob-Toolbox-0.0.1/paymob/accept/constants.py` & `Paymob-Toolbox-0.0.2/paymob/accept/constants.py`

 * *Files identical despite different names*

### Comparing `Paymob-Toolbox-0.0.1/paymob/accept/data_classes/data.py` & `Paymob-Toolbox-0.0.2/paymob/accept/data_classes/data.py`

 * *Files identical despite different names*

### Comparing `Paymob-Toolbox-0.0.1/paymob/accept/data_classes/order.py` & `Paymob-Toolbox-0.0.2/paymob/accept/data_classes/order.py`

 * *Files identical despite different names*

### Comparing `Paymob-Toolbox-0.0.1/paymob/accept/data_classes/transaction.py` & `Paymob-Toolbox-0.0.2/paymob/accept/data_classes/transaction.py`

 * *Files identical despite different names*

### Comparing `Paymob-Toolbox-0.0.1/paymob/accept/hmac_validator.py` & `Paymob-Toolbox-0.0.2/paymob/accept/hmac_validator.py`

 * *Files identical despite different names*

### Comparing `Paymob-Toolbox-0.0.1/paymob/accept/transaction.py` & `Paymob-Toolbox-0.0.2/paymob/accept/transaction.py`

 * *Files identical despite different names*

### Comparing `Paymob-Toolbox-0.0.1/paymob/accept/utils.py` & `Paymob-Toolbox-0.0.2/paymob/accept/utils.py`

 * *Files identical despite different names*

### Comparing `Paymob-Toolbox-0.0.1/paymob/utils/class_factory.py` & `Paymob-Toolbox-0.0.2/paymob/utils/class_factory.py`

 * *Files identical despite different names*

### Comparing `Paymob-Toolbox-0.0.1/pyproject.toml` & `Paymob-Toolbox-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Paymob-Toolbox-0.0.1/setup.py` & `Paymob-Toolbox-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name="Paymob-Toolbox",
-    version='0.0.1',
+    version='0.0.2',
     author="DjangoFam Team",
     author_email="mahmoud.nasser.abdulhamed11@gmail.com",
     description="A simple Python package that provides convenient access to the Paymob APIs from applications written in the Python language.",
     url="https://github.com/muhammedattif/Paymob",
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
```

### Comparing `Paymob-Toolbox-0.0.1/tests/accept/test_accept_utils_class.py` & `Paymob-Toolbox-0.0.2/tests/accept/test_accept_utils_class.py`

 * *Files identical despite different names*

### Comparing `Paymob-Toolbox-0.0.1/tests/accept/test_hmac_validator.py` & `Paymob-Toolbox-0.0.2/tests/accept/test_hmac_validator.py`

 * *Files identical despite different names*

### Comparing `Paymob-Toolbox-0.0.1/tests/utils.py` & `Paymob-Toolbox-0.0.2/tests/utils.py`

 * *Files identical despite different names*

