# Comparing `tmp/autotools-0.4.tar.gz` & `tmp/autotools-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotools-0.4.tar", last modified: Tue Jun 20 17:16:22 2023, max compression
+gzip compressed data, was "autotools-0.5.tar", last modified: Tue Jun 20 18:12:33 2023, max compression
```

## Comparing `autotools-0.4.tar` & `autotools-0.5.tar`

### file list

```diff
@@ -1,12 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 17:16:22.090422 autotools-0.4/
--rw-rw-rw-   0        0        0      324 2023-06-20 17:16:22.074795 autotools-0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-20 17:16:22.027457 autotools-0.4/autotools/
--rw-rw-rw-   0        0        0      637 2023-06-20 17:04:47.000000 autotools-0.4/autotools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 17:16:22.074795 autotools-0.4/autotools.egg-info/
--rw-rw-rw-   0        0        0      324 2023-06-20 17:16:21.000000 autotools-0.4/autotools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2023-06-20 17:16:21.000000 autotools-0.4/autotools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 17:16:21.000000 autotools-0.4/autotools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-20 17:16:21.000000 autotools-0.4/autotools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2023-06-20 17:16:21.000000 autotools-0.4/autotools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-20 17:16:22.090422 autotools-0.4/setup.cfg
--rw-rw-rw-   0        0        0      467 2023-06-20 17:16:14.000000 autotools-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 18:12:33.170534 autotools-0.5/
+-rw-rw-rw-   0        0        0      195 2023-06-20 18:12:33.167532 autotools-0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-20 18:12:33.045408 autotools-0.5/autotools/
+-rw-rw-rw-   0        0        0      157 2023-06-20 18:04:02.000000 autotools-0.5/autotools/__init__.py
+-rw-rw-rw-   0        0        0     1802 2023-06-20 17:55:20.000000 autotools-0.5/autotools/audio.py
+-rw-rw-rw-   0        0        0     2403 2023-06-20 18:11:14.000000 autotools-0.5/autotools/chatgpt.py
+-rw-rw-rw-   0        0        0     3472 2023-06-20 18:09:15.000000 autotools-0.5/autotools/chatgpt_presets.py
+-rw-rw-rw-   0        0        0     2221 2023-06-20 18:11:43.000000 autotools-0.5/autotools/chats.py
+-rw-rw-rw-   0        0        0      899 2023-06-20 18:03:35.000000 autotools-0.5/autotools/img.py
+-rw-rw-rw-   0        0        0      833 2023-06-20 18:07:02.000000 autotools-0.5/autotools/module_get.py
+-rw-rw-rw-   0        0        0      380 2023-06-20 17:42:44.000000 autotools-0.5/autotools/to_ipv4.py
+drwxrwxrwx   0        0        0        0 2023-06-20 18:12:33.160534 autotools-0.5/autotools.egg-info/
+-rw-rw-rw-   0        0        0      195 2023-06-20 18:12:32.000000 autotools-0.5/autotools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      344 2023-06-20 18:12:32.000000 autotools-0.5/autotools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 18:12:32.000000 autotools-0.5/autotools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-06-20 18:12:32.000000 autotools-0.5/autotools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-20 18:12:32.000000 autotools-0.5/autotools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 18:12:33.171532 autotools-0.5/setup.cfg
+-rw-rw-rw-   0        0        0      549 2023-06-20 18:02:44.000000 autotools-0.5/setup.py
```

