# Comparing `tmp/Marl-Factory-Grid-0.0.7.tar.gz` & `tmp/Marl-Factory-Grid-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Marl-Factory-Grid-0.0.7.tar", last modified: Tue Jun 20 16:25:10 2023, max compression
+gzip compressed data, was "Marl-Factory-Grid-0.0.8.tar", last modified: Wed Jun 21 09:29:12 2023, max compression
```

## Comparing `Marl-Factory-Grid-0.0.7.tar` & `Marl-Factory-Grid-0.0.8.tar`

### file list

```diff
@@ -1,166 +1,169 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.034140 Marl-Factory-Grid-0.0.7/
--rw-rw-rw-   0 root         (0) root         (0)      453 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)       45 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/MANIFEST.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.022140 Marl-Factory-Grid-0.0.7/Marl_Factory_Grid.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4328 2023-06-20 16:25:09.000000 Marl-Factory-Grid-0.0.7/Marl_Factory_Grid.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5413 2023-06-20 16:25:10.000000 Marl-Factory-Grid-0.0.7/Marl_Factory_Grid.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 16:25:09.000000 Marl-Factory-Grid-0.0.7/Marl_Factory_Grid.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-20 16:25:09.000000 Marl-Factory-Grid-0.0.7/Marl_Factory_Grid.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-06-20 16:25:09.000000 Marl-Factory-Grid-0.0.7/Marl_Factory_Grid.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     4328 2023-06-20 16:25:10.034140 Marl-Factory-Grid-0.0.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3625 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.022140 Marl-Factory-Grid-0.0.7/images/
--rw-rw-rw-   0 root         (0) root         (0)   303396 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/images/Hooks_FIKS.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.022140 Marl-Factory-Grid-0.0.7/mfg_package/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 16:25:03.000000 Marl-Factory-Grid-0.0.7/mfg_package/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.022140 Marl-Factory-Grid-0.0.7/mfg_package/algorithms/
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/algorithms/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.022140 Marl-Factory-Grid-0.0.7/mfg_package/algorithms/marl/
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/algorithms/marl/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8698 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/algorithms/marl/base_ac.py
--rw-rw-rw-   0 root         (0) root         (0)      636 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/algorithms/marl/example_config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2107 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/algorithms/marl/iac.py
--rw-rw-rw-   0 root         (0) root         (0)     3184 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/algorithms/marl/mappo.py
--rw-rw-rw-   0 root         (0) root         (0)     7763 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/algorithms/marl/memory.py
--rw-rw-rw-   0 root         (0) root         (0)     4784 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/algorithms/marl/networks.py
--rw-rw-rw-   0 root         (0) root         (0)     2261 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/algorithms/marl/seac.py
--rw-rw-rw-   0 root         (0) root         (0)     1293 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/algorithms/marl/snac.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.022140 Marl-Factory-Grid-0.0.7/mfg_package/algorithms/static/
--rw-rw-rw-   0 root         (0) root         (0)     5319 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/algorithms/static/TSP_base_agent.py
--rw-rw-rw-   0 root         (0) root         (0)     1057 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/algorithms/static/TSP_dirt_agent.py
--rw-rw-rw-   0 root         (0) root         (0)     2375 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/algorithms/static/TSP_item_agent.py
--rw-rw-rw-   0 root         (0) root         (0)     1097 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/algorithms/static/TSP_target_agent.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 16:25:03.000000 Marl-Factory-Grid-0.0.7/mfg_package/algorithms/static/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      385 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/algorithms/static/random_agent.py
--rw-rw-rw-   0 root         (0) root         (0)     2687 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/algorithms/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.026140 Marl-Factory-Grid-0.0.7/mfg_package/environment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 16:25:03.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2615 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/actions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.026140 Marl-Factory-Grid-0.0.7/mfg_package/environment/assets/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 16:25:03.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/assets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.026140 Marl-Factory-Grid-0.0.7/mfg_package/environment/assets/agent/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 16:25:03.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/assets/agent/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8521 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/assets/agent/adversary.png
--rw-rw-rw-   0 root         (0) root         (0)     3402 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/assets/agent/agent.png
--rw-rw-rw-   0 root         (0) root         (0)    18857 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/assets/agent/agent_collision.png
--rw-rw-rw-   0 root         (0) root         (0)     1631 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/assets/agent/idle.png
--rw-rw-rw-   0 root         (0) root         (0)     1599 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/assets/agent/invalid.png
--rw-rw-rw-   0 root         (0) root         (0)     5933 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/assets/agent/move.png
--rw-rw-rw-   0 root         (0) root         (0)     5717 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/assets/agent/valid.png
--rw-rw-rw-   0 root         (0) root         (0)     1415 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/assets/wall.png
--rw-rw-rw-   0 root         (0) root         (0)     2766 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.026140 Marl-Factory-Grid-0.0.7/mfg_package/environment/entity/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 16:25:03.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/entity/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2338 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/entity/agent.py
--rw-rw-rw-   0 root         (0) root         (0)     2157 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/entity/entity.py
--rw-rw-rw-   0 root         (0) root         (0)      400 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/entity/mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     3314 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/entity/object.py
--rw-rw-rw-   0 root         (0) root         (0)     1228 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/entity/util.py
--rw-rw-rw-   0 root         (0) root         (0)     3099 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/entity/wall_floor.py
--rw-rw-rw-   0 root         (0) root         (0)     6901 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.026140 Marl-Factory-Grid-0.0.7/mfg_package/environment/groups/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 16:25:03.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/groups/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      877 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/groups/agents.py
--rw-rw-rw-   0 root         (0) root         (0)      945 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/groups/env_objects.py
--rw-rw-rw-   0 root         (0) root         (0)     2044 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/groups/global_entities.py
--rw-rw-rw-   0 root         (0) root         (0)     2898 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/groups/mixins.py
--rw-rw-rw-   0 root         (0) root         (0)     3896 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/groups/objects.py
--rw-rw-rw-   0 root         (0) root         (0)     2363 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/groups/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1562 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/groups/wall_n_floors.py
--rw-rw-rw-   0 root         (0) root         (0)      124 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/rewards.py
--rw-rw-rw-   0 root         (0) root         (0)     2525 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/rules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.026140 Marl-Factory-Grid-0.0.7/mfg_package/logging/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 16:25:03.000000 Marl-Factory-Grid-0.0.7/mfg_package/logging/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2226 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/logging/envmonitor.py
--rw-rw-rw-   0 root         (0) root         (0)     5468 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/logging/recorder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.026140 Marl-Factory-Grid-0.0.7/mfg_package/modules/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 16:25:03.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.026140 Marl-Factory-Grid-0.0.7/mfg_package/modules/_template/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 16:25:03.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/_template/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      319 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/_template/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      583 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/_template/rules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.026140 Marl-Factory-Grid-0.0.7/mfg_package/modules/batteries/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 16:25:03.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/batteries/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/batteries/actions.py
--rw-rw-rw-   0 root         (0) root         (0)      523 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/batteries/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2390 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/batteries/entitites.py
--rw-rw-rw-   0 root         (0) root         (0)     1055 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/batteries/groups.py
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/batteries/rewards.py
--rw-rw-rw-   0 root         (0) root         (0)     2111 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/batteries/rules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.030140 Marl-Factory-Grid-0.0.7/mfg_package/modules/clean_up/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 16:25:03.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/clean_up/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1295 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/clean_up/actions.py
--rw-rw-rw-   0 root         (0) root         (0)      150 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/clean_up/constants.py
--rw-rw-rw-   0 root         (0) root         (0)    39296 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/clean_up/dirtpiles.png
--rw-rw-rw-   0 root         (0) root         (0)     1162 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/clean_up/entitites.py
--rw-rw-rw-   0 root         (0) root         (0)     2581 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/clean_up/groups.py
--rw-rw-rw-   0 root         (0) root         (0)       82 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/clean_up/rewards.py
--rw-rw-rw-   0 root         (0) root         (0)      587 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/clean_up/rule_done_on_all_clean.py
--rw-rw-rw-   0 root         (0) root         (0)      949 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/clean_up/rule_respawn.py
--rw-rw-rw-   0 root         (0) root         (0)     1042 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/clean_up/rule_smear_on_move.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.030140 Marl-Factory-Grid-0.0.7/mfg_package/modules/destinations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 16:25:03.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/destinations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      924 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/destinations/actions.py
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/destinations/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     7037 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/destinations/destinations.png
--rw-rw-rw-   0 root         (0) root         (0)     1783 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/destinations/entitites.py
--rw-rw-rw-   0 root         (0) root         (0)      816 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/destinations/groups.py
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/destinations/rewards.py
--rw-rw-rw-   0 root         (0) root         (0)     3698 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/destinations/rules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.030140 Marl-Factory-Grid-0.0.7/mfg_package/modules/doors/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 16:25:03.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/doors/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1140 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/doors/actions.py
--rw-rw-rw-   0 root         (0) root         (0)      793 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/doors/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      699 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/doors/door_closed.png
--rw-rw-rw-   0 root         (0) root         (0)     4224 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/doors/door_open.png
--rw-rw-rw-   0 root         (0) root         (0)     2716 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/doors/entitites.py
--rw-rw-rw-   0 root         (0) root         (0)      900 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/doors/groups.py
--rw-rw-rw-   0 root         (0) root         (0)       58 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/doors/rewards.py
--rw-rw-rw-   0 root         (0) root         (0)      876 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/doors/rule_door_auto_close.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.030140 Marl-Factory-Grid-0.0.7/mfg_package/modules/items/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 16:25:03.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/items/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1657 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/items/actions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.030140 Marl-Factory-Grid-0.0.7/mfg_package/modules/items/assets/
--rw-rw-rw-   0 root         (0) root         (0)     6610 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/items/assets/charge_pod.png
--rw-rw-rw-   0 root         (0) root         (0)     2318 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/items/assets/dropofflocations.png
--rw-rw-rw-   0 root         (0) root         (0)     3102 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/items/assets/items.png
--rw-rw-rw-   0 root         (0) root         (0)      234 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/items/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2050 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/items/entitites.py
--rw-rw-rw-   0 root         (0) root         (0)     3137 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/items/groups.py
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/items/rewards.py
--rw-rw-rw-   0 root         (0) root         (0)     3123 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/items/rules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.030140 Marl-Factory-Grid-0.0.7/mfg_package/modules/levels/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 16:25:03.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/levels/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1511 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/levels/large.txt
--rw-rw-rw-   0 root         (0) root         (0)     5827 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/levels/large_qquad.txt
--rw-rw-rw-   0 root         (0) root         (0)      207 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/levels/rooms.txt
--rw-rw-rw-   0 root         (0) root         (0)      168 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/levels/shelves.txt
--rw-rw-rw-   0 root         (0) root         (0)      155 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/levels/simple.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.030140 Marl-Factory-Grid-0.0.7/mfg_package/modules/machines/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 16:25:03.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/machines/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      178 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/machines/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1868 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/machines/entitites.py
--rw-rw-rw-   0 root         (0) root         (0)      421 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/machines/groups.py
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/machines/rewards.py
--rw-rw-rw-   0 root         (0) root         (0)      902 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/machines/rules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.030140 Marl-Factory-Grid-0.0.7/mfg_package/plotting/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 16:25:03.000000 Marl-Factory-Grid-0.0.7/mfg_package/plotting/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8640 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/plotting/compare_runs.py
--rw-rw-rw-   0 root         (0) root         (0)     2967 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/plotting/plotting.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.030140 Marl-Factory-Grid-0.0.7/mfg_package/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 16:25:03.000000 Marl-Factory-Grid-0.0.7/mfg_package/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5285 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/utils/config_parser.py
--rw-rw-rw-   0 root         (0) root         (0)    10876 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/utils/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     2236 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/utils/level_parser.py
--rw-rw-rw-   0 root         (0) root         (0)    12481 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/utils/observation_builder.py
--rw-rw-rw-   0 root         (0) root         (0)      283 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/utils/render.py
--rw-rw-rw-   0 root         (0) root         (0)     5759 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/utils/renderer.py
--rw-rw-rw-   0 root         (0) root         (0)     1108 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/utils/results.py
--rw-rw-rw-   0 root         (0) root         (0)     3601 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/utils/states.py
--rw-rw-rw-   0 root         (0) root         (0)     5655 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/utils/tools.py
--rw-rw-rw-   0 root         (0) root         (0)      811 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/utils/utility_classes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.034140 Marl-Factory-Grid-0.0.7/quickstart/
--rw-rw-rw-   0 root         (0) root         (0)     2129 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/quickstart/all_test_config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1381 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/quickstart/default_config.yaml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-20 16:25:10.034140 Marl-Factory-Grid-0.0.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1415 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.097490 Marl-Factory-Grid-0.0.8/
+-rw-rw-rw-   0 root         (0) root         (0)      453 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)       45 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/MANIFEST.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.085491 Marl-Factory-Grid-0.0.8/Marl_Factory_Grid.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4376 2023-06-21 09:29:12.000000 Marl-Factory-Grid-0.0.8/Marl_Factory_Grid.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6265 2023-06-21 09:29:12.000000 Marl-Factory-Grid-0.0.8/Marl_Factory_Grid.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 09:29:12.000000 Marl-Factory-Grid-0.0.8/Marl_Factory_Grid.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-21 09:29:12.000000 Marl-Factory-Grid-0.0.8/Marl_Factory_Grid.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-21 09:29:12.000000 Marl-Factory-Grid-0.0.8/Marl_Factory_Grid.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     4376 2023-06-21 09:29:12.097490 Marl-Factory-Grid-0.0.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3673 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.085491 Marl-Factory-Grid-0.0.8/images/
+-rw-rw-rw-   0 root         (0) root         (0)   303396 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/images/Hooks_FIKS.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.089491 Marl-Factory-Grid-0.0.8/marl_factory_grid/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.089491 Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.089491 Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/marl/
+-rw-rw-rw-   0 root         (0) root         (0)       74 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/marl/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8710 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/marl/base_ac.py
+-rw-rw-rw-   0 root         (0) root         (0)      636 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/marl/example_config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2125 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/marl/iac.py
+-rw-rw-rw-   0 root         (0) root         (0)     3208 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/marl/mappo.py
+-rw-rw-rw-   0 root         (0) root         (0)     7763 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/marl/memory.py
+-rw-rw-rw-   0 root         (0) root         (0)     4784 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/marl/networks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2279 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/marl/seac.py
+-rw-rw-rw-   0 root         (0) root         (0)     1305 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/marl/snac.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.089491 Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/static/
+-rw-rw-rw-   0 root         (0) root         (0)     5337 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/static/TSP_base_agent.py
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/static/TSP_dirt_agent.py
+-rw-rw-rw-   0 root         (0) root         (0)     2387 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/static/TSP_item_agent.py
+-rw-rw-rw-   0 root         (0) root         (0)     1115 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/static/TSP_target_agent.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/static/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      391 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/static/random_agent.py
+-rw-rw-rw-   0 root         (0) root         (0)     2687 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.089491 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2633 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/actions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.089491 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/assets/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/assets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.089491 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/assets/agent/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/assets/agent/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8521 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/assets/agent/adversary.png
+-rw-rw-rw-   0 root         (0) root         (0)     3402 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/assets/agent/agent.png
+-rw-rw-rw-   0 root         (0) root         (0)    18857 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/assets/agent/agent_collision.png
+-rw-rw-rw-   0 root         (0) root         (0)     1631 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/assets/agent/idle.png
+-rw-rw-rw-   0 root         (0) root         (0)     1599 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/assets/agent/invalid.png
+-rw-rw-rw-   0 root         (0) root         (0)     5933 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/assets/agent/move.png
+-rw-rw-rw-   0 root         (0) root         (0)     5717 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/assets/agent/valid.png
+-rw-rw-rw-   0 root         (0) root         (0)     1415 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/assets/wall.png
+-rw-rw-rw-   0 root         (0) root         (0)     2766 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.089491 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/entity/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/entity/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2380 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/entity/agent.py
+-rw-rw-rw-   0 root         (0) root         (0)     2175 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/entity/entity.py
+-rw-rw-rw-   0 root         (0) root         (0)      400 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/entity/mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     3320 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/entity/object.py
+-rw-rw-rw-   0 root         (0) root         (0)     1240 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/entity/util.py
+-rw-rw-rw-   0 root         (0) root         (0)     3123 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/entity/wall_floor.py
+-rw-rw-rw-   0 root         (0) root         (0)     6943 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.093490 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/groups/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/groups/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      895 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/groups/agents.py
+-rw-rw-rw-   0 root         (0) root         (0)      957 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/groups/env_objects.py
+-rw-rw-rw-   0 root         (0) root         (0)     2056 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/groups/global_entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     2910 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/groups/mixins.py
+-rw-rw-rw-   0 root         (0) root         (0)     3902 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/groups/objects.py
+-rw-rw-rw-   0 root         (0) root         (0)     2399 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/groups/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1586 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/groups/wall_n_floors.py
+-rw-rw-rw-   0 root         (0) root         (0)      124 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/rewards.py
+-rw-rw-rw-   0 root         (0) root         (0)     2537 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/rules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.093490 Marl-Factory-Grid-0.0.8/marl_factory_grid/logging/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/logging/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2244 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/logging/envmonitor.py
+-rw-rw-rw-   0 root         (0) root         (0)     5474 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/logging/recorder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.093490 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.093490 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/_template/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/_template/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      319 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/_template/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      595 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/_template/rules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.093490 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/batteries/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/batteries/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1103 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/batteries/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)      523 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/batteries/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2426 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/batteries/entitites.py
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/batteries/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/batteries/rewards.py
+-rw-rw-rw-   0 root         (0) root         (0)     2135 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/batteries/rules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.093490 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/clean_up/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/clean_up/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1319 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/clean_up/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)      150 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/clean_up/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)    39296 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/clean_up/dirtpiles.png
+-rw-rw-rw-   0 root         (0) root         (0)     1180 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/clean_up/entitites.py
+-rw-rw-rw-   0 root         (0) root         (0)     2611 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/clean_up/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)       82 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/clean_up/rewards.py
+-rw-rw-rw-   0 root         (0) root         (0)      611 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/clean_up/rule_done_on_all_clean.py
+-rw-rw-rw-   0 root         (0) root         (0)      967 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/clean_up/rule_respawn.py
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/clean_up/rule_smear_on_move.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.093490 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/destinations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/destinations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      948 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/destinations/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/destinations/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     7037 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/destinations/destinations.png
+-rw-rw-rw-   0 root         (0) root         (0)     1813 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/destinations/entitites.py
+-rw-rw-rw-   0 root         (0) root         (0)      834 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/destinations/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/destinations/rewards.py
+-rw-rw-rw-   0 root         (0) root         (0)     3728 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/destinations/rules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.093490 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/doors/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/doors/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1164 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/doors/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)      793 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/doors/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      699 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/doors/door_closed.png
+-rw-rw-rw-   0 root         (0) root         (0)     4224 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/doors/door_open.png
+-rw-rw-rw-   0 root         (0) root         (0)     2740 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/doors/entitites.py
+-rw-rw-rw-   0 root         (0) root         (0)      924 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/doors/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/doors/rewards.py
+-rw-rw-rw-   0 root         (0) root         (0)      900 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/doors/rule_door_auto_close.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.093490 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/items/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/items/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1681 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/items/actions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.093490 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/items/assets/
+-rw-rw-rw-   0 root         (0) root         (0)     6610 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/items/assets/charge_pod.png
+-rw-rw-rw-   0 root         (0) root         (0)     2318 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/items/assets/dropofflocations.png
+-rw-rw-rw-   0 root         (0) root         (0)     3102 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/items/assets/items.png
+-rw-rw-rw-   0 root         (0) root         (0)      234 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/items/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2074 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/items/entitites.py
+-rw-rw-rw-   0 root         (0) root         (0)     3173 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/items/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/items/rewards.py
+-rw-rw-rw-   0 root         (0) root         (0)     3153 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/items/rules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.097490 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/levels/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/levels/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1511 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/levels/large.txt
+-rw-rw-rw-   0 root         (0) root         (0)     5827 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/levels/large_qquad.txt
+-rw-rw-rw-   0 root         (0) root         (0)      207 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/levels/rooms.txt
+-rw-rw-rw-   0 root         (0) root         (0)      168 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/levels/shelves.txt
+-rw-rw-rw-   0 root         (0) root         (0)      155 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/levels/simple.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.097490 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/machines/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/machines/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      178 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/machines/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1898 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/machines/entitites.py
+-rw-rw-rw-   0 root         (0) root         (0)      439 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/machines/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/machines/rewards.py
+-rw-rw-rw-   0 root         (0) root         (0)      932 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/machines/rules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.097490 Marl-Factory-Grid-0.0.8/marl_factory_grid/plotting/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/plotting/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8652 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/plotting/compare_runs.py
+-rw-rw-rw-   0 root         (0) root         (0)     2967 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/plotting/plotting.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.097490 Marl-Factory-Grid-0.0.8/marl_factory_grid/quickstart/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/quickstart/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1381 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/quickstart/default_config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      413 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/quickstart/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.097490 Marl-Factory-Grid-0.0.8/marl_factory_grid/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5309 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/utils/config_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)    10888 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/utils/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2260 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/utils/level_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)    12499 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/utils/observation_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)      283 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/utils/render.py
+-rw-rw-rw-   0 root         (0) root         (0)     5765 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/utils/renderer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1114 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/utils/results.py
+-rw-rw-rw-   0 root         (0) root         (0)     3625 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/utils/states.py
+-rw-rw-rw-   0 root         (0) root         (0)     5673 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/utils/tools.py
+-rw-rw-rw-   0 root         (0) root         (0)      811 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/utils/utility_classes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.097490 Marl-Factory-Grid-0.0.8/quickstart/
+-rw-rw-rw-   0 root         (0) root         (0)     2129 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/quickstart/all_test_config.yaml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-21 09:29:12.097490 Marl-Factory-Grid-0.0.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1415 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/setup.py
```

### Comparing `Marl-Factory-Grid-0.0.7/Marl_Factory_Grid.egg-info/PKG-INFO` & `Marl-Factory-Grid-0.0.8/Marl_Factory_Grid.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Marl-Factory-Grid
-Version: 0.0.7
+Version: 0.0.8
 Summary: A framework to research MARL agents in various setings.
 Home-page: https://github.com/illiumst/marl-factory-grid/import
 Author: Steffen Illium
 Author-email: steffen.illium@ifi.lmu.de
 License: MIT
 Keywords: artificial intelligence,pytorch,multiagent reinforcement learning,simulation,emergence,gymnasium,environment,deepdiff,natsort
 Classifier: Development Status :: 4 - Beta
@@ -92,35 +92,35 @@
 Varying levels are created by defining Walls, Floor or Doors in *.txt*-files (see [./environment/levels](./environment/levels) for examples).
 Define which *level* to use in your *configfile* as: 
 ```yaml
 General:
     level_name: rooms  # 'double', 'large', 'simple', ...
 ```
 ... or create your own , maybe with the help of [asciiflow.com](https://asciiflow.com/#/).
-Make sure to use `#` as [Walls](mfg_package/environment/entity/wall_floor.py), `-` as free (walkable) [Floor](mfg_package/environment/entity/wall_floor.py)-Tiles, `D` for [Walls](./modules/doors/entities.py).
+Make sure to use `#` as [Walls](marl_factory_grid/environment/entity/wall_floor.py), `-` as free (walkable) [Floor](marl_factory_grid/environment/entity/wall_floor.py)-Tiles, `D` for [Walls](./modules/doors/entities.py).
 Other Entites (define you own) may bring their own `Symbols`
 
 #### Entites
-Entites, either [Objects](mfg_package/environment/entity/object.py) for tracking stats 
-or env. [Entity](mfg_package/environment/entity/entity.py) which can interact.
+Entites, either [Objects](marl_factory_grid/environment/entity/object.py) for tracking stats 
+or env. [Entity](marl_factory_grid/environment/entity/entity.py) which can interact.
 Abstract Entities are provided.
 
 #### Groups
-[Groups](mfg_package/environment/groups/objects.py) are entity Sets that provide administrative access to all group members. 
-All [Entites](mfg_package/environment/entity/global_entities.py) are available at runtime as EnvState property.
+[Groups](marl_factory_grid/environment/groups/objects.py) are entity Sets that provide administrative access to all group members. 
+All [Entites](marl_factory_grid/environment/entity/global_entities.py) are available at runtime as EnvState property.
 
 
 #### Rules
-[Rules](mfg_package/environment/entity/object.py) define how the environment behaves on micro-scale.
+[Rules](marl_factory_grid/environment/entity/object.py) define how the environment behaves on micro-scale.
 Each of the hookes (`on_init`, `pre_step`, `on_step`, '`post_step`', `on_done`) 
 provide env-access to implement customn logic, calculate rewards, or gather information.
 
 ![Hooks](./images/Hooks_FIKS.png)
 
-[Results](mfg_package/environment/entity/object.py) provide a way to return `rule` evaluations such as rewards and state reports 
+[Results](marl_factory_grid/environment/entity/object.py) provide a way to return `rule` evaluations such as rewards and state reports 
 back to the environment.
 #### Assets
 Make sure to bring your own assets for each Entity living in the Gridworl as the `Renderer` relies on it.
 PNG-files (transparent background) of square aspect-ratio should do the job, in general.
 
 <img src=".\environment\assets\wall.png"  width="5%"> 
 &nbsp&nbsp&nbsp&nbsp
```

### Comparing `Marl-Factory-Grid-0.0.7/PKG-INFO` & `Marl-Factory-Grid-0.0.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Marl-Factory-Grid
-Version: 0.0.7
+Version: 0.0.8
 Summary: A framework to research MARL agents in various setings.
 Home-page: https://github.com/illiumst/marl-factory-grid/import
 Author: Steffen Illium
 Author-email: steffen.illium@ifi.lmu.de
 License: MIT
 Keywords: artificial intelligence,pytorch,multiagent reinforcement learning,simulation,emergence,gymnasium,environment,deepdiff,natsort
 Classifier: Development Status :: 4 - Beta
@@ -92,35 +92,35 @@
 Varying levels are created by defining Walls, Floor or Doors in *.txt*-files (see [./environment/levels](./environment/levels) for examples).
 Define which *level* to use in your *configfile* as: 
 ```yaml
 General:
     level_name: rooms  # 'double', 'large', 'simple', ...
 ```
 ... or create your own , maybe with the help of [asciiflow.com](https://asciiflow.com/#/).
-Make sure to use `#` as [Walls](mfg_package/environment/entity/wall_floor.py), `-` as free (walkable) [Floor](mfg_package/environment/entity/wall_floor.py)-Tiles, `D` for [Walls](./modules/doors/entities.py).
+Make sure to use `#` as [Walls](marl_factory_grid/environment/entity/wall_floor.py), `-` as free (walkable) [Floor](marl_factory_grid/environment/entity/wall_floor.py)-Tiles, `D` for [Walls](./modules/doors/entities.py).
 Other Entites (define you own) may bring their own `Symbols`
 
 #### Entites
-Entites, either [Objects](mfg_package/environment/entity/object.py) for tracking stats 
-or env. [Entity](mfg_package/environment/entity/entity.py) which can interact.
+Entites, either [Objects](marl_factory_grid/environment/entity/object.py) for tracking stats 
+or env. [Entity](marl_factory_grid/environment/entity/entity.py) which can interact.
 Abstract Entities are provided.
 
 #### Groups
-[Groups](mfg_package/environment/groups/objects.py) are entity Sets that provide administrative access to all group members. 
-All [Entites](mfg_package/environment/entity/global_entities.py) are available at runtime as EnvState property.
+[Groups](marl_factory_grid/environment/groups/objects.py) are entity Sets that provide administrative access to all group members. 
+All [Entites](marl_factory_grid/environment/entity/global_entities.py) are available at runtime as EnvState property.
 
 
 #### Rules
-[Rules](mfg_package/environment/entity/object.py) define how the environment behaves on micro-scale.
+[Rules](marl_factory_grid/environment/entity/object.py) define how the environment behaves on micro-scale.
 Each of the hookes (`on_init`, `pre_step`, `on_step`, '`post_step`', `on_done`) 
 provide env-access to implement customn logic, calculate rewards, or gather information.
 
 ![Hooks](./images/Hooks_FIKS.png)
 
-[Results](mfg_package/environment/entity/object.py) provide a way to return `rule` evaluations such as rewards and state reports 
+[Results](marl_factory_grid/environment/entity/object.py) provide a way to return `rule` evaluations such as rewards and state reports 
 back to the environment.
 #### Assets
 Make sure to bring your own assets for each Entity living in the Gridworl as the `Renderer` relies on it.
 PNG-files (transparent background) of square aspect-ratio should do the job, in general.
 
 <img src=".\environment\assets\wall.png"  width="5%"> 
 &nbsp&nbsp&nbsp&nbsp
```

### Comparing `Marl-Factory-Grid-0.0.7/README.md` & `Marl-Factory-Grid-0.0.8/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -76,35 +76,35 @@
 Varying levels are created by defining Walls, Floor or Doors in *.txt*-files (see [./environment/levels](./environment/levels) for examples).
 Define which *level* to use in your *configfile* as: 
 ```yaml
 General:
     level_name: rooms  # 'double', 'large', 'simple', ...
 ```
 ... or create your own , maybe with the help of [asciiflow.com](https://asciiflow.com/#/).
-Make sure to use `#` as [Walls](mfg_package/environment/entity/wall_floor.py), `-` as free (walkable) [Floor](mfg_package/environment/entity/wall_floor.py)-Tiles, `D` for [Walls](./modules/doors/entities.py).
+Make sure to use `#` as [Walls](marl_factory_grid/environment/entity/wall_floor.py), `-` as free (walkable) [Floor](marl_factory_grid/environment/entity/wall_floor.py)-Tiles, `D` for [Walls](./modules/doors/entities.py).
 Other Entites (define you own) may bring their own `Symbols`
 
 #### Entites
-Entites, either [Objects](mfg_package/environment/entity/object.py) for tracking stats 
-or env. [Entity](mfg_package/environment/entity/entity.py) which can interact.
+Entites, either [Objects](marl_factory_grid/environment/entity/object.py) for tracking stats 
+or env. [Entity](marl_factory_grid/environment/entity/entity.py) which can interact.
 Abstract Entities are provided.
 
 #### Groups
-[Groups](mfg_package/environment/groups/objects.py) are entity Sets that provide administrative access to all group members. 
-All [Entites](mfg_package/environment/entity/global_entities.py) are available at runtime as EnvState property.
+[Groups](marl_factory_grid/environment/groups/objects.py) are entity Sets that provide administrative access to all group members. 
+All [Entites](marl_factory_grid/environment/entity/global_entities.py) are available at runtime as EnvState property.
 
 
 #### Rules
-[Rules](mfg_package/environment/entity/object.py) define how the environment behaves on micro-scale.
+[Rules](marl_factory_grid/environment/entity/object.py) define how the environment behaves on micro-scale.
 Each of the hookes (`on_init`, `pre_step`, `on_step`, '`post_step`', `on_done`) 
 provide env-access to implement customn logic, calculate rewards, or gather information.
 
 ![Hooks](./images/Hooks_FIKS.png)
 
-[Results](mfg_package/environment/entity/object.py) provide a way to return `rule` evaluations such as rewards and state reports 
+[Results](marl_factory_grid/environment/entity/object.py) provide a way to return `rule` evaluations such as rewards and state reports 
 back to the environment.
 #### Assets
 Make sure to bring your own assets for each Entity living in the Gridworl as the `Renderer` relies on it.
 PNG-files (transparent background) of square aspect-ratio should do the job, in general.
 
 <img src=".\environment\assets\wall.png"  width="5%"> 
 &nbsp&nbsp&nbsp&nbsp
```

### Comparing `Marl-Factory-Grid-0.0.7/images/Hooks_FIKS.png` & `Marl-Factory-Grid-0.0.8/images/Hooks_FIKS.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/algorithms/marl/base_ac.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/marl/base_ac.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import torch
 from typing import Union, List, Dict
 import numpy as np
 from torch.distributions import Categorical
-from mfg_package.algorithms.marl.memory import MARLActorCriticMemory
-from mfg_package.algorithms.utils import add_env_props, instantiate_class
+from marl_factory_grid.algorithms.marl.memory import MARLActorCriticMemory
+from marl_factory_grid.algorithms.utils import add_env_props, instantiate_class
 from pathlib import Path
 import pandas as pd
 from collections import deque
 
 
 class Names:
     REWARD          = 'reward'
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/algorithms/marl/example_config.yaml` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/marl/example_config.yaml`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/algorithms/marl/iac.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/marl/iac.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import torch
-from mfg_package.algorithms.marl.base_ac import BaseActorCritic, nms
-from mfg_package.algorithms.utils import instantiate_class
+from marl_factory_grid.algorithms.marl.base_ac import BaseActorCritic, nms
+from marl_factory_grid.algorithms.utils import instantiate_class
 from pathlib import Path
 from natsort import natsorted
-from mfg_package.algorithms.marl.memory import MARLActorCriticMemory
+from marl_factory_grid.algorithms.marl.memory import MARLActorCriticMemory
 
 
 class LoopIAC(BaseActorCritic):
 
     def __init__(self, cfg):
         super(LoopIAC, self).__init__(cfg)
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/algorithms/marl/mappo.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/marl/mappo.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from mfg_package.algorithms.marl.base_ac import Names as nms
-from mfg_package.algorithms.marl.snac import LoopSNAC
-from mfg_package.algorithms.marl.memory import MARLActorCriticMemory
+from marl_factory_grid.algorithms.marl.base_ac import Names as nms
+from marl_factory_grid.algorithms.marl.snac import LoopSNAC
+from marl_factory_grid.algorithms.marl.memory import MARLActorCriticMemory
 import torch
 from torch.distributions import Categorical
-from mfg_package.algorithms.utils import instantiate_class
+from marl_factory_grid.algorithms.utils import instantiate_class
 
 
 class LoopMAPPO(LoopSNAC):
     def __init__(self, *args, **kwargs):
         super(LoopMAPPO, self).__init__(*args, **kwargs)
         self.reset_memory_after_epoch = False
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/algorithms/marl/memory.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/marl/memory.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/algorithms/marl/networks.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/marl/networks.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/algorithms/marl/seac.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/marl/seac.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import torch
 from torch.distributions import Categorical
-from mfg_package.algorithms.marl.iac import LoopIAC
-from mfg_package.algorithms.marl.base_ac import nms
-from mfg_package.algorithms.marl.memory import MARLActorCriticMemory
+from marl_factory_grid.algorithms.marl.iac import LoopIAC
+from marl_factory_grid.algorithms.marl.base_ac import nms
+from marl_factory_grid.algorithms.marl.memory import MARLActorCriticMemory
 
 
 class LoopSEAC(LoopIAC):
     def __init__(self, cfg):
         super(LoopSEAC, self).__init__(cfg)
 
     def actor_critic(self, tm, networks, gamma, entropy_coef, vf_coef, gae_coef=0.0, **kwargs):
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/algorithms/marl/snac.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/marl/snac.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from mfg_package.algorithms.marl.base_ac import BaseActorCritic
-from mfg_package.algorithms.marl.base_ac import nms
+from marl_factory_grid.algorithms.marl.base_ac import BaseActorCritic
+from marl_factory_grid.algorithms.marl.base_ac import nms
 import torch
 from torch.distributions import Categorical
 from pathlib import Path
 
 
 class LoopSNAC(BaseActorCritic):
     def __init__(self, cfg):
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/algorithms/static/TSP_base_agent.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/static/TSP_base_agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from random import choice
 
 import numpy as np
 
 import networkx as nx
 from networkx.algorithms.approximation import traveling_salesman as tsp
 
-from mfg_package.modules.doors import constants as do
-from mfg_package.environment import constants as c
-from mfg_package.utils.helpers import MOVEMAP
+from marl_factory_grid.modules.doors import constants as do
+from marl_factory_grid.environment import constants as c
+from marl_factory_grid.utils.helpers import MOVEMAP
 
 from abc import abstractmethod, ABC
 
 future_planning = 7
 
 
 def points_to_graph(coordiniates_or_tiles, allow_euclidean_connections=True, allow_manhattan_connections=True):
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/algorithms/static/TSP_dirt_agent.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/static/TSP_dirt_agent.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from mfg_package.algorithms.static.TSP_base_agent import TSPBaseAgent
+from marl_factory_grid.algorithms.static.TSP_base_agent import TSPBaseAgent
 
-from mfg_package.modules.clean_up import constants as di
+from marl_factory_grid.modules.clean_up import constants as di
 
 future_planning = 7
 
 
 class TSPDirtAgent(TSPBaseAgent):
 
     def __init__(self, *args, **kwargs):
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/algorithms/static/TSP_item_agent.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/static/TSP_item_agent.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 
-from mfg_package.algorithms.static.TSP_base_agent import TSPBaseAgent
+from marl_factory_grid.algorithms.static.TSP_base_agent import TSPBaseAgent
 
-from mfg_package.modules.items import constants as i
+from marl_factory_grid.modules.items import constants as i
 
 future_planning = 7
 inventory_size  = 3
 
 MODE_GET        = 'Mode_Get'
 MODE_BRING      = 'Mode_Bring'
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/algorithms/utils.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/utils.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/environment/actions.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/actions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import abc
 from typing import Union
 
-from mfg_package.environment import rewards as r, constants as c
-from mfg_package.utils.helpers import MOVEMAP
-from mfg_package.utils.results import ActionResult
+from marl_factory_grid.environment import rewards as r, constants as c
+from marl_factory_grid.utils.helpers import MOVEMAP
+from marl_factory_grid.utils.results import ActionResult
 
 
 class Action(abc.ABC):
 
     @property
     def name(self):
         return self._identifier
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/environment/assets/agent/adversary.png` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/assets/agent/adversary.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/environment/assets/agent/agent.png` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/assets/agent/agent.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/environment/assets/agent/agent_collision.png` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/assets/agent/agent_collision.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/environment/assets/agent/idle.png` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/assets/agent/idle.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/environment/assets/agent/invalid.png` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/assets/agent/invalid.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/environment/assets/agent/move.png` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/assets/agent/move.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/environment/assets/agent/valid.png` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/assets/agent/valid.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/environment/assets/wall.png` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/assets/wall.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/environment/constants.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/constants.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/environment/entity/agent.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/entity/agent.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import List, Union
 
-from mfg_package.environment import constants as c
-from mfg_package.environment.actions import Action
-from mfg_package.environment.entity.entity import Entity
-from mfg_package.utils.render import RenderEntity
-from mfg_package.utils import renderer
-from mfg_package.utils.helpers import is_move
-from mfg_package.utils.results import ActionResult, Result
+from marl_factory_grid.environment import constants as c
+from marl_factory_grid.environment.actions import Action
+from marl_factory_grid.environment.entity.entity import Entity
+from marl_factory_grid.utils.render import RenderEntity
+from marl_factory_grid.utils import renderer
+from marl_factory_grid.utils.helpers import is_move
+from marl_factory_grid.utils.results import ActionResult, Result
 
 
 class Agent(Entity):
 
     @property
     def obs_tag(self):
         return self.name
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/environment/entity/entity.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/entity/entity.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import abc
 
-from mfg_package.environment import constants as c
-from mfg_package.environment.entity.object import EnvObject
-from mfg_package.utils.render import RenderEntity
+from marl_factory_grid.environment import constants as c
+from marl_factory_grid.environment.entity.object import EnvObject
+from marl_factory_grid.utils.render import RenderEntity
 
 
 class Entity(EnvObject, abc.ABC):
     """Full Env Entity that lives on the environment Grid. Doors, Items, DirtPile etc..."""
 
     @property
     def has_position(self):
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/environment/entity/object.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/entity/object.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from collections import defaultdict
 from typing import Union
 
-from mfg_package.environment import constants as c
+from marl_factory_grid.environment import constants as c
 
 
 class Object:
 
     """Generell Objects for Organisation and Maintanance such as Actions etc..."""
 
     _u_idx = defaultdict(lambda: 0)
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/environment/entity/util.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/entity/util.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import math
 
 import numpy as np
 
-from mfg_package.environment.entity.mixin import BoundEntityMixin
-from mfg_package.environment.entity.object import Object, EnvObject
+from marl_factory_grid.environment.entity.mixin import BoundEntityMixin
+from marl_factory_grid.environment.entity.object import Object, EnvObject
 
 
 ##########################################################################
 # ####################### Objects and Entitys ########################## #
 ##########################################################################
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/environment/entity/wall_floor.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/entity/wall_floor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List
 
 import numpy as np
 
-from mfg_package.environment import constants as c
-from mfg_package.environment.entity.object import EnvObject
-from mfg_package.utils.render import RenderEntity
-from mfg_package.utils import helpers as h
+from marl_factory_grid.environment import constants as c
+from marl_factory_grid.environment.entity.object import EnvObject
+from marl_factory_grid.utils.render import RenderEntity
+from marl_factory_grid.utils import helpers as h
 
 
 class Floor(EnvObject):
 
     @property
     def has_position(self):
         return True
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/environment/factory.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 from itertools import chain
 from os import PathLike
 from pathlib import Path
 from typing import Union
 
 import gymnasium as gym
 
-from mfg_package.utils.level_parser import LevelParser
-from mfg_package.utils.observation_builder import OBSBuilder
-from mfg_package.utils.config_parser import FactoryConfigParser
-from mfg_package.utils import helpers as h
-import mfg_package.environment.constants as c
+from marl_factory_grid.utils.level_parser import LevelParser
+from marl_factory_grid.utils.observation_builder import OBSBuilder
+from marl_factory_grid.utils.config_parser import FactoryConfigParser
+from marl_factory_grid.utils import helpers as h
+import marl_factory_grid.environment.constants as c
 
-from mfg_package.utils.states import Gamestate
+from marl_factory_grid.utils.states import Gamestate
 
 REC_TAC = 'rec_'
 
 
 class BaseFactory(gym.Env):
 
     @property
@@ -167,15 +167,15 @@
     def stop_recording(self):
         self.conf.do_record = False
         return not self.conf.do_record
 
     # noinspection PyGlobalUndefined
     def render(self, mode='human'):
         if not self._renderer:  # lazy init
-            from mfg_package.utils.renderer import Renderer
+            from marl_factory_grid.utils.renderer import Renderer
             global Renderer
             self._renderer = Renderer(self.map.level_shape,  view_radius=self.conf.pomdp_r, fps=10)
 
         render_entities = self.state.entities.render()
         if self.conf.pomdp_r:
             for render_entity in render_entities:
                 if render_entity.name == c.AGENT:
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/environment/groups/agents.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/groups/agents.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from mfg_package.environment.groups.env_objects import EnvObjects
-from mfg_package.environment.groups.mixins import PositionMixin
-from mfg_package.environment.entity.agent import Agent
+from marl_factory_grid.environment.groups.env_objects import EnvObjects
+from marl_factory_grid.environment.groups.mixins import PositionMixin
+from marl_factory_grid.environment.entity.agent import Agent
 
 
 class Agents(PositionMixin, EnvObjects):
     _entity = Agent
     is_blocking_light = False
     can_move = True
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/environment/groups/env_objects.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/groups/env_objects.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from mfg_package.environment.groups.objects import Objects
-from mfg_package.environment.entity.object import EnvObject
+from marl_factory_grid.environment.groups.objects import Objects
+from marl_factory_grid.environment.entity.object import EnvObject
 
 
 class EnvObjects(Objects):
 
     _entity = EnvObject
     is_blocking_light: bool = False
     can_collide: bool = False
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/environment/groups/global_entities.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/groups/global_entities.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from collections import defaultdict
 from operator import itemgetter
 from typing import Dict
 
-from mfg_package.environment.groups.objects import Objects
-from mfg_package.utils.helpers import POS_MASK
+from marl_factory_grid.environment.groups.objects import Objects
+from marl_factory_grid.utils.helpers import POS_MASK
 
 
 class Entities(Objects):
     _entity = Objects
 
     @staticmethod
     def neighboring_positions(pos):
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/environment/groups/mixins.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/groups/mixins.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from mfg_package.environment import constants as c
+from marl_factory_grid.environment import constants as c
 
-from mfg_package.environment.entity.entity import Entity
+from marl_factory_grid.environment.entity.entity import Entity
 
 
 # noinspection PyUnresolvedReferences,PyTypeChecker,PyArgumentList
 class PositionMixin:
 
     _entity = Entity
     is_blocking_light: bool = True
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/environment/groups/objects.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/groups/objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from collections import defaultdict
 from typing import List
 
 import numpy as np
 
-from mfg_package.environment.entity.object import Object
+from marl_factory_grid.environment.entity.object import Object
 
 
 class Objects:
     _entity = Object
 
     @property
     def observers(self):
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/environment/groups/utils.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/groups/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from typing import List, Union
 
 import numpy as np
 
-from mfg_package.environment.groups.env_objects import EnvObjects
-from mfg_package.environment.groups.objects import Objects
-from mfg_package.environment.groups.mixins import HasBoundedMixin, PositionMixin
-from mfg_package.environment.entity.util import GlobalPosition
-from mfg_package.utils import helpers as h
-from mfg_package.environment import constants as c
+from marl_factory_grid.environment.groups.env_objects import EnvObjects
+from marl_factory_grid.environment.groups.objects import Objects
+from marl_factory_grid.environment.groups.mixins import HasBoundedMixin, PositionMixin
+from marl_factory_grid.environment.entity.util import GlobalPosition
+from marl_factory_grid.utils import helpers as h
+from marl_factory_grid.environment import constants as c
 
 
 class Combined(PositionMixin, EnvObjects):
 
     @property
     def name(self):
         return f'{super().name}({self._ident or self._names})'
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/environment/groups/wall_n_floors.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/groups/wall_n_floors.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import random
 from typing import List
 
-from mfg_package.environment import constants as c
-from mfg_package.environment.groups.env_objects import EnvObjects
-from mfg_package.environment.groups.mixins import PositionMixin
-from mfg_package.environment.entity.wall_floor import Wall, Floor
+from marl_factory_grid.environment import constants as c
+from marl_factory_grid.environment.groups.env_objects import EnvObjects
+from marl_factory_grid.environment.groups.mixins import PositionMixin
+from marl_factory_grid.environment.entity.wall_floor import Wall, Floor
 
 
 class Walls(PositionMixin, EnvObjects):
     _entity = Wall
     symbol = c.SYMBOL_WALL
 
     def __init__(self, *args, **kwargs):
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/environment/rules.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/rules.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import abc
 from typing import List
 
-from mfg_package.utils.results import TickResult, DoneResult
-from mfg_package.environment import rewards as r, constants as c
+from marl_factory_grid.utils.results import TickResult, DoneResult
+from marl_factory_grid.environment import rewards as r, constants as c
 
 
 class Rule(abc.ABC):
 
     @property
     def name(self):
         return self.__class__.__name__
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/logging/envmonitor.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/logging/envmonitor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import pickle
 from os import PathLike
 from pathlib import Path
 from typing import Union
 
 from gymnasium import Wrapper
 
-from mfg_package.utils.helpers import IGNORED_DF_COLUMNS
-from mfg_package.environment.factory import REC_TAC
+from marl_factory_grid.utils.helpers import IGNORED_DF_COLUMNS
+from marl_factory_grid.environment.factory import REC_TAC
 
 import pandas as pd
 
-from mfg_package.plotting.compare_runs import plot_single_run
+from marl_factory_grid.plotting.compare_runs import plot_single_run
 
 
 class EnvMonitor(Wrapper):
 
     ext = 'png'
 
     def __init__(self, env, filepath: Union[str, PathLike] = None):
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/logging/recorder.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/logging/recorder.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import yaml
 from gymnasium import Wrapper
 
 import numpy as np
 import pandas as pd
 
-from mfg_package.environment.factory import REC_TAC
+from marl_factory_grid.environment.factory import REC_TAC
 
 
 class EnvRecorder(Wrapper):
 
     def __init__(self, env, entities: str = 'all', filepath: Union[str, PathLike] = None, freq: int = 0):
         super(EnvRecorder, self).__init__(env)
         self.filepath = filepath
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/modules/_template/rules.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/_template/rules.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
-from mfg_package.environment.rules import Rule
-from mfg_package.utils.results import TickResult, DoneResult
+from marl_factory_grid.environment.rules import Rule
+from marl_factory_grid.utils.results import TickResult, DoneResult
 
 
 class TemplateRule(Rule):
 
     def __init__(self, *args, **kwargs):
         super(TemplateRule, self).__init__(*args, **kwargs)
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/modules/batteries/actions.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/batteries/actions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Union
 
-from mfg_package.environment.actions import Action
-from mfg_package.utils.results import ActionResult
+from marl_factory_grid.environment.actions import Action
+from marl_factory_grid.utils.results import ActionResult
 
-from mfg_package.modules.batteries import constants as b, rewards as r
-from mfg_package.environment import constants as c
+from marl_factory_grid.modules.batteries import constants as b, rewards as r
+from marl_factory_grid.environment import constants as c
 
 
 class BtryCharge(Action):
 
     def __init__(self):
         super().__init__(b.CHARGE)
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/modules/batteries/constants.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/batteries/constants.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/modules/batteries/entitites.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/batteries/entitites.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from mfg_package.environment.entity.mixin import BoundEntityMixin
-from mfg_package.environment.entity.object import EnvObject
-from mfg_package.environment.entity.entity import Entity
-from mfg_package.environment import constants as c
-from mfg_package.utils.render import RenderEntity
+from marl_factory_grid.environment.entity.mixin import BoundEntityMixin
+from marl_factory_grid.environment.entity.object import EnvObject
+from marl_factory_grid.environment.entity.entity import Entity
+from marl_factory_grid.environment import constants as c
+from marl_factory_grid.utils.render import RenderEntity
 
-from mfg_package.modules.batteries import constants as b
+from marl_factory_grid.modules.batteries import constants as b
 
 
 class Battery(BoundEntityMixin, EnvObject):
 
     @property
     def is_discharged(self):
         return self.charge_level == 0
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/modules/batteries/groups.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/batteries/groups.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from mfg_package.environment.groups.env_objects import EnvObjects
-from mfg_package.environment.groups.mixins import PositionMixin, HasBoundedMixin
-from mfg_package.modules.batteries.entitites import ChargePod, Battery
+from marl_factory_grid.environment.groups.env_objects import EnvObjects
+from marl_factory_grid.environment.groups.mixins import PositionMixin, HasBoundedMixin
+from marl_factory_grid.modules.batteries.entitites import ChargePod, Battery
 
 
 class Batteries(HasBoundedMixin, EnvObjects):
 
     _entity = Battery
     is_blocking_light: bool = False
     can_collide: bool = False
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/modules/batteries/rules.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/batteries/rules.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List, Union
-from mfg_package.environment.rules import Rule
-from mfg_package.utils.results import TickResult, DoneResult
+from marl_factory_grid.environment.rules import Rule
+from marl_factory_grid.utils.results import TickResult, DoneResult
 
-from mfg_package.environment import constants as c
-from mfg_package.modules.batteries import constants as b, rewards as r
+from marl_factory_grid.environment import constants as c
+from marl_factory_grid.modules.batteries import constants as b, rewards as r
 
 
 class Btry(Rule):
 
     def __init__(self, initial_charge: float = 0.8, per_action_costs: Union[dict, float] = 0.02):
         super().__init__()
         self.per_action_costs = per_action_costs
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/modules/clean_up/actions.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/clean_up/actions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Union
 
-from mfg_package.environment.actions import Action
-from mfg_package.utils.results import ActionResult
+from marl_factory_grid.environment.actions import Action
+from marl_factory_grid.utils.results import ActionResult
 
-from mfg_package.modules.clean_up import constants as d, rewards as r
+from marl_factory_grid.modules.clean_up import constants as d, rewards as r
 
-from mfg_package.environment import constants as c
+from marl_factory_grid.environment import constants as c
 
 
 class CleanUp(Action):
 
     def __init__(self):
         super().__init__(d.CLEAN_UP)
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/modules/clean_up/dirtpiles.png` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/clean_up/dirtpiles.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/modules/clean_up/entitites.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/clean_up/entitites.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from numpy import random
 
-from mfg_package.environment.entity.entity import Entity
-from mfg_package.utils.render import RenderEntity
-from mfg_package.modules.clean_up import constants as d
+from marl_factory_grid.environment.entity.entity import Entity
+from marl_factory_grid.utils.render import RenderEntity
+from marl_factory_grid.modules.clean_up import constants as d
 
 
 class DirtPile(Entity):
 
     @property
     def amount(self):
         return self._amount
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/modules/clean_up/groups.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/clean_up/groups.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from mfg_package.environment.groups.env_objects import EnvObjects
-from mfg_package.environment.groups.mixins import PositionMixin
-from mfg_package.environment.entity.wall_floor import Floor
-from mfg_package.modules.clean_up.entitites import DirtPile
+from marl_factory_grid.environment.groups.env_objects import EnvObjects
+from marl_factory_grid.environment.groups.mixins import PositionMixin
+from marl_factory_grid.environment.entity.wall_floor import Floor
+from marl_factory_grid.modules.clean_up.entitites import DirtPile
 
-from mfg_package.environment import constants as c
+from marl_factory_grid.environment import constants as c
 
 
 class DirtPiles(PositionMixin, EnvObjects):
 
     _entity = DirtPile
     is_blocking_light: bool = False
     can_collide: bool = False
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/modules/clean_up/rule_done_on_all_clean.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/clean_up/rule_done_on_all_clean.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from mfg_package.environment import constants as c
-from mfg_package.environment.rules import Rule
-from mfg_package.utils.results import DoneResult
-from mfg_package.modules.clean_up import constants as d, rewards as r
+from marl_factory_grid.environment import constants as c
+from marl_factory_grid.environment.rules import Rule
+from marl_factory_grid.utils.results import DoneResult
+from marl_factory_grid.modules.clean_up import constants as d, rewards as r
 
 
 class DirtAllCleanDone(Rule):
 
     def __init__(self):
         super().__init__()
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/modules/clean_up/rule_smear_on_move.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/clean_up/rule_smear_on_move.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from mfg_package.environment.rules import Rule
-from mfg_package.utils.helpers import is_move
-from mfg_package.utils.results import TickResult
+from marl_factory_grid.environment.rules import Rule
+from marl_factory_grid.utils.helpers import is_move
+from marl_factory_grid.utils.results import TickResult
 
-from mfg_package.environment import constants as c
-from mfg_package.modules.clean_up import constants as d
+from marl_factory_grid.environment import constants as c
+from marl_factory_grid.modules.clean_up import constants as d
 
 
 class DirtSmearOnMove(Rule):
 
     def __init__(self, smear_amount: float = 0.2):
         super().__init__()
         self.smear_amount = smear_amount
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/modules/destinations/actions.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/destinations/actions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Union
 
-from mfg_package.environment.actions import Action
-from mfg_package.utils.results import ActionResult
+from marl_factory_grid.environment.actions import Action
+from marl_factory_grid.utils.results import ActionResult
 
-from mfg_package.modules.destinations import constants as d, rewards as r
-from mfg_package.environment import constants as c
+from marl_factory_grid.modules.destinations import constants as d, rewards as r
+from marl_factory_grid.environment import constants as c
 
 
 class DestAction(Action):
 
     def __init__(self):
         super().__init__(d.DESTINATION)
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/modules/destinations/destinations.png` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/destinations/destinations.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/modules/destinations/entitites.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/destinations/entitites.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from collections import defaultdict
 
-from mfg_package.environment.entity.agent import Agent
-from mfg_package.environment.entity.entity import Entity
-from mfg_package.environment import constants as c
-from mfg_package.utils.render import RenderEntity
-from mfg_package.modules.destinations import constants as d
+from marl_factory_grid.environment.entity.agent import Agent
+from marl_factory_grid.environment.entity.entity import Entity
+from marl_factory_grid.environment import constants as c
+from marl_factory_grid.utils.render import RenderEntity
+from marl_factory_grid.modules.destinations import constants as d
 
 
 class Destination(Entity):
 
     @property
     def any_agent_has_dwelled(self):
         return bool(len(self._per_agent_times))
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/modules/destinations/groups.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/destinations/groups.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from mfg_package.environment.groups.env_objects import EnvObjects
-from mfg_package.environment.groups.mixins import PositionMixin
-from mfg_package.modules.destinations.entitites import Destination
+from marl_factory_grid.environment.groups.env_objects import EnvObjects
+from marl_factory_grid.environment.groups.mixins import PositionMixin
+from marl_factory_grid.modules.destinations.entitites import Destination
 
 
 class Destinations(PositionMixin, EnvObjects):
 
     _entity = Destination
     is_blocking_light: bool = False
     can_collide: bool = False
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/modules/destinations/rules.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/destinations/rules.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import List, Union
-from mfg_package.environment.rules import Rule
-from mfg_package.utils.results import TickResult, DoneResult
-from mfg_package.environment import constants as c
+from marl_factory_grid.environment.rules import Rule
+from marl_factory_grid.utils.results import TickResult, DoneResult
+from marl_factory_grid.environment import constants as c
 
-from mfg_package.modules.destinations import constants as d, rewards as r
-from mfg_package.modules.destinations.entitites import Destination
+from marl_factory_grid.modules.destinations import constants as d, rewards as r
+from marl_factory_grid.modules.destinations.entitites import Destination
 
 
 class DestinationReach(Rule):
 
     def __init__(self, n_dests: int = 1, tiles: Union[List, None] = None):
         super(DestinationReach, self).__init__()
         self.n_dests = n_dests or len(tiles)
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/modules/doors/actions.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/doors/actions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Union
 
-from mfg_package.environment.actions import Action
-from mfg_package.utils.results import ActionResult
+from marl_factory_grid.environment.actions import Action
+from marl_factory_grid.utils.results import ActionResult
 
-from mfg_package.modules.doors import constants as d, rewards as r
-from mfg_package.environment import constants as c
+from marl_factory_grid.modules.doors import constants as d, rewards as r
+from marl_factory_grid.environment import constants as c
 
 
 class DoorUse(Action):
 
     def __init__(self):
         super().__init__(d.ACTION_DOOR_USE)
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/modules/doors/constants.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/doors/constants.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/modules/doors/door_closed.png` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/doors/door_closed.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/modules/doors/door_open.png` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/doors/door_open.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/modules/doors/entitites.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/doors/entitites.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from mfg_package.environment.entity.entity import Entity
-from mfg_package.utils.render import RenderEntity
-from mfg_package.environment import constants as c
+from marl_factory_grid.environment.entity.entity import Entity
+from marl_factory_grid.utils.render import RenderEntity
+from marl_factory_grid.environment import constants as c
 
-from mfg_package.modules.doors import constants as d
+from marl_factory_grid.modules.doors import constants as d
 
 
 class DoorIndicator(Entity):
 
     @property
     def encoding(self):
         return d.VALUE_ACCESS_INDICATOR
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/modules/doors/rule_door_auto_close.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/doors/rule_door_auto_close.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from mfg_package.environment.rules import Rule
-from mfg_package.environment import constants as c
-from mfg_package.utils.results import TickResult
-from mfg_package.modules.doors import constants as d
+from marl_factory_grid.environment.rules import Rule
+from marl_factory_grid.environment import constants as c
+from marl_factory_grid.utils.results import TickResult
+from marl_factory_grid.modules.doors import constants as d
 
 
 class DoorAutoClose(Rule):
 
     def __init__(self, close_frequency: int = 10):
         super().__init__()
         self.close_frequency = close_frequency
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/modules/items/actions.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/items/actions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Union
 
-from mfg_package.environment.actions import Action
-from mfg_package.utils.results import ActionResult
+from marl_factory_grid.environment.actions import Action
+from marl_factory_grid.utils.results import ActionResult
 
-from mfg_package.modules.items import constants as i, rewards as r
-from mfg_package.environment import constants as c
+from marl_factory_grid.modules.items import constants as i, rewards as r
+from marl_factory_grid.environment import constants as c
 
 
 class ItemAction(Action):
 
     def __init__(self):
         super().__init__(i.ITEM_ACTION)
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/modules/items/assets/charge_pod.png` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/items/assets/charge_pod.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/modules/items/assets/dropofflocations.png` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/items/assets/dropofflocations.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/modules/items/assets/items.png` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/items/assets/items.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/modules/items/entitites.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/items/entitites.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from collections import deque
 
-from mfg_package.environment.entity.entity import Entity
-from mfg_package.environment import constants as c
-from mfg_package.utils.render import RenderEntity
-from mfg_package.modules.items import constants as i
+from marl_factory_grid.environment.entity.entity import Entity
+from marl_factory_grid.environment import constants as c
+from marl_factory_grid.utils.render import RenderEntity
+from marl_factory_grid.modules.items import constants as i
 
 
 class Item(Entity):
 
     def render(self):
         return RenderEntity(i.ITEM, self.tile.pos) if self.pos != c.VALUE_NO_POS else None
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/modules/items/groups.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/items/groups.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List
 
-from mfg_package.environment.groups.env_objects import EnvObjects
-from mfg_package.environment.groups.objects import Objects
-from mfg_package.environment.groups.mixins import PositionMixin, IsBoundMixin, HasBoundedMixin
-from mfg_package.environment.entity.wall_floor import Floor
-from mfg_package.environment.entity.agent import Agent
-from mfg_package.modules.items.entitites import Item, DropOffLocation
+from marl_factory_grid.environment.groups.env_objects import EnvObjects
+from marl_factory_grid.environment.groups.objects import Objects
+from marl_factory_grid.environment.groups.mixins import PositionMixin, IsBoundMixin, HasBoundedMixin
+from marl_factory_grid.environment.entity.wall_floor import Floor
+from marl_factory_grid.environment.entity.agent import Agent
+from marl_factory_grid.modules.items.entitites import Item, DropOffLocation
 
 
 class Items(PositionMixin, EnvObjects):
 
     _entity = Item
     is_blocking_light: bool = False
     can_collide: bool = False
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/modules/items/rules.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/items/rules.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import List
 
-from mfg_package.environment.rules import Rule
-from mfg_package.environment import constants as c
-from mfg_package.utils.results import TickResult
-from mfg_package.modules.items import constants as i
-from mfg_package.modules.items.entitites import DropOffLocation
+from marl_factory_grid.environment.rules import Rule
+from marl_factory_grid.environment import constants as c
+from marl_factory_grid.utils.results import TickResult
+from marl_factory_grid.modules.items import constants as i
+from marl_factory_grid.modules.items.entitites import DropOffLocation
 
 
 class ItemRules(Rule):
 
     def __init__(self, n_items: int = 5, spawn_frequency: int = 15,
                  n_locations: int = 5, max_dropoff_storage_size: int = 0):
         super().__init__()
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/modules/machines/entitites.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/machines/entitites.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from mfg_package.environment.entity.entity import Entity
-from mfg_package.utils.render import RenderEntity
-from mfg_package.environment import constants as c
-from mfg_package.utils.results import TickResult
-from mfg_package.modules.machines import constants as m, rewards as r
+from marl_factory_grid.environment.entity.entity import Entity
+from marl_factory_grid.utils.render import RenderEntity
+from marl_factory_grid.environment import constants as c
+from marl_factory_grid.utils.results import TickResult
+from marl_factory_grid.modules.machines import constants as m, rewards as r
 
 
 class Machine(Entity):
 
     @property
     def encoding(self):
         return self._encodings[self.state]
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/modules/machines/rules.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/machines/rules.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List
-from mfg_package.environment.rules import Rule
-from mfg_package.utils.results import TickResult, DoneResult
-from mfg_package.environment import constants as c
-from mfg_package.modules.machines import constants as m
-from mfg_package.modules.machines.entitites import Machine
+from marl_factory_grid.environment.rules import Rule
+from marl_factory_grid.utils.results import TickResult, DoneResult
+from marl_factory_grid.environment import constants as c
+from marl_factory_grid.modules.machines import constants as m
+from marl_factory_grid.modules.machines.entitites import Machine
 
 
 class MachineRule(Rule):
 
     def __init__(self, n_machines: int = 2):
         super(MachineRule, self).__init__()
         self.n_machines = n_machines
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/plotting/compare_runs.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/plotting/compare_runs.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import re
 from os import PathLike
 from pathlib import Path
 from typing import Union, List
 
 import pandas as pd
 
-from mfg_package.utils.helpers import IGNORED_DF_COLUMNS
-from mfg_package.plotting.plotting import prepare_plot
+from marl_factory_grid.utils.helpers import IGNORED_DF_COLUMNS
+from marl_factory_grid.plotting.plotting import prepare_plot
 
 MODEL_MAP = None
 
 
 def plot_single_run(run_path: Union[str, PathLike], use_tex: bool = False, column_keys=None):
     run_path = Path(run_path)
     df_list = list()
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/plotting/plotting.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/plotting/plotting.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/utils/config_parser.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/utils/config_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from os import PathLike
 from pathlib import Path
 from typing import Union
 
 import yaml
 
-from mfg_package.environment.groups.agents import Agents
-from mfg_package.environment.entity.agent import Agent
-from mfg_package.utils.helpers import locate_and_import_class
-from mfg_package.environment import constants as c
+from marl_factory_grid.environment.groups.agents import Agents
+from marl_factory_grid.environment.entity.agent import Agent
+from marl_factory_grid.utils.helpers import locate_and_import_class
+from marl_factory_grid.environment import constants as c
 
 DEFAULT_PATH = 'environment'
 MODULE_PATH = 'modules'
 
 
 class FactoryConfigParser(object):
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/utils/helpers.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/utils/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from collections import defaultdict
 from pathlib import PurePath, Path
 from typing import Union, Dict, List
 
 import numpy as np
 from numpy.typing import ArrayLike
 
-from mfg_package.environment import constants as c
+from marl_factory_grid.environment import constants as c
 
 """
 This file is used for:
     1. string based definition
         Use a class like `Constants`, to define attributes, which then reveal strings.
         These can be used for naming convention along the environments as well as keys for mappings such as dicts etc.
         When defining new envs, use class inheritance. 
@@ -214,15 +214,15 @@
     import sys
     sys.path.append("../../environment")
     folder_path = Path(folder_path).resolve()
     module_paths = [x.resolve() for x in folder_path.rglob('*.py') if x.is_file() and '__init__' not in x.name]
     # possible_package_path = folder_path / '__init__.py'
     # package = str(possible_package_path) if possible_package_path.exists() else None
     all_found_modules = list()
-    package_pos = next(idx for idx, x in enumerate(Path(__file__).resolve().parts) if x == 'mfg_package')
+    package_pos = next(idx for idx, x in enumerate(Path(__file__).resolve().parts) if x == 'marl_factory_grid')
     for module_path in module_paths:
         module_parts = [x.replace('.py', '') for idx, x in enumerate(module_path.parts) if idx >= package_pos]
         mod = importlib.import_module('.'.join(module_parts))
         all_found_modules.extend([x for x in dir(mod) if not(x.startswith('__') or len(x) < 2 or x.isupper())
                                   and x not in ['Entity',  'NamedTuple', 'List', 'Rule', 'Union', 'random', 'Floor'
                                                 'TickResult', 'ActionResult', 'Action', 'Agent', 'deque',
                                                 'BoundEntityMixin', 'RenderEntity', 'TemplateRule', 'defaultdict',
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/utils/level_parser.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/utils/level_parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from os import PathLike
 from pathlib import Path
 from typing import Dict
 
 import numpy as np
 
-from mfg_package.environment.groups.global_entities import Entities
-from mfg_package.environment.groups.wall_n_floors import Walls, Floors
-from mfg_package.utils import helpers as h
-from mfg_package.environment import constants as c
+from marl_factory_grid.environment.groups.global_entities import Entities
+from marl_factory_grid.environment.groups.wall_n_floors import Walls, Floors
+from marl_factory_grid.utils import helpers as h
+from marl_factory_grid.environment import constants as c
 
 
 class LevelParser(object):
 
     @property
     def pomdp_d(self):
         return self.pomdp_r * 2 + 1
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/utils/observation_builder.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/utils/observation_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 from collections import defaultdict
 from itertools import product
 from typing import Dict, List
 
 import numpy as np
 from numba import njit
 
-from mfg_package.environment.groups.utils import Combined
-from mfg_package.utils.states import Gamestate
+from marl_factory_grid.environment.groups.utils import Combined
+from marl_factory_grid.utils.states import Gamestate
 
-from mfg_package.environment import constants as c
+from marl_factory_grid.environment import constants as c
 
 
 class OBSBuilder(object):
 
     default_obs = [c.WALLS, c.OTHERS]
 
     @property
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/utils/renderer.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/utils/renderer.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from itertools import product
 
 import numpy as np
 import pygame
 from typing import Tuple, Union
 import time
 
-from mfg_package.utils.render import RenderEntity
+from marl_factory_grid.utils.render import RenderEntity
 
 AGENT: str = 'agent'
 STATE_IDLE: str = 'idle'
 STATE_MOVE: str = 'move'
 STATE_VALID: str = 'valid'
 STATE_INVALID: str = 'invalid'
 STATE_COLLISION: str = 'agent_collision'
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/utils/results.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/utils/results.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Union
 from dataclasses import dataclass
 
-from mfg_package.environment.entity.entity import Entity
+from marl_factory_grid.environment.entity.entity import Entity
 
 TYPE_VALUE  = 'value'
 TYPE_REWARD = 'reward'
 types = [TYPE_VALUE, TYPE_REWARD]
 
 @dataclass
 class InfoObject:
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/utils/states.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/utils/states.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List, Dict
 
 import numpy as np
 
-from mfg_package.environment.entity.wall_floor import Floor
-from mfg_package.environment.rules import Rule
-from mfg_package.utils.results import Result
-from mfg_package.environment import constants as c
+from marl_factory_grid.environment.entity.wall_floor import Floor
+from marl_factory_grid.environment.rules import Rule
+from marl_factory_grid.utils.results import Result
+from marl_factory_grid.environment import constants as c
 
 
 class StepRules:
     def __init__(self, *args):
         if args:
             self.rules = list(args)
         else:
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/utils/tools.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/utils/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import inspect
 from os import PathLike
 from pathlib import Path
 from typing import Union
 
 import yaml
 
-from mfg_package.environment import constants as c
-from mfg_package.utils.helpers import locate_and_import_class
+from marl_factory_grid.environment import constants as c
+from marl_factory_grid.utils.helpers import locate_and_import_class
 
 ACTION       = 'Action'
 GENERAL      = 'General'
 ENTITIES     = 'Objects'
 OBSERVATIONS = 'Observations'
 RULES        = 'Rule'
 ASSETS       = 'Assets'
@@ -29,15 +29,15 @@
     def explain_module(self, class_to_explain):
         parameters = inspect.signature(class_to_explain).parameters
         explained = {class_to_explain.__name__: {key: val.default for key, val in parameters.items() if key not in EXCLUDED}}
         return explained
 
     def _load_and_compare(self, compare_class, paths):
         conf = {}
-        package_pos = next(idx for idx, x in enumerate(Path(__file__).resolve().parts) if x == 'mfg_package')
+        package_pos = next(idx for idx, x in enumerate(Path(__file__).resolve().parts) if x == 'marl_factory_grid')
         for module_path in paths:
             module_parts = [x.replace('.py', '') for idx, x in enumerate(module_path.parts) if idx >= package_pos]
             mods = importlib.import_module('.'.join(module_parts))
             for key in mods.__dict__.keys():
                 if key not in EXCLUDED and not key.startswith('_'):
                     mod = mods.__getattribute__(key)
                     try:
```

### Comparing `Marl-Factory-Grid-0.0.7/mfg_package/utils/utility_classes.py` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/utils/utility_classes.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.7/quickstart/all_test_config.yaml` & `Marl-Factory-Grid-0.0.8/quickstart/all_test_config.yaml`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.7/quickstart/default_config.yaml` & `Marl-Factory-Grid-0.0.8/marl_factory_grid/quickstart/default_config.yaml`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.7/setup.py` & `Marl-Factory-Grid-0.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(name='Marl-Factory-Grid',
-      version='0.0.7',
+      version='0.0.8',
       description='A framework to research MARL agents in various setings.',
       author='Steffen Illium',
       author_email='steffen.illium@ifi.lmu.de',
       url='https://github.com/illiumst/marl-factory-grid/import',
       license='MIT',
       keywords=[
             'artificial intelligence',
```

