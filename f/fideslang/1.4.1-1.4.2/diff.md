# Comparing `tmp/fideslang-1.4.1.tar.gz` & `tmp/fideslang-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fideslang-1.4.1.tar", last modified: Wed Jun  7 19:00:34 2023, max compression
+gzip compressed data, was "fideslang-1.4.2.tar", last modified: Wed Jun 21 21:18:36 2023, max compression
```

## Comparing `fideslang-1.4.1.tar` & `fideslang-1.4.2.tar`

### file list

```diff
@@ -1,36 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:00:34.811407 fideslang-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    18656 2023-06-07 19:00:29.000000 fideslang-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-07 19:00:29.000000 fideslang-1.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-06-07 19:00:34.811407 fideslang-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-06-07 19:00:29.000000 fideslang-1.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-07 19:00:29.000000 fideslang-1.4.1/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-06-07 19:00:29.000000 fideslang-1.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-07 19:00:29.000000 fideslang-1.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-07 19:00:34.811407 fideslang-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-07 19:00:29.000000 fideslang-1.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:00:34.807407 fideslang-1.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:00:34.811407 fideslang-1.4.1/src/fideslang/
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-07 19:00:29.000000 fideslang-1.4.1/src/fideslang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-07 19:00:34.811407 fideslang-1.4.1/src/fideslang/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    12917 2023-06-07 19:00:29.000000 fideslang-1.4.1/src/fideslang/default_fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:00:34.811407 fideslang-1.4.1/src/fideslang/default_taxonomy/
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-07 19:00:29.000000 fideslang-1.4.1/src/fideslang/default_taxonomy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15437 2023-06-07 19:00:29.000000 fideslang-1.4.1/src/fideslang/default_taxonomy/data_categories.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-06-07 19:00:29.000000 fideslang-1.4.1/src/fideslang/default_taxonomy/data_qualifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-06-07 19:00:29.000000 fideslang-1.4.1/src/fideslang/default_taxonomy/data_subjects.py
--rw-r--r--   0 runner    (1001) docker     (123)    14996 2023-06-07 19:00:29.000000 fideslang-1.4.1/src/fideslang/default_taxonomy/data_uses.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-07 19:00:29.000000 fideslang-1.4.1/src/fideslang/default_taxonomy/organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-06-07 19:00:29.000000 fideslang-1.4.1/src/fideslang/manifests.py
--rw-r--r--   0 runner    (1001) docker     (123)    34869 2023-06-07 19:00:29.000000 fideslang-1.4.1/src/fideslang/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-07 19:00:29.000000 fideslang-1.4.1/src/fideslang/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:00:29.000000 fideslang-1.4.1/src/fideslang/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-06-07 19:00:29.000000 fideslang-1.4.1/src/fideslang/relationships.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-07 19:00:29.000000 fideslang-1.4.1/src/fideslang/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-06-07 19:00:29.000000 fideslang-1.4.1/src/fideslang/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:00:34.811407 fideslang-1.4.1/src/fideslang.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-06-07 19:00:34.000000 fideslang-1.4.1/src/fideslang.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-07 19:00:34.000000 fideslang-1.4.1/src/fideslang.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 19:00:34.000000 fideslang-1.4.1/src/fideslang.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-07 19:00:34.000000 fideslang-1.4.1/src/fideslang.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-07 19:00:34.000000 fideslang-1.4.1/src/fideslang.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    57971 2023-06-07 19:00:29.000000 fideslang-1.4.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:18:36.364539 fideslang-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    18656 2023-06-21 21:18:17.000000 fideslang-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-21 21:18:17.000000 fideslang-1.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-06-21 21:18:36.364539 fideslang-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-06-21 21:18:17.000000 fideslang-1.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-21 21:18:17.000000 fideslang-1.4.2/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-06-21 21:18:17.000000 fideslang-1.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-21 21:18:17.000000 fideslang-1.4.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-21 21:18:36.364539 fideslang-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-21 21:18:17.000000 fideslang-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:18:36.360539 fideslang-1.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:18:36.364539 fideslang-1.4.2/src/fideslang/
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-21 21:18:17.000000 fideslang-1.4.2/src/fideslang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-21 21:18:36.364539 fideslang-1.4.2/src/fideslang/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12917 2023-06-21 21:18:17.000000 fideslang-1.4.2/src/fideslang/default_fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:18:36.364539 fideslang-1.4.2/src/fideslang/default_taxonomy/
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-21 21:18:17.000000 fideslang-1.4.2/src/fideslang/default_taxonomy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15437 2023-06-21 21:18:17.000000 fideslang-1.4.2/src/fideslang/default_taxonomy/data_categories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-06-21 21:18:17.000000 fideslang-1.4.2/src/fideslang/default_taxonomy/data_qualifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-06-21 21:18:17.000000 fideslang-1.4.2/src/fideslang/default_taxonomy/data_subjects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14996 2023-06-21 21:18:17.000000 fideslang-1.4.2/src/fideslang/default_taxonomy/data_uses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-21 21:18:17.000000 fideslang-1.4.2/src/fideslang/default_taxonomy/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-06-21 21:18:17.000000 fideslang-1.4.2/src/fideslang/manifests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35159 2023-06-21 21:18:17.000000 fideslang-1.4.2/src/fideslang/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-21 21:18:17.000000 fideslang-1.4.2/src/fideslang/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 21:18:17.000000 fideslang-1.4.2/src/fideslang/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-06-21 21:18:17.000000 fideslang-1.4.2/src/fideslang/relationships.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-21 21:18:17.000000 fideslang-1.4.2/src/fideslang/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-06-21 21:18:17.000000 fideslang-1.4.2/src/fideslang/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:18:36.364539 fideslang-1.4.2/src/fideslang.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-06-21 21:18:36.000000 fideslang-1.4.2/src/fideslang.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-21 21:18:36.000000 fideslang-1.4.2/src/fideslang.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 21:18:36.000000 fideslang-1.4.2/src/fideslang.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-21 21:18:36.000000 fideslang-1.4.2/src/fideslang.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-21 21:18:36.000000 fideslang-1.4.2/src/fideslang.egg-info/top_level.txt
```

### Comparing `fideslang-1.4.1/LICENSE` & `fideslang-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fideslang-1.4.1/PKG-INFO` & `fideslang-1.4.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: fideslang
-Version: 1.4.1
+Version: 1.4.2
 Summary: Fides Taxonomy Language
 Home-page: https://github.com/ethyca/fideslang
 Author: Ethyca, Inc.
 Author-email: fidesteam@ethyca.com
 License: Apache License 2.0
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
-Provides-Extra: all
 Provides-Extra: fastapi
+Provides-Extra: all
 License-File: LICENSE
 
 # Fideslang
 
 [![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/) [![Twitter](https://img.shields.io/twitter/follow/ethyca?style=social)](https://twitter.com/ethyca)
 
 ![Fideslang banner](mkdocs/docs/img/fideslang.png "Fideslang banner")
@@ -84,9 +83,7 @@
 ### Extensibility & Interoperability
 
 The taxonomy is designed to support common privacy compliance regulations and standards out of the box, these include GDPR, CCPA, LGPD and ISO 19944.
 
 You can extend the taxonomy to support your system needs. If you do this, we recommend extending from the existing class structures to ensure interoperability inside and outside your organization.
 
 If you have suggestions for missing classifications or concepts, please submit them for addition.
-
-
```

### Comparing `fideslang-1.4.1/README.md` & `fideslang-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `fideslang-1.4.1/pyproject.toml` & `fideslang-1.4.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 [build-system]
-requires = ["setuptools", "wheel", "versioneer-518"]  # PEP 508 specifications.
+requires = ["setuptools", "wheel", "versioneer[toml]==0.28"]  # PEP 508 specifications.
+
+[tool.versioneer]
+VCS = "git"
+style = "pep440"
+versionfile_source = "src/fideslang/_version.py"
+versionfile_build = "fideslang/_version.py"
+tag_prefix = ""
+parentdir_prefix = ""
 
 ######
 # MyPy
 ######
 # [tool.mypy] Waiting for new version of Mypy
 # warn_unused_configs = true
 # ignore_missing_imports = true
@@ -69,12 +77,11 @@
 ########
 [tool.pytest.ini_options]
 testpaths="tests"
 log_level = "DEBUG"
 addopts = ["--cov=fideslang",
             "--cov-report=term-missing",
             "-vv",
-            "--no-cov-on-fail",
-            "--disable-pytest-warnings"]
+            "--no-cov-on-fail",]
 markers = [
     "unit: only runs tests that don't require non-python dependencies (i.e. a database)",
 ]
```

### Comparing `fideslang-1.4.1/setup.py` & `fideslang-1.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `fideslang-1.4.1/src/fideslang/__init__.py` & `fideslang-1.4.2/src/fideslang/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 """
 
 from typing import Dict, Type, Union
 
 from fideslang.default_fixtures import COUNTRY_CODES
 from fideslang.default_taxonomy import DEFAULT_TAXONOMY
 
+from . import _version
+
+__version__ = _version.get_versions()["version"]
+
 # Export the Models
 from .models import (
     DataCategory,
     DataFlow,
     DataQualifier,
     Dataset,
     DatasetField,
```

### Comparing `fideslang-1.4.1/src/fideslang/default_fixtures.py` & `fideslang-1.4.2/src/fideslang/default_fixtures.py`

 * *Files identical despite different names*

### Comparing `fideslang-1.4.1/src/fideslang/default_taxonomy/__init__.py` & `fideslang-1.4.2/src/fideslang/default_taxonomy/__init__.py`

 * *Files identical despite different names*

### Comparing `fideslang-1.4.1/src/fideslang/default_taxonomy/data_categories.py` & `fideslang-1.4.2/src/fideslang/default_taxonomy/data_categories.py`

 * *Files identical despite different names*

### Comparing `fideslang-1.4.1/src/fideslang/default_taxonomy/data_qualifiers.py` & `fideslang-1.4.2/src/fideslang/default_taxonomy/data_qualifiers.py`

 * *Files identical despite different names*

### Comparing `fideslang-1.4.1/src/fideslang/default_taxonomy/data_subjects.py` & `fideslang-1.4.2/src/fideslang/default_taxonomy/data_subjects.py`

 * *Files identical despite different names*

### Comparing `fideslang-1.4.1/src/fideslang/default_taxonomy/data_uses.py` & `fideslang-1.4.2/src/fideslang/default_taxonomy/data_uses.py`

 * *Files identical despite different names*

### Comparing `fideslang-1.4.1/src/fideslang/manifests.py` & `fideslang-1.4.2/src/fideslang/manifests.py`

 * *Files identical despite different names*

### Comparing `fideslang-1.4.1/src/fideslang/models.py` & `fideslang-1.4.2/src/fideslang/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,17 +16,14 @@
     Field,
     HttpUrl,
     PositiveInt,
     root_validator,
     validator,
 )
 
-# import `Literal` from typing_extensions to work around https://github.com/pydantic/pydantic/issues/5821
-from typing_extensions import Literal
-
 from fideslang.validation import (
     FidesKey,
     check_valid_country_code,
     matching_parent_key,
     no_self_reference,
     parse_data_type_string,
     sort_list_objects_by_name,
@@ -177,14 +174,27 @@
     parent_key: Optional[FidesKey]
     is_default: bool = is_default_field
 
     _matching_parent_key: classmethod = matching_parent_key_validator
     _no_self_reference: classmethod = no_self_reference_validator
 
 
+class Cookies(BaseModel):
+    """The Cookies resource model"""
+
+    name: str
+    path: Optional[str]
+    domain: Optional[str]
+
+    class Config:
+        """Config for the cookies"""
+
+        orm_mode = True
+
+
 class DataSubjectRights(BaseModel):
     """
     The DataSubjectRights resource model.
 
     Includes a strategy and optionally a
     list of data subject rights to apply
     via the set strategy.
@@ -306,15 +316,19 @@
         description="A Data Qualifier that applies to this field. Note that this field holds a single value, therefore, the property name is singular.",
     )
     retention: Optional[str] = Field(
         description="An optional string to describe the retention policy for a dataset. This field can also be applied more granularly at either the Collection or field level of a Dataset.",
     )
 
 
-EdgeDirection = Literal["from", "to"]
+class EdgeDirection(str, Enum):
+    """Direction of a FidesDataSetReference"""
+
+    FROM = "from"
+    TO = "to"
 
 
 class FidesDatasetReference(BaseModel):
     """Reference to a field from another Collection"""
 
     dataset: FidesKey
     field: str
@@ -814,14 +828,17 @@
     )
     egress: Optional[List[FidesKey]] = Field(
         description="The resources to which data is sent. Any `fides_key`s included in this list reference `DataFlow` entries in the `egress` array of any `System` resources to which this `PrivacyDeclaration` is applied."
     )
     ingress: Optional[List[FidesKey]] = Field(
         description="The resources from which data is received. Any `fides_key`s included in this list reference `DataFlow` entries in the `ingress` array of any `System` resources to which this `PrivacyDeclaration` is applied."
     )
+    cookies: Optional[List[Cookies]] = Field(
+        description="Cookies associated with this data use to deliver services and functionality",
+    )
 
     @validator("dataset_references")
     @classmethod
     def deprecate_dataset_references(cls, value: List[FidesKey]) -> List[FidesKey]:
         """
         Warn that the `dataset_references` field is deprecated, if set.
         """
@@ -955,15 +972,14 @@
         default="Not defined",
         description="An optional value to identify the owning department or group of the system within your organization",
     )
     data_protection_impact_assessment: DataProtectionImpactAssessment = Field(
         default=DataProtectionImpactAssessment(),
         description=DataProtectionImpactAssessment.__doc__,
     )
-
     _sort_privacy_declarations: classmethod = validator(
         "privacy_declarations", allow_reuse=True
     )(sort_list_objects_by_name)
 
     _check_valid_country_code: classmethod = country_code_validator
 
     @validator("privacy_declarations", each_item=True)
```

### Comparing `fideslang-1.4.1/src/fideslang/parse.py` & `fideslang-1.4.2/src/fideslang/parse.py`

 * *Files identical despite different names*

### Comparing `fideslang-1.4.1/src/fideslang/relationships.py` & `fideslang-1.4.2/src/fideslang/relationships.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 This module is responsible for calculating what resources are referenced
 by each other and building a dependency graph of relationships.
 """
 
 import inspect
+from enum import Enum
 from functools import reduce
-from typing import List, Set
+from typing import List, Optional, Set
 
 from fideslang.models import BaseModel, FidesKey, Taxonomy
 from fideslang.utils import get_resource_by_fides_key
 
 
 def find_nested_keys_in_list(parameter_value: List[BaseModel]) -> List[str]:
     """
@@ -25,52 +26,64 @@
 
 def find_referenced_fides_keys(resource: object) -> Set[FidesKey]:
     """
     Use type-signature introspection to figure out which fields
     include the FidesKey type and return all of those values.
 
     Note that this finds _all_ fides_keys, including the resource's own fides_key
+
+    This function is used recursively for arbitrary-depth objects.
     """
     referenced_fides_keys: Set[FidesKey] = set()
+
+    # Str type doesn't have a signature, so we return early
+    if isinstance(resource, str) and not isinstance(resource, Enum):
+        return set()
+
     signature = inspect.signature(type(resource), follow_wrapped=True)
-    parameter_values = filter(
+    attributes = filter(
         lambda parameter: hasattr(resource, parameter.name),
         signature.parameters.values(),
     )
-    for parameter in parameter_values:
-        parameter_value = resource.__getattribute__(parameter.name)
-        if parameter_value:
-            if parameter.annotation == FidesKey:
-                referenced_fides_keys.add(parameter_value)
-            elif parameter.annotation == List[FidesKey]:
-                referenced_fides_keys.update(resource.__getattribute__(parameter.name))
+
+    for attribute in attributes:
+        attribute_value = resource.__getattribute__(attribute.name)
+        if attribute_value:
+            # If it is a single FidesKey, add it directly
+            if attribute.annotation in (FidesKey, Optional[FidesKey]):
+                referenced_fides_keys.add(attribute_value)
+            # Add the list of FidesKeys to the set
+            elif attribute.annotation == List[FidesKey]:
+                referenced_fides_keys.update(resource.__getattribute__(attribute.name))
+            # If it is a list, but not of strings, recurse into each one
             elif (
-                isinstance(parameter_value, list) and parameter.annotation != List[str]
+                isinstance(attribute_value, list) and attribute.annotation != List[str]
             ):
-                nested_keys = find_nested_keys_in_list(parameter_value)
+                nested_keys = find_nested_keys_in_list(attribute_value)
                 referenced_fides_keys.update(nested_keys)
-            elif hasattr(parameter_value, "__dict__"):
+            # If it is a Pydantic Model then recurse
+            elif isinstance(attribute_value, BaseModel):
                 referenced_fides_keys.update(
-                    find_referenced_fides_keys(parameter_value)
+                    find_referenced_fides_keys(attribute_value)
                 )
     return referenced_fides_keys
 
 
-def get_referenced_missing_keys(taxonomy: Taxonomy) -> List[FidesKey]:
+def get_referenced_missing_keys(taxonomy: Taxonomy) -> Set[FidesKey]:
     """
     Iterate through the Taxonomy and create a set of all of the FidesKeys
     that are contained within it.
     """
     referenced_keys: List[Set[FidesKey]] = [
         find_referenced_fides_keys(resource)
         for resource_type in taxonomy.__fields_set__
         for resource in getattr(taxonomy, resource_type)
     ]
     key_set: Set[FidesKey] = set(
         reduce(lambda x, y: set().union(x).union(y), referenced_keys)
     )
-    keys_not_in_taxonomy = [
+    keys_not_in_taxonomy = {
         fides_key
         for fides_key in key_set
         if get_resource_by_fides_key(taxonomy, fides_key) is None
-    ]
+    }
     return keys_not_in_taxonomy
```

### Comparing `fideslang-1.4.1/src/fideslang/utils.py` & `fideslang-1.4.2/src/fideslang/utils.py`

 * *Files identical despite different names*

### Comparing `fideslang-1.4.1/src/fideslang/validation.py` & `fideslang-1.4.2/src/fideslang/validation.py`

 * *Files identical despite different names*

### Comparing `fideslang-1.4.1/src/fideslang.egg-info/PKG-INFO` & `fideslang-1.4.2/src/fideslang.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: fideslang
-Version: 1.4.1
+Version: 1.4.2
 Summary: Fides Taxonomy Language
 Home-page: https://github.com/ethyca/fideslang
 Author: Ethyca, Inc.
 Author-email: fidesteam@ethyca.com
 License: Apache License 2.0
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
-Provides-Extra: all
 Provides-Extra: fastapi
+Provides-Extra: all
 License-File: LICENSE
 
 # Fideslang
 
 [![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/) [![Twitter](https://img.shields.io/twitter/follow/ethyca?style=social)](https://twitter.com/ethyca)
 
 ![Fideslang banner](mkdocs/docs/img/fideslang.png "Fideslang banner")
@@ -84,9 +83,7 @@
 ### Extensibility & Interoperability
 
 The taxonomy is designed to support common privacy compliance regulations and standards out of the box, these include GDPR, CCPA, LGPD and ISO 19944.
 
 You can extend the taxonomy to support your system needs. If you do this, we recommend extending from the existing class structures to ensure interoperability inside and outside your organization.
 
 If you have suggestions for missing classifications or concepts, please submit them for addition.
-
-
```

### Comparing `fideslang-1.4.1/src/fideslang.egg-info/SOURCES.txt` & `fideslang-1.4.2/src/fideslang.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 MANIFEST.in
 README.md
 dev-requirements.txt
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
-versioneer.py
 src/fideslang/__init__.py
 src/fideslang/_version.py
 src/fideslang/default_fixtures.py
 src/fideslang/manifests.py
 src/fideslang/models.py
 src/fideslang/parse.py
 src/fideslang/py.typed
```

