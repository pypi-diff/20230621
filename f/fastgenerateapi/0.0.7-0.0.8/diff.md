# Comparing `tmp/fastgenerateapi-0.0.7.tar.gz` & `tmp/fastgenerateapi-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastgenerateapi-0.0.7.tar", last modified: Tue Jun 20 12:52:40 2023, max compression
+gzip compressed data, was "fastgenerateapi-0.0.8.tar", last modified: Wed Jun 21 03:21:11 2023, max compression
```

## Comparing `fastgenerateapi-0.0.7.tar` & `fastgenerateapi-0.0.8.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 12:52:40.868601 fastgenerateapi-0.0.7/
--rw-rw-rw-   0        0        0    35821 2023-06-18 00:11:53.000000 fastgenerateapi-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     4383 2023-06-20 12:52:40.867604 fastgenerateapi-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     3741 2023-06-20 12:51:34.000000 fastgenerateapi-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 12:52:40.841813 fastgenerateapi-0.0.7/fastgenerateapi/
--rw-rw-rw-   0        0        0     1022 2023-06-18 06:05:08.000000 fastgenerateapi-0.0.7/fastgenerateapi/__init__.py
--rw-rw-rw-   0        0        0      496 2023-06-20 12:49:43.000000 fastgenerateapi-0.0.7/fastgenerateapi/__version__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 12:52:40.848440 fastgenerateapi-0.0.7/fastgenerateapi/api_view/
--rw-rw-rw-   0        0        0       14 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.7/fastgenerateapi/api_view/__init__.py
--rw-rw-rw-   0        0        0     1160 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.7/fastgenerateapi/api_view/api_view.py
--rw-rw-rw-   0        0        0     9399 2023-06-20 12:36:30.000000 fastgenerateapi-0.0.7/fastgenerateapi/api_view/base_view.py
--rw-rw-rw-   0        0        0     4177 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.7/fastgenerateapi/api_view/create_view.py
--rw-rw-rw-   0        0        0     3628 2023-06-18 03:11:06.000000 fastgenerateapi-0.0.7/fastgenerateapi/api_view/delete_tree_view.py
--rw-rw-rw-   0        0        0     3035 2023-06-18 03:11:06.000000 fastgenerateapi-0.0.7/fastgenerateapi/api_view/delete_view.py
--rw-rw-rw-   0        0        0     7469 2023-06-18 06:05:08.000000 fastgenerateapi-0.0.7/fastgenerateapi/api_view/get_all_view.py
--rw-rw-rw-   0        0        0     3077 2023-06-18 01:49:07.000000 fastgenerateapi-0.0.7/fastgenerateapi/api_view/get_one_view.py
--rw-rw-rw-   0        0        0     9795 2023-06-18 06:05:08.000000 fastgenerateapi-0.0.7/fastgenerateapi/api_view/get_relation_view.py
--rw-rw-rw-   0        0        0     7275 2023-06-18 06:05:08.000000 fastgenerateapi-0.0.7/fastgenerateapi/api_view/get_tree_view.py
-drwxrwxrwx   0        0        0        0 2023-06-20 12:52:40.851431 fastgenerateapi-0.0.7/fastgenerateapi/api_view/mixin/
--rw-rw-rw-   0        0        0        0 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.7/fastgenerateapi/api_view/mixin/__init__.py
--rw-rw-rw-   0        0        0     4453 2023-06-18 04:59:15.000000 fastgenerateapi-0.0.7/fastgenerateapi/api_view/mixin/base_mixin.py
--rw-rw-rw-   0        0        0     3826 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.7/fastgenerateapi/api_view/mixin/dbmodel_mixin.py
--rw-rw-rw-   0        0        0      266 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.7/fastgenerateapi/api_view/mixin/get_mixin.py
--rw-rw-rw-   0        0        0     2290 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.7/fastgenerateapi/api_view/mixin/response_mixin.py
--rw-rw-rw-   0        0        0      317 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.7/fastgenerateapi/api_view/mixin/save_mixin.py
--rw-rw-rw-   0        0        0    13529 2023-06-20 12:11:25.000000 fastgenerateapi-0.0.7/fastgenerateapi/api_view/mixin/tool_mixin.py
--rw-rw-rw-   0        0        0     6899 2023-06-20 12:48:13.000000 fastgenerateapi-0.0.7/fastgenerateapi/api_view/sql_get_view.py
--rw-rw-rw-   0        0        0     3070 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.7/fastgenerateapi/api_view/switch_view.py
--rw-rw-rw-   0        0        0     3553 2023-06-18 04:41:09.000000 fastgenerateapi-0.0.7/fastgenerateapi/api_view/update_relation_view.py
--rw-rw-rw-   0        0        0     4006 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.7/fastgenerateapi/api_view/update_view.py
-drwxrwxrwx   0        0        0        0 2023-06-20 12:52:40.858578 fastgenerateapi-0.0.7/fastgenerateapi/controller/
--rw-rw-rw-   0        0        0      316 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.7/fastgenerateapi/controller/__init__.py
--rw-rw-rw-   0        0        0     3391 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.7/fastgenerateapi/controller/filter_controller.py
--rw-rw-rw-   0        0        0     3292 2023-06-20 12:22:23.000000 fastgenerateapi-0.0.7/fastgenerateapi/controller/router_controller.py
--rw-rw-rw-   0        0        0     2298 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.7/fastgenerateapi/controller/rpc_controller.py
--rw-rw-rw-   0        0        0      873 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.7/fastgenerateapi/controller/search_controller.py
-drwxrwxrwx   0        0        0        0 2023-06-20 12:52:40.859582 fastgenerateapi-0.0.7/fastgenerateapi/data_type/
--rw-rw-rw-   0        0        0        0 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.7/fastgenerateapi/data_type/__init__.py
--rw-rw-rw-   0        0        0      727 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.7/fastgenerateapi/data_type/data_type.py
-drwxrwxrwx   0        0        0        0 2023-06-20 12:52:40.860572 fastgenerateapi-0.0.7/fastgenerateapi/deps/
--rw-rw-rw-   0        0        0      160 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.7/fastgenerateapi/deps/__init__.py
--rw-rw-rw-   0        0        0      813 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.7/fastgenerateapi/deps/filter_params_deps.py
--rw-rw-rw-   0        0        0     3171 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.7/fastgenerateapi/deps/paginator_deps.py
--rw-rw-rw-   0        0        0     1264 2023-06-18 01:09:58.000000 fastgenerateapi-0.0.7/fastgenerateapi/deps/tree_params_deps.py
-drwxrwxrwx   0        0        0        0 2023-06-20 12:52:40.862617 fastgenerateapi-0.0.7/fastgenerateapi/example/
--rw-rw-rw-   0        0        0        0 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.7/fastgenerateapi/example/__init__.py
--rw-rw-rw-   0        0        0     1611 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.7/fastgenerateapi/example/models.py
--rw-rw-rw-   0        0        0      195 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.7/fastgenerateapi/example/routers.py
--rw-rw-rw-   0        0        0      400 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.7/fastgenerateapi/example/views.py
-drwxrwxrwx   0        0        0        0 2023-06-20 12:52:40.862617 fastgenerateapi-0.0.7/fastgenerateapi/pydantic_utils/
--rw-rw-rw-   0        0        0        0 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.7/fastgenerateapi/pydantic_utils/__init__.py
--rw-rw-rw-   0        0        0      694 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.7/fastgenerateapi/pydantic_utils/base_model.py
--rw-rw-rw-   0        0        0     2814 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.7/fastgenerateapi/pydantic_utils/json_encoders.py
-drwxrwxrwx   0        0        0        0 2023-06-20 12:52:40.865609 fastgenerateapi-0.0.7/fastgenerateapi/schemas_factory/
--rw-rw-rw-   0        0        0      472 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.7/fastgenerateapi/schemas_factory/__init__.py
--rw-rw-rw-   0        0        0     4305 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.7/fastgenerateapi/schemas_factory/common_function.py
--rw-rw-rw-   0        0        0     2292 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.7/fastgenerateapi/schemas_factory/create_schema_factory.py
--rw-rw-rw-   0        0        0     1284 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.7/fastgenerateapi/schemas_factory/filter_schema_factory.py
--rw-rw-rw-   0        0        0     3303 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.7/fastgenerateapi/schemas_factory/get_all_schema_factory.py
--rw-rw-rw-   0        0        0     2194 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.7/fastgenerateapi/schemas_factory/get_one_schema_factory.py
--rw-rw-rw-   0        0        0     2391 2023-06-18 06:05:08.000000 fastgenerateapi-0.0.7/fastgenerateapi/schemas_factory/get_relation_schema_factory.py
--rw-rw-rw-   0        0        0     3187 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.7/fastgenerateapi/schemas_factory/get_tree_schema_factory.py
--rw-rw-rw-   0        0        0     1647 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.7/fastgenerateapi/schemas_factory/response_factory.py
--rw-rw-rw-   0        0        0     2292 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.7/fastgenerateapi/schemas_factory/update_schema_factory.py
-drwxrwxrwx   0        0        0        0 2023-06-20 12:52:40.866606 fastgenerateapi-0.0.7/fastgenerateapi/settings/
--rw-rw-rw-   0        0        0        6 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.7/fastgenerateapi/settings/__init__.py
--rw-rw-rw-   0        0        0       97 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.7/fastgenerateapi/settings/register_settings.py
--rw-rw-rw-   0        0        0     4064 2023-06-18 06:05:08.000000 fastgenerateapi-0.0.7/fastgenerateapi/settings/settings.py
-drwxrwxrwx   0        0        0        0 2023-06-20 12:52:40.867604 fastgenerateapi-0.0.7/fastgenerateapi/utils/
--rw-rw-rw-   0        0        0        0 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.7/fastgenerateapi/utils/__init__.py
--rw-rw-rw-   0        0        0      121 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.7/fastgenerateapi/utils/exception.py
--rw-rw-rw-   0        0        0      670 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.7/fastgenerateapi/utils/parse_str.py
-drwxrwxrwx   0        0        0        0 2023-06-20 12:52:40.842800 fastgenerateapi-0.0.7/fastgenerateapi.egg-info/
--rw-rw-rw-   0        0        0     4383 2023-06-20 12:52:40.000000 fastgenerateapi-0.0.7/fastgenerateapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2652 2023-06-20 12:52:40.000000 fastgenerateapi-0.0.7/fastgenerateapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 12:52:40.000000 fastgenerateapi-0.0.7/fastgenerateapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-20 12:52:40.000000 fastgenerateapi-0.0.7/fastgenerateapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-20 12:52:40.868601 fastgenerateapi-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     3832 2023-06-18 06:18:28.000000 fastgenerateapi-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:21:11.019039 fastgenerateapi-0.0.8/
+-rw-rw-rw-   0        0        0    35821 2023-06-15 11:33:13.000000 fastgenerateapi-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     4383 2023-06-21 03:21:11.019039 fastgenerateapi-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3741 2023-06-21 03:19:46.000000 fastgenerateapi-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-21 03:21:10.940278 fastgenerateapi-0.0.8/fastgenerateapi/
+-rw-rw-rw-   0        0        0     1022 2023-06-19 06:02:37.000000 fastgenerateapi-0.0.8/fastgenerateapi/__init__.py
+-rw-rw-rw-   0        0        0      496 2023-06-21 01:21:22.000000 fastgenerateapi-0.0.8/fastgenerateapi/__version__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:21:10.971546 fastgenerateapi-0.0.8/fastgenerateapi/api_view/
+-rw-rw-rw-   0        0        0       14 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.8/fastgenerateapi/api_view/__init__.py
+-rw-rw-rw-   0        0        0     1160 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.8/fastgenerateapi/api_view/api_view.py
+-rw-rw-rw-   0        0        0     9518 2023-06-21 01:20:11.000000 fastgenerateapi-0.0.8/fastgenerateapi/api_view/base_view.py
+-rw-rw-rw-   0        0        0     4177 2023-06-16 00:58:02.000000 fastgenerateapi-0.0.8/fastgenerateapi/api_view/create_view.py
+-rw-rw-rw-   0        0        0     3628 2023-06-19 06:02:37.000000 fastgenerateapi-0.0.8/fastgenerateapi/api_view/delete_tree_view.py
+-rw-rw-rw-   0        0        0     3035 2023-06-19 06:02:37.000000 fastgenerateapi-0.0.8/fastgenerateapi/api_view/delete_view.py
+-rw-rw-rw-   0        0        0     7469 2023-06-19 06:02:37.000000 fastgenerateapi-0.0.8/fastgenerateapi/api_view/get_all_view.py
+-rw-rw-rw-   0        0        0     3077 2023-06-19 06:02:37.000000 fastgenerateapi-0.0.8/fastgenerateapi/api_view/get_one_view.py
+-rw-rw-rw-   0        0        0     9795 2023-06-19 06:02:37.000000 fastgenerateapi-0.0.8/fastgenerateapi/api_view/get_relation_view.py
+-rw-rw-rw-   0        0        0     7275 2023-06-19 06:02:37.000000 fastgenerateapi-0.0.8/fastgenerateapi/api_view/get_tree_view.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:21:10.987793 fastgenerateapi-0.0.8/fastgenerateapi/api_view/mixin/
+-rw-rw-rw-   0        0        0        0 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.8/fastgenerateapi/api_view/mixin/__init__.py
+-rw-rw-rw-   0        0        0     4453 2023-06-19 06:02:37.000000 fastgenerateapi-0.0.8/fastgenerateapi/api_view/mixin/base_mixin.py
+-rw-rw-rw-   0        0        0     3826 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.8/fastgenerateapi/api_view/mixin/dbmodel_mixin.py
+-rw-rw-rw-   0        0        0      266 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.8/fastgenerateapi/api_view/mixin/get_mixin.py
+-rw-rw-rw-   0        0        0     2290 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.8/fastgenerateapi/api_view/mixin/response_mixin.py
+-rw-rw-rw-   0        0        0      317 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.8/fastgenerateapi/api_view/mixin/save_mixin.py
+-rw-rw-rw-   0        0        0    13529 2023-06-21 01:11:03.000000 fastgenerateapi-0.0.8/fastgenerateapi/api_view/mixin/tool_mixin.py
+-rw-rw-rw-   0        0        0     6899 2023-06-21 01:11:03.000000 fastgenerateapi-0.0.8/fastgenerateapi/api_view/sql_get_view.py
+-rw-rw-rw-   0        0        0     3070 2023-06-16 01:29:40.000000 fastgenerateapi-0.0.8/fastgenerateapi/api_view/switch_view.py
+-rw-rw-rw-   0        0        0     3553 2023-06-19 06:02:37.000000 fastgenerateapi-0.0.8/fastgenerateapi/api_view/update_relation_view.py
+-rw-rw-rw-   0        0        0     4006 2023-06-16 03:02:52.000000 fastgenerateapi-0.0.8/fastgenerateapi/api_view/update_view.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:21:10.987793 fastgenerateapi-0.0.8/fastgenerateapi/controller/
+-rw-rw-rw-   0        0        0      316 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.8/fastgenerateapi/controller/__init__.py
+-rw-rw-rw-   0        0        0     3391 2023-06-16 00:44:07.000000 fastgenerateapi-0.0.8/fastgenerateapi/controller/filter_controller.py
+-rw-rw-rw-   0        0        0     3341 2023-06-21 01:20:11.000000 fastgenerateapi-0.0.8/fastgenerateapi/controller/router_controller.py
+-rw-rw-rw-   0        0        0     2298 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.8/fastgenerateapi/controller/rpc_controller.py
+-rw-rw-rw-   0        0        0      873 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.8/fastgenerateapi/controller/search_controller.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:21:10.987793 fastgenerateapi-0.0.8/fastgenerateapi/data_type/
+-rw-rw-rw-   0        0        0        0 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.8/fastgenerateapi/data_type/__init__.py
+-rw-rw-rw-   0        0        0      727 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.8/fastgenerateapi/data_type/data_type.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:21:10.987793 fastgenerateapi-0.0.8/fastgenerateapi/deps/
+-rw-rw-rw-   0        0        0      160 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.8/fastgenerateapi/deps/__init__.py
+-rw-rw-rw-   0        0        0      813 2023-06-16 02:41:05.000000 fastgenerateapi-0.0.8/fastgenerateapi/deps/filter_params_deps.py
+-rw-rw-rw-   0        0        0     3171 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.8/fastgenerateapi/deps/paginator_deps.py
+-rw-rw-rw-   0        0        0     1264 2023-06-19 06:02:37.000000 fastgenerateapi-0.0.8/fastgenerateapi/deps/tree_params_deps.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:21:11.003419 fastgenerateapi-0.0.8/fastgenerateapi/example/
+-rw-rw-rw-   0        0        0        0 2023-06-15 11:43:17.000000 fastgenerateapi-0.0.8/fastgenerateapi/example/__init__.py
+-rw-rw-rw-   0        0        0     1611 2023-06-16 05:36:12.000000 fastgenerateapi-0.0.8/fastgenerateapi/example/models.py
+-rw-rw-rw-   0        0        0      195 2023-06-15 11:43:17.000000 fastgenerateapi-0.0.8/fastgenerateapi/example/routers.py
+-rw-rw-rw-   0        0        0      400 2023-06-16 05:42:12.000000 fastgenerateapi-0.0.8/fastgenerateapi/example/views.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:21:11.003419 fastgenerateapi-0.0.8/fastgenerateapi/pydantic_utils/
+-rw-rw-rw-   0        0        0        0 2023-06-15 11:43:17.000000 fastgenerateapi-0.0.8/fastgenerateapi/pydantic_utils/__init__.py
+-rw-rw-rw-   0        0        0      694 2023-06-16 00:57:41.000000 fastgenerateapi-0.0.8/fastgenerateapi/pydantic_utils/base_model.py
+-rw-rw-rw-   0        0        0     2814 2023-06-15 11:43:17.000000 fastgenerateapi-0.0.8/fastgenerateapi/pydantic_utils/json_encoders.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:21:11.019039 fastgenerateapi-0.0.8/fastgenerateapi/schemas_factory/
+-rw-rw-rw-   0        0        0      472 2023-06-15 11:43:17.000000 fastgenerateapi-0.0.8/fastgenerateapi/schemas_factory/__init__.py
+-rw-rw-rw-   0        0        0     4305 2023-06-16 00:44:35.000000 fastgenerateapi-0.0.8/fastgenerateapi/schemas_factory/common_function.py
+-rw-rw-rw-   0        0        0     2292 2023-06-16 01:54:38.000000 fastgenerateapi-0.0.8/fastgenerateapi/schemas_factory/create_schema_factory.py
+-rw-rw-rw-   0        0        0     1284 2023-06-16 02:48:31.000000 fastgenerateapi-0.0.8/fastgenerateapi/schemas_factory/filter_schema_factory.py
+-rw-rw-rw-   0        0        0     3303 2023-06-16 06:01:18.000000 fastgenerateapi-0.0.8/fastgenerateapi/schemas_factory/get_all_schema_factory.py
+-rw-rw-rw-   0        0        0     2194 2023-06-16 06:01:18.000000 fastgenerateapi-0.0.8/fastgenerateapi/schemas_factory/get_one_schema_factory.py
+-rw-rw-rw-   0        0        0     2391 2023-06-19 06:02:37.000000 fastgenerateapi-0.0.8/fastgenerateapi/schemas_factory/get_relation_schema_factory.py
+-rw-rw-rw-   0        0        0     3187 2023-06-16 06:21:06.000000 fastgenerateapi-0.0.8/fastgenerateapi/schemas_factory/get_tree_schema_factory.py
+-rw-rw-rw-   0        0        0     1647 2023-06-16 00:43:56.000000 fastgenerateapi-0.0.8/fastgenerateapi/schemas_factory/response_factory.py
+-rw-rw-rw-   0        0        0     2292 2023-06-16 01:54:38.000000 fastgenerateapi-0.0.8/fastgenerateapi/schemas_factory/update_schema_factory.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:21:11.019039 fastgenerateapi-0.0.8/fastgenerateapi/settings/
+-rw-rw-rw-   0        0        0        6 2023-06-15 11:43:17.000000 fastgenerateapi-0.0.8/fastgenerateapi/settings/__init__.py
+-rw-rw-rw-   0        0        0       97 2023-06-16 00:40:41.000000 fastgenerateapi-0.0.8/fastgenerateapi/settings/register_settings.py
+-rw-rw-rw-   0        0        0     4064 2023-06-19 06:02:37.000000 fastgenerateapi-0.0.8/fastgenerateapi/settings/settings.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:21:11.019039 fastgenerateapi-0.0.8/fastgenerateapi/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-15 11:43:17.000000 fastgenerateapi-0.0.8/fastgenerateapi/utils/__init__.py
+-rw-rw-rw-   0        0        0      121 2023-06-15 11:43:17.000000 fastgenerateapi-0.0.8/fastgenerateapi/utils/exception.py
+-rw-rw-rw-   0        0        0      670 2023-06-15 11:43:17.000000 fastgenerateapi-0.0.8/fastgenerateapi/utils/parse_str.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:21:10.955899 fastgenerateapi-0.0.8/fastgenerateapi.egg-info/
+-rw-rw-rw-   0        0        0     4383 2023-06-21 03:21:10.000000 fastgenerateapi-0.0.8/fastgenerateapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2652 2023-06-21 03:21:10.000000 fastgenerateapi-0.0.8/fastgenerateapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 03:21:10.000000 fastgenerateapi-0.0.8/fastgenerateapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-21 03:21:10.000000 fastgenerateapi-0.0.8/fastgenerateapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 03:21:11.019039 fastgenerateapi-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     3832 2023-06-15 11:33:14.000000 fastgenerateapi-0.0.8/setup.py
```

### Comparing `fastgenerateapi-0.0.7/LICENSE` & `fastgenerateapi-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.7/PKG-INFO` & `fastgenerateapi-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastgenerateapi
-Version: 0.0.7
+Version: 0.0.8
 Summary: FastAPIView Class View
 Author: ShiLiang
 Author-email: 2509144896@qq.com
 License: GPL-3.0-or-later
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fastgenerateapi-0.0.7/README.md` & `fastgenerateapi-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.7/fastgenerateapi/__init__.py` & `fastgenerateapi-0.0.8/fastgenerateapi/__init__.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.7/fastgenerateapi/api_view/api_view.py` & `fastgenerateapi-0.0.8/fastgenerateapi/api_view/api_view.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.7/fastgenerateapi/api_view/base_view.py` & `fastgenerateapi-0.0.8/fastgenerateapi/api_view/base_view.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import uuid
 from copy import copy
 from typing import Optional, Type, List, Union, Sequence, Dict
 from urllib.parse import parse_qs
 
 from fastapi import params
+from fastgenerateapi.schemas_factory.get_all_schema_factory import get_list_schema_factory
+
 from fastgenerateapi.controller.router_controller import BaseRouter
 from pydantic import create_model
 from starlette.requests import Request
 from tortoise import Model
 from tortoise.expressions import Q
 
 from fastgenerateapi.api_view.mixin.base_mixin import BaseMixin
@@ -67,15 +69,15 @@
 
         self.router_summary = RouterController(self, self._get_cls_func())
         for router in self.router_summary.router_data:
             self._add_api_route(
                 f"/{router.prefix}",
                 getattr(self, router.func_name),
                 methods=[router.method],
-                response_model=router.response_model,
+                response_model=get_list_schema_factory(router.response_model),
                 summary=router.summary,
                 dependencies=router.dependencies,
                 error_responses=[NOT_FOUND],
             )
 
         if self.model_class:
             for route_field in self._get_routes(is_controller_field=True):
```

### Comparing `fastgenerateapi-0.0.7/fastgenerateapi/api_view/create_view.py` & `fastgenerateapi-0.0.8/fastgenerateapi/api_view/create_view.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.7/fastgenerateapi/api_view/delete_tree_view.py` & `fastgenerateapi-0.0.8/fastgenerateapi/api_view/delete_tree_view.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.7/fastgenerateapi/api_view/delete_view.py` & `fastgenerateapi-0.0.8/fastgenerateapi/api_view/delete_view.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.7/fastgenerateapi/api_view/get_all_view.py` & `fastgenerateapi-0.0.8/fastgenerateapi/api_view/get_all_view.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.7/fastgenerateapi/api_view/get_one_view.py` & `fastgenerateapi-0.0.8/fastgenerateapi/api_view/get_one_view.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.7/fastgenerateapi/api_view/get_relation_view.py` & `fastgenerateapi-0.0.8/fastgenerateapi/api_view/get_relation_view.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.7/fastgenerateapi/api_view/get_tree_view.py` & `fastgenerateapi-0.0.8/fastgenerateapi/api_view/get_tree_view.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.7/fastgenerateapi/api_view/mixin/base_mixin.py` & `fastgenerateapi-0.0.8/fastgenerateapi/api_view/mixin/base_mixin.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.7/fastgenerateapi/api_view/mixin/dbmodel_mixin.py` & `fastgenerateapi-0.0.8/fastgenerateapi/api_view/mixin/dbmodel_mixin.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.7/fastgenerateapi/api_view/mixin/response_mixin.py` & `fastgenerateapi-0.0.8/fastgenerateapi/api_view/mixin/response_mixin.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.7/fastgenerateapi/api_view/mixin/tool_mixin.py` & `fastgenerateapi-0.0.8/fastgenerateapi/api_view/mixin/tool_mixin.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.7/fastgenerateapi/api_view/sql_get_view.py` & `fastgenerateapi-0.0.8/fastgenerateapi/api_view/sql_get_view.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.7/fastgenerateapi/api_view/switch_view.py` & `fastgenerateapi-0.0.8/fastgenerateapi/api_view/switch_view.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.7/fastgenerateapi/api_view/update_relation_view.py` & `fastgenerateapi-0.0.8/fastgenerateapi/api_view/update_relation_view.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.7/fastgenerateapi/api_view/update_view.py` & `fastgenerateapi-0.0.8/fastgenerateapi/api_view/update_view.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.7/fastgenerateapi/controller/filter_controller.py` & `fastgenerateapi-0.0.8/fastgenerateapi/controller/filter_controller.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.7/fastgenerateapi/controller/router_controller.py` & `fastgenerateapi-0.0.8/fastgenerateapi/controller/router_controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,17 +26,17 @@
             prefix += "/"
         self.prefix = prefix
 
         # if function in ["get_one", "get_all", "create", "update", "update_optional", "destroy", "switch"]:
         #     self.is_new = False
         # else:
         #     self.is_new = True
-        router_args = router_class.router_args.get(func_name, None) if router_class.router_args else {}
+        router_args = router_class.router_args.get(func_name, {}) if router_class.router_args else {}
         if router_args:
-            if isinstance(router_args, BaseModel):
+            if type(router_args).__name__ == 'ModelMetaclass' and issubclass(router_args, BaseModel):
                 router_args = {"response_model": router_args}
             if isinstance(router_args, list):
                 router_args = {"dependencies": router_args}
             if isinstance(router_args, str):
                 router_args = {"summary": router_args}
 
         self.dependencies = router_args.get("dependencies") if router_args and router_args.get("dependencies") else []
```

### Comparing `fastgenerateapi-0.0.7/fastgenerateapi/controller/rpc_controller.py` & `fastgenerateapi-0.0.8/fastgenerateapi/controller/rpc_controller.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.7/fastgenerateapi/controller/search_controller.py` & `fastgenerateapi-0.0.8/fastgenerateapi/controller/search_controller.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.7/fastgenerateapi/data_type/data_type.py` & `fastgenerateapi-0.0.8/fastgenerateapi/data_type/data_type.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.7/fastgenerateapi/deps/filter_params_deps.py` & `fastgenerateapi-0.0.8/fastgenerateapi/deps/filter_params_deps.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.7/fastgenerateapi/deps/paginator_deps.py` & `fastgenerateapi-0.0.8/fastgenerateapi/deps/paginator_deps.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.7/fastgenerateapi/deps/tree_params_deps.py` & `fastgenerateapi-0.0.8/fastgenerateapi/deps/tree_params_deps.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.7/fastgenerateapi/example/models.py` & `fastgenerateapi-0.0.8/fastgenerateapi/example/models.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.7/fastgenerateapi/pydantic_utils/base_model.py` & `fastgenerateapi-0.0.8/fastgenerateapi/pydantic_utils/base_model.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.7/fastgenerateapi/pydantic_utils/json_encoders.py` & `fastgenerateapi-0.0.8/fastgenerateapi/pydantic_utils/json_encoders.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.7/fastgenerateapi/schemas_factory/common_function.py` & `fastgenerateapi-0.0.8/fastgenerateapi/schemas_factory/common_function.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.7/fastgenerateapi/schemas_factory/create_schema_factory.py` & `fastgenerateapi-0.0.8/fastgenerateapi/schemas_factory/create_schema_factory.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.7/fastgenerateapi/schemas_factory/filter_schema_factory.py` & `fastgenerateapi-0.0.8/fastgenerateapi/schemas_factory/filter_schema_factory.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.7/fastgenerateapi/schemas_factory/get_all_schema_factory.py` & `fastgenerateapi-0.0.8/fastgenerateapi/schemas_factory/get_all_schema_factory.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.7/fastgenerateapi/schemas_factory/get_one_schema_factory.py` & `fastgenerateapi-0.0.8/fastgenerateapi/schemas_factory/get_one_schema_factory.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.7/fastgenerateapi/schemas_factory/get_relation_schema_factory.py` & `fastgenerateapi-0.0.8/fastgenerateapi/schemas_factory/get_relation_schema_factory.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.7/fastgenerateapi/schemas_factory/get_tree_schema_factory.py` & `fastgenerateapi-0.0.8/fastgenerateapi/schemas_factory/get_tree_schema_factory.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.7/fastgenerateapi/schemas_factory/response_factory.py` & `fastgenerateapi-0.0.8/fastgenerateapi/schemas_factory/response_factory.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.7/fastgenerateapi/schemas_factory/update_schema_factory.py` & `fastgenerateapi-0.0.8/fastgenerateapi/schemas_factory/update_schema_factory.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.7/fastgenerateapi/settings/settings.py` & `fastgenerateapi-0.0.8/fastgenerateapi/settings/settings.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.7/fastgenerateapi/utils/parse_str.py` & `fastgenerateapi-0.0.8/fastgenerateapi/utils/parse_str.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.7/fastgenerateapi.egg-info/PKG-INFO` & `fastgenerateapi-0.0.8/fastgenerateapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastgenerateapi
-Version: 0.0.7
+Version: 0.0.8
 Summary: FastAPIView Class View
 Author: ShiLiang
 Author-email: 2509144896@qq.com
 License: GPL-3.0-or-later
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fastgenerateapi-0.0.7/fastgenerateapi.egg-info/SOURCES.txt` & `fastgenerateapi-0.0.8/fastgenerateapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.7/setup.py` & `fastgenerateapi-0.0.8/setup.py`

 * *Files identical despite different names*

