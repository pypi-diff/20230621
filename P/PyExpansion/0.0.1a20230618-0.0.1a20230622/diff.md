# Comparing `tmp/PyExpansion-0.0.1a20230618.tar.gz` & `tmp/PyExpansion-0.0.1a20230622.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyExpansion-0.0.1a20230618.tar", last modified: Sun Jun 18 16:09:54 2023, max compression
+gzip compressed data, was "PyExpansion-0.0.1a20230622.tar", last modified: Wed Jun 21 17:26:17 2023, max compression
```

## Comparing `PyExpansion-0.0.1a20230618.tar` & `PyExpansion-0.0.1a20230622.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 16:09:54.779796 PyExpansion-0.0.1a20230618/
--rw-rw-rw-   0        0        0     1081 2023-06-17 07:28:57.000000 PyExpansion-0.0.1a20230618/LICENSE.txt
--rw-rw-rw-   0        0        0        0 2023-06-17 09:17:44.000000 PyExpansion-0.0.1a20230618/MANIFEST.in
--rw-rw-rw-   0        0        0      116 2023-06-18 16:09:54.777788 PyExpansion-0.0.1a20230618/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-18 16:09:54.650125 PyExpansion-0.0.1a20230618/PyExpansion/
--rw-rw-rw-   0        0        0        0 2023-06-05 07:29:27.000000 PyExpansion-0.0.1a20230618/PyExpansion/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-18 16:09:54.675058 PyExpansion-0.0.1a20230618/PyExpansion/application/
-drwxrwxrwx   0        0        0        0 2023-06-18 16:09:54.697996 PyExpansion-0.0.1a20230618/PyExpansion/application/PyIC/
--rw-rw-rw-   0        0        0        0 2023-06-17 03:59:05.000000 PyExpansion-0.0.1a20230618/PyExpansion/application/PyIC/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-18 16:09:54.712957 PyExpansion-0.0.1a20230618/PyExpansion/application/PyIC/country/
--rw-rw-rw-   0        0        0        0 2023-06-17 06:05:34.000000 PyExpansion-0.0.1a20230618/PyExpansion/application/PyIC/country/__init__.py
--rw-rw-rw-   0        0        0     1628 2023-06-18 09:14:26.000000 PyExpansion-0.0.1a20230618/PyExpansion/application/PyIC/country/base.py
--rw-rw-rw-   0        0        0     8558 2023-06-18 09:14:27.000000 PyExpansion-0.0.1a20230618/PyExpansion/application/PyIC/country/malaysia.py
--rw-rw-rw-   0        0        0      912 2023-06-18 09:14:27.000000 PyExpansion-0.0.1a20230618/PyExpansion/application/PyIC/main.py
--rw-rw-rw-   0        0        0      544 2023-06-18 08:32:21.000000 PyExpansion-0.0.1a20230618/PyExpansion/application/PyIC/status_code_list.py
--rw-rw-rw-   0        0        0     1379 2023-06-18 09:14:26.000000 PyExpansion-0.0.1a20230618/PyExpansion/application/PyIC/tests.py
--rw-rw-rw-   0        0        0      473 2023-06-18 15:13:16.000000 PyExpansion-0.0.1a20230618/PyExpansion/application/PyIC/version.py
--rw-rw-rw-   0        0        0        0 2023-06-17 09:22:08.000000 PyExpansion-0.0.1a20230618/PyExpansion/application/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-18 16:09:54.745882 PyExpansion-0.0.1a20230618/PyExpansion/common/
--rw-rw-rw-   0        0        0        0 2023-06-17 09:35:58.000000 PyExpansion-0.0.1a20230618/PyExpansion/common/__init__.py
--rw-rw-rw-   0        0        0      144 2023-06-18 10:34:10.000000 PyExpansion-0.0.1a20230618/PyExpansion/common/basic_function.py
-drwxrwxrwx   0        0        0        0 2023-06-18 16:09:54.750855 PyExpansion-0.0.1a20230618/PyExpansion/common/data_type/
--rw-rw-rw-   0        0        0        0 2023-06-18 07:42:28.000000 PyExpansion-0.0.1a20230618/PyExpansion/common/data_type/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-18 16:09:54.771807 PyExpansion-0.0.1a20230618/PyExpansion/common/data_type/lists/
--rw-rw-rw-   0        0        0        0 2023-06-18 08:46:51.000000 PyExpansion-0.0.1a20230618/PyExpansion/common/data_type/lists/__init__.py
--rw-rw-rw-   0        0        0      464 2023-06-18 09:06:26.000000 PyExpansion-0.0.1a20230618/PyExpansion/common/data_type/lists/main.py
--rw-rw-rw-   0        0        0      327 2023-06-18 09:06:26.000000 PyExpansion-0.0.1a20230618/PyExpansion/common/data_type/lists/status_code_list.py
--rw-rw-rw-   0        0        0      395 2023-06-18 09:13:12.000000 PyExpansion-0.0.1a20230618/PyExpansion/common/data_type/lists/tests.py
--rw-rw-rw-   0        0        0     1166 2023-06-18 09:13:12.000000 PyExpansion-0.0.1a20230618/PyExpansion/common/message.py
--rw-rw-rw-   0        0        0      532 2023-06-18 16:08:44.000000 PyExpansion-0.0.1a20230618/PyExpansion/common/status_code_list.py
--rw-rw-rw-   0        0        0     1069 2023-06-18 08:38:41.000000 PyExpansion-0.0.1a20230618/PyExpansion/common/utils.py
--rw-rw-rw-   0        0        0     2532 2023-06-18 15:13:08.000000 PyExpansion-0.0.1a20230618/PyExpansion/common/version_history.py
--rw-rw-rw-   0        0        0       28 2023-06-17 09:42:46.000000 PyExpansion-0.0.1a20230618/PyExpansion/version.py
-drwxrwxrwx   0        0        0        0 2023-06-18 16:09:54.670071 PyExpansion-0.0.1a20230618/PyExpansion.egg-info/
--rw-rw-rw-   0        0        0      116 2023-06-18 16:09:54.000000 PyExpansion-0.0.1a20230618/PyExpansion.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1046 2023-06-18 16:09:54.000000 PyExpansion-0.0.1a20230618/PyExpansion.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 16:09:54.000000 PyExpansion-0.0.1a20230618/PyExpansion.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-18 16:09:54.000000 PyExpansion-0.0.1a20230618/PyExpansion.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      297 2023-06-18 16:08:44.000000 PyExpansion-0.0.1a20230618/README.md
--rw-rw-rw-   0        0        0       42 2023-06-18 16:09:54.780775 PyExpansion-0.0.1a20230618/setup.cfg
--rw-rw-rw-   0        0        0      300 2023-06-18 09:14:26.000000 PyExpansion-0.0.1a20230618/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 17:26:17.101498 PyExpansion-0.0.1a20230622/
+-rw-rw-rw-   0        0        0     1081 2023-06-17 07:28:57.000000 PyExpansion-0.0.1a20230622/LICENSE.txt
+-rw-rw-rw-   0        0        0        0 2023-06-17 09:17:44.000000 PyExpansion-0.0.1a20230622/MANIFEST.in
+-rw-rw-rw-   0        0        0     1141 2023-06-21 17:26:17.101498 PyExpansion-0.0.1a20230622/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-21 17:26:16.992141 PyExpansion-0.0.1a20230622/PyExpansion/
+-rw-rw-rw-   0        0        0        0 2023-06-05 07:29:27.000000 PyExpansion-0.0.1a20230622/PyExpansion/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 17:26:17.023391 PyExpansion-0.0.1a20230622/PyExpansion/application/
+drwxrwxrwx   0        0        0        0 2023-06-21 17:26:17.039012 PyExpansion-0.0.1a20230622/PyExpansion/application/PyIC/
+-rw-rw-rw-   0        0        0        0 2023-06-17 03:59:05.000000 PyExpansion-0.0.1a20230622/PyExpansion/application/PyIC/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 17:26:17.054633 PyExpansion-0.0.1a20230622/PyExpansion/application/PyIC/country/
+-rw-rw-rw-   0        0        0     8513 2023-06-21 15:35:07.000000 PyExpansion-0.0.1a20230622/PyExpansion/application/PyIC/country/Malaysia.py
+-rw-rw-rw-   0        0        0     2899 2023-06-21 16:10:29.000000 PyExpansion-0.0.1a20230622/PyExpansion/application/PyIC/country/Singapore.py
+-rw-rw-rw-   0        0        0        0 2023-06-17 06:05:34.000000 PyExpansion-0.0.1a20230622/PyExpansion/application/PyIC/country/__init__.py
+-rw-rw-rw-   0        0        0     1654 2023-06-21 15:48:39.000000 PyExpansion-0.0.1a20230622/PyExpansion/application/PyIC/country/base.py
+-rw-rw-rw-   0        0        0     1016 2023-06-21 15:31:03.000000 PyExpansion-0.0.1a20230622/PyExpansion/application/PyIC/main.py
+-rw-rw-rw-   0        0        0      621 2023-06-21 16:51:40.000000 PyExpansion-0.0.1a20230622/PyExpansion/application/PyIC/status_code_list.py
+-rw-rw-rw-   0        0        0     1760 2023-06-21 16:53:12.000000 PyExpansion-0.0.1a20230622/PyExpansion/application/PyIC/tests.py
+-rw-rw-rw-   0        0        0      473 2023-06-18 15:13:16.000000 PyExpansion-0.0.1a20230622/PyExpansion/application/PyIC/version.py
+-rw-rw-rw-   0        0        0        0 2023-06-17 09:22:08.000000 PyExpansion-0.0.1a20230622/PyExpansion/application/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 17:26:17.085878 PyExpansion-0.0.1a20230622/PyExpansion/common/
+-rw-rw-rw-   0        0        0        0 2023-06-17 09:35:58.000000 PyExpansion-0.0.1a20230622/PyExpansion/common/__init__.py
+-rw-rw-rw-   0        0        0      144 2023-06-18 10:34:10.000000 PyExpansion-0.0.1a20230622/PyExpansion/common/basic_function.py
+drwxrwxrwx   0        0        0        0 2023-06-21 17:26:17.085878 PyExpansion-0.0.1a20230622/PyExpansion/common/data_type/
+-rw-rw-rw-   0        0        0        0 2023-06-18 07:42:28.000000 PyExpansion-0.0.1a20230622/PyExpansion/common/data_type/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 17:26:17.101498 PyExpansion-0.0.1a20230622/PyExpansion/common/data_type/lists/
+-rw-rw-rw-   0        0        0        0 2023-06-18 08:46:51.000000 PyExpansion-0.0.1a20230622/PyExpansion/common/data_type/lists/__init__.py
+-rw-rw-rw-   0        0        0      464 2023-06-18 09:06:26.000000 PyExpansion-0.0.1a20230622/PyExpansion/common/data_type/lists/main.py
+-rw-rw-rw-   0        0        0      327 2023-06-18 09:06:26.000000 PyExpansion-0.0.1a20230622/PyExpansion/common/data_type/lists/status_code_list.py
+-rw-rw-rw-   0        0        0      395 2023-06-18 09:13:12.000000 PyExpansion-0.0.1a20230622/PyExpansion/common/data_type/lists/tests.py
+-rw-rw-rw-   0        0        0     1166 2023-06-18 09:13:12.000000 PyExpansion-0.0.1a20230622/PyExpansion/common/message.py
+-rw-rw-rw-   0        0        0      532 2023-06-18 16:08:44.000000 PyExpansion-0.0.1a20230622/PyExpansion/common/status_code_list.py
+-rw-rw-rw-   0        0        0     1069 2023-06-18 08:38:41.000000 PyExpansion-0.0.1a20230622/PyExpansion/common/utils.py
+-rw-rw-rw-   0        0        0     2532 2023-06-18 15:13:08.000000 PyExpansion-0.0.1a20230622/PyExpansion/common/version_history.py
+-rw-rw-rw-   0        0        0       28 2023-06-21 16:56:25.000000 PyExpansion-0.0.1a20230622/PyExpansion/version.py
+drwxrwxrwx   0        0        0        0 2023-06-21 17:26:17.007766 PyExpansion-0.0.1a20230622/PyExpansion.egg-info/
+-rw-rw-rw-   0        0        0     1141 2023-06-21 17:26:16.000000 PyExpansion-0.0.1a20230622/PyExpansion.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1145 2023-06-21 17:26:16.000000 PyExpansion-0.0.1a20230622/PyExpansion.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 17:26:16.000000 PyExpansion-0.0.1a20230622/PyExpansion.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-21 17:26:16.000000 PyExpansion-0.0.1a20230622/PyExpansion.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      980 2023-06-21 17:09:08.000000 PyExpansion-0.0.1a20230622/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-21 17:26:17.101498 PyExpansion-0.0.1a20230622/setup.cfg
+-rw-rw-rw-   0        0        0      522 2023-06-21 17:16:35.000000 PyExpansion-0.0.1a20230622/setup.py
```

### Comparing `PyExpansion-0.0.1a20230618/LICENSE.txt` & `PyExpansion-0.0.1a20230622/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyExpansion-0.0.1a20230618/PyExpansion/application/PyIC/country/malaysia.py` & `PyExpansion-0.0.1a20230622/PyExpansion/application/PyIC/country/Malaysia.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,18 @@
 from PyExpansion.common import message
 from PyExpansion.application.PyIC.country import base
 from PyExpansion.application.PyIC import status_code_list
 
 
 class PyIC(base.PyICBase):
     country = "Malaysia"
-    ic_length = 12
-    separator = "-"
-    max_length_after_separator = 3
+    ic_pattern = "############"
 
     """
-    YYMMDD-PB-###G
+    YYMMDD PB ###G
 
     YY  - last 2 number of the year of birth
     MM  - number of month of birth
     DD  - number of day of birth
     PB  - place of birth
     ### - generic special number generated by the National Registration Department of Malaysia's computer system
     G   - Gender of person, odd number is male, even number is female  
@@ -124,34 +122,35 @@
         "98": "Stateless / Stateless Person Article 1/1954",
         "99": "Mecca / Neutral Zone / No Information / Refugee / Refugee Article 1/1951 / United Nations Specialized Agency / United Nations Organization / Unspecified Nationality",
     }
 
     def get_detail(self):
         flag = True
         if not self.get_info():
-            return message.error_default_message(True)
+            return message.error_default_message(False)
         else:
             temp = self.get_info()
             birthday = temp[:6]
             pb_code = temp[6:8]
-            gender = temp[self.ic_length-1]
+            gender = temp[len(temp)-1]
 
         try:
             birthday = datetime.strptime(birthday, '%y%m%d').date()
             self.correct_code = status_code_list.correct_code
         except:
             flag = False
             self.error_code = status_code_list.error_code_M_1
+
         states = self.pb_code_list[pb_code]
         gender = "Male" if int(gender) % 2 == 1 else "Female"
 
         if flag:
             return {"birthday": birthday, "states": states, "gender": gender, "error": False}
         else:
-            return message.error_default_message(True)
+            return message.error_default_message(False)
 
     def get_birthday(self):
         return self.get_detail()["birthday"]
 
     def get_states(self):
         return self.get_detail()["states"]
```

### Comparing `PyExpansion-0.0.1a20230618/PyExpansion/application/PyIC/tests.py` & `PyExpansion-0.0.1a20230622/PyExpansion/application/PyIC/tests.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,55 @@
 from PyExpansion.application.PyIC import main
 
 test_case_material = [
     {
-       "country": "M",
-       "ic_word": "123456478",
-       "test_condition": "Invalid Country",
-       "special": "",
+        "country": "M",
+        "ic_word": "123456478",
+        "test_condition": "Invalid Country",
+        "special": "",
     },
     {
-       "country": "Malaysia",
-       "ic_word": "001112108790",
-       "test_condition": "Correct Case",
-       "special": "",
+        "country": "Malaysia",
+        "ic_word": "001112108790",
+        "test_condition": "Correct Case",
+        "special": "",
     },
     {
-       "country": "Malaysia",
-       "ic_word": "00111108790",
-       "test_condition": "IC length is not correct",
-       "special": "only apply to the country that have ic length validation",
+        "country": "Malaysia",
+        "ic_word": "00111108790",
+        "test_condition": "IC length is not correct",
+        "special": "only apply to the country that have ic length validation",
     },
     {
-       "country": "Malaysia",
-       "ic_word": "001112-108790",
-       "test_condition": "Format IC Invalid",
-       "special": "only apply to the country that have ic pattern validation",
+        "country": "Malaysia",
+        "ic_word": "001112-108790",
+        "test_condition": "Format IC Invalid",
+        "special": "only apply to the country that have ic pattern validation",
     },
     {
         "country": "Malaysia",
         "ic_word": "001512108790",
         "test_condition": "Format Date Invalid",
         "special": "only apply to the country that have date validation",
     },
+    {
+        "country": "Singapore",
+        "ic_word": "S1234567K",
+        "test_condition": "Correct Case",
+        "special": "",
+    },
 ]
 
 for count, x in enumerate(test_case_material, start=1):
     try:
         del test_case
     except NameError:
         pass
+    print("Test Condition: ", x["test_condition"])
     test_case = main.PyIC(x["country"], x["ic_word"])
-    print("Case %s: " % str(count), test_case.get_detail())
+    print("Case %s (sample: %s): " % (str(count), x["ic_word"]), test_case.get_detail())
     print("Error Check Case %s: " % str(count), test_case.check_error())
-    if x["special"]:
-        print("This function ", x["special"])
+    if x.get("special", ""):
+        print("This function", x["special"])
+    if x["country"] == "Singapore":
+        print("Is Valid: ", main.Singapore.PyIC(x["ic_word"]).valid_ic())
+    print("\n")
```

### Comparing `PyExpansion-0.0.1a20230618/PyExpansion/common/message.py` & `PyExpansion-0.0.1a20230622/PyExpansion/common/message.py`

 * *Files identical despite different names*

### Comparing `PyExpansion-0.0.1a20230618/PyExpansion/common/status_code_list.py` & `PyExpansion-0.0.1a20230622/PyExpansion/common/status_code_list.py`

 * *Files identical despite different names*

### Comparing `PyExpansion-0.0.1a20230618/PyExpansion/common/utils.py` & `PyExpansion-0.0.1a20230622/PyExpansion/common/utils.py`

 * *Files identical despite different names*

### Comparing `PyExpansion-0.0.1a20230618/PyExpansion/common/version_history.py` & `PyExpansion-0.0.1a20230622/PyExpansion/common/version_history.py`

 * *Files identical despite different names*

### Comparing `PyExpansion-0.0.1a20230618/PyExpansion.egg-info/SOURCES.txt` & `PyExpansion-0.0.1a20230622/PyExpansion.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 PyExpansion.egg-info/top_level.txt
 PyExpansion/application/__init__.py
 PyExpansion/application/PyIC/__init__.py
 PyExpansion/application/PyIC/main.py
 PyExpansion/application/PyIC/status_code_list.py
 PyExpansion/application/PyIC/tests.py
 PyExpansion/application/PyIC/version.py
+PyExpansion/application/PyIC/country/Malaysia.py
+PyExpansion/application/PyIC/country/Singapore.py
 PyExpansion/application/PyIC/country/__init__.py
 PyExpansion/application/PyIC/country/base.py
 PyExpansion/application/PyIC/country/malaysia.py
 PyExpansion/common/__init__.py
 PyExpansion/common/basic_function.py
 PyExpansion/common/message.py
 PyExpansion/common/status_code_list.py
```

