# Comparing `tmp/apx-changelog-1.0.16.tar.gz` & `tmp/apx-changelog-1.0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apx-changelog-1.0.16.tar", last modified: Wed Feb  3 16:25:10 2021, max compression
+gzip compressed data, was "apx-changelog-1.0.18.tar", last modified: Wed Jun 21 18:08:25 2023, max compression
```

## Comparing `apx-changelog-1.0.16.tar` & `apx-changelog-1.0.18.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-03 16:25:10.823683 apx-changelog-1.0.16/
--rw-r--r--   0 runner    (1001) docker     (121)     1075 2021-02-03 16:25:00.000000 apx-changelog-1.0.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       34 2021-02-03 16:25:00.000000 apx-changelog-1.0.16/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3488 2021-02-03 16:25:10.823683 apx-changelog-1.0.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2213 2021-02-03 16:25:00.000000 apx-changelog-1.0.16/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      103 2021-02-03 16:25:00.000000 apx-changelog-1.0.16/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-03 16:25:10.823683 apx-changelog-1.0.16/apx_changelog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3488 2021-02-03 16:25:10.000000 apx-changelog-1.0.16/apx_changelog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      294 2021-02-03 16:25:10.000000 apx-changelog-1.0.16/apx_changelog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-02-03 16:25:10.000000 apx-changelog-1.0.16/apx_changelog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       53 2021-02-03 16:25:10.000000 apx-changelog-1.0.16/apx_changelog.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2021-02-03 16:25:10.000000 apx-changelog-1.0.16/apx_changelog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2021-02-03 16:25:10.000000 apx-changelog-1.0.16/apx_changelog.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)    10937 2021-02-03 16:25:00.000000 apx-changelog-1.0.16/apxchangelog.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-02-03 16:25:10.823683 apx-changelog-1.0.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2201 2021-02-03 16:25:00.000000 apx-changelog-1.0.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:08:25.489791 apx-changelog-1.0.18/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 18:08:14.000000 apx-changelog-1.0.18/.version
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-21 18:08:14.000000 apx-changelog-1.0.18/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-21 18:08:14.000000 apx-changelog-1.0.18/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-06-21 18:08:25.489791 apx-changelog-1.0.18/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-21 18:08:14.000000 apx-changelog-1.0.18/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-21 18:08:14.000000 apx-changelog-1.0.18/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:08:25.489791 apx-changelog-1.0.18/apx_changelog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-06-21 18:08:25.000000 apx-changelog-1.0.18/apx_changelog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-21 18:08:25.000000 apx-changelog-1.0.18/apx_changelog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 18:08:25.000000 apx-changelog-1.0.18/apx_changelog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-21 18:08:25.000000 apx-changelog-1.0.18/apx_changelog.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-21 18:08:25.000000 apx-changelog-1.0.18/apx_changelog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-21 18:08:25.000000 apx-changelog-1.0.18/apx_changelog.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11045 2023-06-21 18:08:14.000000 apx-changelog-1.0.18/apxchangelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 18:08:25.489791 apx-changelog-1.0.18/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-21 18:08:14.000000 apx-changelog-1.0.18/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:08:25.489791 apx-changelog-1.0.18/templates/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      121 2023-06-21 18:08:14.000000 apx-changelog-1.0.18/templates/changes.jinja2
+-rwxr-xr-x   0 runner    (1001) docker     (123)      859 2023-06-21 18:08:14.000000 apx-changelog-1.0.18/templates/commits_format.jinja2
```

### Comparing `apx-changelog-1.0.16/LICENSE` & `apx-changelog-1.0.18/LICENSE`

 * *Files identical despite different names*

### Comparing `apx-changelog-1.0.16/README.md` & `apx-changelog-1.0.18/README.md`

 * *Files identical despite different names*

### Comparing `apx-changelog-1.0.16/apxchangelog.py` & `apx-changelog-1.0.18/apxchangelog.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python
+#!/usr/bin/env python3
 # encoding: utf-8
 
 """A tool to generate changelog markdown from a git repository."""
 
 # Copyright (c) 2021 Aliaksei Stratsilatau
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -92,15 +92,15 @@
         return '<{}: {} "{}">'.format(
             self.__class__.__name__,
             self.commit_hash[:7],
             self.date.strftime('%x %X'))
 
 
 class Changelog:
-    def __init__(self):
+    def __init__(self, ver=None):
         self.changes = ''
 
         # find repository
         self.repo = git.Repo(search_parent_directories=True)
         assert not self.repo.bare
 
         self.repo_name = '/'.join(self.repo.remotes.origin.url.replace(':', '/').split('.git')
@@ -123,20 +123,23 @@
         print('Commit: {}'.format(self.commit))
 
         self.date = datetime.datetime.fromtimestamp(
             self.repo.head.commit.committed_date)
         print('Date: {}'.format(self.date))
 
         # find current version
-        self.version = '.'.join(
-            self.repo.git.describe('--always', '--tags', '--match=v*.*')
-                .strip()
-                .replace('-', '.')
-                .split('.')[:3]
-        ).strip()
+        if ver:
+            self.version = 'v'+ver
+        else:
+            self.version = '.'.join(
+                self.repo.git.describe('--always', '--tags', '--match=v*.*')
+                    .strip()
+                    .replace('-', '.')
+                    .split('.')[:3]
+            ).strip()
         assert len(self.version) > 0
         print('Version: {}'.format(self.version))
 
     def update_changes(self, from_ref, do_comments=True, releases_repo_name=None):
 
         if not releases_repo_name:
             releases_repo_name = self.repo_name
@@ -274,15 +277,15 @@
                         help='project title for changelog file updates')
     parser.add_argument('--ver', action='store',
                         help='project version X.Y[.Z] for changelog file updates')
     parser.add_argument('--mkver', action='store',
                         help='filename to store current version (X.Y.Z)')
     args = parser.parse_args()
 
-    ch = Changelog()
+    ch = Changelog(args.ver)
 
     if args.ver:
         ch.version = 'v'+args.ver
 
     if args.ref:
         ch.update_changes(args.ref, args.comments, args.releases)
```

### Comparing `apx-changelog-1.0.16/setup.py` & `apx-changelog-1.0.18/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python
+#!/usr/bin/env python3
 # encoding: utf-8
 
 """Packaging script."""
 
 import setuptools
 import os
 import re
```

