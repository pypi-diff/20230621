# Comparing `tmp/jaraco.vcs-1.0.0.tar.gz` & `tmp/jaraco.vcs-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco.vcs-1.0.0.tar", last modified: Tue Jun 20 18:03:14 2023, max compression
+gzip compressed data, was "jaraco.vcs-1.1.0.tar", last modified: Wed Jun 21 00:48:32 2023, max compression
```

## Comparing `jaraco.vcs-1.0.0.tar` & `jaraco.vcs-1.1.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:03:14.275751 jaraco.vcs-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-20 18:02:54.000000 jaraco.vcs-1.0.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-20 18:02:54.000000 jaraco.vcs-1.0.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:03:14.267752 jaraco.vcs-1.0.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-20 18:02:54.000000 jaraco.vcs-1.0.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:03:14.267752 jaraco.vcs-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-06-20 18:02:54.000000 jaraco.vcs-1.0.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-20 18:02:54.000000 jaraco.vcs-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-20 18:02:54.000000 jaraco.vcs-1.0.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-20 18:02:54.000000 jaraco.vcs-1.0.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-20 18:02:54.000000 jaraco.vcs-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-20 18:03:14.275751 jaraco.vcs-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-20 18:02:54.000000 jaraco.vcs-1.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:03:14.267752 jaraco.vcs-1.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-20 18:02:54.000000 jaraco.vcs-1.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-20 18:02:54.000000 jaraco.vcs-1.0.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-20 18:02:54.000000 jaraco.vcs-1.0.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:03:14.263752 jaraco.vcs-1.0.0/jaraco/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:03:14.271751 jaraco.vcs-1.0.0/jaraco/vcs/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-20 18:02:54.000000 jaraco.vcs-1.0.0/jaraco/vcs/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3530 2023-06-20 18:02:54.000000 jaraco.vcs-1.0.0/jaraco/vcs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-06-20 18:02:54.000000 jaraco.vcs-1.0.0/jaraco/vcs/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-20 18:02:54.000000 jaraco.vcs-1.0.0/jaraco/vcs/library.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-20 18:02:54.000000 jaraco.vcs-1.0.0/jaraco/vcs/reentry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-06-20 18:02:54.000000 jaraco.vcs-1.0.0/jaraco/vcs/subprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:03:14.267752 jaraco.vcs-1.0.0/jaraco.vcs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-20 18:03:14.000000 jaraco.vcs-1.0.0/jaraco.vcs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-20 18:03:14.000000 jaraco.vcs-1.0.0/jaraco.vcs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 18:03:14.000000 jaraco.vcs-1.0.0/jaraco.vcs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-20 18:03:14.000000 jaraco.vcs-1.0.0/jaraco.vcs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 18:03:14.000000 jaraco.vcs-1.0.0/jaraco.vcs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-20 18:02:54.000000 jaraco.vcs-1.0.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-20 18:02:54.000000 jaraco.vcs-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-20 18:02:54.000000 jaraco.vcs-1.0.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-20 18:03:14.275751 jaraco.vcs-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:03:14.271751 jaraco.vcs-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 18:02:54.000000 jaraco.vcs-1.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-20 18:02:54.000000 jaraco.vcs-1.0.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-20 18:02:54.000000 jaraco.vcs-1.0.0/tests/test_git.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-20 18:02:54.000000 jaraco.vcs-1.0.0/tests/test_managers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-06-20 18:02:54.000000 jaraco.vcs-1.0.0/tests/test_mercurial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-06-20 18:02:54.000000 jaraco.vcs-1.0.0/tests/test_reentry.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-20 18:02:54.000000 jaraco.vcs-1.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:48:32.724885 jaraco.vcs-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-21 00:48:05.000000 jaraco.vcs-1.1.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-21 00:48:05.000000 jaraco.vcs-1.1.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:48:32.720885 jaraco.vcs-1.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-21 00:48:05.000000 jaraco.vcs-1.1.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:48:32.720885 jaraco.vcs-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-06-21 00:48:05.000000 jaraco.vcs-1.1.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-21 00:48:05.000000 jaraco.vcs-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-21 00:48:05.000000 jaraco.vcs-1.1.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-21 00:48:05.000000 jaraco.vcs-1.1.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-21 00:48:05.000000 jaraco.vcs-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-06-21 00:48:32.724885 jaraco.vcs-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-06-21 00:48:05.000000 jaraco.vcs-1.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:48:32.720885 jaraco.vcs-1.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-21 00:48:05.000000 jaraco.vcs-1.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-21 00:48:05.000000 jaraco.vcs-1.1.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-21 00:48:05.000000 jaraco.vcs-1.1.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:48:32.716885 jaraco.vcs-1.1.0/jaraco/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:48:32.720885 jaraco.vcs-1.1.0/jaraco/vcs/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-21 00:48:05.000000 jaraco.vcs-1.1.0/jaraco/vcs/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3553 2023-06-21 00:48:05.000000 jaraco.vcs-1.1.0/jaraco/vcs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-06-21 00:48:05.000000 jaraco.vcs-1.1.0/jaraco/vcs/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-21 00:48:05.000000 jaraco.vcs-1.1.0/jaraco/vcs/library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-21 00:48:05.000000 jaraco.vcs-1.1.0/jaraco/vcs/reentry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-21 00:48:05.000000 jaraco.vcs-1.1.0/jaraco/vcs/subprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:48:32.720885 jaraco.vcs-1.1.0/jaraco.vcs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-06-21 00:48:32.000000 jaraco.vcs-1.1.0/jaraco.vcs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-21 00:48:32.000000 jaraco.vcs-1.1.0/jaraco.vcs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 00:48:32.000000 jaraco.vcs-1.1.0/jaraco.vcs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-21 00:48:32.000000 jaraco.vcs-1.1.0/jaraco.vcs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-21 00:48:32.000000 jaraco.vcs-1.1.0/jaraco.vcs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-21 00:48:05.000000 jaraco.vcs-1.1.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-21 00:48:05.000000 jaraco.vcs-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-21 00:48:05.000000 jaraco.vcs-1.1.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-21 00:48:32.724885 jaraco.vcs-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:48:32.724885 jaraco.vcs-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 00:48:05.000000 jaraco.vcs-1.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-21 00:48:05.000000 jaraco.vcs-1.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-21 00:48:05.000000 jaraco.vcs-1.1.0/tests/test_git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-21 00:48:05.000000 jaraco.vcs-1.1.0/tests/test_managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-06-21 00:48:05.000000 jaraco.vcs-1.1.0/tests/test_mercurial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-06-21 00:48:05.000000 jaraco.vcs-1.1.0/tests/test_reentry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-21 00:48:05.000000 jaraco.vcs-1.1.0/tox.ini
```

### Comparing `jaraco.vcs-1.0.0/.github/workflows/main.yml` & `jaraco.vcs-1.1.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `jaraco.vcs-1.0.0/LICENSE` & `jaraco.vcs-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jaraco.vcs-1.0.0/PKG-INFO` & `jaraco.vcs-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaraco.vcs
-Version: 1.0.0
+Version: 1.1.0
 Summary: Facilities for working with VCS repositories
 Home-page: https://github.com/jaraco/jaraco.vcs
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -77,10 +77,10 @@
 For example, if the repo contains the tags 0.1, 0.2, and 0.3 and the
 repo is not on any of those tags, get_current_version will return
 '0.3.1dev' and get_current_version(increment='0.1') will return
 '0.4dev'.
 
 Example::
 
-    >>> from jaraco.vcs import RepoManager
-    >>> RepoManager().get_first_valid_manager().get_current_version()
+    >>> import jaraco.vcs
+    >>> jaraco.vcs.repo().get_current_version()
     '9.0.1.dev0'
```

### Comparing `jaraco.vcs-1.0.0/README.rst` & `jaraco.vcs-1.1.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -59,10 +59,10 @@
 For example, if the repo contains the tags 0.1, 0.2, and 0.3 and the
 repo is not on any of those tags, get_current_version will return
 '0.3.1dev' and get_current_version(increment='0.1') will return
 '0.4dev'.
 
 Example::
 
-    >>> from jaraco.vcs import RepoManager
-    >>> RepoManager().get_first_valid_manager().get_current_version()
+    >>> import jaraco.vcs
+    >>> jaraco.vcs.repo().get_current_version()
     '9.0.1.dev0'
```

### Comparing `jaraco.vcs-1.0.0/docs/conf.py` & `jaraco.vcs-1.1.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     )
 }
 
 # Be strict about any broken references
 nitpicky = True
 
 nitpick_ignore = [
-    ('py:class', 'jaraco.versioning.VersionManagement'),
+    ('py:class', 'jaraco.versioning.Versioned'),
 ]
 
 # Include Python intersphinx mapping to prevent failures
 # jaraco/skeleton#51
 extensions += ['sphinx.ext.intersphinx']
 intersphinx_mapping = {
     'python': ('https://docs.python.org/3', None),
```

### Comparing `jaraco.vcs-1.0.0/jaraco/vcs/base.py` & `jaraco.vcs-1.1.0/jaraco/vcs/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import itertools
 
 import jaraco.versioning as versioning
 from jaraco.classes.ancestry import iter_subclasses
 from more_itertools import one
 
 
-class RepoManager(versioning.VersionManagement, object):
+class Repo(versioning.VersionManagement):
     """
     An abstract class defining some interfaces for working with
     repositories.
     """
 
     def __init__(self, location='.'):
         self.location = location
@@ -38,21 +38,24 @@
             return getattr(c, 'priority', 0)
 
         classes = sorted(iter_subclasses(cls), key=by_priority_attr, reverse=True)
         all_managers = (c(location) for c in classes)
         return (mgr for mgr in all_managers if mgr.is_valid())
 
     @staticmethod
-    def get_first_valid_manager(location='.'):
+    def detect(location='.'):
         try:
-            return next(RepoManager.get_valid_managers(location))
+            return next(Repo.get_valid_managers(location))
         except StopIteration as e:
             e.args = ("No source repo or suitable VCS version found",)
             raise
 
+    # for compatibility
+    get_first_valid_manager = detect
+
     @staticmethod
     def existing_only(managers):
         """
         Return only those managers that refer to an existing repo
         """
         return (mgr for mgr in managers if mgr.find_root())
```

### Comparing `jaraco.vcs-1.0.0/jaraco/vcs/cmd.py` & `jaraco.vcs-1.1.0/jaraco/vcs/cmd.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 class Command:
     def is_valid(self):
         try:
             # Check if both command and repo are valid
             self._invoke('status')
         except Exception:
             return False
-        return super(Command, self).is_valid()
+        return super().is_valid()
 
     def version(self):
         """
         Return the underlying version
         """
         lines = iter(self._invoke('version').splitlines())
         version = next(lines).strip()
@@ -62,15 +62,15 @@
         current revision if not specified).
         """
         rev_num = self._get_rev_num(rev)
         # rev_num might end with '+', indicating local modifications.
         return (
             set(self._read_tags_for_rev(rev_num))
             if not rev_num.endswith('+')
-            else set([])
+            else set()
         )
 
     def _read_tags_for_rev(self, rev_num):
         """
         Return the tags for revision sorted by when the tags were
         created (latest first)
         """
@@ -113,17 +113,17 @@
         by_revision = operator.attrgetter('revision')
         tags = sorted(self.get_tags(), key=by_revision)
         revision_tags = itertools.groupby(tags, key=by_revision)
 
         def get_id(rev):
             return rev.split(':', 1)[0]
 
-        return dict(
-            (get_id(rev), [tr.tag for tr in tr_list]) for rev, tr_list in revision_tags
-        )
+        return {
+            get_id(rev): [tr.tag for tr in tr_list] for rev, tr_list in revision_tags
+        }
 
     def get_repo_tags(self):
         lines = self._invoke('tags').splitlines()
         return (TaggedRevision(*line.rsplit(None, 1)) for line in lines if line)
 
     def get_ancestral_tags(self, rev='.'):
         """
@@ -139,19 +139,21 @@
 
 
 class Git(Command):
     exe = 'git'
     version_pattern = r'git version (\d+\.\d+[^ ]*)'
 
     def is_valid(self):
-        return super(Git, self).is_valid() and self.version_suitable()
+        return super().is_valid() and self.version_suitable()
 
     def version_suitable(self):
         req_ver = packaging.version.Version('1.7.10')
-        act_ver = packaging.version.Version(self.version())
+        act_ver = packaging.version.Version(
+            self.version().replace('.windows', '+windows')
+        )
         return act_ver >= req_ver
 
     def find_root(self):
         try:
             return self._invoke('rev-parse', '--top-level').strip()
         except Exception:
             pass
@@ -179,7 +181,16 @@
         return (TaggedRevision(*line.rsplit(None, 1)) for line in lines if line)
 
     def is_modified(self):
         """
         Is the current state modified? (currently stubbed assuming no)
         """
         return False
+
+    def get_ancestral_tags(self, rev=None):
+        """
+        Like get_repo_tags, but only get those tags ancestral to the current
+        changeset.
+        """
+        rev = rev or 'HEAD'
+        matches = self._invoke('tags', '--merged', rev).splitlines()
+        return (rev for rev in self.get_repo_tags() if rev.tag in matches)
```

### Comparing `jaraco.vcs-1.0.0/jaraco/vcs/library.py` & `jaraco.vcs-1.1.0/jaraco/vcs/library.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 
 from . import base
 from . import cmd
 from . import reentry
 
 
-class MercurialInProcManager(cmd.Mercurial, base.RepoManager):
+class Mercurial(cmd.Mercurial, base.Repo):
     """
     A RepoManager implemented by invoking the hg command in-process.
     """
 
     def _invoke(self, *params):
         """
         Run the self.exe command in-process with the supplied params.
```

### Comparing `jaraco.vcs-1.0.0/jaraco/vcs/reentry.py` & `jaraco.vcs-1.1.0/jaraco/vcs/reentry.py`

 * *Files identical despite different names*

### Comparing `jaraco.vcs-1.0.0/jaraco/vcs/subprocess.py` & `jaraco.vcs-1.1.0/jaraco/vcs/subprocess.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,17 +22,17 @@
         )
         stdout, stderr = proc.communicate()
         if not proc.returncode == 0:
             raise RuntimeError(stderr.strip() or stdout.strip())
         return stdout.decode('utf-8')
 
 
-class MercurialManager(Subprocess, cmd.Mercurial, base.RepoManager):
+class Mercurial(Subprocess, cmd.Mercurial, base.Repo):
     """
-    A RepoManager implemented by calling into the 'hg' command-line
+    A Repo implemented by calling into the 'hg' command-line
     as a subprocess.
     """
 
     priority = 1 + os.path.isdir('.hg')
 
     @property
     def env(self):
@@ -45,14 +45,14 @@
         https://github.com/jaraco/jaraco.vcs/issues/7 for details.
         """
         env = os.environ.copy()
         env.pop('MACOSX_DEPLOYMENT_TARGET', None)
         return env
 
 
-class GitManager(Subprocess, cmd.Git, base.RepoManager):
+class Git(Subprocess, cmd.Git, base.Repo):
     """
     A RepoManager implemented by calling into the 'git' command-line
     as a subprocess.
     """
 
     priority = 1 + os.path.isdir('.git')
```

### Comparing `jaraco.vcs-1.0.0/jaraco.vcs.egg-info/PKG-INFO` & `jaraco.vcs-1.1.0/jaraco.vcs.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaraco.vcs
-Version: 1.0.0
+Version: 1.1.0
 Summary: Facilities for working with VCS repositories
 Home-page: https://github.com/jaraco/jaraco.vcs
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -77,10 +77,10 @@
 For example, if the repo contains the tags 0.1, 0.2, and 0.3 and the
 repo is not on any of those tags, get_current_version will return
 '0.3.1dev' and get_current_version(increment='0.1') will return
 '0.4dev'.
 
 Example::
 
-    >>> from jaraco.vcs import RepoManager
-    >>> RepoManager().get_first_valid_manager().get_current_version()
+    >>> import jaraco.vcs
+    >>> jaraco.vcs.repo().get_current_version()
     '9.0.1.dev0'
```

### Comparing `jaraco.vcs-1.0.0/jaraco.vcs.egg-info/SOURCES.txt` & `jaraco.vcs-1.1.0/jaraco.vcs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jaraco.vcs-1.0.0/pytest.ini` & `jaraco.vcs-1.1.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `jaraco.vcs-1.0.0/setup.cfg` & `jaraco.vcs-1.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `jaraco.vcs-1.0.0/tests/conftest.py` & `jaraco.vcs-1.1.0/tests/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,27 +24,27 @@
         baz="",
     ),
 )
 
 
 @pytest.fixture
 def hg_repo(temp_work_dir):
-    mgr = vcs.MercurialManager()
+    mgr = vcs.Mercurial()
     _ensure_present(mgr)
     mgr._invoke('init', '.')
     jaraco.path.build(source_tree)
     mgr._invoke('addremove')
     mgr._invoke('ci', '-m', 'committed')
     pathlib.Path('bar/baz').write_text('content', encoding='utf-8')
     mgr._invoke('ci', '-m', 'added content')
 
 
 @pytest.fixture
 def git_repo(temp_work_dir):
-    mgr = vcs.GitManager()
+    mgr = vcs.Git()
     _ensure_present(mgr)
     mgr._invoke('init')
     mgr._invoke('config', 'user.email', 'vip@example.com')
     mgr._invoke('config', 'user.name', 'Important User')
     jaraco.path.build(source_tree)
     mgr._invoke('add', '.')
     mgr._invoke('commit', '-m', 'committed')
```

### Comparing `jaraco.vcs-1.0.0/tests/test_git.py` & `jaraco.vcs-1.1.0/tests/test_git.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,33 +10,33 @@
 def test_subprocess_manager_invalid_when_exe_missing():
     """
     If the hg executable dosen't exist, the manager should report
     False for .is_valid().
     """
     non_existent_exe = '/non_existent_executable'
     assert not os.path.exists(non_existent_exe)
-    mgr = subprocess.GitManager()
+    mgr = subprocess.Git()
     mgr.exe = non_existent_exe
     assert not mgr.is_valid()
 
 
 @pytest.mark.usefixtures("git_repo")
 class TestTags:
     def setup_method(self, method):
-        self.mgr = vcs.GitManager('.')
+        self.mgr = vcs.Git('.')
 
     def teardown_method(self, method):
         del self.mgr
 
     def test_single_tag(self):
-        assert self.mgr.get_tags() == set([])
+        assert self.mgr.get_tags() == set()
         self.mgr._invoke('tag', '-am', "Tagging 1.0", '1.0')
-        assert self.mgr.get_tags() == set(['1.0'])
+        assert self.mgr.get_tags() == {'1.0'}
         self.mgr._invoke('checkout', '1.0')
-        assert self.mgr.get_tags() == set(['1.0'])
+        assert self.mgr.get_tags() == {'1.0'}
 
 
 class TestParseVersion:
     def test_simple(self):
         assert cmd.Git._parse_version('git version 1.9.3') == '1.9.3'
 
     def test_trailing_mess(self):
```

### Comparing `jaraco.vcs-1.0.0/tests/test_managers.py` & `jaraco.vcs-1.1.0/tests/test_managers.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 
 def test_existing_only():
     """
     Test the static method RepoManager.existing_only.
     """
     # presumably, '/' is never an hg repo - at least for our purposes, that's
     #  a reasonable assumption.
-    mgrs = vcs.RepoManager.get_valid_managers('/')
-    existing = list(vcs.RepoManager.existing_only(mgrs))
+    mgrs = vcs.Repo.get_valid_managers('/')
+    existing = list(vcs.Repo.existing_only(mgrs))
     assert not existing
 
 
 @mock.patch.object(
-    vcs.RepoManager,
+    vcs.Repo,
     'get_valid_managers',
     classmethod(lambda cls, location: iter(())),
 )
 def test_no_valid_managers():
     """
     When no valid managers can be found, a StopIteration is raised providing
     a nice message.
     """
     with pytest.raises(StopIteration) as err:
-        vcs.RepoManager.get_first_valid_manager()
+        vcs.Repo.get_first_valid_manager()
     assert 'no source repo' in str(err).lower()
```

### Comparing `jaraco.vcs-1.0.0/tests/test_mercurial.py` & `jaraco.vcs-1.1.0/tests/test_mercurial.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,106 +17,106 @@
     class to bypass this issue.
     """
     if platform.system() != 'Windows':
         return
 
     def _invoke(self, *params):
         params = ('--config', 'ui.username=tester') + params
-        return super(subprocess.MercurialManager, self)._invoke(*params)
+        return super(subprocess.Mercurial, self)._invoke(*params)
 
-    monkeypatch.setattr(subprocess.MercurialManager, '_invoke', _invoke)
+    monkeypatch.setattr(subprocess.Mercurial, '_invoke', _invoke)
 
 
 def test_subprocess_manager_invalid_when_exe_missing():
     """
     If the hg executable dosen't exist, the manager should report
     False for .is_valid().
     """
     non_existent_exe = '/non_existent_executable'
     assert not os.path.exists(non_existent_exe)
-    mgr = subprocess.MercurialManager()
+    mgr = subprocess.Mercurial()
     mgr.exe = non_existent_exe
     assert not mgr.is_valid()
 
 
 @pytest.mark.usefixtures("hg_repo")
 class TestRelativePaths:
     """
     Issue #9 demonstrated that the Manager would inadvertently return too many
     files when location is not the root of the repo. This test demonstrates
     the expected behavior.
     """
 
     def test_nested_child(self):
-        test_mgr = vcs.MercurialManager('.')
+        test_mgr = vcs.Mercurial('.')
         assert test_mgr.find_files() == [os.path.join('bar', 'baz')]
 
     def test_manager_in_child(self):
-        test_mgr = vcs.MercurialManager('bar')
+        test_mgr = vcs.Mercurial('bar')
         assert test_mgr.find_files() == ['baz']
 
     def test_current_dir_in_child(self):
         os.chdir('bar')
-        test_mgr = vcs.MercurialManager('.')
+        test_mgr = vcs.Mercurial('.')
         assert test_mgr.find_files() == ['baz']
 
 
 @pytest.mark.usefixtures("hg_repo")
 class TestTags:
     def setup_method(self, method):
-        self.mgr = vcs.MercurialManager('.')
+        self.mgr = vcs.Mercurial('.')
 
     def teardown_method(self, method):
         del self.mgr
 
     def test_single_tag(self):
         self.mgr._invoke('tag', '1.0')
-        assert self.mgr.get_tags() == set(['tip'])
+        assert self.mgr.get_tags() == {'tip'}
         self.mgr._invoke('update', '1.0')
-        assert self.mgr.get_tags() == set(['1.0'])
+        assert self.mgr.get_tags() == {'1.0'}
 
     def test_no_tags(self):
         "No tag should return empty set"
-        assert self.mgr.get_tags('0') == set([])
+        assert self.mgr.get_tags('0') == set()
 
     def test_local_modifications(self):
         "Local modifications should return empty set"
         with open('bar/baz', 'w', encoding='utf-8') as f:
             f.write('changed')
-        assert self.mgr.get_tags() == set([])
+        assert self.mgr.get_tags() == set()
 
     def test_parent_tag(self):
         self.mgr._invoke('tag', '1.0')
-        assert self.mgr.get_tags() == set(['tip'])
-        assert self.mgr.get_parent_tags() == set(['tip'])
-        assert self.mgr.get_parent_tags('.') == set(['1.0'])
-        assert self.mgr.get_parent_tags('tip') == set(['1.0'])
+        assert self.mgr.get_tags() == {'tip'}
+        assert self.mgr.get_parent_tags() == {'tip'}
+        assert self.mgr.get_parent_tags('.') == {'1.0'}
+        assert self.mgr.get_parent_tags('tip') == {'1.0'}
         self.mgr._invoke('tag', '1.1')
-        assert self.mgr.get_tags() == set(['tip'])
-        assert self.mgr.get_parent_tags() == set(['tip'])
-        assert self.mgr.get_parent_tags('.') == set(['1.1'])
-        assert self.mgr.get_parent_tags('tip') == set(['1.1'])
+        assert self.mgr.get_tags() == {'tip'}
+        assert self.mgr.get_parent_tags() == {'tip'}
+        assert self.mgr.get_parent_tags('.') == {'1.1'}
+        assert self.mgr.get_parent_tags('tip') == {'1.1'}
 
     def test_two_tags_same_revision(self):
         """
         Always return the latest tag for a given revision
         """
         self.mgr._invoke('tag', '1.0')
         self.mgr._invoke('tag', '-r', '1.0', '1.1')
         self.mgr._invoke('update', '1.0')
-        assert set(self.mgr.get_tags()) == set(['1.0', '1.1'])
+        assert set(self.mgr.get_tags()) == {'1.0', '1.1'}
 
     def test_two_tags_same_revision_lexicographically_earlier(self):
         """
         Always return the latest tag for a given revision
         """
         self.mgr._invoke('tag', '1.9')
         self.mgr._invoke('tag', '-r', '1.9', '1.10')
         self.mgr._invoke('update', '1.9')
-        assert set(self.mgr.get_tags()) == set(['1.9', '1.10'])
+        assert set(self.mgr.get_tags()) == {'1.9', '1.10'}
 
     def _setup_branchy_tags(self):
         """
         Create two heads, one which has a 1.0 tag and a different one which
         has a 1.1 tag.
         """
         # create a commit with a tag
```

### Comparing `jaraco.vcs-1.0.0/tests/test_reentry.py` & `jaraco.vcs-1.1.0/tests/test_reentry.py`

 * *Files identical despite different names*

### Comparing `jaraco.vcs-1.0.0/tox.ini` & `jaraco.vcs-1.1.0/tox.ini`

 * *Files identical despite different names*

