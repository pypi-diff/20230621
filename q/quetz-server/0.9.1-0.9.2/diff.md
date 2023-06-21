# Comparing `tmp/quetz-server-0.9.1.tar.gz` & `tmp/quetz-server-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quetz-server-0.9.1.tar", last modified: Tue Jun 20 13:38:58 2023, max compression
+gzip compressed data, was "quetz-server-0.9.2.tar", last modified: Wed Jun 21 11:20:20 2023, max compression
```

## Comparing `quetz-server-0.9.1.tar` & `quetz-server-0.9.2.tar`

### file list

```diff
@@ -1,216 +1,216 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:38:58.799596 quetz-server-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-20 13:38:36.000000 quetz-server-0.9.1/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-20 13:38:36.000000 quetz-server-0.9.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-20 13:38:36.000000 quetz-server-0.9.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    24285 2023-06-20 13:38:46.000000 quetz-server-0.9.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-20 13:38:36.000000 quetz-server-0.9.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-20 13:38:36.000000 quetz-server-0.9.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-20 13:38:36.000000 quetz-server-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-20 13:38:36.000000 quetz-server-0.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    18021 2023-06-20 13:38:58.799596 quetz-server-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17446 2023-06-20 13:38:36.000000 quetz-server-0.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-20 13:38:36.000000 quetz-server-0.9.1/RELEASE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-20 13:38:36.000000 quetz-server-0.9.1/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-20 13:38:36.000000 quetz-server-0.9.1/dev_config.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:38:58.775596 quetz-server-0.9.1/docker/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-20 13:38:36.000000 quetz-server-0.9.1/docker/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-20 13:38:36.000000 quetz-server-0.9.1/docker/Dockerfile.jupyterhub
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-20 13:38:36.000000 quetz-server-0.9.1/docker/docker_config.toml
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-20 13:38:36.000000 quetz-server-0.9.1/docker/grafana.env
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-20 13:38:36.000000 quetz-server-0.9.1/docker/graphana_datasources.yml
--rw-r--r--   0 runner    (1001) docker     (123)    44096 2023-06-20 13:38:36.000000 quetz-server-0.9.1/docker/jupyterhub_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-20 13:38:36.000000 quetz-server-0.9.1/docker/nginx.conf
--rw-r--r--   0 runner    (1001) docker     (123)    26521 2023-06-20 13:38:36.000000 quetz-server-0.9.1/docker/postgres.conf
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-20 13:38:36.000000 quetz-server-0.9.1/docker/postgres.env
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-20 13:38:36.000000 quetz-server-0.9.1/docker/prometheus.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      272 2023-06-20 13:38:36.000000 quetz-server-0.9.1/docker/wait-for-postgres.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-06-20 13:38:36.000000 quetz-server-0.9.1/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:38:58.779595 quetz-server-0.9.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-20 13:38:36.000000 quetz-server-0.9.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:38:58.779595 quetz-server-0.9.1/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    40864 2023-06-20 13:38:36.000000 quetz-server-0.9.1/docs/assets/quetz_header.png
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-20 13:38:36.000000 quetz-server-0.9.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:38:58.779595 quetz-server-0.9.1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:38:58.779595 quetz-server-0.9.1/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-20 13:38:36.000000 quetz-server-0.9.1/docs/source/_static/quetz_favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    26122 2023-06-20 13:38:36.000000 quetz-server-0.9.1/docs/source/_static/quetz_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-20 13:38:36.000000 quetz-server-0.9.1/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:38:58.779595 quetz-server-0.9.1/docs/source/deploying/
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-06-20 13:38:36.000000 quetz-server-0.9.1/docs/source/deploying/authenticators.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-06-20 13:38:36.000000 quetz-server-0.9.1/docs/source/deploying/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-20 13:38:36.000000 quetz-server-0.9.1/docs/source/deploying/database.rst
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-20 13:38:36.000000 quetz-server-0.9.1/docs/source/deploying/frontend.rst
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-20 13:38:36.000000 quetz-server-0.9.1/docs/source/deploying/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-06-20 13:38:36.000000 quetz-server-0.9.1/docs/source/deploying/migrations.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-06-20 13:38:36.000000 quetz-server-0.9.1/docs/source/deploying/nginx.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-06-20 13:38:36.000000 quetz-server-0.9.1/docs/source/deploying/workers.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-20 13:38:36.000000 quetz-server-0.9.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-06-20 13:38:36.000000 quetz-server-0.9.1/docs/source/plugins.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:38:58.779595 quetz-server-0.9.1/docs/source/qeps/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-20 13:38:36.000000 quetz-server-0.9.1/docs/source/qeps/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-06-20 13:38:36.000000 quetz-server-0.9.1/docs/source/qeps/qep-001-user-permissions.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:38:58.779595 quetz-server-0.9.1/docs/source/using/
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-20 13:38:36.000000 quetz-server-0.9.1/docs/source/using/basics.rst
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-20 13:38:36.000000 quetz-server-0.9.1/docs/source/using/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9431 2023-06-20 13:38:36.000000 quetz-server-0.9.1/docs/source/using/mirroring.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      410 2023-06-20 13:38:36.000000 quetz-server-0.9.1/download-test-package.sh
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-20 13:38:36.000000 quetz-server-0.9.1/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-06-20 13:38:36.000000 quetz-server-0.9.1/init_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-06-20 13:38:44.000000 quetz-server-0.9.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:38:58.783596 quetz-server-0.9.1/quetz/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-20 13:38:44.000000 quetz-server-0.9.1/quetz/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:38:58.783596 quetz-server-0.9.1/quetz/authentication/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/authentication/auth_dao.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/authentication/azuread.py
--rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/authentication/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/authentication/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/authentication/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/authentication/google.py
--rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/authentication/jupyterhub.py
--rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/authentication/oauth2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/authentication/pam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/authentication/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/authorization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:38:58.787596 quetz-server-0.9.1/quetz/basic_frontend/
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/basic_frontend/avatar.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/basic_frontend/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/basic_frontend/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/channel_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    23996 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/condainfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    20496 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/config.toml
--rw-r--r--   0 runner    (1001) docker     (123)    42862 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/dao.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/database_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11299 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/db_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/deps.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:38:58.787596 quetz-server-0.9.1/quetz/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/jobs/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/jobs/dao.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/jobs/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/jobs/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/jobs/rest_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    12029 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/jobs/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    57633 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:38:58.787596 quetz-server-0.9.1/quetz/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/metrics/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/metrics/db_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/metrics/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/metrics/rest_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/metrics/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/metrics/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:38:58.787596 quetz-server-0.9.1/quetz/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/migrations/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/migrations/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:38:58.791596 quetz-server-0.9.1/quetz/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/migrations/versions/0653794b6252_adding_url_and_platforms_dirs.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/migrations/versions/0a0ab48887ab_adding_function_args_to_job_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/migrations/versions/30241b33d849_add_task_pending_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/migrations/versions/303ff70c27fc_configure_mirror_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/migrations/versions/3c3288034362_add_channel_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/migrations/versions/53f81aba78ce_use_biginteger_for_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/migrations/versions/794249a0b1bd_adding_jobs_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/migrations/versions/8d1e9a9e0b1f_adding_download_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/migrations/versions/8dfb7c4bfbd7_new_package_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/migrations/versions/98c04a65df4a_register_mirrors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/migrations/versions/a3ffa287d074_case_insensitive_channel_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     9084 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/migrations/versions/a80fb051a659_create_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/migrations/versions/b9886d9cadb0_create_indexes_for_download_count_.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/migrations/versions/cd404ed93cc0_add_per_channel_ttl.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/migrations/versions/cddba8e6e639_scheduling_spec_for_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/migrations/versions/d212023a8e0b_add_useremail_table_for_email_addresses.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/migrations/versions/db1c56bf4d57_add_channel_size_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/migrations/versions/ea6eba9a9ffc_merge_ebe550f9fbbe_and_b9886d9cadb0.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/migrations/versions/ebe550f9fbbe_added_create_at_and_expire_at_date_to_.py
--rw-r--r--   0 runner    (1001) docker     (123)    26855 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/pkgstores.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/repo_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8571 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/rest_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:38:58.791596 quetz-server-0.9.1/quetz/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/tasks/assertions.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/tasks/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/tasks/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/tasks/indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)    18320 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/tasks/mirror.py
--rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/tasks/reindexing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9671 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/tasks/workers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:38:58.791596 quetz-server-0.9.1/quetz/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/templates/channeldata-index.html.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/templates/subdir-index.html.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:38:58.791596 quetz-server-0.9.1/quetz/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/testing/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/testing/mockups.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/testing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:38:58.795596 quetz-server-0.9.1/quetz/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:38:58.795596 quetz-server-0.9.1/quetz/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/tests/api/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/tests/api/test_api_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)    22577 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/tests/api/test_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/tests/api/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    23467 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/tests/api/test_main_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)     9173 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/tests/api/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/tests/api/test_users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:38:58.795596 quetz-server-0.9.1/quetz/tests/authentification/
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/tests/authentification/test_auth_dao.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/tests/authentification/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17757 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/tests/authentification/test_oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/tests/authentification/test_pam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:38:58.795596 quetz-server-0.9.1/quetz/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:38:58.771596 quetz-server-0.9.1/quetz/tests/data/dummy-plugin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:38:58.795596 quetz-server-0.9.1/quetz/tests/data/dummy-plugin/quetz_dummyplugin/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/tests/data/dummy-plugin/quetz_dummyplugin/jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:38:58.795596 quetz-server-0.9.1/quetz/tests/data/dummy-plugin/quetz_dummyplugin-1.0-py3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/tests/data/dummy-plugin/quetz_dummyplugin-1.0-py3.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/tests/data/dummy-plugin/quetz_dummyplugin-1.0-py3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/tests/data/other-package-0.1-0.tar.bz2
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/tests/data/other-package-0.2-0.tar.bz2
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/tests/data/test-package-0.1-0.tar.bz2
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/tests/data/test-package-0.1-0_copy.tar.bz2
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/tests/data/test-package-0.2-0.tar.bz2
--rw-r--r--   0 runner    (1001) docker     (123)    20798 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    18709 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13028 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/tests/test_dao.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/tests/test_db_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/tests/test_health.py
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/tests/test_indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)    27357 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)    38275 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/tests/test_mirror.py
--rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/tests/test_pkg_stores.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/tests/test_profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/tests/test_versionorder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/tests/test_workers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8985 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11429 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz/versionorder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:38:58.799596 quetz-server-0.9.1/quetz_db_ext/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz_db_ext/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz_db_ext/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz_db_ext/LIBSOLV_LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14617 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz_db_ext/conda.c
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz_db_ext/conda.h
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz_db_ext/quetz_pg.c
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-20 13:38:36.000000 quetz-server-0.9.1/quetz_db_ext/quetz_sqlite.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:38:58.799596 quetz-server-0.9.1/quetz_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18021 2023-06-20 13:38:58.000000 quetz-server-0.9.1/quetz_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-06-20 13:38:58.000000 quetz-server-0.9.1/quetz_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 13:38:58.000000 quetz-server-0.9.1/quetz_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-20 13:38:58.000000 quetz-server-0.9.1/quetz_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-20 13:38:58.000000 quetz-server-0.9.1/quetz_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 13:38:58.000000 quetz-server-0.9.1/quetz_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-20 13:38:58.799596 quetz-server-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 13:38:36.000000 quetz-server-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:20:20.650103 quetz-server-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-21 11:20:03.000000 quetz-server-0.9.2/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-21 11:20:03.000000 quetz-server-0.9.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-21 11:20:03.000000 quetz-server-0.9.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    25649 2023-06-21 11:20:11.000000 quetz-server-0.9.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-21 11:20:03.000000 quetz-server-0.9.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-21 11:20:03.000000 quetz-server-0.9.2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-21 11:20:03.000000 quetz-server-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-21 11:20:03.000000 quetz-server-0.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18021 2023-06-21 11:20:20.650103 quetz-server-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17446 2023-06-21 11:20:03.000000 quetz-server-0.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-21 11:20:03.000000 quetz-server-0.9.2/RELEASE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-21 11:20:03.000000 quetz-server-0.9.2/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-21 11:20:03.000000 quetz-server-0.9.2/dev_config.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:20:20.630102 quetz-server-0.9.2/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-21 11:20:03.000000 quetz-server-0.9.2/docker/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-21 11:20:03.000000 quetz-server-0.9.2/docker/Dockerfile.jupyterhub
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-21 11:20:03.000000 quetz-server-0.9.2/docker/docker_config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-21 11:20:03.000000 quetz-server-0.9.2/docker/grafana.env
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-21 11:20:03.000000 quetz-server-0.9.2/docker/graphana_datasources.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    44096 2023-06-21 11:20:03.000000 quetz-server-0.9.2/docker/jupyterhub_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-21 11:20:03.000000 quetz-server-0.9.2/docker/nginx.conf
+-rw-r--r--   0 runner    (1001) docker     (123)    26521 2023-06-21 11:20:03.000000 quetz-server-0.9.2/docker/postgres.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-21 11:20:03.000000 quetz-server-0.9.2/docker/postgres.env
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-21 11:20:03.000000 quetz-server-0.9.2/docker/prometheus.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      272 2023-06-21 11:20:03.000000 quetz-server-0.9.2/docker/wait-for-postgres.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-06-21 11:20:03.000000 quetz-server-0.9.2/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:20:20.630102 quetz-server-0.9.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-21 11:20:03.000000 quetz-server-0.9.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:20:20.630102 quetz-server-0.9.2/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    40864 2023-06-21 11:20:03.000000 quetz-server-0.9.2/docs/assets/quetz_header.png
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-21 11:20:03.000000 quetz-server-0.9.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:20:20.630102 quetz-server-0.9.2/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:20:20.630102 quetz-server-0.9.2/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-21 11:20:03.000000 quetz-server-0.9.2/docs/source/_static/quetz_favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    26122 2023-06-21 11:20:03.000000 quetz-server-0.9.2/docs/source/_static/quetz_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-21 11:20:03.000000 quetz-server-0.9.2/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:20:20.634102 quetz-server-0.9.2/docs/source/deploying/
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-06-21 11:20:03.000000 quetz-server-0.9.2/docs/source/deploying/authenticators.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11547 2023-06-21 11:20:03.000000 quetz-server-0.9.2/docs/source/deploying/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-21 11:20:03.000000 quetz-server-0.9.2/docs/source/deploying/database.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-21 11:20:03.000000 quetz-server-0.9.2/docs/source/deploying/frontend.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-21 11:20:03.000000 quetz-server-0.9.2/docs/source/deploying/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-06-21 11:20:03.000000 quetz-server-0.9.2/docs/source/deploying/migrations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-06-21 11:20:03.000000 quetz-server-0.9.2/docs/source/deploying/nginx.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-06-21 11:20:03.000000 quetz-server-0.9.2/docs/source/deploying/workers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-21 11:20:03.000000 quetz-server-0.9.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-06-21 11:20:03.000000 quetz-server-0.9.2/docs/source/plugins.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:20:20.634102 quetz-server-0.9.2/docs/source/qeps/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-21 11:20:03.000000 quetz-server-0.9.2/docs/source/qeps/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-06-21 11:20:03.000000 quetz-server-0.9.2/docs/source/qeps/qep-001-user-permissions.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:20:20.634102 quetz-server-0.9.2/docs/source/using/
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-21 11:20:03.000000 quetz-server-0.9.2/docs/source/using/basics.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-21 11:20:03.000000 quetz-server-0.9.2/docs/source/using/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9431 2023-06-21 11:20:03.000000 quetz-server-0.9.2/docs/source/using/mirroring.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      410 2023-06-21 11:20:03.000000 quetz-server-0.9.2/download-test-package.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-21 11:20:03.000000 quetz-server-0.9.2/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-06-21 11:20:03.000000 quetz-server-0.9.2/init_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-06-21 11:20:09.000000 quetz-server-0.9.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:20:20.634102 quetz-server-0.9.2/quetz/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-21 11:20:09.000000 quetz-server-0.9.2/quetz/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:20:20.638103 quetz-server-0.9.2/quetz/authentication/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/authentication/auth_dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/authentication/azuread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/authentication/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/authentication/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/authentication/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/authentication/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/authentication/jupyterhub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/authentication/oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/authentication/pam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/authentication/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/authorization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:20:20.638103 quetz-server-0.9.2/quetz/basic_frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/basic_frontend/avatar.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/basic_frontend/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/basic_frontend/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/channel_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24855 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/condainfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20495 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    42862 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/database_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11299 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/db_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/deps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:20:20.638103 quetz-server-0.9.2/quetz/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/jobs/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/jobs/dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/jobs/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/jobs/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/jobs/rest_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12029 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/jobs/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57637 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:20:20.638103 quetz-server-0.9.2/quetz/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/metrics/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/metrics/db_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/metrics/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/metrics/rest_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/metrics/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/metrics/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:20:20.638103 quetz-server-0.9.2/quetz/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/migrations/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/migrations/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:20:20.642103 quetz-server-0.9.2/quetz/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/migrations/versions/0653794b6252_adding_url_and_platforms_dirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/migrations/versions/0a0ab48887ab_adding_function_args_to_job_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/migrations/versions/30241b33d849_add_task_pending_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/migrations/versions/303ff70c27fc_configure_mirror_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/migrations/versions/3c3288034362_add_channel_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/migrations/versions/53f81aba78ce_use_biginteger_for_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/migrations/versions/794249a0b1bd_adding_jobs_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/migrations/versions/8d1e9a9e0b1f_adding_download_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/migrations/versions/8dfb7c4bfbd7_new_package_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/migrations/versions/98c04a65df4a_register_mirrors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/migrations/versions/a3ffa287d074_case_insensitive_channel_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9084 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/migrations/versions/a80fb051a659_create_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/migrations/versions/b9886d9cadb0_create_indexes_for_download_count_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/migrations/versions/cd404ed93cc0_add_per_channel_ttl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/migrations/versions/cddba8e6e639_scheduling_spec_for_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/migrations/versions/d212023a8e0b_add_useremail_table_for_email_addresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/migrations/versions/db1c56bf4d57_add_channel_size_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/migrations/versions/ea6eba9a9ffc_merge_ebe550f9fbbe_and_b9886d9cadb0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/migrations/versions/ebe550f9fbbe_added_create_at_and_expire_at_date_to_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26855 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/pkgstores.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/repo_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8571 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/rest_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:20:20.642103 quetz-server-0.9.2/quetz/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/tasks/assertions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/tasks/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/tasks/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/tasks/indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18320 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/tasks/mirror.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/tasks/reindexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9671 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/tasks/workers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:20:20.642103 quetz-server-0.9.2/quetz/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/templates/channeldata-index.html.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/templates/subdir-index.html.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:20:20.642103 quetz-server-0.9.2/quetz/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/testing/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/testing/mockups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/testing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:20:20.646103 quetz-server-0.9.2/quetz/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:20:20.646103 quetz-server-0.9.2/quetz/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/tests/api/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/tests/api/test_api_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22577 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/tests/api/test_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/tests/api/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23467 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/tests/api/test_main_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9173 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/tests/api/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/tests/api/test_users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:20:20.646103 quetz-server-0.9.2/quetz/tests/authentification/
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/tests/authentification/test_auth_dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/tests/authentification/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17929 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/tests/authentification/test_oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/tests/authentification/test_pam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:20:20.646103 quetz-server-0.9.2/quetz/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:20:20.626102 quetz-server-0.9.2/quetz/tests/data/dummy-plugin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:20:20.646103 quetz-server-0.9.2/quetz/tests/data/dummy-plugin/quetz_dummyplugin/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/tests/data/dummy-plugin/quetz_dummyplugin/jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:20:20.646103 quetz-server-0.9.2/quetz/tests/data/dummy-plugin/quetz_dummyplugin-1.0-py3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/tests/data/dummy-plugin/quetz_dummyplugin-1.0-py3.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/tests/data/dummy-plugin/quetz_dummyplugin-1.0-py3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/tests/data/other-package-0.1-0.tar.bz2
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/tests/data/other-package-0.2-0.tar.bz2
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/tests/data/test-package-0.1-0.tar.bz2
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/tests/data/test-package-0.1-0_copy.tar.bz2
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/tests/data/test-package-0.2-0.tar.bz2
+-rw-r--r--   0 runner    (1001) docker     (123)    20798 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18709 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13028 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/tests/test_dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/tests/test_db_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/tests/test_health.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/tests/test_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27357 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38275 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/tests/test_mirror.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/tests/test_pkg_stores.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/tests/test_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/tests/test_versionorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/tests/test_workers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8985 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11429 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz/versionorder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:20:20.650103 quetz-server-0.9.2/quetz_db_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz_db_ext/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz_db_ext/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz_db_ext/LIBSOLV_LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14617 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz_db_ext/conda.c
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz_db_ext/conda.h
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz_db_ext/quetz_pg.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-21 11:20:03.000000 quetz-server-0.9.2/quetz_db_ext/quetz_sqlite.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:20:20.650103 quetz-server-0.9.2/quetz_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18021 2023-06-21 11:20:20.000000 quetz-server-0.9.2/quetz_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-06-21 11:20:20.000000 quetz-server-0.9.2/quetz_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 11:20:20.000000 quetz-server-0.9.2/quetz_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-21 11:20:20.000000 quetz-server-0.9.2/quetz_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-21 11:20:20.000000 quetz-server-0.9.2/quetz_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 11:20:20.000000 quetz-server-0.9.2/quetz_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-21 11:20:20.650103 quetz-server-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 11:20:03.000000 quetz-server-0.9.2/setup.py
```

### Comparing `quetz-server-0.9.1/.pre-commit-config.yaml` & `quetz-server-0.9.2/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -34,10 +34,10 @@
           - types-aiofiles
         args: [--show-error-codes]
   - repo: https://github.com/Quantco/pre-commit-mirrors-prettier
     rev: 2.7.1
     hooks:
       - id: prettier-conda
   - repo: https://github.com/RobertCraigie/pyright-python
-    rev: v1.1.294
+    rev: v1.1.314
     hooks:
       - id: pyright
```

### Comparing `quetz-server-0.9.1/CHANGELOG.md` & `quetz-server-0.9.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,33 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 0.9.2
+
+([Full Changelog](https://github.com/mamba-org/quetz/compare/v0.9.1...efd519fd840304fb73fe6fd31ee4ae7f010ab1a2))
+
+### Bugs fixed
+
+- Remove DB dependency for health endpoint [#652](https://github.com/mamba-org/quetz/pull/652) ([@AndreasAlbertQC](https://github.com/AndreasAlbertQC))
+- Do not pass pooling arguments to sqlite [#641](https://github.com/mamba-org/quetz/pull/641) ([@AndreasAlbertQC](https://github.com/AndreasAlbertQC))
+
+### Maintenance and upkeep improvements
+
+- Use PEP-593 Annotated for options and arguments in CLI commands [#644](https://github.com/mamba-org/quetz/pull/644) ([@rominf](https://github.com/rominf))
+- Bump pyright-python version [#643](https://github.com/mamba-org/quetz/pull/643) ([@rominf](https://github.com/rominf))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/mamba-org/quetz/graphs/contributors?from=2023-06-20&to=2023-06-21&type=c))
+
+[@AndreasAlbertQC](https://github.com/search?q=repo%3Amamba-org%2Fquetz+involves%3AAndreasAlbertQC+updated%3A2023-06-20..2023-06-21&type=Issues) | [@codecov-commenter](https://github.com/search?q=repo%3Amamba-org%2Fquetz+involves%3Acodecov-commenter+updated%3A2023-06-20..2023-06-21&type=Issues) | [@rominf](https://github.com/search?q=repo%3Amamba-org%2Fquetz+involves%3Arominf+updated%3A2023-06-20..2023-06-21&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 0.9.1
 
 ([Full Changelog](https://github.com/mamba-org/quetz/compare/v0.9.0...13f588cc16560c78927e4b2406a77958a62d5ca6))
 
 ### Bugs fixed
 
 - Fix event loop errors [#650](https://github.com/mamba-org/quetz/pull/650) ([@janjagusch](https://github.com/janjagusch))
@@ -16,16 +38,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/mamba-org/quetz/graphs/contributors?from=2023-06-05&to=2023-06-20&type=c))
 
 [@janjagusch](https://github.com/search?q=repo%3Amamba-org%2Fquetz+involves%3Ajanjagusch+updated%3A2023-06-05..2023-06-20&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 0.9.0
 
 ([Full Changelog](https://github.com/mamba-org/quetz/compare/v0.8.0...935be5b02961e952396ca1fac20e073ec8907062))
 
 ### Enhancements made
 
 - Add async friendly upload [#626](https://github.com/mamba-org/quetz/pull/626) ([@ivergara](https://github.com/ivergara))
```

### Comparing `quetz-server-0.9.1/CONTRIBUTING.md` & `quetz-server-0.9.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/Dockerfile` & `quetz-server-0.9.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/LICENSE` & `quetz-server-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/MANIFEST.in` & `quetz-server-0.9.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/PKG-INFO` & `quetz-server-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quetz-server
-Version: 0.9.1
+Version: 0.9.2
 Summary: The mamba-org server for conda packages
 Home-page: https://github.com/mamba-org/quetz
 Author: QuantStack & Quetz contributors
 Author-email: wolf.vollprecht@quantstack.net
 Keywords: conda,mamba,server
 Platform: Linux
 Platform: Mac OS X
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: quetz-server Version: 0.9.1 Summary: The mamba-org
+Metadata-Version: 2.1 Name: quetz-server Version: 0.9.2 Summary: The mamba-org
 server for conda packages Home-page: https://github.com/mamba-org/quetz Author:
 QuantStack & Quetz contributors Author-email: wolf.vollprecht@quantstack.net
 Keywords: conda,mamba,server Platform: Linux Platform: Mac OS X Requires-
 Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra: azure
 Provides-Extra: gcs Provides-Extra: pam Provides-Extra: postgre Provides-Extra:
 s3 Provides-Extra: all Provides-Extra: client Provides-Extra: dev Provides-
 Extra: test License-File: LICENSE ![quetz header image](docs/assets/
```

### Comparing `quetz-server-0.9.1/README.md` & `quetz-server-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/RELEASE.md` & `quetz-server-0.9.2/RELEASE.md`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/alembic.ini` & `quetz-server-0.9.2/alembic.ini`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/dev_config.toml` & `quetz-server-0.9.2/dev_config.toml`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/docker/Dockerfile` & `quetz-server-0.9.2/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/docker/docker_config.toml` & `quetz-server-0.9.2/docker/docker_config.toml`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/docker/jupyterhub_config.py` & `quetz-server-0.9.2/docker/jupyterhub_config.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/docker/nginx.conf` & `quetz-server-0.9.2/docker/nginx.conf`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/docker/postgres.conf` & `quetz-server-0.9.2/docker/postgres.conf`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/docker-compose.yml` & `quetz-server-0.9.2/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/docs/Makefile` & `quetz-server-0.9.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/docs/assets/quetz_header.png` & `quetz-server-0.9.2/docs/assets/quetz_header.png`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/docs/make.bat` & `quetz-server-0.9.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/docs/source/_static/quetz_favicon.ico` & `quetz-server-0.9.2/docs/source/_static/quetz_favicon.ico`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/docs/source/_static/quetz_logo.png` & `quetz-server-0.9.2/docs/source/_static/quetz_logo.png`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/docs/source/conf.py` & `quetz-server-0.9.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/docs/source/deploying/authenticators.rst` & `quetz-server-0.9.2/docs/source/deploying/authenticators.rst`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/docs/source/deploying/configuration.rst` & `quetz-server-0.9.2/docs/source/deploying/configuration.rst`

 * *Files 5% similar despite different names*

```diff
@@ -26,29 +26,31 @@
    database_plugin_path = ""
 
    # Passed directly to the "echo" argument of sqlalchemy.create_engine
    echo_sql = false
 
    # The pool size for sqlalchemy engine connections to postgres DBs
    # see https://docs.sqlalchemy.org/en/latest/core/pooling.html
-   postgres_pool_size = 100
+   # Ignored for sqlite data bases
+   postgres_pool_size = 10
 
    # The maximal number of overflow connections beyond the pool size
    # see https://docs.sqlalchemy.org/en/latest/core/pooling.html
+   # Ignored for sqlite data bases
    postgres_max_overflow = 100
 
 :database_url: URL of the database (may contain user credentials) prefixed with either ``sqlite://`` or ``postgresql://``.
 
 :database_plugin_path: Undocumented setting, unknown use, default: `""`.
 
 :echo_sql: Passed directly to the "echo" argument of sqlalchemy.create_engine, default: `false`.
 
-:postgres_pool_size: The pool size for sqlalchemy engine connections to postgres DBs. See `sqlalchemy docs <https://docs.sqlalchemy.org/en/latest/core/pooling.html>`_. Default: `100`
+:postgres_pool_size: The pool size for sqlalchemy engine connections to postgres DBs. See `sqlalchemy docs <https://docs.sqlalchemy.org/en/latest/core/pooling.html>`_. Ignored for sqlite data bases. Default: `10`
 
-:postgres_max_overflow: The maximal number of overflow connections beyond the pool size. See `sqlalchemy docs <https://docs.sqlalchemy.org/en/latest/core/pooling.html>`_. Default: `100`
+:postgres_max_overflow: The maximal number of overflow connections beyond the pool size. See `sqlalchemy docs <https://docs.sqlalchemy.org/en/latest/core/pooling.html>`_.  Ignored for sqlite data bases. Default: `100`
 
 ``github`` section
 ^^^^^^^^^^^^^^^^^^
 
 You can use github as identity provider, i.e., users will connect to quetz with their github accounts. To register quetz as a github application, please go to the URL: `<https://github.com/settings/applications/new>`_ and add your quetz application, than copy-and-paste the provided ``client_id`` and ``client_secret`` credentials in this section.
 
 :client_id:
```

### Comparing `quetz-server-0.9.1/docs/source/deploying/database.rst` & `quetz-server-0.9.2/docs/source/deploying/database.rst`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/docs/source/deploying/migrations.rst` & `quetz-server-0.9.2/docs/source/deploying/migrations.rst`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/docs/source/deploying/nginx.rst` & `quetz-server-0.9.2/docs/source/deploying/nginx.rst`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/docs/source/deploying/workers.rst` & `quetz-server-0.9.2/docs/source/deploying/workers.rst`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/docs/source/index.rst` & `quetz-server-0.9.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/docs/source/plugins.rst` & `quetz-server-0.9.2/docs/source/plugins.rst`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/docs/source/qeps/qep-001-user-permissions.rst` & `quetz-server-0.9.2/docs/source/qeps/qep-001-user-permissions.rst`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/docs/source/using/basics.rst` & `quetz-server-0.9.2/docs/source/using/basics.rst`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/docs/source/using/mirroring.rst` & `quetz-server-0.9.2/docs/source/using/mirroring.rst`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/environment.yml` & `quetz-server-0.9.2/environment.yml`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/init_db.py` & `quetz-server-0.9.2/init_db.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/pyproject.toml` & `quetz-server-0.9.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 [tool.jupyter-releaser.options]
 check-imports = ["quetz"]
 
 [tool.check-wheel-contents]
 ignore = ["W004"]
 
 [tool.tbump.version]
-current = "0.9.1"
+current = "0.9.2"
 regex = '''
   (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)
   ((?P<channel>a|b|rc|.dev)(?P<release>\d+))?
 '''
 
 [[tool.tbump.field]]
 name = "channel"
```

### Comparing `quetz-server-0.9.1/quetz/authentication/auth_dao.py` & `quetz-server-0.9.2/quetz/authentication/auth_dao.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/authentication/azuread.py` & `quetz-server-0.9.2/quetz/authentication/azuread.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/authentication/base.py` & `quetz-server-0.9.2/quetz/authentication/base.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/authentication/github.py` & `quetz-server-0.9.2/quetz/authentication/github.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/authentication/gitlab.py` & `quetz-server-0.9.2/quetz/authentication/gitlab.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/authentication/google.py` & `quetz-server-0.9.2/quetz/authentication/google.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/authentication/jupyterhub.py` & `quetz-server-0.9.2/quetz/authentication/jupyterhub.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/authentication/oauth2.py` & `quetz-server-0.9.2/quetz/authentication/oauth2.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,14 +81,15 @@
 
     @property
     def router(self):
         return self.handler.router
 
     def __init__(self, config: Config, client_kwargs=None, provider=None, app=None):
         super().__init__(config, provider, app)
+        self.client: OAuthAuthenticator
         if self.is_enabled:
             self.register(client_kwargs=client_kwargs)
 
     async def userinfo(self, request, token):
         raise NotImplementedError("subclasses need to implement userinfo")
 
     async def authenticate(self, request, data=None, dao=None, config=None):
```

### Comparing `quetz-server-0.9.1/quetz/authentication/pam.py` & `quetz-server-0.9.2/quetz/authentication/pam.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/authentication/registry.py` & `quetz-server-0.9.2/quetz/authentication/registry.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/authorization.py` & `quetz-server-0.9.2/quetz/authorization.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/basic_frontend/avatar.jpg` & `quetz-server-0.9.2/quetz/basic_frontend/avatar.jpg`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/basic_frontend/favicon.ico` & `quetz-server-0.9.2/quetz/basic_frontend/favicon.ico`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/basic_frontend/index.html` & `quetz-server-0.9.2/quetz/basic_frontend/index.html`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/channel_data.py` & `quetz-server-0.9.2/quetz/channel_data.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/cli.py` & `quetz-server-0.9.2/quetz/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import typer
 import uvicorn
 from alembic import command
 from alembic.config import Config as AlembicConfig
 from importlib_metadata import entry_points
 from sqlalchemy.orm.session import Session
 from sqlalchemy_utils.functions import database_exists
+from typing_extensions import Annotated
 
 from quetz import pkgstores
 from quetz.config import (
     Config,
     _env_config_file,
     _env_prefix,
     configure_logger,
@@ -322,29 +323,29 @@
                 return True
 
     return False
 
 
 @app.command()
 def init_db(
-    path: str = typer.Argument(None, help="The path of the deployment"),
+    path: Annotated[str, typer.Argument(help="The path of the deployment")],
 ):
     """init database and fill users from config file [users] sections"""
 
     logger.info("Initializing database")
 
     config = _get_config(path)
 
     with working_directory(path):
         _run_migrations(config.sqlalchemy_database_url)
 
 
 @app.command()
 def add_user_roles(
-    path: str = typer.Argument(None, help="The path of the deployment"),
+    path: Annotated[str, typer.Argument(help="The path of the deployment")],
 ):
     """Set user roles according to the values from config file [users] sections.
 
     This command will assign roles only if they were not set before
     (for example using API or an earlier setting in config). The only exception
     is that users who already have a role defined as default_role will have a
     new role set from the config.
@@ -360,60 +361,70 @@
     with working_directory(path):
         db = get_session(config.sqlalchemy_database_url)
         _set_user_roles(db, config)
 
 
 @app.command()
 def make_migrations(
-    path: str = typer.Argument(None, help="The path of the deployment"),
-    message: str = typer.Option(None, help="revision message"),
-    plugin: str = typer.Option("quetz", help="head or heads or plugin name"),
-    initialize: bool = typer.Option(False, help="initialize migrations"),
+    path: Annotated[str, typer.Argument(help="The path of the deployment")],
+    message: Annotated[str, typer.Option(help="revision message")],
+    plugin: Annotated[str, typer.Option(help="head or heads or plugin name")] = "quetz",
+    initialize: Annotated[bool, typer.Option(help="initialize migrations")] = False,
 ):
     """make database migrations for quetz or a plugin"""
 
     logger.info("Initializing database")
 
     config = _get_config(path)
 
     with working_directory(path):
         _make_migrations(config.sqlalchemy_database_url, message, plugin, initialize)
 
 
 @app.command()
 def create(
-    path: str = typer.Argument(
-        None,
-        help=(
-            "The directory in which the deployment will be created "
-            "(will be created if does not exist)"
-        ),
-    ),
-    copy_conf: str = typer.Option(
-        None, help="The configuration to copy from (e.g. dev_config.toml)"
-    ),
-    create_conf: bool = typer.Option(
-        False,
-        help="Enable/disable creation of a default configuration file",
-    ),
-    delete: bool = typer.Option(
-        False,
-        help="Delete the the deployment if it exists. "
-        "Must be specified with --copy-conf or --create-conf",
-    ),
-    exists_ok: bool = typer.Option(
-        False, help="Skip the creation if deployment already exists."
-    ),
-    dev: bool = typer.Option(
-        False,
-        help=(
-            "Enable/disable dev mode "
-            "(fills the database with test data and allows http access)"
+    path: Annotated[
+        str,
+        typer.Argument(
+            help=(
+                "The directory in which the deployment will be created "
+                "(will be created if does not exist)"
+            ),
         ),
-    ),
+    ],
+    copy_conf: Annotated[
+        Optional[str],
+        typer.Option(help="The configuration to copy from (e.g. dev_config.toml)"),
+    ] = None,
+    create_conf: Annotated[
+        bool,
+        typer.Option(
+            help="Enable/disable creation of a default configuration file",
+        ),
+    ] = False,
+    delete: Annotated[
+        bool,
+        typer.Option(
+            help="Delete the the deployment if it exists. "
+            "Must be specified with --copy-conf or --create-conf",
+        ),
+    ] = False,
+    exists_ok: Annotated[
+        bool,
+        typer.Option(help="Skip the creation if deployment already exists."),
+    ] = False,
+    dev: Annotated[
+        bool,
+        typer.Option(
+            help=(
+                "Enable/disable dev mode "
+                "(fills the database with test data and allows http access)"
+            ),
+        ),
+    ] = False,
 ):
     """Create a new Quetz deployment."""
 
     logger.info(f"creating new deployment in path {path}")
     deployment_folder = Path(path).resolve()
     config_file = deployment_folder / "config.toml"
 
@@ -504,32 +515,45 @@
         os.environ[_env_prefix + _env_config_file] = str(config_file.resolve())
 
     return config
 
 
 @app.command()
 def start(
-    path: str = typer.Argument(None, help="The path of the deployment"),
-    port: int = typer.Option(8000, help="The port to bind"),
-    host: str = typer.Option("127.0.0.1", help="The network interface to bind"),
-    proxy_headers: bool = typer.Option(True, help="Enable/disable X-Forwarded headers"),
-    log_level: LogLevel = typer.Option(
-        LogLevel.info,
-        help="Set the logging level",
-    ),
-    reload: bool = typer.Option(
-        False,
-        help=(
-            "Enable/disable automatic reloading of the server when sources are modified"
-        ),
-    ),
-    supervisor: bool = typer.Option(
-        True,
-        help="Start job supervisor with quetz",
-    ),
+    path: Annotated[
+        Optional[str], typer.Argument(help="The path of the deployment")
+    ] = None,
+    port: Annotated[int, typer.Option(help="The port to bind")] = 8000,
+    host: Annotated[
+        str, typer.Option(help="The network interface to bind")
+    ] = "127.0.0.1",
+    proxy_headers: Annotated[
+        bool, typer.Option(help="Enable/disable X-Forwarded headers")
+    ] = True,
+    log_level: Annotated[
+        LogLevel,
+        typer.Option(
+            help="Set the logging level",
+        ),
+    ] = LogLevel.info,
+    reload: Annotated[
+        bool,
+        typer.Option(
+            help=(
+                "Enable/disable automatic reloading of the server when sources are "
+                "modified"
+            ),
+        ),
+    ] = False,
+    supervisor: Annotated[
+        bool,
+        typer.Option(
+            help="Start job supervisor with quetz",
+        ),
+    ] = True,
 ) -> NoReturn:
     """Start a Quetz deployment.
 
     To be started, a deployment has to be already created.
     At this time, only Uvicorn is supported as manager.
     """
 
@@ -580,66 +604,82 @@
     if supervisor_process is not None:
         supervisor_process.terminate()
         supervisor_process.join()
 
 
 @app.command()
 def run(
-    path: str = typer.Argument(None, help="The path of the deployment"),
-    copy_conf: str = typer.Option(
-        None, help="The configuration to copy from (e.g. dev_config.toml)"
-    ),
-    create_conf: bool = typer.Option(
-        False,
-        help="Enable/disable creation of a default configuration file",
-    ),
-    delete: bool = typer.Option(
-        False,
-        help="Delete the the deployment if it exists. "
-        "Must be specified with --copy-conf or --create-conf",
-    ),
-    skip_if_exists: bool = typer.Option(
-        False, help="Skip the creation if deployment already exists."
-    ),
-    dev: bool = typer.Option(
-        False,
-        help=(
-            "Enable/disable dev mode "
-            "(fills the database with test data and allows http access)"
-        ),
-    ),
-    port: int = typer.Option(8000, help="The port to bind"),
-    host: str = typer.Option("127.0.0.1", help="The network interface to bind"),
-    proxy_headers: bool = typer.Option(True, help="Enable/disable X-Forwarded headers"),
-    log_level: LogLevel = typer.Option(
-        LogLevel.info,
-        help="Set the logging level",
-    ),
-    reload: bool = typer.Option(
-        False,
-        help=(
-            "Enable/disable automatic reloading of the server when sources are modified"
+    path: Annotated[str, typer.Argument(help="The path of the deployment")],
+    copy_conf: Annotated[
+        Optional[str],
+        typer.Option(help="The configuration to copy from (e.g. dev_config.toml)"),
+    ] = None,
+    create_conf: Annotated[
+        bool,
+        typer.Option(
+            help="Enable/disable creation of a default configuration file",
+        ),
+    ] = False,
+    delete: Annotated[
+        bool,
+        typer.Option(
+            help="Delete the the deployment if it exists. "
+            "Must be specified with --copy-conf or --create-conf",
+        ),
+    ] = False,
+    skip_if_exists: Annotated[
+        bool,
+        typer.Option(help="Skip the creation if deployment already exists."),
+    ] = False,
+    dev: Annotated[
+        bool,
+        typer.Option(
+            help=(
+                "Enable/disable dev mode "
+                "(fills the database with test data and allows http access)"
+            ),
+        ),
+    ] = False,
+    port: Annotated[int, typer.Option(help="The port to bind")] = 8000,
+    host: Annotated[
+        str, typer.Option(help="The network interface to bind")
+    ] = "127.0.0.1",
+    proxy_headers: Annotated[
+        bool, typer.Option(help="Enable/disable X-Forwarded headers")
+    ] = True,
+    log_level: Annotated[
+        LogLevel,
+        typer.Option(
+            help="Set the logging level",
+        ),
+    ] = LogLevel.info,
+    reload: Annotated[
+        bool,
+        typer.Option(
+            help="Enable/disable automatic reloading of the server when sources are "
+            "modified",
         ),
-    ),
+    ] = False,
 ) -> NoReturn:
     """Run a Quetz deployment.
 
     It performs sequentially create and start operations."""
 
     abs_path = os.path.abspath(path)
     create(abs_path, copy_conf, create_conf, delete, skip_if_exists, dev)
     start(abs_path, port, host, proxy_headers, log_level, reload)
 
 
 @app.command()
 def delete(
-    path: str = typer.Argument(None, help="The path of the deployment"),
-    force: bool = typer.Option(
-        False, help="Enable/disable removal without confirmation prompt"
-    ),
+    path: Annotated[str, typer.Argument(help="The path of the deployment")],
+    force: Annotated[
+        bool,
+        typer.Option(help="Enable/disable removal without confirmation prompt"),
+    ] = False,
 ) -> None:
     """Delete a Quetz deployment."""
 
     deployment_dir = Path(path)
     if not _is_deployment(deployment_dir):
         typer.echo(f'No Quetz deployment found at {path}.', err=True)
         raise typer.Abort()
@@ -648,15 +688,16 @@
         raise typer.Abort()
 
     shutil.rmtree(deployment_dir)
 
 
 @app.command()
 def plugin(
-    cmd: str, path: str = typer.Argument(None, help="Path to the plugin folder")
+    cmd: str,
+    path: Annotated[str, typer.Argument(help="Path to the plugin folder")],
 ) -> None:
     if cmd == 'install':
         abs_path = Path(path).absolute()
         if not (abs_path / "setup.py").exists():
             raise ValueError(f"Could not find any setup.py file in {abs_path}/.")
         requirements = abs_path / "conda-requirements.txt"
 
@@ -725,17 +766,18 @@
             logger.info("stopping supervisor")
         finally:
             db.close()
 
 
 @app.command()
 def watch_job_queue(
-    path: str = typer.Argument(None, help="Path to the plugin folder"),
-    num_procs: Optional[int] = typer.Option(
-        None, help="Number of processes to use. Default: number of CPU cores"
-    ),
+    path: Annotated[str, typer.Argument(help="Path to the plugin folder")],
+    num_procs: Annotated[
+        Optional[int],
+        typer.Option(help="Number of processes to use. Default: number of CPU cores"),
+    ] = None,
 ) -> None:
     start_supervisor_daemon(Path(path), num_procs)
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `quetz-server-0.9.1/quetz/condainfo.py` & `quetz-server-0.9.2/quetz/condainfo.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/config.py` & `quetz-server-0.9.2/quetz/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         ),
         ConfigSection(
             "sqlalchemy",
             [
                 ConfigEntry("database_url", str),
                 ConfigEntry("database_plugin_path", str, default="", required=False),
                 ConfigEntry("echo_sql", bool, default=False, required=False),
-                ConfigEntry("postgres_pool_size", int, default=100, required=False),
+                ConfigEntry("postgres_pool_size", int, default=10, required=False),
                 ConfigEntry("postgres_max_overflow", int, default=100, required=False),
             ],
         ),
         ConfigSection(
             "session",
             [ConfigEntry("secret", str), ConfigEntry("https_only", bool, default=True)],
         ),
```

### Comparing `quetz-server-0.9.1/quetz/dao.py` & `quetz-server-0.9.2/quetz/dao.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/database.py` & `quetz-server-0.9.2/quetz/database.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,28 +25,30 @@
     checked_in = engine.pool.checkedin()
     checked_out = engine.pool.checkedout()
     pool_size = checked_in + checked_out
     DATABASE_POOL_SIZE.set(pool_size)
     DATABASE_CONNECTIONS_USED.set(checked_out)
 
 
-def get_engine(db_url, reuse_engine=True, **kwargs) -> Engine:
+def get_engine(db_url, reuse_engine=True, postgres_kwargs=None, **kwargs) -> Engine:
     if db_url.startswith('sqlite'):
         kwargs.setdefault('connect_args', {'check_same_thread': False})
 
     if db_url.endswith(':memory:'):
         # If we're using an in-memory database, ensure that only one connection
         # is ever created.
         kwargs.setdefault('poolclass', StaticPool)
 
     global engine
 
     if not engine or not reuse_engine:
         if db_url.startswith('postgres'):
-            engine = create_engine(db_url, **kwargs)
+            engine = create_engine(
+                db_url, **(postgres_kwargs if postgres_kwargs else {}), **kwargs
+            )
             for event_name in ['connect', 'close', 'checkin', 'checkout']:
                 event.listen(engine, event_name, set_metrics)
         else:
             engine = create_engine(db_url, **kwargs)
 
         def on_connect(dbapi_conn, conn_record):
             logger.debug("connection opened: %s", engine.pool.status())
@@ -75,16 +77,18 @@
 
 @contextmanager
 def get_db_manager():
     config = Config()
     db = get_session(
         db_url=config.sqlalchemy_database_url,
         echo=config.sqlalchemy_echo_sql,
-        pool_size=config.sqlalchemy_postgres_pool_size,
-        max_overflow=config.sqlalchemy_postgres_max_overflow,
+        postgres_kwargs=dict(
+            pool_size=config.sqlalchemy_postgres_pool_size,
+            max_overflow=config.sqlalchemy_postgres_max_overflow,
+        ),
     )
 
     try:
         yield db
     finally:
         db.close()
```

### Comparing `quetz-server-0.9.1/quetz/database_extensions.py` & `quetz-server-0.9.2/quetz/database_extensions.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/db_models.py` & `quetz-server-0.9.2/quetz/db_models.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/deps.py` & `quetz-server-0.9.2/quetz/deps.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/frontend.py` & `quetz-server-0.9.2/quetz/frontend.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/hooks.py` & `quetz-server-0.9.2/quetz/hooks.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/jobs/api.py` & `quetz-server-0.9.2/quetz/jobs/api.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/jobs/dao.py` & `quetz-server-0.9.2/quetz/jobs/dao.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/jobs/handlers.py` & `quetz-server-0.9.2/quetz/jobs/handlers.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/jobs/models.py` & `quetz-server-0.9.2/quetz/jobs/models.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/jobs/rest_models.py` & `quetz-server-0.9.2/quetz/jobs/rest_models.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/jobs/runner.py` & `quetz-server-0.9.2/quetz/jobs/runner.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/main.py` & `quetz-server-0.9.2/quetz/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1859,12 +1859,12 @@
     dao: Dao = Depends(get_dao),
 ):
     return serve_path("index.html", channel, accept_encoding, session, dao)
 
 
 @app.get("/health/ready", status_code=status.HTTP_200_OK)
 @app.get("/health/live", status_code=status.HTTP_200_OK)
-def is_ready_live(task: Task = Depends(get_tasks_worker)):
-    return {}
+def is_ready_live():
+    return {"component": "http-server", "status": "ok"}
 
 
 frontend.register(app)
```

### Comparing `quetz-server-0.9.1/quetz/metrics/api.py` & `quetz-server-0.9.2/quetz/metrics/api.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/metrics/db_models.py` & `quetz-server-0.9.2/quetz/metrics/db_models.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/metrics/middleware.py` & `quetz-server-0.9.2/quetz/metrics/middleware.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/metrics/rest_models.py` & `quetz-server-0.9.2/quetz/metrics/rest_models.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/metrics/tasks.py` & `quetz-server-0.9.2/quetz/metrics/tasks.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/metrics/view.py` & `quetz-server-0.9.2/quetz/metrics/view.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/migrations/env.py` & `quetz-server-0.9.2/quetz/migrations/env.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/migrations/versions/0653794b6252_adding_url_and_platforms_dirs.py` & `quetz-server-0.9.2/quetz/migrations/versions/0653794b6252_adding_url_and_platforms_dirs.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/migrations/versions/0a0ab48887ab_adding_function_args_to_job_spec.py` & `quetz-server-0.9.2/quetz/migrations/versions/0a0ab48887ab_adding_function_args_to_job_spec.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/migrations/versions/30241b33d849_add_task_pending_state.py` & `quetz-server-0.9.2/quetz/migrations/versions/30241b33d849_add_task_pending_state.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/migrations/versions/303ff70c27fc_configure_mirror_endpoints.py` & `quetz-server-0.9.2/quetz/migrations/versions/303ff70c27fc_configure_mirror_endpoints.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/migrations/versions/3c3288034362_add_channel_metadata.py` & `quetz-server-0.9.2/quetz/migrations/versions/3c3288034362_add_channel_metadata.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/migrations/versions/53f81aba78ce_use_biginteger_for_size.py` & `quetz-server-0.9.2/quetz/migrations/versions/53f81aba78ce_use_biginteger_for_size.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/migrations/versions/794249a0b1bd_adding_jobs_tables.py` & `quetz-server-0.9.2/quetz/migrations/versions/794249a0b1bd_adding_jobs_tables.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/migrations/versions/8d1e9a9e0b1f_adding_download_metrics.py` & `quetz-server-0.9.2/quetz/migrations/versions/8d1e9a9e0b1f_adding_download_metrics.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/migrations/versions/8dfb7c4bfbd7_new_package_versions.py` & `quetz-server-0.9.2/quetz/migrations/versions/8dfb7c4bfbd7_new_package_versions.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/migrations/versions/98c04a65df4a_register_mirrors.py` & `quetz-server-0.9.2/quetz/migrations/versions/98c04a65df4a_register_mirrors.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/migrations/versions/a3ffa287d074_case_insensitive_channel_names.py` & `quetz-server-0.9.2/quetz/migrations/versions/a3ffa287d074_case_insensitive_channel_names.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/migrations/versions/a80fb051a659_create_tables.py` & `quetz-server-0.9.2/quetz/migrations/versions/a80fb051a659_create_tables.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/migrations/versions/b9886d9cadb0_create_indexes_for_download_count_.py` & `quetz-server-0.9.2/quetz/migrations/versions/b9886d9cadb0_create_indexes_for_download_count_.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/migrations/versions/cd404ed93cc0_add_per_channel_ttl.py` & `quetz-server-0.9.2/quetz/migrations/versions/cd404ed93cc0_add_per_channel_ttl.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/migrations/versions/cddba8e6e639_scheduling_spec_for_jobs.py` & `quetz-server-0.9.2/quetz/migrations/versions/cddba8e6e639_scheduling_spec_for_jobs.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/migrations/versions/d212023a8e0b_add_useremail_table_for_email_addresses.py` & `quetz-server-0.9.2/quetz/migrations/versions/d212023a8e0b_add_useremail_table_for_email_addresses.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/migrations/versions/db1c56bf4d57_add_channel_size_limit.py` & `quetz-server-0.9.2/quetz/migrations/versions/db1c56bf4d57_add_channel_size_limit.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/migrations/versions/ebe550f9fbbe_added_create_at_and_expire_at_date_to_.py` & `quetz-server-0.9.2/quetz/migrations/versions/ebe550f9fbbe_added_create_at_and_expire_at_date_to_.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/pkgstores.py` & `quetz-server-0.9.2/quetz/pkgstores.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/repo_data.py` & `quetz-server-0.9.2/quetz/repo_data.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/rest_models.py` & `quetz-server-0.9.2/quetz/rest_models.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/tasks/common.py` & `quetz-server-0.9.2/quetz/tasks/common.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/tasks/indexing.py` & `quetz-server-0.9.2/quetz/tasks/indexing.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/tasks/mirror.py` & `quetz-server-0.9.2/quetz/tasks/mirror.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/tasks/reindexing.py` & `quetz-server-0.9.2/quetz/tasks/reindexing.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/tasks/workers.py` & `quetz-server-0.9.2/quetz/tasks/workers.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/templates/channeldata-index.html.j2` & `quetz-server-0.9.2/quetz/templates/channeldata-index.html.j2`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/templates/subdir-index.html.j2` & `quetz-server-0.9.2/quetz/templates/subdir-index.html.j2`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/testing/fixtures.py` & `quetz-server-0.9.2/quetz/testing/fixtures.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/testing/mockups.py` & `quetz-server-0.9.2/quetz/testing/mockups.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/testing/utils.py` & `quetz-server-0.9.2/quetz/testing/utils.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/tests/api/conftest.py` & `quetz-server-0.9.2/quetz/tests/api/conftest.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/tests/api/test_api_keys.py` & `quetz-server-0.9.2/quetz/tests/api/test_api_keys.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/tests/api/test_channels.py` & `quetz-server-0.9.2/quetz/tests/api/test_channels.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/tests/api/test_main.py` & `quetz-server-0.9.2/quetz/tests/api/test_main.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/tests/api/test_main_packages.py` & `quetz-server-0.9.2/quetz/tests/api/test_main_packages.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/tests/api/test_metrics.py` & `quetz-server-0.9.2/quetz/tests/api/test_metrics.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/tests/api/test_users.py` & `quetz-server-0.9.2/quetz/tests/api/test_users.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/tests/authentification/test_auth_dao.py` & `quetz-server-0.9.2/quetz/tests/authentification/test_auth_dao.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/tests/authentification/test_base.py` & `quetz-server-0.9.2/quetz/tests/authentification/test_base.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/tests/authentification/test_oauth.py` & `quetz-server-0.9.2/quetz/tests/authentification/test_oauth.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import hashlib
 import time
 
 import pytest
 from authlib.jose import JsonWebKey, jwt
 from authlib.oidc.core.util import create_half_hash
 from fastapi.testclient import TestClient
 
@@ -218,31 +219,36 @@
 hlTXwdECgYAwqpJKC2Ls7i+3lSPomCNK1VtbVZzfHl1YrNy7y2Eo8DsFkcnHWZJ+
 qPCpHZ4sbgfziCRxOaGa+1kOXjhgXITPA/tkkhh4cglOvhHNBEVzdfHBMDxZd3HF
 mD1rl6xev7GRoqUYdKYdt9NJyDGEULZ6NbIWyXo3kTp7HdQLRn0BJg==
 -----END RSA PRIVATE KEY-----
 """
 
 
+@pytest.mark.skipif(
+    not hasattr(hashlib, "RS256"), reason="hashlib does not support RS256"
+)
 @pytest.fixture
 def google_response(login):
     google_client_id = 'aaa'
     key = GOOGLE_PRIVATE_KEY
     cert = GOOGLE_CERT
 
     user_claims = {
         "picture": "http://avatar",
         "name": "monalisa",
     }
     access_token = "b"
+    half_hash = create_half_hash(access_token, "RS256")
+    assert half_hash is not None
     payload = {
         "iss": "https://accounts.google.com",
         "azp": google_client_id,
         "aud": "1234987819200.apps.googleusercontent.com",
         "sub": login + "_id",
-        "at_hash": create_half_hash(access_token, "RS256").decode("ascii"),
+        "at_hash": half_hash.decode("ascii"),
         "hd": "example.com",
         "email": login,
         "email_verified": "true",
         "iat": int(time.time()),
         "exp": int(time.time()) + 100,
         "nonce": "0394852-3190485-2490358",
         **user_claims,
```

### Comparing `quetz-server-0.9.1/quetz/tests/authentification/test_pam.py` & `quetz-server-0.9.2/quetz/tests/authentification/test_pam.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/tests/conftest.py` & `quetz-server-0.9.2/quetz/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/tests/data/other-package-0.1-0.tar.bz2` & `quetz-server-0.9.2/quetz/tests/data/other-package-0.1-0.tar.bz2`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/tests/data/other-package-0.2-0.tar.bz2` & `quetz-server-0.9.2/quetz/tests/data/other-package-0.2-0.tar.bz2`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/tests/data/test-package-0.1-0.tar.bz2` & `quetz-server-0.9.2/quetz/tests/data/test-package-0.1-0.tar.bz2`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/tests/data/test-package-0.1-0_copy.tar.bz2` & `quetz-server-0.9.2/quetz/tests/data/test-package-0.1-0_copy.tar.bz2`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/tests/data/test-package-0.2-0.tar.bz2` & `quetz-server-0.9.2/quetz/tests/data/test-package-0.2-0.tar.bz2`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/tests/test_auth.py` & `quetz-server-0.9.2/quetz/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/tests/test_cli.py` & `quetz-server-0.9.2/quetz/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/tests/test_config.py` & `quetz-server-0.9.2/quetz/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/tests/test_dao.py` & `quetz-server-0.9.2/quetz/tests/test_dao.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/tests/test_database.py` & `quetz-server-0.9.2/quetz/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/tests/test_indexing.py` & `quetz-server-0.9.2/quetz/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/tests/test_jobs.py` & `quetz-server-0.9.2/quetz/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/tests/test_mirror.py` & `quetz-server-0.9.2/quetz/tests/test_mirror.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/tests/test_pkg_stores.py` & `quetz-server-0.9.2/quetz/tests/test_pkg_stores.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/tests/test_tasks.py` & `quetz-server-0.9.2/quetz/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/tests/test_versionorder.py` & `quetz-server-0.9.2/quetz/tests/test_versionorder.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/tests/test_workers.py` & `quetz-server-0.9.2/quetz/tests/test_workers.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/utils.py` & `quetz-server-0.9.2/quetz/utils.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz/versionorder.py` & `quetz-server-0.9.2/quetz/versionorder.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz_db_ext/CMakeLists.txt` & `quetz-server-0.9.2/quetz_db_ext/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz_db_ext/LIBSOLV_LICENSE.txt` & `quetz-server-0.9.2/quetz_db_ext/LIBSOLV_LICENSE.txt`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz_db_ext/conda.c` & `quetz-server-0.9.2/quetz_db_ext/conda.c`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz_db_ext/conda.h` & `quetz-server-0.9.2/quetz_db_ext/conda.h`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz_db_ext/quetz_pg.c` & `quetz-server-0.9.2/quetz_db_ext/quetz_pg.c`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz_db_ext/quetz_sqlite.c` & `quetz-server-0.9.2/quetz_db_ext/quetz_sqlite.c`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz_server.egg-info/PKG-INFO` & `quetz-server-0.9.2/quetz_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quetz-server
-Version: 0.9.1
+Version: 0.9.2
 Summary: The mamba-org server for conda packages
 Home-page: https://github.com/mamba-org/quetz
 Author: QuantStack & Quetz contributors
 Author-email: wolf.vollprecht@quantstack.net
 Keywords: conda,mamba,server
 Platform: Linux
 Platform: Mac OS X
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: quetz-server Version: 0.9.1 Summary: The mamba-org
+Metadata-Version: 2.1 Name: quetz-server Version: 0.9.2 Summary: The mamba-org
 server for conda packages Home-page: https://github.com/mamba-org/quetz Author:
 QuantStack & Quetz contributors Author-email: wolf.vollprecht@quantstack.net
 Keywords: conda,mamba,server Platform: Linux Platform: Mac OS X Requires-
 Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra: azure
 Provides-Extra: gcs Provides-Extra: pam Provides-Extra: postgre Provides-Extra:
 s3 Provides-Extra: all Provides-Extra: client Provides-Extra: dev Provides-
 Extra: test License-File: LICENSE ![quetz header image](docs/assets/
```

### Comparing `quetz-server-0.9.1/quetz_server.egg-info/SOURCES.txt` & `quetz-server-0.9.2/quetz_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/quetz_server.egg-info/requires.txt` & `quetz-server-0.9.2/quetz_server.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `quetz-server-0.9.1/setup.cfg` & `quetz-server-0.9.2/setup.cfg`

 * *Files identical despite different names*

