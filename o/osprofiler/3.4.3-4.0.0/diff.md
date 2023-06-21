# Comparing `tmp/osprofiler-3.4.3.tar.gz` & `tmp/osprofiler-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osprofiler-3.4.3.tar", last modified: Thu May  5 09:53:51 2022, max compression
+gzip compressed data, was "osprofiler-4.0.0.tar", last modified: Wed Jun 21 11:15:26 2023, max compression
```

## Comparing `osprofiler-3.4.3.tar` & `osprofiler-4.0.0.tar`

### file list

```diff
@@ -1,143 +1,150 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-05 09:53:51.021370 osprofiler-3.4.3/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1363 2022-05-05 09:53:10.000000 osprofiler-3.4.3/.pre-commit-config.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2022-05-05 09:53:10.000000 osprofiler-3.4.3/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1493 2022-05-05 09:53:10.000000 osprofiler-3.4.3/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3295 2022-05-05 09:53:50.000000 osprofiler-3.4.3/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      543 2022-05-05 09:53:10.000000 osprofiler-3.4.3/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13957 2022-05-05 09:53:50.000000 osprofiler-3.4.3/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10273 2022-05-05 09:53:10.000000 osprofiler-3.4.3/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2474 2022-05-05 09:53:51.021370 osprofiler-3.4.3/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1279 2022-05-05 09:53:10.000000 osprofiler-3.4.3/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2022-05-05 09:53:10.000000 osprofiler-3.4.3/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-05 09:53:51.001368 osprofiler-3.4.3/devstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3499 2022-05-05 09:53:10.000000 osprofiler-3.4.3/devstack/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-05 09:53:51.001368 osprofiler-3.4.3/devstack/lib/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4369 2022-05-05 09:53:10.000000 osprofiler-3.4.3/devstack/lib/osprofiler
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      613 2022-05-05 09:53:10.000000 osprofiler-3.4.3/devstack/plugin.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      430 2022-05-05 09:53:10.000000 osprofiler-3.4.3/devstack/settings
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-05 09:53:51.001368 osprofiler-3.4.3/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2022-05-05 09:53:10.000000 osprofiler-3.4.3/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-05 09:53:51.001368 osprofiler-3.4.3/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6778 2022-05-05 09:53:10.000000 osprofiler-3.4.3/doc/source/Makefile
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4186 2022-05-05 09:53:10.000000 osprofiler-3.4.3/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      738 2022-05-05 09:53:10.000000 osprofiler-3.4.3/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-05 09:53:51.001368 osprofiler-3.4.3/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7211 2022-05-05 09:53:10.000000 osprofiler-3.4.3/doc/source/user/api.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1215 2022-05-05 09:53:10.000000 osprofiler-3.4.3/doc/source/user/background.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2455 2022-05-05 09:53:10.000000 osprofiler-3.4.3/doc/source/user/collectors.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       32 2022-05-05 09:53:10.000000 osprofiler-3.4.3/doc/source/user/history.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      633 2022-05-05 09:53:10.000000 osprofiler-3.4.3/doc/source/user/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5293 2022-05-05 09:53:10.000000 osprofiler-3.4.3/doc/source/user/integration.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      533 2022-05-05 09:53:10.000000 osprofiler-3.4.3/doc/source/user/similar_projects.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-05 09:53:51.001368 osprofiler-3.4.3/doc/specs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      354 2022-05-05 09:53:10.000000 osprofiler-3.4.3/doc/specs/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-05 09:53:51.005369 osprofiler-3.4.3/doc/specs/implemented/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      290 2022-05-05 09:53:10.000000 osprofiler-3.4.3/doc/specs/implemented/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2403 2022-05-05 09:53:10.000000 osprofiler-3.4.3/doc/specs/implemented/make_paste_ini_config_optional.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2656 2022-05-05 09:53:10.000000 osprofiler-3.4.3/doc/specs/implemented/multi_backend_support.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-05 09:53:51.005369 osprofiler-3.4.3/doc/specs/in-progress/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      306 2022-05-05 09:53:10.000000 osprofiler-3.4.3/doc/specs/in-progress/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1451 2022-05-05 09:53:10.000000 osprofiler-3.4.3/doc/specs/in-progress/better_devstack_integration.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1601 2022-05-05 09:53:10.000000 osprofiler-3.4.3/doc/specs/in-progress/integration_testing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2397 2022-05-05 09:53:10.000000 osprofiler-3.4.3/doc/specs/template.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      407 2022-05-05 09:53:10.000000 osprofiler-3.4.3/lower-constraints.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-05 09:53:51.005369 osprofiler-3.4.3/osprofiler/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      855 2022-05-05 09:53:10.000000 osprofiler-3.4.3/osprofiler/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5476 2022-05-05 09:53:10.000000 osprofiler-3.4.3/osprofiler/_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-05 09:53:51.009369 osprofiler-3.4.3/osprofiler/cmd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-05-05 09:53:10.000000 osprofiler-3.4.3/osprofiler/cmd/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1731 2022-05-05 09:53:10.000000 osprofiler-3.4.3/osprofiler/cmd/cliutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7734 2022-05-05 09:53:10.000000 osprofiler-3.4.3/osprofiler/cmd/commands.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2950 2022-05-05 09:53:10.000000 osprofiler-3.4.3/osprofiler/cmd/shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13940 2022-05-05 09:53:10.000000 osprofiler-3.4.3/osprofiler/cmd/template.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-05 09:53:51.013369 osprofiler-3.4.3/osprofiler/drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      405 2022-05-05 09:53:10.000000 osprofiler-3.4.3/osprofiler/drivers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10891 2022-05-05 09:53:10.000000 osprofiler-3.4.3/osprofiler/drivers/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6810 2022-05-05 09:53:10.000000 osprofiler-3.4.3/osprofiler/drivers/elasticsearch_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5535 2022-05-05 09:53:10.000000 osprofiler-3.4.3/osprofiler/drivers/jaeger.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9699 2022-05-05 09:53:10.000000 osprofiler-3.4.3/osprofiler/drivers/loginsight.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7412 2022-05-05 09:53:10.000000 osprofiler-3.4.3/osprofiler/drivers/messaging.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4377 2022-05-05 09:53:10.000000 osprofiler-3.4.3/osprofiler/drivers/mongodb.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8271 2022-05-05 09:53:10.000000 osprofiler-3.4.3/osprofiler/drivers/redis_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5617 2022-05-05 09:53:10.000000 osprofiler-3.4.3/osprofiler/drivers/sqlalchemy_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      941 2022-05-05 09:53:10.000000 osprofiler-3.4.3/osprofiler/exc.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-05 09:53:51.013369 osprofiler-3.4.3/osprofiler/hacking/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-05-05 09:53:10.000000 osprofiler-3.4.3/osprofiler/hacking/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13136 2022-05-05 09:53:10.000000 osprofiler-3.4.3/osprofiler/hacking/checks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1474 2022-05-05 09:53:10.000000 osprofiler-3.4.3/osprofiler/initializer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2635 2022-05-05 09:53:10.000000 osprofiler-3.4.3/osprofiler/notifier.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7594 2022-05-05 09:53:10.000000 osprofiler-3.4.3/osprofiler/opts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16071 2022-05-05 09:53:10.000000 osprofiler-3.4.3/osprofiler/profiler.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3455 2022-05-05 09:53:10.000000 osprofiler-3.4.3/osprofiler/sqlalchemy.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-05 09:53:51.013369 osprofiler-3.4.3/osprofiler/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-05-05 09:53:10.000000 osprofiler-3.4.3/osprofiler/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-05 09:53:51.013369 osprofiler-3.4.3/osprofiler/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-05-05 09:53:10.000000 osprofiler-3.4.3/osprofiler/tests/functional/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2022-05-05 09:53:10.000000 osprofiler-3.4.3/osprofiler/tests/functional/config.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5268 2022-05-05 09:53:10.000000 osprofiler-3.4.3/osprofiler/tests/functional/test_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1008 2022-05-05 09:53:10.000000 osprofiler-3.4.3/osprofiler/tests/test.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-05 09:53:51.013369 osprofiler-3.4.3/osprofiler/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-05-05 09:53:10.000000 osprofiler-3.4.3/osprofiler/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-05 09:53:51.017370 osprofiler-3.4.3/osprofiler/tests/unit/cmd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-05-05 09:53:10.000000 osprofiler-3.4.3/osprofiler/tests/unit/cmd/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6136 2022-05-05 09:53:10.000000 osprofiler-3.4.3/osprofiler/tests/unit/cmd/test_shell.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-05 09:53:51.017370 osprofiler-3.4.3/osprofiler/tests/unit/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-05-05 09:53:10.000000 osprofiler-3.4.3/osprofiler/tests/unit/doc/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4501 2022-05-05 09:53:10.000000 osprofiler-3.4.3/osprofiler/tests/unit/doc/test_specs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-05 09:53:51.017370 osprofiler-3.4.3/osprofiler/tests/unit/drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-05-05 09:53:10.000000 osprofiler-3.4.3/osprofiler/tests/unit/drivers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4137 2022-05-05 09:53:10.000000 osprofiler-3.4.3/osprofiler/tests/unit/drivers/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4405 2022-05-05 09:53:10.000000 osprofiler-3.4.3/osprofiler/tests/unit/drivers/test_elasticsearch.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2690 2022-05-05 09:53:10.000000 osprofiler-3.4.3/osprofiler/tests/unit/drivers/test_jaeger.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12953 2022-05-05 09:53:10.000000 osprofiler-3.4.3/osprofiler/tests/unit/drivers/test_loginsight.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2488 2022-05-05 09:53:10.000000 osprofiler-3.4.3/osprofiler/tests/unit/drivers/test_messaging.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13596 2022-05-05 09:53:10.000000 osprofiler-3.4.3/osprofiler/tests/unit/drivers/test_mongodb.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14002 2022-05-05 09:53:10.000000 osprofiler-3.4.3/osprofiler/tests/unit/drivers/test_redis_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1644 2022-05-05 09:53:10.000000 osprofiler-3.4.3/osprofiler/tests/unit/test_initializer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1966 2022-05-05 09:53:10.000000 osprofiler-3.4.3/osprofiler/tests/unit/test_notifier.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2896 2022-05-05 09:53:10.000000 osprofiler-3.4.3/osprofiler/tests/unit/test_opts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21169 2022-05-05 09:53:10.000000 osprofiler-3.4.3/osprofiler/tests/unit/test_profiler.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6550 2022-05-05 09:53:10.000000 osprofiler-3.4.3/osprofiler/tests/unit/test_sqlalchemy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5306 2022-05-05 09:53:10.000000 osprofiler-3.4.3/osprofiler/tests/unit/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11622 2022-05-05 09:53:10.000000 osprofiler-3.4.3/osprofiler/tests/unit/test_web.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4519 2022-05-05 09:53:10.000000 osprofiler-3.4.3/osprofiler/web.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-05 09:53:51.009369 osprofiler-3.4.3/osprofiler.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2474 2022-05-05 09:53:50.000000 osprofiler-3.4.3/osprofiler.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3509 2022-05-05 09:53:50.000000 osprofiler-3.4.3/osprofiler.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-05-05 09:53:50.000000 osprofiler-3.4.3/osprofiler.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      192 2022-05-05 09:53:50.000000 osprofiler-3.4.3/osprofiler.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-05-05 09:53:50.000000 osprofiler-3.4.3/osprofiler.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2022-05-05 09:53:50.000000 osprofiler-3.4.3/osprofiler.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      475 2022-05-05 09:53:50.000000 osprofiler-3.4.3/osprofiler.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       11 2022-05-05 09:53:50.000000 osprofiler-3.4.3/osprofiler.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-05 09:53:51.017370 osprofiler-3.4.3/playbooks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1911 2022-05-05 09:53:10.000000 osprofiler-3.4.3/playbooks/osprofiler-post.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-05 09:53:50.997368 osprofiler-3.4.3/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-05 09:53:51.017370 osprofiler-3.4.3/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2022-05-05 09:53:10.000000 osprofiler-3.4.3/releasenotes/notes/add-reno-996dd44974d53238.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2022-05-05 09:53:10.000000 osprofiler-3.4.3/releasenotes/notes/drop-python-2-7-73d3113c69d724d6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      751 2022-05-05 09:53:10.000000 osprofiler-3.4.3/releasenotes/notes/redis-improvement-d4c91683fc89f570.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-05 09:53:51.021370 osprofiler-3.4.3/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-05 09:53:51.021370 osprofiler-3.4.3/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-05-05 09:53:10.000000 osprofiler-3.4.3/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-05 09:53:51.021370 osprofiler-3.4.3/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-05-05 09:53:10.000000 osprofiler-3.4.3/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9019 2022-05-05 09:53:10.000000 osprofiler-3.4.3/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2022-05-05 09:53:10.000000 osprofiler-3.4.3/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2022-05-05 09:53:10.000000 osprofiler-3.4.3/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2022-05-05 09:53:10.000000 osprofiler-3.4.3/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2022-05-05 09:53:10.000000 osprofiler-3.4.3/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-05-05 09:53:10.000000 osprofiler-3.4.3/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-05-05 09:53:10.000000 osprofiler-3.4.3/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2022-05-05 09:53:10.000000 osprofiler-3.4.3/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2022-05-05 09:53:10.000000 osprofiler-3.4.3/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2022-05-05 09:53:10.000000 osprofiler-3.4.3/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2022-05-05 09:53:10.000000 osprofiler-3.4.3/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2022-05-05 09:53:10.000000 osprofiler-3.4.3/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1091 2022-05-05 09:53:51.025370 osprofiler-3.4.3/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      699 2022-05-05 09:53:10.000000 osprofiler-3.4.3/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      522 2022-05-05 09:53:10.000000 osprofiler-3.4.3/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-05-05 09:53:51.021370 osprofiler-3.4.3/tools/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      911 2022-05-05 09:53:10.000000 osprofiler-3.4.3/tools/lint.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1615 2022-05-05 09:53:10.000000 osprofiler-3.4.3/tools/patch_tox_venv.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2831 2022-05-05 09:53:10.000000 osprofiler-3.4.3/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.224339 osprofiler-4.0.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1363 2023-06-21 11:14:46.000000 osprofiler-4.0.0/.pre-commit-config.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2023-06-21 11:14:46.000000 osprofiler-4.0.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1493 2023-06-21 11:14:46.000000 osprofiler-4.0.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3504 2023-06-21 11:15:26.000000 osprofiler-4.0.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      543 2023-06-21 11:14:46.000000 osprofiler-4.0.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14425 2023-06-21 11:15:26.000000 osprofiler-4.0.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10273 2023-06-21 11:14:46.000000 osprofiler-4.0.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2424 2023-06-21 11:15:26.224339 osprofiler-4.0.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1279 2023-06-21 11:14:46.000000 osprofiler-4.0.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2023-06-21 11:14:46.000000 osprofiler-4.0.0/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.204339 osprofiler-4.0.0/devstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3499 2023-06-21 11:14:46.000000 osprofiler-4.0.0/devstack/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.204339 osprofiler-4.0.0/devstack/lib/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4925 2023-06-21 11:14:46.000000 osprofiler-4.0.0/devstack/lib/osprofiler
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      837 2023-06-21 11:14:46.000000 osprofiler-4.0.0/devstack/plugin.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      430 2023-06-21 11:14:46.000000 osprofiler-4.0.0/devstack/settings
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.204339 osprofiler-4.0.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2023-06-21 11:14:46.000000 osprofiler-4.0.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.204339 osprofiler-4.0.0/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6778 2023-06-21 11:14:46.000000 osprofiler-4.0.0/doc/source/Makefile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4180 2023-06-21 11:14:46.000000 osprofiler-4.0.0/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      738 2023-06-21 11:14:46.000000 osprofiler-4.0.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.208339 osprofiler-4.0.0/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7211 2023-06-21 11:14:46.000000 osprofiler-4.0.0/doc/source/user/api.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1215 2023-06-21 11:14:46.000000 osprofiler-4.0.0/doc/source/user/background.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2890 2023-06-21 11:14:46.000000 osprofiler-4.0.0/doc/source/user/collectors.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2023-06-21 11:14:46.000000 osprofiler-4.0.0/doc/source/user/history.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      633 2023-06-21 11:14:46.000000 osprofiler-4.0.0/doc/source/user/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5293 2023-06-21 11:14:46.000000 osprofiler-4.0.0/doc/source/user/integration.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      533 2023-06-21 11:14:46.000000 osprofiler-4.0.0/doc/source/user/similar_projects.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.208339 osprofiler-4.0.0/doc/specs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      354 2023-06-21 11:14:46.000000 osprofiler-4.0.0/doc/specs/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.208339 osprofiler-4.0.0/doc/specs/implemented/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      290 2023-06-21 11:14:46.000000 osprofiler-4.0.0/doc/specs/implemented/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2403 2023-06-21 11:14:46.000000 osprofiler-4.0.0/doc/specs/implemented/make_paste_ini_config_optional.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2656 2023-06-21 11:14:46.000000 osprofiler-4.0.0/doc/specs/implemented/multi_backend_support.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.208339 osprofiler-4.0.0/doc/specs/in-progress/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      306 2023-06-21 11:14:46.000000 osprofiler-4.0.0/doc/specs/in-progress/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1451 2023-06-21 11:14:46.000000 osprofiler-4.0.0/doc/specs/in-progress/better_devstack_integration.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1601 2023-06-21 11:14:46.000000 osprofiler-4.0.0/doc/specs/in-progress/integration_testing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2397 2023-06-21 11:14:46.000000 osprofiler-4.0.0/doc/specs/template.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      469 2023-06-21 11:14:46.000000 osprofiler-4.0.0/lower-constraints.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.212339 osprofiler-4.0.0/osprofiler/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      855 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5826 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.212339 osprofiler-4.0.0/osprofiler/cmd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/cmd/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1731 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/cmd/cliutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7734 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/cmd/commands.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2950 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/cmd/shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13940 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/cmd/template.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.216339 osprofiler-4.0.0/osprofiler/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      448 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/drivers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10891 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/drivers/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6810 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/drivers/elasticsearch_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5850 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/drivers/jaeger.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9699 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/drivers/loginsight.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7412 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/drivers/messaging.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4377 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/drivers/mongodb.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6841 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/drivers/otlp.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8270 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/drivers/redis_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5617 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/drivers/sqlalchemy_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      941 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/exc.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.216339 osprofiler-4.0.0/osprofiler/hacking/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/hacking/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13136 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/hacking/checks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1474 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/initializer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2635 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/notifier.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8572 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/opts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16071 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/profiler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3455 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/sqlalchemy.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.216339 osprofiler-4.0.0/osprofiler/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.216339 osprofiler-4.0.0/osprofiler/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/functional/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/functional/config.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5268 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/functional/test_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1008 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/test.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.216339 osprofiler-4.0.0/osprofiler/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.216339 osprofiler-4.0.0/osprofiler/tests/unit/cmd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/unit/cmd/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6136 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/unit/cmd/test_shell.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.216339 osprofiler-4.0.0/osprofiler/tests/unit/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/unit/doc/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4501 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/unit/doc/test_specs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.220339 osprofiler-4.0.0/osprofiler/tests/unit/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/unit/drivers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4137 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/unit/drivers/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4405 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/unit/drivers/test_elasticsearch.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3788 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/unit/drivers/test_jaeger.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12953 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/unit/drivers/test_loginsight.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2488 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/unit/drivers/test_messaging.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13596 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/unit/drivers/test_mongodb.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2736 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/unit/drivers/test_otlp.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14002 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/unit/drivers/test_redis_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1644 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/unit/test_initializer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1966 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/unit/test_notifier.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2896 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/unit/test_opts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21169 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/unit/test_profiler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6550 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/unit/test_sqlalchemy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5306 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/unit/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11622 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/unit/test_web.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4519 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/web.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.212339 osprofiler-4.0.0/osprofiler.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2424 2023-06-21 11:15:26.000000 osprofiler-4.0.0/osprofiler.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3905 2023-06-21 11:15:26.000000 osprofiler-4.0.0/osprofiler.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-06-21 11:15:26.000000 osprofiler-4.0.0/osprofiler.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      192 2023-06-21 11:15:26.000000 osprofiler-4.0.0/osprofiler.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-06-21 11:15:26.000000 osprofiler-4.0.0/osprofiler.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-06-21 11:15:26.000000 osprofiler-4.0.0/osprofiler.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      537 2023-06-21 11:15:26.000000 osprofiler-4.0.0/osprofiler.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       11 2023-06-21 11:15:26.000000 osprofiler-4.0.0/osprofiler.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.220339 osprofiler-4.0.0/playbooks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1911 2023-06-21 11:14:46.000000 osprofiler-4.0.0/playbooks/osprofiler-post.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.200339 osprofiler-4.0.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.220339 osprofiler-4.0.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2023-06-21 11:14:46.000000 osprofiler-4.0.0/releasenotes/notes/add-reno-996dd44974d53238.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2023-06-21 11:14:46.000000 osprofiler-4.0.0/releasenotes/notes/drop-jaeger-container-when-unstacking-e8fcdc036f80158a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2023-06-21 11:14:46.000000 osprofiler-4.0.0/releasenotes/notes/drop-python-2-7-73d3113c69d724d6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2023-06-21 11:14:46.000000 osprofiler-4.0.0/releasenotes/notes/jaeger-add-process-tags-79d5f5d7a0b049ef.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2023-06-21 11:14:46.000000 osprofiler-4.0.0/releasenotes/notes/jaeger-service-name-prefix-72878a930f700878.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2023-06-21 11:14:46.000000 osprofiler-4.0.0/releasenotes/notes/otlp-driver-cb932038ad580ac2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      751 2023-06-21 11:14:46.000000 osprofiler-4.0.0/releasenotes/notes/redis-improvement-d4c91683fc89f570.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2023-06-21 11:14:46.000000 osprofiler-4.0.0/releasenotes/notes/remove-strict-redis-9eb43d30c9c1fc43.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.220339 osprofiler-4.0.0/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.220339 osprofiler-4.0.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:14:46.000000 osprofiler-4.0.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.224339 osprofiler-4.0.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:14:46.000000 osprofiler-4.0.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9011 2023-06-21 11:14:46.000000 osprofiler-4.0.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-06-21 11:14:46.000000 osprofiler-4.0.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-06-21 11:14:46.000000 osprofiler-4.0.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-06-21 11:14:46.000000 osprofiler-4.0.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-06-21 11:14:46.000000 osprofiler-4.0.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-06-21 11:14:46.000000 osprofiler-4.0.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-06-21 11:14:46.000000 osprofiler-4.0.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-06-21 11:14:46.000000 osprofiler-4.0.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-06-21 11:14:46.000000 osprofiler-4.0.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-06-21 11:14:46.000000 osprofiler-4.0.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-06-21 11:14:46.000000 osprofiler-4.0.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2023-06-21 11:14:46.000000 osprofiler-4.0.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1052 2023-06-21 11:15:26.224339 osprofiler-4.0.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      699 2023-06-21 11:14:46.000000 osprofiler-4.0.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      584 2023-06-21 11:14:46.000000 osprofiler-4.0.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.224339 osprofiler-4.0.0/tools/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      911 2023-06-21 11:14:46.000000 osprofiler-4.0.0/tools/lint.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1615 2023-06-21 11:14:46.000000 osprofiler-4.0.0/tools/patch_tox_venv.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2588 2023-06-21 11:14:46.000000 osprofiler-4.0.0/tox.ini
```

### Comparing `osprofiler-3.4.3/.pre-commit-config.yaml` & `osprofiler-4.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/.zuul.yaml` & `osprofiler-4.0.0/.zuul.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -5,20 +5,20 @@
       - openstack-cover-jobs
       - openstack-python3-jobs
       - periodic-stable-jobs
       - publish-openstack-docs-pti
       - release-notes-jobs-python3
     check:
       jobs:
-        - openstack-tox-functional-py36
+        - openstack-tox-functional-py38
         - tempest-smoke-py3-osprofiler-redis
         - tempest-smoke-py3-osprofiler-sqlalchemy
     gate:
       jobs:
-        - openstack-tox-functional-py36
+        - openstack-tox-functional-py38
 
 - job:
     name: tempest-smoke-py3-osprofiler-redis
     parent: tempest-full-py3
     voting: false
     post-run: playbooks/osprofiler-post.yaml
     description: |
```

### Comparing `osprofiler-3.4.3/AUTHORS` & `osprofiler-4.0.0/AUTHORS`

 * *Files 10% similar despite different names*

```diff
@@ -43,40 +43,45 @@
 Nguyen Van Trung <trungnv@vn.fujitsu.com>
 Oleksii Chuprykov <ochuprykov@mirantis.com>
 Omer Anson <omer.anson@toganetworks.com>
 Ondřej Nový <ondrej.novy@firma.seznam.cz>
 OpenStack Release Bot <infra-root@openstack.org>
 Radoslaw Smigielski <radoslaw.smigielski@nokia.com>
 Roman Podoliaka <rpodolyaka@mirantis.com>
+Sahid Orentino Ferdjaoui <sahid.ferdjaoui@industrialdiscipline.com>
 Sean McGinnis <sean.mcginnis@gmail.com>
 Shoham Peller <shohamp@gmail.com>
 Simon Pasquier <spasquier@mirantis.com>
 Slawek Kaplonski <skaplons@redhat.com>
 Stephen Finucane <stephenfin@redhat.com>
 Stuart Grace <stuart.grace@bbc.co.uk>
+Takashi Kajinami <tkajinam@redhat.com>
 Thomas Bechtold <tbechtold@suse.com>
 Timur Sufiev <tsufiev@mirantis.com>
+Tobias Urdin <tobias.urdin@binero.com>
 Tony Xu <hhktony@gmail.com>
 Tovin Seven <vinhnt@vn.fujitsu.com>
 Victor Morales <victor.morales@intel.com>
 Vieri <15050873171@163.com>
 Vipin Balachandran <vbala@vmware.com>
 Vu Cong Tuan <tuanvc@vn.fujitsu.com>
 Wander Way <wanderwayout@gmail.com>
 XiaojueGuan <guanalbertjone@gmail.com>
+YuehuiLei <leiyuehui@inspur.com>
 Zhi Yan Liu <zhiyanl@cn.ibm.com>
 caoyuan <cao.yuan@99cloud.net>
 chenxu <424024687@qq.com>
 francotseng <francotseng18@gmail.com>
 gecong1973 <ge.cong@zte.com.cn>
 howardlee <lihongweibj@inspur.com>
 kavithahr <kavitha.r@nectechnologies.in>
 lipan <lipan7195@fiberhome.com>
 lvdongbing <dongbing.lv@kylin-cloud.com>
 melissaml <ma.lei@99cloud.net>
+niuke <niuke19970315@163.com>
 qingszhao <zhao.daqing@99cloud.net>
 reedip <reedip.banerjee@nectechnologies.in>
 ricolin <rico.lin@easystack.cn>
 ritesh.arya <ritesh.arya@nectechnologies.in>
 shangxiaobj <shangxiaobj@inspur.com>
 sunyandi <sunyd@inspur.com>
 uppi <helendile@gmail.com>
```

### Comparing `osprofiler-3.4.3/CONTRIBUTING.rst` & `osprofiler-4.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/ChangeLog` & `osprofiler-4.0.0/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,25 @@
 CHANGES
 =======
 
+4.0.0
+-----
+
+* add support of otlp exporter
+* devstack: remove jaeger container on unstack
+* [profiler] hmac\_key should be secret
+* jaeger: introduce process tags' option for tracer
+* jaeger: introduce service name prefix
+* jaeger: fix driver initialization for tests
+* setup.cfg: Replace dashes with underscores
+* Change StrictRedis usage to Redis
+* tox: Add functional-py38, functional-py39 envs
+* remove unicode prefix from code
+* Fix formattiing of release list
+
 3.4.3
 -----
 
 * Make some revisions in the document
 * Update CI to use unversioned jobs template
 * Fix api index and module index
```

### Comparing `osprofiler-3.4.3/LICENSE` & `osprofiler-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/PKG-INFO` & `osprofiler-4.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osprofiler
-Version: 3.4.3
+Version: 4.0.0
 Summary: OpenStack Profiler Library
 Home-page: https://docs.openstack.org/osprofiler/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ===================================================
          OSProfiler -- Library for cross-project profiling
@@ -41,15 +41,14 @@
 Classifier: Environment :: OpenStack
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Provides-Extra: oslo_config
 Provides-Extra: test
```

### Comparing `osprofiler-3.4.3/README.rst` & `osprofiler-4.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/devstack/README.rst` & `osprofiler-4.0.0/devstack/README.rst`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/devstack/lib/osprofiler` & `osprofiler-4.0.0/devstack/lib/osprofiler`

 * *Files 10% similar despite different names*

```diff
@@ -54,27 +54,41 @@
     fi
 
     start_service redis
 
     pip_install_gr redis
 }
 
-function install_jaeger() {
+function install_jaeger_backend() {
     if is_ubuntu; then
         install_package docker.io
         start_service docker
         add_user_to_group $STACK_USER docker
-        sg docker -c "docker run -d --name jaeger -p 6831:6831/udp -p 16686:16686 jaegertracing/all-in-one:1.7"
+        sg docker -c "docker run -d --name jaeger -e COLLECTOR_OTLP_ENABLED=true -p 6831:6831/udp -p 16686:16686 -p 4318:4318 jaegertracing/all-in-one:1.42"
     else
         exit_distro_not_supported "docker.io installation"
     fi
+}
 
+function install_jaeger() {
+    install_jaeger_backend
     pip_install jaeger-client
 }
 
+function install_otlp() {
+    # For OTLP we use Jaeger backend but any OTLP compatible backend
+    # can be used.
+    install_jaeger_backend
+    pip_install opentelemetry-sdk opentelemetry-exporter-otlp
+}
+
+function drop_jaeger() {
+    sg docker -c 'docker rm jaeger --force'
+}
+
 function install_elasticsearch() {
     if is_ubuntu; then
         install_package docker.io
         start_service docker
         add_user_to_group $STACK_USER docker
         # https://www.elastic.co/guide/en/elasticsearch/reference/5.6/docker.html#docker-cli-run-dev-mode
         sg docker -c 'docker run -d --name elasticsearch -p 9200:9200 -p 9300:9300 -e "discovery.type=single-node" docker.elastic.co/elasticsearch/elasticsearch:5.6.14'
@@ -104,14 +118,17 @@
         OSPROFILER_CONNECTION_STRING=${OSPROFILER_CONNECTION_STRING:-"messaging://"}
     elif [ "$OSPROFILER_COLLECTOR" == "redis" ]; then
         install_redis
         OSPROFILER_CONNECTION_STRING=${OSPROFILER_CONNECTION_STRING:-"redis://localhost:6379"}
     elif [ "$OSPROFILER_COLLECTOR" == "jaeger" ]; then
         install_jaeger
         OSPROFILER_CONNECTION_STRING=${OSPROFILER_CONNECTION_STRING:-"jaeger://localhost:6831"}
+    elif [ "$OSPROFILER_COLLECTOR" == "otlp" ]; then
+        install_otlp
+        OSPROFILER_CONNECTION_STRING=${OSPROFILER_CONNECTION_STRING:-"otlp://localhost:4318"}
     elif [ "$OSPROFILER_COLLECTOR" == "elasticsearch" ]; then
         install_elasticsearch
         OSPROFILER_CONNECTION_STRING=${OSPROFILER_CONNECTION_STRING:-"elasticsearch://elastic:changeme@localhost:9200"}
     elif [ "$OSPROFILER_COLLECTOR" == "mongodb" ]; then
         install_mongodb
         OSPROFILER_CONNECTION_STRING=${OSPROFILER_CONNECTION_STRING:-"mongodb://localhost:27017"}
     elif [ "$OSPROFILER_COLLECTOR" == "sqlalchemy" ]; then
```

### Comparing `osprofiler-3.4.3/devstack/plugin.sh` & `osprofiler-4.0.0/devstack/plugin.sh`

 * *Files 22% similar despite different names*

```diff
@@ -15,11 +15,17 @@
     echo_summary "Configuring OSProfiler"
     configure_osprofiler
 
 elif [[ "$1" == "stack" && "$2" == "test-config" ]]; then
     echo_summary "Configuring Tempest"
     configure_osprofiler_in_tempest
 
+elif [[ "$1" == "unstack" ]]; then
+    if [[ "$OSPROFILER_COLLECTOR" == "jaeger" || \
+            "$OSPROFILER_COLLECTOR" == "otlp" ]]; then
+        echo_summary "Deleting jaeger docker container"
+        drop_jaeger
+    fi
 fi
 
 # Restore xtrace
 $XTRACE
```

### Comparing `osprofiler-3.4.3/doc/source/Makefile` & `osprofiler-4.0.0/doc/source/Makefile`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/doc/source/conf.py` & `osprofiler-4.0.0/doc/source/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,16 +66,16 @@
 # The suffix of source filenames.
 source_suffix = '.rst'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
-project = u'OSprofiler'
-copyright = u'2016, OpenStack Foundation'
+project = 'OSprofiler'
+copyright = '2016, OpenStack Foundation'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 exclude_patterns = []
 
 # If true, '()' will be appended to :func: etc. cross-reference text.
 add_function_parentheses = True
@@ -107,29 +107,29 @@
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author,
 # documentclass [howto/manual]).
 latex_documents = [
     ('index',
      '%s.tex' % project,
-     u'%s Documentation' % project,
-     u'OpenStack Foundation', 'manual'),
+     '%s Documentation' % project,
+     'OpenStack Foundation', 'manual'),
 ]
 
 # -- Options for Texinfo output -----------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
     (
         'index',
         'OSprofiler',
-        u'OSprofiler Documentation',
-        u'OSprofiler Team',
+        'OSprofiler Documentation',
+        'OSprofiler Team',
         'OSprofiler',
         'One line description of project.',
         'Miscellaneous'
     ),
 ]
 
 apidoc_output_dir = 'contributor/modules'
```

### Comparing `osprofiler-3.4.3/doc/source/index.rst` & `osprofiler-4.0.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/doc/source/user/api.rst` & `osprofiler-4.0.0/doc/source/user/api.rst`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/doc/source/user/background.rst` & `osprofiler-4.0.0/doc/source/user/background.rst`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/doc/source/user/collectors.rst` & `osprofiler-4.0.0/doc/source/user/collectors.rst`

 * *Files 4% similar despite different names*

```diff
@@ -67,7 +67,29 @@
    SQLAlchemy collector requires database JSON data type support.
    This type of data is supported by versions listed below or higher:
 
    - MariaDB 10.2
    - MySQL 5.7.8
 
 .. _SQLAlchemy understands: https://docs.sqlalchemy.org/en/latest/core/engines.html#database-urls
+
+
+OTLP
+----
+
+Use OTLP exporter. Can be used with any comptable backend that support
+OTLP.
+
+Usage
+=====
+To use the driver, the `connection_string` in the `[osprofiler]` config section
+needs to be set::
+
+  [osprofiler]
+  connection_string = otlp://192.168.192.81:4318
+
+Example: By default, jaeger is listening OTLP on 4318.
+
+.. note::
+
+   Curently the exporter is only supporting HTTP. In future some work
+   may happen to support gRPC.
```

### Comparing `osprofiler-3.4.3/doc/source/user/index.rst` & `osprofiler-4.0.0/doc/source/user/index.rst`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/doc/source/user/integration.rst` & `osprofiler-4.0.0/doc/source/user/integration.rst`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/doc/source/user/similar_projects.rst` & `osprofiler-4.0.0/doc/source/user/similar_projects.rst`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/doc/specs/implemented/make_paste_ini_config_optional.rst` & `osprofiler-4.0.0/doc/specs/implemented/make_paste_ini_config_optional.rst`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/doc/specs/implemented/multi_backend_support.rst` & `osprofiler-4.0.0/doc/specs/implemented/multi_backend_support.rst`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/doc/specs/in-progress/better_devstack_integration.rst` & `osprofiler-4.0.0/doc/specs/in-progress/better_devstack_integration.rst`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/doc/specs/in-progress/integration_testing.rst` & `osprofiler-4.0.0/doc/specs/in-progress/integration_testing.rst`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/doc/specs/template.rst` & `osprofiler-4.0.0/doc/specs/template.rst`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/osprofiler/__init__.py` & `osprofiler-4.0.0/osprofiler/__init__.py`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/osprofiler/_utils.py` & `osprofiler-4.0.0/osprofiler/_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -157,7 +157,19 @@
         return span_id & int64_max
     try:
         short_id = uuid.UUID(span_id).int & int64_max
     except ValueError:
         # Return a new short id for this
         short_id = shorten_id(uuidutils.generate_uuid())
     return short_id
+
+
+def uuid_to_int128(span_uuid):
+    """Convert from uuid4 to 128 bit id for OpenTracing"""
+    if isinstance(span_uuid, int):
+        return span_uuid
+    try:
+        span_int = uuid.UUID(span_uuid).int
+    except ValueError:
+        # Return a new short id for this
+        span_int = uuid_to_int128(uuidutils.generate_uuid())
+    return span_int
```

### Comparing `osprofiler-3.4.3/osprofiler/cmd/cliutils.py` & `osprofiler-4.0.0/osprofiler/cmd/cliutils.py`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/osprofiler/cmd/commands.py` & `osprofiler-4.0.0/osprofiler/cmd/commands.py`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/osprofiler/cmd/shell.py` & `osprofiler-4.0.0/osprofiler/cmd/shell.py`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/osprofiler/cmd/template.html` & `osprofiler-4.0.0/osprofiler/cmd/template.html`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/osprofiler/drivers/base.py` & `osprofiler-4.0.0/osprofiler/drivers/base.py`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/osprofiler/drivers/elasticsearch_driver.py` & `osprofiler-4.0.0/osprofiler/drivers/elasticsearch_driver.py`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/osprofiler/drivers/jaeger.py` & `osprofiler-4.0.0/osprofiler/drivers/jaeger.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,24 +45,31 @@
             )
 
         parsed_url = parser.urlparse(connection_str)
         cfg = {
             "local_agent": {
                 "reporting_host": parsed_url.hostname,
                 "reporting_port": parsed_url.port,
-            }
+            },
+            "tags": conf.profiler_jaeger.process_tags
         }
 
         # Initialize tracer for each profiler
-        service_name = "{}-{}".format(project, service)
+        service_name = self._get_service_name(conf, project, service)
         config = jaeger_client.Config(cfg, service_name=service_name)
         self.tracer = config.initialize_tracer()
 
         self.spans = collections.deque()
 
+    def _get_service_name(self, conf, project, service):
+        prefix = conf.profiler_jaeger.service_name_prefix
+        if prefix:
+            return "{}-{}-{}".format(prefix, project, service)
+        return "{}-{}".format(project, service)
+
     @classmethod
     def get_name(cls):
         return "jaeger"
 
     def notify(self, payload):
         if payload["name"].endswith("start"):
             timestamp = datetime.datetime.strptime(payload["timestamp"],
```

### Comparing `osprofiler-3.4.3/osprofiler/drivers/loginsight.py` & `osprofiler-4.0.0/osprofiler/drivers/loginsight.py`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/osprofiler/drivers/messaging.py` & `osprofiler-4.0.0/osprofiler/drivers/messaging.py`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/osprofiler/drivers/mongodb.py` & `osprofiler-4.0.0/osprofiler/drivers/mongodb.py`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/osprofiler/drivers/redis_driver.py` & `osprofiler-4.0.0/osprofiler/drivers/redis_driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,24 +33,24 @@
                  service=None, host=None, conf=cfg.CONF, **kwargs):
         """Redis driver for OSProfiler."""
 
         super(Redis, self).__init__(connection_str, project=project,
                                     service=service, host=host,
                                     conf=conf, **kwargs)
         try:
-            from redis import StrictRedis
+            from redis import Redis as _Redis
         except ImportError:
             raise exc.CommandError(
                 "To use OSProfiler with Redis driver, "
                 "please install `redis` library. "
                 "To install with pip:\n `pip install redis`.")
 
         # only connection over network is supported with schema
         # redis://[:password]@host[:port][/db]
-        self.db = StrictRedis.from_url(self.connection_str)
+        self.db = _Redis.from_url(self.connection_str)
         self.namespace_opt = "osprofiler_opt:"
         self.namespace = "osprofiler:"  # legacy
         self.namespace_error = "osprofiler_error:"
 
     @classmethod
     def get_name(cls):
         return "redis"
```

### Comparing `osprofiler-3.4.3/osprofiler/drivers/sqlalchemy_driver.py` & `osprofiler-4.0.0/osprofiler/drivers/sqlalchemy_driver.py`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/osprofiler/exc.py` & `osprofiler-4.0.0/osprofiler/exc.py`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/osprofiler/hacking/checks.py` & `osprofiler-4.0.0/osprofiler/hacking/checks.py`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/osprofiler/initializer.py` & `osprofiler-4.0.0/osprofiler/initializer.py`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/osprofiler/notifier.py` & `osprofiler-4.0.0/osprofiler/notifier.py`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/osprofiler/opts.py` & `osprofiler-4.0.0/osprofiler/opts.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 * False: Disables SQL requests profiling. The spent time is only shown on a
   higher level of operations. Single SQL queries cannot be analyzed this way.
 """)
 
 _hmac_keys_opt = cfg.StrOpt(
     "hmac_keys",
     default="SECRET_KEY",
+    secret=True,
     help="""
 Secret key(s) to use for encrypting context data for performance profiling.
 
 This string value should have the following format: <key1>[,<key2>,...<keyn>],
 where each key is some random string. A user who triggers the profiling via
 the REST API has to set one of these keys in the headers of the REST API call
 to include profiling results of this node for this particular project.
@@ -166,14 +167,54 @@
     _socket_timeout_opt,
     _sentinel_service_name_opt,
     _filter_error_trace
 ]
 
 cfg.CONF.register_opts(_PROFILER_OPTS, group=_profiler_opt_group)
 
+_jaegerprofiler_opt_group = cfg.OptGroup(
+    "profiler_jaeger",
+    title="Jaeger's profiler driver related options")
+
+_service_name_prefix = cfg.StrOpt(
+    "service_name_prefix",
+    help="""
+Set service name prefix to Jaeger service name.
+""")
+
+_process_tags = cfg.DictOpt(
+    "process_tags",
+    default={},
+    help="""
+Set process tracer tags.
+""")
+
+_JAEGER_OPTS = [
+    _service_name_prefix,
+    _process_tags
+]
+
+cfg.CONF.register_opts(_JAEGER_OPTS, group=_jaegerprofiler_opt_group)
+
+_otlp_profiler_opt_group = cfg.OptGroup(
+    "profiler_otlp",
+    title="OTLP's profiler driver related options")
+
+_otlp_service_name_prefix = cfg.StrOpt(
+    "service_name_prefix",
+    help="""
+Set service name prefix to OTLP exporters.
+""")
+
+_OTLP_OPTS = [
+    _otlp_service_name_prefix,
+]
+
+cfg.CONF.register_opts(_OTLP_OPTS, group=_otlp_profiler_opt_group)
+
 
 def set_defaults(conf, enabled=None, trace_sqlalchemy=None, hmac_keys=None,
                  connection_string=None, es_doc_type=None,
                  es_scroll_time=None, es_scroll_size=None,
                  socket_timeout=None, sentinel_service_name=None):
     conf.register_opts(_PROFILER_OPTS, group=_profiler_opt_group)
 
@@ -235,8 +276,10 @@
     if conf is None:
         conf = cfg.CONF
     if conf.profiler.enabled:
         web.disable()
 
 
 def list_opts():
-    return [(_profiler_opt_group.name, _PROFILER_OPTS)]
+    return [(_profiler_opt_group.name, _PROFILER_OPTS),
+            (_jaegerprofiler_opt_group, _JAEGER_OPTS),
+            (_otlp_profiler_opt_group, _OTLP_OPTS)]
```

### Comparing `osprofiler-3.4.3/osprofiler/profiler.py` & `osprofiler-4.0.0/osprofiler/profiler.py`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/osprofiler/sqlalchemy.py` & `osprofiler-4.0.0/osprofiler/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/osprofiler/tests/functional/test_driver.py` & `osprofiler-4.0.0/osprofiler/tests/functional/test_driver.py`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/osprofiler/tests/test.py` & `osprofiler-4.0.0/osprofiler/tests/test.py`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/osprofiler/tests/unit/cmd/test_shell.py` & `osprofiler-4.0.0/osprofiler/tests/unit/cmd/test_shell.py`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/osprofiler/tests/unit/doc/test_specs.py` & `osprofiler-4.0.0/osprofiler/tests/unit/doc/test_specs.py`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/osprofiler/tests/unit/drivers/test_base.py` & `osprofiler-4.0.0/osprofiler/tests/unit/drivers/test_base.py`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/osprofiler/tests/unit/drivers/test_elasticsearch.py` & `osprofiler-4.0.0/osprofiler/tests/unit/drivers/test_elasticsearch.py`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/osprofiler/tests/unit/drivers/test_jaeger.py` & `osprofiler-4.0.0/osprofiler/tests/unit/drivers/test_jaeger.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,22 +11,32 @@
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 from unittest import mock
 
+from oslo_config import cfg
+
 from osprofiler.drivers import jaeger
+from osprofiler import opts
 from osprofiler.tests import test
 
+from jaeger_client import Config
+
 
 class JaegerTestCase(test.TestCase):
 
     def setUp(self):
         super(JaegerTestCase, self).setUp()
+
+        opts.set_defaults(cfg.CONF)
+        cfg.CONF.set_default(
+            "process_tags", "k1:v1,k2:v2", "profiler_jaeger")
+
         self.payload_start = {
             "name": "api-start",
             "base_id": "4e3e0ec6-2938-40b1-8504-09eb1d4b0dee",
             "trace_id": "1c089ea8-28fe-4f3d-8c00-f6daa2bc32f1",
             "parent_id": "e2715537-3d1c-4f0c-b3af-87355dc5fc5b",
             "timestamp": "2018-05-03T04:31:51.781381",
             "info": {
@@ -44,16 +54,20 @@
                 "host": "test",
                 "function": {
                     "result": 1
                 }
             }
         }
 
+        # Force to False as if already initialized, tracer will be None.
+        # see: jaeger_client/config.py#L374
+        Config._initialized = False
         self.driver = jaeger.Jaeger("jaeger://127.0.0.1:6831",
-                                    project="nova", service="api")
+                                    project="nova", service="api",
+                                    conf=cfg.CONF)
 
     @mock.patch("osprofiler._utils.shorten_id")
     def test_notify_start(self, mock_shorten_id):
         self.driver.notify(self.payload_start)
         calls = [
             mock.call(self.payload_start["base_id"]),
             mock.call(self.payload_start["parent_id"]),
@@ -72,7 +86,25 @@
 
         self.driver.notify(self.payload_stop)
 
         mock_time.assert_called_once()
         mock_time.reset_mock()
 
         span.finish.assert_called_once_with(finish_time=fake_time)
+
+    def test_service_name_default(self):
+        self.assertEqual("pr1-svc1", self.driver._get_service_name(
+            cfg.CONF, "pr1", "svc1"))
+
+    def test_service_name_prefix(self):
+        cfg.CONF.set_default(
+            "service_name_prefix", "prx1", "profiler_jaeger")
+        self.assertEqual("prx1-pr1-svc1", self.driver._get_service_name(
+            cfg.CONF, "pr1", "svc1"))
+
+    def test_process_tags(self):
+        tags = self.driver.tracer.tags
+        # Let's remove variable tags generated by Jaeger client
+        del tags['hostname']
+        del tags['jaeger.version']
+        del tags['ip']
+        self.assertEqual({'k1': 'v1', 'k2': 'v2'}, tags)
```

### Comparing `osprofiler-3.4.3/osprofiler/tests/unit/drivers/test_loginsight.py` & `osprofiler-4.0.0/osprofiler/tests/unit/drivers/test_loginsight.py`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/osprofiler/tests/unit/drivers/test_messaging.py` & `osprofiler-4.0.0/osprofiler/tests/unit/drivers/test_messaging.py`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/osprofiler/tests/unit/drivers/test_mongodb.py` & `osprofiler-4.0.0/osprofiler/tests/unit/drivers/test_mongodb.py`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/osprofiler/tests/unit/drivers/test_redis_driver.py` & `osprofiler-4.0.0/osprofiler/tests/unit/drivers/test_redis_driver.py`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/osprofiler/tests/unit/test_initializer.py` & `osprofiler-4.0.0/osprofiler/tests/unit/test_initializer.py`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/osprofiler/tests/unit/test_notifier.py` & `osprofiler-4.0.0/osprofiler/tests/unit/test_notifier.py`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/osprofiler/tests/unit/test_opts.py` & `osprofiler-4.0.0/osprofiler/tests/unit/test_opts.py`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/osprofiler/tests/unit/test_profiler.py` & `osprofiler-4.0.0/osprofiler/tests/unit/test_profiler.py`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/osprofiler/tests/unit/test_sqlalchemy.py` & `osprofiler-4.0.0/osprofiler/tests/unit/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/osprofiler/tests/unit/test_utils.py` & `osprofiler-4.0.0/osprofiler/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/osprofiler/tests/unit/test_web.py` & `osprofiler-4.0.0/osprofiler/tests/unit/test_web.py`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/osprofiler/web.py` & `osprofiler-4.0.0/osprofiler/web.py`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/osprofiler.egg-info/PKG-INFO` & `osprofiler-4.0.0/osprofiler.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osprofiler
-Version: 3.4.3
+Version: 4.0.0
 Summary: OpenStack Profiler Library
 Home-page: https://docs.openstack.org/osprofiler/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ===================================================
          OSProfiler -- Library for cross-project profiling
@@ -41,15 +41,14 @@
 Classifier: Environment :: OpenStack
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Provides-Extra: oslo_config
 Provides-Extra: test
```

### Comparing `osprofiler-3.4.3/playbooks/osprofiler-post.yaml` & `osprofiler-4.0.0/playbooks/osprofiler-post.yaml`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/releasenotes/notes/redis-improvement-d4c91683fc89f570.yaml` & `osprofiler-4.0.0/releasenotes/notes/redis-improvement-d4c91683fc89f570.yaml`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/releasenotes/source/conf.py` & `osprofiler-4.0.0/releasenotes/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,16 +54,16 @@
 # The encoding of source files.
 # source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
-project = u'osprofiler Release Notes'
-copyright = u'2016, osprofiler Developers'
+project = 'osprofiler Release Notes'
+copyright = '2016, osprofiler Developers'
 
 # Release notes do not need a version in the title, they span
 # multiple versions.
 # The full version, including alpha/beta/rc tags.
 release = ''
 # The short X.Y version.
 version = ''
@@ -205,16 +205,16 @@
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title,
 #  author, documentclass [howto, manual, or own class]).
 latex_documents = [
     ('index', 'osprofilerReleaseNotes.tex',
-     u'osprofiler Release Notes Documentation',
-     u'osprofiler Developers', 'manual'),
+     'osprofiler Release Notes Documentation',
+     'osprofiler Developers', 'manual'),
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
 # latex_logo = None
 
 # For "manual" documents, if this is true, then toplevel headings are parts,
@@ -236,31 +236,31 @@
 
 # -- Options for manual page output ---------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
 man_pages = [
     ('index', 'osprofilerReleaseNotes',
-     u'osprofiler Release Notes Documentation',
-     [u'osprofiler Developers'], 1)
+     'osprofiler Release Notes Documentation',
+     ['osprofiler Developers'], 1)
 ]
 
 # If true, show URL addresses after external links.
 # man_show_urls = False
 
 
 # -- Options for Texinfo output -------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
     ('index', 'osprofilerReleaseNotes',
-     u'osprofiler Release Notes Documentation',
-     u'osprofiler Developers', 'osprofilerReleaseNotes',
+     'osprofiler Release Notes Documentation',
+     'osprofiler Developers', 'osprofilerReleaseNotes',
      'One line description of project.',
      'Miscellaneous'),
 ]
 
 # Documents to append as an appendix to all manuals.
 # texinfo_appendices = []
```

### Comparing `osprofiler-3.4.3/setup.cfg` & `osprofiler-4.0.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 [metadata]
 name = osprofiler
 summary = OpenStack Profiler Library
-description-file = 
+description_file = 
 	README.rst
 author = OpenStack
-author-email = openstack-discuss@lists.openstack.org
-home-page = https://docs.openstack.org/osprofiler/latest/
-python-requires = >=3.6
+author_email = openstack-discuss@lists.openstack.org
+home_page = https://docs.openstack.org/osprofiler/latest/
+python_requires = >=3.8
 classifier = 
 	Environment :: OpenStack
 	Intended Audience :: Developers
 	Intended Audience :: Information Technology
 	License :: OSI Approved :: Apache Software License
 	Operating System :: POSIX :: Linux
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.6
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
+	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: Implementation :: CPython
 
 [files]
 packages = 
 	osprofiler
```

### Comparing `osprofiler-3.4.3/setup.py` & `osprofiler-4.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/tools/lint.py` & `osprofiler-4.0.0/tools/lint.py`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/tools/patch_tox_venv.py` & `osprofiler-4.0.0/tools/patch_tox_venv.py`

 * *Files identical despite different names*

### Comparing `osprofiler-3.4.3/tox.ini` & `osprofiler-4.0.0/tox.ini`

 * *Files 17% similar despite different names*

```diff
@@ -1,69 +1,63 @@
 [tox]
 minversion = 3.18.0
-# Needed to create ChangeLog for docs building
-skipsdist = False
 envlist = py3,pep8
-ignore_basepython_conflict = True
+ignore_basepython_conflict = true
 
 [testenv]
 basepython = python3
-setenv = VIRTUAL_ENV={envdir}
-         LANG=en_US.UTF-8
-         LANGUAGE=en_US:en
-         LC_ALL=C
+setenv =
+  LANG=en_US.UTF-8
+  LANGUAGE=en_US:en
+  LC_ALL=C
 deps =
   -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
   -r{toxinidir}/requirements.txt
   -r{toxinidir}/test-requirements.txt
 usedevelop = True
 commands = stestr run --slowest {posargs}
 distribute = false
 
-[testenv:functional]
-setenv = {[testenv]setenv}
-         OS_TEST_PATH=./osprofiler/tests/functional
+[testenv:functional{,-py38,-py39}]
+setenv =
+  {[testenv]setenv}
+  OS_TEST_PATH=./osprofiler/tests/functional
 deps =
   {[testenv]deps}
   oslo.messaging
 
-[testenv:functional-py36]
-basepython = python3.6
-setenv = {[testenv:functional]setenv}
-deps =
-  {[testenv:functional]deps}
-
 [testenv:pep8]
 commands =
   pre-commit run -a
   # Run security linter
   bandit -r osprofiler -n5
 distribute = false
 
 [testenv:venv]
 commands = {posargs}
 
 [testenv:cover]
 setenv =
-    PYTHON=coverage run --source osprofiler --parallel-mode
+  PYTHON=coverage run --source osprofiler --parallel-mode
 commands =
-    stestr run {posargs}
-    coverage combine
-    coverage html -d cover
-    coverage xml -o cover/coverage.xml
+  stestr run {posargs}
+  coverage combine
+  coverage html -d cover
+  coverage xml -o cover/coverage.xml
 
 [testenv:docs]
 deps =
-    -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
-    -r{toxinidir}/requirements.txt
-    -r{toxinidir}/doc/requirements.txt
+  -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
+  -r{toxinidir}/requirements.txt
+  -r{toxinidir}/doc/requirements.txt
 allowlist_externals = rm
 commands =
   rm -rf doc/build api-guide/build api-ref/build doc/source/contributor/modules
   sphinx-build -W --keep-going -b html -d doc/build/doctrees doc/source doc/build/html
+usedevelop = false
 
 [testenv:bandit]
 commands = bandit -r osprofiler -n5
 
 [flake8]
 show-source = true
 builtins = _
@@ -72,30 +66,30 @@
 ignore = E741,W503
 exclude=.venv,.git,.tox,dist,doc,*lib/python*,*egg,tools,setup.py,build,releasenotes
 import-order-style = pep8
 application-import-names = osprofiler
 
 [flake8:local-plugins]
 extension =
-    N301 = checks:check_assert_methods_from_mock
-    N320 = checks:assert_true_instance
-    N321 = checks:assert_equal_type
-    N322 = checks:assert_equal_none
-    N323 = checks:assert_true_or_false_with_in
-    N324 = checks:assert_equal_in
-    N351 = checks:check_no_constructor_data_struct
-    N352 = checks:check_dict_formatting_in_string
-    N353 = checks:check_using_unicode
-    N354 = checks:check_raises
+  N301 = checks:check_assert_methods_from_mock
+  N320 = checks:assert_true_instance
+  N321 = checks:assert_equal_type
+  N322 = checks:assert_equal_none
+  N323 = checks:assert_true_or_false_with_in
+  N324 = checks:assert_equal_in
+  N351 = checks:check_no_constructor_data_struct
+  N352 = checks:check_dict_formatting_in_string
+  N353 = checks:check_using_unicode
+  N354 = checks:check_raises
 paths = ./osprofiler/hacking
 
 [testenv:releasenotes]
 deps =
-    -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
-    -r{toxinidir}/doc/requirements.txt
+  -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
+  -r{toxinidir}/doc/requirements.txt
 allowlist_externals = rm
 commands =
   rm -rf releasenotes/build
   sphinx-build -a -E -W -d releasenotes/build/doctrees -b html releasenotes/source releasenotes/build/html
 
 [testenv:lower-constraints]
 deps =
```

