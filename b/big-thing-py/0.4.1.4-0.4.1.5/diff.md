# Comparing `tmp/big_thing_py-0.4.1.4-9-py3-none-any.whl.zip` & `tmp/big_thing_py-0.4.1.5-1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,55 +1,97 @@
-Zip file size: 73799 bytes, number of entries: 53
--rw-rw-r--  2.0 unx        0 b- defN 22-Nov-18 05:09 big_thing_py/__init__.py
--rw-rw-r--  2.0 unx    40278 b- defN 23-Jan-31 17:55 big_thing_py/big_thing.py
--rw-rw-r--  2.0 unx    32312 b- defN 22-Dec-08 03:45 big_thing_py/manager_thing.py
--rw-rw-r--  2.0 unx     1871 b- defN 22-Dec-08 03:45 big_thing_py/staff_thing.py
--rw-rw-r--  2.0 unx    33419 b- defN 23-Feb-01 06:19 big_thing_py/super_thing.py
--rw-rw-r--  2.0 unx      139 b- defN 22-Nov-18 05:09 big_thing_py/common/__init__.py
--rw-rw-r--  2.0 unx     1119 b- defN 23-Jan-30 08:23 big_thing_py/common/common.py
--rw-rw-r--  2.0 unx      620 b- defN 22-Dec-19 08:29 big_thing_py/common/error.py
--rw-rw-r--  2.0 unx    20669 b- defN 23-Jan-30 10:14 big_thing_py/common/mqtt_message.py
--rw-rw-r--  2.0 unx     1913 b- defN 23-Jan-30 07:00 big_thing_py/common/request.py
--rw-rw-r--  2.0 unx    12796 b- defN 22-Dec-19 08:29 big_thing_py/common/soptype.py
--rw-rw-r--  2.0 unx     1603 b- defN 22-Nov-18 05:09 big_thing_py/common/thread.py
--rw-rw-r--  2.0 unx      132 b- defN 22-Sep-21 07:09 big_thing_py/core/__init__.py
--rw-rw-r--  2.0 unx      709 b- defN 23-Jan-27 07:57 big_thing_py/core/argument.py
--rw-rw-r--  2.0 unx     7616 b- defN 22-Dec-19 08:29 big_thing_py/core/function.py
--rw-rw-r--  2.0 unx     3143 b- defN 22-Dec-19 08:29 big_thing_py/core/service.py
--rw-rw-r--  2.0 unx     1080 b- defN 22-Oct-30 11:56 big_thing_py/core/tag.py
--rw-rw-r--  2.0 unx     4991 b- defN 23-Jan-27 08:56 big_thing_py/core/thing.py
--rw-rw-r--  2.0 unx     4419 b- defN 22-Nov-18 05:09 big_thing_py/core/value.py
--rw-rw-r--  2.0 unx       59 b- defN 22-Dec-08 03:45 big_thing_py/manager/__init__.py
--rw-rw-r--  2.0 unx      746 b- defN 22-Dec-08 03:45 big_thing_py/manager/manager_common.py
--rw-rw-r--  2.0 unx     3669 b- defN 22-Dec-08 03:45 big_thing_py/manager/manager_utils.py
--rw-rw-r--  2.0 unx       65 b- defN 22-Nov-18 05:09 big_thing_py/super/__init__.py
--rw-rw-r--  2.0 unx    34205 b- defN 23-Jan-30 06:29 big_thing_py/super/super_function.py
--rw-rw-r--  2.0 unx    17528 b- defN 23-Jan-30 08:33 big_thing_py/super/super_request.py
--rw-rw-r--  2.0 unx      781 b- defN 22-Nov-18 05:09 big_thing_py/super/super_service_utils.py
--rw-rw-r--  2.0 unx        0 b- defN 22-Sep-21 07:09 big_thing_py/tests/__init__.py
--rw-rw-r--  2.0 unx       24 b- defN 22-Dec-21 04:28 big_thing_py/tests/conftest.py
--rw-rw-r--  2.0 unx        0 b- defN 22-Sep-21 07:09 big_thing_py/tests/basic/__init__.py
--rw-rw-r--  2.0 unx    10704 b- defN 22-Dec-19 08:29 big_thing_py/tests/basic/test_basic_feature.py
--rw-rw-r--  2.0 unx     8107 b- defN 22-Dec-19 08:29 big_thing_py/tests/basic/test_tolerance_feature.py
--rw-rw-r--  2.0 unx        0 b- defN 22-Sep-21 07:09 big_thing_py/tests/manager/__init__.py
--rw-rw-r--  2.0 unx     7248 b- defN 22-Sep-21 07:09 big_thing_py/tests/manager/test_hejhome_manager_thing.py
--rw-rw-r--  2.0 unx     7248 b- defN 22-Sep-21 07:09 big_thing_py/tests/manager/test_hue_manager_thing.py
--rw-rw-r--  2.0 unx     9126 b- defN 22-Sep-21 07:09 big_thing_py/tests/manager/test_rf_manager_thing.py
--rw-rw-r--  2.0 unx     7248 b- defN 22-Sep-21 07:09 big_thing_py/tests/manager/test_smartthings_manager_thing.py
--rw-rw-r--  2.0 unx        0 b- defN 22-Sep-21 07:09 big_thing_py/tests/super/__init__.py
--rw-rw-r--  2.0 unx     5298 b- defN 22-Sep-21 07:09 big_thing_py/tests/super/test_super_feature.py
--rw-rw-r--  2.0 unx      230 b- defN 22-Sep-21 07:09 big_thing_py/utils/__init__.py
--rw-rw-r--  2.0 unx     9753 b- defN 22-Dec-08 03:45 big_thing_py/utils/api_util.py
--rw-rw-r--  2.0 unx      286 b- defN 22-Sep-21 07:09 big_thing_py/utils/base64_util.py
--rw-rw-r--  2.0 unx     4246 b- defN 22-Nov-18 05:09 big_thing_py/utils/common_util.py
--rw-rw-r--  2.0 unx      212 b- defN 22-Oct-21 08:09 big_thing_py/utils/exception_util.py
--rw-rw-r--  2.0 unx      844 b- defN 22-Dec-19 08:29 big_thing_py/utils/file_util.py
--rw-rw-r--  2.0 unx     1068 b- defN 22-Dec-19 08:29 big_thing_py/utils/json_util.py
--rw-rw-r--  2.0 unx     7486 b- defN 22-Dec-19 08:29 big_thing_py/utils/log_util.py
--rw-rw-r--  2.0 unx     2038 b- defN 22-Nov-18 05:09 big_thing_py/utils/mqtt_util.py
--rw-rw-r--  2.0 unx     1680 b- defN 22-Nov-18 05:09 big_thing_py/utils/rf_util.py
--rw-r--r--  2.0 unx     1062 b- defN 23-Feb-01 06:21 big_thing_py-0.4.1.4.dist-info/LICENSE
--rw-rw-r--  2.0 unx      574 b- defN 23-Feb-01 06:21 big_thing_py-0.4.1.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Feb-01 06:21 big_thing_py-0.4.1.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx       13 b- defN 23-Feb-01 06:21 big_thing_py-0.4.1.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     4762 b- defN 23-Feb-01 06:21 big_thing_py-0.4.1.4.dist-info/RECORD
-53 files, 315231 bytes uncompressed, 66103 bytes compressed:  79.0%
+Zip file size: 140339 bytes, number of entries: 95
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 big_thing_py/__init__.py
+-rw-r--r--  2.0 unx    49645 b- defN 80-Jan-01 00:00 big_thing_py/big_thing.py
+-rw-r--r--  2.0 unx       87 b- defN 80-Jan-01 00:00 big_thing_py/common/__init__.py
+-rw-r--r--  2.0 unx     1226 b- defN 80-Jan-01 00:00 big_thing_py/common/common.py
+-rw-r--r--  2.0 unx     2980 b- defN 80-Jan-01 00:00 big_thing_py/common/error.py
+-rw-r--r--  2.0 unx    19163 b- defN 80-Jan-01 00:00 big_thing_py/common/mxtype.py
+-rw-r--r--  2.0 unx     1542 b- defN 80-Jan-01 00:00 big_thing_py/common/thread.py
+-rw-r--r--  2.0 unx      132 b- defN 80-Jan-01 00:00 big_thing_py/core/__init__.py
+-rw-r--r--  2.0 unx     1711 b- defN 80-Jan-01 00:00 big_thing_py/core/argument.py
+-rw-r--r--  2.0 unx    12748 b- defN 80-Jan-01 00:00 big_thing_py/core/function.py
+-rw-r--r--  2.0 unx     9322 b- defN 80-Jan-01 00:00 big_thing_py/core/mqtt_message.py
+-rw-r--r--  2.0 unx     1705 b- defN 80-Jan-01 00:00 big_thing_py/core/request.py
+-rw-r--r--  2.0 unx     4781 b- defN 80-Jan-01 00:00 big_thing_py/core/service.py
+-rw-r--r--  2.0 unx     1283 b- defN 80-Jan-01 00:00 big_thing_py/core/tag.py
+-rw-r--r--  2.0 unx     7360 b- defN 80-Jan-01 00:00 big_thing_py/core/thing.py
+-rw-r--r--  2.0 unx     5766 b- defN 80-Jan-01 00:00 big_thing_py/core/value.py
+-rw-r--r--  2.0 unx       59 b- defN 80-Jan-01 00:00 big_thing_py/manager/__init__.py
+-rw-r--r--  2.0 unx      768 b- defN 80-Jan-01 00:00 big_thing_py/manager/manager_common.py
+-rw-r--r--  2.0 unx     3674 b- defN 80-Jan-01 00:00 big_thing_py/manager/manager_utils.py
+-rw-r--r--  2.0 unx    27560 b- defN 80-Jan-01 00:00 big_thing_py/manager_thing.py
+-rw-r--r--  2.0 unx     1835 b- defN 80-Jan-01 00:00 big_thing_py/staff_thing.py
+-rw-r--r--  2.0 unx       93 b- defN 80-Jan-01 00:00 big_thing_py/super/__init__.py
+-rw-r--r--  2.0 unx    36953 b- defN 80-Jan-01 00:00 big_thing_py/super/super_function.py
+-rw-r--r--  2.0 unx    12707 b- defN 80-Jan-01 00:00 big_thing_py/super/super_mqtt_message.py
+-rw-r--r--  2.0 unx    18331 b- defN 80-Jan-01 00:00 big_thing_py/super/super_request.py
+-rw-r--r--  2.0 unx    34983 b- defN 80-Jan-01 00:00 big_thing_py/super_thing.py
+-rw-r--r--  2.0 unx      459 b- defN 80-Jan-01 00:00 big_thing_py/tests/README.md
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 big_thing_py/tests/__init__.py
+-rw-r--r--  2.0 unx       10 b- defN 80-Jan-01 00:00 big_thing_py/tests/api/.gitignore
+-rw-r--r--  2.0 unx     2964 b- defN 80-Jan-01 00:00 big_thing_py/tests/api/test_hejhome_api.py
+-rw-r--r--  2.0 unx     4188 b- defN 80-Jan-01 00:00 big_thing_py/tests/api/test_hue_api.py
+-rw-r--r--  2.0 unx     2596 b- defN 80-Jan-01 00:00 big_thing_py/tests/api/test_smartthings_api.py
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 big_thing_py/tests/basic/__init__.py
+-rw-r--r--  2.0 unx     1392 b- defN 80-Jan-01 00:00 big_thing_py/tests/basic/test_alive.py
+-rw-r--r--  2.0 unx    23301 b- defN 80-Jan-01 00:00 big_thing_py/tests/basic/test_eq.py
+-rw-r--r--  2.0 unx    34112 b- defN 80-Jan-01 00:00 big_thing_py/tests/basic/test_function_execution.py
+-rw-r--r--  2.0 unx     1814 b- defN 80-Jan-01 00:00 big_thing_py/tests/basic/test_generate_thing_id.py
+-rw-r--r--  2.0 unx    73901 b- defN 80-Jan-01 00:00 big_thing_py/tests/basic/test_init_element.py
+-rw-r--r--  2.0 unx     8399 b- defN 80-Jan-01 00:00 big_thing_py/tests/basic/test_mqtt.py
+-rw-r--r--  2.0 unx    19140 b- defN 80-Jan-01 00:00 big_thing_py/tests/basic/test_register.py
+-rw-r--r--  2.0 unx     4866 b- defN 80-Jan-01 00:00 big_thing_py/tests/basic/test_unregister.py
+-rw-r--r--  2.0 unx     7520 b- defN 80-Jan-01 00:00 big_thing_py/tests/basic/test_value_publish.py
+-rw-r--r--  2.0 unx    37286 b- defN 80-Jan-01 00:00 big_thing_py/tests/conftest.py
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 big_thing_py/tests/manager/__init__.py
+-rw-r--r--  2.0 unx     7229 b- defN 80-Jan-01 00:00 big_thing_py/tests/manager/test_hejhome_manager_thing.py
+-rw-r--r--  2.0 unx     7229 b- defN 80-Jan-01 00:00 big_thing_py/tests/manager/test_hue_manager_thing.py
+-rw-r--r--  2.0 unx     9107 b- defN 80-Jan-01 00:00 big_thing_py/tests/manager/test_rf_manager_thing.py
+-rw-r--r--  2.0 unx     7229 b- defN 80-Jan-01 00:00 big_thing_py/tests/manager/test_smartthings_manager_thing.py
+-rwxr-xr-x  2.0 unx      646 b- defN 80-Jan-01 00:00 big_thing_py/tests/run_test.sh
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 big_thing_py/tests/super/__init__.py
+-rw-r--r--  2.0 unx    13915 b- defN 80-Jan-01 00:00 big_thing_py/tests/super/service_list_result_input_1.json
+-rw-r--r--  2.0 unx     9777 b- defN 80-Jan-01 00:00 big_thing_py/tests/super/service_list_result_input_2.json
+-rw-r--r--  2.0 unx     5639 b- defN 80-Jan-01 00:00 big_thing_py/tests/super/service_list_result_input_3.json
+-rw-r--r--  2.0 unx    13891 b- defN 80-Jan-01 00:00 big_thing_py/tests/super/service_list_result_input_4.json
+-rw-r--r--  2.0 unx    13916 b- defN 80-Jan-01 00:00 big_thing_py/tests/super/service_list_result_input_5.json
+-rw-r--r--  2.0 unx    13916 b- defN 80-Jan-01 00:00 big_thing_py/tests/super/service_list_result_input_6.json
+-rw-r--r--  2.0 unx    13913 b- defN 80-Jan-01 00:00 big_thing_py/tests/super/service_list_result_input_7.json
+-rw-r--r--  2.0 unx    13913 b- defN 80-Jan-01 00:00 big_thing_py/tests/super/service_list_result_input_8.json
+-rw-r--r--  2.0 unx    13341 b- defN 80-Jan-01 00:00 big_thing_py/tests/super/service_list_result_input_level1_with_0_service.json
+-rw-r--r--  2.0 unx    17293 b- defN 80-Jan-01 00:00 big_thing_py/tests/super/service_list_result_input_level1_with_1_service.json
+-rw-r--r--  2.0 unx    25197 b- defN 80-Jan-01 00:00 big_thing_py/tests/super/service_list_result_input_level1_with_3_service.json
+-rw-r--r--  2.0 unx    13443 b- defN 80-Jan-01 00:00 big_thing_py/tests/super/service_list_result_input_level2_with_0_service.json
+-rw-r--r--  2.0 unx    17304 b- defN 80-Jan-01 00:00 big_thing_py/tests/super/service_list_result_input_level2_with_1_service.json
+-rw-r--r--  2.0 unx    25208 b- defN 80-Jan-01 00:00 big_thing_py/tests/super/service_list_result_input_level2_with_3_service.json
+-rw-r--r--  2.0 unx    13545 b- defN 80-Jan-01 00:00 big_thing_py/tests/super/service_list_result_input_level3_with_0_service.json
+-rw-r--r--  2.0 unx    18678 b- defN 80-Jan-01 00:00 big_thing_py/tests/super/service_list_result_input_level3_with_1_service.json
+-rw-r--r--  2.0 unx    25413 b- defN 80-Jan-01 00:00 big_thing_py/tests/super/service_list_result_input_level3_with_3_service.json
+-rw-r--r--  2.0 unx    13377 b- defN 80-Jan-01 00:00 big_thing_py/tests/super/test_init_super_service.py
+-rw-r--r--  2.0 unx    18728 b- defN 80-Jan-01 00:00 big_thing_py/tests/super/test_req.py
+-rw-r--r--  2.0 unx   109138 b- defN 80-Jan-01 00:00 big_thing_py/tests/super/test_super_execute.py
+-rw-r--r--  2.0 unx    70037 b- defN 80-Jan-01 00:00 big_thing_py/tests/super/test_super_schedule.py
+-rw-r--r--  2.0 unx     4034 b- defN 80-Jan-01 00:00 big_thing_py/tests/super/test_super_service_list.py
+-rw-r--r--  2.0 unx    11474 b- defN 80-Jan-01 00:00 big_thing_py/tests/thing_factory.py
+-rw-r--r--  2.0 unx      121 b- defN 80-Jan-01 00:00 big_thing_py/tests/utils/test_api_util.py
+-rw-r--r--  2.0 unx      120 b- defN 80-Jan-01 00:00 big_thing_py/tests/utils/test_base64_util.py
+-rw-r--r--  2.0 unx    12246 b- defN 80-Jan-01 00:00 big_thing_py/tests/utils/test_common_util.py
+-rw-r--r--  2.0 unx      120 b- defN 80-Jan-01 00:00 big_thing_py/tests/utils/test_exception_util.py
+-rw-r--r--  2.0 unx      120 b- defN 80-Jan-01 00:00 big_thing_py/tests/utils/test_file_util.py
+-rw-r--r--  2.0 unx     2909 b- defN 80-Jan-01 00:00 big_thing_py/tests/utils/test_json_util.py
+-rw-r--r--  2.0 unx      120 b- defN 80-Jan-01 00:00 big_thing_py/tests/utils/test_log_util.py
+-rw-r--r--  2.0 unx      275 b- defN 80-Jan-01 00:00 big_thing_py/tests/utils/test_mqtt_util.py
+-rw-r--r--  2.0 unx      120 b- defN 80-Jan-01 00:00 big_thing_py/tests/utils/test_rf_util.py
+-rw-r--r--  2.0 unx      230 b- defN 80-Jan-01 00:00 big_thing_py/utils/__init__.py
+-rw-r--r--  2.0 unx     2388 b- defN 80-Jan-01 00:00 big_thing_py/utils/api_util.py
+-rw-r--r--  2.0 unx      749 b- defN 80-Jan-01 00:00 big_thing_py/utils/base64_util.py
+-rw-r--r--  2.0 unx     6198 b- defN 80-Jan-01 00:00 big_thing_py/utils/common_util.py
+-rw-r--r--  2.0 unx      211 b- defN 80-Jan-01 00:00 big_thing_py/utils/exception_util.py
+-rw-r--r--  2.0 unx      842 b- defN 80-Jan-01 00:00 big_thing_py/utils/file_util.py
+-rw-r--r--  2.0 unx     1356 b- defN 80-Jan-01 00:00 big_thing_py/utils/json_util.py
+-rw-r--r--  2.0 unx     8361 b- defN 80-Jan-01 00:00 big_thing_py/utils/log_util.py
+-rw-r--r--  2.0 unx     2137 b- defN 80-Jan-01 00:00 big_thing_py/utils/mqtt_util.py
+-rw-r--r--  2.0 unx     1676 b- defN 80-Jan-01 00:00 big_thing_py/utils/rf_util.py
+-rw-r--r--  2.0 unx     3180 b- defN 80-Jan-01 00:00 big_thing_py-0.4.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 big_thing_py-0.4.1.5.dist-info/WHEEL
+?rw-r--r--  2.0 unx     9350 b- defN 16-Jan-01 00:00 big_thing_py-0.4.1.5.dist-info/RECORD
+95 files, 1057809 bytes uncompressed, 125109 bytes compressed:  88.2%
```

## zipnote {}

```diff
@@ -1,52 +1,43 @@
 Filename: big_thing_py/__init__.py
 Comment: 
 
 Filename: big_thing_py/big_thing.py
 Comment: 
 
-Filename: big_thing_py/manager_thing.py
-Comment: 
-
-Filename: big_thing_py/staff_thing.py
-Comment: 
-
-Filename: big_thing_py/super_thing.py
-Comment: 
-
 Filename: big_thing_py/common/__init__.py
 Comment: 
 
 Filename: big_thing_py/common/common.py
 Comment: 
 
 Filename: big_thing_py/common/error.py
 Comment: 
 
-Filename: big_thing_py/common/mqtt_message.py
-Comment: 
-
-Filename: big_thing_py/common/request.py
-Comment: 
-
-Filename: big_thing_py/common/soptype.py
+Filename: big_thing_py/common/mxtype.py
 Comment: 
 
 Filename: big_thing_py/common/thread.py
 Comment: 
 
 Filename: big_thing_py/core/__init__.py
 Comment: 
 
 Filename: big_thing_py/core/argument.py
 Comment: 
 
 Filename: big_thing_py/core/function.py
 Comment: 
 
+Filename: big_thing_py/core/mqtt_message.py
+Comment: 
+
+Filename: big_thing_py/core/request.py
+Comment: 
+
 Filename: big_thing_py/core/service.py
 Comment: 
 
 Filename: big_thing_py/core/tag.py
 Comment: 
 
 Filename: big_thing_py/core/thing.py
@@ -60,39 +51,84 @@
 
 Filename: big_thing_py/manager/manager_common.py
 Comment: 
 
 Filename: big_thing_py/manager/manager_utils.py
 Comment: 
 
+Filename: big_thing_py/manager_thing.py
+Comment: 
+
+Filename: big_thing_py/staff_thing.py
+Comment: 
+
 Filename: big_thing_py/super/__init__.py
 Comment: 
 
 Filename: big_thing_py/super/super_function.py
 Comment: 
 
+Filename: big_thing_py/super/super_mqtt_message.py
+Comment: 
+
 Filename: big_thing_py/super/super_request.py
 Comment: 
 
-Filename: big_thing_py/super/super_service_utils.py
+Filename: big_thing_py/super_thing.py
+Comment: 
+
+Filename: big_thing_py/tests/README.md
 Comment: 
 
 Filename: big_thing_py/tests/__init__.py
 Comment: 
 
-Filename: big_thing_py/tests/conftest.py
+Filename: big_thing_py/tests/api/.gitignore
+Comment: 
+
+Filename: big_thing_py/tests/api/test_hejhome_api.py
+Comment: 
+
+Filename: big_thing_py/tests/api/test_hue_api.py
+Comment: 
+
+Filename: big_thing_py/tests/api/test_smartthings_api.py
 Comment: 
 
 Filename: big_thing_py/tests/basic/__init__.py
 Comment: 
 
-Filename: big_thing_py/tests/basic/test_basic_feature.py
+Filename: big_thing_py/tests/basic/test_alive.py
+Comment: 
+
+Filename: big_thing_py/tests/basic/test_eq.py
+Comment: 
+
+Filename: big_thing_py/tests/basic/test_function_execution.py
+Comment: 
+
+Filename: big_thing_py/tests/basic/test_generate_thing_id.py
+Comment: 
+
+Filename: big_thing_py/tests/basic/test_init_element.py
+Comment: 
+
+Filename: big_thing_py/tests/basic/test_mqtt.py
 Comment: 
 
-Filename: big_thing_py/tests/basic/test_tolerance_feature.py
+Filename: big_thing_py/tests/basic/test_register.py
+Comment: 
+
+Filename: big_thing_py/tests/basic/test_unregister.py
+Comment: 
+
+Filename: big_thing_py/tests/basic/test_value_publish.py
+Comment: 
+
+Filename: big_thing_py/tests/conftest.py
 Comment: 
 
 Filename: big_thing_py/tests/manager/__init__.py
 Comment: 
 
 Filename: big_thing_py/tests/manager/test_hejhome_manager_thing.py
 Comment: 
@@ -102,18 +138,114 @@
 
 Filename: big_thing_py/tests/manager/test_rf_manager_thing.py
 Comment: 
 
 Filename: big_thing_py/tests/manager/test_smartthings_manager_thing.py
 Comment: 
 
+Filename: big_thing_py/tests/run_test.sh
+Comment: 
+
 Filename: big_thing_py/tests/super/__init__.py
 Comment: 
 
-Filename: big_thing_py/tests/super/test_super_feature.py
+Filename: big_thing_py/tests/super/service_list_result_input_1.json
+Comment: 
+
+Filename: big_thing_py/tests/super/service_list_result_input_2.json
+Comment: 
+
+Filename: big_thing_py/tests/super/service_list_result_input_3.json
+Comment: 
+
+Filename: big_thing_py/tests/super/service_list_result_input_4.json
+Comment: 
+
+Filename: big_thing_py/tests/super/service_list_result_input_5.json
+Comment: 
+
+Filename: big_thing_py/tests/super/service_list_result_input_6.json
+Comment: 
+
+Filename: big_thing_py/tests/super/service_list_result_input_7.json
+Comment: 
+
+Filename: big_thing_py/tests/super/service_list_result_input_8.json
+Comment: 
+
+Filename: big_thing_py/tests/super/service_list_result_input_level1_with_0_service.json
+Comment: 
+
+Filename: big_thing_py/tests/super/service_list_result_input_level1_with_1_service.json
+Comment: 
+
+Filename: big_thing_py/tests/super/service_list_result_input_level1_with_3_service.json
+Comment: 
+
+Filename: big_thing_py/tests/super/service_list_result_input_level2_with_0_service.json
+Comment: 
+
+Filename: big_thing_py/tests/super/service_list_result_input_level2_with_1_service.json
+Comment: 
+
+Filename: big_thing_py/tests/super/service_list_result_input_level2_with_3_service.json
+Comment: 
+
+Filename: big_thing_py/tests/super/service_list_result_input_level3_with_0_service.json
+Comment: 
+
+Filename: big_thing_py/tests/super/service_list_result_input_level3_with_1_service.json
+Comment: 
+
+Filename: big_thing_py/tests/super/service_list_result_input_level3_with_3_service.json
+Comment: 
+
+Filename: big_thing_py/tests/super/test_init_super_service.py
+Comment: 
+
+Filename: big_thing_py/tests/super/test_req.py
+Comment: 
+
+Filename: big_thing_py/tests/super/test_super_execute.py
+Comment: 
+
+Filename: big_thing_py/tests/super/test_super_schedule.py
+Comment: 
+
+Filename: big_thing_py/tests/super/test_super_service_list.py
+Comment: 
+
+Filename: big_thing_py/tests/thing_factory.py
+Comment: 
+
+Filename: big_thing_py/tests/utils/test_api_util.py
+Comment: 
+
+Filename: big_thing_py/tests/utils/test_base64_util.py
+Comment: 
+
+Filename: big_thing_py/tests/utils/test_common_util.py
+Comment: 
+
+Filename: big_thing_py/tests/utils/test_exception_util.py
+Comment: 
+
+Filename: big_thing_py/tests/utils/test_file_util.py
+Comment: 
+
+Filename: big_thing_py/tests/utils/test_json_util.py
+Comment: 
+
+Filename: big_thing_py/tests/utils/test_log_util.py
+Comment: 
+
+Filename: big_thing_py/tests/utils/test_mqtt_util.py
+Comment: 
+
+Filename: big_thing_py/tests/utils/test_rf_util.py
 Comment: 
 
 Filename: big_thing_py/utils/__init__.py
 Comment: 
 
 Filename: big_thing_py/utils/api_util.py
 Comment: 
@@ -138,23 +270,17 @@
 
 Filename: big_thing_py/utils/mqtt_util.py
 Comment: 
 
 Filename: big_thing_py/utils/rf_util.py
 Comment: 
 
-Filename: big_thing_py-0.4.1.4.dist-info/LICENSE
-Comment: 
-
-Filename: big_thing_py-0.4.1.4.dist-info/METADATA
-Comment: 
-
-Filename: big_thing_py-0.4.1.4.dist-info/WHEEL
+Filename: big_thing_py-0.4.1.5.dist-info/METADATA
 Comment: 
 
-Filename: big_thing_py-0.4.1.4.dist-info/top_level.txt
+Filename: big_thing_py-0.4.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: big_thing_py-0.4.1.4.dist-info/RECORD
+Filename: big_thing_py-0.4.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## big_thing_py/big_thing.py

```diff
@@ -1,190 +1,262 @@
-from big_thing_py.common.request import *
 from big_thing_py.core.thing import *
 
 import paho.mqtt.client as mqtt
-from paho.mqtt.client import Client as SoPClient
-from zeroconf import IPVersion, ServiceBrowser, ServiceStateChange, Zeroconf, ZeroconfServiceTypes
+from paho.mqtt.client import Client as MXClient
+from zeroconf import IPVersion, ServiceBrowser, ServiceStateChange, Zeroconf, ServiceInfo
 import ssl
 import argparse
+import socket
 
-# ======================================================================
-#  _____        ______ ______  _         _____  _      _
-# /  ___|       | ___ \| ___ \(_)       |_   _|| |    (_)
-# \ `--.   ___  | |_/ /| |_/ / _   __ _   | |  | |__   _  _ __    __ _
-#  `--. \ / _ \ |  __/ | ___ \| | / _` |  | |  | '_ \ | || '_ \  / _` |
-# /\__/ /| (_) || |    | |_/ /| || (_| |  | |  | | | || || | | || (_| |
-# \____/  \___/ \_|    \____/ |_| \__, |  \_/  |_| |_||_||_| |_| \__, |
-#                                  __/ |                          __/ |
-#                                 |___/                          |___/
-# ======================================================================
-
-
-class SoPBigThing(SoPThing):
-    def __init__(self, name: str, service_list: List[SoPService], alive_cycle: float, is_super: bool = False, is_parallel: bool = True,
-                 ip: str = None, port: int = None, ssl_ca_path: str = None, ssl_enable: bool = False, 
-                 log_name: str = None, log_enable: bool = True, log_mode: SoPPrintMode = SoPPrintMode.ABBR, 
-                 append_mac_address: bool = True, retry_register: bool = True):
+# ASCII Art from https://patorjk.com/software/taag/#p=display&h=1&v=1&f=Big
+
+# ======================================================================== #
+#    _____         _____   ____   _      _______  _      _                 #
+#   / ____|       |  __ \ |  _ \ (_)    |__   __|| |    (_)                #
+#  | (___    ___  | |__) || |_) | _   __ _ | |   | |__   _  _ __    __ _   #
+#   \___ \  / _ \ |  ___/ |  _ < | | / _` || |   | '_ \ | || '_ \  / _` |  #
+#   ____) || (_) || |     | |_) || || (_| || |   | | | || || | | || (_| |  #
+#  |_____/  \___/ |_|     |____/ |_| \__, ||_|   |_| |_||_||_| |_| \__, |  #
+#                                     __/ |                         __/ |  #
+#                                    |___/                         |___/   #
+# ======================================================================== #
+
+
+class MXBigThing(MXThing):
+
+    def __init__(self, name: str = MXThing.DEFAULT_NAME, service_list: List[MXService] = [], alive_cycle: float = 60, is_super: bool = False, is_parallel: bool = True,
+                 ip: str = '127.0.0.1', port: int = 1883, ssl_ca_path: str = '', ssl_enable: bool = False,
+                 log_name: str = '', log_enable: bool = True, log_mode: MXPrintMode = MXPrintMode.ABBR,
+                 append_mac_address: bool = True):
         super().__init__(name, service_list, alive_cycle, is_super, is_parallel)
 
+        # Log
         self._log_mode = log_mode
-        if log_enable:
-            START_LOGGER(whole_log_path=log_name,
-                         logging_mode=SoPLogger.LoggingMode.ALL)
-        else:
-            START_LOGGER(logging_mode=SoPLogger.LoggingMode.OFF)
+        self._log_enable = log_enable
+        self._log_name = log_name
 
         # MQTT
-        self._connected = False
-        self._ip: str = get_ip_from_url(ip.strip())
-        self._port: int = port
-        self._mac_address: str = get_mac_address()
-        self._ssl_ca_path: str = ssl_ca_path
-        self._ssl_enable: bool = ssl_enable
-        self._avahi_discovered_middleware_list: List[str] = []
-        self._avahi_middleware_name = None
-        
-        self.retry_register = retry_register
+        self._mqtt_client: MXClient = None
+        self._ip = convert_url_to_ip(ip)
+        self._port = port
+        self._ssl_ca_path = ssl_ca_path
+        self._ssl_enable = ssl_enable
+
+        # Util
+        self._append_mac_address = append_mac_address
 
+        # Thread
         self._g_exit: Event = Event()
         self._g_comm_exit: Event = Event()
-        self._comm_thread_list: List[SoPThread] = []
-        self._thread_list: List[SoPThread] = []
-
-        # Queue
-        self._receive_queue: Queue = Queue()
-        self._publish_queue: Queue = Queue()
+        self._comm_thread_list: List[MXThread] = []
+        self._thread_list: List[MXThread] = []
 
         self._thread_comm_func_list: List[Callable] = [
-            self._receive_message_thread_func,
-            self._publish_message_thread_func,]
+            self._message_receiving_thread_func,
+            self._message_publishing_thread_func,
+        ]
         self._thread_func_list: List[Callable] = [
-            self._alive_thread_func,
-            self._value_publish_thread_func,
+            self._alive_publishing_thread_func,
+            self._value_publishing_thread_func,
         ]
 
-        if append_mac_address:
-            self._name = self._name + f'_{self._mac_address}'
+        if not is_valid_ip_address(self._ip) or not 1024 < self._port <= 65535:
+            raise MXValueError('Invalid IP address, port number')
         else:
-            pass
-        self._mqtt_client = SoPClient(userdata=None, client_id=self._name)
+            self._ip = convert_url_to_ip(ip)
 
-        for function in self._function_list:
-            function.set_publish_queue(self._publish_queue)
+        if self._is_super and not self._is_parallel:
+            raise MXValueError('Super Thing must be parallel')
+
+        if self._ssl_enable:
+            if not self._ssl_ca_path:
+                raise MXValueError(
+                    'ssl_enable is True but ssl_ca_path is empty')
+            elif not (os.path.exists(f'{self._ssl_ca_path}/ca.crt') and
+                      os.path.exists(f'{self._ssl_ca_path}/client.crt') and
+                      os.path.exists(f'{self._ssl_ca_path}/client.key')):
+                raise MXValueError('SSL CA file not found')
 
-    def __eq__(self, o: object) -> bool:
+    def __eq__(self, o: 'MXBigThing') -> bool:
+        instance_check = isinstance(o, MXBigThing)
         is_parallel_check = (self._is_parallel == o._is_parallel)
         is_super_check = (self._is_super == o._is_super)
 
-        return super().__eq__(o) and is_parallel_check and is_super_check
+        return super().__eq__(o) and instance_check and is_parallel_check and is_super_check
+
+    def __getstate__(self):
+        state = super().__getstate__()
+
+        state['_ip'] = self._ip
+        state['_port'] = self._port
+        state['_ssl_ca_path'] = self._ssl_ca_path
+        state['_ssl_enable'] = self._ssl_enable
+        state['_append_mac_address'] = self._append_mac_address
+
+        del state['_log_mode']
+        del state['_log_enable']
+        del state['_log_name']
+        del state['_mqtt_client']
+        del state['_g_exit']
+        del state['_g_comm_exit']
+        del state['_comm_thread_list']
+        del state['_thread_list']
+        del state['_thread_comm_func_list']
+        del state['_thread_func_list']
+
+        return state
+
+    def __setstate__(self, state):
+        super().__setstate__(state)
+
+        self._type = state['_type']
+        self._min = state['_min']
+        self._max = state['_max']
+        self._cycle = state['_cycle']
+        self._format = state['_format']
+
+        self._log_mode = MXPrintMode.ABBR
+        self._log_enable = True
+        self._log_name = ''
+        self._mqtt_client = None
+        self._g_exit = Event()
+        self._g_comm_exit = Event()
+        self._comm_thread_list = []
+        self._thread_list = []
+        self._thread_comm_func_list = [
+            self._message_receiving_thread_func,
+            self._message_publishing_thread_func,
+        ]
+        self._thread_func_list = [
+            self._alive_publishing_thread_func,
+            self._value_publishing_thread_func,
+        ]
+
+    def setup(self, avahi_enable=True) -> 'MXBigThing':
+        self._init_logger()
+        self._update_thing_ID(self._name)
+
+        self._receive_queue = Queue()
+        self._publish_queue = Queue()
+
+        self._mqtt_client = MXClient(client_id=self._name)
+
+        for function in self._function_list:
+            function.set_publish_queue(self._publish_queue)
+
+        # TODO: MXThing에서 처리할 것인지 MXBigThing에서 처리할 것인지 정해야함.
+        self._value_list = []
+        self._function_list = []
+        for service in self._service_list:
+            if isinstance(service, (MXFunction, MXValue)):
+                self.add_service(service)
+            else:
+                raise MXTypeError(
+                    f'service_list must contain MXFunction or MXValue object')
 
-    def setup(self, avahi_enable=True):
         try:
-            self._avahi_enable = avahi_enable
-            self._avahi_init(avahi_enable)
+            if avahi_enable:
+                check_python_version()
+                self._auto_setup_middleware()
+            else:
+                MXLOG_DEBUG('Skip Middleware discover...')
+
             if self._ssl_enable == True:
+                MXLOG_DEBUG('Connect with SSL mode...', 'blue')
                 self._set_ssl_config()
             else:
-                SOPLOG_DEBUG('SSL is not enabled...')
-            self._connect()
+                MXLOG_DEBUG('Connect with Non-SSL mode...', 'blue')
+            # self._connect(self._ip, self._port)
 
             # receive, publish쓰레드는 나머지 쓰레드들과 분리하여 exit event를 설정
             # wrapup 할 때 나머지 쓰레드들은 한꺼번에 종료가 되어도 되지만, receive, publish 쓰레드는
             # receive, publish queue에 남아있는 메시지를 모두 전송, 처리하고 종료되어야 하기 때문에
             # exit event를 따로 설정하여 종료시킴
             for func in self._thread_comm_func_list:
-                thread = SoPThread(func=func, arg_list=(self._g_comm_exit, ))
+                thread = MXThread(target=func, args=(self._g_comm_exit, ))
                 self._comm_thread_list.append(thread)
             for func in self._thread_func_list:
-                thread = SoPThread(func=func, arg_list=(self._g_exit, ))
+                thread = MXThread(target=func, args=(self._g_exit, ))
                 self._thread_list.append(thread)
 
-            return True
+            return self
         except KeyboardInterrupt:
-            SOPLOG_DEBUG('Ctrl + C Exit', 'red')
-            return self.wrapup()
-        except ConnectionRefusedError:
-            SOPLOG_DEBUG(
-                'Connection error while connect to broker. Check ip and port', 'red')
+            MXLOG_DEBUG('Ctrl + C Exit', 'red')
             return self.wrapup()
         except Exception as e:
             print_error(e)
             return self.wrapup()
 
     def run(self):
 
-        def try_register_only_once():
-            SOPLOG_DEBUG(f'Register send', 'yellow')
-            self._subscribe_init_topics(self)
-            self._send_TM_REGISTER(
-                thing_name=self._name, payload=self.dump())
-
-            while not self._registered:
-                time.sleep(THREAD_TIME_OUT)
-
-        def try_register_cyclic(period: float = 10, retry: int = 5):
-            while not self._registered and retry:
-                SOPLOG_DEBUG(f'Register try {6-retry}', 'yellow')
+        # def try_register_only_once():
+        #     MXLOG_DEBUG(f'Register send', 'yellow')
+        #     self._subscribe_init_topic_list(self)
+        #     self._send_TM_REGISTER()
+
+        #     while not self._is_registered:
+        #         time.sleep(THREAD_TIME_OUT)
+
+        def try_register(period: float = 10, retry: int = 5):
+            while not self._is_registered and retry:
+                MXLOG_DEBUG(f'Register try {6-retry}', 'yellow')
                 retry -= 1
 
-                self._subscribe_init_topics(self)
-                self._send_TM_REGISTER(
-                    thing_name=self._name, payload=self.dump())
+                self._subscribe_init_topic_list()
+                self._send_TM_REGISTER()
 
                 current_time = get_current_time()
                 while get_current_time() - current_time < period:
-                    if self._registered:
+                    if self._is_registered:
                         break
                     else:
                         time.sleep(THREAD_TIME_OUT)
 
         try:
+            self._connect(self._ip, self._port)
             # Start main threads
+
             for thread in self._comm_thread_list + self._thread_list:
                 thread.start()
 
-            if self.retry_register:
-                try_register_cyclic(period=10, retry=5)
-            else:
-                try_register_only_once()
+            try_register(period=10, retry=5)
 
             # Maintain main thread
             while not self._g_exit.wait(THREAD_TIME_OUT):
                 time.sleep(1000)
         except KeyboardInterrupt as e:
-            SOPLOG_DEBUG('Ctrl + C Exit', 'red')
+            MXLOG_DEBUG('Ctrl + C Exit', 'red')
             return self.wrapup()
         except ConnectionRefusedError as e:
-            SOPLOG_DEBUG(
-                'Connection error while connect to broker. Check ip and port', 'red')
-            return self.wrapup()
+            MXLOG_DEBUG(f'Connection error while connect to broker. Check ip and port - {self._ip}:{self._port}', 'red')
+            sys.exit(1)
         except Exception as e:
             print_error(e)
             return self.wrapup()
 
     def wrapup(self):
         try:
-            self._send_TM_UNREGISTER(self._name)
+            self._send_TM_UNREGISTER()
             cur_time = get_current_time()
 
             self._g_exit.set()
             for thread in self._thread_list:
                 thread.join()
-                SOPLOG_DEBUG(f'{thread._name} is terminated', 'yellow')
+                MXLOG_DEBUG(f'{thread._name} is terminated', 'yellow')
 
             while not ((self._publish_queue.empty() and self._receive_queue.empty()) or (get_current_time() - cur_time > 3)):
                 time.sleep(THREAD_TIME_OUT)
 
             self._g_comm_exit.set()
             for thread in self._comm_thread_list:
                 thread.join()
-                SOPLOG_DEBUG(f'{thread._name} is terminated', 'yellow')
+                MXLOG_DEBUG(f'{thread._name} is terminated', 'yellow')
 
             self._mqtt_client.disconnect()
-            SOPLOG_DEBUG('Thing Exit', 'red')
+            MXLOG_DEBUG('Thing Exit', 'red')
             return True
         except Exception as e:
             print_error(e)
             return False
 
     def arg_parse():
         parser = argparse.ArgumentParser()
@@ -208,725 +280,883 @@
                             required=False, help="Specify ssl CA file folder path")
         parser.add_argument("--append_mac_address", action='store_true', type=bool,
                             required=False, help="Whether to include a mac address in big thing name")
         args = parser.parse_args()
 
         return args
 
-    # ===========================================================================================
-    #  _    _                             _    __                      _    _
-    # | |  | |                           | |  / _|                    | |  (_)
-    # | |_ | |__   _ __   ___   __ _   __| | | |_  _   _  _ __    ___ | |_  _   ___   _ __   ___
-    # | __|| '_ \ | '__| / _ \ / _` | / _` | |  _|| | | || '_ \  / __|| __|| | / _ \ | '_ \ / __|
-    # | |_ | | | || |   |  __/| (_| || (_| | | |  | |_| || | | || (__ | |_ | || (_) || | | |\__ \
-    #  \__||_| |_||_|    \___| \__,_| \__,_| |_|   \__,_||_| |_| \___| \__||_| \___/ |_| |_||___/
-    # ===========================================================================================
+    # ================================================================================================= #
+    #   _______  _                            _   ______                    _    _                      #
+    #  |__   __|| |                          | | |  ____|                  | |  (_)                     #
+    #     | |   | |__   _ __  ___   __ _   __| | | |__  _   _  _ __    ___ | |_  _   ___   _ __   ___   #
+    #     | |   | '_ \ | '__|/ _ \ / _` | / _` | |  __|| | | || '_ \  / __|| __|| | / _ \ | '_ \ / __|  #
+    #     | |   | | | || |  |  __/| (_| || (_| | | |   | |_| || | | || (__ | |_ | || (_) || | | |\__ \  #
+    #     |_|   |_| |_||_|   \___| \__,_| \__,_| |_|    \__,_||_| |_| \___| \__||_| \___/ |_| |_||___/  #
+    # ================================================================================================= #
 
-    def _receive_message_thread_func(self, stop_event: Event):
+    def _message_receiving_thread_func(self, stop_event: Event):
         try:
             while not stop_event.wait(THREAD_TIME_OUT):
                 if self._receive_queue.empty():
                     continue
 
                 recv_msg = self._receive_queue.get()
-                self._handle_mqtt_message(recv_msg)
+                # TODO: 결과에 따라 어떤 동작을 할지 정의
+                rc = self._handle_mqtt_message(recv_msg)
         except Exception as e:
             stop_event.set()
             print_error(e)
             return False
 
-    def _publish_message_thread_func(self, stop_event: Event):
+    def _message_publishing_thread_func(self, stop_event: Event):
         try:
             while not stop_event.wait(THREAD_TIME_OUT):
                 if self._publish_queue.empty():
                     continue
 
                 pub_msg = self._publish_queue.get()
                 topic, payload, timestamp = decode_MQTT_message(
                     pub_msg, mode=str)
                 self._publish(topic, payload)
         except Exception as e:
             stop_event.set()
             print_error(e)
             return False
 
-    def _alive_thread_func(self, stop_event: Event) -> Union[bool, None]:
+    def _alive_publishing_thread_func(self, stop_event: Event) -> Union[bool, None]:
         try:
             while not stop_event.wait(THREAD_TIME_OUT):
-                if self._registered:
+                if self._is_registered:
                     current_time = get_current_time()
                     if current_time - self._last_alive_time > self._alive_cycle:
-                        self._send_TM_ALIVE(thing_name=self._name)
+                        self._send_TM_ALIVE()
                         self._last_alive_time = current_time
                 else:
                     pass
 
         except Exception as e:
             stop_event.set()
             print_error(e)
             return False
 
-    def _value_publish_thread_func(self, stop_event: Event) -> Union[bool, None]:
+    def _value_publishing_thread_func(self, stop_event: Event) -> Union[bool, None]:
         try:
             while not stop_event.wait(THREAD_TIME_OUT):
-                if not self._registered:
+                if not self._is_registered:
                     continue
                 current_time = get_current_time()
                 for value in self._value_list:
                     if not (current_time - value.get_last_update_time()) > value.get_cycle():
                         continue
-                    arg_list = tuple(value.get_arg_list())
-                    if value.update(*arg_list) is not None:
-                        self._send_TM_VALUE_PUBLISH(
-                            self._name, value.get_name(), value.dump_pub())
+
+                    is_updated = value.update()
+                    if is_updated is not None:
+                        self._send_TM_VALUE_PUBLISH(value=value)
         except Exception as e:
             stop_event.set()
             print_error(e)
             return False
 
-    # ====================================================================================================================
-    #  _                        _  _        ___  ___ _____  _____  _____
-    # | |                      | || |       |  \/  ||  _  ||_   _||_   _|
-    # | |__    __ _  _ __    __| || |  ___  | .  . || | | |  | |    | |    _ __ ___    ___  ___  ___   __ _   __ _   ___
-    # | '_ \  / _` || '_ \  / _` || | / _ \ | |\/| || | | |  | |    | |   | '_ ` _ \  / _ \/ __|/ __| / _` | / _` | / _ \
-    # | | | || (_| || | | || (_| || ||  __/ | |  | |\ \/' /  | |    | |   | | | | | ||  __/\__ \\__ \| (_| || (_| ||  __/
-    # |_| |_| \__,_||_| |_| \__,_||_| \___| \_|  |_/ \_/\_\  \_/    \_/   |_| |_| |_| \___||___/|___/ \__,_| \__, | \___|
-    #                                                                                                         __/ |
-    #                                                                                                        |___/
-    # ====================================================================================================================
-
-    def _handle_mqtt_message(self, msg: mqtt.MQTTMessage) -> None:
-        topic, payload, timestamp = unpack_mqtt_message(msg)
-        msg.timestamp = time.time()
-
-        if topic[0] == 'MT':
-            if topic[1] == 'RESULT':
-                if topic[2] == 'REGISTER':
-                    self._handle_MT_RESULT_REGISTER(msg)
-                elif topic[2] == 'UNREGISTER':
-                    self._handle_MT_RESULT_UNREGISTER(msg)
-                elif topic[2] == 'BINARY_VALUE':
-                    self._handle_MT_RESULT_BINARY_VALUE(msg)
+    # ======================================================================================================================= #
+    # _    _                    _  _         __  __   ____  _______  _______   __  __                                         #
+    # | |  | |                  | || |       |  \/  | / __ \|__   __||__   __| |  \/  |                                       #
+    # | |__| |  __ _  _ __    __| || |  ___  | \  / || |  | |  | |      | |    | \  / |  ___  ___  ___   __ _   __ _   ___    #
+    # |  __  | / _` || '_ \  / _` || | / _ \ | |\/| || |  | |  | |      | |    | |\/| | / _ \/ __|/ __| / _` | / _` | / _ \   #
+    # | |  | || (_| || | | || (_| || ||  __/ | |  | || |__| |  | |      | |    | |  | ||  __/\__ \\__ \| (_| || (_| ||  __/   #
+    # |_|  |_| \__,_||_| |_| \__,_||_| \___| |_|  |_| \___\_\  |_|      |_|    |_|  |_| \___||___/|___/ \__,_| \__, | \___|   #
+    #                                                                                                         __/ |           #
+    #                                                                                                         |___/           #
+    # ======================================================================================================================= #
+
+    def _classify_topic(self, topic: str) -> Union[MXProtocolType, bool]:
+        topic_token = topic_split(topic)
+        if topic_token[0] == 'MT':
+            if topic_token[1] == 'RESULT':
+                if topic_token[2] == 'REGISTER':
+                    MXProtocolType.Base.MT_RESULT_REGISTER
+                    protocol = MXProtocolType.Base.MT_RESULT_REGISTER
+                elif topic_token[2] == 'UNREGISTER':
+                    protocol = MXProtocolType.Base.MT_RESULT_UNREGISTER
+                elif topic_token[2] == 'BINARY_VALUE':
+                    protocol = MXProtocolType.Base.MT_RESULT_BINARY_VALUE
                 else:
-                    SOPLOG_DEBUG(
-                        f'[handle_mqtt_message] Unexpected MT_RESULT topic! topic: {topic}')
-            elif topic[1] == 'EXECUTE':
-                self._handle_MT_EXECUTE(msg)
+                    # FIXME: Errorcode
+                    return False
+            elif topic_token[1] == 'EXECUTE':
+                protocol = MXProtocolType.Base.MT_EXECUTE
             else:
-                SOPLOG_DEBUG(
-                    f'[handle_mqtt_message] Unexpected MT topic! topic: {topic}')
+                return False
+        else:
+            return False
 
-            return True
+        return protocol
+
+    def _handle_mqtt_message(self, msg: mqtt.MQTTMessage) -> bool:
+        topic_string = decode_MQTT_message(msg)[0]
+        protocol = self._classify_topic(topic_string)
+        msg.timestamp = time.time()
+
+        if protocol == MXProtocolType.Base.MT_RESULT_REGISTER:
+            rc = self._handle_MT_RESULT_REGISTER(msg)
+        elif protocol == MXProtocolType.Base.MT_RESULT_UNREGISTER:
+            rc = self._handle_MT_RESULT_UNREGISTER(msg)
+        elif protocol == MXProtocolType.Base.MT_RESULT_BINARY_VALUE:
+            rc = self._handle_MT_RESULT_BINARY_VALUE(msg)
+        elif protocol == MXProtocolType.Base.MT_EXECUTE:
+            rc = self._handle_MT_EXECUTE(msg)
         else:
+            MXLOG_DEBUG(
+                f'[{get_current_function_name()}] Unexpected topic! topic: {topic_string}')
             return False
 
+        return rc
+
     # ===============
     # ___  ___ _____
     # |  \/  ||_   _|
     # | .  . |  | |
     # | |\/| |  | |
     # | |  | |  | |
     # \_|  |_/  \_/
     # ===============
 
     def _handle_MT_RESULT_REGISTER(self, msg: mqtt.MQTTMessage):
-        register_result_msg = SoPRegisterResultMessage(msg)
-        if not self._name == register_result_msg._thing_name:
-            SOPLOG_DEBUG(
-                f'Wrong payload arrive... {self._name} should be arrive, not {register_result_msg._thing_name}', 'red')
-            raise
-
-        if self._check_register_result(register_result_msg._error):
-            self._middleware_name = register_result_msg._middleware_name
-            self._registered = True
-            self._subscribe_service_topics(self)
+        register_result_msg = MXRegisterResultMessage(msg)
+        if self._name != register_result_msg.thing_name:
+            MXLOG_DEBUG(
+                f'[{get_current_function_name()}] Wrong payload arrive... {self._name} should be arrive, not {register_result_msg.thing_name}')
+            # FIXME: False -> ErrorCode
+            return False
+
+        # FIXME: False -> ErrorCode
+        error = register_result_msg.error
+        if error in [MXErrorCode.NO_ERROR, MXErrorCode.DUPLICATE]:
+            MXLOG_DEBUG(
+                f'{PrintTag.GOOD if error == MXErrorCode.NO_ERROR else PrintTag.DUP} Thing {self._name} register success!')
+            self._middleware_name = register_result_msg.middleware_name
+            self._is_registered = True
+            for service in self._function_list + self._value_list:
+                service.set_middleware_name(self._middleware_name)
+                service.set_thing_name(self._name)
+            self._subscribe_service_topic_list()
+            return True
+        elif error == MXErrorCode.FAIL:
+            MXLOG_DEBUG(
+                f'{PrintTag.ERROR} Register failed... Thing {self._name} register packet is not valid. error code: {register_result_msg.error}', 'red')
+            return False
         else:
-            SOPLOG_DEBUG(
-                f'[handle_MT_RESULT_REGISTER] Register failed... error code : {register_result_msg._error}')
+            MXLOG_DEBUG(
+                f'{PrintTag.ERROR} Register failed... Unexpected error occurred!!! error code: {register_result_msg.error}', 'red')
+            return False
 
     def _handle_MT_RESULT_UNREGISTER(self, msg: mqtt.MQTTMessage):
-        unregister_result_msg = SoPUnregisterResultMessage(msg)
-        if not self._name == unregister_result_msg._thing_name:
-            SOPLOG_DEBUG(
-                f'Wrong payload arrive... {self._name} should be arrive, not {unregister_result_msg._thing_name}', 'red')
-            raise
-
-        if self._check_register_result(unregister_result_msg._error):
-            self._registered = False
-            self._unsubscrube_all_topics(self)
+        unregister_result_msg = MXUnregisterResultMessage(msg)
+        if self._name != unregister_result_msg.thing_name:
+            MXLOG_DEBUG(
+                f'[{get_current_function_name()}] Wrong payload arrive... {self._name} should be arrive, not {unregister_result_msg.thing_name}', 'red')
+            # FIXME: False -> ErrorCode
+            return False
+
+        # FIXME: False -> ErrorCode
+        error = unregister_result_msg.error
+        if error in [MXErrorCode.NO_ERROR, MXErrorCode.DUPLICATE]:
+            MXLOG_DEBUG(
+                f'{PrintTag.GOOD if error == MXErrorCode.NO_ERROR else PrintTag.DUP} Thing {self._name} register success!')
+            self._is_registered = False
+            self._unsubscribe_all_topic_list()
+            return True
+        elif error == MXErrorCode.FAIL:
+            MXLOG_DEBUG(
+                f'{PrintTag.ERROR} Unregister failed... Thing {self._name} unregister packet is not valid. error code: {unregister_result_msg.error}', 'red')
+            return False
         else:
-            SOPLOG_DEBUG(
-                f'[handle_MT_RESULT_UNREGISTER] Unregister failed... error code : {unregister_result_msg._error}')
+            MXLOG_DEBUG(
+                f'{PrintTag.ERROR} Unregister failed... Unexpected error occurred!!! error code: {unregister_result_msg.error}', 'red')
+            return False
 
     def _handle_MT_EXECUTE(self, msg: mqtt.MQTTMessage):
-        execute_msg = SoPExecuteMessage(msg)
-        execute_request = SoPExecuteRequest(
-            trigger_msg=execute_msg)
-        execute_request.timer_start()
-
-        # 만약 타켓 함수를 얻는데 성공했다면 병렬실행이 가능한지 옵션을 살펴보고, 이후에 실행 중인지 살펴본다.
-        target_function = self._find_function(execute_msg._function_name)
-        if target_function:
-            if self._is_parallel:
-                target_function.execute(execute_request)
+        execute_msg = MXExecuteMessage(msg)
+        target_function = self._get_function(execute_msg.function_name)
+
+        if not target_function:
+            MXLOG_DEBUG(
+                f'[{get_current_function_name()}] Target function not found! - topic: {decode_MQTT_message(msg)[0]}')
+            return False
+        if self._name != execute_msg.thing_name:
+            MXLOG_DEBUG(
+                f'[{get_current_function_name()}] Wrong payload arrive... {self._name} should be arrive, not {execute_msg.thing_name}', 'red')
+            return False
+        if execute_msg.topic_error or execute_msg.payload_error:
+            MXLOG_DEBUG(
+                f'[{get_current_function_name()}] execute_msg error! - topic: {decode_MQTT_message(msg)[0]}{execute_msg.topic_error}')
+            return False
+
+        # 서로의 arg_list가 일치하는 지 확인한다.
+        if not self._compare_arg_list(target_function.get_arg_list(), list(execute_msg.tuple_arguments())):
+            MXLOG_DEBUG(f'Not matched arg_list', 'red')
+            target_function._send_TM_RESULT_EXECUTE(scenario=execute_msg.scenario,
+                                                    error=MXErrorCode.FAIL,
+                                                    request_ID=execute_msg.request_ID)
+            return False
+
+        # 병렬실행이 가능한지 옵션을 살펴보고, 이후에 실행 중인지 살펴본다.
+        if self._is_parallel:
+            # 중복된 시나리오로부터 온 실행 요청이면 -4 에러코드를 보낸다.
+            if execute_msg.scenario in target_function.get_running_scenario_list():
+                target_function._send_TM_RESULT_EXECUTE(scenario=execute_msg.scenario,
+                                                        error=MXErrorCode.DUPLICATE,
+                                                        request_ID=execute_msg.request_ID)
                 return True
-            else:
-                if not target_function._running:
-                    target_function.execute(execute_request)
-                    return True
-                else:
-                    # TODO: 계속 도는게 아니라 FAILED를 보내야함
-                    while not target_function._running:
-                        SOPLOG_DEBUG(
-                            f'Wait for finish Function {execute_request._trigger_msg._function_name} execute...', 'yellow')
-                        time.sleep(0.1)
-                    target_function.execute(execute_request)
-                    return True
+            execute_thread = target_function.start_execute_thread(execute_msg)
+        elif not target_function._running:
+            execute_thread = target_function.start_execute_thread(execute_msg)
         else:
+            target_function._send_TM_RESULT_EXECUTE(scenario=execute_msg.scenario,
+                                                    error=MXErrorCode.FAIL,
+                                                    request_ID=execute_msg.request_ID)
+            return True
+
+        if not execute_thread:
             return False
+        else:
+            return True
 
     # TODO: complete this function
     def _handle_MT_RESULT_BINARY_VALUE(self, msg: mqtt.MQTTMessage) -> None:
-        SOPLOG_DEBUG(
-            '[handle_mqtt_message] MT_RESULT_BINARY_VALUE is not implemented yet!')
+        execute_msg = MXBinaryValueResultMessage(msg)
+
+        if self._name != execute_msg.thing_name:
+            MXLOG_DEBUG(
+                f'[{get_current_function_name()}] Wrong payload arrive... {self._name} should be arrive, not {execute_msg.thing_name}', 'red')
+            return False
+
+        for value in self._value_list:
+            if value.get_name() == execute_msg.value_name and value.get_type() == MXType.BINARY:
+                value.set_binary_sending(False)
+                return True
+        else:
+            MXLOG_DEBUG(
+                f'[{get_current_function_name()}] Value {execute_msg.value_name} does not exist!!!', 'red')
+            return False
 
     ############################################################################################################
 
     # TODO: implement auto reregister feature
     # for middleware detect and reregister
     # def handle_ME_SERVICE_LIST(self, msg: mqtt.MQTTMessage) -> None:
-    #     service_list_msg = SoPServiceListResultMessage(msg)
+    #     service_list_msg = MXServiceListResultMessage(msg)
 
     #     self.send_TM_REGISTER(self._name, self.dump())
 
     # ===============
     #  _____ ___  ___
     # |_   _||  \/  |
     #   | |  | .  . |
     #   | |  | |\/| |
     #   | |  | |  | |
     #   \_/  \_|  |_/
     # ===============
 
-    def _send_TM_REGISTER(self, thing_name: str, payload: dict) -> None:
-        self._publish_queue.put(SoPRegisterMessage(
-            thing_name, payload).mqtt_message())
-
-    def _send_TM_UNREGISTER(self, thing_name: str):
-        self._publish_queue.put(
-            SoPUnregisterMessage(thing_name).mqtt_message())
-
-    def _send_TM_ALIVE(self, thing_name: str):
-        self._publish_queue.put(SoPAliveMessage(thing_name).mqtt_message())
-
-    def _send_TM_VALUE_PUBLISH(self, thing_name, value_name: str, payload: dict) -> None:
-        self._publish_queue.put(SoPValueMessage(
-            thing_name, value_name, payload).mqtt_message())
-
-    def _send_TM_RESULT_EXECUTE(self, function_name: str, thing_name: str,
-                                return_type: SoPType, return_value: Union[str, float, bool], scenario: str, error: SoPErrorType,
-                                middleware_name: str = '', request_ID: str = '') -> None:
-        self._publish_queue.put(SoPExecuteResultMessage(
-            function_name, thing_name, scenario, return_type, return_value, error, middleware_name=middleware_name, request_ID=request_ID).mqtt_message())
+    def _send_TM_REGISTER(self) -> None:
+        register_msg = self._generate_register_message()
+        if not register_msg:
+            raise Exception('TM_REGISTER packet error')
+
+        register_mqtt_msg = register_msg.mqtt_message()
+        self._publish_queue.put(register_mqtt_msg)
+
+    def _send_TM_UNREGISTER(self):
+        unregister_msg = self._generate_unregister_message()
+        unregister_mqtt_msg = unregister_msg.mqtt_message()
+        self._publish_queue.put(unregister_mqtt_msg)
+
+    def _send_TM_ALIVE(self):
+        alive_msg = self._generate_alive_message()
+        alive_mqtt_msg = alive_msg.mqtt_message()
+        self._publish_queue.put(alive_mqtt_msg)
+
+    def _send_TM_VALUE_PUBLISH(self, value: MXValue) -> None:
+        value_publish_msg = self._generate_value_publish_message(value=value)
+        value_publish_mqtt_msg = value_publish_msg.mqtt_message()
+
+        if value.get_type() == MXType.BINARY:
+            value.set_binary_sending(True)
+        self._publish_queue.put(value_publish_mqtt_msg)
 
     # ========================
     #         _    _  _
     #        | |  (_)| |
     #  _   _ | |_  _ | | ___
     # | | | || __|| || |/ __|
     # | |_| || |_ | || |\__ \
     #  \__,_| \__||_||_||___/
     # ========================
 
-    def _subscribe_init_topics(self, thing: SoPThing):
+    def _generate_thing_id(self, name: str, interface: str = None) -> str:
+        mac_address = get_mac_address(interface=interface)
+
+        if not check_valid_identifier(name):
+            raise MXValueError(
+                f'name cannot be empty & can only contain alphanumeric characters and underscores')
+
+        if not self._append_mac_address:
+            return f'{name}'
+        elif mac_address:
+            return f'{name}_{mac_address}'
+        else:
+            mac = [random.randint(0x00, 0xff) for _ in range(6)]
+            rand_mac_address = ''.join(map(lambda x: "%02x" % x, mac)).upper()
+            return f'{name}_{rand_mac_address}'
+
+    def _generate_register_message(self) -> MXRegisterMessage:
+        if self._is_super:
+            for function in self._function_list:
+                if not hasattr(function, '_sub_service_request_list'):
+                    return False
+        else:
+            for function in self._function_list:
+                if hasattr(function, '_sub_service_request_list'):
+                    return False
+
+        for function in self._function_list:
+            for arg in function.get_arg_list():
+                bound = arg.get_bound()
+                if not arg._name:
+                    return False
+                if bound[1] - bound[0] <= 0:
+                    return False
+
+        for value in self._value_list:
+            bound = value.get_bound()
+            if bound[1] - bound[0] <= 0:
+                return False
+
+        register_msg = MXRegisterMessage(thing=self)
+        return register_msg
+
+    def _generate_unregister_message(self) -> MXUnregisterMessage:
+        return MXUnregisterMessage(thing=self)
+
+    def _generate_alive_message(self) -> MXAliveMessage:
+        return MXAliveMessage(thing=self)
+
+    def _generate_value_publish_message(self, value: MXValue) -> MXValuePublishMessage:
+        return MXValuePublishMessage(thing=self, value=value)
+
+    # need for middleware detect
+    def _generate_client_refresh_message(self) -> MXClientRefreshMessage:
+        return MXClientRefreshMessage(thing=self)
+
+    def _subscribe_init_topic_list(self):
         topic_list = [
-            SoPProtocolType.Base.MT_RESULT_REGISTER.value % thing.get_name(),
-            SoPProtocolType.Base.MT_RESULT_UNREGISTER.value % thing.get_name(),
-            SoPProtocolType.Base.MT_RESULT_BINARY_VALUE.value % thing.get_name()]
+            MXProtocolType.Base.MT_RESULT_REGISTER.value % self._name,
+            MXProtocolType.Base.MT_RESULT_UNREGISTER.value % self._name,
+            MXProtocolType.Base.MT_RESULT_BINARY_VALUE.value % self._name]
 
         # TODO: implement auto reregister feature
         # for middleware detect
         # topic_list.append(
-        #     SoPProtocolType.WebClient.ME_RESULT_SERVICE_LIST.value % ('#'))
+        #     MXProtocolType.WebClient.ME_RESULT_SERVICE_LIST.value % ('#'))
 
         for topic in topic_list:
-            self._subscribe(topic, thing=thing)
+            self._subscribe(topic)
 
-    def _subscribe_service_topics(self, thing: SoPThing):
+    def _subscribe_service_topic_list(self):
         topic_list = []
 
-        for function in thing.get_function_list():
-            topic_list += [SoPProtocolType.Base.MT_EXECUTE.value % (function.get_name(), thing.get_name(), '+', '#'),
-                           (SoPProtocolType.Base.MT_EXECUTE.value % (function.get_name(), thing.get_name(), '', '')).rstrip('/')]
+        for function in self._function_list:
+            topic_list += [MXProtocolType.Base.MT_EXECUTE.value % (function.get_name(), self._name, '+', '#'),
+                           (MXProtocolType.Base.MT_EXECUTE.value % (function.get_name(), self._name, '', '')).rstrip('/')]
 
         for topic in topic_list:
-            self._subscribe(topic, thing=thing)
+            self._subscribe(topic)
 
-    def _unsubscrube_all_topics(self, thing: SoPThing):
+    def _unsubscribe_all_topic_list(self):
         # whenever _unsubscribe function execute, it remove target topic from self._subscribed_topic_set
         # so it need to iterate with copy of self._subscribed_topic_set
-        target_topic_list = list(thing.get_subscribed_topic_set())
+        target_topic_list = list(self._subscribed_topic_set)
         for topic in target_topic_list:
-            self._unsubscribe(topic, thing=thing)
+            self._unsubscribe(topic)
 
-    def _check_register_result(self, error: SoPErrorType, thing: SoPThing = None):
-        if not isinstance(error, SoPErrorType):
-            error = SoPErrorType.get(error)
-        if not thing:
-            thing = self
-
-        if error == SoPErrorType.NO_ERROR:
-            SOPLOG_DEBUG(
-                f'{PrintTag.GOOD} Thing {thing.get_name()} register success!')
+    # FIXME: This method will be deprecated. Remove after ManagerThing fixed
+    def _check_register_result(self, error: MXErrorCode):
+        if not isinstance(error, MXErrorCode):
+            error = MXErrorCode.get(error)
+
+        if error == MXErrorCode.NO_ERROR:
+            MXLOG_DEBUG(
+                f'{PrintTag.GOOD} Thing {self._name} register success!')
             return True
-        elif error == SoPErrorType.DUPLICATE:
-            SOPLOG_DEBUG(
-                f'{PrintTag.DUP} Thing {thing.get_name()} register success!')
+        elif error == MXErrorCode.DUPLICATE:
+            MXLOG_DEBUG(f'{PrintTag.DUP} Thing {self._name} register success!')
             return True
-        elif error == SoPErrorType.FAIL:
-            SOPLOG_DEBUG(
-                f'{PrintTag.ERROR} Thing {thing.get_name()} register packset was nonvaild')
+        elif error == MXErrorCode.FAIL:
+            MXLOG_DEBUG(
+                f'{PrintTag.ERROR} Thing {self._name} register packet is not vaild')
             return False
         else:
-            SOPLOG_DEBUG(
-                f'[MT_message_parser] Unexpected error occured!!!', 'red')
+            MXLOG_DEBUG(
+                f'[{get_current_function_name()}] Unexpected error occured!!!', 'red')
             return False
 
-    def _print_packet(self, msg: mqtt.MQTTMessage, mode: SoPPrintMode = SoPPrintMode.FULL):
+    # FIXME: This method will be deprecated. Remove after ManagerThing fixed
+    def _check_unregister_result(self, error: MXErrorCode):
+        if not isinstance(error, MXErrorCode):
+            error = MXErrorCode.get(error)
+
+        if error == MXErrorCode.NO_ERROR:
+            MXLOG_DEBUG(
+                f'{PrintTag.GOOD} Thing {self._name} unregister success!')
+            return True
+        elif error == MXErrorCode.FAIL:
+            MXLOG_DEBUG(
+                f'{PrintTag.ERROR} Thing {self._name} unregister packet is not vaild')
+            return False
+        else:
+            MXLOG_DEBUG(
+                f'[{get_current_function_name()}] Unexpected error occured!!!', 'red')
+            return False
 
-        def mode_select(mode: SoPPrintMode, payload: str):
-            if mode == SoPPrintMode.SKIP:
-                return colored(f'skip... (print_packet mode={mode})', 'yellow'), payload
-            elif mode == SoPPrintMode.ABBR:
-                payload_raw = payload
-                if payload.count('\n') > 10:
-                    payload = '\n'.join(payload.split('\n')[:10]) + '\n' + \
-                        colored(
-                            f'skip... (print_packet mode={mode})', 'yellow')
-                    return payload, payload_raw
-                elif len(payload) > 1000:
-                    payload = payload[:1000] + '\n' + \
-                        colored(
-                            f'skip... (print_packet mode={mode})', 'yellow')
-                    return payload, payload_raw
-                else:
-                    return payload, payload_raw
-            elif mode == SoPPrintMode.FULL:
-                return payload, payload
-            else:
-                SOPLOG_DEBUG(
-                    f'[print_packet] Unknown mode!!! mode should be [skip|abbr|full] mode : {mode}', 'red')
+    def _convert_arg_list(self, arg_list: List[Union[MXArgument, Union[int, float, str, bool]]]) -> List[MXType]:
+        if isinstance(arg_list, list) and all([isinstance(arg, (int, float, str, bool)) for arg in arg_list]):
+            arg_type_list = []
+            for arg in arg_list:
+                # if is_base64(arg):
+                #     arg_type_list.append(MXType.BINARY)
+                # else:
+                #     arg_type_list.append(MXType.get(type(arg)))
+                arg_type_list.append(MXType.get(type(arg)))
+        elif isinstance(arg_list, list) and all([isinstance(arg, MXArgument) for arg in arg_list]):
+            arg_type_list = [arg.get_type() for arg in arg_list]
+        else:
+            raise MXTypeError(
+                f'arg_list must be list of MXArgument or list of int, float, str, bool: {arg_list}')
 
-        def print_result_topic(topic, payload):
-            topic_str = topic_join(topic)
-            topic_indicator = f'{topic[0]}_{topic[1]}_{topic[2]}'
+        return arg_type_list
 
-            payload, payload_raw = mode_select(mode, payload)
-            payload = colored(payload, attrs=['bold'])
+    def _compare_arg_list(self, arg_list1: List[Union[MXArgument, Union[int, float, str, bool]]], arg_list2: List[Union[MXArgument, Union[int, float, str, bool]]]):
+        arg_type_list1 = self._convert_arg_list(arg_list1)
+        arg_type_list2 = self._convert_arg_list(arg_list2)
 
-            SOPLOG_DEBUG(
-                f'[{topic_indicator:20}] topic : {topic_str} payload : {payload}')
+        if len(arg_type_list1) != len(arg_type_list2):
+            MXLOG_DEBUG(f'Not matched arg_list length: {len(arg_type_list1)} != {len(arg_type_list2)}', 'red')
+            return False
 
-        def print_topic(topic, payload):
-            topic_str = topic_join(topic)
-            topic_indicator = f'{topic[0]}_{topic[1]}'
+        for arg_type1, arg_type2 in zip(arg_type_list1, arg_type_list2):
+            if arg_type1 in [MXType.INTEGER, MXType.DOUBLE] and arg_type2 in [MXType.INTEGER, MXType.DOUBLE]:
+                pass
+            elif arg_type1 != arg_type2:
+                MXLOG_DEBUG(f'Not matched arg_list type: {arg_type1} != {arg_type2}', 'red')
+                return False
+        else:
+            return True
 
-            payload, payload_raw = mode_select(mode, payload)
-            payload = colored(payload, attrs=['bold'])
+    def _print_packet(self, topic: str, payload: str, direction: Direction, mode: MXPrintMode = MXPrintMode.FULL, pretty: bool = False) -> str:
 
-            SOPLOG_DEBUG(
-                f'[{topic_indicator:20}] topic : {topic_str} payload : {payload}')
+        def prune_payload(payload: str, mode: MXPrintMode) -> str:
+            if mode == MXPrintMode.SKIP:
+                payload = colored(f'skip... (print_packet mode={mode})', 'yellow')
+            elif mode == MXPrintMode.ABBR:
+                if payload.count('\n') > 10:
+                    payload = '\n'.join(payload.split('\n')[:10]) + '\n' + colored(f'skip... (print_packet mode={mode})', 'yellow')
+                elif len(payload) > 1000:
+                    payload = payload[:1000] + '\n' + colored(f'skip... (print_packet mode={mode})', 'yellow')
+                else:
+                    pass
+            elif mode == MXPrintMode.FULL:
+                pass
+            else:
+                raise Exception(f'[print_packet] Unknown mode!!! mode should be [skip|abbr|full] mode : {mode}', 'red')
 
-        topic, payload, timestamp = decode_MQTT_message(msg, str)
-        topic = topic_split(topic)
+            return payload
 
-        payload = dict_to_json_string(payload)
+        topic_template = MXProtocolType.get(topic)
+        if not topic_template:
+            MXLOG_DEBUG(f'[print_packet] Unknown topic!!! topic : {topic}')
 
-        if topic[0] == 'MT':
-            if topic[1] == 'RESULT':
-                if topic[2] in ['REGISTER', 'UNREGISTER', 'BINARY_VALUE']:
-                    print_result_topic(topic, payload)
-                else:
-                    SOPLOG_DEBUG(
-                        f'[print_packet] Unknown {topic[0]}_{topic[1]} Topic!!!', 'red')
-            else:
-                if topic[1] in ['EXECUTE']:
-                    print_topic(topic, payload)
-                else:
-                    SOPLOG_DEBUG(
-                        f'[print_packet] Unknown {topic[0]} Topic!!!', 'red')
-        elif topic[0] == 'TM':
-            if topic[1] == 'RESULT':
-                if topic[2] in ['EXECUTE']:
-                    print_result_topic(topic, payload)
-                else:
-                    SOPLOG_DEBUG(
-                        f'[print_packet] Unknown {topic[0]}_{topic[1]} Topic!!!', 'red')
-            else:
-                if topic[1] in ['REGISTER', 'UNREGISTER', 'ALIVE', 'VALUE_PUBLISH']:
-                    print_topic(topic, payload)
-                else:
-                    SOPLOG_DEBUG(
-                        f'[print_packet] Unknown {topic[0]} Topic!!!', 'red')
-        elif topic[0] == 'MS':
-            if topic[1] == 'RESULT':
-                if topic[2] in ['SCHEDULE', 'EXECUTE', 'SERVICE_LIST']:
-                    print_result_topic(topic, payload)
-                else:
-                    SOPLOG_DEBUG(
-                        f'[print_packet] Unknown {topic[0]}_{topic[1]} Topic!!!', 'red')
-            else:
-                if topic[1] in ['SCHEDULE', 'EXECUTE']:
-                    print_topic(topic, payload)
-                else:
-                    SOPLOG_DEBUG(
-                        f'[print_packet] Unknown {topic[0]} Topic!!!', 'red')
-        elif topic[0] == 'SM':
-            if topic[1] == 'RESULT':
-                if topic[2] in ['SCHEDULE', 'EXECUTE']:
-                    print_result_topic(topic, payload)
-                else:
-                    SOPLOG_DEBUG(
-                        f'[print_packet] Unknown {topic[0]}_{topic[1]} Topic!!!', 'red')
-            else:
-                if topic[1] in ['SCHEDULE', 'EXECUTE', 'AVAILABILITY', 'REFRESH']:
-                    print_topic(topic, payload)
-                else:
-                    SOPLOG_DEBUG(
-                        f'[print_packet] Unknown {topic[0]} Topic!!!', 'red')
-        elif topic[0] == 'ME':
-            if topic[1] == 'NOTIFY_CHANGE':
-                print_topic(topic, payload)
-            else:
-                SOPLOG_DEBUG(
-                    f'[print_packet] Unknown {topic[0]} Topic!!!', 'red')
-        elif topic[0] == self._name:
-            if topic[1] in [value.get_name() for value in self._value_list]:
-                print_topic(topic, payload)
-            else:
-                SOPLOG_DEBUG(
-                    f'[print_packet] Unknown VALUE PUBLISH Topic!!!, topic : {topic}', 'red')
-        else:
-            topic = topic_join(topic)
-            SOPLOG_DEBUG(
-                f'[print_packet] Unexpected topic!!! : {topic} ', 'red')
+        topic_indicator = '_'.join([topic_token for topic_token in topic_template.value.split('/') if topic_token != '%s'])
+        payload = prune_payload(payload=dict_to_json_string(dict_object=payload, pretty=pretty), mode=mode)
+
+        MXLOG_DEBUG(f'[{topic_indicator:20}][{direction.value}] topic: {topic} payload: {payload}')
 
     # MQTT utils
     # ========================
     #         _    _  _
     #        | |  (_)| |
     #  _   _ | |_  _ | | ___
     # | | | || __|| || |/ __|
     # | |_| || |_ | || |\__ \
     #  \__,_| \__||_||_||___/
     # ========================
 
-    def _connect(self):
+    def _connect(self, ip: str, port: int):
         self._mqtt_client.on_connect = self._on_connect
         self._mqtt_client.on_disconnect = self._on_disconnect
         self._mqtt_client.on_publish = self._on_publish
         self._mqtt_client.on_subscribe = self._on_subscribe
         self._mqtt_client.on_unsubscribe = self._on_unsubscribe
         self._mqtt_client.on_message = self._on_message
 
-        self._mqtt_client.connect(self._ip, self._port)
+        self._mqtt_client.connect(ip, port)
         self._mqtt_client.loop_start()
 
     def _disconnect(self):
         self._mqtt_client.loop_stop()
         ret = self._mqtt_client.disconnect()
 
-        SOPLOG_DEBUG(
-            f'{PrintTag.DISCONNECT} disconnect from Host: {self._ip}:{self._port}', 'red')
-
-    def _subscribe(self, topic: str, qos: int = 2, thing: SoPThing = None):
+    def _subscribe(self, topic: str, qos: int = 0):
         if topic not in self._subscribed_topic_set:
             ret = self._mqtt_client.subscribe(topic, qos=qos)
             if not ret[0] == 0:
-                SOPLOG_DEBUG(
-                    f'{PrintTag.SUBSCRIBE} subscribe failed!!!', 'red')
+                MXLOG_DEBUG(f'{PrintTag.SUBSCRIBE} subscribe failed!!!', 'red')
                 return False
-            if not thing:
-                self.get_subscribed_topic_set().add(topic)
-            else:
-                thing.get_subscribed_topic_set().add(topic)
+            self._subscribed_topic_set.add(topic)
 
-        SOPLOG_DEBUG(f'{PrintTag.SUBSCRIBE} {topic}')
+        MXLOG_DEBUG(f'{PrintTag.SUBSCRIBE} {topic}')
         return True
 
-    def _unsubscribe(self, topic: str, thing: SoPThing = None):
+    def _unsubscribe(self, topic: str):
         if topic in self._subscribed_topic_set:
             ret = self._mqtt_client.unsubscribe(topic)
             if not ret[0] == 0:
-                SOPLOG_DEBUG(
-                    f'{PrintTag.UNSUBSCRIBE} unsubscribe failed!!!', 'red')
+                MXLOG_DEBUG(f'{PrintTag.UNSUBSCRIBE} unsubscribe failed!!!', 'red')
                 return False
-            if not thing:
-                self.get_subscribed_topic_set().add(topic)
-            else:
-                thing.get_subscribed_topic_set().add(topic)
 
-        SOPLOG_DEBUG(f'{PrintTag.UNSUBSCRIBE} {topic}')
+            self._subscribed_topic_set.add(topic)
+
+        MXLOG_DEBUG(f'{PrintTag.UNSUBSCRIBE} {topic}')
         return True
 
-    def _publish(self, topic: str, payload, qos: int = 2):
-        cnt = 3
-        send_time = 0
+    def _publish(self, topic: str, payload, qos: int = 0):
+        cnt = 1
+        # send_time = 0
         while cnt:
+            self._print_packet(topic=topic, payload=payload, direction=Direction.PUBLISH, mode=self._log_mode)
             ret = self._mqtt_client.publish(topic, payload, qos=qos)
             if ret.rc != 0:
-                SOPLOG_DEBUG('Publish failed!!!', 'red')
-                SOPLOG_DEBUG(f'Topic : {topic}', 'red')
-                SOPLOG_DEBUG(f'Payload : {payload}', 'red')
-                SOPLOG_DEBUG(f'Retry {4-cnt}', 'red')
+                MXLOG_DEBUG('Publish failed!!!', 'red')
+                MXLOG_DEBUG(f'Topic : {topic}', 'red')
+                MXLOG_DEBUG(f'Payload : {payload}', 'red')
+                MXLOG_DEBUG(f'Retry {4-cnt}', 'red')
                 cnt -= 1
                 time.sleep(0.2)
             else:
-                send_time = time.time()
+                # send_time = time.time()
                 break
         else:
-            SOPLOG_DEBUG(
-                'Publish mqtt is not work... exit program', 'red')
+            MXLOG_DEBUG('Publish mqtt is not work... exit program', 'red')
             self._publish_queue.queue.clear()
             # self.wrapup()
 
-        msg = encode_MQTT_message(topic, payload, send_time)
-        self._print_packet(msg, mode=self._log_mode)
-
-    # Avahi feature (WARNING: not work on python3.6<)
-    def _avahi_discover(self, MQTT_SOPIOT_AVAHI_LIST=["_mqtt_sopiot._tcp.local.", "_mqtt_ssl_sopiot._tcp.local."]):
-
-        def on_service_state_change(zeroconf: Zeroconf, service_type: str, name: str, state_change: ServiceStateChange) -> None:
-            # SOPLOG_DEBUG(
-            #     f"Service {name} of type {service_type} state changed: {state_change}")
-
-            if state_change is ServiceStateChange.Added:
-                info = zeroconf.get_service_info(
-                    service_type, name)
-                # SOPLOG_DEBUG("Info from zeroconf.get_service_info: %r" % (info))
-
-                if info:
-                    addresses = ["%s:%d" % (addr, cast(int, info.port))
-                                 for addr in info.parsed_scoped_addresses()]
-                    ipv4_address = addresses[0]
-                    ipv6_address = addresses[1]
-                    ip = ipv4_address.split(':')[0]
-                    port = int(ipv4_address.split(':')[1])
-
-                    discovered_middleware = {
-                        'ip': ip,
-                        'port': port,
-                        'name': info.server,
-                    }
-
-                    SOPLOG_DEBUG(f"Server name: {info.server}")
-                    SOPLOG_DEBUG(f"Address: {ip}")
-                    SOPLOG_DEBUG(
-                        f"Weight: {info.weight}, priority: {info.priority}")
-                    if info.properties:
-                        for key, value in info.properties.items():
-                            SOPLOG_DEBUG(
-                                f"Properties -> {key.decode('utf-8')}: {value.decode('utf-8')}")
-                    else:
-                        SOPLOG_DEBUG("No properties", 'yellow')
-
-                    self._avahi_discovered_middleware_list.append(
-                        discovered_middleware)
-                    self._avahi_middleware_name = info.server
-                else:
-                    SOPLOG_DEBUG("No info")
-
-        zeroconf = Zeroconf(ip_version=IPVersion.V4Only)
-        services = MQTT_SOPIOT_AVAHI_LIST
-        # services = list(ZeroconfServiceTypes.find(zc=zeroconf))
-        browser = ServiceBrowser(zeroconf, services, handlers=[
-                                 on_service_state_change])
-        time.sleep(3)
-        browser.cancel()
-        zeroconf.close()
+    def _init_logger(self):
+        if self._log_enable:
+            START_LOGGER(whole_log_path=self._log_name,
+                         logging_mode=MXLogger.LoggingMode.ALL)
+        else:
+            START_LOGGER(logging_mode=MXLogger.LoggingMode.OFF)
 
     def _set_ssl_config(self):
-        SOPLOG_DEBUG('SSL enabled...')
         try:
             self._mqtt_client.tls_set(
                 ca_certs=f'{self._ssl_ca_path}/ca.crt',
                 certfile=f'{self._ssl_ca_path}/client.crt',
                 keyfile=f'{self._ssl_ca_path}/client.key',
                 cert_reqs=ssl.CERT_REQUIRED,
-                tls_version=ssl.PROTOCOL_TLSv1_2,
-                ciphers=None)
+                tls_version=ssl.PROTOCOL_TLS_CLIENT)
             self._mqtt_client.tls_insecure_set(True)
         except ValueError as e:
-            SOPLOG_DEBUG('SSL/TLS has already been configured.', 'yellow')
+            MXLOG_DEBUG('SSL/TLS has already been configured.', 'yellow')
 
-    def _avahi_init(self, avahi_enable):
+    def _check_valid_middleware(self, device_list: List[dict]):
+        valid_middleware_list = []
+        for device in device_list:
+            host = device['host']
+            port = device['port']
+            try:
+                ack_topic = MXProtocolType.WebClient.ME_RESULT_SERVICE_LIST.value % (
+                    self._name)
+
+                test_mqtt_client = MXClient(client_id=self._name)
+                test_mqtt_client.on_message = self._on_message
+                # ssl 연결의 경우 ssl 연결을 미리 설정 후 연결해야한다.
+                # 그런데 ssl 연결인지 아닌지 판단을 어떻게 해야할지?
+                rc = test_mqtt_client.connect(host, port)
+                test_mqtt_client.loop_start()
+
+                test_mqtt_client.subscribe(ack_topic)
+                refresh_msg = self._generate_client_refresh_message()
+                test_mqtt_client.publish(
+                    refresh_msg.topic, refresh_msg.payload)
+
+                self._receive_queue.get(timeout=0.5)
+                valid_middleware_list.append(device)
+                MXLOG_DEBUG(f'valid middleware on {host}:{port}', 'green')
+            except Empty:
+                MXLOG_DEBUG(
+                    f'Not valid middleware on {host}:{port}', 'yellow')
+            except ConnectionRefusedError:
+                MXLOG_DEBUG(
+                    f'No middleware on {host}:{port}', 'yellow')
+
+            test_mqtt_client.unsubscribe(ack_topic)
+            test_mqtt_client.loop_stop()
+            test_mqtt_client.disconnect()
+            del test_mqtt_client
+
+        return valid_middleware_list
+
+    def _discover_middleware(self, timeout: float = 10) -> List[dict]:
+        discovered_device_list = []
+        # FIXME: rename to sopiot -> mxiot
+        service_type_list = ['_mqtt_sopiot._tcp.local.',
+                             '_mqtt_ssl_sopiot._tcp.local.']
 
-        def save_middleware_info():
-            middleware_info = {
-                "middleware_list": [
-                    {
-                        "name": self._avahi_middleware_name,
-                        "ip": self._ip,
-                        "port": self._port,
-                        "lastest_connect_time": time.time()
-                    }
-                ]
-            }
-            json_file_write('middleware_info.json',
-                            middleware_info)
-
-        def set_connect_info(selected_middleware: dict):
-            self._ip = selected_middleware['ip']
-            self._port = selected_middleware['port']
-
-        if avahi_enable:
-            if sys.version_info[0] <= 3 and sys.version_info[1] < 6:
-                raise Exception(
-                    'Avahi feature is not supported on python3.6<. try python3.7 or higher. or disable avahi feature. (avahi_enable=False)')
-
-            self._avahi_discover(MQTT_SOPIOT_AVAHI_LIST=[
-                "_mqtt_sopiot._tcp.local.",
-                "_mqtt_ssl_sopiot._tcp.local."])
-            if len(self._avahi_discovered_middleware_list) > 1:
-                SOPLOG_DEBUG('More than 2 avahi_enable host searched...')
-                middleware_info = json_file_read('middleware_info.json')
-
-                if middleware_info:
-                    middleware_list = sorted(
-                        middleware_info['middleware_list'], key=lambda x: x['lastest_connect_time'])
-                    set_connect_info(middleware_list[0])
-                    SOPLOG_DEBUG(
-                        'Connect to lastest connected middleware...')
-                else:
-                    SOPLOG_DEBUG('middleware_info.json is empty...:')
-                    for i, discovered_middleware in enumerate(self._avahi_discovered_middleware_list):
-                        ip = discovered_middleware['ip']
-                        port = discovered_middleware['port']
-                        middleware_name = discovered_middleware['name']
-                        SOPLOG_DEBUG(
-                            f'{i}: {ip}:{port} ({middleware_name})')
-                    while True:
-                        user_input = int(input('select middleware : '))
-                        if user_input not in range(len(self._avahi_discovered_middleware_list)):
-                            SOPLOG_DEBUG(
-                                'Invalid input...', 'red')
-                        else:
-                            break
-                    set_connect_info(
-                        self._avahi_discovered_middleware_list[user_input])
-                    save_middleware_info()
-
-                if self._ssl_enable == True:
-                    self._set_ssl_config()
-                elif self._port == 8883:
-                    self._set_ssl_config()
+        def on_service_state_change(zeroconf: Zeroconf, service_type: str, name: str, state_change: ServiceStateChange) -> None:
+            if state_change is ServiceStateChange.Added:
+                info = zeroconf.get_service_info(service_type, name)
+
+                if not info:
+                    MXLOG_DEBUG('No info')
+                    return
+
+                parsed_address_info_list = info.parsed_scoped_addresses()
+                if not parsed_address_info_list:
+                    MXLOG_DEBUG('No address info')
+                    return
+
+                addresses = [
+                    f'{address_info}:{cast(int, info.port)}' for address_info in parsed_address_info_list]
+                ipv4_address = addresses[0].split(':')[0]
+                # ipv6_address = addresses[1]
+                port = int(addresses[0].split(':')[1])
+
+                discovered_device_info = dict(
+                    name=info.server, host=ipv4_address, port=port)
+
+                MXLOG_DEBUG(f'Server name: {info.server}')
+                MXLOG_DEBUG(f'Address: {ipv4_address}')
+                MXLOG_DEBUG(
+                    f'Weight: {info.weight}, priority: {info.priority}')
+                if info.properties:
+                    for key, value in info.properties.items():
+                        MXLOG_DEBUG(
+                            f'Properties -> {key.decode("utf-8")}: {value.decode("utf-8")}')
                 else:
-                    SOPLOG_DEBUG('SSL is not enabled...')
+                    MXLOG_DEBUG('No properties', 'yellow')
+
+                discovered_device_list.append(
+                    discovered_device_info)
+
+        zeroconf = Zeroconf(ip_version=IPVersion.V4Only)
+        browser = ServiceBrowser(zeroconf, service_type_list, handlers=[
+            on_service_state_change], delay=0.1)
+
+        time.sleep(timeout)
+        browser.cancel()
+        zeroconf.close()
 
-            elif len(self._avahi_discovered_middleware_list) == 1:
-                set_connect_info(self._avahi_discovered_middleware_list[0])
-                save_middleware_info()
+        # Check middleware validity
+        valid_middleware_list = self._check_valid_middleware(
+            discovered_device_list)
+        return valid_middleware_list
+
+    def _auto_setup_middleware(self, timeout: float = 10) -> List[dict]:
+
+        def save_middleware_info(discovered_middleware_list: List[dict]):
+            middleware_info = dict(middleware_list=[dict(**middleware, lastest_connect_time=get_current_time())
+                                                    for middleware in discovered_middleware_list])
+            json_file_write(
+                f'/tmp/middleware_info-{self._name}.json', middleware_info)
+
+        discovered_middleware_list = self._discover_middleware(timeout=timeout)
+        if len(discovered_middleware_list) > 1:
+            MXLOG_DEBUG('More than 2 middleware searched...')
+            middleware_info = json_file_read(
+                f'/tmp/middleware_info-{self._name}.json')
+
+            if middleware_info:
+                middleware_list = sorted(
+                    middleware_info['middleware_list'], key=lambda x: x['lastest_connect_time'])
+                self._ip = middleware_list[0]['host']
+                self._port = middleware_list[0]['port']
+                MXLOG_DEBUG(
+                    'Connect to lastest connected middleware...')
+                return True
             else:
-                SOPLOG_DEBUG(
-                    'avahi_enable search failed... connect to default ip...')
+                MXLOG_DEBUG(
+                    f'/tmp/middleware_info-{self._name}.json does not exist...', 'yellow')
+                for i, discovered_middleware in enumerate(discovered_middleware_list):
+                    host = discovered_middleware['host']
+                    port = discovered_middleware['port']
+                    middleware_name = discovered_middleware['name']
+                    MXLOG_DEBUG(
+                        f'{i}: {host}:{port} ({middleware_name})')
+                while True:
+                    user_input = int(input('select middleware : '))
+                    if user_input not in range(len(discovered_middleware_list)):
+                        MXLOG_DEBUG(
+                            'Invalid input...', 'red')
+                    else:
+                        break
+                self._ip = discovered_middleware_list[user_input]['host']
+                self._port = discovered_middleware_list[user_input]['port']
+                save_middleware_info(discovered_middleware_list)
+                return True
+        elif len(discovered_middleware_list) == 1:
+            self._ip = discovered_middleware_list[0]['host']
+            self._port = discovered_middleware_list[0]['port']
+            save_middleware_info(discovered_middleware_list)
+            return True
         else:
-            SOPLOG_DEBUG('Skip avahi_enable search...')
+            MXLOG_DEBUG(
+                'Middleware discover failed... connect to default middleware...', 'red')
+            return False
+
+    def _update_thing_ID(self, name: str, interface: str = None) -> None:
+        self._name = self._generate_thing_id(name, interface=interface)
+
 
 # ===================================================================================
 # ___  ___ _____  _____  _____   _____         _  _  _                   _
 # |  \/  ||  _  ||_   _||_   _| /  __ \       | || || |                 | |
 # | .  . || | | |  | |    | |   | /  \/  __ _ | || || |__    __ _   ___ | | __ ___
 # | |\/| || | | |  | |    | |   | |     / _` || || || '_ \  / _` | / __|| |/ // __|
 # | |  | |\ \/' /  | |    | |   | \__/\| (_| || || || |_) || (_| || (__ |   < \__ \
 # \_|  |_/ \_/\_\  \_/    \_/    \____/ \__,_||_||_||_.__/  \__,_| \___||_|\_\|___/
 # ===================================================================================
 
     # for MQTT version<5.0
-    def _on_connect(self, client: SoPClient, userdata, flags, result):
+
+
+    def _on_connect(self, client: MXClient, userdata, flags, result):
         if result == 0:
             self._connected = True
-            SOPLOG_DEBUG(
+            MXLOG_DEBUG(
                 f'{PrintTag.CONNECT} Connect to Host: {self._ip}:{self._port}')
             # TODO: implement auto reregister feature
-            if self._registered:
+            if self._is_registered:
                 pass
         else:
-            SOPLOG_DEBUG(
+            MXLOG_DEBUG(
                 f'{PrintTag.ERROR} Bad connection... Returned code: {result}', 'red')
 
-    def _on_disconnect(self, client: SoPClient, userdata, rc):
+    def _on_disconnect(self, client: MXClient, userdata, rc):
         if rc == 0:
             self._connected = False
-            SOPLOG_DEBUG(
+            MXLOG_DEBUG(
                 f'{PrintTag.DISCONNECT} Disconnect from Host: {self._ip}:{self._port}')
         else:
-            SOPLOG_DEBUG(
+            MXLOG_DEBUG(
                 f'{PrintTag.ERROR} Bad disconnection... Returned code: {rc}', 'red')
 
-    def _on_subscribe(self, client: SoPClient, userdata: str, mid, granted_qos):
+    def _on_subscribe(self, client: MXClient, userdata: str, mid, granted_qos):
         pass
 
-    def _on_unsubscribe(self, client: SoPClient, userdata: str, mid):
+    def _on_unsubscribe(self, client: MXClient, userdata: str, mid):
         pass
 
-    def _on_publish(self, client: SoPClient, userdata: mqtt.MQTTMessage, mid):
+    def _on_publish(self, client: MXClient, userdata: mqtt.MQTTMessage, mid):
         pass
 
-    def _on_message(self, client: SoPClient, userdata: Callable, msg: mqtt.MQTTMessage):
-        self._print_packet(msg, mode=self._log_mode)
+    def _on_message(self, client: MXClient, userdata: Callable, msg: mqtt.MQTTMessage):
+        topic, payload, _ = decode_MQTT_message(msg)
+        self._print_packet(topic=topic, payload=payload, direction=Direction.RECEIVED, mode=self._log_mode)
         self._receive_queue.put(msg)
 
     # TODO: test this functions
     # for MQTT version>=5.0
-    def _on_connect_v5(self, client: SoPClient, userdata, flags, reason, properties):
+    def _on_connect_v5(self, client: MXClient, userdata, flags, reason, properties):
         if reason == 0:
             self._connected = True
-            SOPLOG_DEBUG(
+            MXLOG_DEBUG(
                 f'{PrintTag.CONNECT} Connect to Host: {self._ip}:{self._port}')
             # TODO: implement auto reregister feature
-            if self._registered:
+            if self._is_registered:
                 pass
         else:
-            SOPLOG_DEBUG(
+            MXLOG_DEBUG(
                 f'{PrintTag.ERROR} Bad connection... Returned code: {reason}', 'red')
 
-    def _on_disconnect_v5(self, client: SoPClient, userdata, rc, properties):
+    def _on_disconnect_v5(self, client: MXClient, userdata, rc, properties):
         if rc == 0:
             self._connected = False
-            SOPLOG_DEBUG(
+            MXLOG_DEBUG(
                 f'{PrintTag.DISCONNECT} Disconnect from Host: {self._ip}:{self._port}')
         else:
-            SOPLOG_DEBUG(
+            MXLOG_DEBUG(
                 f'{PrintTag.ERROR} Bad disconnection... Returned code: {rc}', 'red')
 
-    def _on_subscribe_v5(self, client: SoPClient, userdata: str, mid, reasoncodes, properties):
+    def _on_subscribe_v5(self, client: MXClient, userdata: str, mid, reasoncodes, properties):
         pass
 
-    def _on_unsubscribe_v5(self, client: SoPClient, userdata: str, mid,  properties, reasoncodes):
+    def _on_unsubscribe_v5(self, client: MXClient, userdata: str, mid,  properties, reasoncodes):
         pass
 
-    def _on_publish_v5(self, client: SoPClient, userdata: mqtt.MQTTMessage, mid):
+    def _on_publish_v5(self, client: MXClient, userdata: mqtt.MQTTMessage, mid):
         pass
 
-    def _on_message_v5(self, client: SoPClient, userdata: Callable, msg: mqtt.MQTTMessage):
-        self._print_packet(msg, mode=self._log_mode)
+    def _on_message_v5(self, client: MXClient, userdata: Callable, msg: mqtt.MQTTMessage):
+        topic, payload, _ = decode_MQTT_message(msg)
+        self._print_packet(topic=topic, payload=payload, direction=Direction.RECEIVED, mode=self._log_mode)
         self._receive_queue.put(msg)
 
     # ====================================
     #               _    _
     #              | |  | |
     #   __ _   ___ | |_ | |_   ___  _ __
     #  / _` | / _ \| __|| __| / _ \| '__|
     # | (_| ||  __/| |_ | |_ |  __/| |
     #  \__, | \___| \__| \__| \___||_|
     #   __/ |
     #  |___/
     # ====================================
 
+    def get_log_mode(self) -> MXPrintMode:
+        return self._log_mode
+
+    def get_log_enable(self) -> bool:
+        return self._log_enable
+
+    def get_log_name(self) -> str:
+        return self._log_enable
+
+    def get_ip(self) -> str:
+        return self._ip
+
+    def get_port(self) -> int:
+        return self._port
+
+    def get_ssl_ca_path(self) -> str:
+        return self._ssl_ca_path
+
+    def get_ssl_enable(self) -> bool:
+        return self._ssl_enable
+
     # ==================================
     #             _    _
     #            | |  | |
     #  ___   ___ | |_ | |_   ___  _ __
     # / __| / _ \| __|| __| / _ \| '__|
     # \__ \|  __/| |_ | |_ |  __/| |
     # |___/ \___| \__| \__| \___||_|
     # ==================================
+
+    def set_log_mode(self, mode: MXPrintMode) -> None:
+        self._log_mode = mode
+
+    def set_log_enable(self, enable: bool) -> None:
+        self._log_enable = enable
+
+    def set_log_name(self, name: str) -> None:
+        self._log_name = name
+
+    def set_ip(self, ip: str) -> None:
+        self._ip = ip
+
+    def set_port(self, port: int) -> None:
+        self._port = port
+
+    def set_ssl_ca_path(self, path: str) -> None:
+        self._ssl_ca_path = path
+
+    def set_ssl_enable(self, enable: bool) -> None:
+        self._ssl_enable = enable
```

## big_thing_py/manager_thing.py

```diff
@@ -1,28 +1,28 @@
 from big_thing_py.big_thing import *
 from big_thing_py.staff_thing import *
 from big_thing_py.manager import *
 import uuid
 
 
-class SoPManagerThing(SoPBigThing, metaclass=ABCMeta):
+class MXManagerThing(MXBigThing, metaclass=ABCMeta):
 
     MANAGER_THREAD_TIME_OUT = THREAD_TIME_OUT
 
-    def __init__(self, name: str, service_list: List[SoPService], alive_cycle: float, is_super: bool = False, is_parallel: bool = True,
-                 ip: str = None, port: int = None, ssl_ca_path: str = None, ssl_enable: bool = False, log_name: str = None, log_enable: bool = True, log_mode: SoPPrintMode = SoPPrintMode.ABBR, append_mac_address: bool = True,
-                 manager_mode: SoPManagerMode = SoPManagerMode.SPLIT, scan_cycle=5):
+    def __init__(self, name: str, service_list: List[MXService], alive_cycle: float, is_super: bool = False, is_parallel: bool = True,
+                 ip: str = None, port: int = None, ssl_ca_path: str = None, ssl_enable: bool = False, log_name: str = None, log_enable: bool = True, log_mode: MXPrintMode = MXPrintMode.ABBR, append_mac_address: bool = True,
+                 manager_mode: MXManagerMode = MXManagerMode.SPLIT, scan_cycle=5):
         super().__init__(name, service_list, alive_cycle, is_super, is_parallel, ip, port,
                          ssl_ca_path, ssl_enable, log_name, log_enable, log_mode, append_mac_address)
 
         self._scan_cycle = scan_cycle
-        self._manager_mode = SoPManagerMode.get(
+        self._manager_mode = MXManagerMode.get(
             manager_mode) if isinstance(manager_mode, str) else manager_mode
 
-        self._staff_thing_list: List[SoPStaffThing] = []
+        self._staff_thing_list: List[MXStaffThing] = []
         self._manager_mode_handler = ManagerModeHandler(
             mode=self._manager_mode)
 
         self._last_scan_time = 0
 
         # Threading
         self._thread_func_list += [
@@ -34,73 +34,73 @@
     # override
     def run(self):
         try:
             # Start main threads
             for thread in self._comm_thread_list + self._thread_list:
                 thread.start()
 
-            if self._manager_mode == SoPManagerMode.JOIN:
+            if self._manager_mode == MXManagerMode.JOIN:
                 # Register try
                 retry = 5
                 while not self._registered and retry:
-                    SOPLOG_DEBUG(f'Register try {6-retry}', 'yellow')
+                    MXLOG_DEBUG(f'Register try {6-retry}', 'yellow')
                     retry -= 1
 
-                    self._subscribe_init_topics(self)
-                    self._send_TM_REGISTER(
-                        thing_name=self._name, payload=self.dump())
+                    # FIXME: Need to override to fit managerThing (Receive StaffThing as a factor)
+                    self._subscribe_init_topic_list(self)
+                    self._send_TM_REGISTER()
 
                     current_time = get_current_time()
                     while get_current_time() - current_time < 5:
                         if self._registered:
                             break
                         else:
                             time.sleep(0.1)
-            elif self._manager_mode == SoPManagerMode.SPLIT:
+            elif self._manager_mode == MXManagerMode.SPLIT:
                 # SPLIT 모드일 땐, manager thing 자기자신은 등록하지 않는다.
                 pass
             else:
                 pass
 
             # Maintain main thread
             while not self._g_exit.wait(THREAD_TIME_OUT):
                 time.sleep(1000)
         except KeyboardInterrupt as e:
-            SOPLOG_DEBUG('Ctrl + C Exit', 'red')
+            MXLOG_DEBUG('Ctrl + C Exit', 'red')
             return self.wrapup()
         except ConnectionRefusedError as e:
-            SOPLOG_DEBUG(
+            MXLOG_DEBUG(
                 'Connection error while connect to broker. Check ip and port', 'red')
             return self.wrapup()
         except Exception as e:
             print_error(e)
             return self.wrapup()
 
     # override
     def wrapup(self):
         try:
             for staff_thing in self._staff_thing_list:
-                self._send_TM_UNREGISTER(staff_thing.get_name())
+                self._send_TM_UNREGISTER()
             cur_time = get_current_time()
 
             self._g_exit.set()
             for thread in self._thread_list:
                 thread.join()
-                SOPLOG_DEBUG(f'{thread._name} is terminated', 'yellow')
+                MXLOG_DEBUG(f'{thread._name} is terminated', 'yellow')
 
             while not ((self._publish_queue.empty() and self._receive_queue.empty()) or (get_current_time() - cur_time > 3)):
                 time.sleep(THREAD_TIME_OUT)
 
             self._g_comm_exit.set()
             for thread in self._comm_thread_list:
                 thread.join()
-                SOPLOG_DEBUG(f'{thread._name} is terminated', 'yellow')
+                MXLOG_DEBUG(f'{thread._name} is terminated', 'yellow')
 
             self._mqtt_client.disconnect()
-            SOPLOG_DEBUG('Thing Exit', 'red')
+            MXLOG_DEBUG('Thing Exit', 'red')
             return True
         except Exception as e:
             print_error(e)
             return False
 
     # ===========================================================================================
     #  _    _                             _    __                      _    _
@@ -108,54 +108,52 @@
     # | |_ | |__   _ __   ___   __ _   __| | | |_  _   _  _ __    ___ | |_  _   ___   _ __   ___
     # | __|| '_ \ | '__| / _ \ / _` | / _` | |  _|| | | || '_ \  / __|| __|| | / _ \ | '_ \ / __|
     # | |_ | | | || |   |  __/| (_| || (_| | | |  | |_| || | | || (__ | |_ | || (_) || | | |\__ \
     #  \__||_| |_||_|    \___| \__,_| \__,_| |_|   \__,_||_| |_| \___| \__||_| \___/ |_| |_||___/
     # ===========================================================================================
 
     # override
-    def _alive_thread_func(self, stop_event: Event) -> Union[bool, None]:
+    def _alive_publishing_thread_func(self, stop_event: Event) -> Union[bool, None]:
         try:
             while not stop_event.wait(THREAD_TIME_OUT):
-                if self._manager_mode == SoPManagerMode.JOIN:
+                if self._manager_mode == MXManagerMode.JOIN:
                     current_time = get_current_time()
                     if current_time - self._last_alive_time > self._alive_cycle:
                         for staff_thing in self._staff_thing_list:
-                            self._send_TM_ALIVE(
-                                thing_name=staff_thing.get_name())
+                            self._send_TM_ALIVE()
                             staff_thing._last_alive_time = current_time
-                elif self._manager_mode == SoPManagerMode.SPLIT:
+                elif self._manager_mode == MXManagerMode.SPLIT:
                     # split 모드일 때는 staff thing이 alive 신호를 받아서 보내므로 생략
                     # current_time = get_current_time()
                     # for staff_thing in self._staff_thing_list:
                     #     if current_time - staff_thing._last_alive_time > staff_thing._alive_cycle:
-                    #         self._send_TM_ALIVE(thing_name=self._name)
+                    #         self._send_TM_ALIVE()
                     #         staff_thing._last_alive_time = current_time
                     pass
                 else:
                     raise Exception('Invalid Manager Mode')
         except Exception as e:
             stop_event.set()
             print_error(e)
             return False
 
     # override
-    def _value_publish_thread_func(self, stop_event: Event) -> Union[bool, None]:
+    def _value_publishing_thread_func(self, stop_event: Event) -> Union[bool, None]:
         try:
             while not stop_event.wait(THREAD_TIME_OUT):
                 for staff_thing in self._staff_thing_list:
                     if not staff_thing._registered:
                         continue
                     current_time = get_current_time()
                     for value in staff_thing._value_list:
                         if not (current_time - value.get_last_update_time()) > value.get_cycle():
                             continue
                         arg_list = tuple(value.get_arg_list())
                         if value.update(*arg_list) is not None:
-                            self._send_TM_VALUE_PUBLISH(
-                                staff_thing._name, value.get_name(), value.dump_pub())
+                            self._send_TM_VALUE_PUBLISH(value=value)
         except Exception as e:
             stop_event.set()
             print_error(e)
             return False
 
     ############################################################################################################################
 
@@ -169,43 +167,42 @@
 
                 staff_thing_info_list = self._scan_staff_thing()
                 if staff_thing_info_list == False:
                     raise Exception('Scan staff thing error')
 
                 old_staff_thing_list = [
                     staff_thing for staff_thing in self._staff_thing_list]
-                new_staff_thing_list: List[SoPStaffThing] = []
-                latest_staff_thing_list: List[SoPStaffThing] = []
-                removed_staff_thing_list: List[SoPStaffThing] = []
+                new_staff_thing_list: List[MXStaffThing] = []
+                latest_staff_thing_list: List[MXStaffThing] = []
+                removed_staff_thing_list: List[MXStaffThing] = []
                 for staff_thing_info in staff_thing_info_list:
                     staff_thing = self._create_staff(staff_thing_info)
 
                     staff_thing_level, staff_thing = self._check_staff_thing_duplicate(
                         staff_thing)
                     latest_staff_thing_list.append(staff_thing)
-                    if staff_thing_level == SoPNewStaffThingLevel.NEW:
-                        SOPLOG_DEBUG(
+                    if staff_thing_level == MXNewStaffThingLevel.NEW:
+                        MXLOG_DEBUG(
                             f'New staff_thing!!! name: [{staff_thing.get_name()}]', 'green')
                         new_staff_thing_list.append(staff_thing)
-                    elif staff_thing_level == SoPNewStaffThingLevel.DUPLICATE:
-                        SOPLOG_DEBUG(
+                    elif staff_thing_level == MXNewStaffThingLevel.DUPLICATE:
+                        MXLOG_DEBUG(
                             f'Staff thing [{staff_thing.get_name()}] was still alive...', 'yellow')
 
                 removed_staff_thing_list = [
                     item for item in old_staff_thing_list if item not in latest_staff_thing_list]
                 for staff_thing in new_staff_thing_list:
                     self._staff_thing_list.append(staff_thing)
                     self._connect_staff_thing(staff_thing)
                 for staff_thing in removed_staff_thing_list:
                     try:
                         self._disconnect_staff_thing(staff_thing)
                         self._staff_thing_list.remove(staff_thing)
                     except ValueError:
-                        raise Exception(
-                            f'[scan_staff_message_thread_func][{staff_thing.get_name()}] is not in staff thing list')
+                        raise Exception(f'[{get_current_function_name()}][{staff_thing.get_name()}] is not in staff thing list')
 
                 staff_thing_info_list = None
                 self._last_scan_time = get_current_time()
         except Exception as e:
             stop_event.set()
             print_error(e)
             return False
@@ -247,99 +244,102 @@
     # |_| |_| \__,_||_| |_| \__,_||_| \___| \_|  |_/ \_/\_\  \_/    \_/   |_| |_| |_| \___||___/|___/ \__,_| \__, | \___|
     #                                                                                                         __/ |
     #                                                                                                        |___/
     # ====================================================================================================================
 
     # override
     def _handle_MT_RESULT_REGISTER(self, msg: mqtt.MQTTMessage):
-        register_result_msg = SoPRegisterResultMessage(msg)
-        target_staff_thing = self._find_staff_thing_by_name(
-            register_result_msg._thing_name)
+        register_result_msg = MXRegisterResultMessage(msg)
+        target_staff_thing = self._get_staff_thing_by_name(
+            register_result_msg.thing_name)
 
         if target_staff_thing is False:
-            SOPLOG_DEBUG(
-                f'Wrong payload arrive... {self._name} should be arrive, not {register_result_msg._thing_name}', 'red')
+            MXLOG_DEBUG(
+                f'[{get_current_function_name()}] Wrong payload arrive... {self._name} should be arrive, not {register_result_msg.thing_name}', 'red')
             raise
 
-        if self._manager_mode == SoPManagerMode.JOIN:
+        if self._manager_mode == MXManagerMode.JOIN:
+            # FIXME: This method will be deprecated
             ret = self._check_register_result(
-                register_result_msg._error, thing=target_staff_thing)
+                register_result_msg.error, thing=target_staff_thing)
             if ret:
-                self._middleware_name = register_result_msg._middleware_name
+                self._middleware_name = register_result_msg.middleware_name
                 self._registered = True
-                self._subscribe_service_topics(self)
+                # FIXME: Need to override to fit managerThing (Receive StaffThing as a factor)
+                self._subscribe_service_topic_list(self)
                 self._send_RESULT_REGISTER_staff_message(
-                    target_staff_thing, register_result_msg.payload())
+                    target_staff_thing, register_result_msg.payload)
             else:
-                SOPLOG_DEBUG(
-                    f'[handle_MT_RESULT_REGISTER] Register failed... error code : {register_result_msg._error}')
-        elif self._manager_mode == SoPManagerMode.SPLIT:
+                MXLOG_DEBUG(
+                    f'[{get_current_function_name()}] Register failed... error code : {register_result_msg.error}')
+        elif self._manager_mode == MXManagerMode.SPLIT:
+            # FIXME: This method will be deprecated
             ret = self._check_register_result(
-                register_result_msg._error, thing=target_staff_thing)
+                register_result_msg.error, thing=target_staff_thing)
             if ret:
                 target_staff_thing.set_middleware_name(
-                    register_result_msg._middleware_name)
+                    register_result_msg.middleware_name)
                 target_staff_thing.set_registered(True)
-                self._subscribe_service_topics(target_staff_thing)
+                # FIXME: Need to override to fit managerThing (Receive StaffThing as a factor)
+                self._subscribe_service_topic_list(target_staff_thing)
                 self._send_RESULT_REGISTER_staff_message(
-                    target_staff_thing, register_result_msg.payload())
+                    target_staff_thing, register_result_msg.payload)
             else:
-                SOPLOG_DEBUG(
-                    f'[handle_MT_RESULT_REGISTER] Register failed... error code : {register_result_msg._error}')
+                MXLOG_DEBUG(
+                    f'[{get_current_function_name()}] Register failed... error code : {register_result_msg.error}')
 
     # override
     def _handle_MT_RESULT_UNREGISTER(self, msg: mqtt.MQTTMessage):
-        unregister_result_msg = SoPUnregisterResultMessage(msg)
-        target_staff_thing = self._find_staff_thing_by_name(
-            unregister_result_msg._thing_name)
+        unregister_result_msg = MXUnregisterResultMessage(msg)
+        target_staff_thing = self._get_staff_thing_by_name(
+            unregister_result_msg.thing_name)
 
         if target_staff_thing is False:
-            SOPLOG_DEBUG(
-                f'Wrong payload arrive... {self._name} should be arrive, not {unregister_result_msg._thing_name}', 'red')
+            MXLOG_DEBUG(
+                f'[{get_current_function_name()}] Wrong payload arrive... {self._name} should be arrive, not {unregister_result_msg.thing_name}', 'red')
             raise
 
-        if self._manager_mode == SoPManagerMode.JOIN:
-            if self._check_register_result(unregister_result_msg._error):
+        if self._manager_mode == MXManagerMode.JOIN:
+            # FIXME: This method will be deprecated
+            if self._check_register_result(unregister_result_msg.error):
                 self._registered = False
-                self._unsubscrube_all_topics(self)
+                self._unsubscribe_all_topic_list(self)
                 self._send_RESULT_UNREGISTER_staff_message(
-                    target_staff_thing, unregister_result_msg.payload())
+                    target_staff_thing, unregister_result_msg.payload)
             else:
-                SOPLOG_DEBUG(
-                    f'[handle_MT_RESULT_UNREGISTER] Unregister failed... error code : {unregister_result_msg._error}')
-        elif self._manager_mode == SoPManagerMode.SPLIT:
+                MXLOG_DEBUG(
+                    f'[{get_current_function_name()}] Unregister failed... error code : {unregister_result_msg.error}')
+        elif self._manager_mode == MXManagerMode.SPLIT:
             # manager thing의 토픽중 해당 staff thing에 관련된 것만 unsubscribe한다
-            if self._check_register_result(unregister_result_msg._error):
+            # FIXME: This method will be deprecated
+            if self._check_register_result(unregister_result_msg.error):
                 target_staff_thing._registered = False
-                self._unsubscrube_all_topics(target_staff_thing)
+                self._unsubscribe_all_topic_list(target_staff_thing)
                 for topic in self._subscribed_topic_set:
                     if target_staff_thing.get_name() in topic:
                         self._unsubscribe(topic, thing=target_staff_thing)
                 self._send_RESULT_UNREGISTER_staff_message(
-                    target_staff_thing, unregister_result_msg.payload())
+                    target_staff_thing, unregister_result_msg.payload)
             else:
-                SOPLOG_DEBUG(
-                    f'[handle_MT_RESULT_UNREGISTER] Unregister failed... error code : {unregister_result_msg._error}')
+                MXLOG_DEBUG(
+                    f'[{get_current_function_name()}] Unregister failed... error code : {unregister_result_msg.error}')
 
-    # override
+    @override
     def _handle_MT_EXECUTE(self, msg: mqtt.MQTTMessage):
-        execute_msg = SoPExecuteMessage(msg)
-        execute_request = SoPExecuteRequest(
-            trigger_msg=execute_msg)
-        execute_request.timer_start()
-
-        target_staff_thing = self._find_staff_thing_by_name(
-            execute_msg._thing_name)
-        target_function = target_staff_thing._find_function(
-            execute_msg._function_name)
+        execute_msg = MXExecuteMessage(msg)
+
+        target_staff_thing = self._get_staff_thing_by_name(
+            execute_msg.thing_name)
+        target_function = target_staff_thing._get_function(
+            execute_msg.function_name)
 
         if target_function:
-            target_function.execute(execute_request)
+            execute_thread = target_function.start_execute_thread(execute_msg)
         else:
-            SOPLOG_DEBUG('function not exist', 'red')
+            MXLOG_DEBUG('function not exist', 'red')
             return False
 
     # ========================
     #         _    _  _
     #        | |  (_)| |
     #  _   _ | |_  _ | | ___
     # | | | || __|| || |/ __|
@@ -385,362 +385,241 @@
 
             Returns:
                 (None)
         '''
         pass
 
     @abstractmethod
-    def _parse_staff_message(self, staff_msg) -> Tuple[SoPProtocolType, str, str]:
+    def _parse_staff_message(self, staff_msg) -> Tuple[MXProtocolType, str, str]:
         '''
-            staff thing으로 부터 받은 패킷이 어느 SoPIoT 프로토콜에 해당하는지 파싱하는 함수.
-            staff thing가 보내는 패킷의 프로토콜은 다음 SoPIoT 프로토콜 중에 하나로 분류가 되어야한다. 
+            staff thing으로 부터 받은 패킷이 어느 MySSIX 프로토콜에 해당하는지 파싱하는 함수.
+            staff thing가 보내는 패킷의 프로토콜은 다음 MySSIX 프로토콜 중에 하나로 분류가 되어야한다. 
 
-            - SoPProtocolType.Base.TM_REGISTER
-            - SoPProtocolType.Base.TM_UNREGISTER
-            - SoPProtocolType.Base.TM_ALIVE
-            - SoPProtocolType.Base.TM_VALUE_PUBLISH
-            - SoPProtocolType.Base.TM_RESULT_EXECUTE
+            - MXProtocolType.Base.TM_REGISTER
+            - MXProtocolType.Base.TM_UNREGISTER
+            - MXProtocolType.Base.TM_ALIVE
+            - MXProtocolType.Base.TM_VALUE_PUBLISH
+            - MXProtocolType.Base.TM_RESULT_EXECUTE
 
             Args: 
                 staff_msg (str): 파싱할 staff thing의 패킷
 
             Returns:
-                protocol(SoPProtocolType): staff thing 패킷의 SoPIoT 프로토콜
+                protocol(MXProtocolType): staff thing 패킷의 MySSIX 프로토콜
                 device_id(str): staff thing의 device id
                 payload(str): staff thing 패킷의 payload
         '''
         pass
 
     @abstractmethod
-    def _create_staff(self, staff_thing_info: dict) -> SoPStaffThing:
+    def _create_staff(self, staff_thing_info: dict) -> MXStaffThing:
         '''
             _scan_staff_thing() 함수를 통해 수집된 staff thing 정보를 바탕으로 staff thing을 생성하는 함수.
             만약 스캔하는 것만으로 완벽한 staff thing의 정보를 수집할 수 없다면, staff thing의 register 메시지를 받아 처리하는
             _handle_REGISTER_staff_message() 함수에서 staff thing을 self._staff_thing_list에서 찾아 정보를 추가할 수 있다.
 
             Args: 
                 staff_thing_info (dict): staff thing의 정보를 담고 있는 딕셔너리
 
             Returns:
-                staff_thing(SoPStaffThing): 생성한 staff thing 인스턴스
+                staff_thing(MXStaffThing): 생성한 staff thing 인스턴스
         '''
         pass
 
     @abstractmethod
-    def _connect_staff_thing(self, staff_thing: SoPStaffThing) -> bool:
+    def _connect_staff_thing(self, staff_thing: MXStaffThing) -> bool:
         '''
             staff thing과 연결하는 함수.
 
             Args: 
-                staff_thing (SoPStaffThing): 타겟 staff thing 인스턴스
+                staff_thing (MXStaffThing): 타겟 staff thing 인스턴스
 
             Returns:
                 (None)
         '''
         pass
 
     @abstractmethod
-    def _disconnect_staff_thing(self, staff_thing: SoPStaffThing) -> bool:
+    def _disconnect_staff_thing(self, staff_thing: MXStaffThing) -> bool:
         '''
             staff thing과 연결해제하는 함수.
 
             Args: 
-                staff_thing (SoPStaffThing): 타겟 staff thing 인스턴스
+                staff_thing (MXStaffThing): 타겟 staff thing 인스턴스
 
             Returns:
                 (None)
         '''
         pass
 
     @abstractmethod
-    def _handle_REGISTER_staff_message(self, staff_thing: SoPStaffThing, payload: dict) -> Tuple[str, dict]:
+    def _handle_REGISTER_staff_message(self, staff_thing: MXStaffThing, payload: dict) -> Tuple[str, dict]:
         '''
             staff thing으로부터 받은 register 메시지를 처리하는 함수.
 
             Args: 
-                staff_thing (SoPStaffThing): 타겟 staff thing 인스턴스
-                payload (dict): staff thing으로부터 받은 register 메시지의 payload. (SoPThing.dump()의 결과)
+                staff_thing (MXStaffThing): 타겟 staff thing 인스턴스
+                payload (dict): staff thing으로부터 받은 register 메시지의 payload. (MXThing.dump()의 결과)
 
             Returns:
                 (None)
         '''
         pass
 
     @abstractmethod
-    def _handle_UNREGISTER_staff_message(self, staff_thing: SoPStaffThing) -> str:
+    def _handle_UNREGISTER_staff_message(self, staff_thing: MXStaffThing) -> str:
         '''
             staff thing으로부터 받은 unregister 메시지를 처리하는 함수.
 
             Args: 
-                staff_thing (SoPStaffThing): 타겟 staff thing 인스턴스
+                staff_thing (MXStaffThing): 타겟 staff thing 인스턴스
 
             Returns:
                 (None)
         '''
         pass
 
     @abstractmethod
-    def _handle_ALIVE_staff_message(self, staff_thing: SoPStaffThing) -> str:
+    def _handle_ALIVE_staff_message(self, staff_thing: MXStaffThing) -> str:
         '''
             staff thing으로부터 받은 alive 메시지를 처리하는 함수.
 
             Args: 
-                staff_thing (SoPStaffThing): 타겟 staff thing 인스턴스
+                staff_thing (MXStaffThing): 타겟 staff thing 인스턴스
 
             Returns:
                 (None)
         '''
         pass
 
     @abstractmethod
-    def _handle_VALUE_PUBLISH_staff_message(self, staff_thing: SoPStaffThing, payload: dict) -> Tuple[str, str, dict]:
+    def _handle_VALUE_PUBLISH_staff_message(self, staff_thing: MXStaffThing, payload: dict) -> Tuple[str, str, dict]:
         '''
             staff thing으로부터 받은 value publish 메시지를 처리하는 함수.
 
             Args: 
-                staff_thing (SoPStaffThing): 타겟 staff thing 인스턴스
-                payload (dict): staff thing으로부터 받은 value publish 메시지의 payload. (SoPValue.dump()의 결과)
+                staff_thing (MXStaffThing): 타겟 staff thing 인스턴스
+                payload (dict): staff thing으로부터 받은 value publish 메시지의 payload. (MXValue.dump()의 결과)
 
             Returns:
                 (None)
         '''
         pass
 
     @abstractmethod
-    def _handle_RESULT_EXECUTE_staff_message(self, staff_thing: SoPStaffThing, payload: dict) -> str:
+    def _handle_RESULT_EXECUTE_staff_message(self, staff_thing: MXStaffThing, payload: dict) -> str:
         '''
             staff thing으로부터 받은 result execute 메시지를 처리하는 함수.
             해당 기능은 아직 구현되지 않았음.
         '''
         pass
 
     @abstractmethod
-    def _send_RESULT_REGISTER_staff_message(self, staff_thing: SoPStaffThing, payload: str) -> str:
+    def _send_RESULT_REGISTER_staff_message(self, staff_thing: MXStaffThing, payload: str) -> str:
         '''
             staff thing에게 result register 메시지를 전송하는 함수.
 
             Args: 
-                staff_thing (SoPStaffThing): 타겟 staff thing 인스턴스
+                staff_thing (MXStaffThing): 타겟 staff thing 인스턴스
                 payload (str): staff thing 에게 보낼 register result 메시지의 payload. (커스텀형식의 payload)
 
             Returns:
                 (None)
         '''
         pass
 
     @abstractmethod
-    def _send_RESULT_UNREGISTER_staff_message(self, staff_thing: SoPStaffThing, payload: str) -> str:
+    def _send_RESULT_UNREGISTER_staff_message(self, staff_thing: MXStaffThing, payload: str) -> str:
         '''
             staff thing에게 result unregister 메시지를 전송하는 함수.
 
             Args: 
-                staff_thing (SoPStaffThing): 타겟 staff thing 인스턴스
+                staff_thing (MXStaffThing): 타겟 staff thing 인스턴스
                 payload (str): staff thing 에게 보낼 unregister result 메시지의 payload. (커스텀형식의 payload)
 
             Returns:
                 (None)
         '''
         pass
 
     @abstractmethod
-    def _send_EXECUTE_staff_message(self, staff_thing: SoPStaffThing, payload: str) -> str:
+    def _send_EXECUTE_staff_message(self, staff_thing: MXStaffThing, payload: str) -> str:
         '''
             staff thing에게 execute 메시지를 전송하는 함수.
             해당 기능은 아직 구현되지 않았음.
         '''
         pass
 
     ############################################################################################################################
 
     def _handle_staff_message(self, staff_msg):
         staff_protocol, staff_device_id, staff_payload = self._parse_staff_message(
             staff_msg)
-        target_staff_thing = self._find_staff_thing_by_device_id(
+        target_staff_thing = self._get_staff_thing_by_device_id(
             staff_device_id)
 
-        if staff_protocol == SoPProtocolType.Base.TM_REGISTER:
+        if staff_protocol == MXProtocolType.Base.TM_REGISTER:
             thing_name, payload = self._handle_REGISTER_staff_message(
                 target_staff_thing, staff_payload)
-            self._subscribe_init_topics(target_staff_thing)
-            self._send_TM_REGISTER(thing_name, payload)
+            self._subscribe_init_topic_list(target_staff_thing)
+            self._send_TM_REGISTER()
             target_staff_thing.set_registered(True)
 
             if staff_device_id in [staff_thing._device_id for staff_thing in self._staff_thing_list]:
                 target_staff_thing._device_id = staff_device_id
             else:
                 target_staff_thing._device_id = self._generate_device_id()
-        elif staff_protocol == SoPProtocolType.Base.TM_UNREGISTER:
+        elif staff_protocol == MXProtocolType.Base.TM_UNREGISTER:
             thing_name = self._handle_UNREGISTER_staff_message(
                 target_staff_thing)
-            self._send_TM_UNREGISTER(thing_name)
+            self._send_TM_UNREGISTER()
             target_staff_thing.set_registered(False)
-        elif staff_protocol == SoPProtocolType.Base.TM_ALIVE:
+        elif staff_protocol == MXProtocolType.Base.TM_ALIVE:
             thing_name = self._handle_ALIVE_staff_message(target_staff_thing)
-            self._send_TM_ALIVE(thing_name)
-        elif staff_protocol == SoPProtocolType.Base.TM_VALUE_PUBLISH:
-            thing_name, value_name, payload = self._handle_VALUE_PUBLISH_staff_message(
+            self._send_TM_ALIVE()
+        elif staff_protocol == MXProtocolType.Base.TM_VALUE_PUBLISH:
+            # FIXME: MXValue 를 리턴하도록 수정
+            value = self._handle_VALUE_PUBLISH_staff_message(
                 target_staff_thing, staff_payload)
-            self._send_TM_VALUE_PUBLISH(thing_name, value_name, payload)
-        elif staff_protocol == SoPProtocolType.Base.TM_RESULT_EXECUTE:
+            self._send_TM_VALUE_PUBLISH(value=value)
+        elif staff_protocol == MXProtocolType.Base.TM_RESULT_EXECUTE:
             # TODO: complete this
             pass
             # TM/RESULT/EXECUTE/[FunctionName]/[ThingName]/([MiddlewareName]/[Request_ID])
-            # Request_ID = requester_middleware@super_thing@super_function@subrequest_order
+            # Request_ID = requester_middleware@super_thing@super_service@subrequest_order
             # function_name, thing_name, middleware_name, request_ID, return_value = self._handle_RESULT_EXECUTE_staff_message(
             #     target_staff_thing, staff_payload)
-            # target_staff_thing_function = target_staff_thing._find_function(function_name)
+            # target_staff_thing_function = target_staff_thing._get_function(function_name)
             # self._send_TM_RESULT_EXECUTE(function_name, thing_name, target_staff_thing_function.get_return_type(), return_value,
             #                              middleware_name)
 
     ############################################################################################################################
 
     def _generate_device_id(self) -> str:
         return str(uuid.uuid4())
 
-    def _find_staff_thing_by_name(self, staff_name: str) -> SoPStaffThing:
+    def _get_staff_thing_by_name(self, staff_name: str) -> MXStaffThing:
         for staff_thing in self._staff_thing_list:
             if staff_thing.get_name() == staff_name:
                 return staff_thing
         return False
 
-    def _find_staff_thing_by_device_id(self, device_id: str) -> SoPStaffThing:
+    def _get_staff_thing_by_device_id(self, device_id: str) -> MXStaffThing:
         for staff_thing in self._staff_thing_list:
             if staff_thing._device_id == device_id:
                 return staff_thing
         return False
 
-    def _append_staff_thing_value(self, new_staff_thing: SoPStaffThing):
+    def _append_staff_thing_value(self, new_staff_thing: MXStaffThing):
         self._staff_thing_list.append(new_staff_thing)
         for value in new_staff_thing.get_value_list():
             if not value in self._value_list:
                 staff_value_name = f'{new_staff_thing.get_name()}/{value.get_name()}'
                 value.set_name(staff_value_name)
                 self._value_list.append(value)
 
-    def _check_staff_thing_duplicate(self, new_staff_thing: SoPStaffThing) -> Tuple[SoPNewStaffThingLevel, SoPStaffThing]:
+    def _check_staff_thing_duplicate(self, new_staff_thing: MXStaffThing) -> Tuple[MXNewStaffThingLevel, MXStaffThing]:
         for staff_thing in self._staff_thing_list:
             if new_staff_thing == staff_thing:
-                return SoPNewStaffThingLevel.DUPLICATE, staff_thing
-        else:
-            return SoPNewStaffThingLevel.NEW, new_staff_thing
-
-    def _print_packet(self, msg: mqtt.MQTTMessage, mode: SoPPrintMode = SoPPrintMode.FULL):
-
-        def mode_select(mode: SoPPrintMode, payload: str):
-            if mode == SoPPrintMode.SKIP:
-                return colored(f'skip... (print_packet mode={mode})', 'yellow'), payload
-            elif mode == SoPPrintMode.ABBR:
-                payload_raw = payload
-                if payload.count('\n') > 10:
-                    payload = '\n'.join(payload.split('\n')[:10]) + '\n' + \
-                        colored(
-                            f'skip... (print_packet mode={mode})', 'yellow')
-                    return payload, payload_raw
-                elif len(payload) > 1000:
-                    payload = payload[:1000] + '\n' + \
-                        colored(
-                            f'skip... (print_packet mode={mode})', 'yellow')
-                    return payload, payload_raw
-                else:
-                    return payload, payload_raw
-            elif mode == SoPPrintMode.FULL:
-                return payload, payload
-            else:
-                SOPLOG_DEBUG(
-                    f'[print_packet] Unknown mode!!! mode should be [skip|abbr|full] mode : {mode}', 'red')
-
-        def print_result_topic(topic, payload):
-            topic_str = topic_join(topic)
-            topic_indicator = f'{topic[0]}_{topic[1]}_{topic[2]}'
-
-            payload, payload_raw = mode_select(mode, payload)
-            payload = colored(payload, attrs=['bold'])
-
-            SOPLOG_DEBUG(
-                f'[{topic_indicator:20}] topic : {topic_str} payload : {payload}')
-
-            return True
-
-        def print_topic(topic, payload):
-            topic_str = topic_join(topic)
-            topic_indicator = f'{topic[0]}_{topic[1]}'
-
-            payload, payload_raw = mode_select(mode, payload)
-            payload = colored(payload, attrs=['bold'])
-
-            SOPLOG_DEBUG(
-                f'[{topic_indicator:20}] topic : {topic_str} payload : {payload}')
-
-            return True
-
-        topic, payload, timestamp = decode_MQTT_message(msg, str)
-        topic = topic_split(topic)
-        # target_staff_thing = self._find_staff_thing_by_name()
-
-        payload = dict_to_json_string(payload)
-
-        if topic[0] == 'MT':
-            if topic[1] == 'RESULT':
-                if topic[2] in ['REGISTER', 'UNREGISTER', 'BINARY_VALUE']:
-                    print_result_topic(topic, payload)
-                else:
-                    pass
-            else:
-                if topic[1] in ['EXECUTE']:
-                    return print_topic(topic, payload)
-                else:
-                    pass
-        elif topic[0] == 'TM':
-            if topic[1] == 'RESULT':
-                if topic[2] in ['EXECUTE']:
-                    print_result_topic(topic, payload)
-                else:
-                    pass
-            else:
-                if topic[1] in ['REGISTER', 'UNREGISTER', 'ALIVE', 'VALUE_PUBLISH']:
-                    return print_topic(topic, payload)
-                else:
-                    pass
-        elif topic[0] == 'MS':
-            if topic[1] == 'RESULT':
-                if topic[2] in ['SCHEDULE', 'EXECUTE', 'SERVICE_LIST']:
-                    print_result_topic(topic, payload)
-                else:
-                    pass
-            else:
-                if topic[1] in ['SCHEDULE', 'EXECUTE']:
-                    return print_topic(topic, payload)
-                else:
-                    pass
-        elif topic[0] == 'SM':
-            if topic[1] == 'RESULT':
-                if topic[2] in ['SCHEDULE', 'EXECUTE']:
-                    print_result_topic(topic, payload)
-                else:
-                    pass
-            else:
-                if topic[1] in ['SCHEDULE', 'EXECUTE', 'AVAILABILITY', 'REFRESH']:
-                    return print_topic(topic, payload)
-                else:
-                    pass
-        elif topic[0] == 'ME':
-            if topic[1] == 'NOTIFY_CHANGE':
-                return print_topic(topic, payload)
-            else:
-                pass
+                return MXNewStaffThingLevel.DUPLICATE, staff_thing
         else:
-            target_staff_thing = self._find_staff_thing_by_name(topic[0])
-            if target_staff_thing:
-                if topic[1] in [value.get_name() for value in target_staff_thing._value_list]:
-                    return print_topic(topic, payload)
-                else:
-                    SOPLOG_DEBUG(
-                        f'[print_packet] Unexpected value VALUE_PUBLISH topic!!! value: {topic[1]} ', 'red')
-                    return False
-            else:
-                SOPLOG_DEBUG(
-                    f'[print_packet] Unexpected VALUE_PUBLISH topic!!! : {topic_join(topic)} ', 'red')
-                return False
-
-        SOPLOG_DEBUG(
-            f'[print_packet] Unexpected topic!!! : {topic_join(topic)} ', 'red')
-        return False
+            return MXNewStaffThingLevel.NEW, new_staff_thing
```

## big_thing_py/staff_thing.py

```diff
@@ -1,47 +1,46 @@
 from big_thing_py.core.thing import *
 import functools
 
 
-class SoPStaffThing(SoPThing, metaclass=ABCMeta):
-    def __init__(self, name: str, service_list: List[SoPService], alive_cycle: float, is_super: bool = False, is_parallel: bool = True,
+class MXStaffThing(MXThing, metaclass=ABCMeta):
+    def __init__(self, name: str, service_list: List[MXService], alive_cycle: float, is_super: bool = False, is_parallel: bool = True,
                  device_id: str = None):
         super().__init__(name, service_list, alive_cycle, is_super, is_parallel)
         self._device_id = device_id
         self._is_connected = False
 
         self._receive_queue: Queue = Queue()
         self._publish_queue: Queue = Queue()
 
     # TODO: Check this method works correct
-    def __eq__(self, o: object) -> bool:
-        check_instance = isinstance(o, SoPThing)
-        check_device_id = (o._device_id == self._device_id)
-        check_name = (o._name == self._name)
+    def __eq__(self, o: 'MXStaffThing') -> bool:
+        instance_check = isinstance(o, MXStaffThing)
+        device_id_check = (o._device_id == self._device_id)
 
-        return check_instance and check_name and check_device_id
+        return super().__eq__(o) and instance_check and device_id_check
 
     def get_device_id(self) -> str:
         return self._device_id
 
     def set_device_id(self, id: str) -> None:
         self._device_id = id
 
     def is_connected(self) -> bool:
         return self._is_connected
 
     def set_function_result_queue(self, queue: Queue) -> None:
-        for function in self.get_function_list():
+        for function in self._function_list:
             function.set_publish_queue(queue)
 
     def print_func_info(func: Callable):
 
         @functools.wraps(func)
-        def wrap(self: SoPStaffThing, *args, **kwargs):
-            SOPLOG_DEBUG(
+        def wrap(self: MXStaffThing, *args, **kwargs):
+            MXLOG_DEBUG(
                 f'{func.__name__} at {self._name} actuate!!!', 'green')
             ret = func(self, *args, **kwargs)
             return ret
         # TODO: 함수가 데코레이팅 되었으면 staff thing의 service list에 추가하는 기능을 구현하고자 추가함
         # TODO: 근데 위에 @functools.wraps(func)기능과 동시에 사용이 가능한지 확인해야함
         wrap.is_decorated = True
         return wrap
```

## big_thing_py/super_thing.py

```diff
@@ -1,111 +1,114 @@
 from big_thing_py.big_thing import *
 from big_thing_py.super import *
+import threading
 
 
-class SoPSuperThing(SoPBigThing):
-    DUMMY_RESULT_LIST = [dict(error=SoPErrorType.UNDEFINED,
-                              scenario=None,
-                              return_type=SoPType.UNDEFINED,
-                              return_value=None)]
-
-    def __init__(self, name: str, service_list: List[SoPService], alive_cycle: float, is_super: bool = False, is_parallel: bool = True,
-                 ip: str = None, port: int = None, ssl_ca_path: str = None, ssl_enable: bool = False, log_name: str = None, log_enable: bool = True, log_mode: SoPPrintMode = SoPPrintMode.ABBR, append_mac_address: bool = True,
-                 refresh_cycle: float = 10, retry_register: bool = True):
-        super().__init__(name, service_list, alive_cycle, is_super, is_parallel, ip, port,
-                         ssl_ca_path, ssl_enable, log_name, log_enable, log_mode, append_mac_address, retry_register)
+class MXSuperThing(MXBigThing):
 
-        self._hierarchical_service_table: Dict[str, List[SoPService]] = dict(
-            value=[], function=[])
+    DEFAULT_NAME = 'default_super_thing'
 
-        self._last_refresh_time = 0
-        self._last_available_time = 0
+    # Super Service Execution 요청이 들어왔을때 mapping_table에 있는 super_request를 찾기 위한 super_service_request_key 리스트
+    # Super Service는 자신의 이름으로 super_request_key를 찾을 수 있다.
+    # {
+    #     'super_service_request_key1': ['sub_service_request_key1', 'sub_service_request_key2', ...]},
+    #     'super_service_request_key2': ['sub_service_request_key3', 'sub_service_request_key4', ...]},
+    #      ...
+    # }
+    _SUPER_SERVICE_REQUEST_KEY_TABLE: Dict[str, List[str]] = dict()
+
+    def __init__(self, name: str = DEFAULT_NAME, service_list: List[MXService] = [], alive_cycle: float = 60, is_super: bool = True, is_parallel: bool = True,
+                 ip: str = '127.0.0.1', port: int = 1883, ssl_ca_path: str = '', ssl_enable: bool = False,
+                 log_name: str = '', log_enable: bool = True, log_mode: MXPrintMode = MXPrintMode.ABBR,
+                 append_mac_address: bool = True,
+                 refresh_cycle: float = 30):
+
+        self._global_service_table: Dict[str, Union[List[MXFunction], List[MXValue]]] = dict(values=[], functions=[])
+        self._SUPER_SERVICE_REQUEST_KEY_TABLE = dict()
+
+        super().__init__(name, service_list, alive_cycle, is_super, is_parallel, ip, port,
+                         ssl_ca_path, ssl_enable, log_name, log_enable, log_mode, append_mac_address)
 
         self._refresh_cycle = refresh_cycle
-        self._available_cycle = refresh_cycle / 2
 
-        self._function_list: List[SoPSuperFunction] = self._function_list
+        self._last_refresh_time = 0
 
-        # Queue
-        self._super_execute_queue: Queue = Queue()
-        self._schedule_queue: Queue = Queue()
-        self._subscribe_queue: Queue = Queue()
-        self._unsubscribe_queue: Queue = Queue()
+        self._function_list: List[MXSuperFunction] = self._function_list
 
         self._thread_func_list += [
             self._refresh_thread_func,
-            self._available_thread_func,
-            self._subscribe_thread_func,
-            self._unsubscribe_thread_func]
-
-        self._extract_subfunction_reqline_info()
-
-        for super_function in self._function_list:
-            super_function.set_subscribe_queue(self._subscribe_queue)
-            super_function.set_unsubscribe_queue(self._unsubscribe_queue)
+        ]
+
+    def __eq__(self, o: 'MXSuperThing'):
+        instance_check = isinstance(o, MXSuperThing)
+        refresh_cycle_check = (self._refresh_cycle == o._refresh_cycle)
+
+        return super().__eq__(o) and instance_check and refresh_cycle_check
+
+    def __getstate__(self):
+        state = super().__getstate__()
+
+        state['_refresh_cycle'] = self._refresh_cycle
+
+        del state['_last_refresh_time']
+
+        return state
+
+    def __setstate__(self, state):
+        super().__setstate__(state)
+
+        self._refresh_cycle = state['_refresh_cycle']
+
+        self._last_refresh_time = 0
+        self._thread_func_list = self._thread_func_list + [
+            self._refresh_thread_func,
+        ]
+
+    @override
+    def setup(self, avahi_enable=True) -> 'MXSuperThing':
+        self._init_logger()
+        self._extract_sub_service_request_info()
+        return super().setup(avahi_enable)
 
     # ===========================================================================================
     #  _    _                             _    __                      _    _
     # | |  | |                           | |  / _|                    | |  (_)
     # | |_ | |__   _ __   ___   __ _   __| | | |_  _   _  _ __    ___ | |_  _   ___   _ __   ___
     # | __|| '_ \ | '__| / _ \ / _` | / _` | |  _|| | | || '_ \  / __|| __|| | / _ \ | '_ \ / __|
     # | |_ | | | || |   |  __/| (_| || (_| | | |  | |_| || | | || (__ | |_ | || (_) || | | |\__ \
     #  \__||_| |_||_|    \___| \__,_| \__,_| |_|   \__,_||_| |_| \___| \__||_| \___/ |_| |_||___/
     # ===========================================================================================
 
     def _refresh_thread_func(self, stop_event: Event):
         try:
             while not stop_event.wait(THREAD_TIME_OUT):
-                if self._registered:
+                if self._is_registered:
                     if (get_current_time() - self._last_refresh_time) > self._refresh_cycle:
                         self._send_SM_REFRESH()
                         self._last_refresh_time = get_current_time()
                         # time.sleep(self._refresh_cycle / 2)
 
         except Exception as e:
             stop_event.set()
             print_error(e)
             return False
 
-    def _available_thread_func(self, stop_event: Event):
-        try:
-            while not stop_event.wait(THREAD_TIME_OUT):
-                if self._registered:
-                    if (get_current_time() - self._last_available_time) > self._available_cycle:
-                        self._send_SM_AVAILABILITY()
-                        self._last_available_time = get_current_time()
-                        # time.sleep(self._available_cycle / 2)
-
         except Exception as e:
             stop_event.set()
             print_error(e)
             return False
 
-    def _subscribe_thread_func(self, stop_event: Event):
-        try:
-            while not stop_event.wait(THREAD_TIME_OUT):
-                if self._registered:
-                    if not self._subscribe_queue.empty():
-                        topic = self._subscribe_queue.queue[0]
-                        self._subscribe(topic)
-                        self._subscribe_queue.get()
-
-        except Exception as e:
-            stop_event.set()
-            print_error(e)
-            return False
-
-    def _unsubscribe_thread_func(self, stop_event: Event):
-        try:
-            while not stop_event.wait(THREAD_TIME_OUT):
-                if self._registered:
-                    if not self._unsubscribe_queue.empty():
-                        topic = self._unsubscribe_queue.queue[0]
-                        self._unsubscribe(topic)
-                        topic = self._unsubscribe_queue.get()
+    # def _unsubscribe_thread_func(self, stop_event: Event):
+    #     try:
+    #         while not stop_event.wait(THREAD_TIME_OUT):
+    #             if self._registered:
+    #                 if not self._unsubscribe_queue.empty():
+    #                     topic = self._unsubscribe_queue.queue[0]
+    #                     self._unsubscribe(topic)
+    #                     topic = self._unsubscribe_queue.get()
 
         except Exception as e:
             stop_event.set()
             print_error(e)
             return False
 
     # ====================================================================================================================
@@ -115,531 +118,565 @@
     # | '_ \  / _` || '_ \  / _` || | / _ \ | |\/| || | | |  | |    | |   | '_ ` _ \  / _ \/ __|/ __| / _` | / _` | / _ \
     # | | | || (_| || | | || (_| || ||  __/ | |  | |\ \/' /  | |    | |   | | | | | ||  __/\__ \\__ \| (_| || (_| ||  __/
     # |_| |_| \__,_||_| |_| \__,_||_| \___| \_|  |_/ \_/\_\  \_/    \_/   |_| |_| |_| \___||___/|___/ \__,_| \__, | \___|
     #                                                                                                         __/ |
     #                                                                                                        |___/
     # ====================================================================================================================
 
-    def _handle_mqtt_message(self, msg: mqtt.MQTTMessage) -> None:
-        topic, payload, timestamp = unpack_mqtt_message(msg)
+    @override
+    def _classify_topic(self, topic: str) -> Union[MXProtocolType, bool]:
+        topic_token = topic_split(topic)
+        if topic_token[0] == 'MS':
+            if topic_token[1] == 'RESULT':
+                if topic_token[2] == 'SCHEDULE':
+                    protocol = MXProtocolType.Super.MS_RESULT_SCHEDULE
+                elif topic_token[2] == 'EXECUTE':
+                    protocol = MXProtocolType.Super.MS_RESULT_EXECUTE
+                elif topic_token[2] == 'SERVICE_LIST':
+                    protocol = MXProtocolType.Super.MS_RESULT_SERVICE_LIST
+                else:
+                    return False
+            elif topic_token[1] == 'SCHEDULE':
+                protocol = MXProtocolType.Super.MS_SCHEDULE
+            elif topic_token[1] == 'EXECUTE':
+                protocol = MXProtocolType.Super.MS_EXECUTE
+            else:
+                return False
+        elif topic_token[0] == 'ME':
+            if topic_token[1] == 'NOTIFY_CHANGE':
+                protocol = MXProtocolType.WebClient.ME_NOTIFY_CHANGE
+            else:
+                return False
+        else:
+            protocol = super()._classify_topic(topic)
 
-        if super()._handle_mqtt_message(msg):
-            return True
+        return protocol
+
+    @override
+    def _handle_mqtt_message(self, msg: mqtt.MQTTMessage) -> bool:
+        topic_string = decode_MQTT_message(msg)[0]
+        protocol = self._classify_topic(topic_string)
+        msg.timestamp = time.time()
+
+        if protocol == MXProtocolType.Super.MS_RESULT_SCHEDULE:
+            rc = self._handle_MS_RESULT_SCHEDULE(msg)
+        elif protocol == MXProtocolType.Super.MS_RESULT_EXECUTE:
+            rc = self._handle_MS_RESULT_EXECUTE(msg)
+        elif protocol == MXProtocolType.Super.MS_RESULT_SERVICE_LIST:
+            rc = self._handle_MS_RESULT_SERVICE_LIST(msg)
+        elif protocol == MXProtocolType.Super.MS_SCHEDULE:
+            rc = self._handle_MS_SCHEDULE(msg)
+        elif protocol == MXProtocolType.Super.MS_EXECUTE:
+            rc = self._handle_MS_EXECUTE(msg)
+        elif protocol == MXProtocolType.WebClient.ME_NOTIFY_CHANGE:
+            rc = self._handle_ME_NOTIFY(msg)
+
+        elif protocol == MXProtocolType.Base.MT_RESULT_REGISTER:
+            rc = self._handle_MT_RESULT_REGISTER(msg)
+        elif protocol == MXProtocolType.Base.MT_RESULT_UNREGISTER:
+            rc = self._handle_MT_RESULT_UNREGISTER(msg)
+        elif protocol == MXProtocolType.Base.MT_RESULT_BINARY_VALUE:
+            MXLOG_DEBUG(f'[{get_current_function_name()}] Not permitted topic! topic: {topic_string}')
+            return False
+        elif protocol == MXProtocolType.Base.MT_EXECUTE:
+            MXLOG_DEBUG(f'[{get_current_function_name()}] Not permitted topic! topic: {topic_string}')
+            return False
         else:
-            if topic[0] == 'MS':
-                if topic[1] == 'RESULT':
-                    if topic[2] == 'SCHEDULE':
-                        self._handle_MS_RESULT_SCHEDULE(msg)
-                    elif topic[2] == 'EXECUTE':
-                        self._handle_MS_RESULT_EXECUTE(msg)
-                    elif topic[2] == 'SERVICE_LIST':
-                        self._handle_MS_RESULT_SERVICE_LIST(msg)
-                    else:
-                        SOPLOG_DEBUG(
-                            '[handle_mqtt_message] Unexpected MS_RESULT topic!')
-                elif topic[1] == 'SCHEDULE':
-                    self._handle_MS_SCHEDULE(msg)
-                elif topic[1] == 'EXECUTE':
-                    self._handle_MS_EXECUTE(msg)
-                else:
-                    SOPLOG_DEBUG('[handle_mqtt_message] Unexpected MS topic!')
+            MXLOG_DEBUG(f'[{get_current_function_name()}] Unexpected topic! topic: {topic_string}')
+            return False
 
-                return True
-            elif topic[0] == 'ME':
-                if topic[1] == 'NOTIFY_CHANGE':
-                    self._handle_ME_NOTIFY(msg)
-                else:
-                    SOPLOG_DEBUG('[handle_mqtt_message] Unexpected ME topic!')
+        if not rc:
+            MXLOG_DEBUG(f'[{get_current_function_name()}] Unexpected topic! topic: {topic_string}')
+            return False
 
-                return True
-            else:
-                SOPLOG_DEBUG('[handle_mqtt_message] Unexpected topic!')
-                return False
+        return rc
 
     # ================
     # ___  ___ _____
     # |  \/  |/  ___|
     # | .  . |\ `--.
     # | |\/| | `--. \
     # | |  | |/\__/ /
     # \_|  |_/\____/
     # ================
 
-    def _handle_MS_SUPER_ACTION(self, super_action_msg: Union[SoPSuperScheduleMessage, SoPSuperExecuteMessage]):
-        target_super_function = self._find_function(
-            super_action_msg._super_function_name)
-        super_request_key = make_super_request_key(
-            super_action_msg._requester_middleware_name, super_action_msg._scenario)
-        if isinstance(super_action_msg, SoPSuperScheduleMessage):
-            if super_request_key in target_super_function._temporary_scheduling_table:
-                SOPLOG_DEBUG(
-                    f'[handle_MS_SUPER_ACTION] Super request key {super_request_key} is already exist in temporary_scheduling_table!', 'red')
-                return False
+    def _handle_MS_SCHEDULE(self, msg: mqtt.MQTTMessage) -> bool:
+        super_schedule_msg = MXSuperScheduleMessage(msg)
+        target_super_service = self._get_function(super_schedule_msg.super_service_name)
 
-            super_schedule_request = SoPSuperScheduleRequest(
-                trigger_msg=super_action_msg,)
-            target_super_function._temporary_scheduling_table[
-                super_request_key] = super_schedule_request
-            super_action_request = super_schedule_request
-        elif isinstance(super_action_msg, SoPSuperExecuteMessage):
-            if super_request_key in target_super_function._temporary_scheduling_table:
-                SOPLOG_DEBUG(
-                    f'[handle_MS_SUPER_ACTION] Super request key {super_request_key} is already exist in mapping_table!', 'red')
-                return False
+        if not target_super_service:
+            MXLOG_DEBUG(f'[{get_current_function_name()}] Super Service {super_schedule_msg.super_service_name} does not exist...', 'red')
+            return False
+        if self._name != super_schedule_msg.super_thing_name:
+            MXLOG_DEBUG(f'[{get_current_function_name()}] Super Thing name {super_schedule_msg.super_thing_name} is not matched...', 'red')
+            return False
+        if self._middleware_name != super_schedule_msg.super_middleware_name:
+            MXLOG_DEBUG(f'[{get_current_function_name()}] Super Middleware name {super_schedule_msg.super_middleware_name} is not matched...', 'red')
+            return False
+        if super_schedule_msg.topic_error or super_schedule_msg.payload_error:
+            MXLOG_DEBUG(f'[{get_current_function_name()}] super_schedule_msg Message has error!', 'red')
+            return False
+        if not self._check_super_service_exist(target_super_service):
+            MXLOG_DEBUG(f'[{get_current_function_name()}] Super Service {target_super_service.get_name()} does not exist...', 'red')
+            return False
 
-            super_execute_request = target_super_function._mapping_table[super_request_key]
-            super_execute_request._super_arg_list = target_super_function.get_arg_list()
-            super_execute_request._trigger_msg = super_action_msg
-            super_action_request = super_execute_request
-
-        # super action 스레드 생성
-        if target_super_function:
-            super_action_request.timer_start()
-            target_super_function.super_action(
-                super_action_request, self._hierarchical_service_table)
+        schedule_thread = target_super_service.start_super_schedule_thread(super_schedule_msg, self._global_service_table, timeout=1000)
+        if not schedule_thread:
+            return False
+        elif schedule_thread.is_alive():
             return True
-        # 만약 타켓 함수가 없다면 에러를 출력한다.
         else:
-            SOPLOG_DEBUG(
-                f'Function {super_action_request._trigger_msg._super_function_name} is not exist', 'red')
             return False
 
-    def _handle_MS_SUPER_RESULT_ACTION(self, subrequest_key: str, super_action_result_msg: Union[SoPSubScheduleResultMessage, SoPSubExecuteResultMessage]):
-        target_super_function = self._find_function(
-            super_action_result_msg._super_function_name)
-
-        super_request_key = make_super_request_key(
-            super_action_result_msg._requester_middleware_name, super_action_result_msg._scenario)
-        target_super_function.put_subaction_result(
-            super_request_key, subrequest_key, super_action_result_msg)
-
-    def _handle_MS_SCHEDULE(self, msg: mqtt.MQTTMessage):
-        super_schedule_msg = SoPSuperScheduleMessage(msg)
-        super_schedule_msg.set_timestamp()
-        self._handle_MS_SUPER_ACTION(super_schedule_msg)
+    def _handle_MS_EXECUTE(self, msg: mqtt.MQTTMessage) -> bool:
+        super_execute_msg = MXSuperExecuteMessage(msg)
+        target_super_service = self._get_function(super_execute_msg.super_service_name)
+
+        if not target_super_service:
+            MXLOG_DEBUG(f'[{get_current_function_name()}] Super Service {super_execute_msg.super_service_name} does not exist...', 'red')
+            return False
+        if self._name != super_execute_msg.super_thing_name:
+            MXLOG_DEBUG(f'[{get_current_function_name()}] Super Thing name {super_execute_msg.super_thing_name} is not matched...', 'red')
+            return False
+        if self._middleware_name != super_execute_msg.super_middleware_name:
+            MXLOG_DEBUG(f'[{get_current_function_name()}] Super Middleware name {super_execute_msg.super_middleware_name} is not matched...', 'red')
+            return False
+        if super_execute_msg.topic_error or super_execute_msg.payload_error:
+            MXLOG_DEBUG(f'[{get_current_function_name()}] super_execute_msg Message has error!', 'red')
+            return False
+
+        # 중복된 시나리오로부터 온 실행 요청이면 -4 에러코드를 보낸다.
+        if super_execute_msg.scenario in target_super_service.get_running_scenario_list():
+            target_super_service._send_SM_RESULT_EXECUTE(super_service_name=super_execute_msg.super_service_name,
+                                                         super_thing_name=super_execute_msg.super_thing_name,
+                                                         super_middleware_name=super_execute_msg.super_middleware_name,
+                                                         requester_middleware_name=super_execute_msg.requester_middleware_name,
+                                                         scenario=super_execute_msg.scenario,
+                                                         error=MXErrorCode.DUPLICATE)
+            return True
+
+        super_execute_thread = target_super_service.start_super_execute_thread(super_execute_msg, self._SUPER_SERVICE_REQUEST_KEY_TABLE)
+        if not super_execute_thread:
+            return False
+        else:
+            return True
 
-    def _handle_MS_RESULT_SCHEDULE(self, msg: mqtt.MQTTMessage):
-        subschedule_result_msg = SoPSubScheduleResultMessage(msg)
+    def _handle_MS_RESULT_SCHEDULE(self, msg: mqtt.MQTTMessage) -> bool:
+        subschedule_result_msg = MXSubScheduleResultMessage(msg)
         subschedule_result_msg.set_timestamp()
-        subrequest_key = make_sub_request_key(
-            subschedule_result_msg._subfunction_name, subschedule_result_msg._subrequest_order)
-        self._handle_MS_SUPER_RESULT_ACTION(
-            subrequest_key, (subschedule_result_msg))
-
-    def _handle_MS_EXECUTE(self, msg: mqtt.MQTTMessage):
-        super_execute_msg = SoPSuperExecuteMessage(msg)
-        super_execute_msg.set_timestamp()
-        self._handle_MS_SUPER_ACTION(super_execute_msg)
-
-    def _handle_MS_RESULT_EXECUTE(self, msg: mqtt.MQTTMessage):
-        subexecute_result_msg = SoPSubExecuteResultMessage(msg)
-        subexecute_result_msg.set_timestamp()
-        subrequest_key = make_sub_request_key(
-            subexecute_result_msg._subfunction_name, subexecute_result_msg._subrequest_order)
-        self._handle_MS_SUPER_RESULT_ACTION(
-            subrequest_key, subexecute_result_msg)
-
-    def _handle_MS_RESULT_SERVICE_LIST(self, msg: mqtt.MQTTMessage):
-        service_list = SoPServiceListResultMessage(msg)
-        service_list.set_timestamp()
+        super_service_request_key = make_super_request_key(scenario_name=subschedule_result_msg.scenario,
+                                                           requester_middleware_name=subschedule_result_msg.requester_middleware_name,)
+        sub_service_request_key = make_sub_service_request_key(sub_service_name=subschedule_result_msg.sub_service_name,
+                                                               sub_service_request_order=subschedule_result_msg.sub_service_request_order)
+
+        target_super_service = self._get_function(subschedule_result_msg.super_service_name)
+        if not target_super_service:
+            MXLOG_DEBUG(f'[{get_current_function_name()}] Super Service {subschedule_result_msg.super_service_name} does not exist...', 'yellow')
+            return False
+
+        result = target_super_service.put_subschedule_result(super_service_request_key, sub_service_request_key, subschedule_result_msg)
+        return result
+
+    def _handle_MS_RESULT_EXECUTE(self, msg: mqtt.MQTTMessage) -> bool:
+        sub_service_execute_result_msg = MXSubExecuteResultMessage(msg)
+        sub_service_execute_result_msg.set_timestamp()
+        super_service_request_key = make_super_request_key(scenario_name=sub_service_execute_result_msg.scenario,
+                                                           requester_middleware_name=sub_service_execute_result_msg.requester_middleware_name)
+        sub_service_request_key = make_sub_service_request_key(sub_service_name=sub_service_execute_result_msg.sub_service_name,
+                                                               sub_service_request_order=sub_service_execute_result_msg.sub_service_request_order)
+
+        target_super_service = self._get_function(sub_service_execute_result_msg.super_service_name)
+        if not target_super_service:
+            MXLOG_DEBUG(f'[{get_current_function_name()}] Super Service {sub_service_execute_result_msg.super_service_name} does not exist...', 'yellow')
+            return False
 
+        result = target_super_service.put_sub_service_execute_result(super_service_request_key, sub_service_request_key, sub_service_execute_result_msg)
+        return result
+
+    def _handle_MS_RESULT_SERVICE_LIST(self, msg: mqtt.MQTTMessage) -> bool:
         try:
-            for middleware in service_list.service_list():
-                middleware_name = middleware['middleware']
+            service_list = MXSuperServiceListResultMessage(msg)
+            service_list.set_timestamp()
+
+            for middleware in service_list.service_list:
                 hierarchy_type = middleware['hierarchy']
+                if not hierarchy_type in ['local', 'child']:
+                    MXLOG_DEBUG(f'[{get_current_function_name()}] Parent middleware is not supported', 'red')
+                    return False
+
+                middleware_name = middleware['middleware']
+                if not middleware_name:
+                    MXLOG_DEBUG(f'[{get_current_function_name()}] Middleware name does not exist', 'red')
+                    return False
+
                 thing_list = middleware['things']
                 for thing in thing_list:
                     is_alive = thing['is_alive']
                     if is_alive != 1:
                         continue
+
                     is_super = thing['is_super']
-                    # alive_cycle = thing['alive_cycle']
-                    thing_name = thing['name']
-                    value_list = thing['values']
-                    function_list = thing['functions']
+                    alive_cycle = thing['alive_cycle']
 
                     # value 정보를 추출
-                    for value_info in value_list:
-                        value_tag_list = [SoPTag(tag['name'])
-                                          for tag in value_info['tags']]
-
-                        # TODO: energy, cycle info is omit in service list
-                        value_service = SoPValue(name=value_info['name'],
-                                                 thing_name=thing_name,
-                                                 middleware_name=middleware_name,
-                                                 tag_list=value_tag_list,
-                                                 desc=value_info['description'],
-                                                 func=None,
-                                                 energy=None,
-                                                 type=SoPType.get(
-                            value_info['type']),
-                            bound=(float(value_info['bound']['min_value']),
-                                   float(value_info['bound']['max_value'])),
-                            format=value_info['format'],
-                            cycle=None)
-                        if value_service not in self._hierarchical_service_table['value']:
-                            self._hierarchical_service_table['value'].append(
-                                value_service)
-
-                    # function 정보를 추출
-                    for function_info in function_list:
-                        function_tag_list = [SoPTag(tag['name'])
-                                             for tag in function_info['tags']]
-                        arg_list = []
-                        if bool(function_info['use_arg']):
-                            for argument in function_info['arguments']:
-                                arg_list.append(SoPArgument(name=argument['name'],
-                                                            type=SoPType.get(
-                                                                argument['type']),
-                                                            bound=(float(argument['bound']['min_value']),
-                                                                   float(argument['bound']['max_value']))))
-                        function_service = SoPFunction(name=function_info['name'],
-                                                       thing_name=thing_name,
-                                                       middleware_name=middleware_name,
-                                                       tag_list=function_tag_list,
-                                                       desc=function_info['description'],
-                                                       func=None,
-                                                       energy=None,
-                                                       arg_list=arg_list,
-                                                       return_type=SoPType.get(
-                                                           function_info['return_type']),
-                                                       exec_time=function_info['exec_time'],
-                                                       timeout=None)
-                        if function_service not in self._hierarchical_service_table['function']:
-                            self._hierarchical_service_table['function'].append(
-                                function_service)
+                    value_service_list = self._extract_value_info(thing=thing, middleware_name=middleware_name)
+                    self._global_service_table['values'].extend(value_service_list)
+
+                    function_service_list = self._extract_function_info(thing_info=thing, middleware_name=middleware_name)
+                    self._global_service_table['functions'].extend(function_service_list)
 
             self._last_refresh_time = get_current_time()
+            return True
         except KeyError as e:
             print_error(e)
-            SOPLOG_DEBUG('[handle_MS_RESULT_SERVICE_LIST] KeyError', 'red')
+            MXLOG_DEBUG(f'[{get_current_function_name()}] KeyError', 'red')
+            return False
         except ValueError as e:
             print_error(e)
-            SOPLOG_DEBUG('[handle_MS_RESULT_SERVICE_LIST] ValueError', 'red')
+            MXLOG_DEBUG(f'[{get_current_function_name()}] ValueError', 'red')
+            return False
         except Exception as e:
             print_error(e)
-            SOPLOG_DEBUG(
-                '[handle_MS_RESULT_SERVICE_LIST] Unknown Exception', 'red')
+            MXLOG_DEBUG(
+                f'[{get_current_function_name()}] Unknown Exception', 'red')
+            return False
 
     # ===================
     #   __  __   ______
     #  |  \/  | |  ____|
     #  | \  / | | |__
     #  | |\/| | |  __|
     #  | |  | | | |____
     #  |_|  |_| |______|
     # ===================
 
     def _handle_ME_NOTIFY(self, msg: mqtt.MQTTMessage):
-        notify_msg = SoPNotifyMessage(msg)
+        notify_msg = MXNotifyMessage(msg)
         notify_msg.set_timestamp()
         self._send_SM_REFRESH()
 
     # ================
     #  _____ ___  ___
     # /  ___||  \/  |
     # \ `--. | .  . |
     #  `--. \| |\/| |
     # /\__/ /| |  | |
     # \____/ \_|  |_/
     # ================
 
-    def _send_SM_SCHEDULE(self, subfunction_name: str, thing_name: str, middleware_name: str, super_thing_name: str,
-                          scenario_name: str, period: float):
-        self._publish_queue.put(SoPSubScheduleMessage(subfunction_name, thing_name,
-                                middleware_name, super_thing_name, scenario_name, period).mqtt_message())
-
-    # TODO: complete this function
-    def _send_SM_EXECUTE(self, subfunction_name: str, target_thing_name: str, target_middleware_name: str, super_thing_name: str,
-                         scenario_name: str, arguments: Tuple):
-        self._publish_queue.put(SoPSubExecuteMessage(subfunction_name, target_thing_name,
-                                target_middleware_name, super_thing_name, scenario_name, arguments).mqtt_message())
-
-    def _send_SM_RESULT_SCHEDULE(self, super_function_name: str, super_thing_name: str, super_middleware_name: str, requester_middleware_name: str,
-                                 scenario_name: str, error: SoPErrorType):
-        self._publish_queue.put(SoPSuperScheduleResultMessage(super_function_name, super_thing_name, super_middleware_name, requester_middleware_name,
-                                                              scenario_name, error).mqtt_message())
-
-    def _send_SM_RESULT_EXECUTE(self, super_function_name: str, super_thing_name: str, super_middleware_name: str, requester_middleware_name: str,
-                                scenario: str, return_type: SoPType, return_value: Union[int, float, bool, str], error: SoPErrorType):
-        self._publish_queue.put(SoPSuperExecuteResultMessage(super_function_name, super_thing_name, super_middleware_name, requester_middleware_name,
-                                                             scenario, return_type, return_value, error).mqtt_message())
-
-    def _send_SM_AVAILABILITY(self):
-        self._publish_queue.put(SoPAvailablityMessage(
-            self._name, self._dump_availablity()).mqtt_message())
+    def _send_SM_EXECUTE(self, sub_service_execute_msg: MXSubExecuteMessage) -> None:
+        sub_service_execute_mqtt_msg = sub_service_execute_msg.mqtt_message()
+        self._publish_queue.put(sub_service_execute_mqtt_msg)
 
     def _send_SM_REFRESH(self):
-        self._publish_queue.put(SoPRefreshMessage(self._name).mqtt_message())
+        super_refresh_msg = self._generate_super_refresh_message()
+        super_refresh_mqtt_msg = super_refresh_msg.mqtt_message()
+        self._publish_queue.put(super_refresh_mqtt_msg)
 
     # ========================
     #         _    _  _
     #        | |  (_)| |
     #  _   _ | |_  _ | | ___
     # | | | || __|| || |/ __|
     # | |_| || |_ | || |\__ \
     #  \__,_| \__||_||_||___/
     # ========================
 
-    # def schedule(self, schedule_request: SoPScheduleRequest):
-    #     self._thread = SoPThread(
-    #         func=self.schedule_thread_func,
-    #         daemon=True,
-    #         arg_list=(schedule_request, ))
-    #     self._thread.start()
-
-    # def find_super_function_service(self, super_function_service_name):
-    #     for function in self._function_list:
-    #         if function.get_name() == super_function_service_name:
-    #             return function
-
-    # def _catch_subexecute_result_parallel(self, super_request_key: str, target_super_function: SoPSuperFunction, timeout: float = 10):
-    #     result_list: List[dict] = []
-    #     reqline_execution_result_list: List[List[SoPSubExecuteResultMessage]] = [
-    #     ]
-    #     super_execute_request = target_super_function._mapping_table[super_request_key]
-    #     subrequest_key = make_sub_request_key(
-    #         subfunction_name, super_execute_request._current_reqline_num)
-    #     # TODO: 여기서 다 돌지마라.. 3개 다 뺴버리니까
-    #     for subrequest_key, subfunction_reqline in super_execute_request._subfunction_reqline_table.items():
-    #         reqline_execution_result_list.append(super_execute_request.get_subexecute_result_msg_list(
-    #             subrequest_key, timeout))
-    #         SOPLOG_DEBUG(f'get_subresult_msg: {reqline_execution_result_list}')
-
-    #     for sub_execution_result_list in reqline_execution_result_list:
-    #         for sub_execution_result in sub_execution_result_list:
-    #             result_list.append(dict(scenario=sub_execution_result._scenario,
-    #                                     return_type=sub_execution_result._return_type,
-    #                                     return_value=sub_execution_result._return_value,
-    #                                     error=sub_execution_result._error))
-    #     return result_list
+    def _generate_super_refresh_message(self) -> MXSuperRefreshMessage:
+        super_refresh_msg = MXSuperRefreshMessage(self)
+        return super_refresh_msg
 
-    def _find_function(self, function_name: str) -> SoPSuperFunction:
+    @override
+    def _get_function(self, function_name: str) -> MXSuperFunction:
         for function in self._function_list:
             if function.get_name() == function_name:
                 return function
 
-    def _request_subexecute_nonparallel(self, subexecute_request_list, mapping_table: Dict[str, List[SoPFunction]], subfunction_name: str, arg_list: Tuple, result_list: List[dict]):
-        for target_scenario, target_subfunction_list in mapping_table.items():
-            for target_subfunction in target_subfunction_list:
-                if subfunction_name == target_subfunction.get_name():
-                    self._subscribe(SoPProtocolType.Super.MS_RESULT_EXECUTE.value % (target_subfunction.get_name(),
-                                                                                     target_subfunction.get_thing_name(),
-                                                                                     target_subfunction.get_middleware_name(),
-                                                                                     self._name))
-                    json_arg_list = [dict(order=i, value=arg)
-                                     for i, arg in enumerate(arg_list)]
-                    self._send_SM_EXECUTE(target_subfunction.get_name(),
-                                          target_subfunction.get_thing_name(),
-                                          target_subfunction.get_middleware_name(),
-                                          self._name,
-                                          target_scenario,
-                                          json_arg_list)
-                    # 하나의 subfunction의 subexecute 결과를 받을 때까지 기다린다. 이후 다음 subfunction에게 subexecute 요청을 보내고 받는 것을 반복.
-                    self._catch_subexecute_result_nonparallel(
-                        subexecute_request_list, target_subfunction, result_list)
-
-    def _catch_subexecute_result_nonparallel(self, subexecute_request_list: List[dict], target_subfunction: SoPFunction, result_list: List[dict]):
-        for subexecute_request in subexecute_request_list:
-            subexecute_msg: SoPSubExecuteMessage = subexecute_request['subexecute_msg']
-            subexecute_request['end_time'] = time.time()
-            subfunction_check = subexecute_msg._subfunction_name == target_subfunction.get_name()
-            target_thing_check = subexecute_msg._target_thing_name == target_subfunction.get_thing_name()
-            target_middleware_check = subexecute_msg._target_middleware_name == target_subfunction.get_middleware_name()
-            super_thing_check = subexecute_msg._super_thing_name == self._name
-            # self._subexecute_request_list에 있는 request중에 target_subfunction에 해당하는 요청에 대한 결과를 찾는다.
-            if subfunction_check and target_thing_check and target_middleware_check and super_thing_check:
-                result_queue: Queue = subexecute_request['result_queue']
-                subexecute_result_msg: SoPSubExecuteResultMessage = result_queue.get()
-                SOPLOG_DEBUG(
-                    f'[SUBEXECUTE END] {subexecute_result_msg._subfunction_name}|{subexecute_result_msg._target_thing_name} duration: {(subexecute_request["end_time"] - subexecute_request["start_time"]):.4f}', 'cyan')
-
-                self._unsubscribe_queue.put(
-                    subexecute_result_msg.topic())
-                while not self._unsubscribe_queue.empty():
-                    time.sleep(THREAD_TIME_OUT)
-
-                result_list.append(dict(
-                    scenario=subexecute_result_msg._scenario,
-                    return_type=subexecute_result_msg._return_type,
-                    return_value=subexecute_result_msg._return_value,
-                    error=subexecute_result_msg._error))
-
-    # def request_function_service(self, super_request_key: str, target_super_function: SoPSuperFunction, subfunction_name: str, timeout=10) -> Union[List[dict], bool]:
-    #     result_list = []
-
-    #     # 병렬 요청 옵션. _super_execute_wrapper안에서 병렬로 보냈던 subexecute 요청에 대한 결과를 수집한다.
-    #     if target_super_function._request_parallel:
-    #         result_list = self._catch_subexecute_result_parallel(
-    #             super_request_key, target_super_function, timeout=timeout)
-
-    #         if len(result_list) == 0:
-    #             raise Exception('Result_list is empty')
-    #         else:
-    #             return result_list
-    #     # 직렬 요청 옵션. 하나씩 subexecute요청을 보내고 그에 대한 결과를 받는다.
-    #     else:
-    #         # TODO: implement
-    #         # mapping_table에 저장된 subfunction중 현재 request_function_service이 요청하고자하는 subfunction을 찾는다.
-    #         pass
-
-    #     return result_list
-
-    # execute service via super service
-    def req(self, super_request_key: str, subfunction_name: str = '', arg_list: Union[Tuple[SoPArgument], Tuple] = None, tag_list: List[str] = [],
-            service_type: SoPServiceType = SoPServiceType.FUNCTION, policy: SoPPolicy = SoPPolicy.SINGLE,
-            timeout=1000) -> Union[List[dict], bool]:
-        super_function_name = inspect.currentframe().f_back.f_code.co_name
-        target_super_function = self._find_function(super_function_name)
-        # str 타입의 태그를 SoPTag로 변환
-        tag_list = [SoPTag(str_tag) for str_tag in tag_list]
+    @override
+    def _subscribe_init_topic_list(self):
+        super()._subscribe_init_topic_list()
 
-        try:
-            if service_type == SoPServiceType.VALUE:
-                subfunction_name = f'__{subfunction_name}'
-            elif service_type == SoPServiceType.FUNCTION:
-                pass
-            else:
-                SOPLOG_DEBUG(f'Invalid service type: {service_type}', 'red')
-                raise Exception
+        topic_list = [MXProtocolType.Super.MS_RESULT_SERVICE_LIST.value % "#"]
 
-            # super thing을 init할 때 자신이 가지고 있는 super function에 대한 정보를 추출한다.
-            if target_super_function.get_first_execute():
-                target_super_function.add_subfunction_reqline_info(
-                    subfunction_name, arg_list, tag_list, policy)
-            else:
-                super_execute_request = target_super_function._mapping_table[super_request_key]
-                subrequest_key = make_sub_request_key(
-                    subfunction_name, super_execute_request._current_reqline_num)
-                result_msg_list = super_execute_request.get_subexecute_result_msg_list(
-                    subrequest_key=subrequest_key, timeout=timeout)
-                super_execute_request._current_reqline_num += 1
-                result_list = [dict(scenario=result_msg._scenario,
-                                    return_type=result_msg._return_type,
-                                    return_value=result_msg._return_value,
-                                    error=result_msg._error) for result_msg in result_msg_list]
-                return result_list
-                # return self.request_function_service(super_request_key=super_request_key,
-                #                                      target_super_function=target_super_function,
-                #                                      subfunction_name=subfunction_name,
-                #                                      timeout=timeout)
+        for topic in topic_list:
+            self._subscribe(topic)
 
-        except Exception as e:
-            print_error(e)
-            return False
+    @override
+    def _subscribe_service_topic_list(self):
+        for function in self._function_list:
+            # Super Schedule, Super Execute에 필요한 토픽들을 미리 구독을 해놓는다.
+            topic_list = [MXProtocolType.Super.MS_SCHEDULE.value % (function.get_name(), self._name, self._middleware_name, '#'),
+                          MXProtocolType.Super.MS_RESULT_SCHEDULE.value % (
+                              '+', '+', '#'),
+                          MXProtocolType.Super.MS_EXECUTE.value % (
+                              function.get_name(), self._name, self._middleware_name, '#'),
+                          MXProtocolType.Super.MS_RESULT_EXECUTE.value % (
+                              '+', '+', '#')]
 
-    # execute scenario line
-    def r(self, line: str = None, *arg_list) -> Union[List[dict], bool]:
-        super_service_name = inspect.currentframe().f_back.f_code.co_name
+            for topic in topic_list:
+                self._subscribe(topic)
 
-        scope_policy = 'all' if 'all' in line else 'single'
-        function_name = line.split('.')[1][0:line.split('.')[1].find('(')]
-        braket_parse: List[str] = re.findall(r'\(.*?\)', line)
-        tags = [tag[1:] for tag in braket_parse[0][1:-1].split(' ')]
+    def _request_sub_service_execute(self, sub_service_execute_request: MXSubExecuteRequest) -> None:
+        if not isinstance(sub_service_execute_request, MXSubExecuteRequest):
+            raise MXTypeError(f'[{get_current_function_name()}] Invalid type of sub_service_execute_request: {type(sub_service_execute_request)}')
+
+        sub_service_execute_msg = sub_service_execute_request.trigger_msg
+        self._send_SM_EXECUTE(sub_service_execute_msg)
+
+    # 하나의 sub_service_request에 있는 sub_service_execute_request들을 병렬로 실행한다.
+    def _sub_service_execute_parallel(self, sub_service_execute_request_list: List[MXSubExecuteRequest], arg_list: List[Union[int, float, str, bool]]) -> List[Union[int, float, str, bool]]:
+        result_list = []
+        for i, sub_service_execute_request in enumerate(sub_service_execute_request_list):
+            sub_service_execute_request.timer_start()
+            sub_service_execute_request.trigger_msg.arguments = tuple(arg_list)
+
+            sub_service_execute_msg = sub_service_execute_request.trigger_msg
+            MXLOG_DEBUG(f'[SUB_EXECUTE START] {sub_service_execute_msg.sub_service_name}|{sub_service_execute_msg.target_middleware_name}|{sub_service_execute_msg.scenario}|{i}', 'cyan')
+            self._request_sub_service_execute(sub_service_execute_request)
+
+        for i, sub_service_execute_request in enumerate(sub_service_execute_request_list):
+            sub_service_execute_request.result_msg = sub_service_execute_request.get_result_msg()
+            sub_service_execute_request.timer_end()
+            rc_msg = sub_service_execute_request.result_msg
+
+            sub_service_execute_msg: MXSubExecuteMessage = sub_service_execute_request.trigger_msg
+            sub_service_execute_result_msg: MXSubExecuteResultMessage = sub_service_execute_request.result_msg
+            result_list.append(dict(scenario=sub_service_execute_result_msg.scenario,
+                                    return_type=sub_service_execute_result_msg.return_type,
+                                    return_value=sub_service_execute_result_msg.return_value,
+                                    error=sub_service_execute_result_msg.error))
+
+            MXLOG_DEBUG(
+                f'[SUB_EXECUTE END] {sub_service_execute_msg.sub_service_name}|{sub_service_execute_msg.target_middleware_name}|{sub_service_execute_msg.scenario}|{i}'
+                f'duration: {sub_service_execute_request.duration():.4f} Sec', 'cyan')
+
+        return result_list
+
+    def _get_sub_service_from_global_service_table(self, sub_service_name: str) -> MXFunction:
+        for function in self._global_service_table['functions']:
+            if function.get_name() == sub_service_name:
+                return function
+        return None
 
-        argments = []
-        for braket_inner_element in braket_parse[1][1:-1].split(','):
-            braket_inner_element = braket_inner_element.strip(' ')
-            if braket_inner_element == '':
-                continue
-            else:
-                argments.append(braket_inner_element)
+    def _check_sub_service_callable(self, sub_service_name: str, return_type: MXType):
+        global_sub_service = self._get_sub_service_from_global_service_table(sub_service_name)
+        if not global_sub_service:
+            return False
+        if not global_sub_service.get_return_type() == return_type:
+            return False
 
-        for i, arg in enumerate(argments):
-            if '$' in arg:
-                index = int(arg[1:])
-                argments[i] = arg_list[index-1]
+        return True
 
-        argments = tuple(argments)
+    def _check_req_valid(self, sub_service_name: str, tag_list: List[str], arg_list: Union[Tuple[MXArgument], Tuple],
+                         return_type: MXType, service_type: MXServiceType, range_type: MXRangeType):
+        if not sub_service_name:
+            raise MXValueError(f'sub_service_name must be not empty')
+        if not tag_list:
+            raise MXValueError(f'tag_list must be not empty')
+        if not all(tag_list):
+            raise MXValueError(f'tag in tag_list must be not empty string')
+        if not service_type in [MXServiceType.VALUE, MXServiceType.FUNCTION]:
+            raise MXTypeError(f'Invalid service_type: {service_type}')
+        if not return_type in [MXType.INTEGER, MXType.DOUBLE, MXType.STRING, MXType.BOOL, MXType.BINARY, MXType.VOID]:
+            raise MXTypeError(f'Invalid return_type: {return_type}')
+        elif service_type == MXServiceType.VALUE and return_type == MXType.VOID:
+            raise MXTypeError(f'Value service cannot have a return_type of void')
+        if not range_type in [MXRangeType.SINGLE, MXRangeType.ALL]:
+            raise MXTypeError(f'Invalid range_type: {range_type}')
 
-        # TODO: Update this function
-        # result_list = self.request_function_service(tag_list=tags, subfunction_name=function_name, arg_list=argments,
-        #                                             super_function_name=super_service_name, policy=scope_policy)
-        # return result_list
+        return True
 
-    # override
-    def _subscribe_init_topics(self, thing: SoPThing):
-        super()._subscribe_init_topics(thing)
+    def _check_req_return_type(self, sub_service_return_type: MXType, req_return_type: MXType, service_type: MXServiceType):
+        if req_return_type in [MXType.INTEGER, MXType.DOUBLE] and sub_service_return_type in [MXType.INTEGER, MXType.DOUBLE]:
+            return True
+        elif req_return_type == MXType.VOID and service_type == MXServiceType.VALUE:
+            raise MXTypeError(f'Not matched return_type. Value service cannot have a return_type of void: {sub_service_return_type}')
+        elif req_return_type != sub_service_return_type:
+            raise MXTypeError(f'Not matched return_type: {sub_service_return_type} != {req_return_type}')
+
+        return True
+
+    def _check_super_service_exist(self, super_service: MXSuperFunction):
+        return all([self._check_sub_service_callable(sub_service_request._sub_service_type.get_name(), sub_service_request._sub_service_type.get_return_type())
+                    for sub_service_request in super_service._sub_service_request_list])
+
+    def req(self, sub_service_name: str, tag_list: List[str], arg_list: Union[Tuple[MXArgument], Tuple] = [],
+            return_type: MXType = MXType.UNDEFINED, service_type: MXServiceType = MXServiceType.FUNCTION,
+            range_type: MXRangeType = MXRangeType.SINGLE) -> Union[List[dict], bool]:
+        # Detect fatal errors.
+        # If an error occurs, the program terminates by raising an exception.
+        if not self._check_req_valid(sub_service_name=sub_service_name, tag_list=tag_list, arg_list=arg_list, return_type=return_type,
+                                     service_type=service_type, range_type=range_type):
+            return False
 
-        topic_list = [SoPProtocolType.Super.MS_RESULT_SERVICE_LIST.value % "#"]
+        super_service_name = get_upper_function_name()
+        target_super_service = self._get_function(super_service_name)
+        target_sub_service = self._get_sub_service_from_global_service_table(sub_service_name)
+
+        # Convert tag of type [str] to [MXTag]
+        tag_list = [MXTag(str_tag) for str_tag in tag_list]
+
+        if service_type == MXServiceType.VALUE:
+            sub_service_name = f'__{sub_service_name}'
+        elif service_type == MXServiceType.FUNCTION:
+            sub_service_name = sub_service_name
+
+        # When initiate a super thing, extract information about the super service.
+        if not target_super_service.get_is_scanned():
+            target_super_service.add_sub_service_request_info(sub_service_name=sub_service_name,
+                                                              arg_list=arg_list,
+                                                              tag_list=tag_list,
+                                                              return_type=return_type,
+                                                              range_type=range_type)
+            return []
+        else:
+            if not self._check_sub_service_callable(sub_service_name, return_type):
+                MXLOG_DEBUG(f'sub_service {sub_service_name} is not callable', 'red')
+                return False
+            if not self._compare_arg_list(target_sub_service.get_arg_list(), list(arg_list)):
+                MXLOG_DEBUG(f'Not matched arg_list')
+                return False
+            if not self._check_req_return_type(target_sub_service.get_return_type(), req_return_type=return_type, service_type=service_type):
+                MXLOG_DEBUG(f'Not matched return_type')
+                return False
 
-        for topic in topic_list:
-            self._subscribe(topic)
+            current_thread = threading.current_thread()
+            scenario_name = current_thread.user_data['scenario']
+            requester_middleware_name = current_thread.user_data['requester_middleware']
+            # super_service_request_key = scenario_name@requester_middleware_name
+            super_service_request_key = make_super_request_key(scenario_name, requester_middleware_name)
+
+            MXLOG_DEBUG(f'[DEBUG] before pop SUPER_SERVICE_REQUEST_KEY_TABLE: \n{dict_to_json_string(self._SUPER_SERVICE_REQUEST_KEY_TABLE, pretty=True)}'
+                        f'\n super_service_request_key: {super_service_request_key} ')
+            sub_service_request_key_list = self._SUPER_SERVICE_REQUEST_KEY_TABLE[super_service_request_key]
+            # sub_service_request_key = sub_service_name@sub_service_request_order
+            sub_service_request_key = sub_service_request_key_list.pop(0)
+            MXLOG_DEBUG(f'[DEBUG] after pop SUPER_SERVICE_REQUEST_KEY_TABLE: \n{dict_to_json_string(self._SUPER_SERVICE_REQUEST_KEY_TABLE, pretty=True)}'
+                        f'\n super_service_request_key: {super_service_request_key} ')
+            if len(sub_service_request_key_list) == 0:
+                self._SUPER_SERVICE_REQUEST_KEY_TABLE.pop(super_service_request_key)
 
-    # override
-    def _subscribe_service_topics(self, thing: SoPThing):
-        for function in thing.get_function_list():
-            topic_list = [SoPProtocolType.Super.MS_EXECUTE.value % (function.get_name(), thing.get_name(), thing.get_middleware_name(), '#'),
-                          SoPProtocolType.Super.MS_SCHEDULE.value % (
-                function.get_name(), thing.get_name(), thing.get_middleware_name(), '#')]
+            super_service_execute_request = target_super_service._mapping_table[super_service_request_key]
+            sub_service_execute_request_list = super_service_execute_request._sub_service_request_table[sub_service_request_key]._target_request_list
 
-            for topic in topic_list:
-                self._subscribe(topic)
+            result_list = self._sub_service_execute_parallel(sub_service_execute_request_list, arg_list)
+            return result_list
 
-    def _dump_availablity(self) -> Dict:
-        super_function_list = []
+    # TODO: implement this
+    def r(self, line: str = None, *arg_list) -> Union[List[dict], bool]:
+        super_service_name = get_upper_function_name()
 
-        for function in self._function_list:
-            subfunction_list = []
+        range_type = 'all' if 'all' in line else 'single'
+        function_name = line.split('.')[1][0:line.split('.')[1].find('(')]
+        bracket_parse: List[str] = re.findall(r'\(.*?\)', line)
+        tags = [tag[1:] for tag in bracket_parse[0][1:-1].split(' ')]
 
-            for subfunction_reqline in function.get_subfunction_type_list():
-                available_function_service_list = [
-                    function_service for function_service in self._hierarchical_service_table['function']]
-                subfunction_list.append(dict(name=subfunction_reqline._subfunction_type.get_name(),
-                                             status=1 if subfunction_reqline._subfunction_type in available_function_service_list else 0))
-
-            subfunction_status_list = [sub_function['status']
-                                       for sub_function in subfunction_list]
-            super_function_list.append(dict(name=function.get_name(),
-                                            status=0 if 0 in subfunction_status_list else 1,
-                                            sub_functions=subfunction_list))
-        availablity_info = dict(super_functions=super_function_list)
-
-        return availablity_info
-
-    def generate_random_arg(self, arg_list: List[SoPArgument]):
-        random_arg = []
-        for arg in arg_list:
-            if arg._type == SoPType.INTEGER:
-                random_arg.append(random.randint(arg._min, arg._max))
-            elif arg._type == SoPType.DOUBLE:
-                random_arg.append(random.uniform(arg._min, arg._max))
-            elif arg._type in [SoPType.STRING, SoPType.BINARY]:
-                import string
-                random_arg.append(''.join(random.choices(
-                    string.ascii_uppercase + string.digits, k=random.randint(arg._min, arg._max))))
-            elif arg._type == SoPType.BOOL:
-                random_arg.append(random.choice([True, False]))
+        arguments = []
+        for bracket_inner_element in bracket_parse[1][1:-1].split(','):
+            bracket_inner_element = bracket_inner_element.strip(' ')
+            if bracket_inner_element == '':
+                continue
             else:
-                SOPLOG_DEBUG('Unknown argument type')
+                arguments.append(bracket_inner_element)
 
-        return random_arg
+        for i, arg in enumerate(arguments):
+            if '$' in arg:
+                index = int(arg[1:])
+                arguments[i] = arg_list[index-1]
+
+        arguments = tuple(arguments)
 
-    def _extract_subfunction_reqline_info(self) -> None:
+    def _extract_sub_service_request_info(self) -> None:
         for function in self._function_list:
-            if self._is_super:
+            if self._is_super and not function.get_is_scanned():
                 arg_list = function.get_arg_list()
                 try:
-                    function._func(*tuple([None] + list(arg_list)))
-                except Exception as e:
-                    pass
-                function.set_first_execute(False)
+                    MXLOG_DEBUG(f'Detect super service: {function.get_name()}', 'green')
+                    function._func(*tuple(arg_list))
+                except MXError as e:
+                    # req를 실행하다가 MySSIXError와 관련된 에러가 발생한다는 것은 req명세가 잘못
+                    # 되었다는 것을 의미한다. 만약 MySSIXError에러가 아닌 다른 예외가 발생한 경우,
+                    # super service안에 있는 코드 중, req() 코드 부분이 아닌 코드에 의한 예외이므로
+                    # 정상적으로 req()에 대한 정보를 추출한 것이다.
+                    raise e
+                else:
+                    function.set_is_scanned(True)
+
+    def _extract_value_info(self, thing: dict, middleware_name: str) -> List[MXValue]:
+        thing_name = thing['name']
+        value_list = thing['values']
+
+        value_service_list = []
+        for value_info in value_list:
+            value_tag_list = [MXTag(tag['name']) for tag in value_info['tags']]
+
+            # TODO: cycle info is omit in service list
+            value_service = MXValue(func=dummy_func(arg_list=[]),
+                                    type=MXType.get(value_info['type']),
+                                    bound=(float(value_info['bound']['min_value']), float(value_info['bound']['max_value'])),
+                                    cycle=None,
+                                    name=value_info['name'],
+                                    tag_list=value_tag_list,
+                                    desc=value_info['description'],
+                                    thing_name=thing_name,
+                                    middleware_name=middleware_name,
+                                    format=value_info['format'] if not '(null)' in value_info['format'] else '')
+            if value_service not in self._global_service_table['values']:
+                value_service_list.append(value_service)
+
+        return value_service_list
+
+    def _extract_function_info(self, thing_info: dict, middleware_name: str) -> List[MXFunction]:
+        thing_name = thing_info['name']
+        function_list = thing_info['functions']
+
+        function_service_list = []
+        for function_info in function_list:
+            function_tag_list = [MXTag(tag['name']) for tag in function_info['tags']]
+            arg_list = []
+            if bool(function_info['use_arg']):
+                for argument in function_info['arguments']:
+                    arg_list.append(MXArgument(name=argument['name'],
+                                               type=MXType.get(argument['type']),
+                                               bound=(float(argument['bound']['min_value']), float(argument['bound']['max_value']))))
+
+            function_service = MXFunction(func=dummy_func(arg_list=arg_list),
+                                          return_type=MXType.get(function_info['return_type']),
+                                          name=function_info['name'],
+                                          tag_list=function_tag_list,
+                                          desc=function_info['description'],
+                                          thing_name=thing_name,
+                                          middleware_name=middleware_name,
+                                          arg_list=arg_list,
+                                          exec_time=function_info['exec_time'])
+            if function_service not in self._global_service_table['functions']:
+                function_service_list.append(function_service)
+
+        return function_service_list
 
     # ====================================
     #               _    _
     #              | |  | |
     #   __ _   ___ | |_ | |_   ___  _ __
     #  / _` | / _ \| __|| __| / _ \| '__|
     # | (_| ||  __/| |_ | |_ |  __/| |
     #  \__, | \___| \__| \__| \___||_|
     #   __/ |
     #  |___/
     # ====================================
 
+    @override
+    def get_function_list(self) -> List[MXSuperFunction]:
+        return self._function_list
+
     # ==================================
     #             _    _
     #            | |  | |
     #  ___   ___ | |_ | |_   ___  _ __
     # / __| / _ \| __|| __| / _ \| '__|
     # \__ \|  __/| |_ | |_ |  __/| |
     # |___/ \___| \__| \__| \___||_|
     # ==================================
+
+    @override
+    def set_function_list(self, function_list: List[MXSuperFunction]) -> None:
+        self._function_list = function_list
```

## big_thing_py/common/__init__.py

```diff
@@ -1,6 +1,4 @@
 from .common import *
 from .thread import *
 from .error import *
-from .soptype import *
-from .mqtt_message import *
-from .request import *
+from .mxtype import *
```

## big_thing_py/common/common.py

```diff
@@ -1,51 +1,53 @@
-from big_thing_py.common.error import *
-from big_thing_py.common.soptype import *
-
 from typing import *
+from typing_extensions import override
 from termcolor import *
 from abc import *
-from enum import Enum
+from enum import Enum, auto
 
 
-EMPTY_JSON = '{}'
-THREAD_TIME_OUT = 0.001
+EMPTY_JSON = {}
+THREAD_TIME_OUT = 0.0001
 
 
 class TimeFormat(Enum):
     DATETIME1 = '%Y-%m-%d %H:%M:%S'
     DATETIME2 = '%Y%m%d_%H%M%S'
     DATE = '%Y-%m-%d'
     TIME = '%H:%M:%S'
     UNIXTIME = 'unixtime'
 
 
-class SoPPrintMode(Enum):
-    FULL = 0
-    ABBR = 1
-    SKIP = 2
+class MXPrintMode(Enum):
+
+    def _generate_next_value_(name: str, start, count, last_values):
+        return name.lower()
+
+    UNDEFINED = auto()
+    FULL = auto()
+    ABBR = auto()
+    SKIP = auto()
+
+    @classmethod
+    def get(cls, name: str) -> 'MXPrintMode':
+        try:
+            return cls[name.upper()]
+        except Exception:
+            return cls.UNDEFINED
+
+
+class Direction(Enum):
+    PUBLISH = 'PUBLISH'
+    RECEIVED = 'RECEIVED'
 
 
 class PrintTag:
     # MQTT protocol
     GOOD = '[%-30s]' % colored('✔✔✔', 'green')
     DUP = '[%-30s]' % colored('DUP✔', 'green')
     ERROR = '[%-30s]' % colored('✖✖✖', 'red')
 
     CONNECT = '[%-30s]' % colored('-> CONNECT', 'blue')
     DISCONNECT = '[%-30s]' % colored('-> DISCONNECT', 'blue')
 
     SUBSCRIBE = '[%-30s]' % colored('-> SUBSCRIBE', 'white')
     UNSUBSCRIBE = '[%-30s]' % colored('-> UNSUBSCRIBE', 'white')
-
-
-class SoPPolicy(Enum):
-    UNDEFINED = -1
-    ALL = 'all'
-    SINGLE = 'single'
-
-    @classmethod
-    def get(cls, name: str):
-        try:
-            return cls[name.upper()]
-        except Exception:
-            return cls.UNDEFINED
```

## big_thing_py/common/error.py

```diff
@@ -1,22 +1,105 @@
-class NotSupportError(Exception):  # 사용자 정의 에러
-    def __init__(self, msg: str = ''):
-        self.msg = msg
+from enum import Enum, auto
+
+
+class MXErrorCode(Enum):
+    NO_ERROR = 0
+    FAIL = -1
+    TIMEOUT = -2
+    NO_PARALLEL = -3
+    DUPLICATE = -4
+    NOT_SUPPORTED = -5
+    INVALID_REQUEST = -7
+
+    REGISTER_NO_ERROR = -8
+    REGISTER_FAIL = -9
+    REGISTER_DUPLICATE = -10
+
+    EXECUTE_FAIL = -11
+    EXECUTE_TIMEOUT = -12
+    EXECUTE_NO_PARALLEL = -13
+    EXECUTE_DUPLICATE = -14
+
+    EXECUTE_ARG_FAIL = -15
+
+    VALUE_ERROR = -16
+    TYPE_ERROR = -18
+    NOT_FOUND_ERROR = -19
+
+    UNDEFINED = 'undefined'
+
+    @classmethod
+    def to_mx_error_code(cls, type: int):
+        if type is not None:
+            for mx_error_code in MXErrorCode:
+                if mx_error_code.value == type:
+                    return mx_error_code
+        else:
+            return MXErrorCode.get(type)
+
+    @classmethod
+    def get(cls, type: int) -> 'MXErrorCode':
+        try:
+            if type is not None:
+                for mx_error_type in MXErrorCode:
+                    if mx_error_type.value == type:
+                        return mx_error_type
+                return cls.UNDEFINED
+            else:
+                return MXErrorCode.get(type)
+        except Exception:
+            return cls.UNDEFINED
 
     def __str__(self):
-        return 'This feature is not support yet...\n' + self.msg
+        return self.name
 
 
-class SoPTypeError(Exception):  # 사용자 정의 에러
-    def __init__(self, msg: str = ''):
-        self.msg = msg
+class MXError(Exception):
+    def __init__(self, error_code: MXErrorCode, *args: object, **kwargs: dict) -> None:
+        super().__init__(*args, **kwargs)
+        self._error_code: MXErrorCode = error_code
 
-    def __str__(self):
-        return 'Only SoPType type is available.\n' + self.msg
 
+class MXFailError(MXError):
+    def __init__(self, *args: object, **kwargs: dict) -> None:
+        super().__init__(MXErrorCode.FAIL, *args, **kwargs)
 
-class ManagerModeError(Exception):
-    def __init__(self, msg: str = '') -> None:
-        self.msg = msg
 
-    def __str__(self):
-        return 'Only SoPManagerMode type is available.\n' + self.msg
+class MXTimeoutError(MXError):
+    def __init__(self, *args: object, **kwargs: dict) -> None:
+        super().__init__(MXErrorCode.TIMEOUT, *args, **kwargs)
+        self._error_code = MXErrorCode.TIMEOUT
+
+
+class MXNoParallelError(MXError):
+    def __init__(self, *args: object, **kwargs: dict) -> None:
+        super().__init__(MXErrorCode.NO_PARALLEL, *args, **kwargs)
+
+
+class MXDuplicatedError(MXError):
+    def __init__(self, *args: object, **kwargs: dict) -> None:
+        super().__init__(MXErrorCode.DUPLICATE, *args, **kwargs)
+
+
+class MXNotSupportedError(MXError):
+    def __init__(self, *args: object, **kwargs: dict) -> None:
+        super().__init__(MXErrorCode.NOT_SUPPORTED, *args, **kwargs)
+
+
+class MXInvalidRequestError(MXError):
+    def __init__(self, *args: object, **kwargs: dict) -> None:
+        super().__init__(MXErrorCode.INVALID_REQUEST, *args, **kwargs)
+
+
+class MXValueError(MXError):
+    def __init__(self, *args: object, **kwargs: dict) -> None:
+        super().__init__(MXErrorCode.VALUE_ERROR, *args, **kwargs)
+
+
+class MXTypeError(MXError):
+    def __init__(self, *args: object, **kwargs: dict) -> None:
+        super().__init__(MXErrorCode.TYPE_ERROR, *args, **kwargs)
+
+
+class MXNotFoundError(MXError):
+    def __init__(self, *args: object, **kwargs: dict) -> None:
+        super().__init__(MXErrorCode.NOT_FOUND_ERROR, *args, **kwargs)
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## big_thing_py/common/thread.py

```diff
@@ -1,55 +1,55 @@
 from big_thing_py.common.common import *
 
 from threading import Thread, Event, Lock
 from queue import Queue, Empty
 
 
-class SoPThread:
+class MXThread:
 
     class Mode(Enum):
         LOCK = 0
         EVENT = 1
 
-    def __init__(self, name: str = None, func: Callable = None, arg_list: Tuple = None, kwargs_list: dict = None, daemon: bool = True, mode: List[str] = []) -> None:
+    def __init__(self, name: str = None, target: Callable = None, args: Tuple = None, kwargs: dict = None, daemon: bool = True, mode: List[str] = []) -> None:
         self._name: str = name
-        self._func: Callable = func
-        self._arg_list: Tuple = arg_list
-        self._kwargs_list: dict = kwargs_list
+        self._target: Callable = target
+        self._args: Tuple = args
+        self._kwargs: dict = kwargs
         self._daemon: List[str] = daemon
 
         self._thread = Thread()
 
-        if func:
+        if target:
             self.set_thread()
         else:
-            raise Exception('[SoPThread] No function to run')
+            raise Exception('[MXThread] No function to run')
 
     def set_thread(self) -> None:
-        if isinstance(self._arg_list, tuple):
-            self._arg_list: list = list(self._arg_list)
+        if isinstance(self._args, tuple):
+            self._args: list = list(self._args)
         else:
-            self._arg_list = []
+            self._args = []
 
-        self._arg_list = tuple(self._arg_list)
+        self._args = tuple(self._args)
 
         if not self._name:
-            self._name = '_'.join(self._func.__name__.split('_')[:-1])
+            self._name = '_'.join(self._target.__name__.split('_')[:-1])
 
-        if self._kwargs_list:
+        if self._kwargs:
             self._thread = Thread(
-                target=self._func, name=self._name, kwargs=self._kwargs_list, daemon=self._daemon)
+                target=self._target, name=self._name, kwargs=self._kwargs, daemon=self._daemon)
         else:
             self._thread = Thread(
-                target=self._func, name=self._name, args=self._arg_list, daemon=self._daemon)
+                target=self._target, name=self._name, args=self._args, daemon=self._daemon)
 
     def start(self) -> None:
         self._thread.start()
 
     def join(self) -> None:
         self._thread.join()
-        
+
     def is_alive(self) -> bool:
         return self._thread.is_alive()
 
     def get_name(self) -> str:
         return self._name
```

## big_thing_py/core/argument.py

```diff
@@ -1,26 +1,59 @@
 from big_thing_py.utils import *
 
 
-class SoPArgument:
+class MXArgument:
 
-    def __init__(self, name: str = None, type: SoPType = None, bound: Tuple[float, float] = (None, None)):
-        self._name: str = name
-        self._type: SoPType = type
-        self._min: float = bound[0]
-        self._max: float = bound[1]
+    def __init__(self, name: str, type: MXType, bound: Tuple[float, float]):
+        self._name = name
+        self._type = type
+        self._min, self._max = bound
+
+        if not check_valid_identifier(self._name):
+            raise MXValueError(f'name cannot be empty & can only contain alphanumeric characters and underscores')
+
+        if self._min >= self._max:
+            raise MXValueError('bound must be min < max')
+
+        if self._type in [MXType.UNDEFINED, MXType.VOID]:
+            raise MXValueError('type cannot be undefined or void')
 
     def __str__(self) -> str:
         return self._name
 
-    def __eq__(self, o: object) -> bool:
-        return isinstance(o, SoPArgument) and o._name == self._name
+    def __eq__(self, o: 'MXArgument') -> bool:
+        instance_check = isinstance(o, MXArgument)
+        name_check = (o._name == self._name)
+        type_check = (o._type == self._type)
+        min_check = (o._min == self._min)
+        max_check = (o._max == self._max)
 
-    def dump(self) -> Dict:
+        return instance_check and name_check and type_check and min_check and max_check
+
+    def dict(self) -> dict:
         return {
-            "type": self._type.value,
-            "name": self._name,
-            "bound": {
-                "min_value": self._min,
-                "max_value": self._max
+            'name': self._name,
+            'type': self._type.value,
+            'bound': {
+                'min_value': self._min,
+                'max_value': self._max
             }
         }
+
+    def get_name(self) -> str:
+        return self._name
+
+    def get_type(self) -> MXType:
+        return self._type
+
+    def get_bound(self) -> Tuple[float, float]:
+        return self._min, self._max
+
+    def set_name(self, name: str):
+        self._name = name
+
+    def set_type(self, type: MXType):
+        self._type = type
+
+    def set_bound(self, bound: Tuple[float, float]):
+        self._min = bound[0]
+        self._max = bound[1]
```

## big_thing_py/core/function.py

```diff
@@ -1,125 +1,252 @@
 from big_thing_py.common import *
-from big_thing_py.common.request import *
-from big_thing_py.common.mqtt_message import *
+from big_thing_py.core.request import *
+from big_thing_py.core.mqtt_message import *
 from big_thing_py.core.argument import *
 from big_thing_py.core.service import *
 
-from func_timeout import func_timeout, FunctionTimedOut
+from func_timeout import StoppableThread, FunctionTimedOut
+import threading
 
 
-class SoPFunction(SoPService):
-    def __init__(self, name: str = None, thing_name: str = None, middleware_name: str = None, tag_list: List[SoPTag] = [], desc: str = None, func: Callable = None, energy: float = None,
-                 arg_list: List[SoPArgument] = [], return_type: SoPType = SoPType.UNDEFINED, exec_time: float = 10,
-                 timeout: float = 10, policy: SoPPolicy = SoPPolicy.SINGLE) -> None:
-        super().__init__(name=name, thing_name=thing_name,  middleware_name=middleware_name,
-                         tag_list=tag_list, desc=desc, func=func, energy=energy)
+class MXFunction(MXService):
+
+    def __init__(self, func: Callable, tag_list: List[MXTag],
+                 return_type: MXType,
+                 name: str = '', energy: float = 0, desc: str = '', thing_name: str = '', middleware_name: str = '',
+                 arg_list: List[MXArgument] = [], exec_time: float = 0, timeout: float = 0, range_type: MXRangeType = MXRangeType.SINGLE) -> None:
+        super().__init__(func=func, tag_list=tag_list,
+                         name=name, energy=energy, desc=desc, thing_name=thing_name, middleware_name=middleware_name)
 
-        self._arg_list = arg_list
         self._return_type = return_type
-        self._return_value = None
+        self._arg_list = arg_list
         self._exec_time = exec_time
         self._timeout = timeout
+        # TODO: range_type will be removed from MXFunction
+        self._range_type = range_type
 
-        self._running: bool = False
-        self._policy = policy  # for super function feature
+        self._return_value = None
+        self._running = False
+        self._running_scenario_list: List[str] = []
 
         # Queue
+        self._publish_queue: Queue = None
+
+        if self._return_type in [MXType.UNDEFINED]:
+            raise MXValueError('return_type cannot be undefined')
+        if (not len(self._arg_list) == len(get_function_info(self._func)['args'])) if self._func else False:
+            raise MXValueError('Length of argument list must be same with callback function')
+
+        # TODO: return type detection feature
+        # if not self._return_type or self._return_type in [MXType.UNDEFINED]:
+        #     func_info = get_function_info(self._func)
+        #     self._return_type = MXType().get(func_info[2])
+        #     raise MXValueError('type must be specified')
+        # elif self._return_type in [MXType.UNDEFINED]:
+        #     raise MXValueError('type cannot be undefined or void')
+
+    def __eq__(self, o: 'MXFunction') -> bool:
+        instance_check = isinstance(o, MXFunction)
+        arg_list_check = (o._arg_list == self._arg_list)
+        return_type_check = (o._return_type == self._return_type)
+        exec_time_check = (o._exec_time == self._exec_time)
+        timeout_check = (o._timeout == self._timeout)
+        range_type_check = (o._range_type == self._range_type)
+
+        return super().__eq__(o) and instance_check and arg_list_check and return_type_check and exec_time_check and timeout_check and range_type_check
+
+    def __getstate__(self):
+        state = super().__getstate__()
+
+        state['_return_type'] = self._return_type
+        state['_arg_list'] = self._arg_list
+        state['_exec_time'] = self._exec_time
+        state['_timeout'] = self._timeout
+        state['_range_type'] = self._range_type
+
+        del state['_return_value']
+        del state['_running']
+        del state['_publish_queue']
+        del state['_running_scenario_list']
+
+        return state
+
+    def __setstate__(self, state):
+        super().__setstate__(state)
+
+        self._type = state['_type']
+        self._min = state['_min']
+        self._max = state['_max']
+        self._cycle = state['_cycle']
+        self._format = state['_format']
+
+        self._return_value = None
+        self._running = False
         self._publish_queue = None
+        self._running_scenario_list = []
 
-    def __eq__(self, o: object) -> bool:
-        arg_list_check = o._arg_list == self._arg_list
-        return_type_check = o._return_type == self._return_type
-        exec_time_check = o._exec_time == self._exec_time
-        timeout_check = o._timeout == self._timeout
-
-        return super().__eq__(o) and arg_list_check and return_type_check and exec_time_check and timeout_check
-
-    # is_parallel은 현재 사용하지 않음 -> 추후에 사용할 수도 있음..
-    def _wrapper(self, execute_request: SoPExecuteRequest) -> bool:
-        execute_msg = execute_request._trigger_msg
-        SOPLOG_DEBUG(
-            f'[FUNC RUN] run {self._name} function by {execute_msg._scenario}', 'green')
+    def _wrapper(self, execute_request: MXExecuteRequest) -> bool:
+        execute_msg = execute_request.trigger_msg
+        MXLOG_DEBUG(
+            f'[FUNC RUN] run {self._name} function by {execute_msg.scenario}', 'green')
 
         try:
-            if not isinstance(execute_msg, SoPExecuteMessage):
-                SOPLOG_DEBUG(
-                    f'[FUNC ERROR] Wrong ExeucuteMessage type: {type(execute_msg)}', 'red')
-                raise
+            if not isinstance(execute_msg, MXExecuteMessage):
+                raise Exception(f'[{get_current_function_name()}] Wrong ExecuteMessage type - execute_msg: {type(execute_msg)}')
 
             self._running = True
-            error = None
-            self._return_value = func_timeout(
-                self._timeout, self._func, args=(*execute_msg.tuple_arguments(), ))
-            execute_duration = execute_request.timer_end()
-            result_msg = SoPExecuteResultMessage(execute_msg._function_name,
-                                                 execute_msg._thing_name,
-                                                 execute_msg._scenario,
-                                                 self._return_type,
-                                                 self._return_value,
-                                                 error,
-                                                 middleware_name=execute_request._trigger_msg._middleware_name,
-                                                 request_ID=execute_request._trigger_msg._request_ID)
-            execute_request.set_return_msg(result_msg)
+            error = MXErrorCode.NO_ERROR
+
+            if self._timeout:
+                # self._return_value = func_timeout(self._timeout, self._func, args=(*execute_msg.tuple_arguments(), ))
+                current_thread = threading.current_thread()
+                self._return_value = self._run_with_timeout(timeout=self._timeout, func=self._func, name=current_thread.name, 
+                                                            user_data=dict(scenario=execute_msg.scenario), args=(*execute_msg.tuple_arguments(), ))
+            else:
+                self._return_value = self._func(*execute_msg.tuple_arguments())
         except KeyboardInterrupt as e:
-            # TODO: for warpup main thread, but not test it yet
+            # TODO: for wrapup main thread, but not test it yet
             print_error(e)
-            SOPLOG_DEBUG('Function execution exit by user', 'red')
+            MXLOG_DEBUG('Function execution exit by user', 'red')
             raise e
         except FunctionTimedOut as e:
-            # print_error(e)
-            SOPLOG_DEBUG(
-                f'[FUNC TIMEOUT] function {self._name} by scenario {execute_msg._scenario} was timeout!!!', 'yellow')
-            error = SoPErrorType.TIMEOUT
+            MXLOG_DEBUG(
+                f'[FUNC TIMEOUT] function {self._name} by scenario {execute_msg.scenario} was timeout!!!', 'yellow')
+            error = MXErrorCode.TIMEOUT
         except Exception as e:
             print_error(e)
-            SOPLOG_DEBUG(
-                f'[FUNC ERROR] function {self._name} by scenario {execute_msg._scenario} is failed while executing!!!', 'red')
-            error = SoPErrorType.FAIL
+            MXLOG_DEBUG(
+                f'[FUNC FAIL] function {self._name} by scenario {execute_msg.scenario} is failed while executing!!!', 'red')
+            error = MXErrorCode.FAIL
         else:
-            SOPLOG_DEBUG(
-                f'[FUNC FINISH] function {self._name} finish. -> return value : {self._return_value}, duration: {execute_duration:.4f} Sec', 'green')
-            error = SoPErrorType.NO_ERROR
+            error = MXErrorCode.NO_ERROR
         finally:
+            # result_msg = MXExecuteResultMessage(function=self,
+            #                                      scenario=execute_msg.scenario,
+            #                                      request_ID=execute_request.trigger_msg.request_ID,
+            #                                      error=error)
+            # execute_request.set_return_msg(result_msg)
+            self._send_TM_RESULT_EXECUTE(scenario=execute_msg.scenario,
+                                         error=error,
+                                         request_ID=execute_msg.request_ID)
+
+            execute_request.timer_end()
             self._running = False
-            self._send_TM_RESULT_EXECUTE(execute_msg._function_name,
-                                         execute_msg._thing_name,
-                                         self._return_type,
-                                         self._return_value,
-                                         execute_msg._scenario,
-                                         error,
-                                         middleware_name=execute_request._trigger_msg._middleware_name,
-                                         request_ID=execute_request._trigger_msg._request_ID)
-
-    def execute(self, execute_msg: SoPExecuteRequest) -> None:
-        execute_thread = SoPThread(
-            func=self._wrapper,
-            name=f'{self._func.__name__}_thread',
+            self._running_scenario_list.remove(execute_msg.scenario)
+            MXLOG_DEBUG(f'[FUNC END] function {self._name} end. -> return value : {self._return_value}, duration: {execute_request.duration():.4f} Sec', 'green')
+
+    def start_execute_thread(self, execute_msg: MXExecuteMessage) -> MXThread:
+        execute_result_msg = MXExecuteResultMessage(function=self, scenario=execute_msg.scenario)
+        execute_request = MXExecuteRequest(trigger_msg=execute_msg, result_msg=execute_result_msg)
+        self._running_scenario_list.append(execute_msg.scenario)
+        execute_request.timer_start()
+
+        execute_thread = MXThread(
+            target=self._wrapper,
+            name=f'{self._func.__name__}_{execute_msg.scenario}_thread',
             daemon=True,
-            arg_list=(execute_msg, ))
+            args=(execute_request, ))
         execute_thread.start()
 
-    def _send_TM_RESULT_EXECUTE(self, function_name: str, thing_name: str,
-                                return_type: SoPType, return_value: Union[str, float, bool], scenario: str, error: SoPErrorType,
-                                middleware_name: str = '', request_ID: str = '') -> None:
-        self._publish_queue.put(SoPExecuteResultMessage(
-            function_name, thing_name, scenario, return_type, return_value, error, middleware_name=middleware_name, request_ID=request_ID).mqtt_message())
+        return execute_thread
+
+    def _run_with_timeout(self, timeout: float, func: Callable, name: str = '', user_data: dict = None, args: tuple = (), kwargs: dict = None):
+        if not kwargs:
+            kwargs = {}
+        if not args:
+            args = ()
+
+        ret = []
+        exception = []
+        isStopped = False
+
+        def funcwrap(args2, kwargs2):
+            try:
+                ret.append(func(*args2, **kwargs2))
+            except FunctionTimedOut:
+                # Don't print traceback to stderr if we time out
+                pass
+            except Exception as e:
+                exc_info = sys.exc_info()
+                if isStopped is False:
+                    # Assemble the alternate traceback, excluding this function
+                    #  from the trace (by going to next frame)
+                    # Pytohn3 reads native from __traceback__,
+                    # python2 has a different form for "raise"
+                    e.__traceback__ = exc_info[2].tb_next
+                    exception.append(e)
+
+        thread = StoppableThread(target=funcwrap, name=name, args=(args, kwargs))
+        thread.daemon = True
+        thread.user_data = user_data
+
+        thread.start()
+        thread.join(timeout)
+
+        stopException = None
+        if thread.is_alive():
+            isStopped = True
+
+            class FunctionTimedOutTempType(FunctionTimedOut):
+                def __init__(self):
+                    return FunctionTimedOut.__init__(self, '', timeout, func, args, kwargs)
+
+            FunctionTimedOutTemp = type('FunctionTimedOut' + str(hash("%d_%d_%d_%d" % (id(timeout), id(func), id(args), id(kwargs)))),
+                                        FunctionTimedOutTempType.__bases__, dict(FunctionTimedOutTempType.__dict__))
+
+            stopException = FunctionTimedOutTemp
+            thread._stopThread(stopException)
+            thread.join(min(.1, timeout / 50.0))
+            raise FunctionTimedOut('', timeout, func, args, kwargs)
+        else:
+            # We can still cleanup the thread here..
+            # Still give a timeout... just... cuz..
+            thread.join(.5)
+
+        if exception:
+            raise exception[0] from None
+
+        if ret:
+            return ret[0]
+
+    def _send_TM_RESULT_EXECUTE(self, scenario: str, error: MXErrorCode, request_ID: str = None) -> None:
+        execute_result_msg = self._generate_execute_result_message(scenario=scenario,
+                                                                   error=error,
+                                                                   request_ID=request_ID)
+        execute_result_mqtt_msg = execute_result_msg.mqtt_message()
+        self._publish_queue.put(execute_result_mqtt_msg)
 
-    def dump(self) -> Dict:
+    def dict(self) -> dict:
         return {
             "name": self._name,
             "description": self._desc,
             "exec_time": self._exec_time * 1000 if self._exec_time is not None else 0,
             "return_type": self._return_type.value,
             "energy": self._energy,
-            "tags": [tag.dump() for tag in self._tag_list],
+            "tags": [tag.dict() for tag in self._tag_list],
             "use_arg": 1 if self._arg_list else 0,
-            "arguments": [argument.dump() for argument in self._arg_list] if self._arg_list else []
+            "arguments": [argument.dict() for argument in self._arg_list] if self._arg_list else []
         }
 
+    # ========================
+    #         _    _  _
+    #        | |  (_)| |
+    #  _   _ | |_  _ | | ___
+    # | | | || __|| || |/ __|
+    # | |_| || |_ | || |\__ \
+    #  \__,_| \__||_||_||___/
+    # ========================
+
+    def _generate_execute_result_message(self, scenario: str, error: MXErrorCode, request_ID: str) -> MXExecuteResultMessage:
+        execute_result_msg = MXExecuteResultMessage(function=self,
+                                                    scenario=scenario,
+                                                    request_ID=request_ID,
+                                                    error=error)
+        return execute_result_msg
+
     # ====================================
     #               _    _
     #              | |  | |
     #   __ _   ___ | |_ | |_   ___  _ __
     #  / _` | / _ \| __|| __| / _ \| '__|
     # | (_| ||  __/| |_ | |_ |  __/| |
     #  \__, | \___| \__| \__| \___||_|
@@ -129,25 +256,31 @@
 
     def get_exec_time(self) -> float:
         return self._exec_time
 
     def get_timeout(self) -> float:
         return self._timeout
 
-    def get_arg_list(self) -> List[SoPArgument]:
+    def get_arg_list(self) -> List[MXArgument]:
         return self._arg_list
 
-    def get_return_type(self) -> SoPType:
+    def get_return_type(self) -> MXType:
         return self._return_type
 
+    def get_return_value(self) -> Union[int, float, str, bool]:
+        return self._return_value
+
     def get_running(self) -> bool:
         return self._running
 
-    def get_policy(self) -> SoPPolicy:
-        return self._policy
+    def get_range_type(self) -> MXRangeType:
+        return self._range_type
+
+    def get_running_scenario_list(self) -> List[str]:
+        return self._running_scenario_list
 
     # ==================================
     #             _    _
     #            | |  | |
     #  ___   ___ | |_ | |_   ___  _ __
     # / __| / _ \| __|| __| / _ \| '__|
     # \__ \|  __/| |_ | |_ |  __/| |
@@ -156,22 +289,25 @@
 
     def set_exec_time(self, exec_time: float) -> None:
         self._exec_time = exec_time
 
     def set_timeout(self, timeout: float) -> None:
         self._timeout = timeout
 
-    def set_arg_list(self, arg_list: List[SoPArgument]) -> None:
+    def set_arg_list(self, arg_list: List[MXArgument]) -> None:
         self._arg_list = arg_list
 
-    def set_return_type(self, return_type: SoPType) -> None:
+    def set_return_type(self, return_type: MXType) -> None:
         self._return_type = return_type
 
+    def set_return_value(self, return_value: Union[int, float, str, bool]) -> None:
+        self._return_value = return_value
+
     def set_running(self, running: bool) -> None:
         self._running = running
 
-    def set_policy(self, policy: SoPPolicy) -> None:
-        self._policy = policy
+    def set_range_type(self, range_type: MXRangeType) -> None:
+        self._range_type = range_type
 
     # for link to big_thing's publish_queue
     def set_publish_queue(self, queue: Queue):
         self._publish_queue = queue
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## big_thing_py/core/service.py

```diff
@@ -1,46 +1,80 @@
 from big_thing_py.core.tag import *
 from abc import *
 
-import copy
 
-
-class SoPService(metaclass=ABCMeta):
-    def __init__(self, name: str, thing_name: str, middleware_name: str, tag_list: List[SoPTag], desc: str, func: Callable, energy: float) -> None:
-        if name:
-            self._name: str = name
-        else:
-            self._name = func.__name__
-
-        # TODO: why only deepcopy make it works?
-        self._thing_name = thing_name
-        self._middleware_name = middleware_name
-        self._tag_list: List[SoPTag] = copy.deepcopy(tag_list)
-        # self._tag_list: List[SoPTag] = tag_list
-        self._desc = desc
+class MXService(metaclass=ABCMeta):
+    def __init__(self, name: str, func: Callable, tag_list: List[MXTag], energy: float, desc: str, thing_name: str, middleware_name: str) -> None:
+        self._name = name
         self._func = func
+        self._tag_list = tag_list
         self._energy = energy
+        self._desc = desc
+        self._thing_name = thing_name
+        self._middleware_name = middleware_name
 
-    def __str__(self) -> str:
-        return self._name
+        if not callable(self._func):
+            raise MXValueError(f'func must be callable')
+        if not self._name:
+            self._name = func.__name__
+        if not check_valid_identifier(self._name):
+            raise MXValueError(f'name cannot be empty & can only contain alphanumeric characters and underscores')
+        if any([not isinstance(tag, MXTag) for tag in self._tag_list]) or len(self._tag_list) == 0:
+            raise MXValueError('tag_list must contain MXTag object')
+        else:
+            self._tag_list = [MXTag(name=tag) for tag in sorted(list(set(self.get_tag_list(string_mode=True))))]
+        if not isinstance(self._energy, (int, float)):
+            raise MXValueError(f'energy must be int or float')
+        if not isinstance(self._desc, str):
+            raise MXValueError(f'desc must be str')
+        if not isinstance(self._thing_name, str):
+            raise MXValueError(f'thing_name must be str')
+        if not isinstance(self._middleware_name, str):
+            raise MXValueError(f'middleware_name must be str')
 
-    def __eq__(self, o: object) -> bool:
-        instance_check = isinstance(o, SoPService)
+    def __eq__(self, o: 'MXService') -> bool:
+        instance_check = isinstance(o, MXService)
+        name_check = (o._name == self._name)
         thing_name_check = (o._thing_name == self._thing_name)
         middleware_name_check = (o._middleware_name == self._middleware_name)
-        name_check = (o._name == self._name)
         tag_list_check = (o._tag_list == self._tag_list)
+        func_check = (o._func == self._func)
+        energy_check = (o._energy == self._energy)
 
-        return instance_check and name_check and thing_name_check and middleware_name_check and tag_list_check
+        return instance_check and name_check and thing_name_check and middleware_name_check and tag_list_check and func_check and energy_check
+    
+    def __getstate__(self):
+        state = self.__dict__.copy()
+        
+        del state['_func']
+        
+        return state
+
+    def __setstate__(self, state):
+        self.__dict__.update(state)
+        
+        self._func = None
+
+    def add_tag(self, tag: Union[MXTag, List[MXTag]]) -> 'MXService':
+        if not isinstance(tag, (MXTag, list)):
+            raise Exception('tag must be MXTag object')
+
+        if isinstance(tag, MXTag):
+            if not tag in self._tag_list:
+                self._tag_list.append(tag)
+        elif all(isinstance(t, MXTag) for t in tag):
+            for t in tag:
+                if not t in self._tag_list:
+                    self._tag_list.append(t)
+        self._tag_list = sorted(self._tag_list, key=lambda x: x.get_name())
 
-    def add_tag(self, tag: SoPTag) -> None:
-        self._tag_list.append(tag)
+        return self
 
     @abstractmethod
-    def dump(self) -> Dict:
+    def dict(self) -> dict:
         pass
 
     # ====================================
     #               _    _
     #              | |  | |
     #   __ _   ___ | |_ | |_   ___  _ __
     #  / _` | / _ \| __|| __| / _ \| '__|
@@ -55,15 +89,15 @@
 
     def get_thing_name(self) -> str:
         return self._thing_name
 
     def get_middleware_name(self) -> str:
         return self._middleware_name
 
-    def get_tag_list(self, string_mode: bool = False) -> List[SoPTag]:
+    def get_tag_list(self, string_mode: bool = False) -> List[MXTag]:
         if string_mode:
             return [str(tag) for tag in self._tag_list]
         else:
             return self._tag_list
 
     def get_desc(self) -> str:
         return self._desc
@@ -88,18 +122,18 @@
 
     def set_thing_name(self, thing_name: str) -> None:
         self._thing_name = thing_name
 
     def set_middleware_name(self, middleware_name: str) -> None:
         self._middleware_name = middleware_name
 
-    def set_tag_list(self, tag_list: List[SoPTag]) -> None:
+    def set_tag_list(self, tag_list: List[MXTag]) -> None:
         self._tag_list = tag_list
 
     def set_desc(self, desc: str) -> None:
         self._desc = desc
 
     def set_func(self, func: Callable) -> None:
         self._func = func
 
-    def set_func(self, energy: float) -> None:
+    def set_energy(self, energy: float) -> None:
         self._energy = energy
```

## big_thing_py/core/tag.py

```diff
@@ -1,24 +1,29 @@
 from big_thing_py.utils import *
 
 
-class SoPTag:
+class MXTag:
 
-    def __init__(self, name=''):
+    def __init__(self, name: str):
         self._name: str = name
 
+        if not check_valid_identifier(self._name):
+            raise MXValueError(f'name cannot be empty & can only contain alphanumeric characters and underscores')
+
+    def __eq__(self, o: 'MXTag') -> bool:
+        name_check = (o._name == self._name)
+
+        return isinstance(o, MXTag) and name_check
+
     def __str__(self) -> str:
         return self._name
 
-    def __eq__(self, o: object) -> bool:
-        return isinstance(o, SoPTag) and o._name == self._name
-
-    def dump(self):
+    def dict(self):
         return {
-            "name": self._name
+            'name': self._name
         }
 
     # ====================================
     #               _    _
     #              | |  | |
     #   __ _   ___ | |_ | |_   ___  _ __
     #  / _` | / _ \| __|| __| / _ \| '__|
```

## big_thing_py/core/thing.py

```diff
@@ -1,86 +1,131 @@
 from big_thing_py.core.function import *
 from big_thing_py.core.value import *
 
 
-class SoPThing:
+class MXThing:
 
-    def __init__(self, name: str, service_list: List[SoPService], alive_cycle: float, is_super: bool = False, is_parallel: bool = True):
+    DEFAULT_NAME = 'default_big_thing'
+
+    def __init__(self, name: str, service_list: List[MXService], alive_cycle: float, is_super: bool, is_parallel: bool,
+                 middleware_name: str = None):
         # base info
         self._name = name
-        self._middleware_name = None
+        self._service_list = service_list
         self._alive_cycle = alive_cycle
+        self._is_super = is_super
+        self._is_parallel = is_parallel
+        self._middleware_name = middleware_name
+
         self._last_alive_time = 0
-        self._registered = False
+        self._is_connected = False
+        self._is_registered = False
         self._subscribed_topic_set: Set[str] = set()
-        self._function_list: List[SoPFunction] = []
-        self._value_list: List[SoPValue] = []
+        self._function_list: List[MXFunction] = []
+        self._value_list: List[MXValue] = []
 
-        self._is_parallel = is_parallel
-        self._is_super = is_super
+        # Queue
+        self._receive_queue: Queue = Queue()
+        self._publish_queue: Queue = Queue()
+
+        if not self._name:
+            self._name = MXThing.DEFAULT_NAME
+        elif not check_valid_identifier(self._name):
+            raise MXValueError(f'name cannot be empty & can only contain alphanumeric characters and underscores')
+
+        if self._alive_cycle <= 0:
+            raise MXValueError(f'alive cycle must be greater than 0')
+
+        for service in self._service_list:
+            if isinstance(service, (MXFunction, MXValue)):
+                self.add_service(service)
+            else:
+                raise MXTypeError(f'service_list must contain MXFunction or MXValue object')
 
-        if service_list == None:
-            service_list = []
+    def __eq__(self, o: 'MXThing') -> bool:
+        instance_check = isinstance(o, MXThing)
+        name_check = (o._name == self._name)
+        service_list_check = (o._function_list == self._function_list) and (
+            o._value_list == self._value_list)
+        alive_cycle_check = (o._alive_cycle == self._alive_cycle)
+        is_super_check = (o._is_super == self._is_super)
+        is_parallel_check = (o._is_parallel == self._is_parallel)
+
+        return instance_check and name_check and service_list_check and alive_cycle_check and is_super_check and is_parallel_check
+
+    def __getstate__(self):
+        state = self.__dict__.copy()
+
+        del state['_last_alive_time']
+        del state['_is_connected']
+        del state['_is_registered']
+        del state['_subscribed_topic_set']
+        del state['_receive_queue']
+        del state['_publish_queue']
 
-        for service in service_list:
-            if isinstance(service, (SoPFunction, SoPValue)):
-                self._add_service(service)
-            else:
-                SOPLOG_DEBUG(
-                    f'[SoPThing] Service type error -> service type - {type(service)}')
+        return state
 
-    # for add overriding
-    def __eq__(self, o: object) -> bool:
-        check_instance = isinstance(o, SoPThing)
-        check_name = (o._name == self._name)
-        check_middleware_name = (o._middleware_name == self._middleware_name)
+    def __setstate__(self, state):
+        self.__dict__.update(state)
 
-        return check_instance and check_name and check_middleware_name
+        self._last_alive_time = 0
+        self._is_connected = False
+        self._is_registered = False
+        self._subscribed_topic_set = set()
+        self._receive_queue = Queue()
+        self._publish_queue = Queue()
 
     # ========================
     #         _    _  _
     #        | |  (_)| |
     #  _   _ | |_  _ | | ___
     # | | | || __|| || |/ __|
     # | |_| || |_ | || |\__ \
     #  \__,_| \__||_||_||___/
     # ========================
 
-    def _add_service(self, service: SoPService) -> None:
-        if isinstance(service, SoPFunction):
-            service: SoPFunction = service
-            service.set_thing_name(self.get_name())
-            self._function_list.append(service)
-            return True
-        elif isinstance(service, SoPValue):
-            service: SoPValue = service
-            self.get_value_list().append(service)
-            value_getter_function = SoPFunction(name=f'__{service.get_name()}',
-                                                thing_name=self.get_name(),
-                                                tag_list=service.get_tag_list(),
-                                                desc=service.get_desc(),
-                                                func=service.get_func(),
-                                                arg_list=[],
-                                                return_type=service.get_type())
-            self._function_list.append(value_getter_function)
-            return True
-
-    def _find_function(self, function_name: str) -> SoPFunction:
+    def _get_function(self, function_name: str) -> MXFunction:
         for function in self._function_list:
             if function.get_name() == function_name:
                 return function
 
-    def dump(self) -> Dict:
+    def add_service(self, service: MXService) -> 'MXThing':
+        # service_copy = copy.deepcopy(service)
+        # service_copy = copy.copy(service)
+        service.add_tag(MXTag(name=self._name))
+        service.set_thing_name(self._name)
+
+        if isinstance(service, MXFunction):
+            service.set_publish_queue(self._publish_queue)
+            self._function_list.append(service)
+        elif isinstance(service, MXValue):
+            self._value_list.append(service)
+            value_getter_function = MXFunction(func=service.get_func(),
+                                               return_type=service.get_type(),
+                                               name=f'__{service.get_name()}',
+                                               tag_list=service.get_tag_list(),
+                                               energy=service.get_energy(),
+                                               desc=service.get_desc(),
+                                               thing_name=service.get_thing_name(),
+                                               middleware_name=service.get_middleware_name(),
+                                               arg_list=[])
+            self._function_list.append(value_getter_function)
+        self._value_list = sorted(self._value_list, key=lambda x: x.get_name())
+        self._function_list = sorted(self._function_list, key=lambda x: x.get_name())
+
+        return self
+
+    def dict(self) -> dict:
         return {
             "name": self._name,
             "alive_cycle": self._alive_cycle,
             "is_super": self._is_super,
             "is_parallel": self._is_parallel,
-            "values": [value.dump() for value in self._value_list],
-            "functions": [function.dump() for function in self._function_list]
+            "values": [value.dict() for value in self._value_list],
+            "functions": [function.dict() for function in self._function_list]
         }
 
     # ====================================
     #               _    _
     #              | |  | |
     #   __ _   ___ | |_ | |_   ___  _ __
     #  / _` | / _ \| __|| __| / _ \| '__|
@@ -104,20 +149,26 @@
 
     def get_subscribed_topic_set(self) -> Set[str]:
         return self._subscribed_topic_set
 
     def get_registered(self) -> bool:
         return self._registered
 
-    def get_function_list(self) -> List[SoPFunction]:
+    def get_function_list(self) -> List[MXFunction]:
         return self._function_list
 
-    def get_value_list(self) -> List[SoPValue]:
+    def get_value_list(self) -> List[MXValue]:
         return self._value_list
 
+    def get_is_super(self) -> bool:
+        return self._is_super
+
+    def get_is_parallel(self) -> bool:
+        return self._is_parallel
+
     # ==================================
     #             _    _
     #            | |  | |
     #  ___   ___ | |_ | |_   ___  _ __
     # / __| / _ \| __|| __| / _ \| '__|
     # \__ \|  __/| |_ | |_ |  __/| |
     # |___/ \___| \__| \__| \___||_|
@@ -136,7 +187,19 @@
         self._alive_cycle = alive_cycle
 
     def set_subscribe_topic_set(self, subscribe_topic_set: Set[str]) -> None:
         self._subscribed_topic_set = subscribe_topic_set
 
     def set_registered(self, registered: bool) -> None:
         self._registered = registered
+
+    def set_function_list(self, function_list: List[MXFunction]) -> None:
+        self._function_list = function_list
+
+    def set_value_list(self, value_list: List[MXValue]) -> None:
+        self._value_list = value_list
+
+    def set_is_super(self, is_super: bool) -> bool:
+        self._is_super = is_super
+
+    def set_is_parallel(self, is_parallel: bool) -> bool:
+        self._is_parallel = is_parallel
```

## big_thing_py/core/value.py

```diff
@@ -1,67 +1,104 @@
 from big_thing_py.core.service import *
-import sys
 
 
-class SoPValue(SoPService):
+class MXValue(MXService):
 
-    def __init__(self, name: str = None, thing_name: str = None, middleware_name: str = None, tag_list: List[SoPTag] = [], desc: str = '', func: Callable = None, energy: float = None,
-                 type: SoPType = SoPType.UNDEFINED, bound: Tuple[float, float] = (sys.float_info.min, sys.float_info.max), format: str = '', cycle: float = 10) -> None:
-        super().__init__(name=name, thing_name=thing_name, middleware_name=middleware_name,
-                         tag_list=tag_list, desc=desc, func=func, energy=energy)
+    def __init__(self, func: Callable, tag_list: List[MXTag],
+                 type: MXType, bound: Tuple[float, float], cycle: float,
+                 name: str = '',  energy: float = 0, desc: str = '', thing_name: str = '', middleware_name: str = '',
+                 format: str = '') -> None:
+        super().__init__(func=func, tag_list=tag_list,
+                         name=name, energy=energy, desc=desc, thing_name=thing_name, middleware_name=middleware_name,)
 
-        self._type: SoPType = type
-        self._min: float = bound[0]
-        self._max: float = bound[1]
-        self._cycle: float = cycle
-
-        # TODO: Add Enum class for format type in common.py
-        self._format: str = format
+        self._type = type
+        self._min, self._max = bound
+        self._cycle = cycle
+        self._format = format
 
         self._last_value: Union[float, str, bool] = None
         self._last_update_time: float = 0
+        self._binary_sending: bool = False
 
-        self._arg_list = []
+        if (len(get_function_info(self._func)['args']) > 0 or get_function_info(self._func)['return_type'] == None):
+            raise MXValueError('callback function must not have any argument and must return value')
+        if self._min >= self._max:
+            raise MXValueError('bound must be min < max')
+        if self._type in [MXType.UNDEFINED, MXType.VOID]:
+            raise MXValueError('type cannot be undefined or void')
+        if (self._cycle <= 0) if self._cycle != None else False:
+            raise MXValueError('cycle must be > 0')
+        if not isinstance(self._format, str):
+            raise MXValueError('format must be str')
 
-    def __eq__(self, o: object) -> bool:
+    def __eq__(self, o: 'MXValue') -> bool:
+        instance_check = isinstance(o, MXValue)
         type_check = (o._type == self._type)
         bound_check = (o._max == self._max and o._min == self._min)
-        cycle_check = (o._cycle == self._cycle)
         format_check = (o._format == self._format)
+        cycle_check = (o._cycle == self._cycle)
+
+        return super().__eq__(o) and instance_check and type_check and bound_check and format_check and cycle_check
+
+    def __getstate__(self):
+        state = super().__getstate__()
+
+        state['_type'] = self._type
+        state['_min'] = self._min
+        state['_max'] = self._max
+        state['_cycle'] = self._cycle
+        state['_format'] = self._format
+
+        del state['_last_value']
+        del state['_last_update_time']
+        del state['_binary_sending']
+
+        return state
+
+    def __setstate__(self, state):
+        super().__setstate__(state)
+
+        self._type = state['_type']
+        self._min = state['_min']
+        self._max = state['_max']
+        self._cycle = state['_cycle']
+        self._format = state['_format']
 
-        return super().__eq__(o) and type_check and bound_check and cycle_check and format_check
+        self._last_value = None
+        self._last_update_time = 0
+        self._binary_sending = False
 
-    def update(self, *arg_list, **kwargs) -> Union[float, bool]:
+    def update(self, *arg_list, **kwargs) -> Union[int, float, str, bool]:
         try:
             new_value = self._func(*arg_list, **kwargs)
             self._last_update_time = get_current_time()
 
             if not self._last_value == new_value:
                 self._last_value = new_value
                 return new_value
             else:
                 return None
         except Exception as e:
             print_error(e)
             return None
 
-    def dump(self) -> Dict:
+    def dict(self) -> dict:
         return {
             "name": self._name,
             "description": self._desc,
-            "tags": [tag.dump() for tag in self._tag_list],
+            "tags": [tag.dict() for tag in self._tag_list],
             "type": self._type.value,
             "bound": {
                 "min_value": self._min,
                 "max_value": self._max
             },
             "format": self._format
         }
 
-    def dump_pub(self) -> Dict:
+    def publish_dict(self) -> dict:
         return {
             "type": self._type.value,
             "value": self._last_value
         }
 
     # ====================================
     #               _    _
@@ -70,15 +107,15 @@
     #  / _` | / _ \| __|| __| / _ \| '__|
     # | (_| ||  __/| |_ | |_ |  __/| |
     #  \__, | \___| \__| \__| \___||_|
     #   __/ |
     #  |___/
     # ====================================
 
-    def get_type(self) -> SoPType:
+    def get_type(self) -> MXType:
         return self._type
 
     def get_bound(self) -> Tuple[float, float]:
         return (self._min, self._max)
 
     def get_max(self) -> float:
         return self._max
@@ -97,27 +134,27 @@
 
     def get_last_update_time(self) -> float:
         return self._last_update_time
 
     def get_func(self) -> Callable:
         return self._func
 
-    def get_arg_list(self) -> List:
-        return self._arg_list
+    def get_binary_sending(self) -> bool:
+        return self._binary_sending
 
 # ==================================
 #             _    _
 #            | |  | |
 #  ___   ___ | |_ | |_   ___  _ __
 # / __| / _ \| __|| __| / _ \| '__|
 # \__ \|  __/| |_ | |_ |  __/| |
 # |___/ \___| \__| \__| \___||_|
 # ==================================
 
-    def set_type(self, type: SoPType) -> None:
+    def set_type(self, type: MXType) -> None:
         self._type = type
 
     def set_bound(self, bound: Tuple[float, float]) -> None:
         self._min = bound[0]
         self._max = bound[1]
 
     def set_max(self, max: float) -> None:
@@ -134,12 +171,12 @@
 
     def set_last_value(self, last_value: Union[float, str, bool]) -> None:
         self._last_value = last_value
 
     def set_last_update_time(self, last_update_time: float) -> None:
         self._last_update_time = last_update_time
 
-    def set_func(self, func) -> None:
+    def set_func(self, func: Callable) -> None:
         self._func = func
 
-    def set_arg_list(self, arg_list: List) -> None:
-        self._arg_list = arg_list
+    def set_binary_sending(self, binary_send: bool) -> bool:
+        self._binary_sending = binary_send
```

## big_thing_py/manager/manager_common.py

```diff
@@ -1,32 +1,32 @@
 from big_thing_py.utils import *
-from enum import Enum
+from enum import Enum, auto
 
 
-class SoPManagerMode(Enum):
+class MXManagerMode(Enum):
     UNDEFINED = 'UNDEFINED'
     JOIN = 'JOIN'
     SPLIT = 'SPLIT'
 
     @classmethod
-    def get(cls, name: str):
+    def get(cls, name: str) -> 'MXManagerMode':
         try:
             return cls[name.upper()]
         except Exception:
             return cls.UNDEFINED
 
 
-class SoPStaffThingInfo:
+class MXStaffThingInfo:
     def __init__(self, device_id: str) -> None:
         self.device_id = device_id
 
 
 class StaffRegisterResult:
     def __init__(self, staff_thing_name: str, device_id: str, assigned_device_id: str) -> None:
         self.staff_thing_name = staff_thing_name
         self.device_id = device_id
         self.assigned_device_id = assigned_device_id
 
 
-class SoPNewStaffThingLevel(Enum):
+class MXNewStaffThingLevel(Enum):
     NEW = 0
     DUPLICATE = 1
```

## big_thing_py/manager/manager_utils.py

```diff
@@ -1,83 +1,83 @@
 from big_thing_py.manager.manager_common import *
 from big_thing_py.staff_thing import *
 
 
 class ManagerModeHandler:
-    def __init__(self, mode: SoPManagerMode) -> None:
+    def __init__(self, mode: MXManagerMode) -> None:
         self._mode = mode
 
-    def dump_register_packet(self, staff_thing: SoPStaffThing) -> mqtt.MQTTMessage:
-        if self._mode == SoPManagerMode.JOIN:
+    def dump_register_packet(self, staff_thing: MXStaffThing) -> mqtt.MQTTMessage:
+        if self._mode == MXManagerMode.JOIN:
             # in join mode, manager thing don't need to send each staff thing's register packet
             # it's only need to send manager thing's register packet to middleware
             pass
-        elif self._mode == SoPManagerMode.SPLIT:
+        elif self._mode == MXManagerMode.SPLIT:
             if staff_thing.get_registered():
-                SOPLOG_DEBUG(
+                MXLOG_DEBUG(
                     '[dump_register_packet] staff thing already registered')
                 return False
 
-            topic = SoPProtocolType.Base.TM_REGISTER.value % (
+            topic = MXProtocolType.Base.TM_REGISTER.value % (
                 staff_thing.get_name())
-            payload = staff_thing.dump()
+            payload = staff_thing.dict()
             msg = mqtt.MQTTMessage(topic, payload)
             return staff_thing.get_name(), payload
         else:
-            raise ManagerModeError(
-                '[dump_register_packet] please set mode {SoPManagerMode.JOIN|SoPManagerMode.SPLIT}')
+            raise MXInvalidRequestError(
+                '[dump_register_packet] please set mode {MXManagerMode.JOIN|MXManagerMode.SPLIT}')
 
-    def dump_alive_packet(self, staff_thing_list: List[SoPStaffThing]) -> Union[mqtt.MQTTMessage, List[mqtt.MQTTMessage]]:
-        if self._mode == SoPManagerMode.JOIN:
+    def dump_alive_packet(self, staff_thing_list: List[MXStaffThing]) -> Union[mqtt.MQTTMessage, List[mqtt.MQTTMessage]]:
+        if self._mode == MXManagerMode.JOIN:
             # in join mode, manager thing don't need to send each staff thing's alive packet
             # it's only need to send manager thing's alive packet to middleware
             pass
-        elif self._mode == SoPManagerMode.SPLIT:
+        elif self._mode == MXManagerMode.SPLIT:
             packet_list = []
 
             for staff_thing in staff_thing_list:
                 if staff_thing.get_registered():
                     continue
-                topic = SoPProtocolType.Base.TM_ALIVE.value % (
+                topic = MXProtocolType.Base.TM_ALIVE.value % (
                     staff_thing.get_name())
-                payload = EMPTY_JSON
+                payload = str(EMPTY_JSON)
                 msg = mqtt.MQTTMessage(topic, payload)
                 packet_list.append(msg)
 
             return packet_list
         else:
-            raise ManagerModeError(
-                '[dump_alive_packet] please set mode {SoPManagerMode.JOIN|SoPManagerMode.SPLIT}')
+            raise MXInvalidRequestError(
+                '[dump_alive_packet] please set mode {MXManagerMode.JOIN|MXManagerMode.SPLIT}')
 
-    def dump_value_packet(self, staff_thing_list: List[SoPStaffThing]) -> Union[mqtt.MQTTMessage, List[mqtt.MQTTMessage]]:
-        if self._mode == SoPManagerMode.JOIN:
+    def dump_value_packet(self, staff_thing_list: List[MXStaffThing]) -> Union[mqtt.MQTTMessage, List[mqtt.MQTTMessage]]:
+        if self._mode == MXManagerMode.JOIN:
             # in join mode, manager thing don't need to send each staff thing's value packet
             # it's only need to send manager thing's value packet to middleware
             pass
-        elif self._mode == SoPManagerMode.SPLIT:
+        elif self._mode == MXManagerMode.SPLIT:
             packet_list = []
 
             for staff_thing in staff_thing_list:
                 if staff_thing.get_registered():
                     continue
                 for value in staff_thing.get_value_list():
-                    value_dump = value.dump()
+                    value_dump = value.dict()
 
-                    topic = SoPProtocolType.Base.TM_ALIVE.value % (
+                    topic = MXProtocolType.Base.TM_ALIVE.value % (
                         staff_thing.get_name())
-                    payload = EMPTY_JSON
+                    payload = str(EMPTY_JSON)
                     msg = mqtt.MQTTMessage(topic, payload)
                     packet_list.append(msg)
 
             return packet_list
         else:
-            raise ManagerModeError(
-                '[dump_value_packet] please set mode {SoPManagerMode.JOIN|SoPManagerMode.SPLIT}')
+            raise MXInvalidRequestError(
+                '[dump_value_packet] please set mode {MXManagerMode.JOIN|MXManagerMode.SPLIT}')
 
-    def dump_execute_result_packet(self, staff_thing_list: List[SoPStaffThing]) -> Union[mqtt.MQTTMessage, List[mqtt.MQTTMessage]]:
-        if self._mode == SoPManagerMode.JOIN:
+    def dump_execute_result_packet(self, staff_thing_list: List[MXStaffThing]) -> Union[mqtt.MQTTMessage, List[mqtt.MQTTMessage]]:
+        if self._mode == MXManagerMode.JOIN:
             pass
-        elif self._mode == SoPManagerMode.SPLIT:
+        elif self._mode == MXManagerMode.SPLIT:
             pass
         else:
-            raise ManagerModeError(
-                '[dump_execute_result_packet] please set mode {SoPManagerMode.JOIN|SoPManagerMode.SPLIT}')
+            raise MXInvalidRequestError(
+                '[dump_execute_result_packet] please set mode {MXManagerMode.JOIN|MXManagerMode.SPLIT}')
```

## big_thing_py/super/__init__.py

```diff
@@ -1,2 +1,3 @@
 from .super_function import *
-from .super_service_utils import *
+from .super_request import *
+from .super_mqtt_message import *
```

## big_thing_py/super/super_function.py

```diff
@@ -1,532 +1,572 @@
-from big_thing_py.super.super_service_utils import *
 from big_thing_py.super.super_request import *
-import random
-import threading
+from big_thing_py.super.super_mqtt_message import *
 
 
-class SoPSuperFunction(SoPFunction):
+class MXSuperFunction(MXFunction):
     '''
-        [Whole super function structure]
-        super_thing┬── super_function1┬── subfunction1┬────── target_thing1(at Middleware1)
-                   │                  │                ╲
-                   │                  │                 ╲──── target_thing2(at Middleware1)
-                   │                  │                  ╲
-                   │                  │                   ╲── target_thing3(at Middleware2)
-                   │                  │                    ╲
-                   │                  ├── subfunction2      ╲ ....
+        [Whole super service structure]
+        super_thing┬── super_service1┬── sub_service1┬────── target_thing1(at Middleware1)
+                   │                  │               ╲
+                   │                  │                ╲──── target_thing2(at Middleware1)
+                   │                  │                 ╲
+                   │                  │                  ╲── target_thing3(at Middleware2)
+                   │                  │                   ╲
+                   │                  ├── sub_service2      ╲ ....
                    │                  │
                    │                  ├── ...
                    │
                    │
-                   └── super_function2 ── subfunction1(target Thing1, target Middleware2)
+                   └── super_service2 ── sub_service1(target Thing1, target Middleware2)
     '''
 
-    def __init__(self, name: str = None, thing_name: str = None, middleware_name: str = None, tag_list: List[SoPTag] = ..., desc: str = None, func: Callable = None, energy: float = None,
-                 arg_list: List[SoPArgument] = ..., return_type: SoPType = ..., exec_time: float = 10, timeout: float = 10, policy: SoPPolicy = ...) -> None:
-        super().__init__(name, thing_name, middleware_name, tag_list, desc, func, energy,
-                         arg_list, return_type, exec_time, timeout, policy)
-
-        # 사용자가 super thing코드에 명세한 subfunction 조건에 맞는 subfunction 종류. 해당 조건에 맞는 subfunction들이 여러 디바이스에 여러 개 존재할 수 있다.
-        # super function에 명세된 req() 라인 수 만큼 존재한다.
-        self._subfunction_reqline_list: List[SoPSubFunctionReqline] = []
+    def __init__(self, func: Callable,
+                 return_type: MXType,
+                 name: str = '', tag_list: List[MXTag] = [], energy: float = 0, desc: str = '', thing_name: str = '', middleware_name: str = '',
+                 arg_list: List[MXArgument] = [], exec_time: float = 0, timeout: float = 0, range_type: MXRangeType = MXRangeType.SINGLE) -> None:
+        super().__init__(func=func,
+                         return_type=return_type,
+                         name=name, tag_list=tag_list, energy=energy, desc=desc, thing_name=thing_name, middleware_name=middleware_name,
+                         arg_list=arg_list, exec_time=exec_time, timeout=timeout, range_type=range_type)
+
+        # 사용자가 super thing코드에 명세한 sub_service 조건에 맞는 sub_service 종류. 해당 조건에 맞는 sub_service 여러 디바이스에 여러 개 존재할 수 있다.
+        # super service에 명세된 req() 라인 수 만큼 존재한다.
+        self._sub_service_request_list: List[MXSubServiceRequest] = []
 
-        # 처음 실행됬는지 여부를 나타낸다. 이는 super function을 처음 실행할 때, req()을 인식하여 _subfunction_type_list를 뽑아내는 동작을 위해 필요하다.
-        self._first_execute: bool = True
+        # SuperService 안에 있는 req()들에 대한 정보가 스캔되었는지 여부. 스캔된 req()들에 대한 정보는 _sub_service_type_list에 저장된다.
+        self._is_scanned: bool = False
 
         # scheduling에 대한 결과를 super thing이 넣어주기 위해 존재함
-        # key: {requester_middleware}_{scenario}, value: SoPSuperScheduleActionRequest
-        self._temporary_scheduling_table: Dict[str,
-                                               SoPSuperScheduleRequest] = {}
-        # scheduling이 끝나면 해당 scenario에 대해 어떤 subfunction_type에 대해 thing을 선택할 것인지 정해진다.
+        #     super_service_request_key: str = make_super_request_key(requester_middleware, scenario)
+        #     super_service_request_key: {requester_middleware}@{scenario}, value: MXSuperScheduleRequest
+        self._temporary_scheduling_table: Dict[str, MXSuperScheduleRequest] = {}
+
+        # scheduling이 끝나면 해당 scenario에 대해 어떤 sub_service_type에 대해 thing을 선택할 것인지 정해진다.
         # 이렇게 하는 이유는 scenario를 반복해서 돌릴 때마다 다른 thing을 선택하는 것이 아니라 전에 선택했던 thing에 있는 service를 실행하기 위함이다.
-        # key: {requester_middleware}_{scenario}, value: SoPSuperExecuteActionRequest
-        self._mapping_table: Dict[str, SoPSuperExecuteRequest] = {}
+        #     super_service_request_key: str = make_super_request_key(requester_middleware, scenario)
+        #     super_service_request_key: {requester_middleware}@{scenario}, value: MXSuperExecuteRequest
+        self._mapping_table: Dict[str, MXSuperExecuteRequest] = {}
 
-        # super function의 동작을 하는데 있어 필요한 subscribe, unsubscribe동작을 수행하기 위해 필요
-        self._subscribe_queue: Queue = Queue()
-        self._unsubscribe_queue: Queue = Queue()
-
-        # super function의 동작을 하는데 소모된 시간을 측정하기 위해 필요
-        # self.super_schedule_duration_list = []
-        # self.super_execute_duration_list = []
-
-        # for test super service request parallel feature
-        self._request_parallel = True
-        self._single_request_mode: SoPSingleSubRequestSendType = SoPSingleSubRequestSendType.PARALLEL
-
-    def __eq__(self, o: object) -> bool:
-        subfunction_list_check = self.get_subfunction_type_list(
-        ) == o.get_subfunction_type_list()
-        return super().__eq__(o) and subfunction_list_check
+        self._schedule_running: bool = False
 
-    def _add_subfunction_reqline(self, subfunction_reqline: SoPSubFunctionReqline):
-        '''
-            super function에 명세된 req() 라인 수 만큼 존재한다. 따라서 중복된 subfunction_type이 존재할 수 없다.
-        '''
-        subfunction_reqline._subrequest_order = len(
-            self._subfunction_reqline_list)
-        self._subfunction_reqline_list.append(subfunction_reqline)
-
-    def _remove_subfunction_reqline(self, subfunction_reqline: SoPSubFunctionReqline):
-        if subfunction_reqline in self._subfunction_reqline_list:
-            self._subfunction_reqline_list.remove(subfunction_reqline)
-
-    def _request_subaction(self, subaction_request: Union[SoPSubScheduleRequest, SoPSubExecuteRequest]) -> None:
-        subaction_request.timer_start()
-        subaction_msg = subaction_request._trigger_msg
-
-        # 필요한 토픽을 구독한다.
-        if isinstance(subaction_request, SoPSubScheduleRequest):
-            subschedule_msg: SoPSubScheduleMessage = subaction_request._trigger_msg
-            self._subscribe_queue.put(SoPProtocolType.Super.MS_RESULT_SCHEDULE.value % (subschedule_msg._subfunction_name,
-                                                                                        'SUPER',
-                                                                                        subschedule_msg._target_middleware_name,
-                                                                                        subschedule_msg._request_ID))
-        elif isinstance(subaction_request, SoPSubExecuteRequest):
-            subexecute_msg: SoPSubExecuteMessage = subaction_request._trigger_msg
-            self._subscribe_queue.put(SoPProtocolType.Super.MS_RESULT_EXECUTE.value % (subexecute_msg._subfunction_name,
-                                                                                       'SUPER',
-                                                                                       subexecute_msg._target_middleware_name,
-                                                                                       subexecute_msg._request_ID))
-        while self._subscribe_queue.empty():
-            time.sleep(THREAD_TIME_OUT)
-
-        if isinstance(subaction_request, SoPSubScheduleRequest):
-            subschedule_msg: SoPSubScheduleMessage = subaction_request._trigger_msg
-            self.send_SM_SCHEDULE(subschedule_msg)
-
-            if subaction_request._trigger_msg._status == SoPScheduleStatus.CHECK.value:
-                SOPLOG_DEBUG(
-                    f'[{subaction_request._action_type.value.upper()} CHECK START] {subaction_msg._subfunction_name}|{subaction_msg._target_thing_name}|{subaction_msg._target_middleware_name}', 'cyan')
-            elif subaction_request._trigger_msg._status == SoPScheduleStatus.CONFIRM.value:
-                SOPLOG_DEBUG(
-                    f'[{subaction_request._action_type.value.upper()} CONFIRM START] {subaction_msg._subfunction_name}|{subaction_msg._target_thing_name}|{subaction_msg._target_middleware_name}', 'cyan')
-        elif isinstance(subaction_request, SoPSubExecuteRequest):
-            subexecute_msg: SoPSubExecuteMessage = subaction_request._trigger_msg
-            self.send_SM_EXECUTE(subexecute_msg)
-
-            SOPLOG_DEBUG(
-                f'[{subaction_request._action_type.value.upper()} START] {subaction_msg._subfunction_name}|{subaction_msg._target_thing_name}|{subaction_msg._target_middleware_name}', 'cyan')
-
-    def print_request_result(self, request: SoPRequest, color: str, duration: float = None):
-        if isinstance(request, SoPSubScheduleRequest):
-            SOPLOG_DEBUG(f'[{request._action_type.value.upper()} {request._status.value.upper()} END] {request._trigger_msg._subfunction_name}|{request._trigger_msg._target_thing_name}|{request._trigger_msg._target_middleware_name}, duration: {request.duration():.4f} Sec', color)
-        elif isinstance(request, SoPSuperScheduleRequest):
-            if request._status == SoPScheduleStatus.CHECK:
-                SOPLOG_DEBUG(f'[{request._action_type.value.upper()} {request._status.value.upper()} END] {request._trigger_msg._super_function_name}|{request._trigger_msg._super_thing_name}|{request._trigger_msg._super_middleware_name}, duration: {request.check_duarion():.4f} Sec', color)
-            elif request._status == SoPScheduleStatus.CONFIRM:
-                SOPLOG_DEBUG(f'[{request._action_type.value.upper()} {request._status.value.upper()} END] {request._trigger_msg._super_function_name}|{request._trigger_msg._super_thing_name}|{request._trigger_msg._super_middleware_name}, duration: {request.confirm_duarion():.4f} Sec', color)
-        elif isinstance(request, SoPSubExecuteRequest):
-            SOPLOG_DEBUG(f'[{request._action_type.value.upper()} END] {request._trigger_msg._subfunction_name}|{request._trigger_msg._target_thing_name}|{request._trigger_msg._target_middleware_name}, duration: {request.duration():.4f} Sec', color)
-        elif isinstance(request, SoPSuperExecuteRequest):
-            pass
+        if not inspect.ismethod(func):
+            raise MXTypeError('self._func must be a instance method')
 
-    def _subschedule_action_parallel(self, super_schedule_request: SoPSuperScheduleRequest, target_schedule_action: SoPScheduleStatus, result_schedule_action: SoPScheduleStatus, timeout: float = 3) -> List[SoPSubScheduleRequest]:
-        '''
-            subaction 요청을 병렬로 실행하는 함수.
-            기존에 하나씩 요청을 보내고 응답을 기다리는 방식에서 모든 요청 패킷을 빠르게 먼저 보내고 응답을 기다리는 방식으로 변경.
-        '''
+    def __eq__(self, o: 'MXSuperFunction') -> bool:
+        instance_check = isinstance(o, MXSuperFunction)
 
-        subschedule_action_start_time = get_current_time()
-        # 병렬로 subschedule 요청을 보낸다.
-        if self._single_request_mode == SoPSingleSubRequestSendType.PARALLEL:
-            for subrequest_key, subfunction_reqline in super_schedule_request._subfunction_reqline_table.items():
-                for candidate_request in subfunction_reqline._candidate_request_list:
-                    if candidate_request._status != target_schedule_action:
-                        continue
-
-                    # 미들웨어에게 현재 요청인 check 인지 confirm인지 알려주기 위해 trigger_msg에 status를 추가함.
-                    candidate_request._trigger_msg._status = result_schedule_action.value.lower()
-                    self._request_subaction(candidate_request)
-
-            # 해당 super function action에 대한 subfunction들에게 subschedule요청을 보낸 후, 모든 subschedule 결과를 받을 때까지 기다린다.
-            for subrequest_key, subfunction_reqline in super_schedule_request._subfunction_reqline_table.items():
-                for candidate_request in subfunction_reqline._candidate_request_list:
-                    if candidate_request._status != target_schedule_action:
-                        continue
-                    candidate_request._result_msg = candidate_request.get_result_msg(
-                        timeout=timeout)
-                    candidate_request._status = result_schedule_action
-                    subschedule_result_msg: SoPSubScheduleResultMessage = candidate_request._result_msg
-
-                    candidate_request.timer_end()
-                    self.print_request_result(candidate_request, 'cyan')
-
-                    # 굳이 구독 해제를 할 필요가 없다. 재호출될 가능성이 높음.
-                    # self._unsubscribe_queue.put(subschedule_result_msg.topic())
-                    # while not self._unsubscribe_queue.empty():
-                    #     time.sleep(THREAD_TIME_OUT)
-        elif self._single_request_mode == SoPSingleSubRequestSendType.SERIAL:
-            for subrequest_key, subfunction_reqline in super_schedule_request._subfunction_reqline_table.items():
-                for candidate_request in subfunction_reqline._candidate_request_list:
-                    if candidate_request._status != target_schedule_action:
-                        continue
-
-                    # 미들웨어에게 현재 요청이 check 인지 confirm인지 알려주기 위해 trigger_msg에 status를 추가함.
-                    candidate_request._trigger_msg._status = result_schedule_action.value.lower()
-                    self._request_subaction(candidate_request)
-
-                    candidate_request._result_msg = candidate_request.get_result_msg(
-                        timeout=timeout)
-                    candidate_request._status = result_schedule_action
-                    subschedule_result_msg: SoPSubExecuteResultMessage = candidate_request._result_msg
-
-                    candidate_request.timer_end()
-                    self.print_request_result(candidate_request, 'cyan')
-
-                    # 굳이 구독 해제를 할 필요가 없다. 재호출될 가능성이 높음.
-                    # self._unsubscribe_queue.put(subschedule_result_msg.topic())
-                    # while not self._unsubscribe_queue.empty():
-                    #     time.sleep(THREAD_TIME_OUT)
-
-        if result_schedule_action == SoPScheduleStatus.CHECK:
-            super_schedule_request._check_duation = get_current_time() - \
-                subschedule_action_start_time
-        elif result_schedule_action == SoPScheduleStatus.CONFIRM:
-            super_schedule_request._confirm_duation = get_current_time() - \
-                subschedule_action_start_time
-        super_schedule_request._status = result_schedule_action
-        self.print_request_result(
-            super_schedule_request, 'green')
-
-    def _select_target_subfunction_by_policy(self, super_action_request: SoPSuperScheduleRequest) -> SoPSubScheduleRequest:
-        for subfunction_reqline in self._subfunction_reqline_list:
-            reqline_policy = subfunction_reqline._subfunction_type.get_policy()
-            subrequest_key = make_sub_request_key(
-                subfunction_reqline._subfunction_type.get_name(), subfunction_reqline._subrequest_order)
-            target_subfunction_reqline = super_action_request._subfunction_reqline_table[
-                subrequest_key]
-
-            if reqline_policy == SoPPolicy.ALL:
-                for candidate_request in target_subfunction_reqline._candidate_request_list:
-                    if candidate_request._status == SoPScheduleStatus.CHECK:
-                        candidate_request._status = SoPScheduleStatus.SELECT
-            elif reqline_policy == SoPPolicy.SINGLE:
+        return super().__eq__(o) and instance_check
+
+    def __getstate__(self):
+        state = super().__getstate__()
+
+        state['_sub_service_request_list'] = self._sub_service_request_list
+        state['_is_scanned'] = self._is_scanned
+        state['_temporary_scheduling_table'] = self._temporary_scheduling_table
+        state['_mapping_table'] = self._mapping_table
+
+        del state['_schedule_running']
+
+        return state
+
+    def __setstate__(self, state):
+        super().__setstate__(state)
+
+        self._sub_service_request_list = state['_sub_service_request_list']
+        self._is_scanned = state['_is_scanned']
+        self._temporary_scheduling_table = state['_temporary_scheduling_table']
+        self._mapping_table = state['_mapping_table']
+
+        self._schedule_running = False
+
+    def _add_sub_service_request(self, sub_service_request: MXSubServiceRequest):
+        sub_service_request._sub_service_request_order = len(
+            self._sub_service_request_list)
+        self._sub_service_request_list.append(sub_service_request)
+
+    def _remove_sub_service_request(self, sub_service_request: MXSubServiceRequest):
+        if sub_service_request in self._sub_service_request_list:
+            self._sub_service_request_list.remove(sub_service_request)
+
+    def _request_subschedule(self, subschedule_request: MXSubScheduleRequest) -> None:
+        subschedule_request.timer_start()
+        subschedule_msg = subschedule_request.trigger_msg
+
+        # 필요한 토픽 구독과 발행을 한번에 수행한다.
+        if not isinstance(subschedule_request, MXSubScheduleRequest):
+            raise MXTypeError(f'Invalid type of subschedule_request: {type(subschedule_request)}')
+
+        self._send_SM_SCHEDULE(subschedule_msg)
+
+    def _select_target_sub_service_by_range_type(self, super_schedule_request: MXSuperScheduleRequest, single_select_func: Callable) -> MXSubScheduleRequest:
+        for sub_service_request in self._sub_service_request_list:
+            sub_service_request_range_type = sub_service_request._sub_service_type.get_range_type()
+            sub_service_request_key = make_sub_service_request_key(sub_service_name=sub_service_request._sub_service_type.get_name(),
+                                                                   sub_service_request_order=sub_service_request._sub_service_request_order)
+            target_sub_service_request = super_schedule_request._sub_service_request_table[sub_service_request_key]
+
+            if sub_service_request_range_type == MXRangeType.ALL:
+                for candidate_request in target_sub_service_request._candidate_request_list:
+                    if candidate_request._status == MXScheduleStatus.CHECK:
+                        candidate_request._status = MXScheduleStatus.SELECT
+            elif sub_service_request_range_type == MXRangeType.SINGLE:
                 while True:
-                    selected_request = random.choice(
-                        target_subfunction_reqline._candidate_request_list)
-                    if selected_request._status == SoPScheduleStatus.CHECK:
-                        selected_request._status = SoPScheduleStatus.SELECT
+                    selected_request = single_select_func(target_sub_service_request._candidate_request_list)
+                    if selected_request._status == MXScheduleStatus.CHECK:
+                        selected_request._status = MXScheduleStatus.SELECT
                         break
 
-    def _check_parallel(self, super_action_request: SoPSuperScheduleRequest, timeout: float = 3) -> List[SoPSubScheduleRequest]:
-        self._subschedule_action_parallel(
-            super_action_request, SoPScheduleStatus.INIT, SoPScheduleStatus.CHECK, timeout)
-
-    def _confirm_parallel(self, super_action_request: SoPSuperScheduleRequest, timeout: float = 3) -> bool:
-        self._subschedule_action_parallel(
-            super_action_request, SoPScheduleStatus.SELECT, SoPScheduleStatus.CONFIRM, timeout)
-
-    def _subexecute_parallel(self, super_execute_request: SoPSuperExecuteRequest, timeout: float = 3) -> List[Union[SoPSubScheduleRequest, SoPSubExecuteRequest]]:
-        # 병렬로 subaction 요청을 보낸다.
-        for subrequest_key, subfunction_reqline in super_execute_request._subfunction_reqline_table.items():
-            for target_request in subfunction_reqline._target_request_list:
-                self._request_subaction(target_request)
-
-        # 해당 super function action에 대한 subfunction들에게 subaction요청을 보낸 후, 모든 subaction 결과를 받을 때까지 기다린다.
-        for subrequest_key, subfunction_reqline in super_execute_request._subfunction_reqline_table.items():
-            for target_request in subfunction_reqline._target_request_list:
-                target_request._result_msg = target_request.get_result_msg(
-                    timeout=timeout)
-                subexecute_msg: SoPSubExecuteMessage = target_request._trigger_msg
-                subaction_result_msg: SoPSubExecuteResultMessage = target_request._result_msg
-
-                target_request.timer_end()
-                SOPLOG_DEBUG(
-                    f'[{target_request._action_type.value.upper()} END] {subexecute_msg._subfunction_name}|{subexecute_msg._target_thing_name} duration: {target_request.duration():.4f} Sec', 'cyan')
+    def _subschedule_parallel(self, super_schedule_request: MXSuperScheduleRequest, target_schedule_status: MXScheduleStatus, result_schedule_status: MXScheduleStatus) -> List[MXSubScheduleRequest]:
+        subschedule_start_time = get_current_time()
+
+        # 병렬로 subschedule 요청을 보낸다.
+        for sub_service_request in super_schedule_request._sub_service_request_table.values():
+            candidate_subschedule_request_list = [candidate_request for candidate_request in sub_service_request._candidate_request_list
+                                                  if candidate_request._status == target_schedule_status]
+
+            for candidate_subschedule_request in candidate_subschedule_request_list:
+                # 미들웨어에게 현재 요청인 check 인지 confirm인지 알려주기 위해 trigger_msg에 status를 추가함.
+                candidate_subschedule_request.trigger_msg.status = result_schedule_status
+                candidate_subschedule_msg = candidate_subschedule_request.trigger_msg
+                MXLOG_DEBUG(f'[SUB_SCHEDULE {candidate_subschedule_msg._status.value.upper()} START] '
+                            f'{candidate_subschedule_msg.sub_service_name}|{candidate_subschedule_msg.target_thing_name}|'
+                            f'{candidate_subschedule_msg.target_middleware_name}', 'cyan')
+                self._request_subschedule(candidate_subschedule_request)
+
+            # 해당 super service의 sub_service들에게 subschedule 요청을 보낸 후, 모든 subschedule 결과를 받을 때까지 기다린다.
+            for candidate_subschedule_request in candidate_subschedule_request_list:
+                candidate_subschedule_request.result_msg = candidate_subschedule_request.get_result_msg()
+                candidate_subschedule_request._status = result_schedule_status
+
+                candidate_subschedule_request.timer_end()
+                MXLOG_DEBUG(f'[SUB_SCHEDULE {candidate_subschedule_request._status.value.upper()} END] '
+                            f'{candidate_subschedule_request.trigger_msg.sub_service_name}|{candidate_subschedule_request.trigger_msg.target_thing_name}|'
+                            f'{candidate_subschedule_request.trigger_msg.target_middleware_name}, duration: {candidate_subschedule_request.duration():.4f} Sec', 'cyan')
 
                 # 굳이 구독 해제를 할 필요가 없다. 재호출될 가능성이 높음.
-                # self._unsubscribe_queue.put(subaction_result_msg.topic())
+                # subschedule_result_msg: MXSubScheduleResultMessage = candidate_subschedule_request._result_msg
+                # self._unsubscribe_queue.put(subschedule_result_msg.topic)
                 # while not self._unsubscribe_queue.empty():
-                #     time.sleep(THREAD_TIME_OUT)
-
-                # subexecute 결과를 받은 후, 다시 넣는다. req() 함수에서 꺼내어 사용하기 위함.
-                target_request.put_result_msg(subaction_result_msg)
+                #     time.sleep(0.001)
 
-    # def _subschedule_nonparallel(self, target_subfunction_list: List[SoPFunction], subschedule_result_list: List[SoPErrorType], super_schedule_msg: SoPSuperScheduleMessage):
-    #     '''
-    #         subschedule 요청을 직렬로 실행하는 함수.
-    #         기존에 방식처럼 하나씩 요청을 보내고 응답을 받으면 다음 요청으로 넘어가는 방식.
-    #     '''
-    #     for target_subfunction in target_subfunction_list:
-    #         self._request_subschedule(target_subfunction, super_schedule_msg)
-
-    #         # 하나의 subfunction의 subschedule 결과를 받을 때까지 기다린다. 이후 다음 subfunction에게 subschedule 요청을 보내고 받는 것을 반복.
-    #         for subschedule_info in self._subschedule_request_list:
-    #             subschedule_msg: SoPSubScheduleMessage = subschedule_info['subschedule_msg']
-    #             subfunction_check = subschedule_msg._subfunction_name == target_subfunction.get_name()
-    #             target_thing_check = subschedule_msg._target_thing_name == target_subfunction.get_thing_name()
-    #             target_middleware_check = subschedule_msg._target_middleware_name == target_subfunction.get_middleware_name()
-    #             super_thing_check = subschedule_msg._super_thing_name == super_schedule_msg._super_thing_name
-    #             # self._subschedule_request_list에 있는 request중에 target_subfunction에 해당하는 요청에 대한 결과를 찾는다.
-    #             if subfunction_check and target_thing_check and target_middleware_check and super_thing_check:
-    #                 result_queue: Queue = subschedule_info['result_queue']
-
-    #                 subschedule_result_msg: SoPSubScheduleResultMessage = result_queue.get()
-    #                 SOPLOG_DEBUG(
-    #                     f'[SUBSCHEDULE END] {subschedule_result_msg._subfunction_name}|{subschedule_result_msg._target_thing_name} duration: {(subschedule_info["end_time"] - subschedule_info["start_time"]):.4f}', 'cyan')
-
-    #                 self._unsubscribe_queue.put(subschedule_result_msg.topic())
-    #                 while not self._unsubscribe_queue.empty():
-    #                     time.sleep(THREAD_TIME_OUT)
-
-    #                 subschedule_result_list.append(
-    #                     subschedule_result_msg._error)
-
-    def check_reqline_confirm(self, super_action_request: SoPSuperScheduleRequest) -> SoPErrorType:
-        # 스케쥴링 과정에서 super function의 reqline 중 confirm 된 request가 하나도 없는 reqline이 존재한다면 에러를 발생시킨다.
-        for k, subfunction_reqline in super_action_request._subfunction_reqline_table.items():
-            for candidate_request in subfunction_reqline._candidate_request_list:
-                if candidate_request._status == SoPScheduleStatus.CONFIRM:
+        super_schedule_request._status = result_schedule_status
+        if super_schedule_request._status == MXScheduleStatus.CHECK:
+            super_schedule_request._check_duration = get_current_time() - subschedule_start_time
+            MXLOG_DEBUG(f'[SUPER_SCHEDULE CHECK END] '
+                        f'{super_schedule_request.trigger_msg.super_service_name}|{super_schedule_request.trigger_msg.super_thing_name}|'
+                        f'{super_schedule_request.trigger_msg.super_middleware_name}, duration: {super_schedule_request.confirm_duration():.4f} Sec', 'green')
+        elif super_schedule_request._status == MXScheduleStatus.CONFIRM:
+            super_schedule_request._confirm_duration = get_current_time() - subschedule_start_time
+            MXLOG_DEBUG(f'[SUPER_SCHEDULE CONFIRM END] '
+                        f'{super_schedule_request.trigger_msg.super_service_name}|{super_schedule_request.trigger_msg.super_thing_name}|'
+                        f'{super_schedule_request.trigger_msg.super_middleware_name}, duration: {super_schedule_request.confirm_duration():.4f} Sec', 'green')
+
+    def _check_parallel(self, super_schedule_request: MXSuperScheduleRequest) -> List[MXSubScheduleRequest]:
+        self._subschedule_parallel(super_schedule_request=super_schedule_request,
+                                   target_schedule_status=MXScheduleStatus.INIT,
+                                   result_schedule_status=MXScheduleStatus.CHECK)
+
+    def _confirm_parallel(self, super_schedule_request: MXSuperScheduleRequest) -> bool:
+        self._subschedule_parallel(super_schedule_request=super_schedule_request,
+                                   target_schedule_status=MXScheduleStatus.SELECT,
+                                   result_schedule_status=MXScheduleStatus.CONFIRM)
+
+    def _check_sub_service_request_confirm(self, super_schedule_request: MXSuperScheduleRequest) -> bool:
+        # 스케쥴링 과정에서 super service의 sub_service_request 중 confirm 된 request가 하나도 없는 sub_service_request가 존재한다면 에러를 발생시킨다.
+        for sub_service_request in super_schedule_request._sub_service_request_table.values():
+            for candidate_request in sub_service_request._candidate_request_list:
+                if candidate_request._status == MXScheduleStatus.CONFIRM:
                     break
             else:
-                return SoPErrorType.FAIL
+                return False
         else:
-            return SoPErrorType.NO_ERROR
+            return True
+
+    def _check_confirm_parallel(self, super_schedule_request: MXSuperScheduleRequest) -> bool:
+        self._check_parallel(super_schedule_request=super_schedule_request)
+        self._select_target_sub_service_by_range_type(super_schedule_request=super_schedule_request, single_select_func=lambda x: x[0])
+        self._confirm_parallel(super_schedule_request=super_schedule_request)
+
+        return True
 
-    def _super_action_wrapper(self, super_action_request: Union[SoPSuperScheduleRequest, SoPSuperExecuteRequest], hierarchical_service_table: Dict[str, List[SoPService]]):
+    def _print_schedule_result(self, scenario_name: str, requester_middleware_name: str):
+        schedule_result_string = '\n[SCHEDULE RESULT] ============================================\n'
+        super_request_key = make_super_request_key(scenario_name=scenario_name, requester_middleware_name=requester_middleware_name)
+        for super_k, super_execute_req in self._mapping_table.items():
+            if super_k != super_request_key:
+                continue
+            schedule_result_string += f'super_key: {super_k} -> super_service: {self._name}\n'
+            for sub_k, sub_service_req in super_execute_req._sub_service_request_table.items():
+                schedule_result_string += ' ' * 4 + f'sub_key: {sub_k} -> sub_service: {sub_service_req._sub_service_type.get_name()}|{sub_service_req._sub_service_request_order}\n'
+                for target_req in sub_service_req._target_request_list:
+                    schedule_result_string += ' ' * 8 + f'target: {target_req.trigger_msg.sub_service_name}|{target_req.trigger_msg.target_middleware_name}\n'
+        schedule_result_string += '==============================================================\n'
+        MXLOG_DEBUG(schedule_result_string, 'green')
+
+    def _super_schedule_wrapper(self, super_schedule_request: MXSuperScheduleRequest, hierarchical_service_table: Dict[str, List[MXService]], timeout: float = 1000):
         '''
-            super function의 하위 함수에 대한 정보를 추출한다.
+            super service의 하위 함수에 대한 정보를 추출한다.
             service_list 구조는
+
             ============================================
-            super_function -> sub_function_type_list
-                        -> sub_function_list
+            super_service -> sub_function_type_list
+                           -> sub_function_list
             ============================================
+
             로 이루어져있다.
             sub_function_type_list과 sub_function_list는 독립적인 공간을 가진다.
-            super_function 내부에 req함수 가 존재하여 사용자가 요청하고 싶은 subfunction이 명세되어있는데 여기서 명세되어지는
-            subfunction은 실제 타겟 subfunction이 아닌 subfunction_type이다. 실제 subfunction 정보는 middleware로 부터 받은
-            service_list를 통해 추출한다. 그리고 해당 정보는 super_function의 subfunction_list에 저장된다.
+            super_service 내부에 req함수 가 존재하여 사용자가 요청하고 싶은 sub_service이 명세되어있는데 여기서 명세되어지는
+            sub_service은 실제 타겟 sub_service이 아닌 sub_service_type이다. 실제 sub_service 정보는 middleware로 부터 받은
+            service_list를 통해 추출한다. 그리고 해당 정보는 super_service의 sub_service_list에 저장된다.
         '''
+        if not isinstance(super_schedule_request, MXSuperScheduleRequest):
+            raise MXTypeError(f'[{get_current_function_name()}] Wrong Request type: {type(super_schedule_request)}')
 
-        try:
-            super_action_error = SoPErrorType.FAIL
-            super_request_key = make_super_request_key(
-                super_action_request._trigger_msg._requester_middleware_name, super_action_request._trigger_msg._scenario)
-
-            # 만약 super_schedule_msg이 SoPSuperScheduleMessage이 아니라면 에러를 발생시킨다.
-            if not isinstance(super_action_request, (SoPSuperScheduleRequest, SoPSuperExecuteRequest)):
-                SOPLOG_DEBUG(
-                    f'[SUPER_SCHEDULE ERROR] Wrong SoPSuperScheduleMessage type: {type(super_action_request)}', 'red')
-                raise Exception
-
-            SOPLOG_DEBUG(
-                f'[{super_action_request._action_type.value.upper()} START] -------- Start {self._name} {super_action_request._action_type.value} by {super_action_request._trigger_msg._scenario} scenario --------', 'green')
-
-            if isinstance(super_action_request, SoPSuperScheduleRequest):
-                hierarchical_function_service_table: List[SoPFunction] = hierarchical_service_table["function"]
-
-                # 후보 subfunction들에 대해서 스케쥴링을 진행한다.
-                if self._request_parallel:
-                    super_action_request.generate_subschedule_request(
-                        self._subfunction_reqline_list, hierarchical_function_service_table)
-                    # TODO: 각 reqline마다 check, confirm이 이루어지고 나서 다음 reqline으로 넘어가야한다. 그게 제대로된 스케쥴링이다.
-                    # 어느 한 reqline이 confirm 됨으로 인해서 다음 reqline의 스케쥴링에 영향을 주기 때문임.
-                    # self._dfddf() # reqline을 돌면서 _check_parallel + _confirm_parallel
-                    self._check_parallel(super_action_request, timeout=30)
-                    self._select_target_subfunction_by_policy(
-                        super_action_request)
-                    self._confirm_parallel(super_action_request, timeout=30)
-                else:
-                    # TODO: update nonparallel feature
-                    pass
-
-                # 만약 현재 super function의 subfunction_list가 비어있는 경우 에러를 발생시킨다.
-                if len(super_action_request._subfunction_reqline_table) == 0 and len(self._subfunction_reqline_list) != 0:
-                    raise Exception(
-                        f'No target_subfunction_list found in {self._name} super function')
-            elif isinstance(super_action_request, SoPSuperExecuteRequest):
-                # self._scheduling_table에서 해당 항목을 제거한다.
-                super_action_request.exchange_argument()
-
-                if self._request_parallel:
-                    super_action_request._current_reqline_num = 0
-                    self._subexecute_parallel(
-                        super_action_request, timeout=30)
-                else:
-                    # TODO: update nonparallel feature
-                    pass
+        super_schedule_msg = super_schedule_request.trigger_msg
+        requester_middleware_name = super_schedule_msg.requester_middleware_name
+        scenario = super_schedule_msg.scenario
+        super_service_request_key = make_super_request_key(scenario_name=scenario,
+                                                           requester_middleware_name=requester_middleware_name)
 
-                self._running = True
+        MXLOG_DEBUG(f'[SUPER_SCHEDULE START] {self._name} by scenario {scenario}.', 'green')
 
-                super_execute_result = func_timeout(
-                    self._timeout / 1000, self._func, args=(*tuple([super_request_key] + list(super_action_request._trigger_msg.tuple_arguments())), ))
+        try:
+            super_schedule_request._running = True
+            self._schedule_running = True
+            error = MXErrorCode.NO_ERROR
+
+            # 후보 sub_service들에 대해서 스케쥴링을 진행한다.
+            super_schedule_request.generate_sub_service_schedule_request(self._sub_service_request_list, hierarchical_service_table['functions'])
+
+            # func_timeout(timeout, self._check_confirm_parallel, args=(super_schedule_request, ))
+            current_thread = threading.current_thread()
+            self._run_with_timeout(timeout=timeout, func=self._check_confirm_parallel, name=current_thread.name,
+                                   user_data=dict(scenario=super_schedule_msg.scenario, requester_middleware=requester_middleware_name), args=(super_schedule_request, ))
+
+            # 만약 현재 super service의 sub_service_list가 비어있는 경우 에러를 발생시킨다.
+            if len(super_schedule_request._sub_service_request_table) == 0 and len(self._sub_service_request_list) != 0:
+                raise Exception(f'No target_sub_service_list found in {self._name} super service')
         except KeyboardInterrupt as e:
             print_error(e)
-            SOPLOG_DEBUG('Function execution exit by user', 'red')
+            MXLOG_DEBUG('Function scheduling exit by user', 'red')
             raise e
         except FunctionTimedOut as e:
-            # print_error(e)
-            SOPLOG_DEBUG(
-                f'[FUNC TIMEOUT] {super_action_request._action_type.value} of {self._name} by scenario {super_action_request._trigger_msg._requester_middleware_name}|{super_action_request._trigger_msg._scenario} timeout...', 'red')
-            super_action_error = SoPErrorType.TIMEOUT
-
-            if super_action_request._action_type == SoPActionType.SUPER_EXECUTE:
-                self._mapping_table.pop(super_request_key)
-                self._running = False
-            elif super_action_request._action_type == SoPActionType.SUPER_SCHEDULE:
-                self._temporary_scheduling_table.pop(super_request_key)
-            super_execute_result = None
+            MXLOG_DEBUG(f'[SUPER_SCHEDULE TIMEOUT] {super_schedule_request._action_type.value} of {self._name}'
+                        'by scenario {requester_middleware_name}|{scenario} timeout...', 'red')
 
+            error = MXErrorCode.TIMEOUT
             return False
         except Exception as e:
             print_error(e)
-            SOPLOG_DEBUG(
-                f'[{super_action_request._action_type.value.upper()} FAILED] {super_action_request._action_type.value} of {self._name} by scenario {super_action_request._trigger_msg._requester_middleware_name}|{super_action_request._trigger_msg._scenario} failed...', 'red')
-            super_action_error = SoPErrorType.FAIL
-
-            if super_action_request._action_type == SoPActionType.SUPER_EXECUTE:
-                self._mapping_table.pop(super_request_key)
-                self._running = False
-            elif super_action_request._action_type == SoPActionType.SUPER_SCHEDULE:
-                self._temporary_scheduling_table.pop(super_request_key)
-            super_execute_result = None
+            MXLOG_DEBUG(f'[SUPER_SCHEDULE FAILED] {super_schedule_request._action_type.value} of {self._name}'
+                        'by scenario {requester_middleware_name}|{scenario} failed...', 'red')
 
+            error = MXErrorCode.FAIL
             return False
         else:
-            if isinstance(super_action_request, SoPSuperScheduleRequest):
-                super_action_error = self.check_reqline_confirm(
-                    super_action_request)
-                super_execute_request = SoPSuperExecuteRequest()
-                super_execute_request.generate_subexecute_request_list(
-                    super_action_request)
-                # super_execute_request._subexecute_request_list = [to_subexecute_request(
-                #     subschedule_request) for subschedule_request in super_action_request.subschedule_request_target_list()]
-                self._temporary_scheduling_table.pop(super_request_key)
-                self._mapping_table[super_request_key] = super_execute_request
-                # self.super_schedule_duration_list.append(
-                #     super_action_request.duration)
-            elif isinstance(super_action_request, SoPSuperExecuteRequest):
-                pass
-                # self.super_execute_duration_list.append(
-                #     super_action_request.duration)
+            if not self._check_sub_service_request_confirm(super_schedule_request):
+                return False
 
-            super_action_error = SoPErrorType.NO_ERROR
+            super_service_execute_request = MXSuperExecuteRequest(super_schedule_request=super_schedule_request)
+            self._mapping_table[super_service_request_key] = super_service_execute_request
+
+            error = error = MXErrorCode.NO_ERROR
             return True
         finally:
-            if isinstance(super_action_request, SoPSuperScheduleRequest):
-                super_schedule_msg: SoPSuperScheduleMessage = super_action_request._trigger_msg
-                self.send_SM_RESULT_SCHEDULE(super_schedule_msg._super_function_name,
-                                             super_schedule_msg._super_thing_name,
-                                             super_schedule_msg._super_middleware_name,
-                                             super_schedule_msg._requester_middleware_name,
-                                             super_schedule_msg._scenario,
-                                             super_action_error)
-            elif isinstance(super_action_request, SoPSuperExecuteRequest):
-                super_execute_msg: SoPSuperExecuteMessage = super_action_request._trigger_msg
-                self.send_SM_RESULT_EXECUTE(super_execute_msg._super_function_name,
-                                            super_execute_msg._super_thing_name,
-                                            super_execute_msg._super_middleware_name,
-                                            super_execute_msg._requester_middleware_name,
-                                            super_execute_msg._scenario,
-                                            self._return_type,
-                                            super_execute_result,
-                                            super_action_error)
-            super_action_request.timer_end()
-            SOPLOG_DEBUG(
-                f'[{super_action_request._action_type.value.upper()} FINISH] {super_action_request._action_type.value} of {self._name} by scenario {super_action_request._trigger_msg._requester_middleware_name}|{super_action_request._trigger_msg._scenario} finish. duration: {super_action_request.duration():.4f} Sec', 'green')
-
-    def super_action(self, super_action_request: Union[SoPSuperScheduleRequest, SoPSuperExecuteRequest], hierarchical_service_table: Dict[str, List[SoPService]]) -> None:
-        super_action_thread = SoPThread(
-            func=self._super_action_wrapper,
-            name=f'{self._func.__name__}_{super_action_request._action_type.value}_thread',
-            daemon=True,
-            arg_list=(super_action_request, hierarchical_service_table, ))
-        super_action_thread.start()
+            self._send_SM_RESULT_SCHEDULE(super_service_name=super_schedule_msg.super_service_name,
+                                          super_thing_name=super_schedule_msg.super_thing_name,
+                                          super_middleware_name=super_schedule_msg.super_middleware_name,
+                                          requester_middleware_name=requester_middleware_name,
+                                          scenario=scenario,
+                                          error=error)
+
+            super_schedule_request.timer_end()
+            super_schedule_request._running = False
+            self._schedule_running = False
+            self._temporary_scheduling_table.pop(super_service_request_key)
+            MXLOG_DEBUG(f'[SUPER_SCHEDULE END] {self._name} by scenario {scenario}. duration: {super_schedule_request.duration():.4f} Sec', 'green')
+            self._print_schedule_result(scenario_name=scenario, requester_middleware_name=requester_middleware_name)
+
+    def _super_execute_wrapper(self, super_service_execute_request: MXSuperExecuteRequest):
+        '''
+            super service의 하위 함수에 대한 정보를 추출한다.
+            service_list 구조는
+
+            ============================================
+            super_service -> sub_function_type_list
+                           -> sub_function_list
+            ============================================
+
+            로 이루어져있다.
+            sub_function_type_list과 sub_function_list는 독립적인 공간을 가진다.
+            super_service 내부에 req함수 가 존재하여 사용자가 요청하고 싶은 sub_service이 명세되어있는데 여기서 명세되어지는
+            sub_service은 실제 타겟 sub_service이 아닌 sub_service_type이다. 실제 sub_service 정보는 middleware로 부터 받은
+            service_list를 통해 추출한다. 그리고 해당 정보는 super_service의 sub_service_list에 저장된다.
+        '''
+
+        if not isinstance(super_service_execute_request, MXSuperExecuteRequest):
+            raise MXTypeError(f'[{get_current_function_name()}] Wrong Request type: {type(super_service_execute_request)}')
 
-    def add_subfunction_reqline_info(self, subfunction_name: str, arg_list: Union[Tuple[SoPArgument], Tuple], tag_list: List[SoPTag], policy: SoPPolicy):
-        if not arg_list:
-            arg_list = []
-            sop_arg_list = []
+        super_execute_msg = super_service_execute_request.trigger_msg
+        requester_middleware_name = super_execute_msg.requester_middleware_name
+        scenario = super_execute_msg.scenario
+
+        MXLOG_DEBUG(
+            f'[SUPER_EXECUTE START] {self._name} by scenario {scenario}.', 'green')
+
+        try:
+            super_service_execute_request._running = True
+            self._running = True
+            error = MXErrorCode.NO_ERROR
+
+            # super service argument check
+            arguments = list(super_execute_msg.tuple_arguments())
+            for i, (arg, real_arg) in enumerate(zip(self._arg_list, arguments)):
+                if arg.get_type() in [MXType.INTEGER, MXType.DOUBLE] and MXType.get(type(real_arg)) in [MXType.INTEGER, MXType.DOUBLE]:
+                    arguments[i] = float(real_arg)
+                elif arg.get_type() != MXType.get(type(real_arg)):
+                    raise Exception(f'Argument type is not matched: {arg.get_name()}: {arg.get_type()} != {MXType.get(real_arg)}')
+
+            if self._timeout:
+                # self._return_value = func_timeout(self._timeout, self._func, args=(*tuple(arguments), ))
+                current_thread = threading.current_thread()
+                self._return_value = self._run_with_timeout(timeout=self._timeout, func=self._func, name=current_thread.name,
+                                                            user_data=dict(scenario=super_execute_msg.scenario, requester_middleware=requester_middleware_name), args=(*tuple(arguments), ))
+            else:
+                self._return_value = self._func(*tuple(arguments))
+        except KeyboardInterrupt as e:
+            print_error(e)
+            MXLOG_DEBUG('Function execution exit by user', 'red')
+            raise e
+        except FunctionTimedOut as e:
+            MXLOG_DEBUG(f'[SUPER_EXECUTE TIMEOUT] {super_service_execute_request._action_type.value} of {self._name} \
+                    by scenario {requester_middleware_name}|{scenario} timeout...', 'red')
+
+            # Timeout이 발생했다고 해서 mapping_table에서 삭제하지는 않는다.
+            # if super_service_execute_request._action_type == MXActionType.SUPER_EXECUTE:
+            #     self._mapping_table.pop(super_service_request_key)
+
+            error = MXErrorCode.TIMEOUT
+            self._return_value = None
+            return False
+        except Exception as e:
+            print_error(e)
+            MXLOG_DEBUG(f'[SUB_EXECUTE FAILED] {super_service_execute_request._action_type.value} of {self._name} \
+                by scenario {requester_middleware_name}|{scenario} failed...', 'red')
+
+            # Exception이 발생했다고 해서 mapping_table에서 삭제하지는 않는다.
+            # if super_service_execute_request._action_type == MXActionType.SUPER_EXECUTE:
+            #     self._mapping_table.pop(super_service_request_key)
+
+            error = MXErrorCode.FAIL
+            self._return_value = None
+            return False
         else:
-            sop_arg_list = list(arg_list)
-            for i, arg in enumerate(sop_arg_list):
-                if not isinstance(arg, SoPArgument):
-                    sop_arg_list[i] = SoPArgument(
-                        name=f'FIXED_ARG({arg})',
-                        type=SoPType.to_soptype(type(arg)))
-
-        subfunction_type = SoPFunction(name=subfunction_name,
-                                       arg_list=sop_arg_list,
-                                       tag_list=tag_list,
-                                       policy=policy)
-        self._add_subfunction_reqline(
-            SoPSubFunctionReqline(subfunction_type=subfunction_type, argument_list=arg_list))
-        SOPLOG_DEBUG(
-            f'Extract subfunction_reqline finish. super function: {self._name}, subfunction: {subfunction_name}, arg_list: [{", ".join([sop_arg._name for sop_arg in sop_arg_list])}] tag_list: [{", ".join([str(tag) for tag in tag_list])}]', 'green')
+            error = MXErrorCode.NO_ERROR
+            return True
+        finally:
+            self._send_SM_RESULT_EXECUTE(super_service_name=super_execute_msg.super_service_name,
+                                         super_thing_name=super_execute_msg.super_thing_name,
+                                         super_middleware_name=super_execute_msg.super_middleware_name,
+                                         requester_middleware_name=requester_middleware_name,
+                                         scenario=scenario,
+                                         error=error)
+
+            super_service_execute_request.timer_end()
+            super_service_execute_request._running = False
+            self._running = False
+            self._running_scenario_list.remove(super_execute_msg.scenario)
+            MXLOG_DEBUG(
+                f'[SUPER_EXECUTE END] {self._name} by scenario {scenario}. duration: {super_service_execute_request.duration():.4f} Sec', 'green')
+
+    def start_super_schedule_thread(self, super_schedule_msg: MXSuperScheduleMessage, hierarchical_service_table: Dict[str, List[MXService]], timeout: float = 1000) -> MXThread:
+        super_service_request_key = make_super_request_key(scenario_name=super_schedule_msg.scenario,
+                                                           requester_middleware_name=super_schedule_msg.requester_middleware_name)
+        if super_service_request_key in self._temporary_scheduling_table:
+            MXLOG_DEBUG(f'[{get_current_function_name()}] Super request with key: {super_service_request_key} is currently in the scheduling phase!', 'red')
+            return False
+
+        super_schedule_result_msg = MXSuperScheduleResultMessage(super_service_name=self._name,
+                                                                 super_thing_name=self._thing_name,
+                                                                 super_middleware_name=self._middleware_name,
+                                                                 requester_middleware_name=super_schedule_msg.requester_middleware_name,
+                                                                 scenario=super_schedule_msg.scenario)
+        super_schedule_request = MXSuperScheduleRequest(trigger_msg=super_schedule_msg,
+                                                        result_msg=super_schedule_result_msg)
+        super_service_request_key = make_super_request_key(scenario_name=super_schedule_msg.scenario,
+                                                           requester_middleware_name=super_schedule_msg.requester_middleware_name)
+        self._temporary_scheduling_table[super_service_request_key] = super_schedule_request
+        super_schedule_request.timer_start()
+
+        super_schedule_thread = MXThread(
+            target=self._super_schedule_wrapper,
+            name=f'{self._func.__name__}_{super_schedule_request._action_type.value}_thread',
+            daemon=True,
+            args=(super_schedule_request, hierarchical_service_table, timeout, ))
+        super_schedule_thread.start()
+
+        return super_schedule_thread
+
+    def start_super_execute_thread(self, super_execute_msg: MXSuperExecuteMessage, SUPER_SERVICE_REQUEST_KEY_TABLE: Dict[str, List[str]]) -> MXThread:
+        super_service_request_key = make_super_request_key(scenario_name=super_execute_msg.scenario,
+                                                           requester_middleware_name=super_execute_msg.requester_middleware_name)
+        if super_service_request_key in self._temporary_scheduling_table:
+            MXLOG_DEBUG(f'[{get_current_function_name()}] Super request with key: {super_service_request_key} is currently in the scheduling phase!', 'red')
+            return False
+
+        super_service_execute_request = self._mapping_table[super_service_request_key]
+        if super_service_execute_request._running:
+            MXLOG_DEBUG(f'[{get_current_function_name()}] Super Execute of Super request key: {super_service_request_key} is already executed!', 'red')
+            return False
+
+        super_service_execute_request.trigger_msg = super_execute_msg
+        super_service_execute_request.result_msg = MXSuperExecuteResultMessage(super_service_name=self._name,
+                                                                               super_thing_name=self._thing_name,
+                                                                               super_middleware_name=self._middleware_name,
+                                                                               requester_middleware_name=super_execute_msg.requester_middleware_name,
+                                                                               scenario=super_execute_msg.scenario,
+                                                                               return_type=self._return_type)
+        self._running_scenario_list.append(super_execute_msg.scenario)
+        super_service_execute_request.timer_start()
+
+        thread_name = f'{self._func.__name__}_{super_execute_msg.scenario}_thread'
+        super_execute_thread = MXThread(
+            target=self._super_execute_wrapper,
+            name=thread_name,
+            daemon=True,
+            args=(super_service_execute_request, ))
+        super_execute_thread.start()
+
+        sub_service_request_key_list = list(super_service_execute_request._sub_service_request_table)
+        SUPER_SERVICE_REQUEST_KEY_TABLE[super_service_request_key] = sub_service_request_key_list
+
+        return super_execute_thread
+
+    # FIXME: hardcoding 된 부분 수정하기 (DUMMY_ARG_)
+    def add_sub_service_request_info(self, sub_service_name: str, arg_list: Union[Tuple[MXArgument], Tuple], tag_list: List[MXTag], return_type: MXType, range_type: MXRangeType):
+        mx_arg_list = [arg if isinstance(arg, MXArgument) else MXArgument(name=f'DUMMY_ARG_{i}',
+                                                                          bound=(-sys.maxsize - 1, sys.maxsize),
+                                                                          type=MXType.get(type(arg))) for i, arg in enumerate(arg_list)]
+        sub_service_request_order = len(self._sub_service_request_list)
+        sub_service_type = MXFunction(name=sub_service_name,
+                                      func=dummy_func(arg_list=mx_arg_list),
+                                      return_type=return_type,
+                                      arg_list=mx_arg_list,
+                                      tag_list=tag_list,
+                                      range_type=range_type)
+        sub_service_request = MXSubServiceRequest(sub_service_type=sub_service_type,
+                                                  sub_service_request_order=sub_service_request_order)
+        self._add_sub_service_request(sub_service_request)
+
+        MXLOG_DEBUG(f'sub_service: {sub_service_name}:{sub_service_request_order}', 'green')
         return True
 
-    def put_subaction_result(self, super_request_key: str, subrequest_key: str, subaction_result_msg: Union[SoPSubScheduleResultMessage, SoPSubExecuteResultMessage]) -> None:
-        '''
-            super thing에 의해 호출되어 super thing이 받은 subaction결과를 super function에게 전달한다.
-        '''
+    def put_subschedule_result(self, super_service_request_key: str, sub_service_request_key: str, subschedule_result_msg: MXSubScheduleResultMessage) -> bool:
+        if super_service_request_key not in self._temporary_scheduling_table:
+            MXLOG_DEBUG(f'Could not find key {super_service_request_key} in temporary_scheduling_table... This key is not mine!', 'yellow')
+            return False
+
+        super_schedule_request = self._temporary_scheduling_table[super_service_request_key]
+        result = super_schedule_request.put_sub_service_schedule_result_msg(sub_service_request_key, subschedule_result_msg)
+        return result
+
+    def put_sub_service_execute_result(self, super_service_request_key: str, sub_service_request_key: str, sub_service_execute_result_msg: MXSubExecuteResultMessage) -> bool:
+        if super_service_request_key not in self._mapping_table:
+            MXLOG_DEBUG(f'Could not find key {super_service_request_key} in mapping_table... This key is not mine!', 'yellow')
+            return False
 
-        if isinstance(subaction_result_msg, SoPSubScheduleResultMessage):
-            action_table = self._temporary_scheduling_table
-        elif isinstance(subaction_result_msg, SoPSubExecuteResultMessage):
-            action_table = self._mapping_table
-
-        if super_request_key not in action_table:
-            SOPLOG_DEBUG(
-                f'Could not find key {super_request_key} in subexecute_request_list...', 'red')
-            raise Exception
-
-        super_action_request = action_table[super_request_key]
-        super_action_request.put_subresult_msg(
-            subrequest_key, subaction_result_msg)
-
-    def send_SM_SCHEDULE(self, subschedule_msg: SoPSubScheduleMessage) -> None:
-        self._publish_queue.put(subschedule_msg.mqtt_message())
-
-    def send_SM_RESULT_SCHEDULE(self, super_function_name: str, super_thing_name: str, super_middleware_name: str, requester_middleware_name: str,
-                                scenario: str, error: SoPErrorType) -> None:
-        self._publish_queue.put(SoPSuperScheduleResultMessage(
-            super_function_name, super_thing_name, super_middleware_name, requester_middleware_name, scenario=scenario, error=error).mqtt_message())
-
-    def send_SM_EXECUTE(self, subexecute_msg: SoPSubExecuteMessage) -> None:
-        self._publish_queue.put(subexecute_msg.mqtt_message())
-
-    def send_SM_RESULT_EXECUTE(self, super_function_name: str, super_thing_name: str, super_middleware_name: str, requester_middleware_name: str,
-                               scenario: str, return_type: SoPType, return_value: Union[int, float, bool, str], error: SoPErrorType) -> None:
-        self._publish_queue.put(SoPSuperExecuteResultMessage(
-            super_function_name, super_thing_name, super_middleware_name, requester_middleware_name,
-            scenario=scenario, return_type=return_type, return_value=return_value, error=error).mqtt_message())
+        super_service_execute_request = self._mapping_table[super_service_request_key]
+        result = super_service_execute_request.put_sub_service_execute_result_msg(sub_service_request_key, sub_service_execute_result_msg)
+        return result
+
+    def _send_SM_SCHEDULE(self, subschedule_msg: MXSubScheduleMessage) -> None:
+        subschedule_mqtt_msg = subschedule_msg.mqtt_message()
+        self._publish_queue.put(subschedule_mqtt_msg)
+
+    def _send_SM_EXECUTE(self, sub_service_execute_msg: MXSubExecuteMessage) -> None:
+        sub_service_execute_mqtt_msg = sub_service_execute_msg.mqtt_message()
+        self._publish_queue.put(sub_service_execute_mqtt_msg)
+
+    def _send_SM_RESULT_SCHEDULE(self, super_service_name: str, super_thing_name: str, super_middleware_name: str, requester_middleware_name: str,
+                                 scenario: str, error: MXErrorCode) -> None:
+        super_schedule_result_msg = self._generate_super_schedule_result_message(super_service_name=super_service_name,
+                                                                                 super_thing_name=super_thing_name,
+                                                                                 super_middleware_name=super_middleware_name,
+                                                                                 requester_middleware_name=requester_middleware_name,
+                                                                                 scenario=scenario,
+                                                                                 error=error)
+        super_schedule_result_mqtt_msg = super_schedule_result_msg.mqtt_message()
+        self._publish_queue.put(super_schedule_result_mqtt_msg)
+
+    def _send_SM_RESULT_EXECUTE(self, super_service_name: str, super_thing_name: str, super_middleware_name: str, requester_middleware_name: str,
+                                scenario: str, error: MXErrorCode):
+        super_execute_result_msg = self._generate_super_execute_result_message(super_service_name=super_service_name,
+                                                                               super_thing_name=super_thing_name,
+                                                                               super_middleware_name=super_middleware_name,
+                                                                               requester_middleware_name=requester_middleware_name,
+                                                                               scenario=scenario,
+                                                                               error=error)
+        super_execute_result_mqtt_msg = super_execute_result_msg.mqtt_message()
+        self._publish_queue.put(super_execute_result_mqtt_msg)
+
+    # ========================
+    #         _    _  _
+    #        | |  (_)| |
+    #  _   _ | |_  _ | | ___
+    # | | | || __|| || |/ __|
+    # | |_| || |_ | || |\__ \
+    #  \__,_| \__||_||_||___/
+    # ========================
+
+    def _generate_super_schedule_result_message(self, super_service_name: str, super_thing_name: str, super_middleware_name: str, requester_middleware_name: str,
+                                                scenario: str, error: MXErrorCode) -> MXSuperScheduleResultMessage:
+        super_schedule_result_msg = MXSuperScheduleResultMessage(super_service_name=super_service_name,
+                                                                 super_thing_name=super_thing_name,
+                                                                 super_middleware_name=super_middleware_name,
+                                                                 requester_middleware_name=requester_middleware_name,
+                                                                 scenario=scenario,
+                                                                 error=error)
+        return super_schedule_result_msg
+
+    def _generate_super_execute_result_message(self, super_service_name: str, super_thing_name: str, super_middleware_name: str, requester_middleware_name: str,
+                                               scenario: str, error: MXErrorCode) -> MXSuperExecuteResultMessage:
+        super_execute_result_msg = MXSuperExecuteResultMessage(super_service_name=super_service_name,
+                                                               super_thing_name=super_thing_name,
+                                                               super_middleware_name=super_middleware_name,
+                                                               requester_middleware_name=requester_middleware_name,
+                                                               scenario=scenario,
+                                                               return_type=self._return_type,
+                                                               return_value=self._return_value,
+                                                               error=error)
+        return super_execute_result_msg
 
     # ====================================
     #               _    _
     #              | |  | |
     #   __ _   ___ | |_ | |_   ___  _ __
     #  / _` | / _ \| __|| __| / _ \| '__|
     # | (_| ||  __/| |_ | |_ |  __/| |
     #  \__, | \___| \__| \__| \___||_|
     #   __/ |
     #  |___/
     # ====================================
 
-    def get_subfunction_type_list(self) -> List[SoPSubFunctionReqline]:
-        return self._subfunction_reqline_list
+    def get_sub_service_type_list(self) -> List[MXSubServiceRequest]:
+        return self._sub_service_request_list
 
-    def get_first_execute(self) -> bool:
-        return self._first_execute
+    def get_is_scanned(self) -> bool:
+        return self._is_scanned
 
     # ==================================
     #             _    _
     #            | |  | |
     #  ___   ___ | |_ | |_   ___  _ __
     # / __| / _ \| __|| __| / _ \| '__|
     # \__ \|  __/| |_ | |_ |  __/| |
     # |___/ \___| \__| \__| \___||_|
     # ==================================
 
-    def set_subfunction_type_list(self, target_subfunction_reqline_list: List[SoPSubFunctionReqline]) -> None:
-        self._subfunction_reqline_list = target_subfunction_reqline_list
-
-    def set_first_execute(self, first_execute: bool) -> None:
-        self._first_execute = first_execute
-
-    # for super service
-    def set_subscribe_queue(self, queue: Queue):
-        self._subscribe_queue = queue
+    def set_sub_service_type_list(self, target_sub_service_request_list: List[MXSubServiceRequest]) -> None:
+        self._sub_service_request_list = target_sub_service_request_list
 
-    def set_unsubscribe_queue(self, queue: Queue):
-        self._unsubscribe_queue = queue
+    def set_is_scanned(self, is_scanned: bool) -> None:
+        self._is_scanned = is_scanned
```

## big_thing_py/super/super_request.py

```diff
@@ -1,322 +1,311 @@
-from big_thing_py.common.request import *
-from big_thing_py.common.mqtt_message import *
-from big_thing_py.super.super_service_utils import *
+from big_thing_py.core.request import *
+from big_thing_py.super.super_mqtt_message import *
+from big_thing_py.core.function import *
 
 
-class SoPSuperScheduleRequest(SoPRequest):
-    def __init__(self, trigger_msg: SoPSuperScheduleMessage = None,
-                 result_msg: SoPSuperScheduleResultMessage = None) -> None:
+class MXSuperScheduleRequest(MXRequest):
+    def __init__(self, trigger_msg: MXSuperScheduleMessage = None,
+                 result_msg: MXSuperScheduleResultMessage = None) -> None:
         super().__init__(trigger_msg, result_msg)
-        self._action_type = SoPActionType.SUPER_SCHEDULE
+        self._action_type = MXActionType.SUPER_SCHEDULE
 
-        self._trigger_msg: SoPSuperScheduleMessage
-        self._result_msg: SoPSuperScheduleResultMessage
-        self._check_duation: float = 0.0
-        self._confirm_duation: float = 0.0
-        self._status: SoPScheduleStatus = SoPScheduleStatus.INIT
-        self._subfunction_reqline_table: Dict[str, SoPSubFunctionReqline] = {}
+        self.trigger_msg: MXSuperScheduleMessage
+        self.result_msg: MXSuperScheduleResultMessage
+        self._check_duration: float = 0.0
+        self._confirm_duration: float = 0.0
+        self._status: MXScheduleStatus = MXScheduleStatus.INIT
+        self._running: bool = False
+
+        # sub_request_key = make_sub_request_key(subschedule_result_msg.sub_service_name, subschedule_result_msg.sub_service_request_order)
+        # sub_request_key: {sub_service_name}@{sub_service_request_order}
+        self._sub_service_request_table: Dict[str, MXSubServiceRequest] = {}
 
-    def set_result_msg(self, result_msg: SoPSuperScheduleResultMessage):
-        self._result_msg = result_msg
+    def set_result_msg(self, result_msg: MXSuperScheduleResultMessage):
+        self.result_msg = result_msg
 
     def get_result_msg(self):
-        return self._result_msg
+        return self.result_msg
 
     def is_completed(self):
-        if self._result_msg:
+        if self.result_msg:
             return True
         else:
             return False
 
-    def check_duarion(self):
-        return self._check_duation
+    def check_duration(self):
+        return self._check_duration
 
-    def confirm_duarion(self):
-        return self._confirm_duation
+    def confirm_duration(self):
+        return self._confirm_duration
 
-    def put_subresult_msg(self, subrequest_key: str, result_msg: SoPSubScheduleResultMessage, timeout: float = None):
-        target_subfunction_reqline = self._subfunction_reqline_table[subrequest_key]
-        if target_subfunction_reqline == None:
-            raise Exception(
-                f'No subfunction {subrequest_key} found in _subfunction_reqline_table')
-
-        found_request = None
-        for candidate_request in target_subfunction_reqline._candidate_request_list:
-            thing_check = (
-                candidate_request._trigger_msg._target_thing_name == result_msg._target_thing_name)
-            middleware_check = (
-                candidate_request._trigger_msg._target_middleware_name == result_msg._target_middleware_name)
-            request_ID_check = (
-                candidate_request._trigger_msg._request_ID == result_msg._request_ID)
-            if thing_check and middleware_check and request_ID_check:
-                found_request = candidate_request
-                break
+    def put_sub_service_schedule_result_msg(self, sub_service_request_key: str, result_msg: MXSubScheduleResultMessage, timeout: float = None) -> bool:
+        if sub_service_request_key not in self._sub_service_request_table:
+            MXLOG_DEBUG(f'Could not find key {sub_service_request_key} in sub_service_request_table... This key is not mine!', 'yellow')
+            return False
 
-        if found_request:
-            found_request.put_result_msg(result_msg, timeout=timeout)
+        target_sub_service_request = self._sub_service_request_table[sub_service_request_key]
+        for candidate_request in target_sub_service_request._candidate_request_list:
+            thing_check = (candidate_request.trigger_msg.target_thing_name == result_msg.target_thing_name)
+            middleware_check = (candidate_request.trigger_msg.target_middleware_name == result_msg.target_middleware_name)
+            request_ID_check = (candidate_request.trigger_msg.request_ID == result_msg.request_ID)
+            status_check = (result_msg.status == MXScheduleStatus.CONFIRM and candidate_request._status == MXScheduleStatus.SELECT) or (result_msg.status == MXScheduleStatus.CHECK)
+
+            if thing_check and middleware_check and request_ID_check and status_check:
+                candidate_request.put_result_msg(result_msg, timeout=timeout)
+                return True
         else:
-            raise Exception(
-                f'No subfunction {subrequest_key} found in _subfunction_reqline_table')
-
-        return
+            raise Exception(f'No sub_service {sub_service_request_key} found in _sub_service_request_table')
 
-    def generate_subschedule_request(self, subfunction_reqline_list: List['SoPSubFunctionReqline'], hierarchical_function_service_table: List[SoPFunction]):
-        for subfunction_reqline in subfunction_reqline_list:
-            target_subfunction_reqline = SoPSubFunctionReqline(subfunction_type=subfunction_reqline._subfunction_type,
-                                                               subrequest_order=subfunction_reqline._subrequest_order,
-                                                               argument_list=subfunction_reqline._argument_list)
+    def generate_sub_service_schedule_request(self, sub_service_request_list: List['MXSubServiceRequest'], hierarchical_function_service_table: List[MXFunction]):
+        for sub_service_request in sub_service_request_list:
+            target_sub_service_request = MXSubServiceRequest(sub_service_type=sub_service_request._sub_service_type,
+                                                             sub_service_request_order=sub_service_request._sub_service_request_order)
             # TODO: 해당 로직 부분 분리하기
-            # 미들웨어 마다 reqline가 실행하고자 하는 subfunction이 존재하는 지 체크한다.
-            target_subfunction = target_subfunction_reqline._subfunction_type
+            # 미들웨어 마다 sub_service_request가 실행하고자 하는 sub_service이 존재하는 지 체크한다.
+            target_sub_service = target_sub_service_request._sub_service_type
 
             candidate_middleware_name_list = []
             for function_service in hierarchical_function_service_table:
-                name_check = (target_subfunction.get_name()
+                name_check = (target_sub_service.get_name()
                               == function_service.get_name())
                 if name_check and function_service.get_middleware_name() not in candidate_middleware_name_list:
                     candidate_middleware_name_list.append(
                         function_service.get_middleware_name())
-                    target_subfunction.set_middleware_name(
+                    target_sub_service.set_middleware_name(
                         function_service.get_middleware_name())
 
             candidate_request_list = []
             for middleware_name in candidate_middleware_name_list:
-                subschedule_msg = SoPSubScheduleMessage(target_subfunction.get_name(),
-                                                        'SUPER',
-                                                        middleware_name,
-                                                        self._trigger_msg._requester_middleware_name,
-                                                        self._trigger_msg._super_thing_name,
-                                                        self._trigger_msg._super_function_name,
-                                                        target_subfunction_reqline._subrequest_order,
-                                                        self._trigger_msg._scenario,
-                                                        self._trigger_msg._period,
-                                                        request_ID=None,
-                                                        tag_list=[
-                                                            dict(name=tag.get_name()) for tag in function_service.get_tag_list()],
-                                                        policy=target_subfunction.get_policy())
-
-                # NOTE:reqline에 대한 부분이 미들웨어당 1개만 생성될 것으로 예상됨. len(candidate_request_list) == 1 ?
-                subschedule_request = SoPSubScheduleRequest(trigger_msg=subschedule_msg,
-                                                            subfunction=target_subfunction)
-                candidate_request_list.append(subschedule_request)
-
-            target_subfunction_reqline._candidate_request_list = candidate_request_list
-            subreqeust_key = make_sub_request_key(
-                target_subfunction.get_name(), target_subfunction_reqline._subrequest_order)
-            self._subfunction_reqline_table[subreqeust_key] = target_subfunction_reqline
+                sub_service_schedule_msg = MXSubScheduleMessage(sub_service_name=target_sub_service.get_name(),
+                                                                target_thing_name='SUPER',
+                                                                target_middleware_name=middleware_name,
+                                                                requester_middleware_name=self.trigger_msg.requester_middleware_name,
+                                                                super_thing_name=self.trigger_msg.super_thing_name,
+                                                                super_service_name=self.trigger_msg.super_service_name,
+                                                                sub_service_request_order=target_sub_service_request._sub_service_request_order,
+                                                                scenario=self.trigger_msg.scenario,
+                                                                period=self.trigger_msg.period,
+                                                                tag_list=[dict(name=tag.get_name()) for tag in target_sub_service.get_tag_list()],
+                                                                range_type=target_sub_service.get_range_type(),
+                                                                request_ID=None,
+                                                                status=MXScheduleStatus.INIT)
+
+                # NOTE:sub_service_request에 대한 부분이 미들웨어당 1개만 생성될 것으로 예상됨. len(candidate_request_list) == 1 ?
+                # TODO: _result_msg도 생성해서 넣어서 나중에 결과 토픽을 구독할 때 topic()으로 간단하게 사용할 수 있게 하면 좋을 것 같다.
+                sub_service_schedule_request = MXSubScheduleRequest(trigger_msg=sub_service_schedule_msg)
+                candidate_request_list.append(sub_service_schedule_request)
+
+            target_sub_service_request._candidate_request_list = candidate_request_list
+            sub_service_request_key = make_sub_service_request_key(sub_service_name=target_sub_service.get_name(),
+                                                                   sub_service_request_order=target_sub_service_request._sub_service_request_order)
+            self._sub_service_request_table[sub_service_request_key] = target_sub_service_request
 
-            if len(target_subfunction_reqline._candidate_request_list) == 0:
+            if len(target_sub_service_request._candidate_request_list) == 0:
                 for function_service in hierarchical_function_service_table:
-                    SOPLOG_DEBUG(
-                        f'subfunction found! - {function_service.get_name()}|{function_service.get_thing_name()}|{function_service.get_middleware_name()}')
+                    MXLOG_DEBUG(
+                        f'sub_service found! - {function_service.get_name()}|{function_service.get_thing_name()}|{function_service.get_middleware_name()}')
                 raise Exception(
-                    f'No candidate subfunction found in key:{subreqeust_key} {self._trigger_msg._super_function_name} super function')
+                    f'No candidate sub_service found in key:{sub_service_request_key} {self.trigger_msg.super_service_name} super service')
 
 
-class SoPSuperExecuteRequest(SoPRequest):
-    def __init__(self, trigger_msg: SoPSuperExecuteMessage = None) -> None:
+class MXSuperExecuteRequest(MXRequest):
+    def __init__(self, trigger_msg: MXSuperExecuteMessage = None, super_schedule_request: MXSuperScheduleRequest = None) -> None:
         super().__init__(trigger_msg, None)
-        self._action_type = SoPActionType.SUPER_EXECUTE
+        self._action_type = MXActionType.SUPER_EXECUTE
 
-        self._trigger_msg: SoPSuperExecuteMessage
-        self._result_msg: SoPSuperExecuteResultMessage
-        self._super_arg_list: List[SoPArgument] = None
-        self._subfunction_reqline_table: Dict[str, SoPSubFunctionReqline] = {}
-        self._current_reqline_num: int = 0
+        self.trigger_msg: MXSuperExecuteMessage
+        self.result_msg: MXSuperExecuteResultMessage
+        self._running: bool = False
+
+        # scheduling이 끝나면 해당 scenario에 대해 어떤 sub_service_type에 대해 thing을 선택할 것인지 정해진다.
+        # sub_request_key = make_sub_request_key(subschedule_result_msg.sub_service_name, subschedule_result_msg.sub_service_request_order)
+        # sub_request_key: {sub_service_name}@{sub_service_request_order}
+        self._sub_service_request_table: Dict[str, MXSubServiceRequest] = {}
 
-    def set_result_msg(self, result_msg: SoPSuperExecuteResultMessage):
-        self._result_msg = result_msg
+        if super_schedule_request:
+            self.generate_sub_service_execute_request_list(super_schedule_request=super_schedule_request)
 
-    def get_result_msg(self):
-        return self._result_msg
+    def set_result_msg(self, result_msg: MXSuperExecuteResultMessage):
+        self.result_msg = result_msg
 
-    def get_arg_list(self):
-        return self._super_arg_list
+    def get_result_msg(self):
+        return self.result_msg
 
     def is_completed(self):
-        if self._result_msg:
+        if self.result_msg:
             return True
         else:
             return False
 
-    def put_subresult_msg(self, subrequest_key: str, result_msg: SoPSubExecuteResultMessage, timeout: float = None):
-        target_subfunction_reqline = self._subfunction_reqline_table[subrequest_key]
-        if target_subfunction_reqline == None:
-            raise Exception(
-                f'No subfunction {subrequest_key} found in _subfunction_reqline_table')
-
-        found_request = None
-        for target_request in target_subfunction_reqline._target_request_list:
-            thing_check = (
-                target_request._trigger_msg._target_thing_name == result_msg._target_thing_name)
-            middleware_check = (
-                target_request._trigger_msg._target_middleware_name == result_msg._target_middleware_name)
-            request_ID_check = (
-                target_request._trigger_msg._request_ID == result_msg._request_ID)
-            if thing_check and middleware_check and request_ID_check:
-                found_request = target_request
-                break
+    def put_sub_service_execute_result_msg(self, sub_service_request_key: str, result_msg: MXSubExecuteResultMessage, timeout: float = None) -> bool:
+        if sub_service_request_key not in self._sub_service_request_table:
+            MXLOG_DEBUG(f'Could not find key {sub_service_request_key} in sub_service_request_table... This key is not mine!', 'yellow')
+            return False
 
-        if found_request:
-            found_request.put_result_msg(result_msg, timeout=timeout)
+        target_sub_service_request = self._sub_service_request_table[sub_service_request_key]
+        for target_request in target_sub_service_request._target_request_list:
+            target_thing_check = (target_request.trigger_msg.target_thing_name == result_msg.target_thing_name)
+            target_middleware_check = (target_request.trigger_msg.target_middleware_name == result_msg.target_middleware_name)
+            request_ID_check = (target_request.trigger_msg.request_ID == result_msg.request_ID)
+            if target_thing_check and target_middleware_check and request_ID_check:
+                target_request.put_result_msg(result_msg, timeout=timeout)
+                return True
         else:
-            raise Exception(
-                f'No subfunction {subrequest_key} found in _subfunction_reqline_table')
-
-        return
+            raise Exception(f'No sub_service {sub_service_request_key} found in _sub_service_request_table')
 
-    def get_subexecute_result_msg_list(self, subrequest_key: str, timeout: float = None) -> List[SoPSubExecuteResultMessage]:
+    def get_sub_service_execute_result_msg_list(self, sub_service_request_key: str, timeout: float = None) -> List[MXSubExecuteResultMessage]:
         result_msg_list = []
-        target_subfunction_reqline = self._subfunction_reqline_table[subrequest_key]
-        for target_request in target_subfunction_reqline._target_request_list:
-            result_msg_list.append(
-                target_request.get_result_msg(timeout=timeout))
+        target_sub_service_request = self._sub_service_request_table[sub_service_request_key]
+        for target_request in target_sub_service_request._target_request_list:
+            result_msg_list.append(target_request.get_result_msg(timeout=timeout))
         return result_msg_list
 
-    def make_real_subfunction_arguments(self, super_arg_list: List[SoPArgument], reqline_arg_list: Union[Tuple[SoPArgument], Tuple]):
-        real_argument_list = []
+    def generate_sub_service_execute_request_list(self, super_schedule_request: 'MXSuperScheduleRequest' = None) -> 'MXSuperExecuteRequest':
+        # schedule 단계에서 MXSuperExecuteRequest를 생성한다.
+        for sub_service_request_key, sub_service_request in super_schedule_request._sub_service_request_table.items():
+            self._sub_service_request_table[sub_service_request_key] = MXSubServiceRequest(sub_service_type=sub_service_request._sub_service_type,
+                                                                                           sub_service_request_order=sub_service_request._sub_service_request_order,
+                                                                                           candidate_request_list=sub_service_request._candidate_request_list)
+            target_request_list = []
+            for candidate_request in sub_service_request._candidate_request_list:
+                if candidate_request._status == MXScheduleStatus.CONFIRM:
+                    target_request_list.append(
+                        to_sub_service_execute_request(candidate_request))
+            self._sub_service_request_table[sub_service_request_key]._target_request_list = target_request_list
+        return self
+
+
+class MXSubScheduleRequest(MXRequest):
+    def __init__(self, trigger_msg: MXSubScheduleMessage = None,
+                 result_mqtt_msg: MXSubScheduleResultMessage = None) -> None:
+        super().__init__(trigger_msg, result_mqtt_msg)
+        self._action_type = MXActionType.SUB_SCHEDULE
 
-        for i, reqline_arg in enumerate(reqline_arg_list):
-            if isinstance(reqline_arg_list[i], SoPArgument):
-                if reqline_arg in super_arg_list:
-                    real_argument_list.append(dict(order=i,
-                                                   value=self._trigger_msg._arguments[i]['value']))
-            else:
-                real_argument_list.append(dict(order=i, value=reqline_arg))
-        return real_argument_list
+        self.trigger_msg: MXSubScheduleMessage
+        self.result_msg: MXSubScheduleResultMessage
+        self._status: MXScheduleStatus = MXScheduleStatus.INIT
+        self._result_queue = Queue()
 
-    # def put_real_arguments(self, real_arguments: List[dict], subexecute_request: 'SoPSubExecuteRequest'):
-    #     subexecute_request._trigger_msg._arguments = real_arguments
-    #     for subexecute_request in self._subexecute_request_list:
-    #         subexecute_msg = subexecute_request._trigger_msg
-    #         subfunction_check = (
-    #             subexecute_msg._subfunction_name == subexecute_request._subfunction.get_name())
-    #         target_middleware_check = (
-    #             subexecute_msg._target_middleware_name == subexecute_request._subfunction.get_middleware_name())
-    #         target_thing_check = (
-    #             subexecute_msg._target_thing_name == subexecute_request._subfunction.get_thing_name())
-    #         if subfunction_check and target_middleware_check and target_thing_check:
-    #             subexecute_msg._arguments = real_arguments
+    def __getstate__(self):
+        state = self.__dict__.copy()
 
-    def generate_subexecute_request_list(self, super_schedule_request: 'SoPSuperScheduleRequest' = None):
-        # schedule 단계에서 SoPSuperExecuteRequest를 생성한다.
-        if super_schedule_request:
-            for subrequest_key, subfunction_reqline in super_schedule_request._subfunction_reqline_table.items():
-                self._subfunction_reqline_table[subrequest_key] = SoPSubFunctionReqline(subfunction_type=subfunction_reqline._subfunction_type,
-                                                                                        subrequest_order=subfunction_reqline._subrequest_order,
-                                                                                        candidate_request_list=subfunction_reqline._candidate_request_list,
-                                                                                        argument_list=subfunction_reqline._argument_list)
-                target_request_list = []
-                for candidate_request in subfunction_reqline._candidate_request_list:
-                    if candidate_request._status == SoPScheduleStatus.CONFIRM:
-                        target_request_list.append(
-                            to_subexecute_request(candidate_request))
-                self._subfunction_reqline_table[subrequest_key]._target_request_list = target_request_list
-
-    def exchange_argument(self):
-        # execute 단계에서 실제 execute를 하기 위해 argument를 추출한다.
-        for subrequest_key, subfunction_reqline in self._subfunction_reqline_table.items():
-            for target_request in subfunction_reqline._target_request_list:
-                # middleware_check = (target_request._trigger_msg._target_middleware_name ==
-                #                     target_request._subfunction.get_middleware_name())
-                # if middleware_check:
-                real_subfunction_argument_list = self.make_real_subfunction_arguments(
-                    self._super_arg_list, subfunction_reqline._argument_list)
-                target_request._trigger_msg._arguments = real_subfunction_argument_list
-
-
-class SoPSubScheduleRequest(SoPRequest):
-    def __init__(self, trigger_msg: SoPSubScheduleMessage = None,
-                 result_mqtt_msg: SoPSubScheduleResultMessage = None, subfunction: SoPFunction = None) -> None:
-        super().__init__(trigger_msg, result_mqtt_msg)
-        self._action_type = SoPActionType.SUB_SCHEDULE
+        del state['_result_queue']
+
+        return state
+
+    def __setstate__(self, state):
+        self.__dict__.update(state)
 
-        self._trigger_msg: SoPSubScheduleMessage
-        self._result_msg: SoPSubScheduleResultMessage
-        self._subfunction = subfunction
-        self._status: SoPScheduleStatus = SoPScheduleStatus.INIT
         self._result_queue = Queue()
 
-    def put_result_msg(self, result_msg: SoPSubScheduleResultMessage, timeout: float = None):
+    def put_result_msg(self, result_msg: MXSubScheduleResultMessage, timeout: float = None):
         self._result_queue.put(result_msg, timeout=timeout)
 
     def get_result_msg(self, timeout: float = None):
         try:
             return self._result_queue.get(timeout=timeout)
         except Empty:
             raise FunctionTimedOut
 
 
-class SoPSubExecuteRequest(SoPRequest):
-    def __init__(self, trigger_msg: SoPSubExecuteMessage = None,
-                 result_mqtt_msg: SoPSubExecuteResultMessage = None, subfunction: SoPFunction = None) -> None:
+class MXSubExecuteRequest(MXRequest):
+    def __init__(self, trigger_msg: MXSubExecuteMessage = None,
+                 result_mqtt_msg: MXSubExecuteResultMessage = None) -> None:
         super().__init__(trigger_msg, result_mqtt_msg)
-        self._action_type = SoPActionType.SUB_EXECUTE
+        self._action_type = MXActionType.SUB_EXECUTE
+
+        self.trigger_msg: MXSubExecuteMessage
+        self.result_msg: MXSubExecuteResultMessage
+        self._result_queue = Queue()
+
+    def __getstate__(self):
+        state = self.__dict__.copy()
+
+        del state['_result_queue']
+
+        return state
+
+    def __setstate__(self, state):
+        self.__dict__.update(state)
 
-        self._trigger_msg: SoPSubExecuteMessage
-        self._result_msg: SoPSubExecuteResultMessage
-        self._subfunction = subfunction
         self._result_queue = Queue()
 
-    def put_result_msg(self, result_msg: SoPSubExecuteResultMessage, timeout: float = None):
+    def put_result_msg(self, result_msg: MXSubExecuteResultMessage, timeout: float = None):
         self._result_queue.put(result_msg, timeout=timeout)
 
-    def get_result_msg(self, timeout: float = None) -> SoPSubExecuteResultMessage:
+    def get_result_msg(self, timeout: float = None) -> MXSubExecuteResultMessage:
         try:
             return self._result_queue.get(timeout=timeout)
         except Empty:
             raise FunctionTimedOut
 
 
-class SoPSubFunctionReqline():
-    def __init__(self, subfunction_type: SoPFunction, subrequest_order: int = None, candidate_request_list: List[SoPSubScheduleRequest] = [],
-                 target_request_list: List[SoPSubExecuteRequest] = [], argument_list: Union[Tuple[SoPArgument], Tuple] = []) -> None:
-        self._subfunction_type = subfunction_type
-        self._subrequest_order = subrequest_order
+class MXSubServiceRequest():
+    def __init__(self, sub_service_type: MXFunction, candidate_request_list: List[MXSubScheduleRequest] = [], target_request_list: List[MXSubExecuteRequest] = [],
+                 sub_service_request_order: int = None) -> None:
+        self._sub_service_type = sub_service_type
         self._candidate_request_list = candidate_request_list
         self._target_request_list = target_request_list
-        self._argument_list = argument_list
+        self._sub_service_request_order = sub_service_request_order
+
+    def __eq__(self, o: 'MXSubServiceRequest') -> bool:
+        instance_check = isinstance(o, MXSubServiceRequest)
+        # sub_service_type_check = (o._sub_service_type == self._sub_service_type)
+
+        def sub_service_type_check():
+            return_type_check = (o._sub_service_type._return_type == self._sub_service_type._return_type)
+            exec_time_check = (o._sub_service_type._exec_time == self._sub_service_type._exec_time)
+            timeout_check = (o._sub_service_type._timeout == self._sub_service_type._timeout)
+            range_type_check = (o._sub_service_type._range_type == self._sub_service_type._range_type)
+
+            if return_type_check and exec_time_check and timeout_check and range_type_check:
+                return True
+            else:
+                return False
+
+        candidate_request_list_check = (o._candidate_request_list == self._candidate_request_list)
+        target_request_list_check = (o._target_request_list == self._target_request_list)
+        sub_service_request_order_check = (o._sub_service_request_order == self._sub_service_request_order)
+
+        return instance_check and sub_service_type_check and candidate_request_list_check and target_request_list_check and sub_service_request_order_check
 
     def __deepcopy__(self, memodict={}):
-        new_instance = SoPSubFunctionReqline(
-            self._subfunction_type, self._subrequest_order, list(), list())
+        new_instance = MXSubServiceRequest(self._sub_service_type, self._sub_service_request_order, list())
         new_instance.__dict__.update(self.__dict__)
-        new_instance._subfunction_type = copy.deepcopy(
-            self._subfunction_type, memodict)
-        new_instance._subrequest_order = copy.deepcopy(
-            self._subrequest_order, memodict)
+        new_instance._sub_service_type = copy.deepcopy(
+            self._sub_service_type, memodict)
+        new_instance._sub_service_request_order = copy.deepcopy(
+            self._sub_service_request_order, memodict)
         new_instance._candidate_request_list = list()
         new_instance._target_request_list = list()
         return new_instance
 
 
-def to_subexecute_request(subschedule_request: SoPSubScheduleRequest) -> SoPSubExecuteRequest:
-    subschedule_msg: SoPSubScheduleMessage = subschedule_request._trigger_msg
-    subexecute_msg = SoPSubExecuteMessage(subschedule_msg._subfunction_name,
-                                          'SUPER',
-                                          subschedule_msg._target_middleware_name,
-                                          subschedule_msg._requester_middleware_name,
-                                          subschedule_msg._super_thing_name,
-                                          subschedule_msg._super_function_name,
-                                          subschedule_msg._subrequest_order,
-                                          subschedule_msg._scenario,
-                                          request_ID=subschedule_msg._request_ID)
-    subexecute_request = SoPSubExecuteRequest(
-        trigger_msg=subexecute_msg, subfunction=subschedule_request._subfunction)
-    return subexecute_request
-
-
-def to_subschedule_request(subexecute_request: SoPSubExecuteRequest) -> SoPSubScheduleRequest:
-    subexecute_msg: SoPSubExecuteMessage = subexecute_request._trigger_msg
-    subschedule_msg = SoPSubScheduleMessage(subexecute_msg._subfunction_name,
-                                            subexecute_msg._target_thing_name,
-                                            subexecute_msg._target_middleware_name,
-                                            subexecute_msg._requester_middleware_name,
-                                            subexecute_msg._super_thing_name,
-                                            subexecute_msg._super_function_name,
-                                            subexecute_msg._subrequest_order,
-                                            subexecute_msg._scenario,
-                                            request_ID=subexecute_msg._request_ID)
-    subschedule_request = SoPSubScheduleRequest(
-        trigger_msg=subschedule_msg, subfunction=subexecute_request._subfunction)
-    return subschedule_request
+def to_sub_service_execute_request(sub_service_schedule_request: MXSubScheduleRequest) -> MXSubExecuteRequest:
+    sub_service_schedule_msg: MXSubScheduleMessage = sub_service_schedule_request.trigger_msg
+    sub_service_execute_msg = MXSubExecuteMessage(sub_service_schedule_msg.sub_service_name,
+                                                  'SUPER',
+                                                  sub_service_schedule_msg.target_middleware_name,
+                                                  sub_service_schedule_msg.requester_middleware_name,
+                                                  sub_service_schedule_msg.super_thing_name,
+                                                  sub_service_schedule_msg.super_service_name,
+                                                  sub_service_schedule_msg.sub_service_request_order,
+                                                  sub_service_schedule_msg.scenario,
+                                                  request_ID=sub_service_schedule_msg.request_ID)
+    sub_service_execute_request = MXSubExecuteRequest(trigger_msg=sub_service_execute_msg)
+    return sub_service_execute_request
+
+
+def to_sub_service_schedule_request(sub_service_execute_request: MXSubExecuteRequest) -> MXSubScheduleRequest:
+    sub_service_execute_msg: MXSubExecuteMessage = sub_service_execute_request.trigger_msg
+    sub_service_schedule_msg = MXSubScheduleMessage(sub_service_name=sub_service_execute_msg.sub_service_name,
+                                                    target_thing_name=sub_service_execute_msg.target_thing_name,
+                                                    target_middleware_name=sub_service_execute_msg.target_middleware_name,
+                                                    requester_middleware_name=sub_service_execute_msg.requester_middleware_name,
+                                                    super_thing_name=sub_service_execute_msg.super_thing_name,
+                                                    super_service_name=sub_service_execute_msg.super_service_name,
+                                                    sub_service_request_order=sub_service_execute_msg.sub_service_request_order,
+                                                    scenario=sub_service_execute_msg.scenario,
+                                                    request_ID=sub_service_execute_msg.request_ID)
+    sub_service_schedule_request = MXSubScheduleRequest(trigger_msg=sub_service_schedule_msg)
+    return sub_service_schedule_request
```

## big_thing_py/tests/conftest.py

```diff
@@ -1,2 +1,837 @@
-import os
+from big_thing_py.big_thing import *
+from big_thing_py.tests.thing_factory import *
+
 import pytest
+import subprocess
+
+PARAMETRIZE_STRING_OLD = 'test_id, input, expected_output, expected_exception_message'
+PARAMETRIZE_STRING = 'test_id, input, expected_output'
+START_LOGGER()
+
+# ----------------------------------------------------------------------------------------------------------------------
+
+
+def fail_function() -> int:
+    raise Exception('fail function')
+
+
+@static_vars(int_value=0)
+def int_function_no_arg_timeout_3() -> int:
+    int_function_no_arg_timeout_3.int_value += 1
+
+    time.sleep(5)
+
+    MXLOG_DEBUG(
+        f'{get_current_function_name()} run. return {int_function_no_arg_timeout_3.int_value}', 'green')
+    return int_function_no_arg_timeout_3.int_value
+
+
+@static_vars(int_value=0)
+def int_function_no_arg_with_delay_1() -> int:
+    int_function_no_arg_with_delay_1.int_value += 1
+
+    time.sleep(1)
+
+    MXLOG_DEBUG(
+        f'{get_current_function_name()} run. return {int_function_no_arg_with_delay_1.int_value}', 'green')
+    return int_function_no_arg_with_delay_1.int_value
+
+
+@static_vars(int_value=0)
+def int_function_no_arg() -> int:
+    int_function_no_arg.int_value += 1
+    MXLOG_DEBUG(
+        f'{get_current_function_name()} run. return {int_function_no_arg.int_value}', 'green')
+    return int_function_no_arg.int_value
+
+
+@static_vars(float_value=0.0)
+def float_function_no_arg() -> float:
+    float_function_no_arg.float_value += 1.0
+    MXLOG_DEBUG(
+        f'{get_current_function_name()} run. return {float_function_no_arg.float_value}', 'green')
+    return float_function_no_arg.float_value
+
+
+@static_vars(str_value=str(0))
+def str_function_no_arg() -> str:
+    str_function_no_arg.str_value = str(
+        int(str_function_no_arg.str_value) + 1)
+    MXLOG_DEBUG(
+        f'{get_current_function_name()} run. return {str_function_no_arg.str_value}', 'green')
+    return str_function_no_arg.str_value
+
+
+@static_vars(bool_value=True)
+def bool_function_no_arg() -> bool:
+    bool_function_no_arg.bool_value = bool_function_no_arg.int_value % 2 == 0
+    MXLOG_DEBUG(
+        f'{get_current_function_name()} run. return {bool_function_no_arg.bool_value}', 'green')
+    return bool_function_no_arg.bool_value
+
+
+# def binary_function_no_arg() -> str:
+#     ReturnValue()
+#     return_value = ReturnValue()
+#     ReturnValue.binary_value = string_to_base64(
+#         str(int(ReturnValue.binary_value) + 1))
+#     MXLOG_DEBUG(
+#         f'{get_current_function_name()} run. return {ReturnValue.binary_value}', 'green')
+#     return ReturnValue.binary_value
+
+
+def void_function_no_arg() -> None:
+    MXLOG_DEBUG(f'{get_current_function_name()} run. no return', 'green')
+
+# ----------------------------------------------------------------------------------------------------------------------
+
+
+def int_value_return_5() -> int:
+    MXLOG_DEBUG(
+        f'{get_current_function_name()} run. return {5}', 'green')
+    return 5
+
+
+@static_vars(int_value=0)
+def int_value_no_arg() -> int:
+    int_value_no_arg.int_value += 1
+    MXLOG_DEBUG(
+        f'{get_current_function_name()} run. return {int_value_no_arg.int_value}', 'green')
+    return int_value_no_arg.int_value
+
+
+@static_vars(float_value=0.0)
+def float_value_no_arg() -> float:
+    float_value_no_arg.float_value += 1.0
+    MXLOG_DEBUG(
+        f'{get_current_function_name()} run. return {float_value_no_arg.float_value}', 'green')
+    return float_value_no_arg.float_value
+
+
+@static_vars(str_value=str(0))
+def str_value_no_arg() -> str:
+    str_value_no_arg.str_value = str(
+        int(str_value_no_arg.str_value) + 1)
+    MXLOG_DEBUG(
+        f'{get_current_function_name()} run. return {str_value_no_arg.str_value}', 'green')
+    return str_value_no_arg.str_value
+
+
+@static_vars(bool_value=True)
+def bool_value_no_arg() -> bool:
+    bool_value_no_arg.bool_value = bool_value_no_arg.int_value % 2 == 0
+    MXLOG_DEBUG(
+        f'{get_current_function_name()} run. return {bool_value_no_arg.bool_value}', 'green')
+    return bool_value_no_arg.bool_value
+
+
+# def binary_function_no_arg() -> str:
+#     ReturnValue()
+#     return_value = ReturnValue()
+#     ReturnValue.binary_value = string_to_base64(
+#         str(int(ReturnValue.binary_value) + 1))
+#     MXLOG_DEBUG(
+#         f'{get_current_function_name()} run. return {ReturnValue.binary_value}', 'green')
+#     return ReturnValue.binary_value
+
+
+def void_value_no_arg() -> None:
+    MXLOG_DEBUG(f'{get_current_function_name()} run. no return', 'green')
+
+# ----------------------------------------------------------------------------------------------------------------------
+
+
+def int_function_with_arg(int_arg: int) -> int:
+    MXLOG_DEBUG(
+        f'{get_current_function_name()} run. argument : {int_arg}, return {int_arg}', 'green')
+    return int_arg
+
+
+def float_function_with_arg(float_arg: int) -> float:
+    MXLOG_DEBUG(
+        f'{get_current_function_name()} run. argument : {float_arg}, return {float_arg}', 'green')
+    return float_arg
+
+
+def str_function_with_arg(str_arg: int) -> str:
+    MXLOG_DEBUG(
+        f'{get_current_function_name()} run. argument : {str_arg}, return {str_arg}', 'green')
+    return str_arg
+
+
+def bool_function_with_arg(bool_arg: int) -> bool:
+    MXLOG_DEBUG(
+        f'{get_current_function_name()} run. argument : {bool_arg}, return {bool_arg}', 'green')
+    return bool_arg
+
+
+# def binary_function_with_arg(binary_arg: int) -> str:
+#     MXLOG_DEBUG(
+#         f'{get_current_function_name()} run. argument : {binary_arg}, return {binary_arg}', 'green')
+#     return binary_arg
+
+
+def void_function_with_arg(int_arg: int, float_arg: float, str_arg: str, bool_arg: bool) -> None:
+    MXLOG_DEBUG(
+        f'{get_current_function_name()} run. argument : {int_arg}, {float_arg}, {str_arg}, {bool_arg} no return.', 'green')
+
+# def void_function_with_arg(int_arg: int, float_arg: float, str_arg: str, bool_arg: bool, binary_arg: str) -> None:
+#     MXLOG_DEBUG(
+#         f'{get_current_function_name()} run. argument : {int_arg}, {float_arg}, {str_arg}, {bool_arg}, {binary_arg} no return.', 'green')
+
+# ----------------------------------------------------------------------------------------------------------------------
+
+
+def generate_full_feature_thing(name: str, ip: str, port: int, alive_cycle: float) -> MXBigThing:
+    alive_cycle = 1
+    value_cycle = alive_cycle
+
+    tag_list = [MXTag('full')]
+
+    int_arg_list = [MXArgument(name='int_arg',
+                               type=MXType.INTEGER,
+                               bound=(-2147483648, 2147483647)), ]
+    float_arg_list = [MXArgument(name='float_arg',
+                                 type=MXType.DOUBLE,
+                                 bound=(-2147483648, 2147483647)), ]
+    str_arg_list = [MXArgument(name='str_arg',
+                               type=MXType.STRING,
+                               bound=(-2147483648, 2147483647)), ]
+    bool_arg_list = [MXArgument(name='bool_arg',
+                                type=MXType.BOOL,
+                                bound=(-2147483648, 2147483647)), ]
+    binary_arg_list = [MXArgument(name='binary_arg',
+                                  type=MXType.BINARY,
+                                  bound=(-2147483648, 2147483647))]
+    full_arg_list = [MXArgument(name='int_arg',
+                                type=MXType.INTEGER,
+                                bound=(-2147483648, 2147483647)),
+                     MXArgument(name='float_arg',
+                                type=MXType.DOUBLE,
+                                bound=(-2147483648, 2147483647)),
+                     MXArgument(name='str_arg',
+                                type=MXType.STRING,
+                                bound=(-2147483648, 2147483647)),
+                     MXArgument(name='bool_arg',
+                                type=MXType.BOOL,
+                                bound=(-2147483648, 2147483647)),
+                     # MXArgument(name='binary_arg',
+                     #             type=MXType.BINARY,
+                     #             bound=(-2147483648, 2147483647))
+                     ]
+
+    value_list = [
+        MXValue(name='int_value_return_5',
+                func=int_value_return_5,
+                type=MXType.INTEGER,
+                bound=(-2147483648, 2147483647),
+                tag_list=tag_list + [MXTag('INTEGER')],
+                cycle=value_cycle),
+        MXValue(name='int_value',
+                func=int_value_no_arg,
+                type=MXType.INTEGER,
+                bound=(-2147483648, 2147483647),
+                tag_list=tag_list + [MXTag('INTEGER')],
+                cycle=value_cycle),
+        MXValue(name='float_value',
+                func=float_value_no_arg,
+                type=MXType.DOUBLE,
+                bound=(-2147483648, 2147483647),
+                tag_list=tag_list + [MXTag('DOUBLE')],
+                cycle=value_cycle),
+        MXValue(name='str_value',
+                func=str_value_no_arg,
+                type=MXType.STRING,
+                bound=(-2147483648, 2147483647),
+                tag_list=tag_list + [MXTag('STRING')],
+                cycle=value_cycle),
+        MXValue(name='bool_value',
+                func=bool_value_no_arg,
+                type=MXType.BOOL,
+                bound=(-2147483648, 2147483647),
+                tag_list=tag_list + [MXTag('BOOL')],
+                cycle=value_cycle),
+        # MXValue(name='binary_value',
+        #          func=binary_function_no_arg,
+        #          type=MXType.BINARY,
+        #          bound=(-2147483648, 2147483647),
+        #          tag_list=default_tag_list + value_tag_list + [MXTag('BINARY')],
+        #          cycle=value_cycle)
+    ]
+
+    no_arg_function_list = [
+        MXFunction(name='fail_function',
+                   func=fail_function,
+                   return_type=MXType.INTEGER,
+                   desc='fail_function',
+                   tag_list=tag_list + [MXTag('INTEGER')],
+                   arg_list=[],
+                   exec_time=1,
+                   timeout=1,
+                   range_type=MXRangeType.SINGLE,
+                   energy=10),
+        MXFunction(name='int_function_no_arg_timeout_3',
+                   func=int_function_no_arg_timeout_3,
+                   return_type=MXType.INTEGER,
+                   desc='int_function_no_arg_timeout_3',
+                   tag_list=tag_list + [MXTag('INTEGER')],
+                   arg_list=[],
+                   exec_time=1,
+                   timeout=3,
+                   range_type=MXRangeType.SINGLE,
+                   energy=10),
+        MXFunction(name='int_function_no_arg_with_delay_1',
+                   func=int_function_no_arg_with_delay_1,
+                   return_type=MXType.INTEGER,
+                   desc='int_function_no_arg_with_delay_1',
+                   tag_list=tag_list + [MXTag('INTEGER')],
+                   arg_list=[],
+                   exec_time=1,
+                   timeout=1,
+                   range_type=MXRangeType.SINGLE,
+                   energy=10),
+        MXFunction(name='int_function_no_arg',
+                   func=int_function_no_arg,
+                   return_type=MXType.INTEGER,
+                   desc='int_function_no_arg',
+                   tag_list=tag_list + [MXTag('INTEGER')],
+                   arg_list=[],
+                   exec_time=1,
+                   timeout=1,
+                   range_type=MXRangeType.SINGLE,
+                   energy=10),
+        MXFunction(name='float_function_no_arg',
+                   func=float_function_no_arg,
+                   return_type=MXType.DOUBLE,
+                   desc='float_function_no_arg',
+                   tag_list=tag_list + [MXTag('DOUBLE')],
+                   arg_list=[],
+                   exec_time=1,
+                   timeout=1,
+                   range_type=MXRangeType.SINGLE,
+                   energy=10),
+        MXFunction(name='str_function_no_arg',
+                   func=str_function_no_arg,
+                   return_type=MXType.STRING,
+                   desc='str_function_no_arg',
+                   tag_list=tag_list + [MXTag('STRING')],
+                   arg_list=[],
+                   exec_time=1,
+                   timeout=1,
+                   range_type=MXRangeType.SINGLE,
+                   energy=10),
+        MXFunction(name='bool_function_no_arg',
+                   func=bool_function_no_arg,
+                   return_type=MXType.BOOL,
+                   desc='bool_function_no_arg',
+                   tag_list=tag_list + [MXTag('BOOL')],
+                   arg_list=[],
+                   exec_time=1,
+                   timeout=1,
+                   range_type=MXRangeType.SINGLE,
+                   energy=10),
+        # MXFunction(name='binary_function_no_arg',
+        #             func=binary_function_no_arg,
+        #             return_type=MXType.BINARY,
+        #             desc='binary_function_no_arg',
+        #             tag_list=default_tag_list +
+        #             [MXTag('BINARY')],
+        #             arg_list=[],
+        #             exec_time=1,
+        #             timeout=1,
+        #             range_type=MXRangeType.SINGLE),
+        MXFunction(name='void_function_no_arg',
+                   func=void_function_no_arg,
+                   return_type=MXType.VOID,
+                   desc='void_function_no_arg',
+                   tag_list=tag_list + [MXTag('VOID')],
+                   arg_list=[],
+                   exec_time=1,
+                   timeout=1,
+                   range_type=MXRangeType.SINGLE,
+                   energy=10)
+    ]
+    arg_function_list = [
+        MXFunction(name='int_function_with_arg',
+                   func=int_function_with_arg,
+                   return_type=MXType.INTEGER,
+                   desc='int_function_with_arg',
+                   tag_list=tag_list + [MXTag('INTEGER')],
+                   arg_list=int_arg_list,
+                   exec_time=1,
+                   timeout=1,
+                   range_type=MXRangeType.SINGLE,
+                   energy=20),
+        MXFunction(name='float_function_with_arg',
+                   func=float_function_with_arg,
+                   return_type=MXType.DOUBLE,
+                   desc='float_function_with_arg',
+                   tag_list=tag_list + [MXTag('DOUBLE')],
+                   arg_list=float_arg_list,
+                   exec_time=1,
+                   timeout=1,
+                   range_type=MXRangeType.SINGLE,
+                   energy=20),
+        MXFunction(name='str_function_with_arg',
+                   func=str_function_with_arg,
+                   return_type=MXType.STRING,
+                   desc='str_function_with_arg',
+                   tag_list=tag_list + [MXTag('STRING')],
+                   arg_list=str_arg_list,
+                   exec_time=1,
+                   timeout=1,
+                   range_type=MXRangeType.SINGLE,
+                   energy=20),
+        MXFunction(name='bool_function_with_arg',
+                   func=bool_function_with_arg,
+                   return_type=MXType.BOOL,
+                   desc='bool_function_with_arg',
+                   tag_list=tag_list + [MXTag('BOOL')],
+                   arg_list=bool_arg_list,
+                   exec_time=1,
+                   timeout=1,
+                   range_type=MXRangeType.SINGLE,
+                   energy=20),
+        # MXFunction(name='binary_function_with_arg',
+        #             func=binary_function_with_arg,
+        #             return_type=MXType.BINARY,
+        #             desc='binary_function_with_arg',
+        #             tag_list=default_tag_list +
+        #             [MXTag('BINARY')],
+        #             arg_list=arg_list,
+        #             exec_time=1,
+        #             timeout=1,
+        #             range_type=MXRangeType.SINGLE),
+        MXFunction(name='void_function_with_arg',
+                   func=void_function_with_arg,
+                   return_type=MXType.VOID,
+                   desc='void_function_with_arg',
+                   tag_list=tag_list + [MXTag('VOID')],
+                   arg_list=full_arg_list,
+                   exec_time=1,
+                   timeout=1,
+                   range_type=MXRangeType.SINGLE,
+                   energy=20)
+    ]
+    thing = MXBigThing(name=name, ip=ip, port=port, alive_cycle=alive_cycle,
+                       service_list=value_list + no_arg_function_list + arg_function_list, append_mac_address=False)
+    return thing
+
+####################################################################################################################################
+
+
+class MXBasicSuperThing(MXSuperThing):
+
+    def __init__(self, name: str = MXSuperThing.DEFAULT_NAME, service_list: List[MXService] = [], alive_cycle: float = 60, is_super: bool = True, is_parallel: bool = True,
+                 ip: str = '127.0.0.1', port: int = 1883, ssl_ca_path: str = '', ssl_enable: bool = False,
+                 log_name: str = None, log_enable: bool = True, log_mode: MXPrintMode = MXPrintMode.ABBR,
+                 append_mac_address: bool = True,
+                 refresh_cycle: float = 30):
+
+        tag_list = [MXTag(name='super'),
+                    MXTag(name='basic'),
+                    MXTag(name='big_thing'),
+                    MXTag(name='function')]
+        int_arg = MXArgument(name='int_arg',
+                             type=MXType.INTEGER,
+                             bound=(0, 1000000))
+        delay_arg = MXArgument(name='delay_arg',
+                               type=MXType.DOUBLE,
+                               bound=(0.0, 1000000.0))
+
+        value_list = []
+        function_list = [MXSuperFunction(func=self.super_func_execute_func_no_arg_SINGLE,
+                                         return_type=MXType.INTEGER,
+                                         tag_list=tag_list,
+                                         arg_list=[],
+                                         timeout=1,
+                                         energy=100),
+                         MXSuperFunction(func=self.super_func_execute_func_no_arg_ALL,
+                                         return_type=MXType.INTEGER,
+                                         tag_list=tag_list,
+                                         arg_list=[],
+                                         timeout=1,
+                                         energy=100),
+                         MXSuperFunction(func=self.super_func_execute_func_with_arg_SINGLE,
+                                         return_type=MXType.INTEGER,
+                                         tag_list=tag_list,
+                                         arg_list=[int_arg],
+                                         timeout=1,
+                                         energy=100),
+                         MXSuperFunction(func=self.super_func_execute_func_with_arg_ALL,
+                                         return_type=MXType.INTEGER,
+                                         tag_list=tag_list,
+                                         arg_list=[int_arg],
+                                         timeout=1,
+                                         energy=100),
+                         MXSuperFunction(func=self.super_func_execute_func_with_arg_and_delay_SINGLE,
+                                         return_type=MXType.INTEGER,
+                                         tag_list=tag_list,
+                                         arg_list=[int_arg, delay_arg],
+                                         timeout=1,
+                                         energy=100),
+                         MXSuperFunction(func=self.super_func_execute_func_with_arg_and_delay_ALL,
+                                         return_type=MXType.INTEGER,
+                                         tag_list=tag_list,
+                                         arg_list=[int_arg, delay_arg],
+                                         timeout=1,
+                                         energy=100),
+                         MXSuperFunction(func=self.super_func_get_value_current_time_SINGLE,
+                                         return_type=MXType.INTEGER,
+                                         tag_list=tag_list,
+                                         arg_list=[],
+                                         timeout=1,
+                                         energy=100),
+                         MXSuperFunction(func=self.super_func_get_value_current_time_ALL,
+                                         return_type=MXType.INTEGER,
+                                         tag_list=tag_list,
+                                         arg_list=[],
+                                         timeout=1,
+                                         energy=100),
+                         MXSuperFunction(func=self.super_multiple_sub_service_request1,
+                                         return_type=MXType.INTEGER,
+                                         tag_list=tag_list,
+                                         arg_list=[int_arg, delay_arg],
+                                         timeout=1,
+                                         energy=100),
+                         MXSuperFunction(func=self.super_multiple_sub_service_request2,
+                                         return_type=MXType.INTEGER,
+                                         tag_list=tag_list,
+                                         arg_list=[int_arg, delay_arg],
+                                         timeout=1,
+                                         energy=100),
+                         MXSuperFunction(func=self.super_multiple_sub_service_request_with_fixed_argument1,
+                                         return_type=MXType.INTEGER,
+                                         tag_list=tag_list,
+                                         arg_list=[int_arg, delay_arg],
+                                         timeout=1,
+                                         energy=100),
+                         MXSuperFunction(func=self.super_multiple_sub_service_request_with_fixed_argument2,
+                                         return_type=MXType.INTEGER,
+                                         tag_list=tag_list,
+                                         arg_list=[int_arg, delay_arg],
+                                         timeout=1,
+                                         energy=100),
+                         MXSuperFunction(func=self.super_multiple_sub_service_request_with_argument_pass,
+                                         return_type=MXType.INTEGER,
+                                         tag_list=tag_list,
+                                         arg_list=[int_arg, delay_arg],
+                                         timeout=1,
+                                         energy=100), ]
+
+        service_list = value_list + function_list
+        super().__init__(name=name, service_list=service_list, alive_cycle=alive_cycle, is_super=is_super, is_parallel=is_parallel,
+                         ip=ip, port=port, ssl_ca_path=ssl_ca_path, ssl_enable=ssl_enable,
+                         log_name=log_name, log_enable=log_enable, log_mode=log_mode,
+                         append_mac_address=append_mac_address,
+                         refresh_cycle=refresh_cycle)
+
+    def load_super_service_params(self, super_service_params_list: List[str]):
+        for super_service_params in super_service_params_list:
+            super_service = eval(f'MXSuperFunction({super_service_params})')
+            self.add_service(super_service)
+
+    def super_func_execute_func_no_arg_SINGLE(self) -> int:
+        result_list = self.req(sub_service_name='func_no_arg', tag_list=['basic'], return_type=MXType.INTEGER,
+                               service_type=MXServiceType.FUNCTION, range_type=MXRangeType.SINGLE)
+
+        result_sum = 0
+        if result_list:
+            for result in result_list:
+                result_sum += result['return_value']
+
+            return result_sum
+        else:
+            return 0
+
+    def super_func_execute_func_no_arg_ALL(self) -> int:
+        result_list = self.req(sub_service_name='func_no_arg', tag_list=['basic'], return_type=MXType.INTEGER,
+                               service_type=MXServiceType.FUNCTION, range_type=MXRangeType.ALL)
+
+        result_sum = 0
+        if result_list:
+            for result in result_list:
+                result_sum += result['return_value']
+
+            return result_sum
+        else:
+            return 0
+
+    def super_func_execute_func_with_arg_SINGLE(self, int_arg: int) -> int:
+        result_list = self.req(sub_service_name='func_with_arg', tag_list=['basic'], arg_list=(int_arg, ),  return_type=MXType.INTEGER,
+                               service_type=MXServiceType.FUNCTION, range_type=MXRangeType.SINGLE)
+
+        result_sum = 0
+        if result_list:
+            for result in result_list:
+                result_sum += result['return_value']
+
+            return result_sum
+        else:
+            return 0
+
+    def super_func_execute_func_with_arg_ALL(self, int_arg: int) -> int:
+        result_list = self.req(sub_service_name='func_with_arg', tag_list=['basic'], arg_list=(int_arg, ), return_type=MXType.INTEGER,
+                               service_type=MXServiceType.FUNCTION, range_type=MXRangeType.ALL)
+
+        result_sum = 0
+        if result_list:
+            for result in result_list:
+                result_sum += result['return_value']
+
+            return result_sum
+        else:
+            return 0
+
+    def super_func_execute_func_with_arg_and_delay_SINGLE(self, int_arg: int, delay: float) -> int:
+        result_list = self.req(sub_service_name='func_with_arg_and_delay', tag_list=['basic'], arg_list=(int_arg, delay, ), return_type=MXType.INTEGER,
+                               service_type=MXServiceType.FUNCTION, range_type=MXRangeType.SINGLE)
+
+        result_sum = 0
+        if result_list:
+            for result in result_list:
+                result_sum += result['return_value']
+
+            return result_sum
+        else:
+            return 0
+
+    def super_func_execute_func_with_arg_and_delay_ALL(self, int_arg: int, delay: float) -> int:
+        result_list = self.req(sub_service_name='func_with_arg_and_delay', tag_list=['basic'], arg_list=(int_arg, delay, ), return_type=MXType.INTEGER,
+                               service_type=MXServiceType.FUNCTION, range_type=MXRangeType.ALL)
+
+        result_sum = 0
+        if result_list:
+            for result in result_list:
+                result_sum += result['return_value']
+
+            return result_sum
+        else:
+            return 0
+
+    def super_func_get_value_current_time_SINGLE(self) -> int:
+        result_list = self.req(sub_service_name='value_current_time', tag_list=['basic'], return_type=MXType.INTEGER,
+                               service_type=MXServiceType.VALUE, range_type=MXRangeType.SINGLE)
+
+        result_sum = 0
+        if result_list:
+            for result in result_list:
+                result_sum += result['return_value']
+
+            return result_sum
+        else:
+            return 0
+
+    def super_func_get_value_current_time_ALL(self) -> int:
+        result_list = self.req(sub_service_name='value_current_time', tag_list=['basic'], return_type=MXType.INTEGER,
+                               service_type=MXServiceType.VALUE, range_type=MXRangeType.ALL)
+
+        result_sum = 0
+        if result_list:
+            for result in result_list:
+                result_sum += result['return_value']
+
+            return result_sum
+        else:
+            return 0
+
+    def super_multiple_sub_service_request1(self, int_arg: int, delay: float) -> int:
+        result_list1 = self.req(sub_service_name='func_with_arg_and_delay', tag_list=['basic'], arg_list=(int_arg, delay, ), return_type=MXType.INTEGER,
+                                service_type=MXServiceType.FUNCTION, range_type=MXRangeType.SINGLE)
+        result_list2 = self.req(sub_service_name='func_with_arg', tag_list=['basic'], arg_list=(int_arg, ), return_type=MXType.INTEGER,
+                                service_type=MXServiceType.FUNCTION, range_type=MXRangeType.ALL)
+        result_list3 = self.req(sub_service_name='func_no_arg', tag_list=['basic'], arg_list=(), return_type=MXType.INTEGER,
+                                service_type=MXServiceType.FUNCTION, range_type=MXRangeType.ALL)
+
+        result_sum = 0
+        if result_list1 and result_list2 and result_list3:
+            for result in result_list1:
+                result_sum += result['return_value']
+            for result in result_list2:
+                result_sum += result['return_value']
+            for result in result_list3:
+                result_sum += result['return_value']
+
+            return result_sum
+        else:
+            return 0
+
+    def super_multiple_sub_service_request2(self, int_arg: int, delay: float) -> int:
+        result_list1 = self.req(sub_service_name='func_with_arg_and_delay', tag_list=['basic'], arg_list=(int_arg, delay, ), return_type=MXType.INTEGER,
+                                service_type=MXServiceType.FUNCTION, range_type=MXRangeType.SINGLE)
+        result_list2 = self.req(sub_service_name='func_with_arg', tag_list=['basic'], arg_list=(int_arg, ), return_type=MXType.INTEGER,
+                                service_type=MXServiceType.FUNCTION, range_type=MXRangeType.ALL)
+        result_list3 = self.req(sub_service_name='func_no_arg', tag_list=['basic'], arg_list=(), return_type=MXType.INTEGER,
+                                service_type=MXServiceType.FUNCTION, range_type=MXRangeType.ALL)
+
+        result_sum = 0
+        if result_list1 and result_list2 and result_list3:
+            for result in result_list1:
+                result_sum += result['return_value']
+            for result in result_list2:
+                result_sum += result['return_value']
+            for result in result_list3:
+                result_sum += result['return_value']
+
+            return result_sum
+        else:
+            return 0
+
+    def super_multiple_sub_service_request_with_fixed_argument1(self, int_arg: int, delay: float) -> int:
+        result_list1 = self.req(sub_service_name='func_with_arg', tag_list=['basic'], arg_list=(int_arg, ), return_type=MXType.INTEGER,
+                                service_type=MXServiceType.FUNCTION, range_type=MXRangeType.SINGLE)
+        result_list2 = self.req(sub_service_name='func_with_arg_and_delay', tag_list=['basic'], arg_list=(142, delay, ), return_type=MXType.INTEGER,
+                                service_type=MXServiceType.FUNCTION, range_type=MXRangeType.SINGLE)
+        result_list3 = self.req(sub_service_name='func_no_arg', tag_list=['basic'], arg_list=(), return_type=MXType.INTEGER,
+                                service_type=MXServiceType.FUNCTION, range_type=MXRangeType.SINGLE)
+
+        result_sum = 0
+        if result_list1 and result_list2 and result_list3:
+            for result in result_list1:
+                result_sum += result['return_value']
+            for result in result_list2:
+                result_sum += result['return_value']
+            for result in result_list3:
+                result_sum += result['return_value']
+
+            return result_sum
+        else:
+            return 0
+
+    def super_multiple_sub_service_request_with_fixed_argument2(self, int_arg: int, delay: float) -> int:
+        result_list1 = self.req(sub_service_name='func_with_arg', tag_list=['basic'], arg_list=(int_arg, ), return_type=MXType.INTEGER,
+                                service_type=MXServiceType.FUNCTION, range_type=MXRangeType.SINGLE)
+        result_list2 = self.req(sub_service_name='func_with_arg_and_delay', tag_list=['basic'], arg_list=(142, delay, ), return_type=MXType.INTEGER,
+                                service_type=MXServiceType.FUNCTION, range_type=MXRangeType.ALL)
+        result_list3 = self.req(sub_service_name='func_no_arg', tag_list=['basic'], arg_list=(), return_type=MXType.INTEGER,
+                                service_type=MXServiceType.FUNCTION, range_type=MXRangeType.SINGLE)
+
+        result_sum = 0
+        if result_list1 and result_list2 and result_list3:
+            for result in result_list1:
+                result_sum += result['return_value']
+            for result in result_list2:
+                result_sum += result['return_value']
+            for result in result_list3:
+                result_sum += result['return_value']
+
+            return result_sum
+        else:
+            return 0
+
+    def super_multiple_sub_service_request_with_argument_pass(self, int_arg: int, delay: float) -> int:
+        result_list1 = self.req(sub_service_name='func_with_arg', tag_list=['basic'], arg_list=(int_arg, ), return_type=MXType.INTEGER,
+                                service_type=MXServiceType.FUNCTION, range_type=MXRangeType.SINGLE)
+        result1 = result_list1[0]['return_value'] if result_list1 else 0
+        result_list2 = self.req(sub_service_name='func_with_arg_and_delay', tag_list=['basic'], arg_list=(result1, delay, ), return_type=MXType.INTEGER,
+                                service_type=MXServiceType.FUNCTION, range_type=MXRangeType.ALL)
+        result_list3 = self.req(sub_service_name='func_with_arg', tag_list=['basic'], arg_list=(100, ), return_type=MXType.INTEGER,
+                                service_type=MXServiceType.FUNCTION, range_type=MXRangeType.SINGLE)
+
+        result_sum = 0
+        if result_list1 and result_list2 and result_list3:
+            for result in result_list1:
+                result_sum += result['return_value']
+            for result in result_list2:
+                result_sum += result['return_value']
+            for result in result_list3:
+                result_sum += result['return_value']
+
+            return result_sum
+        else:
+            return 0
+
+####################################################################################################################################
+
+
+@pytest.fixture
+def full_feature_big_thing() -> MXBigThing:
+    big_thing = generate_full_feature_thing(
+        name='test_thing', ip='localhost', port=1883, alive_cycle=60)
+    return big_thing
+
+
+@pytest.fixture
+def default_big_thing() -> MXBigThing:
+    big_thing = BigThingFactory().create_default_thing()
+    return big_thing
+
+
+@pytest.fixture
+def big_thing() -> MXBigThing:
+    big_thing = MXBigThing()
+    return big_thing
+
+
+@pytest.fixture
+def basic_super_thing() -> MXBasicSuperThing:
+    super_thing = MXBasicSuperThing()
+    return super_thing
+
+
+@pytest.fixture
+def super_thing() -> MXSuperThing:
+    super_thing = MXSuperThing()
+    return super_thing
+
+# TODO: remove. do not connect to broker in thing sdk test
+
+
+@pytest.fixture()
+def run_mosquitto():
+    mosquitto_process = subprocess.Popen(
+        ['mosquitto'], stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+    yield mosquitto_process
+    mosquitto_process.terminate()
+    mosquitto_process.wait()
+
+
+@pytest.fixture()
+def run_ssl_mosquitto():
+    os.chdir(f'{get_project_root()}/big_thing_py/tests')
+    mosquitto_process = subprocess.Popen(
+        ['mosquitto', '-c', f'{get_project_root()}/res/mosquitto.conf'], stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+    yield mosquitto_process
+    mosquitto_process.terminate()
+    mosquitto_process.wait()
+
+
+@pytest.fixture()
+def install_CA():
+    result = subprocess.Popen([f'cp {get_project_root()}/res/CA/ca.crt /tmp/mosquitto/ca_certificates;'], shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+    result = subprocess.Popen([f'cp {get_project_root()}/res/CA/host.crt /tmp/mosquitto/certs;',], shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+    result = subprocess.Popen([f'cp {get_project_root()}/res/CA/host.key /tmp/mosquitto/certs;',], shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+    result = subprocess.Popen([f'chmod -R 707 {get_project_root()}/res/CA/certs;',], shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+    result = subprocess.Popen([f'chmod -R 707 {get_project_root()}/res/CA/ca_certificates;'], shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+    return result
+
+
+def compare_mqtt_msg(output_msg: mqtt.MQTTMessage, expected_msg: mqtt.MQTTMessage):
+    # if not isinstance(output_msg,  mqtt.MQTTMessage) or not isinstance(expected_msg, mqtt.MQTTMessage):
+    #     return output_msg == expected_msg
+
+    topic_check = (decode_MQTT_message(output_msg)[0] == decode_MQTT_message(expected_msg)[0])
+    payload_check = (decode_MQTT_message(output_msg)[1] == decode_MQTT_message(expected_msg)[1])
+
+    return topic_check and payload_check
+
+
+def compare_mqtt_msg_list(output_msg_list: List[mqtt.MQTTMessage], expected_msg_list: List[mqtt.MQTTMessage], ignore_order=False):
+    if len(output_msg_list) != len(expected_msg_list):
+        return False
+
+    if ignore_order:
+        for msg1 in output_msg_list:
+            found = False
+            for msg2 in expected_msg_list:
+                if compare_mqtt_msg(msg1, msg2):
+                    found = True
+                    break
+            if not found:
+                return False
+        return True
+    else:
+        for i in range(len(output_msg_list)):
+            if not compare_mqtt_msg(output_msg_list[i], expected_msg_list[i]):
+                return False
+        return True
```

## big_thing_py/tests/manager/test_hejhome_manager_thing.py

```diff
@@ -6,53 +6,53 @@
     json_string_to_dict,
     get_current_time,
     type_converter,
     get_function_return_type,
     get_function_parameter,
     get_ip_from_url)
 
-from big_thing.SoPTag import SoPTag
-from big_thing.SoPArgument import SoPArgument
-from big_thing.SoPFunction import SoPFunction
-from big_thing.SoPValue import SoPValue
-from big_thing.SoPThing import SoPThing
-from sample_class.manager_client.HueManagerClient import SoPHueManagerClient
+from big_thing.MXTag import MXTag
+from big_thing.MXArgument import MXArgument
+from big_thing.MXFunction import MXFunction
+from big_thing.MXValue import MXValue
+from big_thing.MXThing import MXThing
+from sample_class.manager_client.HueManagerClient import MXHueManagerClient
 
 from typing import *
 from threading import Thread, Event, current_thread
 from functools import singledispatch
 from queue import Queue
 from time import sleep, time
 import json
 
 from termcolor import colored, cprint
 import paho.mqtt.client as mqtt
 import pytest
 
 
 def test_manager_client_init():
-    client = SoPHueManagerClient(ip='iotdev.snu.ac.kr', port=11883,
-                                 bridge_ip='http://147.46.114.24/api/', bridge_port=80,
-                                 user_key='L-idzo6XFfRVA-DzXyA66xKzi-KxIJA75neakYyS',
-                                 refresh_cycle=5,)
+    client = MXHueManagerClient(ip='iotdev.snu.ac.kr', port=11883,
+                                bridge_ip='http://147.46.114.24/api/', bridge_port=80,
+                                user_key='L-idzo6XFfRVA-DzXyA66xKzi-KxIJA75neakYyS',
+                                refresh_cycle=5,)
     assert client.setup()
     assert client.run(timeout=5)
     assert client.wrapup()
 
 
 cnt = 3
 
 
 def test_manager_client_run():
     global cnt
 
-    client = SoPHueManagerClient(ip='iotdev.snu.ac.kr', port=11883,
-                                 bridge_ip='http://147.46.114.24/api/', bridge_port=80,
-                                 user_key='L-idzo6XFfRVA-DzXyA66xKzi-KxIJA75neakYyS',
-                                 refresh_cycle=5,)
+    client = MXHueManagerClient(ip='iotdev.snu.ac.kr', port=11883,
+                                bridge_ip='http://147.46.114.24/api/', bridge_port=80,
+                                user_key='L-idzo6XFfRVA-DzXyA66xKzi-KxIJA75neakYyS',
+                                refresh_cycle=5,)
     assert client.setup()
 
     execute_event: Event = Event()
     execute_thread: Thread = Thread(
         target=client.run, daemon=True, kwargs={'stop_event': execute_event, 'timeout': 20, })
     execute_thread.start()
     base_run_time = 2
```

## big_thing_py/tests/manager/test_hue_manager_thing.py

```diff
@@ -6,53 +6,53 @@
     json_string_to_dict,
     get_current_time,
     type_converter,
     get_function_return_type,
     get_function_parameter,
     get_ip_from_url)
 
-from big_thing.SoPTag import SoPTag
-from big_thing.SoPArgument import SoPArgument
-from big_thing.SoPFunction import SoPFunction
-from big_thing.SoPValue import SoPValue
-from big_thing.SoPThing import SoPThing
-from sample_class.manager_client.HueManagerClient import SoPHueManagerClient
+from big_thing.MXTag import MXTag
+from big_thing.MXArgument import MXArgument
+from big_thing.MXFunction import MXFunction
+from big_thing.MXValue import MXValue
+from big_thing.MXThing import MXThing
+from sample_class.manager_client.HueManagerClient import MXHueManagerClient
 
 from typing import *
 from threading import Thread, Event, current_thread
 from functools import singledispatch
 from queue import Queue
 from time import sleep, time
 import json
 
 from termcolor import colored, cprint
 import paho.mqtt.client as mqtt
 import pytest
 
 
 def test_manager_client_init():
-    client = SoPHueManagerClient(ip='iotdev.snu.ac.kr', port=11883,
-                                 bridge_ip='http://147.46.114.24/api/', bridge_port=80,
-                                 user_key='L-idzo6XFfRVA-DzXyA66xKzi-KxIJA75neakYyS',
-                                 refresh_cycle=5,)
+    client = MXHueManagerClient(ip='iotdev.snu.ac.kr', port=11883,
+                                bridge_ip='http://147.46.114.24/api/', bridge_port=80,
+                                user_key='L-idzo6XFfRVA-DzXyA66xKzi-KxIJA75neakYyS',
+                                refresh_cycle=5,)
     assert client.setup()
     assert client.run(timeout=5)
     assert client.wrapup()
 
 
 cnt = 3
 
 
 def test_manager_client_run():
     global cnt
 
-    client = SoPHueManagerClient(ip='iotdev.snu.ac.kr', port=11883,
-                                 bridge_ip='http://147.46.114.24/api/', bridge_port=80,
-                                 user_key='L-idzo6XFfRVA-DzXyA66xKzi-KxIJA75neakYyS',
-                                 refresh_cycle=5,)
+    client = MXHueManagerClient(ip='iotdev.snu.ac.kr', port=11883,
+                                bridge_ip='http://147.46.114.24/api/', bridge_port=80,
+                                user_key='L-idzo6XFfRVA-DzXyA66xKzi-KxIJA75neakYyS',
+                                refresh_cycle=5,)
     assert client.setup()
 
     execute_event: Event = Event()
     execute_thread: Thread = Thread(
         target=client.run, daemon=True, kwargs={'stop_event': execute_event, 'timeout': 20, })
     execute_thread.start()
     base_run_time = 2
```

## big_thing_py/tests/manager/test_rf_manager_thing.py

```diff
@@ -6,53 +6,53 @@
     json_string_to_dict,
     get_current_time,
     type_converter,
     get_function_return_type,
     get_function_parameter,
     get_ip_from_url)
 
-from big_thing.SoPTag import SoPTag
-from big_thing.SoPArgument import SoPArgument
-from big_thing.SoPFunction import SoPFunction
-from big_thing.SoPValue import SoPValue
-from big_thing.SoPThing import SoPThing
-from sample_class.manager_client.HueManagerClient import SoPHueManagerClient
+from big_thing.MXTag import MXTag
+from big_thing.MXArgument import MXArgument
+from big_thing.MXFunction import MXFunction
+from big_thing.MXValue import MXValue
+from big_thing.MXThing import MXThing
+from sample_class.manager_client.HueManagerClient import MXHueManagerClient
 
 from typing import *
 from threading import Thread, Event, current_thread
 from functools import singledispatch
 from queue import Queue
 from time import sleep, time
 import json
 
 from termcolor import colored, cprint
 import paho.mqtt.client as mqtt
 import pytest
 
 
 def test_manager_client_init():
-    client = SoPHueManagerClient(ip='iotdev.snu.ac.kr', port=11883,
-                                 bridge_ip='http://147.46.114.24/api/', bridge_port=80,
-                                 user_key='L-idzo6XFfRVA-DzXyA66xKzi-KxIJA75neakYyS',
-                                 refresh_cycle=5,)
+    client = MXHueManagerClient(ip='iotdev.snu.ac.kr', port=11883,
+                                bridge_ip='http://147.46.114.24/api/', bridge_port=80,
+                                user_key='L-idzo6XFfRVA-DzXyA66xKzi-KxIJA75neakYyS',
+                                refresh_cycle=5,)
     assert client.setup()
     assert client.run(timeout=5)
     assert client.wrapup()
 
 
 cnt = 3
 
 
 def test_manager_client_run():
     global cnt
 
-    client = SoPHueManagerClient(ip='iotdev.snu.ac.kr', port=11883,
-                                 bridge_ip='http://147.46.114.24/api/', bridge_port=80,
-                                 user_key='L-idzo6XFfRVA-DzXyA66xKzi-KxIJA75neakYyS',
-                                 refresh_cycle=5,)
+    client = MXHueManagerClient(ip='iotdev.snu.ac.kr', port=11883,
+                                bridge_ip='http://147.46.114.24/api/', bridge_port=80,
+                                user_key='L-idzo6XFfRVA-DzXyA66xKzi-KxIJA75neakYyS',
+                                refresh_cycle=5,)
     assert client.setup()
 
     execute_event: Event = Event()
     execute_thread: Thread = Thread(
         target=client.run, daemon=True, kwargs={'stop_event': execute_event, 'timeout': 20, })
     execute_thread.start()
     base_run_time = 2
```

## big_thing_py/tests/manager/test_smartthings_manager_thing.py

```diff
@@ -6,53 +6,53 @@
     json_string_to_dict,
     get_current_time,
     type_converter,
     get_function_return_type,
     get_function_parameter,
     get_ip_from_url)
 
-from big_thing.SoPTag import SoPTag
-from big_thing.SoPArgument import SoPArgument
-from big_thing.SoPFunction import SoPFunction
-from big_thing.SoPValue import SoPValue
-from big_thing.SoPThing import SoPThing
-from sample_class.manager_client.HueManagerClient import SoPHueManagerClient
+from big_thing.MXTag import MXTag
+from big_thing.MXArgument import MXArgument
+from big_thing.MXFunction import MXFunction
+from big_thing.MXValue import MXValue
+from big_thing.MXThing import MXThing
+from sample_class.manager_client.HueManagerClient import MXHueManagerClient
 
 from typing import *
 from threading import Thread, Event, current_thread
 from functools import singledispatch
 from queue import Queue
 from time import sleep, time
 import json
 
 from termcolor import colored, cprint
 import paho.mqtt.client as mqtt
 import pytest
 
 
 def test_manager_client_init():
-    client = SoPHueManagerClient(ip='iotdev.snu.ac.kr', port=11883,
-                                 bridge_ip='http://147.46.114.24/api/', bridge_port=80,
-                                 user_key='L-idzo6XFfRVA-DzXyA66xKzi-KxIJA75neakYyS',
-                                 refresh_cycle=5,)
+    client = MXHueManagerClient(ip='iotdev.snu.ac.kr', port=11883,
+                                bridge_ip='http://147.46.114.24/api/', bridge_port=80,
+                                user_key='L-idzo6XFfRVA-DzXyA66xKzi-KxIJA75neakYyS',
+                                refresh_cycle=5,)
     assert client.setup()
     assert client.run(timeout=5)
     assert client.wrapup()
 
 
 cnt = 3
 
 
 def test_manager_client_run():
     global cnt
 
-    client = SoPHueManagerClient(ip='iotdev.snu.ac.kr', port=11883,
-                                 bridge_ip='http://147.46.114.24/api/', bridge_port=80,
-                                 user_key='L-idzo6XFfRVA-DzXyA66xKzi-KxIJA75neakYyS',
-                                 refresh_cycle=5,)
+    client = MXHueManagerClient(ip='iotdev.snu.ac.kr', port=11883,
+                                bridge_ip='http://147.46.114.24/api/', bridge_port=80,
+                                user_key='L-idzo6XFfRVA-DzXyA66xKzi-KxIJA75neakYyS',
+                                refresh_cycle=5,)
     assert client.setup()
 
     execute_event: Event = Event()
     execute_thread: Thread = Thread(
         target=client.run, daemon=True, kwargs={'stop_event': execute_event, 'timeout': 20, })
     execute_thread.start()
     base_run_time = 2
```

## big_thing_py/utils/api_util.py

```diff
@@ -1,221 +1,18 @@
 from big_thing_py.utils import *
 import requests
-from enum import Enum
+from enum import Enum, auto
 
 
 class RequestMethod(Enum):
     GET = 0
     POST = 1
     PUT = 2
     DELETE = 3
 
-# class GoogleAPIClient():
-#     def __init__(self, client_id: str = None, api_key: str = None) -> None:
-#         self.client_id = client_id
-#         self.api_key = api_key
-#         self.headers = {"X-Naver-Client-Id": self.client_id,
-#                         "X-Naver-Client-Secret": self.api_key}
-
-
-class NaverAPIClient():
-    def __init__(self, client_id: str = None, api_key: str = None) -> None:
-        self.client_id = client_id
-        self.api_key = api_key
-        self.headers = {"X-Naver-Client-Id": self.client_id,
-                        "X-Naver-Client-Secret": self.api_key}
-
-    # def search(self, ):
-    #     url = "https://openapi.naver.com/v1/datalab/search"
-    #     self.headers['Content-Type'] = 'application/json'
-
-    #     files = "{\"startDate\":\"2017-01-01\",\"endDate\":\"2017-04-30\",\"timeUnit\":\"month\",\"keywordGroups\":[{\"groupName\":\"한글\",\"keywords\":[\"한글\",\"korean\"]},{\"groupName\":\"영어\",\"keywords\":[\"영어\",\"english\"]}],\"device\":\"pc\",\"ages\":[\"1\",\"2\"],\"gender\":\"f\"}"
-
-    #     request = urllib.request.Request(url)
-    #     request.add_header("X-Naver-Client-Id", self.client_id)
-    #     request.add_header("X-Naver-Client-Secret", self.api_key)
-    #     request.add_header("Content-Type", "application/json")
-    #     response = urllib.request.urlopen(request, data=files.encode("utf-8"))
-    #     rescode = response.getcode()
-    #     if (rescode == 200):
-    #         response_body = response.read()
-    #         print(response_body.decode('utf-8'))
-    #     else:
-    #         print("Error Code:" + rescode)
-
-    def face_detect(self, image: str):
-        url = "https://openapi.naver.com/v1/vision/face"  # 얼굴감지
-
-        files = {'image': open(image, 'rb')}
-        response = requests.post(url,  files=files, headers=self.headers)
-        rescode = response.status_code
-        if (rescode == 200):
-            return response.text
-        else:
-            return f"Error Code: {rescode}"
-
-    def face_detect_celebrity(self, image: str) -> str:
-        url = "https://openapi.naver.com/v1/vision/celebrity"  # 유명인 얼굴인식
-
-        files = {'image': open(image, 'rb')}
-        response = requests.post(url,  files=files, headers=self.headers)
-        rescode = response.status_code
-        if (rescode == 200):
-            return json_string_to_dict(response.text)['faces'][0]['celebrity']['value']
-        else:
-            return "해당없음"
-
-    def papago(self, text: str, src: str, dst: str):
-        url = "https://openapi.naver.com/v1/papago/n2mt"
-
-        data = {'source': src,
-                'target': dst,
-                'text': text.encode('utf-8')}
-
-        response = requests.post(url, data=data, headers=self.headers)
-        rescode = response.status_code
-
-        if (rescode == 200):
-            return json_string_to_dict(response.text)['message']['result']['translatedText']
-        else:
-            return f"Error Code: {rescode}"
-
-    def papago_detect_lang(self, text: str):
-        url = "https://openapi.naver.com/v1/papago/detectLangs"
-
-        data = {'query': text.encode('utf-8')}
-
-        response = requests.post(url, data=data, headers=self.headers)
-        rescode = response.status_code
-
-        if (rescode == 200):
-            return response.text
-        else:
-            return f"Error Code: {rescode}"
-
-
-class KakaoAPIClient():
-    def __init__(self, api_key: str = None) -> None:
-        self.api_key = api_key
-        self.headers = {
-            'Authorization': f'KakaoAK {self.api_key}'
-        }
-
-    def search(self, text) -> dict:
-        '''
-        Ref: https://developers.kakao.com/docs/latest/ko/daum-search/dev-guide
-        '''
-        url = 'https://dapi.kakao.com/v2/search/web'
-        params = {
-            'query': text
-        }
-        data = None
-        response = requests.get(
-            url, headers=self.headers, params=params, data=data)
-        return response.json()
-
-    def pose(self, image: str) -> dict:
-        '''
-        Ref: https://developers.kakao.com/docs/latest/ko/pose/dev-guide
-        '''
-
-        url = "https://cv-api.kakaobrain.com/pose"
-        params = None
-        data = {'image_url': image} if 'http' in image else None
-        files = {'file': open(image, 'rb').read()
-                 } if 'http' not in image else None
-        response = requests.post(
-            url=url, headers=self.headers, params=params, data=data, files=files)
-        return response.json()
-
-    def OCR(self, image: str):
-        '''
-        Ref: https://www.kakaoicloud.com/service/detail/6-9
-        '''
-        url = "https://dapi.kakao.com/v2/vision/text/ocr"
-        params = None
-        data = None
-        files = {'image': open(image, 'rb').read()
-                 } if 'http' not in image else None
-        response = requests.post(
-            url=url, headers=self.headers, params=params, data=data, files=files)
-        return response.json()
-
-    def translation(self, text: str, src: str, dst: str):
-        '''
-        Ref: https://www.kakaoicloud.com/service/detail/6-10
-        '''
-        from kakaotrans import Translator
-        translator = Translator()
-        # result = translator.translate("Try your best rather than be the best.")
-        result = translator.translate(text, src, dst)
-        return result
-
-        # url = 'https://dapi.kakao.com/v2/translation/translate'
-        # params = None
-        # data = { 'query': '안녕하세요. 반갑습니다.',}
-        # files = {'image': open(image, 'rb').read()
-        #          } if 'http' not in image else None
-        # response = requests.post(
-        #     url=url, headers=self.headers, params=params, data=data, files=files)
-        # return response.json()
-
-    # def speech_to_text(self):
-    #     '''
-    #     Ref: https://www.kakaoicloud.com/service/detail/6-23
-    #     '''
-    #     from pydub import AudioSegment
-
-    #     url = "https://kakaoi-newtone-openapi.kakao.com/v1/recognize"
-    #     headers = {
-    #         "Content-Type": "application/octet-stream",
-    #         "Transfer-Encoding": "chunked",
-    #         "Authorization": "KakaoAK " + self.api_key,
-    #     }
-
-    #     src = "transcript.mp3"
-    #     dst = "test.wav"
-
-    #     audSeg = AudioSegment.from_mp3(src)
-    #     audSeg.export(dst, format="wav")
-
-    #     with open('heykakao.wav', 'rb') as fp:
-    #         audio = fp.read()
-
-    #     res = requests.post(url, headers=headers, data=audio)
-    #     print(res.text)
-
-    # def text_to_speech(self, text: str):
-    #     from playsound import playsound
-    #     url = "https://kakaoi-newtone-openapi.kakao.com/v1/synthesize"
-    #     self.headers["Content-Type"] = "application/xml"
-
-    #     data = f"<speak>{text}</speak>".encode('utf-8')
-    #     res = requests.post(url, headers=self.headers, data=data)
-    #     file_name = 'test_file.wav'
-    #     with open(file_name, 'wb') as f:
-    #         f.write(res.content)
-
-    #     playsound(file_name)
-
-    # def NLP(self):
-    #     '''
-    #     Ref: https://www.kakaoicloud.com/service/detail/6-25
-    #     '''
-
-    # def Vision(self, image: str):
-    #     '''
-    #     Ref: https://www.kakaoicloud.com/service/detail/6-28
-    #     '''
-
-    # def Conversion(self):
-    #     '''
-    #     Ref: https://www.kakaoicloud.com/service/detail/6-29
-    #     '''
-
 
 def API_response_check(res: requests.Response):
     if res.status_code not in [200, 204]:
         return False
     else:
         return res
 
@@ -241,17 +38,17 @@
         elif method == RequestMethod.PUT:
             res = requests.put(url, headers=header, data=body, verify=verify)
             if API_response_check(res):
                 return res
             else:
                 return False
         elif method == RequestMethod.DELETE:
-            SOPLOG_DEBUG('Not implement yet')
+            MXLOG_DEBUG('Not implement yet')
         else:
-            SOPLOG_DEBUG(
+            MXLOG_DEBUG(
                 f'[decode_MQTT_message] Unexpected request!!!', 'red')
     except Exception as e:
         print_error(e)
         return False
 
 
 # def kakao_test():
```

## big_thing_py/utils/base64_util.py

```diff
@@ -1,13 +1,33 @@
 import base64
+import re
+
+
+def file_to_base64(file_path: str) -> str:
+    with open(file_path, 'rb') as f:
+        return base64.b64encode(f.read()).decode()
+
+
+def base64_to_file(base64_string: str, file_path: str) -> None:
+    with open(file_path, 'wb') as f:
+        f.write(base64.b64decode(base64_string))
 
 
 def string_to_base64(string: str):
-    return base64.b64encode(string.encode('utf-8')).decode('utf-8')
+    return base64.b64encode(string.encode()).decode()
 
 
 def base64_to_string(base64_string: str):
-    return base64.b64decode(base64_string).decode('utf-8')
+    return base64.b64decode(base64_string).decode()
+
+
+def is_base64(s):
+    pattern = re.compile(r'^([A-Za-z0-9+/]{4})*([A-Za-z0-9+/]{3}=|[A-Za-z0-9+/]{2}==)?$')
+
+    if pattern.match(s):
+        return True
+    else:
+        return False
 
 
 if __name__ == '__main__':
-    print(string_to_base64('100'))
+    print(is_base64('asdfsdfdfasd'))
```

## big_thing_py/utils/common_util.py

```diff
@@ -1,144 +1,214 @@
 from big_thing_py.common import *
 
 import inspect
 import socket
 import json
 import time
+import copy
+import random
 from pathlib import Path
 import getmac
+import re
+import sys
+import typing
 
 
 def static_vars(**kwargs):
     def decorate(func):
         for k in kwargs:
-            # print(k)
-            # print(kwargs[k])
             setattr(func, k, kwargs[k])
         return func
     return decorate
 
 
-def get_function_return_type(func: Callable):
-    # sig = signature(func)
-    return func.__annotations__['return']
-
-
-def get_function_parameter(func: Callable):
-    del func.__annotations__['return']
-    return func.__annotations__
-
+def get_type_name(typ: typing.Type) -> str:
+    origin = typing.get_origin(typ)
+    if origin is None:
+        return typ.__name__
+    args = typing.get_args(typ)
+    args_str = ", ".join(get_type_name(arg) for arg in args)
+    return f"{origin.__name__}[{args_str}]"
+
+
+def get_function_info(func: Callable) -> Dict[str, Union[str, List[Tuple[str, Any]]]]:
+    sig = inspect.signature(func)
+    params = [(param.name, param.annotation)
+              for param in sig.parameters.values()]
+    ret_type = sig.return_annotation
+    if ret_type is not None:
+        ret_type = get_type_name(ret_type)
+    return dict(name=func.__name__, args=params, return_type=ret_type)
+
+
+def get_current_function_name() -> str:
+    return inspect.stack()[1].function
+
+
+def get_upper_function_name(step: int = 1, frame=None) -> str:
+    if frame is None:
+        frame = inspect.stack()[1].frame
+    if step == 1:
+        co_name = frame.f_back.f_code.co_name
+    elif step > 1:
+        co_name = get_upper_function_name(step - 1, frame.f_back)
+    else:
+        co_name = 'too many steps... return MAX upper function name'
+    return co_name
 
-def get_ip_from_url(URL: str):
-    return socket.gethostbyname(URL)
 
+def get_mac_address(interface: str = None) -> str:
+    mac_address = getmac.get_mac_address(interface)
 
-def get_mac_address():
-    return str(getmac.get_mac_address()).replace(':', '').upper()
+    if mac_address:
+        mac_address = mac_address.replace(':', '').upper()
+        return mac_address
+    else:
+        return None
 
 
-def get_current_time(mode: TimeFormat = TimeFormat.UNIXTIME):
+def get_current_time(mode: TimeFormat = TimeFormat.UNIXTIME) -> Union[str, float]:
     if mode == TimeFormat.DATETIME1:
         return time.strftime("%Y-%m-%d %H:%M:%S", time.localtime())
     elif mode == TimeFormat.DATETIME2:
         return time.strftime("%Y%m%d_%H%M%S", time.localtime())
     elif mode == TimeFormat.DATE:
         return time.strftime("%Y-%m-%d", time.localtime())
     elif mode == TimeFormat.TIME:
         return time.strftime("%H:%M:%S", time.localtime())
     elif mode == TimeFormat.UNIXTIME:
         return time.time()
     return time.time()
 
 
-def type_converter(in_type: Union[SoPType, type, str]) -> str:
-    if type(in_type) == SoPType:
-        if in_type in (SoPType.BINARY, SoPType.STRING):
+def type_converter(in_type: Union[MXType, type, str, None]) -> Union[type, MXType]:
+    if type(in_type) == MXType:
+        if in_type in (MXType.BINARY, MXType.STRING):
             return str
-        elif in_type == SoPType.BOOL:
+        elif in_type == MXType.BOOL:
             return bool
-        elif in_type == SoPType.DOUBLE:
+        elif in_type == MXType.DOUBLE:
             return float
-        elif in_type == SoPType.INTEGER:
+        elif in_type == MXType.INTEGER:
             return int
-        elif in_type == (SoPType.VOID, SoPType.UNDEFINED):
+        elif in_type in (MXType.VOID, MXType.UNDEFINED):
             return None
         else:
-            raise SoPTypeError('Unexpected python type!!!')
+            raise MXNotSupportedError('Unexpected python type!!!')
     elif type(in_type) == type:
         if in_type == int:
-            return SoPType.INTEGER
-        elif in_type == type(None) or in_type == None:
-            return SoPType.VOID
+            return MXType.INTEGER
         elif in_type == float:
-            return SoPType.DOUBLE
+            return MXType.DOUBLE
         elif in_type == bool:
-            return SoPType.BOOL
+            return MXType.BOOL
         elif in_type == bytes:
-            return SoPType.BINARY
+            return MXType.BINARY
         elif in_type == str:
-            return SoPType.STRING
+            return MXType.STRING
+        elif in_type == type(None):
+            return MXType.VOID
         else:
-            raise SoPTypeError('Unexpected SoPType type!!!')
+            raise MXNotSupportedError('Unexpected MXType type!!!')
     elif type(in_type) == str:
         if in_type == 'int':
-            return SoPType.INTEGER
+            return MXType.INTEGER
         elif in_type == 'void':
-            return SoPType.VOID
+            return MXType.VOID
         elif in_type == 'double':
-            return SoPType.DOUBLE
+            return MXType.DOUBLE
         elif in_type == 'bool':
-            return SoPType.BOOL
+            return MXType.BOOL
         elif in_type == 'binary':
-            return SoPType.BINARY
+            return MXType.BINARY
         elif in_type == 'string':
-            return SoPType.STRING
+            return MXType.STRING
+        elif in_type == 'undefined':
+            return MXType.UNDEFINED
         else:
-            raise SoPTypeError('Unexpected SoPType type!!!')
-
-
-def get_current_function_name():
-    return inspect.currentframe().f_back.f_code.co_name
-
-
-def get_upper_function_name(step: int = 1):
-    if step == 1:
-        return inspect.currentframe().f_back.f_back.f_code.co_name
-    elif step == 2:
-        return inspect.currentframe().f_back.f_back.f_back.f_code.co_name
-    elif step == 3:
-        return inspect.currentframe().f_back.f_back.f_back.f_back.f_code.co_name
-    elif step == 4:
-        return inspect.currentframe().f_back.f_back.f_back.f_back.f_back.f_code.co_name
-    else:
-        print('too many steps... return MAX upper function name')
-        return inspect.currentframe().f_back.f_back.f_back.f_back.f_back.f_code.co_name
+            raise MXNotSupportedError('Unexpected MXType type!!!')
+    elif in_type == None or type(in_type) == type(None):
+        return MXType.VOID
 
 
-def json_file_read(path):
+def json_file_read(path: str) -> Union[dict, bool]:
     try:
         with open(path, 'r') as f:
             return json.load(f)
     except FileNotFoundError:
         return False
 
 
-def json_file_write(path, data, indent: int = 4):
+def json_file_write(path: str, data: Union[str, dict], indent: int = 4) -> None:
     with open(path, 'w') as f:
         if isinstance(data, (dict, str)):
             json.dump(data, f, indent=indent)
         else:
             raise Exception(
                 f'common_util.json_file_write: data type error - {type(data)}')
 
 
-def get_project_root() -> Path:
+def get_project_root(project_name: str = 'big-thing-py') -> Path:
     start_path = Path(__file__)
     while True:
-        if str(start_path).split('/')[-1] == 'big-thing-py':
-            return start_path
+        if str(start_path).split('/')[-1] == project_name:
+            return str(start_path)
         else:
             start_path = start_path.parent
 
 
-def is_file_exist(path):
-    return Path(path).is_file()
+def check_valid_identifier(identifier: str) -> bool:
+    pattern = r'^[a-zA-Z_][a-zA-Z0-9_]*$'
+    return bool(re.match(pattern, identifier))
+
+
+def convert_url_to_ip(url: str) -> str:
+    ip_list = url.split(".")
+    not_ip = False
+
+    for ip_token in ip_list:
+        if not ip_token.isdigit():
+            not_ip = True
+            break
+
+    if not_ip:
+        host_ip = socket.gethostbyname(url.strip())
+        return host_ip
+    elif not all([(0 <= int(ip_token) <= 255) for ip_token in ip_list]) or len(ip_list) != 4:
+        raise Exception('wrong ip format')
+    else:
+        return url
+
+
+def check_python_version():
+    if sys.version_info[0] <= 3 and sys.version_info[1] < 6:
+        raise Exception(
+            'Avahi feature is not supported on python3.6<=. try python3.7 or higher. or disable avahi feature. (avahi_enable=False)')
+
+
+def is_valid_ip_address(ip_address: str) -> bool:
+    if ip_address:
+        octets = ip_address.split('.')
+    else:
+        return False
+
+    if len(octets) != 4:
+        return False
+    for octet in octets:
+        try:
+            value = int(octet)
+        except ValueError:
+            return False
+        if not 0 <= value <= 255:
+            return False
+    return True
+
+
+def dummy_func(arg_list: list):
+    args = ', '.join([str(arg) for arg in arg_list])
+    lambda_str = f"lambda {args}: None"
+    exec(lambda_str)
+    return eval(lambda_str)
+
+
+if __name__ == '__main__':
+    pass
```

## big_thing_py/utils/exception_util.py

```diff
@@ -1,8 +1,8 @@
 from big_thing_py.utils.log_util import *
 
 import traceback
 
 
 def print_error(e: Exception):
     traceback_msg = traceback.format_exc()
-    SOPLOG_DEBUG(f'Traceback message : {traceback_msg}\nError: {e}', 'red')
+    MXLOG_DEBUG(f'Traceback message : {traceback_msg}\nError: {e}', 'red')
```

## big_thing_py/utils/file_util.py

```diff
@@ -5,24 +5,24 @@
 
 def read_file(path: str) -> List[str]:
     try:
         with open(path, 'r') as f:
             return f.readlines()
     except FileNotFoundError as e:
         print_error(e)
-        SOPLOG_DEBUG(f'File not found: {path}')
+        MXLOG_DEBUG(f'File not found: {path}')
         raise e
 
 
 def write_file(path: str, content: Union[str, List[str]]) -> None:
     try:
         os.makedirs(os.path.dirname(path), exist_ok=True)
         with open(path, 'w') as f:
             if isinstance(content, str):
                 f.write(content)
             elif isinstance(content, list):
                 f.writelines(content)
         return path
     except FileNotFoundError as e:
         print_error(e)
-        SOPLOG_DEBUG(f'Path not found: {path}')
+        MXLOG_DEBUG(f'Path not found: {path}')
         raise e
```

## big_thing_py/utils/json_util.py

```diff
@@ -1,32 +1,38 @@
 from big_thing_py.common import *
 from big_thing_py.utils.log_util import *
 
 import json
 
 
-def json_string_to_dict(jsonstring: str) -> Union[str, Dict]:
+def json_string_to_dict(json_string: str) -> Union[str, dict]:
     try:
-        if type(jsonstring) in [str, bytes]:
-            return json.loads(jsonstring)
+        if type(json_string) in [str, bytes]:
+            return json.loads(json_string)
         else:
-            return jsonstring
+            return json_string
 
     except json.JSONDecodeError as e:
-        # TODO: will be removed if middleware ME/NOTIFY_CHANGE payload issue is fixed
-        # print_error(e)
-        # SOPLOG_DEBUG(
-        #     f'[json_string_to_dict] input string must be json format string... return raw string...', 'red')
-        return False
+        MXLOG_DEBUG(f'[json_string_to_dict] input string must be json format string... return raw string...', 'red')
+        return json_string
 
 
-def dict_to_json_string(dict_object: dict) -> str:
+def dict_to_json_string(dict_object: Union[dict, list, str], pretty: bool = True, indent: int = 4) -> str:
     try:
         if type(dict_object) == dict:
-            return json.dumps(dict_object, sort_keys=True, indent=4)
+            if pretty:
+                return json.dumps(dict_object, sort_keys=True, indent=indent)
+            else:
+                return json.dumps(dict_object)
         elif type(dict_object) == list:
-            return '\n'.join([json.dumps(item, sort_keys=True, indent=4) for item in dict_object])
+            if pretty:
+                return '\n'.join([json.dumps(item, sort_keys=True, indent=indent) for item in dict_object])
+            else:
+                return '\n'.join([json.dumps(item) for item in dict_object])
         else:
-            return str(dict_object)
+            if pretty:
+                json.dumps(json.loads(dict_object), sort_keys=True, indent=indent)
+            else:
+                return str(dict_object)
     except Exception as e:
-        SOPLOG_DEBUG('[dict_to_json_string] ' + str(e), 'red')
+        MXLOG_DEBUG('[dict_to_json_string] ' + str(e), 'red')
         return False
```

## big_thing_py/utils/log_util.py

```diff
@@ -1,20 +1,42 @@
 from big_thing_py.common import *
 
-from typing import *
 from termcolor import *
 
 import logging
 import os
 import time
 import re
 from enum import Enum
+from datetime import datetime
 
 
-class SoPLogger:
+class MicrosecondFormatter(logging.Formatter):
+    def formatTime(self, record, datefmt=None):
+        ct = self.converter(record.created)
+        if datefmt:
+            s = datetime.now().strftime(datefmt)
+        else:
+            t = time.strftime("%Y-%m-%d %H:%M:%S", ct)
+            s = "%s,%03d" % (t, record.msecs)  # 마이크로초까지 출력
+        return s
+
+
+class MicrosecondFormatter(logging.Formatter):
+    def formatTime(self, record, datefmt=None):
+        ct = self.converter(record.created)
+        if datefmt:
+            s = datetime.now().strftime(datefmt)
+        else:
+            t = time.strftime("%Y-%m-%d %H:%M:%S", ct)
+            s = "%s,%03d" % (t, record.msecs)  # 마이크로초까지 출력
+        return s
+
+
+class MXLogger:
 
     class LoggingMode(Enum):
         ALL = 0
         FILE = 1
         CONSOLE = 2
         OFF = 3
 
@@ -30,15 +52,16 @@
         self._file_path = file_path
         self._logging_mode = logging_mode
 
         self._console_logger = None
         self._file_logger = None
 
     def start(self):
-        formatter = logging.Formatter('[%(asctime)-10s]: %(message)s')
+        formatter = MicrosecondFormatter('[%(asctime)s] %(message)s', datefmt='%Y/%m/%d %H:%M:%S.%f')
+        # formatter = logging.Formatter('[%(asctime)s.%(msecs)d] %(message)s', datefmt='%Y/%m/%d %H:%M:%S')
         level_list = [logging.DEBUG, logging.INFO,
                       logging.WARN, logging.ERROR, logging.CRITICAL]
 
         if self._logging_mode == self.LoggingMode.ALL:
             os.makedirs(
                 '/'.join(self._file_path.rstrip('/').split('/')), exist_ok=True)
 
@@ -115,15 +138,15 @@
             self.select_by_logger_name(logger.name, logger.warn, msg, color)
         elif print_mode == self.PrintMode.ERROR:
             self.select_by_logger_name(logger.name, logger.error,  msg, color)
         elif print_mode == self.PrintMode.CRITICAL:
             self.select_by_logger_name(
                 logger.name, logger.critical,  msg, color)
         else:
-            cprint(f'[SOPLOG_DEBUG] not supported print mode...', 'red')
+            cprint(f'[MXLOG_DEBUG] not supported print mode...', 'red')
 
     def print(self, msg: List[str], color: str = None, mode: PrintMode = PrintMode.DEBUG):
         try:
             if self._logging_mode == self.LoggingMode.ALL:
                 self.select_by_print_mode(
                     self._console_logger, msg, color, mode)
                 self.select_by_print_mode(self._file_logger, msg, color, mode)
@@ -131,54 +154,54 @@
                 self.select_by_print_mode(self._file_logger, msg, color, mode)
             elif self._logging_mode == self.LoggingMode.CONSOLE:
                 self.select_by_print_mode(
                     self._console_logger, msg, color, mode)
             elif self._logging_mode == self.LoggingMode.OFF:
                 pass
             else:
-                raise Exception(f'[SOPLOG_DEBUG] Not supported logging mode ')
+                raise Exception(f'[MXLOG_DEBUG] Not supported logging mode ')
         except Exception as e:
-            print(f'[SOPLOG_DEBUG] Unknown exception error : {str(e)}')
+            print(f'[MXLOG_DEBUG] Unknown exception error : {str(e)}')
             pass
 
 
-base_logger: SoPLogger = None
+base_logger: MXLogger = None
 
 
 def START_LOGGER(whole_log_path: str = None,
-                 logging_mode: SoPLogger.LoggingMode = SoPLogger.LoggingMode.ALL):
+                 logging_mode: MXLogger.LoggingMode = MXLogger.LoggingMode.ALL):
     global base_logger
 
     if not whole_log_path:
         whole_log_path = f'./log/mqtt_message_{time.strftime("%Y%m%d%H%M", time.localtime(time.time()))}.log'
     else:
-        whole_log_path = f'{whole_log_path.rsplit(".", 1)[0]}_{time.strftime("%Y%m%d%H%M", time.localtime(time.time()))}.log'
+        whole_log_path = f'./{whole_log_path.rsplit(".", 1)[0]}_{time.strftime("%Y%m%d%H%M", time.localtime(time.time()))}.log'
     os.makedirs(os.path.dirname(whole_log_path), exist_ok=True)
     log_name = os.path.basename(whole_log_path)
     log_path = os.path.dirname(whole_log_path)
 
     if base_logger is None:
-        base_logger = SoPLogger(log_name, log_path, logging_mode)
+        base_logger = MXLogger(log_name, log_path, logging_mode)
         base_logger.start()
-        # cprint('logger is started!', 'green')
+    # cprint('logger is started!', 'green')
 
 
-def SOPLOG_DEBUG(msg: List[str], color: str = None, mode: SoPLogger.PrintMode = SoPLogger.PrintMode.DEBUG):
+def MXLOG_DEBUG(msg: List[str], color: str = None, mode: MXLogger.PrintMode = MXLogger.PrintMode.DEBUG):
     global base_logger
     if base_logger is not None:
         base_logger.print(msg, color, mode)
     else:
-        cprint('SoPLogger is not initialized... start logger init', 'red')
-        START_LOGGER()
+        cprint('MXLogger is not initialized... start logger init', 'red')
+        # START_LOGGER()
 
 
 if __name__ == '__main__':
-    # START_LOGGER(logging_mode=SoPLogger.LoggingMode.ALL)
-    START_LOGGER(logging_mode=SoPLogger.LoggingMode.FILE)
-    # START_LOGGER(logging_mode=SoPLogger.LoggingMode.CONSOLE)
-    SOPLOG_DEBUG('test', 'red')
-    SOPLOG_DEBUG('test')
-    # logger.print(f'INFO test', color='red', mode=SOPLogger.PrintMode.INFO)
-    # logger.print(f'WARN test', color='red', mode=SOPLogger.PrintMode.WARN)
-    # logger.print(f'ERROR test', color='red', mode=SOPLogger.PrintMode.ERROR)
+    # START_LOGGER(logging_mode=MXLogger.LoggingMode.ALL)
+    START_LOGGER(logging_mode=MXLogger.LoggingMode.FILE)
+    # START_LOGGER(logging_mode=MXLogger.LoggingMode.CONSOLE)
+    MXLOG_DEBUG('test', 'red')
+    MXLOG_DEBUG('test')
+    # logger.print(f'INFO test', color='red', mode=MXLogger.PrintMode.INFO)
+    # logger.print(f'WARN test', color='red', mode=MXLogger.PrintMode.WARN)
+    # logger.print(f'ERROR test', color='red', mode=MXLogger.PrintMode.ERROR)
     # logger.print(f'CRITICAL test', color='red',
-    #              mode=SOPLogger.PrintMode.CRITICAL)
+    #              mode=MXLogger.PrintMode.CRITICAL)
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## big_thing_py/utils/mqtt_util.py

```diff
@@ -1,56 +1,58 @@
 from big_thing_py.utils.exception_util import *
 from big_thing_py.utils.log_util import *
 from big_thing_py.utils.json_util import *
 
 import paho.mqtt.client as mqtt
 
 
-def decode_MQTT_message(msg: mqtt.MQTTMessage = None, mode=dict) -> Tuple[str, dict]:
-    try:
-        topic: str = msg.topic
-        payload: dict = msg.payload
-        timestamp: float = msg.timestamp
-
-        if type(msg.payload) == dict:
-            payload: dict = msg.payload
-        elif type(msg.payload) in [str, bytes]:
-            payload: Union[str, dict] = json_string_to_dict(msg.payload)
-            if payload is False:
-                return topic, None, timestamp
-        else:
-            raise Exception('Unexpected type!!!')
-
-        if type(payload) in [str, bytes]:
-            return topic, str(msg.payload), timestamp
-        if mode == dict:
-            return topic, payload, timestamp
-        elif mode == str:
-            return topic, dict_to_json_string(payload), timestamp
-        else:
-            SOPLOG_DEBUG(f'Unexpected mode!!! : {mode}', 'red')
-    except Exception as e:
-        print_error(e)
-        raise e
-
-
-def encode_MQTT_message(topic: str, payload: str, timestamp: float = None) -> mqtt.MQTTMessage:
+def encode_MQTT_message(topic: str, payload: Union[str, dict], timestamp: float = None) -> mqtt.MQTTMessage:
     try:
         msg = mqtt.MQTTMessage()
         msg.topic = bytes(topic, encoding='utf-8')
-        msg.payload = dict_to_json_string(
-            payload) if type(payload) == dict else payload
+        if isinstance(payload, str):
+            msg.payload = bytes(payload, encoding='utf-8')
+        elif isinstance(payload, dict):
+            msg.payload = dict_to_json_string(payload)
         msg.timestamp = timestamp
 
         return msg
     except Exception as e:
         print_error(e)
         raise e
 
 
+def decode_MQTT_message(msg: mqtt.MQTTMessage, mode=dict) -> Tuple[str, dict]:
+    topic = msg.topic
+    payload = msg.payload
+    timestamp: float = msg.timestamp
+
+    if isinstance(topic, bytes):
+        topic = topic.decode()
+    if isinstance(payload, bytes):
+        payload = payload.decode()
+
+    if isinstance(payload, str):
+        if mode == str:
+            return topic, payload, timestamp
+        elif mode == dict:
+            return topic, json_string_to_dict(payload), timestamp
+        else:
+            raise MXNotSupportedError(f'Unexpected mode!!! - {mode}')
+    elif isinstance(payload, dict):
+        if mode == str:
+            return topic, dict_to_json_string(payload), timestamp
+        elif mode == dict:
+            return topic, payload, timestamp
+        else:
+            raise MXNotSupportedError(f'Unexpected mode!!! - {mode}')
+    else:
+        raise MXNotSupportedError(f'Unexpected type!!! - {type(payload)}')
+
+
 def topic_split(topic: str):
     return topic.split('/')
 
 
 def topic_join(topic: List[str]):
     return '/'.join(topic)
```

## big_thing_py/utils/rf_util.py

```diff
@@ -1,60 +1,60 @@
 from big_thing_py.utils import *
 
-from enum import Enum
+from enum import Enum, auto
 
 
 try:
     from RF24 import RF24, RF24_PA_LOW, RF24_PA_MAX
 except ImportError:
     pass
     # print('RF24 not found', 'red')
 
 
-class SoPRFProtocol(Enum):
+class MXRFProtocol(Enum):
     REG = 'REG'
     RACK = 'RACK'
     VAL = 'VAL'
     LIVE = 'LIVE'
     EXEC = 'EXEC'
     EACK = 'EACK'
 
 
-class SoPRFPowerMode(Enum):
+class MXRFPowerMode(Enum):
     try:
         LOW = RF24_PA_LOW
         HIGH = RF24_PA_MAX
     except Exception:
         pass
-        # SOPLOG_DEBUG('RF24_PA_LOW or RF24_PA_MAX not found', 'red')
+        # MXLOG_DEBUG('RF24_PA_LOW or RF24_PA_MAX not found', 'red')
 
 
-class SoPRFMessage:
-    def __init__(self, protocol_type: SoPRFProtocol, device_id: bytearray, service_name: str, payload: bytearray) -> None:
+class MXRFMessage:
+    def __init__(self, protocol_type: MXRFProtocol, device_id: bytearray, service_name: str, payload: bytearray) -> None:
         self.protocol_type = protocol_type
         self.device_id = device_id
         self.service_name = service_name
         self.payload = payload
 
 
-def decode_RF_message(raw_msg: bytearray) -> SoPRFMessage:
+def decode_RF_message(raw_msg: bytearray) -> MXRFMessage:
     try:
-        protocol_type = SoPRFProtocol(
+        protocol_type = MXRFProtocol(
             raw_msg[:4].rstrip().rstrip(b'\x00').decode().upper())
         device_id = raw_msg[4:8].decode()
         service_name = raw_msg[8:16].rstrip().rstrip(b'\x00').decode()
         payload = raw_msg[16:32].decode()
 
-        return SoPRFMessage(protocol_type=protocol_type, device_id=device_id, service_name=service_name, payload=payload)
+        return MXRFMessage(protocol_type=protocol_type, device_id=device_id, service_name=service_name, payload=payload)
     except Exception as e:
-        SOPLOG_DEBUG('[mqtt_util.py|dict_to_json_string]' + str(e), 'red')
+        MXLOG_DEBUG('[mqtt_util.py|dict_to_json_string]' + str(e), 'red')
         return False
 
 
-def encode_RF_message(msg: SoPRFMessage) -> bytearray:
+def encode_RF_message(msg: MXRFMessage) -> bytearray:
 
     protocol_type = bytearray(msg.protocol_type.value.encode())
     device_id = msg.device_id
     service_name = bytearray(msg.service_name.encode())
     payload = msg.payload
 
     return protocol_type + device_id + service_name + payload
```

## Comparing `big_thing_py/common/request.py` & `big_thing_py/core/request.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,51 @@
-from big_thing_py.common.mqtt_message import *
-from big_thing_py.common.soptype import *
+from big_thing_py.common.mxtype import *
+from big_thing_py.core.mqtt_message import *
 
 
-class SoPRequest(metaclass=ABCMeta):
-    def __init__(self, trigger_msg: SoPMQTTMessage = None, result_msg: SoPMQTTMessage = None) -> None:
-        self._action_type: SoPActionType = None
-        self._trigger_msg = trigger_msg
-        self._result_msg = result_msg
+class MXRequest(metaclass=ABCMeta):
+    def __init__(self, trigger_msg: MXMQTTMessage = None, result_msg: MXMQTTMessage = None) -> None:
+        self._action_type: MXActionType = None
+        self.trigger_msg = trigger_msg
+        self.result_msg = result_msg
 
         # seconds
-        self._duration: float = None
+        self._duration: float = 0
 
     def duration(self):
         return self._duration
 
     def timer_start(self):
-        self._trigger_msg.set_timestamp(time.time())
+        self.trigger_msg.set_timestamp(get_current_time())
 
     def timer_end(self):
         try:
-            self._result_msg.set_timestamp(time.time())
-            self._duration = self._result_msg.timestamp() - \
-                self._trigger_msg.timestamp()
+            self.result_msg.set_timestamp(get_current_time())
+            self._duration = self.result_msg.timestamp - \
+                self.trigger_msg.timestamp
         except Exception:
-            self._duration = time.time() - self._trigger_msg.timestamp()
+            self._duration = time.time() - self.trigger_msg.timestamp
         return self.duration()
 
 
-class SoPRegisterRequest(SoPRequest):
-    def __init__(self, trigger_msg: SoPMQTTMessage = None, result_msg: SoPMQTTMessage = None) -> None:
+class MXRegisterRequest(MXRequest):
+    def __init__(self, trigger_msg: MXMQTTMessage = None, result_msg: MXMQTTMessage = None) -> None:
         super().__init__(trigger_msg, result_msg)
-        self._action_type = SoPActionType.REGISTER
+        self._action_type = MXActionType.REGISTER
 
-        self._trigger_msg: SoPExecuteMessage
-        self._result_msg: SoPExecuteResultMessage
+        self._trigger_msg: MXExecuteMessage
+        self._result_msg: MXExecuteResultMessage
 
 
-class SoPExecuteRequest(SoPRequest):
-    def __init__(self, trigger_msg: SoPExecuteMessage = None, result_msg: SoPExecuteResultMessage = None) -> None:
+class MXExecuteRequest(MXRequest):
+    def __init__(self, trigger_msg: MXExecuteMessage = None, result_msg: MXExecuteResultMessage = None) -> None:
         super().__init__(trigger_msg, result_msg)
-        self._action_type = SoPActionType.EXECUTE
+        self._action_type = MXActionType.EXECUTE
 
-        self._trigger_msg: SoPExecuteMessage
-        self._result_msg: SoPExecuteResultMessage
+        self.trigger_msg: MXExecuteMessage
+        self.result_msg: MXExecuteResultMessage
 
-    def set_return_msg(self, result: SoPExecuteResultMessage):
-        self._result_msg = result
-
-    def set_return_value(self, return_value):
-        self._result_msg._return_value = return_value
+    def set_return_msg(self, result: MXExecuteResultMessage):
+        self.result_msg = result
 
     def get_return_msg(self):
-        return self._result_msg
-
-    def get_return_value(self):
-        return self._result_msg._return_value
+        return self.result_msg
```

