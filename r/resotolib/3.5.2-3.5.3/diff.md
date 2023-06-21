# Comparing `tmp/resotolib-3.5.2.tar.gz` & `tmp/resotolib-3.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotolib-3.5.2.tar", last modified: Tue Jun 13 13:11:54 2023, max compression
+gzip compressed data, was "resotolib-3.5.3.tar", last modified: Wed Jun 21 14:27:16 2023, max compression
```

## Comparing `resotolib-3.5.2.tar` & `resotolib-3.5.3.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:11:54.485172 resotolib-3.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-13 13:07:07.000000 resotolib-3.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-13 13:11:54.485172 resotolib-3.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-13 13:07:07.000000 resotolib-3.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-13 13:07:07.000000 resotolib-3.5.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:11:54.473172 resotolib-3.5.2/resotolib/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:11:54.477172 resotolib-3.5.2/resotolib/asynchronous/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/asynchronous/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/asynchronous/periodic.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/asynchronous/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:11:54.477172 resotolib-3.5.2/resotolib/asynchronous/web/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/asynchronous/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/asynchronous/web/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/asynchronous/web/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/asynchronous/web/ws_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/baseplugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    40063 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/baseresources.py
--rw-r--r--   0 runner    (1001) docker     (123)    17327 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:11:54.477172 resotolib-3.5.2/resotolib/core/
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/core/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13827 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/core/ca.py
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/core/custom_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/core/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/core/model_check.py
--rw-r--r--   0 runner    (1001) docker     (123)    15596 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/core/model_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/core/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/core/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/core/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/durations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:11:54.477172 resotolib-3.5.2/resotolib/graph/
--rw-r--r--   0 runner    (1001) docker     (123)    26663 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/graph/graph_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/json.py
--rw-r--r--   0 runner    (1001) docker     (123)    16553 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/json_bender.py
--rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/lock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:11:54.477172 resotolib-3.5.2/resotolib/log/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/parse_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11594 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/proc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    33805 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/units.py
--rw-r--r--   0 runner    (1001) docker     (123)    23264 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:11:54.481172 resotolib-3.5.2/resotolib/web/
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/web/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:11:54.481172 resotolib-3.5.2/resotolib/web/static/
--rw-r--r--   0 runner    (1001) docker     (123)    14848 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/web/static/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (123)    31503 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/web/static/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (123)    13501 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/web/static/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/web/static/browserconfig.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/web/static/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/web/static/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/web/static/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     8841 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/web/static/mstile-150x150.png
--rw-r--r--   0 runner    (1001) docker     (123)    39028 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/web/static/picnic.min.css
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/web/static/site.webmanifest
--rw-r--r--   0 runner    (1001) docker     (123)    11813 2023-06-13 13:07:07.000000 resotolib-3.5.2/resotolib/x509.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:11:54.473172 resotolib-3.5.2/resotolib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-13 13:11:54.000000 resotolib-3.5.2/resotolib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-06-13 13:11:54.000000 resotolib-3.5.2/resotolib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:11:54.000000 resotolib-3.5.2/resotolib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:08:04.000000 resotolib-3.5.2/resotolib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-13 13:11:54.000000 resotolib-3.5.2/resotolib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-13 13:11:54.000000 resotolib-3.5.2/resotolib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-13 13:11:54.485172 resotolib-3.5.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:11:54.485172 resotolib-3.5.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-13 13:07:07.000000 resotolib-3.5.2/test/test_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-13 13:07:07.000000 resotolib-3.5.2/test/test_baseresources.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-13 13:07:07.000000 resotolib-3.5.2/test/test_ca.py
--rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-06-13 13:07:07.000000 resotolib-3.5.2/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-06-13 13:07:07.000000 resotolib-3.5.2/test/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-13 13:07:07.000000 resotolib-3.5.2/test/test_graph_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-13 13:07:07.000000 resotolib-3.5.2/test/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-06-13 13:07:07.000000 resotolib-3.5.2/test/test_jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-13 13:07:07.000000 resotolib-3.5.2/test/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-13 13:07:07.000000 resotolib-3.5.2/test/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-06-13 13:07:07.000000 resotolib-3.5.2/test/test_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    15731 2023-06-13 13:07:07.000000 resotolib-3.5.2/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-06-13 13:07:07.000000 resotolib-3.5.2/test/test_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-13 13:07:07.000000 resotolib-3.5.2/test/test_x509.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:27:16.601560 resotolib-3.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-21 14:23:23.000000 resotolib-3.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-21 14:27:16.601560 resotolib-3.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-21 14:23:23.000000 resotolib-3.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-21 14:23:23.000000 resotolib-3.5.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:27:16.597560 resotolib-3.5.3/resotolib/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:27:16.597560 resotolib-3.5.3/resotolib/asynchronous/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/asynchronous/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/asynchronous/periodic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/asynchronous/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:27:16.597560 resotolib-3.5.3/resotolib/asynchronous/web/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/asynchronous/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/asynchronous/web/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/asynchronous/web/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/asynchronous/web/ws_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/baseplugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40063 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/baseresources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17397 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:27:16.597560 resotolib-3.5.3/resotolib/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9951 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/core/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13827 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/core/ca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/core/custom_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/core/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/core/model_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15596 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/core/model_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/core/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/core/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/core/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/durations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:27:16.601560 resotolib-3.5.3/resotolib/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)    26663 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/graph/graph_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16553 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/json_bender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/lock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:27:16.601560 resotolib-3.5.3/resotolib/log/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/parse_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11594 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    33805 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23264 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:27:16.601560 resotolib-3.5.3/resotolib/web/
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/web/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:27:16.601560 resotolib-3.5.3/resotolib/web/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    14848 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/web/static/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31503 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/web/static/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13501 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/web/static/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/web/static/browserconfig.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/web/static/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/web/static/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/web/static/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8841 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/web/static/mstile-150x150.png
+-rw-r--r--   0 runner    (1001) docker     (123)    39028 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/web/static/picnic.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/web/static/site.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (123)    11826 2023-06-21 14:23:23.000000 resotolib-3.5.3/resotolib/x509.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:27:16.597560 resotolib-3.5.3/resotolib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-21 14:27:16.000000 resotolib-3.5.3/resotolib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-06-21 14:27:16.000000 resotolib-3.5.3/resotolib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:27:16.000000 resotolib-3.5.3/resotolib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:24:08.000000 resotolib-3.5.3/resotolib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-21 14:27:16.000000 resotolib-3.5.3/resotolib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-21 14:27:16.000000 resotolib-3.5.3/resotolib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-21 14:27:16.601560 resotolib-3.5.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:27:16.601560 resotolib-3.5.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-21 14:23:23.000000 resotolib-3.5.3/test/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-21 14:23:23.000000 resotolib-3.5.3/test/test_baseresources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-21 14:23:23.000000 resotolib-3.5.3/test/test_ca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-06-21 14:23:23.000000 resotolib-3.5.3/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-06-21 14:23:23.000000 resotolib-3.5.3/test/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-21 14:23:23.000000 resotolib-3.5.3/test/test_graph_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-21 14:23:23.000000 resotolib-3.5.3/test/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-06-21 14:23:23.000000 resotolib-3.5.3/test/test_jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-21 14:23:23.000000 resotolib-3.5.3/test/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-21 14:23:23.000000 resotolib-3.5.3/test/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-06-21 14:23:23.000000 resotolib-3.5.3/test/test_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15731 2023-06-21 14:23:23.000000 resotolib-3.5.3/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-06-21 14:23:23.000000 resotolib-3.5.3/test/test_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-21 14:23:23.000000 resotolib-3.5.3/test/test_x509.py
```

### Comparing `resotolib-3.5.2/PKG-INFO` & `resotolib-3.5.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotolib
-Version: 3.5.2
+Version: 3.5.3
 Summary: Resoto common library.
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/resotolib
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
```

### Comparing `resotolib-3.5.2/README.md` & `resotolib-3.5.3/README.md`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.2/pyproject.toml` & `resotolib-3.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "resotolib"
-version = "3.5.2"
+version = "3.5.3"
 authors = [{name="Some Engineering Inc."}]
 description = "Resoto common library."
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
```

### Comparing `resotolib-3.5.2/resotolib/args.py` & `resotolib-3.5.3/resotolib/args.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.2/resotolib/asynchronous/periodic.py` & `resotolib-3.5.3/resotolib/asynchronous/periodic.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.2/resotolib/asynchronous/utils.py` & `resotolib-3.5.3/resotolib/asynchronous/utils.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.2/resotolib/asynchronous/web/auth.py` & `resotolib-3.5.3/resotolib/asynchronous/web/auth.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.2/resotolib/asynchronous/web/ws_handler.py` & `resotolib-3.5.3/resotolib/asynchronous/web/ws_handler.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.2/resotolib/baseplugin.py` & `resotolib-3.5.3/resotolib/baseplugin.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.2/resotolib/baseresources.py` & `resotolib-3.5.3/resotolib/baseresources.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.2/resotolib/config.py` & `resotolib-3.5.3/resotolib/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,14 +80,17 @@
 
     def __getattr__(self, name: str) -> Any:
         if name in self.running_config.data:
             return self.running_config.data[name]
         else:
             raise ConfigNotFoundError(f"No such config {name}")
 
+    def connected(self) -> bool:
+        return self._ce.connected()
+
     def shutdown(self) -> None:
         self._ce.shutdown()
 
     @staticmethod
     def init_default_config() -> None:
         for config_id, config_data in Config.running_config.classes.items():
             if config_id not in Config.running_config.data:
```

### Comparing `resotolib-3.5.2/resotolib/core/__init__.py` & `resotolib-3.5.3/resotolib/core/__init__.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.2/resotolib/core/actions.py` & `resotolib-3.5.3/resotolib/core/actions.py`

 * *Files 3% similar despite different names*

```diff
@@ -104,14 +104,18 @@
         self.message_processor = message_processor
         self.ws: Optional[websocket.WebSocketApp] = None
         self.incoming_messages = incoming_messages
         self.tls_data = tls_data
         self.shutdown_event = threading.Event()
         # one thread is taken by the queue listener
         self.executor = ThreadPoolExecutor(max_workers=max_concurrent_actions + 1, thread_name_prefix=self.identifier)
+        self.__connected = False
+
+    def connected(self) -> bool:
+        return self.__connected
 
     def run(self) -> None:
         def listen_on_queue(in_messages: Queue[Json]) -> None:
             while not self.shutdown_event.is_set():
                 with suppress(Exception):
                     message = in_messages.get(timeout=1)
                     log.debug("Got feedback message. Send it to core", message)
@@ -225,17 +229,19 @@
             except Exception:
                 log.exception(f"Something went wrong while processing {message}")
 
     def on_error(self, _: websocket.WebSocketApp, e: Exception) -> None:
         log.debug(f"{self.identifier} message bus error: {e!r}")
 
     def on_close(self, _: websocket.WebSocketApp, close_status_code: int, close_msg: str) -> None:
+        self.__connected = False
         log.debug(f"{self.identifier} disconnected from resotocore message bus: {close_status_code}: {close_msg}")
 
     def on_open(self, _: websocket.WebSocketApp) -> None:
+        self.__connected = True
         log.debug(f"{self.identifier} connected to resotocore message bus")
 
     def on_ping(self, _: websocket.WebSocketApp, message: str) -> None:
         log.debug(f"{self.identifier} actions ping from resotocore message bus")
 
     def on_pong(self, _: websocket.WebSocketApp, message: str) -> None:
         log.debug(f"{self.identifier} actions pong from resotocore message bus")
```

### Comparing `resotolib-3.5.2/resotolib/core/ca.py` & `resotolib-3.5.3/resotolib/core/ca.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.2/resotolib/core/config.py` & `resotolib-3.5.3/resotolib/core/config.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.2/resotolib/core/custom_command.py` & `resotolib-3.5.3/resotolib/core/custom_command.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.2/resotolib/core/events.py` & `resotolib-3.5.3/resotolib/core/events.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,14 +26,18 @@
         if events:
             query_string = urlencode({"show": ",".join(events)})
             self.ws_uri += f"?{query_string}"
         self.message_processor = message_processor
         self.tls_data = tls_data
         self.ws: Optional[websocket.WebSocketApp] = None
         self.shutdown_event = threading.Event()
+        self.__connected = False
+
+    def connected(self) -> bool:
+        return self.__connected
 
     def __del__(self) -> None:
         remove_event_listener(EventType.SHUTDOWN, self.shutdown)
 
     def run(self) -> None:
         self.name = "eventbus-listener"
         add_event_listener(EventType.SHUTDOWN, self.shutdown)
@@ -84,17 +88,19 @@
             except Exception:
                 log.exception(f"Something went wrong while processing {message}")
 
     def on_error(self, _: websocket.WebSocketApp, e: Exception) -> None:
         log.debug(f"Event bus error: {e!r}")
 
     def on_close(self, _: websocket.WebSocketApp, close_status_code: int, close_msg: str) -> None:
+        self.__connected = False
         log.debug("Disconnected from resotocore event bus")
 
     def on_open(self, _: websocket.WebSocketApp) -> None:
+        self.__connected = True
         log.debug("Connected to resotocore event bus")
 
     def on_ping(self, _: websocket.WebSocketApp, message: str) -> None:
         log.debug("Ping from resotocore event bus")
 
     def on_pong(self, _: websocket.WebSocketApp, message: str) -> None:
         log.debug("Pong from resotocore event bus")
```

### Comparing `resotolib-3.5.2/resotolib/core/model_check.py` & `resotolib-3.5.3/resotolib/core/model_check.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.2/resotolib/core/model_export.py` & `resotolib-3.5.3/resotolib/core/model_export.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.2/resotolib/core/progress.py` & `resotolib-3.5.3/resotolib/core/progress.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.2/resotolib/core/search.py` & `resotolib-3.5.3/resotolib/core/search.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.2/resotolib/core/tasks.py` & `resotolib-3.5.3/resotolib/core/tasks.py`

 * *Files 3% similar despite different names*

```diff
@@ -117,14 +117,18 @@
         self.resotocore_ws_uri = resotocore_ws_uri
         self.task_handler = task_handler
         self.max_workers = max_workers
         self.tls_data = tls_data
         self.ws: Optional[websocket.WebSocketApp] = None
         self.shutdown_event = threading.Event()
         self.queue: queue.Queue[Json] = queue.Queue()
+        self.__connected = False
+
+    def connected(self) -> bool:
+        return self.__connected
 
     def __del__(self) -> None:
         remove_event_listener(EventType.SHUTDOWN, self.shutdown)
 
     def run(self) -> None:
         self.name = self.identifier
         add_event_listener(EventType.SHUTDOWN, self.shutdown)
@@ -198,17 +202,19 @@
             return
         self.queue.put(jsom_message)
 
     def on_error(self, _: websocket.WebSocketApp, e: Exception) -> None:
         log.debug(f"{self.identifier} event bus error: {e!r}")
 
     def on_close(self, _: websocket.WebSocketApp, close_status_code: int, close_msg: str) -> None:
+        self.__connected = False
         log.debug(f"{self.identifier} disconnected from resotocore task queue")
 
     def on_open(self, ws: websocket.WebSocketApp) -> None:
+        self.__connected = True
         log.debug(f"{self.identifier} connected to resotocore, register at task queue")
         # when we are connected, we register at the task queue
         # by sending all task handler definitions
         ws.send(json.dumps([handler.core_json() for handler in self.task_handler]))
 
     def on_ping(self, _: websocket.WebSocketApp, message: str) -> None:
         log.debug(f"{self.identifier} tasks ping from resotocore message bus")
```

### Comparing `resotolib-3.5.2/resotolib/durations.py` & `resotolib-3.5.3/resotolib/durations.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.2/resotolib/event.py` & `resotolib-3.5.3/resotolib/event.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.2/resotolib/graph/__init__.py` & `resotolib-3.5.3/resotolib/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.2/resotolib/graph/graph_extensions.py` & `resotolib-3.5.3/resotolib/graph/graph_extensions.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.2/resotolib/json.py` & `resotolib-3.5.3/resotolib/json.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import sys
 from datetime import timedelta, datetime, date
-from typing import TypeVar, Any, Type, Optional, Union, List, get_args, Literal, get_origin, Callable, Iterable
+from typing import TypeVar, Any, Type, Optional, Union, List, get_args, Literal, get_origin, Callable, Iterable, Set
 
 from dateutil.parser import isoparse
 
 if sys.version_info >= (3, 10):
     from types import UnionType, NoneType
 else:
     UnionType = Union
@@ -90,23 +90,31 @@
     try:
         return json.dumps(to_json(node, strip_attr, strip_nulls))
     except Exception as e:
         log.debug(f"Can not serialize object {node} to json. Error: {e}")
         raise
 
 
-def to_json(node: Any, strip_attr: Union[None, str, Iterable[str]] = None, strip_nulls: bool = False) -> Json:
+def to_json(
+    node: Any,
+    strip_attr: Union[None, str, Iterable[str]] = None,
+    strip_nulls: bool = False,
+    keep_untouched: Optional[Set[str]] = None,
+) -> Json:
     """
     Use this method, if the given node is known as complex object,
     so the result will be a json object.
     """
 
     def walk_js_object(js: Json, filter_fn: Optional[Callable[[str, Any], bool]] = None) -> Json:
         result: Json = {}
         for k, v in js.items():
+            if keep_untouched and k in keep_untouched:
+                result[k] = v
+                continue
             if filter_fn and not filter_fn(k, v):
                 continue
             if isinstance(v, dict):
                 v = walk_js_object(v, filter_fn)
             elif isinstance(v, (list, tuple)):
                 v = [walk_js_object(e, filter_fn) if isinstance(e, dict) else e for e in v]
             result[k] = v
```

### Comparing `resotolib-3.5.2/resotolib/json_bender.py` & `resotolib-3.5.3/resotolib/json_bender.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.2/resotolib/jwt.py` & `resotolib-3.5.3/resotolib/jwt.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.2/resotolib/lock.py` & `resotolib-3.5.3/resotolib/lock.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.2/resotolib/logger.py` & `resotolib-3.5.3/resotolib/logger.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.2/resotolib/parse_util.py` & `resotolib-3.5.3/resotolib/parse_util.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.2/resotolib/proc.py` & `resotolib-3.5.3/resotolib/proc.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.2/resotolib/tree.py` & `resotolib-3.5.3/resotolib/tree.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.2/resotolib/utils.py` & `resotolib-3.5.3/resotolib/utils.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.2/resotolib/web/__init__.py` & `resotolib-3.5.3/resotolib/web/__init__.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.2/resotolib/web/metrics.py` & `resotolib-3.5.3/resotolib/web/metrics.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,42 @@
 import os
+from typing import Optional, Dict, Callable
+
 import cherrypy
 from prometheus_client.exposition import generate_latest, CONTENT_TYPE_LATEST
 
 
 class WebApp:
-    def __init__(self, mountpoint: str = "/") -> None:
+    def __init__(
+        self, mountpoint: str = "/", health_conditions: Optional[Dict[str, Callable[[], bool]]] = None
+    ) -> None:
         self.mountpoint = mountpoint
         local_path = os.path.abspath(os.path.dirname(__file__))
         config = {
             "tools.gzip.on": True,
             "tools.staticdir.index": "index.html",
             "tools.staticdir.on": True,
             "tools.staticdir.dir": f"{local_path}/static",
         }
         self.config = {"/": config}
+        self.health_conditions = health_conditions if health_conditions is not None else {}
         if self.mountpoint not in ("/", ""):
             self.config[self.mountpoint] = config
 
     @cherrypy.expose
     @cherrypy.tools.allow(methods=["GET"])
     def health(self) -> str:
         cherrypy.response.headers["Content-Type"] = "text/plain"
-        return "ok\r\n"
+        unhealthy = [f"- {name}" for name, fn in self.health_conditions.items() if not fn()]
+        if not unhealthy:
+            cherrypy.response.status = 200
+            return "ok\r\n"
+        else:
+            cherrypy.response.status = 503
+            cherrypy.response.headers["Content-Type"] = "text/plain"
+            return "not ok\r\n\r\n" + "\r\n".join(unhealthy) + "\r\n"
 
     @cherrypy.expose
     @cherrypy.tools.allow(methods=["GET"])
     def metrics(self) -> bytes:
         cherrypy.response.headers["Content-Type"] = CONTENT_TYPE_LATEST
         return generate_latest()
```

### Comparing `resotolib-3.5.2/resotolib/web/static/android-chrome-192x192.png` & `resotolib-3.5.3/resotolib/web/static/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.2/resotolib/web/static/android-chrome-512x512.png` & `resotolib-3.5.3/resotolib/web/static/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.2/resotolib/web/static/apple-touch-icon.png` & `resotolib-3.5.3/resotolib/web/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.2/resotolib/web/static/favicon-16x16.png` & `resotolib-3.5.3/resotolib/web/static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.2/resotolib/web/static/favicon-32x32.png` & `resotolib-3.5.3/resotolib/web/static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.2/resotolib/web/static/index.html` & `resotolib-3.5.3/resotolib/web/static/index.html`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.2/resotolib/web/static/mstile-150x150.png` & `resotolib-3.5.3/resotolib/web/static/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.2/resotolib/web/static/picnic.min.css` & `resotolib-3.5.3/resotolib/web/static/picnic.min.css`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.2/resotolib/x509.py` & `resotolib-3.5.3/resotolib/x509.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,15 +211,15 @@
 def write_key_to_file(
     key: RSAPrivateKey,
     key_path: str,
     passphrase: Optional[str] = None,
     rename: bool = True,
 ) -> None:
     tmp_key_path = f"{key_path}.tmp" if rename else key_path
-    with open(os.open(tmp_key_path, os.O_CREAT | os.O_WRONLY, 0o600), "wb") as f:
+    with open(os.open(tmp_key_path, os.O_CREAT | os.O_WRONLY | os.O_TRUNC, 0o600), "wb") as f:
         f.write(key_to_bytes(key, passphrase))
     if rename:
         os.rename(tmp_key_path, key_path)
 
 
 def key_to_bytes(
     key: RSAPrivateKey,
```

### Comparing `resotolib-3.5.2/resotolib.egg-info/PKG-INFO` & `resotolib-3.5.3/resotolib.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotolib
-Version: 3.5.2
+Version: 3.5.3
 Summary: Resoto common library.
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/resotolib
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
```

### Comparing `resotolib-3.5.2/resotolib.egg-info/SOURCES.txt` & `resotolib-3.5.3/resotolib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.2/test/test_args.py` & `resotolib-3.5.3/test/test_args.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.2/test/test_baseresources.py` & `resotolib-3.5.3/test/test_baseresources.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.2/test/test_config.py` & `resotolib-3.5.3/test/test_config.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.2/test/test_graph.py` & `resotolib-3.5.3/test/test_graph.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.2/test/test_graph_extensions.py` & `resotolib-3.5.3/test/test_graph_extensions.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.2/test/test_json.py` & `resotolib-3.5.3/test/test_json.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.2/test/test_jwt.py` & `resotolib-3.5.3/test/test_jwt.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.2/test/test_plugin.py` & `resotolib-3.5.3/test/test_plugin.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.2/test/test_tree.py` & `resotolib-3.5.3/test/test_tree.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.2/test/test_utils.py` & `resotolib-3.5.3/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.2/test/test_web.py` & `resotolib-3.5.3/test/test_web.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.2/test/test_x509.py` & `resotolib-3.5.3/test/test_x509.py`

 * *Files identical despite different names*

