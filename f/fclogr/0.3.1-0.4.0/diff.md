# Comparing `tmp/fclogr-0.3.1.tar.gz` & `tmp/fclogr-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fclogr-0.3.1.tar", last modified: Sat Apr 15 21:44:43 2023, max compression
+gzip compressed data, was "fclogr-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fclogr-0.3.1.tar` & `fclogr-0.4.0.tar`

### file list

```diff
@@ -1,27 +1,34 @@
--rw-r--r--   0        0        0      273 2023-04-15 20:35:53.456294 fclogr-0.3.1/.copr/Makefile
-lrwxr-xr-x   0        0        0        0 2023-04-15 20:35:53.456294 fclogr-0.3.1/LICENSE -> LICENSES/GPL-2.0-or-later.txt
--rw-r--r--   0        0        0    17337 2023-04-15 20:35:53.456294 fclogr-0.3.1/LICENSES/GPL-2.0-or-later.txt
--rw-r--r--   0        0        0     1078 2023-04-15 16:21:50.774739 fclogr-0.3.1/LICENSES/MIT.txt
--rw-r--r--   0        0        0      498 2023-04-15 21:43:41.007762 fclogr-0.3.1/NEWS.md
--rw-r--r--   0        0        0       89 2023-04-15 20:35:53.457294 fclogr-0.3.1/NEWS.md.license
--rw-r--r--   0        0        0     8142 2023-04-15 21:40:29.166607 fclogr-0.3.1/README.md
--rwxr-xr-x   0        0        0      932 2023-04-15 16:49:14.180578 fclogr-0.3.1/contrib/fedoraify.py
--rw-r--r--   0        0        0     1341 2023-04-15 21:43:41.008762 fclogr-0.3.1/fclogr.spec
--rw-r--r--   0        0        0    10542 2023-04-15 21:21:19.356312 fclogr-0.3.1/noxfile.py
--rw-r--r--   0        0        0     1973 2023-04-15 21:44:43.703486 fclogr-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      104 2023-01-13 06:17:16.597082 fclogr-0.3.1/src/fclogr/__init__.py
--rw-r--r--   0        0        0      209 2023-01-13 23:30:50.869984 fclogr-0.3.1/src/fclogr/__main__.py
--rw-r--r--   0        0        0     2047 2023-04-14 04:40:12.125463 fclogr-0.3.1/src/fclogr/cli/__init__.py
--rw-r--r--   0        0        0     1331 2023-04-14 04:14:48.656998 fclogr-0.3.1/src/fclogr/cli/base.py
--rw-r--r--   0        0        0     6512 2023-04-15 20:35:53.457294 fclogr-0.3.1/src/fclogr/cli/bump.py
--rw-r--r--   0        0        0     9971 2023-04-14 04:14:48.657998 fclogr-0.3.1/src/fclogr/cli/dev_entries.py
--rw-r--r--   0        0        0     2256 2023-04-01 04:25:07.641592 fclogr-0.3.1/src/fclogr/cli/sync.py
--rw-r--r--   0        0        0        0 2023-01-07 08:21:55.207097 fclogr-0.3.1/src/fclogr/py.typed
--rw-r--r--   0        0        0        0 2023-03-03 18:54:38.037265 fclogr-0.3.1/tests/__init__.py
--rw-r--r--   0        0        0      292 2023-04-15 20:35:53.457294 fclogr-0.3.1/tests/conftest.py
--rw-r--r--   0        0        0     4369 2023-04-15 20:35:53.457294 fclogr-0.3.1/tests/test_bumper.py
--rw-r--r--   0        0        0      418 2023-04-01 04:25:07.638592 fclogr-0.3.1/tests/test_data/package.2.spec
--rw-r--r--   0        0        0      442 2023-03-03 22:00:05.714861 fclogr-0.3.1/tests/test_data/package.3.spec
--rw-r--r--   0        0        0      376 2023-03-03 20:18:25.858606 fclogr-0.3.1/tests/test_data/package.spec
--rw-r--r--   0        0        0      961 2023-04-15 20:35:53.457294 fclogr-0.3.1/tests/test_syncer.py
--rw-r--r--   0        0        0     9637 1970-01-01 00:00:00.000000 fclogr-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      653 2023-06-20 23:09:40.277850 fclogr-0.4.0/.builds/main.yml
+-rw-r--r--   0        0        0      635 2023-06-20 23:09:40.277850 fclogr-0.4.0/.builds/mockbuild-epel9.yml
+-rw-r--r--   0        0        0      631 2023-06-20 23:09:40.277850 fclogr-0.4.0/.builds/mockbuild-f37.yml
+-rw-r--r--   0        0        0      640 2023-06-20 23:09:40.277850 fclogr-0.4.0/.builds/mockbuild.yml
+-rw-r--r--   0        0        0      273 2023-04-26 05:13:46.788278 fclogr-0.4.0/.copr/Makefile
+-rw-r--r--   0        0        0      160 2023-06-20 23:09:40.277850 fclogr-0.4.0/.gitignore
+lrwxr-xr-x   0        0        0        0 2023-06-20 22:17:33.348915 fclogr-0.4.0/LICENSE -> LICENSES/GPL-2.0-or-later.txt
+-rw-r--r--   0        0        0    17337 2023-04-15 20:35:53.456294 fclogr-0.4.0/LICENSES/GPL-2.0-or-later.txt
+-rw-r--r--   0        0        0     1078 2023-04-15 16:21:50.774739 fclogr-0.4.0/LICENSES/MIT.txt
+-rw-r--r--   0        0        0      881 2023-06-20 23:36:19.355132 fclogr-0.4.0/NEWS.md
+-rw-r--r--   0        0        0       89 2023-04-15 20:35:53.457294 fclogr-0.4.0/NEWS.md.license
+-rw-r--r--   0        0        0     8142 2023-04-26 05:13:46.788278 fclogr-0.4.0/README.md
+-rwxr-xr-x   0        0        0      932 2023-04-15 16:49:14.180578 fclogr-0.4.0/contrib/fedoraify.py
+-rw-r--r--   0        0        0     1275 2023-06-20 23:36:18.886133 fclogr-0.4.0/fclogr.spec
+-rw-r--r--   0        0        0     4406 2023-06-20 23:19:22.167601 fclogr-0.4.0/noxfile.py
+-rw-r--r--   0        0        0     2252 2023-06-20 23:09:40.277850 fclogr-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      707 2023-06-20 23:09:40.277850 fclogr-0.4.0/ruff.toml
+-rw-r--r--   0        0        0      163 2023-06-20 23:36:13.039138 fclogr-0.4.0/src/fclogr/__init__.py
+-rw-r--r--   0        0        0      209 2023-01-13 23:30:50.869984 fclogr-0.4.0/src/fclogr/__main__.py
+-rw-r--r--   0        0        0     2047 2023-06-20 21:41:01.480167 fclogr-0.4.0/src/fclogr/cli/__init__.py
+-rw-r--r--   0        0        0     1323 2023-06-20 21:41:01.481167 fclogr-0.4.0/src/fclogr/cli/base.py
+-rw-r--r--   0        0        0     6857 2023-06-20 23:19:22.342601 fclogr-0.4.0/src/fclogr/cli/bump.py
+-rw-r--r--   0        0        0     9932 2023-06-20 22:44:54.029677 fclogr-0.4.0/src/fclogr/cli/dev_entries.py
+-rw-r--r--   0        0        0     2256 2023-04-01 04:25:07.641592 fclogr-0.4.0/src/fclogr/cli/sync.py
+-rw-r--r--   0        0        0        0 2023-01-07 08:21:55.207097 fclogr-0.4.0/src/fclogr/py.typed
+-rw-r--r--   0        0        0        0 2023-03-03 18:54:38.037265 fclogr-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0      292 2023-04-15 20:35:53.457294 fclogr-0.4.0/tests/conftest.py
+-rw-r--r--   0        0        0     6469 2023-06-20 23:19:22.343601 fclogr-0.4.0/tests/test_bumper.py
+-rw-r--r--   0        0        0      321 2023-04-27 04:27:59.767798 fclogr-0.4.0/tests/test_data/package-autospec.spec
+-rw-r--r--   0        0        0      418 2023-04-01 04:25:07.638592 fclogr-0.4.0/tests/test_data/package.2.spec
+-rw-r--r--   0        0        0      442 2023-03-03 22:00:05.714861 fclogr-0.4.0/tests/test_data/package.3.spec
+-rw-r--r--   0        0        0      376 2023-03-03 20:18:25.858606 fclogr-0.4.0/tests/test_data/package.spec
+-rw-r--r--   0        0        0      961 2023-04-15 20:35:53.457294 fclogr-0.4.0/tests/test_syncer.py
+-rw-r--r--   0        0        0     9920 1970-01-01 00:00:00.000000 fclogr-0.4.0/PKG-INFO
```

### Comparing `fclogr-0.3.1/LICENSES/GPL-2.0-or-later.txt` & `fclogr-0.4.0/LICENSES/GPL-2.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `fclogr-0.3.1/LICENSES/MIT.txt` & `fclogr-0.4.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `fclogr-0.3.1/README.md` & `fclogr-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `fclogr-0.3.1/contrib/fedoraify.py` & `fclogr-0.4.0/contrib/fedoraify.py`

 * *Files identical despite different names*

### Comparing `fclogr-0.3.1/fclogr.spec` & `fclogr-0.4.0/fclogr.spec`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,27 @@
 # This specfile is licensed under:
 #
 # Copyright (C) 2023 Maxwell G <gotmax@e.email>
 # SPDX-License-Identifier: MIT
 # License text: https://spdx.org/licenses/MIT.html
 
 Name:           fclogr
-Version:        0.3.0
+Version:        0.4.0
 Release:        1%{?dist}
 Summary:        A tool for managing RPM changelogs and updates
 
 License:        GPL-2.0-or-later
 URL:            https://sr.ht/~gotmax23/fclogr
 %global furl    https://git.sr.ht/~gotmax23/fclogr
 Source0:        %{furl}/refs/download/v%{version}/fclogr-%{version}.tar.gz
 
 BuildArch:      noarch
 BuildRequires:  gnupg2
 BuildRequires:  python3-devel
 
-BuildRequires:  %{py3_dist pytest}
-BuildRequires:  rpmdevtools
-
-# This is currently used for `fclogr bump`.
-# TODO: Remove once https://github.com/packit/specfile/pull/220
-# is merged.
-Recommends:     rpmdevtools
-
 
 %description
 fclogr is a tool for managing RPM changelogs and updates.
 
 
 %prep
 %autosetup -p1 -n fclogr-%{version}
@@ -56,12 +48,18 @@
 %license LICENSES/*.txt
 %doc README.md
 %doc NEWS.md
 %{_bindir}/fclogr*
 
 
 %changelog
+* Tue Jun 20 2023 Maxwell G <maxwell@gtmx.me> - 0.4.0-1
+- Release 0.4.0.
+
+* Sat Apr 15 2023 Maxwell G <maxwell@gtmx.me> - 0.3.1-1
+- Release 0.3.1.
+
 * Sat Apr 15 2023 Maxwell G <maxwell@gtmx.me> - 0.3.0-1
 - Release 0.3.0.
 
 * Sat Mar 18 2023 Maxwell G <maxwell@gtmx.me> - 0.2.0-1
 - Initial package
```

### Comparing `fclogr-0.3.1/src/fclogr/cli/__init__.py` & `fclogr-0.4.0/src/fclogr/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `fclogr-0.3.1/src/fclogr/cli/base.py` & `fclogr-0.4.0/src/fclogr/cli/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,11 +41,11 @@
         if getattr(self, "_cleanup", None) is None:
             self._cleanup = []
         return self._cleanup
 
     def _v_specpath(self, path: Path | None = None) -> Path:
         if not path:
             pwd = Path.cwd()
-            path = pwd.joinpath(pwd.name + ".spec")
+            path = Path(pwd.name + ".spec")
         if not path.is_file() or path.suffix != ".spec":
             raise InvalidArgumentError(f"{path} must exist an end with '.spec'")
         return path
```

### Comparing `fclogr-0.3.1/src/fclogr/cli/bump.py` & `fclogr-0.4.0/src/fclogr/cli/bump.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import specfile.changelog
 
 from fclogr.cli.base import Command, InvalidArgumentError
 
 if TYPE_CHECKING:
     from _typeshed import StrOrBytesPath
 
+PERCENT_MATCHER = re.compile("%([^%])?")
 # https://pagure.io/fedora-infra/rpmautospec/blob/edf18a1967f05253f937aa93ea90209459d18695/f/rpmautospec/misc.py#_11
 AUTORELEASE_RE = re.compile(
     r"%(?:autorelease(?:\s|$)|\{\??autorelease(?:\s+[^\}]*)?\})"
 )
 #
 PRE_REL_MATCHER = re.compile(r"^(0\.)(\d+)(.*)")
 REL_MATCHER = re.compile(r"^(\d+)(.*)")
@@ -56,21 +57,22 @@
     ) -> None:
         self.specpath: Path = self._v_specpath(specpath)
         self.version: str | None = version
         self.entry_only: bool = entry_only
         self.commit: bool = gpg_sign or commit
         self.gpg_sign: bool = gpg_sign
         try:
-            self.spec = specfile.Specfile(self.specpath)
+            self.spec = specfile.Specfile(self.specpath, force_parse=True)
         except specfile.exceptions.SpecfileException as err:
             LOG.debug("Failed to load specfile", exc_info=True)
             raise InvalidArgumentError(f"Failed to load specfile: {err}") from None
         comment = comment or [f"Update to {self.version}." if self.version else "bump"]
         self.comment: list[str] = [
-            c if c.startswith("- ") else "- " + c for c in comment
+            PERCENT_MATCHER.sub(r"%%\1", c if c.startswith("- ") else "- " + c)
+            for c in comment
         ]
         if entry_only and version:
             raise InvalidArgumentError("--entry-only and --new are mutually exclusive.")
 
     def _write_spec(self) -> int | str:
         try:
             self.specpath.write_text(str(self.spec), encoding="utf-8")
@@ -80,24 +82,34 @@
 
     def _evr(self) -> str:
         return self.spec.expand("%{?epoch:%{epoch}:}%{version}-%{release}")
 
     def run(self) -> int | str:
         uses_autorelease: bool = False
         old_evr = self._evr()
+
         if self.version:
-            self.spec.set_version_and_release(self.version)
-        elif self.entry_only:
+            self.spec.update_tag("Version", self.version)
+
+        if self.entry_only:
             pass
         elif any(AUTORELEASE_RE.search(line) for line in str(self.spec).splitlines()):
             uses_autorelease = True
             LOG.info("%s uses %%autorelease. Preserving Release.", self.specpath)
+        elif self.version:
+            self.spec.release = "1"
         else:
             self._handle_release()
+
+        if not uses_autorelease:
             LOG.info("%s: bumped %s -> %s", self.specpath, old_evr, self._evr())
+        elif self.version:
+            LOG.info(
+                "%s: bumped Version to %s", self.specpath, self.spec.expanded_version
+            )
 
         if not self.spec.has_autochangelog:
             if uses_autorelease:
                 LOG.warning(
                     "%s uses %%autorelease, but it does not use %%autochangelog."
                     " We're adding a changelog entry,"
                     " but its EVR part may be incorrect.",
```

### Comparing `fclogr-0.3.1/src/fclogr/cli/dev_entries.py` & `fclogr-0.4.0/src/fclogr/cli/dev_entries.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
     @property
     def date(self) -> dt.date:
         # Use UTC date
         timestamp = dt.datetime.fromtimestamp(
             self.commit.commit_time, tz=dt.timezone.utc
         )
-        return dt.date(timestamp.year, timestamp.month, timestamp.day)
+        return timestamp.date()
 
     @property
     def version(self) -> str:
         return "{ref}{sep}{num}.{date:%Y%m%d}.{hash}".format(
             ref=self.baseversion,
             sep="~" if self.pre else "^",
             num=self.index,
```

### Comparing `fclogr-0.3.1/src/fclogr/cli/sync.py` & `fclogr-0.4.0/src/fclogr/cli/sync.py`

 * *Files identical despite different names*

### Comparing `fclogr-0.3.1/tests/test_bumper.py` & `fclogr-0.4.0/tests/test_bumper.py`

 * *Files 26% similar despite different names*

```diff
@@ -47,68 +47,88 @@
     date_str: str = DATE_STR,
     packager: str = DEFAULT_PACKAGER,
 ):
     header = f"* {date_str} {packager} - {evr}"
     return specfile.changelog.ChangelogEntry(header, lines, following_lines)
 
 
-INITIAL_ENTRY = get_entry_obj(
-    "1-1",
-    ["- Initial package"],
-    [],
-    "Fri Mar 03 2023",
-    "Packager <example@example.com>",
+INITIAL_ENTRIES = (
+    get_entry_obj(
+        "1-1",
+        ["- Initial package"],
+        [],
+        "Fri Mar 03 2023",
+        "Packager <example@example.com>",
+    ),
+    get_entry_obj(
+        "1-2",
+        ["- rebuilt"],
+        [""],
+        "Fri Mar 03 2023",
+        "Packager <example@example.com>",
+    ),
 )
 
 
 @pytest.mark.parametrize(
     "args, changelog, version, raw_release, subprocess_calls",
     [
         pytest.param(
             [],
-            [INITIAL_ENTRY, get_entry_obj("1-2", ["- bump"], [""])],
+            [*INITIAL_ENTRIES, get_entry_obj("1-3", ["- bump"], [""])],
             "1",
-            "2%{?dist}",
+            "3%{?dist}",
             [],
             id="no-arguments",
         ),
         pytest.param(
             ["--new", "3"],
-            [INITIAL_ENTRY, get_entry_obj("3-1", ["- Update to 3."], [""])],
+            [*INITIAL_ENTRIES, get_entry_obj("3-1", ["- Update to 3."], [""])],
             "3",
             "1%{?dist}",
             [],
             id="new-version-no-arguments",
         ),
         pytest.param(
             ["--new", "3", "--commit"],
-            [INITIAL_ENTRY, get_entry_obj("3-1", ["- Update to 3."], [""])],
+            [*INITIAL_ENTRIES, get_entry_obj("3-1", ["- Update to 3."], [""])],
             "3",
             "1%{?dist}",
             [
                 lambda p: mock.call(
                     ["add", p],
                     check=True,
                     stdout=subprocess.DEVNULL,
                 ),
                 lambda _: mock.call(["commit", "-m", "Update to 3."], check=True),
             ],
             id="new-version-commit",
         ),
         pytest.param(
             ["--comment", "abc"],
-            [INITIAL_ENTRY, get_entry_obj("1-2", ["- abc"], [""])],
+            [*INITIAL_ENTRIES, get_entry_obj("1-3", ["- abc"], [""])],
             "1",
-            "2%{?dist}",
+            "3%{?dist}",
             [],
             id="comment",
         ),
         pytest.param(
+            ["--comment", "%changelog is escaped"],
+            [
+                *INITIAL_ENTRIES,
+                get_entry_obj("1-3", ["- %%changelog is escaped"], [""]),
+            ],
+            "1",
+            "3%{?dist}",
+            [],
+            id="comment-escape",
+        ),
+        pytest.param(
             ["--comment", "- abc", "-c", "xyz", "--new", "5", "-S"],
-            [INITIAL_ENTRY, get_entry_obj("5-1", ["- abc", "- xyz"], [""])],
+            [*INITIAL_ENTRIES, get_entry_obj("5-1", ["- abc", "- xyz"], [""])],
             "5",
             "1%{?dist}",
             [
                 lambda p: mock.call(
                     ["add", p],
                     check=True,
                     stdout=subprocess.DEVNULL,
@@ -122,28 +142,81 @@
     ],
 )
 def test_bumper_full(
     test_data: Path,
     tmp_path: Path,
     monkeypatch: pytest.MonkeyPatch,
     mocker: pytest_mock.MockerFixture,
+    #
     args: Sequence[str],
     changelog: list[specfile.changelog.ChangelogEntry],
     version: str,
     raw_release: str,
-    subprocess_calls: Sequence[mock.call],
+    subprocess_calls: Sequence[mock._Call],
 ):
     monkeypatch.setenv("RPM_PACKAGER", DEFAULT_PACKAGER)
     subprocess_mock: mock.MagicMock = mocker.patch.object(Bumper, "_git")
-    name = "package.spec"
+    name = "package.2.spec"
     path = tmp_path / name
     copy2(test_data / name, path)
     args = ["bump", *args, str(path)]
     assert main(args) == 0
     specfile.macros.Macros.reinit()
 
     with specfile.Specfile(path) as spec:
         assert spec.raw_release == raw_release
         assert spec.version == version
         with spec.changelog() as spec_changelog:
             assert list(spec_changelog) == changelog
     assert subprocess_mock.call_args_list == [call(path) for call in subprocess_calls]
+
+
+@pytest.mark.parametrize(
+    "args,subprocess_calls,version",
+    [
+        pytest.param([], [], None, id="simple-noop"),
+        pytest.param(["--new", "10"], [], "10", id="new"),
+        pytest.param(
+            ["--new", "10", "--commit"],
+            [
+                lambda p: mock.call(
+                    ["add", p],
+                    check=True,
+                    stdout=subprocess.DEVNULL,
+                ),
+                lambda _: mock.call(
+                    ["commit", "-m", "Update to 10.", "--allow-empty"], check=True
+                ),
+            ],
+            "10",
+            id="new-commit",
+        ),
+    ],
+)
+def test_bumper_autospec(
+    test_data: Path,
+    tmp_path: Path,
+    monkeypatch: pytest.MonkeyPatch,
+    mocker: pytest_mock.MockerFixture,
+    #
+    args: Sequence[str],
+    version: str | None,
+    subprocess_calls,
+) -> None:
+    subprocess_mock: mock.MagicMock = mocker.patch.object(Bumper, "_git")
+    name = "package-autospec.spec"
+    src = test_data / name
+    dest = tmp_path / name
+    copy2(src, dest)
+
+    args = ["bump", *args, str(dest)]
+    assert main(args) == 0
+    if version is None:
+        assert src.read_text() == dest.read_text()
+    else:
+        specfile.macros.Macros.reinit()
+        with specfile.Specfile(dest) as spec:
+            assert spec.expanded_version == version
+            spec.update_tag("Version", "1")
+            assert spec.expanded_version == "1"
+            assert src.read_text() == str(spec)
+    assert subprocess_mock.call_args_list == [call(dest) for call in subprocess_calls]
```

### Comparing `fclogr-0.3.1/tests/test_syncer.py` & `fclogr-0.4.0/tests/test_syncer.py`

 * *Files identical despite different names*

### Comparing `fclogr-0.3.1/PKG-INFO` & `fclogr-0.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
 Name: fclogr
-Version: 0.3.1
+Version: 0.4.0
 Summary: fclogr is a tool for managing RPM changelogs and updates
-Keywords: 
-Author-email: Maxwell G <gotmax@e.email>
+Author-email: Maxwell G <maxwell@gtmx.me>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
@@ -18,27 +17,32 @@
 Requires-Dist: pygit2
 Requires-Dist: specfile
 Requires-Dist: ruff ; extra == "codeqa"
 Requires-Dist: reuse ; extra == "codeqa"
 Requires-Dist: fclogr[codeqa] ; extra == "dev"
 Requires-Dist: fclogr[formatters] ; extra == "dev"
 Requires-Dist: fclogr[test] ; extra == "dev"
-Requires-Dist: nox>=2022.11.21 ; extra == "dev"
+Requires-Dist: fclogr[typing] ; extra == "dev"
+Requires-Dist: nox ; extra == "dev"
 Requires-Dist: black ; extra == "formatters"
 Requires-Dist: isort ; extra == "formatters"
-Requires-Dist: fclogr[formatters] ; extra == "lint"
-Requires-Dist: fclogr[typing] ; extra == "lint"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-mock ; extra == "test"
 Requires-Dist: mypy ; extra == "typing"
-Project-URL: Homepage, https://git.sr.ht/~gotmax23/fclogr
+Requires-Dist: pytest ; extra == "typing"
+Requires-Dist: pytest-mock ; extra == "typing"
+Requires-Dist: typing_extensions ; extra == "typing"
+Requires-Dist: nox ; extra == "typing"
+Project-URL: Changelog, https://git.sr.ht/~gotmax23/fclogr/tree/main/item/NEWS.md
+Project-URL: Homepage, https://sr.ht/~gotmax23/fclogr
+Project-URL: Mailing List, https://lists.sr.ht/~gotmax23/fclogr
+Project-URL: Source, https://git.sr.ht/~gotmax23/fclogr
 Provides-Extra: codeqa
 Provides-Extra: dev
 Provides-Extra: formatters
-Provides-Extra: lint
 Provides-Extra: test
 Provides-Extra: typing
 
 <!--
 SPDX-FileCopyrightText: 2023 Maxwell G <gotmax@e.email>
 
 SPDX-License-Identifier: GPL-2.0-or-later
```

