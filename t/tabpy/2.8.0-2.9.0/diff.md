# Comparing `tmp/tabpy-2.8.0.tar.gz` & `tmp/tabpy-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabpy-2.8.0.tar", last modified: Tue May 23 12:42:09 2023, max compression
+gzip compressed data, was "tabpy-2.9.0.tar", last modified: Wed Jun 21 21:32:07 2023, max compression
```

## Comparing `tabpy-2.8.0.tar` & `tabpy-2.9.0.tar`

### file list

```diff
@@ -1,170 +1,170 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 12:42:09.526171 tabpy-2.8.0/
-drwxrwxrwx   0        0        0        0 2023-05-23 12:42:08.411565 tabpy-2.8.0/.github/
-drwxrwxrwx   0        0        0        0 2023-05-23 12:42:08.613079 tabpy-2.8.0/.github/ISSUE_TEMPLATE/
--rw-rw-rw-   0        0        0      715 2023-05-02 13:24:30.000000 tabpy-2.8.0/.github/ISSUE_TEMPLATE/tabpy-issue-report.md
-drwxrwxrwx   0        0        0        0 2023-05-23 12:42:08.613079 tabpy-2.8.0/.github/PULL_REQUEST_TEMPLATE/
--rw-rw-rw-   0        0        0     1400 2023-05-02 13:24:30.000000 tabpy-2.8.0/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
-drwxrwxrwx   0        0        0        0 2023-05-23 12:42:08.659955 tabpy-2.8.0/.github/workflows/
--rw-rw-rw-   0        0        0      971 2023-05-02 13:24:30.000000 tabpy-2.8.0/.github/workflows/coverage.yml
--rw-rw-rw-   0        0        0     1439 2023-05-02 13:24:30.000000 tabpy-2.8.0/.github/workflows/docker-publish.yml
--rw-rw-rw-   0        0        0     1138 2023-05-02 13:24:30.000000 tabpy-2.8.0/.github/workflows/lint.yml
--rw-rw-rw-   0        0        0      758 2023-05-02 13:24:30.000000 tabpy-2.8.0/.github/workflows/pull_request.yml
--rw-rw-rw-   0        0        0      752 2023-05-02 13:24:30.000000 tabpy-2.8.0/.github/workflows/push.yml
--rw-rw-rw-   0        0        0     1659 2023-05-02 13:24:30.000000 tabpy-2.8.0/.gitignore
--rw-rw-rw-   0        0        0       66 2023-05-02 13:24:30.000000 tabpy-2.8.0/.pep8speaks.yml
--rw-rw-rw-   0        0        0      831 2023-05-02 13:24:30.000000 tabpy-2.8.0/.scrutinizer.yml
--rw-rw-rw-   0        0        0     5351 2023-05-23 12:40:10.000000 tabpy-2.8.0/CHANGELOG
--rw-rw-rw-   0        0        0     3969 2023-05-02 13:24:30.000000 tabpy-2.8.0/CONTRIBUTING.md
--rw-rw-rw-   0        0        0      272 2023-05-02 13:24:30.000000 tabpy-2.8.0/Dockerfile
--rw-rw-rw-   0        0        0     1099 2023-05-02 13:24:30.000000 tabpy-2.8.0/LICENSE
--rw-rw-rw-   0        0        0      549 2023-05-02 13:24:30.000000 tabpy-2.8.0/MANIFEST.in
--rw-rw-rw-   0        0        0     6907 2023-05-23 12:42:09.526171 tabpy-2.8.0/PKG-INFO
--rw-rw-rw-   0        0        0      131 2023-05-02 13:24:30.000000 tabpy-2.8.0/Procfile
--rw-rw-rw-   0        0        0     3334 2023-05-02 13:24:30.000000 tabpy-2.8.0/README.md
--rw-rw-rw-   0        0        0       27 2023-05-02 13:24:30.000000 tabpy-2.8.0/_config.yml
--rw-rw-rw-   0        0        0      765 2023-05-02 13:24:30.000000 tabpy-2.8.0/app.json
--rw-rw-rw-   0        0        0     2523 2023-05-02 13:24:30.000000 tabpy-2.8.0/codeql-analysis.yml
-drwxrwxrwx   0        0        0        0 2023-05-23 12:42:08.722367 tabpy-2.8.0/docs/
--rw-rw-rw-   0        0        0     7688 2023-05-02 13:24:30.000000 tabpy-2.8.0/docs/TableauConfiguration.md
--rw-rw-rw-   0        0        0      887 2023-05-02 13:24:30.000000 tabpy-2.8.0/docs/about.md
--rw-rw-rw-   0        0        0      426 2023-05-02 13:24:30.000000 tabpy-2.8.0/docs/deploy-to-heroku.md
-drwxrwxrwx   0        0        0        0 2023-05-23 12:42:08.738080 tabpy-2.8.0/docs/img/
--rw-rw-rw-   0        0        0   136889 2023-05-02 13:24:30.000000 tabpy-2.8.0/docs/img/Example1-SimpleFunctionCall.png
--rw-rw-rw-   0        0        0   188230 2023-05-02 13:24:30.000000 tabpy-2.8.0/docs/img/Example2-MultipleFunctionCalls.png
--rw-rw-rw-   0        0        0    43399 2023-05-02 13:24:30.000000 tabpy-2.8.0/docs/img/python-calculated-field.png
--rw-rw-rw-   0        0        0     1229 2023-05-02 13:24:30.000000 tabpy-2.8.0/docs/security.md
--rw-rw-rw-   0        0        0    13360 2023-05-02 13:24:30.000000 tabpy-2.8.0/docs/server-config.md
--rw-rw-rw-   0        0        0     1422 2023-05-02 13:24:30.000000 tabpy-2.8.0/docs/server-install.md
--rw-rw-rw-   0        0        0     4268 2023-05-02 13:24:30.000000 tabpy-2.8.0/docs/server-rest.md
--rw-rw-rw-   0        0        0    17022 2023-05-02 13:24:30.000000 tabpy-2.8.0/docs/tabpy-tools.md
--rw-rw-rw-   0        0        0     2174 2023-05-02 13:24:30.000000 tabpy-2.8.0/docs/tabpy-virtualenv.md
-drwxrwxrwx   0        0        0        0 2023-05-23 12:42:08.753703 tabpy-2.8.0/misc/
--rw-rw-rw-   0        0        0     3747 2023-05-02 13:24:30.000000 tabpy-2.8.0/misc/TabPy.postman_collection.json
--rw-rw-rw-   0        0        0     7855 2023-05-02 13:24:30.000000 tabpy-2.8.0/misc/TabPy.yml
--rw-rw-rw-   0        0        0       90 2023-05-02 13:24:30.000000 tabpy-2.8.0/requirements.txt
--rw-rw-rw-   0        0        0        6 2023-05-02 13:24:30.000000 tabpy-2.8.0/requirements_dev.txt
--rw-rw-rw-   0        0        0      337 2023-05-23 12:42:09.526171 tabpy-2.8.0/setup.cfg
--rw-rw-rw-   0        0        0     3708 2023-05-02 13:24:30.000000 tabpy-2.8.0/setup.py
--rw-rw-rw-   0        0        0      512 2023-05-02 13:24:30.000000 tabpy-2.8.0/start.sh
-drwxrwxrwx   0        0        0        0 2023-05-23 12:42:08.769235 tabpy-2.8.0/tabpy/
--rw-rw-rw-   0        0        0        7 2023-05-23 12:40:10.000000 tabpy-2.8.0/tabpy/VERSION
--rw-rw-rw-   0        0        0        0 2023-05-02 13:24:30.000000 tabpy-2.8.0/tabpy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 12:42:08.831833 tabpy-2.8.0/tabpy/models/
--rw-rw-rw-   0        0        0        0 2023-05-02 13:24:30.000000 tabpy-2.8.0/tabpy/models/__init__.py
--rw-rw-rw-   0        0        0      820 2023-05-02 13:24:30.000000 tabpy-2.8.0/tabpy/models/deploy_models.py
-drwxrwxrwx   0        0        0        0 2023-05-23 12:42:08.863090 tabpy-2.8.0/tabpy/models/scripts/
--rw-rw-rw-   0        0        0      715 2023-05-02 13:24:30.000000 tabpy-2.8.0/tabpy/models/scripts/ANOVA.py
--rw-rw-rw-   0        0        0     2258 2023-05-02 13:24:30.000000 tabpy-2.8.0/tabpy/models/scripts/PCA.py
--rw-rw-rw-   0        0        0     1476 2023-05-02 13:24:30.000000 tabpy-2.8.0/tabpy/models/scripts/SentimentAnalysis.py
--rw-rw-rw-   0        0        0        0 2023-05-02 13:24:30.000000 tabpy-2.8.0/tabpy/models/scripts/__init__.py
--rw-rw-rw-   0        0        0     1416 2023-05-02 13:24:30.000000 tabpy-2.8.0/tabpy/models/scripts/tTest.py
-drwxrwxrwx   0        0        0        0 2023-05-23 12:42:08.878705 tabpy-2.8.0/tabpy/models/utils/
--rw-rw-rw-   0        0        0        0 2023-05-02 13:24:30.000000 tabpy-2.8.0/tabpy/models/utils/__init__.py
--rw-rw-rw-   0        0        0     1789 2023-05-02 13:24:30.000000 tabpy-2.8.0/tabpy/models/utils/setup_utils.py
--rw-rw-rw-   0        0        0      889 2023-05-02 13:24:30.000000 tabpy-2.8.0/tabpy/tabpy.py
-drwxrwxrwx   0        0        0        0 2023-05-23 12:42:08.894383 tabpy-2.8.0/tabpy/tabpy_server/
--rw-rw-rw-   0        0        0        0 2023-05-02 13:24:30.000000 tabpy-2.8.0/tabpy/tabpy_server/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 12:42:08.925580 tabpy-2.8.0/tabpy/tabpy_server/app/
--rw-rw-rw-   0        0        0        0 2023-05-02 13:24:30.000000 tabpy-2.8.0/tabpy/tabpy_server/app/__init__.py
--rw-rw-rw-   0        0        0    20759 2023-05-23 12:40:10.000000 tabpy-2.8.0/tabpy/tabpy_server/app/app.py
--rw-rw-rw-   0        0        0     1560 2023-05-02 13:24:30.000000 tabpy-2.8.0/tabpy/tabpy_server/app/app_parameters.py
--rw-rw-rw-   0        0        0     5396 2023-05-02 13:24:30.000000 tabpy-2.8.0/tabpy/tabpy_server/app/arrow_server.py
--rw-rw-rw-   0        0        0     2723 2023-05-02 13:24:30.000000 tabpy-2.8.0/tabpy/tabpy_server/app/util.py
-drwxrwxrwx   0        0        0        0 2023-05-23 12:42:08.956884 tabpy-2.8.0/tabpy/tabpy_server/common/
--rw-rw-rw-   0        0        0        0 2023-05-02 13:24:30.000000 tabpy-2.8.0/tabpy/tabpy_server/common/__init__.py
--rw-rw-rw-   0        0        0     1985 2023-05-02 13:24:30.000000 tabpy-2.8.0/tabpy/tabpy_server/common/default.conf
--rw-rw-rw-   0        0        0     3010 2023-05-02 13:24:30.000000 tabpy-2.8.0/tabpy/tabpy_server/common/endpoint_file_mgr.py
--rw-rw-rw-   0        0        0     3828 2023-05-02 13:24:30.000000 tabpy-2.8.0/tabpy/tabpy_server/common/messages.py
--rw-rw-rw-   0        0        0      107 2023-05-02 13:24:30.000000 tabpy-2.8.0/tabpy/tabpy_server/common/util.py
-drwxrwxrwx   0        0        0        0 2023-05-23 12:42:09.069768 tabpy-2.8.0/tabpy/tabpy_server/handlers/
--rw-rw-rw-   0        0        0     1014 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_server/handlers/__init__.py
--rw-rw-rw-   0        0        0    16470 2023-05-23 12:40:10.000000 tabpy-2.8.0/tabpy/tabpy_server/handlers/base_handler.py
--rw-rw-rw-   0        0        0     1735 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_server/handlers/basic_auth_server_middleware_factory.py
--rw-rw-rw-   0        0        0     5068 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_server/handlers/endpoint_handler.py
--rw-rw-rw-   0        0        0     2598 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_server/handlers/endpoints_handler.py
--rw-rw-rw-   0        0        0     8376 2023-05-23 12:40:10.000000 tabpy-2.8.0/tabpy/tabpy_server/handlers/evaluation_plane_handler.py
--rw-rw-rw-   0        0        0     5840 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_server/handlers/management_handler.py
--rw-rw-rw-   0        0        0      211 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_server/handlers/no_op_auth_handler.py
--rw-rw-rw-   0        0        0     8448 2023-05-23 12:40:10.000000 tabpy-2.8.0/tabpy/tabpy_server/handlers/query_plane_handler.py
--rw-rw-rw-   0        0        0      998 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_server/handlers/service_info_handler.py
--rw-rw-rw-   0        0        0      921 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_server/handlers/status_handler.py
--rw-rw-rw-   0        0        0      721 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_server/handlers/upload_destination_handler.py
--rw-rw-rw-   0        0        0     1005 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_server/handlers/util.py
-drwxrwxrwx   0        0        0        0 2023-05-23 12:42:09.085290 tabpy-2.8.0/tabpy/tabpy_server/management/
--rw-rw-rw-   0        0        0        0 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_server/management/__init__.py
--rw-rw-rw-   0        0        0    21331 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_server/management/state.py
--rw-rw-rw-   0        0        0     1524 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_server/management/util.py
-drwxrwxrwx   0        0        0        0 2023-05-23 12:42:09.116642 tabpy-2.8.0/tabpy/tabpy_server/psws/
--rw-rw-rw-   0        0        0        0 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_server/psws/__init__.py
--rw-rw-rw-   0        0        0     7364 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_server/psws/callbacks.py
--rw-rw-rw-   0        0        0     9732 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_server/psws/python_service.py
--rw-rw-rw-   0        0        0      269 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_server/state.ini.template
-drwxrwxrwx   0        0        0        0 2023-05-23 12:42:09.147893 tabpy-2.8.0/tabpy/tabpy_server/static/
--rw-rw-rw-   0        0        0     1768 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_server/static/TabPy_logo.png
--rw-rw-rw-   0        0        0     1619 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_server/static/index.html
--rw-rw-rw-   0        0        0    33575 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_server/static/tableau.png
-drwxrwxrwx   0        0        0        0 2023-05-23 12:42:09.179046 tabpy-2.8.0/tabpy/tabpy_tools/
--rw-rw-rw-   0        0        0        0 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_tools/__init__.py
--rw-rw-rw-   0        0        0    12171 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_tools/client.py
--rw-rw-rw-   0        0        0     2429 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_tools/custom_query_object.py
--rw-rw-rw-   0        0        0     3052 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_tools/query_object.py
--rw-rw-rw-   0        0        0    13521 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_tools/rest.py
--rw-rw-rw-   0        0        0     7283 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_tools/rest_client.py
--rw-rw-rw-   0        0        0     4241 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_tools/schema.py
-drwxrwxrwx   0        0        0        0 2023-05-23 12:42:09.194671 tabpy-2.8.0/tabpy/utils/
--rw-rw-rw-   0        0        0        0 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/utils/__init__.py
--rw-rw-rw-   0        0        0     4394 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/utils/tabpy_user.py
-drwxrwxrwx   0        0        0        0 2023-05-23 12:42:08.816209 tabpy-2.8.0/tabpy.egg-info/
--rw-rw-rw-   0        0        0     6907 2023-05-23 12:42:08.000000 tabpy-2.8.0/tabpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4829 2023-05-23 12:42:08.000000 tabpy-2.8.0/tabpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 12:42:08.000000 tabpy-2.8.0/tabpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      138 2023-05-23 12:42:08.000000 tabpy-2.8.0/tabpy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      218 2023-05-23 12:42:08.000000 tabpy-2.8.0/tabpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-23 12:42:08.000000 tabpy-2.8.0/tabpy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-23 12:42:09.210302 tabpy-2.8.0/tests/
--rw-rw-rw-   0        0        0        0 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 12:42:09.335501 tabpy-2.8.0/tests/integration/
--rw-rw-rw-   0        0        0        0 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/integration/__init__.py
--rw-rw-rw-   0        0        0    10362 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/integration/integ_test_base.py
-drwxrwxrwx   0        0        0        0 2023-05-23 12:42:09.382165 tabpy-2.8.0/tests/integration/resources/
--rw-rw-rw-   0        0        0     1398 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/integration/resources/2019_04_24_to_3018_08_25.crt
--rw-rw-rw-   0        0        0     1706 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/integration/resources/2019_04_24_to_3018_08_25.key
--rw-rw-rw-   0        0        0     1347 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/integration/resources/data.csv
--rw-rw-rw-   0        0        0     1569 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/integration/resources/deploy_and_evaluate_model.conf
--rw-rw-rw-   0        0        0     1582 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/integration/resources/deploy_and_evaluate_model_auth.conf
--rw-rw-rw-   0        0        0      136 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/integration/resources/pwdfile.txt
--rw-rw-rw-   0        0        0     2246 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/integration/test_arrow_server.py
--rw-rw-rw-   0        0        0     2461 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/integration/test_auth.py
--rw-rw-rw-   0        0        0     1261 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/integration/test_custom_evaluate_timeout.py
--rw-rw-rw-   0        0        0     1067 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/integration/test_deploy_and_evaluate_model.py
--rw-rw-rw-   0        0        0     1267 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/integration/test_deploy_and_evaluate_model_auth_on.py
--rw-rw-rw-   0        0        0     1506 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/integration/test_deploy_and_evaluate_model_ssl.py
--rw-rw-rw-   0        0        0      736 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/integration/test_deploy_model_ssl_off_auth_off.py
--rw-rw-rw-   0        0        0      950 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/integration/test_deploy_model_ssl_off_auth_on.py
--rw-rw-rw-   0        0        0     1112 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/integration/test_deploy_model_ssl_on_auth_off.py
--rw-rw-rw-   0        0        0     3045 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/integration/test_deploy_model_ssl_on_auth_on.py
--rw-rw-rw-   0        0        0     3295 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/integration/test_evaluate.py
--rw-rw-rw-   0        0        0     3376 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/integration/test_gzip.py
--rw-rw-rw-   0        0        0      725 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/integration/test_url.py
--rw-rw-rw-   0        0        0      986 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/integration/test_url_ssl.py
-drwxrwxrwx   0        0        0        0 2023-05-23 12:42:09.397890 tabpy-2.8.0/tests/unit/
--rw-rw-rw-   0        0        0        0 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/unit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 12:42:09.460385 tabpy-2.8.0/tests/unit/server_tests/
--rw-rw-rw-   0        0        0        0 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/unit/server_tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 12:42:09.491659 tabpy-2.8.0/tests/unit/server_tests/resources/
--rw-rw-rw-   0        0        0      758 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/unit/server_tests/resources/expired.crt
--rw-rw-rw-   0        0        0     4330 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/unit/server_tests/resources/future.crt
--rw-rw-rw-   0        0        0     1410 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/unit/server_tests/resources/valid.crt
--rw-rw-rw-   0        0        0    13712 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/unit/server_tests/test_config.py
--rw-rw-rw-   0        0        0      486 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/unit/server_tests/test_endpoint_file_manager.py
--rw-rw-rw-   0        0        0     5347 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/unit/server_tests/test_endpoint_handler.py
--rw-rw-rw-   0        0        0     4729 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/unit/server_tests/test_endpoints_handler.py
--rw-rw-rw-   0        0        0    18446 2023-05-23 12:40:10.000000 tabpy-2.8.0/tests/unit/server_tests/test_evaluation_plane_handler.py
--rw-rw-rw-   0        0        0     5711 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/unit/server_tests/test_pwd_file.py
--rw-rw-rw-   0        0        0     5519 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/unit/server_tests/test_service_info_handler.py
-drwxrwxrwx   0        0        0        0 2023-05-23 12:42:09.526171 tabpy-2.8.0/tests/unit/tools_tests/
--rw-rw-rw-   0        0        0      100 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/unit/tools_tests/__init__.py
--rw-rw-rw-   0        0        0     3262 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/unit/tools_tests/test_client.py
--rw-rw-rw-   0        0        0     7665 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/unit/tools_tests/test_rest.py
--rw-rw-rw-   0        0        0     1959 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/unit/tools_tests/test_rest_object.py
--rw-rw-rw-   0        0        0     1082 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/unit/tools_tests/test_schema.py
+drwxrwxrwx   0        0        0        0 2023-06-21 21:32:07.196187 tabpy-2.9.0/
+drwxrwxrwx   0        0        0        0 2023-06-21 21:32:06.195418 tabpy-2.9.0/.github/
+drwxrwxrwx   0        0        0        0 2023-06-21 21:32:06.490851 tabpy-2.9.0/.github/ISSUE_TEMPLATE/
+-rw-rw-rw-   0        0        0      715 2023-05-02 13:24:30.000000 tabpy-2.9.0/.github/ISSUE_TEMPLATE/tabpy-issue-report.md
+drwxrwxrwx   0        0        0        0 2023-06-21 21:32:06.490851 tabpy-2.9.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-rw-rw-   0        0        0     1400 2023-05-02 13:24:30.000000 tabpy-2.9.0/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
+drwxrwxrwx   0        0        0        0 2023-06-21 21:32:06.522211 tabpy-2.9.0/.github/workflows/
+-rw-rw-rw-   0        0        0      971 2023-06-21 19:08:14.000000 tabpy-2.9.0/.github/workflows/coverage.yml
+-rw-rw-rw-   0        0        0     1439 2023-05-02 13:24:30.000000 tabpy-2.9.0/.github/workflows/docker-publish.yml
+-rw-rw-rw-   0        0        0     1138 2023-05-02 13:24:30.000000 tabpy-2.9.0/.github/workflows/lint.yml
+-rw-rw-rw-   0        0        0      903 2023-06-21 21:31:04.000000 tabpy-2.9.0/.github/workflows/pull_request.yml
+-rw-rw-rw-   0        0        0      897 2023-06-21 21:31:04.000000 tabpy-2.9.0/.github/workflows/push.yml
+-rw-rw-rw-   0        0        0     1659 2023-05-02 13:24:30.000000 tabpy-2.9.0/.gitignore
+-rw-rw-rw-   0        0        0       66 2023-05-02 13:24:30.000000 tabpy-2.9.0/.pep8speaks.yml
+-rw-rw-rw-   0        0        0      831 2023-05-02 13:24:30.000000 tabpy-2.9.0/.scrutinizer.yml
+-rw-rw-rw-   0        0        0     5537 2023-06-21 21:31:04.000000 tabpy-2.9.0/CHANGELOG
+-rw-rw-rw-   0        0        0     3969 2023-05-02 13:24:30.000000 tabpy-2.9.0/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0      272 2023-05-02 13:24:30.000000 tabpy-2.9.0/Dockerfile
+-rw-rw-rw-   0        0        0     1099 2023-05-02 13:24:30.000000 tabpy-2.9.0/LICENSE
+-rw-rw-rw-   0        0        0      549 2023-05-02 13:24:30.000000 tabpy-2.9.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     7093 2023-06-21 21:32:07.196187 tabpy-2.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0      131 2023-05-02 13:24:30.000000 tabpy-2.9.0/Procfile
+-rw-rw-rw-   0        0        0     3334 2023-05-02 13:24:30.000000 tabpy-2.9.0/README.md
+-rw-rw-rw-   0        0        0       27 2023-05-02 13:24:30.000000 tabpy-2.9.0/_config.yml
+-rw-rw-rw-   0        0        0      765 2023-05-02 13:24:30.000000 tabpy-2.9.0/app.json
+-rw-rw-rw-   0        0        0     2523 2023-05-02 13:24:30.000000 tabpy-2.9.0/codeql-analysis.yml
+drwxrwxrwx   0        0        0        0 2023-06-21 21:32:06.569085 tabpy-2.9.0/docs/
+-rw-rw-rw-   0        0        0     7688 2023-05-02 13:24:30.000000 tabpy-2.9.0/docs/TableauConfiguration.md
+-rw-rw-rw-   0        0        0      887 2023-05-02 13:24:30.000000 tabpy-2.9.0/docs/about.md
+-rw-rw-rw-   0        0        0      426 2023-05-02 13:24:30.000000 tabpy-2.9.0/docs/deploy-to-heroku.md
+drwxrwxrwx   0        0        0        0 2023-06-21 21:32:06.600338 tabpy-2.9.0/docs/img/
+-rw-rw-rw-   0        0        0   136889 2023-05-02 13:24:30.000000 tabpy-2.9.0/docs/img/Example1-SimpleFunctionCall.png
+-rw-rw-rw-   0        0        0   188230 2023-05-02 13:24:30.000000 tabpy-2.9.0/docs/img/Example2-MultipleFunctionCalls.png
+-rw-rw-rw-   0        0        0    43399 2023-05-02 13:24:30.000000 tabpy-2.9.0/docs/img/python-calculated-field.png
+-rw-rw-rw-   0        0        0     1229 2023-05-02 13:24:30.000000 tabpy-2.9.0/docs/security.md
+-rw-rw-rw-   0        0        0    13360 2023-05-02 13:24:30.000000 tabpy-2.9.0/docs/server-config.md
+-rw-rw-rw-   0        0        0     1422 2023-05-02 13:24:30.000000 tabpy-2.9.0/docs/server-install.md
+-rw-rw-rw-   0        0        0     4268 2023-05-02 13:24:30.000000 tabpy-2.9.0/docs/server-rest.md
+-rw-rw-rw-   0        0        0    17022 2023-05-02 13:24:30.000000 tabpy-2.9.0/docs/tabpy-tools.md
+-rw-rw-rw-   0        0        0     2174 2023-05-02 13:24:30.000000 tabpy-2.9.0/docs/tabpy-virtualenv.md
+drwxrwxrwx   0        0        0        0 2023-06-21 21:32:06.615959 tabpy-2.9.0/misc/
+-rw-rw-rw-   0        0        0     3747 2023-05-02 13:24:30.000000 tabpy-2.9.0/misc/TabPy.postman_collection.json
+-rw-rw-rw-   0        0        0     7855 2023-05-02 13:24:30.000000 tabpy-2.9.0/misc/TabPy.yml
+-rw-rw-rw-   0        0        0       90 2023-05-02 13:24:30.000000 tabpy-2.9.0/requirements.txt
+-rw-rw-rw-   0        0        0        6 2023-05-02 13:24:30.000000 tabpy-2.9.0/requirements_dev.txt
+-rw-rw-rw-   0        0        0      337 2023-06-21 21:32:07.196187 tabpy-2.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     3708 2023-06-21 18:37:59.000000 tabpy-2.9.0/setup.py
+-rw-rw-rw-   0        0        0      512 2023-05-02 13:24:30.000000 tabpy-2.9.0/start.sh
+drwxrwxrwx   0        0        0        0 2023-06-21 21:32:06.631587 tabpy-2.9.0/tabpy/
+-rw-rw-rw-   0        0        0        7 2023-06-21 21:31:04.000000 tabpy-2.9.0/tabpy/VERSION
+-rw-rw-rw-   0        0        0        0 2023-05-02 13:24:30.000000 tabpy-2.9.0/tabpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 21:32:06.694088 tabpy-2.9.0/tabpy/models/
+-rw-rw-rw-   0        0        0        0 2023-05-02 13:24:30.000000 tabpy-2.9.0/tabpy/models/__init__.py
+-rw-rw-rw-   0        0        0      820 2023-05-02 13:24:30.000000 tabpy-2.9.0/tabpy/models/deploy_models.py
+drwxrwxrwx   0        0        0        0 2023-06-21 21:32:06.725336 tabpy-2.9.0/tabpy/models/scripts/
+-rw-rw-rw-   0        0        0      715 2023-05-02 13:24:30.000000 tabpy-2.9.0/tabpy/models/scripts/ANOVA.py
+-rw-rw-rw-   0        0        0     2258 2023-05-02 13:24:30.000000 tabpy-2.9.0/tabpy/models/scripts/PCA.py
+-rw-rw-rw-   0        0        0     1476 2023-05-02 13:24:30.000000 tabpy-2.9.0/tabpy/models/scripts/SentimentAnalysis.py
+-rw-rw-rw-   0        0        0        0 2023-05-02 13:24:30.000000 tabpy-2.9.0/tabpy/models/scripts/__init__.py
+-rw-rw-rw-   0        0        0     1416 2023-05-02 13:24:30.000000 tabpy-2.9.0/tabpy/models/scripts/tTest.py
+drwxrwxrwx   0        0        0        0 2023-06-21 21:32:06.725336 tabpy-2.9.0/tabpy/models/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-02 13:24:30.000000 tabpy-2.9.0/tabpy/models/utils/__init__.py
+-rw-rw-rw-   0        0        0     1789 2023-05-02 13:24:30.000000 tabpy-2.9.0/tabpy/models/utils/setup_utils.py
+-rw-rw-rw-   0        0        0     1126 2023-06-21 21:31:04.000000 tabpy-2.9.0/tabpy/tabpy.py
+drwxrwxrwx   0        0        0        0 2023-06-21 21:32:06.740968 tabpy-2.9.0/tabpy/tabpy_server/
+-rw-rw-rw-   0        0        0        0 2023-05-02 13:24:30.000000 tabpy-2.9.0/tabpy/tabpy_server/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 21:32:06.772287 tabpy-2.9.0/tabpy/tabpy_server/app/
+-rw-rw-rw-   0        0        0        0 2023-05-02 13:24:30.000000 tabpy-2.9.0/tabpy/tabpy_server/app/__init__.py
+-rw-rw-rw-   0        0        0    22085 2023-06-21 21:31:04.000000 tabpy-2.9.0/tabpy/tabpy_server/app/app.py
+-rw-rw-rw-   0        0        0     1560 2023-05-02 13:24:30.000000 tabpy-2.9.0/tabpy/tabpy_server/app/app_parameters.py
+-rw-rw-rw-   0        0        0     5396 2023-05-02 13:24:30.000000 tabpy-2.9.0/tabpy/tabpy_server/app/arrow_server.py
+-rw-rw-rw-   0        0        0     2723 2023-05-02 13:24:30.000000 tabpy-2.9.0/tabpy/tabpy_server/app/util.py
+drwxrwxrwx   0        0        0        0 2023-06-21 21:32:06.787833 tabpy-2.9.0/tabpy/tabpy_server/common/
+-rw-rw-rw-   0        0        0        0 2023-05-02 13:24:30.000000 tabpy-2.9.0/tabpy/tabpy_server/common/__init__.py
+-rw-rw-rw-   0        0        0     1985 2023-05-02 13:24:30.000000 tabpy-2.9.0/tabpy/tabpy_server/common/default.conf
+-rw-rw-rw-   0        0        0     3010 2023-05-02 13:24:30.000000 tabpy-2.9.0/tabpy/tabpy_server/common/endpoint_file_mgr.py
+-rw-rw-rw-   0        0        0     3828 2023-05-02 13:24:30.000000 tabpy-2.9.0/tabpy/tabpy_server/common/messages.py
+-rw-rw-rw-   0        0        0      107 2023-05-02 13:24:30.000000 tabpy-2.9.0/tabpy/tabpy_server/common/util.py
+drwxrwxrwx   0        0        0        0 2023-06-21 21:32:06.850369 tabpy-2.9.0/tabpy/tabpy_server/handlers/
+-rw-rw-rw-   0        0        0     1014 2023-05-02 13:24:31.000000 tabpy-2.9.0/tabpy/tabpy_server/handlers/__init__.py
+-rw-rw-rw-   0        0        0    16470 2023-05-23 12:40:10.000000 tabpy-2.9.0/tabpy/tabpy_server/handlers/base_handler.py
+-rw-rw-rw-   0        0        0     1735 2023-05-02 13:24:31.000000 tabpy-2.9.0/tabpy/tabpy_server/handlers/basic_auth_server_middleware_factory.py
+-rw-rw-rw-   0        0        0     5068 2023-05-02 13:24:31.000000 tabpy-2.9.0/tabpy/tabpy_server/handlers/endpoint_handler.py
+-rw-rw-rw-   0        0        0     2598 2023-05-02 13:24:31.000000 tabpy-2.9.0/tabpy/tabpy_server/handlers/endpoints_handler.py
+-rw-rw-rw-   0        0        0     8376 2023-05-23 12:40:10.000000 tabpy-2.9.0/tabpy/tabpy_server/handlers/evaluation_plane_handler.py
+-rw-rw-rw-   0        0        0     5840 2023-05-02 13:24:31.000000 tabpy-2.9.0/tabpy/tabpy_server/handlers/management_handler.py
+-rw-rw-rw-   0        0        0      211 2023-05-02 13:24:31.000000 tabpy-2.9.0/tabpy/tabpy_server/handlers/no_op_auth_handler.py
+-rw-rw-rw-   0        0        0     8448 2023-05-23 12:40:10.000000 tabpy-2.9.0/tabpy/tabpy_server/handlers/query_plane_handler.py
+-rw-rw-rw-   0        0        0      998 2023-05-02 13:24:31.000000 tabpy-2.9.0/tabpy/tabpy_server/handlers/service_info_handler.py
+-rw-rw-rw-   0        0        0      921 2023-05-02 13:24:31.000000 tabpy-2.9.0/tabpy/tabpy_server/handlers/status_handler.py
+-rw-rw-rw-   0        0        0      721 2023-05-02 13:24:31.000000 tabpy-2.9.0/tabpy/tabpy_server/handlers/upload_destination_handler.py
+-rw-rw-rw-   0        0        0     1005 2023-05-02 13:24:31.000000 tabpy-2.9.0/tabpy/tabpy_server/handlers/util.py
+drwxrwxrwx   0        0        0        0 2023-06-21 21:32:06.865867 tabpy-2.9.0/tabpy/tabpy_server/management/
+-rw-rw-rw-   0        0        0        0 2023-05-02 13:24:31.000000 tabpy-2.9.0/tabpy/tabpy_server/management/__init__.py
+-rw-rw-rw-   0        0        0    21331 2023-05-02 13:24:31.000000 tabpy-2.9.0/tabpy/tabpy_server/management/state.py
+-rw-rw-rw-   0        0        0     1524 2023-05-02 13:24:31.000000 tabpy-2.9.0/tabpy/tabpy_server/management/util.py
+drwxrwxrwx   0        0        0        0 2023-06-21 21:32:06.881493 tabpy-2.9.0/tabpy/tabpy_server/psws/
+-rw-rw-rw-   0        0        0        0 2023-05-02 13:24:31.000000 tabpy-2.9.0/tabpy/tabpy_server/psws/__init__.py
+-rw-rw-rw-   0        0        0     7364 2023-05-02 13:24:31.000000 tabpy-2.9.0/tabpy/tabpy_server/psws/callbacks.py
+-rw-rw-rw-   0        0        0     9732 2023-05-02 13:24:31.000000 tabpy-2.9.0/tabpy/tabpy_server/psws/python_service.py
+-rw-rw-rw-   0        0        0      269 2023-05-02 13:24:31.000000 tabpy-2.9.0/tabpy/tabpy_server/state.ini.template
+drwxrwxrwx   0        0        0        0 2023-06-21 21:32:06.881493 tabpy-2.9.0/tabpy/tabpy_server/static/
+-rw-rw-rw-   0        0        0     1768 2023-05-02 13:24:31.000000 tabpy-2.9.0/tabpy/tabpy_server/static/TabPy_logo.png
+-rw-rw-rw-   0        0        0     1619 2023-05-02 13:24:31.000000 tabpy-2.9.0/tabpy/tabpy_server/static/index.html
+-rw-rw-rw-   0        0        0    33575 2023-05-02 13:24:31.000000 tabpy-2.9.0/tabpy/tabpy_server/static/tableau.png
+drwxrwxrwx   0        0        0        0 2023-06-21 21:32:06.912802 tabpy-2.9.0/tabpy/tabpy_tools/
+-rw-rw-rw-   0        0        0        0 2023-05-02 13:24:31.000000 tabpy-2.9.0/tabpy/tabpy_tools/__init__.py
+-rw-rw-rw-   0        0        0    12171 2023-05-02 13:24:31.000000 tabpy-2.9.0/tabpy/tabpy_tools/client.py
+-rw-rw-rw-   0        0        0     2429 2023-05-02 13:24:31.000000 tabpy-2.9.0/tabpy/tabpy_tools/custom_query_object.py
+-rw-rw-rw-   0        0        0     3052 2023-05-02 13:24:31.000000 tabpy-2.9.0/tabpy/tabpy_tools/query_object.py
+-rw-rw-rw-   0        0        0    13521 2023-05-02 13:24:31.000000 tabpy-2.9.0/tabpy/tabpy_tools/rest.py
+-rw-rw-rw-   0        0        0     7283 2023-05-02 13:24:31.000000 tabpy-2.9.0/tabpy/tabpy_tools/rest_client.py
+-rw-rw-rw-   0        0        0     4241 2023-05-02 13:24:31.000000 tabpy-2.9.0/tabpy/tabpy_tools/schema.py
+drwxrwxrwx   0        0        0        0 2023-06-21 21:32:06.928368 tabpy-2.9.0/tabpy/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-02 13:24:31.000000 tabpy-2.9.0/tabpy/utils/__init__.py
+-rw-rw-rw-   0        0        0     4394 2023-05-02 13:24:31.000000 tabpy-2.9.0/tabpy/utils/tabpy_user.py
+drwxrwxrwx   0        0        0        0 2023-06-21 21:32:06.678368 tabpy-2.9.0/tabpy.egg-info/
+-rw-rw-rw-   0        0        0     7093 2023-06-21 21:32:05.000000 tabpy-2.9.0/tabpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4829 2023-06-21 21:32:06.000000 tabpy-2.9.0/tabpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 21:32:05.000000 tabpy-2.9.0/tabpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      138 2023-06-21 21:32:05.000000 tabpy-2.9.0/tabpy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      218 2023-06-21 21:32:05.000000 tabpy-2.9.0/tabpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-21 21:32:05.000000 tabpy-2.9.0/tabpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-21 21:32:06.928368 tabpy-2.9.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-02 13:24:31.000000 tabpy-2.9.0/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 21:32:07.024403 tabpy-2.9.0/tests/integration/
+-rw-rw-rw-   0        0        0        0 2023-05-02 13:24:31.000000 tabpy-2.9.0/tests/integration/__init__.py
+-rw-rw-rw-   0        0        0    10388 2023-06-21 21:31:04.000000 tabpy-2.9.0/tests/integration/integ_test_base.py
+drwxrwxrwx   0        0        0        0 2023-06-21 21:32:07.071281 tabpy-2.9.0/tests/integration/resources/
+-rw-rw-rw-   0        0        0     1398 2023-05-02 13:24:31.000000 tabpy-2.9.0/tests/integration/resources/2019_04_24_to_3018_08_25.crt
+-rw-rw-rw-   0        0        0     1706 2023-05-02 13:24:31.000000 tabpy-2.9.0/tests/integration/resources/2019_04_24_to_3018_08_25.key
+-rw-rw-rw-   0        0        0     1347 2023-05-02 13:24:31.000000 tabpy-2.9.0/tests/integration/resources/data.csv
+-rw-rw-rw-   0        0        0     1569 2023-05-02 13:24:31.000000 tabpy-2.9.0/tests/integration/resources/deploy_and_evaluate_model.conf
+-rw-rw-rw-   0        0        0     1582 2023-05-02 13:24:31.000000 tabpy-2.9.0/tests/integration/resources/deploy_and_evaluate_model_auth.conf
+-rw-rw-rw-   0        0        0      136 2023-05-02 13:24:31.000000 tabpy-2.9.0/tests/integration/resources/pwdfile.txt
+-rw-rw-rw-   0        0        0     2246 2023-05-02 13:24:31.000000 tabpy-2.9.0/tests/integration/test_arrow_server.py
+-rw-rw-rw-   0        0        0     2461 2023-05-02 13:24:31.000000 tabpy-2.9.0/tests/integration/test_auth.py
+-rw-rw-rw-   0        0        0     1261 2023-05-02 13:24:31.000000 tabpy-2.9.0/tests/integration/test_custom_evaluate_timeout.py
+-rw-rw-rw-   0        0        0     1067 2023-05-02 13:24:31.000000 tabpy-2.9.0/tests/integration/test_deploy_and_evaluate_model.py
+-rw-rw-rw-   0        0        0     1267 2023-05-02 13:24:31.000000 tabpy-2.9.0/tests/integration/test_deploy_and_evaluate_model_auth_on.py
+-rw-rw-rw-   0        0        0     1506 2023-05-02 13:24:31.000000 tabpy-2.9.0/tests/integration/test_deploy_and_evaluate_model_ssl.py
+-rw-rw-rw-   0        0        0      736 2023-05-02 13:24:31.000000 tabpy-2.9.0/tests/integration/test_deploy_model_ssl_off_auth_off.py
+-rw-rw-rw-   0        0        0      950 2023-05-02 13:24:31.000000 tabpy-2.9.0/tests/integration/test_deploy_model_ssl_off_auth_on.py
+-rw-rw-rw-   0        0        0     1112 2023-05-02 13:24:31.000000 tabpy-2.9.0/tests/integration/test_deploy_model_ssl_on_auth_off.py
+-rw-rw-rw-   0        0        0     3045 2023-05-02 13:24:31.000000 tabpy-2.9.0/tests/integration/test_deploy_model_ssl_on_auth_on.py
+-rw-rw-rw-   0        0        0     3295 2023-05-02 13:24:31.000000 tabpy-2.9.0/tests/integration/test_evaluate.py
+-rw-rw-rw-   0        0        0     3376 2023-05-02 13:24:31.000000 tabpy-2.9.0/tests/integration/test_gzip.py
+-rw-rw-rw-   0        0        0      725 2023-05-02 13:24:31.000000 tabpy-2.9.0/tests/integration/test_url.py
+-rw-rw-rw-   0        0        0      986 2023-05-02 13:24:31.000000 tabpy-2.9.0/tests/integration/test_url_ssl.py
+drwxrwxrwx   0        0        0        0 2023-06-21 21:32:07.071281 tabpy-2.9.0/tests/unit/
+-rw-rw-rw-   0        0        0        0 2023-05-02 13:24:31.000000 tabpy-2.9.0/tests/unit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 21:32:07.133779 tabpy-2.9.0/tests/unit/server_tests/
+-rw-rw-rw-   0        0        0        0 2023-05-02 13:24:31.000000 tabpy-2.9.0/tests/unit/server_tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 21:32:07.149314 tabpy-2.9.0/tests/unit/server_tests/resources/
+-rw-rw-rw-   0        0        0      758 2023-05-02 13:24:31.000000 tabpy-2.9.0/tests/unit/server_tests/resources/expired.crt
+-rw-rw-rw-   0        0        0     4330 2023-05-02 13:24:31.000000 tabpy-2.9.0/tests/unit/server_tests/resources/future.crt
+-rw-rw-rw-   0        0        0     1410 2023-05-02 13:24:31.000000 tabpy-2.9.0/tests/unit/server_tests/resources/valid.crt
+-rw-rw-rw-   0        0        0    14427 2023-06-21 21:31:04.000000 tabpy-2.9.0/tests/unit/server_tests/test_config.py
+-rw-rw-rw-   0        0        0      486 2023-05-02 13:24:31.000000 tabpy-2.9.0/tests/unit/server_tests/test_endpoint_file_manager.py
+-rw-rw-rw-   0        0        0     5347 2023-05-02 13:24:31.000000 tabpy-2.9.0/tests/unit/server_tests/test_endpoint_handler.py
+-rw-rw-rw-   0        0        0     4729 2023-05-02 13:24:31.000000 tabpy-2.9.0/tests/unit/server_tests/test_endpoints_handler.py
+-rw-rw-rw-   0        0        0    18446 2023-05-23 12:40:10.000000 tabpy-2.9.0/tests/unit/server_tests/test_evaluation_plane_handler.py
+-rw-rw-rw-   0        0        0     5711 2023-05-02 13:24:31.000000 tabpy-2.9.0/tests/unit/server_tests/test_pwd_file.py
+-rw-rw-rw-   0        0        0     5519 2023-05-02 13:24:31.000000 tabpy-2.9.0/tests/unit/server_tests/test_service_info_handler.py
+drwxrwxrwx   0        0        0        0 2023-06-21 21:32:07.180564 tabpy-2.9.0/tests/unit/tools_tests/
+-rw-rw-rw-   0        0        0      100 2023-05-02 13:24:31.000000 tabpy-2.9.0/tests/unit/tools_tests/__init__.py
+-rw-rw-rw-   0        0        0     3262 2023-05-02 13:24:31.000000 tabpy-2.9.0/tests/unit/tools_tests/test_client.py
+-rw-rw-rw-   0        0        0     7665 2023-05-02 13:24:31.000000 tabpy-2.9.0/tests/unit/tools_tests/test_rest.py
+-rw-rw-rw-   0        0        0     1959 2023-05-02 13:24:31.000000 tabpy-2.9.0/tests/unit/tools_tests/test_rest_object.py
+-rw-rw-rw-   0        0        0     1082 2023-05-02 13:24:31.000000 tabpy-2.9.0/tests/unit/tools_tests/test_schema.py
```

### Comparing `tabpy-2.8.0/.github/ISSUE_TEMPLATE/tabpy-issue-report.md` & `tabpy-2.9.0/.github/ISSUE_TEMPLATE/tabpy-issue-report.md`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md` & `tabpy-2.9.0/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/.github/workflows/coverage.yml` & `tabpy-2.9.0/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/.github/workflows/docker-publish.yml` & `tabpy-2.9.0/.github/workflows/docker-publish.yml`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/.github/workflows/lint.yml` & `tabpy-2.9.0/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/.github/workflows/pull_request.yml` & `tabpy-2.9.0/.github/workflows/pull_request.yml`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 jobs:
   build:
     name: ${{ matrix.python-version }} on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     
     strategy:
       matrix:
-        python-version: [3.7, 3.8, 3.9]
+        # TODO: Add 3.7 to python-versions after GitHub action regression is resolved.
+        # https://github.com/actions/setup-python/issues/682
+        python-version: [3.8, 3.9]
         os: [ubuntu-latest, windows-latest, macos-latest]
 
     steps:
     - uses: actions/checkout@v1
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v1
```

### Comparing `tabpy-2.8.0/.github/workflows/push.yml` & `tabpy-2.9.0/.github/workflows/push.yml`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 jobs:
   build:
     name: ${{ matrix.python-version }} on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     
     strategy:
       matrix:
-        python-version: [3.7, 3.8, 3.9]
+        # TODO: Add 3.7 to python-versions after GitHub action regression is resolved.
+        # https://github.com/actions/setup-python/issues/682
+        python-version: [3.8, 3.9]
         os: [ubuntu-latest, windows-latest, macos-latest]
 
     steps:
     - uses: actions/checkout@v1
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v1
```

### Comparing `tabpy-2.8.0/.gitignore` & `tabpy-2.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/.scrutinizer.yml` & `tabpy-2.9.0/.scrutinizer.yml`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/CHANGELOG` & `tabpy-2.9.0/CHANGELOG`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Changelog
 
+## v2.9.0
+
+### Improvements
+
+- Require confirmation to continue when starting TabPy without authentication, 
+  with a warning that this is an insecure state and not recommended.
+
 ## v2.8.0
 
 ### Improvements
 
 - Returns 413 error code when request payload exceeds 
 TABPY_MAX_REQUEST_SIZE_MB config setting.
```

### Comparing `tabpy-2.8.0/CONTRIBUTING.md` & `tabpy-2.9.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/LICENSE` & `tabpy-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/MANIFEST.in` & `tabpy-2.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/PKG-INFO` & `tabpy-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabpy
-Version: 2.8.0
+Version: 2.9.0
 Summary: Web server Tableau uses to run Python scripts.
 Home-page: https://github.com/tableau/TabPy
 Download-URL: https://pypi.org/project/tabpy
 Author: Tableau
 Author-email: github@tableau.com
 Maintainer: Tableau
 Maintainer-email: github@tableau.com
@@ -37,14 +37,21 @@
 
 TabPy (the Tableau Python Server) is an external service implementation
 which expands Tableau's capabilities by allowing users to execute Python
 scripts and saved functions via Tableau's table calculations.
 
 # Changelog
 
+## v2.9.0
+
+### Improvements
+
+- Require confirmation to continue when starting TabPy without authentication, 
+  with a warning that this is an insecure state and not recommended.
+
 ## v2.8.0
 
 ### Improvements
 
 - Returns 413 error code when request payload exceeds 
 TABPY_MAX_REQUEST_SIZE_MB config setting.
```

### Comparing `tabpy-2.8.0/README.md` & `tabpy-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/app.json` & `tabpy-2.9.0/app.json`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/codeql-analysis.yml` & `tabpy-2.9.0/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/docs/TableauConfiguration.md` & `tabpy-2.9.0/docs/TableauConfiguration.md`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/docs/about.md` & `tabpy-2.9.0/docs/about.md`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/docs/img/Example1-SimpleFunctionCall.png` & `tabpy-2.9.0/docs/img/Example1-SimpleFunctionCall.png`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/docs/img/Example2-MultipleFunctionCalls.png` & `tabpy-2.9.0/docs/img/Example2-MultipleFunctionCalls.png`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/docs/img/python-calculated-field.png` & `tabpy-2.9.0/docs/img/python-calculated-field.png`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/docs/security.md` & `tabpy-2.9.0/docs/security.md`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/docs/server-config.md` & `tabpy-2.9.0/docs/server-config.md`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/docs/server-install.md` & `tabpy-2.9.0/docs/server-install.md`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/docs/server-rest.md` & `tabpy-2.9.0/docs/server-rest.md`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/docs/tabpy-tools.md` & `tabpy-2.9.0/docs/tabpy-tools.md`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/docs/tabpy-virtualenv.md` & `tabpy-2.9.0/docs/tabpy-virtualenv.md`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/misc/TabPy.postman_collection.json` & `tabpy-2.9.0/misc/TabPy.postman_collection.json`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/misc/TabPy.yml` & `tabpy-2.9.0/misc/TabPy.yml`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/setup.py` & `tabpy-2.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/start.sh` & `tabpy-2.9.0/start.sh`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tabpy/models/deploy_models.py` & `tabpy-2.9.0/tabpy/models/deploy_models.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tabpy/models/scripts/ANOVA.py` & `tabpy-2.9.0/tabpy/models/scripts/ANOVA.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tabpy/models/scripts/PCA.py` & `tabpy-2.9.0/tabpy/models/scripts/PCA.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tabpy/models/scripts/SentimentAnalysis.py` & `tabpy-2.9.0/tabpy/models/scripts/SentimentAnalysis.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tabpy/models/scripts/tTest.py` & `tabpy-2.9.0/tabpy/models/scripts/tTest.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tabpy/models/utils/setup_utils.py` & `tabpy-2.9.0/tabpy/models/utils/setup_utils.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tabpy/tabpy.py` & `tabpy-2.9.0/tabpy/tabpy.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """
 TabPy Server.
 
 Usage:
   tabpy [-h] | [--help]
-  tabpy [--config <CONFIG>]
+  tabpy [--config <CONFIG>] [--disable-auth-warning]
 
 Options:
-  -h --help         Show this screen.
-  --config <CONFIG> Path to a config file.
+  -h --help                 Show this screen.
+  --config <CONFIG>         Path to a config file.
+  --disable-auth-warning    Disable authentication warning.
 """
 
 import docopt
 import os
 from pathlib import Path
 
 
@@ -34,15 +35,19 @@
 __version__ = read_version()
 
 
 def main():
     args = docopt.docopt(__doc__)
     config = args["--config"] or None
 
+    disable_auth_warning = False
+    if args["--disable-auth-warning"]:
+        disable_auth_warning = True
+
     from tabpy.tabpy_server.app.app import TabPyApp
 
-    app = TabPyApp(config)
+    app = TabPyApp(config, disable_auth_warning)
     app.run()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `tabpy-2.8.0/tabpy/tabpy_server/app/app.py` & `tabpy-2.9.0/tabpy/tabpy_server/app/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,15 +63,16 @@
     subdirectory = ""
     tabpy_state = None
     python_service = None
     credentials = {}
     arrow_server = None
     max_request_size = None
 
-    def __init__(self, config_file):
+    def __init__(self, config_file, disable_auth_warning=True):
+        self.disable_auth_warning = disable_auth_warning
         if config_file is None:
             config_file = os.path.join(
                 os.path.dirname(__file__), os.path.pardir, "common", "default.conf"
             )
 
         if os.path.isfile(config_file):
             try:
@@ -390,17 +391,15 @@
                 msg = (
                     "Failed to read passwords file "
                     f"{self.settings[ConfigParameters.TABPY_PWD_FILE]}"
                 )
                 logger.critical(msg)
                 raise RuntimeError(msg)
         else:
-            logger.info(
-                "Password file is not specified: " "Authentication is not enabled"
-            )
+            self._handle_configuration_without_authentication()
 
         features = self._get_features()
         self.settings[SettingsParameters.ApiVersions] = {"v1": {"features": features}}
 
         self.settings[SettingsParameters.LogRequestContext] = (
             self.settings[SettingsParameters.LogRequestContext].lower() != "false"
         )
@@ -467,14 +466,39 @@
 
         if succeeded and len(self.credentials) == 0:
             logger.error("No credentials found")
             succeeded = False
 
         return succeeded
 
+    def _handle_configuration_without_authentication(self):
+        std_no_auth_msg = "Password file is not specified: Authentication is not enabled"
+
+        if self.disable_auth_warning == True:
+            logger.info(std_no_auth_msg)
+            return  
+
+        confirm_no_auth_msg = "\nWARNING: This TabPy server is not currently configured for username/password authentication. "
+
+        if self.settings[SettingsParameters.EvaluateEnabled]:
+            confirm_no_auth_msg += ("This means that, because the TABPY_EVALUATE_ENABLE feature is enabled, there is " 
+                "the potential that unauthenticated individuals may be able to remotely execute code on this machine. ")
+
+        confirm_no_auth_msg += ("We strongly advise against proceeding without authentication as it poses a significant security risk.\n\n"
+            "Do you wish to proceed without authentication? (y/N): ")
+
+        confirm_no_auth_input = input(confirm_no_auth_msg)
+
+        if confirm_no_auth_input == 'y':
+            logger.info(std_no_auth_msg)
+        else:
+            print("\nAborting start up. To enable authentication for your TabPy server, see "
+                "https://github.com/tableau/TabPy/blob/master/docs/server-config.md#authentication.")
+            exit()
+
     def _get_features(self):
         features = {}
 
         # Check for auth
         if ConfigParameters.TABPY_PWD_FILE in self.settings:
             features["authentication"] = {
                 "required": True,
```

### Comparing `tabpy-2.8.0/tabpy/tabpy_server/app/app_parameters.py` & `tabpy-2.9.0/tabpy/tabpy_server/app/app_parameters.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tabpy/tabpy_server/app/arrow_server.py` & `tabpy-2.9.0/tabpy/tabpy_server/app/arrow_server.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tabpy/tabpy_server/app/util.py` & `tabpy-2.9.0/tabpy/tabpy_server/app/util.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tabpy/tabpy_server/common/default.conf` & `tabpy-2.9.0/tabpy/tabpy_server/common/default.conf`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tabpy/tabpy_server/common/endpoint_file_mgr.py` & `tabpy-2.9.0/tabpy/tabpy_server/common/endpoint_file_mgr.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tabpy/tabpy_server/common/messages.py` & `tabpy-2.9.0/tabpy/tabpy_server/common/messages.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tabpy/tabpy_server/handlers/__init__.py` & `tabpy-2.9.0/tabpy/tabpy_server/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tabpy/tabpy_server/handlers/base_handler.py` & `tabpy-2.9.0/tabpy/tabpy_server/handlers/base_handler.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tabpy/tabpy_server/handlers/basic_auth_server_middleware_factory.py` & `tabpy-2.9.0/tabpy/tabpy_server/handlers/basic_auth_server_middleware_factory.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tabpy/tabpy_server/handlers/endpoint_handler.py` & `tabpy-2.9.0/tabpy/tabpy_server/handlers/endpoint_handler.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tabpy/tabpy_server/handlers/endpoints_handler.py` & `tabpy-2.9.0/tabpy/tabpy_server/handlers/endpoints_handler.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tabpy/tabpy_server/handlers/evaluation_plane_handler.py` & `tabpy-2.9.0/tabpy/tabpy_server/handlers/evaluation_plane_handler.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tabpy/tabpy_server/handlers/management_handler.py` & `tabpy-2.9.0/tabpy/tabpy_server/handlers/management_handler.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tabpy/tabpy_server/handlers/query_plane_handler.py` & `tabpy-2.9.0/tabpy/tabpy_server/handlers/query_plane_handler.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tabpy/tabpy_server/handlers/service_info_handler.py` & `tabpy-2.9.0/tabpy/tabpy_server/handlers/service_info_handler.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tabpy/tabpy_server/handlers/status_handler.py` & `tabpy-2.9.0/tabpy/tabpy_server/handlers/status_handler.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tabpy/tabpy_server/handlers/upload_destination_handler.py` & `tabpy-2.9.0/tabpy/tabpy_server/handlers/upload_destination_handler.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tabpy/tabpy_server/handlers/util.py` & `tabpy-2.9.0/tabpy/tabpy_server/handlers/util.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tabpy/tabpy_server/management/state.py` & `tabpy-2.9.0/tabpy/tabpy_server/management/state.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tabpy/tabpy_server/management/util.py` & `tabpy-2.9.0/tabpy/tabpy_server/management/util.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tabpy/tabpy_server/psws/callbacks.py` & `tabpy-2.9.0/tabpy/tabpy_server/psws/callbacks.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tabpy/tabpy_server/psws/python_service.py` & `tabpy-2.9.0/tabpy/tabpy_server/psws/python_service.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tabpy/tabpy_server/static/TabPy_logo.png` & `tabpy-2.9.0/tabpy/tabpy_server/static/TabPy_logo.png`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tabpy/tabpy_server/static/index.html` & `tabpy-2.9.0/tabpy/tabpy_server/static/index.html`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tabpy/tabpy_server/static/tableau.png` & `tabpy-2.9.0/tabpy/tabpy_server/static/tableau.png`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tabpy/tabpy_tools/client.py` & `tabpy-2.9.0/tabpy/tabpy_tools/client.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tabpy/tabpy_tools/custom_query_object.py` & `tabpy-2.9.0/tabpy/tabpy_tools/custom_query_object.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tabpy/tabpy_tools/query_object.py` & `tabpy-2.9.0/tabpy/tabpy_tools/query_object.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tabpy/tabpy_tools/rest.py` & `tabpy-2.9.0/tabpy/tabpy_tools/rest.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tabpy/tabpy_tools/rest_client.py` & `tabpy-2.9.0/tabpy/tabpy_tools/rest_client.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tabpy/tabpy_tools/schema.py` & `tabpy-2.9.0/tabpy/tabpy_tools/schema.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tabpy/utils/tabpy_user.py` & `tabpy-2.9.0/tabpy/utils/tabpy_user.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tabpy.egg-info/PKG-INFO` & `tabpy-2.9.0/tabpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabpy
-Version: 2.8.0
+Version: 2.9.0
 Summary: Web server Tableau uses to run Python scripts.
 Home-page: https://github.com/tableau/TabPy
 Download-URL: https://pypi.org/project/tabpy
 Author: Tableau
 Author-email: github@tableau.com
 Maintainer: Tableau
 Maintainer-email: github@tableau.com
@@ -37,14 +37,21 @@
 
 TabPy (the Tableau Python Server) is an external service implementation
 which expands Tableau's capabilities by allowing users to execute Python
 scripts and saved functions via Tableau's table calculations.
 
 # Changelog
 
+## v2.9.0
+
+### Improvements
+
+- Require confirmation to continue when starting TabPy without authentication, 
+  with a warning that this is an insecure state and not recommended.
+
 ## v2.8.0
 
 ### Improvements
 
 - Returns 413 error code when request payload exceeds 
 TABPY_MAX_REQUEST_SIZE_MB config setting.
```

### Comparing `tabpy-2.8.0/tabpy.egg-info/SOURCES.txt` & `tabpy-2.9.0/tabpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tests/integration/integ_test_base.py` & `tabpy-2.9.0/tests/integration/integ_test_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,15 +222,15 @@
         )
         if orig_config_file_name != self.config_file_name:
             shutil.copyfile(orig_config_file_name, self.config_file_name)
 
         # Platform specific - for integration tests we want to engage
         # startup script
         with open(self.tmp_dir + "/output.txt", "w") as outfile:
-            cmd = ["tabpy", "--config=" + self.config_file_name]
+            cmd = ["tabpy", "--config=" + self.config_file_name, "--disable-auth-warning"]
             preexec_fn = None
             if platform.system() == "Windows":
                 self.py = "python"
             else:
                 self.py = "python3"
                 preexec_fn = os.setsid
```

### Comparing `tabpy-2.8.0/tests/integration/resources/2019_04_24_to_3018_08_25.crt` & `tabpy-2.9.0/tests/integration/resources/2019_04_24_to_3018_08_25.crt`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tests/integration/resources/2019_04_24_to_3018_08_25.key` & `tabpy-2.9.0/tests/integration/resources/2019_04_24_to_3018_08_25.key`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tests/integration/resources/data.csv` & `tabpy-2.9.0/tests/integration/resources/data.csv`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tests/integration/resources/deploy_and_evaluate_model.conf` & `tabpy-2.9.0/tests/integration/resources/deploy_and_evaluate_model.conf`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tests/integration/resources/deploy_and_evaluate_model_auth.conf` & `tabpy-2.9.0/tests/integration/resources/deploy_and_evaluate_model_auth.conf`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tests/integration/test_arrow_server.py` & `tabpy-2.9.0/tests/integration/test_arrow_server.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tests/integration/test_auth.py` & `tabpy-2.9.0/tests/integration/test_auth.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tests/integration/test_custom_evaluate_timeout.py` & `tabpy-2.9.0/tests/integration/test_custom_evaluate_timeout.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tests/integration/test_deploy_and_evaluate_model.py` & `tabpy-2.9.0/tests/integration/test_deploy_and_evaluate_model.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tests/integration/test_deploy_and_evaluate_model_auth_on.py` & `tabpy-2.9.0/tests/integration/test_deploy_and_evaluate_model_auth_on.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tests/integration/test_deploy_and_evaluate_model_ssl.py` & `tabpy-2.9.0/tests/integration/test_deploy_and_evaluate_model_ssl.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tests/integration/test_deploy_model_ssl_off_auth_off.py` & `tabpy-2.9.0/tests/integration/test_deploy_model_ssl_off_auth_off.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tests/integration/test_deploy_model_ssl_off_auth_on.py` & `tabpy-2.9.0/tests/integration/test_deploy_model_ssl_off_auth_on.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tests/integration/test_deploy_model_ssl_on_auth_off.py` & `tabpy-2.9.0/tests/integration/test_deploy_model_ssl_on_auth_off.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tests/integration/test_deploy_model_ssl_on_auth_on.py` & `tabpy-2.9.0/tests/integration/test_deploy_model_ssl_on_auth_on.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tests/integration/test_evaluate.py` & `tabpy-2.9.0/tests/integration/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tests/integration/test_gzip.py` & `tabpy-2.9.0/tests/integration/test_gzip.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tests/integration/test_url.py` & `tabpy-2.9.0/tests/integration/test_url.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tests/integration/test_url_ssl.py` & `tabpy-2.9.0/tests/integration/test_url_ssl.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tests/unit/server_tests/resources/expired.crt` & `tabpy-2.9.0/tests/unit/server_tests/resources/expired.crt`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tests/unit/server_tests/resources/future.crt` & `tabpy-2.9.0/tests/unit/server_tests/resources/future.crt`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tests/unit/server_tests/resources/valid.crt` & `tabpy-2.9.0/tests/unit/server_tests/resources/valid.crt`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tests/unit/server_tests/test_config.py` & `tabpy-2.9.0/tests/unit/server_tests/test_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,34 @@
         mock_psws,
         mock_management_util,
         mock_tabpy_state,
     ):
         TabPyApp(None)
         self.assertEqual(len(mock_os.makedirs.mock_calls), 1)
 
+    @patch('builtins.input', return_value='y')
+    @patch("tabpy.tabpy_server.app.app.os")
+    @patch("tabpy.tabpy_server.app.app.os.path.exists", return_value=False)
+    @patch("tabpy.tabpy_server.app.app.PythonServiceHandler")
+    @patch("tabpy.tabpy_server.app.app._get_state_from_file")
+    @patch("tabpy.tabpy_server.app.app.TabPyState")
+    def test_handle_configuration_without_authentication(
+        self,
+        mock_tabpy_state,
+        mock_get_state_from_file,
+        mock_psws,
+        mock_os_path_exists,
+        mock_os,
+        mock_input,
+    ):
+        TabPyApp(None)
+        mock_input.assert_not_called()
+
+        TabPyApp(None, False)
+        mock_input.assert_called()
 
 class TestPartialConfigFile(unittest.TestCase):
     def setUp(self):
         self.config_file = NamedTemporaryFile(delete=False)
 
     def tearDown(self):
         os.remove(self.config_file.name)
```

### Comparing `tabpy-2.8.0/tests/unit/server_tests/test_endpoint_handler.py` & `tabpy-2.9.0/tests/unit/server_tests/test_endpoint_handler.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tests/unit/server_tests/test_endpoints_handler.py` & `tabpy-2.9.0/tests/unit/server_tests/test_endpoints_handler.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tests/unit/server_tests/test_evaluation_plane_handler.py` & `tabpy-2.9.0/tests/unit/server_tests/test_evaluation_plane_handler.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tests/unit/server_tests/test_pwd_file.py` & `tabpy-2.9.0/tests/unit/server_tests/test_pwd_file.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tests/unit/server_tests/test_service_info_handler.py` & `tabpy-2.9.0/tests/unit/server_tests/test_service_info_handler.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tests/unit/tools_tests/test_client.py` & `tabpy-2.9.0/tests/unit/tools_tests/test_client.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tests/unit/tools_tests/test_rest.py` & `tabpy-2.9.0/tests/unit/tools_tests/test_rest.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tests/unit/tools_tests/test_rest_object.py` & `tabpy-2.9.0/tests/unit/tools_tests/test_rest_object.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.8.0/tests/unit/tools_tests/test_schema.py` & `tabpy-2.9.0/tests/unit/tools_tests/test_schema.py`

 * *Files identical despite different names*

