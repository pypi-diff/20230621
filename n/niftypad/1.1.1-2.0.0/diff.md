# Comparing `tmp/niftypad-1.1.1.tar.gz` & `tmp/niftypad-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "niftypad-1.1.1.tar", last modified: Wed Oct  6 21:30:11 2021, max compression
+gzip compressed data, was "niftypad-2.0.0.tar", last modified: Wed Jun 21 00:46:28 2023, max compression
```

## Comparing `niftypad-1.1.1.tar` & `niftypad-2.0.0.tar`

### file list

```diff
@@ -1,49 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-06 21:30:11.336912 niftypad-1.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-06 21:30:11.332912 niftypad-1.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-06 21:30:11.332912 niftypad-1.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2059 2021-10-06 21:29:59.000000 niftypad-1.1.1/.github/workflows/comment-bot.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2880 2021-10-06 21:29:59.000000 niftypad-1.1.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (121)      165 2021-10-06 21:29:59.000000 niftypad-1.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)       65 2021-10-06 21:29:59.000000 niftypad-1.1.1/.mailmap
--rw-r--r--   0 runner    (1001) docker     (121)     1037 2021-10-06 21:29:59.000000 niftypad-1.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-10-06 21:29:59.000000 niftypad-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1430 2021-10-06 21:30:11.336912 niftypad-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       75 2021-10-06 21:29:59.000000 niftypad-1.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-06 21:30:11.336912 niftypad-1.1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     3171 2021-10-06 21:29:59.000000 niftypad-1.1.1/examples/demo_img.py
--rw-r--r--   0 runner    (1001) docker     (121)     2122 2021-10-06 21:29:59.000000 niftypad-1.1.1/examples/demo_img_suvr.py
--rw-r--r--   0 runner    (1001) docker     (121)     2692 2021-10-06 21:29:59.000000 niftypad-1.1.1/examples/demo_tac.py
--rw-r--r--   0 runner    (1001) docker     (121)     2763 2021-10-06 21:29:59.000000 niftypad-1.1.1/examples/dt_fill_gaps_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-06 21:30:11.336912 niftypad-1.1.1/niftypad/
--rw-r--r--   0 runner    (1001) docker     (121)      322 2021-10-06 21:29:59.000000 niftypad-1.1.1/niftypad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       30 2021-10-06 21:29:59.000000 niftypad-1.1.1/niftypad/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-10-06 21:30:10.000000 niftypad-1.1.1/niftypad/_dist_ver.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-06 21:30:11.336912 niftypad-1.1.1/niftypad/api/
--rw-r--r--   0 runner    (1001) docker     (121)     4178 2021-10-06 21:29:59.000000 niftypad-1.1.1/niftypad/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1313 2021-10-06 21:29:59.000000 niftypad-1.1.1/niftypad/api/readers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2345 2021-10-06 21:29:59.000000 niftypad-1.1.1/niftypad/basis.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-06 21:30:11.336912 niftypad-1.1.1/niftypad/image_process/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-06 21:29:59.000000 niftypad-1.1.1/niftypad/image_process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2808 2021-10-06 21:29:59.000000 niftypad-1.1.1/niftypad/image_process/motion_correction.py
--rw-r--r--   0 runner    (1001) docker     (121)     3172 2021-10-06 21:29:59.000000 niftypad-1.1.1/niftypad/image_process/parametric_image.py
--rw-r--r--   0 runner    (1001) docker     (121)     1190 2021-10-06 21:29:59.000000 niftypad-1.1.1/niftypad/image_process/regions.py
--rw-r--r--   0 runner    (1001) docker     (121)     7901 2021-10-06 21:29:59.000000 niftypad-1.1.1/niftypad/image_process/transforms.py
--rw-r--r--   0 runner    (1001) docker     (121)      588 2021-10-06 21:29:59.000000 niftypad-1.1.1/niftypad/kp.py
--rw-r--r--   0 runner    (1001) docker     (121)     3189 2021-10-06 21:29:59.000000 niftypad-1.1.1/niftypad/kt.py
--rw-r--r--   0 runner    (1001) docker     (121)    32154 2021-10-06 21:29:59.000000 niftypad-1.1.1/niftypad/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     3499 2021-10-06 21:29:59.000000 niftypad-1.1.1/niftypad/tac.py
--rw-r--r--   0 runner    (1001) docker     (121)     1530 2021-10-06 21:29:59.000000 niftypad-1.1.1/niftypad/weight.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-06 21:30:11.336912 niftypad-1.1.1/niftypad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1430 2021-10-06 21:30:10.000000 niftypad-1.1.1/niftypad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      913 2021-10-06 21:30:11.000000 niftypad-1.1.1/niftypad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-06 21:30:10.000000 niftypad-1.1.1/niftypad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       48 2021-10-06 21:30:10.000000 niftypad-1.1.1/niftypad.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       83 2021-10-06 21:30:10.000000 niftypad-1.1.1/niftypad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-10-06 21:30:10.000000 niftypad-1.1.1/niftypad.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      191 2021-10-06 21:29:59.000000 niftypad-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     2235 2021-10-06 21:30:11.336912 niftypad-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       58 2021-10-06 21:29:59.000000 niftypad-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-06 21:30:11.336912 niftypad-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-06 21:29:59.000000 niftypad-1.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      319 2021-10-06 21:29:59.000000 niftypad-1.1.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)      106 2021-10-06 21:29:59.000000 niftypad-1.1.1/tests/test_basic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:46:28.714854 niftypad-2.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:46:28.702854 niftypad-2.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:46:28.706854 niftypad-2.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-21 00:46:08.000000 niftypad-2.0.0/.github/workflows/comment-bot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-06-21 00:46:08.000000 niftypad-2.0.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-21 00:46:08.000000 niftypad-2.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-21 00:46:08.000000 niftypad-2.0.0/.mailmap
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-21 00:46:08.000000 niftypad-2.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-21 00:46:08.000000 niftypad-2.0.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-21 00:46:08.000000 niftypad-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-21 00:46:28.714854 niftypad-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-21 00:46:08.000000 niftypad-2.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:46:28.706854 niftypad-2.0.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-06-21 00:46:08.000000 niftypad-2.0.0/examples/demo_img.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-21 00:46:08.000000 niftypad-2.0.0/examples/demo_img_suvr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-21 00:46:08.000000 niftypad-2.0.0/examples/demo_tac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-06-21 00:46:08.000000 niftypad-2.0.0/examples/dt_fill_gaps_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:46:28.706854 niftypad-2.0.0/images/
+-rw-r--r--   0 runner    (1001) docker     (123)  1809454 2023-06-21 00:46:08.000000 niftypad-2.0.0/images/Fig1.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:46:28.710854 niftypad-2.0.0/niftypad/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-21 00:46:08.000000 niftypad-2.0.0/niftypad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-21 00:46:08.000000 niftypad-2.0.0/niftypad/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 00:46:28.000000 niftypad-2.0.0/niftypad/_dist_ver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:46:28.714854 niftypad-2.0.0/niftypad/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-06-21 00:46:08.000000 niftypad-2.0.0/niftypad/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-21 00:46:08.000000 niftypad-2.0.0/niftypad/api/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-06-21 00:46:08.000000 niftypad-2.0.0/niftypad/basis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:46:28.714854 niftypad-2.0.0/niftypad/image_process/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 00:46:08.000000 niftypad-2.0.0/niftypad/image_process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-06-21 00:46:08.000000 niftypad-2.0.0/niftypad/image_process/motion_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-06-21 00:46:08.000000 niftypad-2.0.0/niftypad/image_process/parametric_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-21 00:46:08.000000 niftypad-2.0.0/niftypad/image_process/regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-06-21 00:46:08.000000 niftypad-2.0.0/niftypad/image_process/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-21 00:46:08.000000 niftypad-2.0.0/niftypad/kp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-06-21 00:46:08.000000 niftypad-2.0.0/niftypad/kt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34764 2023-06-21 00:46:08.000000 niftypad-2.0.0/niftypad/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-06-21 00:46:08.000000 niftypad-2.0.0/niftypad/tac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-21 00:46:08.000000 niftypad-2.0.0/niftypad/weight.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:46:28.710854 niftypad-2.0.0/niftypad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-21 00:46:28.000000 niftypad-2.0.0/niftypad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-21 00:46:28.000000 niftypad-2.0.0/niftypad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 00:46:28.000000 niftypad-2.0.0/niftypad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-21 00:46:28.000000 niftypad-2.0.0/niftypad.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-21 00:46:28.000000 niftypad-2.0.0/niftypad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-21 00:46:28.000000 niftypad-2.0.0/niftypad.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-21 00:46:08.000000 niftypad-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 00:46:28.714854 niftypad-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:46:28.714854 niftypad-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 00:46:08.000000 niftypad-2.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-21 00:46:08.000000 niftypad-2.0.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-21 00:46:08.000000 niftypad-2.0.0/tests/test_basic.py
```

### Comparing `niftypad-1.1.1/.github/workflows/comment-bot.yml` & `niftypad-2.0.0/.github/workflows/comment-bot.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 name: Comment Bot
 on:
-  issue_comment:
-    types: [created]
-  pull_request_review_comment:
-    types: [created]
+  issue_comment: {types: [created]}
+  pull_request_review_comment: {types: [created]}
 jobs:
   tag:  # /tag <tagname> <commit>
     if: startsWith(github.event.comment.body, '/tag ')
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: React Seen
-      uses: actions/github-script@v2
+      uses: actions/github-script@v6
       with:
         script: |
-          const perm = await github.repos.getCollaboratorPermissionLevel({
+          const perm = await github.rest.repos.getCollaboratorPermissionLevel({
             owner: context.repo.owner, repo: context.repo.repo,
             username: context.payload.comment.user.login})
           post = (context.eventName == "issue_comment"
-            ? github.reactions.createForIssueComment
-            : github.reactions.createForPullRequestReviewComment)
+            ? github.rest.reactions.createForIssueComment
+            : github.rest.reactions.createForPullRequestReviewComment)
           if (!["admin", "write"].includes(perm.data.permission)){
             post({
               owner: context.repo.owner, repo: context.repo.repo,
               comment_id: context.payload.comment.id, content: "laugh"})
             throw "Permission denied for user " + context.payload.comment.user.login
           }
           post({
@@ -36,17 +34,17 @@
         git -C repo tag $(echo "$BODY" | awk '{print $2" "$3}')
         git -C repo push --tags
         rm -rf repo
       env:
         BODY: ${{ github.event.comment.body }}
         GITHUB_TOKEN: ${{ secrets.GH_TOKEN }}
     - name: React Success
-      uses: actions/github-script@v2
+      uses: actions/github-script@v6
       with:
         script: |
           post = (context.eventName == "issue_comment"
-            ? github.reactions.createForIssueComment
-            : github.reactions.createForPullRequestReviewComment)
+            ? github.rest.reactions.createForIssueComment
+            : github.rest.reactions.createForPullRequestReviewComment)
           post({
             owner: context.repo.owner, repo: context.repo.repo,
             comment_id: context.payload.comment.id, content: "rocket"})
         github-token: ${{ secrets.GH_TOKEN }}
```

### Comparing `niftypad-1.1.1/.github/workflows/test.yml` & `niftypad-2.0.0/.github/workflows/test.yml`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 name: Test
 on: [push, pull_request]
 jobs:
   check:
-    if: github.event_name != 'pull_request' || github.repository_owner != 'AMYPAD'
+    if: github.event_name != 'pull_request' || !contains('OWNER,MEMBER,COLLABORATOR', github.event.pull_request.author_association)
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v2
-    - uses: actions/setup-python@v2
+    - uses: actions/checkout@v3
+    - uses: actions/setup-python@v4
+      with:
+        python-version: '3.x'
     - name: set PYSHA
       run: echo "PYSHA=$(python -VV | sha256sum | cut -d' ' -f1)" >> $GITHUB_ENV
-    - uses: actions/cache@v1
+    - uses: actions/cache@v3
       with:
         path: ~/.cache/pre-commit
         key: pre-commit|${{ env.PYSHA }}|${{ hashFiles('.pre-commit-config.yaml') }}
     - name: dependencies
       run: pip install -U pre-commit
     - uses: reviewdog/action-setup@v1
     - if: github.event_name == 'push' || github.event_name == 'pull_request'
@@ -27,56 +29,49 @@
         pre-commit run -a todo | reviewdog -efm="%f:%l: %m" -name=TODO -tee -reporter=$REPORTER -filter-mode nofilter
         pre-commit run -a flake8 | reviewdog -f=pep8 -name=flake8 -tee -reporter=$REPORTER -filter-mode nofilter
       env:
         REVIEWDOG_GITHUB_API_TOKEN: ${{ secrets.GITHUB_TOKEN }}
         EVENT: ${{ github.event_name }}
     - run: pre-commit run -a --show-diff-on-failure
   test:
-    if: github.event_name != 'pull_request' || github.repository_owner != 'AMYPAD'
+    if: github.event_name != 'pull_request' || !contains('OWNER,MEMBER,COLLABORATOR', github.event.pull_request.author_association)
     name: py${{ matrix.python }}
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python: [3.6, 3.9]
+        python: [3.7, 3.11]
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
       with:
         fetch-depth: 0
-    - uses: actions/setup-python@v2
+    - uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python }}
     - run: pip install -U -e .[dev]
     - run: pytest
-    - uses: codecov/codecov-action@v1
+    - uses: codecov/codecov-action@v3
   deploy:
     needs: [check, test]
     name: PyPI Deploy
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
       with:
         fetch-depth: 0
-    - uses: actions/setup-python@v2
+    - uses: actions/setup-python@v4
+      with:
+        python-version: '3.x'
     - id: dist
       uses: casperdcl/deploy-pypi@v2
       with:
-        requirements: twine setuptools wheel setuptools_scm[toml]
         build: true
         gpg_key: ${{ secrets.GPG_KEY }}
         password: ${{ secrets.PYPI_TOKEN }}
         upload: ${{ github.event_name == 'push' && startsWith(github.ref, 'refs/tags') }}
-    - id: meta
-      name: Changelog
-      run: |
-        echo ::set-output name=tag::${GITHUB_REF#refs/tags/}
-        git log --pretty='format:%d%n- %s%n%b---' $(git tag --sort=v:refname | tail -n2 | head -n1)..HEAD > _CHANGES.md
     - if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
-      uses: softprops/action-gh-release@v1
+      name: Release
+      run: |
+        changelog=$(git log --pretty='format:%d%n- %s%n%b---' $(git tag --sort=v:refname | tail -n2 | head -n1)..HEAD)
+        tag="${GITHUB_REF#refs/tags/}"
+        gh release create --title "NiftyPAD $tag beta" --draft --notes "$changelog" "$tag" dist/${{ steps.dist.outputs.whl }} dist/${{ steps.dist.outputs.whl_asc }}
       env:
-        GITHUB_TOKEN: ${{ secrets.GH_TOKEN }}
-      with:
-        name: NiftyPAD ${{ steps.meta.outputs.tag }} beta
-        body_path: _CHANGES.md
-        draft: true
-        files: |
-          dist/${{ steps.dist.outputs.whl }}
-          dist/${{ steps.dist.outputs.whl_asc }}
+        GH_TOKEN: ${{ secrets.GH_TOKEN || github.token }}
```

### Comparing `niftypad-1.1.1/.pre-commit-config.yaml` & `niftypad-2.0.0/.pre-commit-config.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 default_language_version:
   python: python3
 repos:
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.0.1
+  rev: v4.4.0
   hooks:
   - id: check-added-large-files
   - id: check-case-conflict
   - id: check-docstring-first
   - id: check-executables-have-shebangs
   - id: check-toml
   - id: check-merge-conflict
@@ -21,26 +21,30 @@
   - id: todo
     name: Check TODO
     language: pygrep
     args: [-i]
     entry: TODO
     types: [text]
     exclude: ^(.pre-commit-config.yaml|.github/workflows/test.yml)$
-- repo: https://gitlab.com/pycqa/flake8
-  rev: 3.9.2
+- repo: https://github.com/PyCQA/flake8
+  rev: 5.0.4
   hooks:
   - id: flake8
     args: [-j8]
     additional_dependencies:
+    - flake8-broken-line
     - flake8-bugbear
     - flake8-comprehensions
     - flake8-debugger
+    - flake8-isort
+    - flake8-pyproject
     - flake8-string-format
 - repo: https://github.com/google/yapf
-  rev: v0.31.0
+  rev: v0.40.0
   hooks:
   - id: yapf
     args: [-i]
+    additional_dependencies: [toml]
 - repo: https://github.com/PyCQA/isort
-  rev: 5.9.3
+  rev: 5.12.0
   hooks:
   - id: isort
```

### Comparing `niftypad-1.1.1/LICENSE` & `niftypad-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `niftypad-1.1.1/examples/demo_img.py` & `niftypad-2.0.0/examples/demo_img.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 ref = Ref(cer_GM, dt)
 ref.interp_1cubic()
 
 # img file
 file_path = ''
 pet_file = file_path + 'E301_FLUT_AC1_combined_ID_cleared.nii'
 img = nib.load(pet_file)
-pet_image = img.get_data()
+pet_image = np.asanyarray(img.dataobj)
 
 # k2p
 k2p = 0.000250
 
 # basis functions
 beta_lim = [0.0100000 / 60, 0.300000 / 60]
 n_beta = 40
@@ -61,17 +61,18 @@
     'srtmb_basis', 'srtmb_k2p_basis', 'srtmb_asl_basis', 'logan_ref', 'logan_ref_k2p', 'mrtm',
     'mrtm_k2p']
 km_outputs = ['R1', 'k2', 'BP']
 
 for model_name in models:
     print(model_name)
     model_inputs = get_model_inputs(user_inputs, model_name)
-    parametric_images_dict, pet_image_fit = image_to_parametric(pet_image, dt, model_name,
-                                                                model_inputs, km_outputs, thr=0.1)
-    for kp in parametric_images_dict.keys():
+    parametric_images_dict = image_to_parametric(pet_image, dt, model_name, model_inputs,
+                                                 km_outputs, thr=0.1)
+    pet_image_fit = parametric_images_dict.pop('fit', None)
+    for kp in parametric_images_dict:
         nib.save(
             nib.Nifti1Image(parametric_images_dict[kp], img.affine),
             os.path.splitext(img.get_filename())[0] + '_' + model_name + '_' + kp +
             os.path.splitext(img.get_filename())[1])
     nib.save(
         nib.Nifti1Image(pet_image_fit, img.affine),
         os.path.splitext(img.get_filename())[0] + '_' + model_name + '_' + 'fit' +
```

### Comparing `niftypad-1.1.1/examples/demo_img_suvr.py` & `niftypad-2.0.0/examples/demo_img_suvr.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 cer_GM = cer_right_GM/2 + cer_left_GM/2
 ref = Ref(cer_GM, dt)
 
 # img file
 file_path = '/Users/Himiko/data/amsterdam_data/'
 pet_file = file_path + 'E301_FLUT_AC1_combined_ID_cleared.nii'
 img = nib.load(pet_file)
-pet_image = img.get_data()
+pet_image = np.asanyarray(img.dataobj)
 frame_index = np.arange(pet_image.shape[-1])
 
 image_suvr = image_to_suvr_with_reference_tac(pet_image=pet_image, dt=dt,
                                               reference_regional_tac=ref.tac,
                                               selected_frame_index=frame_index[-2:])
 nib.save(
     nib.Nifti1Image(image_suvr, img.affine),
```

### Comparing `niftypad-1.1.1/examples/demo_tac.py` & `niftypad-2.0.0/examples/demo_tac.py`

 * *Files identical despite different names*

### Comparing `niftypad-1.1.1/examples/dt_fill_gaps_test.py` & `niftypad-2.0.0/examples/dt_fill_gaps_test.py`

 * *Files identical despite different names*

### Comparing `niftypad-1.1.1/niftypad/api/__init__.py` & `niftypad-2.0.0/niftypad/api/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 from pathlib import Path
 
 from . import readers
 
 log = logging.getLogger(__name__)
 
 
-def kinetic_model(src, dst=None, params=None, model='srtmb_basis', input_interp_method='linear',
-                  w=None, r1=1, k2p=0.000250, beta_lim=None, n_beta=40, linear_phase_start=500,
-                  linear_phase_end=None, km_outputs=None, thr=0.1, fig=False):
+def kinetic_model(src, dst=None, params=None, models=None, input_interp_method='linear', w=None,
+                  r1=1, k2p=0.000250, beta_lim=None, n_beta=40, linear_phase_start=500,
+                  linear_phase_end=None, km_outputs=None, mask=None, thr=0.1, fig=False):
     """
     Args:
       src (Path or str): input patient directory or filename
       dst (Path or str): output directory (default: `src` directory)
       params (Path or str): config (relative to `src` directory)
-      model (str): any model from `niftypad.models` (see `niftypad.models.NAMES`)
+      models (list[str] or str): any model from `niftypad.models` (see `niftypad.models.NAMES`)
       input_interp_method (str): the interpolation method for getting reference input:
         linear, cubic, exp_1, exp_2, feng_srtm
       w (ndarray): weights for weighted model fitting
       r1 (float): a pre-chosen value between 0 and 1 for r1, used in srtmb_asl_basis
       k2p (float): a pre-chosen value for k2p, in second^-1, used in
         srtmb_k2p_basis, logan_ref_k2p, mrtm_k2p
       beta_lim (list[int]): [beta_min, beta_max] for setting the lower and upper limits
@@ -27,23 +27,24 @@
       n_beta (int): number of beta values/basis functions, used in
         srtmb_basis, srtmb_k2p_basis, srtmb_asl_basis
       linear_phase_start (int): start time of linear phase in seconds, used in logan_ref,
         logan_ref_k2p, mrtm, mrtm_k2p
       linear_phase_end (int): end time of linear phase in seconds, used in logan_ref,
         logan_ref_k2p, mrtm, mrtm_k2p
       km_outputs (list[str]): the kinetic parameters to save, e.g. ['R1', 'k2', 'BP']
-      thr (float): threshold value between 0 and 1. Used to mask out voxels with mean value
-        over time exceeding `thr * max(image value)`
+      mask (str): image file that contain a mask to select voxels to apply kinetic models, where
+        `mask[voxel] > 0` indicates `voxel` is selected
+      thr (float): threshold value between `0` and `1`. Only used if `mask=None`. Used to mask out
+        voxels with mean value over time less than `thr * max(image value)`
       fig (bool): whether to show a figure to check model fitting
     """
-    import nibabel as nib
     import numpy as np
 
     from niftypad import basis
-    from niftypad.image_process.parametric_image import image_to_parametric
+    from niftypad.image_process.parametric_image import image_to_parametric_files
     from niftypad.models import get_model_inputs
     from niftypad.tac import Ref
 
     src_path = Path(src)
     if src_path.is_dir():
         fpath = next(src_path.glob('*.nii'))
     else:
@@ -53,42 +54,37 @@
 
     if dst is None:
         dst_path = src_path
     else:
         dst_path = Path(dst)
         assert dst_path.is_dir()
 
+    if isinstance(models, str):
+        models = [models]
+
     meta = readers.find_meta(src_path, filter(None, [params, fpath.stem]))
     dt = np.asarray(meta['dt'])
     ref = np.asarray(meta['ref'])
     ref = Ref(ref, dt)
     # change ref interpolation to selected method
     ref.run_interp(input_interp_method=input_interp_method)
 
-    log.debug("looking for first `*.nii` file in %s", src_path)
-    img = nib.load(fpath)
-    # pet_image = img.get_fdata(dtype=np.float32)
-    pet_image = np.asanyarray(img.dataobj)
-
     # basis functions
     if beta_lim is None:
         beta_lim = [0.01 / 60, 0.3 / 60]
     # change ref.inputf1cubic -> ref.input_interp_1
     b = basis.make_basis(ref.input_interp_1, dt, beta_lim=beta_lim, n_beta=n_beta, w=w, k2p=k2p)
 
     if km_outputs is None:
         km_outputs = ['R1', 'k2', 'BP']
-    # change ref.inputf1cubic -> ref.input_interp_1
+
     user_inputs = {
-        'dt': dt, 'ref': ref, 'inputf1': ref.input_interp_1, 'w': w, 'r1': r1, 'k2p': k2p,
-        'beta_lim': beta_lim, 'n_beta': n_beta, 'b': b, 'linear_phase_start': linear_phase_start,
-        'linear_phase_end': linear_phase_end, 'fig': fig}
-    model_inputs = get_model_inputs(user_inputs, model)
-    # log.debug("model_inputs:%s", model_inputs)
-
-    parametric_images_dict, pet_image_fit = image_to_parametric(pet_image, dt, model, model_inputs,
-                                                                km_outputs, thr=thr)
-    for kp in parametric_images_dict:
-        nib.save(nib.Nifti1Image(parametric_images_dict[kp], img.affine),
-                 f"{dst_path / fpath.stem}_{model}_{kp}_{fpath.suffix}")
-    nib.save(nib.Nifti1Image(pet_image_fit, img.affine),
-             f"{dst_path / fpath.stem}_{model}_fit_{fpath.suffix}")
+        'dt': dt, 'inputf1': ref.input_interp_1, 'fig': fig, 'w': w, 'r1': r1, 'ref': ref,
+        'k2p': k2p, 'beta_lim': beta_lim, 'n_beta': n_beta, 'b': b,
+        'linear_phase_start': linear_phase_start, 'linear_phase_end': linear_phase_end}
+
+    for model in models:
+        model_inputs = get_model_inputs(user_inputs, model)
+        log.debug("model_inputs:%s", model_inputs)
+        image_to_parametric_files(pet_image_path=fpath, dt=dt, model_name=model,
+                                  model_inputs=model_inputs, km_outputs=km_outputs, mask_file=mask,
+                                  thr=thr, save_path=dst_path)
```

### Comparing `niftypad-1.1.1/niftypad/api/readers.py` & `niftypad-2.0.0/niftypad/api/readers.py`

 * *Files identical despite different names*

### Comparing `niftypad-1.1.1/niftypad/basis.py` & `niftypad-2.0.0/niftypad/basis.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 __author__ = 'jieqing jiao'
 
 import matplotlib.pyplot as plt
 import numpy as np
+from scipy.interpolate import interp1d
 
 from . import kt
 
 
 def make_basis(inputf1, dt, beta_lim=None, n_beta=128, beta_space='log', w=None, k2p=None,
                fig=False):
     if beta_lim is None:
         beta_lim = [10e-6, 10e-1]
 
     # dt can skip frames if needed
 
     # calculate input based on dt
     tdur = kt.dt2tdur(dt)
-    input = kt.int2dt(inputf1, dt)
     t1 = np.arange(np.amax(dt))
 
     # generate basis functions and m based on dt
     if beta_space == 'log':
         beta = np.logspace(start=np.log10(beta_lim[0]), stop=np.log10(beta_lim[1]), num=n_beta,
-                           endpoint=False)
+                           endpoint=True)
     elif beta_space == 'natural':
         beta = np.zeros(n_beta)
         for i in range(0, n_beta):
             beta[i] = -1 / t1[-1] * np.log(
                 (np.exp(-beta_lim[0] * t1[-1]) - np.exp(-beta_lim[1] * t1[-1])) / n_beta * i +
                 np.exp(-beta_lim[1] * t1[-1]))
     basis = np.zeros((beta.size, tdur.size))
@@ -34,16 +34,28 @@
     m_w = np.zeros((beta.size * 2, tdur.size))
     basis_k2p = np.zeros((beta.size, tdur.size)) # no need to calculate basis_k2p_w
 
     for i in range(0, beta.size):
         # make basis
         # inputf1[inputf1 < 0] = 0.0
         basis1 = np.convolve(inputf1, np.exp(-beta[i] * t1))
-        # basis1 = scipy.signal.convolve(inputf1, np.exp(-beta[i]*t1), method='direct')
+
         basis[i, :] = kt.int2dt(basis1, dt)
+        input = kt.int2dt(inputf1, dt)
+        # print(input)
+
+        # # QM basis and input
+        mft = kt.dt2mft(dt)
+        basis_f = interp1d(t1, basis1[:t1.size], kind='linear', fill_value='extrapolate')
+        basis[i, :] = basis_f(mft)
+        inputf = interp1d(np.arange(inputf1.size), inputf1, kind='linear')
+        input = inputf(mft)
+        # print(input)
+
+        # print(input)
         if w is not None:
             basis_w[i, :] = basis[i, :] * w
         # make m
         a = np.column_stack((input, basis[i, :]))
         q, r = np.linalg.qr(a)
         m[i * 2:i*2 + 2, :] = np.linalg.solve(r, q.T)
         if w is not None:
```

### Comparing `niftypad-1.1.1/niftypad/image_process/motion_correction.py` & `niftypad-2.0.0/niftypad/image_process/motion_correction.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 __author__ = 'jieqing jiao'
 __contact__ = 'jieqing.jiao@gmail.com'
 
 import csv
 import os
 
 import nibabel as nib
+import numpy as np
 
 from .parametric_image import image_to_parametric, parametric_to_image
 from .transforms import image_registration_3d_plus_t
 
 
 def kinetic_model_motion_correction(pet_image, dt, model, km_inputs_initial, km_inputs, km_outputs,
                                     initial_fit_index, motion_correction_index, n_iteration,
                                     translation_t, rotation_t):
-    parametric_images_dict, _ = image_to_parametric(pet_image[:, :, :, initial_fit_index],
-                                                    dt[:, initial_fit_index], model,
-                                                    km_inputs_initial, km_outputs)
+    parametric_images_dict = image_to_parametric(pet_image[:, :, :, initial_fit_index],
+                                                 dt[:, initial_fit_index], model,
+                                                 km_inputs_initial, km_outputs)
     pet_image_fit = parametric_to_image(parametric_images_dict, dt, model, km_inputs)
     for ii in range(n_iteration):
         print('iteration ' + str(ii + 1))
         print('updating motion ...')
         translation_t, rotation_t, pet_image_realigned = image_registration_3d_plus_t(
             pet_image, pet_image_fit, translation_t, rotation_t, motion_correction_index)
         print('updating kinetics ...')
-        parametric_images_dict, pet_image_fit = image_to_parametric(pet_image_realigned, dt, model,
-                                                                    km_inputs, km_outputs)
+        parametric_images_dict = image_to_parametric(pet_image_realigned, dt, model, km_inputs,
+                                                     km_outputs)
     return pet_image_realigned, translation_t, rotation_t, parametric_images_dict
 
 
 def kinetic_model_motion_correction_file(pet_file, dt, model, km_inputs_initial, km_inputs,
                                          km_outputs, initial_fit_index, motion_correction_index,
                                          n_iteration, translation_t, rotation_t, save_file):
     pet_img = nib.load(pet_file)
-    pet_img_data = pet_img.get_data()
+    pet_img_data = np.asanyarray(pet_img.dataobj)
     # pet_img_data[pet_img_data < 0] = 0
     pet_img_data[:, :, 0:1, :] = 0
-    pet_image_realigned, translation_t, rotation_t, parametric_images_dict = \
-        kinetic_model_motion_correction(
-            pet_img_data, dt, model, km_inputs_initial, km_inputs, km_outputs, initial_fit_index,
-            motion_correction_index, n_iteration, translation_t, rotation_t)
+    pet_image_realigned, translation_t, rotation_t, parametric_images_dict = (
+        kinetic_model_motion_correction(pet_img_data, dt, model, km_inputs_initial, km_inputs,
+                                        km_outputs, initial_fit_index, motion_correction_index,
+                                        n_iteration, translation_t, rotation_t))
     if save_file:
         parametric_images_dict.update({'mc': pet_image_realigned})
         for kk in parametric_images_dict.keys():
             nib.save(nib.Nifti1Image(parametric_images_dict[kk].squeeze(), pet_img.affine),
                      os.path.splitext(pet_file)[0] + '_mc_' + model + '_' + kk + '.nii')
         motion_file_name = os.path.splitext(pet_file)[0] + '_' + model + '_motion' + '.csv'
         motion_file = open(motion_file_name, 'w')
```

### Comparing `niftypad-1.1.1/niftypad/image_process/parametric_image.py` & `niftypad-2.0.0/niftypad/image_process/parametric_image.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,61 +1,105 @@
 __author__ = 'jieqing jiao'
 __contact__ = 'jieqing.jiao@gmail.com'
+from pathlib import Path
 
+import nibabel as nib
 import numpy as np
 from tqdm import trange
 
 from ..kt import dt2tdur
 from ..tac import TAC
 from .regions import extract_regional_values
 
 
-def image_to_parametric(pet_image, dt, model_name, model_inputs, km_outputs, thr=0.005):
+def image_to_parametric(pet_image, dt, model_name, model_inputs, km_outputs, mask=None, thr=0.005):
     parametric_images = []
-    tac = TAC(pet_image[0, 0, 0,] * 0 + 1, dt)
+    tac = TAC(pet_image[
+        0,
+        0,
+        0,] * 0 + 1, dt)
     tac.run_model(model_name, model_inputs)
     km_outputs = list({c.lower() for c in km_outputs} & set(tac.km_results.keys()))
     for _ in range(len(km_outputs)):
         parametric_images.append(np.zeros(pet_image.shape[0:3]))
     pet_image_fit = np.zeros(pet_image.shape)
-    thr = thr * np.amax(pet_image)
-    mask = np.argwhere(np.mean(pet_image, axis=-1) > thr)
+    if mask is None:
+        thr = thr * np.amax(pet_image)
+        mask = np.argwhere(np.mean(pet_image, axis=-1) > thr)
     for i in trange(mask.shape[0]):
-        tac = TAC(pet_image[mask[i][0], mask[i][1], mask[i][2],], dt)
+        tac = TAC(pet_image[
+            mask[i][0],
+            mask[i][1],
+            mask[i][2],], dt)
         tac.run_model(model_name, model_inputs)
         # # #
         # plt.plot(tac.mft, tac.km_results['tacf'],'r', tac.mft, tac.tac, 'go')
         # plt.show()
         # # #
         if 'tacf' in tac.km_results:
-            pet_image_fit[mask[i][0], mask[i][1], mask[i][2],] = tac.km_results['tacf']
+            pet_image_fit[
+                mask[i][0],
+                mask[i][1],
+                mask[i][2],] = tac.km_results['tacf']
         # # #
         # print(tac.km_results)
         # # #
         for p in range(len(km_outputs)):
-            parametric_images[p][mask[i][0], mask[i][1],
-                                 mask[i][2],] = tac.km_results[km_outputs[p].lower()]
+            parametric_images[p][
+                mask[i][0],
+                mask[i][1],
+                mask[i][2],] = tac.km_results[km_outputs[p].lower()]
     parametric_images_dict = dict(zip(km_outputs, parametric_images))
-    if 'tacf' in tac.km_results:
-        return parametric_images_dict, pet_image_fit
+    if np.any(pet_image_fit):
+        parametric_images_dict.update({'fit': pet_image_fit})
     return parametric_images_dict
 
 
+def image_to_parametric_files(pet_image_path, dt, model_name, model_inputs, km_outputs,
+                              mask_file=None, thr=0.005, save_path=None):
+    img = nib.load(pet_image_path)
+    pet_image = np.asanyarray(img.dataobj)
+
+    if mask_file is not None:
+        mask = nib.load(mask_file)
+        mask = np.asanyarray(mask.dataobj)
+        mask = np.argwhere(mask > 0)
+    else:
+        mask = None
+    if save_path is None:
+        save_path = ''
+    dst_path = Path(save_path)
+
+    parametric_images_dict = image_to_parametric(pet_image, dt, model_name, model_inputs,
+                                                 km_outputs, mask=mask, thr=thr)
+    pet_image_fit = parametric_images_dict.pop('fit', None)
+
+    for kp in parametric_images_dict:
+        nib.save(nib.Nifti1Image(parametric_images_dict[kp], img.affine),
+                 f"{dst_path / pet_image_path.stem}_{model_name}_{kp}{pet_image_path.suffix}")
+    if pet_image_fit is not None:
+        nib.save(nib.Nifti1Image(pet_image_fit, img.affine),
+                 f"{dst_path / pet_image_path.stem}_{model_name}_fit{pet_image_path.suffix}")
+
+
 def parametric_to_image(parametric_images_dict, dt, model, km_inputs):
     parametric_images = list(parametric_images_dict.values())
     pet_image = np.zeros(parametric_images[0].shape[0:3] + (dt.shape[-1],))
     mask = np.argwhere(parametric_images[0] != 0)
     for i in range(mask.shape[0]):
         km_inputs_local = km_inputs.copy()
-        for p in parametric_images_dict.keys():
+        for p in set(parametric_images_dict) - {'fit'}:
             km_inputs_local.update({
                 p.lower(): parametric_images_dict[p][mask[i][0], mask[i][1], mask[i][2]]})
         tac = TAC([], dt)
         getattr(tac, 'run_' + model + '_para2tac')(**km_inputs_local)
-        pet_image[mask[i][0], mask[i][1], mask[i][2],] = tac.km_results['tacf']
+        pet_image[
+            mask[i][0],
+            mask[i][1],
+            mask[i][2],] = tac.km_results['tacf']
     return pet_image
 
 
 def image_to_suvr_with_parcellation(pet_image, dt, parcellation, reference_region_labels,
                                     selected_frame_index):
     reference_regional_tac = extract_regional_values(pet_image, parcellation,
                                                      reference_region_labels)
```

### Comparing `niftypad-1.1.1/niftypad/image_process/regions.py` & `niftypad-2.0.0/niftypad/image_process/regions.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,33 +3,41 @@
 
 import nibabel as nib
 import numpy as np
 
 
 def extract_regional_values(image, parcellation, labels):
     idx = labels_to_index(parcellation, labels)
-    regional_values = np.mean(image[idx,], axis=0)
+    regional_values = np.mean(image[
+        idx,], axis=0)
     return regional_values
 
 
 def labels_to_index(parcellation, labels):
     parcellation = np.squeeze(parcellation)
     idx = np.zeros(parcellation.shape, dtype='bool')
     for i in range(len(labels)):
         idx = np.logical_or(idx, parcellation == labels[i])
     return idx
 
 
 def extract_regional_values_image_file(image_file, parcellation_file):
     image = nib.load(image_file)
-    image_data = image.get_data()
+    image_data = np.asanyarray(image.dataobj)
     n_frames = 1
     if image_data.ndim == 4:
         n_frames = image_data.shape[-1]
     parcellation_img = nib.load(parcellation_file)
-    parcellation = parcellation_img.get_data()
+    parcellation = np.asanyarray(parcellation_img.dataobj)
     regions_label = np.unique(parcellation)
     regions_data = np.zeros((regions_label.size, n_frames))
     regions_data = np.squeeze(regions_data)
     for i in range(regions_label.size):
         regions_data[i] = extract_regional_values(image_data, parcellation, [regions_label[i]])
     return regions_data, regions_label
+
+
+def get_index_and_value_for_a_region(image, parcellation, labels):
+    idx = labels_to_index(parcellation, labels) # idx is a binary mask
+    region_values = image[
+        idx,]
+    return idx, region_values
```

### Comparing `niftypad-1.1.1/niftypad/image_process/transforms.py` & `niftypad-2.0.0/niftypad/image_process/transforms.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,12 +175,11 @@
     return translation, rotation, image_new_g
 
 
 def image_registration_3d_plus_t(image_t, image_ref_t, translation_t, rotation_t,
                                  registration_index, n_iter=100):
     image_new_t = image_t * 1
     for t in registration_index:
-        translation_t[t], rotation_t[t], image_new_t[:, :, :, t] = \
-            image_registration_3d_gn(
-                image_t[:, :, :, t], image_ref_t[:, :, :, t],
-                translation=translation_t[t], rotation=rotation_t[t], n_iter=n_iter)
+        translation_t[t], rotation_t[t], image_new_t[:, :, :, t] = image_registration_3d_gn(
+            image_t[:, :, :, t], image_ref_t[:, :, :, t], translation=translation_t[t],
+            rotation=rotation_t[t], n_iter=n_iter)
     return translation_t, rotation_t, image_new_t
```

### Comparing `niftypad-1.1.1/niftypad/kp.py` & `niftypad-2.0.0/niftypad/kp.py`

 * *Files identical despite different names*

### Comparing `niftypad-1.1.1/niftypad/kt.py` & `niftypad-2.0.0/niftypad/kt.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,89 +8,124 @@
 
 def dt2mft(dt):
     mft = np.mean(dt, axis=0)
     return mft
 
 
 def dt2tdur(dt):
-    tdur = dt[1,] - dt[0,]
+    tdur = dt[
+        1,] - dt[
+            0,]
     return tdur
 
 
 def mft2tdur(mft):
-    print('mind the gap')
     tdur = np.zeros_like(mft)
     tdur[0] = mft[0] * 2
     for i in range(1, len(mft)):
         tdur[i] = (mft[i] - np.sum(tdur)) * 2
     return tdur
 
 
 def tdur2dt(tdur):
-    print('mind the gap')
     st = np.zeros_like(tdur)
     et = np.zeros_like(tdur)
     st[0] = 0
     et[0] = tdur[0]
     for i in range(1, len(tdur)):
         st[i] = et[i - 1]
         et[i] = st[i] + tdur[i]
-    dt = [st, et]
+    dt = np.array([st, et])
     return dt
 
 
 def mft2dt(mft):
-    print('mind the gap')
     tdur = mft2tdur(mft)
     dt = tdur2dt(tdur)
+    dt = np.rint(dt).astype(int)
     return dt
 
 
 def tdur2mft(tdur):
-    print('mind the gap')
     dt = tdur2dt(tdur)
     mft = dt2mft(dt)
     return mft
 
 
+def mft_tdur2dt(mft, tdur):
+
+    tdur_dummy = mft2tdur(mft)
+    index = np.where(tdur_dummy - tdur != 0)
+    dt = mft2dt(mft)
+    for i in index:
+        dt[0, i] = mft[i] - tdur[i] / 2
+        dt[1, i] = mft[i] + tdur[i] / 2
+    dt = np.round(dt)
+    dt = np.rint(dt).astype(int)
+    return dt
+
+
 def dt_has_gaps(dt):
     dt_has_gaps = False
     unique, counts = np.unique(dt, return_counts=True)
     gap_ends = unique[counts == 1]
     if len(gap_ends) > 2:
         dt_has_gaps = True
     return dt_has_gaps
 
 
+def dt_find_gaps(dt):
+    dt_gaps = []
+    unique, counts = np.unique(dt, return_counts=True)
+    gap_ends = unique[counts == 1]
+    if len(gap_ends) > 2:
+        gap_ends = gap_ends[1:-1]
+        gap_starts_index = range(0, len(gap_ends), 2)
+        for i in gap_starts_index:
+            dt_gaps.append(list(gap_ends[i:i + 2]))
+    return dt_gaps
+
+
 def dt_fill_gaps(dt):
     unique, counts = np.unique(dt, return_counts=True)
     gap_ends = unique[counts == 1]
     if len(gap_ends) > 2:
         gap_ends = gap_ends[1:-1]
         gap_starts_index = range(0, len(gap_ends), 2)
         for i in gap_starts_index:
             # print(gap_ends[i:i+2])
             dt_gap = np.unique(np.floor(np.linspace(gap_ends[i], gap_ends[i + 1],
-                                                    10))).astype('int16')
+                                                    10 + 2))).astype('int16')
             tdur_to_insert = np.diff(dt_gap)
             dt_to_insert = tdur2dt(tdur_to_insert) + gap_ends[i]
-            dt = np.insert(dt, np.where(dt[1,] == gap_ends[i])[0] + 1, dt_to_insert, axis=-1)
+            dt = np.insert(dt,
+                           np.where(dt[
+                               1,] == gap_ends[i])[0] + 1, dt_to_insert, axis=-1)
     return dt
 
 
-def tac_dt_fill_coffee_break(tac, dt, fig=False):
-    # interpolate tac with coffee break using cubic interpolation
+def tac_dt_fill_coffee_break(tac, dt, interp, fig=False):
+    # interpolate tac with coffee break using linear or cubic interpolation
     mft = dt2mft(dt)
-    tac_inputf1cubic = interpt1cubic(mft, tac, dt)
     dt_no_gaps = dt_fill_gaps(dt)
-    tac_no_gaps = int2dt(tac_inputf1cubic, dt_no_gaps)
+    mft_no_gaps = dt2mft(dt_no_gaps)
+    if interp in ['linear', 'cubic']:
+        tac_inputf1 = {'linear': interpt1, 'cubic': interpt1cubic}[interp](mft, tac, dt)
+        tac_no_gaps = int2dt(tac_inputf1, dt_no_gaps)
+    elif interp == 'zero':
+        tac_no_gaps = np.zeros_like(mft_no_gaps)
+    else:
+        raise ValueError(interp)
     if fig:
         plt.plot(mft, tac, '.')
         plt.plot(dt2mft(dt_no_gaps), tac_no_gaps, 'r')
         plt.show()
+    # replace tac with the original values without interpolation
+    _, index_no_gaps, index = np.intersect1d(mft_no_gaps, mft, return_indices=True)
+    tac_no_gaps[index_no_gaps] = tac[index]
     return tac_no_gaps, dt_no_gaps
 
 
 # # # #
 
 
 def int2dt(f1, dt):
@@ -102,18 +137,25 @@
         f[j] = np.sum(f1[dt[0, j]:dt[1, j]]) / tdur[j]
     return f
 
 
 def interpt1(inputt, inputf, dt):
     # interpolate function
     t1 = np.arange(np.amax(dt))
-    if inputt[0] > t1[0]:
-        inputt = np.append(t1[0], inputt)
-        inputf = np.append(0, inputf)
+    # if inputt[0] > t1[0]:
+    #     inputt = np.append(t1[0], inputt)
+    #     inputf = np.append(0, inputf)
+    inputt = np.append(0, inputt)
+    inputf = np.append(0, inputf)
     inputff = interp1d(inputt, inputf, kind='linear', fill_value='extrapolate')
+
+    # # Qmodelling interpolation
+    # inputff = interp1d(inputt, inputf, kind='linear', fill_value=(inputf[0], inputf[-1]),
+    #                    bounds_error=False)
+
     inputf1 = inputff(t1)
     return inputf1
 
 
 def interpt1cubic(inputt, inputf, dt):
     # interpolate function
     t1 = np.arange(np.amax(dt))
```

### Comparing `niftypad-1.1.1/niftypad/models.py` & `niftypad-2.0.0/niftypad/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # - *_ppet: kinetic model implementations of the PPET software
 # - *_para2tac: generative models for motion correction
 NAMES = [
     'exp_1', 'exp_1_fun', 'exp_1_fun_t', 'exp_2', 'exp_2_fun', 'exp_2_fun_t', 'feng_fun_t',
     'feng_srtm', 'feng_srtm_fun', 'feng_srtm_fun_t', 'list_models', 'logan_ref', 'logan_ref_k2p',
     'mrtm', 'mrtm_k2p', 'srtm', 'srtm_fun', 'srtm_fun_k2p', 'srtm_fun_k2p_w', 'srtm_fun_w',
     'srtm_k2p', 'srtmb', 'srtmb_asl', 'srtmb_asl_basis', 'srtmb_basis', 'srtmb_k2p',
-    'srtmb_k2p_basis']
+    'srtmb_k2p_basis', 'srtmb_basis_para2tac', 'srtmb_k2p_basis_para2tac', 'srtm_para2tac']
 __all__ = NAMES + ['NAMES', 'get_model_inputs']
 
 
 def get_model_inputs(user_inputs, model_name):
     """select model args from user_inputs"""
     if model_name not in NAMES:
         raise ValueError(f"Unknown model:'{model_name}' not in {NAMES}")
@@ -65,14 +65,40 @@
 
     theta = np.append(theta, b['beta'][i])
     r1, k2, bp = kp.srtm_theta2kp(theta)
     kps = {'r1': r1, 'k2': k2, 'bp': bp, 'tacf': tacf}
     return kps
 
 
+def srtmb_basis_ppet(tac, b):
+    tac[tac < 0] = 0.0
+
+    n_beta = b['beta'].size
+    ssq = np.zeros(n_beta)
+
+    if b['w'] is None:
+        b['w'] = 1
+
+    for i in range(0, n_beta):
+        a = np.column_stack((b['input'], b['basis'][i, :]))
+        theta = np.linalg.inv(a.T @ a) @ a.T @ tac
+        tacf = np.dot(a, theta)
+        res = (tac-tacf) * b['w']
+        ssq[i] = np.sum(res**2)
+    i = np.argmin(ssq)
+    a = np.column_stack((b['input'], b['basis'][i, :]))
+    theta = np.linalg.inv(a.T @ a) @ a.T @ tac
+    tacf = np.dot(a, theta)
+
+    theta = np.append(theta, b['beta'][i])
+    r1, k2, bp = kp.srtm_theta2kp(theta)
+    kps = {'r1': r1, 'k2': k2, 'bp': bp, 'tacf': tacf}
+    return kps
+
+
 def srtmb_basis_para2tac(r1, k2, bp, b):
     tacf = []
     theta = kp.srtm_kp2theta(r1, k2, bp)
     i = np.argwhere(abs(b['beta'] - theta[-1]) < 1e-10).squeeze()
     if not i == []:
         a = np.column_stack((b['input'], b['basis'][i, :]))
         tacf = np.dot(a, theta[:-1])
@@ -130,17 +156,17 @@
 
 def srtmb_k2p_basis(tac, b):
     """srtm model for img with fixed k2p and pre-calculated basis functions"""
     tac[tac < 0] = 0.0
 
     n_beta = b['beta'].size
     ssq = np.zeros(n_beta)
-
     if b['w'] is None:
-        b['w'] = 1
+        b['w'] = np.ones_like(tac)
+
     for i in range(0, n_beta):
         r1 = np.sum(b['w'] * b['basis_k2p'][i] * tac) / np.sum(b['w'] * b['basis_k2p'][i]**2)
         ssq[i] = np.sum(b['w'] * (tac - r1 * b['basis_k2p'][i])**2)
 
     i = np.argmin(ssq)
     r1 = np.sum(b['w'] * b['basis_k2p'][i] * tac) / np.sum(b['w'] * b['basis_k2p'][i]**2)
     tacf = r1 * b['basis_k2p'][i]
@@ -170,26 +196,32 @@
     kps = srtmb_k2p_basis(tac, b)
     return kps
 
 
 # # # # # # graphic models
 
 
-def logan_ref(tac, dt, inputf1, linear_phase_start, linear_phase_end, fig):
+def logan_ref(tac, dt, inputf1, w, linear_phase_start, linear_phase_end, fig):
     """
     logan reference plot without fixed k2p for tac, based on eq.7 in
     "Distribution Volume Ratios Without Blood Sampling from Graphical Analysis of PET Data"
     """
+    if w is None:
+        w = np.ones_like(tac)
     if linear_phase_start is None:
         linear_phase_start = 0
     if linear_phase_end is None:
         linear_phase_end = np.amax(dt)
+    if linear_phase_end > np.amax(dt):
+        linear_phase_end = np.amax(dt)
+
     # fill the coffee break gap
     if kt.dt_has_gaps(dt):
-        tac, dt = kt.tac_dt_fill_coffee_break(tac, dt)
+        w, _ = kt.tac_dt_fill_coffee_break(w, dt, interp='zero')
+        tac, dt = kt.tac_dt_fill_coffee_break(tac, dt, interp='linear')
     mft = kt.dt2mft(dt)
     mft = np.append(0, mft)
     dt_new = np.array([mft[:-1], mft[1:]])
     tdur = kt.dt2tdur(dt_new)
     # input_dt = kt.int2dt(inputf1, dt)
     inputff = interp1d(np.arange(len(inputf1)), inputf1, kind='linear', fill_value='extrapolate')
     input_dt = inputff(mft)
@@ -216,42 +248,56 @@
     tt = tt[1:]
     # select tt for tac > 0
     tt = np.logical_and(tt, tac > 0)
     # select tt for xx < inf, yy < inf
     infinf = 1e10
     tt = np.logical_and(tt, xx < infinf)
     tt = np.logical_and(tt, yy < infinf)
+    tt = np.logical_and(tt, w > 0)
 
     # do linear regression with selected tt
-    xx = xx[tt]
-    yy = yy[tt]
+    # xx = xx[tt]
+    # yy = yy[tt]
+    # dvr, inter, _, _, _ = linregress(xx, yy)
+    # bp = dvr - 1
+    # yyf = dvr * xx + inter
+    try:
+        reg = LinearRegression().fit(xx[tt].reshape(-1, 1), yy[tt], sample_weight=w[tt])
+        dvr = reg.coef_[0]
+        bp = dvr - 1
+        yyf = reg.predict(xx.reshape(-1, 1))
+    except Exception:
+        bp = 0
+        yyf = yy[tt] * 0
 
-    dvr, inter, _, _, _ = linregress(xx, yy)
-    bp = dvr - 1
-    yyf = dvr*xx + inter
     if fig:
         plt.plot(xx, yy, '.')
         plt.plot(xx, yyf, 'r')
         plt.show()
     kps = {'bp': bp}
     return kps
 
 
-def logan_ref_k2p(tac, dt, inputf1, k2p, linear_phase_start, linear_phase_end, fig):
+def logan_ref_k2p(tac, dt, inputf1, k2p, w, linear_phase_start, linear_phase_end, fig):
     """
     logan reference plot with fixed k2p for tac, based on eq.6 in
     "Distribution Volume Ratios Without Blood Sampling from Graphical Analysis of PET Data"
     """
+    if w is None:
+        w = np.ones_like(tac)
     if linear_phase_start is None:
         linear_phase_start = 0
     if linear_phase_end is None:
         linear_phase_end = np.amax(dt)
+    if linear_phase_end > np.amax(dt):
+        linear_phase_end = np.amax(dt)
     # fill the coffee break gap
     if kt.dt_has_gaps(dt):
-        tac, dt = kt.tac_dt_fill_coffee_break(tac, dt)
+        w, _ = kt.tac_dt_fill_coffee_break(w, dt, interp='zero')
+        tac, dt = kt.tac_dt_fill_coffee_break(tac, dt, interp='linear')
     mft = kt.dt2mft(dt)
     mft = np.append(0, mft)
     dt_new = np.array([mft[:-1], mft[1:]])
     tdur = kt.dt2tdur(dt_new)
     # input_dt = kt.int2dt(inputf1, dt)
     inputff = interp1d(np.arange(len(inputf1)), inputf1, kind='linear', fill_value='extrapolate')
     input_dt = inputff(mft)
@@ -273,42 +319,48 @@
 
     # find tt for the linear phase
     tt = np.logical_and(mft >= linear_phase_start, mft <= linear_phase_end)
     tt = tt[1:]
     # select tt for tac > 0
     tt = np.logical_and(tt, tac > 0)
     # select tt for xx < inf, yy < inf
-    infinf = 1e10
+    infinf = 1e20
     tt = np.logical_and(tt, xx < infinf)
     tt = np.logical_and(tt, yy < infinf)
+    tt = np.logical_and(tt, w > 0)
 
     # do linear regression with selected tt
-    xx = xx[tt]
-    yy = yy[tt]
 
-    dvr, inter, _, _, _ = linregress(xx, yy)
+    reg = LinearRegression().fit(xx[tt].reshape(-1, 1), yy[tt], sample_weight=w[tt])
+    dvr = reg.coef_[0]
     bp = dvr - 1
-    yyf = dvr*xx + inter
+    yyf = reg.predict(xx.reshape(-1, 1))
+
     if fig:
         plt.plot(xx, yy, '.')
         plt.plot(xx[tt], yyf[tt], 'r')
         plt.show()
     kps = {'bp': bp}
     return kps
 
 
-def mrtm(tac, dt, inputf1, linear_phase_start, linear_phase_end, fig):
+def mrtm(tac, dt, inputf1, w, linear_phase_start, linear_phase_end, fig):
     """Ichise's multilinear reference tissue model"""
+    if w is None:
+        w = np.ones_like(tac)
     if linear_phase_start is None:
         linear_phase_start = 0
     if linear_phase_end is None:
         linear_phase_end = np.amax(dt)
+    if linear_phase_end > np.amax(dt):
+        linear_phase_end = np.amax(dt)
     # fill the coffee break gap
     if kt.dt_has_gaps(dt):
-        tac, dt = kt.tac_dt_fill_coffee_break(tac, dt)
+        w, _ = kt.tac_dt_fill_coffee_break(w, dt, interp='zero')
+        tac, dt = kt.tac_dt_fill_coffee_break(tac, dt, interp='linear')
     mft = kt.dt2mft(dt)
     mft = np.append(0, mft)
     dt_new = np.array([mft[:-1], mft[1:]])
     tdur = kt.dt2tdur(dt_new)
     # input_dt = kt.int2dt(inputf1, dt)
     inputff = interp1d(np.arange(len(inputf1)), inputf1, kind='linear', fill_value='extrapolate')
     input_dt = inputff(mft)
@@ -329,15 +381,18 @@
 
     # find tt for the linear phase
     tt = np.logical_and(mft >= linear_phase_start, mft <= linear_phase_end)
     tt = tt[1:]
 
     mft = mft[1:]
 
-    reg = LinearRegression(fit_intercept=False).fit(xx[tt,], yy[tt])
+    tt = np.logical_and(tt, w > 0)
+
+    reg = LinearRegression(fit_intercept=False).fit(xx[
+        tt,], yy[tt], sample_weight=w[tt])
     bp = -reg.coef_[0] / reg.coef_[1] - 1
     k2p = reg.coef_[0] / reg.coef_[2]
     # for 1 TC
     r1 = reg.coef_[2]
     k2 = -reg.coef_[1]
 
     if np.isnan(bp):
@@ -349,32 +404,37 @@
     if r1 < -5:
         r1 = -5
     if bp > 10:
         bp = 0
     if bp < -10:
         bp = 0
 
-    yyf = reg.predict(xx)
     if fig:
+        yyf = reg.predict(xx)
         plt.plot(mft, yy, '.')
         plt.plot(mft, yyf, 'r')
         plt.show()
     kps = {'bp': bp, 'k2p': k2p, 'r1': r1, 'k2': k2}
     return kps
 
 
-def mrtm_k2p(tac, dt, inputf1, k2p, linear_phase_start, linear_phase_end, fig):
+def mrtm_k2p(tac, dt, inputf1, k2p, w, linear_phase_start, linear_phase_end, fig):
     """Ichise's multilinear reference tissue model with fixed k2prime"""
+    if w is None:
+        w = np.ones_like(tac)
     if linear_phase_start is None:
         linear_phase_start = 0
     if linear_phase_end is None:
         linear_phase_end = np.amax(dt)
+    if linear_phase_end > np.amax(dt):
+        linear_phase_end = np.amax(dt)
     # fill the coffee break gap
     if kt.dt_has_gaps(dt):
-        tac, dt = kt.tac_dt_fill_coffee_break(tac, dt)
+        w, _ = kt.tac_dt_fill_coffee_break(w, dt, interp='zero')
+        tac, dt = kt.tac_dt_fill_coffee_break(tac, dt, interp='linear')
     mft = kt.dt2mft(dt)
     mft = np.append(0, mft)
     dt_new = np.array([mft[:-1], mft[1:]])
     tdur = kt.dt2tdur(dt_new)
     # input_dt = kt.int2dt(inputf1,dt)
     inputff = interp1d(np.arange(len(inputf1)), inputf1, kind='linear', fill_value='extrapolate')
     input_dt = inputff(mft)
@@ -395,15 +455,19 @@
     xx = np.column_stack((input_cum + 1/k2p*input_dt, tac_cum))
 
     # find tt for the linear phase
     tt = np.logical_and(mft >= linear_phase_start, mft <= linear_phase_end)
     tt = tt[1:]
 
     mft = mft[1:]
-    reg = LinearRegression(fit_intercept=False).fit(xx[tt,], yy[tt])
+
+    tt = np.logical_and(tt, w > 0)
+
+    reg = LinearRegression(fit_intercept=False).fit(xx[
+        tt,], yy[tt], sample_weight=w[tt])
     bp = -reg.coef_[0] / reg.coef_[1] - 1
 
     # for 1 TC
     # k2 = -reg.coef_[1]
     r1 = reg.coef_[0] / k2p
 
     if np.isnan(bp):
@@ -500,15 +564,15 @@
         plt.plot(xx, yy, '.')
         plt.plot(xx, yyf, 'r')
         plt.show()
     kps = {'bp': bp}
     return kps
 
 
-def logan_ref_k2p_ppet(tac, dt, ref, k2p, linear_phase_start, linear_phase_end, fig):
+def logan_ref_k2p_ppet(tac, dt, ref, k2p, w, linear_phase_start, linear_phase_end, fig):
     """
     logan_ref_k2p - logan reference plot with fixed k2p for tac, based on eq.6 in
     "Distribution Volume Ratios Without Blood Sampling from Graphical Analysis of PET Data"
     PPET version: calculate input_dt and input_cum differently
     """
     if linear_phase_start is None:
         linear_phase_start = 0
@@ -571,67 +635,79 @@
         plt.plot(xx, yy, '.')
         plt.plot(xx[tt], yyf[tt], 'r')
         plt.show()
     kps = {'bp': bp}
     return kps
 
 
-def mrtm_ppet(tac, dt, ref, linear_phase_start, linear_phase_end, fig):
+def mrtm_ppet(tac, dt, inputf1, w, linear_phase_start, linear_phase_end, fig):
     """
     Ichise's multilinear reference tissue model.
-    PPET version: calculate input_dt and input_cum differently
+    PPET version: calculate input_dt and input_cum, tac_cum differently
     """
+    if w is None:
+        w = np.ones_like(tac)
     if linear_phase_start is None:
         linear_phase_start = 0
     if linear_phase_end is None:
         linear_phase_end = np.amax(dt)
+    if linear_phase_end > np.amax(dt):
+        linear_phase_end = np.amax(dt)
     # fill the coffee break gap
     if kt.dt_has_gaps(dt):
-        tac, dt = kt.tac_dt_fill_coffee_break(tac, dt)
+        w, _ = kt.tac_dt_fill_coffee_break(w, dt, interp='zero')
+        tac, dt = kt.tac_dt_fill_coffee_break(tac, dt, interp='linear')
+
     mft = kt.dt2mft(dt)
     mft = np.append(0, mft)
-    dt_new = np.array([mft[:-1], mft[1:]])
-    tdur = kt.dt2tdur(dt_new)
-    # get input_dt from ref.tac, if dt and ref.dt are the same
-    if np.array_equal(dt, ref.dt):
-        input_dt = ref.tac
-    else:
-        inputff = interp1d(kt.dt2mft(ref.dt), ref.tac, kind='linear', fill_value='extrapolate')
-        input_dt = inputff(mft)
-        input_dt = input_dt[1:]
 
+    # input_dt = kt.int2dt(inputf1, dt)
+    inputff = interp1d(np.arange(len(inputf1)), inputf1, kind='linear', fill_value='extrapolate')
+    input_dt = inputff(mft)
+    input_dt = input_dt[1:]
     tac = np.append(0, tac)
     input_dt = np.append(0, input_dt)
 
     # set negative values to zero
     tac[tac < 0] = 0.0
     input_dt[input_dt < 0] = 0.0
 
-    tac_cum = np.cumsum((tac[:-1] + tac[1:]) / 2 * tdur)
     # calculate input_cum using inputf1, and only until mid frame time
-    inputf1 = kt.interpt1(kt.dt2mft(ref.dt), ref.tac, dt)
     input_cum1 = np.cumsum(inputf1)
     input_cum1_mft = input_cum1[mft.astype(int)]
     input_cum = input_cum1_mft
     # tac_cum and input_cum are calculated in such a way to match tac
     tac = tac[1:]
     input_dt = input_dt[1:]
     input_cum = input_cum[1:]
+
+    # PPET tac_cum calculation
+    tac_cum = np.zeros_like(input_cum)
+    mft_tac = mft[1:]
+    for i in range(len(mft_tac)):
+        if i == 0:
+            tac_cum[i] = tac[i] * (mft_tac[i] - dt[0, i])
+        else:
+            tac_cum[i] = tac_cum[i - 1] + tac[i - 1] * (dt[1, i - 1] - mft_tac[i - 1]) + tac[i] * (
+                mft_tac[i] - dt[0, i])
+    # PPET tac_cum calculation
+
     yy = tac
     xx = np.column_stack((input_cum, tac_cum, input_dt))
 
     # find tt for the linear phase
     tt = np.logical_and(mft >= linear_phase_start, mft <= linear_phase_end)
     tt = tt[1:]
 
     mft = mft[1:]
 
-    reg = LinearRegression(fit_intercept=False).fit(xx[tt,], yy[tt])
-    bp = -reg.coef_[0] / reg.coef_[1] - 1
-    k2p = reg.coef_[0] / reg.coef_[2]
+    reg = LinearRegression(fit_intercept=False).fit(xx[
+        tt,], yy[tt], sample_weight=w[tt])
+    bp = -reg.coef_[0] / (reg.coef_[1] + 0.0000000000000001) - 1
+    k2p = reg.coef_[0] / (reg.coef_[2] + 0.0000000000000001)
     # for 1 TC
     r1 = reg.coef_[2]
     k2 = -reg.coef_[1]
 
     if np.isnan(bp):
         bp = 0
     if np.isnan(r1):
@@ -650,15 +726,15 @@
         plt.plot(mft, yy, '.')
         plt.plot(mft, yyf, 'r')
         plt.show()
     kps = {'bp': bp, 'k2p': k2p, 'r1': r1, 'k2': k2}
     return kps
 
 
-def mrtm_k2p_ppet(tac, dt, ref, k2p, linear_phase_start, linear_phase_end, fig):
+def mrtm_k2p_ppet(tac, dt, ref, k2p, w, linear_phase_start, linear_phase_end, fig):
     """
     Ichise's multilinear reference tissue model with fixed k2prime.
     PPET version: calculate input_dt and input_cum differently
     """
     if linear_phase_start is None:
         linear_phase_start = 0
     if linear_phase_end is None:
@@ -700,15 +776,16 @@
     xx = np.column_stack((input_cum + 1/k2p*input_dt, tac_cum))
 
     # find tt for the linear phase
     tt = np.logical_and(mft >= linear_phase_start, mft <= linear_phase_end)
     tt = tt[1:]
 
     mft = mft[1:]
-    reg = LinearRegression(fit_intercept=False).fit(xx[tt,], yy[tt])
+    reg = LinearRegression(fit_intercept=False).fit(xx[
+        tt,], yy[tt], sample_weight=w)
     bp = -reg.coef_[0] / reg.coef_[1] - 1
 
     # for 1 TC
     # k2 = -reg.coef_[1]
     r1 = reg.coef_[0] / k2p
 
     if np.isnan(bp):
@@ -832,15 +909,15 @@
 
 
 def exp_1(tac, dt, idx, w, fig):
     tac[tac < 0] = 0.0
     if w is None:
         w = np.ones_like(tac)
     ts_te_w = (dt[0, idx], dt[1, idx], w[idx])
-    p0 = (1000, 5000, 10)
+    p0 = (3000, 1, 1)
     p, _ = curve_fit(exp_1_fun, ts_te_w, tac[idx] * w[idx], p0)
     a0, a1, b1 = p
     t1 = np.arange(np.amax(dt))
     tac1f = exp_1_fun_t(t1, a0, a1, b1)
     if fig:
         print(p)
         mft = kt.dt2mft(dt)
@@ -864,15 +941,15 @@
 
 
 def exp_2(tac, dt, idx, w, fig):
     tac[tac < 0] = 0.0
     if w is None:
         w = np.ones_like(tac)
     ts_te_w = (dt[0, idx], dt[1, idx], w[idx])
-    p0 = (1, 1, 1, 0, 0)
+    p0 = (3000, 1, 1, 1, 1)
     p, _ = curve_fit(exp_2_fun, ts_te_w, tac[idx] * w[idx], p0)
     a0, a1, a2, b1, b2 = p
     t1 = np.arange(np.amax(dt))
     tac1f = exp_2_fun_t(t1, a0, a1, a2, b1, b2)
     if fig:
         print(p)
         mft = kt.dt2mft(dt)
@@ -973,25 +1050,27 @@
     return cr
 
 
 def feng_srtm(tac, dt, w, fig):
     tac[tac < 0] = 0.0
     if w is None:
         w = 1
-    ts_te_w = (dt[0,], dt[1,], w)
+    ts_te_w = (dt[
+        0,], dt[
+            1,], w)
     # p0 = [3.90671734e+00, 4.34910151e+02, 9.22189828e+01, 1.35949657e-02,
     #       4.56109635e-02, 4.53841116e-02, 4.54180443e-02, 7.71163349e-04]
     p0 = [1, 2, 3, 4, 0.1, 0.2, 0.3, 0.4]
     # p0 = [6.85579165e-05, -2.08643110e+01, -1.81889002e+02, 7.16906660e+00,
     #       4.21217390e-04, 7.23514957e-02, 7.84986975e-02, 8.27340347e-02]
     p, _ = curve_fit(feng_srtm_fun, ts_te_w, tac * w, p0=p0)
     a0, a1, a2, a3, b0, b1, b2, b3 = p
     t1 = np.arange(np.amax(dt))
     tac1f = feng_srtm_fun_t(t1, a0, a1, a2, a3, b0, b1, b2, b3)
-    print(tac1f)
+    # print(tac1f)
     if fig:
         print(p)
         cp1f = feng_fun_t(t1, a0, a1, a2, b0, b1, b2)
         mft = kt.dt2mft(dt)
         plt.plot(t1, cp1f, 'r', t1, tac1f, 'b', mft, tac, 'go')
         plt.show()
     return tac1f, p
```

### Comparing `niftypad-1.1.1/niftypad/tac.py` & `niftypad-2.0.0/niftypad/tac.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-__author__ = 'jieqing jiao'
-__email__ = "jieqing.jiao@gmail.com"
+import numpy as np
 
 from . import kt, models
 
+__author__ = "jieqing jiao <jieqing.jiao@gmail.com>"
+
 
 class TAC:
     def __init__(self, tac, dt):
         self.tac = tac
         self.dt = dt
         self.mft = kt.dt2mft(dt)
 
@@ -35,60 +36,84 @@
         self.inputf1 = []
         self.inputf1cubic = []
         self.inputf1_exp1 = []
         self.inputf1_exp2 = []
         self.inputf1_exp_am = []
         self.input_interp_method = []
         self.input_interp_1 = []
+        self.idx_to_fit = None
+        self.fill_in_seconds = None
+        self.w = None
 
-    def run_feng_srtm(self, w=None):
-        self.inputf1_feng_srtm, _ = models.feng_srtm(self.tac, self.dt, w=w, fig=True)
+    def run_feng_srtm(self):
+        self.inputf1_feng_srtm, _ = models.feng_srtm(self.tac, self.dt, w=self.w, fig=True)
         self.input_interp_1 = self.inputf1_feng_srtm
+        self.input_interp_method = 'feng_srtm'
 
     def interp_1(self):
         mft = kt.dt2mft(self.dt)
         self.inputf1 = kt.interpt1(mft, self.tac, self.dt)
         self.input_interp_1 = self.inputf1
+        self.input_interp_method = 'linear'
 
     def interp_1cubic(self):
         mft = kt.dt2mft(self.dt)
         self.inputf1cubic = kt.interpt1cubic(mft, self.tac, self.dt)
         self.input_interp_1 = self.inputf1cubic
+        self.input_interp_method = 'cubic'
 
-    def run_exp1(self, w=None, idx_to_fit=None, fill_in_seconds=None):
+    def run_exp1(self):
         self.interp_1()
         self.inputf1_exp1 = self.inputf1
         inputf1_exp1 = 0
-        if idx_to_fit is not None:
-            inputf1_exp1, _ = models.exp_1(self.tac, self.dt, idx=idx_to_fit, w=w, fig=True)
-        if fill_in_seconds is not None:
-            self.inputf1_exp1[fill_in_seconds] = inputf1_exp1[fill_in_seconds]
+        if self.idx_to_fit is not None:
+            inputf1_exp1, _ = models.exp_1(self.tac, self.dt, idx=self.idx_to_fit, w=self.w,
+                                           fig=True)
+        if self.fill_in_seconds is not None:
+            self.inputf1_exp1[self.fill_in_seconds] = inputf1_exp1[self.fill_in_seconds]
         self.input_interp_1 = self.inputf1_exp1
+        self.input_interp_method = 'exp_1'
 
-    def run_exp2(self, w=None, idx_to_fit=None, fill_in_seconds=None):
+    def run_exp2(self):
         self.interp_1()
         self.inputf1_exp2 = self.inputf1
         inputf1_exp2 = 0
-        if idx_to_fit is not None:
-            inputf1_exp2, _ = models.exp_2(self.tac, self.dt, idx=idx_to_fit, w=w, fig=True)
-        if fill_in_seconds is not None:
-            self.inputf1_exp2[fill_in_seconds] = inputf1_exp2[fill_in_seconds]
+        if self.idx_to_fit is not None:
+            inputf1_exp2, _ = models.exp_2(self.tac, self.dt, idx=self.idx_to_fit, w=self.w,
+                                           fig=True)
+        if self.fill_in_seconds is not None:
+            self.inputf1_exp2[self.fill_in_seconds] = inputf1_exp2[self.fill_in_seconds]
         self.input_interp_1 = self.inputf1_exp2
+        self.input_interp_method = 'exp_2'
 
-    def run_exp_am(self, idx_to_fit=None, fill_in_seconds=None):
+    def run_exp_am(self):
         self.interp_1()
         self.inputf1_exp_am = self.inputf1
         inputf1_exp_am = 0
-        if idx_to_fit is not None:
-            inputf1_exp_am, _ = models.exp_am(self.tac, self.dt, idx=idx_to_fit, fig=True)
-        if fill_in_seconds is not None:
-            self.inputf1_exp_am[fill_in_seconds] = inputf1_exp_am[fill_in_seconds]
+        if self.idx_to_fit is not None:
+            inputf1_exp_am, _ = models.exp_am(self.tac, self.dt, idx=self.idx_to_fit, fig=True)
+        if self.fill_in_seconds is not None:
+            self.inputf1_exp_am[self.fill_in_seconds] = inputf1_exp_am[self.fill_in_seconds]
         self.input_interp_1 = self.inputf1_exp_am
+        self.input_interp_method = 'exp_am'
+
+    def auto_find_idx_to_fit(self):
+        self.idx_to_fit = list(range(np.argmax(self.tac), self.tac.size))
+
+    def auto_find_fill_in_seconds(self):
+        self.fill_in_seconds = []
+        dt_gaps = kt.dt_find_gaps(self.dt)
+        for i in dt_gaps:
+            self.fill_in_seconds = self.fill_in_seconds + list(range(i[0], i[1]))
 
-    def run_interp(self, input_interp_method='linear', **kwargs):
+    def run_interp(self, input_interp_method='linear'):
         input_interp_methods = {
             'linear': 'interp_1', 'cubic': 'interp_1cubic', 'exp_1': 'run_exp1',
             'exp_2': 'run_exp2', 'exp_am': 'run_exp_am', 'feng_srtm': 'run_feng_srtm'}
         self.input_interp_method = input_interp_method
-        interp_method = getattr(self,
-                                input_interp_methods.get(input_interp_method, input_interp_method))
-        return interp_method(**kwargs)
+        interp_method = getattr(self, input_interp_methods[input_interp_method])
+        if 'exp' in input_interp_method:
+            if self.idx_to_fit is None:
+                self.auto_find_idx_to_fit()
+            if self.fill_in_seconds is None:
+                self.auto_find_fill_in_seconds()
+        interp_method()
```

### Comparing `niftypad-1.1.1/niftypad/weight.py` & `niftypad-2.0.0/niftypad/weight.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,24 +6,26 @@
 import numpy as np
 
 from . import kt
 
 
 def get_weight(dt, isotope='18F', a=1, t=None, r=None, tac=None):
 
-    if isotope == '18F':
+    if isotope == '12C':
         half_life = 20.39 * 60
-    elif isotope == '12C':
+    elif isotope == '18F':
         half_life = 109.77 * 60
     else:
         print('not known yet')
 
     decay_const = np.log(2) / half_life
     tdur = kt.dt2tdur(dt)
-    dcf = decay_const * tdur / (np.exp(-decay_const * dt[0,]) - np.exp(-decay_const * dt[1,]))
+    dcf = decay_const * tdur / (np.exp(-decay_const * dt[
+        0,]) - np.exp(-decay_const * dt[
+            1,]))
 
     n_model = 5
     w_m = [None] * n_model
     i = 0
     w_m[i] = a * dcf * dcf * t / tdur / tdur
     i += 1
     w_m[i] = a * dcf * dcf * (t + 2*r) / tdur / tdur
@@ -37,24 +39,26 @@
     for i in range(n_model):
         w_m[i] = 1 / w_m[i]
 
     return w_m
 
 
 def get_weight_ppet(dt, tac, isotope='12C', a=1):
-    if isotope == '18F':
+    if isotope == '12C':
         half_life = 20.39 * 60
-    elif isotope == '12C':
+    elif isotope == '18F':
         half_life = 109.77 * 60
     else:
         print('not known yet')
     decay_const = np.log(2) / half_life
 
     tdur = kt.dt2tdur(dt)
-    dcf = decay_const * tdur / (np.exp(-decay_const * dt[0,]) - np.exp(-decay_const * dt[1,]))
+    dcf = decay_const * tdur / (np.exp(-decay_const * dt[
+        0,]) - np.exp(-decay_const * dt[
+            1,]))
     tac_0 = tac * 1
     tac[tac < 0] = 1
 
     abundance = 1 / a
     prompts = abundance / dcf * tdur * tac
     normalised = prompts / np.max(prompts) * 100000000
     w = tdur * tdur / normalised / dcf
```

### Comparing `niftypad-1.1.1/niftypad.egg-info/SOURCES.txt` & `niftypad-2.0.0/niftypad.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 .gitignore
 .mailmap
 .pre-commit-config.yaml
+CITATION.cff
 LICENSE
 README.rst
 pyproject.toml
-setup.cfg
-setup.py
 .github/workflows/comment-bot.yml
 .github/workflows/test.yml
 examples/demo_img.py
 examples/demo_img_suvr.py
 examples/demo_tac.py
 examples/dt_fill_gaps_test.py
+images/Fig1.jpg
 niftypad/__init__.py
 niftypad/__main__.py
 niftypad/_dist_ver.py
 niftypad/basis.py
 niftypad/kp.py
 niftypad/kt.py
 niftypad/models.py
```

