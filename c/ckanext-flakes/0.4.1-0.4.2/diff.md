# Comparing `tmp/ckanext-flakes-0.4.1.tar.gz` & `tmp/ckanext-flakes-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-flakes-0.4.1.tar", last modified: Sun Jun 11 11:26:05 2023, max compression
+gzip compressed data, was "ckanext-flakes-0.4.2.tar", last modified: Wed Jun 21 13:08:01 2023, max compression
```

## Comparing `ckanext-flakes-0.4.1.tar` & `ckanext-flakes-0.4.2.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-11 11:26:05.768905 ckanext-flakes-0.4.1/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    34500 2022-10-25 15:10:26.000000 ckanext-flakes-0.4.1/LICENSE
--rw-r--r--   0 sergey    (1000) sergey    (1000)      204 2023-03-11 13:04:37.000000 ckanext-flakes-0.4.1/MANIFEST.in
--rw-r--r--   0 sergey    (1000) sergey    (1000)    13698 2023-06-11 11:26:05.768905 ckanext-flakes-0.4.1/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)    13078 2023-04-12 09:35:34.000000 ckanext-flakes-0.4.1/README.md
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-11 11:26:05.748905 ckanext-flakes-0.4.1/ckanext/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      221 2022-10-25 15:10:26.000000 ckanext-flakes-0.4.1/ckanext/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-11 11:26:05.748905 ckanext-flakes-0.4.1/ckanext/flakes/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-25 15:10:26.000000 ckanext-flakes-0.4.1/ckanext/flakes/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      430 2023-03-11 10:05:29.000000 ckanext-flakes-0.4.1/ckanext/flakes/config_declaration.yaml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1263 2022-10-25 15:10:26.000000 ckanext-flakes-0.4.1/ckanext/flakes/interfaces.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-11 11:26:05.748905 ckanext-flakes-0.4.1/ckanext/flakes/logic/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-25 15:10:26.000000 ckanext-flakes-0.4.1/ckanext/flakes/logic/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)    12927 2023-03-23 22:28:12.000000 ckanext-flakes-0.4.1/ckanext/flakes/logic/action.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2932 2023-03-11 09:14:54.000000 ckanext-flakes-0.4.1/ckanext/flakes/logic/auth.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4241 2023-03-23 22:28:12.000000 ckanext-flakes-0.4.1/ckanext/flakes/logic/schema.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      663 2022-10-25 15:10:26.000000 ckanext-flakes-0.4.1/ckanext/flakes/logic/validators.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-11 11:26:05.738905 ckanext-flakes-0.4.1/ckanext/flakes/migration/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-11 11:26:05.748905 ckanext-flakes-0.4.1/ckanext/flakes/migration/flakes/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1780 2022-10-25 15:10:26.000000 ckanext-flakes-0.4.1/ckanext/flakes/migration/flakes/alembic.ini
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2228 2022-10-25 15:10:26.000000 ckanext-flakes-0.4.1/ckanext/flakes/migration/flakes/env.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      494 2022-10-25 15:10:26.000000 ckanext-flakes-0.4.1/ckanext/flakes/migration/flakes/script.py.mako
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-11 11:26:05.748905 ckanext-flakes-0.4.1/ckanext/flakes/migration/flakes/versions/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      439 2023-03-11 04:52:30.000000 ckanext-flakes-0.4.1/ckanext/flakes/migration/flakes/versions/a7384c7e0e27_nullable_author.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1114 2023-03-11 09:14:54.000000 ckanext-flakes-0.4.1/ckanext/flakes/migration/flakes/versions/b8a5f5419306_create_flake_table.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-11 11:26:05.748905 ckanext-flakes-0.4.1/ckanext/flakes/model/
--rw-r--r--   0 sergey    (1000) sergey    (1000)       46 2022-10-25 15:10:26.000000 ckanext-flakes-0.4.1/ckanext/flakes/model/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      139 2023-03-09 06:46:46.000000 ckanext-flakes-0.4.1/ckanext/flakes/model/base.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3028 2023-03-23 22:28:12.000000 ckanext-flakes-0.4.1/ckanext/flakes/model/flake.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1934 2023-05-10 13:57:04.000000 ckanext-flakes-0.4.1/ckanext/flakes/plugin.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-11 11:26:05.748905 ckanext-flakes-0.4.1/ckanext/flakes/plugins/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-25 15:10:26.000000 ckanext-flakes-0.4.1/ckanext/flakes/plugins/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-11 11:26:05.748905 ckanext-flakes-0.4.1/ckanext/flakes/plugins/feedback/
--rw-r--r--   0 sergey    (1000) sergey    (1000)       84 2023-03-23 14:32:10.000000 ckanext-flakes-0.4.1/ckanext/flakes/plugins/feedback/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-11 11:26:05.748905 ckanext-flakes-0.4.1/ckanext/flakes/plugins/feedback/assets/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      159 2023-03-23 14:34:44.000000 ckanext-flakes-0.4.1/ckanext/flakes/plugins/feedback/assets/webassets.yml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      507 2023-06-11 11:17:31.000000 ckanext-flakes-0.4.1/ckanext/flakes/plugins/feedback/config_declaration.yaml
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-11 11:26:05.758905 ckanext-flakes-0.4.1/ckanext/flakes/plugins/feedback/logic/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-03-23 18:32:20.000000 ckanext-flakes-0.4.1/ckanext/flakes/plugins/feedback/logic/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4596 2023-06-11 11:24:03.000000 ckanext-flakes-0.4.1/ckanext/flakes/plugins/feedback/logic/action.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      844 2023-03-23 22:28:12.000000 ckanext-flakes-0.4.1/ckanext/flakes/plugins/feedback/logic/auth.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1048 2023-06-07 15:18:49.000000 ckanext-flakes-0.4.1/ckanext/flakes/plugins/feedback/logic/schema.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1130 2023-03-23 22:28:12.000000 ckanext-flakes-0.4.1/ckanext/flakes/plugins/feedback/plugin.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-11 11:26:05.748905 ckanext-flakes-0.4.1/ckanext/flakes/plugins/feedback/templates/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-11 11:26:05.758905 ckanext-flakes-0.4.1/ckanext/flakes/plugins/feedback/templates/flakes_feedback/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      704 2023-03-23 22:16:21.000000 ckanext-flakes-0.4.1/ckanext/flakes/plugins/feedback/templates/flakes_feedback/delete.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1594 2023-06-07 15:43:55.000000 ckanext-flakes-0.4.1/ckanext/flakes/plugins/feedback/templates/flakes_feedback/index.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1314 2023-03-23 22:21:28.000000 ckanext-flakes-0.4.1/ckanext/flakes/plugins/feedback/templates/flakes_feedback/post.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-11 11:26:05.758905 ckanext-flakes-0.4.1/ckanext/flakes/plugins/feedback/templates/package/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      269 2023-04-12 09:33:57.000000 ckanext-flakes-0.4.1/ckanext/flakes/plugins/feedback/templates/package/read_base.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4502 2023-06-11 11:19:27.000000 ckanext-flakes-0.4.1/ckanext/flakes/plugins/feedback/views.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-11 11:26:05.758905 ckanext-flakes-0.4.1/ckanext/flakes/plugins/rating/
--rw-r--r--   0 sergey    (1000) sergey    (1000)       80 2023-03-11 13:07:23.000000 ckanext-flakes-0.4.1/ckanext/flakes/plugins/rating/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-11 11:26:05.758905 ckanext-flakes-0.4.1/ckanext/flakes/plugins/rating/assets/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1421 2023-04-19 15:41:33.000000 ckanext-flakes-0.4.1/ckanext/flakes/plugins/rating/assets/flakes-rating-rate.js
--rw-r--r--   0 sergey    (1000) sergey    (1000)      145 2022-11-07 20:13:24.000000 ckanext-flakes-0.4.1/ckanext/flakes/plugins/rating/assets/webassets.yml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      638 2023-03-23 14:47:46.000000 ckanext-flakes-0.4.1/ckanext/flakes/plugins/rating/config.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      589 2023-03-23 14:46:56.000000 ckanext-flakes-0.4.1/ckanext/flakes/plugins/rating/config_declaration.yaml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      655 2023-03-23 22:28:12.000000 ckanext-flakes-0.4.1/ckanext/flakes/plugins/rating/helpers.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-11 11:26:05.758905 ckanext-flakes-0.4.1/ckanext/flakes/plugins/rating/logic/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-11-07 20:13:24.000000 ckanext-flakes-0.4.1/ckanext/flakes/plugins/rating/logic/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3401 2023-03-23 22:28:12.000000 ckanext-flakes-0.4.1/ckanext/flakes/plugins/rating/logic/action.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      903 2023-03-23 22:28:12.000000 ckanext-flakes-0.4.1/ckanext/flakes/plugins/rating/logic/auth.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1286 2023-03-23 22:28:12.000000 ckanext-flakes-0.4.1/ckanext/flakes/plugins/rating/logic/schema.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      854 2023-03-23 22:28:12.000000 ckanext-flakes-0.4.1/ckanext/flakes/plugins/rating/plugin.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-11 11:26:05.748905 ckanext-flakes-0.4.1/ckanext/flakes/plugins/rating/templates/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-11 11:26:05.748905 ckanext-flakes-0.4.1/ckanext/flakes/plugins/rating/templates/flakes_rating/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-11 11:26:05.758905 ckanext-flakes-0.4.1/ckanext/flakes/plugins/rating/templates/flakes_rating/snippets/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1469 2023-04-19 13:33:00.000000 ckanext-flakes-0.4.1/ckanext/flakes/plugins/rating/templates/flakes_rating/snippets/rate_widget.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-11 11:26:05.758905 ckanext-flakes-0.4.1/ckanext/flakes/plugins/rating/templates/package/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      530 2023-03-23 14:45:35.000000 ckanext-flakes-0.4.1/ckanext/flakes/plugins/rating/templates/package/read_base.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1376 2022-10-25 15:10:26.000000 ckanext-flakes-0.4.1/ckanext/flakes/plugins/scheming.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-11 11:26:05.758905 ckanext-flakes-0.4.1/ckanext/flakes/tests/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-25 15:10:26.000000 ckanext-flakes-0.4.1/ckanext/flakes/tests/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      423 2023-03-09 06:46:46.000000 ckanext-flakes-0.4.1/ckanext/flakes/tests/conftest.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      186 2022-10-25 15:10:26.000000 ckanext-flakes-0.4.1/ckanext/flakes/tests/flake_dataset.yaml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      130 2022-10-25 15:10:26.000000 ckanext-flakes-0.4.1/ckanext/flakes/tests/flake_group.yaml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      144 2022-10-25 15:10:26.000000 ckanext-flakes-0.4.1/ckanext/flakes/tests/flake_organization.yaml
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-11 11:26:05.758905 ckanext-flakes-0.4.1/ckanext/flakes/tests/logic/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-25 15:10:26.000000 ckanext-flakes-0.4.1/ckanext/flakes/tests/logic/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)    17166 2023-03-11 09:14:54.000000 ckanext-flakes-0.4.1/ckanext/flakes/tests/logic/test_action.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6713 2023-03-11 09:14:54.000000 ckanext-flakes-0.4.1/ckanext/flakes/tests/logic/test_auth.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1606 2023-03-09 06:46:46.000000 ckanext-flakes-0.4.1/ckanext/flakes/tests/logic/test_validators.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-11 11:26:05.758905 ckanext-flakes-0.4.1/ckanext/flakes/tests/model/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-25 15:10:26.000000 ckanext-flakes-0.4.1/ckanext/flakes/tests/model/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5762 2023-03-11 09:14:54.000000 ckanext-flakes-0.4.1/ckanext/flakes/tests/model/test_flake.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      311 2022-10-25 15:10:26.000000 ckanext-flakes-0.4.1/ckanext/flakes/tests/plugin.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-11 11:26:05.758905 ckanext-flakes-0.4.1/ckanext/flakes/tests/plugins/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-25 15:10:26.000000 ckanext-flakes-0.4.1/ckanext/flakes/tests/plugins/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2254 2023-03-09 06:46:46.000000 ckanext-flakes-0.4.1/ckanext/flakes/tests/plugins/test_scheming.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      449 2023-03-09 06:46:46.000000 ckanext-flakes-0.4.1/ckanext/flakes/tests/test_plugin.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2513 2023-03-09 06:46:46.000000 ckanext-flakes-0.4.1/ckanext/flakes/types.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-11 11:26:05.768905 ckanext-flakes-0.4.1/ckanext_flakes.egg-info/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    13698 2023-06-11 11:26:05.000000 ckanext-flakes-0.4.1/ckanext_flakes.egg-info/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3065 2023-06-11 11:26:05.000000 ckanext-flakes-0.4.1/ckanext_flakes.egg-info/SOURCES.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-06-11 11:26:05.000000 ckanext-flakes-0.4.1/ckanext_flakes.egg-info/dependency_links.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)      403 2023-06-11 11:26:05.000000 ckanext-flakes-0.4.1/ckanext_flakes.egg-info/entry_points.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-06-11 11:26:05.000000 ckanext-flakes-0.4.1/ckanext_flakes.egg-info/namespace_packages.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       55 2023-06-11 11:26:05.000000 ckanext-flakes-0.4.1/ckanext_flakes.egg-info/requires.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-06-11 11:26:05.000000 ckanext-flakes-0.4.1/ckanext_flakes.egg-info/top_level.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2820 2023-03-11 09:14:51.000000 ckanext-flakes-0.4.1/pyproject.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-25 15:10:26.000000 ckanext-flakes-0.4.1/requirements.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1927 2023-06-11 11:26:05.768905 ckanext-flakes-0.4.1/setup.cfg
--rw-r--r--   0 sergey    (1000) sergey    (1000)      528 2022-10-25 15:10:26.000000 ckanext-flakes-0.4.1/setup.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-21 13:08:01.686298 ckanext-flakes-0.4.2/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    34500 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/LICENSE
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      204 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/MANIFEST.in
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    13698 2023-06-21 13:08:01.686298 ckanext-flakes-0.4.2/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    13078 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/README.md
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-21 13:08:01.686298 ckanext-flakes-0.4.2/ckanext/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      221 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-21 13:08:01.686298 ckanext-flakes-0.4.2/ckanext/flakes/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      430 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/config_declaration.yaml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1263 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/interfaces.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-21 13:08:01.686298 ckanext-flakes-0.4.2/ckanext/flakes/logic/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/logic/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    12927 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/logic/action.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2932 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/logic/auth.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4241 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/logic/schema.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      663 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/logic/validators.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-21 13:08:01.676299 ckanext-flakes-0.4.2/ckanext/flakes/migration/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-21 13:08:01.686298 ckanext-flakes-0.4.2/ckanext/flakes/migration/flakes/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1780 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/migration/flakes/alembic.ini
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2228 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/migration/flakes/env.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      494 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/migration/flakes/script.py.mako
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-21 13:08:01.686298 ckanext-flakes-0.4.2/ckanext/flakes/migration/flakes/versions/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      439 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/migration/flakes/versions/a7384c7e0e27_nullable_author.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1114 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/migration/flakes/versions/b8a5f5419306_create_flake_table.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-21 13:08:01.686298 ckanext-flakes-0.4.2/ckanext/flakes/model/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       46 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/model/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      139 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/model/base.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3028 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/model/flake.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1934 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/plugin.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-21 13:08:01.686298 ckanext-flakes-0.4.2/ckanext/flakes/plugins/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/plugins/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-21 13:08:01.686298 ckanext-flakes-0.4.2/ckanext/flakes/plugins/feedback/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       84 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/plugins/feedback/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-21 13:08:01.686298 ckanext-flakes-0.4.2/ckanext/flakes/plugins/feedback/assets/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      159 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/plugins/feedback/assets/webassets.yml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      507 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/plugins/feedback/config_declaration.yaml
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-21 13:08:01.686298 ckanext-flakes-0.4.2/ckanext/flakes/plugins/feedback/logic/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/plugins/feedback/logic/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4607 2023-06-21 13:02:21.000000 ckanext-flakes-0.4.2/ckanext/flakes/plugins/feedback/logic/action.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      844 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/plugins/feedback/logic/auth.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1048 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/plugins/feedback/logic/schema.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1130 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/plugins/feedback/plugin.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-21 13:08:01.686298 ckanext-flakes-0.4.2/ckanext/flakes/plugins/feedback/templates/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-21 13:08:01.686298 ckanext-flakes-0.4.2/ckanext/flakes/plugins/feedback/templates/flakes_feedback/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      704 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/plugins/feedback/templates/flakes_feedback/delete.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1594 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/plugins/feedback/templates/flakes_feedback/index.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1314 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/plugins/feedback/templates/flakes_feedback/post.html
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-21 13:08:01.686298 ckanext-flakes-0.4.2/ckanext/flakes/plugins/feedback/templates/package/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      269 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/plugins/feedback/templates/package/read_base.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4502 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/plugins/feedback/views.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-21 13:08:01.686298 ckanext-flakes-0.4.2/ckanext/flakes/plugins/rating/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       80 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/plugins/rating/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-21 13:08:01.686298 ckanext-flakes-0.4.2/ckanext/flakes/plugins/rating/assets/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1421 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/plugins/rating/assets/flakes-rating-rate.js
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      145 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/plugins/rating/assets/webassets.yml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      638 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/plugins/rating/config.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      589 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/plugins/rating/config_declaration.yaml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      655 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/plugins/rating/helpers.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-21 13:08:01.686298 ckanext-flakes-0.4.2/ckanext/flakes/plugins/rating/logic/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/plugins/rating/logic/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3401 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/plugins/rating/logic/action.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      903 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/plugins/rating/logic/auth.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1286 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/plugins/rating/logic/schema.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      854 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/plugins/rating/plugin.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-21 13:08:01.686298 ckanext-flakes-0.4.2/ckanext/flakes/plugins/rating/templates/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-21 13:08:01.686298 ckanext-flakes-0.4.2/ckanext/flakes/plugins/rating/templates/flakes_rating/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-21 13:08:01.686298 ckanext-flakes-0.4.2/ckanext/flakes/plugins/rating/templates/flakes_rating/snippets/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1469 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/plugins/rating/templates/flakes_rating/snippets/rate_widget.html
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-21 13:08:01.686298 ckanext-flakes-0.4.2/ckanext/flakes/plugins/rating/templates/package/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      530 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/plugins/rating/templates/package/read_base.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1376 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/plugins/scheming.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-21 13:08:01.686298 ckanext-flakes-0.4.2/ckanext/flakes/tests/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/tests/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      423 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/tests/conftest.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      186 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/tests/flake_dataset.yaml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      130 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/tests/flake_group.yaml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      144 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/tests/flake_organization.yaml
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-21 13:08:01.686298 ckanext-flakes-0.4.2/ckanext/flakes/tests/logic/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/tests/logic/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    17166 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/tests/logic/test_action.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6713 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/tests/logic/test_auth.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1606 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/tests/logic/test_validators.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-21 13:08:01.686298 ckanext-flakes-0.4.2/ckanext/flakes/tests/model/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/tests/model/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5762 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/tests/model/test_flake.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      311 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/tests/plugin.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-21 13:08:01.686298 ckanext-flakes-0.4.2/ckanext/flakes/tests/plugins/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/tests/plugins/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2254 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/tests/plugins/test_scheming.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      449 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/tests/test_plugin.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2513 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/ckanext/flakes/types.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-21 13:08:01.686298 ckanext-flakes-0.4.2/ckanext_flakes.egg-info/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    13698 2023-06-21 13:08:01.000000 ckanext-flakes-0.4.2/ckanext_flakes.egg-info/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3065 2023-06-21 13:08:01.000000 ckanext-flakes-0.4.2/ckanext_flakes.egg-info/SOURCES.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-06-21 13:08:01.000000 ckanext-flakes-0.4.2/ckanext_flakes.egg-info/dependency_links.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      403 2023-06-21 13:08:01.000000 ckanext-flakes-0.4.2/ckanext_flakes.egg-info/entry_points.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-06-21 13:08:01.000000 ckanext-flakes-0.4.2/ckanext_flakes.egg-info/namespace_packages.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       55 2023-06-21 13:08:01.000000 ckanext-flakes-0.4.2/ckanext_flakes.egg-info/requires.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-06-21 13:08:01.000000 ckanext-flakes-0.4.2/ckanext_flakes.egg-info/top_level.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2820 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/pyproject.toml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/requirements.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1927 2023-06-21 13:08:01.686298 ckanext-flakes-0.4.2/setup.cfg
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      528 2023-06-21 12:32:03.000000 ckanext-flakes-0.4.2/setup.py
```

### Comparing `ckanext-flakes-0.4.1/LICENSE` & `ckanext-flakes-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.4.1/PKG-INFO` & `ckanext-flakes-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-flakes
-Version: 0.4.1
+Version: 0.4.2
 Home-page: https://github.com/DataShades/ckanext-flakes
 Author: Sergey Motornyuk
 Author-email: sergey.motornyuk@linkdigital.com.au
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `ckanext-flakes-0.4.1/README.md` & `ckanext-flakes-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.4.1/ckanext/flakes/interfaces.py` & `ckanext-flakes-0.4.2/ckanext/flakes/interfaces.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.4.1/ckanext/flakes/logic/action.py` & `ckanext-flakes-0.4.2/ckanext/flakes/logic/action.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.4.1/ckanext/flakes/logic/auth.py` & `ckanext-flakes-0.4.2/ckanext/flakes/logic/auth.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.4.1/ckanext/flakes/logic/schema.py` & `ckanext-flakes-0.4.2/ckanext/flakes/logic/schema.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.4.1/ckanext/flakes/logic/validators.py` & `ckanext-flakes-0.4.2/ckanext/flakes/logic/validators.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.4.1/ckanext/flakes/migration/flakes/alembic.ini` & `ckanext-flakes-0.4.2/ckanext/flakes/migration/flakes/alembic.ini`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.4.1/ckanext/flakes/migration/flakes/env.py` & `ckanext-flakes-0.4.2/ckanext/flakes/migration/flakes/env.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.4.1/ckanext/flakes/migration/flakes/versions/b8a5f5419306_create_flake_table.py` & `ckanext-flakes-0.4.2/ckanext/flakes/migration/flakes/versions/b8a5f5419306_create_flake_table.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.4.1/ckanext/flakes/model/flake.py` & `ckanext-flakes-0.4.2/ckanext/flakes/model/flake.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.4.1/ckanext/flakes/plugin.py` & `ckanext-flakes-0.4.2/ckanext/flakes/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.4.1/ckanext/flakes/plugins/feedback/logic/action.py` & `ckanext-flakes-0.4.2/ckanext/flakes/plugins/feedback/logic/action.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
                 "secondary_key": secondary_key,
             }
         },
     }
 
     try:
         existing = tk.get_action("flakes_feedback_feedback_lookup")(
-            {},
+            dict(context),
             {
                 "package_id": pkg.id,
                 "secondary_key": secondary_key,
             },
         )
     except tk.ObjectNotFound:
         payload["name"] = _name(pkg.id, secondary_key)
```

### Comparing `ckanext-flakes-0.4.1/ckanext/flakes/plugins/feedback/logic/auth.py` & `ckanext-flakes-0.4.2/ckanext/flakes/plugins/feedback/logic/auth.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.4.1/ckanext/flakes/plugins/feedback/logic/schema.py` & `ckanext-flakes-0.4.2/ckanext/flakes/plugins/feedback/logic/schema.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.4.1/ckanext/flakes/plugins/feedback/plugin.py` & `ckanext-flakes-0.4.2/ckanext/flakes/plugins/feedback/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.4.1/ckanext/flakes/plugins/feedback/templates/flakes_feedback/delete.html` & `ckanext-flakes-0.4.2/ckanext/flakes/plugins/feedback/templates/flakes_feedback/delete.html`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.4.1/ckanext/flakes/plugins/feedback/templates/flakes_feedback/index.html` & `ckanext-flakes-0.4.2/ckanext/flakes/plugins/feedback/templates/flakes_feedback/index.html`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.4.1/ckanext/flakes/plugins/feedback/templates/flakes_feedback/post.html` & `ckanext-flakes-0.4.2/ckanext/flakes/plugins/feedback/templates/flakes_feedback/post.html`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.4.1/ckanext/flakes/plugins/feedback/views.py` & `ckanext-flakes-0.4.2/ckanext/flakes/plugins/feedback/views.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.4.1/ckanext/flakes/plugins/rating/assets/flakes-rating-rate.js` & `ckanext-flakes-0.4.2/ckanext/flakes/plugins/rating/assets/flakes-rating-rate.js`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.4.1/ckanext/flakes/plugins/rating/config.py` & `ckanext-flakes-0.4.2/ckanext/flakes/plugins/rating/config.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.4.1/ckanext/flakes/plugins/rating/config_declaration.yaml` & `ckanext-flakes-0.4.2/ckanext/flakes/plugins/rating/config_declaration.yaml`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.4.1/ckanext/flakes/plugins/rating/helpers.py` & `ckanext-flakes-0.4.2/ckanext/flakes/plugins/rating/helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.4.1/ckanext/flakes/plugins/rating/logic/action.py` & `ckanext-flakes-0.4.2/ckanext/flakes/plugins/rating/logic/action.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.4.1/ckanext/flakes/plugins/rating/logic/auth.py` & `ckanext-flakes-0.4.2/ckanext/flakes/plugins/rating/logic/auth.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.4.1/ckanext/flakes/plugins/rating/logic/schema.py` & `ckanext-flakes-0.4.2/ckanext/flakes/plugins/rating/logic/schema.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.4.1/ckanext/flakes/plugins/rating/plugin.py` & `ckanext-flakes-0.4.2/ckanext/flakes/plugins/rating/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.4.1/ckanext/flakes/plugins/rating/templates/flakes_rating/snippets/rate_widget.html` & `ckanext-flakes-0.4.2/ckanext/flakes/plugins/rating/templates/flakes_rating/snippets/rate_widget.html`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.4.1/ckanext/flakes/plugins/rating/templates/package/read_base.html` & `ckanext-flakes-0.4.2/ckanext/flakes/plugins/rating/templates/package/read_base.html`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.4.1/ckanext/flakes/plugins/scheming.py` & `ckanext-flakes-0.4.2/ckanext/flakes/plugins/scheming.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.4.1/ckanext/flakes/tests/logic/test_action.py` & `ckanext-flakes-0.4.2/ckanext/flakes/tests/logic/test_action.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.4.1/ckanext/flakes/tests/logic/test_auth.py` & `ckanext-flakes-0.4.2/ckanext/flakes/tests/logic/test_auth.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.4.1/ckanext/flakes/tests/logic/test_validators.py` & `ckanext-flakes-0.4.2/ckanext/flakes/tests/logic/test_validators.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.4.1/ckanext/flakes/tests/model/test_flake.py` & `ckanext-flakes-0.4.2/ckanext/flakes/tests/model/test_flake.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.4.1/ckanext/flakes/tests/plugins/test_scheming.py` & `ckanext-flakes-0.4.2/ckanext/flakes/tests/plugins/test_scheming.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.4.1/ckanext/flakes/types.py` & `ckanext-flakes-0.4.2/ckanext/flakes/types.py`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.4.1/ckanext_flakes.egg-info/PKG-INFO` & `ckanext-flakes-0.4.2/ckanext_flakes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-flakes
-Version: 0.4.1
+Version: 0.4.2
 Home-page: https://github.com/DataShades/ckanext-flakes
 Author: Sergey Motornyuk
 Author-email: sergey.motornyuk@linkdigital.com.au
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `ckanext-flakes-0.4.1/ckanext_flakes.egg-info/SOURCES.txt` & `ckanext-flakes-0.4.2/ckanext_flakes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.4.1/pyproject.toml` & `ckanext-flakes-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ckanext-flakes-0.4.1/setup.cfg` & `ckanext-flakes-0.4.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ckanext-flakes
-version = 0.4.1
+version = 0.4.2
 description = 
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/DataShades/ckanext-flakes
 author = Sergey Motornyuk
 author_email = sergey.motornyuk@linkdigital.com.au
 license = AGPL
```

### Comparing `ckanext-flakes-0.4.1/setup.py` & `ckanext-flakes-0.4.2/setup.py`

 * *Files identical despite different names*

