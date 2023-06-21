# Comparing `tmp/edc-0.4.98.tar.gz` & `tmp/edc-0.4.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-0.4.98.tar", last modified: Tue Jun 20 13:00:51 2023, max compression
+gzip compressed data, was "edc-0.4.99.tar", last modified: Wed Jun 21 14:18:42 2023, max compression
```

## Comparing `edc-0.4.98.tar` & `edc-0.4.99.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 jw         (502) staff       (20)        0 2023-06-20 13:00:51.665048 edc-0.4.98/
--rw-r--r--   0 jw         (502) staff       (20)     1410 2023-04-18 18:48:47.000000 edc-0.4.98/.gitignore
--rw-r--r--   0 jw         (502) staff       (20)     1076 2023-06-20 12:58:31.000000 edc-0.4.98/.pre-commit-config.yaml
--rw-r--r--   0 jw         (502) staff       (20)      291 2023-04-18 18:48:47.000000 edc-0.4.98/.yamllint
--rw-r--r--   0 jw         (502) staff       (20)        0 2023-04-18 18:48:47.000000 edc-0.4.98/AUTHORS
--rw-r--r--   0 jw         (502) staff       (20)    40367 2023-06-20 13:00:41.000000 edc-0.4.98/CHANGES
--rw-r--r--   0 jw         (502) staff       (20)    35147 2021-07-06 12:52:00.000000 edc-0.4.98/LICENSE
--rw-r--r--   0 jw         (502) staff       (20)      151 2021-07-06 12:52:00.000000 edc-0.4.98/MANIFEST.in
--rw-r--r--   0 jw         (502) staff       (20)    38295 2023-06-20 13:00:51.665327 edc-0.4.98/PKG-INFO
--rw-r--r--   0 jw         (502) staff       (20)    37432 2023-05-07 19:08:23.000000 edc-0.4.98/README.rst
-drwxr-xr-x   0 jw         (502) staff       (20)        0 2023-06-20 13:00:51.631015 edc-0.4.98/bin/
-drwxr-xr-x   0 jw         (502) staff       (20)        0 2023-06-20 13:00:51.637714 edc-0.4.98/bin/nginx/
--rw-r--r--   0 jw         (502) staff       (20)      350 2023-04-18 18:48:47.000000 edc-0.4.98/bin/nginx/edc-sites.conf
--rw-r--r--   0 jw         (502) staff       (20)      706 2023-04-18 18:48:47.000000 edc-0.4.98/bin/nginx/edc-uat.conf
--rw-r--r--   0 jw         (502) staff       (20)      656 2023-04-18 18:48:47.000000 edc-0.4.98/bin/nginx/edc.conf
-drwxr-xr-x   0 jw         (502) staff       (20)        0 2023-06-20 13:00:51.640611 edc-0.4.98/bin/scripts/
--rw-r--r--   0 jw         (502) staff       (20)     2753 2023-04-18 18:48:47.000000 edc-0.4.98/bin/scripts/dev_repos.sh
--rw-r--r--   0 jw         (502) staff       (20)      276 2021-07-06 12:52:00.000000 edc-0.4.98/bin/scripts/list_db_files.sh
--rw-r--r--   0 jw         (502) staff       (20)      416 2021-07-06 12:52:00.000000 edc-0.4.98/bin/scripts/restore_db_file.sh
--rw-r--r--   0 jw         (502) staff       (20)     2408 2023-04-18 18:48:47.000000 edc-0.4.98/bin/scripts/update_edc.sh
-drwxr-xr-x   0 jw         (502) staff       (20)        0 2023-06-20 13:00:51.643952 edc-0.4.98/bin/systemd/
--rw-r--r--   0 jw         (502) staff       (20)      835 2021-07-06 12:52:00.000000 edc-0.4.98/bin/systemd/celery-uat.service
--rw-r--r--   0 jw         (502) staff       (20)      820 2021-07-06 12:52:00.000000 edc-0.4.98/bin/systemd/celery.service
--rw-r--r--   0 jw         (502) staff       (20)      501 2021-07-06 12:52:00.000000 edc-0.4.98/bin/systemd/celerybeat-uat.service
--rw-r--r--   0 jw         (502) staff       (20)      487 2021-07-06 12:52:00.000000 edc-0.4.98/bin/systemd/celerybeat.service
--rw-r--r--   0 jw         (502) staff       (20)      485 2021-07-06 12:52:00.000000 edc-0.4.98/bin/systemd/gunicorn-uat.service
--rw-r--r--   0 jw         (502) staff       (20)      121 2021-07-06 12:52:00.000000 edc-0.4.98/bin/systemd/gunicorn-uat.socket
--rw-r--r--   0 jw         (502) staff       (20)      474 2021-07-06 12:52:00.000000 edc-0.4.98/bin/systemd/gunicorn.service
--rw-r--r--   0 jw         (502) staff       (20)      111 2021-07-06 12:52:00.000000 edc-0.4.98/bin/systemd/gunicorn.socket
-drwxr-xr-x   0 jw         (502) staff       (20)        0 2023-06-20 13:00:51.654791 edc-0.4.98/docs/
--rw-r--r--   0 jw         (502) staff       (20)      634 2023-04-18 18:48:47.000000 edc-0.4.98/docs/Makefile
--rw-r--r--   0 jw         (502) staff       (20)    12969 2023-05-07 19:08:23.000000 edc-0.4.98/docs/README.rst
--rw-r--r--   0 jw         (502) staff       (20)     4441 2023-04-18 18:48:47.000000 edc-0.4.98/docs/backup.rst
--rw-r--r--   0 jw         (502) staff       (20)     5437 2023-04-27 10:01:42.000000 edc-0.4.98/docs/celery.rst
--rw-r--r--   0 jw         (502) staff       (20)      580 2023-04-18 18:48:47.000000 edc-0.4.98/docs/conda.rst
--rw-r--r--   0 jw         (502) staff       (20)      975 2023-04-18 18:48:47.000000 edc-0.4.98/docs/conf.py
--rw-r--r--   0 jw         (502) staff       (20)     4806 2023-04-18 18:48:47.000000 edc-0.4.98/docs/configure_web_services.rst
--rw-r--r--   0 jw         (502) staff       (20)     3646 2023-04-18 18:48:47.000000 edc-0.4.98/docs/deploy_new_droplet.rst
--rw-r--r--   0 jw         (502) staff       (20)      163 2021-07-06 12:52:00.000000 edc-0.4.98/docs/dump_users.rst
--rw-r--r--   0 jw         (502) staff       (20)      845 2021-07-06 12:52:00.000000 edc-0.4.98/docs/exporting_encrypted_data.rst
--rw-r--r--   0 jw         (502) staff       (20)   258708 2023-04-18 18:48:47.000000 edc-0.4.98/docs/forms_reference.md
--rw-r--r--   0 jw         (502) staff       (20)      445 2023-04-18 18:48:47.000000 edc-0.4.98/docs/index.rst
--rw-r--r--   0 jw         (502) staff       (20)      778 2021-07-06 12:52:00.000000 edc-0.4.98/docs/landing_page.rst
--rw-r--r--   0 jw         (502) staff       (20)      765 2023-04-18 18:48:47.000000 edc-0.4.98/docs/make.bat
--rw-r--r--   0 jw         (502) staff       (20)        0 2021-07-06 12:52:00.000000 edc-0.4.98/docs/multisite_deployment.rst
--rw-r--r--   0 jw         (502) staff       (20)     3928 2023-04-18 18:48:47.000000 edc-0.4.98/docs/prepare_database.rst
--rw-r--r--   0 jw         (502) staff       (20)     1211 2023-04-18 18:48:47.000000 edc-0.4.98/docs/printing.rst
--rw-r--r--   0 jw         (502) staff       (20)      187 2021-07-06 12:52:00.000000 edc-0.4.98/docs/redis.rst
--rw-r--r--   0 jw         (502) staff       (20)      766 2021-07-06 12:52:00.000000 edc-0.4.98/docs/update_deployment.rst
-drwxr-xr-x   0 jw         (502) staff       (20)        0 2023-06-20 13:00:51.657302 edc-0.4.98/edc.egg-info/
--rw-r--r--   0 jw         (502) staff       (20)    38295 2023-06-20 13:00:51.000000 edc-0.4.98/edc.egg-info/PKG-INFO
--rw-r--r--   0 jw         (502) staff       (20)     1508 2023-06-20 13:00:51.000000 edc-0.4.98/edc.egg-info/SOURCES.txt
--rw-r--r--   0 jw         (502) staff       (20)        1 2023-06-20 13:00:51.000000 edc-0.4.98/edc.egg-info/dependency_links.txt
--rw-r--r--   0 jw         (502) staff       (20)        1 2021-09-27 09:58:54.000000 edc-0.4.98/edc.egg-info/not-zip-safe
--rw-r--r--   0 jw         (502) staff       (20)     1923 2023-06-20 13:00:51.000000 edc-0.4.98/edc.egg-info/requires.txt
--rw-r--r--   0 jw         (502) staff       (20)        6 2023-06-20 13:00:51.000000 edc-0.4.98/edc.egg-info/top_level.txt
-drwxr-xr-x   0 jw         (502) staff       (20)        0 2023-06-20 13:00:51.657598 edc-0.4.98/image/
--rw-r--r--   0 jw         (502) staff       (20)   160721 2021-08-24 11:21:23.000000 edc-0.4.98/image/icon-pycharm.png
--rw-r--r--   0 jw         (502) staff       (20)      162 2023-04-18 18:48:47.000000 edc-0.4.98/pyproject.toml
-drwxr-xr-x   0 jw         (502) staff       (20)        0 2023-06-20 13:00:51.664001 edc-0.4.98/requirements.tests/
--rw-r--r--   0 jw         (502) staff       (20)       21 2023-04-18 18:48:47.000000 edc-0.4.98/requirements.tests/coverage.txt
--rw-r--r--   0 jw         (502) staff       (20)       14 2023-04-18 18:48:47.000000 edc-0.4.98/requirements.tests/docs.txt
--rw-r--r--   0 jw         (502) staff       (20)     1053 2023-05-07 19:16:29.000000 edc-0.4.98/requirements.tests/edc.txt
--rw-r--r--   0 jw         (502) staff       (20)     4100 2023-04-18 18:48:47.000000 edc-0.4.98/requirements.tests/edc_dev.txt
--rw-r--r--   0 jw         (502) staff       (20)       68 2021-07-06 12:52:00.000000 edc-0.4.98/requirements.tests/edc_offline.txt
--rw-r--r--   0 jw         (502) staff       (20)       54 2023-04-18 18:48:47.000000 edc-0.4.98/requirements.tests/lint.txt
--rw-r--r--   0 jw         (502) staff       (20)       11 2023-04-18 18:48:47.000000 edc-0.4.98/requirements.tests/mysql.txt
--rw-r--r--   0 jw         (502) staff       (20)       22 2021-07-06 12:52:00.000000 edc-0.4.98/requirements.tests/postgres.txt
--rw-r--r--   0 jw         (502) staff       (20)       86 2023-04-18 18:48:47.000000 edc-0.4.98/requirements.tests/test_utils.txt
--rw-r--r--   0 jw         (502) staff       (20)      238 2023-04-18 18:48:47.000000 edc-0.4.98/requirements.tests/third_party_dev.txt
--rw-r--r--   0 jw         (502) staff       (20)       50 2023-04-18 18:48:47.000000 edc-0.4.98/requirements.tests/tox.txt
--rw-r--r--   0 jw         (502) staff       (20)     2995 2023-06-20 13:00:51.666222 edc-0.4.98/setup.cfg
-drwxr-xr-x   0 jw         (502) staff       (20)        0 2023-06-20 13:00:51.664633 edc-0.4.98/utils/
--rw-r--r--   0 jw         (502) staff       (20)        0 2021-07-06 12:52:00.000000 edc-0.4.98/utils/__init__.py
--rw-r--r--   0 jw         (502) staff       (20)      721 2023-04-18 18:48:47.000000 edc-0.4.98/utils/get_edc_requirements.py
+drwxr-xr-x   0 jw         (502) staff       (20)        0 2023-06-21 14:18:42.177269 edc-0.4.99/
+-rw-r--r--   0 jw         (502) staff       (20)     1410 2023-04-18 18:48:47.000000 edc-0.4.99/.gitignore
+-rw-r--r--   0 jw         (502) staff       (20)     1076 2023-06-20 12:58:31.000000 edc-0.4.99/.pre-commit-config.yaml
+-rw-r--r--   0 jw         (502) staff       (20)      291 2023-04-18 18:48:47.000000 edc-0.4.99/.yamllint
+-rw-r--r--   0 jw         (502) staff       (20)        0 2023-04-18 18:48:47.000000 edc-0.4.99/AUTHORS
+-rw-r--r--   0 jw         (502) staff       (20)    40501 2023-06-21 14:18:31.000000 edc-0.4.99/CHANGES
+-rw-r--r--   0 jw         (502) staff       (20)    35147 2021-07-06 12:52:00.000000 edc-0.4.99/LICENSE
+-rw-r--r--   0 jw         (502) staff       (20)      151 2021-07-06 12:52:00.000000 edc-0.4.99/MANIFEST.in
+-rw-r--r--   0 jw         (502) staff       (20)    38295 2023-06-21 14:18:42.177508 edc-0.4.99/PKG-INFO
+-rw-r--r--   0 jw         (502) staff       (20)    37432 2023-05-07 19:08:23.000000 edc-0.4.99/README.rst
+drwxr-xr-x   0 jw         (502) staff       (20)        0 2023-06-21 14:18:42.144749 edc-0.4.99/bin/
+drwxr-xr-x   0 jw         (502) staff       (20)        0 2023-06-21 14:18:42.152889 edc-0.4.99/bin/nginx/
+-rw-r--r--   0 jw         (502) staff       (20)      350 2023-04-18 18:48:47.000000 edc-0.4.99/bin/nginx/edc-sites.conf
+-rw-r--r--   0 jw         (502) staff       (20)      706 2023-04-18 18:48:47.000000 edc-0.4.99/bin/nginx/edc-uat.conf
+-rw-r--r--   0 jw         (502) staff       (20)      656 2023-04-18 18:48:47.000000 edc-0.4.99/bin/nginx/edc.conf
+drwxr-xr-x   0 jw         (502) staff       (20)        0 2023-06-21 14:18:42.155165 edc-0.4.99/bin/scripts/
+-rw-r--r--   0 jw         (502) staff       (20)     2753 2023-04-18 18:48:47.000000 edc-0.4.99/bin/scripts/dev_repos.sh
+-rw-r--r--   0 jw         (502) staff       (20)      276 2021-07-06 12:52:00.000000 edc-0.4.99/bin/scripts/list_db_files.sh
+-rw-r--r--   0 jw         (502) staff       (20)      416 2021-07-06 12:52:00.000000 edc-0.4.99/bin/scripts/restore_db_file.sh
+-rw-r--r--   0 jw         (502) staff       (20)     2408 2023-04-18 18:48:47.000000 edc-0.4.99/bin/scripts/update_edc.sh
+drwxr-xr-x   0 jw         (502) staff       (20)        0 2023-06-21 14:18:42.158560 edc-0.4.99/bin/systemd/
+-rw-r--r--   0 jw         (502) staff       (20)      835 2021-07-06 12:52:00.000000 edc-0.4.99/bin/systemd/celery-uat.service
+-rw-r--r--   0 jw         (502) staff       (20)      820 2021-07-06 12:52:00.000000 edc-0.4.99/bin/systemd/celery.service
+-rw-r--r--   0 jw         (502) staff       (20)      501 2021-07-06 12:52:00.000000 edc-0.4.99/bin/systemd/celerybeat-uat.service
+-rw-r--r--   0 jw         (502) staff       (20)      487 2021-07-06 12:52:00.000000 edc-0.4.99/bin/systemd/celerybeat.service
+-rw-r--r--   0 jw         (502) staff       (20)      485 2021-07-06 12:52:00.000000 edc-0.4.99/bin/systemd/gunicorn-uat.service
+-rw-r--r--   0 jw         (502) staff       (20)      121 2021-07-06 12:52:00.000000 edc-0.4.99/bin/systemd/gunicorn-uat.socket
+-rw-r--r--   0 jw         (502) staff       (20)      474 2021-07-06 12:52:00.000000 edc-0.4.99/bin/systemd/gunicorn.service
+-rw-r--r--   0 jw         (502) staff       (20)      111 2021-07-06 12:52:00.000000 edc-0.4.99/bin/systemd/gunicorn.socket
+drwxr-xr-x   0 jw         (502) staff       (20)        0 2023-06-21 14:18:42.167423 edc-0.4.99/docs/
+-rw-r--r--   0 jw         (502) staff       (20)      634 2023-04-18 18:48:47.000000 edc-0.4.99/docs/Makefile
+-rw-r--r--   0 jw         (502) staff       (20)    12969 2023-05-07 19:08:23.000000 edc-0.4.99/docs/README.rst
+-rw-r--r--   0 jw         (502) staff       (20)     4441 2023-04-18 18:48:47.000000 edc-0.4.99/docs/backup.rst
+-rw-r--r--   0 jw         (502) staff       (20)     5437 2023-04-27 10:01:42.000000 edc-0.4.99/docs/celery.rst
+-rw-r--r--   0 jw         (502) staff       (20)      580 2023-04-18 18:48:47.000000 edc-0.4.99/docs/conda.rst
+-rw-r--r--   0 jw         (502) staff       (20)      975 2023-04-18 18:48:47.000000 edc-0.4.99/docs/conf.py
+-rw-r--r--   0 jw         (502) staff       (20)     4806 2023-04-18 18:48:47.000000 edc-0.4.99/docs/configure_web_services.rst
+-rw-r--r--   0 jw         (502) staff       (20)     3646 2023-04-18 18:48:47.000000 edc-0.4.99/docs/deploy_new_droplet.rst
+-rw-r--r--   0 jw         (502) staff       (20)      163 2021-07-06 12:52:00.000000 edc-0.4.99/docs/dump_users.rst
+-rw-r--r--   0 jw         (502) staff       (20)      845 2021-07-06 12:52:00.000000 edc-0.4.99/docs/exporting_encrypted_data.rst
+-rw-r--r--   0 jw         (502) staff       (20)   258708 2023-04-18 18:48:47.000000 edc-0.4.99/docs/forms_reference.md
+-rw-r--r--   0 jw         (502) staff       (20)      445 2023-04-18 18:48:47.000000 edc-0.4.99/docs/index.rst
+-rw-r--r--   0 jw         (502) staff       (20)      778 2021-07-06 12:52:00.000000 edc-0.4.99/docs/landing_page.rst
+-rw-r--r--   0 jw         (502) staff       (20)      765 2023-04-18 18:48:47.000000 edc-0.4.99/docs/make.bat
+-rw-r--r--   0 jw         (502) staff       (20)        0 2021-07-06 12:52:00.000000 edc-0.4.99/docs/multisite_deployment.rst
+-rw-r--r--   0 jw         (502) staff       (20)     3928 2023-04-18 18:48:47.000000 edc-0.4.99/docs/prepare_database.rst
+-rw-r--r--   0 jw         (502) staff       (20)     1211 2023-04-18 18:48:47.000000 edc-0.4.99/docs/printing.rst
+-rw-r--r--   0 jw         (502) staff       (20)      187 2021-07-06 12:52:00.000000 edc-0.4.99/docs/redis.rst
+-rw-r--r--   0 jw         (502) staff       (20)      766 2021-07-06 12:52:00.000000 edc-0.4.99/docs/update_deployment.rst
+drwxr-xr-x   0 jw         (502) staff       (20)        0 2023-06-21 14:18:42.169774 edc-0.4.99/edc.egg-info/
+-rw-r--r--   0 jw         (502) staff       (20)    38295 2023-06-21 14:18:42.000000 edc-0.4.99/edc.egg-info/PKG-INFO
+-rw-r--r--   0 jw         (502) staff       (20)     1508 2023-06-21 14:18:42.000000 edc-0.4.99/edc.egg-info/SOURCES.txt
+-rw-r--r--   0 jw         (502) staff       (20)        1 2023-06-21 14:18:42.000000 edc-0.4.99/edc.egg-info/dependency_links.txt
+-rw-r--r--   0 jw         (502) staff       (20)        1 2021-09-27 09:58:54.000000 edc-0.4.99/edc.egg-info/not-zip-safe
+-rw-r--r--   0 jw         (502) staff       (20)     1923 2023-06-21 14:18:42.000000 edc-0.4.99/edc.egg-info/requires.txt
+-rw-r--r--   0 jw         (502) staff       (20)        6 2023-06-21 14:18:42.000000 edc-0.4.99/edc.egg-info/top_level.txt
+drwxr-xr-x   0 jw         (502) staff       (20)        0 2023-06-21 14:18:42.170056 edc-0.4.99/image/
+-rw-r--r--   0 jw         (502) staff       (20)   160721 2021-08-24 11:21:23.000000 edc-0.4.99/image/icon-pycharm.png
+-rw-r--r--   0 jw         (502) staff       (20)      162 2023-04-18 18:48:47.000000 edc-0.4.99/pyproject.toml
+drwxr-xr-x   0 jw         (502) staff       (20)        0 2023-06-21 14:18:42.176102 edc-0.4.99/requirements.tests/
+-rw-r--r--   0 jw         (502) staff       (20)       21 2023-04-18 18:48:47.000000 edc-0.4.99/requirements.tests/coverage.txt
+-rw-r--r--   0 jw         (502) staff       (20)       14 2023-04-18 18:48:47.000000 edc-0.4.99/requirements.tests/docs.txt
+-rw-r--r--   0 jw         (502) staff       (20)     1053 2023-05-07 19:16:29.000000 edc-0.4.99/requirements.tests/edc.txt
+-rw-r--r--   0 jw         (502) staff       (20)     4100 2023-04-18 18:48:47.000000 edc-0.4.99/requirements.tests/edc_dev.txt
+-rw-r--r--   0 jw         (502) staff       (20)       68 2021-07-06 12:52:00.000000 edc-0.4.99/requirements.tests/edc_offline.txt
+-rw-r--r--   0 jw         (502) staff       (20)       54 2023-04-18 18:48:47.000000 edc-0.4.99/requirements.tests/lint.txt
+-rw-r--r--   0 jw         (502) staff       (20)       11 2023-04-18 18:48:47.000000 edc-0.4.99/requirements.tests/mysql.txt
+-rw-r--r--   0 jw         (502) staff       (20)       22 2021-07-06 12:52:00.000000 edc-0.4.99/requirements.tests/postgres.txt
+-rw-r--r--   0 jw         (502) staff       (20)       86 2023-04-18 18:48:47.000000 edc-0.4.99/requirements.tests/test_utils.txt
+-rw-r--r--   0 jw         (502) staff       (20)      238 2023-04-18 18:48:47.000000 edc-0.4.99/requirements.tests/third_party_dev.txt
+-rw-r--r--   0 jw         (502) staff       (20)       50 2023-04-18 18:48:47.000000 edc-0.4.99/requirements.tests/tox.txt
+-rw-r--r--   0 jw         (502) staff       (20)     2995 2023-06-21 14:18:42.178653 edc-0.4.99/setup.cfg
+drwxr-xr-x   0 jw         (502) staff       (20)        0 2023-06-21 14:18:42.176897 edc-0.4.99/utils/
+-rw-r--r--   0 jw         (502) staff       (20)        0 2021-07-06 12:52:00.000000 edc-0.4.99/utils/__init__.py
+-rw-r--r--   0 jw         (502) staff       (20)      721 2023-04-18 18:48:47.000000 edc-0.4.99/utils/get_edc_requirements.py
```

### Comparing `edc-0.4.98/.gitignore` & `edc-0.4.99/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-0.4.98/.pre-commit-config.yaml` & `edc-0.4.99/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `edc-0.4.98/CHANGES` & `edc-0.4.99/CHANGES`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changes
 -------
 
+0.4.99
+------
+- fix rounding issue with md section numbers, allow opt out of timestamp on
+  every form rendered (edc-form-describer)
+
 0.4.98
 ------
 - allow fbg date to be 'on or after' report date instead of only after (edc-glucose)
 - minor fix in date_is_after_or_raise validation message when using
   inclusive=True (edc-form-validators)
 
 0.4.97
```

### Comparing `edc-0.4.98/LICENSE` & `edc-0.4.99/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-0.4.98/PKG-INFO` & `edc-0.4.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc
-Version: 0.4.98
+Version: 0.4.99
 Summary: EDC core modules for clinicedc/edc projects.
 Home-page: https://github.com/clinicedc/edc
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc clinical trials research
 Classifier: Environment :: Web Environment
```

### Comparing `edc-0.4.98/README.rst` & `edc-0.4.99/README.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.98/bin/nginx/edc-uat.conf` & `edc-0.4.99/bin/nginx/edc-uat.conf`

 * *Files identical despite different names*

### Comparing `edc-0.4.98/bin/nginx/edc.conf` & `edc-0.4.99/bin/nginx/edc.conf`

 * *Files identical despite different names*

### Comparing `edc-0.4.98/bin/scripts/dev_repos.sh` & `edc-0.4.99/bin/scripts/dev_repos.sh`

 * *Files identical despite different names*

### Comparing `edc-0.4.98/bin/scripts/update_edc.sh` & `edc-0.4.99/bin/scripts/update_edc.sh`

 * *Files identical despite different names*

### Comparing `edc-0.4.98/bin/systemd/celery-uat.service` & `edc-0.4.99/bin/systemd/celery-uat.service`

 * *Files identical despite different names*

### Comparing `edc-0.4.98/bin/systemd/celery.service` & `edc-0.4.99/bin/systemd/celery.service`

 * *Files identical despite different names*

### Comparing `edc-0.4.98/docs/Makefile` & `edc-0.4.99/docs/Makefile`

 * *Files identical despite different names*

### Comparing `edc-0.4.98/docs/README.rst` & `edc-0.4.99/docs/README.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.98/docs/backup.rst` & `edc-0.4.99/docs/backup.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.98/docs/celery.rst` & `edc-0.4.99/docs/celery.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.98/docs/conda.rst` & `edc-0.4.99/docs/conda.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.98/docs/conf.py` & `edc-0.4.99/docs/conf.py`

 * *Files identical despite different names*

### Comparing `edc-0.4.98/docs/configure_web_services.rst` & `edc-0.4.99/docs/configure_web_services.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.98/docs/deploy_new_droplet.rst` & `edc-0.4.99/docs/deploy_new_droplet.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.98/docs/exporting_encrypted_data.rst` & `edc-0.4.99/docs/exporting_encrypted_data.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.98/docs/forms_reference.md` & `edc-0.4.99/docs/forms_reference.md`

 * *Files identical despite different names*

### Comparing `edc-0.4.98/docs/landing_page.rst` & `edc-0.4.99/docs/landing_page.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.98/docs/make.bat` & `edc-0.4.99/docs/make.bat`

 * *Files identical despite different names*

### Comparing `edc-0.4.98/docs/prepare_database.rst` & `edc-0.4.99/docs/prepare_database.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.98/docs/printing.rst` & `edc-0.4.99/docs/printing.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.98/docs/update_deployment.rst` & `edc-0.4.99/docs/update_deployment.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.98/edc.egg-info/PKG-INFO` & `edc-0.4.99/edc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc
-Version: 0.4.98
+Version: 0.4.99
 Summary: EDC core modules for clinicedc/edc projects.
 Home-page: https://github.com/clinicedc/edc
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc clinical trials research
 Classifier: Environment :: Web Environment
```

### Comparing `edc-0.4.98/edc.egg-info/SOURCES.txt` & `edc-0.4.99/edc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edc-0.4.98/edc.egg-info/requires.txt` & `edc-0.4.99/edc.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 edc-document-status==0.1.4
 edc-dx==0.1.19
 edc-dx-review==0.1.39
 edc-egfr==0.1.11
 edc-export==0.3.26
 edc-facility==0.3.15
 edc-fieldsets==0.3.13
-edc-form-describer==0.3.13
+edc-form-describer==0.3.14
 edc-form-label==0.3.9
 edc-form-validators==0.3.34
 edc-glucose==0.1.29
 edc-he==0.1.7
 edc-identifier==0.3.23
 edc-lab==0.3.43
 edc-lab-dashboard==0.3.11
```

### Comparing `edc-0.4.98/image/icon-pycharm.png` & `edc-0.4.99/image/icon-pycharm.png`

 * *Files identical despite different names*

### Comparing `edc-0.4.98/requirements.tests/edc.txt` & `edc-0.4.99/requirements.tests/edc.txt`

 * *Files identical despite different names*

### Comparing `edc-0.4.98/requirements.tests/edc_dev.txt` & `edc-0.4.99/requirements.tests/edc_dev.txt`

 * *Files identical despite different names*

### Comparing `edc-0.4.98/setup.cfg` & `edc-0.4.99/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 	edc-document-status==0.1.4
 	edc-dx==0.1.19
 	edc-dx-review==0.1.39
 	edc-egfr==0.1.11
 	edc-export==0.3.26
 	edc-facility==0.3.15
 	edc-fieldsets==0.3.13
-	edc-form-describer==0.3.13
+	edc-form-describer==0.3.14
 	edc-form-label==0.3.9
 	edc-form-validators==0.3.34
 	edc-glucose==0.1.29
 	edc-he==0.1.7
 	edc-identifier==0.3.23
 	edc-lab==0.3.43
 	edc-lab-dashboard==0.3.11
```

### Comparing `edc-0.4.98/utils/get_edc_requirements.py` & `edc-0.4.99/utils/get_edc_requirements.py`

 * *Files identical despite different names*

