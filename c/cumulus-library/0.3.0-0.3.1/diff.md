# Comparing `tmp/cumulus_library-0.3.0.tar.gz` & `tmp/cumulus_library-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cumulus_library-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "cumulus_library-0.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cumulus_library-0.3.0.tar` & `cumulus_library-0.3.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-lrwxr-xr-x   0        0        0        0 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/.sqlfluff -> cumulus_library/.sqlfluff
--rw-r--r--   0        0        0      421 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/README.md
--rw-r--r--   0        0        0      866 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/.sqlfluff
--rw-r--r--   0        0        0        0 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/__init__.py
--rw-r--r--   0        0        0      628 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/base_runner.py
--rwxr-xr-x   0        0        0    10545 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/cli.py
--rw-r--r--   0        0        0     5129 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/cli_parser.py
--rw-r--r--   0        0        0      190 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/errors.py
--rw-r--r--   0        0        0     1889 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/helper.py
--rw-r--r--   0        0        0      205 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/module_allowlist.json
--rw-r--r--   0        0        0     2343 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/parsers/fhir_valueset.py
--rw-r--r--   0        0        0        0 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/schema/__init__.py
--rw-r--r--   0        0        0     4848 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/schema/columns.py
--rw-r--r--   0        0        0     3346 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/schema/counts.py
--rw-r--r--   0        0        0     3364 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/schema/typesystem.py
--rw-r--r--   0        0        0     5876 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/schema/valueset.py
--rw-r--r--   0        0        0     2982 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/studies/core/condition.sql
--rw-r--r--   0        0        0     2867 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/studies/core/documentreference.sql
--rw-r--r--   0        0        0     3402 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/studies/core/encounter.sql
--rw-r--r--   0        0        0     4146 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/studies/core/fhir_define.sql
--rw-r--r--   0        0        0      673 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/studies/core/manifest.toml
--rw-r--r--   0        0        0     1241 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/studies/core/medication_request.sql
--rw-r--r--   0        0        0     1208 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/studies/core/observation.sql
--rw-r--r--   0        0        0     2884 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/studies/core/observation_lab.sql
--rw-r--r--   0        0        0     1272 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/studies/core/observation_vital_signs.sql
--rw-r--r--   0        0        0     1701 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/studies/core/patient.sql
--rw-r--r--   0        0        0     2241 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/studies/core/patient_extensions.py
--rw-r--r--   0        0        0     1436 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/studies/core/setup.sql
--rw-r--r--   0        0        0     1472 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/studies/core/study_period.sql
--rw-r--r--   0        0        0      834 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/studies/template/counts.sql
--rw-r--r--   0        0        0      187 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/studies/template/date_range.sql
--rw-r--r--   0        0        0      566 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/studies/template/lab_observations.sql
--rw-r--r--   0        0        0     1562 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/studies/template/manifest.toml
--rw-r--r--   0        0        0     1152 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/studies/template/setup.sql
--rw-r--r--   0        0        0 26867633 2023-06-20 19:33:37.045363 cumulus_library-0.3.0/cumulus_library/studies/vocab/ICD10.bsv
--rw-r--r--   0        0        0  2988766 2023-06-20 19:33:37.057363 cumulus_library-0.3.0/cumulus_library/studies/vocab/ICD9.bsv
--rw-r--r--   0        0        0      404 2023-06-20 19:33:37.057363 cumulus_library-0.3.0/cumulus_library/studies/vocab/icd_legend.sql
--rw-r--r--   0        0        0      138 2023-06-20 19:33:37.057363 cumulus_library-0.3.0/cumulus_library/studies/vocab/manifest.toml
--rw-r--r--   0        0        0     4834 2023-06-20 19:33:37.057363 cumulus_library-0.3.0/cumulus_library/studies/vocab/vocab_icd_builder.py
--rw-r--r--   0        0        0    16090 2023-06-20 19:33:37.057363 cumulus_library-0.3.0/cumulus_library/study_parser.py
--rw-r--r--   0        0        0      577 2023-06-20 19:33:37.057363 cumulus_library-0.3.0/cumulus_library/template_sql/create_view_as.sql.jinja
--rw-r--r--   0        0        0      610 2023-06-20 19:33:37.057363 cumulus_library-0.3.0/cumulus_library/template_sql/ctas.sql.jinja
--rw-r--r--   0        0        0       61 2023-06-20 19:33:37.057363 cumulus_library-0.3.0/cumulus_library/template_sql/drop_view_table.sql.jinja
--rw-r--r--   0        0        0     1800 2023-06-20 19:33:37.057363 cumulus_library-0.3.0/cumulus_library/template_sql/extension_denormalize.sql.jinja
--rw-r--r--   0        0        0      370 2023-06-20 19:33:37.057363 cumulus_library-0.3.0/cumulus_library/template_sql/insert_into.sql.jinja
--rw-r--r--   0        0        0       52 2023-06-20 19:33:37.057363 cumulus_library-0.3.0/cumulus_library/template_sql/show_tables.sql.jinja
--rw-r--r--   0        0        0       54 2023-06-20 19:33:37.057363 cumulus_library-0.3.0/cumulus_library/template_sql/show_views.sql.jinja
--rw-r--r--   0        0        0     6517 2023-06-20 19:33:37.057363 cumulus_library-0.3.0/cumulus_library/template_sql/templates.py
--rw-r--r--   0        0        0     2618 2023-06-20 19:33:37.057363 cumulus_library-0.3.0/cumulus_library/upload.py
--rw-r--r--   0        0        0     1586 2023-06-20 19:33:37.057363 cumulus_library-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1666 1970-01-01 00:00:00.000000 cumulus_library-0.3.0/PKG-INFO
+lrwxr-xr-x   0        0        0        0 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/.sqlfluff -> cumulus_library/.sqlfluff
+-rw-r--r--   0        0        0      421 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/README.md
+-rw-r--r--   0        0        0      866 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/.sqlfluff
+-rw-r--r--   0        0        0        0 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/__init__.py
+-rw-r--r--   0        0        0      628 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/base_runner.py
+-rwxr-xr-x   0        0        0    11070 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/cli.py
+-rw-r--r--   0        0        0     5129 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/cli_parser.py
+-rw-r--r--   0        0        0      272 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/errors.py
+-rw-r--r--   0        0        0     1889 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/helper.py
+-rw-r--r--   0        0        0      205 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/module_allowlist.json
+-rw-r--r--   0        0        0     2343 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/parsers/fhir_valueset.py
+-rw-r--r--   0        0        0        0 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/schema/__init__.py
+-rw-r--r--   0        0        0     4848 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/schema/columns.py
+-rw-r--r--   0        0        0     3346 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/schema/counts.py
+-rw-r--r--   0        0        0     3364 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/schema/typesystem.py
+-rw-r--r--   0        0        0     5876 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/schema/valueset.py
+-rw-r--r--   0        0        0     2962 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/studies/core/condition.sql
+-rw-r--r--   0        0        0     2857 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/studies/core/documentreference.sql
+-rw-r--r--   0        0        0     3294 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/studies/core/encounter.sql
+-rw-r--r--   0        0        0     4126 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/studies/core/fhir_define.sql
+-rw-r--r--   0        0        0      673 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/studies/core/manifest.toml
+-rw-r--r--   0        0        0     1231 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/studies/core/medication_request.sql
+-rw-r--r--   0        0        0     1208 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/studies/core/observation.sql
+-rw-r--r--   0        0        0     2874 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/studies/core/observation_lab.sql
+-rw-r--r--   0        0        0     1272 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/studies/core/observation_vital_signs.sql
+-rw-r--r--   0        0        0     1691 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/studies/core/patient.sql
+-rw-r--r--   0        0        0     2241 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/studies/core/patient_extensions.py
+-rw-r--r--   0        0        0     1426 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/studies/core/setup.sql
+-rw-r--r--   0        0        0     1472 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/studies/core/study_period.sql
+-rw-r--r--   0        0        0      824 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/studies/template/counts.sql
+-rw-r--r--   0        0        0      187 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/studies/template/date_range.sql
+-rw-r--r--   0        0        0      566 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/studies/template/lab_observations.sql
+-rw-r--r--   0        0        0     1562 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/studies/template/manifest.toml
+-rw-r--r--   0        0        0     1142 2023-06-21 20:33:20.887714 cumulus_library-0.3.1/cumulus_library/studies/template/setup.sql
+-rw-r--r--   0        0        0 26867633 2023-06-21 20:33:20.963716 cumulus_library-0.3.1/cumulus_library/studies/vocab/ICD10.bsv
+-rw-r--r--   0        0        0  2988766 2023-06-21 20:33:20.975716 cumulus_library-0.3.1/cumulus_library/studies/vocab/ICD9.bsv
+-rw-r--r--   0        0        0      394 2023-06-21 20:33:20.975716 cumulus_library-0.3.1/cumulus_library/studies/vocab/icd_legend.sql
+-rw-r--r--   0        0        0      138 2023-06-21 20:33:20.975716 cumulus_library-0.3.1/cumulus_library/studies/vocab/manifest.toml
+-rw-r--r--   0        0        0     4824 2023-06-21 20:33:20.975716 cumulus_library-0.3.1/cumulus_library/studies/vocab/vocab_icd_builder.py
+-rw-r--r--   0        0        0    16059 2023-06-21 20:33:20.975716 cumulus_library-0.3.1/cumulus_library/study_parser.py
+-rw-r--r--   0        0        0      577 2023-06-21 20:33:20.975716 cumulus_library-0.3.1/cumulus_library/template_sql/create_view_as.sql.jinja
+-rw-r--r--   0        0        0      610 2023-06-21 20:33:20.975716 cumulus_library-0.3.1/cumulus_library/template_sql/ctas.sql.jinja
+-rw-r--r--   0        0        0       61 2023-06-21 20:33:20.975716 cumulus_library-0.3.1/cumulus_library/template_sql/drop_view_table.sql.jinja
+-rw-r--r--   0        0        0     1800 2023-06-21 20:33:20.975716 cumulus_library-0.3.1/cumulus_library/template_sql/extension_denormalize.sql.jinja
+-rw-r--r--   0        0        0      370 2023-06-21 20:33:20.975716 cumulus_library-0.3.1/cumulus_library/template_sql/insert_into.sql.jinja
+-rw-r--r--   0        0        0       52 2023-06-21 20:33:20.975716 cumulus_library-0.3.1/cumulus_library/template_sql/show_tables.sql.jinja
+-rw-r--r--   0        0        0       54 2023-06-21 20:33:20.975716 cumulus_library-0.3.1/cumulus_library/template_sql/show_views.sql.jinja
+-rw-r--r--   0        0        0     6517 2023-06-21 20:33:20.975716 cumulus_library-0.3.1/cumulus_library/template_sql/templates.py
+-rw-r--r--   0        0        0     2618 2023-06-21 20:33:20.975716 cumulus_library-0.3.1/cumulus_library/upload.py
+-rw-r--r--   0        0        0     1586 2023-06-21 20:33:20.975716 cumulus_library-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1666 1970-01-01 00:00:00.000000 cumulus_library-0.3.1/PKG-INFO
```

### Comparing `cumulus_library-0.3.0/cumulus_library/.sqlfluff` & `cumulus_library-0.3.1/cumulus_library/.sqlfluff`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.0/cumulus_library/base_runner.py` & `cumulus_library-0.3.1/cumulus_library/base_runner.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.0/cumulus_library/cli.py` & `cumulus_library-0.3.1/cumulus_library/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,26 +43,38 @@
 
     verbose = False
     schema_name = None
 
     def __init__(  # pylint: disable=too-many-arguments
         self, region: str, workgroup: str, profile: str, schema: str
     ):
+        connect_kwargs = {}
+        for aws_env_name in [
+            "AWS_ACCESS_KEY_ID",
+            "AWS_SECRET_ACCESS_KEY",
+            "AWS_SESSION_TOKEN",
+        ]:
+            if aws_env_val := os.environ.get(aws_env_name):
+                connect_kwargs[aws_env_name.lower()] = aws_env_val
+        # the profile may not be required, provided the above three AWS env vars
+        # are set. If both are present, the env vars take precedence
+        if profile is not None:
+            connect_kwargs["profile_name"] = profile
         self.cursor = pyathena.connect(
             region_name=region,
             work_group=workgroup,
-            profile_name=profile,
             schema_name=schema,
+            **connect_kwargs,
         ).cursor()
         self.pandas_cursor = pyathena.connect(
             region_name=region,
             work_group=workgroup,
-            profile_name=profile,
             schema_name=schema,
             cursor_class=PandasCursor,
+            **connect_kwargs,
         ).cursor()
         self.schema_name = schema
 
     def reset_data_path(self, study: PosixPath) -> None:
         """
         Removes existing exports from a study's local data dir
         """
@@ -280,15 +292,14 @@
         posix_paths = []
         for path in args["study_dir"]:
             posix_paths.append(get_abs_posix_path(path))
         args["study_dir"] = posix_paths
 
     if args.get("data_path"):
         args["data_path"] = get_abs_posix_path(args["data_path"])
-
     return run_cli(args)
 
 
 def main_cli():  # called by the generated wrapper scripts
     main()
```

### Comparing `cumulus_library-0.3.0/cumulus_library/cli_parser.py` & `cumulus_library-0.3.1/cumulus_library/cli_parser.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.0/cumulus_library/helper.py` & `cumulus_library-0.3.1/cumulus_library/helper.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.0/cumulus_library/parsers/fhir_valueset.py` & `cumulus_library-0.3.1/cumulus_library/parsers/fhir_valueset.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.0/cumulus_library/schema/columns.py` & `cumulus_library-0.3.1/cumulus_library/schema/columns.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.0/cumulus_library/schema/counts.py` & `cumulus_library-0.3.1/cumulus_library/schema/counts.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.0/cumulus_library/schema/typesystem.py` & `cumulus_library-0.3.1/cumulus_library/schema/typesystem.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.0/cumulus_library/schema/valueset.py` & `cumulus_library-0.3.1/cumulus_library/schema/valueset.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.0/cumulus_library/studies/core/condition.sql` & `cumulus_library-0.3.1/cumulus_library/studies/core/condition.sql`

 * *Files 2% similar despite different names*

```diff
@@ -43,28 +43,28 @@
     date_trunc('year', date(tc.recordeddate)) AS recorded_year
 FROM temp_condition AS tc,
     unnest(category) AS t_category (category_coding), --noqa
     unnest(category_coding.coding) AS t_category_coding (category_row), --noqa
     unnest(code.coding) AS t_coding (code_row) --noqa
 WHERE tc.recordeddate BETWEEN date('2016-01-01') AND current_date;
 
-CREATE OR REPLACE VIEW core__join_condition_icd AS
+CREATE TABLE core__join_condition_icd AS
 SELECT
     cc.subject_ref,
     cc.encounter_ref,
     cc.recorded_month AS cond_month,
     ce.enc_class.code AS enc_class_code,
     vil.code AS cond_code,
     vil.code_display AS cond_code_display
 FROM core__condition AS cc, core__encounter AS ce, vocab__icd_legend AS vil
 WHERE
     cc.encounter_ref = ce.encounter_ref
     AND cc.cond_code.coding[1].code = vil.code; --noqa
 
-CREATE OR REPLACE VIEW core__count_condition_icd10_month AS
+CREATE TABLE core__count_condition_icd10_month AS
 WITH powerset AS (
     SELECT
         count(DISTINCT cc.subject_ref) AS cnt_subject,
         count(DISTINCT cc.encounter_ref) AS cnt_encounter,
         vil.code_display,
         cc.recorded_month,
         ce.enc_class
```

### Comparing `cumulus_library-0.3.0/cumulus_library/studies/core/documentreference.sql` & `cumulus_library-0.3.1/cumulus_library/studies/core/documentreference.sql`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     tdr.doc_ref
 FROM temp_documentreference AS tdr,
     unnest(context.encounter) AS context_encounter (encounter), --noqa
     unnest(type.coding) AS type_coding (type_row)
 WHERE author_date BETWEEN date('2016-06-01') AND current_date;
 
 -- count *group by* DocumentReference.type
-CREATE OR REPLACE VIEW core__count_documentreference_month AS
+CREATE TABLE core__count_documentreference_month AS
 WITH powerset AS (
     SELECT
         count(DISTINCT d.subject_ref) AS cnt_subject,
         count(DISTINCT d.encounter_ref) AS cnt_encounter,
         count(DISTINCT d.doc_id) AS cnt_document,
         d.doc_type_display,
         d.author_month,
```

### Comparing `cumulus_library-0.3.0/cumulus_library/studies/core/encounter.sql` & `cumulus_library-0.3.1/cumulus_library/studies/core/encounter.sql`

 * *Files 8% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     e.encounter_ref,
     e.encounter_id
 FROM temp_encounter AS e, core__patient AS p
 WHERE
     e.subject_ref = p.subject_ref
     AND start_date BETWEEN date('2016-06-01') AND current_date;
 
-CREATE OR REPLACE VIEW core__join_encounter_patient AS
+CREATE TABLE core__join_encounter_patient AS
 SELECT
     ce.enc_class,
     ce.enc_type,
     ce.age_at_visit,
     ce.start_date,
     ce.end_date,
     ce.start_week,
@@ -54,55 +54,52 @@
     cp.race_display,
     cp.ethnicity_display,
     cp.postalcode3
 FROM core__encounter AS ce, core__patient AS cp
 WHERE ce.subject_ref = cp.subject_ref;
 
 
-CREATE OR REPLACE VIEW core__count_encounter_month AS
+CREATE TABLE core__count_encounter_month AS
 WITH powerset AS (
     SELECT
         count(DISTINCT ce.subject_ref) AS cnt_subject,
         count(DISTINCT ce.encounter_id) AS cnt_encounter,
         ce.enc_class.code AS enc_class_code,
         ce.start_month,
         ce.age_at_visit,
         cp.gender,
         cp.race_display,
-        cp.ethnicity_display,
-        cp.postalcode3
+        cp.ethnicity_display
     FROM core__encounter AS ce, core__patient AS cp
     WHERE ce.subject_ref = cp.subject_ref
     GROUP BY
         cube(
             ce.enc_class,
             ce.start_month,
             ce.age_at_visit,
             cp.gender,
             cp.race_display,
-            cp.ethnicity_display,
-            cp.postalcode3
+            cp.ethnicity_display
         )
 )
 
 SELECT DISTINCT
     powerset.cnt_encounter AS cnt,
     powerset.enc_class_code,
     powerset.start_month,
     powerset.age_at_visit,
     powerset.gender,
     powerset.race_display,
-    powerset.ethnicity_display,
-    powerset.postalcode3
+    powerset.ethnicity_display
 FROM powerset
 WHERE powerset.cnt_subject >= 10
 ORDER BY
     powerset.start_month ASC, powerset.enc_class_code ASC, powerset.age_at_visit ASC;
 
-CREATE OR REPLACE VIEW core__count_encounter_day AS
+CREATE TABLE core__count_encounter_day AS
 WITH powerset AS (
     SELECT
         count(DISTINCT ce.subject_ref) AS cnt_subject,
         count(DISTINCT ce.encounter_id) AS cnt_encounter,
         ce.enc_class.code AS enc_class_code,
         ce.start_date
     FROM core__encounter AS ce, core__patient AS cp
```

### Comparing `cumulus_library-0.3.0/cumulus_library/studies/core/fhir_define.sql` & `cumulus_library-0.3.1/cumulus_library/studies/core/fhir_define.sql`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 -- ############################################################
 -- FHIR Terminology
 
-CREATE OR REPLACE VIEW core__fhir_vocab AS SELECT * FROM
+CREATE TABLE core__fhir_vocab AS SELECT * FROM
     (
         VALUES
         ('ICD10', 'http://hl7.org/fhir/sid/icd-10-cm'),
         ('ICD10', '2.16.840.1.113883.6.90'),
         ('ICD10', 'ICD10'),
         ('ICD10', 'ICD-10'),
         ('ICD10', 'ICD-10-CM'),
@@ -39,15 +39,15 @@
         ('CPT', 'http://www.ama-assn.org/go/cpt'),
         ('CPT', 'CPT')
     ) AS t (alias, vocab); --noqa: AL05
 
 -- ############################################################
 -- FHIR StructureDefinition
 
-CREATE OR REPLACE VIEW core__fhir_define AS
+CREATE TABLE core__fhir_define AS
 SELECT * FROM
     (
         VALUES
         (
             'Patient',
             'http://hl7.org/fhir/us/core/StructureDefinition/us-core-patient'
         ),
```

### Comparing `cumulus_library-0.3.0/cumulus_library/studies/core/manifest.toml` & `cumulus_library-0.3.1/cumulus_library/studies/core/manifest.toml`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.0/cumulus_library/studies/core/medication_request.sql` & `cumulus_library-0.3.1/cumulus_library/studies/core/medication_request.sql`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     mr.id AS med_admin_id,
     mr.subject.reference AS subject_id
 FROM medicationrequest AS mr,
     unnest(mr.medicationcodeableconcept.coding) AS t (med_coding) --noqa: AL05
 WHERE med_coding.system = 'http://www.nlm.nih.gov/research/umls/rxnorm';
 
 
-CREATE OR REPLACE VIEW core__count_medicationrequest_month AS
+CREATE TABLE core__count_medicationrequest_month AS
 WITH powerset AS (
     SELECT
         count(DISTINCT cmr.subject_id) AS cnt_subject,
         cmr.status,
         cmr.intent,
         cmr.authoredon_month,
         cmr.display
```

### Comparing `cumulus_library-0.3.0/cumulus_library/studies/core/observation.sql` & `cumulus_library-0.3.1/cumulus_library/studies/core/observation.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.0/cumulus_library/studies/core/observation_lab.sql` & `cumulus_library-0.3.1/cumulus_library/studies/core/observation_lab.sql`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     unnest(code.coding) AS t_coding (code_row),
     unnest(valuecodeableconcept.coding) AS t_vcc (value_concept_row)
 WHERE tol.effectivedatetime BETWEEN date('2016-06-01') AND current_date;
 
 -- ###########################################################################
 -- COUNT Patients, Encounters, Lab Results
 -- ###########################################################################
-CREATE OR REPLACE VIEW core__count_observation_lab_month AS
+CREATE TABLE core__count_observation_lab_month AS
 WITH powerset AS (
     SELECT
         count(DISTINCT o.subject_ref) AS cnt_subject,
         count(DISTINCT o.encounter_ref) AS cnt_encounter,
         count(DISTINCT o.observation_id) AS cnt_observation,
         o.lab_month,
         o.lab_code,
```

### Comparing `cumulus_library-0.3.0/cumulus_library/studies/core/observation_vital_signs.sql` & `cumulus_library-0.3.1/cumulus_library/studies/core/observation_vital_signs.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.0/cumulus_library/studies/core/patient.sql` & `cumulus_library-0.3.1/cumulus_library/studies/core/patient.sql`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     unnest(tp.address) AS t_address (addr_row) --noqa: AL05
 
 WHERE
     tp.birthdate IS NOT NULL
     AND tp.gender IS NOT NULL;
 
 
-CREATE OR REPLACE VIEW core__count_patient AS
+CREATE TABLE core__count_patient AS
 WITH powerset AS (
     SELECT
         count(DISTINCT cp.subject_ref) AS cnt_subject,
         cp.gender,
         cp.age,
         cp.race_display,
         cp.ethnicity_display
```

### Comparing `cumulus_library-0.3.0/cumulus_library/studies/core/patient_extensions.py` & `cumulus_library-0.3.1/cumulus_library/studies/core/patient_extensions.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.0/cumulus_library/studies/core/setup.sql` & `cumulus_library-0.3.1/cumulus_library/studies/core/setup.sql`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 -- Emergency Department Notes
 --
-CREATE OR REPLACE VIEW core__ed_note AS
+CREATE TABLE core__ed_note AS
 SELECT
     t.from_system,
     t.from_code,
     t.analyte,
     t.system,
     t.code,
     t.display
```

### Comparing `cumulus_library-0.3.0/cumulus_library/studies/core/study_period.sql` & `cumulus_library-0.3.1/cumulus_library/studies/core/study_period.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.0/cumulus_library/studies/template/counts.sql` & `cumulus_library-0.3.1/cumulus_library/studies/template/counts.sql`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-CREATE OR REPLACE VIEW template__count_influenza_test_month AS
+CREATE TABLE template__count_influenza_test_month AS
 WITH powerset AS (
     SELECT
         count(DISTINCT tflo.subject_ref) AS cnt_subject,
         count(DISTINCT tflo.encounter_ref) AS cnt_encounter,
         tflo.influenza_test_code AS influenza_lab_code,
         upper(tflo.influenza_test_result.display) AS influenza_result_display,
         tflo.influenza_test_month
```

### Comparing `cumulus_library-0.3.0/cumulus_library/studies/template/lab_observations.sql` & `cumulus_library-0.3.1/cumulus_library/studies/template/lab_observations.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.0/cumulus_library/studies/template/manifest.toml` & `cumulus_library-0.3.1/cumulus_library/studies/template/manifest.toml`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.0/cumulus_library/studies/template/setup.sql` & `cumulus_library-0.3.1/cumulus_library/studies/template/setup.sql`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-CREATE OR REPLACE VIEW template__influenza_codes AS
+CREATE TABLE template__influenza_codes AS
 SELECT
     t.from_system,
     t.analyte,
     t.system,
     t.code,
     t.display
 FROM
```

### Comparing `cumulus_library-0.3.0/cumulus_library/studies/vocab/ICD10.bsv` & `cumulus_library-0.3.1/cumulus_library/studies/vocab/ICD10.bsv`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.0/cumulus_library/studies/vocab/ICD9.bsv` & `cumulus_library-0.3.1/cumulus_library/studies/vocab/ICD9.bsv`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.0/cumulus_library/studies/vocab/vocab_icd_builder.py` & `cumulus_library-0.3.1/cumulus_library/studies/vocab/vocab_icd_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """ Module for directly loading ICD bsvs into athena tables """
 import csv
 
 from pathlib import Path
 
-from rich.progress import Progress
-
 from cumulus_library.base_runner import BaseRunner
-from cumulus_library.helper import query_console_output
+from cumulus_library.helper import query_console_output, get_progress_bar
 from cumulus_library.template_sql.templates import (
     get_ctas_query,
     get_insert_into_query,
 )
 
 
 class VocabIcdRunner(BaseRunner):
@@ -45,15 +43,15 @@
         path = Path(__file__).parent
         query_count = 1  # accounts for static CTAS query
         for filename in icd_files:
             query_count += (
                 sum(1 for i in open(f"{path}/{filename}.bsv", "rb")) / partition_size
             )
 
-        with Progress(disable=verbose) as progress:
+        with get_progress_bar(disable=verbose) as progress:
             task = progress.add_task(
                 f"Uploading {table_name} data...",
                 total=query_count,
                 visible=not verbose,
             )
             self.build_vocab_icd(
                 self,
```

### Comparing `cumulus_library-0.3.0/cumulus_library/study_parser.py` & `cumulus_library-0.3.1/cumulus_library/study_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from typing import List, Optional
 
 import toml
 
 from rich.progress import Progress, TaskID, track
 
 from cumulus_library.base_runner import BaseRunner
+from cumulus_library.errors import StudyManifestParsingError
 from cumulus_library.helper import (
     query_console_output,
     load_text,
     parse_sql,
     get_progress_bar,
 )
 from cumulus_library.template_sql.templates import (
@@ -24,18 +25,14 @@
 )
 
 StrList = List[str]
 
 RESERVED_TABLE_KEYWORDS = ["etl", "nlp", "lib"]
 
 
-class StudyManifestParsingError(Exception):
-    """Basic error for StudyManifestParser"""
-
-
 class StudyManifestParser:
     """Handles loading of study data from manifest files.
 
     The goal of this class is to make it so that a researcher can contribute a study
     definition without touching the main python infrastructure. It provides
     mechanisms for IDing studies/files of interest, and for executing queries, but
     specifically it should never be in charge of instantiation a cursor itself -
```

### Comparing `cumulus_library-0.3.0/cumulus_library/template_sql/create_view_as.sql.jinja` & `cumulus_library-0.3.1/cumulus_library/template_sql/create_view_as.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.0/cumulus_library/template_sql/ctas.sql.jinja` & `cumulus_library-0.3.1/cumulus_library/template_sql/ctas.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.0/cumulus_library/template_sql/extension_denormalize.sql.jinja` & `cumulus_library-0.3.1/cumulus_library/template_sql/extension_denormalize.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.0/cumulus_library/template_sql/templates.py` & `cumulus_library-0.3.1/cumulus_library/template_sql/templates.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.0/cumulus_library/upload.py` & `cumulus_library-0.3.1/cumulus_library/upload.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.0/pyproject.toml` & `cumulus_library-0.3.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "cumulus-library"
-version = "0.3.0"
+version = "0.3.1"
 # In order to support 3.12, we wil need to refactor out load_module, which is
 # targeted for deprecation in that version.
 requires-python = ">= 3.9, <3.12"
 dependencies = [
     "ctakesclient >= 1.3",
     "fhirclient >= 4.1",
     "Jinja2 > 3",
```

### Comparing `cumulus_library-0.3.0/PKG-INFO` & `cumulus_library-0.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cumulus-library
-Version: 0.3.0
+Version: 0.3.1
 Summary: Clinical study SQL generation for data derived from bulk FHIR
 Keywords: FHIR,SQL,Health Informatics
 Requires-Python: >= 3.9, <3.12
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

