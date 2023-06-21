# Comparing `tmp/eido-0.1.9.tar.gz` & `tmp/eido-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eido-0.1.9.tar", last modified: Mon Sep 12 17:06:01 2022, max compression
+gzip compressed data, was "eido-0.2.0.tar", last modified: Wed Jun 21 14:51:07 2023, max compression
```

## Comparing `eido-0.1.9.tar` & `eido-0.2.0.tar`

### file list

```diff
@@ -1,33 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 17:06:01.613964 eido-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (121)     1269 2022-09-12 17:05:51.000000 eido-0.1.9/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-09-12 17:05:51.000000 eido-0.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1309 2022-09-12 17:06:01.613964 eido-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      632 2022-09-12 17:05:51.000000 eido-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 17:06:01.613964 eido-0.1.9/eido/
--rw-r--r--   0 runner    (1001) docker     (121)      529 2022-09-12 17:05:51.000000 eido-0.1.9/eido/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-09-12 17:05:51.000000 eido-0.1.9/eido/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-09-12 17:05:51.000000 eido-0.1.9/eido/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     4620 2022-09-12 17:05:51.000000 eido-0.1.9/eido/argparser.py
--rw-r--r--   0 runner    (1001) docker     (121)     4499 2022-09-12 17:05:51.000000 eido-0.1.9/eido/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     1096 2022-09-12 17:05:51.000000 eido-0.1.9/eido/const.py
--rw-r--r--   0 runner    (1001) docker     (121)     3912 2022-09-12 17:05:51.000000 eido-0.1.9/eido/conversion.py
--rw-r--r--   0 runner    (1001) docker     (121)     2488 2022-09-12 17:05:51.000000 eido-0.1.9/eido/conversion_plugins.py
--rw-r--r--   0 runner    (1001) docker     (121)     1014 2022-09-12 17:05:51.000000 eido-0.1.9/eido/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)      672 2022-09-12 17:05:51.000000 eido-0.1.9/eido/inspection.py
--rw-r--r--   0 runner    (1001) docker     (121)     4495 2022-09-12 17:05:51.000000 eido-0.1.9/eido/output_formatters.py
--rw-r--r--   0 runner    (1001) docker     (121)     3015 2022-09-12 17:05:51.000000 eido-0.1.9/eido/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     7477 2022-09-12 17:05:51.000000 eido-0.1.9/eido/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 17:06:01.613964 eido-0.1.9/eido.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1309 2022-09-12 17:06:01.000000 eido-0.1.9/eido.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      588 2022-09-12 17:06:01.000000 eido-0.1.9/eido.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-12 17:06:01.000000 eido-0.1.9/eido.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      263 2022-09-12 17:06:01.000000 eido-0.1.9/eido.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-09-12 17:06:01.000000 eido-0.1.9/eido.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-09-12 17:06:01.000000 eido-0.1.9/eido.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 17:06:01.613964 eido-0.1.9/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-09-12 17:05:51.000000 eido-0.1.9/requirements/requirements-all.txt
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-09-12 17:05:51.000000 eido-0.1.9/requirements/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-09-12 17:05:51.000000 eido-0.1.9/requirements/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-09-12 17:05:51.000000 eido-0.1.9/requirements/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-12 17:06:01.613964 eido-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2538 2022-09-12 17:05:51.000000 eido-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:51:07.686725 eido-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-21 14:50:58.000000 eido-0.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-21 14:50:58.000000 eido-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-21 14:51:07.686725 eido-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-21 14:50:58.000000 eido-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:51:07.682725 eido-0.2.0/eido/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-21 14:50:58.000000 eido-0.2.0/eido/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-21 14:50:58.000000 eido-0.2.0/eido/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 14:50:58.000000 eido-0.2.0/eido/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-06-21 14:50:58.000000 eido-0.2.0/eido/argparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-06-21 14:50:58.000000 eido-0.2.0/eido/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-21 14:50:58.000000 eido-0.2.0/eido/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-06-21 14:50:58.000000 eido-0.2.0/eido/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-21 14:50:58.000000 eido-0.2.0/eido/conversion_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-21 14:50:58.000000 eido-0.2.0/eido/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-06-21 14:50:58.000000 eido-0.2.0/eido/inspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-06-21 14:50:58.000000 eido-0.2.0/eido/output_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-21 14:50:58.000000 eido-0.2.0/eido/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-06-21 14:50:58.000000 eido-0.2.0/eido/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:51:07.686725 eido-0.2.0/eido.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-21 14:51:07.000000 eido-0.2.0/eido.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-21 14:51:07.000000 eido-0.2.0/eido.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:51:07.000000 eido-0.2.0/eido.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-21 14:51:07.000000 eido-0.2.0/eido.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-21 14:51:07.000000 eido-0.2.0/eido.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-21 14:51:07.000000 eido-0.2.0/eido.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:51:07.686725 eido-0.2.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-21 14:50:58.000000 eido-0.2.0/requirements/requirements-all.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-21 14:50:58.000000 eido-0.2.0/requirements/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-21 14:50:58.000000 eido-0.2.0/requirements/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 14:51:07.686725 eido-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-06-21 14:50:58.000000 eido-0.2.0/setup.py
```

### Comparing `eido-0.1.9/LICENSE.txt` & `eido-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `eido-0.1.9/PKG-INFO` & `eido-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: eido
-Version: 0.1.9
+Version: 0.2.0
 Summary: A project metadata validator
 Home-page: https://github.com/pepkit/eido/
 Author: Michal Stolarczyk, Nathan Sheffield
 License: BSD2
 Keywords: project,metadata,bioinformatics,sequencing,ngs,workflow
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # <img src="docs/img/eido.svg" alt="eido logo" height="70">
 
 ![Run pytests](https://github.com/pepkit/eido/workflows/Run%20pytests/badge.svg)
```

### Comparing `eido-0.1.9/README.md` & `eido-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `eido-0.1.9/eido/argparser.py` & `eido-0.2.0/eido/argparser.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,21 +3,15 @@
 from peppy.const import SAMPLE_NAME_ATTR
 from peppy import __version__ as peppy_version
 from ubiquerg import VersionInHelpParser
 
 from . import __version__
 from .const import *
 
-LEVEL_BY_VERBOSITY = [
-    ERROR,
-    CRITICAL,
-    WARN,
-    INFO,
-    DEBUG,
-]
+LEVEL_BY_VERBOSITY = [ERROR, CRITICAL, WARN, INFO, DEBUG]
 
 version_combined = f"{__version__} (peppy {peppy_version})"
 
 
 def build_argparser():
     banner = "%(prog)s - Interact with PEPs"
     additional_description = "\nhttp://eido.databio.org/"
@@ -42,37 +36,54 @@
         "--dbg",
         dest="dbg",
         action="store_true",
         help="Turn on debug mode (default: %(default)s)",
     )
     sps = {}
     for cmd, desc in SUBPARSER_MSGS.items():
-        sps[cmd] = subparsers.add_parser(cmd, description=desc, help=desc)
-        sps[cmd].add_argument(
+        subparser = subparsers.add_parser(cmd, description=desc, help=desc)
+        subparser.add_argument(
             "--st-index",
             required=False,
             type=str,
+            default=SAMPLE_NAME_ATTR,
             help=f"Sample table index to use, samples are identified by '{SAMPLE_NAME_ATTR}' by default.",
         )
+        subparser.add_argument(
+            "--sst-index",
+            required=False,
+            type=str,
+            default=SAMPLE_NAME_ATTR,
+            help=f"Subsample table index to use, samples are identified by '{SAMPLE_NAME_ATTR}' by default.",
+        )
+        subparser.add_argument(
+            "--amendments",
+            required=False,
+            type=str,
+            nargs="+",
+            help=f"Names of the amendments to activate.",
+        )
         if cmd != CONVERT_CMD:
-            sps[cmd].add_argument(
+            subparser.add_argument(
                 "pep",
                 metavar="PEP",
                 help="Path to a PEP configuration file in yaml format.",
                 default=None,
             )
         else:
-            sps[cmd].add_argument(
+            subparser.add_argument(
                 "pep",
                 metavar="PEP",
                 nargs="?",
                 help="Path to a PEP configuration file in yaml format.",
                 default=None,
             )
 
+        sps[cmd] = subparser
+
     sps[VALIDATE_CMD].add_argument(
         "-s",
         "--schema",
         required=True,
         help="Path to a PEP schema file in yaml format.",
         metavar="S",
     )
```

### Comparing `eido-0.1.9/eido/cli.py` & `eido-0.2.0/eido/cli.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from .argparser import LEVEL_BY_VERBOSITY, build_argparser
 from .const import *
 from .conversion import (
     convert_project,
     get_available_pep_filters,
     pep_conversion_plugins,
 )
-from .exceptions import EidoFilterError
+from .exceptions import EidoFilterError, EidoValidationError
 from .inspection import inspect_project
 from .validation import validate_config, validate_project, validate_sample
 
 
 def _parse_filter_args_str(input):
     """
     Parse user input specification.
@@ -30,14 +30,34 @@
     return (
         {x.split("=")[0]: x.split("=")[1] for x in lst if "=" in x}
         if lst is not None
         else lst
     )
 
 
+def print_error_summary(errors_by_type):
+    """Print a summary of errors, organized by error type"""
+    n_error_types = len(errors_by_type)
+    print(f"Found {n_error_types} types of error:")
+    for type in errors_by_type:
+        n = len(errors_by_type[type])
+        msg = f"  - {type}: ({n} samples) "
+        if n < 50:
+            msg += ", ".join([x["sample_name"] for x in errors_by_type[type]])
+        print(msg)
+
+    if len(errors_by_type) > 1:
+        final_msg = f"Validation unsuccessful. {len(errors_by_type)} error types found."
+    else:
+        final_msg = f"Validation unsuccessful. {len(errors_by_type)} error type found."
+
+    print(final_msg)
+    return final_msg
+
+
 def main():
     """Primary workflow"""
     parser, sps = build_argparser()
     args, remaining_args = parser.parse_known_args()
 
     if args.command is None:
         parser.print_help(sys.stderr)
@@ -85,46 +105,70 @@
             _LOGGER.info("The following arguments are required: PEP")
             sys.exit(1)
         if args.paths:
             paths = {y[0]: y[1] for y in [x.split("=") for x in args.paths]}
         else:
             paths = None
 
-        p = Project(args.pep, sample_table_index=args.st_index)
+        p = Project(
+            args.pep,
+            sample_table_index=args.st_index,
+            subsample_table_index=args.sst_index,
+            amendments=args.amendments,
+        )
         plugin_kwargs = _parse_filter_args_str(args.args)
 
         # append paths
         plugin_kwargs["paths"] = paths
 
         convert_project(p, args.format, plugin_kwargs)
         _LOGGER.info("Conversion successful")
         sys.exit(0)
 
     _LOGGER.debug(f"Creating a Project object from: {args.pep}")
     if args.command == VALIDATE_CMD:
-        p = Project(cfg=args.pep, sample_table_index=args.st_index)
+        p = Project(
+            args.pep,
+            sample_table_index=args.st_index,
+            subsample_table_index=args.sst_index,
+            amendments=args.amendments,
+        )
         if args.sample_name:
             try:
                 args.sample_name = int(args.sample_name)
             except ValueError:
                 pass
             _LOGGER.debug(
                 f"Comparing Sample ('{args.pep}') in Project ('{args.pep}') "
                 f"against a schema: {args.schema}"
             )
-            validate_sample(p, args.sample_name, args.schema, args.exclude_case)
+            validator = validate_sample
+            arguments = [p, args.sample_name, args.schema, args.exclude_case]
         elif args.just_config:
             _LOGGER.debug(
                 f"Comparing Project ('{args.pep}') against a schema: {args.schema}"
             )
-            validate_config(p, args.schema, args.exclude_case)
+            validator = validate_config
+            arguments = [p, args.schema, args.exclude_case]
         else:
             _LOGGER.debug(
                 f"Comparing Project ('{args.pep}') against a schema: {args.schema}"
             )
-            validate_project(p, args.schema, args.exclude_case)
+            validator = validate_project
+            arguments = [p, args.schema, args.exclude_case]
+        try:
+            validator(*arguments)
+        except EidoValidationError as e:
+            print_error_summary(e.errors_by_type)
+            return False
         _LOGGER.info("Validation successful")
+        sys.exit(0)
 
     if args.command == INSPECT_CMD:
-        p = Project(cfg=args.pep, sample_table_index=args.st_index)
+        p = Project(
+            args.pep,
+            sample_table_index=args.st_index,
+            subsample_table_index=args.sst_index,
+            amendments=args.amendments,
+        )
         inspect_project(p, args.sample_name, args.attr_limit)
         sys.exit(0)
```

### Comparing `eido-0.1.9/eido/const.py` & `eido-0.2.0/eido/const.py`

 * *Files identical despite different names*

### Comparing `eido-0.1.9/eido/conversion.py` & `eido-0.2.0/eido/conversion.py`

 * *Files identical despite different names*

### Comparing `eido-0.1.9/eido/conversion_plugins.py` & `eido-0.2.0/eido/conversion_plugins.py`

 * *Files identical despite different names*

### Comparing `eido-0.1.9/eido/exceptions.py` & `eido-0.2.0/eido/exceptions.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 """ Exceptions for specific eido issues. """
 
 from abc import ABCMeta
 
-_all__ = ["PathAttrNotFoundError", "EidoSchemaInvalidError", "EidoFilterError"]
+_all__ = [
+    "EidoFilterError",
+    "EidoSchemaInvalidError",
+    "EidoValidationError",
+    "PathAttrNotFoundError",
+]
 
 
 class EidoException(Exception):
     """Base type for custom package errors."""
 
     __metaclass__ = ABCMeta
 
@@ -31,10 +36,10 @@
     def __init__(self, key):
         super(EidoFilterError, self).__init__(key)
 
 
 class EidoValidationError(EidoException):
     """Object was not validated successfully according to schema."""
 
-    def __init__(self, message, errors):
+    def __init__(self, message, errors_by_type):
         super().__init__(message)
-        self.errors = errors
+        self.errors_by_type = errors_by_type
```

### Comparing `eido-0.1.9/eido/output_formatters.py` & `eido-0.2.0/eido/output_formatters.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,14 @@
             attribute
             for attribute in samples[0].keys()
             if not attribute.startswith("_") and not attribute == "subsample_name"
         ]
         header = MultilineOutputFormatter._get_header(sample_attributes)
 
         for sample in samples:
-
             attribute_with_multiple_properties = MultilineOutputFormatter._get_the_name_of_the_first_attribute_with_multiple_properties(
                 sample, sample_attributes
             )
             if attribute_with_multiple_properties:
                 sample_rows = MultilineOutputFormatter._split_sample_to_multiple_rows(
                     sample, sample_attributes, attribute_with_multiple_properties
                 )
@@ -99,22 +98,23 @@
             sample_attributes: Array of all attributes names (column names) for given sample.
             sample_index: Number indicating which value will be used to create row. Some samples
 
         Returns:
             Representation of sample as a CSV row.
         """
         sample_row = []
-        for attribute in sample_attributes:
 
-            if MultilineOutputFormatter._sample_attribute_is_list(
-                sample, attribute
-            ) and getattr(sample, attribute):
-                value = getattr(sample, attribute)[sample_index]
+        for attribute in sample_attributes:
+            if (
+                MultilineOutputFormatter._sample_attribute_is_list(sample, attribute)
+                and sample[attribute]
+            ):
+                value = sample[attribute][sample_index]
             else:
-                value = getattr(sample, attribute, "")
+                value = sample[attribute]
 
             sample_row.append(value or "")
 
         return ",".join(sample_row)
 
     @staticmethod
     def _sample_attribute_is_list(sample: Sample, attribute: str) -> bool:
```

### Comparing `eido-0.1.9/eido/schema.py` & `eido-0.2.0/eido/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,15 @@
             else:
                 raise TypeError("In schema the 'imports' section has to be a list")
         lst.append(x)
         return lst
 
     schema_list = []
     if isinstance(schema, str):
-        return _recursively_read_schemas(load_yaml(schema), schema_list)
-    elif isinstance(schema, dict):
-        return _recursively_read_schemas(schema, schema_list)
-    raise TypeError(
-        f"schema has to be a dict, path to an existing file or URL to a remote one. "
-        f"Got: {type(schema)}"
-    )
+        _LOGGER.debug(f"Reading schema: {schema}")
+        schema = load_yaml(schema)
+    if not isinstance(schema, dict):
+        raise TypeError(
+            f"schema has to be a dict, path to an existing file or URL to a remote one. "
+            f"Got: {type(schema)}"
+        )
+    return _recursively_read_schemas(schema, schema_list)
```

### Comparing `eido-0.1.9/eido/validation.py` & `eido-0.2.0/eido/validation.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,196 +1,220 @@
 import os
 from copy import deepcopy as dpcpy
 from logging import getLogger
-from warnings import catch_warnings as cw
+
+from warnings import warn
+
 from .exceptions import EidoValidationError
 
-from pandas.core.common import flatten
-from ubiquerg import size
 
+from pandas.core.common import flatten
 from jsonschema import Draft7Validator
 
 from .const import (
-    ALL_INPUTS_KEY,
     FILES_KEY,
-    INPUT_FILE_SIZE_KEY,
-    MISSING_KEY,
     PROP_KEY,
     REQUIRED_FILES_KEY,
-    REQUIRED_INPUTS_KEY,
 )
+from .exceptions import PathAttrNotFoundError
 from .schema import preprocess_schema, read_schema
 
 _LOGGER = getLogger(__name__)
 
 
-def _validate_object(object, schema, exclude_case=False):
+def _validate_object(object, schema, sample_name_colname=False):
     """
     Generic function to validate object against a schema
 
     :param Mapping object: an object to validate
     :param str | dict schema: schema dict to validate against or a path to one
-    :param bool exclude_case: whether to exclude validated objects
         from the error. Useful when used ith large projects
+    :raises EidoValidationError: if validation is unsuccessful
     """
-
     validator = Draft7Validator(schema)
+    print(object, schema)
     if not validator.is_valid(object):
         errors = sorted(validator.iter_errors(object), key=lambda e: e.path)
-        raise EidoValidationError(
-            f"Validation unsuccessful. {len(errors)} errors found.", errors
-        )
+        errors_by_type = {}
 
+        # Accumulate and restructure error objects by error type
+        for error in errors:
+            if not error.message in errors_by_type:
+                errors_by_type[error.message] = []
 
-def validate_project(project, schema, exclude_case=False):
+            try:
+                instance_name = error.instance[sample_name_colname]
+            except KeyError:
+                instance_name = "project"
+            errors_by_type[error.message].append(
+                {
+                    "type": error.message,
+                    "message": f"{error.message} on instance {instance_name}",
+                    "sample_name": instance_name,
+                }
+            )
+
+        raise EidoValidationError("Validation failed", errors_by_type)
+    else:
+        _LOGGER.debug("Validation was successful...")
+
+
+def validate_project(project, schema):
     """
     Validate a project object against a schema
 
-    :param peppy.Sample project: a project object to validate
+    :param peppy.Project project: a project object to validate
     :param str | dict schema: schema dict to validate against or a path to one
-    :param bool exclude_case: whether to exclude validated objects
     from the error. Useful when used ith large projects
     """
+    sample_name_colname = project.sample_name_colname
     schema_dicts = read_schema(schema=schema)
     for schema_dict in schema_dicts:
         project_dict = project.to_dict()
-        _validate_object(project_dict, preprocess_schema(schema_dict), exclude_case)
+        _validate_object(
+            project_dict, preprocess_schema(schema_dict), sample_name_colname
+        )
         _LOGGER.debug("Project validation successful")
 
 
-def _validate_sample_object(sample, schemas, exclude_case=False):
+def _validate_sample_object(sample, schemas):
     """
     Internal function that allows to validate a peppy.Sample object without
     requiring a reference to peppy.Project.
 
     :param peppy.Sample sample: a sample object to validate
     :param list[dict] schemas: list of schemas to validate against or a path to one
-    :param bool exclude_case: whether to exclude validated objects
-        from the error. Useful when used ith large projects
     """
     for schema_dict in schemas:
         schema_dict = preprocess_schema(schema_dict)
         sample_schema_dict = schema_dict[PROP_KEY]["_samples"]["items"]
-        _validate_object(sample, sample_schema_dict, exclude_case)
+        _validate_object(sample.to_dict(), sample_schema_dict)
         _LOGGER.debug(
             f"{getattr(sample, 'sample_name', '')} sample validation successful"
         )
 
 
-def validate_sample(project, sample_name, schema, exclude_case=False):
+def validate_sample(project, sample_name, schema):
     """
     Validate the selected sample object against a schema
 
     :param peppy.Project project: a project object to validate
     :param str | int sample_name: name or index of the sample to validate
     :param str | dict schema: schema dict to validate against or a path to one
-    :param bool exclude_case: whether to exclude validated objects
-        from the error. Useful when used ith large projects
     """
     sample = (
         project.samples[sample_name]
         if isinstance(sample_name, int)
         else project.get_sample(sample_name)
     )
     _validate_sample_object(
-        sample=sample, schemas=read_schema(schema=schema), exclude_case=exclude_case
+        sample=sample,
+        schemas=read_schema(schema=schema),
     )
 
 
-def validate_config(project, schema, exclude_case=False):
+def validate_config(project, schema):
     """
     Validate the config part of the Project object against a schema
 
     :param peppy.Project project: a project object to validate
     :param str | dict schema: schema dict to validate against or a path to one
-    :param bool exclude_case: whether to exclude validated objects
-        from the error. Useful when used ith large projects
     """
     schema_dicts = read_schema(schema=schema)
     for schema_dict in schema_dicts:
         schema_cpy = preprocess_schema(dpcpy(schema_dict))
         try:
             del schema_cpy[PROP_KEY]["_samples"]
         except KeyError:
             pass
         if "required" in schema_cpy:
             try:
                 schema_cpy["required"].remove("_samples")
             except ValueError:
                 pass
         project_dict = project.to_dict()
-        _validate_object(project_dict, schema_cpy, exclude_case)
+        _validate_object(project_dict, schema_cpy)
         _LOGGER.debug("Config validation successful")
 
 
-def validate_inputs(sample, schema, exclude_case=False):
+def _get_attr_values(obj, attrlist):
     """
-    Determine which of this Sample's required attributes/files are missing
-    and calculate sizes of the inputs.
+    Get value corresponding to each given attribute.
+
+    :param Mapping obj: an object to get the attributes from
+    :param str | Iterable[str] attrlist: names of attributes to
+        retrieve values for
+    :return dict: value corresponding to
+        each named attribute; null if this Sample's value for the
+        attribute given by the argument to the "attrlist" parameter is
+        empty/null, or if this Sample lacks the indicated attribute
+    """
+    # If attribute is None, then value is also None.
+    if not attrlist:
+        return None
+    if not isinstance(attrlist, list):
+        attrlist = [attrlist]
+    # Strings contained here are appended later so shouldn't be null.
+    return list(flatten([getattr(obj, attr, "") for attr in attrlist]))
+
+
+def validate_input_files(project, schemas, sample_name=None):
+    """
+    Determine which of the required and optional files are missing.
 
     The names of the attributes that are required and/or deemed as inputs
-    are sourced from the schema, more specifically from required_input_attrs
-    and input_attrs sections in samples section. Note, this function does
-    perform actual Sample object validation with jsonschema.
-
-    :param peppy.Sample sample: sample to investigate
-    :param list[dict] | str schema: schema dict to validate against or a path to one
-    :return dict: dictionary with validation data, i.e missing,
-        required_inputs, all_inputs, input_file_size
-    :param bool exclude_case: whether to exclude validated objects
-        from the error. Useful when used ith large projects
-    :raise ValidationError: if any required sample attribute is missing
+    are sourced from the schema, more specifically from `required_files`
+    and `files` sections in samples section:
+
+    - If any of the required files are missing, this function raises an error.
+    - If any of the optional files are missing, the function raises a warning.
+
+    Note, this function also performs Sample object validation with jsonschema.
+
+    :param peppy.Project project: project that defines the samples to validate
+    :param str | dict schema: schema dict to validate against or a path to one
+    :param str | int sample_name: name or index of the sample to validate. If None,
+        validate all samples in the project
+    :raise PathAttrNotFoundError: if any required sample attribute is missing
     """
 
-    def _get_attr_values(obj, attrlist):
-        """
-        Get value corresponding to each given attribute.
-
-        :param Mapping obj: an object to get the attributes from
-        :param str | Iterable[str] attrlist: names of attributes to
-            retrieve values for
-        :return dict: value corresponding to
-            each named attribute; null if this Sample's value for the
-            attribute given by the argument to the "attrlist" parameter is
-            empty/null, or if this Sample lacks the indicated attribute
-        """
-        # If attribute is None, then value is also None.
-        if not attrlist:
-            return None
-        if not isinstance(attrlist, list):
-            attrlist = [attrlist]
-        # Strings contained here are appended later so shouldn't be null.
-        return list(flatten([getattr(obj, attr, "") for attr in attrlist]))
-
-    if isinstance(schema, str):
-        schema = read_schema(schema)
-
-    # validate attrs existence first
-    _validate_sample_object(schemas=schema, sample=sample, exclude_case=exclude_case)
-
-    all_inputs = set()
-    required_inputs = set()
-    schema = schema[-1]  # use only first schema, in case there are imports
-    sample_schema_dict = schema["properties"]["_samples"]["items"]
-    if FILES_KEY in sample_schema_dict:
-        all_inputs.update(_get_attr_values(sample, sample_schema_dict[FILES_KEY]))
-    if REQUIRED_FILES_KEY in sample_schema_dict:
-        required_inputs = set(
-            _get_attr_values(sample, sample_schema_dict[REQUIRED_FILES_KEY])
+    if sample_name is None:
+        samples = project.samples
+    else:
+        samples = (
+            project.samples[sample_name]
+            if isinstance(sample_name, int)
+            else project.get_sample(sample_name)
         )
-        all_inputs.update(required_inputs)
-    with cw(record=True) as w:
-        input_file_size = sum(
-            [size(f, size_str=False) or 0.0 for f in all_inputs if f != ""]
-        ) / (1024**3)
-        if w:
-            _LOGGER.warning(
-                f"{len(w)} input files missing, job input size was "
-                f"not calculated accurately"
+        samples = [samples]
+
+    if isinstance(schemas, str):
+        schemas = read_schema(schemas)
+
+    for sample in samples:
+        # validate attrs existence first
+        _validate_sample_object(schemas=schemas, sample=sample)
+
+        all_inputs = set()
+        required_inputs = set()
+        schema = schemas[-1]  # use only first schema, in case there are imports
+        sample_schema_dict = schema["properties"]["_samples"]["items"]
+        if FILES_KEY in sample_schema_dict:
+            all_inputs.update(_get_attr_values(sample, sample_schema_dict[FILES_KEY]))
+        if REQUIRED_FILES_KEY in sample_schema_dict:
+            required_inputs = set(
+                _get_attr_values(sample, sample_schema_dict[REQUIRED_FILES_KEY])
             )
+            all_inputs.update(required_inputs)
 
-    return {
-        MISSING_KEY: [i for i in required_inputs if not os.path.exists(i)],
-        REQUIRED_INPUTS_KEY: required_inputs,
-        ALL_INPUTS_KEY: all_inputs,
-        INPUT_FILE_SIZE_KEY: input_file_size,
-    }
+        missing_required_inputs = [i for i in required_inputs if not os.path.exists(i)]
+        missing_inputs = [i for i in all_inputs if not os.path.exists(i)]
+        if missing_inputs:
+            warn(
+                f"For sample '{getattr(sample, project.sample_table_index)}'. "
+                f"Optional inputs not found: {missing_inputs}"
+            )
+        if missing_required_inputs:
+            raise PathAttrNotFoundError(
+                f"For sample '{getattr(sample, project.sample_table_index)}'. "
+                f"Required inputs not found: {required_inputs}"
+            )
```

### Comparing `eido-0.1.9/eido.egg-info/PKG-INFO` & `eido-0.2.0/eido.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: eido
-Version: 0.1.9
+Version: 0.2.0
 Summary: A project metadata validator
 Home-page: https://github.com/pepkit/eido/
 Author: Michal Stolarczyk, Nathan Sheffield
 License: BSD2
 Keywords: project,metadata,bioinformatics,sequencing,ngs,workflow
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # <img src="docs/img/eido.svg" alt="eido logo" height="70">
 
 ![Run pytests](https://github.com/pepkit/eido/workflows/Run%20pytests/badge.svg)
```

### Comparing `eido-0.1.9/setup.py` & `eido-0.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
         if not line.strip():
             continue
         # DEPENDENCIES.append(line.split("=")[0].rstrip("<>"))
         DEPENDENCIES.append(line)
 
 extra["install_requires"] = DEPENDENCIES
 
+
 # Additional files to include with package
 def get_static(name, condition=None):
     static = [
         os.path.join(name, f)
         for f in os.listdir(
             os.path.join(os.path.dirname(os.path.realpath(__file__)), name)
         )
@@ -50,18 +51,18 @@
     version=version,
     description="A project metadata validator",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: BSD License",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
     ],
     keywords="project, metadata, bioinformatics, sequencing, ngs, workflow",
     url="https://github.com/pepkit/eido/",
     author="Michal Stolarczyk, Nathan Sheffield",
     license="BSD2",
     entry_points={
```

