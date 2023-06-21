# Comparing `tmp/metldata-0.3.3.tar.gz` & `tmp/metldata-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metldata-0.3.3.tar", last modified: Tue Jun 20 13:39:26 2023, max compression
+gzip compressed data, was "metldata-0.3.5.tar", last modified: Wed Jun 21 15:49:17 2023, max compression
```

## Comparing `metldata-0.3.3.tar` & `metldata-0.3.5.tar`

### file list

```diff
@@ -1,188 +1,188 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:39:26.110925 metldata-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-06-20 13:39:16.000000 metldata-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18300 2023-06-20 13:39:26.110925 metldata-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17604 2023-06-20 13:39:16.000000 metldata-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:39:26.094925 metldata-0.3.3/metldata/
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:39:26.094925 metldata-0.3.3/metldata/accession_registry/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/accession_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/accession_registry/accession_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/accession_registry/accession_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/accession_registry/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:39:26.094925 metldata-0.3.3/metldata/artifacts_rest/
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/artifacts_rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/artifacts_rest/api_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/artifacts_rest/artifact_dao.py
--rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/artifacts_rest/artifact_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/artifacts_rest/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/artifacts_rest/load_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/artifacts_rest/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/artifacts_rest/query_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:39:26.094925 metldata-0.3.3/metldata/builtin_transformations/
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/builtin_transformations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:39:26.094925 metldata-0.3.3/metldata/builtin_transformations/add_accessions/
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/builtin_transformations/add_accessions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/builtin_transformations/add_accessions/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/builtin_transformations/add_accessions/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/builtin_transformations/add_accessions/metadata_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/builtin_transformations/add_accessions/model_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:39:26.094925 metldata-0.3.3/metldata/builtin_transformations/custom_embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/builtin_transformations/custom_embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/builtin_transformations/custom_embeddings/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/builtin_transformations/custom_embeddings/embedding_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/builtin_transformations/custom_embeddings/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/builtin_transformations/custom_embeddings/metadata_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     8517 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/builtin_transformations/custom_embeddings/model_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:39:26.098925 metldata-0.3.3/metldata/builtin_transformations/delete_slots/
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/builtin_transformations/delete_slots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/builtin_transformations/delete_slots/assumptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/builtin_transformations/delete_slots/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/builtin_transformations/delete_slots/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/builtin_transformations/delete_slots/metadata_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/builtin_transformations/delete_slots/model_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:39:26.098925 metldata-0.3.3/metldata/builtin_transformations/infer_references/
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/builtin_transformations/infer_references/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/builtin_transformations/infer_references/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/builtin_transformations/infer_references/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/builtin_transformations/infer_references/metadata_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/builtin_transformations/infer_references/model_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:39:26.098925 metldata-0.3.3/metldata/builtin_transformations/infer_references/path/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/builtin_transformations/infer_references/path/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/builtin_transformations/infer_references/path/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/builtin_transformations/infer_references/path/path_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/builtin_transformations/infer_references/path/path_str.py
--rw-r--r--   0 runner    (1001) docker     (123)     8736 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/builtin_transformations/infer_references/path/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/builtin_transformations/infer_references/reference.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:39:26.098925 metldata-0.3.3/metldata/builtin_transformations/merge_slots/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/builtin_transformations/merge_slots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/builtin_transformations/merge_slots/assumptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/builtin_transformations/merge_slots/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/builtin_transformations/merge_slots/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/builtin_transformations/merge_slots/metadata_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/builtin_transformations/merge_slots/model_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/builtin_transformations/merge_slots/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:39:26.098925 metldata-0.3.3/metldata/builtin_workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/builtin_workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/builtin_workflows/ghga_archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/combined.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/custom_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:39:26.098925 metldata-0.3.3/metldata/event_handling/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/event_handling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/event_handling/artifact_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/event_handling/event_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/event_handling/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/event_handling/submission_events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:39:26.102925 metldata-0.3.3/metldata/load/
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/load/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/load/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/load/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/load/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/load/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/load/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/load/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/load/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/load/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     9384 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/metadata_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:39:26.102925 metldata-0.3.3/metldata/model_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/model_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/model_utils/anchors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/model_utils/assumptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/model_utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/model_utils/essentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/model_utils/identifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/model_utils/manipulate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/model_utils/metadata_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:39:26.102925 metldata-0.3.3/metldata/submission_registry/
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/submission_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/submission_registry/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/submission_registry/event_publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/submission_registry/identifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/submission_registry/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/submission_registry/submission_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/submission_registry/submission_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:39:26.102925 metldata-0.3.3/metldata/transform/
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/transform/artifact_publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/transform/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/transform/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9449 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/transform/handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/transform/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-20 13:39:16.000000 metldata-0.3.3/metldata/transform/source_event_subscriber.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:39:26.094925 metldata-0.3.3/metldata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18300 2023-06-20 13:39:26.000000 metldata-0.3.3/metldata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6524 2023-06-20 13:39:26.000000 metldata-0.3.3/metldata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 13:39:26.000000 metldata-0.3.3/metldata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-20 13:39:26.000000 metldata-0.3.3/metldata.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 13:39:25.000000 metldata-0.3.3/metldata.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-20 13:39:26.000000 metldata-0.3.3/metldata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 13:39:26.000000 metldata-0.3.3/metldata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-20 13:39:26.110925 metldata-0.3.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-06-20 13:39:16.000000 metldata-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:39:26.102925 metldata-0.3.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:39:26.102925 metldata-0.3.3/tests/accession_registry/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/accession_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/accession_registry/test_accession_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/accession_registry/test_accession_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:39:26.106925 metldata-0.3.3/tests/artifact_rest/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/artifact_rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/artifact_rest/test_api_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/artifact_rest/test_artifact_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/artifact_rest/test_load_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/artifact_rest/test_query_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:39:26.106925 metldata-0.3.3/tests/builtin_tranformations/
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/builtin_tranformations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:39:26.106925 metldata-0.3.3/tests/builtin_tranformations/infer_references/
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/builtin_tranformations/infer_references/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:39:26.106925 metldata-0.3.3/tests/builtin_tranformations/infer_references/path/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/builtin_tranformations/infer_references/path/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/builtin_tranformations/infer_references/path/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/builtin_tranformations/infer_references/path/test_path.py
--rw-r--r--   0 runner    (1001) docker     (123)    10233 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/builtin_tranformations/infer_references/path/test_path_str.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:39:26.106925 metldata-0.3.3/tests/builtin_tranformations/merge_slots/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/builtin_tranformations/merge_slots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/builtin_tranformations/merge_slots/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/builtin_tranformations/merge_slots/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/builtin_tranformations/test_happy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:39:26.106925 metldata-0.3.3/tests/builtin_workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/builtin_workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/builtin_workflows/test_happy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:39:26.106925 metldata-0.3.3/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/fixtures/artifact_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/fixtures/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/fixtures/event_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/fixtures/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/fixtures/metadata_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/fixtures/transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/fixtures/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/fixtures/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:39:26.106925 metldata-0.3.3/tests/load/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/load/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/load/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/load/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:39:26.106925 metldata-0.3.3/tests/model_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/model_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/model_utils/test_anchor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/model_utils/test_assumptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/model_utils/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/model_utils/test_essentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/model_utils/test_identifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7201 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/model_utils/test_manipulate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/model_utils/test_metadata_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:39:26.110925 metldata-0.3.3/tests/submission_registry/
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/submission_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/submission_registry/test_event_publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/submission_registry/test_identifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/submission_registry/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8824 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/submission_registry/test_submission_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/submission_registry/test_submission_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/test_event_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/test_metadata_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:39:26.110925 metldata-0.3.3/tests/transform/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7115 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/transform/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/transform/test_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-20 13:39:16.000000 metldata-0.3.3/tests/transform/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:49:17.783540 metldata-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-06-21 15:49:08.000000 metldata-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18300 2023-06-21 15:49:17.783540 metldata-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17604 2023-06-21 15:49:08.000000 metldata-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:49:17.747539 metldata-0.3.5/metldata/
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:49:17.751539 metldata-0.3.5/metldata/accession_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/accession_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/accession_registry/accession_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/accession_registry/accession_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/accession_registry/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:49:17.751539 metldata-0.3.5/metldata/artifacts_rest/
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/artifacts_rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/artifacts_rest/api_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/artifacts_rest/artifact_dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/artifacts_rest/artifact_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/artifacts_rest/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/artifacts_rest/load_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/artifacts_rest/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/artifacts_rest/query_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:49:17.751539 metldata-0.3.5/metldata/builtin_transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/builtin_transformations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:49:17.751539 metldata-0.3.5/metldata/builtin_transformations/add_accessions/
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/builtin_transformations/add_accessions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/builtin_transformations/add_accessions/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/builtin_transformations/add_accessions/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/builtin_transformations/add_accessions/metadata_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/builtin_transformations/add_accessions/model_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:49:17.755540 metldata-0.3.5/metldata/builtin_transformations/custom_embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/builtin_transformations/custom_embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/builtin_transformations/custom_embeddings/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/builtin_transformations/custom_embeddings/embedding_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/builtin_transformations/custom_embeddings/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/builtin_transformations/custom_embeddings/metadata_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8517 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/builtin_transformations/custom_embeddings/model_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:49:17.755540 metldata-0.3.5/metldata/builtin_transformations/delete_slots/
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/builtin_transformations/delete_slots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/builtin_transformations/delete_slots/assumptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/builtin_transformations/delete_slots/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/builtin_transformations/delete_slots/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/builtin_transformations/delete_slots/metadata_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/builtin_transformations/delete_slots/model_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:49:17.759539 metldata-0.3.5/metldata/builtin_transformations/infer_references/
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/builtin_transformations/infer_references/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/builtin_transformations/infer_references/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/builtin_transformations/infer_references/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/builtin_transformations/infer_references/metadata_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/builtin_transformations/infer_references/model_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:49:17.759539 metldata-0.3.5/metldata/builtin_transformations/infer_references/path/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/builtin_transformations/infer_references/path/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/builtin_transformations/infer_references/path/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/builtin_transformations/infer_references/path/path_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/builtin_transformations/infer_references/path/path_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8736 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/builtin_transformations/infer_references/path/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/builtin_transformations/infer_references/reference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:49:17.759539 metldata-0.3.5/metldata/builtin_transformations/merge_slots/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/builtin_transformations/merge_slots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/builtin_transformations/merge_slots/assumptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/builtin_transformations/merge_slots/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/builtin_transformations/merge_slots/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/builtin_transformations/merge_slots/metadata_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/builtin_transformations/merge_slots/model_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/builtin_transformations/merge_slots/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:49:17.759539 metldata-0.3.5/metldata/builtin_workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/builtin_workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/builtin_workflows/ghga_archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/combined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/custom_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:49:17.763539 metldata-0.3.5/metldata/event_handling/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/event_handling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/event_handling/artifact_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/event_handling/event_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/event_handling/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/event_handling/submission_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:49:17.763539 metldata-0.3.5/metldata/load/
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/load/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/load/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/load/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/load/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/load/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/load/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/load/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/load/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/load/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9384 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/metadata_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:49:17.767540 metldata-0.3.5/metldata/model_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/model_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/model_utils/anchors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/model_utils/assumptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/model_utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/model_utils/essentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/model_utils/identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/model_utils/manipulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/model_utils/metadata_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:49:17.767540 metldata-0.3.5/metldata/submission_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/submission_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/submission_registry/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/submission_registry/event_publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/submission_registry/identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/submission_registry/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/submission_registry/submission_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/submission_registry/submission_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:49:17.771540 metldata-0.3.5/metldata/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/transform/artifact_publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/transform/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/transform/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9449 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/transform/handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/transform/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-21 15:49:08.000000 metldata-0.3.5/metldata/transform/source_event_subscriber.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:49:17.751539 metldata-0.3.5/metldata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18300 2023-06-21 15:49:17.000000 metldata-0.3.5/metldata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6524 2023-06-21 15:49:17.000000 metldata-0.3.5/metldata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 15:49:17.000000 metldata-0.3.5/metldata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-21 15:49:17.000000 metldata-0.3.5/metldata.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 15:49:17.000000 metldata-0.3.5/metldata.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-21 15:49:17.000000 metldata-0.3.5/metldata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-21 15:49:17.000000 metldata-0.3.5/metldata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-21 15:49:17.783540 metldata-0.3.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-06-21 15:49:08.000000 metldata-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:49:17.771540 metldata-0.3.5/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:49:17.771540 metldata-0.3.5/tests/accession_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/accession_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/accession_registry/test_accession_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/accession_registry/test_accession_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:49:17.771540 metldata-0.3.5/tests/artifact_rest/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/artifact_rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/artifact_rest/test_api_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/artifact_rest/test_artifact_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/artifact_rest/test_load_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/artifact_rest/test_query_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:49:17.771540 metldata-0.3.5/tests/builtin_tranformations/
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/builtin_tranformations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:49:17.771540 metldata-0.3.5/tests/builtin_tranformations/infer_references/
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/builtin_tranformations/infer_references/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:49:17.775540 metldata-0.3.5/tests/builtin_tranformations/infer_references/path/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/builtin_tranformations/infer_references/path/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/builtin_tranformations/infer_references/path/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/builtin_tranformations/infer_references/path/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10233 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/builtin_tranformations/infer_references/path/test_path_str.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:49:17.775540 metldata-0.3.5/tests/builtin_tranformations/merge_slots/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/builtin_tranformations/merge_slots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/builtin_tranformations/merge_slots/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/builtin_tranformations/merge_slots/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/builtin_tranformations/test_happy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:49:17.775540 metldata-0.3.5/tests/builtin_workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/builtin_workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/builtin_workflows/test_happy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:49:17.779540 metldata-0.3.5/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/fixtures/artifact_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/fixtures/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/fixtures/event_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/fixtures/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/fixtures/metadata_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/fixtures/transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/fixtures/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/fixtures/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:49:17.779540 metldata-0.3.5/tests/load/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/load/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/load/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/load/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:49:17.779540 metldata-0.3.5/tests/model_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/model_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/model_utils/test_anchor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/model_utils/test_assumptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/model_utils/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/model_utils/test_essentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/model_utils/test_identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7201 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/model_utils/test_manipulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/model_utils/test_metadata_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:49:17.783540 metldata-0.3.5/tests/submission_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/submission_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/submission_registry/test_event_publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/submission_registry/test_identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/submission_registry/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8824 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/submission_registry/test_submission_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/submission_registry/test_submission_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/test_event_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/test_metadata_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:49:17.783540 metldata-0.3.5/tests/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7115 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/transform/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/transform/test_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-06-21 15:49:08.000000 metldata-0.3.5/tests/transform/test_main.py
```

### Comparing `metldata-0.3.3/LICENSE` & `metldata-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/PKG-INFO` & `metldata-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metldata
-Version: 0.3.3
+Version: 0.3.5
 Summary: metldata - A framework for handling metadata based on ETL, CQRS, and event sourcing.
 Home-page: https://github.com/ghga-de/metldata
 Author: German Human Genome Phenome Archive (GHGA)
 Author-email: contact@ghga.de
 License: Apache 2.0
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
@@ -76,29 +76,29 @@
 
 
 ## Installation
 We recommend using the provided Docker container.
 
 A pre-build version is available at [docker hub](https://hub.docker.com/repository/docker/ghga/metldata):
 ```bash
-docker pull ghga/metldata:0.3.3
+docker pull ghga/metldata:0.3.5
 ```
 
 Or you can build the container yourself from the [`./Dockerfile`](./Dockerfile):
 ```bash
 # Execute in the repo's root dir:
-docker build -t ghga/metldata:0.3.3 .
+docker build -t ghga/metldata:0.3.5 .
 ```
 
 For production-ready deployment, we recommend using Kubernetes, however,
 for simple use cases, you could execute the service using docker
 on a single server:
 ```bash
 # The entrypoint is preconfigured:
-docker run -p 8080:8080 ghga/metldata:0.3.3 --help
+docker run -p 8080:8080 ghga/metldata:0.3.5 --help
 ```
 
 If you prefer not to use containers, you may install the service from source:
 ```bash
 # Execute in the repo's root dir:
 pip install .
```

### Comparing `metldata-0.3.3/README.md` & `metldata-0.3.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -58,29 +58,29 @@
 
 
 ## Installation
 We recommend using the provided Docker container.
 
 A pre-build version is available at [docker hub](https://hub.docker.com/repository/docker/ghga/metldata):
 ```bash
-docker pull ghga/metldata:0.3.3
+docker pull ghga/metldata:0.3.5
 ```
 
 Or you can build the container yourself from the [`./Dockerfile`](./Dockerfile):
 ```bash
 # Execute in the repo's root dir:
-docker build -t ghga/metldata:0.3.3 .
+docker build -t ghga/metldata:0.3.5 .
 ```
 
 For production-ready deployment, we recommend using Kubernetes, however,
 for simple use cases, you could execute the service using docker
 on a single server:
 ```bash
 # The entrypoint is preconfigured:
-docker run -p 8080:8080 ghga/metldata:0.3.3 --help
+docker run -p 8080:8080 ghga/metldata:0.3.5 --help
 ```
 
 If you prefer not to use containers, you may install the service from source:
 ```bash
 # Execute in the repo's root dir:
 pip install .
```

### Comparing `metldata-0.3.3/metldata/__init__.py` & `metldata-0.3.5/metldata/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Short description of package"""  # Please adapt to package
 
-__version__ = "0.3.3"
+__version__ = "0.3.5"
```

### Comparing `metldata-0.3.3/metldata/__main__.py` & `metldata-0.3.5/metldata/__main__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/accession_registry/__init__.py` & `metldata-0.3.5/metldata/accession_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/accession_registry/accession_registry.py` & `metldata-0.3.5/metldata/accession_registry/accession_registry.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/accession_registry/accession_store.py` & `metldata-0.3.5/metldata/accession_registry/accession_store.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/accession_registry/config.py` & `metldata-0.3.5/metldata/accession_registry/config.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/artifacts_rest/__init__.py` & `metldata-0.3.5/metldata/artifacts_rest/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/artifacts_rest/api_factory.py` & `metldata-0.3.5/metldata/artifacts_rest/api_factory.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/artifacts_rest/artifact_dao.py` & `metldata-0.3.5/metldata/artifacts_rest/artifact_dao.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/artifacts_rest/artifact_info.py` & `metldata-0.3.5/metldata/artifacts_rest/artifact_info.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/artifacts_rest/config.py` & `metldata-0.3.5/metldata/artifacts_rest/config.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/artifacts_rest/load_resources.py` & `metldata-0.3.5/metldata/artifacts_rest/load_resources.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/artifacts_rest/models.py` & `metldata-0.3.5/metldata/artifacts_rest/models.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/artifacts_rest/query_resources.py` & `metldata-0.3.5/metldata/artifacts_rest/query_resources.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/builtin_transformations/__init__.py` & `metldata-0.3.5/metldata/builtin_transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/builtin_transformations/add_accessions/__init__.py` & `metldata-0.3.5/metldata/builtin_transformations/add_accessions/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/builtin_transformations/add_accessions/config.py` & `metldata-0.3.5/metldata/builtin_transformations/add_accessions/config.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/builtin_transformations/add_accessions/main.py` & `metldata-0.3.5/metldata/builtin_transformations/add_accessions/main.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/builtin_transformations/add_accessions/metadata_transform.py` & `metldata-0.3.5/metldata/builtin_transformations/add_accessions/metadata_transform.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/builtin_transformations/add_accessions/model_transform.py` & `metldata-0.3.5/metldata/builtin_transformations/add_accessions/model_transform.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/builtin_transformations/custom_embeddings/__init__.py` & `metldata-0.3.5/metldata/builtin_transformations/custom_embeddings/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/builtin_transformations/custom_embeddings/config.py` & `metldata-0.3.5/metldata/builtin_transformations/custom_embeddings/config.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/builtin_transformations/custom_embeddings/embedding_profile.py` & `metldata-0.3.5/metldata/builtin_transformations/custom_embeddings/embedding_profile.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/builtin_transformations/custom_embeddings/main.py` & `metldata-0.3.5/metldata/builtin_transformations/custom_embeddings/main.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/builtin_transformations/custom_embeddings/metadata_transform.py` & `metldata-0.3.5/metldata/builtin_transformations/custom_embeddings/metadata_transform.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/builtin_transformations/custom_embeddings/model_transform.py` & `metldata-0.3.5/metldata/builtin_transformations/custom_embeddings/model_transform.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/builtin_transformations/delete_slots/__init__.py` & `metldata-0.3.5/metldata/builtin_transformations/delete_slots/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/builtin_transformations/delete_slots/assumptions.py` & `metldata-0.3.5/metldata/builtin_transformations/delete_slots/assumptions.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/builtin_transformations/delete_slots/config.py` & `metldata-0.3.5/metldata/builtin_transformations/delete_slots/config.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/builtin_transformations/delete_slots/main.py` & `metldata-0.3.5/metldata/builtin_transformations/delete_slots/main.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/builtin_transformations/delete_slots/metadata_transform.py` & `metldata-0.3.5/metldata/builtin_transformations/delete_slots/metadata_transform.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/builtin_transformations/delete_slots/model_transform.py` & `metldata-0.3.5/metldata/builtin_transformations/delete_slots/model_transform.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/builtin_transformations/infer_references/__init__.py` & `metldata-0.3.5/metldata/builtin_transformations/infer_references/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/builtin_transformations/infer_references/config.py` & `metldata-0.3.5/metldata/builtin_transformations/infer_references/config.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/builtin_transformations/infer_references/main.py` & `metldata-0.3.5/metldata/builtin_transformations/infer_references/main.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/builtin_transformations/infer_references/metadata_transform.py` & `metldata-0.3.5/metldata/builtin_transformations/infer_references/metadata_transform.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/builtin_transformations/infer_references/model_transform.py` & `metldata-0.3.5/metldata/builtin_transformations/infer_references/model_transform.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/builtin_transformations/infer_references/path/__init__.py` & `metldata-0.3.5/metldata/builtin_transformations/infer_references/path/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/builtin_transformations/infer_references/path/path.py` & `metldata-0.3.5/metldata/builtin_transformations/infer_references/path/path.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/builtin_transformations/infer_references/path/path_elements.py` & `metldata-0.3.5/metldata/builtin_transformations/infer_references/path/path_elements.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/builtin_transformations/infer_references/path/path_str.py` & `metldata-0.3.5/metldata/builtin_transformations/infer_references/path/path_str.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/builtin_transformations/infer_references/path/resolve.py` & `metldata-0.3.5/metldata/builtin_transformations/infer_references/path/resolve.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/builtin_transformations/infer_references/reference.py` & `metldata-0.3.5/metldata/builtin_transformations/infer_references/reference.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/builtin_transformations/merge_slots/__init__.py` & `metldata-0.3.5/metldata/builtin_transformations/merge_slots/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/builtin_transformations/merge_slots/assumptions.py` & `metldata-0.3.5/metldata/builtin_transformations/merge_slots/assumptions.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/builtin_transformations/merge_slots/config.py` & `metldata-0.3.5/metldata/builtin_transformations/merge_slots/config.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/builtin_transformations/merge_slots/main.py` & `metldata-0.3.5/metldata/builtin_transformations/merge_slots/main.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/builtin_transformations/merge_slots/metadata_transform.py` & `metldata-0.3.5/metldata/builtin_transformations/merge_slots/metadata_transform.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/builtin_transformations/merge_slots/model_transform.py` & `metldata-0.3.5/metldata/builtin_transformations/merge_slots/model_transform.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/builtin_transformations/merge_slots/models.py` & `metldata-0.3.5/metldata/builtin_transformations/merge_slots/models.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/builtin_workflows/__init__.py` & `metldata-0.3.5/metldata/builtin_workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/builtin_workflows/ghga_archive.py` & `metldata-0.3.5/metldata/builtin_workflows/ghga_archive.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/cli.py` & `metldata-0.3.5/metldata/cli.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/combined.py` & `metldata-0.3.5/metldata/combined.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/config.py` & `metldata-0.3.5/metldata/config.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/custom_types.py` & `metldata-0.3.5/metldata/custom_types.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/event_handling/__init__.py` & `metldata-0.3.5/metldata/event_handling/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/event_handling/artifact_events.py` & `metldata-0.3.5/metldata/event_handling/artifact_events.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/event_handling/event_handling.py` & `metldata-0.3.5/metldata/event_handling/event_handling.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/event_handling/models.py` & `metldata-0.3.5/metldata/event_handling/models.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/event_handling/submission_events.py` & `metldata-0.3.5/metldata/event_handling/submission_events.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/load/__init__.py` & `metldata-0.3.5/metldata/load/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/load/api.py` & `metldata-0.3.5/metldata/load/api.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/load/auth.py` & `metldata-0.3.5/metldata/load/auth.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/load/client.py` & `metldata-0.3.5/metldata/load/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,15 +40,17 @@
     event_collector = FileSystemEventCollector(config=config)
     artifacts = collect_artifacts(config=config, event_collector=event_collector)
 
     with httpx.Client() as client:
         response = client.post(
             f"{config.loader_api_root}/rpc/load-artifacts",
             json=artifacts,
-            headers={"Authorization": f"Bearer {token}"},
+            headers={
+                "Authorization": f"Bearer {token}",
+            },
             timeout=60,
         )
 
     if response.status_code != 204:
         raise ArtifactUploadException(
             f"Uploading artifacts failed with status code {response.status_code}."
         )
```

### Comparing `metldata-0.3.3/metldata/load/collect.py` & `metldata-0.3.5/metldata/load/collect.py`

 * *Files 10% similar despite different names*

```diff
@@ -62,10 +62,13 @@
     artifact_resources: ArtifactResourceDict = defaultdict(list)
     for artifact_type in config.artifact_types:
         topic = get_artifact_topic(
             artifact_topic_prefix=config.artifact_topic_prefix,
             artifact_type=artifact_type,
         )
         for event in event_collector.collect_events(topic=topic):
-            artifact_resources[artifact_type].append(event.payload)
+            content = event.payload.get("content")
+            if not content:
+                raise RuntimeError("Artifact does not contain 'content' field.")
+            artifact_resources[artifact_type].append(content)
 
     return artifact_resources
```

### Comparing `metldata-0.3.3/metldata/load/config.py` & `metldata-0.3.5/metldata/load/config.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/load/load.py` & `metldata-0.3.5/metldata/load/load.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/load/main.py` & `metldata-0.3.5/metldata/load/main.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/load/models.py` & `metldata-0.3.5/metldata/load/models.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/metadata_utils.py` & `metldata-0.3.5/metldata/metadata_utils.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/model_utils/__init__.py` & `metldata-0.3.5/metldata/model_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/model_utils/anchors.py` & `metldata-0.3.5/metldata/model_utils/anchors.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/model_utils/assumptions.py` & `metldata-0.3.5/metldata/model_utils/assumptions.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/model_utils/config.py` & `metldata-0.3.5/metldata/model_utils/config.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/model_utils/essentials.py` & `metldata-0.3.5/metldata/model_utils/essentials.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/model_utils/identifiers.py` & `metldata-0.3.5/metldata/model_utils/identifiers.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/model_utils/manipulate.py` & `metldata-0.3.5/metldata/model_utils/manipulate.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/model_utils/metadata_validator.py` & `metldata-0.3.5/metldata/model_utils/metadata_validator.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/submission_registry/config.py` & `metldata-0.3.5/metldata/submission_registry/config.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/submission_registry/event_publisher.py` & `metldata-0.3.5/metldata/submission_registry/event_publisher.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/submission_registry/identifiers.py` & `metldata-0.3.5/metldata/submission_registry/identifiers.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/submission_registry/models.py` & `metldata-0.3.5/metldata/submission_registry/models.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/submission_registry/submission_registry.py` & `metldata-0.3.5/metldata/submission_registry/submission_registry.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/submission_registry/submission_store.py` & `metldata-0.3.5/metldata/submission_registry/submission_store.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/transform/__init__.py` & `metldata-0.3.5/metldata/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/transform/artifact_publisher.py` & `metldata-0.3.5/metldata/transform/artifact_publisher.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,17 +18,19 @@
 
 
 import json
 
 from hexkit.protocols.eventpub import EventPublisherProtocol
 from pydantic import BaseModel
 
-from metldata.event_handling.artifact_events import ArtifactEventConfig
+from metldata.event_handling.artifact_events import (
+    ArtifactEventConfig,
+    get_artifact_topic,
+)
 from metldata.event_handling.models import SubmissionEventPayload
-from metldata.submission_registry import get_artifact_topic
 
 
 class ArtifactEventPublisherConfig(ArtifactEventConfig):
     """Config parameters and their defaults."""
 
 
 class ArtifactEvent(BaseModel):
```

### Comparing `metldata-0.3.3/metldata/transform/base.py` & `metldata-0.3.5/metldata/transform/base.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/transform/config.py` & `metldata-0.3.5/metldata/transform/config.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/transform/handling.py` & `metldata-0.3.5/metldata/transform/handling.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/transform/main.py` & `metldata-0.3.5/metldata/transform/main.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata/transform/source_event_subscriber.py` & `metldata-0.3.5/metldata/transform/source_event_subscriber.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/metldata.egg-info/PKG-INFO` & `metldata-0.3.5/metldata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metldata
-Version: 0.3.3
+Version: 0.3.5
 Summary: metldata - A framework for handling metadata based on ETL, CQRS, and event sourcing.
 Home-page: https://github.com/ghga-de/metldata
 Author: German Human Genome Phenome Archive (GHGA)
 Author-email: contact@ghga.de
 License: Apache 2.0
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
@@ -76,29 +76,29 @@
 
 
 ## Installation
 We recommend using the provided Docker container.
 
 A pre-build version is available at [docker hub](https://hub.docker.com/repository/docker/ghga/metldata):
 ```bash
-docker pull ghga/metldata:0.3.3
+docker pull ghga/metldata:0.3.5
 ```
 
 Or you can build the container yourself from the [`./Dockerfile`](./Dockerfile):
 ```bash
 # Execute in the repo's root dir:
-docker build -t ghga/metldata:0.3.3 .
+docker build -t ghga/metldata:0.3.5 .
 ```
 
 For production-ready deployment, we recommend using Kubernetes, however,
 for simple use cases, you could execute the service using docker
 on a single server:
 ```bash
 # The entrypoint is preconfigured:
-docker run -p 8080:8080 ghga/metldata:0.3.3 --help
+docker run -p 8080:8080 ghga/metldata:0.3.5 --help
 ```
 
 If you prefer not to use containers, you may install the service from source:
 ```bash
 # Execute in the repo's root dir:
 pip install .
```

### Comparing `metldata-0.3.3/metldata.egg-info/SOURCES.txt` & `metldata-0.3.5/metldata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/setup.cfg` & `metldata-0.3.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/setup.py` & `metldata-0.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/tests/accession_registry/__init__.py` & `metldata-0.3.5/tests/accession_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/tests/accession_registry/test_accession_registry.py` & `metldata-0.3.5/tests/accession_registry/test_accession_registry.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/tests/accession_registry/test_accession_store.py` & `metldata-0.3.5/tests/accession_registry/test_accession_store.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/tests/artifact_rest/__init__.py` & `metldata-0.3.5/tests/artifact_rest/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/tests/artifact_rest/test_api_factory.py` & `metldata-0.3.5/tests/artifact_rest/test_api_factory.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/tests/artifact_rest/test_artifact_info.py` & `metldata-0.3.5/tests/artifact_rest/test_artifact_info.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/tests/artifact_rest/test_load_artifacts.py` & `metldata-0.3.5/tests/artifact_rest/test_load_artifacts.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/tests/artifact_rest/test_query_resources.py` & `metldata-0.3.5/tests/artifact_rest/test_query_resources.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/tests/builtin_tranformations/__init__.py` & `metldata-0.3.5/tests/builtin_tranformations/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/tests/builtin_tranformations/infer_references/__init__.py` & `metldata-0.3.5/tests/builtin_tranformations/infer_references/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/tests/builtin_tranformations/infer_references/path/__init__.py` & `metldata-0.3.5/tests/builtin_tranformations/infer_references/path/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/tests/builtin_tranformations/infer_references/path/test_config.py` & `metldata-0.3.5/tests/builtin_tranformations/infer_references/path/test_config.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/tests/builtin_tranformations/infer_references/path/test_path.py` & `metldata-0.3.5/tests/builtin_tranformations/infer_references/path/test_path.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/tests/builtin_tranformations/infer_references/path/test_path_str.py` & `metldata-0.3.5/tests/builtin_tranformations/infer_references/path/test_path_str.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/tests/builtin_tranformations/merge_slots/__init__.py` & `metldata-0.3.5/tests/builtin_tranformations/merge_slots/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/tests/builtin_tranformations/merge_slots/test_config.py` & `metldata-0.3.5/tests/builtin_tranformations/merge_slots/test_config.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/tests/builtin_tranformations/merge_slots/test_models.py` & `metldata-0.3.5/tests/builtin_tranformations/merge_slots/test_models.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/tests/builtin_tranformations/test_happy.py` & `metldata-0.3.5/tests/builtin_tranformations/test_happy.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/tests/builtin_workflows/__init__.py` & `metldata-0.3.5/tests/builtin_workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/tests/builtin_workflows/test_happy.py` & `metldata-0.3.5/tests/builtin_workflows/test_happy.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/tests/fixtures/__init__.py` & `metldata-0.3.5/tests/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/tests/fixtures/artifact_info.py` & `metldata-0.3.5/tests/fixtures/artifact_info.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/tests/fixtures/config.py` & `metldata-0.3.5/tests/fixtures/config.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/tests/fixtures/event_handling.py` & `metldata-0.3.5/tests/fixtures/event_handling.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/tests/fixtures/metadata.py` & `metldata-0.3.5/tests/fixtures/metadata.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/tests/fixtures/metadata_models.py` & `metldata-0.3.5/tests/fixtures/metadata_models.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/tests/fixtures/transformations.py` & `metldata-0.3.5/tests/fixtures/transformations.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/tests/fixtures/utils.py` & `metldata-0.3.5/tests/fixtures/utils.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/tests/fixtures/workflows.py` & `metldata-0.3.5/tests/fixtures/workflows.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/tests/load/__init__.py` & `metldata-0.3.5/tests/load/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/tests/load/test_client.py` & `metldata-0.3.5/tests/load/test_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         Event(
             topic=get_artifact_topic(
                 artifact_topic_prefix=config.artifact_topic_prefix,
                 artifact_type=artifact_type,
             ),
             type_=artifact_type,
             key=str(uuid4()),  # will later be the submission id
-            payload=artifact_content,
+            payload={"content": artifact_content},
         )
         for artifact_type, artifact_contents in EXAMPLE_ARTIFACTS.items()
         for artifact_content in artifact_contents
     ]
     await file_system_event_fixture.publish_events(artifact_events)
 
     # mock the api:
```

### Comparing `metldata-0.3.3/tests/load/test_main.py` & `metldata-0.3.5/tests/load/test_main.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/tests/model_utils/__init__.py` & `metldata-0.3.5/tests/model_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/tests/model_utils/test_anchor.py` & `metldata-0.3.5/tests/model_utils/test_anchor.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/tests/model_utils/test_assumptions.py` & `metldata-0.3.5/tests/model_utils/test_assumptions.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/tests/model_utils/test_config.py` & `metldata-0.3.5/tests/model_utils/test_config.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/tests/model_utils/test_essentials.py` & `metldata-0.3.5/tests/model_utils/test_essentials.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/tests/model_utils/test_identifiers.py` & `metldata-0.3.5/tests/model_utils/test_identifiers.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/tests/model_utils/test_manipulate.py` & `metldata-0.3.5/tests/model_utils/test_manipulate.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/tests/model_utils/test_metadata_validator.py` & `metldata-0.3.5/tests/model_utils/test_metadata_validator.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/tests/submission_registry/__init__.py` & `metldata-0.3.5/tests/submission_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/tests/submission_registry/test_event_publisher.py` & `metldata-0.3.5/tests/submission_registry/test_event_publisher.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/tests/submission_registry/test_identifiers.py` & `metldata-0.3.5/tests/submission_registry/test_identifiers.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/tests/submission_registry/test_models.py` & `metldata-0.3.5/tests/submission_registry/test_models.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/tests/submission_registry/test_submission_registry.py` & `metldata-0.3.5/tests/submission_registry/test_submission_registry.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/tests/submission_registry/test_submission_store.py` & `metldata-0.3.5/tests/submission_registry/test_submission_store.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/tests/test_event_handling.py` & `metldata-0.3.5/tests/test_event_handling.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/tests/test_metadata_utils.py` & `metldata-0.3.5/tests/test_metadata_utils.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/tests/transform/__init__.py` & `metldata-0.3.5/tests/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/tests/transform/test_base.py` & `metldata-0.3.5/tests/transform/test_base.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/tests/transform/test_handling.py` & `metldata-0.3.5/tests/transform/test_handling.py`

 * *Files identical despite different names*

### Comparing `metldata-0.3.3/tests/transform/test_main.py` & `metldata-0.3.5/tests/transform/test_main.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 
 """Test the main module."""
 
 import json
 
 import pytest
 
+from metldata.event_handling.artifact_events import get_artifact_topic
 from metldata.event_handling.models import SubmissionEventPayload
-from metldata.submission_registry import get_artifact_topic
 from metldata.transform.main import (
     TransformationEventHandlingConfig,
     run_workflow_on_all_source_events,
 )
 from tests.fixtures.event_handling import file_system_event_fixture  # noqa: F401
 from tests.fixtures.event_handling import Event, FileSystemEventFixture
 from tests.fixtures.workflows import (
```

