# Comparing `tmp/fclogr-0.4.0.tar.gz` & `tmp/fclogr-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fclogr-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fclogr-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fclogr-0.4.0.tar` & `fclogr-0.5.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0      653 2023-06-20 23:09:40.277850 fclogr-0.4.0/.builds/main.yml
--rw-r--r--   0        0        0      635 2023-06-20 23:09:40.277850 fclogr-0.4.0/.builds/mockbuild-epel9.yml
--rw-r--r--   0        0        0      631 2023-06-20 23:09:40.277850 fclogr-0.4.0/.builds/mockbuild-f37.yml
--rw-r--r--   0        0        0      640 2023-06-20 23:09:40.277850 fclogr-0.4.0/.builds/mockbuild.yml
--rw-r--r--   0        0        0      273 2023-04-26 05:13:46.788278 fclogr-0.4.0/.copr/Makefile
--rw-r--r--   0        0        0      160 2023-06-20 23:09:40.277850 fclogr-0.4.0/.gitignore
-lrwxr-xr-x   0        0        0        0 2023-06-20 22:17:33.348915 fclogr-0.4.0/LICENSE -> LICENSES/GPL-2.0-or-later.txt
--rw-r--r--   0        0        0    17337 2023-04-15 20:35:53.456294 fclogr-0.4.0/LICENSES/GPL-2.0-or-later.txt
--rw-r--r--   0        0        0     1078 2023-04-15 16:21:50.774739 fclogr-0.4.0/LICENSES/MIT.txt
--rw-r--r--   0        0        0      881 2023-06-20 23:36:19.355132 fclogr-0.4.0/NEWS.md
--rw-r--r--   0        0        0       89 2023-04-15 20:35:53.457294 fclogr-0.4.0/NEWS.md.license
--rw-r--r--   0        0        0     8142 2023-04-26 05:13:46.788278 fclogr-0.4.0/README.md
--rwxr-xr-x   0        0        0      932 2023-04-15 16:49:14.180578 fclogr-0.4.0/contrib/fedoraify.py
--rw-r--r--   0        0        0     1275 2023-06-20 23:36:18.886133 fclogr-0.4.0/fclogr.spec
--rw-r--r--   0        0        0     4406 2023-06-20 23:19:22.167601 fclogr-0.4.0/noxfile.py
--rw-r--r--   0        0        0     2252 2023-06-20 23:09:40.277850 fclogr-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      707 2023-06-20 23:09:40.277850 fclogr-0.4.0/ruff.toml
--rw-r--r--   0        0        0      163 2023-06-20 23:36:13.039138 fclogr-0.4.0/src/fclogr/__init__.py
--rw-r--r--   0        0        0      209 2023-01-13 23:30:50.869984 fclogr-0.4.0/src/fclogr/__main__.py
--rw-r--r--   0        0        0     2047 2023-06-20 21:41:01.480167 fclogr-0.4.0/src/fclogr/cli/__init__.py
--rw-r--r--   0        0        0     1323 2023-06-20 21:41:01.481167 fclogr-0.4.0/src/fclogr/cli/base.py
--rw-r--r--   0        0        0     6857 2023-06-20 23:19:22.342601 fclogr-0.4.0/src/fclogr/cli/bump.py
--rw-r--r--   0        0        0     9932 2023-06-20 22:44:54.029677 fclogr-0.4.0/src/fclogr/cli/dev_entries.py
--rw-r--r--   0        0        0     2256 2023-04-01 04:25:07.641592 fclogr-0.4.0/src/fclogr/cli/sync.py
--rw-r--r--   0        0        0        0 2023-01-07 08:21:55.207097 fclogr-0.4.0/src/fclogr/py.typed
--rw-r--r--   0        0        0        0 2023-03-03 18:54:38.037265 fclogr-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0      292 2023-04-15 20:35:53.457294 fclogr-0.4.0/tests/conftest.py
--rw-r--r--   0        0        0     6469 2023-06-20 23:19:22.343601 fclogr-0.4.0/tests/test_bumper.py
--rw-r--r--   0        0        0      321 2023-04-27 04:27:59.767798 fclogr-0.4.0/tests/test_data/package-autospec.spec
--rw-r--r--   0        0        0      418 2023-04-01 04:25:07.638592 fclogr-0.4.0/tests/test_data/package.2.spec
--rw-r--r--   0        0        0      442 2023-03-03 22:00:05.714861 fclogr-0.4.0/tests/test_data/package.3.spec
--rw-r--r--   0        0        0      376 2023-03-03 20:18:25.858606 fclogr-0.4.0/tests/test_data/package.spec
--rw-r--r--   0        0        0      961 2023-04-15 20:35:53.457294 fclogr-0.4.0/tests/test_syncer.py
--rw-r--r--   0        0        0     9920 1970-01-01 00:00:00.000000 fclogr-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      653 2023-06-20 23:09:40.277850 fclogr-0.5.0/.builds/main.yml
+-rw-r--r--   0        0        0      635 2023-06-20 23:09:40.277850 fclogr-0.5.0/.builds/mockbuild-epel9.yml
+-rw-r--r--   0        0        0      631 2023-06-20 23:09:40.277850 fclogr-0.5.0/.builds/mockbuild-f37.yml
+-rw-r--r--   0        0        0      640 2023-06-20 23:09:40.277850 fclogr-0.5.0/.builds/mockbuild.yml
+-rw-r--r--   0        0        0      273 2023-04-26 05:13:46.788278 fclogr-0.5.0/.copr/Makefile
+-rw-r--r--   0        0        0      160 2023-06-20 23:09:40.277850 fclogr-0.5.0/.gitignore
+lrwxr-xr-x   0        0        0        0 2023-06-20 22:17:33.348915 fclogr-0.5.0/LICENSE -> LICENSES/GPL-2.0-or-later.txt
+-rw-r--r--   0        0        0    17337 2023-04-15 20:35:53.456294 fclogr-0.5.0/LICENSES/GPL-2.0-or-later.txt
+-rw-r--r--   0        0        0     1078 2023-04-15 16:21:50.774739 fclogr-0.5.0/LICENSES/MIT.txt
+-rw-r--r--   0        0        0      993 2023-06-21 01:02:33.272414 fclogr-0.5.0/NEWS.md
+-rw-r--r--   0        0        0       89 2023-04-15 20:35:53.457294 fclogr-0.5.0/NEWS.md.license
+-rw-r--r--   0        0        0     8142 2023-04-26 05:13:46.788278 fclogr-0.5.0/README.md
+-rwxr-xr-x   0        0        0      932 2023-04-15 16:49:14.180578 fclogr-0.5.0/contrib/fedoraify.py
+-rw-r--r--   0        0        0     1349 2023-06-21 01:02:32.885415 fclogr-0.5.0/fclogr.spec
+-rw-r--r--   0        0        0     4407 2023-06-20 23:39:06.178970 fclogr-0.5.0/noxfile.py
+-rw-r--r--   0        0        0     2252 2023-06-20 23:09:40.277850 fclogr-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      707 2023-06-20 23:09:40.277850 fclogr-0.5.0/ruff.toml
+-rw-r--r--   0        0        0      163 2023-06-21 01:02:28.054424 fclogr-0.5.0/src/fclogr/__init__.py
+-rw-r--r--   0        0        0      209 2023-01-13 23:30:50.869984 fclogr-0.5.0/src/fclogr/__main__.py
+-rw-r--r--   0        0        0      273 2023-06-21 00:53:26.613455 fclogr-0.5.0/src/fclogr/_util.py
+-rw-r--r--   0        0        0     2047 2023-06-20 21:41:01.480167 fclogr-0.5.0/src/fclogr/cli/__init__.py
+-rw-r--r--   0        0        0     1323 2023-06-20 21:41:01.481167 fclogr-0.5.0/src/fclogr/cli/base.py
+-rw-r--r--   0        0        0     6836 2023-06-21 00:56:05.887135 fclogr-0.5.0/src/fclogr/cli/bump.py
+-rw-r--r--   0        0        0     9989 2023-06-21 00:56:05.891135 fclogr-0.5.0/src/fclogr/cli/dev_entries.py
+-rw-r--r--   0        0        0     2256 2023-04-01 04:25:07.641592 fclogr-0.5.0/src/fclogr/cli/sync.py
+-rw-r--r--   0        0        0        0 2023-01-07 08:21:55.207097 fclogr-0.5.0/src/fclogr/py.typed
+-rw-r--r--   0        0        0        0 2023-03-03 18:54:38.037265 fclogr-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0      292 2023-04-15 20:35:53.457294 fclogr-0.5.0/tests/conftest.py
+-rw-r--r--   0        0        0     6469 2023-06-20 23:19:22.343601 fclogr-0.5.0/tests/test_bumper.py
+-rw-r--r--   0        0        0      321 2023-04-27 04:27:59.767798 fclogr-0.5.0/tests/test_data/package-autospec.spec
+-rw-r--r--   0        0        0      418 2023-04-01 04:25:07.638592 fclogr-0.5.0/tests/test_data/package.2.spec
+-rw-r--r--   0        0        0      442 2023-03-03 22:00:05.714861 fclogr-0.5.0/tests/test_data/package.3.spec
+-rw-r--r--   0        0        0      376 2023-03-03 20:18:25.858606 fclogr-0.5.0/tests/test_data/package.spec
+-rw-r--r--   0        0        0      961 2023-04-15 20:35:53.457294 fclogr-0.5.0/tests/test_syncer.py
+-rw-r--r--   0        0        0     9920 1970-01-01 00:00:00.000000 fclogr-0.5.0/PKG-INFO
```

### Comparing `fclogr-0.4.0/.builds/main.yml` & `fclogr-0.5.0/.builds/main.yml`

 * *Files identical despite different names*

### Comparing `fclogr-0.4.0/.builds/mockbuild-epel9.yml` & `fclogr-0.5.0/.builds/mockbuild-epel9.yml`

 * *Files identical despite different names*

### Comparing `fclogr-0.4.0/.builds/mockbuild-f37.yml` & `fclogr-0.5.0/.builds/mockbuild-f37.yml`

 * *Files identical despite different names*

### Comparing `fclogr-0.4.0/.builds/mockbuild.yml` & `fclogr-0.5.0/.builds/mockbuild.yml`

 * *Files identical despite different names*

### Comparing `fclogr-0.4.0/LICENSES/GPL-2.0-or-later.txt` & `fclogr-0.5.0/LICENSES/GPL-2.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `fclogr-0.4.0/LICENSES/MIT.txt` & `fclogr-0.5.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `fclogr-0.4.0/NEWS.md` & `fclogr-0.5.0/NEWS.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 NEWS
 ======
 
+## 0.5.0 - 2023-06-21 <a id='0.5.0'></a>
+
+- dev-srpm and dev-spec - escape percentage signs in commit messages
+
 ## 0.4.0 - 2023-06-20 <a id='0.4.0'></a>
 
 - bump - preserve macros when updating Version and Release
 - bump - support specfiles with `%include` statements
 - bump - properly escape percentage signs
 - bump - use relative paths in logging statements
 - RPM package - remove dependency on rpmdevtools
```

### Comparing `fclogr-0.4.0/README.md` & `fclogr-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `fclogr-0.4.0/contrib/fedoraify.py` & `fclogr-0.5.0/contrib/fedoraify.py`

 * *Files identical despite different names*

### Comparing `fclogr-0.4.0/fclogr.spec` & `fclogr-0.5.0/fclogr.spec`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # This specfile is licensed under:
 #
 # Copyright (C) 2023 Maxwell G <gotmax@e.email>
 # SPDX-License-Identifier: MIT
 # License text: https://spdx.org/licenses/MIT.html
 
 Name:           fclogr
-Version:        0.4.0
+Version:        0.5.0
 Release:        1%{?dist}
 Summary:        A tool for managing RPM changelogs and updates
 
 License:        GPL-2.0-or-later
 URL:            https://sr.ht/~gotmax23/fclogr
 %global furl    https://git.sr.ht/~gotmax23/fclogr
 Source0:        %{furl}/refs/download/v%{version}/fclogr-%{version}.tar.gz
@@ -48,14 +48,17 @@
 %license LICENSES/*.txt
 %doc README.md
 %doc NEWS.md
 %{_bindir}/fclogr*
 
 
 %changelog
+* Wed Jun 21 2023 Maxwell G <maxwell@gtmx.me> - 0.5.0-1
+- Release 0.5.0.
+
 * Tue Jun 20 2023 Maxwell G <maxwell@gtmx.me> - 0.4.0-1
 - Release 0.4.0.
 
 * Sat Apr 15 2023 Maxwell G <maxwell@gtmx.me> - 0.3.1-1
 - Release 0.3.1.
 
 * Sat Apr 15 2023 Maxwell G <maxwell@gtmx.me> - 0.3.0-1
```

### Comparing `fclogr-0.4.0/noxfile.py` & `fclogr-0.5.0/noxfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,15 @@
     ).lower() in ("", "y"):
         git(session, "push", "--follow-tags")
         session.run("hut", "git", "artifact", "upload", *iglob("dist/*"), external=True)
         copr_release(session)
 
     # Post-release bump
     session.run("releaserr", "post-version", "-s", "file")
-    git(session, "add", "src/{PROJECT}/__init__.py")
+    git(session, "add", f"src/{PROJECT}/__init__.py")
     git(session, "commit", "-S", "-m", "Post release version bump")
 
 
 @nox.session
 def copr_release(session: nox.Session):
     install(session, "copr-cli", "requests-gssapi", "specfile")
     tmp = Path(session.create_tmp())
```

### Comparing `fclogr-0.4.0/pyproject.toml` & `fclogr-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fclogr-0.4.0/ruff.toml` & `fclogr-0.5.0/ruff.toml`

 * *Files identical despite different names*

### Comparing `fclogr-0.4.0/src/fclogr/cli/__init__.py` & `fclogr-0.5.0/src/fclogr/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `fclogr-0.4.0/src/fclogr/cli/base.py` & `fclogr-0.5.0/src/fclogr/cli/base.py`

 * *Files identical despite different names*

### Comparing `fclogr-0.4.0/src/fclogr/cli/bump.py` & `fclogr-0.5.0/src/fclogr/cli/bump.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 from collections.abc import Callable, Sequence
 from pathlib import Path
 from typing import TYPE_CHECKING
 
 import specfile
 import specfile.changelog
 
+from fclogr._util import escape_percentage
 from fclogr.cli.base import Command, InvalidArgumentError
 
 if TYPE_CHECKING:
     from _typeshed import StrOrBytesPath
 
-PERCENT_MATCHER = re.compile("%([^%])?")
 # https://pagure.io/fedora-infra/rpmautospec/blob/edf18a1967f05253f937aa93ea90209459d18695/f/rpmautospec/misc.py#_11
 AUTORELEASE_RE = re.compile(
     r"%(?:autorelease(?:\s|$)|\{\??autorelease(?:\s+[^\}]*)?\})"
 )
 #
 PRE_REL_MATCHER = re.compile(r"^(0\.)(\d+)(.*)")
 REL_MATCHER = re.compile(r"^(\d+)(.*)")
@@ -63,16 +63,15 @@
         try:
             self.spec = specfile.Specfile(self.specpath, force_parse=True)
         except specfile.exceptions.SpecfileException as err:
             LOG.debug("Failed to load specfile", exc_info=True)
             raise InvalidArgumentError(f"Failed to load specfile: {err}") from None
         comment = comment or [f"Update to {self.version}." if self.version else "bump"]
         self.comment: list[str] = [
-            PERCENT_MATCHER.sub(r"%%\1", c if c.startswith("- ") else "- " + c)
-            for c in comment
+            escape_percentage(c if c.startswith("- ") else "- " + c) for c in comment
         ]
         if entry_only and version:
             raise InvalidArgumentError("--entry-only and --new are mutually exclusive.")
 
     def _write_spec(self) -> int | str:
         try:
             self.specpath.write_text(str(self.spec), encoding="utf-8")
```

### Comparing `fclogr-0.4.0/src/fclogr/cli/dev_entries.py` & `fclogr-0.5.0/src/fclogr/cli/dev_entries.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from collections.abc import Callable
 from pathlib import Path
 from typing import TYPE_CHECKING
 
 import pygit2
 import specfile as sfile
 
+from .._util import escape_percentage
 from .base import Command, InvalidArgumentError
 
 if TYPE_CHECKING:
     from _typeshed import StrOrBytesPath
 
 LOG = logging.getLogger(__name__)
 
@@ -44,15 +45,15 @@
 
     @property
     def message(self) -> list[str]:
         message = self.commit.message.splitlines()
         # --allow-empty-message
         if not message:
             message = ["bump"]
-        return ["- " + message[0]]
+        return ["- " + escape_percentage(message[0])]
 
     @property
     def author(self) -> str:
         return f"{self.commit.author.name} <{self.commit.author.email}>"
 
     @property
     def date(self) -> dt.date:
```

### Comparing `fclogr-0.4.0/src/fclogr/cli/sync.py` & `fclogr-0.5.0/src/fclogr/cli/sync.py`

 * *Files identical despite different names*

### Comparing `fclogr-0.4.0/tests/test_bumper.py` & `fclogr-0.5.0/tests/test_bumper.py`

 * *Files identical despite different names*

### Comparing `fclogr-0.4.0/tests/test_syncer.py` & `fclogr-0.5.0/tests/test_syncer.py`

 * *Files identical despite different names*

### Comparing `fclogr-0.4.0/PKG-INFO` & `fclogr-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fclogr
-Version: 0.4.0
+Version: 0.5.0
 Summary: fclogr is a tool for managing RPM changelogs and updates
 Author-email: Maxwell G <maxwell@gtmx.me>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
```

