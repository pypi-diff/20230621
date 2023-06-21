# Comparing `tmp/drfexts-1.1.5.tar.gz` & `tmp/drfexts-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drfexts-1.1.5.tar", max compression
+gzip compressed data, was "drfexts-1.1.6.tar", max compression
```

## Comparing `drfexts-1.1.5.tar` & `drfexts-1.1.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    11347 2022-08-12 03:23:59.731526 drfexts-1.1.5/LICENSE
--rw-r--r--   0        0        0     3514 2022-12-20 09:03:24.666040 drfexts-1.1.5/README.md
--rw-r--r--   0        0        0       22 2023-05-16 02:00:18.998914 drfexts-1.1.5/drfexts/__init__.py
--rw-r--r--   0        0        0      234 2022-08-31 09:46:14.033000 drfexts-1.1.5/drfexts/authentication.py
--rw-r--r--   0        0        0      773 2022-12-20 09:03:31.323137 drfexts-1.1.5/drfexts/choices.py
--rw-r--r--   0        0        0      773 2022-12-20 09:03:31.323301 drfexts-1.1.5/drfexts/constants.py
--rw-r--r--   0        0        0     1028 2022-12-20 09:03:24.666662 drfexts-1.1.5/drfexts/exceptions.py
--rw-r--r--   0        0        0    11580 2022-12-20 09:03:31.323500 drfexts-1.1.5/drfexts/fields.py
--rw-r--r--   0        0        0        0 2022-08-31 09:46:14.033000 drfexts-1.1.5/drfexts/filtersets/__init__.py
--rw-r--r--   0        0        0    13759 2023-03-14 06:41:02.737534 drfexts-1.1.5/drfexts/filtersets/backends.py
--rw-r--r--   0        0        0      964 2022-12-20 09:03:24.667627 drfexts-1.1.5/drfexts/filtersets/fields.py
--rw-r--r--   0        0        0     7174 2022-12-20 09:03:24.667894 drfexts-1.1.5/drfexts/filtersets/filters.py
--rw-r--r--   0        0        0     3156 2022-12-20 09:03:24.668112 drfexts-1.1.5/drfexts/filtersets/widgets.py
--rw-r--r--   0        0        0     6800 2022-12-20 09:03:31.324165 drfexts-1.1.5/drfexts/models.py
--rw-r--r--   0        0        0     6304 2023-02-19 06:30:29.180143 drfexts-1.1.5/drfexts/pagination.py
--rw-r--r--   0        0        0     1505 2022-12-20 09:03:24.668996 drfexts-1.1.5/drfexts/paginators.py
--rw-r--r--   0        0        0     1510 2022-12-20 09:03:24.669231 drfexts-1.1.5/drfexts/parsers.py
--rw-r--r--   0        0        0        0 2022-08-31 09:46:14.034000 drfexts-1.1.5/drfexts/permissions.py
--rw-r--r--   0        0        0    10536 2023-02-16 01:58:40.544719 drfexts-1.1.5/drfexts/renderers.py
--rw-r--r--   0        0        0      281 2022-12-20 09:03:24.669838 drfexts-1.1.5/drfexts/routers.py
--rw-r--r--   0        0        0        0 2022-08-31 09:46:14.035000 drfexts-1.1.5/drfexts/serializers/__init__.py
--rw-r--r--   0        0        0     5415 2023-02-28 07:56:13.159259 drfexts-1.1.5/drfexts/serializers/fields.py
--rw-r--r--   0        0        0     3991 2022-12-20 09:03:31.324941 drfexts-1.1.5/drfexts/serializers/mixins.py
--rw-r--r--   0        0        0      510 2023-05-16 01:59:57.760919 drfexts-1.1.5/drfexts/serializers/serializers.py
--rw-r--r--   0        0        0     1399 2022-12-20 09:03:24.671091 drfexts-1.1.5/drfexts/settings.py
--rw-r--r--   0        0        0     1018 2022-12-20 09:03:24.671352 drfexts-1.1.5/drfexts/storages.py
--rw-r--r--   0        0        0     2695 2022-12-20 09:03:31.325393 drfexts-1.1.5/drfexts/utils.py
--rw-r--r--   0        0        0     9040 2022-12-20 09:03:31.325680 drfexts-1.1.5/drfexts/viewsets.py
--rw-r--r--   0        0        0     1647 2023-05-16 02:00:19.006301 drfexts-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     4578 1970-01-01 00:00:00.000000 drfexts-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0    11347 2022-08-12 03:23:59.731526 drfexts-1.1.6/LICENSE
+-rw-r--r--   0        0        0     3514 2022-12-20 09:03:24.666040 drfexts-1.1.6/README.md
+-rw-r--r--   0        0        0       22 2023-06-21 10:04:52.411601 drfexts-1.1.6/drfexts/__init__.py
+-rw-r--r--   0        0        0      234 2022-08-31 09:46:14.033000 drfexts-1.1.6/drfexts/authentication.py
+-rw-r--r--   0        0        0      773 2022-12-20 09:03:31.323137 drfexts-1.1.6/drfexts/choices.py
+-rw-r--r--   0        0        0      773 2022-12-20 09:03:31.323301 drfexts-1.1.6/drfexts/constants.py
+-rw-r--r--   0        0        0     1028 2022-12-20 09:03:24.666662 drfexts-1.1.6/drfexts/exceptions.py
+-rw-r--r--   0        0        0    11580 2022-12-20 09:03:31.323500 drfexts-1.1.6/drfexts/fields.py
+-rw-r--r--   0        0        0        0 2022-08-31 09:46:14.033000 drfexts-1.1.6/drfexts/filtersets/__init__.py
+-rw-r--r--   0        0        0    14161 2023-06-21 10:04:36.868744 drfexts-1.1.6/drfexts/filtersets/backends.py
+-rw-r--r--   0        0        0      964 2022-12-20 09:03:24.667627 drfexts-1.1.6/drfexts/filtersets/fields.py
+-rw-r--r--   0        0        0     7174 2022-12-20 09:03:24.667894 drfexts-1.1.6/drfexts/filtersets/filters.py
+-rw-r--r--   0        0        0     3156 2022-12-20 09:03:24.668112 drfexts-1.1.6/drfexts/filtersets/widgets.py
+-rw-r--r--   0        0        0     6800 2022-12-20 09:03:31.324165 drfexts-1.1.6/drfexts/models.py
+-rw-r--r--   0        0        0     6304 2023-02-19 06:30:29.180143 drfexts-1.1.6/drfexts/pagination.py
+-rw-r--r--   0        0        0     1505 2022-12-20 09:03:24.668996 drfexts-1.1.6/drfexts/paginators.py
+-rw-r--r--   0        0        0     1510 2022-12-20 09:03:24.669231 drfexts-1.1.6/drfexts/parsers.py
+-rw-r--r--   0        0        0        0 2022-08-31 09:46:14.034000 drfexts-1.1.6/drfexts/permissions.py
+-rw-r--r--   0        0        0    10536 2023-02-16 01:58:40.544719 drfexts-1.1.6/drfexts/renderers.py
+-rw-r--r--   0        0        0      281 2022-12-20 09:03:24.669838 drfexts-1.1.6/drfexts/routers.py
+-rw-r--r--   0        0        0        0 2022-08-31 09:46:14.035000 drfexts-1.1.6/drfexts/serializers/__init__.py
+-rw-r--r--   0        0        0     5415 2023-02-28 07:56:13.159259 drfexts-1.1.6/drfexts/serializers/fields.py
+-rw-r--r--   0        0        0     3991 2022-12-20 09:03:31.324941 drfexts-1.1.6/drfexts/serializers/mixins.py
+-rw-r--r--   0        0        0      510 2023-05-16 01:59:57.760919 drfexts-1.1.6/drfexts/serializers/serializers.py
+-rw-r--r--   0        0        0     1399 2022-12-20 09:03:24.671091 drfexts-1.1.6/drfexts/settings.py
+-rw-r--r--   0        0        0     1018 2022-12-20 09:03:24.671352 drfexts-1.1.6/drfexts/storages.py
+-rw-r--r--   0        0        0     2695 2022-12-20 09:03:31.325393 drfexts-1.1.6/drfexts/utils.py
+-rw-r--r--   0        0        0     9040 2022-12-20 09:03:31.325680 drfexts-1.1.6/drfexts/viewsets.py
+-rw-r--r--   0        0        0     1647 2023-06-21 10:04:52.420205 drfexts-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0     4578 1970-01-01 00:00:00.000000 drfexts-1.1.6/PKG-INFO
```

### Comparing `drfexts-1.1.5/LICENSE` & `drfexts-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `drfexts-1.1.5/README.md` & `drfexts-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `drfexts-1.1.5/drfexts/choices.py` & `drfexts-1.1.6/drfexts/choices.py`

 * *Files identical despite different names*

### Comparing `drfexts-1.1.5/drfexts/constants.py` & `drfexts-1.1.6/drfexts/constants.py`

 * *Files identical despite different names*

### Comparing `drfexts-1.1.5/drfexts/exceptions.py` & `drfexts-1.1.6/drfexts/exceptions.py`

 * *Files identical despite different names*

### Comparing `drfexts-1.1.5/drfexts/fields.py` & `drfexts-1.1.6/drfexts/fields.py`

 * *Files identical despite different names*

### Comparing `drfexts-1.1.5/drfexts/filtersets/backends.py` & `drfexts-1.1.6/drfexts/filtersets/backends.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,14 +207,22 @@
                 kwargs = {
                     "field_name": field_name,
                     "label": field.label,
                     "help_text": field.help_text,
                 }
                 if callable(extra):
                     kwargs.update(extra(field))
+                # Fix when set custom through model for `MantToManyField`
+                if (
+                    isinstance(field, serializers.ManyRelatedField)
+                    and kwargs.get("queryset") is None
+                ):
+                    kwargs["queryset"] = getattr(
+                        field.root.Meta.model, field.source
+                    ).rel.model._default_manager.all()
 
                 if "queryset" in kwargs and kwargs["queryset"] is None:
                     logger.debug(f"{filter_name} 字段未提供queryset, 跳过自动成filter!")
                     continue
 
                 if isinstance(field, ComplexPKRelatedField) and getattr(
                     field, "display_field", None
```

### Comparing `drfexts-1.1.5/drfexts/filtersets/fields.py` & `drfexts-1.1.6/drfexts/filtersets/fields.py`

 * *Files identical despite different names*

### Comparing `drfexts-1.1.5/drfexts/filtersets/filters.py` & `drfexts-1.1.6/drfexts/filtersets/filters.py`

 * *Files identical despite different names*

### Comparing `drfexts-1.1.5/drfexts/filtersets/widgets.py` & `drfexts-1.1.6/drfexts/filtersets/widgets.py`

 * *Files identical despite different names*

### Comparing `drfexts-1.1.5/drfexts/models.py` & `drfexts-1.1.6/drfexts/models.py`

 * *Files identical despite different names*

### Comparing `drfexts-1.1.5/drfexts/pagination.py` & `drfexts-1.1.6/drfexts/pagination.py`

 * *Files identical despite different names*

### Comparing `drfexts-1.1.5/drfexts/paginators.py` & `drfexts-1.1.6/drfexts/paginators.py`

 * *Files identical despite different names*

### Comparing `drfexts-1.1.5/drfexts/parsers.py` & `drfexts-1.1.6/drfexts/parsers.py`

 * *Files identical despite different names*

### Comparing `drfexts-1.1.5/drfexts/renderers.py` & `drfexts-1.1.6/drfexts/renderers.py`

 * *Files identical despite different names*

### Comparing `drfexts-1.1.5/drfexts/serializers/fields.py` & `drfexts-1.1.6/drfexts/serializers/fields.py`

 * *Files identical despite different names*

### Comparing `drfexts-1.1.5/drfexts/serializers/mixins.py` & `drfexts-1.1.6/drfexts/serializers/mixins.py`

 * *Files identical despite different names*

### Comparing `drfexts-1.1.5/drfexts/settings.py` & `drfexts-1.1.6/drfexts/settings.py`

 * *Files identical despite different names*

### Comparing `drfexts-1.1.5/drfexts/storages.py` & `drfexts-1.1.6/drfexts/storages.py`

 * *Files identical despite different names*

### Comparing `drfexts-1.1.5/drfexts/utils.py` & `drfexts-1.1.6/drfexts/utils.py`

 * *Files identical despite different names*

### Comparing `drfexts-1.1.5/drfexts/viewsets.py` & `drfexts-1.1.6/drfexts/viewsets.py`

 * *Files identical despite different names*

### Comparing `drfexts-1.1.5/pyproject.toml` & `drfexts-1.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.commitizen]
-version = "1.1.5"
+version = "1.1.6"
 tag_format = "v$major.$minor.$patch$prerelease"
 version_files = [
     "pyproject.toml:version",
     "drfexts/__init__.py"
 ]
 
 [tool.poetry]
 name = "drfexts"
-version = "1.1.5"
+version = "1.1.6"
 readme = "README.md"
 description = "Django Restframework Utils"
 authors = ["aiden <allaher@icloud.com>"]
 keywords = ["django", "restframework"]
 homepage = "https://github.com/aiden520/drfexts"
 repository = "https://github.com/aiden520/drfexts"
 license = "Apache-2.0"
```

### Comparing `drfexts-1.1.5/PKG-INFO` & `drfexts-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drfexts
-Version: 1.1.5
+Version: 1.1.6
 Summary: Django Restframework Utils
 Home-page: https://github.com/aiden520/drfexts
 License: Apache-2.0
 Keywords: django,restframework
 Author: aiden
 Author-email: allaher@icloud.com
 Requires-Python: >=3.8,<4.0.0
```

