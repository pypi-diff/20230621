# Comparing `tmp/captif_cpx_db-0.7.tar.gz` & `tmp/captif_cpx_db-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "captif_cpx_db-0.7.tar", max compression
+gzip compressed data, was "captif_cpx_db-0.8.tar", max compression
```

## Comparing `captif_cpx_db-0.7.tar` & `captif_cpx_db-0.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1084 2023-06-12 00:05:09.043789 captif_cpx_db-0.7/LICENSE
--rw-r--r--   0        0        0       16 2023-06-12 00:05:09.043789 captif_cpx_db-0.7/README.md
--rw-r--r--   0        0        0       20 2023-06-12 00:05:09.043789 captif_cpx_db-0.7/captif_cpx_db/__init__.py
--rw-r--r--   0        0        0    26968 2023-06-12 00:05:09.043789 captif_cpx_db-0.7/captif_cpx_db/models.py
--rw-r--r--   0        0        0      504 2023-06-12 00:05:09.043789 captif_cpx_db-0.7/pyproject.toml
--rw-r--r--   0        0        0      494 1970-01-01 00:00:00.000000 captif_cpx_db-0.7/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-06-21 21:39:41.054948 captif_cpx_db-0.8/LICENSE
+-rw-r--r--   0        0        0       16 2023-06-21 21:39:41.054948 captif_cpx_db-0.8/README.md
+-rw-r--r--   0        0        0       20 2023-06-21 21:39:41.054948 captif_cpx_db-0.8/captif_cpx_db/__init__.py
+-rw-r--r--   0        0        0    27030 2023-06-21 21:39:41.058948 captif_cpx_db-0.8/captif_cpx_db/models.py
+-rw-r--r--   0        0        0      504 2023-06-21 21:39:41.058948 captif_cpx_db-0.8/pyproject.toml
+-rw-r--r--   0        0        0      494 1970-01-01 00:00:00.000000 captif_cpx_db-0.8/PKG-INFO
```

### Comparing `captif_cpx_db-0.7/LICENSE` & `captif_cpx_db-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `captif_cpx_db-0.7/captif_cpx_db/models.py` & `captif_cpx_db-0.8/captif_cpx_db/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,24 +150,26 @@
         default=None,
         primary_key=True,
     )
     microphone_position: int = Field(
         primary_key=True,
         description="microphone position (1-6) as per ISO 11819-2:2017",
     )
-    microphone_serial_number: str = Field(
-        nullable=False,
+    microphone_serial_number: Optional[str] = Field(
+        default=None,
+        nullable=True,
         description="microphone serial number",
     )
     microphone_sensitivity_mv_pa: condecimal(decimal_places=2) = Field(
         nullable=False,
         description="microphone sensitivity in mV/Pa",
     )
-    microphone_calibration_date: date_ = Field(
-        nullable=False,
+    microphone_calibration_date: Optional[date_] = Field(
+        default=None,
+        nullable=True,
         description="microphone calibration date",
     )
     wav_file_channel_number: int = Field(
         nullable=False,
         description=(
             "channel number in the wav file corresponding to the microphone " "position"
         ),
```

