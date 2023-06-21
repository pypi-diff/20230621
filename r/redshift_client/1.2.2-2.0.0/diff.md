# Comparing `tmp/redshift_client-1.2.2.tar.gz` & `tmp/redshift_client-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redshift_client-1.2.2.tar", last modified: Tue Jan  1 00:00:00 1980, max compression
+gzip compressed data, was "redshift_client-2.0.0.tar", last modified: Tue Jan  1 00:00:00 1980, max compression
```

## Comparing `redshift_client-1.2.2.tar` & `redshift_client-2.0.0.tar`

### file list

```diff
@@ -1,55 +1,58 @@
--rw-r--r--   0        0        0       83 1980-01-01 00:00:00.000000 redshift_client-1.2.2/.envrc
--rw-r--r--   0        0        0       47 1980-01-01 00:00:00.000000 redshift_client-1.2.2/.gitignore
--rw-r--r--   0        0        0     2088 1980-01-01 00:00:00.000000 redshift_client-1.2.2/.gitlab-ci.yml
--rw-r--r--   0        0        0      262 1980-01-01 00:00:00.000000 redshift_client-1.2.2/build/ci/check.nix
--rw-r--r--   0        0        0      191 1980-01-01 00:00:00.000000 redshift_client-1.2.2/build/ci/utils.sh
--rw-r--r--   0        0        0      780 1980-01-01 00:00:00.000000 redshift_client-1.2.2/build/default.nix
--rw-r--r--   0        0        0      984 1980-01-01 00:00:00.000000 redshift_client-1.2.2/build/deps/default.nix
--rw-r--r--   0        0        0      217 1980-01-01 00:00:00.000000 redshift_client-1.2.2/build/deps/deprecated/stubs.nix
--rw-r--r--   0        0        0      251 1980-01-01 00:00:00.000000 redshift_client-1.2.2/build/deps/networkx.nix
--rw-r--r--   0        0        0     1368 1980-01-01 00:00:00.000000 redshift_client-1.2.2/build/deps/override_utils.nix
--rw-r--r--   0        0        0      202 1980-01-01 00:00:00.000000 redshift_client-1.2.2/build/deps/psycopg2/stubs.nix
--rw-r--r--   0        0        0      182 1980-01-01 00:00:00.000000 redshift_client-1.2.2/build/dev_env/default.nix
--rwxr-xr-x   0        0        0      131 1980-01-01 00:00:00.000000 redshift_client-1.2.2/build/dev_env/hook.sh
--rw-r--r--   0        0        0     1482 1980-01-01 00:00:00.000000 redshift_client-1.2.2/build/dev_env/vs_settings.py
--rw-r--r--   0        0        0      210 1980-01-01 00:00:00.000000 redshift_client-1.2.2/build/generic_builder/check.nix
--rw-r--r--   0        0        0      341 1980-01-01 00:00:00.000000 redshift_client-1.2.2/build/generic_builder/default.nix
--rw-r--r--   0        0        0      245 1980-01-01 00:00:00.000000 redshift_client-1.2.2/build/generic_builder/env.nix
--rw-r--r--   0        0        0      310 1980-01-01 00:00:00.000000 redshift_client-1.2.2/build/generic_builder/metadata.nix
--rwxr-xr-x   0        0        0      127 1980-01-01 00:00:00.000000 redshift_client-1.2.2/build/generic_builder/pkg/check/tests.sh
--rwxr-xr-x   0        0        0      160 1980-01-01 00:00:00.000000 redshift_client-1.2.2/build/generic_builder/pkg/check/types.sh
--rw-r--r--   0        0        0      625 1980-01-01 00:00:00.000000 redshift_client-1.2.2/build/generic_builder/pkg/default.nix
--rw-r--r--   0        0        0     3085 1980-01-01 00:00:00.000000 redshift_client-1.2.2/flake.lock
--rw-r--r--   0        0        0     1687 1980-01-01 00:00:00.000000 redshift_client-1.2.2/flake.nix
--rw-r--r--   0        0        0      122 1980-01-01 00:00:00.000000 redshift_client-1.2.2/makes.lock.nix
--rw-r--r--   0        0        0      524 1980-01-01 00:00:00.000000 redshift_client-1.2.2/makes.nix
--rw-r--r--   0        0        0      714 1980-01-01 00:00:00.000000 redshift_client-1.2.2/mypy.ini
--rw-r--r--   0        0        0      260 1980-01-01 00:00:00.000000 redshift_client-1.2.2/nix.conf
--rw-r--r--   0        0        0      514 1980-01-01 00:00:00.000000 redshift_client-1.2.2/pyproject.toml
--rw-r--r--   0        0        0       22 1980-01-01 00:00:00.000000 redshift_client-1.2.2/redshift_client/__init__.py
--rw-r--r--   0        0        0      423 1980-01-01 00:00:00.000000 redshift_client-1.2.2/redshift_client/column.py
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-1.2.2/redshift_client/data_type/__init__.py
--rw-r--r--   0        0        0     1584 1980-01-01 00:00:00.000000 redshift_client-1.2.2/redshift_client/data_type/alias.py
--rw-r--r--   0        0        0     1108 1980-01-01 00:00:00.000000 redshift_client-1.2.2/redshift_client/data_type/core.py
--rw-r--r--   0        0        0     1555 1980-01-01 00:00:00.000000 redshift_client-1.2.2/redshift_client/data_type/decode.py
--rw-r--r--   0        0        0      175 1980-01-01 00:00:00.000000 redshift_client-1.2.2/redshift_client/id_objs.py
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-1.2.2/redshift_client/py.typed
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-1.2.2/redshift_client/schema/__init__.py
--rw-r--r--   0        0        0     6728 1980-01-01 00:00:00.000000 redshift_client-1.2.2/redshift_client/schema/client.py
--rw-r--r--   0        0        0      604 1980-01-01 00:00:00.000000 redshift_client-1.2.2/redshift_client/schema/core.py
--rw-r--r--   0        0        0     4410 1980-01-01 00:00:00.000000 redshift_client-1.2.2/redshift_client/sql_client/__init__.py
--rw-r--r--   0        0        0     1046 1980-01-01 00:00:00.000000 redshift_client-1.2.2/redshift_client/sql_client/_assert.py
--rw-r--r--   0        0        0     2381 1980-01-01 00:00:00.000000 redshift_client-1.2.2/redshift_client/sql_client/connection.py
--rw-r--r--   0        0        0     1534 1980-01-01 00:00:00.000000 redshift_client-1.2.2/redshift_client/sql_client/primitive.py
--rw-r--r--   0        0        0     1236 1980-01-01 00:00:00.000000 redshift_client-1.2.2/redshift_client/sql_client/query.py
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-1.2.2/redshift_client/table/__init__.py
--rw-r--r--   0        0        0     1284 1980-01-01 00:00:00.000000 redshift_client-1.2.2/redshift_client/table/_assert.py
--rw-r--r--   0        0        0    12339 1980-01-01 00:00:00.000000 redshift_client-1.2.2/redshift_client/table/client.py
--rw-r--r--   0        0        0     1219 1980-01-01 00:00:00.000000 redshift_client-1.2.2/redshift_client/table/core.py
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-1.2.2/tests/__init__.py
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-1.2.2/tests/arch/__init__.py
--rw-r--r--   0        0        0     1559 1980-01-01 00:00:00.000000 redshift_client-1.2.2/tests/arch/arch.py
--rw-r--r--   0        0        0     1055 1980-01-01 00:00:00.000000 redshift_client-1.2.2/tests/arch/test_arch.py
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-1.2.2/tests/py.typed
--rw-r--r--   0        0        0       45 1980-01-01 00:00:00.000000 redshift_client-1.2.2/tests/test_placeholder.py
--rw-r--r--   0        0        0      394 1970-01-01 00:00:00.000000 redshift_client-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0       83 1980-01-01 00:00:00.000000 redshift_client-2.0.0/.envrc
+-rw-r--r--   0        0        0       47 1980-01-01 00:00:00.000000 redshift_client-2.0.0/.gitignore
+-rw-r--r--   0        0        0     2106 1980-01-01 00:00:00.000000 redshift_client-2.0.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0      262 1980-01-01 00:00:00.000000 redshift_client-2.0.0/build/ci/check.nix
+-rw-r--r--   0        0        0      191 1980-01-01 00:00:00.000000 redshift_client-2.0.0/build/ci/utils.sh
+-rw-r--r--   0        0        0      780 1980-01-01 00:00:00.000000 redshift_client-2.0.0/build/default.nix
+-rw-r--r--   0        0        0      984 1980-01-01 00:00:00.000000 redshift_client-2.0.0/build/deps/default.nix
+-rw-r--r--   0        0        0      217 1980-01-01 00:00:00.000000 redshift_client-2.0.0/build/deps/deprecated/stubs.nix
+-rw-r--r--   0        0        0      251 1980-01-01 00:00:00.000000 redshift_client-2.0.0/build/deps/networkx.nix
+-rw-r--r--   0        0        0     1368 1980-01-01 00:00:00.000000 redshift_client-2.0.0/build/deps/override_utils.nix
+-rw-r--r--   0        0        0      202 1980-01-01 00:00:00.000000 redshift_client-2.0.0/build/deps/psycopg2/stubs.nix
+-rw-r--r--   0        0        0      182 1980-01-01 00:00:00.000000 redshift_client-2.0.0/build/dev_env/default.nix
+-rwxr-xr-x   0        0        0      131 1980-01-01 00:00:00.000000 redshift_client-2.0.0/build/dev_env/hook.sh
+-rw-r--r--   0        0        0     1482 1980-01-01 00:00:00.000000 redshift_client-2.0.0/build/dev_env/vs_settings.py
+-rw-r--r--   0        0        0      210 1980-01-01 00:00:00.000000 redshift_client-2.0.0/build/generic_builder/check.nix
+-rw-r--r--   0        0        0      341 1980-01-01 00:00:00.000000 redshift_client-2.0.0/build/generic_builder/default.nix
+-rw-r--r--   0        0        0      245 1980-01-01 00:00:00.000000 redshift_client-2.0.0/build/generic_builder/env.nix
+-rw-r--r--   0        0        0      309 1980-01-01 00:00:00.000000 redshift_client-2.0.0/build/generic_builder/metadata.nix
+-rwxr-xr-x   0        0        0      127 1980-01-01 00:00:00.000000 redshift_client-2.0.0/build/generic_builder/pkg/check/tests.sh
+-rwxr-xr-x   0        0        0      160 1980-01-01 00:00:00.000000 redshift_client-2.0.0/build/generic_builder/pkg/check/types.sh
+-rw-r--r--   0        0        0      625 1980-01-01 00:00:00.000000 redshift_client-2.0.0/build/generic_builder/pkg/default.nix
+-rw-r--r--   0        0        0     3034 1980-01-01 00:00:00.000000 redshift_client-2.0.0/flake.lock
+-rw-r--r--   0        0        0     1672 1980-01-01 00:00:00.000000 redshift_client-2.0.0/flake.nix
+-rw-r--r--   0        0        0      122 1980-01-01 00:00:00.000000 redshift_client-2.0.0/makes.lock.nix
+-rw-r--r--   0        0        0      674 1980-01-01 00:00:00.000000 redshift_client-2.0.0/makes.nix
+-rw-r--r--   0        0        0      714 1980-01-01 00:00:00.000000 redshift_client-2.0.0/mypy.ini
+-rw-r--r--   0        0        0      260 1980-01-01 00:00:00.000000 redshift_client-2.0.0/nix.conf
+-rw-r--r--   0        0        0      514 1980-01-01 00:00:00.000000 redshift_client-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0       22 1980-01-01 00:00:00.000000 redshift_client-2.0.0/redshift_client/__init__.py
+-rw-r--r--   0        0        0       82 1980-01-01 00:00:00.000000 redshift_client-2.0.0/redshift_client/client/__init__.py
+-rw-r--r--   0        0        0     7120 1980-01-01 00:00:00.000000 redshift_client-2.0.0/redshift_client/client/schema.py
+-rw-r--r--   0        0        0    10682 1980-01-01 00:00:00.000000 redshift_client-2.0.0/redshift_client/client/table/__init__.py
+-rw-r--r--   0        0        0     1575 1980-01-01 00:00:00.000000 redshift_client-2.0.0/redshift_client/client/table/_assert.py
+-rw-r--r--   0        0        0      283 1980-01-01 00:00:00.000000 redshift_client-2.0.0/redshift_client/client/table/_encode.py
+-rw-r--r--   0        0        0     1925 1980-01-01 00:00:00.000000 redshift_client-2.0.0/redshift_client/client/table/_new.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-2.0.0/redshift_client/core/__init__.py
+-rw-r--r--   0        0        0      508 1980-01-01 00:00:00.000000 redshift_client-2.0.0/redshift_client/core/column.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-2.0.0/redshift_client/core/data_type/__init__.py
+-rw-r--r--   0        0        0     1589 1980-01-01 00:00:00.000000 redshift_client-2.0.0/redshift_client/core/data_type/alias.py
+-rw-r--r--   0        0        0     1585 1980-01-01 00:00:00.000000 redshift_client-2.0.0/redshift_client/core/data_type/core.py
+-rw-r--r--   0        0        0     1565 1980-01-01 00:00:00.000000 redshift_client-2.0.0/redshift_client/core/data_type/decode.py
+-rw-r--r--   0        0        0      843 1980-01-01 00:00:00.000000 redshift_client-2.0.0/redshift_client/core/id_objs.py
+-rw-r--r--   0        0        0      589 1980-01-01 00:00:00.000000 redshift_client-2.0.0/redshift_client/core/schema.py
+-rw-r--r--   0        0        0     5401 1980-01-01 00:00:00.000000 redshift_client-2.0.0/redshift_client/core/table.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-2.0.0/redshift_client/py.typed
+-rw-r--r--   0        0        0     4410 1980-01-01 00:00:00.000000 redshift_client-2.0.0/redshift_client/sql_client/__init__.py
+-rw-r--r--   0        0        0     1046 1980-01-01 00:00:00.000000 redshift_client-2.0.0/redshift_client/sql_client/_assert.py
+-rw-r--r--   0        0        0     2381 1980-01-01 00:00:00.000000 redshift_client-2.0.0/redshift_client/sql_client/connection.py
+-rw-r--r--   0        0        0     1534 1980-01-01 00:00:00.000000 redshift_client-2.0.0/redshift_client/sql_client/primitive.py
+-rw-r--r--   0        0        0     1236 1980-01-01 00:00:00.000000 redshift_client-2.0.0/redshift_client/sql_client/query.py
+-rw-r--r--   0        0        0     1022 1980-01-01 00:00:00.000000 redshift_client-2.0.0/redshift_client/utils.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-2.0.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-2.0.0/tests/arch/__init__.py
+-rw-r--r--   0        0        0     1655 1980-01-01 00:00:00.000000 redshift_client-2.0.0/tests/arch/arch.py
+-rw-r--r--   0        0        0     1055 1980-01-01 00:00:00.000000 redshift_client-2.0.0/tests/arch/test_arch.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-2.0.0/tests/py.typed
+-rw-r--r--   0        0        0      233 1980-01-01 00:00:00.000000 redshift_client-2.0.0/tests/test_column.py
+-rw-r--r--   0        0        0      394 1970-01-01 00:00:00.000000 redshift_client-2.0.0/PKG-INFO
```

### Comparing `redshift_client-1.2.2/.gitlab-ci.yml` & `redshift_client-2.0.0/.gitlab-ci.yml`

 * *Files 13% similar despite different names*

```diff
@@ -39,28 +39,28 @@
 
 .new_version: &new_version
   rules:
     - if: '$CI_COMMIT_TAG =~ /^v\d+\.\d+\.\d+$/'
       when: on_success
 
 format-code:
-  image: ghcr.io/fluidattacks/makes:21.11
+  image: ghcr.io/fluidattacks/makes/amd64:23.06
   stage: lint
   <<: *in_dev_branch
   script:
     - m . /formatPython
 
 lint-nix:
-  image: ghcr.io/fluidattacks/makes:21.11
+  image: ghcr.io/fluidattacks/makes/amd64:23.06
   stage: lint
   <<: *in_dev_branch
   script: m . /formatNix && m . /lintNix
 
 lint-bash:
-  image: ghcr.io/fluidattacks/makes:21.11
+  image: ghcr.io/fluidattacks/makes/amd64:23.06
   stage: lint
   <<: *in_dev_branch
   script: m . /formatBash && m . /lintBash
 
 build-for-python38:
   <<: *with_nix
   <<: *in_dev_branch
```

### Comparing `redshift_client-1.2.2/build/default.nix` & `redshift_client-2.0.0/build/default.nix`

 * *Files identical despite different names*

### Comparing `redshift_client-1.2.2/build/deps/default.nix` & `redshift_client-2.0.0/build/deps/default.nix`

 * *Files identical despite different names*

### Comparing `redshift_client-1.2.2/build/deps/override_utils.nix` & `redshift_client-2.0.0/build/deps/override_utils.nix`

 * *Files identical despite different names*

### Comparing `redshift_client-1.2.2/build/dev_env/vs_settings.py` & `redshift_client-2.0.0/build/dev_env/vs_settings.py`

 * *Files identical despite different names*

### Comparing `redshift_client-1.2.2/build/generic_builder/pkg/default.nix` & `redshift_client-2.0.0/build/generic_builder/pkg/default.nix`

 * *Files identical despite different names*

### Comparing `redshift_client-1.2.2/flake.lock` & `redshift_client-2.0.0/flake.lock`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.998015873015873%*

 * *Differences: {"'nodes'": "{'arch-lint': {'locked': {'lastModified': 1685371599, 'narHash': "*

 * *            "'sha256-DcOPPeAKrjdev/2K1o3pnZUL2+nggMmqa6uJ5An9IxA=', 'rev': "*

 * *            "'72a495bb933f052ad812292b468ca3e18fd9dde4'}, 'original': {delete: ['ref']}}, "*

 * *            "'fa-purity': {'locked': {'lastModified': 1685212251, 'narHash': "*

 * *            "'sha256-b/2MMuPOFcfgyJpoGJg/71lNMUhoLiv3lpN3MUAH4Ag=', 'rev': "*

 * *            "'feaa69ef3ad93ad91fd679d8169c80458457d779'}, 'original': {delete: ['ref']}}}"}*

```diff
@@ -4,46 +4,44 @@
             "inputs": {
                 "nix_filter": "nix_filter",
                 "nixpkgs": [
                     "nixpkgs"
                 ]
             },
             "locked": {
-                "lastModified": 1683562176,
-                "narHash": "sha256-dlbR1p3lGlyJbr02EhOT11Mv0MfV7Rdqx81UYsd4I6M=",
+                "lastModified": 1685371599,
+                "narHash": "sha256-DcOPPeAKrjdev/2K1o3pnZUL2+nggMmqa6uJ5An9IxA=",
                 "owner": "dmurciaatfluid",
                 "repo": "arch_lint",
-                "rev": "067d033fc82af3142b9faf6fb307c8812210873b",
+                "rev": "72a495bb933f052ad812292b468ca3e18fd9dde4",
                 "type": "gitlab"
             },
             "original": {
                 "owner": "dmurciaatfluid",
-                "ref": "v2.4.0",
                 "repo": "arch_lint",
                 "type": "gitlab"
             }
         },
         "fa-purity": {
             "inputs": {
                 "nix_filter": "nix_filter_2",
                 "nixpkgs": [
                     "nixpkgs"
                 ]
             },
             "locked": {
-                "lastModified": 1683067095,
-                "narHash": "sha256-PXtAE7mLIlr6urKo+yH+Vwjf4cL+NwjNxa0YhjwQR/4=",
+                "lastModified": 1685212251,
+                "narHash": "sha256-b/2MMuPOFcfgyJpoGJg/71lNMUhoLiv3lpN3MUAH4Ag=",
                 "owner": "dmurciaatfluid",
                 "repo": "purity",
-                "rev": "a89d23efd5ee2b2b49b951f187448a1afc6565a3",
+                "rev": "feaa69ef3ad93ad91fd679d8169c80458457d779",
                 "type": "gitlab"
             },
             "original": {
                 "owner": "dmurciaatfluid",
-                "ref": "v1.33.2",
                 "repo": "purity",
                 "type": "gitlab"
             }
         },
         "nix_filter": {
             "locked": {
                 "lastModified": 1645371475,
```

### Comparing `redshift_client-1.2.2/flake.nix` & `redshift_client-2.0.0/flake.nix`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 {
   description = "Redshift client-SDK";
   inputs = {
     arch-lint = {
-      url = "gitlab:dmurciaatfluid/arch_lint/v2.4.0";
+      url = "gitlab:dmurciaatfluid/arch_lint";
       inputs.nixpkgs.follows = "nixpkgs";
     };
     fa-purity = {
-      url = "gitlab:dmurciaatfluid/purity/v1.33.2";
+      url = "gitlab:dmurciaatfluid/purity";
       inputs.nixpkgs.follows = "nixpkgs";
     };
     nix_filter.url = "github:numtide/nix-filter";
     nixpkgs.url = "github:nixos/nixpkgs?rev=0cd51a933d91078775b300cf0f29aa3495231aa2";
   };
   outputs = {
     self,
```

### Comparing `redshift_client-1.2.2/makes.nix` & `redshift_client-2.0.0/makes.nix`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # https://github.com/fluidattacks/makes
 {
   cache = {
-    readAndWrite = {
-      enable = true;
-      name = "fa-foss";
-      pubKey = "fa-foss.cachix.org-1:RoFAjJdHUUFrNAfbaLFqvFQVfmNmyMMAorl7j2VqV9M=";
+    readNixos = true;
+    extra = {
+      fa-foss = {
+        enable = true;
+        pubKey = "fa-foss.cachix.org-1:RoFAjJdHUUFrNAfbaLFqvFQVfmNmyMMAorl7j2VqV9M=";
+        type = "cachix";
+        token = "CACHIX_AUTH_TOKEN";
+        url = "https://fa-foss.cachix.org";
+        write = true;
+      };
     };
   };
   formatBash = {
     enable = true;
     targets = ["/"];
   };
   formatNix = {
```

### Comparing `redshift_client-1.2.2/mypy.ini` & `redshift_client-2.0.0/mypy.ini`

 * *Files identical despite different names*

### Comparing `redshift_client-1.2.2/pyproject.toml` & `redshift_client-2.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `redshift_client-1.2.2/redshift_client/data_type/alias.py` & `redshift_client-2.0.0/redshift_client/core/data_type/alias.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from fa_purity.frozen import (
     FrozenDict,
 )
-from redshift_client.data_type.core import (
+from redshift_client.core.data_type.core import (
     DataType,
     NonStcDataTypes,
     PrecisionType,
     PrecisionTypes,
     ScaleTypes,
     StaticTypes,
 )
```

### Comparing `redshift_client-1.2.2/redshift_client/data_type/decode.py` & `redshift_client-2.0.0/redshift_client/core/data_type/decode.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from fa_purity.maybe import (
     Maybe,
 )
 from fa_purity.utils import (
     raise_exception,
 )
-from redshift_client.data_type.alias import (
+from redshift_client.core.data_type.alias import (
     NON_STC_ALIAS_MAP,
     STC_ALIAS_MAP,
 )
-from redshift_client.data_type.core import (
+from redshift_client.core.data_type.core import (
     DataType,
     DecimalType,
     NonStcDataTypes,
     PrecisionType,
     PrecisionTypes,
     ScaleTypes,
     StaticTypes,
```

### Comparing `redshift_client-1.2.2/redshift_client/schema/client.py` & `redshift_client-2.0.0/redshift_client/client/schema.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,36 +15,38 @@
 )
 from fa_purity.pure_iter.transform import (
     consume,
 )
 from fa_purity.utils import (
     raise_exception,
 )
-from redshift_client.id_objs import (
+from redshift_client.client.table import (
+    TableClient,
+)
+from redshift_client.core.id_objs import (
+    DbTableId,
+    Identifier,
     SchemaId,
     TableId,
 )
-from redshift_client.schema.core import (
+from redshift_client.core.schema import (
     Quota,
     SchemaPolicy,
 )
 from redshift_client.sql_client import (
     QueryValues,
     SqlClient,
 )
 from redshift_client.sql_client.primitive import (
     PrimitiveVal,
 )
 from redshift_client.sql_client.query import (
     dynamic_query,
     new_query,
 )
-from redshift_client.table.client import (
-    TableClient,
-)
 from typing import (
     Callable,
     Dict,
     FrozenSet,
     TypeVar,
 )
 
@@ -69,55 +71,64 @@
             "ORDER BY table_schema",
         )
         stm = " ".join(_stm)
         return self._db_client.execute(
             new_query(stm), None
         ) + self._db_client.fetch_all().map(
             lambda i: frozenset(
-                SchemaId(to_primitive(e.data[0], str).unwrap()) for e in i
+                SchemaId(Identifier.new(to_primitive(e.data[0], str).unwrap()))
+                for e in i
             )
         )
 
-    def table_ids(self, schema: SchemaId) -> Cmd[FrozenSet[TableId]]:
+    def table_ids(self, schema: SchemaId) -> Cmd[FrozenSet[DbTableId]]:
         _stm = (
             "SELECT tables.table_name FROM information_schema.tables",
             "WHERE table_schema = %(schema_name)s",
         )
         stm = " ".join(_stm)
-        args: Dict[str, PrimitiveVal] = {"schema_name": schema.name}
+        args: Dict[str, PrimitiveVal] = {"schema_name": schema.name.to_str()}
         return self._db_client.execute(
             new_query(stm), QueryValues(FrozenDict(args))
         ) + self._db_client.fetch_all().map(
             lambda i: frozenset(
-                TableId(schema, to_primitive(e.data[0], str).unwrap())
+                DbTableId(
+                    schema,
+                    TableId(
+                        Identifier.new(to_primitive(e.data[0], str).unwrap())
+                    ),
+                )
                 for e in i
             )
         )
 
     def exist(self, schema: SchemaId) -> Cmd[bool]:
         _stm = (
             "SELECT EXISTS",
             "(SELECT 1 FROM pg_namespace",
             "WHERE nspname = %(schema_name)s)",
         )
         stm = " ".join(_stm)
-        args: Dict[str, PrimitiveVal] = {"schema_name": schema.name}
+        args: Dict[str, PrimitiveVal] = {"schema_name": schema.name.to_str()}
         return self._db_client.execute(
             new_query(stm), QueryValues(FrozenDict(args))
         ) + self._db_client.fetch_one().map(lambda x: x.value_or(None)).map(
             lambda i: _assert_bool(i.data[0])
             if i is not None
             else raise_exception(TypeError("Expected not None"))
         )
 
     def _delete(self, schema: SchemaId, cascade: bool) -> Cmd[None]:
         opt = " CASCADE" if cascade else ""
         stm: str = "DROP SCHEMA {schema_name}" + opt
         return self._db_client.execute(
-            dynamic_query(stm, FrozenDict({"schema_name": schema.name})), None
+            dynamic_query(
+                stm, FrozenDict({"schema_name": schema.name.to_str()})
+            ),
+            None,
         )
 
     def delete(self, schema: SchemaId) -> Cmd[None]:
         return self._delete(schema, False)
 
     def delete_cascade(self, schema: SchemaId) -> Cmd[None]:
         return self._delete(schema, True)
@@ -125,29 +136,30 @@
     def rename(self, old: SchemaId, new: SchemaId) -> Cmd[None]:
         stm = "ALTER SCHEMA {from_schema} RENAME TO {to_schema}"
         return self._db_client.execute(
             dynamic_query(
                 stm,
                 FrozenDict(
                     {
-                        "from_schema": old.name,
-                        "to_schema": new.name,
+                        "from_schema": old.name.to_str(),
+                        "to_schema": new.name.to_str(),
                     }
                 ),
             ),
             None,
         )
 
     def create(
         self, schema: SchemaId, if_not_exist: bool = False
     ) -> Cmd[None]:
         not_exist = " IF NOT EXISTS " if if_not_exist else ""
         stm = f"CREATE SCHEMA {not_exist} {{schema}}"
         return self._db_client.execute(
-            dynamic_query(stm, FrozenDict({"schema": schema.name})), None
+            dynamic_query(stm, FrozenDict({"schema": schema.name.to_str()})),
+            None,
         )
 
     def _recreate(self, schema: SchemaId, cascade: bool) -> Cmd[None]:
         nothing = Cmd.from_cmd(lambda: None)
         return self.exist(schema).bind(
             lambda b: self._delete(schema, cascade) if b else nothing
         ) + self.create(schema)
@@ -158,22 +170,22 @@
     def recreate_cascade(self, schema: SchemaId) -> Cmd[None]:
         return self._recreate(schema, True)
 
     def _move(
         self,
         source: SchemaId,
         target: SchemaId,
-        move_op: Callable[[TableId, TableId], Cmd[None]],
+        move_op: Callable[[DbTableId, DbTableId], Cmd[None]],
     ) -> Cmd[None]:
         return (
             self.table_ids(source)
             .map(lambda x: from_flist(tuple(x)))
             .bind(
                 lambda p: p.map(
-                    lambda t: move_op(t, TableId(target, t.name))
+                    lambda t: move_op(t, DbTableId(target, t.table))
                 ).transform(lambda x: consume(x))
             )
         ) + self.delete(source)
 
     def migrate(self, source: SchemaId, target: SchemaId) -> Cmd[None]:
         """
         Moves all tables from `source` to `target` overwriting `target` data.
@@ -196,19 +208,22 @@
         stm2 = (
             f"ALTER SCHEMA {{schema}} QUOTA %(quota)s {policy.quota.unit.value}"
             if isinstance(policy.quota, Quota)
             else "ALTER SCHEMA {schema} QUOTA UNLIMITED"
         )
         set_owner = self._db_client.execute(
             dynamic_query(
-                stm, FrozenDict({"schema": schema.name, "owner": policy.owner})
+                stm,
+                FrozenDict(
+                    {"schema": schema.name.to_str(), "owner": policy.owner}
+                ),
             ),
             None,
         )
-        id_args: Dict[str, str] = {"schema": schema.name}
+        id_args: Dict[str, str] = {"schema": schema.name.to_str()}
         args: Dict[str, PrimitiveVal] = (
             {"quota": policy.quota.value}
             if isinstance(policy.quota, Quota)
             else {}
         )
         set_quota = self._db_client.execute(
             dynamic_query(stm2, FrozenDict(id_args)),
```

### Comparing `redshift_client-1.2.2/redshift_client/schema/core.py` & `redshift_client-2.0.0/redshift_client/core/schema.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
+from .table import (
+    Table,
+)
 from dataclasses import (
     dataclass,
 )
 from enum import (
     Enum,
 )
 from fa_purity.frozen import (
     FrozenDict,
 )
-from redshift_client.id_objs import (
+from redshift_client.core.id_objs import (
     TableId,
 )
-from redshift_client.table.core import (
-    Table,
-)
 from typing import (
     Literal,
     Union,
 )
 
 
 @dataclass(frozen=True)
```

### Comparing `redshift_client-1.2.2/redshift_client/sql_client/__init__.py` & `redshift_client-2.0.0/redshift_client/sql_client/__init__.py`

 * *Files identical despite different names*

### Comparing `redshift_client-1.2.2/redshift_client/sql_client/_assert.py` & `redshift_client-2.0.0/redshift_client/sql_client/_assert.py`

 * *Files identical despite different names*

### Comparing `redshift_client-1.2.2/redshift_client/sql_client/connection.py` & `redshift_client-2.0.0/redshift_client/sql_client/connection.py`

 * *Files identical despite different names*

### Comparing `redshift_client-1.2.2/redshift_client/sql_client/primitive.py` & `redshift_client-2.0.0/redshift_client/sql_client/primitive.py`

 * *Files identical despite different names*

### Comparing `redshift_client-1.2.2/redshift_client/sql_client/query.py` & `redshift_client-2.0.0/redshift_client/sql_client/query.py`

 * *Files identical despite different names*

### Comparing `redshift_client-1.2.2/redshift_client/table/client.py` & `redshift_client-2.0.0/redshift_client/client/table/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,17 @@
+from . import (
+    _encode,
+    _new,
+)
+from ._assert import (
+    to_column,
+)
 from dataclasses import (
     dataclass,
 )
-from deprecated import (
-    deprecated,
-)
 from fa_purity import (
     PureIter,
 )
 from fa_purity.cmd import (
     Cmd,
 )
 from fa_purity.frozen import (
@@ -16,101 +20,87 @@
 )
 from fa_purity.pure_iter.factory import (
     from_flist,
 )
 from fa_purity.pure_iter.transform import (
     consume,
 )
-from redshift_client.column import (
+from redshift_client.core.column import (
     Column,
     ColumnId,
     ColumnObj,
 )
-from redshift_client.data_type.core import (
-    DataType,
-    PrecisionType,
-    StaticTypes,
-)
-from redshift_client.id_objs import (
+from redshift_client.core.id_objs import (
+    DbTableId,
+    Identifier,
     TableId,
 )
+from redshift_client.core.table import (
+    ManifestId,
+    Table,
+    TableAttrs,
+)
 from redshift_client.sql_client import (
     QueryValues,
     RowData,
     SqlClient,
 )
 from redshift_client.sql_client.primitive import (
     PrimitiveVal,
 )
 from redshift_client.sql_client.query import (
     dynamic_query,
     new_query,
 )
-from redshift_client.table._assert import (
-    to_column,
-)
-from redshift_client.table.core import (
-    new as new_table,
-    Table,
-)
 from typing import (
-    Callable,
     Dict,
     TypeVar,
 )
 
 _T = TypeVar("_T")
 
 
 def _assert_bool(raw: _T) -> bool:
     if isinstance(raw, bool):
         return raw
     raise TypeError("Expected bool")
 
 
 @dataclass(frozen=True)
-class ManifestId:
-    uri: str
-
-
-def _encode_data_type(d_type: DataType) -> str:
-    if isinstance(d_type.value, StaticTypes):
-        return d_type.value.value
-    if isinstance(d_type.value, PrecisionType):
-        return f"{d_type.value.data_type.value}({d_type.value.precision})"
-    return f"DECIMAL({d_type.value.precision},{d_type.value.scale})"
-
-
-@dataclass(frozen=True)
 class TableClient:
     _db_client: SqlClient
 
     def unload(
-        self, table: TableId, prefix: str, role: str
+        self, table: DbTableId, prefix: str, role: str
     ) -> Cmd[ManifestId]:
         """
         prefix: a s3 uri prefix
         role: an aws role id-arn
         """
         stm = """
             UNLOAD ('SELECT * FROM {schema}.{table}')
             TO %(prefix)s iam_role %(role)s MANIFEST ESCAPE
         """
         args: Dict[str, PrimitiveVal] = {"prefix": prefix, "role": role}
         return self._db_client.execute(
             dynamic_query(
                 stm,
-                FrozenDict({"schema": table.schema.name, "table": table.name}),
+                FrozenDict(
+                    {
+                        "schema": table.schema.name.to_str(),
+                        "table": table.table.name.to_str(),
+                    }
+                ),
             ),
             QueryValues(FrozenDict(args)),
         ).map(lambda _: ManifestId(f"{prefix}manifest"))
 
     def load(
         self,
-        table: TableId,
+        table: DbTableId,
         manifest: ManifestId,
         role: str,
         nan_handler: bool = True,
     ) -> Cmd[None]:
         """
         If `nan_handler` is disabled, ensure that the table does not contain NaN values on float columns
         """
@@ -122,261 +112,229 @@
         args: Dict[str, PrimitiveVal] = {
             "manifest_file": manifest.uri,
             "role": role,
         }
         return self._db_client.execute(
             dynamic_query(
                 stm,
-                FrozenDict({"schema": table.schema.name, "table": table.name}),
+                FrozenDict(
+                    {
+                        "schema": table.schema.name.to_str(),
+                        "table": table.table.name.to_str(),
+                    }
+                ),
             ),
             QueryValues(FrozenDict(args)),
         )
 
-    def get(self, table: TableId) -> Cmd[Table]:
+    def get(self, table: DbTableId) -> Cmd[Table]:
         stm = """
             SELECT ordinal_position,
                 column_name,
                 data_type,
                 CASE WHEN character_maximum_length IS not null
                         THEN character_maximum_length
                         ELSE numeric_precision end AS max_length,
                 numeric_scale,
                 is_nullable,
                 column_default AS default_value
             FROM information_schema.columns
-            WHERE table_name = %(table_name)s
-                AND table_schema = %(table_schema)s
+            WHERE table_schema = %(table_schema)s
+                AND table_name = %(table_name)s
             ORDER BY ordinal_position
         """
         args: Dict[str, PrimitiveVal] = {
-            "table_schema": table.schema.name,
-            "table_name": table.name,
+            "table_schema": table.schema.name.to_str(),
+            "table_name": table.table.name.to_str(),
         }
         exe = self._db_client.execute(
             new_query(stm),
             QueryValues(FrozenDict(args)),
         )
         results = self._db_client.fetch_all()
 
         def _extract(raw: FrozenList[RowData]) -> Table:
             columns_pairs = tuple(to_column(column.data) for column in raw)
             columns = FrozenDict(dict(columns_pairs))
             order = tuple(i for i, _ in columns_pairs)
-            return new_table(order, columns, frozenset()).unwrap()
+            return Table.new(order, columns, frozenset()).unwrap()
 
         return (exe + results).map(_extract)
 
-    def exist(self, table_id: TableId) -> Cmd[bool]:
+    def exist(self, table: DbTableId) -> Cmd[bool]:
         stm = """
             SELECT EXISTS (
                 SELECT * FROM information_schema.tables
                 WHERE table_schema = %(table_schema)s
                 AND table_name = %(table_name)s
             );
         """
         args: Dict[str, PrimitiveVal] = {
-            "table_schema": table_id.schema.name,
-            "table_name": table_id.name,
+            "table_schema": table.schema.name.to_str(),
+            "table_name": table.table.name.to_str(),
         }
         return self._db_client.execute(
             new_query(stm), QueryValues(FrozenDict(args))
         ) + self._db_client.fetch_one().map(
             lambda m: m.map(lambda i: _assert_bool(i.data[0]))
             .to_result()
             .alt(lambda _: TypeError("Expected not None"))
             .unwrap()
         )
 
     def insert(
         self,
-        table_id: TableId,
+        table_id: DbTableId,
         table: Table,
         items: PureIter[RowData],
         limit: int,
     ) -> Cmd[None]:
         _fields = ",".join(f"{{field_{i}}}" for i, _ in enumerate(table.order))
         stm = f"""
             INSERT INTO {{schema}}.{{table}} ({_fields}) VALUES %s
         """
         identifiers: Dict[str, str] = {
-            "schema": table_id.schema.name,
-            "table": table_id.name,
+            "schema": table_id.schema.name.to_str(),
+            "table": table_id.table.name.to_str(),
         }
         for i, c in enumerate(table.order):
-            identifiers[f"field_{i}"] = c.name
+            identifiers[f"field_{i}"] = c.name.to_str()
         return self._db_client.values(
             dynamic_query(stm, FrozenDict(identifiers)), items, limit
         )
 
-    def rename(self, table_id: TableId, new_name: str) -> Cmd[TableId]:
+    def rename(self, table_id: DbTableId, new_name: str) -> Cmd[TableId]:
         stm = """
             ALTER TABLE {schema}.{table} RENAME TO {new_name}
         """
         identifiers: Dict[str, str] = {
-            "schema": table_id.schema.name,
-            "table": table_id.name,
+            "schema": table_id.schema.name.to_str(),
+            "table": table_id.table.name.to_str(),
             "new_name": new_name,
         }
         return self._db_client.execute(
             dynamic_query(stm, FrozenDict(identifiers)), None
-        ).map(lambda _: TableId(table_id.schema, new_name))
+        ).map(lambda _: TableId(Identifier.new(new_name)))
 
-    def _delete(self, table_id: TableId, cascade: bool) -> Cmd[None]:
+    def _delete(self, table_id: DbTableId, cascade: bool) -> Cmd[None]:
         _cascade = "CASCADE" if cascade else ""
         stm = f"""
             DROP TABLE {{schema}}.{{table}} {_cascade}
         """
         identifiers: Dict[str, str] = {
-            "schema": table_id.schema.name,
-            "table": table_id.name,
+            "schema": table_id.schema.name.to_str(),
+            "table": table_id.table.name.to_str(),
         }
         return self._db_client.execute(
             dynamic_query(stm, FrozenDict(identifiers)), None
         )
 
-    def delete(self, table_id: TableId) -> Cmd[None]:
+    def delete(self, table_id: DbTableId) -> Cmd[None]:
         return self._delete(table_id, False)
 
-    def delete_cascade(self, table_id: TableId) -> Cmd[None]:
+    def delete_cascade(self, table_id: DbTableId) -> Cmd[None]:
         return self._delete(table_id, True)
 
-    def add_column(self, table_id: TableId, column: ColumnObj) -> Cmd[None]:
+    def add_column(self, table_id: DbTableId, column: ColumnObj) -> Cmd[None]:
         stm = f"""
             ALTER TABLE {{table_schema}}.{{table_name}}
             ADD COLUMN {{column_name}}
-            {_encode_data_type(column.column.data_type)} DEFAULT %(default_val)s
+            {_encode.encode_data_type(column.column.data_type)} DEFAULT %(default_val)s
         """
         identifiers: Dict[str, str] = {
-            "table_schema": table_id.schema.name,
-            "table_name": table_id.name,
-            "column_name": column.id_obj.name,
+            "table_schema": table_id.schema.name.to_str(),
+            "table_name": table_id.table.name.to_str(),
+            "column_name": column.id_obj.name.to_str(),
         }
         args: Dict[str, PrimitiveVal] = {
             "default_val": column.column.default,
         }
         return self._db_client.execute(
             dynamic_query(stm, FrozenDict(identifiers)),
             QueryValues(FrozenDict(args)),
         )
 
     def add_columns(
         self,
-        table: TableId,
+        table: DbTableId,
         columns: FrozenDict[ColumnId, Column],
     ) -> Cmd[None]:
         return (
             from_flist(tuple(columns.items()))
             .map(lambda c: ColumnObj(c[0], c[1]))
             .map(lambda c: self.add_column(table, c))
             .transform(lambda x: consume(x))
         )
 
     def new(
-        self, table_id: TableId, table: Table, if_not_exist: bool = False
+        self,
+        table_id: DbTableId,
+        table: Table,
+        attrs: TableAttrs,
+        if_not_exist: bool = False,
     ) -> Cmd[None]:
-        enum_primary_keys = tuple(enumerate(table.primary_keys))
-        enum_columns = tuple(
-            enumerate(tuple((i, table.columns[i]) for i in table.order))
-        )
-        p_fields = ",".join([f"{{pkey_{i}}}" for i, _ in enum_primary_keys])
-        pkeys_template = (
-            f",PRIMARY KEY({p_fields})" if table.primary_keys else ""
-        )
-        not_exists = "" if not if_not_exist else "IF NOT EXISTS"
-        encode_nullable: Callable[[bool], str] = (
-            lambda b: "NULL" if b else "NOT NULL"
-        )
-        fields_template: str = ",".join(
-            [
-                f"""
-                    {{name_{n}}} {_encode_data_type(c.data_type)}
-                    DEFAULT %(default_{n})s {encode_nullable(c.nullable)}
-                """
-                for n, (_, c) in enum_columns
-            ]
-        )
-        stm = f"CREATE TABLE {not_exists} {{schema}}.{{table}} ({fields_template}{pkeys_template})"
-        identifiers: Dict[str, str] = {
-            "schema": table_id.schema.name,
-            "table": table_id.name,
-        }
-        for index, cid in enum_primary_keys:
-            identifiers[f"pkey_{index}"] = cid.name
-        for index, (cid, _) in enum_columns:
-            identifiers[f"name_{index}"] = cid.name
-        values = FrozenDict(
-            {f"default_{index}": c.default for index, (_, c) in enum_columns}
-        )
-        return self._db_client.execute(
-            dynamic_query(stm, FrozenDict(identifiers)), QueryValues(values)
-        )
+        return _new.new(self._db_client, table_id, table, if_not_exist)
 
-    def create_like(self, blueprint: TableId, new_table: TableId) -> Cmd[None]:
+    def create_like(
+        self, blueprint: DbTableId, new_table: DbTableId
+    ) -> Cmd[None]:
         stm = """
             CREATE TABLE {new_schema}.{new_table} (
                 LIKE {blueprint_schema}.{blueprint_table}
             )
         """
         identifiers: Dict[str, str] = {
-            "new_schema": new_table.schema.name,
-            "new_table": new_table.name,
-            "blueprint_schema": blueprint.schema.name,
-            "blueprint_table": blueprint.name,
+            "blueprint_schema": blueprint.schema.name.to_str(),
+            "blueprint_table": blueprint.table.name.to_str(),
+            "new_schema": new_table.schema.name.to_str(),
+            "new_table": new_table.table.name.to_str(),
         }
         return self._db_client.execute(
             dynamic_query(stm, FrozenDict(identifiers)), None
         )
 
-    def move_data(self, source: TableId, target: TableId) -> Cmd[None]:
+    def move_data(self, source: DbTableId, target: DbTableId) -> Cmd[None]:
         """
         This method moves data from source to target.
-        After the operation source will be empty.
-        Both tables must exists.
+        - After the operation source will be empty.
+        - Both tables must exists.
         """
         stm = """
             ALTER TABLE {target_schema}.{target_table}
             APPEND FROM {source_schema}.{source_table}
         """
         identifiers: Dict[str, str] = {
-            "source_schema": source.schema.name,
-            "source_table": source.name,
-            "target_schema": target.schema.name,
-            "target_table": target.name,
+            "source_schema": source.schema.name.to_str(),
+            "source_table": source.table.name.to_str(),
+            "target_schema": target.schema.name.to_str(),
+            "target_table": target.table.name.to_str(),
         }
         return self._db_client.execute(
             dynamic_query(stm, FrozenDict(identifiers)), None
         )
 
-    @deprecated(reason="Renamed method, use 'move_data' instead")  # type: ignore[misc]
-    def append(self, source: TableId, target: TableId) -> Cmd[None]:
-        return self.move_data(source, target)
-
-    def move(self, source: TableId, target: TableId) -> Cmd[None]:
+    def move(self, source: DbTableId, target: DbTableId) -> Cmd[None]:
         """
         - create target if not exist
         - move_data (append) data from source into target
-        - delete source table
+        - delete source table (that will be empty)
         """
         nothing = Cmd.from_cmd(lambda: None)
         create = self.exist(target).bind(
             lambda b: self.create_like(source, target) if not b else nothing
         )
         return (
             create
             + self.move_data(source, target)
             + self.delete_cascade(source)
         )
 
-    def migrate(self, source: TableId, target: TableId) -> Cmd[None]:
+    def migrate(self, source: DbTableId, target: DbTableId) -> Cmd[None]:
         """
         - delete target if exist
         - move source into target (see move method)
         """
         nothing = Cmd.from_cmd(lambda: None)
         delete = self.exist(target).bind(
             lambda b: self.delete_cascade(target) if b else nothing
         )
         return delete + self.move(source, target)
-
-    @deprecated(reason="Renamed method, use 'migrate' instead")  # type: ignore[misc]
-    def overwrite(self, source: TableId, target: TableId) -> Cmd[None]:
-        return self.migrate(source, target)
```

### Comparing `redshift_client-1.2.2/redshift_client/table/core.py` & `redshift_client-2.0.0/redshift_client/client/table/_assert.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,70 @@
-from dataclasses import (
-    dataclass,
-)
 from fa_purity.frozen import (
-    FrozenDict,
     FrozenList,
 )
+from fa_purity.maybe import (
+    Maybe,
+)
 from fa_purity.result import (
     Result,
     ResultE,
 )
-from redshift_client.column import (
+from fa_purity.utils import (
+    raise_exception,
+)
+from redshift_client.core.column import (
     Column,
     ColumnId,
 )
+from redshift_client.core.data_type.decode import (
+    decode_type,
+)
+from redshift_client.core.id_objs import (
+    Identifier,
+)
+from redshift_client.sql_client.primitive import (
+    PrimitiveVal,
+)
 from typing import (
-    Callable,
-    FrozenSet,
+    Optional,
+    Tuple,
+    TypeVar,
 )
 
+_T = TypeVar("_T")
+
+
+def _to_opt(item: _T) -> Optional[_T]:
+    return item
+
 
-@dataclass(frozen=True)
-class _Table:
-    order: FrozenList[ColumnId]
-    columns: FrozenDict[ColumnId, Column]
-    primary_keys: FrozenSet[ColumnId]
-
-
-@dataclass(frozen=True)
-class Table(_Table):
-    def __init__(self, obj: _Table) -> None:
-        super().__init__(obj.order, obj.columns, obj.primary_keys)
-
-
-def new(
-    order: FrozenList[ColumnId],
-    columns: FrozenDict[ColumnId, Column],
-    primary_keys: FrozenSet[ColumnId],
-) -> ResultE[Table]:
-    in_columns: Callable[[ColumnId], bool] = lambda k: k in columns
-    non_duplicated = len(frozenset(order)) == len(order)
-    if not non_duplicated:
-        return Result.failure(
-            Exception("order list must have unique `ColumnId` objs")
-        )
-    if all(map(in_columns, primary_keys)):
-        draft = _Table(order, columns, primary_keys)
-        return Result.success(Table(draft))
-    return Result.failure(Exception("All primary keys must be in columns"))
+def _assert_opt_int(val: PrimitiveVal) -> ResultE[Optional[int]]:
+    if isinstance(val, (int, str)):
+        try:
+            return Result.success(_to_opt(int(val)))
+        except ValueError as err:
+            return Result.failure(Exception(err))
+    if val is None:
+
+        def none() -> Optional[int]:
+            return None
+
+        return Result.success(none())
+    error = ValueError("not a int|str")
+    return Result.failure(Exception(error))
+
+
+def to_column(raw: FrozenList[PrimitiveVal]) -> Tuple[ColumnId, Column]:
+    col = Column(
+        decode_type(
+            str(raw[2]),
+            Maybe.from_optional(
+                _assert_opt_int(raw[3]).alt(raise_exception).unwrap()
+            ),
+            Maybe.from_optional(
+                _assert_opt_int(raw[4]).alt(raise_exception).unwrap()
+            ),
+        ),
+        str(raw[5]).upper() == "YES",
+        raw[6],
+    )
+    return (ColumnId(Identifier.new(str(raw[1]))), col)
```

### Comparing `redshift_client-1.2.2/tests/arch/arch.py` & `redshift_client-2.0.0/tests/arch/arch.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,39 +12,43 @@
     FrozenSet,
     TypeVar,
     Union,
 )
 
 _dag: Dict[str, FrozenList[Union[FrozenList[str], str]]] = {
     "redshift_client": (
+        "client",
+        "core",
+        "sql_client",
+        "utils",
+    ),
+    "redshift_client.core": (
         "schema",
         "table",
         "column",
-        "data_type",
-        "id_objs",
-        "sql_client",
+        ("data_type", "id_objs"),
     ),
-    "redshift_client.sql_client": (
-        ("connection", "query"),
-        "_assert",
-        "primitive",
-    ),
-    "redshift_client.schema": (
-        "client",
+    "redshift_client.core.data_type": (
+        "decode",
+        "alias",
         "core",
     ),
-    "redshift_client.table": (
-        "client",
-        "core",
+    "redshift_client.client": (
+        "schema",
+        "table",
+    ),
+    "redshift_client.client.table": (
+        "_new",
+        "_encode",
         "_assert",
     ),
-    "redshift_client.data_type": (
-        "decode",
-        "alias",
-        "core",
+    "redshift_client.sql_client": (
+        ("connection", "query"),
+        "_assert",
+        "primitive",
     ),
 }
 _T = TypeVar("_T")
 
 
 def raise_or_return(item: Union[Exception, _T]) -> _T:
     if isinstance(item, Exception):
```

### Comparing `redshift_client-1.2.2/tests/arch/test_arch.py` & `redshift_client-2.0.0/tests/arch/test_arch.py`

 * *Files identical despite different names*

