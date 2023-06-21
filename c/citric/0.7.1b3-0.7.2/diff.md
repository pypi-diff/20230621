# Comparing `tmp/citric-0.7.1b3.tar.gz` & `tmp/citric-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citric-0.7.1b3.tar", max compression
+gzip compressed data, was "citric-0.7.2.tar", max compression
```

## Comparing `citric-0.7.1b3.tar` & `citric-0.7.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1083 2023-06-01 04:42:30.650182 citric-0.7.1b3/LICENSE
--rw-r--r--   0        0        0     4775 2023-06-01 04:42:30.650182 citric-0.7.1b3/README.md
--rw-r--r--   0        0        0     4390 2023-06-01 04:42:30.654182 citric-0.7.1b3/pyproject.toml
--rw-r--r--   0        0        0      399 2023-06-01 04:42:30.654182 citric-0.7.1b3/src/citric/__init__.py
--rw-r--r--   0        0        0     1509 2023-06-01 04:42:30.654182 citric-0.7.1b3/src/citric/_compat.py
--rw-r--r--   0        0        0    46924 2023-06-01 04:42:30.654182 citric-0.7.1b3/src/citric/client.py
--rw-r--r--   0        0        0     1739 2023-06-01 04:42:30.654182 citric-0.7.1b3/src/citric/enums.py
--rw-r--r--   0        0        0     1345 2023-06-01 04:42:30.654182 citric-0.7.1b3/src/citric/exceptions.py
--rw-r--r--   0        0        0     1055 2023-06-01 04:42:30.654182 citric-0.7.1b3/src/citric/method.py
--rw-r--r--   0        0        0     1171 2023-06-01 04:42:30.654182 citric-0.7.1b3/src/citric/objects.py
--rw-r--r--   0        0        0        0 2023-06-01 04:42:30.654182 citric-0.7.1b3/src/citric/py.typed
--rw-r--r--   0        0        0     6964 2023-06-01 04:42:30.654182 citric-0.7.1b3/src/citric/session.py
--rw-r--r--   0        0        0    14009 2023-06-01 04:42:30.654182 citric-0.7.1b3/src/citric/types.py
--rw-r--r--   0        0        0     6790 1970-01-01 00:00:00.000000 citric-0.7.1b3/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-06-21 05:16:35.637342 citric-0.7.2/LICENSE
+-rw-r--r--   0        0        0     4771 2023-06-21 05:16:35.637342 citric-0.7.2/README.md
+-rw-r--r--   0        0        0     4424 2023-06-21 05:16:35.641342 citric-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0      399 2023-06-21 05:16:35.641342 citric-0.7.2/src/citric/__init__.py
+-rw-r--r--   0        0        0     1509 2023-06-21 05:16:35.641342 citric-0.7.2/src/citric/_compat.py
+-rw-r--r--   0        0        0    46924 2023-06-21 05:16:35.641342 citric-0.7.2/src/citric/client.py
+-rw-r--r--   0        0        0     1790 2023-06-21 05:16:35.641342 citric-0.7.2/src/citric/enums.py
+-rw-r--r--   0        0        0     1345 2023-06-21 05:16:35.641342 citric-0.7.2/src/citric/exceptions.py
+-rw-r--r--   0        0        0     1055 2023-06-21 05:16:35.641342 citric-0.7.2/src/citric/method.py
+-rw-r--r--   0        0        0     1171 2023-06-21 05:16:35.641342 citric-0.7.2/src/citric/objects.py
+-rw-r--r--   0        0        0        0 2023-06-21 05:16:35.641342 citric-0.7.2/src/citric/py.typed
+-rw-r--r--   0        0        0     7264 2023-06-21 05:16:35.641342 citric-0.7.2/src/citric/session.py
+-rw-r--r--   0        0        0    13897 2023-06-21 05:16:35.641342 citric-0.7.2/src/citric/types.py
+-rw-r--r--   0        0        0     6784 1970-01-01 00:00:00.000000 citric-0.7.2/PKG-INFO
```

### Comparing `citric-0.7.1b3/LICENSE` & `citric-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `citric-0.7.1b3/README.md` & `citric-0.7.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   </a>
   <a href="https://github.com/edgarrmondragon/citric/blob/main/LICENSE">
     <img alt="License" src="https://img.shields.io/github/license/edgarrmondragon/citric"/>
   </a>
   <a href="https://citric.readthedocs.io/en/latest/?badge=latest">
     <img alt="Documentation Status" src="https://readthedocs.org/projects/citric/badge/?version=latest"/>
   </a>
-  <a href="https://github.com/charliermarsh/ruff">
+  <a href="https://github.com/astral-sh/ruff">
     <img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json" alt="Ruff" style="max-width:100%;">
   </a>
   <a href="https://codecov.io/gh/edgarrmondragon/citric">
     <img alt="codecov" src="https://codecov.io/gh/edgarrmondragon/citric/branch/main/graph/badge.svg"/>
   </a>
   <a href="https://app.fossa.com/projects/git%2Bgithub.com%2Fedgarrmondragon%2Fcitric?ref=badge_shield">
     <img alt="FOSSA Status" src="https://app.fossa.com/api/projects/git%2Bgithub.com%2Fedgarrmondragon%2Fcitric.svg?type=shield"/>
```

### Comparing `citric-0.7.1b3/pyproject.toml` & `citric-0.7.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 homepage = 'https://github.com/edgarrmondragon/citric'
 keywords = ["limesurvey", "json-rpc"]
 license = "MIT"
 maintainers = ["Edgar Ramírez-Mondragón <edgarrm358@gmail.com>"]
 name = "citric"
 readme = "README.md"
 repository = 'https://github.com/edgarrmondragon/citric'
-version = "0.7.1-b3"
+version = "0.7.2"
 
 [tool.poetry.urls]
 "Issue Tracker" = "https://github.com/edgarrmondragon/citric/issues"
 
 [tool.poetry.dependencies]
 importlib_metadata = {version = ">=1.6", python = "<3.8"}
 python = ">=3.7.0"
@@ -65,61 +65,19 @@
   "sphinx-autodoc-typehints",
   "sphinx-copybutton",
 ]
 
 [tool.black]
 line-length = 88
 
-[tool.pytest.ini_options]
-addopts = '-vvv'
-markers = [
-  "integration_test: Integration and end-to-end tests",
-  "version(ref): Mark a test that depends on a specific version of LimeSurvey",
-  "xfail_mysql: Mark a test as expected to fail on MySQL",
-]
-
-[tool.coverage.paths]
-source = ["src", "*/site-packages"]
-
-[tool.coverage.run]
-branch = true
-source = ["citric"]
-
-[tool.coverage.report]
-exclude_lines = [
-    "pragma: no cover",
-    '''if (t\.)?TYPE_CHECKING:''',
-]
-fail_under = 90
-omit = [
-  "src/citric/types.py",
-]
-show_missing = true
-
-[tool.mypy]
-enable_incomplete_feature = "Unpack"
-warn_unreachable = true
-warn_unused_configs = true
-warn_unused_ignores = true
-
-[[tool.mypy.overrides]]
-ignore_missing_imports = true
-module = [
-  "nox.*",
-  "nox_poetry.*",
-  "pytest.*",
-]
-
-[tool.codespell]
-skip = ".mypy_cache,.nox,.ruff_cache,build,docs/index.md,poetry.lock"
-
 [tool.ruff]
 ignore = [
   "ANN101", # missing-type-self
-  "DJ", # flake8-django
+  "DJ",     # flake8-django
+  "FIX002", # line-contains-todo
 ]
 line-length = 88
 select = ["ALL"]
 src = ["src", "tests", "docs"]
 target-version = "py37"
 
 [tool.ruff.per-file-ignores]
@@ -168,12 +126,55 @@
 
 [tool.ruff.pydocstyle]
 convention = "google"
 
 [tool.ruff.pylint]
 max-args = 10
 
+[tool.pytest.ini_options]
+addopts = '-vvv'
+markers = [
+  "integration_test: Integration and end-to-end tests",
+  "version(ref): Mark a test that depends on a specific version of LimeSurvey",
+  "xfail_mysql: Mark a test as expected to fail on MySQL",
+]
+
+[tool.coverage.paths]
+source = ["src", "*/site-packages"]
+
+[tool.coverage.run]
+branch = true
+source = ["citric"]
+
+[tool.coverage.report]
+exclude_lines = [
+    "pragma: no cover",
+    '''if (t\.)?TYPE_CHECKING:''',
+]
+fail_under = 90
+omit = [
+  "src/citric/types.py",
+]
+show_missing = true
+
+[tool.mypy]
+enable_incomplete_feature = "Unpack"
+warn_unreachable = true
+warn_unused_configs = true
+warn_unused_ignores = true
+
+[[tool.mypy.overrides]]
+ignore_missing_imports = true
+module = [
+  "nox.*",
+  "nox_poetry.*",
+  "pytest.*",
+]
+
+[tool.codespell]
+skip = ".mypy_cache,.nox,.ruff_cache,build,docs/index.md,poetry.lock"
+
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = [
   "poetry-core>=1",
 ]
```

### Comparing `citric-0.7.1b3/src/citric/_compat.py` & `citric-0.7.2/src/citric/_compat.py`

 * *Files identical despite different names*

### Comparing `citric-0.7.1b3/src/citric/client.py` & `citric-0.7.2/src/citric/client.py`

 * *Files identical despite different names*

### Comparing `citric-0.7.1b3/src/citric/enums.py` & `citric-0.7.2/src/citric/enums.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,87 +1,93 @@
 """Useful enums."""
 
 from __future__ import annotations
 
 import enum
 
 
-class ImportGroupType(str, enum.Enum):
+class StringEnum(str, enum.Enum):
+    """Enum with string values."""
+
+    __slots__ = ()
+
+
+class ImportGroupType(StringEnum):
     """Group file type."""
 
     LSG = "lsg"
     CSV = "csv"
 
 
-class ImportSurveyType(str, enum.Enum):
+class ImportSurveyType(StringEnum):
     """Survey file type."""
 
     LSS = "lss"
     CSV = "csv"
     TXT = "txt"
     LSA = "lsa"
 
 
-class NewSurveyType(str, enum.Enum):
+class NewSurveyType(StringEnum):
     """New survey type."""
 
     ALL_ON_ONE_PAGE = "A"
     GROUP_BY_GROUP = "G"
     SINGLE_QUESTIONS = "S"
 
 
-class StatisticsExportFormat(str, enum.Enum):
+class StatisticsExportFormat(StringEnum):
     """Statistics export type."""
 
     PDF = "pdf"
     XLS = "xls"
     HTML = "html"
 
 
-class ResponsesExportFormat(str, enum.Enum):
+class ResponsesExportFormat(StringEnum):
     """Responses export type."""
 
     PDF = "pdf"
     CSV = "csv"
     XLS = "xls"
     DOC = "doc"
     JSON = "json"
 
 
-class SurveyCompletionStatus(str, enum.Enum):
+class SurveyCompletionStatus(StringEnum):
     """Survey completion status values."""
 
     COMPLETE = "complete"
     INCOMPLETE = "incomplete"
     ALL = "all"
 
 
-class HeadingType(str, enum.Enum):
+class HeadingType(StringEnum):
     """Types of heading in responses export."""
 
     CODE = "code"
     FULL = "full"
     ABBREVIATED = "abbreviated"
 
 
-class ResponseType(str, enum.Enum):
+class ResponseType(StringEnum):
     """Types of responses in export."""
 
     LONG = "long"
     SHORT = "short"
 
 
-class TimelineAggregationPeriod(str, enum.Enum):
+class TimelineAggregationPeriod(StringEnum):
     """Timeline aggregation level."""
 
     HOUR = "hour"
     DAY = "day"
 
 
-class QuotaAction(str, enum.Enum):
+class QuotaAction(StringEnum):
     """Quota action."""
 
     TERMINATE = "terminate"
     CONFIRM_TERMINATE = "confirm_terminate"
 
     @property
     def integer_value(self) -> int:
```

### Comparing `citric-0.7.1b3/src/citric/exceptions.py` & `citric-0.7.2/src/citric/exceptions.py`

 * *Files identical despite different names*

### Comparing `citric-0.7.1b3/src/citric/method.py` & `citric-0.7.2/src/citric/method.py`

 * *Files identical despite different names*

### Comparing `citric-0.7.1b3/src/citric/objects.py` & `citric-0.7.2/src/citric/objects.py`

 * *Files identical despite different names*

### Comparing `citric-0.7.1b3/src/citric/session.py` & `citric-0.7.2/src/citric/session.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 """Low level wrapper for connecting to the LSRC2."""
 
 from __future__ import annotations
 
 import json
 import logging
 import random
+import sys
 import typing as t
 
 import requests
 
 from citric.exceptions import (
     InvalidJSONResponseError,
     LimeSurveyApiError,
     LimeSurveyStatusError,
     ResponseMismatchError,
     RPCInterfaceNotEnabledError,
 )
 from citric.method import Method
 
+if sys.version_info >= (3, 8):
+    from importlib import metadata
+else:
+    import importlib_metadata as metadata
+
 if t.TYPE_CHECKING:
     from types import TracebackType
 
     from citric.types import Result, RPCResponse
 
 __all__ = ["Session"]
 
@@ -83,33 +89,34 @@
     .. _requests.Session:
         https://requests.readthedocs.io/en/latest/api/#request-sessions
     .. _key: #citric.session.Session.key
     .. _closure: #citric.session.Session.close
     .. _JSONEncoder: https://docs.python.org/3/library/json.html#json.JSONEncoder
     """
 
-    _headers = {
-        "user-agent": "citric-client",
-    }
+    USER_AGENT = f"citric/{metadata.version('citric')}"
 
-    __attrs__ = ["url", "key"]
+    # TODO(edgarrmondragon): Remove this.
+    # https://github.com/edgarrmondragon/citric/issues/893
+    _headers: t.ClassVar[dict[str, t.Any]] = {}
 
     def __init__(
         self,
         url: str,
         username: str,
         password: str,
         *,
         auth_plugin: str = "Authdb",
         requests_session: requests.Session | None = None,
         json_encoder: type[json.JSONEncoder] | None = None,
     ) -> None:
         """Create a LimeSurvey RPC session."""
         self.url = url
         self._session = requests_session or requests.session()
+        self._session.headers["User-Agent"] = self.USER_AGENT
         self._session.headers.update(self._headers)
         self._encoder = json_encoder or json.JSONEncoder
 
         self.__key: str | None = self.get_session_key(
             username,
             password,
             auth_plugin,
```

### Comparing `citric-0.7.1b3/src/citric/types.py` & `citric-0.7.2/src/citric/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,25 +173,25 @@
         same_default: The question same default.
         relevance: The question relevance.
         question_theme_name: The question theme name.
         modulename: The question module name.
         same_script: The question same script.
     """
 
-    id: int  # noqa: A003
+    id: int
     qid: int
     parent_qid: int
     gid: int
     sid: int
 
     question: str
-    help: str  # noqa: A003
+    help: str
     language: str
 
-    type: str  # noqa: A003
+    type: str
     title: str
     preg: str
     other: YesNo
     mandatory: YesNo
     encrypted: YesNo
     question_order: int
     scale_id: int
@@ -236,15 +236,15 @@
     """
 
     qid: int
     parent_qid: int
     gid: int
     sid: int
 
-    type: str  # noqa: A003
+    type: str
     title: str
     preg: str
     other: YesNo
     mandatory: YesNo
     encrypted: YesNo
     question_order: int
     scale_id: int
@@ -271,15 +271,15 @@
         name: The quota name.
         qlimit: The quota limit.
         active: Whether the quota is active.
         action: The quota action.
         autoload_url: Whether the quota autoload URL is active.
     """
 
-    id: int  # noqa: A003
+    id: int
     name: str
     action: int
     limit: int
     active: int
     autoload_url: int
 
 
@@ -292,15 +292,15 @@
         name: The quota name.
         qlimit: The quota limit.
         action: The quota action.
         active: Whether the quota is active.
         autoload_url: Whether the quota autoload URL is active.
     """
 
-    id: int  # noqa: A003
+    id: int
     sid: int
     name: str
     qlimit: int
     action: int
     active: int
     autoload_url: int
 
@@ -310,15 +310,15 @@
 
     Keys:
         id: The ID of the request.
         result: The result of the RPC call.
         error: The error message of the RPC call.
     """
 
-    id: int  # noqa: A003
+    id: int
     result: Result
     error: str | None
 
 
 class SetQuotaPropertiesResult(TypedDict):
     """Set quota properties result.
 
@@ -408,15 +408,15 @@
     owner_id: int
     gsid: int
     active: YesNo
     expires: str | None
     startdate: str | None
     anonymized: YesNo
     faxto: str
-    format: enums.NewSurveyType  # noqa: A003
+    format: enums.NewSurveyType
     savetiming: YesNo
     template: str
     datesstamp: YesNo
     usecookie: YesNo
     allowregister: YesNo
     allowsave: YesNo
     autonumber_start: int
```

### Comparing `citric-0.7.1b3/PKG-INFO` & `citric-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citric
-Version: 0.7.1b3
+Version: 0.7.2
 Summary: A client to the LimeSurvey Remote Control API 2, written in modern Python.
 Home-page: https://github.com/edgarrmondragon/citric
 License: MIT
 Keywords: limesurvey,json-rpc
 Author: Edgar Ramírez-Mondragón
 Author-email: edgarrm358@gmail.com
 Maintainer: Edgar Ramírez-Mondragón
@@ -54,15 +54,15 @@
   </a>
   <a href="https://github.com/edgarrmondragon/citric/blob/main/LICENSE">
     <img alt="License" src="https://img.shields.io/github/license/edgarrmondragon/citric"/>
   </a>
   <a href="https://citric.readthedocs.io/en/latest/?badge=latest">
     <img alt="Documentation Status" src="https://readthedocs.org/projects/citric/badge/?version=latest"/>
   </a>
-  <a href="https://github.com/charliermarsh/ruff">
+  <a href="https://github.com/astral-sh/ruff">
     <img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json" alt="Ruff" style="max-width:100%;">
   </a>
   <a href="https://codecov.io/gh/edgarrmondragon/citric">
     <img alt="codecov" src="https://codecov.io/gh/edgarrmondragon/citric/branch/main/graph/badge.svg"/>
   </a>
   <a href="https://app.fossa.com/projects/git%2Bgithub.com%2Fedgarrmondragon%2Fcitric?ref=badge_shield">
     <img alt="FOSSA Status" src="https://app.fossa.com/api/projects/git%2Bgithub.com%2Fedgarrmondragon%2Fcitric.svg?type=shield"/>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: citric Version: 0.7.1b3 Summary: A client to the
+Metadata-Version: 2.1 Name: citric Version: 0.7.2 Summary: A client to the
 LimeSurvey Remote Control API 2, written in modern Python. Home-page: https://
 github.com/edgarrmondragon/citric License: MIT Keywords: limesurvey,json-rpc
 Author: Edgar RamÃ­rez-MondragÃ³n Author-email: edgarrm358@gmail.com
 Maintainer: Edgar RamÃ­rez-MondragÃ³n Maintainer-email: edgarrm358@gmail.com
 Requires-Python: >=3.7.0 Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: MIT License Classifier: Natural Language :: English Classifier:
```

