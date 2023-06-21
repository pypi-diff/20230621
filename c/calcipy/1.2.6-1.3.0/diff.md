# Comparing `tmp/calcipy-1.2.6.tar.gz` & `tmp/calcipy-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calcipy-1.2.6.tar", max compression
+gzip compressed data, was "calcipy-1.3.0.tar", max compression
```

## Comparing `calcipy-1.2.6.tar` & `calcipy-1.3.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1066 2023-06-17 12:45:29.997841 calcipy-1.2.6/LICENSE
--rw-r--r--   0        0        0      167 2023-06-17 13:10:01.526420 calcipy-1.2.6/calcipy/__init__.py
--rw-r--r--   0        0        0     1241 2023-05-13 10:55:19.213121 calcipy-1.2.6/calcipy/can_skip.py
--rw-r--r--   0        0        0      175 2023-03-02 02:58:57.029784 calcipy-1.2.6/calcipy/check_for_stale_packages/__init__.py
--rw-r--r--   0        0        0     8307 2023-06-17 12:44:50.659243 calcipy-1.2.6/calcipy/check_for_stale_packages/_check_for_stale_packages.py
--rw-r--r--   0        0        0     6436 2023-05-17 11:02:50.475557 calcipy-1.2.6/calcipy/cli.py
--rw-r--r--   0        0        0      154 2023-03-02 02:58:57.946199 calcipy-1.2.6/calcipy/code_tag_collector/__init__.py
--rw-r--r--   0        0        0    11131 2023-06-17 12:45:50.740401 calcipy-1.2.6/calcipy/code_tag_collector/_collector.py
--rw-r--r--   0        0        0      140 2023-03-02 02:58:58.498973 calcipy-1.2.6/calcipy/dot_dict/__init__.py
--rw-r--r--   0        0        0      803 2023-02-25 23:58:05.004832 calcipy-1.2.6/calcipy/dot_dict/_dot_dict.py
--rw-r--r--   0        0        0        0 2023-04-05 02:28:27.975837 calcipy-1.2.6/calcipy/experiments/__init__.py
--rw-r--r--   0        0        0     1988 2023-05-13 11:16:09.447581 calcipy-1.2.6/calcipy/experiments/check_duplicate_test_names.py
--rw-r--r--   0        0        0     3271 2023-02-23 02:19:12.613926 calcipy-1.2.6/calcipy/file_search.py
--rw-r--r--   0        0        0     1942 2023-05-17 11:00:03.480459 calcipy-1.2.6/calcipy/invoke_helpers.py
--rw-r--r--   0        0        0      162 2023-03-02 02:58:58.973806 calcipy-1.2.6/calcipy/md_writer/__init__.py
--rw-r--r--   0        0        0     7827 2023-05-31 23:56:53.468487 calcipy-1.2.6/calcipy/md_writer/_writer.py
--rw-r--r--   0        0        0      162 2023-03-02 02:58:59.584964 calcipy-1.2.6/calcipy/noxfile/__init__.py
--rw-r--r--   0        0        0     6546 2023-04-22 15:10:18.113523 calcipy-1.2.6/calcipy/noxfile/_noxfile.py
--rw-r--r--   0        0        0     1258 2023-05-17 10:59:02.930491 calcipy-1.2.6/calcipy/scripts.py
--rw-r--r--   0        0        0        0 2023-02-21 03:18:10.928974 calcipy-1.2.6/calcipy/tasks/__init__.py
--rw-r--r--   0        0        0     3488 2023-05-17 11:01:15.749443 calcipy-1.2.6/calcipy/tasks/all_tasks.py
--rw-r--r--   0        0        0     1884 2023-05-16 23:59:46.273109 calcipy-1.2.6/calcipy/tasks/cl.py
--rw-r--r--   0        0        0     1169 2023-05-17 10:45:25.212981 calcipy-1.2.6/calcipy/tasks/defaults.py
--rw-r--r--   0        0        0     3617 2023-05-16 23:59:46.277097 calcipy-1.2.6/calcipy/tasks/doc.py
--rw-r--r--   0        0        0     3896 2023-05-28 12:34:20.588583 calcipy-1.2.6/calcipy/tasks/lint.py
--rw-r--r--   0        0        0      462 2023-05-16 23:59:46.283536 calcipy-1.2.6/calcipy/tasks/nox.py
--rw-r--r--   0        0        0     1667 2023-05-17 10:56:42.232544 calcipy-1.2.6/calcipy/tasks/pack.py
--rw-r--r--   0        0        0      565 2023-05-16 23:59:46.291723 calcipy-1.2.6/calcipy/tasks/stale.py
--rw-r--r--   0        0        0     1506 2023-05-16 23:59:46.294332 calcipy-1.2.6/calcipy/tasks/tags.py
--rw-r--r--   0        0        0     3667 2023-05-16 23:59:46.301475 calcipy-1.2.6/calcipy/tasks/test.py
--rw-r--r--   0        0        0      642 2023-05-16 23:59:46.303934 calcipy-1.2.6/calcipy/tasks/types.py
--rw-r--r--   0        0        0     6651 2023-06-17 13:10:08.138851 calcipy-1.2.6/docs/README.md
--rw-r--r--   0        0        0     6547 2023-06-17 13:10:01.567848 calcipy-1.2.6/pyproject.toml
--rw-r--r--   0        0        0    11268 1970-01-01 00:00:00.000000 calcipy-1.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-17 12:45:29.997841 calcipy-1.3.0/LICENSE
+-rw-r--r--   0        0        0      167 2023-06-21 12:44:59.035443 calcipy-1.3.0/calcipy/__init__.py
+-rw-r--r--   0        0        0     1241 2023-05-13 10:55:19.213121 calcipy-1.3.0/calcipy/can_skip.py
+-rw-r--r--   0        0        0      175 2023-03-02 02:58:57.029784 calcipy-1.3.0/calcipy/check_for_stale_packages/__init__.py
+-rw-r--r--   0        0        0     8399 2023-06-21 08:48:44.073873 calcipy-1.3.0/calcipy/check_for_stale_packages/_check_for_stale_packages.py
+-rw-r--r--   0        0        0     6436 2023-05-17 11:02:50.475557 calcipy-1.3.0/calcipy/cli.py
+-rw-r--r--   0        0        0      154 2023-03-02 02:58:57.946199 calcipy-1.3.0/calcipy/code_tag_collector/__init__.py
+-rw-r--r--   0        0        0    11270 2023-06-21 12:22:01.579173 calcipy-1.3.0/calcipy/code_tag_collector/_collector.py
+-rw-r--r--   0        0        0      140 2023-03-02 02:58:58.498973 calcipy-1.3.0/calcipy/dot_dict/__init__.py
+-rw-r--r--   0        0        0      803 2023-02-25 23:58:05.004832 calcipy-1.3.0/calcipy/dot_dict/_dot_dict.py
+-rw-r--r--   0        0        0        0 2023-04-05 02:28:27.975837 calcipy-1.3.0/calcipy/experiments/__init__.py
+-rw-r--r--   0        0        0     1988 2023-06-18 22:07:03.089724 calcipy-1.3.0/calcipy/experiments/check_duplicate_test_names.py
+-rw-r--r--   0        0        0     3271 2023-02-23 02:19:12.613926 calcipy-1.3.0/calcipy/file_search.py
+-rw-r--r--   0        0        0     1942 2023-05-17 11:00:03.480459 calcipy-1.3.0/calcipy/invoke_helpers.py
+-rw-r--r--   0        0        0      162 2023-03-02 02:58:58.973806 calcipy-1.3.0/calcipy/md_writer/__init__.py
+-rw-r--r--   0        0        0     7789 2023-06-21 12:26:00.681287 calcipy-1.3.0/calcipy/md_writer/_writer.py
+-rw-r--r--   0        0        0      162 2023-03-02 02:58:59.584964 calcipy-1.3.0/calcipy/noxfile/__init__.py
+-rw-r--r--   0        0        0     6546 2023-04-22 15:10:18.113523 calcipy-1.3.0/calcipy/noxfile/_noxfile.py
+-rw-r--r--   0        0        0     1258 2023-05-17 10:59:02.930491 calcipy-1.3.0/calcipy/scripts.py
+-rw-r--r--   0        0        0        0 2023-02-21 03:18:10.928974 calcipy-1.3.0/calcipy/tasks/__init__.py
+-rw-r--r--   0        0        0     3488 2023-05-17 11:01:15.749443 calcipy-1.3.0/calcipy/tasks/all_tasks.py
+-rw-r--r--   0        0        0     1884 2023-05-16 23:59:46.273109 calcipy-1.3.0/calcipy/tasks/cl.py
+-rw-r--r--   0        0        0     1169 2023-05-17 10:45:25.212981 calcipy-1.3.0/calcipy/tasks/defaults.py
+-rw-r--r--   0        0        0     3617 2023-05-16 23:59:46.277097 calcipy-1.3.0/calcipy/tasks/doc.py
+-rw-r--r--   0        0        0     3896 2023-05-28 12:34:20.588583 calcipy-1.3.0/calcipy/tasks/lint.py
+-rw-r--r--   0        0        0      462 2023-05-16 23:59:46.283536 calcipy-1.3.0/calcipy/tasks/nox.py
+-rw-r--r--   0        0        0     1667 2023-05-17 10:56:42.232544 calcipy-1.3.0/calcipy/tasks/pack.py
+-rw-r--r--   0        0        0      565 2023-05-16 23:59:46.291723 calcipy-1.3.0/calcipy/tasks/stale.py
+-rw-r--r--   0        0        0     1506 2023-05-16 23:59:46.294332 calcipy-1.3.0/calcipy/tasks/tags.py
+-rw-r--r--   0        0        0     3667 2023-05-16 23:59:46.301475 calcipy-1.3.0/calcipy/tasks/test.py
+-rw-r--r--   0        0        0      642 2023-05-16 23:59:46.303934 calcipy-1.3.0/calcipy/tasks/types.py
+-rw-r--r--   0        0        0     6651 2023-06-21 12:45:04.355949 calcipy-1.3.0/docs/README.md
+-rw-r--r--   0        0        0     6537 2023-06-21 12:44:59.060686 calcipy-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0    11265 1970-01-01 00:00:00.000000 calcipy-1.3.0/PKG-INFO
```

### Comparing `calcipy-1.2.6/LICENSE` & `calcipy-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.6/calcipy/can_skip.py` & `calcipy-1.3.0/calcipy/can_skip.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.6/calcipy/check_for_stale_packages/_check_for_stale_packages.py` & `calcipy-1.3.0/calcipy/check_for_stale_packages/_check_for_stale_packages.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Check for stale packages."""
 
+import asyncio
 import json
 from pathlib import Path
 
 import arrow
+import httpx
 import numpy as np
-import requests
 from arrow import Arrow
 from beartype import beartype
 from beartype.typing import Dict, List, Optional, Union
 from bidict import bidict
 from corallium.file_helpers import LOCK
 from corallium.log import logger
 from corallium.tomllib import tomllib
@@ -46,32 +47,33 @@
 #   https://pypi.org/project/pyrate-limiter/
 _RATE = RequestRate(3, 5 * Duration.SECOND)
 _LIMITER = Limiter(_RATE)
 
 
 @beartype
 @_LIMITER.ratelimit('pypi', delay=True, max_delay=10)  # type: ignore[misc]
-def _get_release_date(package: _HostedPythonPackage) -> _HostedPythonPackage:
+async def _get_release_date(package: _HostedPythonPackage) -> _HostedPythonPackage:
     """Retrieve release date metadata for the specified package.
 
     Args:
         package: `_HostedPythonPackage`
 
     Returns:
         _HostedPythonPackage: updated with release date metadata from API
 
     """
     # Retrieve the JSON summary for the specified package
     json_url = package.domain.format(name=package.name)
-    res = requests.get(json_url, timeout=30)  # nosem
-    res.raise_for_status()
-    res_json = res.json()
-    if not (releases := res_json['releases']):
-        msg = f'Failed to locate "releases" or "urls" from {json_url}: {res_json}'
-        raise RuntimeError(msg)
+    async with httpx.AsyncClient() as client:
+        res = await client.get(json_url, timeout=30)   # nosem
+        res.raise_for_status()
+        res_json = res.json()
+        if not (releases := res_json['releases']):
+            msg = f'Failed to locate "releases" or "urls" from {json_url}: {res_json}'
+            raise RuntimeError(msg)
 
     # Also retrieve the latest release date of the package looking through all releases
     release_dates = bidict({
         arrow.get(release_data[0]['upload_time_iso_8601']): version
         for version, release_data in releases.items()
         if release_data
     })
@@ -125,18 +127,18 @@
 
     updated_packages = []
     for package in packages:
         try:
             cached_package = old_cache.get(package.name)
             cached_version = '' if cached_package is None else cached_package.version
             if package.version != cached_version:
-                updated_packages.append(_get_release_date(package))
+                updated_packages.append(asyncio.run(_get_release_date(package)))
             elif cached_package:
                 updated_packages.append(cached_package)
-        except requests.exceptions.HTTPError as exc:
+        except httpx.HTTPError as exc:
             logger.warning('Could not lock package', package=package, error=str(exc))
     return updated_packages
 
 
 @beartype
 def _write_cache(updated_packages: List[_HostedPythonPackage], path_pack_lock: Path = CALCIPY_CACHE) -> None:
     """Read the cached packaging information.
```

### Comparing `calcipy-1.2.6/calcipy/cli.py` & `calcipy-1.3.0/calcipy/cli.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.6/calcipy/code_tag_collector/_collector.py` & `calcipy-1.3.0/calcipy/code_tag_collector/_collector.py`

 * *Files 3% similar despite different names*

```diff
@@ -110,32 +110,36 @@
 
         if comments := _search_lines(lines, regex_compiled):
             matches.append(_Tags(path_source=path_source, code_tags=comments))
 
     return matches
 
 
+_GITHUB_ORIGIN = r'^.+github.com[:/](?P<owner>[^/]+)/(?P<repository>[^.]+)(?:\.git)?$'
+"""Match owner and repository from a GitHub git origin URI."""
+
+
 @beartype
 def github_blame_url(clone_uri: str) -> str:
     """Format the blame URL.
 
     Args:
         clone_uri: git remote URI
 
     Returns:
        str: `repo_url`
 
     """
-    github_url = 'https://github.com/'
     # Could be ssh or http (with or without .git)
     # > git@github.com:KyleKing/calcipy.git
     # > https://github.com/KyleKing/calcipy.git
-    matches = re.findall(r'^.+github.com[:/]([^.]+)(?:\.git)?$', clone_uri)
-    with suppress(IndexError):
-        return f'{github_url}{matches[0]}'
+    matches = re.compile(_GITHUB_ORIGIN).match(clone_uri)
+    if matches:
+        github_url = 'https://github.com/'
+        return f"{github_url}{matches['owner']}/{matches['repository']}"
     return ''
 
 
 @lru_cache(maxsize=128)
 @beartype
 def _git_info(cwd: Path) -> Tuple[Path, str]:
     """Collect information about the local git repository.
@@ -312,17 +316,17 @@
         regex: compiled regular expression. Expected to have matching groups `(tag, text)`.
             Default is CODE_TAG_RE with tags from tag_order
         tags: subset of all tags to include in the report and specified order. Default is COMMON_CODE_TAGS
         header: header text
 
     """
     tag_order = [_t.strip() for _t in tags.split(',') if _t] or COMMON_CODE_TAGS
-    regex_compiled = re.compile((regex or CODE_TAG_RE).format(tag='|'.join(tag_order)))
+    matcher = (regex or CODE_TAG_RE).format(tag='|'.join(tag_order))
 
-    matches = _search_files(paths_source, regex_compiled)
+    matches = _search_files(paths_source, re.compile(matcher))
     if report := _format_report(
         base_dir, matches, tag_order=tag_order,
     ).strip():
         path_tag_summary.write_text(f'{header}\n\n{report}\n\n<!-- {SKIP_PHRASE} -->\n')
         logger.text('Created Code Tag Summary', path_tag_summary=path_tag_summary)
     elif path_tag_summary.is_file():
         path_tag_summary.unlink()
```

### Comparing `calcipy-1.2.6/calcipy/dot_dict/_dot_dict.py` & `calcipy-1.3.0/calcipy/dot_dict/_dot_dict.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.6/calcipy/experiments/check_duplicate_test_names.py` & `calcipy-1.3.0/calcipy/experiments/check_duplicate_test_names.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.6/calcipy/file_search.py` & `calcipy-1.3.0/calcipy/file_search.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.6/calcipy/invoke_helpers.py` & `calcipy-1.3.0/calcipy/invoke_helpers.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.6/calcipy/md_writer/_writer.py` & `calcipy-1.3.0/calcipy/md_writer/_writer.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import json
 import re
 from pathlib import Path
 
 import pandas as pd
 from beartype import beartype
-from beartype.typing import Any, Callable, Dict, List, Optional, Pattern
+from beartype.typing import Any, Callable, Dict, List, Optional
 from corallium.file_helpers import read_lines
 from corallium.log import logger
 from transitions import Machine
 
 from ..file_search import find_project_files_by_suffix
 from ..invoke_helpers import get_project_path
 
@@ -104,31 +104,31 @@
                 self.end()
         elif self.state == self.state_user:
             lines.append(line)
         # else: discard the lines in the auto-section
         return lines
 
 
-_RE_VAR_COMMENT_HTML = re.compile(r'<!-- {cts} (?P<key>[^=]+)=(?P<value>[^;]+);')
-"""Regex for extracting the vairable from an HTML code comment."""
+_VAR_COMMENT_HTML = r'<!-- {cts} (?P<key>[^=]+)=(?P<value>[^;]+);'
+"""Regex for extracting the variable from an HTML code comment."""
 
 
 @beartype
-def _parse_var_comment(line: str, matcher: Pattern = _RE_VAR_COMMENT_HTML) -> Dict[str, str]:  # type: ignore[type-arg]
+def _parse_var_comment(line: str, matcher: str = _VAR_COMMENT_HTML) -> Dict[str, str]:
     """Parse the variable from a matching comment.
 
     Args:
         line: string from source file
-        matcher: regex pattern to match. Default is `_RE_VAR_COMMENT_HTML`
+        matcher: string regex pattern to match. Default is `_RE_VAR_COMMENT_HTML`
 
     Returns:
         Dict[str, str]: single key and value pair based on the parsed comment
 
     """
-    if match := matcher.match(line.strip()):
+    if match := re.compile(matcher).match(line.strip()):
         matches = match.groupdict()
         return {matches['key']: matches['value']}
     return {}
 
 
 @beartype
 def _handle_source_file(line: str, path_file: Path) -> List[str]:
```

### Comparing `calcipy-1.2.6/calcipy/noxfile/_noxfile.py` & `calcipy-1.3.0/calcipy/noxfile/_noxfile.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.6/calcipy/scripts.py` & `calcipy-1.3.0/calcipy/scripts.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.6/calcipy/tasks/all_tasks.py` & `calcipy-1.3.0/calcipy/tasks/all_tasks.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.6/calcipy/tasks/cl.py` & `calcipy-1.3.0/calcipy/tasks/cl.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.6/calcipy/tasks/defaults.py` & `calcipy-1.3.0/calcipy/tasks/defaults.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.6/calcipy/tasks/doc.py` & `calcipy-1.3.0/calcipy/tasks/doc.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.6/calcipy/tasks/lint.py` & `calcipy-1.3.0/calcipy/tasks/lint.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.6/calcipy/tasks/pack.py` & `calcipy-1.3.0/calcipy/tasks/pack.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.6/calcipy/tasks/stale.py` & `calcipy-1.3.0/calcipy/tasks/stale.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.6/calcipy/tasks/tags.py` & `calcipy-1.3.0/calcipy/tasks/tags.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.6/calcipy/tasks/test.py` & `calcipy-1.3.0/calcipy/tasks/test.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.6/calcipy/tasks/types.py` & `calcipy-1.3.0/calcipy/tasks/types.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.6/docs/README.md` & `calcipy-1.3.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.6/pyproject.toml` & `calcipy-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
 
 [tool.commitizen]
-version = "1.2.6"
+version = "1.3.0"
 version_files = ["calcipy/__init__.py:^__version", "pyproject.toml:^version"]
 
 [tool.poetry]
 authors = ["Kyle King <dev.act.kyle@gmail.com>"]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Framework :: Pytest",
@@ -26,15 +26,15 @@
 include = ["LICENSE"]
 keywords = ["nox", "python-poetry"]
 license = "MIT"
 maintainers = []
 name = "calcipy"
 readme = "docs/README.md"
 repository = "https://github.com/kyleking/calcipy"
-version = "1.2.6"
+version = "1.3.0"
 
 [tool.poetry.dependencies]
 python = "^3.8.12"
 arrow = {optional = true, version = ">=1.2.3"} # tags
 autopep8 = {optional = true, version = ">=2.0.1"} # flake8
 bandit = {optional = true, version = ">=1.7.4"} # lint
 beartype = ">=0.12.0"
@@ -56,14 +56,15 @@
 flake8-sql = {optional = true, version = ">=0.4.1"} # flake8
 flake8-string-format = {optional = true, version = ">=0.3.0"} # flake8
 flake8-super = {optional = true, version = ">=0.1.3"} # flake8
 flake8-tuple = {optional = true, version = ">=0.4.1"} # flake8
 flake8-typing-imports = {optional = true, version = ">=1.14.0"} # flake8
 flake8-use-pathlib = {optional = true, version = ">=0.3.0"} # flake8
 flake8-variables-names = {optional = true, version = ">=0.0.5"} # flake8
+httpx = {optional = true, version = ">=0.24.1"} # stale
 invoke = ">=2.1.2"
 mkdocs = {optional = true, version = ">=1.4.1"} # doc
 mkdocs-build-plantuml-plugin = {optional = true, version = ">=1.7.4"} # doc
 mkdocs-gen-files = {optional = true, version = ">=0.4.0"} # doc
 mkdocs-git-revision-date-localized-plugin = {optional = true, version = ">=1.0.1"} # doc
 mkdocs-include-markdown-plugin = {markers = "python_version < '3.12'", optional = true, version = ">=4.0.3"} # doc
 mkdocs-literate-nav = {optional = true, version = ">=0.5.0"} # doc
@@ -80,15 +81,14 @@
 pyrate_limiter = {optional = true, version = ">=2.4"} # stale
 pytest = {optional = true, version = ">=7.2.1"} # test
 pytest-cov = {optional = true, version = ">=4.0.0"} # test
 pytest-randomly = {optional = true, version = ">=3.12.0"} # test
 pytest-watcher = {optional = true, version = ">=0.2.6"} # test
 python-box = {optional = true, version = ">=6.0.2"} # ddict
 pyyaml = {optional = true, version = ">=5.2"} # doc,tags
-requests = {optional = true, version = ">=2.31.0"} # stale
 ruff = {optional = true, version = ">=0.0.272"} # lint
 semgrep = {optional = true, version = ">=1.12.1"} # lint
 tabulate = {optional = true, version = ">=0.9.0"} # tags: Required for pandas to markdown
 transitions = {optional = true, version = ">=0.9.0"} # tags: docs
 
 [tool.poetry.extras]
 ddict = ["python-box"]
@@ -138,16 +138,16 @@
   "semgrep",
 ]
 nox = ["nox-poetry"]
 pylint = ["pylint"]
 stale = [
   "arrow",
   "bidict",
+  "httpx",
   "pyrate_limiter",
-  "requests",
 ]
 tags = [
   "arrow",
   "pandas",
   "pyyaml",
   "tabulate",
 ]
@@ -158,18 +158,18 @@
   "pytest-watcher",
 ]
 types = ["mypy"]
 
 [tool.poetry.group.dev.dependencies]
 # pytest-benchmark = ">=3.4.1"  # Provides the benchmark fixture
 hypothesis = {extras = ["cli"], version = ">=6.58.0"} # Use CLI with: "poetry run hypothesis write calcipy.dot_dict.ddict"
+pytest-asyncio = ">=0.21.0"
 pytest-recording = ">=0.12.0"
 pytest-subprocess = ">=1.4.1"
 types-pyyaml = ">=6.0.12.6"
-types-requests = ">=2.28.11.13"
 types-setuptools = ">=67.3.0.1"
 
 [tool.poetry.scripts]
 calcipy = "calcipy.scripts:start"
 calcipy_lint = "calcipy.scripts:start_lint"
 calcipy_tags = "calcipy.scripts:start_tags"
 calcipy_types = "calcipy.scripts:start_types"
```

### Comparing `calcipy-1.2.6/PKG-INFO` & `calcipy-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calcipy
-Version: 1.2.6
+Version: 1.3.0
 Summary: Python package to simplify development
 Home-page: https://github.com/kyleking/calcipy
 License: MIT
 Keywords: nox,python-poetry
 Author: Kyle King
 Author-email: dev.act.kyle@gmail.com
 Requires-Python: >=3.8.12,<4.0.0
@@ -52,14 +52,15 @@
 Requires-Dist: flake8-sql (>=0.4.1) ; extra == "flake8"
 Requires-Dist: flake8-string-format (>=0.3.0) ; extra == "flake8"
 Requires-Dist: flake8-super (>=0.1.3) ; extra == "flake8"
 Requires-Dist: flake8-tuple (>=0.4.1) ; extra == "flake8"
 Requires-Dist: flake8-typing-imports (>=1.14.0) ; extra == "flake8"
 Requires-Dist: flake8-use-pathlib (>=0.3.0) ; extra == "flake8"
 Requires-Dist: flake8-variables-names (>=0.0.5) ; extra == "flake8"
+Requires-Dist: httpx (>=0.24.1) ; extra == "stale"
 Requires-Dist: invoke (>=2.1.2)
 Requires-Dist: mkdocs (>=1.4.1) ; extra == "doc"
 Requires-Dist: mkdocs-build-plantuml-plugin (>=1.7.4) ; extra == "doc"
 Requires-Dist: mkdocs-gen-files (>=0.4.0) ; extra == "doc"
 Requires-Dist: mkdocs-git-revision-date-localized-plugin (>=1.0.1) ; extra == "doc"
 Requires-Dist: mkdocs-include-markdown-plugin (>=4.0.3) ; (python_version < "3.12") and (extra == "doc")
 Requires-Dist: mkdocs-literate-nav (>=0.5.0) ; extra == "doc"
@@ -76,15 +77,14 @@
 Requires-Dist: pyrate_limiter (>=2.4) ; extra == "stale"
 Requires-Dist: pytest (>=7.2.1) ; extra == "test"
 Requires-Dist: pytest-cov (>=4.0.0) ; extra == "test"
 Requires-Dist: pytest-randomly (>=3.12.0) ; extra == "test"
 Requires-Dist: pytest-watcher (>=0.2.6) ; extra == "test"
 Requires-Dist: python-box (>=6.0.2) ; extra == "ddict"
 Requires-Dist: pyyaml (>=5.2) ; extra == "doc" or extra == "tags"
-Requires-Dist: requests (>=2.31.0) ; extra == "stale"
 Requires-Dist: ruff (>=0.0.272) ; extra == "lint"
 Requires-Dist: semgrep (>=1.12.1) ; extra == "lint"
 Requires-Dist: tabulate (>=0.9.0) ; extra == "tags"
 Requires-Dist: transitions (>=0.9.0) ; extra == "doc"
 Project-URL: Bug Tracker, https://github.com/kyleking/calcipy/issues
 Project-URL: Changelog, https://github.com/kyleking/calcipy/blob/main/docs/docs/CHANGELOG.md
 Project-URL: Documentation, https://calcipy.kyleking.me
```

