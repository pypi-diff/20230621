# Comparing `tmp/fedrq-0.7.1.tar.gz` & `tmp/fedrq-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedrq-0.7.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fedrq-0.8.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fedrq-0.7.1.tar` & `fedrq-0.8.0.tar`

### file list

```diff
@@ -1,117 +1,116 @@
--rw-r--r--   0        0        0      688 2023-05-28 23:13:09.924385 fedrq-0.7.1/.builds/epel9.yml
--rw-r--r--   0        0        0     2406 2023-05-28 08:06:22.506837 fedrq-0.7.1/.builds/main.yml
--rw-r--r--   0        0        0     1170 2023-05-28 23:13:09.924385 fedrq-0.7.1/.builds/mockbuild-36.yml
--rw-r--r--   0        0        0      751 2023-03-18 19:37:34.175930 fedrq-0.7.1/.builds/mockbuild.yml
--rw-r--r--   0        0        0      227 2023-02-19 18:37:34.746046 fedrq-0.7.1/.copr/Makefile
--rwxr-xr-x   0        0        0      512 2023-02-19 18:37:34.746046 fedrq-0.7.1/.copr/mk.sh
-lrwxr-xr-x   0        0        0        0 2023-02-19 18:37:34.747046 fedrq-0.7.1/.data/share/licenses/fedrq/GPL-2.0-or-later.txt -> ../../../../LICENSES/GPL-2.0-or-later.txt
-lrwxr-xr-x   0        0        0        0 2023-02-25 00:53:10.256118 fedrq-0.7.1/.data/share/licenses/fedrq/MIT.txt -> ../../../../LICENSES/MIT.txt
-lrwxr-xr-x   0        0        0        0 2023-02-25 00:53:10.256118 fedrq-0.7.1/.data/share/licenses/fedrq/PSF-2.0.txt -> ../../../../LICENSES/PSF-2.0.txt
-lrwxr-xr-x   0        0        0        0 2023-02-19 18:37:34.747046 fedrq-0.7.1/.data/share/licenses/fedrq/Unlicense.txt -> ../../../../LICENSES/Unlicense.txt
--rw-r--r--   0        0        0      268 2023-05-30 00:24:53.974774 fedrq-0.7.1/.gitignore
--rw-r--r--   0        0        0     2482 2023-03-19 02:41:47.073223 fedrq-0.7.1/CONTRIBUTING.md
--rw-r--r--   0        0        0    17337 2022-12-13 02:49:11.735043 fedrq-0.7.1/LICENSES/GPL-2.0-or-later.txt
--rw-r--r--   0        0        0     1078 2022-12-13 02:49:11.735043 fedrq-0.7.1/LICENSES/MIT.txt
--rw-r--r--   0        0        0     2427 2023-02-19 18:37:34.747046 fedrq-0.7.1/LICENSES/PSF-2.0.txt
--rw-r--r--   0        0        0     1211 2023-02-19 18:37:34.747046 fedrq-0.7.1/LICENSES/Unlicense.txt
--rw-r--r--   0        0        0    12505 2023-05-31 19:47:52.649519 fedrq-0.7.1/NEWS.md
--rw-r--r--   0        0        0       89 2023-03-18 21:16:55.983019 fedrq-0.7.1/NEWS.md.license
--rw-r--r--   0        0        0    12144 2023-03-27 04:19:29.833647 fedrq-0.7.1/README.md
--rwxr-xr-x   0        0        0      687 2023-04-09 15:43:04.496271 fedrq-0.7.1/contrib/add_frag.py
--rwxr-xr-x   0        0        0      906 2023-03-19 23:05:00.923501 fedrq-0.7.1/contrib/api_examples/a_noarch_bash.py
--rwxr-xr-x   0        0        0     2502 2023-03-19 23:05:00.924501 fedrq-0.7.1/contrib/api_examples/ftbfs_retirements.py
--rw-r--r--   0        0        0      630 2023-03-19 23:07:21.352951 fedrq-0.7.1/contrib/deploy-docsite/main.yaml
--rw-r--r--   0        0        0      183 2023-03-19 23:07:21.352951 fedrq-0.7.1/contrib/deploy-docsite/roles/configure/handlers/main.yaml
--rw-r--r--   0        0        0      885 2023-03-19 23:07:21.352951 fedrq-0.7.1/contrib/deploy-docsite/roles/configure/tasks/main.yml
--rw-r--r--   0        0        0      163 2023-03-19 23:07:21.352951 fedrq-0.7.1/contrib/deploy-docsite/roles/configure/templates/fedrq.caddyfile
--rw-r--r--   0        0        0      415 2023-03-19 23:07:21.352951 fedrq-0.7.1/contrib/deploy-docsite/roles/deploy/tasks/main.yaml
--rw-r--r--   0        0        0      156 2023-03-19 23:07:21.352951 fedrq-0.7.1/contrib/deploy-docsite/vars.yaml
--rwxr-xr-x   0        0        0      914 2023-04-14 16:37:52.615305 fedrq-0.7.1/contrib/fedoraify.py
--rw-r--r--   0        0        0     5728 2023-04-11 14:33:20.624926 fedrq-0.7.1/doc/API/Summary.md
--rw-r--r--   0        0        0      147 2023-03-19 23:07:21.353951 fedrq-0.7.1/doc/API/backends/base.md
--rw-r--r--   0        0        0      343 2023-04-11 19:16:07.821729 fedrq-0.7.1/doc/API/backends/dnf.md
--rw-r--r--   0        0        0      532 2023-04-20 18:33:19.648796 fedrq-0.7.1/doc/API/backends/libdnf5.md
--rw-r--r--   0        0        0      133 2023-03-19 23:07:21.353951 fedrq-0.7.1/doc/API/config.md
--rw-r--r--   0        0        0      145 2023-03-19 23:07:21.353951 fedrq-0.7.1/doc/API/release_repo.md
-lrwxr-xr-x   0        0        0        0 2023-03-19 23:07:21.353951 fedrq-0.7.1/doc/News.md -> ../NEWS.md
--rw-r--r--   0        0        0     3322 2023-05-29 06:28:47.729780 fedrq-0.7.1/doc/dnf-repoquery-diff.md
--rw-r--r--   0        0        0    16162 2023-05-29 23:47:52.009062 fedrq-0.7.1/doc/fedrq.1.scd
--rw-r--r--   0        0        0       98 2023-02-19 18:37:34.749046 fedrq-0.7.1/doc/fedrq.1.scd.license
--rw-r--r--   0        0        0     4958 2023-04-11 12:51:07.649356 fedrq-0.7.1/doc/fedrq.5.scd
--rw-r--r--   0        0        0       98 2023-02-19 18:37:34.749046 fedrq-0.7.1/doc/fedrq.5.scd.license
-lrwxr-xr-x   0        0        0        0 2023-03-19 23:07:21.353951 fedrq-0.7.1/doc/index.md -> ../README.md
--rw-r--r--   0        0        0      131 2023-03-19 23:07:21.353951 fedrq-0.7.1/fedrq.rpmlintrc
--rw-r--r--   0        0        0     3493 2023-05-31 19:47:52.604519 fedrq-0.7.1/fedrq.spec
--rw-r--r--   0        0        0     2169 2023-04-11 19:22:07.524752 fedrq-0.7.1/mkdocs.yml
--rw-r--r--   0        0        0    12535 2023-05-30 00:43:08.753184 fedrq-0.7.1/noxfile.py
--rw-r--r--   0        0        0     2713 2023-05-31 19:47:49.568530 fedrq-0.7.1/pyproject.toml
--rw-r--r--   0        0        0      532 2023-03-18 19:37:34.178930 fedrq-0.7.1/ruff.toml
--rw-r--r--   0        0        0      281 2023-02-21 18:02:47.599086 fedrq-0.7.1/src/fedrq/__init__.py
--rw-r--r--   0        0        0      219 2023-02-19 18:37:34.750046 fedrq-0.7.1/src/fedrq/__main__.py
--rw-r--r--   0        0        0     1713 2023-02-21 18:02:47.600086 fedrq-0.7.1/src/fedrq/_compat.py
--rw-r--r--   0        0        0      173 2023-03-18 19:37:34.178930 fedrq-0.7.1/src/fedrq/_config.py
--rw-r--r--   0        0        0     1248 2023-03-18 19:37:34.179930 fedrq-0.7.1/src/fedrq/_utils.py
--rw-r--r--   0        0        0     2529 2023-02-21 18:02:47.601086 fedrq-0.7.1/src/fedrq/backends/__init__.py
--rw-r--r--   0        0        0    14439 2023-05-29 15:11:03.621468 fedrq-0.7.1/src/fedrq/backends/base.py
--rw-r--r--   0        0        0      630 2023-02-21 18:02:47.603086 fedrq-0.7.1/src/fedrq/backends/dnf/__init__.py
--rw-r--r--   0        0        0     6949 2023-05-29 06:34:45.893651 fedrq-0.7.1/src/fedrq/backends/dnf/backend.py
--rw-r--r--   0        0        0      741 2023-02-21 18:02:47.604086 fedrq-0.7.1/src/fedrq/backends/libdnf5/__init__.py
--rw-r--r--   0        0        0    28232 2023-05-31 17:51:01.797529 fedrq-0.7.1/src/fedrq/backends/libdnf5/backend.py
--rw-r--r--   0        0        0     1955 2023-05-29 23:47:51.875063 fedrq-0.7.1/src/fedrq/cli/__init__.py
--rw-r--r--   0        0        0    15680 2023-05-29 23:47:51.877063 fedrq-0.7.1/src/fedrq/cli/base.py
--rw-r--r--   0        0        0        0 2023-02-19 18:37:34.751046 fedrq-0.7.1/src/fedrq/cli/commands/__init__.py
--rw-r--r--   0        0        0     2854 2023-03-18 19:37:34.182930 fedrq-0.7.1/src/fedrq/cli/commands/pkgs.py
--rw-r--r--   0        0        0     1489 2023-05-29 23:47:51.877063 fedrq-0.7.1/src/fedrq/cli/commands/repolist.py
--rw-r--r--   0        0        0     2425 2023-03-17 02:28:51.186103 fedrq-0.7.1/src/fedrq/cli/commands/subpkgs.py
--rw-r--r--   0        0        0    10843 2023-03-18 19:37:34.182930 fedrq-0.7.1/src/fedrq/cli/commands/whatrequires.py
--rw-r--r--   0        0        0    13071 2023-04-06 12:36:51.698430 fedrq-0.7.1/src/fedrq/cli/formatters.py
--rw-r--r--   0        0        0    16722 2023-05-30 00:06:50.295329 fedrq-0.7.1/src/fedrq/config.py
--rw-r--r--   0        0        0        0 2023-02-19 18:37:34.751046 fedrq-0.7.1/src/fedrq/data/__init__.py
--rw-r--r--   0        0        0     7030 2023-05-29 23:47:52.009062 fedrq-0.7.1/src/fedrq/data/releases.toml
--rw-r--r--   0        0        0        0 2023-02-19 18:37:34.752046 fedrq-0.7.1/src/fedrq/data/repos/__init__.py
--rw-r--r--   0        0        0     2053 2023-05-29 03:25:46.306279 fedrq-0.7.1/src/fedrq/data/repos/almalinux.repo
--rw-r--r--   0        0        0      639 2023-03-27 04:19:29.835647 fedrq-0.7.1/src/fedrq/data/repos/amazonlinux.repo
--rw-r--r--   0        0        0     1386 2023-05-29 03:25:46.306279 fedrq-0.7.1/src/fedrq/data/repos/centos-stream-compose.repo
--rw-r--r--   0        0        0     1850 2023-02-19 18:37:34.752046 fedrq-0.7.1/src/fedrq/data/repos/centos-stream.repo
--rw-r--r--   0        0        0     1494 2023-05-29 03:25:46.306279 fedrq-0.7.1/src/fedrq/data/repos/centos-stream8-compose.repo
--rw-r--r--   0        0        0     1599 2023-03-18 19:37:34.184930 fedrq-0.7.1/src/fedrq/data/repos/centos-stream8.repo
--rw-r--r--   0        0        0     1809 2023-05-29 03:58:29.496700 fedrq-0.7.1/src/fedrq/data/repos/eln.repo
--rw-r--r--   0        0        0     2158 2023-05-29 03:25:46.306279 fedrq-0.7.1/src/fedrq/data/repos/epel.repo
--rw-r--r--   0        0        0    14146 2023-05-29 03:25:46.419279 fedrq-0.7.1/src/fedrq/data/repos/fedora-eln.repo
--rw-r--r--   0        0        0     2402 2023-02-19 18:37:34.752046 fedrq-0.7.1/src/fedrq/data/repos/fedora-rawhide.repo
--rw-r--r--   0        0        0     1480 2023-02-19 18:37:34.752046 fedrq-0.7.1/src/fedrq/data/repos/fedora-updates-testing.repo
--rw-r--r--   0        0        0     1422 2023-02-19 18:37:34.752046 fedrq-0.7.1/src/fedrq/data/repos/fedora-updates.repo
--rw-r--r--   0        0        0     1375 2023-02-19 18:37:34.752046 fedrq-0.7.1/src/fedrq/data/repos/fedora.repo
--rw-r--r--   0        0        0      425 2023-05-29 03:25:46.306279 fedrq-0.7.1/src/fedrq/data/repos/rawhide-buildroot.repo
--rw-r--r--   0        0        0        0 2023-02-19 18:37:34.752046 fedrq-0.7.1/src/fedrq/py.typed
--rw-r--r--   0        0        0     8912 2023-05-28 01:30:25.101262 fedrq-0.7.1/src/fedrq/release_repo.py
--rw-r--r--   0        0        0      984 2023-02-21 18:02:47.612086 fedrq-0.7.1/src/fedrq/repoquery.py
--rwxr-xr-x   0        0        0      488 2023-02-19 18:37:34.753046 fedrq-0.7.1/srpm.sh
--rw-r--r--   0        0        0      154 2023-02-19 18:37:34.753046 fedrq-0.7.1/tests/.gitignore
--rw-r--r--   0        0        0        0 2023-05-29 04:18:46.483879 fedrq-0.7.1/tests/__init__.py
--rw-r--r--   0        0        0     2912 2023-02-21 18:02:47.613086 fedrq-0.7.1/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-05-29 04:18:46.483879 fedrq-0.7.1/tests/integration/__init__.py
--rw-r--r--   0        0        0     1739 2023-02-21 18:02:47.614086 fedrq-0.7.1/tests/integration/test_backends.py
--rw-r--r--   0        0        0      735 2023-05-28 08:06:22.609836 fedrq-0.7.1/tests/integration/test_pkgs.py
--rw-r--r--   0        0        0     1219 2023-03-18 19:37:34.185930 fedrq-0.7.1/tests/integration/test_subpkgs.py
--rw-r--r--   0        0        0     1725 2023-02-19 18:37:34.753046 fedrq-0.7.1/tests/integration/test_whatrequires.py
--rw-r--r--   0        0        0     1334 2023-02-19 18:37:34.753046 fedrq-0.7.1/tests/integration/test_whatrequires_src.py
--rw-r--r--   0        0        0        0 2023-05-29 04:18:46.484879 fedrq-0.7.1/tests/test_data/__init__.py
--rw-r--r--   0        0        0      332 2023-02-19 18:37:34.753046 fedrq-0.7.1/tests/test_data/_template.spec
--rwxr-xr-x   0        0        0     1449 2023-02-19 18:37:34.754046 fedrq-0.7.1/tests/test_data/build.sh
--rw-r--r--   0        0        0     1130 2023-02-19 18:37:34.754046 fedrq-0.7.1/tests/test_data/repos/repo1/specs/e1/packageb.spec
--rw-r--r--   0        0        0     1060 2023-02-19 18:37:34.754046 fedrq-0.7.1/tests/test_data/repos/repo1/specs/packagea.spec
--rw-r--r--   0        0        0     1156 2023-02-19 18:37:34.754046 fedrq-0.7.1/tests/test_data/repos/repo1/specs/packageb.spec
--rw-r--r--   0        0        0        0 2023-05-29 04:18:46.484879 fedrq-0.7.1/tests/unit/__init__.py
--rw-r--r--   0        0        0     2092 2023-05-29 15:11:03.621468 fedrq-0.7.1/tests/unit/test_checkconfig.py
--rw-r--r--   0        0        0     7127 2023-05-28 01:58:42.063000 fedrq-0.7.1/tests/unit/test_command.py
--rw-r--r--   0        0        0     7075 2023-02-21 18:02:47.617086 fedrq-0.7.1/tests/unit/test_formatters.py
--rw-r--r--   0        0        0     2161 2023-05-29 23:47:52.009062 fedrq-0.7.1/tests/unit/test_pkgs.py
--rw-r--r--   0        0        0     1645 2023-03-18 19:37:34.185930 fedrq-0.7.1/tests/unit/test_release.py
--rw-r--r--   0        0        0      413 2023-02-21 18:02:47.618086 fedrq-0.7.1/tests/unit/test_repo.py
--rw-r--r--   0        0        0      604 2023-05-29 23:47:51.877063 fedrq-0.7.1/tests/unit/test_repolist.py
--rw-r--r--   0        0        0     1289 2023-03-20 17:10:06.077134 fedrq-0.7.1/tests/unit/test_repoquery.py
--rw-r--r--   0        0        0     2676 2023-02-19 18:37:34.755046 fedrq-0.7.1/tests/unit/test_subbpkgs.py
--rw-r--r--   0        0        0     4052 2023-03-17 01:22:48.917895 fedrq-0.7.1/tests/unit/test_whatrequires.py
--rw-r--r--   0        0        0      653 2023-02-19 18:37:34.755046 fedrq-0.7.1/tests/unit/test_whatrequires_src.py
--rw-r--r--   0        0        0    14085 1970-01-01 00:00:00.000000 fedrq-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0      749 2023-06-16 02:38:20.599415 fedrq-0.8.0/.builds/epel9.yml
+-rw-r--r--   0        0        0     2348 2023-06-19 17:25:09.703310 fedrq-0.8.0/.builds/main.yml
+-rw-r--r--   0        0        0     1187 2023-06-19 21:38:24.304734 fedrq-0.8.0/.builds/mockbuild-37.yml
+-rw-r--r--   0        0        0      791 2023-06-21 01:13:53.672190 fedrq-0.8.0/.builds/mockbuild.yml
+-rw-r--r--   0        0        0      264 2023-06-16 02:40:08.756301 fedrq-0.8.0/.copr/Makefile
+lrwxr-xr-x   0        0        0        0 2023-02-19 18:37:34.747046 fedrq-0.8.0/.data/share/licenses/fedrq/GPL-2.0-or-later.txt -> ../../../../LICENSES/GPL-2.0-or-later.txt
+lrwxr-xr-x   0        0        0        0 2023-02-25 00:53:10.256118 fedrq-0.8.0/.data/share/licenses/fedrq/MIT.txt -> ../../../../LICENSES/MIT.txt
+lrwxr-xr-x   0        0        0        0 2023-02-25 00:53:10.256118 fedrq-0.8.0/.data/share/licenses/fedrq/PSF-2.0.txt -> ../../../../LICENSES/PSF-2.0.txt
+lrwxr-xr-x   0        0        0        0 2023-02-19 18:37:34.747046 fedrq-0.8.0/.data/share/licenses/fedrq/Unlicense.txt -> ../../../../LICENSES/Unlicense.txt
+-rw-r--r--   0        0        0      268 2023-06-06 22:57:17.280340 fedrq-0.8.0/.gitignore
+-rw-r--r--   0        0        0     2553 2023-06-16 02:38:20.601415 fedrq-0.8.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    17337 2022-12-13 02:49:11.735043 fedrq-0.8.0/LICENSES/GPL-2.0-or-later.txt
+-rw-r--r--   0        0        0     1078 2022-12-13 02:49:11.735043 fedrq-0.8.0/LICENSES/MIT.txt
+-rw-r--r--   0        0        0     2427 2023-02-19 18:37:34.747046 fedrq-0.8.0/LICENSES/PSF-2.0.txt
+-rw-r--r--   0        0        0     1211 2023-02-19 18:37:34.747046 fedrq-0.8.0/LICENSES/Unlicense.txt
+-rw-r--r--   0        0        0    13420 2023-06-21 14:13:12.284398 fedrq-0.8.0/NEWS.md
+-rw-r--r--   0        0        0       89 2023-03-18 21:16:55.983019 fedrq-0.8.0/NEWS.md.license
+-rw-r--r--   0        0        0    12144 2023-03-27 04:19:29.833647 fedrq-0.8.0/README.md
+-rwxr-xr-x   0        0        0      687 2023-06-06 22:57:17.280340 fedrq-0.8.0/contrib/add_frag.py
+-rwxr-xr-x   0        0        0      906 2023-03-19 23:05:00.923501 fedrq-0.8.0/contrib/api_examples/a_noarch_bash.py
+-rwxr-xr-x   0        0        0     2502 2023-03-19 23:05:00.924501 fedrq-0.8.0/contrib/api_examples/ftbfs_retirements.py
+-rw-r--r--   0        0        0      630 2023-03-19 23:07:21.352951 fedrq-0.8.0/contrib/deploy-docsite/main.yaml
+-rw-r--r--   0        0        0      183 2023-03-19 23:07:21.352951 fedrq-0.8.0/contrib/deploy-docsite/roles/configure/handlers/main.yaml
+-rw-r--r--   0        0        0      885 2023-03-19 23:07:21.352951 fedrq-0.8.0/contrib/deploy-docsite/roles/configure/tasks/main.yml
+-rw-r--r--   0        0        0      163 2023-03-19 23:07:21.352951 fedrq-0.8.0/contrib/deploy-docsite/roles/configure/templates/fedrq.caddyfile
+-rw-r--r--   0        0        0      415 2023-03-19 23:07:21.352951 fedrq-0.8.0/contrib/deploy-docsite/roles/deploy/tasks/main.yaml
+-rw-r--r--   0        0        0      156 2023-03-19 23:07:21.352951 fedrq-0.8.0/contrib/deploy-docsite/vars.yaml
+-rwxr-xr-x   0        0        0      914 2023-06-06 22:57:17.280340 fedrq-0.8.0/contrib/fedoraify.py
+-rw-r--r--   0        0        0     5728 2023-06-06 22:57:17.280340 fedrq-0.8.0/doc/API/Summary.md
+-rw-r--r--   0        0        0      147 2023-03-19 23:07:21.353951 fedrq-0.8.0/doc/API/backends/base.md
+-rw-r--r--   0        0        0      343 2023-06-06 22:57:17.280340 fedrq-0.8.0/doc/API/backends/dnf.md
+-rw-r--r--   0        0        0      532 2023-06-06 22:57:17.280340 fedrq-0.8.0/doc/API/backends/libdnf5.md
+-rw-r--r--   0        0        0      133 2023-03-19 23:07:21.353951 fedrq-0.8.0/doc/API/config.md
+-rw-r--r--   0        0        0      145 2023-03-19 23:07:21.353951 fedrq-0.8.0/doc/API/release_repo.md
+lrwxr-xr-x   0        0        0        0 2023-03-19 23:07:21.353951 fedrq-0.8.0/doc/News.md -> ../NEWS.md
+-rw-r--r--   0        0        0     3322 2023-06-06 22:57:17.280340 fedrq-0.8.0/doc/dnf-repoquery-diff.md
+-rw-r--r--   0        0        0    16162 2023-06-06 22:57:17.281340 fedrq-0.8.0/doc/fedrq.1.scd
+-rw-r--r--   0        0        0       98 2023-02-19 18:37:34.749046 fedrq-0.8.0/doc/fedrq.1.scd.license
+-rw-r--r--   0        0        0     4958 2023-06-06 22:57:17.281340 fedrq-0.8.0/doc/fedrq.5.scd
+-rw-r--r--   0        0        0       98 2023-02-19 18:37:34.749046 fedrq-0.8.0/doc/fedrq.5.scd.license
+lrwxr-xr-x   0        0        0        0 2023-03-19 23:07:21.353951 fedrq-0.8.0/doc/index.md -> ../README.md
+-rw-r--r--   0        0        0      193 2023-06-16 02:38:20.601415 fedrq-0.8.0/fedrq.rpmlintrc
+-rw-r--r--   0        0        0     3567 2023-06-21 14:13:11.838399 fedrq-0.8.0/fedrq.spec
+-rw-r--r--   0        0        0     2169 2023-06-06 22:57:17.281340 fedrq-0.8.0/mkdocs.yml
+-rw-r--r--   0        0        0     6722 2023-06-21 14:11:42.850542 fedrq-0.8.0/noxfile.py
+-rw-r--r--   0        0        0     3455 2023-06-21 01:22:32.983394 fedrq-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      532 2023-03-18 19:37:34.178930 fedrq-0.8.0/ruff.toml
+-rw-r--r--   0        0        0      371 2023-06-21 14:13:05.594408 fedrq-0.8.0/src/fedrq/__init__.py
+-rw-r--r--   0        0        0      219 2023-06-05 03:08:57.412761 fedrq-0.8.0/src/fedrq/__main__.py
+-rw-r--r--   0        0        0     1713 2023-06-05 03:08:57.412761 fedrq-0.8.0/src/fedrq/_compat.py
+-rw-r--r--   0        0        0      173 2023-06-05 03:08:57.412761 fedrq-0.8.0/src/fedrq/_config.py
+-rw-r--r--   0        0        0     1181 2023-06-16 02:38:20.603415 fedrq-0.8.0/src/fedrq/_utils.py
+-rw-r--r--   0        0        0     2526 2023-06-16 02:38:20.604415 fedrq-0.8.0/src/fedrq/backends/__init__.py
+-rw-r--r--   0        0        0    14489 2023-06-20 21:21:53.608401 fedrq-0.8.0/src/fedrq/backends/base.py
+-rw-r--r--   0        0        0      630 2023-06-05 03:08:57.412761 fedrq-0.8.0/src/fedrq/backends/dnf/__init__.py
+-rw-r--r--   0        0        0     6949 2023-06-06 22:57:17.282340 fedrq-0.8.0/src/fedrq/backends/dnf/backend.py
+-rw-r--r--   0        0        0      741 2023-06-19 17:06:43.021535 fedrq-0.8.0/src/fedrq/backends/libdnf5/__init__.py
+-rw-r--r--   0        0        0    28272 2023-06-20 21:21:16.516440 fedrq-0.8.0/src/fedrq/backends/libdnf5/backend.py
+-rw-r--r--   0        0        0     2111 2023-06-18 22:08:35.139910 fedrq-0.8.0/src/fedrq/cli/__init__.py
+-rw-r--r--   0        0        0    15896 2023-06-20 21:21:53.609401 fedrq-0.8.0/src/fedrq/cli/base.py
+-rw-r--r--   0        0        0        0 2023-02-19 18:37:34.751046 fedrq-0.8.0/src/fedrq/cli/commands/__init__.py
+-rw-r--r--   0        0        0     2854 2023-06-05 03:08:57.412761 fedrq-0.8.0/src/fedrq/cli/commands/pkgs.py
+-rw-r--r--   0        0        0     1489 2023-06-06 22:57:17.282340 fedrq-0.8.0/src/fedrq/cli/commands/repolist.py
+-rw-r--r--   0        0        0     2425 2023-06-05 03:08:57.412761 fedrq-0.8.0/src/fedrq/cli/commands/subpkgs.py
+-rw-r--r--   0        0        0    10843 2023-06-06 00:02:46.964960 fedrq-0.8.0/src/fedrq/cli/commands/whatrequires.py
+-rw-r--r--   0        0        0    13071 2023-06-19 17:26:45.758192 fedrq-0.8.0/src/fedrq/cli/formatters.py
+-rw-r--r--   0        0        0    16472 2023-06-16 02:38:20.606415 fedrq-0.8.0/src/fedrq/config.py
+-rw-r--r--   0        0        0        0 2023-02-19 18:37:34.751046 fedrq-0.8.0/src/fedrq/data/__init__.py
+-rw-r--r--   0        0        0     7326 2023-06-20 21:21:53.609401 fedrq-0.8.0/src/fedrq/data/releases.toml
+-rw-r--r--   0        0        0        0 2023-02-19 18:37:34.752046 fedrq-0.8.0/src/fedrq/data/repos/__init__.py
+-rw-r--r--   0        0        0     2053 2023-06-06 22:57:17.282340 fedrq-0.8.0/src/fedrq/data/repos/almalinux.repo
+-rw-r--r--   0        0        0      639 2023-03-27 04:19:29.835647 fedrq-0.8.0/src/fedrq/data/repos/amazonlinux.repo
+-rw-r--r--   0        0        0     1386 2023-06-06 22:57:17.282340 fedrq-0.8.0/src/fedrq/data/repos/centos-stream-compose.repo
+-rw-r--r--   0        0        0     1850 2023-02-19 18:37:34.752046 fedrq-0.8.0/src/fedrq/data/repos/centos-stream.repo
+-rw-r--r--   0        0        0     1494 2023-06-06 22:57:17.283340 fedrq-0.8.0/src/fedrq/data/repos/centos-stream8-compose.repo
+-rw-r--r--   0        0        0     1599 2023-03-18 19:37:34.184930 fedrq-0.8.0/src/fedrq/data/repos/centos-stream8.repo
+-rw-r--r--   0        0        0     1342 2023-06-20 21:21:53.609401 fedrq-0.8.0/src/fedrq/data/repos/centos7.repo
+-rw-r--r--   0        0        0     1809 2023-06-06 22:57:17.283340 fedrq-0.8.0/src/fedrq/data/repos/eln.repo
+-rw-r--r--   0        0        0     2158 2023-06-06 22:57:17.283340 fedrq-0.8.0/src/fedrq/data/repos/epel.repo
+-rw-r--r--   0        0        0    14146 2023-06-06 22:57:17.283340 fedrq-0.8.0/src/fedrq/data/repos/fedora-eln.repo
+-rw-r--r--   0        0        0     2402 2023-02-19 18:37:34.752046 fedrq-0.8.0/src/fedrq/data/repos/fedora-rawhide.repo
+-rw-r--r--   0        0        0     1480 2023-02-19 18:37:34.752046 fedrq-0.8.0/src/fedrq/data/repos/fedora-updates-testing.repo
+-rw-r--r--   0        0        0     1422 2023-02-19 18:37:34.752046 fedrq-0.8.0/src/fedrq/data/repos/fedora-updates.repo
+-rw-r--r--   0        0        0     1375 2023-02-19 18:37:34.752046 fedrq-0.8.0/src/fedrq/data/repos/fedora.repo
+-rw-r--r--   0        0        0      425 2023-06-06 22:57:17.283340 fedrq-0.8.0/src/fedrq/data/repos/rawhide-buildroot.repo
+-rw-r--r--   0        0        0        0 2023-02-19 18:37:34.752046 fedrq-0.8.0/src/fedrq/py.typed
+-rw-r--r--   0        0        0     8912 2023-06-19 17:26:45.758192 fedrq-0.8.0/src/fedrq/release_repo.py
+-rw-r--r--   0        0        0      994 2023-06-20 21:21:53.609401 fedrq-0.8.0/src/fedrq/repoquery.py
+-rw-r--r--   0        0        0      154 2023-02-19 18:37:34.753046 fedrq-0.8.0/tests/.gitignore
+-rw-r--r--   0        0        0        0 2023-06-06 22:57:17.283340 fedrq-0.8.0/tests/__init__.py
+-rw-r--r--   0        0        0     2948 2023-06-16 02:38:20.607415 fedrq-0.8.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-06 22:57:17.283340 fedrq-0.8.0/tests/integration/__init__.py
+-rw-r--r--   0        0        0     1775 2023-06-16 02:38:20.607415 fedrq-0.8.0/tests/integration/test_backends.py
+-rw-r--r--   0        0        0      771 2023-06-16 02:38:20.608415 fedrq-0.8.0/tests/integration/test_pkgs.py
+-rw-r--r--   0        0        0     1292 2023-06-20 21:34:55.966590 fedrq-0.8.0/tests/integration/test_subpkgs.py
+-rw-r--r--   0        0        0     1761 2023-06-16 02:38:20.609415 fedrq-0.8.0/tests/integration/test_whatrequires.py
+-rw-r--r--   0        0        0     1370 2023-06-16 02:38:20.609415 fedrq-0.8.0/tests/integration/test_whatrequires_src.py
+-rw-r--r--   0        0        0        0 2023-06-06 22:57:17.283340 fedrq-0.8.0/tests/test_data/__init__.py
+-rw-r--r--   0        0        0      332 2023-02-19 18:37:34.753046 fedrq-0.8.0/tests/test_data/_template.spec
+-rwxr-xr-x   0        0        0     1449 2023-02-19 18:37:34.754046 fedrq-0.8.0/tests/test_data/build.sh
+-rw-r--r--   0        0        0     1130 2023-02-19 18:37:34.754046 fedrq-0.8.0/tests/test_data/repos/repo1/specs/e1/packageb.spec
+-rw-r--r--   0        0        0     1060 2023-02-19 18:37:34.754046 fedrq-0.8.0/tests/test_data/repos/repo1/specs/packagea.spec
+-rw-r--r--   0        0        0     1156 2023-02-19 18:37:34.754046 fedrq-0.8.0/tests/test_data/repos/repo1/specs/packageb.spec
+-rw-r--r--   0        0        0        0 2023-06-06 22:57:17.283340 fedrq-0.8.0/tests/unit/__init__.py
+-rw-r--r--   0        0        0     2128 2023-06-16 02:38:20.610415 fedrq-0.8.0/tests/unit/test_checkconfig.py
+-rw-r--r--   0        0        0     7163 2023-06-16 02:38:20.611415 fedrq-0.8.0/tests/unit/test_command.py
+-rw-r--r--   0        0        0     7780 2023-06-20 21:20:35.641482 fedrq-0.8.0/tests/unit/test_formatters.py
+-rw-r--r--   0        0        0     3361 2023-06-20 21:34:58.442587 fedrq-0.8.0/tests/unit/test_pkgs.py
+-rw-r--r--   0        0        0     1681 2023-06-16 02:38:20.612415 fedrq-0.8.0/tests/unit/test_release.py
+-rw-r--r--   0        0        0      449 2023-06-16 02:38:20.612415 fedrq-0.8.0/tests/unit/test_repo.py
+-rw-r--r--   0        0        0      640 2023-06-16 02:38:20.613415 fedrq-0.8.0/tests/unit/test_repolist.py
+-rw-r--r--   0        0        0     1325 2023-06-16 02:38:20.613415 fedrq-0.8.0/tests/unit/test_repoquery.py
+-rw-r--r--   0        0        0     2712 2023-06-16 02:38:20.614415 fedrq-0.8.0/tests/unit/test_subbpkgs.py
+-rw-r--r--   0        0        0     4088 2023-06-16 02:38:20.614415 fedrq-0.8.0/tests/unit/test_whatrequires.py
+-rw-r--r--   0        0        0      689 2023-06-16 02:38:20.615415 fedrq-0.8.0/tests/unit/test_whatrequires_src.py
+-rw-r--r--   0        0        0    14335 1970-01-01 00:00:00.000000 fedrq-0.8.0/PKG-INFO
```

### Comparing `fedrq-0.7.1/.builds/epel9.yml` & `fedrq-0.8.0/.builds/epel9.yml`

 * *Files 12% similar despite different names*

```diff
@@ -13,12 +13,13 @@
       cd fedrq/
       cat <<- 'EOF' > install.sh
       python3 -m venv venv
       ./venv/bin/pip install -U pip
       ./venv/bin/pip install nox
       EOF
       podman run -d -v $(pwd):/pwd:z -w /pwd --name c9ss --init centos:stream9 sleep infinity
+      podman exec c9ss dnf install -y createrepo_c rpm-build
       podman exec c9ss bash -xeu -o pipefail ./install.sh
   - pytest-py39: |
       podman exec c9ss ./venv/bin/nox -e test -- -v --durations=7
   - typing-py39: |
       podman exec c9ss ./venv/bin/nox -e typing
```

### Comparing `fedrq-0.7.1/.builds/main.yml` & `fedrq-0.8.0/.builds/main.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # SPDX-FileCopyrightText: 2022 Maxwell G <gotmax@e.email>
 # SPDX-License-Identifier: GPL-2.0-or-later
 
 ---
 image: fedora/rawhide
 packages:
+  - createrepo_c
   - hut
   - pandoc
   - python3-libdnf5
+  - rpm-build
   - rsync
   - scd2html
   - tar
 secrets:
   # Production Copr
   # - 759db354-8651-427c-b00a-0755164c8cae
   # Dev Copr
@@ -73,12 +75,11 @@
         exit
       fi
 
       tar czvf fedrq.tar.gz *.html
       hut pages publish fedrq.tar.gz -d gotmax23.srht.site -s "${site}"
   - lint: |
       cd fedrq
-      $nox -e lint -- --check
+      $nox -e lint
   - pytest: |
       cd fedrq
-      FEDRQ_BACKEND=dnf $nox -e test -- -v --durations=7
-      FEDRQ_BACKEND=libdnf5 $nox -e test -- -v --durations=7
+      $nox -e testa -- -v --durations=7
```

### Comparing `fedrq-0.7.1/.builds/mockbuild-36.yml` & `fedrq-0.8.0/.builds/mockbuild-37.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 # SPDX-FileCopyrightText: 2022 Maxwell G <gotmax@e.email>
 # SPDX-License-Identifier: GPL-2.0-or-later
 
 ---
-image: fedora/36
+image: fedora/37
 packages:
+  - createrepo_c
   - fedora-repos-rawhide
   - mock
   - mock-core-configs
+  - rpm-build
 sources:
   - https://git.sr.ht/~gotmax23/fedrq
 environment:
-  CHROOT: "fedora-36"
+  CHROOT: "fedora-37"
   nox: ./venv/bin/nox
 artifacts:
   - fedrq/results_fedrq.tar.gz
 tasks:
   - setup-add-mock-group: |
       sudo usermod -aG mock $USER
   - setup-venv: |
       cd fedrq
       python3 -m venv venv
       ./venv/bin/pip install nox
-  - mockbuild-f36: |
+  - mockbuild-f37: |
       cd fedrq
       $nox -e mockbuild -- --resultdir results_fedrq -r "${CHROOT}-$(rpm -E %_arch)" \
         -a 'https://download.copr.fedorainfracloud.org/results/rpmsoftwaremanagement/dnf5-unstable/fedora-$releasever-$basearch/' \
         --with libdnf5
       tar cvf results_fedrq.tar.gz results_fedrq
-  - pytest-py310: |
+  - pytest-py311: |
       cd fedrq
       sudo dnf copr enable -y rpmsoftwaremanagement/dnf5-unstable
       sudo dnf install -y python3-libdnf5
       # Only run the integration tests. Units are run in the RPM build.
-      FEDRQ_BACKEND=dnf $nox -e test -- -v -k 'no_rpm_mock' --durations=7
-  - typing-py310: |
+      $nox -e dnf_test -- -v -k 'no_rpm_mock' --durations=7
+  - typing-py311: |
       cd fedrq
       $nox -e typing
```

### Comparing `fedrq-0.7.1/.builds/mockbuild.yml` & `fedrq-0.8.0/.builds/mockbuild.yml`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 ---
 image: fedora/rawhide
 packages:
   - mock
   - mock-core-configs
   - rpmlint
+  - rpm-build
 sources:
   - https://git.sr.ht/~gotmax23/fedrq
 environment:
   CHROOT: fedora-rawhide
   nox: ./venv/bin/nox
 artifacts:
   - fedrq/results_fedrq.tar.gz
@@ -23,8 +24,8 @@
       ./venv/bin/pip install nox
   - mockbuild-rawhide: |
       cd fedrq
       $nox -e mockbuild -- --resultdir results_fedrq -r "${CHROOT}-$(rpm -E %_arch)"
       tar cvf results_fedrq.tar.gz results_fedrq
   - rpmlint: |
       cd fedrq/
-      rpmlint -r fedrq.rpmlintrc results_fedrq/*.rpm
+      rpmlint --ignore-unused-rpmlintrc -r fedrq.rpmlintrc results_fedrq/*.rpm
```

### Comparing `fedrq-0.7.1/CONTRIBUTING.md` & `fedrq-0.8.0/CONTRIBUTING.md`

 * *Files 8% similar despite different names*

```diff
@@ -69,14 +69,15 @@
 ## Linting and Unit Tests
 
 Unit tests are run with `pytest`.
 This project uses isort and black to format code, ruff for linting, and mypy
 for type checking.
 `reuse lint` is used to ensure that code follows the REUSE specification.
 You can run all of these tools using nox. Simply install nox with pip or dnf.
+The tests also require the `rpm-build` and createrepo_c` and packages.
 
 CI also runs a mock build against rawhide.
 Run `nox -e srpm` to build an SRPM containing the git HEAD
 or run `nox -e mockbuild` to preform a build in mock.
 
 builds.sr.ht runs CI for patches sent to the mailing list,
 but please run the tests locally before submitting your changes.
```

### Comparing `fedrq-0.7.1/LICENSES/GPL-2.0-or-later.txt` & `fedrq-0.8.0/LICENSES/GPL-2.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.1/LICENSES/MIT.txt` & `fedrq-0.8.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.1/LICENSES/PSF-2.0.txt` & `fedrq-0.8.0/LICENSES/PSF-2.0.txt`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.1/LICENSES/Unlicense.txt` & `fedrq-0.8.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.1/NEWS.md` & `fedrq-0.8.0/NEWS.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,39 @@
 NEWS
 =====
 
+## 0.8.0 - 2023-06-21 <a id='0.8.0'></a>
+
+### Added
+
+- add --version flag to CLI
+- improve repo loading error handling ([#31])
+- add CentOS 7 release configuration
+
+### Changed
+
+- `fedrq.config.Release.get_base` - allow omitting `config` arg.
+  This previously emitted a deprecation warning ([`efc2828`][efc2828]).
+- `ReleaseConfig` - make `repogs` a proper pydantic model field ([`d8cff5a`][d8cff5a]).
+
+### Fixed
+
+- fix Changelog URL in Python/PyPI metadata
+- fix typo in help message for `--latest`. Contributed by Sandro (~penguinpee).
+- backends - fix MissingBackendError message grammar
+
+
+### New contributors
+
+Thanks to Sandro (~penguinpee) for your first fedrq contribution!
+
+[#31]: https://todo.sr.ht/~gotmax23/fedrq/31
+[efc2828]: https://git.sr.ht/~gotmax23/fedrq/commit/efc2828b75b60fe325429ddff39f9082d7f03b1e
+[d8cff5a]: https://git.sr.ht/~gotmax23/fedrq/commit/d8cff5af8696d4c1df8e90cf0d76f9dde09ae45c
+
 ## 0.7.1 - 2023-05-31 <a id='0.7.1'></a>
 
 ### Fixed
 
 - libdnf5: fix downloadsize and size formatters compat.
   This change is needed to maintain compat after
   [rpm-software-management/dnf5#766fb3a][766fb3a].
```

### Comparing `fedrq-0.7.1/README.md` & `fedrq-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.1/contrib/add_frag.py` & `fedrq-0.8.0/contrib/add_frag.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.1/contrib/api_examples/a_noarch_bash.py` & `fedrq-0.8.0/contrib/api_examples/a_noarch_bash.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.1/contrib/api_examples/ftbfs_retirements.py` & `fedrq-0.8.0/contrib/api_examples/ftbfs_retirements.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.1/contrib/deploy-docsite/main.yaml` & `fedrq-0.8.0/contrib/deploy-docsite/main.yaml`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.1/contrib/deploy-docsite/roles/configure/tasks/main.yml` & `fedrq-0.8.0/contrib/deploy-docsite/roles/configure/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.1/contrib/fedoraify.py` & `fedrq-0.8.0/contrib/fedoraify.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.1/doc/API/Summary.md` & `fedrq-0.8.0/doc/API/Summary.md`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.1/doc/API/backends/libdnf5.md` & `fedrq-0.8.0/doc/API/backends/libdnf5.md`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.1/doc/dnf-repoquery-diff.md` & `fedrq-0.8.0/doc/dnf-repoquery-diff.md`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.1/doc/fedrq.1.scd` & `fedrq-0.8.0/doc/fedrq.1.scd`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.1/doc/fedrq.5.scd` & `fedrq-0.8.0/doc/fedrq.5.scd`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.1/fedrq.spec` & `fedrq-0.8.0/fedrq.spec`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright (C) 2022 Maxwell G <gotmax@e.email>
 # SPDX-License-Identifier: MIT
 # License text: https://spdx.org/licenses/MIT.html
 
 %bcond libdnf5 %[0%{?fedora} >= 38]
 
 Name:           fedrq
-Version:        0.7.1
+Version:        0.8.0
 Release:        1%{?dist}
 Summary:        A tool to query the Fedora and EPEL repositories
 
 # - code is GPL-2.0-or-later
 # - the data and config files in fedrq/data are UNLICENSEed
 # - Embeded repo defs are MIT.
 # - PSF-2.0 code copied from Cpython 3.11 for older Python versions
@@ -95,14 +95,17 @@
 %{bash_completions_dir}/fedrq
 %{fish_completions_dir}/fedrq.fish
 %{_mandir}/man1/fedrq.1*
 %{_mandir}/man5/fedrq.5*
 
 
 %changelog
+* Wed Jun 21 2023 Maxwell G <maxwell@gtmx.me> - 0.8.0-1
+- Release 0.8.0.
+
 * Wed May 31 2023 Maxwell G <maxwell@gtmx.me> - 0.7.1-1
 - Release 0.7.1.
 
 * Tue May 30 2023 Maxwell G <maxwell@gtmx.me> - 0.7.0-1
 - Release 0.7.0.
 
 * Sat Apr 08 2023 Maxwell G <maxwell@gtmx.me> - 0.6.0-1
```

### Comparing `fedrq-0.7.1/mkdocs.yml` & `fedrq-0.8.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.1/pyproject.toml` & `fedrq-0.8.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 # seperately
 requires = ["flit_core >=3.7,<4"]
 build-backend = "flit_core.buildapi"
 
 
 [project]
 name = "fedrq"
-description = "fedrq is a tool to query the Fedora and EPEL repositories"
-version = "0.7.1"
+dynamic = ["description", "version"]
 authors = [{ name = "Maxwell G", email = "gotmax@e.email" }]
 readme = "README.md"
 license = { text = "GPL-2.0-or-later AND Unlicense AND MIT" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
@@ -36,47 +35,55 @@
     "requests",
     # Optional dependency for `fedrq check-config --dump`
     # "tomli-w",
 ]
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
-lint = [
+codeqa = [
+    "ruff",
+    "reuse",
+]
+doc = [
+    # mkdocstrings-python uses black to format function signatures
+    "black",
+    "mkdocs",
+    "mkdocs-material",
+    "mkdocstrings[python]>=0.18",
+    "mkdocs-exclude",
+]
+formatters = [
     "black",
     "isort",
+]
+typing = [
     "mypy",
-    "reuse",
-    "ruff",
-    "tomli-w",
     "types-requests",
     # Optional fedrq runtime dependency
     "argcomplete",
     "typing_extensions",
+    "tomli-w",
 ]
 test = [
     "pytest",
     "pytest-mock",
     "tomli-w",
 ]
-doc = [
-    # mkdocstrings-python uses this to format function signatures
-    "black",
-    "mkdocs",
-    "mkdocs-material",
-    "mkdocstrings[python]>=0.18",
-    "mkdocs-exclude",
-]
 dev = [
+    "fedrq[codeqa]",
+    "fedrq[doc]",
+    "fedrq[formatters]",
     "fedrq[test]",
-    "fedrq[lint]",
+    "fedrq[typing]",
+    "nox",
 ]
 
 [project.urls]
 Homepage = "https://fedrq.gtmx.me"
-Changelog = "https://fedrq.gtmx.me/Changelog"
+Changelog = "https://fedrq.gtmx.me/News"
 "Mailing List" = "https://lists.sr.ht/~gotmax23/fedrq"
 Source = "https://git.sr.ht/~gotmax23/fedrq"
 
 [project.scripts]
 fedrq = "fedrq.cli:main"
 
 [tool.flit.sdist]
@@ -105,7 +112,37 @@
 addopts = [
     "--import-mode=importlib",
 ]
 
 
 [tool.isort]
 profile = "black"
+add_imports = [
+    'from __future__ import annotations',
+]
+
+
+[tool.coverage.run]
+omit = [
+    "src/fedrq/_compat.py",
+    "src/fedrq/repoquery.py",
+    "src/fedrq/__main__.py",
+]
+
+[tool.coverage.report]
+# https://coverage.readthedocs.io/en/latest/excluding.html#advanced-exclusion
+# These should use single quotes in TOML, as they're regular expressions.
+exclude_lines = [
+    'pragma: no cover',
+    'raise NotImplementedError',
+    'if __name__ == .__main__.:',
+    'if TYPE_CHECKING:',
+    'if t\.TYPE_CHECKING:',
+    '@(abc\.)?abstractmethod',
+    '@overload',
+    'except ImportError',
+]
+omit = [
+    "src/fedrq/_compat.py",
+    "src/fedrq/repoquery.py",
+    "src/fedrq/__main__.py",
+]
```

### Comparing `fedrq-0.7.1/ruff.toml` & `fedrq-0.8.0/ruff.toml`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.1/src/fedrq/_compat.py` & `fedrq-0.8.0/src/fedrq/_compat.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.1/src/fedrq/_utils.py` & `fedrq-0.8.0/src/fedrq/_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import typing as t
 from collections.abc import MutableMapping
 
 if t.TYPE_CHECKING:
     from fedrq.backends.base import PackageCompat, PackageQueryCompat
 
 logger = logging.getLogger(__name__)
-# PkgIter = t.Union[hawkey.Query, t.Iterable[dnf.package.Package]]
 
 
 def get_source_name(package: PackageCompat) -> str:
     return package.name if package.arch == "src" else t.cast(str, package.source_name)
 
 
 def filter_latest(query: PackageQueryCompat, latest: t.Optional[int]) -> None:
```

### Comparing `fedrq-0.7.1/src/fedrq/backends/__init__.py` & `fedrq-0.8.0/src/fedrq/backends/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,12 +78,12 @@
             return backend.get_backend()
         if not fallback:
             raise backends.missing[default]
         if backend := next(iter(backends.available.values()), None):
             return backend.get_backend()
         _split = ", ".join(backends.missing)
         raise MissingBackendError(
-            f"Neither of the following backends were available: {_split}"
+            f"None of the following backends were available: {_split}"
         )
 
 
 get_default_backend = _DefaultBackend()
```

### Comparing `fedrq-0.7.1/src/fedrq/backends/base.py` & `fedrq-0.8.0/src/fedrq/backends/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     from fedrq.config import Release
 
 _QueryT = TypeVar("_QueryT", bound="PackageQueryCompat")
 LOG = logging.getLogger("fedrq.backends")
 
 
 @runtime_checkable
-class PackageCompat(Protocol):
+class PackageCompat(Protocol):  # pragma: no cover
     """
     Common interface provided by dnf.package.Package and other backends
     """
 
     @property
     def name(self) -> str:
         ...
@@ -194,15 +194,15 @@
         ...
 
     def __ge__(self, other) -> bool:
         ...
 
 
 @runtime_checkable
-class PackageQueryCompat(Protocol):
+class PackageQueryCompat(Protocol):  # pragma: no cover
     """
     Common PackageQuery interface provided by hawkey.Query and other backends.
     """
 
     def filter(self, **kwargs) -> PackageQueryCompat:
         """
         Filter the PackageQuery.
@@ -539,9 +539,9 @@
     """
 
     BACKEND: str
     BaseMaker: type[BaseMakerBase]
     Package: type[PackageCompat]
     PackageQuery: type[PackageQueryCompat]
     Repoquery: type[RepoqueryBase]
-    RepoError: Exception
+    RepoError: type[BaseException]
     get_releasever: Callable[[], str]
```

### Comparing `fedrq-0.7.1/src/fedrq/backends/dnf/__init__.py` & `fedrq-0.8.0/src/fedrq/backends/dnf/__init__.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.1/src/fedrq/backends/dnf/backend.py` & `fedrq-0.8.0/src/fedrq/backends/dnf/backend.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.1/src/fedrq/backends/libdnf5/__init__.py` & `fedrq-0.8.0/src/fedrq/backends/libdnf5/__init__.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.1/src/fedrq/backends/libdnf5/backend.py` & `fedrq-0.8.0/src/fedrq/backends/libdnf5/backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -808,15 +808,15 @@
         return r_query
 
     @property
     def backend(self) -> BackendMod:
         return sys.modules[__name__]
 
 
-def _dnf_getreleasever() -> str:
+def _dnf_getreleasever() -> str:  # pragma: no cover
     # This is taken from dnf and slightly modified
     #
     # SPDX-License-Identifier: GPL-2.0-or-later
     # Copyright (C) 2012-2015  Red Hat, Inc.
     DISTROVERPKG = (
         "system-release(releasever)",
         "system-release",
@@ -869,15 +869,15 @@
     Return the system releasever
     """
     # libdnf5 > 5.0.10
     if hasattr(libdnf5.conf.Vars, "detect_release"):
         base = libdnf5.base.Base()
         return libdnf5.conf.Vars.detect_release(base.get_weak_ptr(), "/").get()
     # Fall back to our copy of dnf4's code
-    else:
+    else:  # pragma: no cover
         return _dnf_getreleasever()
 
 
 RepoError = RuntimeError
 
 __all__ = (
     "BACKEND",
```

### Comparing `fedrq-0.7.1/src/fedrq/cli/__init__.py` & `fedrq-0.8.0/src/fedrq/cli/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -41,19 +41,26 @@
     "Whatrequires",
     "WhatrequiresSrc",
     "Whatsuggests",
     "Whatsupplements",
 )
 
 
+def version() -> str:
+    from fedrq import __version__
+
+    return __version__
+
+
 def main(argv: Sequence | None = None, **kwargs) -> None:
     parser = argparse.ArgumentParser(
         description="fedrq is a tool for querying the Fedora and EPEL repositories.",
         **kwargs,
     )
+    parser.add_argument("--version", action="version", version=version())
     subparsers = parser.add_subparsers(
         title="Subcommands", dest="action", required=True
     )
     for name, cls in COMMANDS.items():
         cls.make_parser(subparsers.add_parser, name=name, add_help=True)
     if HAS_ARGCOMPLETE:
         argcomplete.autocomplete(parser)
```

### Comparing `fedrq-0.7.1/src/fedrq/cli/base.py` & `fedrq-0.8.0/src/fedrq/cli/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,15 +209,15 @@
         )
         parser.add_argument(  # type: ignore[attr-defined]
             "names", metavar="NAME", nargs="*", help="Mutually exclusive with --stdin"
         ).completer = lambda **_: ()
         parser.add_argument(
             "-i", "--stdin", help="Read package names from stdin.", action="store_true"
         )
-        parser.add_argument("-l", "--latest", default=1, help="'all' or an intenger")
+        parser.add_argument("-l", "--latest", default=1, help="'all' or an integer")
         parser.add_argument(  # type: ignore[attr-defined]
             "-F",
             "--formatter",
             default="plain",
         ).completer = cls.formatters._argcompleter
         cachedir_group = parser.add_mutually_exclusive_group()
         cachedir_group.add_argument(
@@ -348,14 +348,15 @@
             elif func == "disable":
                 bm.disable_repo(repo, True)
             else:
                 raise ValueError
 
     @v_fatal_error
     def v_rq(self) -> str | None:
+        flog = mklog("fedrq.cli.Command", "v_rq")
         conf: dict[str, Any] = {}
         bvars: dict[str, Any] = {}
 
         # Set cachedir if it's explicitly passed
         if self.args.cachedir:
             conf["cachedir"] = str(self.args.cachedir)
         # Disable release based smartcache if user explicitly disabled it or if
@@ -368,15 +369,20 @@
             bvars["arch"] = self.args.forcearch
         bm = self.backend.BaseMaker()
         try:
             self.release.make_base(self.config, conf, bvars, bm, False)
             self._enable_disable_bm(bm)
         except ConfigError as exc:
             return str(exc)
-        self.rq = self.backend.Repoquery(bm.fill_sack())
+        try:
+            filled = bm.fill_sack()
+        except self.backend.RepoError as exc:
+            flog.debug("RepoError: ", exc_info=exc)
+            return str(exc)
+        self.rq = self.backend.Repoquery(filled)
         return None
 
     @v_fatal_error
     def v_backend(self) -> str | None:
         try:
             _ = self.backend
         except MissingBackendError as exc:
```

### Comparing `fedrq-0.7.1/src/fedrq/cli/commands/pkgs.py` & `fedrq-0.8.0/src/fedrq/cli/commands/pkgs.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.1/src/fedrq/cli/commands/repolist.py` & `fedrq-0.8.0/src/fedrq/cli/commands/repolist.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.1/src/fedrq/cli/commands/subpkgs.py` & `fedrq-0.8.0/src/fedrq/cli/commands/subpkgs.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.1/src/fedrq/cli/commands/whatrequires.py` & `fedrq-0.8.0/src/fedrq/cli/commands/whatrequires.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.1/src/fedrq/cli/formatters.py` & `fedrq-0.8.0/src/fedrq/cli/formatters.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.1/src/fedrq/config.py` & `fedrq-0.8.0/src/fedrq/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from pathlib import Path
 
 if sys.version_info < (3, 11):
     import tomli as tomllib
 else:
     import tomllib
 
-from pydantic import BaseModel, Field, PrivateAttr, validator
+from pydantic import BaseModel, Field, validator
 
 from fedrq._compat import StrEnum
 from fedrq._config import ConfigError
 from fedrq._utils import merge_dict, mklog
 from fedrq.backends import BACKENDS, get_default_backend
 from fedrq.backends.base import BaseMakerBase
 from fedrq.release_repo import AliasRepoG, DefaultRepoGs, RepoG, Repos
@@ -76,24 +76,23 @@
     append_system_repos: bool = False
 
     koschei_collection: t.Optional[str] = None
     copr_chroot_fmt: t.Optional[str] = None
 
     full_def_paths: t.ClassVar[list[t.Union[Traversable, Path]]] = []
     repo_aliases: dict[str, str] = {}
-    _repogs = PrivateAttr()
+    repogs: Repos = Field(DefaultRepoGs, exclude=True)
 
-    @property
-    def repogs(self) -> Repos:
-        return self._repogs
+    class Config:
+        arbitrary_types_allowed = True
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self._repogs = DefaultRepoGs.new(
-            self.defs | AliasRepoG.from_str_mapping(self.repo_aliases)
+    @validator("repogs", always=True)
+    def v_repogs(cls, value: Repos, values: dict[str, t.Any]) -> Repos:
+        return (
+            value | values["defs"] | AliasRepoG.from_str_mapping(values["repo_aliases"])
         )
 
     @validator("defpaths")
     def v_defpaths(cls, value, values) -> dict[str, t.Any]:
         flog = mklog(__name__, "ReleaseConfig", "_get_full_defpaths")
         flog.debug(f"Getting defpaths for {values['name']}: {value}")
         values["full_def_paths"] = cls._get_full_defpaths(
@@ -251,30 +250,25 @@
         config: RQConfig | None = None,
         base_conf: dict[str, t.Any] | None = None,
         base_vars: dict[str, t.Any] | None = None,
         base_maker: BaseMakerBase | None = None,
         fill_sack: bool = True,
     ) -> dnf.Base | libdnf5.base.Base:
         """
-        :param config: An RQConfig object. Not passing this argument is deprecated.
-                       DEPRECATED since 0.4.0: A new RQConfig object will be
-                                               created if this is None.
+        :param config: An RQConfig object. If this is not passed, `self.config` is used.
         :param base_conf: Base session configuration
         :param base_vars: Base session vars/substitutions (arch, basearch,
                                                            releasever, etc.)
         :param base_maker: Existing BaseMaker object to configure.
                            If base_maker is None, a new one will be created.
         :param fill_sack: Whether to fill the Base object's package sack or
                           just return the Base object after applying configuration.
         """
         if config is None:
-            warnings.warn(
-                "DEPRECATED since 0.4.0: Provide an RQConfig object for 'config'"
-            )
-            config = get_config()
+            config = self.config
         base_conf = base_conf or {}
         base_vars = base_vars or {}
         releasever = config.backend_mod.get_releasever()
         if (
             "cachedir" not in base_conf
             and config.smartcache
             and self.version != releasever
```

### Comparing `fedrq-0.7.1/src/fedrq/data/releases.toml` & `fedrq-0.8.0/src/fedrq/data/releases.toml`

 * *Files 2% similar despite different names*

```diff
@@ -157,14 +157,31 @@
     "centos-stream8-appstream-source",
 ]
 defs.compose-latest = [
     "centos-stream8-compose-latest-*",
 ]
 repo_aliases.kojihub = "@baseurl:https://kojihub.stream.centos.org/kojifiles/repos/{}/latest/$basearch"
 
+[releases.centos7]
+matcher = "^c(7)$"
+defpaths = [
+    "centos7.repo",
+    "epel.repo",
+]
+defs.base = [
+    "centos", "centos-source",
+    "centos-updates", "centos-updates-source",
+    "centos-extras", "centos-extras-source",
+]
+defs.epel = [
+    "@base",
+    "@repo:epel",
+    "epel-source",
+]
+
 [releases.amazonlinux]
 matcher = '^amazon(\d+)$'
 defs.base = ["amazonlinux", "amazonlinux-source"]
 defpaths = ["amazonlinux.repo"]
 
 [releases.almalinux]
 matcher = '^al(9|1\d)$'
```

### Comparing `fedrq-0.7.1/src/fedrq/data/repos/almalinux.repo` & `fedrq-0.8.0/src/fedrq/data/repos/almalinux.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.1/src/fedrq/data/repos/amazonlinux.repo` & `fedrq-0.8.0/src/fedrq/data/repos/amazonlinux.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.1/src/fedrq/data/repos/centos-stream-compose.repo` & `fedrq-0.8.0/src/fedrq/data/repos/centos-stream-compose.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.1/src/fedrq/data/repos/centos-stream.repo` & `fedrq-0.8.0/src/fedrq/data/repos/centos-stream.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.1/src/fedrq/data/repos/centos-stream8-compose.repo` & `fedrq-0.8.0/src/fedrq/data/repos/centos-stream8-compose.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.1/src/fedrq/data/repos/centos-stream8.repo` & `fedrq-0.8.0/src/fedrq/data/repos/centos-stream8.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.1/src/fedrq/data/repos/eln.repo` & `fedrq-0.8.0/src/fedrq/data/repos/eln.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.1/src/fedrq/data/repos/epel.repo` & `fedrq-0.8.0/src/fedrq/data/repos/epel.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.1/src/fedrq/data/repos/fedora-eln.repo` & `fedrq-0.8.0/src/fedrq/data/repos/fedora-eln.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.1/src/fedrq/data/repos/fedora-rawhide.repo` & `fedrq-0.8.0/src/fedrq/data/repos/fedora-rawhide.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.1/src/fedrq/data/repos/fedora-updates-testing.repo` & `fedrq-0.8.0/src/fedrq/data/repos/fedora-updates-testing.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.1/src/fedrq/data/repos/fedora-updates.repo` & `fedrq-0.8.0/src/fedrq/data/repos/fedora-updates.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.1/src/fedrq/data/repos/fedora.repo` & `fedrq-0.8.0/src/fedrq/data/repos/fedora.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.1/src/fedrq/release_repo.py` & `fedrq-0.8.0/src/fedrq/release_repo.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.1/src/fedrq/repoquery.py` & `fedrq-0.8.0/src/fedrq/repoquery.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     RepoqueryBase,
 )
 
 backend: BackendMod = get_default_backend()
 BaseMaker: type[BaseMakerBase] = backend.BaseMaker
 Package: type[PackageCompat] = backend.Package
 PackageQuery: type[PackageQueryCompat] = backend.PackageQuery
-RepoError: Exception = backend.RepoError
+RepoError: type[BaseException] = backend.RepoError
 Repoquery: type[RepoqueryBase] = backend.Repoquery
 get_releasever: Callable[[], str] = backend.get_releasever
 BACKEND: str = backend.BACKEND
 
 __all__ = (
     "BACKEND",
     "BaseMaker",
```

### Comparing `fedrq-0.7.1/tests/conftest.py` & `fedrq-0.8.0/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # SPDX-FileCopyrightText: 2022 Maxwell G <gotmax@e.email>
 # SPDX-License-Identifier: GPL-2.0-or-later
 
+from __future__ import annotations
+
 import os
 import subprocess
 from pathlib import Path
 from shutil import rmtree
 
 import pytest
```

### Comparing `fedrq-0.7.1/tests/integration/test_backends.py` & `fedrq-0.8.0/tests/integration/test_backends.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Copyright (C) 2023 Maxwell G <gotmax@e.email>
 #
 # SPDX-License-Identifier: GPL-2.0-or-later
 
+from __future__ import annotations
+
 import pytest
 
 from fedrq.backends.base import BackendMod
 
 # ruff: noqa: E501
 TEST_REPO = "https://download.copr.fedorainfracloud.org/results/gotmax23/community.general.copr_integration_tests/fedora-$releasever-$basearch/"
 TEST_REPO_KEY = "https://download.copr.fedorainfracloud.org/results/gotmax23/community.general.copr_integration_tests/pubkey.gpg"
```

### Comparing `fedrq-0.7.1/tests/integration/test_pkgs.py` & `fedrq-0.8.0/tests/integration/test_pkgs.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # SPDX-FileCopyrightText: 2022 Maxwell G <gotmax@e.email>
 # SPDX-License-Identifier: GPL-2.0-or-later
 
+from __future__ import annotations
+
 import pytest
 
 import fedrq.cli
 
 
 @pytest.mark.skip(
     "This test loads rawhide metadata and is expensive. We already load f37."
```

### Comparing `fedrq-0.7.1/tests/integration/test_subpkgs.py` & `fedrq-0.8.0/tests/integration/test_subpkgs.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # SPDX-FileCopyrightText: 2022 Maxwell G <gotmax@e.email>
 # SPDX-License-Identifier: GPL-2.0-or-later
 
+from __future__ import annotations
+
 import pytest
 
 import fedrq.cli
 
 YT_DLP_SUPKGS = [
     "yt-dlp-bash-completion",
     "yt-dlp-fish-completion",
@@ -24,14 +26,16 @@
 
 @pytest.mark.no_rpm_mock
 def test_subpkgs_match2(capsys):
     # Find the source packages that contain a subpackage that match '*-devel'
     fedrq.cli.main(
         [
             "subpkgs",
+            "-b",
+            "f37",
             "ansible-core",
             "moby-engine",
             "python-pip",
             "yt-dlp",
             "gh",  # no matches
             "-M",
             "*-fish-completion",
```

### Comparing `fedrq-0.7.1/tests/integration/test_whatrequires.py` & `fedrq-0.8.0/tests/integration/test_whatrequires.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # SPDX-FileCopyrightText: 2022 Maxwell G <gotmax@e.email>
 # SPDX-License-Identifier: GPL-2.0-or-later
 
+from __future__ import annotations
+
 import pytest
 
 import fedrq.cli
 
 YT_DLP_SUPKGS = {
     "yt-dlp-bash-completion",
     "yt-dlp-zsh-completion",
```

### Comparing `fedrq-0.7.1/tests/integration/test_whatrequires_src.py` & `fedrq-0.8.0/tests/integration/test_whatrequires_src.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Copyright (C) 2023 Maxwell G <gotmax@e.email>
 #
 # SPDX-License-Identifier: GPL-2.0-or-later
 
+from __future__ import annotations
+
 import pytest
 
 
 @pytest.mark.no_rpm_mock
 @pytest.mark.parametrize(
     "args",
     [
```

### Comparing `fedrq-0.7.1/tests/test_data/build.sh` & `fedrq-0.8.0/tests/test_data/build.sh`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.1/tests/test_data/repos/repo1/specs/e1/packageb.spec` & `fedrq-0.8.0/tests/test_data/repos/repo1/specs/e1/packageb.spec`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.1/tests/test_data/repos/repo1/specs/packagea.spec` & `fedrq-0.8.0/tests/test_data/repos/repo1/specs/packagea.spec`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.1/tests/test_data/repos/repo1/specs/packageb.spec` & `fedrq-0.8.0/tests/test_data/repos/repo1/specs/packageb.spec`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.1/tests/unit/test_checkconfig.py` & `fedrq-0.8.0/tests/unit/test_checkconfig.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # SPDX-FileCopyrightText: 2022 Maxwell G <gotmax@e.email>
 # SPDX-License-Identifier: GPL-2.0-or-later
 
+from __future__ import annotations
+
 from pathlib import Path
 
 try:
     import tomllib
 except ImportError:
     import tomli as tomllib
```

### Comparing `fedrq-0.7.1/tests/unit/test_command.py` & `fedrq-0.8.0/tests/unit/test_command.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # SPDX-FileCopyrightText: 2022 Maxwell G <gotmax@e.email>
 # SPDX-License-Identifier: GPL-2.0-or-later
 """
 Generic tests for fedrq.cli.Command
 """
+from __future__ import annotations
+
 import os
 import shutil
 from pathlib import Path
 
 import pytest
 import tomli_w
```

### Comparing `fedrq-0.7.1/tests/unit/test_formatters.py` & `fedrq-0.8.0/tests/unit/test_formatters.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,24 @@
 # SPDX-FileCopyrightText: 2022 Maxwell G <gotmax@e.email>
 # SPDX-License-Identifier: GPL-2.0-or-later
 
+from __future__ import annotations
+
 import json
+from functools import cache
 
 import pytest
 
-import fedrq.cli.formatters as formatters
+from fedrq import config as rqconfig
+from fedrq.cli import formatters
+
+
+@cache
+def get_rq():
+    return rqconfig.get_config(load_filelists="always").get_rq("tester", "base")
 
 
 def formatter(query, formatter_name="plain", *args, attr=False, **kwargs):
     result = sorted(
         (
             str(i)
             for i in formatters.DefaultFormatters.get_formatter(formatter_name).format(
@@ -26,15 +35,16 @@
                 ).format(query, *args, **kwargs)
             )
         )
     return result
 
 
 # @pytest.mark.parametrize("special_repos", ("repo1",), indirect=["special_repos"])
-def test_plain_formatter(repo_test_rq, target_cpu):
+def test_plain_formatter(patch_config_dirs, target_cpu):
+    repo_test_rq = get_rq()
     expected = sorted(
         (
             "packagea-1-1.fc36.noarch",
             "packagea-1-1.fc36.src",
             "packagea-sub-1-1.fc36.noarch",
             "packageb-1-1.fc36.src",
             f"packageb-1-1.fc36.{target_cpu}",
@@ -45,15 +55,16 @@
         )
     )
     query = repo_test_rq.query()
     assert formatter(query) == expected
     assert formatter(query, "plain") == expected
 
 
-def test_plainwithrepo_formatter(repo_test_rq, target_cpu):
+def test_plainwithrepo_formatter(patch_config_dirs, repo_test_rq, target_cpu):
+    repo_test_rq = get_rq()
     expected = sorted(
         (
             "packagea-1-1.fc36.noarch testrepo1",
             "packagea-1-1.fc36.src testrepo1",
             "packagea-sub-1-1.fc36.noarch testrepo1",
             "packageb-1-1.fc36.src testrepo1",
             f"packageb-1-1.fc36.{target_cpu} testrepo1",
@@ -64,15 +75,16 @@
         )
     )
     query = repo_test_rq.query()
     assert formatter(query, "plainwithrepo") == expected
     assert formatter(query, "nevrr") == expected
 
 
-def test_name_formatter(repo_test_rq):
+def test_name_formatter(patch_config_dirs):
+    repo_test_rq = get_rq()
     expected = sorted(
         (
             "packagea",
             "packagea",
             "packagea-sub",
             "packageb",
             "packageb",
@@ -83,15 +95,16 @@
         )
     )
     query = repo_test_rq.query()
     assert formatter(query, "name") == expected
     assert formatter(query, "attr:name") == expected
 
 
-def test_evr_formatter(repo_test_rq):
+def test_evr_formatter(patch_config_dirs):
+    repo_test_rq = get_rq()
     query = repo_test_rq.query(name__glob="packageb*")
     result = sorted(
         (
             "11111:2-1.fc36",
             "11111:2-1.fc36",
             "11111:2-1.fc36",
             "1-1.fc36",
@@ -99,86 +112,96 @@
             "1-1.fc36",
         )
     )
     assert formatter(query, "evr") == result
     assert formatter(query, "attr:evr") == result
 
 
-def test_nv_formatter(repo_test_rq):
+def test_nv_formatter(patch_config_dirs):
+    repo_test_rq = get_rq()
     query = repo_test_rq.query(name__glob="packagea*")
     expected = sorted(("packagea-1", "packagea-1", "packagea-sub-1"))
     assert formatter(query, "nv") == expected
 
 
-def test_source_formatter(repo_test_rq):
+def test_source_formatter(patch_config_dirs):
+    repo_test_rq = get_rq()
     query = repo_test_rq.query()
     assert formatter(query, "source") == ["packagea", "packageb"]
 
 
 @pytest.mark.parametrize(
     "latest,expected",
     (
         (None, ["1", "1", "2", "2"]),
         (1, ["2", "2"]),
     ),
 )
-def test_version_formatter(repo_test_rq, latest, expected):
+def test_version_formatter(patch_config_dirs, latest, expected):
+    repo_test_rq = get_rq()
     query = repo_test_rq.query(name="packageb", latest=latest)
     assert formatter(query, "version") == expected
     assert formatter(query, "attr:version") == expected
 
 
-def test_epoch_formatter(repo_test_rq):
+def test_epoch_formatter(patch_config_dirs):
+    repo_test_rq = get_rq()
     query = repo_test_rq.query(name="packageb-sub")
     assert formatter(query, "epoch") == ["0", "11111"]
     assert formatter(query, "attr:epoch") == ["0", "11111"]
 
 
-def test_requires_formatter(repo_test_rq):
+def test_requires_formatter(patch_config_dirs):
+    repo_test_rq = get_rq()
     query = repo_test_rq.query(name=("packagea-sub", "packageb-sub"))
     assert len(query) == 3
     expected = [
         "/usr/share/packageb-sub",
         "package(b)",
         "packagea = 1-1.fc36",
         "vpackage(b) = 1-1.fc36",
     ]
     assert formatter(query, "requires", attr=True) == expected
 
 
-def test_repo_formatter(repo_test_rq):
+def test_repo_formatter(patch_config_dirs):
+    repo_test_rq = get_rq()
     query = repo_test_rq.query()
     result = formatter(query, "reponame", attr=True)
     assert len(query) == len(result)
     assert {"testrepo1"} == set(result)
 
 
-def test_repo_license_formatter(repo_test_rq):
+def test_repo_license_formatter(patch_config_dirs):
+    repo_test_rq = get_rq()
     query = repo_test_rq.query(name__glob="packagea*")
     result = formatter(query, "license", attr=True)
     assert result == ["Unlicense"] * 3
 
 
-def test_debug_name_formatter(repo_test_rq):
+def test_debug_name_formatter(patch_config_dirs):
+    repo_test_rq = get_rq()
     query = repo_test_rq.query(name="packageb")
     result = formatter(query, "debug_name", attr=True)
     assert result == ["packageb-debuginfo"] * len(query)
 
 
-def test_repo_files_formatter(repo_test_rq):
+def test_repo_files_formatter(patch_config_dirs):
+    repo_test_rq = get_rq()
     query = repo_test_rq.query(name=["packagea", "packageb"], arch="notsrc", latest=1)
     result = formatter(query, "files", attr=True)
     assert result == ["/usr/share/packagea", "/usr/share/packageb"]
 
 
 @pytest.mark.parametrize("attr", formatters._ATTRS)
-def test_formatter_sanity(repo_test_rq, attr):
+def test_formatter_sanity(patch_config_dirs, attr):
     """
     Sanity test to ensure that supported formatters work at all
     """
+    repo_test_rq = get_rq()
     query = repo_test_rq.query(
         name=["packagea", "packagea-sub", "packageb", "packageb-sub"], latest=1
     )
     result = formatter(query, attr)
     if attr not in (
         "provides",
         "requires",
@@ -188,15 +211,15 @@
         "suggests",
         "enhances",
         "supplements",
     ):
         assert len(result) == len(query)
 
 
-def test_json_formatter(repo_test_rq):
+def test_json_formatter(patch_config_dirs):
     expected = [
         {
             "name": "packagea",
             "evr": "1-1.fc36",
             "arch": "noarch",
             "requires": ["vpackage(b)"],
             "conflicts": [],
@@ -222,13 +245,14 @@
                 "subpackage(a)",
                 "packagea-sub = 1-1.fc36",
                 "vsubpackage(a) = 1-1.fc36",
             ],
             "source_name": "packagea",
         },
     ]
+    repo_test_rq = get_rq()
     query = repo_test_rq.resolve_pkg_specs(["packagea*"], latest=1)
     output = formatter(
         query, "json:name,evr,arch,requires,conflicts,provides,source_name"
     )
     assert len(output) == 1
     assert json.loads(output[0]) == expected
```

### Comparing `fedrq-0.7.1/tests/unit/test_pkgs.py` & `fedrq-0.8.0/tests/unit/test_pkgs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 # Copyright (C) 2023 Maxwell G <maxwell@gtmx.me>
 #
 # SPDX-License-Identifier: GPL-2.0-or-later
 
+from __future__ import annotations
+
 from collections.abc import Callable, Sequence
+from io import StringIO
 
 import pytest
+from pytest_mock import MockerFixture
 
 import fedrq.backends
 import fedrq.cli
+import fedrq.cli.base
 from fedrq.backends.base import BackendMod
 
 
 def test_disablerepo_wildcard(patch_config_dirs, capsys):
     fedrq.cli.main(["pkgs", "--disablerepo=*", "*"])
     out, err = capsys.readouterr()
     assert not out and not err
@@ -62,7 +67,41 @@
     base_maker = backend.BaseMaker(obj.rq.base)
     assert sorted(base_maker.repolist()) == sorted(repolist)
     # TODO: Add a proper API for this
     if backend.BACKEND == "dnf":
         assert releasever(backend) == base_maker.base.conf.substitutions["releasever"]
     else:
         assert releasever(backend) == base_maker.base.get_vars().get_value("releasever")
+
+
+def test_repo_error(
+    patch_config_dirs, mocker: MockerFixture, capsys: pytest.CaptureFixture
+):
+    backend = fedrq.backends.get_default_backend()
+    mocker.patch.object(
+        backend.BaseMaker,
+        "fill_sack",
+        side_effect=backend.RepoError("Failed to load repos!!!"),
+    )
+    with pytest.raises(SystemExit, match="^1$"):
+        fedrq.cli.main(["pkgs", "packagea"])
+    _, err = capsys.readouterr()
+    assert err == "FATAL ERROR: Failed to load repos!!!\n"
+
+
+def test_packages_stdin_error(capsys: pytest.CaptureFixture):
+    with pytest.raises(
+        SystemExit, match="Postional NAMEs can not be used with --stdin"
+    ):
+        fedrq.cli.main(["pkgs", "-i", "packagea"])
+
+
+def test_package_stdin(
+    patch_config_dirs,
+    capsys: pytest.CaptureFixture,
+    monkeypatch: pytest.MonkeyPatch,
+    target_cpu: str,
+):
+    monkeypatch.setattr(fedrq.cli.base.sys, "stdin", StringIO("packageb\n"))
+    fedrq.cli.main(["pkgs", "-i", "-F", "line:name,arch", "-A", "arched"])
+    out, _ = capsys.readouterr()
+    assert out == f"packageb : {target_cpu}\n"
```

### Comparing `fedrq-0.7.1/tests/unit/test_release.py` & `fedrq-0.8.0/tests/unit/test_release.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Copyright (C) 2023 Maxwell G <maxwell@gtmx.me>
 #
 # SPDX-License-Identifier: GPL-2.0-or-later
 
+from __future__ import annotations
+
 import pytest
 
 import fedrq.config
 
 
 @pytest.mark.parametrize(
     "args",
```

### Comparing `fedrq-0.7.1/tests/unit/test_repoquery.py` & `fedrq-0.8.0/tests/unit/test_repoquery.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # SPDX-FileCopyrightText: 2022 Maxwell G <gotmax@e.email>
 # SPDX-License-Identifier: GPL-2.0-or-later
 
 
+from __future__ import annotations
+
 from pathlib import Path
 
 from fedrq import config as rqconfig
 from fedrq.backends.base import PackageCompat, PackageQueryCompat, RepoqueryBase
 
 
 def test_make_base_rawhide_repos() -> None:
```

### Comparing `fedrq-0.7.1/tests/unit/test_subbpkgs.py` & `fedrq-0.8.0/tests/unit/test_subbpkgs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # SPDX-FileCopyrightText: 2022 Maxwell G <gotmax@e.email>
 # SPDX-License-Identifier: GPL-2.0-or-later
 
+from __future__ import annotations
+
 import pytest
 
 import fedrq.cli
 
 
 @pytest.fixture
 def run_command(capsys, patch_config_dirs):
```

### Comparing `fedrq-0.7.1/tests/unit/test_whatrequires.py` & `fedrq-0.8.0/tests/unit/test_whatrequires.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # SPDX-FileCopyrightText: 2022 Maxwell G <gotmax@e.email>
 # SPDX-License-Identifier: GPL-2.0-or-later
 
+from __future__ import annotations
+
 import pytest
 
 import fedrq.cli
 
 
 @pytest.fixture
 def run_command(capsys, patch_config_dirs):
```

### Comparing `fedrq-0.7.1/PKG-INFO` & `fedrq-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedrq
-Version: 0.7.1
+Version: 0.8.0
 Summary: fedrq is a tool to query the Fedora and EPEL repositories
 Author-email: Maxwell G <gotmax@e.email>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -14,41 +14,47 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Development Status :: 4 - Beta
 Classifier: Typing :: Typed
 Classifier: Environment :: Console
 Requires-Dist: pydantic ~= 1.0
 Requires-Dist: tomli; python_version<'3.11'
 Requires-Dist: requests
+Requires-Dist: ruff ; extra == "codeqa"
+Requires-Dist: reuse ; extra == "codeqa"
+Requires-Dist: fedrq[codeqa] ; extra == "dev"
+Requires-Dist: fedrq[doc] ; extra == "dev"
+Requires-Dist: fedrq[formatters] ; extra == "dev"
 Requires-Dist: fedrq[test] ; extra == "dev"
-Requires-Dist: fedrq[lint] ; extra == "dev"
+Requires-Dist: fedrq[typing] ; extra == "dev"
+Requires-Dist: nox ; extra == "dev"
 Requires-Dist: black ; extra == "doc"
 Requires-Dist: mkdocs ; extra == "doc"
 Requires-Dist: mkdocs-material ; extra == "doc"
 Requires-Dist: mkdocstrings[python]>=0.18 ; extra == "doc"
 Requires-Dist: mkdocs-exclude ; extra == "doc"
-Requires-Dist: black ; extra == "lint"
-Requires-Dist: isort ; extra == "lint"
-Requires-Dist: mypy ; extra == "lint"
-Requires-Dist: reuse ; extra == "lint"
-Requires-Dist: ruff ; extra == "lint"
-Requires-Dist: tomli-w ; extra == "lint"
-Requires-Dist: types-requests ; extra == "lint"
-Requires-Dist: argcomplete ; extra == "lint"
-Requires-Dist: typing_extensions ; extra == "lint"
+Requires-Dist: black ; extra == "formatters"
+Requires-Dist: isort ; extra == "formatters"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-mock ; extra == "test"
 Requires-Dist: tomli-w ; extra == "test"
-Project-URL: Changelog, https://fedrq.gtmx.me/Changelog
+Requires-Dist: mypy ; extra == "typing"
+Requires-Dist: types-requests ; extra == "typing"
+Requires-Dist: argcomplete ; extra == "typing"
+Requires-Dist: typing_extensions ; extra == "typing"
+Requires-Dist: tomli-w ; extra == "typing"
+Project-URL: Changelog, https://fedrq.gtmx.me/News
 Project-URL: Homepage, https://fedrq.gtmx.me
 Project-URL: Mailing List, https://lists.sr.ht/~gotmax23/fedrq
 Project-URL: Source, https://git.sr.ht/~gotmax23/fedrq
+Provides-Extra: codeqa
 Provides-Extra: dev
 Provides-Extra: doc
-Provides-Extra: lint
+Provides-Extra: formatters
 Provides-Extra: test
+Provides-Extra: typing
 
 <!--
 SPDX-FileCopyrightText: 2022 Maxwell G <gotmax@e.email>
 SPDX-License-Identifier: GPL-2.0-or-later
 -->
 
 # fedrq
```

