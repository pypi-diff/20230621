# Comparing `tmp/django-gcloud-connectors-0.3.7.tar.gz` & `tmp/django-gcloud-connectors-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-gcloud-connectors-0.3.7.tar", last modified: Wed Jul 20 11:14:40 2022, max compression
+gzip compressed data, was "dist/django-gcloud-connectors-0.4.0.tar", last modified: Wed Jun 21 10:08:17 2023, max compression
```

## Comparing `django-gcloud-connectors-0.3.7.tar` & `django-gcloud-connectors-0.4.0.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 11:14:40.000000 django-gcloud-connectors-0.3.7/
--rw-rw-rw-   0 root         (0) root         (0)     1526 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      184 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1509 2022-07-20 11:14:40.000000 django-gcloud-connectors-0.3.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      829 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 11:14:40.000000 django-gcloud-connectors-0.3.7/django_gcloud_connectors.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1509 2022-07-20 11:14:40.000000 django-gcloud-connectors-0.3.7/django_gcloud_connectors.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3115 2022-07-20 11:14:40.000000 django-gcloud-connectors-0.3.7/django_gcloud_connectors.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-20 11:14:40.000000 django-gcloud-connectors-0.3.7/django_gcloud_connectors.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       98 2022-07-20 11:14:40.000000 django-gcloud-connectors-0.3.7/django_gcloud_connectors.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2022-07-20 11:14:40.000000 django-gcloud-connectors-0.3.7/django_gcloud_connectors.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 11:14:40.000000 django-gcloud-connectors-0.3.7/gcloudc/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 11:14:40.000000 django-gcloud-connectors-0.3.7/gcloudc/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/commands/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 11:14:40.000000 django-gcloud-connectors-0.3.7/gcloudc/commands/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/commands/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 11:14:40.000000 django-gcloud-connectors-0.3.7/gcloudc/commands/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)     5692 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/commands/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      156 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/commands/management/commands/runserver.py
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/commands/management/commands/shell.py
--rw-rw-rw-   0 root         (0) root         (0)      501 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/commands/management/commands/test.py
--rw-rw-rw-   0 root         (0) root         (0)     3697 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/context_decorator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 11:14:40.000000 django-gcloud-connectors-0.3.7/gcloudc/core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1473 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/core/validators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 11:14:40.000000 django-gcloud-connectors-0.3.7/gcloudc/db/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/db/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 11:14:40.000000 django-gcloud-connectors-0.3.7/gcloudc/db/backends/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/db/backends/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 11:14:40.000000 django-gcloud-connectors-0.3.7/gcloudc/db/backends/datastore/
--rw-rw-rw-   0 root         (0) root         (0)      458 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/db/backends/datastore/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    24614 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/db/backends/datastore/base.py
--rw-rw-rw-   0 root         (0) root         (0)     5831 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/db/backends/datastore/caching.py
--rw-rw-rw-   0 root         (0) root         (0)    39246 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/db/backends/datastore/commands.py
--rw-rw-rw-   0 root         (0) root         (0)     3270 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/db/backends/datastore/compiler.py
--rw-rw-rw-   0 root         (0) root         (0)     2247 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/db/backends/datastore/constraints.py
--rw-rw-rw-   0 root         (0) root         (0)    12062 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/db/backends/datastore/context.py
--rw-rw-rw-   0 root         (0) root         (0)      556 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/db/backends/datastore/dbapi.py
--rw-rw-rw-   0 root         (0) root         (0)    12560 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/db/backends/datastore/dnf.py
--rw-rw-rw-   0 root         (0) root         (0)     1818 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/db/backends/datastore/expressions.py
--rw-rw-rw-   0 root         (0) root         (0)     4827 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/db/backends/datastore/formatting.py
--rw-rw-rw-   0 root         (0) root         (0)    33337 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/db/backends/datastore/indexing.py
--rw-rw-rw-   0 root         (0) root         (0)    17917 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/db/backends/datastore/meta_queries.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 11:14:40.000000 django-gcloud-connectors-0.3.7/gcloudc/db/backends/datastore/parsers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/db/backends/datastore/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21257 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/db/backends/datastore/parsers/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1376 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/db/backends/datastore/parsers/version_18.py
--rw-rw-rw-   0 root         (0) root         (0)     5637 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/db/backends/datastore/parsers/version_19.py
--rw-rw-rw-   0 root         (0) root         (0)    24204 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/db/backends/datastore/query.py
--rw-rw-rw-   0 root         (0) root         (0)     1430 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/db/backends/datastore/query_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     5499 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/db/backends/datastore/schema.py
--rw-rw-rw-   0 root         (0) root         (0)    14967 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/db/backends/datastore/transaction.py
--rw-rw-rw-   0 root         (0) root         (0)     3728 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/db/backends/datastore/unique_mixins.py
--rw-rw-rw-   0 root         (0) root         (0)     7310 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/db/backends/datastore/unique_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    16102 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/db/backends/datastore/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      404 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/db/decorators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 11:14:40.000000 django-gcloud-connectors-0.3.7/gcloudc/db/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/db/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 11:14:40.000000 django-gcloud-connectors-0.3.7/gcloudc/db/models/fields/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/db/models/fields/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   290599 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/db/models/fields/allkeys-5.2.0.zip
--rw-rw-rw-   0 root         (0) root         (0)     1843 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/db/models/fields/charfields.py
--rw-rw-rw-   0 root         (0) root         (0)     5603 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/db/models/fields/computed.py
--rw-rw-rw-   0 root         (0) root         (0)    15112 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/db/models/fields/iterable.py
--rw-rw-rw-   0 root         (0) root         (0)     7711 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/db/models/fields/json.py
--rw-rw-rw-   0 root         (0) root         (0)    30847 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/db/models/fields/related.py
--rw-rw-rw-   0 root         (0) root         (0)     2590 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/db/transaction.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 11:14:40.000000 django-gcloud-connectors-0.3.7/gcloudc/forms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/forms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10447 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/forms/fields.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 11:14:40.000000 django-gcloud-connectors-0.3.7/gcloudc/tests/
--rw-rw-rw-   0 root         (0) root         (0)      556 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9807 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/tests/models.py
--rw-rw-rw-   0 root         (0) root         (0)     2736 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/tests/test_async_multi_query.py
--rw-rw-rw-   0 root         (0) root         (0)     9820 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/tests/test_atomic.py
--rw-rw-rw-   0 root         (0) root         (0)      925 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/tests/test_cloud_datastore_runner.py
--rw-rw-rw-   0 root         (0) root         (0)      330 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/tests/test_collation_field.py
--rw-rw-rw-   0 root         (0) root         (0)     1266 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/tests/test_computed_field.py
--rw-rw-rw-   0 root         (0) root         (0)    83494 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/tests/test_connector.py
--rw-rw-rw-   0 root         (0) root         (0)    11266 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/tests/test_db_fields.py
--rw-rw-rw-   0 root         (0) root         (0)     1171 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/tests/test_delete.py
--rw-rw-rw-   0 root         (0) root         (0)      747 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/tests/test_django_interactions.py
--rw-rw-rw-   0 root         (0) root         (0)     1030 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/tests/test_excluding_pks.py
--rw-rw-rw-   0 root         (0) root         (0)    13790 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/tests/test_iterable_fields.py
--rw-rw-rw-   0 root         (0) root         (0)     3947 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/tests/test_json_field.py
--rw-rw-rw-   0 root         (0) root         (0)     1202 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/tests/test_operations.py
--rw-rw-rw-   0 root         (0) root         (0)     2399 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/tests/test_query_by_keys.py
--rw-rw-rw-   0 root         (0) root         (0)    19748 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/tests/test_query_transform.py
--rw-rw-rw-   0 root         (0) root         (0)    25599 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/tests/test_related_fields.py
--rw-rw-rw-   0 root         (0) root         (0)     5653 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/tests/test_transaction_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)    14153 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/tests/test_unique_constraints.py
--rw-rw-rw-   0 root         (0) root         (0)      934 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/gcloudc/utils.py
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-20 11:14:40.000000 django-gcloud-connectors-0.3.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1362 2022-07-20 11:14:30.000000 django-gcloud-connectors-0.3.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 11:14:40.000000 django-gcloud-connectors-0.3.7/test/
--rw-r--r--   0 root         (0) root         (0)     5706 2022-07-20 11:06:53.000000 django-gcloud-connectors-0.3.7/test/404.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 11:14:40.000000 django-gcloud-connectors-0.3.7/test/commercial_support/
--rw-r--r--   0 root         (0) root         (0)     6553 2022-07-20 11:06:53.000000 django-gcloud-connectors-0.3.7/test/commercial_support/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 11:14:40.000000 django-gcloud-connectors-0.3.7/test/concepts_limitations/
--rw-r--r--   0 root         (0) root         (0)    14025 2022-07-20 11:06:53.000000 django-gcloud-connectors-0.3.7/test/concepts_limitations/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 11:14:40.000000 django-gcloud-connectors-0.3.7/test/contributing/
--rw-r--r--   0 root         (0) root         (0)    10760 2022-07-20 11:06:53.000000 django-gcloud-connectors-0.3.7/test/contributing/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 11:14:40.000000 django-gcloud-connectors-0.3.7/test/fields/
--rw-r--r--   0 root         (0) root         (0)    15460 2022-07-20 11:06:53.000000 django-gcloud-connectors-0.3.7/test/fields/index.html
--rw-r--r--   0 root         (0) root         (0)     6780 2022-07-20 11:06:53.000000 django-gcloud-connectors-0.3.7/test/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 11:14:40.000000 django-gcloud-connectors-0.3.7/test/installation/
--rw-r--r--   0 root         (0) root         (0)     7649 2022-07-20 11:06:53.000000 django-gcloud-connectors-0.3.7/test/installation/index.html
--rw-r--r--   0 root         (0) root         (0)     5360 2022-07-20 11:06:53.000000 django-gcloud-connectors-0.3.7/test/search.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 11:14:40.000000 django-gcloud-connectors-0.3.7/test/transactions/
--rw-r--r--   0 root         (0) root         (0)    12467 2022-07-20 11:06:53.000000 django-gcloud-connectors-0.3.7/test/transactions/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 11:14:40.000000 django-gcloud-connectors-0.3.7/test/work_with_potato/
--rw-r--r--   0 root         (0) root         (0)     6225 2022-07-20 11:06:53.000000 django-gcloud-connectors-0.3.7/test/work_with_potato/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 10:08:17.000000 django-gcloud-connectors-0.4.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1526 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      184 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1508 2023-06-21 10:08:17.000000 django-gcloud-connectors-0.4.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      829 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 10:08:17.000000 django-gcloud-connectors-0.4.0/django_gcloud_connectors.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1508 2023-06-21 10:08:17.000000 django-gcloud-connectors-0.4.0/django_gcloud_connectors.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3115 2023-06-21 10:08:17.000000 django-gcloud-connectors-0.4.0/django_gcloud_connectors.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 10:08:17.000000 django-gcloud-connectors-0.4.0/django_gcloud_connectors.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       96 2023-06-21 10:08:17.000000 django-gcloud-connectors-0.4.0/django_gcloud_connectors.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-21 10:08:17.000000 django-gcloud-connectors-0.4.0/django_gcloud_connectors.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 10:08:17.000000 django-gcloud-connectors-0.4.0/gcloudc/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 10:08:17.000000 django-gcloud-connectors-0.4.0/gcloudc/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/commands/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 10:08:17.000000 django-gcloud-connectors-0.4.0/gcloudc/commands/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/commands/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 10:08:17.000000 django-gcloud-connectors-0.4.0/gcloudc/commands/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)     6907 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/commands/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/commands/management/commands/runserver.py
+-rw-rw-rw-   0 root         (0) root         (0)      152 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/commands/management/commands/shell.py
+-rw-rw-rw-   0 root         (0) root         (0)      163 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/commands/management/commands/test.py
+-rw-rw-rw-   0 root         (0) root         (0)     3697 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/context_decorator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 10:08:17.000000 django-gcloud-connectors-0.4.0/gcloudc/core/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1473 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/core/validators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 10:08:17.000000 django-gcloud-connectors-0.4.0/gcloudc/db/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/db/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 10:08:17.000000 django-gcloud-connectors-0.4.0/gcloudc/db/backends/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/db/backends/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 10:08:17.000000 django-gcloud-connectors-0.4.0/gcloudc/db/backends/datastore/
+-rw-rw-rw-   0 root         (0) root         (0)      458 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/db/backends/datastore/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    24666 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/db/backends/datastore/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     5831 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/db/backends/datastore/caching.py
+-rw-rw-rw-   0 root         (0) root         (0)    39798 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/db/backends/datastore/commands.py
+-rw-rw-rw-   0 root         (0) root         (0)     3270 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/db/backends/datastore/compiler.py
+-rw-rw-rw-   0 root         (0) root         (0)     2247 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/db/backends/datastore/constraints.py
+-rw-rw-rw-   0 root         (0) root         (0)    12062 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/db/backends/datastore/context.py
+-rw-rw-rw-   0 root         (0) root         (0)      556 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/db/backends/datastore/dbapi.py
+-rw-rw-rw-   0 root         (0) root         (0)    13219 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/db/backends/datastore/dnf.py
+-rw-rw-rw-   0 root         (0) root         (0)     1818 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/db/backends/datastore/expressions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4827 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/db/backends/datastore/formatting.py
+-rw-rw-rw-   0 root         (0) root         (0)    33337 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/db/backends/datastore/indexing.py
+-rw-rw-rw-   0 root         (0) root         (0)    17917 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/db/backends/datastore/meta_queries.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 10:08:17.000000 django-gcloud-connectors-0.4.0/gcloudc/db/backends/datastore/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/db/backends/datastore/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21415 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/db/backends/datastore/parsers/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1376 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/db/backends/datastore/parsers/version_18.py
+-rw-rw-rw-   0 root         (0) root         (0)     5637 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/db/backends/datastore/parsers/version_19.py
+-rw-rw-rw-   0 root         (0) root         (0)    24424 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/db/backends/datastore/query.py
+-rw-rw-rw-   0 root         (0) root         (0)     1650 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/db/backends/datastore/query_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     5499 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/db/backends/datastore/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    14779 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/db/backends/datastore/transaction.py
+-rw-rw-rw-   0 root         (0) root         (0)     3728 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/db/backends/datastore/unique_mixins.py
+-rw-rw-rw-   0 root         (0) root         (0)     7310 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/db/backends/datastore/unique_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    16233 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/db/backends/datastore/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      404 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/db/decorators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 10:08:17.000000 django-gcloud-connectors-0.4.0/gcloudc/db/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/db/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 10:08:17.000000 django-gcloud-connectors-0.4.0/gcloudc/db/models/fields/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/db/models/fields/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   290599 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/db/models/fields/allkeys-5.2.0.zip
+-rw-rw-rw-   0 root         (0) root         (0)     1843 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/db/models/fields/charfields.py
+-rw-rw-rw-   0 root         (0) root         (0)     5603 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/db/models/fields/computed.py
+-rw-rw-rw-   0 root         (0) root         (0)    15112 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/db/models/fields/iterable.py
+-rw-rw-rw-   0 root         (0) root         (0)     7711 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/db/models/fields/json.py
+-rw-rw-rw-   0 root         (0) root         (0)    30847 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/db/models/fields/related.py
+-rw-rw-rw-   0 root         (0) root         (0)     2590 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/db/transaction.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 10:08:17.000000 django-gcloud-connectors-0.4.0/gcloudc/forms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/forms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10447 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/forms/fields.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 10:08:17.000000 django-gcloud-connectors-0.4.0/gcloudc/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      556 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10122 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/tests/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     2736 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/tests/test_async_multi_query.py
+-rw-rw-rw-   0 root         (0) root         (0)     9820 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/tests/test_atomic.py
+-rw-rw-rw-   0 root         (0) root         (0)      925 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/tests/test_cloud_datastore_runner.py
+-rw-rw-rw-   0 root         (0) root         (0)      330 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/tests/test_collation_field.py
+-rw-rw-rw-   0 root         (0) root         (0)     1266 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/tests/test_computed_field.py
+-rw-rw-rw-   0 root         (0) root         (0)    83494 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/tests/test_connector.py
+-rw-rw-rw-   0 root         (0) root         (0)    12549 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/tests/test_db_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     1171 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/tests/test_delete.py
+-rw-rw-rw-   0 root         (0) root         (0)      747 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/tests/test_django_interactions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2203 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/tests/test_excluding_pks.py
+-rw-rw-rw-   0 root         (0) root         (0)    16541 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/tests/test_iterable_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     3947 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/tests/test_json_field.py
+-rw-rw-rw-   0 root         (0) root         (0)     1202 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/tests/test_operations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2399 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/tests/test_query_by_keys.py
+-rw-rw-rw-   0 root         (0) root         (0)    19748 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/tests/test_query_transform.py
+-rw-rw-rw-   0 root         (0) root         (0)    25599 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/tests/test_related_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     5653 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/tests/test_transaction_hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)    14757 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/tests/test_unique_constraints.py
+-rw-rw-rw-   0 root         (0) root         (0)      934 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/gcloudc/utils.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-21 10:08:17.000000 django-gcloud-connectors-0.4.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1359 2023-06-21 10:08:08.000000 django-gcloud-connectors-0.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 10:08:17.000000 django-gcloud-connectors-0.4.0/test/
+-rw-r--r--   0 root         (0) root         (0)     5738 2023-06-21 10:01:47.000000 django-gcloud-connectors-0.4.0/test/404.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 10:08:17.000000 django-gcloud-connectors-0.4.0/test/commercial_support/
+-rw-r--r--   0 root         (0) root         (0)     6577 2023-06-21 10:01:47.000000 django-gcloud-connectors-0.4.0/test/commercial_support/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 10:08:17.000000 django-gcloud-connectors-0.4.0/test/concepts_limitations/
+-rw-r--r--   0 root         (0) root         (0)    14049 2023-06-21 10:01:47.000000 django-gcloud-connectors-0.4.0/test/concepts_limitations/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 10:08:17.000000 django-gcloud-connectors-0.4.0/test/contributing/
+-rw-r--r--   0 root         (0) root         (0)    13334 2023-06-21 10:01:47.000000 django-gcloud-connectors-0.4.0/test/contributing/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 10:08:17.000000 django-gcloud-connectors-0.4.0/test/fields/
+-rw-r--r--   0 root         (0) root         (0)    15484 2023-06-21 10:01:47.000000 django-gcloud-connectors-0.4.0/test/fields/index.html
+-rw-r--r--   0 root         (0) root         (0)     6804 2023-06-21 10:01:47.000000 django-gcloud-connectors-0.4.0/test/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 10:08:17.000000 django-gcloud-connectors-0.4.0/test/installation/
+-rw-r--r--   0 root         (0) root         (0)     7690 2023-06-21 10:01:47.000000 django-gcloud-connectors-0.4.0/test/installation/index.html
+-rw-r--r--   0 root         (0) root         (0)     5421 2023-06-21 10:01:47.000000 django-gcloud-connectors-0.4.0/test/search.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 10:08:17.000000 django-gcloud-connectors-0.4.0/test/transactions/
+-rw-r--r--   0 root         (0) root         (0)    12491 2023-06-21 10:01:47.000000 django-gcloud-connectors-0.4.0/test/transactions/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 10:08:17.000000 django-gcloud-connectors-0.4.0/test/work_with_potato/
+-rw-r--r--   0 root         (0) root         (0)     6249 2023-06-21 10:01:47.000000 django-gcloud-connectors-0.4.0/test/work_with_potato/index.html
```

### Comparing `django-gcloud-connectors-0.3.7/LICENSE` & `django-gcloud-connectors-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-0.3.7/PKG-INFO` & `django-gcloud-connectors-0.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: django-gcloud-connectors
-Version: 0.3.7
+Version: 0.4.0
 Summary: A Django library for connecting to Google Cloud Datastore from Python 3 runtimes.
 Home-page: https://gitlab.com/potato-oss/google-cloud/django-gcloud-connectors
 Author: Potato London Ltd.
 Author-email: mail@p.ota.to
 License: UNKNOWN
 Keywords: Google Cloud Datastore,Google App Engine,Django
 Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `django-gcloud-connectors-0.3.7/README.md` & `django-gcloud-connectors-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-0.3.7/django_gcloud_connectors.egg-info/PKG-INFO` & `django-gcloud-connectors-0.4.0/django_gcloud_connectors.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: django-gcloud-connectors
-Version: 0.3.7
+Version: 0.4.0
 Summary: A Django library for connecting to Google Cloud Datastore from Python 3 runtimes.
 Home-page: https://gitlab.com/potato-oss/google-cloud/django-gcloud-connectors
 Author: Potato London Ltd.
 Author-email: mail@p.ota.to
 License: UNKNOWN
 Keywords: Google Cloud Datastore,Google App Engine,Django
 Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `django-gcloud-connectors-0.3.7/django_gcloud_connectors.egg-info/SOURCES.txt` & `django-gcloud-connectors-0.4.0/django_gcloud_connectors.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/commands/management/commands/__init__.py` & `django-gcloud-connectors-0.4.0/gcloudc/commands/management/commands/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -29,32 +29,52 @@
 
     def __init__(self, *args, **kwargs):
         self._process = None
         super().__init__(*args, **kwargs)
 
     def add_arguments(self, parser):
         super().add_arguments(parser)
-        parser.add_argument("--no-datastore", action="store_false", dest="datastore", default=True)
+        parser.add_argument(
+            "--use-remote-datastore",
+            action="store_true",
+            dest="use_remote_datastore",
+            default=False,
+            help=(
+                "When set the tests are run against a remote instance of datastore. "
+                "The target GCP project has to be configured by setting GCLOUDC_PROJECT_ID env variable."
+            )
+        )
         parser.add_argument("--datastore-port", action="store", dest="port", default=_DEFAULT_PORT)
         parser.add_argument(
             "--use-memory-datastore",
             action="store_true",
             dest="use_memory_datastore",
             default=self.USE_MEMORY_DATASTORE_BY_DEFAULT,
         )
 
     def execute(self, *args, **kwargs):
-        try:
-            if kwargs.get("datastore", True) and os.environ.get(DJANGO_AUTORELOAD_ENV) != "true":
-                self._check_gcloud_components()
-                self._start_emulator(**kwargs)
-
+        if not kwargs.get("use_remote_datastore"):
+            try:
+                if os.environ.get(DJANGO_AUTORELOAD_ENV) != "true":
+                    self._check_gcloud_components()
+                    self._start_emulator(**kwargs)
+
+                super().execute(*args, **kwargs)
+            finally:
+                self._stop_emulator()
+        else:
+            gcloudc_project_id = os.getenv("GCLOUDC_PROJECT_ID")
+            if not gcloudc_project_id or os.getenv("GCLOUDC_PROJECT_ID") == 'test':
+                raise RuntimeError(
+                    "When setting --use-remote-datastore, you need to set the GCLOUDC_PROJECT_ID.\n"
+                    "Please set the GCLOUDC_PROJECT_ID environment variable to the name of a GCP "
+                    "project you want to use for testing and then set GCLOUDC_PROJECT_ID to its "
+                    "project-id.\nNOTE: All data on that project will be LOST."
+                )
             super().execute(*args, **kwargs)
-        finally:
-            self._stop_emulator()
 
     def _check_gcloud_components(self):
         finished_process = subprocess.run(_COMPONENTS_LIST_COMMAND, stdout=subprocess.PIPE, encoding="utf-8")
         installed_components = set(
             [cp["id"] for cp in json.loads(finished_process.stdout) if cp["current_version_string"] is not None]
         )
 
@@ -64,27 +84,28 @@
                 "Please run `gcloud components install` to install missing components.".format(
                     ", ".join(_REQUIRED_COMPONENTS - installed_components)
                 )
             )
 
     def _datastore_filename(self):
         BASE_DIR = getattr(settings, "BASE_DIR", None)
-
+        logger.info(f"BASEDIR from __init__: {BASE_DIR}")
         if not BASE_DIR:
             raise ImproperlyConfigured("Please define BASE_DIR in your Django settings")
 
         return os.path.join(BASE_DIR, ".datastore")
 
     def _get_args(self, **kwargs):
         args = ["--host-port=127.0.0.1:%s" % kwargs.get("port", _DEFAULT_PORT)]
 
         if kwargs["use_memory_datastore"]:
             logger.info("Using in-memory datastore")
             args.append("--no-store-on-disk")
         else:
+            logger.info(f"Saving data.... to {self._datastore_filename()}")
             args.append("--data-dir=%s" % self._datastore_filename())
 
         return args
 
     def _wait_for_datastore(self, **kwargs):
         TIMEOUT = 60.0
 
@@ -114,14 +135,15 @@
             if (datetime.now() - start).total_seconds() > TIMEOUT:
                 raise RuntimeError("Unable to start Cloud Datastore Emulator. Please check the logs.")
 
             time.sleep(1)
 
     def _start_emulator(self, **kwargs):
         logger.info("Starting Cloud Datastore Emulator")
+        logger.info(f"GCLOUDC_PROJECT_ID: {os.getenv('GCLOUDC_PROJECT_ID', default='test')}")
 
         os.environ["DATASTORE_EMULATOR_HOST"] = "127.0.0.1:%s" % kwargs["port"]
         os.environ["DATASTORE_PROJECT_ID"] = "test"
 
         # The Cloud Datastore emulator regularly runs out of heap space
         # so set a higher max
         os.environ["JDK_JAVA_OPTIONS"] = "-Xms512M -Xmx1024M"
```

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/context_decorator.py` & `django-gcloud-connectors-0.4.0/gcloudc/context_decorator.py`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/core/validators.py` & `django-gcloud-connectors-0.4.0/gcloudc/core/validators.py`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/db/backends/datastore/base.py` & `django-gcloud-connectors-0.4.0/gcloudc/db/backends/datastore/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,14 +179,15 @@
 
     # Datastore will store all integers as 64bit long values
     integer_field_ranges = {
         "SmallIntegerField": (-MAXINT, MAXINT - 1),
         "IntegerField": (-MAXINT, MAXINT - 1),
         "BigIntegerField": (-MAXINT, MAXINT - 1),
         "PositiveSmallIntegerField": (0, MAXINT - 1),
+        "PositiveBigIntegerField": (0, MAXINT - 1),
         "PositiveIntegerField": (0, MAXINT - 1),
         "SmallAutoField": (1, MAXINT - 1),
         "AutoField": (1, MAXINT - 1),
         "BigAutoField": (1, MAXINT - 1),
     }
 
     def bulk_batch_size(self, field, objs):
```

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/db/backends/datastore/caching.py` & `django-gcloud-connectors-0.4.0/gcloudc/db/backends/datastore/caching.py`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/db/backends/datastore/commands.py` & `django-gcloud-connectors-0.4.0/gcloudc/db/backends/datastore/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 )
 
 from django.utils.encoding import (
     force_str,
 )
 from google.cloud.datastore.entity import Entity
 from google.cloud.datastore.key import Key
-from google.cloud.datastore.query import Query
 
 from . import (
     POLYMODEL_CLASS_ATTRIBUTE,
     caching,
     meta_queries,
     transaction,
     utils,
@@ -479,17 +478,22 @@
                 # didn't seem to indicate much of a performance difference, even when doing the pk__in
                 # with GetAsync while the count was running. That might not be true of prod though so
                 # if anyone comes up with a faster idea let me know!
                 if isinstance(query, meta_queries.QueryByKeys):
                     # If this is a QueryByKeys, just do the datastore Get and count the results
                     resultset = (x.key for x in query.fetch(limit=limit, offset=offset) if x)
                 else:
-                    count_query = Query(query._Query__kind, keys_only=True, namespace=self.namespace)
-                    count_query.update(query)
-                    resultset = count_query.Run(limit=limit, offset=offset)
+                    query.keys_only()
+                    resultset = (
+                        # When using __in filter, the key is returned directly.
+                        # When using eq filter, the entity is returned.
+                        # Not sure why. ExcludingPKTests covers both cases.
+                        (x.key if isinstance(x, Entity) else x)
+                        for x in query.fetch(limit=limit, offset=offset)
+                    )
                 self.results = [len([y for y in resultset if y not in excluded_pks])]
                 self.results_returned = 1
             else:
                 query.keys_only()
 
                 self.results = [len(list(query.fetch(limit=limit, offset=offset)))]
                 self.results_returned = 1
@@ -595,32 +599,44 @@
         return
 
     gclient = connection.connection.gclient
     gclient.reserve_ids_sequential(gclient.key(kind, id_or_name, namespace=namespace), 1)
 
 
 def perform_unique_checks(namespace, model, rpc, primary, test_fn):
-    combinations = _unique_combinations(model, ignore_pk=True)
-    for combination in combinations:
+
+    def _test_combination(combination):
+        # We can't `break` two levels at once, hence the nested function
         query = rpc.query(kind=primary.kind, namespace=namespace)
 
         for field in combination:
             col_name = model._meta.get_field(field).column
             value = primary.get(col_name)
             if isinstance(value, list):
+                if not value:
+                    # For lists, empty values are treated as effectively NULL
+                    return
                 for item in value:
                     query.add_filter(col_name, '=', item)
-            elif value is not None:
+            elif value is None:
+                return
+            else:
                 query.add_filter(col_name, '=', value)
 
         # only perform the query if there are filters on it
         if len(query.filters):
             res = list(query.fetch(1))
             if test_fn(res):
-                raise IntegrityError(CONSTRAINT_VIOLATION_MSG.format(model._meta.db_table, ", ".join(combination)))
+                raise IntegrityError(
+                    CONSTRAINT_VIOLATION_MSG.format(model._meta.db_table, ", ".join(combination))
+                )
+
+    combinations = _unique_combinations(model, ignore_pk=True)
+    for combination in combinations:
+        _test_combination(combination)
 
 
 class BulkInsertError(IntegrityError, NotSupportedError):
     pass
 
 
 class BulkDeleteError(IntegrityError, NotSupportedError):
```

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/db/backends/datastore/compiler.py` & `django-gcloud-connectors-0.4.0/gcloudc/db/backends/datastore/compiler.py`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/db/backends/datastore/constraints.py` & `django-gcloud-connectors-0.4.0/gcloudc/db/backends/datastore/constraints.py`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/db/backends/datastore/context.py` & `django-gcloud-connectors-0.4.0/gcloudc/db/backends/datastore/context.py`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/db/backends/datastore/dbapi.py` & `django-gcloud-connectors-0.4.0/gcloudc/db/backends/datastore/dbapi.py`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/db/backends/datastore/dnf.py` & `django-gcloud-connectors-0.4.0/gcloudc/db/backends/datastore/dnf.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 
             elif node.negated and child.operator == "=":
                 # Excluded equalities become inequalities
 
                 lhs, rhs = WhereNode(node.using), WhereNode(node.using)
                 lhs.column = rhs.column = child.column
                 lhs.value = rhs.value = child.value
+                lhs.is_iterable_field = rhs.is_iterable_field = child.is_iterable_field
                 lhs.operator = "<"
                 rhs.operator = ">"
 
                 child.operator = child.value = child.column = None
                 child.connector = "OR"
                 child.children = [lhs, rhs]
 
@@ -58,40 +59,43 @@
                 new_children = []
 
                 for value in child.value:
                     if node.negated:
                         lhs, rhs = WhereNode(node.using), WhereNode(node.using)
                         lhs.column = rhs.column = child.column
                         lhs.value = rhs.value = value
+                        lhs.is_iterable_field = rhs.is_iterable_field = child.is_iterable_field
                         lhs.operator = "<"
                         rhs.operator = ">"
 
                         bridge = WhereNode(node.using)
                         bridge.connector = "OR"
                         bridge.children = [lhs, rhs]
 
                         new_children.append(bridge)
                     else:
                         new_node = WhereNode(node.using)
                         new_node.operator = "="
                         new_node.value = value
                         new_node.column = child.column
+                        new_node.is_iterable_field = child.is_iterable_field
                         new_children.append(new_node)
 
                 child.column = None
                 child.operator = None
                 child.connector = "AND" if negated else "OR"
                 child.value = None
                 child.children = new_children
 
                 assert not child.is_leaf
 
             elif child.operator == "RANGE":
                 lhs, rhs = WhereNode(node.using), WhereNode(node.using)
                 lhs.column = rhs.column = child.column
+                lhs.is_iterable_field = rhs.is_iterable_field = child.is_iterable_field
                 if node.negated:
                     lhs.operator = "<"
                     rhs.operator = ">"
                     child.connector = "OR"
                 else:
                     lhs.operator = ">="
                     rhs.operator = "<="
@@ -282,14 +286,15 @@
             this happens we need to simplify, e.g.:
 
             AND:[username<A],[username<B] -> AND:[username<A]
         """
 
         for and_branch in top_node.children[:]:
             seen = {}
+            preserve = []
 
             altered = False
             for node in and_branch.children:
                 key = (node.column, node.operator)
                 if key in seen:
                     altered = True
 
@@ -303,26 +308,30 @@
                         seen[key].value = max(seen[key].value, node.value, **cmp_kwargs)
                     elif node.operator == "=":
                         if isinstance(node.value, (list, tuple, set)):
                             # Iterable fields can filter on more than one value using
                             # .filter(field__contains=[a, b]), and several such filters can be
                             # applied, which should be combined
                             seen[key].value = list(set(list(seen[key].value) + list(node.value)))
+                        elif node.is_iterable_field:
+                            # This scenario can occur when there are multiple __overlap filters
+                            # on the same field. They should all be kept.
+                            preserve.append(node)
                         else:
                             # Impossible filter! remove the AND branch entirely
                             if and_branch in top_node.children and seen[key].value != node.value:
                                 top_node.children.remove(and_branch)
                             break
                     else:
                         pass
                 else:
                     seen[key] = node
 
             if altered:
-                and_branch.children = [x for x in seen.values()]
+                and_branch.children = [x for x in seen.values()] + preserve
 
         # If all the OR clause are impossible filters we end up with no filters
         # at all, which is incorrect
         if not top_node.children:
             raise EmptyResultSet()
 
     remove_unnecessary_nodes(query.where)
```

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/db/backends/datastore/expressions.py` & `django-gcloud-connectors-0.4.0/gcloudc/db/backends/datastore/expressions.py`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/db/backends/datastore/formatting.py` & `django-gcloud-connectors-0.4.0/gcloudc/db/backends/datastore/formatting.py`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/db/backends/datastore/indexing.py` & `django-gcloud-connectors-0.4.0/gcloudc/db/backends/datastore/indexing.py`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/db/backends/datastore/meta_queries.py` & `django-gcloud-connectors-0.4.0/gcloudc/db/backends/datastore/meta_queries.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,14 @@
         threads = []
 
         # We need to grab a set of results per query
         result_queues = [None] * len(self._queries)
 
         # Go through the queries, trigger new threads as they become available
         for i, query in enumerate(self._queries):
-
             # Iterate while we have a full thread list
             while len(threads) >= self.THREAD_COUNT:
                 try:
                     complete = next(x for x in threads if x.results_fetched)
                 except StopIteration:
                     # No threads available, continue waiting
                     continue
@@ -177,15 +176,15 @@
 
             This calls _fetch_results which returns a list of iterators,
             where each is the result of a single query. This function does a
             zig-zag merge of the entities. It starts by creating a list of the next
             entry in each resultset, then iteratively picks the next entity and then
             fills the slot from the counterpart result set until all the slots are None.
         """
-        self._min_max_cache = []
+        self._min_max_cache = {}
 
         # We have to assume that one branch might return all the results and as
         # offsetting is done by skipping results we need to get offset + limit results
         # from each branch
         results = self._fetch_results(limit=(offset or 0) + limit if limit is not None else None)
 
         # Go through each outstanding result queue and store
@@ -322,15 +321,15 @@
         cache_results = True
         results = None
 
         if key_count == 1:
             # FIXME: Potentially could use get_multi in memcache and the make a query
             # for whatever remains
             key = next(iter(self.queries_by_key))
-            assert(isinstance(key, Key))
+            assert (isinstance(key, Key))
 
             result = caching.get_from_cache_by_key(key)
             if result is not None:
                 results = [result]
                 cache_results = False  # Don't update cache, we just got it from there
 
         client = transaction._rpc(self.connection)
```

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/db/backends/datastore/parsers/base.py` & `django-gcloud-connectors-0.4.0/gcloudc/db/backends/datastore/parsers/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -215,53 +215,56 @@
         # Leaf
         if hasattr(node.lhs, "target"):
             # from Django 1.9, some node.lhs might not have a target attribute
             # as they might be wrapping date fields
             field = node.lhs.target
             operator = convert_rhs_op(node)
         elif isinstance(node.lhs, Aggregate):
-            raise NotSupportedError("Aggregate filters are not supported on the Datastore")
+            raise NotSupportedError("Aggregate filters are not supported")
         else:
             field = node.lhs.lhs.target
             operator = convert_rhs_op(node)
 
             # This deals with things like datefield__month__gt=X which means from this point
             # on, operator will have two parts in that particular case and will probably need to
             # be dealt with by a special indexer
             if node.lookup_name != node.lhs.lookup_name:
                 operator = "{}__{}".format(node.lhs.lookup_name, node.lookup_name)
 
         if get_top_concrete_parent(field.model) != get_top_concrete_parent(model):
-            raise NotSupportedError("Cross-join where filters are not supported on the Datastore")
+            raise NotSupportedError("Cross-join where filters are not supported")
 
         # Make sure we don't let people try to filter on a text field, otherwise they just won't
         # get any results!
 
         lookup_supports_text = getattr(node, "lookup_supports_text", False)
 
         if field.db_type(connection) in ("bytes", "text") and not lookup_supports_text:
-            raise NotSupportedError("You can't filter on text or blob fields on the Datastore")
+            raise NotSupportedError("You can't filter on text or blob fields")
 
         if operator == "isnull" and field.model._meta.parents.values():
-            raise NotSupportedError("isnull lookups on inherited relations aren't supported on the Datastore")
+            raise NotSupportedError("isnull lookups on inherited relations aren't supported")
+
+        if negated and operator in ("=", ">", ">=", "<", "<=") and field.db_type(connection) in ("list", "set"):
+            raise NotSupportedError("inequality filters on list fields return unexpected results")
 
         lhs = field.column
 
         if hasattr(node.rhs, "get_compiler"):
             if len(node.rhs.select) == 1:
                 # In Django >= 1.11 this is a values list type query, which we explicitly handle
                 # because of the common case of pk__in=Something.objects.values_list("pk", flat=True)
                 qs = QuerySet(query=node.rhs, using=self.connection.alias)
 
                 # We make the query for the values, but wrap in a list to trick the
                 # was_iter code below. This whole set of if/elif statements needs rethinking!
                 rhs = [list(qs.values_list("pk", flat=True))]
             else:
                 # This is a subquery
-                raise NotSupportedError("Attempted to run a subquery on the Datastore")
+                raise NotSupportedError("Attempted to run a subquery on an non-relational database")
         elif isinstance(node.rhs, ValuesListQuerySet):
             # We explicitly handle ValuesListQuerySet because of the
             # common case of pk__in=Something.objects.values_list("pk", flat=True)
             # this WILL execute another query, but that is to be expected on a
             # non-relational database.
 
             rhs = [x for x in node.rhs]  # Evaluate the queryset
```

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/db/backends/datastore/parsers/version_18.py` & `django-gcloud-connectors-0.4.0/gcloudc/db/backends/datastore/parsers/version_18.py`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/db/backends/datastore/parsers/version_19.py` & `django-gcloud-connectors-0.4.0/gcloudc/db/backends/datastore/parsers/version_19.py`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/db/backends/datastore/query.py` & `django-gcloud-connectors-0.4.0/gcloudc/db/backends/datastore/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 
         self.column = None
         self.operator = None
         self.value = None
         self.output_field = None
         self.will_never_return_results = False
         self.lookup_name = None
+        self.is_iterable_field = False
 
         self.children = []
         self.connector = "AND"
         self.negated = False
 
     @property
     def is_leaf(self):
@@ -144,14 +145,15 @@
             column = special_indexer.indexed_column_name(column, value, index_type)
             operator = special_indexer.prep_query_operator(operator)
 
         self.column = column
         self.operator = convert_operator(operator)
         self.value = value
         self.lookup_name = lookup_name
+        self.is_iterable_field = target_field.db_type(wrapper) in ['list', 'set']
 
     def __iter__(self):
         for child in chain(*map(iter, self.children)):
             yield child
         yield self
 
     def __repr__(self):
@@ -171,15 +173,16 @@
         if self.is_leaf:
             return self.column == rhs.column and self.value == rhs.value and self.operator == rhs.operator
         else:
             return self.connector == rhs.connector and self.children == rhs.children
 
     def __hash__(self):
         if self.is_leaf:
-            return hash((self.column, self.value, self.operator))
+            value = frozenset(self.value) if isinstance(self.value, (set, list, tuple)) else self.value
+            return hash((self.column, value, self.operator))
         else:
             return hash((self.connector,) + tuple([hash(x) for x in self.children]))
 
 
 class Query(object):
     def __init__(self, model, kind):
         assert kind in VALID_QUERY_KINDS
```

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/db/backends/datastore/query_utils.py` & `django-gcloud-connectors-0.4.0/gcloudc/db/backends/datastore/query_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 """
     Utility functions for gathering data from Google Datastore Query
     objects.
 """
 
 
+# TODO: This function seems problematic, because what if the same col_and_operator
+# TODO: exists multiple times? It would always return the first item in the query filters.
+# TODO: Seems we should remove this function.
 def get_filter(query, col_and_operator):
     """
         query: A Cloud Datastore Query object
         col_and_operator: tuple of column name and operator
     """
     for col, operator, value in query.filters:
         if (col, operator) == tuple(col_and_operator):
```

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/db/backends/datastore/schema.py` & `django-gcloud-connectors-0.4.0/gcloudc/db/backends/datastore/schema.py`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/db/backends/datastore/transaction.py` & `django-gcloud-connectors-0.4.0/gcloudc/db/backends/datastore/transaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import copy
+import secrets
 import threading
-import uuid
 
+from django.db import (
+    DatabaseError,
+    connections,
+)
 from google.cloud import exceptions
 from google.cloud.datastore.transaction import \
     Transaction as DatastoreTransaction
 
-from django.db import connections, DatabaseError
 from gcloudc import context_decorator
 from gcloudc.db.backends.datastore import caching
 from gcloudc.db.backends.datastore.dbapi import CouldBeSupportedError
 
 TRANSACTION_ENTITY_LIMIT = 500
 
 
@@ -34,34 +37,30 @@
         self._seen_keys = set()
 
     def _generate_id(self):
         """
             The Datastore API won't generate keys automatically until a
             transaction commits, that's too late!
 
-            This is a hack, it might be the only hack we can do :(
-
-            Note. Even though the Datastore can handle negative IDs (it's a signed
-            64 bit integer) the default allocate never does, and also, this breaks
-            Django URL regexes etc. So like the allocator we just do 32 bit ones.
+            This returns a random 53 bit ID to remain inside the MAX_SAFE_INTEGER
+            range in Javascript (ideally this would be 63 bit)
         """
-        unsigned = uuid.uuid4().int & (1 << 32) - 1
-        return unsigned
+        return secrets.randbits(53)
 
     def key(self, *args, **kwargs):
         """
         Interface to the Datastore client Key factory.
         """
-        assert("namespace" not in kwargs)
+        assert ("namespace" not in kwargs)
         namespace = self._connection.namespace
         kwargs["namespace"] = namespace
 
         parent = kwargs.get("parent")
         if parent:
-            assert(parent.namespace == namespace)
+            assert (parent.namespace == namespace)
 
         return self._connection.gclient.key(*args, **kwargs)
 
     def get(self, key_or_keys, missing=None):
         # For some reason Datastore Transactions don't provide their
         # own get
         if hasattr(key_or_keys, "__iter__") and not isinstance(key_or_keys, str):
@@ -235,16 +234,16 @@
     """
         In the low-level connector code, we use this function
         to return a transaction to perform a Get/Put/Delete on
         this effectively returns the current_transaction or a new
         RootTransaction() which is basically no transaction at all.
     """
 
-    assert(isinstance(using, str))
-    assert(using)
+    assert (isinstance(using, str))
+    assert (using)
 
     class RootTransaction(Transaction):
         def _enter(self):
             pass
 
         def _exit(self):
             pass
@@ -336,15 +335,15 @@
         connection = connections[using]
 
         # Connect if necessary (mainly in tests)
         if not connection.connection:
             connection.connect()
 
         connection = connection.connection
-        assert(connection)
+        assert (connection)
 
         if independent:
             new_transaction = IndependentTransaction(connection)
         elif in_atomic_block():
             new_transaction = NestedTransaction(connection)
         elif mandatory:
             raise TransactionFailedError(
@@ -425,15 +424,15 @@
         connection = connections[using]
 
         # Connect if necessary (mainly in tests)
         if not connection.connection:
             connection.connect()
 
         connection = connection.connection
-        assert(connection)
+        assert (connection)
 
         # For non_atomic blocks we pass a Batch as the transaction
         new_transaction = NoTransaction(connection.gclient.batch())
 
         _STORAGE.transaction_stack.setdefault(using, []).append(new_transaction)
         _STORAGE.transaction_stack[using][-1].enter()
 
@@ -450,15 +449,15 @@
     def _do_exit(cls, state, decorator_args, exception):
         _init_storage()
 
         context = caching.get_context()
         transaction = _STORAGE.transaction_stack[state.using].pop()
 
         try:
-            assert(not transaction._datastore_transaction)
+            assert (not transaction._datastore_transaction)
         finally:
             # Restore the context stack as it was
             context.stack.stack = context.stack.stack + state.original_stack
             transaction.exit()
 
 
 non_atomic = NonAtomicDecorator
```

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/db/backends/datastore/unique_mixins.py` & `django-gcloud-connectors-0.4.0/gcloudc/db/backends/datastore/unique_mixins.py`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/db/backends/datastore/unique_utils.py` & `django-gcloud-connectors-0.4.0/gcloudc/db/backends/datastore/unique_utils.py`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/db/backends/datastore/utils.py` & `django-gcloud-connectors-0.4.0/gcloudc/db/backends/datastore/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 from django.db.backends.utils import format_number
 from django.utils import timezone
 from google.cloud.datastore.entity import Entity
 from google.cloud.datastore.key import Key
 
 from gcloudc.utils import memoized
 
-from .query_utils import get_filter
-
 try:
     from django.db.models.expressions import BaseExpression
 except ImportError:
     from django.db.models.expressions import ExpressionNode as BaseExpression
 
 
 def make_utc_compatible(value):
@@ -405,42 +403,45 @@
     queries = [query]
     if isinstance(query, meta_queries.AsyncMultiQuery):
         raise NotImplementedError(
             "We just need to separate the multiquery " "into 'queries' then everything should work"
         )
 
     for query in queries:
-        comparisons = chain([("__kind__", "=")], [(x[0], x[1]) for x in query.filters])
+        comparisons = chain([("__kind__", "=", None)], [(x[0], x[1], x[2]) for x in query.filters])
 
-        for ent_attr, op in comparisons:
+        for ent_attr, op, query_value in comparisons:
             if ent_attr == "__key__":
                 continue
 
             compare = OPERATORS[op]  # We want this to throw if there's some op we don't know about
 
             if ent_attr == "__kind__":
                 ent_value = entity.kind
                 query_value = query.kind
             else:
-                query_value = get_filter(query, (ent_attr, op))
                 ent_value = entity.get(ent_attr)
 
             if not isinstance(query_value, (list, tuple)):
                 query_values = [query_value]
             else:
                 # The query value can be a list of ANDed values
                 query_values = query_value
 
             if not isinstance(ent_value, (list, tuple)):
                 ent_value = [ent_value]
 
             matches = False
             for value in query_values:  # [22, 23]
                 # If any of the values don't match then this query doesn't match
-                if not any(compare(attr, value) for attr in ent_value):
+                if op == '=' and isinstance(value, (list, tuple)):
+                    if any(attr not in ent_attr for attr in value):
+                        matches = False
+                        break
+                elif not any(compare(attr, value) for attr in ent_value):
                     matches = False
                     break
             else:
                 # One of the ent_attrs matches the query_attrs
                 matches = True
 
             if not matches:
```

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/db/models/fields/allkeys-5.2.0.zip` & `django-gcloud-connectors-0.4.0/gcloudc/db/models/fields/allkeys-5.2.0.zip`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/db/models/fields/charfields.py` & `django-gcloud-connectors-0.4.0/gcloudc/db/models/fields/charfields.py`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/db/models/fields/computed.py` & `django-gcloud-connectors-0.4.0/gcloudc/db/models/fields/computed.py`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/db/models/fields/iterable.py` & `django-gcloud-connectors-0.4.0/gcloudc/db/models/fields/iterable.py`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/db/models/fields/json.py` & `django-gcloud-connectors-0.4.0/gcloudc/db/models/fields/json.py`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/db/models/fields/related.py` & `django-gcloud-connectors-0.4.0/gcloudc/db/models/fields/related.py`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/db/transaction.py` & `django-gcloud-connectors-0.4.0/gcloudc/db/transaction.py`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/forms/fields.py` & `django-gcloud-connectors-0.4.0/gcloudc/forms/fields.py`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/tests/__init__.py` & `django-gcloud-connectors-0.4.0/gcloudc/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/tests/models.py` & `django-gcloud-connectors-0.4.0/gcloudc/tests/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,24 @@
     def __str__(self):
         return self.username
 
     class Meta:
         unique_together = ("first_name", "second_name")
 
 
+class NullableUniqueTogether(models.Model):
+
+    field1 = models.PositiveIntegerField(blank=True, null=True)
+    field2 = models.PositiveIntegerField(blank=True, null=True)
+    field3 = models.PositiveIntegerField(blank=True, null=True)
+
+    class Meta:
+        unique_together = [("field1", "field2", "field3")]
+
+
 class TestUserTwo(models.Model):
     username = models.CharField(max_length=32, unique=True)
 
 
 class BasicTestModel(models.Model):
     field1 = models.CharField(max_length=100)
     field2 = models.IntegerField(unique=True)
```

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/tests/test_async_multi_query.py` & `django-gcloud-connectors-0.4.0/gcloudc/tests/test_async_multi_query.py`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/tests/test_atomic.py` & `django-gcloud-connectors-0.4.0/gcloudc/tests/test_atomic.py`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/tests/test_cloud_datastore_runner.py` & `django-gcloud-connectors-0.4.0/gcloudc/tests/test_cloud_datastore_runner.py`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/tests/test_computed_field.py` & `django-gcloud-connectors-0.4.0/gcloudc/tests/test_computed_field.py`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/tests/test_connector.py` & `django-gcloud-connectors-0.4.0/gcloudc/tests/test_connector.py`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/tests/test_db_fields.py` & `django-gcloud-connectors-0.4.0/gcloudc/tests/test_db_fields.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pickle
 from datetime import timedelta
 
+import django
 from django import forms
 from django.core.exceptions import ValidationError
 from django.db import (
     connection,
     models,
 )
 from django.test import override_settings
@@ -26,14 +27,15 @@
 
 from . import TestCase
 from .models import (
     BasicTestModel,
     BinaryFieldModel,
     ModelWithCharField,
     NonIndexedModel,
+    NullableFieldModel,
     PFAwards,
     PFAuthor,
     PFPost,
     ISOther,
     ISStringReferenceModel,
 )
 
@@ -349,7 +351,40 @@
 
         instance = self._create_instance_with_null_field_value()
 
         instance.save()
         instance.refresh_from_db()
 
         self.assertEqual(instance.some_field, 1086)
+
+
+class NullableFieldModelTests(TestCase):
+
+    def test_query_in_list_of_null_not_supported_in_django_32(self):
+        """Before Django 3.2, this unit test's query used to return [1],
+        but since the following change is no longer supported:
+        https://code.djangoproject.com/ticket/31667"""
+
+        NullableFieldModel.objects.create(pk=1)
+        NullableFieldModel.objects.create(pk=5, nullable=2)
+
+        results = NullableFieldModel.objects.filter(nullable__in=[None])
+
+        self.assertEqual(
+            [r.pk for r in results],
+            [] if django.VERSION >= (3, 2) else [1]
+        )
+
+    def test_query_isnull(self):
+        NullableFieldModel.objects.create(pk=1)
+        NullableFieldModel.objects.create(pk=5, nullable=2)
+
+        results = NullableFieldModel.objects.filter(nullable__isnull=True)
+        self.assertEqual([r.pk for r in results], [1])
+
+    def test_query_in_list_of_null_and_non_null(self):
+        NullableFieldModel.objects.create(pk=1)
+        NullableFieldModel.objects.create(pk=5, nullable=2)
+        NullableFieldModel.objects.create(pk=6, nullable=3)
+
+        results = NullableFieldModel.objects.filter(nullable__in=[None, 3])
+        self.assertEqual({r.pk for r in results}, {1, 6})
```

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/tests/test_delete.py` & `django-gcloud-connectors-0.4.0/gcloudc/tests/test_delete.py`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/tests/test_django_interactions.py` & `django-gcloud-connectors-0.4.0/gcloudc/tests/test_django_interactions.py`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/tests/test_excluding_pks.py` & `django-gcloud-connectors-0.4.0/gcloudc/tests/test_excluding_pks.py`

 * *Files 26% similar despite different names*

```diff
@@ -25,7 +25,37 @@
     def test_count_on_excluded_pks(self):
         ExcludedPKModel.objects.create(name="Apple", color="Red")
         ExcludedPKModel.objects.create(name="Orange", color="Orange")
 
         self.assertEqual(
             1, ExcludedPKModel.objects.filter(pk__in=["Apple", "Orange"]).exclude(pk__in=["Apple"]).count()
         )
+
+    def test_count_using_in_filter_with_excluded_pks(self):
+        ExcludedPKModel.objects.create(name="Apple", color="Red")
+        ExcludedPKModel.objects.create(name="Orange", color="Orange")
+
+        self.assertEqual(
+            1, ExcludedPKModel.objects.filter(color__in=["Red", "Orange"]).exclude(pk__in=["Apple"]).count()
+        )
+
+    def test_count_using_eq_filter_with_excluded_pk(self):
+        ExcludedPKModel.objects.create(name="Apple", color="Red")
+        ExcludedPKModel.objects.create(name="Orange", color="Orange")
+
+        self.assertEqual(
+            0, ExcludedPKModel.objects.filter(color="Red").exclude(pk="Apple").count()
+        )
+        self.assertEqual(
+            1, ExcludedPKModel.objects.filter(color="Red").exclude(pk="Orange").count()
+        )
+
+    def test_exclude_pks_with_filter(self):
+        ExcludedPKModel.objects.create(name="Apple", color="Red")
+        ExcludedPKModel.objects.create(name="Orange", color="Orange")
+
+        self.assertEqual(
+            ['Orange'],
+            [e.pk for e in ExcludedPKModel.objects.filter(
+                color__in=["Red", "Orange"]
+            ).exclude(pk__in=["Apple"])]
+        )
```

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/tests/test_iterable_fields.py` & `django-gcloud-connectors-0.4.0/gcloudc/tests/test_iterable_fields.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,31 @@
 import datetime
 
-from . import TestCase
 from django import forms
 from django.core import serializers
-from django.core.exceptions import ValidationError, ImproperlyConfigured
-from django.db import models
-from gcloudc.db.models.fields.iterable import ListField, SetField
-from gcloudc.db.models.fields.related import RelatedListField, RelatedSetField
+from django.core.exceptions import (
+    ImproperlyConfigured,
+    ValidationError,
+)
+from django.db import (
+    NotSupportedError,
+    models,
+)
+
 from gcloudc.db.models.fields.charfields import CharField
+from gcloudc.db.models.fields.iterable import (
+    ListField,
+    SetField,
+)
+from gcloudc.db.models.fields.related import (
+    RelatedListField,
+    RelatedSetField,
+)
+
+from . import TestCase
 
 
 class IterableIterableRelatedModel(models.Model):
     name = models.CharField(max_length=500)
 
     def __str__(self):
         return "%s:%s" % (self.pk, self.name)
@@ -60,16 +74,16 @@
             self.assertEqual(sorted(x.pk for x in qry), sorted([list1.pk, list2.pk]))
             # filtering using __contains lookup
             qry = IterableFieldModel.objects.filter(**{f"{field}__contains": ["A"]})
             self.assertEqual(sorted(x.pk for x in qry), sorted([list1.pk, list2.pk]))
             qry = IterableFieldModel.objects.filter(**{f"{field}__contains": ["H"]})
             self.assertEqual(sorted(x.pk for x in qry), [list2.pk])
             # Filtering using two __contains filters, applied together
-            qry = IterableFieldModel.objects.filter(**{f"{field}__contains": ["A", "B"]})
-            self.assertEqual(sorted(x.pk for x in qry), sorted([list1.pk, list2.pk]))
+            qry = IterableFieldModel.objects.filter(**{f"{field}__contains": ["A", "D"]})
+            self.assertEqual(sorted(x.pk for x in qry), sorted([list1.pk]))
             # Filtering using two __contains filters, applied one after the other
             qry = IterableFieldModel.objects.filter(
                 **{f"{field}__contains": ["A"]}
             ).filter(
                 **{f"{field}__contains": ["B"]}
             )
             self.assertEqual(sorted(x.pk for x in qry), sorted([list1.pk, list2.pk]))
@@ -123,27 +137,81 @@
 
         # filtering using __overlap lookup with SetField:
         qry = IterableFieldModel.objects.filter(set_field__overlap=set(["A", "B"]))
         self.assertEqual(sorted(x.pk for x in qry), sorted([list1.pk, list2.pk]))
         qry = IterableFieldModel.objects.filter(set_field__overlap=["H"])
         self.assertEqual(sorted(x.pk for x in qry), [list2.pk])
 
+        # Filtering using two __overlap filters, applied one after the other
+        qry = IterableFieldModel.objects.filter(
+                **{"list_field__overlap": ["A"]}
+            ).filter(
+                **{"list_field__overlap": ["J"]}
+            )
+        self.assertEqual(list(qry), [list2])
+
+        # Filtering with combination of __contains and __overlap filters, in either order.
+        qry = IterableFieldModel.objects.filter(
+                **{"list_field__contains": ["A", "D"]}
+            ).filter(
+                **{"list_field__overlap": ["B", "J"]}
+            )
+        self.assertEqual(list(qry), [list1])
+        qry = IterableFieldModel.objects.filter(
+                **{"list_field__overlap": ["B", "J"]}
+            ).filter(
+                **{"list_field__contains": ["A", "D"]}
+            )
+        self.assertEqual(list(qry), [list1])
+
+        # Combine multiple __contains with pk__in
+        qry = IterableFieldModel.objects.filter(
+                **{"list_field__contains": ["A"]}
+            ).filter(
+                **{"list_field__contains": ["G"]}
+            ).filter(
+                **{"pk__in": [list1.pk, list2.pk]}
+            )
+        self.assertEqual(list(qry), [list1])
+        qry = IterableFieldModel.objects.filter(
+                **{"list_field__contains": ["A"]}
+            ).filter(
+                **{"list_field__contains": ["B"]}
+            ).filter(
+                **{"pk__in": [list1.pk]}
+            )
+        self.assertEqual(list(qry), [list1])
+
     def test_empty_iterable_fields(self):
         """ Test that an empty set field always returns set(), not None """
         instance = IterableFieldModel()
         # When assigning
         self.assertEqual(instance.set_field, set())
         self.assertEqual(instance.list_field, [])
         instance.save()
 
         instance = IterableFieldModel.objects.get()
         # When getting it from the db
         self.assertEqual(instance.set_field, set())
         self.assertEqual(instance.list_field, [])
 
+    def test_filtering_multiple_contains_and_pk_in(self):
+        A = IterableFieldModel.objects.create(list_field=["A"])
+        IterableFieldModel.objects.create(list_field=["B"])
+        AB = IterableFieldModel.objects.create(list_field=["A", "B"])
+        IterableFieldModel.objects.create(list_field=["A", "B", "C"])
+
+        qry = (
+            IterableFieldModel.objects
+            .filter(list_field__contains='A')
+            .filter(list_field__contains='B')
+            .filter(pk__in=[A.pk, AB.pk])
+        )
+        self.assertEqual(set(qry), {AB})
+
     def test_list_field(self):
         instance = IterableFieldModel.objects.create()
         self.assertEqual([], instance.list_field)
         instance.list_field.append("One")
         self.assertEqual(["One"], instance.list_field)
         instance.save()
 
@@ -181,14 +249,32 @@
 
         self.assertFalse(IterableFieldModel.objects.filter(set_field__isempty=True).exists())
         self.assertTrue(IterableFieldModel.objects.filter(set_field__isempty=False).exists())
 
         self.assertFalse(IterableFieldModel.objects.exclude(set_field__isempty=False).exists())
         self.assertTrue(IterableFieldModel.objects.exclude(set_field__isempty=True).exists())
 
+    def test_exclude_contains(self):
+        IterableFieldModel.objects.create(list_field=["apples", "bananas"])
+        IterableFieldModel.objects.create(list_field=["apples", "pears"])
+
+        self.assertRaises(
+            NotSupportedError, list,
+            IterableFieldModel.objects.exclude(
+                list_field__contains="bananas"
+            ).order_by("list_field")
+        )
+
+        self.assertRaises(
+            NotSupportedError, list,
+            IterableFieldModel.objects.exclude(
+                list_field__contains="pears"
+            ).order_by("list_field"),
+        )
+
     def test_serialization(self):
         dt = datetime.datetime(2017, 1, 1, 12)
         instance = IterableFieldModel.objects.create(
             set_field={u"foo"},
             list_field=[u"bar"],
             set_field_int={123},
             list_field_int=[456],
```

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/tests/test_json_field.py` & `django-gcloud-connectors-0.4.0/gcloudc/tests/test_json_field.py`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/tests/test_operations.py` & `django-gcloud-connectors-0.4.0/gcloudc/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/tests/test_query_by_keys.py` & `django-gcloud-connectors-0.4.0/gcloudc/tests/test_query_by_keys.py`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/tests/test_query_transform.py` & `django-gcloud-connectors-0.4.0/gcloudc/tests/test_query_transform.py`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/tests/test_related_fields.py` & `django-gcloud-connectors-0.4.0/gcloudc/tests/test_related_fields.py`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/tests/test_transaction_hooks.py` & `django-gcloud-connectors-0.4.0/gcloudc/tests/test_transaction_hooks.py`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/tests/test_unique_constraints.py` & `django-gcloud-connectors-0.4.0/gcloudc/tests/test_unique_constraints.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from django.db import connection
 from django.db.utils import IntegrityError
 
 from gcloudc.db.backends.datastore.transaction import TransactionFailedError
 
 from . import TestCase
 from .models import (
+    NullableUniqueTogether,
     TestUser,
     TestUserTwo,
 )
 
 
 def _get_client():
     return connection.connection.gclient
@@ -25,15 +26,17 @@
     if keys_only:
         query.keys_only()
     return list(query.fetch())
 
 
 class TestUniqueConstraints(TestCase):
 
-    KINDS_TO_DELETE = ["uniquemarker", "test_testuser", "test_testusertwo"]
+    KINDS_TO_DELETE = [
+        "uniquemarker", "test_testuser", "test_testusertwo", "test_nullableuniquetogether"
+    ]
 
     def test_insert(self):
         """
         Assert that when creating a new instance, unique markers are also
         created to reflect the constraints defined on the model.
 
         If a subsequent insert is attempted, these should be compared to
@@ -372,7 +375,16 @@
 
         child = Child.objects.create(unique_field="unique_value")
         self.assertIsNotNone(child)
 
         # Check that actual integrity issues are reported
         with self.assertRaises(IntegrityError):
             Child.objects.create(unique_field="unique_value")
+
+    def test_unique_together_with_null(self):
+        """ If one of the field values in a unique_together constraint is null then the whole
+            combination should be ignored for that object.
+        """
+        # This is the expected behaviour based on Postgres:
+        # https://www.postgresql.org/docs/13/ddl-constraints.html#DDL-CONSTRAINTS-UNIQUE-CONSTRAINTS
+        NullableUniqueTogether.objects.create(field1=1, field2=2, field3=None)
+        NullableUniqueTogether.objects.create(field1=1, field2=2, field3=None)
```

### Comparing `django-gcloud-connectors-0.3.7/gcloudc/utils.py` & `django-gcloud-connectors-0.4.0/gcloudc/utils.py`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-0.3.7/setup.py` & `django-gcloud-connectors-0.4.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,36 +11,36 @@
 
 AUTHOR = "Potato London Ltd."
 AUTHOR_EMAIL = "mail@p.ota.to"
 
 if os.environ.get('CI_COMMIT_TAG'):
     VERSION = os.environ['CI_COMMIT_TAG']
 else:
-    VERSION = '0.3.6'
+    VERSION = '0.4.0'
 
 setup(
     name=NAME,
     version=VERSION,
     packages=find_packages(),
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     author=AUTHOR,
     author_email=AUTHOR_EMAIL,
     url=URL,
     keywords=["Google Cloud Datastore", "Google App Engine", "Django"],
     classifiers=[
-        'Development Status :: 3 - Alpha',
+        'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
     ],
     install_requires=[
-        'django>=2.0,<=3.3.*',
+        'django>=2.0,<=3.3',
         'pyyaml>=5.3.1,<6.0',
         'google-cloud-datastore>=1.15.3',
         'sleuth-mock==0.1',
         'pyuca==1.2',
     ],
     include_package_data=True,
 )
```

### Comparing `django-gcloud-connectors-0.3.7/test/404.html` & `django-gcloud-connectors-0.4.0/test/404.html`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
   <div class="wy-grid-for-nav">
     <nav data-toggle="wy-nav-shift" class="wy-nav-side stickynav">
     <div class="wy-side-scroll">
       <div class="wy-side-nav-search">
           <a href="/google-cloud/django-gcloud-connectors/." class="icon icon-home"> Django Gcloud Connectors Documentation
         </a><div role="search">
   <form id ="rtd-search-form" class="wy-form" action="/google-cloud/django-gcloud-connectors//search.html" method="get">
-      <input type="text" name="q" placeholder="Search docs" title="Type search term here" />
+      <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" title="Type search term here" />
   </form>
 </div>
       </div>
 
       <div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
               <ul>
                 <li class="toctree-l1"><a class="reference internal" href="/google-cloud/django-gcloud-connectors/.">Home</a>
@@ -74,15 +74,15 @@
           <i data-toggle="wy-nav-top" class="fa fa-bars"></i>
           <a href="/google-cloud/django-gcloud-connectors/.">Django Gcloud Connectors Documentation</a>
         
       </nav>
       <div class="wy-nav-content">
         <div class="rst-content"><div role="navigation" aria-label="breadcrumbs navigation">
   <ul class="wy-breadcrumbs">
-    <li><a href="/google-cloud/django-gcloud-connectors/." class="icon icon-home" alt="Docs"></a> &raquo;</li>
+    <li><a href="/google-cloud/django-gcloud-connectors/." class="icon icon-home" aria-label="Docs"></a> &raquo;</li>
     <li class="wy-breadcrumbs-aside">
     </li>
   </ul>
   <hr/>
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
             <div class="section" itemprop="articleBody">
```

### Comparing `django-gcloud-connectors-0.3.7/test/commercial_support/index.html` & `django-gcloud-connectors-0.4.0/test/commercial_support/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
   <div class="wy-grid-for-nav">
     <nav data-toggle="wy-nav-shift" class="wy-nav-side stickynav">
     <div class="wy-side-scroll">
       <div class="wy-side-nav-search">
           <a href=".." class="icon icon-home"> Django Gcloud Connectors Documentation
         </a><div role="search">
   <form id ="rtd-search-form" class="wy-form" action="../search.html" method="get">
-      <input type="text" name="q" placeholder="Search docs" title="Type search term here" />
+      <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" title="Type search term here" />
   </form>
 </div>
       </div>
 
       <div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
               <ul>
                 <li class="toctree-l1"><a class="reference internal" href="..">Home</a>
@@ -83,19 +83,18 @@
           <i data-toggle="wy-nav-top" class="fa fa-bars"></i>
           <a href="..">Django Gcloud Connectors Documentation</a>
         
       </nav>
       <div class="wy-nav-content">
         <div class="rst-content"><div role="navigation" aria-label="breadcrumbs navigation">
   <ul class="wy-breadcrumbs">
-    <li><a href=".." class="icon icon-home" alt="Docs"></a> &raquo;</li>
+    <li><a href=".." class="icon icon-home" aria-label="Docs"></a> &raquo;</li>
       <li>Commercial Support</li>
     <li class="wy-breadcrumbs-aside">
-        <a href="https://gitlab.com/potato-oss/google-cloud/django-gcloud-connectors/edit/master/docs/commercial_support.md"
-          class="icon icon-gitlab"> Edit on GitLab</a>
+          <a href="https://gitlab.com/potato-oss/google-cloud/django-gcloud-connectors/edit/master/docs/commercial_support.md" class="icon icon-gitlab"> Edit on GitLab</a>
     </li>
   </ul>
   <hr/>
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
             <div class="section" itemprop="articleBody">
```

### Comparing `django-gcloud-connectors-0.3.7/test/concepts_limitations/index.html` & `django-gcloud-connectors-0.4.0/test/concepts_limitations/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
   <div class="wy-grid-for-nav">
     <nav data-toggle="wy-nav-shift" class="wy-nav-side stickynav">
     <div class="wy-side-scroll">
       <div class="wy-side-nav-search">
           <a href=".." class="icon icon-home"> Django Gcloud Connectors Documentation
         </a><div role="search">
   <form id ="rtd-search-form" class="wy-form" action="../search.html" method="get">
-      <input type="text" name="q" placeholder="Search docs" title="Type search term here" />
+      <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" title="Type search term here" />
   </form>
 </div>
       </div>
 
       <div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
               <ul>
                 <li class="toctree-l1"><a class="reference internal" href="..">Home</a>
@@ -103,19 +103,18 @@
           <i data-toggle="wy-nav-top" class="fa fa-bars"></i>
           <a href="..">Django Gcloud Connectors Documentation</a>
         
       </nav>
       <div class="wy-nav-content">
         <div class="rst-content"><div role="navigation" aria-label="breadcrumbs navigation">
   <ul class="wy-breadcrumbs">
-    <li><a href=".." class="icon icon-home" alt="Docs"></a> &raquo;</li>
+    <li><a href=".." class="icon icon-home" aria-label="Docs"></a> &raquo;</li>
       <li>Concepts & limitations</li>
     <li class="wy-breadcrumbs-aside">
-        <a href="https://gitlab.com/potato-oss/google-cloud/django-gcloud-connectors/edit/master/docs/concepts_limitations.md"
-          class="icon icon-gitlab"> Edit on GitLab</a>
+          <a href="https://gitlab.com/potato-oss/google-cloud/django-gcloud-connectors/edit/master/docs/concepts_limitations.md" class="icon icon-gitlab"> Edit on GitLab</a>
     </li>
   </ul>
   <hr/>
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
             <div class="section" itemprop="articleBody">
```

### Comparing `django-gcloud-connectors-0.3.7/test/contributing/index.html` & `django-gcloud-connectors-0.4.0/test/contributing/index.html`

 * *Files 17% similar despite different names*

```diff
@@ -30,15 +30,15 @@
   <div class="wy-grid-for-nav">
     <nav data-toggle="wy-nav-shift" class="wy-nav-side stickynav">
     <div class="wy-side-scroll">
       <div class="wy-side-nav-search">
           <a href=".." class="icon icon-home"> Django Gcloud Connectors Documentation
         </a><div role="search">
   <form id ="rtd-search-form" class="wy-form" action="../search.html" method="get">
-      <input type="text" name="q" placeholder="Search docs" title="Type search term here" />
+      <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" title="Type search term here" />
   </form>
 </div>
       </div>
 
       <div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
               <ul>
                 <li class="toctree-l1"><a class="reference internal" href="..">Home</a>
@@ -70,14 +70,26 @@
     <li class="toctree-l2"><a class="reference internal" href="#code-style">Code style</a>
     </li>
     <li class="toctree-l2"><a class="reference internal" href="#need-help">Need help?</a>
     </li>
     <li class="toctree-l2"><a class="reference internal" href="#merge-request-requirements">Merge request requirements</a>
     </li>
     <li class="toctree-l2"><a class="reference internal" href="#running-tests">Running tests</a>
+        <ul>
+    <li class="toctree-l3"><a class="reference internal" href="#running-tests-with-real-datastore">Running tests with real Datastore</a>
+    </li>
+        </ul>
+    </li>
+    <li class="toctree-l2"><a class="reference internal" href="#indexes-management">Indexes management</a>
+        <ul>
+    <li class="toctree-l3"><a class="reference internal" href="#updating-during-development">Updating during development</a>
+    </li>
+    <li class="toctree-l3"><a class="reference internal" href="#deploying-indexes">Deploying indexes</a>
+    </li>
+        </ul>
     </li>
     <li class="toctree-l2"><a class="reference internal" href="#release-process">Release process</a>
     </li>
     </ul>
                 </li>
               </ul>
               <ul>
@@ -97,19 +109,18 @@
           <i data-toggle="wy-nav-top" class="fa fa-bars"></i>
           <a href="..">Django Gcloud Connectors Documentation</a>
         
       </nav>
       <div class="wy-nav-content">
         <div class="rst-content"><div role="navigation" aria-label="breadcrumbs navigation">
   <ul class="wy-breadcrumbs">
-    <li><a href=".." class="icon icon-home" alt="Docs"></a> &raquo;</li>
+    <li><a href=".." class="icon icon-home" aria-label="Docs"></a> &raquo;</li>
       <li>Contributing & Testing</li>
     <li class="wy-breadcrumbs-aside">
-        <a href="https://gitlab.com/potato-oss/google-cloud/django-gcloud-connectors/edit/master/docs/contributing.md"
-          class="icon icon-gitlab"> Edit on GitLab</a>
+          <a href="https://gitlab.com/potato-oss/google-cloud/django-gcloud-connectors/edit/master/docs/contributing.md" class="icon icon-gitlab"> Edit on GitLab</a>
     </li>
   </ul>
   <hr/>
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
             <div class="section" itemprop="articleBody">
               
@@ -144,21 +155,43 @@
 <li>Install the gcloud datastore emulator: <code>gcloud components install cloud-datastore-emulator</code><ul>
 <li>If you don't have <code>gcloud</code> (the Google Cloud SDK) installed, installation instructions can be found <a href="https://cloud.google.com/sdk/install">here</a></li>
 <li>Note that the Datastore emulator <a href="https://cloud.google.com/datastore/docs/tools/datastore-emulator">requires the Java JRE</a>.</li>
 </ul>
 </li>
 <li>Create a Python 3 virtualenv: <code>python3 -m venv .venv &amp;&amp; source ./.venv/bin/activate</code></li>
 <li>Install the prerequisites: <code>pip3 install tox</code></li>
+<li>Create test output directory: <code>mkdir .reports</code></li>
 </ul>
 <p>Then you can run:</p>
 <pre><code>$ tox
 </code></pre>
 <p>Under the hood tox runs <code>./manage.py test</code>. To pass down arguments to this command simply separate them with a double hyphen. e.g.</p>
 <pre><code>tox -e py37 -- --failfast
 </code></pre>
+<h3 id="running-tests-with-real-datastore">Running tests with real Datastore</h3>
+<p>It is sometime useful to be able to run tests against a real version of the Datastore instead of the emulator.</p>
+<p>You need to create your own GCP project and then set the <code>GCLOUDC_PROJECT_ID</code> environment variable.
+Two GCP Projects have been set for Pototo employees:
+- <code>gclouc-test-optimistic</code> for datastore running in OPTIMISTIC concurrency mode.
+- <code>gclouc-test-pessimistic</code> for datastore running in PESSIMISTIC concurrency mode.</p>
+<p>Make sure you have the have configured the application default credentials by running:</p>
+<pre><code>gcloud auth application-default login
+</code></pre>
+<p>You can then run tox passing the <code>--use-remote-datastore</code> option like this:</p>
+<pre><code>$ tox -e py39-22 -- --use-remote-datastore
+</code></pre>
+<h2 id="indexes-management">Indexes management</h2>
+<h3 id="updating-during-development">Updating during development</h3>
+<p>When running the test locally, we use the Google Cloud datastore emulator as database.
+When a query that requires a composite index is run, the emulator detects it and if not present already, it adds it to the <code>.index.yaml</code> file, below the <code># AUTOGENERATED</code> row.</p>
+<p>You'll notice this, because the file will appear to have changes in git.
+Unfortunately, all the automatically-added lines are discarded every time the emulator starts. If you notice new indexes have been added, move them above the <code># AUTOGENERATED</code> line and save the file. This will ensure they won't be deleted automatically.</p>
+<h3 id="deploying-indexes">Deploying indexes</h3>
+<p>If new indexes have been added since the last deployment, and you want to run test against a real instance of Datastore they need to be deployed to.
+<code>gcloud app deploy --project=&lt;your-project&gt; .index.yaml</code></p>
 <h2 id="release-process">Release process</h2>
 <p>Release to pypi is managed by GitLab CI. To create a new release create the relevant tag
 and push it to the gitlab remote. But first you should do some version fiddling...</p>
 <pre><code>1. Update the version in setup.py to the new version by removing the 'a' suffix (most likely)
 2. Commit this change
 3. Run `git tag -a X.Y.Z -m &quot;Some description&quot;
 4. Run `git push origin master &amp;&amp; git push --tags`
```

#### html2text {}

```diff
@@ -14,14 +14,18 @@
     * Contributing_&_Testing
           o Get_started_with_development
           o Pick_an_issue_&_send_a_merge_request
           o Code_style
           o Need_help?
           o Merge_request_requirements
           o Running_tests
+                # Running_tests_with_real_Datastore
+          o Indexes_management
+                # Updating_during_development
+                # Deploying_indexes
           o Release_process
     * Commercial_Support
     * Work_with_us!
     Django_Gcloud_Connectors_Documentation
     *  »
     * Contributing & Testing
     * Edit_on_GitLab
@@ -56,19 +60,47 @@
       datastore-emulator
           o If you don't have gcloud (the Google Cloud SDK) installed,
             installation instructions can be found here
           o Note that the Datastore emulator requires_the_Java_JRE.
     * Create a Python 3 virtualenv: python3 -m venv .venv && source ./.venv/
       bin/activate
     * Install the prerequisites: pip3 install tox
+    * Create test output directory: mkdir .reports
 Then you can run:
 $ tox
 Under the hood tox runs ./manage.py test. To pass down arguments to this
 command simply separate them with a double hyphen. e.g.
 tox -e py37 -- --failfast
+**** Running tests with real Datastore ****
+It is sometime useful to be able to run tests against a real version of the
+Datastore instead of the emulator.
+You need to create your own GCP project and then set the GCLOUDC_PROJECT_ID
+environment variable. Two GCP Projects have been set for Pototo employees: -
+gclouc-test-optimistic for datastore running in OPTIMISTIC concurrency mode. -
+gclouc-test-pessimistic for datastore running in PESSIMISTIC concurrency mode.
+Make sure you have the have configured the application default credentials by
+running:
+gcloud auth application-default login
+You can then run tox passing the --use-remote-datastore option like this:
+$ tox -e py39-22 -- --use-remote-datastore
+***** Indexes management *****
+**** Updating during development ****
+When running the test locally, we use the Google Cloud datastore emulator as
+database. When a query that requires a composite index is run, the emulator
+detects it and if not present already, it adds it to the .index.yaml file,
+below the # AUTOGENERATED row.
+You'll notice this, because the file will appear to have changes in git.
+Unfortunately, all the automatically-added lines are discarded every time the
+emulator starts. If you notice new indexes have been added, move them above the
+# AUTOGENERATED line and save the file. This will ensure they won't be deleted
+automatically.
+**** Deploying indexes ****
+If new indexes have been added since the last deployment, and you want to run
+test against a real instance of Datastore they need to be deployed to. gcloud
+app deploy --project=<your-project> .index.yaml
 ***** Release process *****
 Release to pypi is managed by GitLab CI. To create a new release create the
 relevant tag and push it to the gitlab remote. But first you should do some
 version fiddling...
 1. Update the version in setup.py to the new version by removing the 'a' suffix
 (most likely)
 2. Commit this change
```

### Comparing `django-gcloud-connectors-0.3.7/test/fields/index.html` & `django-gcloud-connectors-0.4.0/test/fields/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
   <div class="wy-grid-for-nav">
     <nav data-toggle="wy-nav-shift" class="wy-nav-side stickynav">
     <div class="wy-side-scroll">
       <div class="wy-side-nav-search">
           <a href=".." class="icon icon-home"> Django Gcloud Connectors Documentation
         </a><div role="search">
   <form id ="rtd-search-form" class="wy-form" action="../search.html" method="get">
-      <input type="text" name="q" placeholder="Search docs" title="Type search term here" />
+      <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" title="Type search term here" />
   </form>
 </div>
       </div>
 
       <div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
               <ul>
                 <li class="toctree-l1"><a class="reference internal" href="..">Home</a>
@@ -99,19 +99,18 @@
           <i data-toggle="wy-nav-top" class="fa fa-bars"></i>
           <a href="..">Django Gcloud Connectors Documentation</a>
         
       </nav>
       <div class="wy-nav-content">
         <div class="rst-content"><div role="navigation" aria-label="breadcrumbs navigation">
   <ul class="wy-breadcrumbs">
-    <li><a href=".." class="icon icon-home" alt="Docs"></a> &raquo;</li>
+    <li><a href=".." class="icon icon-home" aria-label="Docs"></a> &raquo;</li>
       <li>Fields</li>
     <li class="wy-breadcrumbs-aside">
-        <a href="https://gitlab.com/potato-oss/google-cloud/django-gcloud-connectors/edit/master/docs/fields.md"
-          class="icon icon-gitlab"> Edit on GitLab</a>
+          <a href="https://gitlab.com/potato-oss/google-cloud/django-gcloud-connectors/edit/master/docs/fields.md" class="icon icon-gitlab"> Edit on GitLab</a>
     </li>
   </ul>
   <hr/>
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
             <div class="section" itemprop="articleBody">
```

### Comparing `django-gcloud-connectors-0.3.7/test/index.html` & `django-gcloud-connectors-0.4.0/test/index.html`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,15 @@
   <div class="wy-grid-for-nav">
     <nav data-toggle="wy-nav-shift" class="wy-nav-side stickynav">
     <div class="wy-side-scroll">
       <div class="wy-side-nav-search">
           <a href="." class="icon icon-home"> Django Gcloud Connectors Documentation
         </a><div role="search">
   <form id ="rtd-search-form" class="wy-form" action="./search.html" method="get">
-      <input type="text" name="q" placeholder="Search docs" title="Type search term here" />
+      <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" title="Type search term here" />
   </form>
 </div>
       </div>
 
       <div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
               <ul class="current">
                 <li class="toctree-l1 current"><a class="reference internal current" href=".">Home</a>
@@ -83,19 +83,18 @@
           <i data-toggle="wy-nav-top" class="fa fa-bars"></i>
           <a href=".">Django Gcloud Connectors Documentation</a>
         
       </nav>
       <div class="wy-nav-content">
         <div class="rst-content"><div role="navigation" aria-label="breadcrumbs navigation">
   <ul class="wy-breadcrumbs">
-    <li><a href="." class="icon icon-home" alt="Docs"></a> &raquo;</li>
+    <li><a href="." class="icon icon-home" aria-label="Docs"></a> &raquo;</li>
       <li>Home</li>
     <li class="wy-breadcrumbs-aside">
-        <a href="https://gitlab.com/potato-oss/google-cloud/django-gcloud-connectors/edit/master/docs/index.md"
-          class="icon icon-gitlab"> Edit on GitLab</a>
+          <a href="https://gitlab.com/potato-oss/google-cloud/django-gcloud-connectors/edit/master/docs/index.md" class="icon icon-gitlab"> Edit on GitLab</a>
     </li>
   </ul>
   <hr/>
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
             <div class="section" itemprop="articleBody">
               
@@ -153,10 +152,10 @@
         };
     </script>
 
 </body>
 </html>
 
 <!--
-MkDocs version : 1.3.1
-Build Date UTC : 2022-07-20 11:06:53.129438+00:00
+MkDocs version : 1.4.3
+Build Date UTC : 2023-06-21 10:01:47.452151+00:00
 -->
```

### Comparing `django-gcloud-connectors-0.3.7/test/installation/index.html` & `django-gcloud-connectors-0.4.0/test/installation/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
   <div class="wy-grid-for-nav">
     <nav data-toggle="wy-nav-shift" class="wy-nav-side stickynav">
     <div class="wy-side-scroll">
       <div class="wy-side-nav-search">
           <a href=".." class="icon icon-home"> Django Gcloud Connectors Documentation
         </a><div role="search">
   <form id ="rtd-search-form" class="wy-form" action="../search.html" method="get">
-      <input type="text" name="q" placeholder="Search docs" title="Type search term here" />
+      <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" title="Type search term here" />
   </form>
 </div>
       </div>
 
       <div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
               <ul>
                 <li class="toctree-l1"><a class="reference internal" href="..">Home</a>
@@ -85,29 +85,28 @@
           <i data-toggle="wy-nav-top" class="fa fa-bars"></i>
           <a href="..">Django Gcloud Connectors Documentation</a>
         
       </nav>
       <div class="wy-nav-content">
         <div class="rst-content"><div role="navigation" aria-label="breadcrumbs navigation">
   <ul class="wy-breadcrumbs">
-    <li><a href=".." class="icon icon-home" alt="Docs"></a> &raquo;</li>
+    <li><a href=".." class="icon icon-home" aria-label="Docs"></a> &raquo;</li>
       <li>Installation</li>
     <li class="wy-breadcrumbs-aside">
-        <a href="https://gitlab.com/potato-oss/google-cloud/django-gcloud-connectors/edit/master/docs/installation.md"
-          class="icon icon-gitlab"> Edit on GitLab</a>
+          <a href="https://gitlab.com/potato-oss/google-cloud/django-gcloud-connectors/edit/master/docs/installation.md" class="icon icon-gitlab"> Edit on GitLab</a>
     </li>
   </ul>
   <hr/>
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
             <div class="section" itemprop="articleBody">
               
                 <h1 id="installation">Installation</h1>
 <p>The most common way to install <code>gcloudc</code> is to use it as part of <a href="https://potato-oss.gitlab.io/djangae/djangae/">Djangae</a>.</p>
-<p>You can also install it on its own with <code>pip install glcoudc</code>.</p>
+<p>You can also install it on its own with <code>pip install django-gcloud-connectors</code>.</p>
 <p>However you install it, you will need to set your <code>DATABASES</code> configuration in your Django settings module to look something like this:</p>
 <pre><code class="language-python">from djangae
 DATABASES = {
     &quot;default&quot;: {
         'ENGINE': 'gcloudc.db.backends.datastore',
         'PROJECT': 'YOUR_GCP_PROJECT_NAME',  # You can use djangae.environment.project_id() here
         'INDEXES_FILE': 'PATH_TO_A_FILE_FOR_SPECICAL_INDEXES',
```

#### html2text {}

```diff
@@ -18,15 +18,15 @@
     Django_Gcloud_Connectors_Documentation
     *  »
     * Installation
     * Edit_on_GitLab
 ===============================================================================
 ****** Installation ******
 The most common way to install gcloudc is to use it as part of Djangae.
-You can also install it on its own with pip install glcoudc.
+You can also install it on its own with pip install django-gcloud-connectors.
 However you install it, you will need to set your DATABASES configuration in
 your Django settings module to look something like this:
 from djangae
 DATABASES = {
     "default": {
         'ENGINE': 'gcloudc.db.backends.datastore',
         'PROJECT': 'YOUR_GCP_PROJECT_NAME',  # You can use
```

### Comparing `django-gcloud-connectors-0.3.7/test/search.html` & `django-gcloud-connectors-0.4.0/test/search.html`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
   <div class="wy-grid-for-nav">
     <nav data-toggle="wy-nav-shift" class="wy-nav-side stickynav">
     <div class="wy-side-scroll">
       <div class="wy-side-nav-search">
           <a href="./." class="icon icon-home"> Django Gcloud Connectors Documentation
         </a><div role="search">
   <form id ="rtd-search-form" class="wy-form" action="./search.html" method="get">
-      <input type="text" name="q" placeholder="Search docs" title="Type search term here" />
+      <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" title="Type search term here" />
   </form>
 </div>
       </div>
 
       <div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
               <ul>
                 <li class="toctree-l1"><a class="reference internal" href="./.">Home</a>
@@ -74,29 +74,29 @@
           <i data-toggle="wy-nav-top" class="fa fa-bars"></i>
           <a href="./.">Django Gcloud Connectors Documentation</a>
         
       </nav>
       <div class="wy-nav-content">
         <div class="rst-content"><div role="navigation" aria-label="breadcrumbs navigation">
   <ul class="wy-breadcrumbs">
-    <li><a href="./." class="icon icon-home" alt="Docs"></a> &raquo;</li>
+    <li><a href="./." class="icon icon-home" aria-label="Docs"></a> &raquo;</li>
     <li class="wy-breadcrumbs-aside">
     </li>
   </ul>
   <hr/>
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
             <div class="section" itemprop="articleBody">
               
 
   <h1 id="search">Search Results</h1>
 
   <form id="content_search" action="search.html">
     <span role="status" aria-live="polite" class="ui-helper-hidden-accessible"></span>
-    <input name="q" id="mkdocs-search-query" type="text" class="search_input search-query ui-autocomplete-input" placeholder="Search the Docs" autocomplete="off" autofocus title="Type search term here">
+    <input name="q" id="mkdocs-search-query" type="text" class="search_input search-query ui-autocomplete-input" placeholder="Search the Docs" aria-label="Search the Docs" autocomplete="off" autofocus title="Type search term here">
   </form>
 
   <div id="mkdocs-search-results" class="search-results" data-no-results-text="No results found">
     Searching...
   </div>
```

### Comparing `django-gcloud-connectors-0.3.7/test/transactions/index.html` & `django-gcloud-connectors-0.4.0/test/transactions/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
   <div class="wy-grid-for-nav">
     <nav data-toggle="wy-nav-shift" class="wy-nav-side stickynav">
     <div class="wy-side-scroll">
       <div class="wy-side-nav-search">
           <a href=".." class="icon icon-home"> Django Gcloud Connectors Documentation
         </a><div role="search">
   <form id ="rtd-search-form" class="wy-form" action="../search.html" method="get">
-      <input type="text" name="q" placeholder="Search docs" title="Type search term here" />
+      <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" title="Type search term here" />
   </form>
 </div>
       </div>
 
       <div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
               <ul>
                 <li class="toctree-l1"><a class="reference internal" href="..">Home</a>
@@ -101,19 +101,18 @@
           <i data-toggle="wy-nav-top" class="fa fa-bars"></i>
           <a href="..">Django Gcloud Connectors Documentation</a>
         
       </nav>
       <div class="wy-nav-content">
         <div class="rst-content"><div role="navigation" aria-label="breadcrumbs navigation">
   <ul class="wy-breadcrumbs">
-    <li><a href=".." class="icon icon-home" alt="Docs"></a> &raquo;</li>
+    <li><a href=".." class="icon icon-home" aria-label="Docs"></a> &raquo;</li>
       <li>Transactions</li>
     <li class="wy-breadcrumbs-aside">
-        <a href="https://gitlab.com/potato-oss/google-cloud/django-gcloud-connectors/edit/master/docs/transactions.md"
-          class="icon icon-gitlab"> Edit on GitLab</a>
+          <a href="https://gitlab.com/potato-oss/google-cloud/django-gcloud-connectors/edit/master/docs/transactions.md" class="icon icon-gitlab"> Edit on GitLab</a>
     </li>
   </ul>
   <hr/>
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
             <div class="section" itemprop="articleBody">
```

### Comparing `django-gcloud-connectors-0.3.7/test/work_with_potato/index.html` & `django-gcloud-connectors-0.4.0/test/work_with_potato/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
   <div class="wy-grid-for-nav">
     <nav data-toggle="wy-nav-shift" class="wy-nav-side stickynav">
     <div class="wy-side-scroll">
       <div class="wy-side-nav-search">
           <a href=".." class="icon icon-home"> Django Gcloud Connectors Documentation
         </a><div role="search">
   <form id ="rtd-search-form" class="wy-form" action="../search.html" method="get">
-      <input type="text" name="q" placeholder="Search docs" title="Type search term here" />
+      <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" title="Type search term here" />
   </form>
 </div>
       </div>
 
       <div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
               <ul>
                 <li class="toctree-l1"><a class="reference internal" href="..">Home</a>
@@ -83,19 +83,18 @@
           <i data-toggle="wy-nav-top" class="fa fa-bars"></i>
           <a href="..">Django Gcloud Connectors Documentation</a>
         
       </nav>
       <div class="wy-nav-content">
         <div class="rst-content"><div role="navigation" aria-label="breadcrumbs navigation">
   <ul class="wy-breadcrumbs">
-    <li><a href=".." class="icon icon-home" alt="Docs"></a> &raquo;</li>
+    <li><a href=".." class="icon icon-home" aria-label="Docs"></a> &raquo;</li>
       <li>Work with us!</li>
     <li class="wy-breadcrumbs-aside">
-        <a href="https://gitlab.com/potato-oss/google-cloud/django-gcloud-connectors/edit/master/docs/work_with_potato.md"
-          class="icon icon-gitlab"> Edit on GitLab</a>
+          <a href="https://gitlab.com/potato-oss/google-cloud/django-gcloud-connectors/edit/master/docs/work_with_potato.md" class="icon icon-gitlab"> Edit on GitLab</a>
     </li>
   </ul>
   <hr/>
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
             <div class="section" itemprop="articleBody">
```

