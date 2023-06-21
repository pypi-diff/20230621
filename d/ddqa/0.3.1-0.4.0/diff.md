# Comparing `tmp/ddqa-0.3.1.tar.gz` & `tmp/ddqa-0.4.0.tar.gz`

## Comparing `ddqa-0.3.1.tar` & `ddqa-0.4.0.tar`

### file list

```diff
@@ -1,130 +1,131 @@
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ddqa-0.3.1/.gitattributes
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 ddqa-0.3.1/.linkcheckerrc
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 ddqa-0.3.1/HISTORY.md
--rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 ddqa-0.3.1/mkdocs.yml
--rw-r--r--   0        0        0     2821 2020-02-02 00:00:00.000000 ddqa-0.3.1/pyoxidizer.bzl
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 ddqa-0.3.1/.github/dependabot.yml
--rw-r--r--   0        0        0    12900 2020-02-02 00:00:00.000000 ddqa-0.3.1/.github/workflows/build.yml
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 ddqa-0.3.1/.github/workflows/docs.yml
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 ddqa-0.3.1/.github/workflows/publish-docs.yml
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 ddqa-0.3.1/.github/workflows/test.yml
--rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/index.md
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/install.md
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/.snippets/abbrs.txt
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/.snippets/links.txt
--rw-r--r--   0        0        0     4706 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/actions/create.md
--rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/actions/status.md
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/assets/css/custom.css
--rw-r--r--   0        0        0    15039 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/assets/images/creation-screen-candidate-assignments.png
--rw-r--r--   0        0        0    94623 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/assets/images/creation-screen-candidate-description.png
--rw-r--r--   0        0        0     7207 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/assets/images/creation-screen-candidate-pr-labels.png
--rw-r--r--   0        0        0     6464 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/assets/images/creation-screen-candidate-title.png
--rw-r--r--   0        0        0    77999 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/assets/images/creation-screen-candidates.png
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/assets/images/creation-screen-exit.png
--rw-r--r--   0        0        0   207825 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/assets/images/creation-screen-full.png
--rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/assets/images/creation-screen-items.png
--rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/assets/images/creation-screen-progress.png
--rw-r--r--   0        0        0     3824 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/assets/images/creation-screen-queue.png
--rw-r--r--   0        0        0     5639 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/assets/images/creation-screen-results.png
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/assets/images/creation-screen-transition.png
--rw-r--r--   0        0        0    40436 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/assets/images/favicon.ico
--rw-r--r--   0        0        0    43005 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/assets/images/github-token1.png
--rw-r--r--   0        0        0    38694 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/assets/images/github-token2.png
--rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/assets/images/logo.svg
--rw-r--r--   0        0        0   177330 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/assets/images/screen-config.png
--rw-r--r--   0        0        0     5341 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/assets/images/status-screen-filters.png
--rw-r--r--   0        0        0   285123 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/assets/images/status-screen-full.png
--rw-r--r--   0        0        0   253690 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/assets/images/status-screen-issues.png
--rw-r--r--   0        0        0     5262 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/assets/images/status-screen-metadata.png
--rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/assets/images/status-screen-progress.png
--rw-r--r--   0        0        0    10824 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/assets/images/status-screen-qa-status.png
--rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/config/repo.md
--rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/config/user.md
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/__init__.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/__main__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/py.typed
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/app/__init__.py
--rw-r--r--   0        0        0     6606 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/app/core.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/app/style.py
--rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/cli/__init__.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/cli/config/__init__.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/cli/config/edit.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/cli/config/explore.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/cli/config/find.py
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/cli/config/restore.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/cli/config/show.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/cli/create/__init__.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/cli/status/__init__.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/cli/sync/__init__.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/config/__init__.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/config/constants.py
--rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/config/core.py
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/config/file.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/config/utils.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/data/__init__.py
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/data/logo.png
--rw-r--r--   0        0        0   345099 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/data/shame.png
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/models/__init__.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/models/github.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/models/jira.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/models/config/__init__.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/models/config/app.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/models/config/auth.py
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/models/config/repo.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/models/config/team.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/screens/__init__.py
--rw-r--r--   0        0        0     7782 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/screens/configure.py
--rw-r--r--   0        0        0    15712 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/screens/create.py
--rw-r--r--   0        0        0    17067 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/screens/status.py
--rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/screens/sync.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/utils/__init__.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/utils/ci.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/utils/errors.py
--rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/utils/fs.py
--rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/utils/git.py
--rw-r--r--   0        0        0     9133 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/utils/github.py
--rw-r--r--   0        0        0    11019 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/utils/jira.py
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/utils/network.py
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/utils/structures.py
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/utils/time.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/utils/widgets.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/widgets/__init__.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/widgets/input.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/widgets/layout.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/widgets/static.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/__init__.py
--rw-r--r--   0        0        0     5132 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/conftest.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/cli/__init__.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/cli/config/__init__.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/cli/config/test_edit.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/cli/config/test_explore.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/cli/config/test_find.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/cli/config/test_restore.py
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/cli/config/test_show.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/cli/create/__init__.py
--rw-r--r--   0        0        0     3575 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/cli/create/test_create.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/cli/status/__init__.py
--rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/cli/status/test_status.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/cli/sync/__init__.py
--rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/cli/sync/test_sync.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/helpers/__init__.py
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/helpers/api.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/screens/__init__.py
--rw-r--r--   0        0        0    23170 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/screens/test_configure.py
--rw-r--r--   0        0        0    34995 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/screens/test_create.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/screens/test_status.py
--rw-r--r--   0        0        0     7905 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/screens/test_sync.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/utils/__init__.py
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/utils/test_fs.py
--rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/utils/test_git.py
--rw-r--r--   0        0        0    22924 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/utils/test_github.py
--rw-r--r--   0        0        0    28668 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/utils/test_jira.py
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/utils/test_structures.py
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/utils/test_time.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 ddqa-0.3.1/.gitignore
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ddqa-0.3.1/LICENSE.txt
--rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 ddqa-0.3.1/README.md
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 ddqa-0.3.1/hatch.toml
--rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 ddqa-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     3615 2020-02-02 00:00:00.000000 ddqa-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ddqa-0.4.0/.gitattributes
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 ddqa-0.4.0/.linkcheckerrc
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 ddqa-0.4.0/HISTORY.md
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 ddqa-0.4.0/README.md
+-rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 ddqa-0.4.0/mkdocs.yml
+-rw-r--r--   0        0        0     2821 2020-02-02 00:00:00.000000 ddqa-0.4.0/pyoxidizer.bzl
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 ddqa-0.4.0/.github/dependabot.yml
+-rw-r--r--   0        0        0    12882 2020-02-02 00:00:00.000000 ddqa-0.4.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 ddqa-0.4.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 ddqa-0.4.0/.github/workflows/publish-docs.yml
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 ddqa-0.4.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 ddqa-0.4.0/docs/index.md
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 ddqa-0.4.0/docs/install.md
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 ddqa-0.4.0/docs/.snippets/abbrs.txt
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ddqa-0.4.0/docs/.snippets/links.txt
+-rw-r--r--   0        0        0     4706 2020-02-02 00:00:00.000000 ddqa-0.4.0/docs/actions/create.md
+-rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 ddqa-0.4.0/docs/actions/status.md
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 ddqa-0.4.0/docs/assets/css/custom.css
+-rw-r--r--   0        0        0    15039 2020-02-02 00:00:00.000000 ddqa-0.4.0/docs/assets/images/creation-screen-candidate-assignments.png
+-rw-r--r--   0        0        0    94623 2020-02-02 00:00:00.000000 ddqa-0.4.0/docs/assets/images/creation-screen-candidate-description.png
+-rw-r--r--   0        0        0     7207 2020-02-02 00:00:00.000000 ddqa-0.4.0/docs/assets/images/creation-screen-candidate-pr-labels.png
+-rw-r--r--   0        0        0     6464 2020-02-02 00:00:00.000000 ddqa-0.4.0/docs/assets/images/creation-screen-candidate-title.png
+-rw-r--r--   0        0        0    77999 2020-02-02 00:00:00.000000 ddqa-0.4.0/docs/assets/images/creation-screen-candidates.png
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 ddqa-0.4.0/docs/assets/images/creation-screen-exit.png
+-rw-r--r--   0        0        0   207825 2020-02-02 00:00:00.000000 ddqa-0.4.0/docs/assets/images/creation-screen-full.png
+-rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 ddqa-0.4.0/docs/assets/images/creation-screen-items.png
+-rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 ddqa-0.4.0/docs/assets/images/creation-screen-progress.png
+-rw-r--r--   0        0        0     3824 2020-02-02 00:00:00.000000 ddqa-0.4.0/docs/assets/images/creation-screen-queue.png
+-rw-r--r--   0        0        0     5639 2020-02-02 00:00:00.000000 ddqa-0.4.0/docs/assets/images/creation-screen-results.png
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 ddqa-0.4.0/docs/assets/images/creation-screen-transition.png
+-rw-r--r--   0        0        0    40436 2020-02-02 00:00:00.000000 ddqa-0.4.0/docs/assets/images/favicon.ico
+-rw-r--r--   0        0        0    43005 2020-02-02 00:00:00.000000 ddqa-0.4.0/docs/assets/images/github-token1.png
+-rw-r--r--   0        0        0    38694 2020-02-02 00:00:00.000000 ddqa-0.4.0/docs/assets/images/github-token2.png
+-rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 ddqa-0.4.0/docs/assets/images/logo.svg
+-rw-r--r--   0        0        0   177330 2020-02-02 00:00:00.000000 ddqa-0.4.0/docs/assets/images/screen-config.png
+-rw-r--r--   0        0        0     5341 2020-02-02 00:00:00.000000 ddqa-0.4.0/docs/assets/images/status-screen-filters.png
+-rw-r--r--   0        0        0   285123 2020-02-02 00:00:00.000000 ddqa-0.4.0/docs/assets/images/status-screen-full.png
+-rw-r--r--   0        0        0   253690 2020-02-02 00:00:00.000000 ddqa-0.4.0/docs/assets/images/status-screen-issues.png
+-rw-r--r--   0        0        0     5262 2020-02-02 00:00:00.000000 ddqa-0.4.0/docs/assets/images/status-screen-metadata.png
+-rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 ddqa-0.4.0/docs/assets/images/status-screen-progress.png
+-rw-r--r--   0        0        0    10824 2020-02-02 00:00:00.000000 ddqa-0.4.0/docs/assets/images/status-screen-qa-status.png
+-rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 ddqa-0.4.0/docs/config/repo.md
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 ddqa-0.4.0/docs/config/sync.md
+-rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 ddqa-0.4.0/docs/config/user.md
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/__init__.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/__main__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/py.typed
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/app/__init__.py
+-rw-r--r--   0        0        0     6606 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/app/core.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/app/style.py
+-rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/cli/__init__.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/cli/config/__init__.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/cli/config/edit.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/cli/config/explore.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/cli/config/find.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/cli/config/restore.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/cli/config/show.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/cli/create/__init__.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/cli/status/__init__.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/cli/sync/__init__.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/config/__init__.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/config/constants.py
+-rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/config/core.py
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/config/file.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/config/utils.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/data/__init__.py
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/data/logo.png
+-rw-r--r--   0        0        0   345099 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/data/shame.png
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/models/__init__.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/models/github.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/models/jira.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/models/config/__init__.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/models/config/app.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/models/config/auth.py
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/models/config/repo.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/models/config/team.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/screens/__init__.py
+-rw-r--r--   0        0        0     7782 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/screens/configure.py
+-rw-r--r--   0        0        0    15712 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/screens/create.py
+-rw-r--r--   0        0        0    17067 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/screens/status.py
+-rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/screens/sync.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/utils/__init__.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/utils/ci.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/utils/errors.py
+-rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/utils/fs.py
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/utils/git.py
+-rw-r--r--   0        0        0     9133 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/utils/github.py
+-rw-r--r--   0        0        0    11019 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/utils/jira.py
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/utils/network.py
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/utils/structures.py
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/utils/time.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/utils/widgets.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/widgets/__init__.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/widgets/input.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/widgets/layout.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 ddqa-0.4.0/src/ddqa/widgets/static.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     5132 2020-02-02 00:00:00.000000 ddqa-0.4.0/tests/conftest.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.4.0/tests/cli/__init__.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.4.0/tests/cli/config/__init__.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 ddqa-0.4.0/tests/cli/config/test_edit.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 ddqa-0.4.0/tests/cli/config/test_explore.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 ddqa-0.4.0/tests/cli/config/test_find.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 ddqa-0.4.0/tests/cli/config/test_restore.py
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 ddqa-0.4.0/tests/cli/config/test_show.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.4.0/tests/cli/create/__init__.py
+-rw-r--r--   0        0        0     3575 2020-02-02 00:00:00.000000 ddqa-0.4.0/tests/cli/create/test_create.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.4.0/tests/cli/status/__init__.py
+-rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 ddqa-0.4.0/tests/cli/status/test_status.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.4.0/tests/cli/sync/__init__.py
+-rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 ddqa-0.4.0/tests/cli/sync/test_sync.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.4.0/tests/helpers/__init__.py
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 ddqa-0.4.0/tests/helpers/api.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.4.0/tests/screens/__init__.py
+-rw-r--r--   0        0        0    23170 2020-02-02 00:00:00.000000 ddqa-0.4.0/tests/screens/test_configure.py
+-rw-r--r--   0        0        0    34995 2020-02-02 00:00:00.000000 ddqa-0.4.0/tests/screens/test_create.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.4.0/tests/screens/test_status.py
+-rw-r--r--   0        0        0     7905 2020-02-02 00:00:00.000000 ddqa-0.4.0/tests/screens/test_sync.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.4.0/tests/utils/__init__.py
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 ddqa-0.4.0/tests/utils/test_fs.py
+-rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 ddqa-0.4.0/tests/utils/test_git.py
+-rw-r--r--   0        0        0    22924 2020-02-02 00:00:00.000000 ddqa-0.4.0/tests/utils/test_github.py
+-rw-r--r--   0        0        0    28668 2020-02-02 00:00:00.000000 ddqa-0.4.0/tests/utils/test_jira.py
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 ddqa-0.4.0/tests/utils/test_structures.py
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 ddqa-0.4.0/tests/utils/test_time.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 ddqa-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ddqa-0.4.0/LICENSE.txt
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 ddqa-0.4.0/hatch.toml
+-rw-r--r--   0        0        0     3275 2020-02-02 00:00:00.000000 ddqa-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3737 2020-02-02 00:00:00.000000 ddqa-0.4.0/PKG-INFO
```

### Comparing `ddqa-0.3.1/HISTORY.md` & `ddqa-0.4.0/HISTORY.md`

 * *Files 26% similar despite different names*

```diff
@@ -4,14 +4,21 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## Unreleased
 
+## 0.4.0 - 2023-06-21
+
+***Added:***
+
+- Upgrade PyApp to 0.9.0
+- Build for PowerPC
+
 ## 0.3.1 - 2023-06-02
 
 ***Fixed:***
 
 - Fix race condition when prematurely creating issues
 
 ## 0.3.0 - 2023-05-24
```

### Comparing `ddqa-0.3.1/mkdocs.yml` & `ddqa-0.4.0/mkdocs.yml`

 * *Files 8% similar despite different names*

```diff
@@ -27,36 +27,41 @@
         name: Switch to light mode
     - media: "(prefers-color-scheme: light)"
       scheme: default
       toggle:
         icon: material/weather-sunny
         name: Switch to dark mode
   features:
-    - navigation.sections
+    - content.action.edit
+    - content.code.copy
     - navigation.expand
+    - navigation.footer
     - navigation.instant
+    - navigation.sections
 
 nav:
   - About: index.md
   - Installation: install.md
   - Configuration:
     - User: config/user.md
     - Repository: config/repo.md
+    - Synchronization: config/sync.md
   - Actions:
     - Create items: actions/create.md
     - View dashboard: actions/status.md
 
 plugins:
   # Built-in
   search: {}
   # Extra
   glightbox: {}
   minify:
     minify_html: true
   git-revision-date-localized:
+    strict: false
     type: date
 
 markdown_extensions:
   # Built-in
   - markdown.extensions.abbr:
   - markdown.extensions.admonition:
   - markdown.extensions.attr_list:
@@ -119,8 +124,8 @@
       link: https://github.com/DataDog
     - icon: fontawesome/brands/twitter
       link: https://twitter.com/datadoghq
     - icon: fontawesome/brands/instagram
       link: https://www.instagram.com/datadoghq
 extra_css:
   - assets/css/custom.css
-  - https://cdn.jsdelivr.net/gh/tonsky/FiraCode@5.2/distr/fira_code.css
+  - https://cdn.jsdelivr.net/npm/firacode@6.2.0/distr/fira_code.css
```

### Comparing `ddqa-0.3.1/pyoxidizer.bzl` & `ddqa-0.4.0/pyoxidizer.bzl`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/.github/workflows/build.yml` & `ddqa-0.4.0/.github/workflows/build.yml`

 * *Files 4% similar despite different names*

```diff
@@ -65,14 +65,17 @@
           cross: true
         - target: x86_64-unknown-linux-musl
           os: ubuntu-22.04
           cross: true
         - target: i686-unknown-linux-gnu
           os: ubuntu-22.04
           cross: true
+        - target: powerpc64le-unknown-linux-gnu
+          os: ubuntu-22.04
+          cross: true
         # Windows
         - target: x86_64-pc-windows-msvc
           os: windows-2022
         - target: i686-pc-windows-msvc
           os: windows-2022
         # macOS
         - target: aarch64-apple-darwin
@@ -83,15 +86,15 @@
     outputs:
       version: ${{ steps.version.outputs.version }}
 
     env:
       CARGO: cargo
       CARGO_BUILD_TARGET: ${{ matrix.job.target }}
       PYAPP_REPO: pyapp
-      PYAPP_VERSION: "0.7.0"
+      PYAPP_VERSION: "0.9.0"
 
     steps:
     - name: Checkout code
       uses: actions/checkout@v3
       with:
         fetch-depth: 0
 
@@ -121,14 +124,21 @@
       with:
         tool: cross
 
     - name: Configure cross compiling
       if: matrix.job.cross
       run: echo "CARGO=cross" >> $GITHUB_ENV
 
+    - name: Configure target
+      run: |-
+        config_file="$PYAPP_REPO/.cargo/config_${{ matrix.job.target }}.toml"
+        if [[ -f "$config_file" ]]; then
+          mv "$config_file" "$PYAPP_REPO/.cargo/config.toml"
+        fi
+
     - name: Download Python artifacts
       if: ${{ !startsWith(github.event.ref, 'refs/tags') }}
       uses: actions/download-artifact@v3
       with:
         name: python-artifacts
         path: dist
 
@@ -189,18 +199,15 @@
       with:
         name: standalone
         path: packaging/*
         if-no-files-found: error
 
   windows-packaging:
     name: Build Windows installers
-    if: >-
-      github.event_name == 'push'
-      &&
-      (github.ref == 'refs/heads/master' || startsWith(github.event.ref, 'refs/tags'))
+    if: github.event_name == 'push' || github.event.pull_request.head.repo.full_name == github.repository
     needs: binaries
     runs-on: windows-2022
 
     env:
       VERSION: ${{ needs.binaries.outputs.version }}
 
     steps:
@@ -262,18 +269,15 @@
       uses: actions/upload-artifact@v3
       with:
         name: installers
         path: installers/*
 
   macos-packaging:
     name: Build macOS installer and sign/notarize artifacts
-    if: >-
-      github.event_name == 'push'
-      &&
-      (github.ref == 'refs/heads/master' || startsWith(github.event.ref, 'refs/tags'))
+    if: github.event_name == 'push' || github.event.pull_request.head.repo.full_name == github.repository
     needs: binaries
     runs-on: macos-12
 
     env:
       VERSION: ${{ needs.binaries.outputs.version }}
 
     steps:
@@ -288,21 +292,15 @@
     - name: Install PyOxidizer ${{ env.PYOXIDIZER_VERSION }}
       run: pip install pyoxidizer==${{ env.PYOXIDIZER_VERSION }}
 
     - name: Install create-dmg
       run: brew install create-dmg
 
     - name: Install rcodesign
-      env:
-        ARCHIVE_NAME: "apple-codesign-0.22.0-x86_64-apple-darwin"
-      run: >-
-        curl -L
-        "https://github.com/indygreg/apple-platform-rs/releases/download/apple-codesign%2F0.22.0/$ARCHIVE_NAME.tar.gz"
-        |
-        tar --strip-components=1 -xzf - -C /usr/local/bin "$ARCHIVE_NAME/rcodesign"
+      run: cargo install apple-codesign
 
     - name: Download staged binaries
       uses: actions/download-artifact@v3
       with:
         name: staged-${{ runner.os }}
         path: archives
```

### Comparing `ddqa-0.3.1/.github/workflows/docs.yml` & `ddqa-0.4.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/.github/workflows/publish-docs.yml` & `ddqa-0.4.0/.github/workflows/publish-docs.yml`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/.github/workflows/test.yml` & `ddqa-0.4.0/.github/workflows/test.yml`

 * *Files 9% similar despite different names*

```diff
@@ -25,14 +25,16 @@
       fail-fast: false
       matrix:
         os: [ubuntu-latest, windows-latest, macos-latest]
         python-version: ['3.11']
 
     steps:
     - uses: actions/checkout@v3
+      with:
+        fetch-depth: 0
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
 
     - name: Install Hatch
```

### Comparing `ddqa-0.3.1/docs/index.md` & `ddqa-0.4.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/docs/install.md` & `ddqa-0.4.0/docs/install.md`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/docs/actions/create.md` & `ddqa-0.4.0/docs/actions/create.md`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/docs/actions/status.md` & `ddqa-0.4.0/docs/actions/status.md`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/docs/assets/css/custom.css` & `ddqa-0.4.0/docs/assets/css/custom.css`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-:root {
+:root > * {
   /* https://www.datadoghq.com/about/resources/#datadog-purple */
   --md-primary-fg-color: #632CA6;
   --md-primary-fg-color--dark: #632CA6;
 
   /* https://github.com/squidfunk/mkdocs-material/blob/9.1.2/src/assets/stylesheets/palette/_primary.scss#L34 */
   --md-primary-fg-color--light: #9574CD;
```

### Comparing `ddqa-0.3.1/docs/assets/images/creation-screen-candidate-assignments.png` & `ddqa-0.4.0/docs/assets/images/creation-screen-candidate-assignments.png`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/docs/assets/images/creation-screen-candidate-description.png` & `ddqa-0.4.0/docs/assets/images/creation-screen-candidate-description.png`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/docs/assets/images/creation-screen-candidate-pr-labels.png` & `ddqa-0.4.0/docs/assets/images/creation-screen-candidate-pr-labels.png`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/docs/assets/images/creation-screen-candidate-title.png` & `ddqa-0.4.0/docs/assets/images/creation-screen-candidate-title.png`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/docs/assets/images/creation-screen-candidates.png` & `ddqa-0.4.0/docs/assets/images/creation-screen-candidates.png`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/docs/assets/images/creation-screen-exit.png` & `ddqa-0.4.0/docs/assets/images/creation-screen-exit.png`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/docs/assets/images/creation-screen-full.png` & `ddqa-0.4.0/docs/assets/images/creation-screen-full.png`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/docs/assets/images/creation-screen-items.png` & `ddqa-0.4.0/docs/assets/images/creation-screen-items.png`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/docs/assets/images/creation-screen-progress.png` & `ddqa-0.4.0/docs/assets/images/creation-screen-progress.png`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/docs/assets/images/creation-screen-queue.png` & `ddqa-0.4.0/docs/assets/images/creation-screen-queue.png`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/docs/assets/images/creation-screen-results.png` & `ddqa-0.4.0/docs/assets/images/creation-screen-results.png`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/docs/assets/images/creation-screen-transition.png` & `ddqa-0.4.0/docs/assets/images/creation-screen-transition.png`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/docs/assets/images/favicon.ico` & `ddqa-0.4.0/docs/assets/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/docs/assets/images/github-token1.png` & `ddqa-0.4.0/docs/assets/images/github-token1.png`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/docs/assets/images/github-token2.png` & `ddqa-0.4.0/docs/assets/images/github-token2.png`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/docs/assets/images/logo.svg` & `ddqa-0.4.0/docs/assets/images/logo.svg`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/docs/assets/images/screen-config.png` & `ddqa-0.4.0/docs/assets/images/screen-config.png`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/docs/assets/images/status-screen-filters.png` & `ddqa-0.4.0/docs/assets/images/status-screen-filters.png`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/docs/assets/images/status-screen-full.png` & `ddqa-0.4.0/docs/assets/images/status-screen-full.png`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/docs/assets/images/status-screen-issues.png` & `ddqa-0.4.0/docs/assets/images/status-screen-issues.png`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/docs/assets/images/status-screen-metadata.png` & `ddqa-0.4.0/docs/assets/images/status-screen-metadata.png`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/docs/assets/images/status-screen-progress.png` & `ddqa-0.4.0/docs/assets/images/status-screen-progress.png`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/docs/assets/images/status-screen-qa-status.png` & `ddqa-0.4.0/docs/assets/images/status-screen-qa-status.png`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/docs/config/repo.md` & `ddqa-0.4.0/docs/config/repo.md`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/docs/config/user.md` & `ddqa-0.4.0/docs/config/user.md`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/src/ddqa/app/core.py` & `ddqa-0.4.0/src/ddqa/app/core.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/src/ddqa/cli/__init__.py` & `ddqa-0.4.0/src/ddqa/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/src/ddqa/cli/config/__init__.py` & `ddqa-0.4.0/src/ddqa/cli/config/__init__.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/src/ddqa/cli/config/show.py` & `ddqa-0.4.0/src/ddqa/cli/config/show.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/src/ddqa/cli/create/__init__.py` & `ddqa-0.4.0/src/ddqa/cli/create/__init__.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/src/ddqa/cli/status/__init__.py` & `ddqa-0.4.0/src/ddqa/cli/status/__init__.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/src/ddqa/config/core.py` & `ddqa-0.4.0/src/ddqa/config/core.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/src/ddqa/config/file.py` & `ddqa-0.4.0/src/ddqa/config/file.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/src/ddqa/data/logo.png` & `ddqa-0.4.0/src/ddqa/data/logo.png`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/src/ddqa/data/shame.png` & `ddqa-0.4.0/src/ddqa/data/shame.png`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/src/ddqa/models/github.py` & `ddqa-0.4.0/src/ddqa/models/github.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/src/ddqa/models/jira.py` & `ddqa-0.4.0/src/ddqa/models/jira.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/src/ddqa/models/config/repo.py` & `ddqa-0.4.0/src/ddqa/models/config/repo.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/src/ddqa/screens/configure.py` & `ddqa-0.4.0/src/ddqa/screens/configure.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/src/ddqa/screens/create.py` & `ddqa-0.4.0/src/ddqa/screens/create.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/src/ddqa/screens/status.py` & `ddqa-0.4.0/src/ddqa/screens/status.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/src/ddqa/screens/sync.py` & `ddqa-0.4.0/src/ddqa/screens/sync.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/src/ddqa/utils/fs.py` & `ddqa-0.4.0/src/ddqa/utils/fs.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/src/ddqa/utils/git.py` & `ddqa-0.4.0/src/ddqa/utils/git.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/src/ddqa/utils/github.py` & `ddqa-0.4.0/src/ddqa/utils/github.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/src/ddqa/utils/jira.py` & `ddqa-0.4.0/src/ddqa/utils/jira.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/src/ddqa/utils/network.py` & `ddqa-0.4.0/src/ddqa/utils/network.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/src/ddqa/utils/structures.py` & `ddqa-0.4.0/src/ddqa/utils/structures.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/src/ddqa/utils/time.py` & `ddqa-0.4.0/src/ddqa/utils/time.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/src/ddqa/widgets/input.py` & `ddqa-0.4.0/src/ddqa/widgets/input.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/src/ddqa/widgets/layout.py` & `ddqa-0.4.0/src/ddqa/widgets/layout.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/src/ddqa/widgets/static.py` & `ddqa-0.4.0/src/ddqa/widgets/static.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/tests/conftest.py` & `ddqa-0.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/tests/cli/config/test_restore.py` & `ddqa-0.4.0/tests/cli/config/test_restore.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/tests/cli/config/test_show.py` & `ddqa-0.4.0/tests/cli/config/test_show.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/tests/cli/create/test_create.py` & `ddqa-0.4.0/tests/cli/create/test_create.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/tests/cli/status/test_status.py` & `ddqa-0.4.0/tests/cli/status/test_status.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/tests/cli/sync/test_sync.py` & `ddqa-0.4.0/tests/cli/sync/test_sync.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/tests/helpers/api.py` & `ddqa-0.4.0/tests/helpers/api.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/tests/screens/test_configure.py` & `ddqa-0.4.0/tests/screens/test_configure.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/tests/screens/test_create.py` & `ddqa-0.4.0/tests/screens/test_create.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/tests/screens/test_sync.py` & `ddqa-0.4.0/tests/screens/test_sync.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/tests/utils/test_fs.py` & `ddqa-0.4.0/tests/utils/test_fs.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/tests/utils/test_git.py` & `ddqa-0.4.0/tests/utils/test_git.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/tests/utils/test_github.py` & `ddqa-0.4.0/tests/utils/test_github.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/tests/utils/test_jira.py` & `ddqa-0.4.0/tests/utils/test_jira.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/tests/utils/test_structures.py` & `ddqa-0.4.0/tests/utils/test_structures.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/tests/utils/test_time.py` & `ddqa-0.4.0/tests/utils/test_time.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/LICENSE.txt` & `ddqa-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.1/README.md` & `ddqa-0.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Datadog QA
 
+![example screenshot](docs/assets/images/creation-screen-full.png)
+
 | | |
 | --- | --- |
 | CI/CD | [![CI - Test](https://github.com/DataDog/ddqa/actions/workflows/test.yml/badge.svg)](https://github.com/DataDog/ddqa/actions/workflows/test.yml) [![CD - Build](https://github.com/DataDog/ddqa/actions/workflows/build.yml/badge.svg)](https://github.com/DataDog/ddqa/actions/workflows/build.yml) |
 | Docs | [![Docs - Build](https://github.com/DataDog/ddqa/actions/workflows/docs.yml/badge.svg)](https://github.com/DataDog/ddqa/actions/workflows/docs.yml) [![Docs - Publish](https://github.com/DataDog/ddqa/actions/workflows/publish-docs.yml/badge.svg)](https://github.com/DataDog/ddqa/actions/workflows/publish-docs.yml) |
 | Package | [![PyPI - Version](https://img.shields.io/pypi/v/ddqa.svg?logo=pypi&label=PyPI&logoColor=gold)](https://pypi.org/project/ddqa/) [![PyPI - Downloads](https://img.shields.io/pypi/dm/ddqa.svg?color=blue&label=Downloads&logo=pypi&logoColor=gold)](https://pypi.org/project/ddqa/) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ddqa.svg?logo=python&label=Python&logoColor=gold)](https://pypi.org/project/ddqa/) |
 | Meta | [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch) [![linting - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v0.json)](https://github.com/charliermarsh/ruff) [![code style - Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://github.com/python/mypy) [![License - MIT](https://img.shields.io/badge/license-MIT-9400d3.svg)](https://spdx.org/licenses/) |
```

### Comparing `ddqa-0.3.1/hatch.toml` & `ddqa-0.4.0/hatch.toml`

 * *Files 6% similar despite different names*

```diff
@@ -44,24 +44,24 @@
   "style",
   "typing",
 ]
 
 [envs.docs]
 detached = true
 dependencies = [
-  "mkdocs~=1.4.0",
-  "mkdocs-material~=8.5.6",
+  "mkdocs~=1.4.3",
+  "mkdocs-material~=9.1.16",
   # Plugins
-  "mkdocs-minify-plugin~=0.5.0",
-  "mkdocs-git-revision-date-localized-plugin~=1.1.0",
-  "mkdocs-glightbox~=0.3.0",
+  "mkdocs-minify-plugin~=0.6.4",
+  "mkdocs-git-revision-date-localized-plugin~=1.2.0",
+  "mkdocs-glightbox~=0.3.4",
   # Extensions
-  "pymdown-extensions~=9.6.0",
+  "pymdown-extensions~=10.0.1",
   # Necessary for syntax highlighting in code blocks
-  "pygments~=2.13.0",
+  "pygments~=2.15.1",
   # Validation
   # https://github.com/linkchecker/linkchecker/pull/669#issuecomment-1267236287
   "linkchecker @ git+https://github.com/linkchecker/linkchecker.git@d9265bb71c2054bf57b8c5734a4825d62505c779",
 ]
 [envs.docs.env-vars]
 SOURCE_DATE_EPOCH = "1580601600"
 PYTHONUNBUFFERED = "1"
```

### Comparing `ddqa-0.3.1/pyproject.toml` & `ddqa-0.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 [build-system]
-requires = ["hatchling>=1.17.0", "hatch-vcs"]
+requires = ["hatchling>=1.17.0", "hatch-vcs", "hatch-fancy-pypi-readme"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ddqa"
-dynamic = ["version"]
+dynamic = ["version", "readme"]
 description = "Datadog's QA manager for releases of GitHub repositories"
-readme = "README.md"
 requires-python = ">=3.11"
 license = "MIT"
 keywords = [
   "datadog",
   "qa",
   "testing",
   "tooling",
@@ -46,14 +45,24 @@
 [tool.hatch.version]
 source = "vcs"
 raw-options = { version_scheme = "python-simplified-semver", local_scheme = "no-local-version" }
 
 [tool.hatch.build.hooks.vcs]
 version-file = "src/ddqa/_version.py"
 
+[tool.hatch.metadata.hooks.fancy-pypi-readme]
+content-type = "text/markdown"
+fragments = [
+  { path = "README.md" },
+]
+
+[[tool.hatch.metadata.hooks.fancy-pypi-readme.substitutions]]
+pattern = '(docs/assets/images/.*?)'
+replacement = 'https://raw.githubusercontent.com/DataDog/ddqa/master/\1'
+
 [tool.black]
 target-version = ["py311"]
 line-length = 120
 skip-string-normalization = true
 
 [tool.mypy]
 disallow_untyped_defs = false
```

### Comparing `ddqa-0.3.1/PKG-INFO` & `ddqa-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddqa
-Version: 0.3.1
+Version: 0.4.0
 Summary: Datadog's QA manager for releases of GitHub repositories
 Project-URL: Source, https://github.com/DataDog/ddqa
 Author-email: "Datadog, Inc." <dev@datadoghq.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Keywords: datadog,qa,testing,tooling
 Classifier: Development Status :: 4 - Beta
@@ -22,14 +22,16 @@
 Requires-Dist: textual-autocomplete>=2.1.0b0
 Requires-Dist: textual~=0.20.1
 Requires-Dist: tomli-w
 Description-Content-Type: text/markdown
 
 # Datadog QA
 
+![example screenshot](https://raw.githubusercontent.com/DataDog/ddqa/master/docs/assets/images/creation-screen-full.png)
+
 | | |
 | --- | --- |
 | CI/CD | [![CI - Test](https://github.com/DataDog/ddqa/actions/workflows/test.yml/badge.svg)](https://github.com/DataDog/ddqa/actions/workflows/test.yml) [![CD - Build](https://github.com/DataDog/ddqa/actions/workflows/build.yml/badge.svg)](https://github.com/DataDog/ddqa/actions/workflows/build.yml) |
 | Docs | [![Docs - Build](https://github.com/DataDog/ddqa/actions/workflows/docs.yml/badge.svg)](https://github.com/DataDog/ddqa/actions/workflows/docs.yml) [![Docs - Publish](https://github.com/DataDog/ddqa/actions/workflows/publish-docs.yml/badge.svg)](https://github.com/DataDog/ddqa/actions/workflows/publish-docs.yml) |
 | Package | [![PyPI - Version](https://img.shields.io/pypi/v/ddqa.svg?logo=pypi&label=PyPI&logoColor=gold)](https://pypi.org/project/ddqa/) [![PyPI - Downloads](https://img.shields.io/pypi/dm/ddqa.svg?color=blue&label=Downloads&logo=pypi&logoColor=gold)](https://pypi.org/project/ddqa/) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ddqa.svg?logo=python&label=Python&logoColor=gold)](https://pypi.org/project/ddqa/) |
 | Meta | [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch) [![linting - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v0.json)](https://github.com/charliermarsh/ruff) [![code style - Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://github.com/python/mypy) [![License - MIT](https://img.shields.io/badge/license-MIT-9400d3.svg)](https://spdx.org/licenses/) |
```

