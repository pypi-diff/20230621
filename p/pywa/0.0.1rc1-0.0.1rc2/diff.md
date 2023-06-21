# Comparing `tmp/pywa-0.0.1rc1.linux-x86_64.tar.gz` & `tmp/pywa-0.0.1rc2.linux-x86_64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywa-0.0.1rc1.linux-x86_64.tar", last modified: Sun Jun  4 03:57:11 2023, max compression
+gzip compressed data, was "pywa-0.0.1rc2.linux-x86_64.tar", last modified: Wed Jun 21 08:44:24 2023, max compression
```

## Comparing `pywa-0.0.1rc1.linux-x86_64.tar` & `pywa-0.0.1rc2.linux-x86_64.tar`

### file list

```diff
@@ -1,14 +1,37 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-04 03:57:11.963889 ./
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-04 03:57:11.963889 ./home/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-04 03:57:11.963889 ./home/david/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-04 03:57:11.963889 ./home/david/Downloads/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-04 03:57:11.963889 ./home/david/Downloads/test/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-04 03:57:11.963889 ./home/david/Downloads/test/venv/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-04 03:57:11.963889 ./home/david/Downloads/test/venv/lib/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-04 03:57:11.963889 ./home/david/Downloads/test/venv/lib/python3.10/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-04 03:57:11.963889 ./home/david/Downloads/test/venv/lib/python3.10/site-packages/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-04 03:57:11.963889 ./home/david/Downloads/test/venv/lib/python3.10/site-packages/pywa-0.0.1rc1.egg-info/
--rw-rw-r--   0 david     (1000) david     (1000)      132 2023-06-04 03:57:11.963889 ./home/david/Downloads/test/venv/lib/python3.10/site-packages/pywa-0.0.1rc1.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)      120 2023-06-04 03:57:11.963889 ./home/david/Downloads/test/venv/lib/python3.10/site-packages/pywa-0.0.1rc1.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2023-06-04 03:57:11.963889 ./home/david/Downloads/test/venv/lib/python3.10/site-packages/pywa-0.0.1rc1.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2023-06-04 03:57:11.963889 ./home/david/Downloads/test/venv/lib/python3.10/site-packages/pywa-0.0.1rc1.egg-info/top_level.txt
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-21 08:44:24.861170 ./
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-21 08:44:24.861170 ./home/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-21 08:44:24.861170 ./home/david/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-21 08:44:24.861170 ./home/david/Documents/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-21 08:44:24.861170 ./home/david/Documents/private/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-21 08:44:24.861170 ./home/david/Documents/private/python/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-21 08:44:24.861170 ./home/david/Documents/private/python/pywa/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-21 08:44:24.861170 ./home/david/Documents/private/python/pywa/venv/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-21 08:44:24.861170 ./home/david/Documents/private/python/pywa/venv/lib/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-21 08:44:24.861170 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-21 08:44:24.877170 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-21 08:44:24.861170 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/
+-rw-rw-r--   0 david     (1000) david     (1000)      143 2023-06-21 08:44:14.000000 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-21 08:44:24.873170 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/
+-rw-rw-r--   0 david     (1000) david     (1000)      388 2023-06-21 08:44:24.861170 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/__init__.cpython-311.pyc
+-rw-rw-r--   0 david     (1000) david     (1000)    10312 2023-06-21 08:44:24.869170 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/api.cpython-311.pyc
+-rw-rw-r--   0 david     (1000) david     (1000)    24827 2023-06-21 08:44:24.873170 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/client.cpython-311.pyc
+-rw-rw-r--   0 david     (1000) david     (1000)     1849 2023-06-21 08:44:24.869170 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/errors.cpython-311.pyc
+-rw-rw-r--   0 david     (1000) david     (1000)    27626 2023-06-21 08:44:24.869170 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/filters.cpython-311.pyc
+-rw-rw-r--   0 david     (1000) david     (1000)     3401 2023-06-21 08:44:24.869170 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/handlers.cpython-311.pyc
+-rw-rw-r--   0 david     (1000) david     (1000)    39766 2023-06-21 08:44:24.865170 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/types.cpython-311.pyc
+-rw-rw-r--   0 david     (1000) david     (1000)     2153 2023-06-21 08:44:24.861170 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/utils.cpython-311.pyc
+-rw-rw-r--   0 david     (1000) david     (1000)     6136 2023-06-21 08:44:24.865170 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/webhook.cpython-311.pyc
+-rw-rw-r--   0 david     (1000) david     (1000)     7598 2023-06-20 20:53:37.000000 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/api.py
+-rw-rw-r--   0 david     (1000) david     (1000)    22338 2023-06-20 20:45:27.000000 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py
+-rw-rw-r--   0 david     (1000) david     (1000)      989 2023-06-19 21:14:34.000000 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/errors.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12393 2023-06-20 20:14:12.000000 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1656 2023-06-20 09:34:04.000000 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/handlers.py
+-rw-rw-r--   0 david     (1000) david     (1000)    24771 2023-06-20 20:21:31.000000 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py
+-rw-rw-r--   0 david     (1000) david     (1000)      991 2023-06-20 16:58:34.000000 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/utils.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4141 2023-06-20 09:37:01.000000 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/webhook.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-21 08:44:24.877170 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa-0.0.1rc2-py3.11.egg-info/
+-rw-rw-r--   0 david     (1000) david     (1000)     4573 2023-06-21 08:44:24.877170 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa-0.0.1rc2-py3.11.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)      293 2023-06-21 08:44:24.877170 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa-0.0.1rc2-py3.11.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-06-21 08:44:24.877170 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa-0.0.1rc2-py3.11.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       51 2023-06-21 08:44:24.877170 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa-0.0.1rc2-py3.11.egg-info/requires.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        5 2023-06-21 08:44:24.877170 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa-0.0.1rc2-py3.11.egg-info/top_level.txt
```

