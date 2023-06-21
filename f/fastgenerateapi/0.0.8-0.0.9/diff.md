# Comparing `tmp/fastgenerateapi-0.0.8.tar.gz` & `tmp/fastgenerateapi-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastgenerateapi-0.0.8.tar", last modified: Wed Jun 21 03:21:11 2023, max compression
+gzip compressed data, was "fastgenerateapi-0.0.9.tar", last modified: Wed Jun 21 03:45:55 2023, max compression
```

## Comparing `fastgenerateapi-0.0.8.tar` & `fastgenerateapi-0.0.9.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 03:21:11.019039 fastgenerateapi-0.0.8/
--rw-rw-rw-   0        0        0    35821 2023-06-15 11:33:13.000000 fastgenerateapi-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     4383 2023-06-21 03:21:11.019039 fastgenerateapi-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3741 2023-06-21 03:19:46.000000 fastgenerateapi-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-21 03:21:10.940278 fastgenerateapi-0.0.8/fastgenerateapi/
--rw-rw-rw-   0        0        0     1022 2023-06-19 06:02:37.000000 fastgenerateapi-0.0.8/fastgenerateapi/__init__.py
--rw-rw-rw-   0        0        0      496 2023-06-21 01:21:22.000000 fastgenerateapi-0.0.8/fastgenerateapi/__version__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 03:21:10.971546 fastgenerateapi-0.0.8/fastgenerateapi/api_view/
--rw-rw-rw-   0        0        0       14 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.8/fastgenerateapi/api_view/__init__.py
--rw-rw-rw-   0        0        0     1160 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.8/fastgenerateapi/api_view/api_view.py
--rw-rw-rw-   0        0        0     9518 2023-06-21 01:20:11.000000 fastgenerateapi-0.0.8/fastgenerateapi/api_view/base_view.py
--rw-rw-rw-   0        0        0     4177 2023-06-16 00:58:02.000000 fastgenerateapi-0.0.8/fastgenerateapi/api_view/create_view.py
--rw-rw-rw-   0        0        0     3628 2023-06-19 06:02:37.000000 fastgenerateapi-0.0.8/fastgenerateapi/api_view/delete_tree_view.py
--rw-rw-rw-   0        0        0     3035 2023-06-19 06:02:37.000000 fastgenerateapi-0.0.8/fastgenerateapi/api_view/delete_view.py
--rw-rw-rw-   0        0        0     7469 2023-06-19 06:02:37.000000 fastgenerateapi-0.0.8/fastgenerateapi/api_view/get_all_view.py
--rw-rw-rw-   0        0        0     3077 2023-06-19 06:02:37.000000 fastgenerateapi-0.0.8/fastgenerateapi/api_view/get_one_view.py
--rw-rw-rw-   0        0        0     9795 2023-06-19 06:02:37.000000 fastgenerateapi-0.0.8/fastgenerateapi/api_view/get_relation_view.py
--rw-rw-rw-   0        0        0     7275 2023-06-19 06:02:37.000000 fastgenerateapi-0.0.8/fastgenerateapi/api_view/get_tree_view.py
-drwxrwxrwx   0        0        0        0 2023-06-21 03:21:10.987793 fastgenerateapi-0.0.8/fastgenerateapi/api_view/mixin/
--rw-rw-rw-   0        0        0        0 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.8/fastgenerateapi/api_view/mixin/__init__.py
--rw-rw-rw-   0        0        0     4453 2023-06-19 06:02:37.000000 fastgenerateapi-0.0.8/fastgenerateapi/api_view/mixin/base_mixin.py
--rw-rw-rw-   0        0        0     3826 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.8/fastgenerateapi/api_view/mixin/dbmodel_mixin.py
--rw-rw-rw-   0        0        0      266 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.8/fastgenerateapi/api_view/mixin/get_mixin.py
--rw-rw-rw-   0        0        0     2290 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.8/fastgenerateapi/api_view/mixin/response_mixin.py
--rw-rw-rw-   0        0        0      317 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.8/fastgenerateapi/api_view/mixin/save_mixin.py
--rw-rw-rw-   0        0        0    13529 2023-06-21 01:11:03.000000 fastgenerateapi-0.0.8/fastgenerateapi/api_view/mixin/tool_mixin.py
--rw-rw-rw-   0        0        0     6899 2023-06-21 01:11:03.000000 fastgenerateapi-0.0.8/fastgenerateapi/api_view/sql_get_view.py
--rw-rw-rw-   0        0        0     3070 2023-06-16 01:29:40.000000 fastgenerateapi-0.0.8/fastgenerateapi/api_view/switch_view.py
--rw-rw-rw-   0        0        0     3553 2023-06-19 06:02:37.000000 fastgenerateapi-0.0.8/fastgenerateapi/api_view/update_relation_view.py
--rw-rw-rw-   0        0        0     4006 2023-06-16 03:02:52.000000 fastgenerateapi-0.0.8/fastgenerateapi/api_view/update_view.py
-drwxrwxrwx   0        0        0        0 2023-06-21 03:21:10.987793 fastgenerateapi-0.0.8/fastgenerateapi/controller/
--rw-rw-rw-   0        0        0      316 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.8/fastgenerateapi/controller/__init__.py
--rw-rw-rw-   0        0        0     3391 2023-06-16 00:44:07.000000 fastgenerateapi-0.0.8/fastgenerateapi/controller/filter_controller.py
--rw-rw-rw-   0        0        0     3341 2023-06-21 01:20:11.000000 fastgenerateapi-0.0.8/fastgenerateapi/controller/router_controller.py
--rw-rw-rw-   0        0        0     2298 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.8/fastgenerateapi/controller/rpc_controller.py
--rw-rw-rw-   0        0        0      873 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.8/fastgenerateapi/controller/search_controller.py
-drwxrwxrwx   0        0        0        0 2023-06-21 03:21:10.987793 fastgenerateapi-0.0.8/fastgenerateapi/data_type/
--rw-rw-rw-   0        0        0        0 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.8/fastgenerateapi/data_type/__init__.py
--rw-rw-rw-   0        0        0      727 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.8/fastgenerateapi/data_type/data_type.py
-drwxrwxrwx   0        0        0        0 2023-06-21 03:21:10.987793 fastgenerateapi-0.0.8/fastgenerateapi/deps/
--rw-rw-rw-   0        0        0      160 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.8/fastgenerateapi/deps/__init__.py
--rw-rw-rw-   0        0        0      813 2023-06-16 02:41:05.000000 fastgenerateapi-0.0.8/fastgenerateapi/deps/filter_params_deps.py
--rw-rw-rw-   0        0        0     3171 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.8/fastgenerateapi/deps/paginator_deps.py
--rw-rw-rw-   0        0        0     1264 2023-06-19 06:02:37.000000 fastgenerateapi-0.0.8/fastgenerateapi/deps/tree_params_deps.py
-drwxrwxrwx   0        0        0        0 2023-06-21 03:21:11.003419 fastgenerateapi-0.0.8/fastgenerateapi/example/
--rw-rw-rw-   0        0        0        0 2023-06-15 11:43:17.000000 fastgenerateapi-0.0.8/fastgenerateapi/example/__init__.py
--rw-rw-rw-   0        0        0     1611 2023-06-16 05:36:12.000000 fastgenerateapi-0.0.8/fastgenerateapi/example/models.py
--rw-rw-rw-   0        0        0      195 2023-06-15 11:43:17.000000 fastgenerateapi-0.0.8/fastgenerateapi/example/routers.py
--rw-rw-rw-   0        0        0      400 2023-06-16 05:42:12.000000 fastgenerateapi-0.0.8/fastgenerateapi/example/views.py
-drwxrwxrwx   0        0        0        0 2023-06-21 03:21:11.003419 fastgenerateapi-0.0.8/fastgenerateapi/pydantic_utils/
--rw-rw-rw-   0        0        0        0 2023-06-15 11:43:17.000000 fastgenerateapi-0.0.8/fastgenerateapi/pydantic_utils/__init__.py
--rw-rw-rw-   0        0        0      694 2023-06-16 00:57:41.000000 fastgenerateapi-0.0.8/fastgenerateapi/pydantic_utils/base_model.py
--rw-rw-rw-   0        0        0     2814 2023-06-15 11:43:17.000000 fastgenerateapi-0.0.8/fastgenerateapi/pydantic_utils/json_encoders.py
-drwxrwxrwx   0        0        0        0 2023-06-21 03:21:11.019039 fastgenerateapi-0.0.8/fastgenerateapi/schemas_factory/
--rw-rw-rw-   0        0        0      472 2023-06-15 11:43:17.000000 fastgenerateapi-0.0.8/fastgenerateapi/schemas_factory/__init__.py
--rw-rw-rw-   0        0        0     4305 2023-06-16 00:44:35.000000 fastgenerateapi-0.0.8/fastgenerateapi/schemas_factory/common_function.py
--rw-rw-rw-   0        0        0     2292 2023-06-16 01:54:38.000000 fastgenerateapi-0.0.8/fastgenerateapi/schemas_factory/create_schema_factory.py
--rw-rw-rw-   0        0        0     1284 2023-06-16 02:48:31.000000 fastgenerateapi-0.0.8/fastgenerateapi/schemas_factory/filter_schema_factory.py
--rw-rw-rw-   0        0        0     3303 2023-06-16 06:01:18.000000 fastgenerateapi-0.0.8/fastgenerateapi/schemas_factory/get_all_schema_factory.py
--rw-rw-rw-   0        0        0     2194 2023-06-16 06:01:18.000000 fastgenerateapi-0.0.8/fastgenerateapi/schemas_factory/get_one_schema_factory.py
--rw-rw-rw-   0        0        0     2391 2023-06-19 06:02:37.000000 fastgenerateapi-0.0.8/fastgenerateapi/schemas_factory/get_relation_schema_factory.py
--rw-rw-rw-   0        0        0     3187 2023-06-16 06:21:06.000000 fastgenerateapi-0.0.8/fastgenerateapi/schemas_factory/get_tree_schema_factory.py
--rw-rw-rw-   0        0        0     1647 2023-06-16 00:43:56.000000 fastgenerateapi-0.0.8/fastgenerateapi/schemas_factory/response_factory.py
--rw-rw-rw-   0        0        0     2292 2023-06-16 01:54:38.000000 fastgenerateapi-0.0.8/fastgenerateapi/schemas_factory/update_schema_factory.py
-drwxrwxrwx   0        0        0        0 2023-06-21 03:21:11.019039 fastgenerateapi-0.0.8/fastgenerateapi/settings/
--rw-rw-rw-   0        0        0        6 2023-06-15 11:43:17.000000 fastgenerateapi-0.0.8/fastgenerateapi/settings/__init__.py
--rw-rw-rw-   0        0        0       97 2023-06-16 00:40:41.000000 fastgenerateapi-0.0.8/fastgenerateapi/settings/register_settings.py
--rw-rw-rw-   0        0        0     4064 2023-06-19 06:02:37.000000 fastgenerateapi-0.0.8/fastgenerateapi/settings/settings.py
-drwxrwxrwx   0        0        0        0 2023-06-21 03:21:11.019039 fastgenerateapi-0.0.8/fastgenerateapi/utils/
--rw-rw-rw-   0        0        0        0 2023-06-15 11:43:17.000000 fastgenerateapi-0.0.8/fastgenerateapi/utils/__init__.py
--rw-rw-rw-   0        0        0      121 2023-06-15 11:43:17.000000 fastgenerateapi-0.0.8/fastgenerateapi/utils/exception.py
--rw-rw-rw-   0        0        0      670 2023-06-15 11:43:17.000000 fastgenerateapi-0.0.8/fastgenerateapi/utils/parse_str.py
-drwxrwxrwx   0        0        0        0 2023-06-21 03:21:10.955899 fastgenerateapi-0.0.8/fastgenerateapi.egg-info/
--rw-rw-rw-   0        0        0     4383 2023-06-21 03:21:10.000000 fastgenerateapi-0.0.8/fastgenerateapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2652 2023-06-21 03:21:10.000000 fastgenerateapi-0.0.8/fastgenerateapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 03:21:10.000000 fastgenerateapi-0.0.8/fastgenerateapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-21 03:21:10.000000 fastgenerateapi-0.0.8/fastgenerateapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-21 03:21:11.019039 fastgenerateapi-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     3832 2023-06-15 11:33:14.000000 fastgenerateapi-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:45:55.635428 fastgenerateapi-0.0.9/
+-rw-rw-rw-   0        0        0    35821 2023-06-15 11:33:13.000000 fastgenerateapi-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     4383 2023-06-21 03:45:55.635428 fastgenerateapi-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3741 2023-06-21 03:19:46.000000 fastgenerateapi-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-21 03:45:55.562837 fastgenerateapi-0.0.9/fastgenerateapi/
+-rw-rw-rw-   0        0        0     1022 2023-06-19 06:02:37.000000 fastgenerateapi-0.0.9/fastgenerateapi/__init__.py
+-rw-rw-rw-   0        0        0      496 2023-06-21 03:45:30.000000 fastgenerateapi-0.0.9/fastgenerateapi/__version__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:45:55.588564 fastgenerateapi-0.0.9/fastgenerateapi/api_view/
+-rw-rw-rw-   0        0        0       14 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.9/fastgenerateapi/api_view/__init__.py
+-rw-rw-rw-   0        0        0     1160 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.9/fastgenerateapi/api_view/api_view.py
+-rw-rw-rw-   0        0        0     9518 2023-06-21 01:20:11.000000 fastgenerateapi-0.0.9/fastgenerateapi/api_view/base_view.py
+-rw-rw-rw-   0        0        0     4177 2023-06-16 00:58:02.000000 fastgenerateapi-0.0.9/fastgenerateapi/api_view/create_view.py
+-rw-rw-rw-   0        0        0     3628 2023-06-19 06:02:37.000000 fastgenerateapi-0.0.9/fastgenerateapi/api_view/delete_tree_view.py
+-rw-rw-rw-   0        0        0     3035 2023-06-19 06:02:37.000000 fastgenerateapi-0.0.9/fastgenerateapi/api_view/delete_view.py
+-rw-rw-rw-   0        0        0     7469 2023-06-19 06:02:37.000000 fastgenerateapi-0.0.9/fastgenerateapi/api_view/get_all_view.py
+-rw-rw-rw-   0        0        0     3077 2023-06-19 06:02:37.000000 fastgenerateapi-0.0.9/fastgenerateapi/api_view/get_one_view.py
+-rw-rw-rw-   0        0        0     9795 2023-06-19 06:02:37.000000 fastgenerateapi-0.0.9/fastgenerateapi/api_view/get_relation_view.py
+-rw-rw-rw-   0        0        0     7275 2023-06-19 06:02:37.000000 fastgenerateapi-0.0.9/fastgenerateapi/api_view/get_tree_view.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:45:55.604184 fastgenerateapi-0.0.9/fastgenerateapi/api_view/mixin/
+-rw-rw-rw-   0        0        0        0 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.9/fastgenerateapi/api_view/mixin/__init__.py
+-rw-rw-rw-   0        0        0     4453 2023-06-19 06:02:37.000000 fastgenerateapi-0.0.9/fastgenerateapi/api_view/mixin/base_mixin.py
+-rw-rw-rw-   0        0        0     3826 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.9/fastgenerateapi/api_view/mixin/dbmodel_mixin.py
+-rw-rw-rw-   0        0        0      266 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.9/fastgenerateapi/api_view/mixin/get_mixin.py
+-rw-rw-rw-   0        0        0     2290 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.9/fastgenerateapi/api_view/mixin/response_mixin.py
+-rw-rw-rw-   0        0        0      317 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.9/fastgenerateapi/api_view/mixin/save_mixin.py
+-rw-rw-rw-   0        0        0    13529 2023-06-21 01:11:03.000000 fastgenerateapi-0.0.9/fastgenerateapi/api_view/mixin/tool_mixin.py
+-rw-rw-rw-   0        0        0     6899 2023-06-21 01:11:03.000000 fastgenerateapi-0.0.9/fastgenerateapi/api_view/sql_get_view.py
+-rw-rw-rw-   0        0        0     3070 2023-06-16 01:29:40.000000 fastgenerateapi-0.0.9/fastgenerateapi/api_view/switch_view.py
+-rw-rw-rw-   0        0        0     3553 2023-06-19 06:02:37.000000 fastgenerateapi-0.0.9/fastgenerateapi/api_view/update_relation_view.py
+-rw-rw-rw-   0        0        0     4006 2023-06-16 03:02:52.000000 fastgenerateapi-0.0.9/fastgenerateapi/api_view/update_view.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:45:55.604184 fastgenerateapi-0.0.9/fastgenerateapi/controller/
+-rw-rw-rw-   0        0        0      316 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.9/fastgenerateapi/controller/__init__.py
+-rw-rw-rw-   0        0        0     3391 2023-06-16 00:44:07.000000 fastgenerateapi-0.0.9/fastgenerateapi/controller/filter_controller.py
+-rw-rw-rw-   0        0        0     3341 2023-06-21 01:20:11.000000 fastgenerateapi-0.0.9/fastgenerateapi/controller/router_controller.py
+-rw-rw-rw-   0        0        0     2298 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.9/fastgenerateapi/controller/rpc_controller.py
+-rw-rw-rw-   0        0        0      873 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.9/fastgenerateapi/controller/search_controller.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:45:55.604184 fastgenerateapi-0.0.9/fastgenerateapi/data_type/
+-rw-rw-rw-   0        0        0        0 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.9/fastgenerateapi/data_type/__init__.py
+-rw-rw-rw-   0        0        0      727 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.9/fastgenerateapi/data_type/data_type.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:45:55.604184 fastgenerateapi-0.0.9/fastgenerateapi/deps/
+-rw-rw-rw-   0        0        0      160 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.9/fastgenerateapi/deps/__init__.py
+-rw-rw-rw-   0        0        0      813 2023-06-16 02:41:05.000000 fastgenerateapi-0.0.9/fastgenerateapi/deps/filter_params_deps.py
+-rw-rw-rw-   0        0        0     3171 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.9/fastgenerateapi/deps/paginator_deps.py
+-rw-rw-rw-   0        0        0     1264 2023-06-19 06:02:37.000000 fastgenerateapi-0.0.9/fastgenerateapi/deps/tree_params_deps.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:45:55.619806 fastgenerateapi-0.0.9/fastgenerateapi/example/
+-rw-rw-rw-   0        0        0        0 2023-06-15 11:43:17.000000 fastgenerateapi-0.0.9/fastgenerateapi/example/__init__.py
+-rw-rw-rw-   0        0        0     1611 2023-06-16 05:36:12.000000 fastgenerateapi-0.0.9/fastgenerateapi/example/models.py
+-rw-rw-rw-   0        0        0      195 2023-06-15 11:43:17.000000 fastgenerateapi-0.0.9/fastgenerateapi/example/routers.py
+-rw-rw-rw-   0        0        0      400 2023-06-16 05:42:12.000000 fastgenerateapi-0.0.9/fastgenerateapi/example/views.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:45:55.619806 fastgenerateapi-0.0.9/fastgenerateapi/pydantic_utils/
+-rw-rw-rw-   0        0        0        0 2023-06-15 11:43:17.000000 fastgenerateapi-0.0.9/fastgenerateapi/pydantic_utils/__init__.py
+-rw-rw-rw-   0        0        0      694 2023-06-16 00:57:41.000000 fastgenerateapi-0.0.9/fastgenerateapi/pydantic_utils/base_model.py
+-rw-rw-rw-   0        0        0     2814 2023-06-15 11:43:17.000000 fastgenerateapi-0.0.9/fastgenerateapi/pydantic_utils/json_encoders.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:45:55.635428 fastgenerateapi-0.0.9/fastgenerateapi/schemas_factory/
+-rw-rw-rw-   0        0        0      472 2023-06-15 11:43:17.000000 fastgenerateapi-0.0.9/fastgenerateapi/schemas_factory/__init__.py
+-rw-rw-rw-   0        0        0     4305 2023-06-16 00:44:35.000000 fastgenerateapi-0.0.9/fastgenerateapi/schemas_factory/common_function.py
+-rw-rw-rw-   0        0        0     2292 2023-06-16 01:54:38.000000 fastgenerateapi-0.0.9/fastgenerateapi/schemas_factory/create_schema_factory.py
+-rw-rw-rw-   0        0        0     1284 2023-06-16 02:48:31.000000 fastgenerateapi-0.0.9/fastgenerateapi/schemas_factory/filter_schema_factory.py
+-rw-rw-rw-   0        0        0     3570 2023-06-21 03:45:30.000000 fastgenerateapi-0.0.9/fastgenerateapi/schemas_factory/get_all_schema_factory.py
+-rw-rw-rw-   0        0        0     2194 2023-06-16 06:01:18.000000 fastgenerateapi-0.0.9/fastgenerateapi/schemas_factory/get_one_schema_factory.py
+-rw-rw-rw-   0        0        0     2391 2023-06-19 06:02:37.000000 fastgenerateapi-0.0.9/fastgenerateapi/schemas_factory/get_relation_schema_factory.py
+-rw-rw-rw-   0        0        0     3187 2023-06-16 06:21:06.000000 fastgenerateapi-0.0.9/fastgenerateapi/schemas_factory/get_tree_schema_factory.py
+-rw-rw-rw-   0        0        0     1647 2023-06-16 00:43:56.000000 fastgenerateapi-0.0.9/fastgenerateapi/schemas_factory/response_factory.py
+-rw-rw-rw-   0        0        0     2292 2023-06-16 01:54:38.000000 fastgenerateapi-0.0.9/fastgenerateapi/schemas_factory/update_schema_factory.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:45:55.635428 fastgenerateapi-0.0.9/fastgenerateapi/settings/
+-rw-rw-rw-   0        0        0        6 2023-06-15 11:43:17.000000 fastgenerateapi-0.0.9/fastgenerateapi/settings/__init__.py
+-rw-rw-rw-   0        0        0       97 2023-06-16 00:40:41.000000 fastgenerateapi-0.0.9/fastgenerateapi/settings/register_settings.py
+-rw-rw-rw-   0        0        0     4064 2023-06-19 06:02:37.000000 fastgenerateapi-0.0.9/fastgenerateapi/settings/settings.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:45:55.635428 fastgenerateapi-0.0.9/fastgenerateapi/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-15 11:43:17.000000 fastgenerateapi-0.0.9/fastgenerateapi/utils/__init__.py
+-rw-rw-rw-   0        0        0      121 2023-06-15 11:43:17.000000 fastgenerateapi-0.0.9/fastgenerateapi/utils/exception.py
+-rw-rw-rw-   0        0        0      670 2023-06-15 11:43:17.000000 fastgenerateapi-0.0.9/fastgenerateapi/utils/parse_str.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:45:55.572939 fastgenerateapi-0.0.9/fastgenerateapi.egg-info/
+-rw-rw-rw-   0        0        0     4383 2023-06-21 03:45:55.000000 fastgenerateapi-0.0.9/fastgenerateapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2652 2023-06-21 03:45:55.000000 fastgenerateapi-0.0.9/fastgenerateapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 03:45:55.000000 fastgenerateapi-0.0.9/fastgenerateapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-21 03:45:55.000000 fastgenerateapi-0.0.9/fastgenerateapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 03:45:55.635428 fastgenerateapi-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     3832 2023-06-15 11:33:14.000000 fastgenerateapi-0.0.9/setup.py
```

### Comparing `fastgenerateapi-0.0.8/LICENSE` & `fastgenerateapi-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.8/PKG-INFO` & `fastgenerateapi-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastgenerateapi
-Version: 0.0.8
+Version: 0.0.9
 Summary: FastAPIView Class View
 Author: ShiLiang
 Author-email: 2509144896@qq.com
 License: GPL-3.0-or-later
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fastgenerateapi-0.0.8/README.md` & `fastgenerateapi-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.8/fastgenerateapi/__init__.py` & `fastgenerateapi-0.0.9/fastgenerateapi/__init__.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.8/fastgenerateapi/api_view/api_view.py` & `fastgenerateapi-0.0.9/fastgenerateapi/api_view/api_view.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.8/fastgenerateapi/api_view/base_view.py` & `fastgenerateapi-0.0.9/fastgenerateapi/api_view/base_view.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.8/fastgenerateapi/api_view/create_view.py` & `fastgenerateapi-0.0.9/fastgenerateapi/api_view/create_view.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.8/fastgenerateapi/api_view/delete_tree_view.py` & `fastgenerateapi-0.0.9/fastgenerateapi/api_view/delete_tree_view.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.8/fastgenerateapi/api_view/delete_view.py` & `fastgenerateapi-0.0.9/fastgenerateapi/api_view/delete_view.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.8/fastgenerateapi/api_view/get_all_view.py` & `fastgenerateapi-0.0.9/fastgenerateapi/api_view/get_all_view.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.8/fastgenerateapi/api_view/get_one_view.py` & `fastgenerateapi-0.0.9/fastgenerateapi/api_view/get_one_view.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.8/fastgenerateapi/api_view/get_relation_view.py` & `fastgenerateapi-0.0.9/fastgenerateapi/api_view/get_relation_view.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.8/fastgenerateapi/api_view/get_tree_view.py` & `fastgenerateapi-0.0.9/fastgenerateapi/api_view/get_tree_view.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.8/fastgenerateapi/api_view/mixin/base_mixin.py` & `fastgenerateapi-0.0.9/fastgenerateapi/api_view/mixin/base_mixin.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.8/fastgenerateapi/api_view/mixin/dbmodel_mixin.py` & `fastgenerateapi-0.0.9/fastgenerateapi/api_view/mixin/dbmodel_mixin.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.8/fastgenerateapi/api_view/mixin/response_mixin.py` & `fastgenerateapi-0.0.9/fastgenerateapi/api_view/mixin/response_mixin.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.8/fastgenerateapi/api_view/mixin/tool_mixin.py` & `fastgenerateapi-0.0.9/fastgenerateapi/api_view/mixin/tool_mixin.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.8/fastgenerateapi/api_view/sql_get_view.py` & `fastgenerateapi-0.0.9/fastgenerateapi/api_view/sql_get_view.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.8/fastgenerateapi/api_view/switch_view.py` & `fastgenerateapi-0.0.9/fastgenerateapi/api_view/switch_view.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.8/fastgenerateapi/api_view/update_relation_view.py` & `fastgenerateapi-0.0.9/fastgenerateapi/api_view/update_relation_view.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.8/fastgenerateapi/api_view/update_view.py` & `fastgenerateapi-0.0.9/fastgenerateapi/api_view/update_view.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.8/fastgenerateapi/controller/filter_controller.py` & `fastgenerateapi-0.0.9/fastgenerateapi/controller/filter_controller.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.8/fastgenerateapi/controller/router_controller.py` & `fastgenerateapi-0.0.9/fastgenerateapi/controller/router_controller.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.8/fastgenerateapi/controller/rpc_controller.py` & `fastgenerateapi-0.0.9/fastgenerateapi/controller/rpc_controller.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.8/fastgenerateapi/controller/search_controller.py` & `fastgenerateapi-0.0.9/fastgenerateapi/controller/search_controller.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.8/fastgenerateapi/data_type/data_type.py` & `fastgenerateapi-0.0.9/fastgenerateapi/data_type/data_type.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.8/fastgenerateapi/deps/filter_params_deps.py` & `fastgenerateapi-0.0.9/fastgenerateapi/deps/filter_params_deps.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.8/fastgenerateapi/deps/paginator_deps.py` & `fastgenerateapi-0.0.9/fastgenerateapi/deps/paginator_deps.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.8/fastgenerateapi/deps/tree_params_deps.py` & `fastgenerateapi-0.0.9/fastgenerateapi/deps/tree_params_deps.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.8/fastgenerateapi/example/models.py` & `fastgenerateapi-0.0.9/fastgenerateapi/example/models.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.8/fastgenerateapi/pydantic_utils/base_model.py` & `fastgenerateapi-0.0.9/fastgenerateapi/pydantic_utils/base_model.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.8/fastgenerateapi/pydantic_utils/json_encoders.py` & `fastgenerateapi-0.0.9/fastgenerateapi/pydantic_utils/json_encoders.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.8/fastgenerateapi/schemas_factory/common_function.py` & `fastgenerateapi-0.0.9/fastgenerateapi/schemas_factory/common_function.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.8/fastgenerateapi/schemas_factory/create_schema_factory.py` & `fastgenerateapi-0.0.9/fastgenerateapi/schemas_factory/create_schema_factory.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.8/fastgenerateapi/schemas_factory/filter_schema_factory.py` & `fastgenerateapi-0.0.9/fastgenerateapi/schemas_factory/filter_schema_factory.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.8/fastgenerateapi/schemas_factory/get_all_schema_factory.py` & `fastgenerateapi-0.0.9/fastgenerateapi/schemas_factory/get_all_schema_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import time
 from typing import Type, Optional, Union, List
 
 from pydantic.fields import FieldInfo
 from tortoise import Model
 from pydantic import create_model
 
 from fastgenerateapi.data_type.data_type import T
@@ -48,18 +49,24 @@
     name = model_class.__name__ + "GetAllSchema"
     schema: Type[T] = create_model(
         __model_name=name, **{field: all_fields_info[field] for field in all_fields}, __config__=Config)
     return schema
 
 
 def get_list_schema_factory(schema_cls: Type[T]) -> Type[T]:
-    fields = {
-        settings.app_settings.LIST_RESPONSE_FIELD: (Optional[List[schema_cls]], FieldInfo(default=[], description="数据返回")),
-    }
-    name = schema_cls.__name__ + "GetListSchema"
+    if schema_cls:
+        fields = {
+            settings.app_settings.LIST_RESPONSE_FIELD: (Optional[List[schema_cls]], FieldInfo(default=[], description="数据返回")),
+        }
+        name = schema_cls.__name__ + "GetListSchema"
+    else:
+        fields = {
+            settings.app_settings.LIST_RESPONSE_FIELD: (Optional[list], FieldInfo(default=[], description="数据返回")),
+        }
+        name = "GetListSchema" + str(time.time())
     schema: Type[T] = create_model(__model_name=name, **fields, __config__=Config)
     return schema
 
 
 def get_page_schema_factory(schema_cls: Type[T]) -> Type[T]:
     fields = {
         settings.app_settings.CURRENT_PAGE_FIELD: (Optional[int], FieldInfo(default=1, description="当前页")),
```

### Comparing `fastgenerateapi-0.0.8/fastgenerateapi/schemas_factory/get_one_schema_factory.py` & `fastgenerateapi-0.0.9/fastgenerateapi/schemas_factory/get_one_schema_factory.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.8/fastgenerateapi/schemas_factory/get_relation_schema_factory.py` & `fastgenerateapi-0.0.9/fastgenerateapi/schemas_factory/get_relation_schema_factory.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.8/fastgenerateapi/schemas_factory/get_tree_schema_factory.py` & `fastgenerateapi-0.0.9/fastgenerateapi/schemas_factory/get_tree_schema_factory.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.8/fastgenerateapi/schemas_factory/response_factory.py` & `fastgenerateapi-0.0.9/fastgenerateapi/schemas_factory/response_factory.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.8/fastgenerateapi/schemas_factory/update_schema_factory.py` & `fastgenerateapi-0.0.9/fastgenerateapi/schemas_factory/update_schema_factory.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.8/fastgenerateapi/settings/settings.py` & `fastgenerateapi-0.0.9/fastgenerateapi/settings/settings.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.8/fastgenerateapi/utils/parse_str.py` & `fastgenerateapi-0.0.9/fastgenerateapi/utils/parse_str.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.8/fastgenerateapi.egg-info/PKG-INFO` & `fastgenerateapi-0.0.9/fastgenerateapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastgenerateapi
-Version: 0.0.8
+Version: 0.0.9
 Summary: FastAPIView Class View
 Author: ShiLiang
 Author-email: 2509144896@qq.com
 License: GPL-3.0-or-later
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fastgenerateapi-0.0.8/fastgenerateapi.egg-info/SOURCES.txt` & `fastgenerateapi-0.0.9/fastgenerateapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.8/setup.py` & `fastgenerateapi-0.0.9/setup.py`

 * *Files identical despite different names*

