# Comparing `tmp/hyko_sdk-0.1.5.tar.gz` & `tmp/hyko_sdk-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyko_sdk-0.1.5.tar", last modified: Wed Jun 21 08:49:37 2023, max compression
+gzip compressed data, was "hyko_sdk-0.1.6.tar", last modified: Wed Jun 21 11:40:16 2023, max compression
```

## Comparing `hyko_sdk-0.1.5.tar` & `hyko_sdk-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-06-21 08:49:37.353699 hyko_sdk-0.1.5/
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      161 2023-06-21 08:49:37.353699 hyko_sdk-0.1.5/PKG-INFO
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      411 2023-05-19 16:11:29.000000 hyko_sdk-0.1.5/README.md
-drwxr-xr-x   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-06-21 08:49:37.353699 hyko_sdk-0.1.5/hyko_sdk/
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)       40 2023-06-21 08:40:10.000000 hyko_sdk-0.1.5/hyko_sdk/__init__.py
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)     2734 2023-06-21 07:53:26.000000 hyko_sdk-0.1.5/hyko_sdk/io.py
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)     1757 2023-06-21 08:47:47.000000 hyko_sdk-0.1.5/hyko_sdk/metadata.py
-drwxr-xr-x   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-06-21 08:49:37.353699 hyko_sdk-0.1.5/hyko_sdk.egg-info/
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      161 2023-06-21 08:49:37.000000 hyko_sdk-0.1.5/hyko_sdk.egg-info/PKG-INFO
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      250 2023-06-21 08:49:37.000000 hyko_sdk-0.1.5/hyko_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)        1 2023-06-21 08:49:37.000000 hyko_sdk-0.1.5/hyko_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)        9 2023-06-21 08:49:37.000000 hyko_sdk-0.1.5/hyko_sdk.egg-info/requires.txt
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)        9 2023-06-21 08:49:37.000000 hyko_sdk-0.1.5/hyko_sdk.egg-info/top_level.txt
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)       80 2023-06-21 08:15:38.000000 hyko_sdk-0.1.5/pyproject.toml
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      296 2023-06-21 08:49:37.353699 hyko_sdk-0.1.5/setup.cfg
+drwxrwxr-x   0 crptx     (1000) crptx     (1000)        0 2023-06-21 11:40:16.723916 hyko_sdk-0.1.6/
+-rw-rw-r--   0 crptx     (1000) crptx     (1000)      192 2023-06-21 11:40:16.723916 hyko_sdk-0.1.6/PKG-INFO
+-rw-rw-r--   0 crptx     (1000) crptx     (1000)      411 2023-05-17 08:56:51.000000 hyko_sdk-0.1.6/README.md
+drwxrwxr-x   0 crptx     (1000) crptx     (1000)        0 2023-06-21 11:40:16.723916 hyko_sdk-0.1.6/hyko_sdk/
+-rw-rw-r--   0 crptx     (1000) crptx     (1000)       40 2023-06-21 11:17:29.000000 hyko_sdk-0.1.6/hyko_sdk/__init__.py
+-rw-rw-r--   0 crptx     (1000) crptx     (1000)     2995 2023-06-21 11:24:07.000000 hyko_sdk-0.1.6/hyko_sdk/io.py
+-rw-rw-r--   0 crptx     (1000) crptx     (1000)     2772 2023-06-21 11:24:49.000000 hyko_sdk-0.1.6/hyko_sdk/metadata.py
+drwxrwxr-x   0 crptx     (1000) crptx     (1000)        0 2023-06-21 11:40:16.723916 hyko_sdk-0.1.6/hyko_sdk.egg-info/
+-rw-rw-r--   0 crptx     (1000) crptx     (1000)      192 2023-06-21 11:40:16.000000 hyko_sdk-0.1.6/hyko_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 crptx     (1000) crptx     (1000)      250 2023-06-21 11:40:16.000000 hyko_sdk-0.1.6/hyko_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 crptx     (1000) crptx     (1000)        1 2023-06-21 11:40:16.000000 hyko_sdk-0.1.6/hyko_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 crptx     (1000) crptx     (1000)        9 2023-06-21 11:40:16.000000 hyko_sdk-0.1.6/hyko_sdk.egg-info/requires.txt
+-rw-rw-r--   0 crptx     (1000) crptx     (1000)        9 2023-06-21 11:40:16.000000 hyko_sdk-0.1.6/hyko_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 crptx     (1000) crptx     (1000)       80 2023-06-21 11:17:29.000000 hyko_sdk-0.1.6/pyproject.toml
+-rw-rw-r--   0 crptx     (1000) crptx     (1000)      327 2023-06-21 11:40:16.723916 hyko_sdk-0.1.6/setup.cfg
```

### Comparing `hyko_sdk-0.1.5/hyko_sdk/io.py` & `hyko_sdk-0.1.6/hyko_sdk/io.py`

 * *Files 18% similar despite different names*

```diff
@@ -81,14 +81,15 @@
     @classmethod
     def __modify_schema__(
         cls,
         field_schema: Dict[str, Any],
         field: Optional[ModelField],
     ):
         if field:
+            field_schema["type"] = "string"
             field_schema["format"] = "image"
 
 
 class Audio(str):
 
     @classmethod
     def __get_validators__(cls) -> Generator[Callable, None, None]:
@@ -101,24 +102,30 @@
     @classmethod
     def __modify_schema__(
         cls,
         field_schema: Dict[str, Any],
         field: Optional[ModelField],
     ):
         if field:
+            field_schema["type"] = "string"
             field_schema["format"] = "audio"
 
 
 # Keep the same
 class IOPortType(str, Enum):
     NUMBER = "number"
     INTEGER = "integer"
     STRING = "string"
     IMAGE = "image"
     AUDIO = "audio"
+    ARRAY_NUMBER = "array[number]"
+    ARRAY_INTEGER = "array[integer]"
+    ARRAY_STRING = "array[string]"
+    ARRAY_IMAGE = "array[image]"
+    ARRAY_AUDIO = "array[audio]"
 
 class IOPort(BaseModel):
     name: str
     description: Optional[str]
     type: IOPortType
     required: bool
     default: Optional[float | int | str]
```

