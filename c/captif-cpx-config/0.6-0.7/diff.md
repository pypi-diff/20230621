# Comparing `tmp/captif_cpx_config-0.6.tar.gz` & `tmp/captif_cpx_config-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "captif_cpx_config-0.6.tar", max compression
+gzip compressed data, was "captif_cpx_config-0.7.tar", max compression
```

## Comparing `captif_cpx_config-0.6.tar` & `captif_cpx_config-0.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1084 2023-06-12 00:08:10.640101 captif_cpx_config-0.6/LICENSE
--rw-r--r--   0        0        0       19 2023-06-12 00:08:10.644101 captif_cpx_config-0.6/README.md
--rw-r--r--   0        0        0       44 2023-06-12 00:08:10.644101 captif_cpx_config-0.6/captif_cpx_config/__init__.py
--rw-r--r--   0        0        0     4089 2023-06-12 00:08:10.644101 captif_cpx_config-0.6/captif_cpx_config/metadata.py
--rw-r--r--   0        0        0      522 2023-06-12 00:08:10.644101 captif_cpx_config-0.6/pyproject.toml
--rw-r--r--   0        0        0      519 1970-01-01 00:00:00.000000 captif_cpx_config-0.6/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-06-21 21:44:08.897554 captif_cpx_config-0.7/LICENSE
+-rw-r--r--   0        0        0       19 2023-06-21 21:44:08.897554 captif_cpx_config-0.7/README.md
+-rw-r--r--   0        0        0       44 2023-06-21 21:44:08.897554 captif_cpx_config-0.7/captif_cpx_config/__init__.py
+-rw-r--r--   0        0        0     4153 2023-06-21 21:44:08.897554 captif_cpx_config-0.7/captif_cpx_config/metadata.py
+-rw-r--r--   0        0        0      522 2023-06-21 21:44:08.897554 captif_cpx_config-0.7/pyproject.toml
+-rw-r--r--   0        0        0      519 1970-01-01 00:00:00.000000 captif_cpx_config-0.7/PKG-INFO
```

### Comparing `captif_cpx_config-0.6/LICENSE` & `captif_cpx_config-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `captif_cpx_config-0.6/captif_cpx_config/metadata.py` & `captif_cpx_config-0.7/captif_cpx_config/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,21 +4,23 @@
 from pydantic import BaseModel, Field, condecimal
 
 
 class MicrophoneDetails(BaseModel):
     microphone_position: int = Field(
         description="microphone position (1-6) as per ISO 11819-2:2017",
     )
-    microphone_serial_number: str = Field(
+    microphone_serial_number: Optional[str] = Field(
+        default=None,
         description="microphone serial number",
     )
     microphone_sensitivity_mv_pa: condecimal(decimal_places=2) = Field(
         description="microphone sensitivity in mV/Pa",
     )
-    microphone_calibration_date: date_ = Field(
+    microphone_calibration_date: Optional[date_] = Field(
+        default=None,
         description="microphone calibration date",
     )
     wav_file_channel_number: int = Field(
         description=(
             "channel number in the wav file corresponding to the microphone "
             "position. The channels number uses zero-based indexing."
         ),
```

### Comparing `captif_cpx_config-0.6/pyproject.toml` & `captif_cpx_config-0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "captif-cpx-config"
-version = "0.6"
+version = "0.7"
 description = ""
 authors = ["John Bull <john.bull@nzta.govt.nz>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "captif_cpx_config"}]
 
 [tool.poetry.dependencies]
@@ -14,12 +14,12 @@
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 pytest-cov = "^4.1.0"
 pytest-randomly = "^3.12.0"
 black = "^23.3.0"
 flake8 = "^6.0.0"
-captif-cpx-db = ">=0.7"
+captif-cpx-db = ">=0.8"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `captif_cpx_config-0.6/PKG-INFO` & `captif_cpx_config-0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: captif-cpx-config
-Version: 0.6
+Version: 0.7
 Summary: 
 License: MIT
 Author: John Bull
 Author-email: john.bull@nzta.govt.nz
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

