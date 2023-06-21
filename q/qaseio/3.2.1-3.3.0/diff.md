# Comparing `tmp/qaseio-3.2.1.tar.gz` & `tmp/qaseio-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qaseio-3.2.1.tar", last modified: Wed Mar 22 05:07:46 2023, max compression
+gzip compressed data, was "qaseio-3.3.0.tar", last modified: Wed Jun 21 12:54:08 2023, max compression
```

## Comparing `qaseio-3.2.1.tar` & `qaseio-3.3.0.tar`

### file list

```diff
@@ -1,357 +1,369 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 05:07:46.207486 qaseio-3.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-03-22 05:07:46.207486 qaseio-3.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19962 2023-03-22 05:07:39.000000 qaseio-3.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 05:07:46.163486 qaseio-3.2.1/qaseio/
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 05:07:46.167486 qaseio-3.2.1/qaseio/api/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22301 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/api/attachments_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12039 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/api/authors_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    32058 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/api/cases_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    28334 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/api/custom_fields_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    41126 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/api/defects_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29664 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/api/environments_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29774 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/api/milestones_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29136 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/api/plans_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    33347 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/api/projects_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    38549 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/api/results_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    36831 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/api/runs_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/api/search_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29981 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/api/shared_steps_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29871 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/api/suites_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    39138 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 05:07:46.167486 qaseio-3.2.1/qaseio/apis/
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17049 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 05:07:46.187486 qaseio-3.2.1/qaseio/model/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/model/attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12301 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/model/attachment_get.py
--rw-r--r--   0 runner    (1001) docker     (123)    12091 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/model/attachment_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)    11772 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/model/attachment_hash_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    14209 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/model/attachment_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/model/attachment_list_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    12210 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/model/attachment_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    14032 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/model/attachment_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11600 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/model/attachment_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    14095 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/model/attachment_uploads_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11627 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/model/attachment_uploads_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    12110 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/model/author.py
--rw-r--r--   0 runner    (1001) docker     (123)    14149 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/model/author_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/model/author_list_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    12148 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/model/author_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    13950 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/model/author_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11538 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/model/author_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    14224 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/model/create_result200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11766 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/model/create_result200_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    11617 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/model/create_result200_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/model/custom_field.py
--rw-r--r--   0 runner    (1001) docker     (123)    14973 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/model/custom_field_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    11640 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/model/custom_field_create_value_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    14027 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/model/custom_field_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11589 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/model/custom_field_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    14228 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/model/custom_field_update.py
--rw-r--r--   0 runner    (1001) docker     (123)    11543 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/model/custom_field_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    14179 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/model/custom_fields_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11736 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/model/custom_fields_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    12190 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/model/custom_fields_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    15445 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/model/defect.py
--rw-r--r--   0 runner    (1001) docker     (123)    12926 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/model/defect_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    14149 2023-03-22 05:07:39.000000 qaseio-3.2.1/qaseio/model/defect_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/defect_list_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    12148 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/defect_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    13950 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/defect_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11538 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/defect_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    11568 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/defect_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    12776 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/defect_update.py
--rw-r--r--   0 runner    (1001) docker     (123)    12163 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12134 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/environment_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    14224 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/environment_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11766 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/environment_list_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/environment_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    14025 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/environment_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11588 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/environment_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    12074 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/environment_update.py
--rw-r--r--   0 runner    (1001) docker     (123)    14057 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/hash_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11655 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/hash_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    11391 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/hash_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    14027 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/id_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11635 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/id_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    11375 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/id_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    13379 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/milestone.py
--rw-r--r--   0 runner    (1001) docker     (123)    12219 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/milestone_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    14194 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/milestone_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11746 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/milestone_list_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    12178 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/milestone_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    13995 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/milestone_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11568 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/milestone_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    11877 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/milestone_update.py
--rw-r--r--   0 runner    (1001) docker     (123)    13006 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    11922 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/plan_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    15914 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/plan_detailed.py
--rw-r--r--   0 runner    (1001) docker     (123)    11873 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/plan_detailed_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/plan_detailed_all_of_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)    14119 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/plan_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11696 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/plan_list_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    12128 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/plan_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    13977 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/plan_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11575 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/plan_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    11856 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/plan_update.py
--rw-r--r--   0 runner    (1001) docker     (123)    11913 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    11432 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/project_access.py
--rw-r--r--   0 runner    (1001) docker     (123)    14164 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/project_code_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11726 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/project_code_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    11412 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/project_code_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    12546 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/project_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)    11565 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/project_counts_defects.py
--rw-r--r--   0 runner    (1001) docker     (123)    11566 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/project_counts_runs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12788 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/project_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    14164 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/project_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11726 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/project_list_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    12158 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/project_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    13965 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11548 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/project_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    14845 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/qql_defect.py
--rw-r--r--   0 runner    (1001) docker     (123)    12421 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/qql_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    17375 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/qql_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)    13504 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/requirement.py
--rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/response.py
--rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/result.py
--rw-r--r--   0 runner    (1001) docker     (123)    14592 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/result_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    11709 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/result_create_bulk.py
--rw-r--r--   0 runner    (1001) docker     (123)    12356 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/result_create_case.py
--rw-r--r--   0 runner    (1001) docker     (123)    14149 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/result_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/result_list_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    12148 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/result_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    13950 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/result_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11538 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/result_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    13334 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/result_update.py
--rw-r--r--   0 runner    (1001) docker     (123)    14970 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/run.py
--rw-r--r--   0 runner    (1001) docker     (123)    13788 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/run_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    11937 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/run_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    14104 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/run_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11686 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/run_list_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    12118 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/run_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    11575 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/run_milestone.py
--rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/run_public.py
--rw-r--r--   0 runner    (1001) docker     (123)    14134 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/run_public_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11706 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/run_public_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    11401 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/run_public_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    13905 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/run_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/run_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    12905 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/run_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)    14087 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/search_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11675 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/search_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    11594 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/search_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    13993 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/shared_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    12397 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/shared_step_content.py
--rw-r--r--   0 runner    (1001) docker     (123)    12492 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/shared_step_content_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    12828 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/shared_step_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    14211 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/shared_step_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11757 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/shared_step_list_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    12189 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/shared_step_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/shared_step_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11579 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/shared_step_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    12828 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/shared_step_update.py
--rw-r--r--   0 runner    (1001) docker     (123)    13732 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/suite.py
--rw-r--r--   0 runner    (1001) docker     (123)    12252 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/suite_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    11543 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/suite_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)    14134 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/suite_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11706 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/suite_list_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    12138 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/suite_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    13935 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/suite_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11528 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/suite_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    12206 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/suite_update.py
--rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/tag_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    18186 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)    15669 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/test_case_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    14181 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/test_case_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11737 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/test_case_list_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/test_case_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    11186 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/test_case_params.py
--rw-r--r--   0 runner    (1001) docker     (123)    13982 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/test_case_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11559 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/test_case_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    15621 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/test_case_update.py
--rw-r--r--   0 runner    (1001) docker     (123)    13699 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/test_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    12944 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/test_step_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/test_step_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model/test_step_result_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    82567 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 05:07:46.187486 qaseio-3.2.1/qaseio/models/
--rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14247 2023-03-22 05:07:40.000000 qaseio-3.2.1/qaseio/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 05:07:46.163486 qaseio-3.2.1/qaseio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-03-22 05:07:46.000000 qaseio-3.2.1/qaseio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-03-22 05:07:46.000000 qaseio-3.2.1/qaseio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 05:07:46.000000 qaseio-3.2.1/qaseio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-22 05:07:46.000000 qaseio-3.2.1/qaseio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-22 05:07:46.000000 qaseio-3.2.1/qaseio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-22 05:07:46.207486 qaseio-3.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-03-22 05:07:40.000000 qaseio-3.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 05:07:46.207486 qaseio-3.2.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_attachment_get.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_attachment_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_attachment_hash_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_attachment_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_attachment_list_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_attachment_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_attachment_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_attachment_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_attachment_uploads_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_attachment_uploads_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_attachments_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_author.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_author_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_author_list_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_author_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_author_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_author_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_authors_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_cases_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_create_result200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_create_result200_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_create_result200_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_custom_field.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_custom_field_create.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_custom_field_create_value_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_custom_field_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_custom_field_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_custom_field_update.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_custom_field_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_custom_fields_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_custom_fields_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_custom_fields_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_custom_fields_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_defect.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_defect_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_defect_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_defect_list_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_defect_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_defect_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_defect_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_defect_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_defect_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_defects_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_environment_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_environment_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_environment_list_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_environment_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_environment_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_environment_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_environment_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_environments_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_hash_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_hash_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_hash_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_id_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_id_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_id_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_milestone.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_milestone_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_milestone_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_milestone_list_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_milestone_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_milestone_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_milestone_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_milestone_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_milestones_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_plan_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_plan_detailed.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_plan_detailed_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_plan_detailed_all_of_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_plan_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_plan_list_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_plan_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_plan_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_plan_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_plan_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_plans_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_project.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_project_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_project_code_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_project_code_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_project_code_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_project_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_project_counts_defects.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_project_counts_runs.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_project_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_project_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_project_list_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_project_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_project_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_projects_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_qql_defect.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_qql_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_qql_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_requirement.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_result_create.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_result_create_bulk.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_result_create_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_result_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_result_list_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_result_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_result_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_result_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_result_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_results_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_run_create.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_run_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_run_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_run_list_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_run_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_run_milestone.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_run_public.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_run_public_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_run_public_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_run_public_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_run_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_run_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_run_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_runs_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_search_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_search_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_search_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_search_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_shared_step.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_shared_step_content.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_shared_step_content_create.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_shared_step_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_shared_step_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_shared_step_list_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_shared_step_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_shared_step_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_shared_step_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_shared_step_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_shared_steps_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_suite_create.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_suite_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_suite_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_suite_list_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_suite_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_suite_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_suite_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_suite_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_suites_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_tag_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_test_case_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_test_case_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_test_case_list_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_test_case_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_test_case_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_test_case_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_test_case_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_test_case_update.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_test_step.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_test_step_create.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_test_step_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-03-22 05:07:40.000000 qaseio-3.2.1/test/test_test_step_result_create.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:54:08.858263 qaseio-3.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-21 12:54:08.858263 qaseio-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20399 2023-06-21 12:54:06.000000 qaseio-3.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:54:08.806263 qaseio-3.3.0/qaseio/
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:54:08.814263 qaseio-3.3.0/qaseio/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22301 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/api/attachments_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12039 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/api/authors_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37659 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/api/cases_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28334 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/api/custom_fields_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41126 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/api/defects_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29664 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/api/environments_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29774 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/api/milestones_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29136 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/api/plans_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33347 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/api/projects_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38549 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/api/results_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36831 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/api/runs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/api/search_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29981 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/api/shared_steps_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29871 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/api/suites_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39138 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:54:08.814263 qaseio-3.3.0/qaseio/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17049 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:54:08.846263 qaseio-3.3.0/qaseio/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12301 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/attachment_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12091 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/attachment_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11772 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/attachment_hash_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14209 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/attachment_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/attachment_list_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12210 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/attachment_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14032 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/attachment_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11600 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/attachment_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14095 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/attachment_uploads_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11627 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/attachment_uploads_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12110 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/author.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14149 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/author_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/author_list_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12148 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/author_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13950 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/author_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11538 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/author_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14102 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/bulk200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11685 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/bulk200_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11401 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/bulk200_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11671 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/bulk_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18544 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/bulk_request_cases_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11423 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/bulk_request_cases_inner_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14224 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/create_result200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11766 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/create_result200_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11617 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/create_result200_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/custom_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14973 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/custom_field_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11640 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/custom_field_create_value_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14027 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/custom_field_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11589 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/custom_field_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14228 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/custom_field_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11543 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/custom_field_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14179 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/custom_fields_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11736 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/custom_fields_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12190 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/custom_fields_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15445 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/defect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12926 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/defect_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14149 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/defect_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/defect_list_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12148 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/defect_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13950 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/defect_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11538 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/defect_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11568 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/defect_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12776 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/defect_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12163 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12134 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/environment_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14224 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/environment_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11766 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/environment_list_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/environment_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14025 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/environment_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11588 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/environment_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12074 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/environment_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14057 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/hash_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11655 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/hash_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11391 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/hash_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14027 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/id_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11635 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/id_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11375 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/id_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13379 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/milestone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12219 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/milestone_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14194 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/milestone_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11746 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/milestone_list_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12178 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/milestone_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13995 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/milestone_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11568 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/milestone_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11877 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/milestone_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13006 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11922 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/plan_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15914 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/plan_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11873 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/plan_detailed_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/plan_detailed_all_of_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14119 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/plan_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11696 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/plan_list_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12128 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/plan_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13977 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/plan_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11575 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/plan_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11856 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/plan_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11913 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11432 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/project_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14164 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/project_code_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11726 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/project_code_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11412 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/project_code_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12546 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/project_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11565 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/project_counts_defects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11566 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/project_counts_runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12788 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/project_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14164 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/project_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11726 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/project_list_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12158 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/project_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13965 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11548 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/project_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14845 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/qql_defect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12421 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/qql_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17375 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/qql_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13504 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/requirement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14592 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/result_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11709 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/result_create_bulk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12873 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/result_create_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14149 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/result_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/result_list_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12148 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/result_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13950 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/result_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11538 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/result_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13334 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/result_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14970 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14224 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/run_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11937 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/run_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14104 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/run_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11686 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/run_list_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12118 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/run_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11575 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/run_milestone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/run_public.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14134 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/run_public_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11706 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/run_public_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11401 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/run_public_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13905 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/run_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/run_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12905 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/run_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14087 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/search_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11675 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/search_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11594 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/search_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13993 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/shared_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12397 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/shared_step_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12492 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/shared_step_content_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12828 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/shared_step_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14211 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/shared_step_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11757 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/shared_step_list_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12189 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/shared_step_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/shared_step_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11579 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/shared_step_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12828 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/shared_step_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13732 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12252 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/suite_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11543 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/suite_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14134 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/suite_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11706 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/suite_list_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12138 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/suite_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13935 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/suite_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11528 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/suite_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12206 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/suite_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/tag_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18186 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16115 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/test_case_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14181 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/test_case_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11737 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/test_case_list_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/test_case_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11186 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/test_case_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13982 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/test_case_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11559 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/test_case_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15621 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/test_case_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13699 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/test_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12944 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/test_step_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/test_step_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model/test_step_result_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82567 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:54:08.846263 qaseio-3.3.0/qaseio/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    10582 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14241 2023-06-21 12:54:06.000000 qaseio-3.3.0/qaseio/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:54:08.810263 qaseio-3.3.0/qaseio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-21 12:54:08.000000 qaseio-3.3.0/qaseio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12358 2023-06-21 12:54:08.000000 qaseio-3.3.0/qaseio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 12:54:08.000000 qaseio-3.3.0/qaseio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-21 12:54:08.000000 qaseio-3.3.0/qaseio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-21 12:54:08.000000 qaseio-3.3.0/qaseio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-21 12:54:08.862263 qaseio-3.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-21 12:54:06.000000 qaseio-3.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:54:08.858263 qaseio-3.3.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_attachment_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_attachment_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_attachment_hash_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_attachment_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_attachment_list_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_attachment_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_attachment_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_attachment_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_attachment_uploads_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_attachment_uploads_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_attachments_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_author.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_author_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_author_list_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_author_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_author_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_author_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_authors_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_bulk200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_bulk200_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_bulk200_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_bulk_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_bulk_request_cases_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_bulk_request_cases_inner_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_cases_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_create_result200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_create_result200_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_create_result200_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_custom_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_custom_field_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_custom_field_create_value_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_custom_field_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_custom_field_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_custom_field_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_custom_field_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_custom_fields_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_custom_fields_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_custom_fields_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_custom_fields_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_defect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_defect_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_defect_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_defect_list_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_defect_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_defect_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_defect_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_defect_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_defect_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_defects_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_environment_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_environment_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_environment_list_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_environment_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_environment_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_environment_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_environment_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_environments_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_hash_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_hash_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_hash_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_id_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_id_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_milestone.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_milestone_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_milestone_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_milestone_list_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_milestone_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_milestone_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_milestone_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_milestone_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_milestones_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_plan_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_plan_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_plan_detailed_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_plan_detailed_all_of_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_plan_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_plan_list_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_plan_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_plan_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_plan_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_plan_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_plans_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_project_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_project_code_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_project_code_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_project_code_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_project_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_project_counts_defects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_project_counts_runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_project_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_project_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_project_list_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_project_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_project_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_projects_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_qql_defect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_qql_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_qql_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_requirement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_result_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_result_create_bulk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_result_create_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_result_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_result_list_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_result_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_result_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_result_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_result_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_results_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_run_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_run_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_run_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_run_list_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_run_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_run_milestone.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_run_public.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_run_public_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_run_public_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_run_public_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_run_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_run_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_run_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_runs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_search_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_search_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_search_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_search_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_shared_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_shared_step_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_shared_step_content_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_shared_step_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_shared_step_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_shared_step_list_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_shared_step_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_shared_step_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_shared_step_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_shared_step_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_shared_steps_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_suite_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_suite_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_suite_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_suite_list_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_suite_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_suite_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_suite_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_suite_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_suites_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_tag_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_test_case_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_test_case_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_test_case_list_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_test_case_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_test_case_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_test_case_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_test_case_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_test_case_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_test_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_test_step_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_test_step_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-21 12:54:06.000000 qaseio-3.3.0/test/test_test_step_result_create.py
```

### Comparing `qaseio-3.2.1/README.md` & `qaseio-3.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # qaseio
 Qase API Specification.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 1.0.0
-- Package version: 3.2.1
+- Package version: 3.3.0
 - Build package: org.openapitools.codegen.languages.PythonPriorClientCodegen
 For more information, please visit [https://qase.io](https://qase.io)
 
 ## Requirements.
 
 Python >=3.6
 
@@ -95,14 +95,15 @@
 ------------ | ------------- | ------------- | -------------
 *AttachmentsApi* | [**delete_attachment**](docs/AttachmentsApi.md#delete_attachment) | **DELETE** /attachment/{hash} | Remove attachment by Hash.
 *AttachmentsApi* | [**get_attachment**](docs/AttachmentsApi.md#get_attachment) | **GET** /attachment/{hash} | Get attachment by Hash.
 *AttachmentsApi* | [**get_attachments**](docs/AttachmentsApi.md#get_attachments) | **GET** /attachment | Get all attachments.
 *AttachmentsApi* | [**upload_attachment**](docs/AttachmentsApi.md#upload_attachment) | **POST** /attachment/{code} | Upload attachment.
 *AuthorsApi* | [**get_author**](docs/AuthorsApi.md#get_author) | **GET** /author/{id} | Get a specific author.
 *AuthorsApi* | [**get_authors**](docs/AuthorsApi.md#get_authors) | **GET** /author | Get all authors.
+*CasesApi* | [**bulk**](docs/CasesApi.md#bulk) | **POST** /case/{code}/bulk | Create a new test cases.
 *CasesApi* | [**create_case**](docs/CasesApi.md#create_case) | **POST** /case/{code} | Create a new test case.
 *CasesApi* | [**delete_case**](docs/CasesApi.md#delete_case) | **DELETE** /case/{code}/{id} | Delete test case.
 *CasesApi* | [**get_case**](docs/CasesApi.md#get_case) | **GET** /case/{code}/{id} | Get a specific test case.
 *CasesApi* | [**get_cases**](docs/CasesApi.md#get_cases) | **GET** /case/{code} | Get all test cases.
 *CasesApi* | [**update_case**](docs/CasesApi.md#update_case) | **PATCH** /case/{code}/{id} | Update test case.
 *CustomFieldsApi* | [**create_custom_field**](docs/CustomFieldsApi.md#create_custom_field) | **POST** /custom_field | Create new Custom Field.
 *CustomFieldsApi* | [**delete_custom_field**](docs/CustomFieldsApi.md#delete_custom_field) | **DELETE** /custom_field/{id} | Delete Custom Field by id.
@@ -177,14 +178,20 @@
  - [AttachmentUploadsResponseAllOf](docs/AttachmentUploadsResponseAllOf.md)
  - [Author](docs/Author.md)
  - [AuthorListResponse](docs/AuthorListResponse.md)
  - [AuthorListResponseAllOf](docs/AuthorListResponseAllOf.md)
  - [AuthorListResponseAllOfResult](docs/AuthorListResponseAllOfResult.md)
  - [AuthorResponse](docs/AuthorResponse.md)
  - [AuthorResponseAllOf](docs/AuthorResponseAllOf.md)
+ - [Bulk200Response](docs/Bulk200Response.md)
+ - [Bulk200ResponseAllOf](docs/Bulk200ResponseAllOf.md)
+ - [Bulk200ResponseAllOfResult](docs/Bulk200ResponseAllOfResult.md)
+ - [BulkRequest](docs/BulkRequest.md)
+ - [BulkRequestCasesInner](docs/BulkRequestCasesInner.md)
+ - [BulkRequestCasesInnerAllOf](docs/BulkRequestCasesInnerAllOf.md)
  - [CreateResult200Response](docs/CreateResult200Response.md)
  - [CreateResult200ResponseAllOf](docs/CreateResult200ResponseAllOf.md)
  - [CreateResult200ResponseAllOfResult](docs/CreateResult200ResponseAllOfResult.md)
  - [CustomField](docs/CustomField.md)
  - [CustomFieldCreate](docs/CustomFieldCreate.md)
  - [CustomFieldCreateValueInner](docs/CustomFieldCreateValueInner.md)
  - [CustomFieldResponse](docs/CustomFieldResponse.md)
```

### Comparing `qaseio-3.2.1/qaseio/__init__.py` & `qaseio-3.3.0/qaseio/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     The version of the OpenAPI document: 1.0.0
     Contact: support@qase.io
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "3.2.1"
+__version__ = "3.3.0"
 
 # import ApiClient
 from qaseio.api_client import ApiClient
 
 # import Configuration
 from qaseio.configuration import Configuration
```

### Comparing `qaseio-3.2.1/qaseio/api/attachments_api.py` & `qaseio-3.3.0/qaseio/api/attachments_api.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/api/authors_api.py` & `qaseio-3.3.0/qaseio/api/authors_api.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/api/cases_api.py` & `qaseio-3.3.0/qaseio/api/plans_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,50 +19,50 @@
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
 from qaseio.model.id_response import IdResponse
-from qaseio.model.test_case_create import TestCaseCreate
-from qaseio.model.test_case_list_response import TestCaseListResponse
-from qaseio.model.test_case_response import TestCaseResponse
-from qaseio.model.test_case_update import TestCaseUpdate
+from qaseio.model.plan_create import PlanCreate
+from qaseio.model.plan_list_response import PlanListResponse
+from qaseio.model.plan_response import PlanResponse
+from qaseio.model.plan_update import PlanUpdate
 
 
-class CasesApi(object):
+class PlansApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
-        self.create_case_endpoint = _Endpoint(
+        self.create_plan_endpoint = _Endpoint(
             settings={
                 'response_type': (IdResponse,),
                 'auth': [
                     'TokenAuth'
                 ],
-                'endpoint_path': '/case/{code}',
-                'operation_id': 'create_case',
+                'endpoint_path': '/plan/{code}',
+                'operation_id': 'create_plan',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'code',
-                    'test_case_create',
+                    'plan_create',
                 ],
                 'required': [
                     'code',
-                    'test_case_create',
+                    'plan_create',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                     'code',
@@ -76,45 +76,45 @@
                     },
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'code':
                         (str,),
-                    'test_case_create':
-                        (TestCaseCreate,),
+                    'plan_create':
+                        (PlanCreate,),
                 },
                 'attribute_map': {
                     'code': 'code',
                 },
                 'location_map': {
                     'code': 'path',
-                    'test_case_create': 'body',
+                    'plan_create': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
-        self.delete_case_endpoint = _Endpoint(
+        self.delete_plan_endpoint = _Endpoint(
             settings={
                 'response_type': (IdResponse,),
                 'auth': [
                     'TokenAuth'
                 ],
-                'endpoint_path': '/case/{code}/{id}',
-                'operation_id': 'delete_case',
+                'endpoint_path': '/plan/{code}/{id}',
+                'operation_id': 'delete_plan',
                 'http_method': 'DELETE',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'code',
                     'id',
@@ -161,22 +161,22 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.get_case_endpoint = _Endpoint(
+        self.get_plan_endpoint = _Endpoint(
             settings={
-                'response_type': (TestCaseResponse,),
+                'response_type': (PlanResponse,),
                 'auth': [
                     'TokenAuth'
                 ],
-                'endpoint_path': '/case/{code}/{id}',
-                'operation_id': 'get_case',
+                'endpoint_path': '/plan/{code}/{id}',
+                'operation_id': 'get_plan',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'code',
                     'id',
@@ -223,37 +223,28 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.get_cases_endpoint = _Endpoint(
+        self.get_plans_endpoint = _Endpoint(
             settings={
-                'response_type': (TestCaseListResponse,),
+                'response_type': (PlanListResponse,),
                 'auth': [
                     'TokenAuth'
                 ],
-                'endpoint_path': '/case/{code}',
-                'operation_id': 'get_cases',
+                'endpoint_path': '/plan/{code}',
+                'operation_id': 'get_plans',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'code',
-                    'search',
-                    'milestone_id',
-                    'suite_id',
-                    'severity',
-                    'priority',
-                    'type',
-                    'behavior',
-                    'automation',
-                    'status',
                     'limit',
                     'offset',
                 ],
                 'required': [
                     'code',
                 ],
                 'nullable': [
@@ -284,97 +275,61 @@
                     },
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'code':
                         (str,),
-                    'search':
-                        (str,),
-                    'milestone_id':
-                        (int,),
-                    'suite_id':
-                        (int,),
-                    'severity':
-                        (str,),
-                    'priority':
-                        (str,),
-                    'type':
-                        (str,),
-                    'behavior':
-                        (str,),
-                    'automation':
-                        (str,),
-                    'status':
-                        (str,),
                     'limit':
                         (int,),
                     'offset':
                         (int,),
                 },
                 'attribute_map': {
                     'code': 'code',
-                    'search': 'search',
-                    'milestone_id': 'milestone_id',
-                    'suite_id': 'suite_id',
-                    'severity': 'severity',
-                    'priority': 'priority',
-                    'type': 'type',
-                    'behavior': 'behavior',
-                    'automation': 'automation',
-                    'status': 'status',
                     'limit': 'limit',
                     'offset': 'offset',
                 },
                 'location_map': {
                     'code': 'path',
-                    'search': 'query',
-                    'milestone_id': 'query',
-                    'suite_id': 'query',
-                    'severity': 'query',
-                    'priority': 'query',
-                    'type': 'query',
-                    'behavior': 'query',
-                    'automation': 'query',
-                    'status': 'query',
                     'limit': 'query',
                     'offset': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.update_case_endpoint = _Endpoint(
+        self.update_plan_endpoint = _Endpoint(
             settings={
                 'response_type': (IdResponse,),
                 'auth': [
                     'TokenAuth'
                 ],
-                'endpoint_path': '/case/{code}/{id}',
-                'operation_id': 'update_case',
+                'endpoint_path': '/plan/{code}/{id}',
+                'operation_id': 'update_plan',
                 'http_method': 'PATCH',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'code',
                     'id',
-                    'test_case_update',
+                    'plan_update',
                 ],
                 'required': [
                     'code',
                     'id',
-                    'test_case_update',
+                    'plan_update',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                     'code',
@@ -390,25 +345,25 @@
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'code':
                         (str,),
                     'id':
                         (int,),
-                    'test_case_update':
-                        (TestCaseUpdate,),
+                    'plan_update':
+                        (PlanUpdate,),
                 },
                 'attribute_map': {
                     'code': 'code',
                     'id': 'id',
                 },
                 'location_map': {
                     'code': 'path',
                     'id': 'path',
-                    'test_case_update': 'body',
+                    'plan_update': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
@@ -416,32 +371,32 @@
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
 
-    def create_case(
+    def create_plan(
         self,
         code,
-        test_case_create,
+        plan_create,
         **kwargs
     ):
-        """Create a new test case.  # noqa: E501
+        """Create a new plan.  # noqa: E501
 
-        This method allows to create a new test case in selected project.   # noqa: E501
+        This method allows to create a plan in selected project.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_case(code, test_case_create, async_req=True)
+        >>> thread = api.create_plan(code, plan_create, async_req=True)
         >>> result = thread.get()
 
         Args:
             code (str): Code of project, where to search entities.
-            test_case_create (TestCaseCreate):
+            plan_create (PlanCreate):
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -499,31 +454,31 @@
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['code'] = \
             code
-        kwargs['test_case_create'] = \
-            test_case_create
-        return self.create_case_endpoint.call_with_http_info(**kwargs)
+        kwargs['plan_create'] = \
+            plan_create
+        return self.create_plan_endpoint.call_with_http_info(**kwargs)
 
-    def delete_case(
+    def delete_plan(
         self,
         code,
         id,
         **kwargs
     ):
-        """Delete test case.  # noqa: E501
+        """Delete plan.  # noqa: E501
 
-        This method completely deletes a test case from repository.   # noqa: E501
+        This method completely deletes a plan from repository.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_case(code, id, async_req=True)
+        >>> thread = api.delete_plan(code, id, async_req=True)
         >>> result = thread.get()
 
         Args:
             code (str): Code of project, where to search entities.
             id (int): Identifier.
 
         Keyword Args:
@@ -588,29 +543,29 @@
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['code'] = \
             code
         kwargs['id'] = \
             id
-        return self.delete_case_endpoint.call_with_http_info(**kwargs)
+        return self.delete_plan_endpoint.call_with_http_info(**kwargs)
 
-    def get_case(
+    def get_plan(
         self,
         code,
         id,
         **kwargs
     ):
-        """Get a specific test case.  # noqa: E501
+        """Get a specific plan.  # noqa: E501
 
-        This method allows to retrieve a specific test case.   # noqa: E501
+        This method allows to retrieve a specific plan.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_case(code, id, async_req=True)
+        >>> thread = api.get_plan(code, id, async_req=True)
         >>> result = thread.get()
 
         Args:
             code (str): Code of project, where to search entities.
             id (int): Identifier.
 
         Keyword Args:
@@ -642,15 +597,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            TestCaseResponse
+            PlanResponse
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -675,43 +630,34 @@
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['code'] = \
             code
         kwargs['id'] = \
             id
-        return self.get_case_endpoint.call_with_http_info(**kwargs)
+        return self.get_plan_endpoint.call_with_http_info(**kwargs)
 
-    def get_cases(
+    def get_plans(
         self,
         code,
         **kwargs
     ):
-        """Get all test cases.  # noqa: E501
+        """Get all plans.  # noqa: E501
 
-        This method allows to retrieve all test cases stored in selected project.   # noqa: E501
+        This method allows to retrieve all plans stored in selected project.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_cases(code, async_req=True)
+        >>> thread = api.get_plans(code, async_req=True)
         >>> result = thread.get()
 
         Args:
             code (str): Code of project, where to search entities.
 
         Keyword Args:
-            search (str): Provide a string that will be used to search by name.. [optional]
-            milestone_id (int): ID of milestone.. [optional]
-            suite_id (int): ID of test suite.. [optional]
-            severity (str): A list of severity values separated by comma. Possible values: undefined, blocker, critical, major, normal, minor, trivial . [optional]
-            priority (str): A list of priority values separated by comma. Possible values: undefined, high, medium, low . [optional]
-            type (str): A list of type values separated by comma. Possible values: other, functional smoke, regression, security, usability, performance, acceptance . [optional]
-            behavior (str): A list of behavior values separated by comma. Possible values: undefined, positive negative, destructive . [optional]
-            automation (str): A list of values separated by comma. Possible values: is-not-automated, automated to-be-automated . [optional]
-            status (str): A list of values separated by comma. Possible values: actual, draft deprecated . [optional]
             limit (int): A number of entities in result set.. [optional] if omitted the server will use the default value of 10
             offset (int): How many entities should be skipped.. [optional] if omitted the server will use the default value of 0
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -738,15 +684,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            TestCaseListResponse
+            PlanListResponse
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -769,36 +715,36 @@
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['code'] = \
             code
-        return self.get_cases_endpoint.call_with_http_info(**kwargs)
+        return self.get_plans_endpoint.call_with_http_info(**kwargs)
 
-    def update_case(
+    def update_plan(
         self,
         code,
         id,
-        test_case_update,
+        plan_update,
         **kwargs
     ):
-        """Update test case.  # noqa: E501
+        """Update plan.  # noqa: E501
 
-        This method updates a test case.   # noqa: E501
+        This method updates a plan.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_case(code, id, test_case_update, async_req=True)
+        >>> thread = api.update_plan(code, id, plan_update, async_req=True)
         >>> result = thread.get()
 
         Args:
             code (str): Code of project, where to search entities.
             id (int): Identifier.
-            test_case_update (TestCaseUpdate):
+            plan_update (PlanUpdate):
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -858,11 +804,11 @@
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['code'] = \
             code
         kwargs['id'] = \
             id
-        kwargs['test_case_update'] = \
-            test_case_update
-        return self.update_case_endpoint.call_with_http_info(**kwargs)
+        kwargs['plan_update'] = \
+            plan_update
+        return self.update_plan_endpoint.call_with_http_info(**kwargs)
```

### Comparing `qaseio-3.2.1/qaseio/api/custom_fields_api.py` & `qaseio-3.3.0/qaseio/api/custom_fields_api.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/api/defects_api.py` & `qaseio-3.3.0/qaseio/api/defects_api.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/api/environments_api.py` & `qaseio-3.3.0/qaseio/api/environments_api.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/api/milestones_api.py` & `qaseio-3.3.0/qaseio/api/milestones_api.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/api/plans_api.py` & `qaseio-3.3.0/qaseio/api/shared_steps_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,51 +18,51 @@
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from qaseio.model.id_response import IdResponse
-from qaseio.model.plan_create import PlanCreate
-from qaseio.model.plan_list_response import PlanListResponse
-from qaseio.model.plan_response import PlanResponse
-from qaseio.model.plan_update import PlanUpdate
+from qaseio.model.hash_response import HashResponse
+from qaseio.model.shared_step_create import SharedStepCreate
+from qaseio.model.shared_step_list_response import SharedStepListResponse
+from qaseio.model.shared_step_response import SharedStepResponse
+from qaseio.model.shared_step_update import SharedStepUpdate
 
 
-class PlansApi(object):
+class SharedStepsApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
-        self.create_plan_endpoint = _Endpoint(
+        self.create_shared_step_endpoint = _Endpoint(
             settings={
-                'response_type': (IdResponse,),
+                'response_type': (HashResponse,),
                 'auth': [
                     'TokenAuth'
                 ],
-                'endpoint_path': '/plan/{code}',
-                'operation_id': 'create_plan',
+                'endpoint_path': '/shared_step/{code}',
+                'operation_id': 'create_shared_step',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'code',
-                    'plan_create',
+                    'shared_step_create',
                 ],
                 'required': [
                     'code',
-                    'plan_create',
+                    'shared_step_create',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                     'code',
@@ -76,56 +76,56 @@
                     },
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'code':
                         (str,),
-                    'plan_create':
-                        (PlanCreate,),
+                    'shared_step_create':
+                        (SharedStepCreate,),
                 },
                 'attribute_map': {
                     'code': 'code',
                 },
                 'location_map': {
                     'code': 'path',
-                    'plan_create': 'body',
+                    'shared_step_create': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
-        self.delete_plan_endpoint = _Endpoint(
+        self.delete_shared_step_endpoint = _Endpoint(
             settings={
-                'response_type': (IdResponse,),
+                'response_type': (HashResponse,),
                 'auth': [
                     'TokenAuth'
                 ],
-                'endpoint_path': '/plan/{code}/{id}',
-                'operation_id': 'delete_plan',
+                'endpoint_path': '/shared_step/{code}/{hash}',
+                'operation_id': 'delete_shared_step',
                 'http_method': 'DELETE',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'code',
-                    'id',
+                    'hash',
                 ],
                 'required': [
                     'code',
-                    'id',
+                    'hash',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                     'code',
@@ -139,55 +139,55 @@
                     },
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'code':
                         (str,),
-                    'id':
-                        (int,),
+                    'hash':
+                        (str,),
                 },
                 'attribute_map': {
                     'code': 'code',
-                    'id': 'id',
+                    'hash': 'hash',
                 },
                 'location_map': {
                     'code': 'path',
-                    'id': 'path',
+                    'hash': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.get_plan_endpoint = _Endpoint(
+        self.get_shared_step_endpoint = _Endpoint(
             settings={
-                'response_type': (PlanResponse,),
+                'response_type': (SharedStepResponse,),
                 'auth': [
                     'TokenAuth'
                 ],
-                'endpoint_path': '/plan/{code}/{id}',
-                'operation_id': 'get_plan',
+                'endpoint_path': '/shared_step/{code}/{hash}',
+                'operation_id': 'get_shared_step',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'code',
-                    'id',
+                    'hash',
                 ],
                 'required': [
                     'code',
-                    'id',
+                    'hash',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                     'code',
@@ -201,50 +201,51 @@
                     },
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'code':
                         (str,),
-                    'id':
-                        (int,),
+                    'hash':
+                        (str,),
                 },
                 'attribute_map': {
                     'code': 'code',
-                    'id': 'id',
+                    'hash': 'hash',
                 },
                 'location_map': {
                     'code': 'path',
-                    'id': 'path',
+                    'hash': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.get_plans_endpoint = _Endpoint(
+        self.get_shared_steps_endpoint = _Endpoint(
             settings={
-                'response_type': (PlanListResponse,),
+                'response_type': (SharedStepListResponse,),
                 'auth': [
                     'TokenAuth'
                 ],
-                'endpoint_path': '/plan/{code}',
-                'operation_id': 'get_plans',
+                'endpoint_path': '/shared_step/{code}',
+                'operation_id': 'get_shared_steps',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'code',
+                    'search',
                     'limit',
                     'offset',
                 ],
                 'required': [
                     'code',
                 ],
                 'nullable': [
@@ -275,61 +276,65 @@
                     },
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'code':
                         (str,),
+                    'search':
+                        (str,),
                     'limit':
                         (int,),
                     'offset':
                         (int,),
                 },
                 'attribute_map': {
                     'code': 'code',
+                    'search': 'search',
                     'limit': 'limit',
                     'offset': 'offset',
                 },
                 'location_map': {
                     'code': 'path',
+                    'search': 'query',
                     'limit': 'query',
                     'offset': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.update_plan_endpoint = _Endpoint(
+        self.update_shared_step_endpoint = _Endpoint(
             settings={
-                'response_type': (IdResponse,),
+                'response_type': (HashResponse,),
                 'auth': [
                     'TokenAuth'
                 ],
-                'endpoint_path': '/plan/{code}/{id}',
-                'operation_id': 'update_plan',
+                'endpoint_path': '/shared_step/{code}/{hash}',
+                'operation_id': 'update_shared_step',
                 'http_method': 'PATCH',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'code',
-                    'id',
-                    'plan_update',
+                    'hash',
+                    'shared_step_update',
                 ],
                 'required': [
                     'code',
-                    'id',
-                    'plan_update',
+                    'hash',
+                    'shared_step_update',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                     'code',
@@ -343,27 +348,27 @@
                     },
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'code':
                         (str,),
-                    'id':
-                        (int,),
-                    'plan_update':
-                        (PlanUpdate,),
+                    'hash':
+                        (str,),
+                    'shared_step_update':
+                        (SharedStepUpdate,),
                 },
                 'attribute_map': {
                     'code': 'code',
-                    'id': 'id',
+                    'hash': 'hash',
                 },
                 'location_map': {
                     'code': 'path',
-                    'id': 'path',
-                    'plan_update': 'body',
+                    'hash': 'path',
+                    'shared_step_update': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
@@ -371,32 +376,32 @@
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
 
-    def create_plan(
+    def create_shared_step(
         self,
         code,
-        plan_create,
+        shared_step_create,
         **kwargs
     ):
-        """Create a new plan.  # noqa: E501
+        """Create a new shared step.  # noqa: E501
 
-        This method allows to create a plan in selected project.   # noqa: E501
+        This method allows to create a shared step in selected project.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_plan(code, plan_create, async_req=True)
+        >>> thread = api.create_shared_step(code, shared_step_create, async_req=True)
         >>> result = thread.get()
 
         Args:
             code (str): Code of project, where to search entities.
-            plan_create (PlanCreate):
+            shared_step_create (SharedStepCreate):
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -423,15 +428,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            IdResponse
+            HashResponse
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -454,36 +459,36 @@
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['code'] = \
             code
-        kwargs['plan_create'] = \
-            plan_create
-        return self.create_plan_endpoint.call_with_http_info(**kwargs)
+        kwargs['shared_step_create'] = \
+            shared_step_create
+        return self.create_shared_step_endpoint.call_with_http_info(**kwargs)
 
-    def delete_plan(
+    def delete_shared_step(
         self,
         code,
-        id,
+        hash,
         **kwargs
     ):
-        """Delete plan.  # noqa: E501
+        """Delete shared step.  # noqa: E501
 
-        This method completely deletes a plan from repository.   # noqa: E501
+        This method completely deletes a shared step from repository.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_plan(code, id, async_req=True)
+        >>> thread = api.delete_shared_step(code, hash, async_req=True)
         >>> result = thread.get()
 
         Args:
             code (str): Code of project, where to search entities.
-            id (int): Identifier.
+            hash (str): Hash.
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -510,15 +515,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            IdResponse
+            HashResponse
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -541,36 +546,36 @@
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['code'] = \
             code
-        kwargs['id'] = \
-            id
-        return self.delete_plan_endpoint.call_with_http_info(**kwargs)
+        kwargs['hash'] = \
+            hash
+        return self.delete_shared_step_endpoint.call_with_http_info(**kwargs)
 
-    def get_plan(
+    def get_shared_step(
         self,
         code,
-        id,
+        hash,
         **kwargs
     ):
-        """Get a specific plan.  # noqa: E501
+        """Get a specific shared step.  # noqa: E501
 
-        This method allows to retrieve a specific plan.   # noqa: E501
+        This method allows to retrieve a specific shared step.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_plan(code, id, async_req=True)
+        >>> thread = api.get_shared_step(code, hash, async_req=True)
         >>> result = thread.get()
 
         Args:
             code (str): Code of project, where to search entities.
-            id (int): Identifier.
+            hash (str): Hash.
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -597,15 +602,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            PlanResponse
+            SharedStepResponse
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -628,36 +633,37 @@
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['code'] = \
             code
-        kwargs['id'] = \
-            id
-        return self.get_plan_endpoint.call_with_http_info(**kwargs)
+        kwargs['hash'] = \
+            hash
+        return self.get_shared_step_endpoint.call_with_http_info(**kwargs)
 
-    def get_plans(
+    def get_shared_steps(
         self,
         code,
         **kwargs
     ):
-        """Get all plans.  # noqa: E501
+        """Get all shared steps.  # noqa: E501
 
-        This method allows to retrieve all plans stored in selected project.   # noqa: E501
+        This method allows to retrieve all shared steps stored in selected project.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_plans(code, async_req=True)
+        >>> thread = api.get_shared_steps(code, async_req=True)
         >>> result = thread.get()
 
         Args:
             code (str): Code of project, where to search entities.
 
         Keyword Args:
+            search (str): Provide a string that will be used to search by name.. [optional]
             limit (int): A number of entities in result set.. [optional] if omitted the server will use the default value of 10
             offset (int): How many entities should be skipped.. [optional] if omitted the server will use the default value of 0
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -684,15 +690,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            PlanListResponse
+            SharedStepListResponse
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -715,36 +721,36 @@
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['code'] = \
             code
-        return self.get_plans_endpoint.call_with_http_info(**kwargs)
+        return self.get_shared_steps_endpoint.call_with_http_info(**kwargs)
 
-    def update_plan(
+    def update_shared_step(
         self,
         code,
-        id,
-        plan_update,
+        hash,
+        shared_step_update,
         **kwargs
     ):
-        """Update plan.  # noqa: E501
+        """Update shared step.  # noqa: E501
 
-        This method updates a plan.   # noqa: E501
+        This method updates a shared step.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_plan(code, id, plan_update, async_req=True)
+        >>> thread = api.update_shared_step(code, hash, shared_step_update, async_req=True)
         >>> result = thread.get()
 
         Args:
             code (str): Code of project, where to search entities.
-            id (int): Identifier.
-            plan_update (PlanUpdate):
+            hash (str): Hash.
+            shared_step_update (SharedStepUpdate):
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -771,15 +777,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            IdResponse
+            HashResponse
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -802,13 +808,13 @@
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['code'] = \
             code
-        kwargs['id'] = \
-            id
-        kwargs['plan_update'] = \
-            plan_update
-        return self.update_plan_endpoint.call_with_http_info(**kwargs)
+        kwargs['hash'] = \
+            hash
+        kwargs['shared_step_update'] = \
+            shared_step_update
+        return self.update_shared_step_endpoint.call_with_http_info(**kwargs)
```

### Comparing `qaseio-3.2.1/qaseio/api/projects_api.py` & `qaseio-3.3.0/qaseio/api/projects_api.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/api/results_api.py` & `qaseio-3.3.0/qaseio/api/results_api.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/api/runs_api.py` & `qaseio-3.3.0/qaseio/api/runs_api.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/api/search_api.py` & `qaseio-3.3.0/qaseio/api/search_api.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/api/shared_steps_api.py` & `qaseio-3.3.0/qaseio/api/suites_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,51 +18,52 @@
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from qaseio.model.hash_response import HashResponse
-from qaseio.model.shared_step_create import SharedStepCreate
-from qaseio.model.shared_step_list_response import SharedStepListResponse
-from qaseio.model.shared_step_response import SharedStepResponse
-from qaseio.model.shared_step_update import SharedStepUpdate
+from qaseio.model.id_response import IdResponse
+from qaseio.model.suite_create import SuiteCreate
+from qaseio.model.suite_delete import SuiteDelete
+from qaseio.model.suite_list_response import SuiteListResponse
+from qaseio.model.suite_response import SuiteResponse
+from qaseio.model.suite_update import SuiteUpdate
 
 
-class SharedStepsApi(object):
+class SuitesApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
-        self.create_shared_step_endpoint = _Endpoint(
+        self.create_suite_endpoint = _Endpoint(
             settings={
-                'response_type': (HashResponse,),
+                'response_type': (IdResponse,),
                 'auth': [
                     'TokenAuth'
                 ],
-                'endpoint_path': '/shared_step/{code}',
-                'operation_id': 'create_shared_step',
+                'endpoint_path': '/suite/{code}',
+                'operation_id': 'create_suite',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'code',
-                    'shared_step_create',
+                    'suite_create',
                 ],
                 'required': [
                     'code',
-                    'shared_step_create',
+                    'suite_create',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                     'code',
@@ -76,56 +77,57 @@
                     },
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'code':
                         (str,),
-                    'shared_step_create':
-                        (SharedStepCreate,),
+                    'suite_create':
+                        (SuiteCreate,),
                 },
                 'attribute_map': {
                     'code': 'code',
                 },
                 'location_map': {
                     'code': 'path',
-                    'shared_step_create': 'body',
+                    'suite_create': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
-        self.delete_shared_step_endpoint = _Endpoint(
+        self.delete_suite_endpoint = _Endpoint(
             settings={
-                'response_type': (HashResponse,),
+                'response_type': (IdResponse,),
                 'auth': [
                     'TokenAuth'
                 ],
-                'endpoint_path': '/shared_step/{code}/{hash}',
-                'operation_id': 'delete_shared_step',
+                'endpoint_path': '/suite/{code}/{id}',
+                'operation_id': 'delete_suite',
                 'http_method': 'DELETE',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'code',
-                    'hash',
+                    'id',
+                    'suite_delete',
                 ],
                 'required': [
                     'code',
-                    'hash',
+                    'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                     'code',
@@ -139,55 +141,60 @@
                     },
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'code':
                         (str,),
-                    'hash':
-                        (str,),
+                    'id':
+                        (int,),
+                    'suite_delete':
+                        (SuiteDelete,),
                 },
                 'attribute_map': {
                     'code': 'code',
-                    'hash': 'hash',
+                    'id': 'id',
                 },
                 'location_map': {
                     'code': 'path',
-                    'hash': 'path',
+                    'id': 'path',
+                    'suite_delete': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
-                'content_type': [],
+                'content_type': [
+                    'application/json'
+                ]
             },
             api_client=api_client
         )
-        self.get_shared_step_endpoint = _Endpoint(
+        self.get_suite_endpoint = _Endpoint(
             settings={
-                'response_type': (SharedStepResponse,),
+                'response_type': (SuiteResponse,),
                 'auth': [
                     'TokenAuth'
                 ],
-                'endpoint_path': '/shared_step/{code}/{hash}',
-                'operation_id': 'get_shared_step',
+                'endpoint_path': '/suite/{code}/{id}',
+                'operation_id': 'get_suite',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'code',
-                    'hash',
+                    'id',
                 ],
                 'required': [
                     'code',
-                    'hash',
+                    'id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                     'code',
@@ -201,44 +208,44 @@
                     },
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'code':
                         (str,),
-                    'hash':
-                        (str,),
+                    'id':
+                        (int,),
                 },
                 'attribute_map': {
                     'code': 'code',
-                    'hash': 'hash',
+                    'id': 'id',
                 },
                 'location_map': {
                     'code': 'path',
-                    'hash': 'path',
+                    'id': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.get_shared_steps_endpoint = _Endpoint(
+        self.get_suites_endpoint = _Endpoint(
             settings={
-                'response_type': (SharedStepListResponse,),
+                'response_type': (SuiteListResponse,),
                 'auth': [
                     'TokenAuth'
                 ],
-                'endpoint_path': '/shared_step/{code}',
-                'operation_id': 'get_shared_steps',
+                'endpoint_path': '/suite/{code}',
+                'operation_id': 'get_suites',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'code',
                     'search',
@@ -306,35 +313,35 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.update_shared_step_endpoint = _Endpoint(
+        self.update_suite_endpoint = _Endpoint(
             settings={
-                'response_type': (HashResponse,),
+                'response_type': (IdResponse,),
                 'auth': [
                     'TokenAuth'
                 ],
-                'endpoint_path': '/shared_step/{code}/{hash}',
-                'operation_id': 'update_shared_step',
+                'endpoint_path': '/suite/{code}/{id}',
+                'operation_id': 'update_suite',
                 'http_method': 'PATCH',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'code',
-                    'hash',
-                    'shared_step_update',
+                    'id',
+                    'suite_update',
                 ],
                 'required': [
                     'code',
-                    'hash',
-                    'shared_step_update',
+                    'id',
+                    'suite_update',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                     'code',
@@ -348,27 +355,27 @@
                     },
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'code':
                         (str,),
-                    'hash':
-                        (str,),
-                    'shared_step_update':
-                        (SharedStepUpdate,),
+                    'id':
+                        (int,),
+                    'suite_update':
+                        (SuiteUpdate,),
                 },
                 'attribute_map': {
                     'code': 'code',
-                    'hash': 'hash',
+                    'id': 'id',
                 },
                 'location_map': {
                     'code': 'path',
-                    'hash': 'path',
-                    'shared_step_update': 'body',
+                    'id': 'path',
+                    'suite_update': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
@@ -376,32 +383,32 @@
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
 
-    def create_shared_step(
+    def create_suite(
         self,
         code,
-        shared_step_create,
+        suite_create,
         **kwargs
     ):
-        """Create a new shared step.  # noqa: E501
+        """Create a new test suite.  # noqa: E501
 
-        This method allows to create a shared step in selected project.   # noqa: E501
+        This method is used to create a new test suite through API.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_shared_step(code, shared_step_create, async_req=True)
+        >>> thread = api.create_suite(code, suite_create, async_req=True)
         >>> result = thread.get()
 
         Args:
             code (str): Code of project, where to search entities.
-            shared_step_create (SharedStepCreate):
+            suite_create (SuiteCreate):
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -428,15 +435,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            HashResponse
+            IdResponse
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -459,38 +466,39 @@
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['code'] = \
             code
-        kwargs['shared_step_create'] = \
-            shared_step_create
-        return self.create_shared_step_endpoint.call_with_http_info(**kwargs)
+        kwargs['suite_create'] = \
+            suite_create
+        return self.create_suite_endpoint.call_with_http_info(**kwargs)
 
-    def delete_shared_step(
+    def delete_suite(
         self,
         code,
-        hash,
+        id,
         **kwargs
     ):
-        """Delete shared step.  # noqa: E501
+        """Delete test suite.  # noqa: E501
 
-        This method completely deletes a shared step from repository.   # noqa: E501
+        This method completely deletes a test suite with test cases from repository.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_shared_step(code, hash, async_req=True)
+        >>> thread = api.delete_suite(code, id, async_req=True)
         >>> result = thread.get()
 
         Args:
             code (str): Code of project, where to search entities.
-            hash (str): Hash.
+            id (int): Identifier.
 
         Keyword Args:
+            suite_delete (SuiteDelete): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -515,15 +523,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            HashResponse
+            IdResponse
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -546,36 +554,36 @@
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['code'] = \
             code
-        kwargs['hash'] = \
-            hash
-        return self.delete_shared_step_endpoint.call_with_http_info(**kwargs)
+        kwargs['id'] = \
+            id
+        return self.delete_suite_endpoint.call_with_http_info(**kwargs)
 
-    def get_shared_step(
+    def get_suite(
         self,
         code,
-        hash,
+        id,
         **kwargs
     ):
-        """Get a specific shared step.  # noqa: E501
+        """Get a specific test suite.  # noqa: E501
 
-        This method allows to retrieve a specific shared step.   # noqa: E501
+        This method allows to retrieve a specific test suite.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_shared_step(code, hash, async_req=True)
+        >>> thread = api.get_suite(code, id, async_req=True)
         >>> result = thread.get()
 
         Args:
             code (str): Code of project, where to search entities.
-            hash (str): Hash.
+            id (int): Identifier.
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -602,15 +610,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            SharedStepResponse
+            SuiteResponse
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -633,30 +641,30 @@
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['code'] = \
             code
-        kwargs['hash'] = \
-            hash
-        return self.get_shared_step_endpoint.call_with_http_info(**kwargs)
+        kwargs['id'] = \
+            id
+        return self.get_suite_endpoint.call_with_http_info(**kwargs)
 
-    def get_shared_steps(
+    def get_suites(
         self,
         code,
         **kwargs
     ):
-        """Get all shared steps.  # noqa: E501
+        """Get all test suites.  # noqa: E501
 
-        This method allows to retrieve all shared steps stored in selected project.   # noqa: E501
+        This method allows to retrieve all test suites stored in selected project.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_shared_steps(code, async_req=True)
+        >>> thread = api.get_suites(code, async_req=True)
         >>> result = thread.get()
 
         Args:
             code (str): Code of project, where to search entities.
 
         Keyword Args:
             search (str): Provide a string that will be used to search by name.. [optional]
@@ -690,15 +698,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            SharedStepListResponse
+            SuiteListResponse
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -721,36 +729,36 @@
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['code'] = \
             code
-        return self.get_shared_steps_endpoint.call_with_http_info(**kwargs)
+        return self.get_suites_endpoint.call_with_http_info(**kwargs)
 
-    def update_shared_step(
+    def update_suite(
         self,
         code,
-        hash,
-        shared_step_update,
+        id,
+        suite_update,
         **kwargs
     ):
-        """Update shared step.  # noqa: E501
+        """Update test suite.  # noqa: E501
 
-        This method updates a shared step.   # noqa: E501
+        This method is used to update a test suite through API.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_shared_step(code, hash, shared_step_update, async_req=True)
+        >>> thread = api.update_suite(code, id, suite_update, async_req=True)
         >>> result = thread.get()
 
         Args:
             code (str): Code of project, where to search entities.
-            hash (str): Hash.
-            shared_step_update (SharedStepUpdate):
+            id (int): Identifier.
+            suite_update (SuiteUpdate):
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -777,15 +785,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            HashResponse
+            IdResponse
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -808,13 +816,13 @@
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['code'] = \
             code
-        kwargs['hash'] = \
-            hash
-        kwargs['shared_step_update'] = \
-            shared_step_update
-        return self.update_shared_step_endpoint.call_with_http_info(**kwargs)
+        kwargs['id'] = \
+            id
+        kwargs['suite_update'] = \
+            suite_update
+        return self.update_suite_endpoint.call_with_http_info(**kwargs)
```

### Comparing `qaseio-3.2.1/qaseio/api/suites_api.py` & `qaseio-3.3.0/qaseio/api/cases_api.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,52 +18,116 @@
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
+from qaseio.model.bulk200_response import Bulk200Response
+from qaseio.model.bulk_request import BulkRequest
 from qaseio.model.id_response import IdResponse
-from qaseio.model.suite_create import SuiteCreate
-from qaseio.model.suite_delete import SuiteDelete
-from qaseio.model.suite_list_response import SuiteListResponse
-from qaseio.model.suite_response import SuiteResponse
-from qaseio.model.suite_update import SuiteUpdate
+from qaseio.model.test_case_create import TestCaseCreate
+from qaseio.model.test_case_list_response import TestCaseListResponse
+from qaseio.model.test_case_response import TestCaseResponse
+from qaseio.model.test_case_update import TestCaseUpdate
 
 
-class SuitesApi(object):
+class CasesApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
-        self.create_suite_endpoint = _Endpoint(
+        self.bulk_endpoint = _Endpoint(
+            settings={
+                'response_type': (Bulk200Response,),
+                'auth': [
+                    'TokenAuth'
+                ],
+                'endpoint_path': '/case/{code}/bulk',
+                'operation_id': 'bulk',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'code',
+                    'bulk_request',
+                ],
+                'required': [
+                    'code',
+                    'bulk_request',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                    'code',
+                ]
+            },
+            root_map={
+                'validations': {
+                    ('code',): {
+                        'max_length': 10,
+                        'min_length': 2,
+                    },
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'code':
+                        (str,),
+                    'bulk_request':
+                        (BulkRequest,),
+                },
+                'attribute_map': {
+                    'code': 'code',
+                },
+                'location_map': {
+                    'code': 'path',
+                    'bulk_request': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
+        self.create_case_endpoint = _Endpoint(
             settings={
                 'response_type': (IdResponse,),
                 'auth': [
                     'TokenAuth'
                 ],
-                'endpoint_path': '/suite/{code}',
-                'operation_id': 'create_suite',
+                'endpoint_path': '/case/{code}',
+                'operation_id': 'create_case',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'code',
-                    'suite_create',
+                    'test_case_create',
                 ],
                 'required': [
                     'code',
-                    'suite_create',
+                    'test_case_create',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                     'code',
@@ -77,53 +141,52 @@
                     },
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'code':
                         (str,),
-                    'suite_create':
-                        (SuiteCreate,),
+                    'test_case_create':
+                        (TestCaseCreate,),
                 },
                 'attribute_map': {
                     'code': 'code',
                 },
                 'location_map': {
                     'code': 'path',
-                    'suite_create': 'body',
+                    'test_case_create': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
-        self.delete_suite_endpoint = _Endpoint(
+        self.delete_case_endpoint = _Endpoint(
             settings={
                 'response_type': (IdResponse,),
                 'auth': [
                     'TokenAuth'
                 ],
-                'endpoint_path': '/suite/{code}/{id}',
-                'operation_id': 'delete_suite',
+                'endpoint_path': '/case/{code}/{id}',
+                'operation_id': 'delete_case',
                 'http_method': 'DELETE',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'code',
                     'id',
-                    'suite_delete',
                 ],
                 'required': [
                     'code',
                     'id',
                 ],
                 'nullable': [
                 ],
@@ -143,47 +206,42 @@
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'code':
                         (str,),
                     'id':
                         (int,),
-                    'suite_delete':
-                        (SuiteDelete,),
                 },
                 'attribute_map': {
                     'code': 'code',
                     'id': 'id',
                 },
                 'location_map': {
                     'code': 'path',
                     'id': 'path',
-                    'suite_delete': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
-                'content_type': [
-                    'application/json'
-                ]
+                'content_type': [],
             },
             api_client=api_client
         )
-        self.get_suite_endpoint = _Endpoint(
+        self.get_case_endpoint = _Endpoint(
             settings={
-                'response_type': (SuiteResponse,),
+                'response_type': (TestCaseResponse,),
                 'auth': [
                     'TokenAuth'
                 ],
-                'endpoint_path': '/suite/{code}/{id}',
-                'operation_id': 'get_suite',
+                'endpoint_path': '/case/{code}/{id}',
+                'operation_id': 'get_case',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'code',
                     'id',
@@ -230,29 +288,37 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.get_suites_endpoint = _Endpoint(
+        self.get_cases_endpoint = _Endpoint(
             settings={
-                'response_type': (SuiteListResponse,),
+                'response_type': (TestCaseListResponse,),
                 'auth': [
                     'TokenAuth'
                 ],
-                'endpoint_path': '/suite/{code}',
-                'operation_id': 'get_suites',
+                'endpoint_path': '/case/{code}',
+                'operation_id': 'get_cases',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'code',
                     'search',
+                    'milestone_id',
+                    'suite_id',
+                    'severity',
+                    'priority',
+                    'type',
+                    'behavior',
+                    'automation',
+                    'status',
                     'limit',
                     'offset',
                 ],
                 'required': [
                     'code',
                 ],
                 'nullable': [
@@ -285,63 +351,95 @@
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'code':
                         (str,),
                     'search':
                         (str,),
+                    'milestone_id':
+                        (int,),
+                    'suite_id':
+                        (int,),
+                    'severity':
+                        (str,),
+                    'priority':
+                        (str,),
+                    'type':
+                        (str,),
+                    'behavior':
+                        (str,),
+                    'automation':
+                        (str,),
+                    'status':
+                        (str,),
                     'limit':
                         (int,),
                     'offset':
                         (int,),
                 },
                 'attribute_map': {
                     'code': 'code',
                     'search': 'search',
+                    'milestone_id': 'milestone_id',
+                    'suite_id': 'suite_id',
+                    'severity': 'severity',
+                    'priority': 'priority',
+                    'type': 'type',
+                    'behavior': 'behavior',
+                    'automation': 'automation',
+                    'status': 'status',
                     'limit': 'limit',
                     'offset': 'offset',
                 },
                 'location_map': {
                     'code': 'path',
                     'search': 'query',
+                    'milestone_id': 'query',
+                    'suite_id': 'query',
+                    'severity': 'query',
+                    'priority': 'query',
+                    'type': 'query',
+                    'behavior': 'query',
+                    'automation': 'query',
+                    'status': 'query',
                     'limit': 'query',
                     'offset': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.update_suite_endpoint = _Endpoint(
+        self.update_case_endpoint = _Endpoint(
             settings={
                 'response_type': (IdResponse,),
                 'auth': [
                     'TokenAuth'
                 ],
-                'endpoint_path': '/suite/{code}/{id}',
-                'operation_id': 'update_suite',
+                'endpoint_path': '/case/{code}/{id}',
+                'operation_id': 'update_case',
                 'http_method': 'PATCH',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'code',
                     'id',
-                    'suite_update',
+                    'test_case_update',
                 ],
                 'required': [
                     'code',
                     'id',
-                    'suite_update',
+                    'test_case_update',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                     'code',
@@ -357,25 +455,25 @@
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'code':
                         (str,),
                     'id':
                         (int,),
-                    'suite_update':
-                        (SuiteUpdate,),
+                    'test_case_update':
+                        (TestCaseUpdate,),
                 },
                 'attribute_map': {
                     'code': 'code',
                     'id': 'id',
                 },
                 'location_map': {
                     'code': 'path',
                     'id': 'path',
-                    'suite_update': 'body',
+                    'test_case_update': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
@@ -383,32 +481,119 @@
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
 
-    def create_suite(
+    def bulk(
+        self,
+        code,
+        bulk_request,
+        **kwargs
+    ):
+        """Create a new test cases.  # noqa: E501
+
+        This method allows to bulk create new test cases in a project.   # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.bulk(code, bulk_request, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            code (str): Code of project, where to search entities.
+            bulk_request (BulkRequest):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            Bulk200Response
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['code'] = \
+            code
+        kwargs['bulk_request'] = \
+            bulk_request
+        return self.bulk_endpoint.call_with_http_info(**kwargs)
+
+    def create_case(
         self,
         code,
-        suite_create,
+        test_case_create,
         **kwargs
     ):
-        """Create a new test suite.  # noqa: E501
+        """Create a new test case.  # noqa: E501
 
-        This method is used to create a new test suite through API.   # noqa: E501
+        This method allows to create a new test case in selected project.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_suite(code, suite_create, async_req=True)
+        >>> thread = api.create_case(code, test_case_create, async_req=True)
         >>> result = thread.get()
 
         Args:
             code (str): Code of project, where to search entities.
-            suite_create (SuiteCreate):
+            test_case_create (TestCaseCreate):
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -466,39 +651,38 @@
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['code'] = \
             code
-        kwargs['suite_create'] = \
-            suite_create
-        return self.create_suite_endpoint.call_with_http_info(**kwargs)
+        kwargs['test_case_create'] = \
+            test_case_create
+        return self.create_case_endpoint.call_with_http_info(**kwargs)
 
-    def delete_suite(
+    def delete_case(
         self,
         code,
         id,
         **kwargs
     ):
-        """Delete test suite.  # noqa: E501
+        """Delete test case.  # noqa: E501
 
-        This method completely deletes a test suite with test cases from repository.   # noqa: E501
+        This method completely deletes a test case from repository.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_suite(code, id, async_req=True)
+        >>> thread = api.delete_case(code, id, async_req=True)
         >>> result = thread.get()
 
         Args:
             code (str): Code of project, where to search entities.
             id (int): Identifier.
 
         Keyword Args:
-            suite_delete (SuiteDelete): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -556,29 +740,29 @@
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['code'] = \
             code
         kwargs['id'] = \
             id
-        return self.delete_suite_endpoint.call_with_http_info(**kwargs)
+        return self.delete_case_endpoint.call_with_http_info(**kwargs)
 
-    def get_suite(
+    def get_case(
         self,
         code,
         id,
         **kwargs
     ):
-        """Get a specific test suite.  # noqa: E501
+        """Get a specific test case.  # noqa: E501
 
-        This method allows to retrieve a specific test suite.   # noqa: E501
+        This method allows to retrieve a specific test case.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_suite(code, id, async_req=True)
+        >>> thread = api.get_case(code, id, async_req=True)
         >>> result = thread.get()
 
         Args:
             code (str): Code of project, where to search entities.
             id (int): Identifier.
 
         Keyword Args:
@@ -610,15 +794,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            SuiteResponse
+            TestCaseResponse
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -643,35 +827,43 @@
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['code'] = \
             code
         kwargs['id'] = \
             id
-        return self.get_suite_endpoint.call_with_http_info(**kwargs)
+        return self.get_case_endpoint.call_with_http_info(**kwargs)
 
-    def get_suites(
+    def get_cases(
         self,
         code,
         **kwargs
     ):
-        """Get all test suites.  # noqa: E501
+        """Get all test cases.  # noqa: E501
 
-        This method allows to retrieve all test suites stored in selected project.   # noqa: E501
+        This method allows to retrieve all test cases stored in selected project.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_suites(code, async_req=True)
+        >>> thread = api.get_cases(code, async_req=True)
         >>> result = thread.get()
 
         Args:
             code (str): Code of project, where to search entities.
 
         Keyword Args:
             search (str): Provide a string that will be used to search by name.. [optional]
+            milestone_id (int): ID of milestone.. [optional]
+            suite_id (int): ID of test suite.. [optional]
+            severity (str): A list of severity values separated by comma. Possible values: undefined, blocker, critical, major, normal, minor, trivial . [optional]
+            priority (str): A list of priority values separated by comma. Possible values: undefined, high, medium, low . [optional]
+            type (str): A list of type values separated by comma. Possible values: other, functional smoke, regression, security, usability, performance, acceptance . [optional]
+            behavior (str): A list of behavior values separated by comma. Possible values: undefined, positive negative, destructive . [optional]
+            automation (str): A list of values separated by comma. Possible values: is-not-automated, automated to-be-automated . [optional]
+            status (str): A list of values separated by comma. Possible values: actual, draft deprecated . [optional]
             limit (int): A number of entities in result set.. [optional] if omitted the server will use the default value of 10
             offset (int): How many entities should be skipped.. [optional] if omitted the server will use the default value of 0
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -698,15 +890,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            SuiteListResponse
+            TestCaseListResponse
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -729,36 +921,36 @@
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['code'] = \
             code
-        return self.get_suites_endpoint.call_with_http_info(**kwargs)
+        return self.get_cases_endpoint.call_with_http_info(**kwargs)
 
-    def update_suite(
+    def update_case(
         self,
         code,
         id,
-        suite_update,
+        test_case_update,
         **kwargs
     ):
-        """Update test suite.  # noqa: E501
+        """Update test case.  # noqa: E501
 
-        This method is used to update a test suite through API.   # noqa: E501
+        This method updates a test case.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_suite(code, id, suite_update, async_req=True)
+        >>> thread = api.update_case(code, id, test_case_update, async_req=True)
         >>> result = thread.get()
 
         Args:
             code (str): Code of project, where to search entities.
             id (int): Identifier.
-            suite_update (SuiteUpdate):
+            test_case_update (TestCaseUpdate):
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -818,11 +1010,11 @@
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['code'] = \
             code
         kwargs['id'] = \
             id
-        kwargs['suite_update'] = \
-            suite_update
-        return self.update_suite_endpoint.call_with_http_info(**kwargs)
+        kwargs['test_case_update'] = \
+            test_case_update
+        return self.update_case_endpoint.call_with_http_info(**kwargs)
```

### Comparing `qaseio-3.2.1/qaseio/api_client.py` & `qaseio-3.3.0/qaseio/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/3.2.1/python'
+        self.user_agent = 'OpenAPI-Generator/3.3.0/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `qaseio-3.2.1/qaseio/apis/__init__.py` & `qaseio-3.3.0/qaseio/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/configuration.py` & `qaseio-3.3.0/qaseio/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -406,15 +406,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0.0\n"\
-               "SDK Package Version: 3.2.1".\
+               "SDK Package Version: 3.3.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `qaseio-3.2.1/qaseio/exceptions.py` & `qaseio-3.3.0/qaseio/exceptions.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/attachment.py` & `qaseio-3.3.0/qaseio/model/attachment.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/attachment_get.py` & `qaseio-3.3.0/qaseio/model/attachment_get.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/attachment_hash.py` & `qaseio-3.3.0/qaseio/model/attachment_hash.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/attachment_hash_list.py` & `qaseio-3.3.0/qaseio/model/attachment_hash_list.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/attachment_list_response.py` & `qaseio-3.3.0/qaseio/model/attachment_list_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/attachment_list_response_all_of.py` & `qaseio-3.3.0/qaseio/model/attachment_list_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/attachment_list_response_all_of_result.py` & `qaseio-3.3.0/qaseio/model/attachment_list_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/attachment_response.py` & `qaseio-3.3.0/qaseio/model/attachment_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/attachment_response_all_of.py` & `qaseio-3.3.0/qaseio/model/attachment_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/attachment_uploads_response.py` & `qaseio-3.3.0/qaseio/model/attachment_uploads_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/attachment_uploads_response_all_of.py` & `qaseio-3.3.0/qaseio/model/attachment_uploads_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/author.py` & `qaseio-3.3.0/qaseio/model/author.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/author_list_response.py` & `qaseio-3.3.0/qaseio/model/author_list_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/author_list_response_all_of.py` & `qaseio-3.3.0/qaseio/model/author_list_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/author_list_response_all_of_result.py` & `qaseio-3.3.0/qaseio/model/author_list_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/author_response.py` & `qaseio-3.3.0/qaseio/model/author_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/author_response_all_of.py` & `qaseio-3.3.0/qaseio/model/author_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/create_result200_response.py` & `qaseio-3.3.0/qaseio/model/create_result200_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/create_result200_response_all_of.py` & `qaseio-3.3.0/qaseio/model/create_result200_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/create_result200_response_all_of_result.py` & `qaseio-3.3.0/qaseio/model/create_result200_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/custom_field.py` & `qaseio-3.3.0/qaseio/model/custom_field.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/custom_field_create.py` & `qaseio-3.3.0/qaseio/model/custom_field_create.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/custom_field_create_value_inner.py` & `qaseio-3.3.0/qaseio/model/custom_field_create_value_inner.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/custom_field_response.py` & `qaseio-3.3.0/qaseio/model/custom_field_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/custom_field_response_all_of.py` & `qaseio-3.3.0/qaseio/model/custom_field_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/custom_field_update.py` & `qaseio-3.3.0/qaseio/model/custom_field_update.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/custom_field_value.py` & `qaseio-3.3.0/qaseio/model/custom_field_value.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/custom_fields_response.py` & `qaseio-3.3.0/qaseio/model/custom_fields_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/custom_fields_response_all_of.py` & `qaseio-3.3.0/qaseio/model/custom_fields_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/custom_fields_response_all_of_result.py` & `qaseio-3.3.0/qaseio/model/custom_fields_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/defect.py` & `qaseio-3.3.0/qaseio/model/defect.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/defect_create.py` & `qaseio-3.3.0/qaseio/model/defect_create.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/defect_list_response.py` & `qaseio-3.3.0/qaseio/model/defect_list_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/defect_list_response_all_of.py` & `qaseio-3.3.0/qaseio/model/defect_list_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/defect_list_response_all_of_result.py` & `qaseio-3.3.0/qaseio/model/defect_list_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/defect_response.py` & `qaseio-3.3.0/qaseio/model/defect_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/defect_response_all_of.py` & `qaseio-3.3.0/qaseio/model/defect_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/defect_status.py` & `qaseio-3.3.0/qaseio/model/defect_status.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/defect_update.py` & `qaseio-3.3.0/qaseio/model/defect_update.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/environment.py` & `qaseio-3.3.0/qaseio/model/environment.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/environment_create.py` & `qaseio-3.3.0/qaseio/model/environment_create.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/environment_list_response.py` & `qaseio-3.3.0/qaseio/model/environment_list_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/environment_list_response_all_of.py` & `qaseio-3.3.0/qaseio/model/environment_list_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/environment_list_response_all_of_result.py` & `qaseio-3.3.0/qaseio/model/environment_list_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/environment_response.py` & `qaseio-3.3.0/qaseio/model/environment_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/environment_response_all_of.py` & `qaseio-3.3.0/qaseio/model/environment_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/environment_update.py` & `qaseio-3.3.0/qaseio/model/environment_update.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/hash_response.py` & `qaseio-3.3.0/qaseio/model/hash_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/hash_response_all_of.py` & `qaseio-3.3.0/qaseio/model/hash_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/hash_response_all_of_result.py` & `qaseio-3.3.0/qaseio/model/hash_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/id_response.py` & `qaseio-3.3.0/qaseio/model/id_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/id_response_all_of.py` & `qaseio-3.3.0/qaseio/model/id_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/id_response_all_of_result.py` & `qaseio-3.3.0/qaseio/model/id_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/milestone.py` & `qaseio-3.3.0/qaseio/model/milestone.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/milestone_create.py` & `qaseio-3.3.0/qaseio/model/milestone_create.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/milestone_list_response.py` & `qaseio-3.3.0/qaseio/model/milestone_list_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/milestone_list_response_all_of.py` & `qaseio-3.3.0/qaseio/model/milestone_list_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/milestone_list_response_all_of_result.py` & `qaseio-3.3.0/qaseio/model/milestone_list_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/milestone_response.py` & `qaseio-3.3.0/qaseio/model/milestone_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/milestone_response_all_of.py` & `qaseio-3.3.0/qaseio/model/milestone_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/milestone_update.py` & `qaseio-3.3.0/qaseio/model/milestone_update.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/plan.py` & `qaseio-3.3.0/qaseio/model/plan.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/plan_create.py` & `qaseio-3.3.0/qaseio/model/plan_create.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/plan_detailed.py` & `qaseio-3.3.0/qaseio/model/plan_detailed.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/plan_detailed_all_of.py` & `qaseio-3.3.0/qaseio/model/plan_detailed_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/plan_detailed_all_of_cases.py` & `qaseio-3.3.0/qaseio/model/plan_detailed_all_of_cases.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/plan_list_response.py` & `qaseio-3.3.0/qaseio/model/plan_list_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/plan_list_response_all_of.py` & `qaseio-3.3.0/qaseio/model/plan_list_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/plan_list_response_all_of_result.py` & `qaseio-3.3.0/qaseio/model/plan_list_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/plan_response.py` & `qaseio-3.3.0/qaseio/model/plan_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/plan_response_all_of.py` & `qaseio-3.3.0/qaseio/model/plan_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/plan_update.py` & `qaseio-3.3.0/qaseio/model/plan_update.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/project.py` & `qaseio-3.3.0/qaseio/model/project.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/project_access.py` & `qaseio-3.3.0/qaseio/model/project_access.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/project_code_response.py` & `qaseio-3.3.0/qaseio/model/project_code_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/project_code_response_all_of.py` & `qaseio-3.3.0/qaseio/model/project_code_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/project_code_response_all_of_result.py` & `qaseio-3.3.0/qaseio/model/project_code_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/project_counts.py` & `qaseio-3.3.0/qaseio/model/project_counts.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/project_counts_defects.py` & `qaseio-3.3.0/qaseio/model/project_counts_defects.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/project_counts_runs.py` & `qaseio-3.3.0/qaseio/model/project_counts_runs.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/project_create.py` & `qaseio-3.3.0/qaseio/model/project_create.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/project_list_response.py` & `qaseio-3.3.0/qaseio/model/project_list_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/project_list_response_all_of.py` & `qaseio-3.3.0/qaseio/model/project_list_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/project_list_response_all_of_result.py` & `qaseio-3.3.0/qaseio/model/project_list_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/project_response.py` & `qaseio-3.3.0/qaseio/model/project_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/project_response_all_of.py` & `qaseio-3.3.0/qaseio/model/project_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/qql_defect.py` & `qaseio-3.3.0/qaseio/model/qql_defect.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/qql_plan.py` & `qaseio-3.3.0/qaseio/model/qql_plan.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/qql_test_case.py` & `qaseio-3.3.0/qaseio/model/qql_test_case.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/requirement.py` & `qaseio-3.3.0/qaseio/model/requirement.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/response.py` & `qaseio-3.3.0/qaseio/model/response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/result.py` & `qaseio-3.3.0/qaseio/model/result.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/result_create.py` & `qaseio-3.3.0/qaseio/model/result_create.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/result_create_bulk.py` & `qaseio-3.3.0/qaseio/model/result_create_bulk.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/result_create_case.py` & `qaseio-3.3.0/qaseio/model/result_create_case.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,27 +81,31 @@
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'title': (str,),  # noqa: E501
             'suite_title': (str, none_type,),  # noqa: E501
             'description': (str, none_type,),  # noqa: E501
+            'preconditions': (str, none_type,),  # noqa: E501
+            'postconditions': (str, none_type,),  # noqa: E501
             'layer': (str,),  # noqa: E501
             'severity': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'title': 'title',  # noqa: E501
         'suite_title': 'suite_title',  # noqa: E501
         'description': 'description',  # noqa: E501
+        'preconditions': 'preconditions',  # noqa: E501
+        'postconditions': 'postconditions',  # noqa: E501
         'layer': 'layer',  # noqa: E501
         'severity': 'severity',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
@@ -142,14 +146,16 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             title (str): [optional]  # noqa: E501
             suite_title (str, none_type): Nested suites should be separated with `TAB` symbol.. [optional]  # noqa: E501
             description (str, none_type): [optional]  # noqa: E501
+            preconditions (str, none_type): [optional]  # noqa: E501
+            postconditions (str, none_type): [optional]  # noqa: E501
             layer (str): [optional]  # noqa: E501
             severity (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
@@ -232,14 +238,16 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             title (str): [optional]  # noqa: E501
             suite_title (str, none_type): Nested suites should be separated with `TAB` symbol.. [optional]  # noqa: E501
             description (str, none_type): [optional]  # noqa: E501
+            preconditions (str, none_type): [optional]  # noqa: E501
+            postconditions (str, none_type): [optional]  # noqa: E501
             layer (str): [optional]  # noqa: E501
             severity (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
```

### Comparing `qaseio-3.2.1/qaseio/model/result_list_response.py` & `qaseio-3.3.0/qaseio/model/result_list_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/result_list_response_all_of.py` & `qaseio-3.3.0/qaseio/model/result_list_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/result_list_response_all_of_result.py` & `qaseio-3.3.0/qaseio/model/result_list_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/result_response.py` & `qaseio-3.3.0/qaseio/model/result_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/result_response_all_of.py` & `qaseio-3.3.0/qaseio/model/result_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/result_update.py` & `qaseio-3.3.0/qaseio/model/result_update.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/run.py` & `qaseio-3.3.0/qaseio/model/run.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/run_create.py` & `qaseio-3.3.0/qaseio/model/run_create.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,14 +103,16 @@
             'cases': ([int],),  # noqa: E501
             'is_autotest': (bool,),  # noqa: E501
             'environment_id': (int,),  # noqa: E501
             'milestone_id': (int,),  # noqa: E501
             'plan_id': (int,),  # noqa: E501
             'tags': ([str],),  # noqa: E501
             'custom_field': ({str: (str,)},),  # noqa: E501
+            'start_time': (datetime,),  # noqa: E501
+            'end_time': (datetime,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -121,14 +123,16 @@
         'cases': 'cases',  # noqa: E501
         'is_autotest': 'is_autotest',  # noqa: E501
         'environment_id': 'environment_id',  # noqa: E501
         'milestone_id': 'milestone_id',  # noqa: E501
         'plan_id': 'plan_id',  # noqa: E501
         'tags': 'tags',  # noqa: E501
         'custom_field': 'custom_field',  # noqa: E501
+        'start_time': 'start_time',  # noqa: E501
+        'end_time': 'end_time',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -176,14 +180,16 @@
             cases ([int]): [optional]  # noqa: E501
             is_autotest (bool): [optional]  # noqa: E501
             environment_id (int): [optional]  # noqa: E501
             milestone_id (int): [optional]  # noqa: E501
             plan_id (int): [optional]  # noqa: E501
             tags ([str]): [optional]  # noqa: E501
             custom_field ({str: (str,)}): A map of custom fields values (id => value). [optional]  # noqa: E501
+            start_time (datetime): [optional]  # noqa: E501
+            end_time (datetime): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -274,14 +280,16 @@
             cases ([int]): [optional]  # noqa: E501
             is_autotest (bool): [optional]  # noqa: E501
             environment_id (int): [optional]  # noqa: E501
             milestone_id (int): [optional]  # noqa: E501
             plan_id (int): [optional]  # noqa: E501
             tags ([str]): [optional]  # noqa: E501
             custom_field ({str: (str,)}): A map of custom fields values (id => value). [optional]  # noqa: E501
+            start_time (datetime): [optional]  # noqa: E501
+            end_time (datetime): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `qaseio-3.2.1/qaseio/model/run_environment.py` & `qaseio-3.3.0/qaseio/model/run_environment.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/run_list_response.py` & `qaseio-3.3.0/qaseio/model/run_list_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/run_list_response_all_of.py` & `qaseio-3.3.0/qaseio/model/run_list_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/run_list_response_all_of_result.py` & `qaseio-3.3.0/qaseio/model/run_list_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/run_milestone.py` & `qaseio-3.3.0/qaseio/model/run_milestone.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/run_public.py` & `qaseio-3.3.0/qaseio/model/run_public.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/run_public_response.py` & `qaseio-3.3.0/qaseio/model/run_public_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/run_public_response_all_of.py` & `qaseio-3.3.0/qaseio/model/run_public_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/run_public_response_all_of_result.py` & `qaseio-3.3.0/qaseio/model/run_public_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/run_response.py` & `qaseio-3.3.0/qaseio/model/run_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/run_response_all_of.py` & `qaseio-3.3.0/qaseio/model/run_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/run_stats.py` & `qaseio-3.3.0/qaseio/model/run_stats.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/search_response.py` & `qaseio-3.3.0/qaseio/model/search_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/search_response_all_of.py` & `qaseio-3.3.0/qaseio/model/search_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/search_response_all_of_result.py` & `qaseio-3.3.0/qaseio/model/search_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/shared_step.py` & `qaseio-3.3.0/qaseio/model/shared_step.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/shared_step_content.py` & `qaseio-3.3.0/qaseio/model/shared_step_content.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/shared_step_content_create.py` & `qaseio-3.3.0/qaseio/model/shared_step_content_create.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/shared_step_create.py` & `qaseio-3.3.0/qaseio/model/shared_step_create.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/shared_step_list_response.py` & `qaseio-3.3.0/qaseio/model/shared_step_list_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/shared_step_list_response_all_of.py` & `qaseio-3.3.0/qaseio/model/shared_step_list_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/shared_step_list_response_all_of_result.py` & `qaseio-3.3.0/qaseio/model/shared_step_list_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/shared_step_response.py` & `qaseio-3.3.0/qaseio/model/shared_step_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/shared_step_response_all_of.py` & `qaseio-3.3.0/qaseio/model/shared_step_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/shared_step_update.py` & `qaseio-3.3.0/qaseio/model/shared_step_update.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/suite.py` & `qaseio-3.3.0/qaseio/model/suite.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/suite_create.py` & `qaseio-3.3.0/qaseio/model/suite_create.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/suite_delete.py` & `qaseio-3.3.0/qaseio/model/suite_delete.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/suite_list_response.py` & `qaseio-3.3.0/qaseio/model/suite_list_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/suite_list_response_all_of.py` & `qaseio-3.3.0/qaseio/model/suite_list_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/suite_list_response_all_of_result.py` & `qaseio-3.3.0/qaseio/model/suite_list_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/suite_response.py` & `qaseio-3.3.0/qaseio/model/suite_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/suite_response_all_of.py` & `qaseio-3.3.0/qaseio/model/suite_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/suite_update.py` & `qaseio-3.3.0/qaseio/model/suite_update.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/tag_value.py` & `qaseio-3.3.0/qaseio/model/tag_value.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/test_case.py` & `qaseio-3.3.0/qaseio/model/test_case.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/test_case_create.py` & `qaseio-3.3.0/qaseio/model/test_case_create.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,16 @@
             'automation': (int,),  # noqa: E501
             'status': (int,),  # noqa: E501
             'attachments': (AttachmentHashList,),  # noqa: E501
             'steps': ([TestStepCreate],),  # noqa: E501
             'tags': ([str],),  # noqa: E501
             'params': ({str: ([str],)}, none_type,),  # noqa: E501
             'custom_field': ({str: (str,)},),  # noqa: E501
+            'created_at': (datetime,),  # noqa: E501
+            'updated_at': (datetime,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -135,14 +137,16 @@
         'automation': 'automation',  # noqa: E501
         'status': 'status',  # noqa: E501
         'attachments': 'attachments',  # noqa: E501
         'steps': 'steps',  # noqa: E501
         'tags': 'tags',  # noqa: E501
         'params': 'params',  # noqa: E501
         'custom_field': 'custom_field',  # noqa: E501
+        'created_at': 'created_at',  # noqa: E501
+        'updated_at': 'updated_at',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -199,14 +203,16 @@
             automation (int): [optional]  # noqa: E501
             status (int): [optional]  # noqa: E501
             attachments (AttachmentHashList): [optional]  # noqa: E501
             steps ([TestStepCreate]): [optional]  # noqa: E501
             tags ([str]): [optional]  # noqa: E501
             params ({str: ([str],)}, none_type): [optional]  # noqa: E501
             custom_field ({str: (str,)}): A map of custom fields values (id => value). [optional]  # noqa: E501
+            created_at (datetime): [optional]  # noqa: E501
+            updated_at (datetime): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -306,14 +312,16 @@
             automation (int): [optional]  # noqa: E501
             status (int): [optional]  # noqa: E501
             attachments (AttachmentHashList): [optional]  # noqa: E501
             steps ([TestStepCreate]): [optional]  # noqa: E501
             tags ([str]): [optional]  # noqa: E501
             params ({str: ([str],)}, none_type): [optional]  # noqa: E501
             custom_field ({str: (str,)}): A map of custom fields values (id => value). [optional]  # noqa: E501
+            created_at (datetime): [optional]  # noqa: E501
+            updated_at (datetime): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `qaseio-3.2.1/qaseio/model/test_case_list_response.py` & `qaseio-3.3.0/qaseio/model/test_case_list_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/test_case_list_response_all_of.py` & `qaseio-3.3.0/qaseio/model/test_case_list_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/test_case_list_response_all_of_result.py` & `qaseio-3.3.0/qaseio/model/test_case_list_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/test_case_params.py` & `qaseio-3.3.0/qaseio/model/test_case_params.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/test_case_response.py` & `qaseio-3.3.0/qaseio/model/test_case_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/test_case_response_all_of.py` & `qaseio-3.3.0/qaseio/model/test_case_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/test_case_update.py` & `qaseio-3.3.0/qaseio/model/test_case_update.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/test_step.py` & `qaseio-3.3.0/qaseio/model/test_step.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/test_step_create.py` & `qaseio-3.3.0/qaseio/model/test_step_create.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/test_step_result.py` & `qaseio-3.3.0/qaseio/model/test_step_result.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model/test_step_result_create.py` & `qaseio-3.3.0/qaseio/model/test_step_result_create.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/model_utils.py` & `qaseio-3.3.0/qaseio/model_utils.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/qaseio/models/__init__.py` & `qaseio-3.3.0/qaseio/models/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,20 @@
 from qaseio.model.attachment_uploads_response_all_of import AttachmentUploadsResponseAllOf
 from qaseio.model.author import Author
 from qaseio.model.author_list_response import AuthorListResponse
 from qaseio.model.author_list_response_all_of import AuthorListResponseAllOf
 from qaseio.model.author_list_response_all_of_result import AuthorListResponseAllOfResult
 from qaseio.model.author_response import AuthorResponse
 from qaseio.model.author_response_all_of import AuthorResponseAllOf
+from qaseio.model.bulk200_response import Bulk200Response
+from qaseio.model.bulk200_response_all_of import Bulk200ResponseAllOf
+from qaseio.model.bulk200_response_all_of_result import Bulk200ResponseAllOfResult
+from qaseio.model.bulk_request import BulkRequest
+from qaseio.model.bulk_request_cases_inner import BulkRequestCasesInner
+from qaseio.model.bulk_request_cases_inner_all_of import BulkRequestCasesInnerAllOf
 from qaseio.model.create_result200_response import CreateResult200Response
 from qaseio.model.create_result200_response_all_of import CreateResult200ResponseAllOf
 from qaseio.model.create_result200_response_all_of_result import CreateResult200ResponseAllOfResult
 from qaseio.model.custom_field import CustomField
 from qaseio.model.custom_field_create import CustomFieldCreate
 from qaseio.model.custom_field_create_value_inner import CustomFieldCreateValueInner
 from qaseio.model.custom_field_response import CustomFieldResponse
```

### Comparing `qaseio-3.2.1/qaseio/rest.py` & `qaseio-3.3.0/qaseio/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         self.urllib3_response = resp
         self.status = resp.status
         self.reason = resp.reason
         self.data = resp.data
 
     def getheaders(self):
         """Returns a dictionary of the response headers."""
-        return self.urllib3_response.headers.get()
+        return self.urllib3_response.headers
 
     def getheader(self, name, default=None):
         """Returns a given response header."""
         return self.urllib3_response.headers.get(name, default)
 
 
 class RESTClientObject(object):
```

### Comparing `qaseio-3.2.1/qaseio.egg-info/SOURCES.txt` & `qaseio-3.3.0/qaseio.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,20 @@
 qaseio/model/attachment_uploads_response_all_of.py
 qaseio/model/author.py
 qaseio/model/author_list_response.py
 qaseio/model/author_list_response_all_of.py
 qaseio/model/author_list_response_all_of_result.py
 qaseio/model/author_response.py
 qaseio/model/author_response_all_of.py
+qaseio/model/bulk200_response.py
+qaseio/model/bulk200_response_all_of.py
+qaseio/model/bulk200_response_all_of_result.py
+qaseio/model/bulk_request.py
+qaseio/model/bulk_request_cases_inner.py
+qaseio/model/bulk_request_cases_inner_all_of.py
 qaseio/model/create_result200_response.py
 qaseio/model/create_result200_response_all_of.py
 qaseio/model/create_result200_response_all_of_result.py
 qaseio/model/custom_field.py
 qaseio/model/custom_field_create.py
 qaseio/model/custom_field_create_value_inner.py
 qaseio/model/custom_field_response.py
@@ -196,14 +202,20 @@
 test/test_author.py
 test/test_author_list_response.py
 test/test_author_list_response_all_of.py
 test/test_author_list_response_all_of_result.py
 test/test_author_response.py
 test/test_author_response_all_of.py
 test/test_authors_api.py
+test/test_bulk200_response.py
+test/test_bulk200_response_all_of.py
+test/test_bulk200_response_all_of_result.py
+test/test_bulk_request.py
+test/test_bulk_request_cases_inner.py
+test/test_bulk_request_cases_inner_all_of.py
 test/test_cases_api.py
 test/test_create_result200_response.py
 test/test_create_result200_response_all_of.py
 test/test_create_result200_response_all_of_result.py
 test/test_custom_field.py
 test/test_custom_field_create.py
 test/test_custom_field_create_value_inner.py
```

### Comparing `qaseio-3.2.1/setup.py` & `qaseio-3.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "qaseio"
-VERSION = "3.2.1"
+VERSION = "3.3.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 
@@ -28,15 +28,15 @@
 setup(
     name=NAME,
     version=VERSION,
     description="Qase TestOps API",
     author="Qase.io",
     author_email="support@qase.io",
     url="https://github.com/qase-tms/qase-python",
-    keywords=["OpenAPI", "OpenAPI-Generator", "Qase.io API"],
+    keywords=["OpenAPI", "OpenAPI-Generator", "Qase TestOps API"],
     python_requires=">=3.6",
     install_requires=REQUIRES,
     packages=find_packages(exclude=["test", "tests"]),
     include_package_data=True,
     license="Apache 2.0",
     long_description="""\
     Qase TestOps API client.  # noqa: E501
```

### Comparing `qaseio-3.2.1/test/test_attachment.py` & `qaseio-3.3.0/test/test_attachment.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_attachment_get.py` & `qaseio-3.3.0/test/test_attachment_get.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_attachment_hash.py` & `qaseio-3.3.0/test/test_attachment_hash.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_attachment_hash_list.py` & `qaseio-3.3.0/test/test_attachment_hash_list.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_attachment_list_response.py` & `qaseio-3.3.0/test/test_attachment_list_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_attachment_list_response_all_of.py` & `qaseio-3.3.0/test/test_attachment_list_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_attachment_list_response_all_of_result.py` & `qaseio-3.3.0/test/test_attachment_list_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_attachment_response.py` & `qaseio-3.3.0/test/test_attachment_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_attachment_response_all_of.py` & `qaseio-3.3.0/test/test_attachment_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_attachment_uploads_response.py` & `qaseio-3.3.0/test/test_attachment_uploads_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_attachment_uploads_response_all_of.py` & `qaseio-3.3.0/test/test_attachment_uploads_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_attachments_api.py` & `qaseio-3.3.0/test/test_attachments_api.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_author.py` & `qaseio-3.3.0/test/test_author.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_author_list_response.py` & `qaseio-3.3.0/test/test_author_list_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_author_list_response_all_of.py` & `qaseio-3.3.0/test/test_author_list_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_author_list_response_all_of_result.py` & `qaseio-3.3.0/test/test_author_list_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_author_response.py` & `qaseio-3.3.0/test/test_author_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_author_response_all_of.py` & `qaseio-3.3.0/test/test_author_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_authors_api.py` & `qaseio-3.3.0/test/test_authors_api.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_cases_api.py` & `qaseio-3.3.0/test/test_cases_api.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_create_result200_response.py` & `qaseio-3.3.0/test/test_create_result200_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_create_result200_response_all_of.py` & `qaseio-3.3.0/test/test_create_result200_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_create_result200_response_all_of_result.py` & `qaseio-3.3.0/test/test_create_result200_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_custom_field.py` & `qaseio-3.3.0/test/test_custom_field.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_custom_field_create.py` & `qaseio-3.3.0/test/test_custom_field_create.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_custom_field_create_value_inner.py` & `qaseio-3.3.0/test/test_custom_field_create_value_inner.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_custom_field_response.py` & `qaseio-3.3.0/test/test_custom_field_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_custom_field_response_all_of.py` & `qaseio-3.3.0/test/test_custom_field_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_custom_field_update.py` & `qaseio-3.3.0/test/test_custom_field_update.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_custom_field_value.py` & `qaseio-3.3.0/test/test_custom_field_value.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_custom_fields_api.py` & `qaseio-3.3.0/test/test_custom_fields_api.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_custom_fields_response.py` & `qaseio-3.3.0/test/test_custom_fields_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_custom_fields_response_all_of.py` & `qaseio-3.3.0/test/test_custom_fields_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_custom_fields_response_all_of_result.py` & `qaseio-3.3.0/test/test_custom_fields_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_defect.py` & `qaseio-3.3.0/test/test_defect.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_defect_create.py` & `qaseio-3.3.0/test/test_defect_create.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_defect_list_response.py` & `qaseio-3.3.0/test/test_defect_list_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_defect_list_response_all_of.py` & `qaseio-3.3.0/test/test_defect_list_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_defect_list_response_all_of_result.py` & `qaseio-3.3.0/test/test_defect_list_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_defect_response.py` & `qaseio-3.3.0/test/test_defect_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_defect_response_all_of.py` & `qaseio-3.3.0/test/test_defect_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_defect_status.py` & `qaseio-3.3.0/test/test_defect_status.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_defect_update.py` & `qaseio-3.3.0/test/test_defect_update.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_defects_api.py` & `qaseio-3.3.0/test/test_defects_api.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_environment.py` & `qaseio-3.3.0/test/test_environment.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_environment_create.py` & `qaseio-3.3.0/test/test_environment_create.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_environment_list_response.py` & `qaseio-3.3.0/test/test_environment_list_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_environment_list_response_all_of.py` & `qaseio-3.3.0/test/test_environment_list_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_environment_list_response_all_of_result.py` & `qaseio-3.3.0/test/test_environment_list_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_environment_response.py` & `qaseio-3.3.0/test/test_environment_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_environment_response_all_of.py` & `qaseio-3.3.0/test/test_environment_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_environment_update.py` & `qaseio-3.3.0/test/test_environment_update.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_environments_api.py` & `qaseio-3.3.0/test/test_environments_api.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_hash_response.py` & `qaseio-3.3.0/test/test_hash_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_hash_response_all_of.py` & `qaseio-3.3.0/test/test_hash_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_hash_response_all_of_result.py` & `qaseio-3.3.0/test/test_hash_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_id_response.py` & `qaseio-3.3.0/test/test_id_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_id_response_all_of.py` & `qaseio-3.3.0/test/test_id_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_id_response_all_of_result.py` & `qaseio-3.3.0/test/test_id_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_milestone.py` & `qaseio-3.3.0/test/test_milestone.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_milestone_create.py` & `qaseio-3.3.0/test/test_milestone_create.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_milestone_list_response.py` & `qaseio-3.3.0/test/test_milestone_list_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_milestone_list_response_all_of.py` & `qaseio-3.3.0/test/test_milestone_list_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_milestone_list_response_all_of_result.py` & `qaseio-3.3.0/test/test_milestone_list_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_milestone_response.py` & `qaseio-3.3.0/test/test_milestone_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_milestone_response_all_of.py` & `qaseio-3.3.0/test/test_milestone_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_milestone_update.py` & `qaseio-3.3.0/test/test_milestone_update.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_milestones_api.py` & `qaseio-3.3.0/test/test_milestones_api.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_plan.py` & `qaseio-3.3.0/test/test_plan.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_plan_create.py` & `qaseio-3.3.0/test/test_plan_create.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_plan_detailed.py` & `qaseio-3.3.0/test/test_plan_detailed.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_plan_detailed_all_of.py` & `qaseio-3.3.0/test/test_plan_detailed_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_plan_detailed_all_of_cases.py` & `qaseio-3.3.0/test/test_plan_detailed_all_of_cases.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_plan_list_response.py` & `qaseio-3.3.0/test/test_plan_list_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_plan_list_response_all_of.py` & `qaseio-3.3.0/test/test_plan_list_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_plan_list_response_all_of_result.py` & `qaseio-3.3.0/test/test_plan_list_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_plan_response.py` & `qaseio-3.3.0/test/test_plan_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_plan_response_all_of.py` & `qaseio-3.3.0/test/test_plan_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_plan_update.py` & `qaseio-3.3.0/test/test_plan_update.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_plans_api.py` & `qaseio-3.3.0/test/test_plans_api.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_project.py` & `qaseio-3.3.0/test/test_project.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_project_access.py` & `qaseio-3.3.0/test/test_project_access.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_project_code_response.py` & `qaseio-3.3.0/test/test_project_code_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_project_code_response_all_of.py` & `qaseio-3.3.0/test/test_project_code_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_project_code_response_all_of_result.py` & `qaseio-3.3.0/test/test_project_code_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_project_counts.py` & `qaseio-3.3.0/test/test_project_counts.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_project_counts_defects.py` & `qaseio-3.3.0/test/test_project_counts_defects.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_project_counts_runs.py` & `qaseio-3.3.0/test/test_project_counts_runs.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_project_create.py` & `qaseio-3.3.0/test/test_project_create.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_project_list_response.py` & `qaseio-3.3.0/test/test_project_list_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_project_list_response_all_of.py` & `qaseio-3.3.0/test/test_project_list_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_project_list_response_all_of_result.py` & `qaseio-3.3.0/test/test_project_list_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_project_response.py` & `qaseio-3.3.0/test/test_project_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_project_response_all_of.py` & `qaseio-3.3.0/test/test_project_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_projects_api.py` & `qaseio-3.3.0/test/test_projects_api.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_qql_defect.py` & `qaseio-3.3.0/test/test_qql_defect.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_qql_plan.py` & `qaseio-3.3.0/test/test_qql_plan.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_qql_test_case.py` & `qaseio-3.3.0/test/test_qql_test_case.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_requirement.py` & `qaseio-3.3.0/test/test_requirement.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_response.py` & `qaseio-3.3.0/test/test_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_result.py` & `qaseio-3.3.0/test/test_result.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_result_create.py` & `qaseio-3.3.0/test/test_result_create.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_result_create_bulk.py` & `qaseio-3.3.0/test/test_result_create_bulk.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_result_create_case.py` & `qaseio-3.3.0/test/test_result_create_case.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_result_list_response.py` & `qaseio-3.3.0/test/test_result_list_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_result_list_response_all_of.py` & `qaseio-3.3.0/test/test_result_list_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_result_list_response_all_of_result.py` & `qaseio-3.3.0/test/test_result_list_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_result_response.py` & `qaseio-3.3.0/test/test_result_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_result_response_all_of.py` & `qaseio-3.3.0/test/test_result_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_result_update.py` & `qaseio-3.3.0/test/test_result_update.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_results_api.py` & `qaseio-3.3.0/test/test_results_api.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_run.py` & `qaseio-3.3.0/test/test_run.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_run_create.py` & `qaseio-3.3.0/test/test_run_create.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_run_environment.py` & `qaseio-3.3.0/test/test_run_environment.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_run_list_response.py` & `qaseio-3.3.0/test/test_run_list_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_run_list_response_all_of.py` & `qaseio-3.3.0/test/test_run_list_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_run_list_response_all_of_result.py` & `qaseio-3.3.0/test/test_run_list_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_run_milestone.py` & `qaseio-3.3.0/test/test_run_milestone.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_run_public.py` & `qaseio-3.3.0/test/test_run_public.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_run_public_response.py` & `qaseio-3.3.0/test/test_run_public_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_run_public_response_all_of.py` & `qaseio-3.3.0/test/test_run_public_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_run_public_response_all_of_result.py` & `qaseio-3.3.0/test/test_run_public_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_run_response.py` & `qaseio-3.3.0/test/test_run_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_run_response_all_of.py` & `qaseio-3.3.0/test/test_run_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_run_stats.py` & `qaseio-3.3.0/test/test_run_stats.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_runs_api.py` & `qaseio-3.3.0/test/test_runs_api.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_search_api.py` & `qaseio-3.3.0/test/test_search_api.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_search_response.py` & `qaseio-3.3.0/test/test_search_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_search_response_all_of.py` & `qaseio-3.3.0/test/test_search_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_search_response_all_of_result.py` & `qaseio-3.3.0/test/test_search_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_shared_step.py` & `qaseio-3.3.0/test/test_shared_step.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_shared_step_content.py` & `qaseio-3.3.0/test/test_shared_step_content.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_shared_step_content_create.py` & `qaseio-3.3.0/test/test_shared_step_content_create.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_shared_step_create.py` & `qaseio-3.3.0/test/test_shared_step_create.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_shared_step_list_response.py` & `qaseio-3.3.0/test/test_shared_step_list_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_shared_step_list_response_all_of.py` & `qaseio-3.3.0/test/test_shared_step_list_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_shared_step_list_response_all_of_result.py` & `qaseio-3.3.0/test/test_shared_step_list_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_shared_step_response.py` & `qaseio-3.3.0/test/test_shared_step_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_shared_step_response_all_of.py` & `qaseio-3.3.0/test/test_shared_step_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_shared_step_update.py` & `qaseio-3.3.0/test/test_shared_step_update.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_shared_steps_api.py` & `qaseio-3.3.0/test/test_shared_steps_api.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_suite.py` & `qaseio-3.3.0/test/test_suite.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_suite_create.py` & `qaseio-3.3.0/test/test_suite_create.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_suite_delete.py` & `qaseio-3.3.0/test/test_suite_delete.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_suite_list_response.py` & `qaseio-3.3.0/test/test_suite_list_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_suite_list_response_all_of.py` & `qaseio-3.3.0/test/test_suite_list_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_suite_list_response_all_of_result.py` & `qaseio-3.3.0/test/test_suite_list_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_suite_response.py` & `qaseio-3.3.0/test/test_suite_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_suite_response_all_of.py` & `qaseio-3.3.0/test/test_suite_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_suite_update.py` & `qaseio-3.3.0/test/test_suite_update.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_suites_api.py` & `qaseio-3.3.0/test/test_suites_api.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_tag_value.py` & `qaseio-3.3.0/test/test_tag_value.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_test_case.py` & `qaseio-3.3.0/test/test_test_case.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_test_case_create.py` & `qaseio-3.3.0/test/test_test_case_create.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_test_case_list_response.py` & `qaseio-3.3.0/test/test_test_case_list_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_test_case_list_response_all_of.py` & `qaseio-3.3.0/test/test_test_case_list_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_test_case_list_response_all_of_result.py` & `qaseio-3.3.0/test/test_test_case_list_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_test_case_params.py` & `qaseio-3.3.0/test/test_test_case_params.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_test_case_response.py` & `qaseio-3.3.0/test/test_test_case_response.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_test_case_response_all_of.py` & `qaseio-3.3.0/test/test_test_case_response_all_of.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_test_case_update.py` & `qaseio-3.3.0/test/test_test_case_update.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_test_step.py` & `qaseio-3.3.0/test/test_test_step.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_test_step_create.py` & `qaseio-3.3.0/test/test_test_step_create.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_test_step_result.py` & `qaseio-3.3.0/test/test_test_step_result.py`

 * *Files identical despite different names*

### Comparing `qaseio-3.2.1/test/test_test_step_result_create.py` & `qaseio-3.3.0/test/test_test_step_result_create.py`

 * *Files identical despite different names*

