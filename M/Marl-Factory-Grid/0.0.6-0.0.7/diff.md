# Comparing `tmp/Marl-Factory-Grid-0.0.6.tar.gz` & `tmp/Marl-Factory-Grid-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Marl-Factory-Grid-0.0.6.tar", last modified: Tue Jun 20 08:27:49 2023, max compression
+gzip compressed data, was "Marl-Factory-Grid-0.0.7.tar", last modified: Tue Jun 20 16:25:10 2023, max compression
```

## Comparing `Marl-Factory-Grid-0.0.6.tar` & `Marl-Factory-Grid-0.0.7.tar`

### file list

```diff
@@ -1,170 +1,166 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:27:49.560525 Marl-Factory-Grid-0.0.6/
--rw-rw-rw-   0 root         (0) root         (0)      453 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)       45 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/MANIFEST.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:27:49.548525 Marl-Factory-Grid-0.0.6/Marl_Factory_Grid.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4116 2023-06-20 08:27:49.000000 Marl-Factory-Grid-0.0.6/Marl_Factory_Grid.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4192 2023-06-20 08:27:49.000000 Marl-Factory-Grid-0.0.6/Marl_Factory_Grid.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 08:27:49.000000 Marl-Factory-Grid-0.0.6/Marl_Factory_Grid.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-20 08:27:49.000000 Marl-Factory-Grid-0.0.6/Marl_Factory_Grid.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       48 2023-06-20 08:27:49.000000 Marl-Factory-Grid-0.0.6/Marl_Factory_Grid.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     4116 2023-06-20 08:27:49.560525 Marl-Factory-Grid-0.0.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3430 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:27:49.548525 Marl-Factory-Grid-0.0.6/algorithms/
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/algorithms/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:27:49.552525 Marl-Factory-Grid-0.0.6/algorithms/marl/
--rw-rw-rw-   0 root         (0) root         (0)      289 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/algorithms/marl/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8658 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/algorithms/marl/base_ac.py
--rw-rw-rw-   0 root         (0) root         (0)      636 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/algorithms/marl/example_config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2071 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/algorithms/marl/iac.py
--rw-rw-rw-   0 root         (0) root         (0)     3145 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/algorithms/marl/mappo.py
--rw-rw-rw-   0 root         (0) root         (0)     7763 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/algorithms/marl/memory.py
--rw-rw-rw-   0 root         (0) root         (0)     4784 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/algorithms/marl/networks.py
--rw-rw-rw-   0 root         (0) root         (0)     2225 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/algorithms/marl/seac.py
--rw-rw-rw-   0 root         (0) root         (0)     1269 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/algorithms/marl/snac.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:27:49.552525 Marl-Factory-Grid-0.0.6/algorithms/static/
--rw-rw-rw-   0 root         (0) root         (0)     5296 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/algorithms/static/TSP_base_agent.py
--rw-rw-rw-   0 root         (0) root         (0)     1033 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/algorithms/static/TSP_dirt_agent.py
--rw-rw-rw-   0 root         (0) root         (0)     2351 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/algorithms/static/TSP_item_agent.py
--rw-rw-rw-   0 root         (0) root         (0)     1061 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/algorithms/static/TSP_target_agent.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/algorithms/static/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      373 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/algorithms/static/random_agent.py
--rw-rw-rw-   0 root         (0) root         (0)     2679 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/algorithms/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:27:49.552525 Marl-Factory-Grid-0.0.6/environment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2626 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/actions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:27:49.552525 Marl-Factory-Grid-0.0.6/environment/assets/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/assets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:27:49.552525 Marl-Factory-Grid-0.0.6/environment/assets/agent/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/assets/agent/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8521 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/assets/agent/adversary.png
--rw-rw-rw-   0 root         (0) root         (0)     3402 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/assets/agent/agent.png
--rw-rw-rw-   0 root         (0) root         (0)    18857 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/assets/agent/agent_collision.png
--rw-rw-rw-   0 root         (0) root         (0)     1631 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/assets/agent/idle.png
--rw-rw-rw-   0 root         (0) root         (0)     1599 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/assets/agent/invalid.png
--rw-rw-rw-   0 root         (0) root         (0)     5933 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/assets/agent/move.png
--rw-rw-rw-   0 root         (0) root         (0)     5717 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/assets/agent/valid.png
--rw-rw-rw-   0 root         (0) root         (0)     1415 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/assets/wall.png
--rw-rw-rw-   0 root         (0) root         (0)     2766 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:27:49.552525 Marl-Factory-Grid-0.0.6/environment/entity/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/entity/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2302 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/entity/agent.py
--rw-rw-rw-   0 root         (0) root         (0)     2125 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/entity/entity.py
--rw-rw-rw-   0 root         (0) root         (0)      400 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/entity/mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     3330 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/entity/object.py
--rw-rw-rw-   0 root         (0) root         (0)     1204 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/entity/util.py
--rw-rw-rw-   0 root         (0) root         (0)     3075 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/entity/wall_floor.py
--rw-rw-rw-   0 root         (0) root         (0)     6881 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:27:49.552525 Marl-Factory-Grid-0.0.6/environment/groups/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/groups/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      875 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/groups/agents.py
--rw-rw-rw-   0 root         (0) root         (0)      921 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/groups/env_objects.py
--rw-rw-rw-   0 root         (0) root         (0)     2077 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/groups/global_entities.py
--rw-rw-rw-   0 root         (0) root         (0)     2940 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/groups/mixins.py
--rw-rw-rw-   0 root         (0) root         (0)     3884 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/groups/objects.py
--rw-rw-rw-   0 root         (0) root         (0)     2337 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/groups/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1534 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/groups/wall_n_floors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:27:49.552525 Marl-Factory-Grid-0.0.6/environment/logging/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/logging/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2202 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/logging/envmonitor.py
--rw-rw-rw-   0 root         (0) root         (0)     5475 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/logging/recorder.py
--rw-rw-rw-   0 root         (0) root         (0)      124 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/rewards.py
--rw-rw-rw-   0 root         (0) root         (0)     2565 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/rules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:27:49.556525 Marl-Factory-Grid-0.0.6/environment/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5146 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/utils/config_parser.py
--rw-rw-rw-   0 root         (0) root         (0)    10740 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/utils/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     2200 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/utils/level_parser.py
--rw-rw-rw-   0 root         (0) root         (0)    12457 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/utils/observation_builder.py
--rw-rw-rw-   0 root         (0) root         (0)      283 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/utils/render.py
--rw-rw-rw-   0 root         (0) root         (0)     5759 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/utils/renderer.py
--rw-rw-rw-   0 root         (0) root         (0)     1104 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/utils/results.py
--rw-rw-rw-   0 root         (0) root         (0)     3565 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/utils/states.py
--rw-rw-rw-   0 root         (0) root         (0)      811 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/environment/utils/utility_classes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:27:49.556525 Marl-Factory-Grid-0.0.6/modules/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:27:49.556525 Marl-Factory-Grid-0.0.6/modules/_template/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/_template/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      319 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/_template/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      571 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/_template/rules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:27:49.556525 Marl-Factory-Grid-0.0.6/modules/batteries/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/batteries/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1043 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/batteries/actions.py
--rw-rw-rw-   0 root         (0) root         (0)      523 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/batteries/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2330 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/batteries/entitites.py
--rw-rw-rw-   0 root         (0) root         (0)     1019 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/batteries/groups.py
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/batteries/rewards.py
--rw-rw-rw-   0 root         (0) root         (0)     2075 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/batteries/rules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:27:49.556525 Marl-Factory-Grid-0.0.6/modules/clean_up/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/clean_up/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1259 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/clean_up/actions.py
--rw-rw-rw-   0 root         (0) root         (0)      150 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/clean_up/constants.py
--rw-rw-rw-   0 root         (0) root         (0)    39296 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/clean_up/dirtpiles.png
--rw-rw-rw-   0 root         (0) root         (0)     1138 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/clean_up/entitites.py
--rw-rw-rw-   0 root         (0) root         (0)     2521 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/clean_up/groups.py
--rw-rw-rw-   0 root         (0) root         (0)       82 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/clean_up/rewards.py
--rw-rw-rw-   0 root         (0) root         (0)      551 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/clean_up/rule_done_on_all_clean.py
--rw-rw-rw-   0 root         (0) root         (0)      925 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/clean_up/rule_respawn.py
--rw-rw-rw-   0 root         (0) root         (0)     1006 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/clean_up/rule_smear_on_move.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:27:49.556525 Marl-Factory-Grid-0.0.6/modules/destinations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/destinations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      888 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/destinations/actions.py
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/destinations/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     7037 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/destinations/destinations.png
--rw-rw-rw-   0 root         (0) root         (0)     1735 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/destinations/entitites.py
--rw-rw-rw-   0 root         (0) root         (0)      780 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/destinations/groups.py
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/destinations/rewards.py
--rw-rw-rw-   0 root         (0) root         (0)     3650 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/destinations/rules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:27:49.556525 Marl-Factory-Grid-0.0.6/modules/doors/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/doors/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1104 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/doors/actions.py
--rw-rw-rw-   0 root         (0) root         (0)      793 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/doors/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      699 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/doors/door_closed.png
--rw-rw-rw-   0 root         (0) root         (0)     4224 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/doors/door_open.png
--rw-rw-rw-   0 root         (0) root         (0)     2680 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/doors/entitites.py
--rw-rw-rw-   0 root         (0) root         (0)      852 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/doors/groups.py
--rw-rw-rw-   0 root         (0) root         (0)       58 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/doors/rewards.py
--rw-rw-rw-   0 root         (0) root         (0)      840 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/doors/rule_door_auto_close.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:27:49.556525 Marl-Factory-Grid-0.0.6/modules/items/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/items/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1621 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/items/actions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:27:49.556525 Marl-Factory-Grid-0.0.6/modules/items/assets/
--rw-rw-rw-   0 root         (0) root         (0)     6610 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/items/assets/charge_pod.png
--rw-rw-rw-   0 root         (0) root         (0)     2318 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/items/assets/dropofflocations.png
--rw-rw-rw-   0 root         (0) root         (0)     3102 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/items/assets/items.png
--rw-rw-rw-   0 root         (0) root         (0)      234 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/items/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2014 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/items/entitites.py
--rw-rw-rw-   0 root         (0) root         (0)     3065 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/items/groups.py
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/items/rewards.py
--rw-rw-rw-   0 root         (0) root         (0)     3075 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/items/rules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:27:49.556525 Marl-Factory-Grid-0.0.6/modules/levels/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/levels/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1511 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/levels/large.txt
--rw-rw-rw-   0 root         (0) root         (0)     5827 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/levels/large_qquad.txt
--rw-rw-rw-   0 root         (0) root         (0)      207 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/levels/rooms.txt
--rw-rw-rw-   0 root         (0) root         (0)      168 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/levels/shelves.txt
--rw-rw-rw-   0 root         (0) root         (0)      155 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/levels/simple.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:27:49.560525 Marl-Factory-Grid-0.0.6/modules/machines/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/machines/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      178 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/machines/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1832 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/machines/entitites.py
--rw-rw-rw-   0 root         (0) root         (0)      385 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/machines/groups.py
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/machines/rewards.py
--rw-rw-rw-   0 root         (0) root         (0)      854 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/modules/machines/rules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:27:49.560525 Marl-Factory-Grid-0.0.6/plotting/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/plotting/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8628 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/plotting/compare_runs.py
--rw-rw-rw-   0 root         (0) root         (0)     2967 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/plotting/plotting.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:27:49.560525 Marl-Factory-Grid-0.0.6/quickstart/
--rw-rw-rw-   0 root         (0) root         (0)     2129 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/quickstart/all_test_config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1381 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/quickstart/default_config.yaml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-20 08:27:49.560525 Marl-Factory-Grid-0.0.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1366 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:27:49.560525 Marl-Factory-Grid-0.0.6/studies/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/studies/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    23919 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/studies/e_1.py
--rw-rw-rw-   0 root         (0) root         (0)    10156 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/studies/e_1_mix.py
--rw-rw-rw-   0 root         (0) root         (0)      786 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/studies/normalization_study.py
--rw-rw-rw-   0 root         (0) root         (0)      708 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/studies/playground_file.py
--rw-rw-rw-   0 root         (0) root         (0)    12396 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/studies/single_run_with_export.py
--rw-rw-rw-   0 root         (0) root         (0)     7417 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/studies/test.py
--rw-rw-rw-   0 root         (0) root         (0)     1295 2023-06-20 08:27:42.000000 Marl-Factory-Grid-0.0.6/studies/viz_policy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.034140 Marl-Factory-Grid-0.0.7/
+-rw-rw-rw-   0 root         (0) root         (0)      453 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)       45 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/MANIFEST.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.022140 Marl-Factory-Grid-0.0.7/Marl_Factory_Grid.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4328 2023-06-20 16:25:09.000000 Marl-Factory-Grid-0.0.7/Marl_Factory_Grid.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5413 2023-06-20 16:25:10.000000 Marl-Factory-Grid-0.0.7/Marl_Factory_Grid.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 16:25:09.000000 Marl-Factory-Grid-0.0.7/Marl_Factory_Grid.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-20 16:25:09.000000 Marl-Factory-Grid-0.0.7/Marl_Factory_Grid.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-20 16:25:09.000000 Marl-Factory-Grid-0.0.7/Marl_Factory_Grid.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     4328 2023-06-20 16:25:10.034140 Marl-Factory-Grid-0.0.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3625 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.022140 Marl-Factory-Grid-0.0.7/images/
+-rw-rw-rw-   0 root         (0) root         (0)   303396 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/images/Hooks_FIKS.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.022140 Marl-Factory-Grid-0.0.7/mfg_package/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 16:25:03.000000 Marl-Factory-Grid-0.0.7/mfg_package/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.022140 Marl-Factory-Grid-0.0.7/mfg_package/algorithms/
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/algorithms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.022140 Marl-Factory-Grid-0.0.7/mfg_package/algorithms/marl/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/algorithms/marl/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8698 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/algorithms/marl/base_ac.py
+-rw-rw-rw-   0 root         (0) root         (0)      636 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/algorithms/marl/example_config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2107 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/algorithms/marl/iac.py
+-rw-rw-rw-   0 root         (0) root         (0)     3184 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/algorithms/marl/mappo.py
+-rw-rw-rw-   0 root         (0) root         (0)     7763 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/algorithms/marl/memory.py
+-rw-rw-rw-   0 root         (0) root         (0)     4784 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/algorithms/marl/networks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2261 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/algorithms/marl/seac.py
+-rw-rw-rw-   0 root         (0) root         (0)     1293 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/algorithms/marl/snac.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.022140 Marl-Factory-Grid-0.0.7/mfg_package/algorithms/static/
+-rw-rw-rw-   0 root         (0) root         (0)     5319 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/algorithms/static/TSP_base_agent.py
+-rw-rw-rw-   0 root         (0) root         (0)     1057 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/algorithms/static/TSP_dirt_agent.py
+-rw-rw-rw-   0 root         (0) root         (0)     2375 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/algorithms/static/TSP_item_agent.py
+-rw-rw-rw-   0 root         (0) root         (0)     1097 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/algorithms/static/TSP_target_agent.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 16:25:03.000000 Marl-Factory-Grid-0.0.7/mfg_package/algorithms/static/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      385 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/algorithms/static/random_agent.py
+-rw-rw-rw-   0 root         (0) root         (0)     2687 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/algorithms/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.026140 Marl-Factory-Grid-0.0.7/mfg_package/environment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 16:25:03.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2615 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/actions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.026140 Marl-Factory-Grid-0.0.7/mfg_package/environment/assets/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 16:25:03.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/assets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.026140 Marl-Factory-Grid-0.0.7/mfg_package/environment/assets/agent/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 16:25:03.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/assets/agent/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8521 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/assets/agent/adversary.png
+-rw-rw-rw-   0 root         (0) root         (0)     3402 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/assets/agent/agent.png
+-rw-rw-rw-   0 root         (0) root         (0)    18857 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/assets/agent/agent_collision.png
+-rw-rw-rw-   0 root         (0) root         (0)     1631 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/assets/agent/idle.png
+-rw-rw-rw-   0 root         (0) root         (0)     1599 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/assets/agent/invalid.png
+-rw-rw-rw-   0 root         (0) root         (0)     5933 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/assets/agent/move.png
+-rw-rw-rw-   0 root         (0) root         (0)     5717 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/assets/agent/valid.png
+-rw-rw-rw-   0 root         (0) root         (0)     1415 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/assets/wall.png
+-rw-rw-rw-   0 root         (0) root         (0)     2766 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.026140 Marl-Factory-Grid-0.0.7/mfg_package/environment/entity/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 16:25:03.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/entity/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2338 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/entity/agent.py
+-rw-rw-rw-   0 root         (0) root         (0)     2157 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/entity/entity.py
+-rw-rw-rw-   0 root         (0) root         (0)      400 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/entity/mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     3314 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/entity/object.py
+-rw-rw-rw-   0 root         (0) root         (0)     1228 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/entity/util.py
+-rw-rw-rw-   0 root         (0) root         (0)     3099 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/entity/wall_floor.py
+-rw-rw-rw-   0 root         (0) root         (0)     6901 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.026140 Marl-Factory-Grid-0.0.7/mfg_package/environment/groups/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 16:25:03.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/groups/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      877 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/groups/agents.py
+-rw-rw-rw-   0 root         (0) root         (0)      945 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/groups/env_objects.py
+-rw-rw-rw-   0 root         (0) root         (0)     2044 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/groups/global_entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     2898 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/groups/mixins.py
+-rw-rw-rw-   0 root         (0) root         (0)     3896 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/groups/objects.py
+-rw-rw-rw-   0 root         (0) root         (0)     2363 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/groups/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1562 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/groups/wall_n_floors.py
+-rw-rw-rw-   0 root         (0) root         (0)      124 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/rewards.py
+-rw-rw-rw-   0 root         (0) root         (0)     2525 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/environment/rules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.026140 Marl-Factory-Grid-0.0.7/mfg_package/logging/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 16:25:03.000000 Marl-Factory-Grid-0.0.7/mfg_package/logging/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2226 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/logging/envmonitor.py
+-rw-rw-rw-   0 root         (0) root         (0)     5468 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/logging/recorder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.026140 Marl-Factory-Grid-0.0.7/mfg_package/modules/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 16:25:03.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.026140 Marl-Factory-Grid-0.0.7/mfg_package/modules/_template/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 16:25:03.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/_template/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      319 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/_template/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      583 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/_template/rules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.026140 Marl-Factory-Grid-0.0.7/mfg_package/modules/batteries/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 16:25:03.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/batteries/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/batteries/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)      523 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/batteries/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2390 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/batteries/entitites.py
+-rw-rw-rw-   0 root         (0) root         (0)     1055 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/batteries/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/batteries/rewards.py
+-rw-rw-rw-   0 root         (0) root         (0)     2111 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/batteries/rules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.030140 Marl-Factory-Grid-0.0.7/mfg_package/modules/clean_up/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 16:25:03.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/clean_up/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1295 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/clean_up/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)      150 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/clean_up/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)    39296 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/clean_up/dirtpiles.png
+-rw-rw-rw-   0 root         (0) root         (0)     1162 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/clean_up/entitites.py
+-rw-rw-rw-   0 root         (0) root         (0)     2581 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/clean_up/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)       82 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/clean_up/rewards.py
+-rw-rw-rw-   0 root         (0) root         (0)      587 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/clean_up/rule_done_on_all_clean.py
+-rw-rw-rw-   0 root         (0) root         (0)      949 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/clean_up/rule_respawn.py
+-rw-rw-rw-   0 root         (0) root         (0)     1042 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/clean_up/rule_smear_on_move.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.030140 Marl-Factory-Grid-0.0.7/mfg_package/modules/destinations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 16:25:03.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/destinations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      924 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/destinations/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/destinations/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     7037 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/destinations/destinations.png
+-rw-rw-rw-   0 root         (0) root         (0)     1783 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/destinations/entitites.py
+-rw-rw-rw-   0 root         (0) root         (0)      816 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/destinations/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/destinations/rewards.py
+-rw-rw-rw-   0 root         (0) root         (0)     3698 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/destinations/rules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.030140 Marl-Factory-Grid-0.0.7/mfg_package/modules/doors/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 16:25:03.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/doors/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1140 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/doors/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)      793 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/doors/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      699 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/doors/door_closed.png
+-rw-rw-rw-   0 root         (0) root         (0)     4224 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/doors/door_open.png
+-rw-rw-rw-   0 root         (0) root         (0)     2716 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/doors/entitites.py
+-rw-rw-rw-   0 root         (0) root         (0)      900 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/doors/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/doors/rewards.py
+-rw-rw-rw-   0 root         (0) root         (0)      876 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/doors/rule_door_auto_close.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.030140 Marl-Factory-Grid-0.0.7/mfg_package/modules/items/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 16:25:03.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/items/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1657 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/items/actions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.030140 Marl-Factory-Grid-0.0.7/mfg_package/modules/items/assets/
+-rw-rw-rw-   0 root         (0) root         (0)     6610 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/items/assets/charge_pod.png
+-rw-rw-rw-   0 root         (0) root         (0)     2318 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/items/assets/dropofflocations.png
+-rw-rw-rw-   0 root         (0) root         (0)     3102 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/items/assets/items.png
+-rw-rw-rw-   0 root         (0) root         (0)      234 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/items/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2050 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/items/entitites.py
+-rw-rw-rw-   0 root         (0) root         (0)     3137 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/items/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/items/rewards.py
+-rw-rw-rw-   0 root         (0) root         (0)     3123 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/items/rules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.030140 Marl-Factory-Grid-0.0.7/mfg_package/modules/levels/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 16:25:03.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/levels/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1511 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/levels/large.txt
+-rw-rw-rw-   0 root         (0) root         (0)     5827 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/levels/large_qquad.txt
+-rw-rw-rw-   0 root         (0) root         (0)      207 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/levels/rooms.txt
+-rw-rw-rw-   0 root         (0) root         (0)      168 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/levels/shelves.txt
+-rw-rw-rw-   0 root         (0) root         (0)      155 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/levels/simple.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.030140 Marl-Factory-Grid-0.0.7/mfg_package/modules/machines/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 16:25:03.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/machines/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      178 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/machines/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1868 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/machines/entitites.py
+-rw-rw-rw-   0 root         (0) root         (0)      421 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/machines/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/machines/rewards.py
+-rw-rw-rw-   0 root         (0) root         (0)      902 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/modules/machines/rules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.030140 Marl-Factory-Grid-0.0.7/mfg_package/plotting/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 16:25:03.000000 Marl-Factory-Grid-0.0.7/mfg_package/plotting/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8640 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/plotting/compare_runs.py
+-rw-rw-rw-   0 root         (0) root         (0)     2967 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/plotting/plotting.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.030140 Marl-Factory-Grid-0.0.7/mfg_package/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 16:25:03.000000 Marl-Factory-Grid-0.0.7/mfg_package/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5285 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/utils/config_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)    10876 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/utils/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2236 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/utils/level_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)    12481 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/utils/observation_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)      283 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/utils/render.py
+-rw-rw-rw-   0 root         (0) root         (0)     5759 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/utils/renderer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1108 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/utils/results.py
+-rw-rw-rw-   0 root         (0) root         (0)     3601 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/utils/states.py
+-rw-rw-rw-   0 root         (0) root         (0)     5655 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/utils/tools.py
+-rw-rw-rw-   0 root         (0) root         (0)      811 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/mfg_package/utils/utility_classes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:25:10.034140 Marl-Factory-Grid-0.0.7/quickstart/
+-rw-rw-rw-   0 root         (0) root         (0)     2129 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/quickstart/all_test_config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1381 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/quickstart/default_config.yaml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-20 16:25:10.034140 Marl-Factory-Grid-0.0.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1415 2023-06-20 16:25:02.000000 Marl-Factory-Grid-0.0.7/setup.py
```

### Comparing `Marl-Factory-Grid-0.0.6/Marl_Factory_Grid.egg-info/PKG-INFO` & `Marl-Factory-Grid-0.0.7/Marl_Factory_Grid.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: Marl-Factory-Grid
-Version: 0.0.6
+Version: 0.0.7
 Summary: A framework to research MARL agents in various setings.
 Home-page: https://github.com/illiumst/marl-factory-grid/import
 Author: Steffen Illium
 Author-email: steffen.illium@ifi.lmu.de
 License: MIT
-Keywords: artificial intelligence,pytorch,multiagent reinforcement learning,simulation,emergence,gymnasium,environment
+Keywords: artificial intelligence,pytorch,multiagent reinforcement learning,simulation,emergence,gymnasium,environment,deepdiff,natsort
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
@@ -92,40 +92,39 @@
 Varying levels are created by defining Walls, Floor or Doors in *.txt*-files (see [./environment/levels](./environment/levels) for examples).
 Define which *level* to use in your *configfile* as: 
 ```yaml
 General:
     level_name: rooms  # 'double', 'large', 'simple', ...
 ```
 ... or create your own , maybe with the help of [asciiflow.com](https://asciiflow.com/#/).
-Be sure to use '#' as Walls, '-' as free (walkable) Floor-Tiles, 'D' for Doors.
-Custom Entites (define you own) may bring their own "Symbol"
+Make sure to use `#` as [Walls](mfg_package/environment/entity/wall_floor.py), `-` as free (walkable) [Floor](mfg_package/environment/entity/wall_floor.py)-Tiles, `D` for [Walls](./modules/doors/entities.py).
+Other Entites (define you own) may bring their own `Symbols`
 
 #### Entites
-Entites are either [Objects](./environment/entity/object.py) for tracking stats or env. [Entity](./environment/entity/entity.py) which can interact.
+Entites, either [Objects](mfg_package/environment/entity/object.py) for tracking stats 
+or env. [Entity](mfg_package/environment/entity/entity.py) which can interact.
 Abstract Entities are provided.
 
 #### Groups
-[Groups](./environment/groups/objects.py) are entity Sets that provide administrative access to all group members. 
-All [Entites](./environment/entity/global_entities.py) are available at runtime as EnvState property.
+[Groups](mfg_package/environment/groups/objects.py) are entity Sets that provide administrative access to all group members. 
+All [Entites](mfg_package/environment/entity/global_entities.py) are available at runtime as EnvState property.
 
 
 #### Rules
-[Rules](./environment/entity/object.py) define how the environment behaves on micro-scale.
-Each of the hookes ('on_init', 'pre-step', 'on_step', 'post_step', 'on_done') 
+[Rules](mfg_package/environment/entity/object.py) define how the environment behaves on micro-scale.
+Each of the hookes (`on_init`, `pre_step`, `on_step`, '`post_step`', `on_done`) 
 provide env-access to implement customn logic, calculate rewards, or gather information.
 
+![Hooks](./images/Hooks_FIKS.png)
 
-
-
-[Results](./environment/entity/object.py) provide a way to return 'rule' evaluations such as rewards and state reports 
+[Results](mfg_package/environment/entity/object.py) provide a way to return `rule` evaluations such as rewards and state reports 
 back to the environment.
 #### Assets
-Make sure to bring your own assets for each Entity, that is living in the Gridworld, the 'Renderer' relies on it.
+Make sure to bring your own assets for each Entity living in the Gridworl as the `Renderer` relies on it.
 PNG-files (transparent background) of square aspect-ratio should do the job, in general.
 
-<div style="margin:0 auto;">
-<img src=".\environment\assets\wall.png"  width="10%"> | <img src=".\environment\assets\agent\agent.png"  width="10%">
-</div>
-
+<img src=".\environment\assets\wall.png"  width="5%"> 
+&nbsp&nbsp&nbsp&nbsp 
+<img src=".\environment\assets\agent\agent.png"  width="5%">
```

### Comparing `Marl-Factory-Grid-0.0.6/PKG-INFO` & `Marl-Factory-Grid-0.0.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: Marl-Factory-Grid
-Version: 0.0.6
+Version: 0.0.7
 Summary: A framework to research MARL agents in various setings.
 Home-page: https://github.com/illiumst/marl-factory-grid/import
 Author: Steffen Illium
 Author-email: steffen.illium@ifi.lmu.de
 License: MIT
-Keywords: artificial intelligence,pytorch,multiagent reinforcement learning,simulation,emergence,gymnasium,environment
+Keywords: artificial intelligence,pytorch,multiagent reinforcement learning,simulation,emergence,gymnasium,environment,deepdiff,natsort
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
@@ -92,40 +92,39 @@
 Varying levels are created by defining Walls, Floor or Doors in *.txt*-files (see [./environment/levels](./environment/levels) for examples).
 Define which *level* to use in your *configfile* as: 
 ```yaml
 General:
     level_name: rooms  # 'double', 'large', 'simple', ...
 ```
 ... or create your own , maybe with the help of [asciiflow.com](https://asciiflow.com/#/).
-Be sure to use '#' as Walls, '-' as free (walkable) Floor-Tiles, 'D' for Doors.
-Custom Entites (define you own) may bring their own "Symbol"
+Make sure to use `#` as [Walls](mfg_package/environment/entity/wall_floor.py), `-` as free (walkable) [Floor](mfg_package/environment/entity/wall_floor.py)-Tiles, `D` for [Walls](./modules/doors/entities.py).
+Other Entites (define you own) may bring their own `Symbols`
 
 #### Entites
-Entites are either [Objects](./environment/entity/object.py) for tracking stats or env. [Entity](./environment/entity/entity.py) which can interact.
+Entites, either [Objects](mfg_package/environment/entity/object.py) for tracking stats 
+or env. [Entity](mfg_package/environment/entity/entity.py) which can interact.
 Abstract Entities are provided.
 
 #### Groups
-[Groups](./environment/groups/objects.py) are entity Sets that provide administrative access to all group members. 
-All [Entites](./environment/entity/global_entities.py) are available at runtime as EnvState property.
+[Groups](mfg_package/environment/groups/objects.py) are entity Sets that provide administrative access to all group members. 
+All [Entites](mfg_package/environment/entity/global_entities.py) are available at runtime as EnvState property.
 
 
 #### Rules
-[Rules](./environment/entity/object.py) define how the environment behaves on micro-scale.
-Each of the hookes ('on_init', 'pre-step', 'on_step', 'post_step', 'on_done') 
+[Rules](mfg_package/environment/entity/object.py) define how the environment behaves on micro-scale.
+Each of the hookes (`on_init`, `pre_step`, `on_step`, '`post_step`', `on_done`) 
 provide env-access to implement customn logic, calculate rewards, or gather information.
 
+![Hooks](./images/Hooks_FIKS.png)
 
-
-
-[Results](./environment/entity/object.py) provide a way to return 'rule' evaluations such as rewards and state reports 
+[Results](mfg_package/environment/entity/object.py) provide a way to return `rule` evaluations such as rewards and state reports 
 back to the environment.
 #### Assets
-Make sure to bring your own assets for each Entity, that is living in the Gridworld, the 'Renderer' relies on it.
+Make sure to bring your own assets for each Entity living in the Gridworl as the `Renderer` relies on it.
 PNG-files (transparent background) of square aspect-ratio should do the job, in general.
 
-<div style="margin:0 auto;">
-<img src=".\environment\assets\wall.png"  width="10%"> | <img src=".\environment\assets\agent\agent.png"  width="10%">
-</div>
-
+<img src=".\environment\assets\wall.png"  width="5%"> 
+&nbsp&nbsp&nbsp&nbsp 
+<img src=".\environment\assets\agent\agent.png"  width="5%">
```

### Comparing `Marl-Factory-Grid-0.0.6/README.md` & `Marl-Factory-Grid-0.0.7/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -76,40 +76,39 @@
 Varying levels are created by defining Walls, Floor or Doors in *.txt*-files (see [./environment/levels](./environment/levels) for examples).
 Define which *level* to use in your *configfile* as: 
 ```yaml
 General:
     level_name: rooms  # 'double', 'large', 'simple', ...
 ```
 ... or create your own , maybe with the help of [asciiflow.com](https://asciiflow.com/#/).
-Be sure to use '#' as Walls, '-' as free (walkable) Floor-Tiles, 'D' for Doors.
-Custom Entites (define you own) may bring their own "Symbol"
+Make sure to use `#` as [Walls](mfg_package/environment/entity/wall_floor.py), `-` as free (walkable) [Floor](mfg_package/environment/entity/wall_floor.py)-Tiles, `D` for [Walls](./modules/doors/entities.py).
+Other Entites (define you own) may bring their own `Symbols`
 
 #### Entites
-Entites are either [Objects](./environment/entity/object.py) for tracking stats or env. [Entity](./environment/entity/entity.py) which can interact.
+Entites, either [Objects](mfg_package/environment/entity/object.py) for tracking stats 
+or env. [Entity](mfg_package/environment/entity/entity.py) which can interact.
 Abstract Entities are provided.
 
 #### Groups
-[Groups](./environment/groups/objects.py) are entity Sets that provide administrative access to all group members. 
-All [Entites](./environment/entity/global_entities.py) are available at runtime as EnvState property.
+[Groups](mfg_package/environment/groups/objects.py) are entity Sets that provide administrative access to all group members. 
+All [Entites](mfg_package/environment/entity/global_entities.py) are available at runtime as EnvState property.
 
 
 #### Rules
-[Rules](./environment/entity/object.py) define how the environment behaves on micro-scale.
-Each of the hookes ('on_init', 'pre-step', 'on_step', 'post_step', 'on_done') 
+[Rules](mfg_package/environment/entity/object.py) define how the environment behaves on micro-scale.
+Each of the hookes (`on_init`, `pre_step`, `on_step`, '`post_step`', `on_done`) 
 provide env-access to implement customn logic, calculate rewards, or gather information.
 
+![Hooks](./images/Hooks_FIKS.png)
 
-
-
-[Results](./environment/entity/object.py) provide a way to return 'rule' evaluations such as rewards and state reports 
+[Results](mfg_package/environment/entity/object.py) provide a way to return `rule` evaluations such as rewards and state reports 
 back to the environment.
 #### Assets
-Make sure to bring your own assets for each Entity, that is living in the Gridworld, the 'Renderer' relies on it.
+Make sure to bring your own assets for each Entity living in the Gridworl as the `Renderer` relies on it.
 PNG-files (transparent background) of square aspect-ratio should do the job, in general.
 
-<div style="margin:0 auto;">
-<img src=".\environment\assets\wall.png"  width="10%"> | <img src=".\environment\assets\agent\agent.png"  width="10%">
-</div>
-
+<img src=".\environment\assets\wall.png"  width="5%"> 
+&nbsp&nbsp&nbsp&nbsp 
+<img src=".\environment\assets\agent\agent.png"  width="5%">
```

### Comparing `Marl-Factory-Grid-0.0.6/algorithms/marl/base_ac.py` & `Marl-Factory-Grid-0.0.7/mfg_package/algorithms/marl/base_ac.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import torch
 from typing import Union, List, Dict
 import numpy as np
 from torch.distributions import Categorical
-from algorithms.marl.memory import MARLActorCriticMemory
-from algorithms.utils import add_env_props, instantiate_class
+from mfg_package.algorithms.marl.memory import MARLActorCriticMemory
+from mfg_package.algorithms.utils import add_env_props, instantiate_class
 from pathlib import Path
 import pandas as pd
 from collections import deque
 
 
 class Names:
     REWARD          = 'reward'
     DONE            = 'done'
     ACTION          = 'action'
     OBSERVATION     = 'observation'
     LOGITS          = 'logits'
     HIDDEN_ACTOR    = 'hidden_actor'
     HIDDEN_CRITIC   = 'hidden_critic'
     AGENT           = 'agent'
-    ENV             = 'env'
+    ENV             = 'environment'
     N_AGENTS        = 'n_agents'
     ALGORITHM       = 'algorithm'
     MAX_STEPS       = 'max_steps'
     N_STEPS         = 'n_steps'
     BUFFER_SIZE     = 'buffer_size'
     CRITIC          = 'critic'
     BATCH_SIZE      = 'bnatch_size'
@@ -168,15 +168,15 @@
                 last_action = action
                 last_hiddens = dict(hidden_actor=out.get(nms.HIDDEN_ACTOR,   None),
                                     hidden_critic=out.get(nms.HIDDEN_CRITIC, None)
                                     )
                 eps_rew += torch.tensor(reward)
             results.append(eps_rew.tolist() + [sum(eps_rew).item()] + [episode])
             episode += 1
-        agent_columns = [f'agent#{i}' for i in range(self.cfg['env']['n_agents'])]
+        agent_columns = [f'agent#{i}' for i in range(self.cfg['environment']['n_agents'])]
         results = pd.DataFrame(results, columns=agent_columns + ['sum', 'episode'])
         results = pd.melt(results, id_vars=['episode'], value_vars=agent_columns + ['sum'], value_name='reward', var_name='agent')
         return results
 
     @staticmethod
     def compute_advantages(critic, reward, done, gamma, gae_coef=0.0):
         tds = (reward + gamma * (1.0 - done) * critic[:, 1:].detach()) - critic[:, :-1]
```

### Comparing `Marl-Factory-Grid-0.0.6/algorithms/marl/example_config.yaml` & `Marl-Factory-Grid-0.0.7/mfg_package/algorithms/marl/example_config.yaml`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.6/algorithms/marl/iac.py` & `Marl-Factory-Grid-0.0.7/mfg_package/algorithms/marl/iac.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import torch
-from algorithms.marl.base_ac import BaseActorCritic, nms
-from algorithms.utils import instantiate_class
+from mfg_package.algorithms.marl.base_ac import BaseActorCritic, nms
+from mfg_package.algorithms.utils import instantiate_class
 from pathlib import Path
 from natsort import natsorted
-from algorithms.marl.memory import MARLActorCriticMemory
+from mfg_package.algorithms.marl.memory import MARLActorCriticMemory
 
 
 class LoopIAC(BaseActorCritic):
 
     def __init__(self, cfg):
         super(LoopIAC, self).__init__(cfg)
```

### Comparing `Marl-Factory-Grid-0.0.6/algorithms/marl/mappo.py` & `Marl-Factory-Grid-0.0.7/mfg_package/algorithms/marl/mappo.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from algorithms.marl.base_ac import Names as nms
-from algorithms.marl import LoopSNAC
-from algorithms.marl.memory import MARLActorCriticMemory
-import random
+from mfg_package.algorithms.marl.base_ac import Names as nms
+from mfg_package.algorithms.marl.snac import LoopSNAC
+from mfg_package.algorithms.marl.memory import MARLActorCriticMemory
 import torch
 from torch.distributions import Categorical
-from algorithms.utils import instantiate_class
+from mfg_package.algorithms.utils import instantiate_class
 
 
 class LoopMAPPO(LoopSNAC):
     def __init__(self, *args, **kwargs):
         super(LoopMAPPO, self).__init__(*args, **kwargs)
         self.reset_memory_after_epoch = False
```

### Comparing `Marl-Factory-Grid-0.0.6/algorithms/marl/memory.py` & `Marl-Factory-Grid-0.0.7/mfg_package/algorithms/marl/memory.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.6/algorithms/marl/networks.py` & `Marl-Factory-Grid-0.0.7/mfg_package/algorithms/marl/networks.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.6/algorithms/marl/seac.py` & `Marl-Factory-Grid-0.0.7/mfg_package/algorithms/marl/seac.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import torch
 from torch.distributions import Categorical
-from algorithms.marl.iac import LoopIAC
-from algorithms.marl.base_ac import nms
-from algorithms.marl.memory import MARLActorCriticMemory
+from mfg_package.algorithms.marl.iac import LoopIAC
+from mfg_package.algorithms.marl.base_ac import nms
+from mfg_package.algorithms.marl.memory import MARLActorCriticMemory
 
 
 class LoopSEAC(LoopIAC):
     def __init__(self, cfg):
         super(LoopSEAC, self).__init__(cfg)
 
     def actor_critic(self, tm, networks, gamma, entropy_coef, vf_coef, gae_coef=0.0, **kwargs):
```

### Comparing `Marl-Factory-Grid-0.0.6/algorithms/marl/snac.py` & `Marl-Factory-Grid-0.0.7/mfg_package/algorithms/marl/snac.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from algorithms.marl.base_ac import BaseActorCritic
-from algorithms.marl.base_ac import nms
+from mfg_package.algorithms.marl.base_ac import BaseActorCritic
+from mfg_package.algorithms.marl.base_ac import nms
 import torch
 from torch.distributions import Categorical
 from pathlib import Path
 
 
 class LoopSNAC(BaseActorCritic):
     def __init__(self, cfg):
```

### Comparing `Marl-Factory-Grid-0.0.6/algorithms/static/TSP_base_agent.py` & `Marl-Factory-Grid-0.0.7/mfg_package/algorithms/static/TSP_base_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 from random import choice
 
 import numpy as np
 
 import networkx as nx
 from networkx.algorithms.approximation import traveling_salesman as tsp
 
-
-from modules.doors import constants as do
-from environment import constants as c
-from environment.utils.helpers import MOVEMAP
+from mfg_package.modules.doors import constants as do
+from mfg_package.environment import constants as c
+from mfg_package.utils.helpers import MOVEMAP
 
 from abc import abstractmethod, ABC
 
 future_planning = 7
 
 
 def points_to_graph(coordiniates_or_tiles, allow_euclidean_connections=True, allow_manhattan_connections=True):
```

### Comparing `Marl-Factory-Grid-0.0.6/algorithms/static/TSP_dirt_agent.py` & `Marl-Factory-Grid-0.0.7/mfg_package/algorithms/static/TSP_dirt_agent.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from algorithms.static.TSP_base_agent import TSPBaseAgent
+from mfg_package.algorithms.static.TSP_base_agent import TSPBaseAgent
 
-from modules.clean_up import constants as di
+from mfg_package.modules.clean_up import constants as di
 
 future_planning = 7
 
 
 class TSPDirtAgent(TSPBaseAgent):
 
     def __init__(self, *args, **kwargs):
```

### Comparing `Marl-Factory-Grid-0.0.6/algorithms/static/TSP_item_agent.py` & `Marl-Factory-Grid-0.0.7/mfg_package/algorithms/static/TSP_item_agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 
-from algorithms.static.TSP_base_agent import TSPBaseAgent
+from mfg_package.algorithms.static.TSP_base_agent import TSPBaseAgent
 
-from modules.items import constants as i
+from mfg_package.modules.items import constants as i
 
 future_planning = 7
 inventory_size  = 3
 
 MODE_GET        = 'Mode_Get'
 MODE_BRING      = 'Mode_Bring'
```

### Comparing `Marl-Factory-Grid-0.0.6/algorithms/utils.py` & `Marl-Factory-Grid-0.0.7/mfg_package/algorithms/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 def load_yaml_file(path: Path):
     with path.open() as stream:
         cfg = yaml.load(stream, Loader=yaml.FullLoader)
     return cfg
 
 
 def add_env_props(cfg):
-    env = instantiate_class(cfg['env'].copy())
+    env = instantiate_class(cfg['environment'].copy())
     cfg['agent'].update(dict(observation_size=list(env.observation_space.shape),
                              n_actions=env.action_space.n))
 
 
 class Checkpointer(object):
     def __init__(self, experiment_name, root, config, total_steps, n_checkpoints):
         self.path = root / experiment_name
```

### Comparing `Marl-Factory-Grid-0.0.6/environment/actions.py` & `Marl-Factory-Grid-0.0.7/mfg_package/environment/actions.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import abc
 from typing import Union
 
-from environment import rewards as r
-from environment import constants as c
-from environment.utils.helpers import MOVEMAP
-from environment.utils.results import ActionResult
+from mfg_package.environment import rewards as r, constants as c
+from mfg_package.utils.helpers import MOVEMAP
+from mfg_package.utils.results import ActionResult
 
 
 class Action(abc.ABC):
 
     @property
     def name(self):
         return self._identifier
```

### Comparing `Marl-Factory-Grid-0.0.6/environment/assets/agent/adversary.png` & `Marl-Factory-Grid-0.0.7/mfg_package/environment/assets/agent/adversary.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.6/environment/assets/agent/agent.png` & `Marl-Factory-Grid-0.0.7/mfg_package/environment/assets/agent/agent.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.6/environment/assets/agent/agent_collision.png` & `Marl-Factory-Grid-0.0.7/mfg_package/environment/assets/agent/agent_collision.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.6/environment/assets/agent/idle.png` & `Marl-Factory-Grid-0.0.7/mfg_package/environment/assets/agent/idle.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.6/environment/assets/agent/invalid.png` & `Marl-Factory-Grid-0.0.7/mfg_package/environment/assets/agent/invalid.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.6/environment/assets/agent/move.png` & `Marl-Factory-Grid-0.0.7/mfg_package/environment/assets/agent/move.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.6/environment/assets/agent/valid.png` & `Marl-Factory-Grid-0.0.7/mfg_package/environment/assets/agent/valid.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.6/environment/assets/wall.png` & `Marl-Factory-Grid-0.0.7/mfg_package/environment/assets/wall.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.6/environment/constants.py` & `Marl-Factory-Grid-0.0.7/mfg_package/environment/constants.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.6/environment/entity/agent.py` & `Marl-Factory-Grid-0.0.7/mfg_package/environment/entity/agent.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import List, Union
 
-from environment import constants as c
-from environment.actions import Action
-from environment.entity.entity import Entity
-from environment.utils.render import RenderEntity
-from environment.utils import renderer
-from environment.utils.helpers import is_move
-from environment.utils.results import ActionResult, Result
+from mfg_package.environment import constants as c
+from mfg_package.environment.actions import Action
+from mfg_package.environment.entity.entity import Entity
+from mfg_package.utils.render import RenderEntity
+from mfg_package.utils import renderer
+from mfg_package.utils.helpers import is_move
+from mfg_package.utils.results import ActionResult, Result
 
 
 class Agent(Entity):
 
     @property
     def obs_tag(self):
         return self.name
```

### Comparing `Marl-Factory-Grid-0.0.6/environment/entity/entity.py` & `Marl-Factory-Grid-0.0.7/mfg_package/environment/entity/entity.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import abc
 
-from environment import constants as c
-from environment.entity.object import EnvObject
-from environment.utils.render import RenderEntity
+from mfg_package.environment import constants as c
+from mfg_package.environment.entity.object import EnvObject
+from mfg_package.utils.render import RenderEntity
 
 
 class Entity(EnvObject, abc.ABC):
-    """Full Env Entity that lives on the env Grid. Doors, Items, DirtPile etc..."""
+    """Full Env Entity that lives on the environment Grid. Doors, Items, DirtPile etc..."""
 
     @property
     def has_position(self):
         return self.pos != c.VALUE_NO_POS
 
     @property
     def x(self):
```

### Comparing `Marl-Factory-Grid-0.0.6/environment/entity/object.py` & `Marl-Factory-Grid-0.0.7/mfg_package/environment/entity/object.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from abc import ABC, abstractmethod
 from collections import defaultdict
 from typing import Union
 
-from environment import constants as c
+from mfg_package.environment import constants as c
 
 
 class Object:
 
     """Generell Objects for Organisation and Maintanance such as Actions etc..."""
 
     _u_idx = defaultdict(lambda: 0)
@@ -63,15 +62,15 @@
 
     def del_observer(self, observer):
         self.observers.remove(observer)
 
 
 class EnvObject(Object):
 
-    """Objects that hold Information that are observable, but have no position on the env grid. Inventories etc..."""
+    """Objects that hold Information that are observable, but have no position on the environment grid. Inventories etc..."""
 
     _u_idx = defaultdict(lambda: 0)
     
     @property
     def obs_tag(self):
         try:
             return self._collection.name or self.name
```

### Comparing `Marl-Factory-Grid-0.0.6/environment/entity/util.py` & `Marl-Factory-Grid-0.0.7/mfg_package/environment/entity/util.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import math
 
 import numpy as np
 
-from environment.entity.mixin import BoundEntityMixin
-from environment.entity.object import Object, EnvObject
+from mfg_package.environment.entity.mixin import BoundEntityMixin
+from mfg_package.environment.entity.object import Object, EnvObject
 
 
 ##########################################################################
 # ####################### Objects and Entitys ########################## #
 ##########################################################################
```

### Comparing `Marl-Factory-Grid-0.0.6/environment/entity/wall_floor.py` & `Marl-Factory-Grid-0.0.7/mfg_package/environment/entity/wall_floor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List
 
 import numpy as np
 
-from environment import constants as c
-from environment.entity.object import EnvObject
-from environment.utils.render import RenderEntity
-from environment.utils import helpers as h
+from mfg_package.environment import constants as c
+from mfg_package.environment.entity.object import EnvObject
+from mfg_package.utils.render import RenderEntity
+from mfg_package.utils import helpers as h
 
 
 class Floor(EnvObject):
 
     @property
     def has_position(self):
         return True
```

### Comparing `Marl-Factory-Grid-0.0.6/environment/factory.py` & `Marl-Factory-Grid-0.0.7/mfg_package/environment/factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 from itertools import chain
 from os import PathLike
 from pathlib import Path
 from typing import Union
 
 import gymnasium as gym
 
-from environment.utils.level_parser import LevelParser
-from environment.utils.observation_builder import OBSBuilder
-from environment.utils.config_parser import FactoryConfigParser
-from environment.utils import helpers as h
-import environment.constants as c
+from mfg_package.utils.level_parser import LevelParser
+from mfg_package.utils.observation_builder import OBSBuilder
+from mfg_package.utils.config_parser import FactoryConfigParser
+from mfg_package.utils import helpers as h
+import mfg_package.environment.constants as c
 
-from environment.utils.states import Gamestate
+from mfg_package.utils.states import Gamestate
 
 REC_TAC = 'rec_'
 
 
 class BaseFactory(gym.Env):
 
     @property
@@ -122,15 +122,15 @@
         info.update(reset_info)
         return None, [x for x in obs.values()], reward, done, info
 
     def summarize_step_results(self, tick_results: list, done_check_results: list) -> (int, dict, bool):
         # Returns: Reward, Info
         rewards = defaultdict(lambda: 0.0)
 
-        # Gather per agent env rewards and
+        # Gather per agent environment rewards and
         # Combine Info dicts into a global one
         combined_info_dict = defaultdict(lambda: 0.0)
         for result in chain(tick_results, done_check_results):
             if result.reward is not None:
                 try:
                     rewards[result.entity.name] += result.reward
                 except AttributeError:
@@ -167,15 +167,15 @@
     def stop_recording(self):
         self.conf.do_record = False
         return not self.conf.do_record
 
     # noinspection PyGlobalUndefined
     def render(self, mode='human'):
         if not self._renderer:  # lazy init
-            from environment.utils.renderer import Renderer
+            from mfg_package.utils.renderer import Renderer
             global Renderer
             self._renderer = Renderer(self.map.level_shape,  view_radius=self.conf.pomdp_r, fps=10)
 
         render_entities = self.state.entities.render()
         if self.conf.pomdp_r:
             for render_entity in render_entities:
                 if render_entity.name == c.AGENT:
```

### Comparing `Marl-Factory-Grid-0.0.6/environment/groups/agents.py` & `Marl-Factory-Grid-0.0.7/mfg_package/environment/groups/agents.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from environment.groups.env_objects import EnvObjects
-from environment.groups.mixins import PositionMixin
-from environment.entity.agent import Agent
-import environment.constants as c
+from mfg_package.environment.groups.env_objects import EnvObjects
+from mfg_package.environment.groups.mixins import PositionMixin
+from mfg_package.environment.entity.agent import Agent
 
 
 class Agents(PositionMixin, EnvObjects):
     _entity = Agent
     is_blocking_light = False
     can_move = True
```

### Comparing `Marl-Factory-Grid-0.0.6/environment/groups/env_objects.py` & `Marl-Factory-Grid-0.0.7/mfg_package/environment/groups/env_objects.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from environment.groups.objects import Objects
-from environment.entity.object import EnvObject
+from mfg_package.environment.groups.objects import Objects
+from mfg_package.environment.entity.object import EnvObject
 
 
 class EnvObjects(Objects):
 
     _entity = EnvObject
     is_blocking_light: bool = False
     can_collide: bool = False
```

### Comparing `Marl-Factory-Grid-0.0.6/environment/groups/global_entities.py` & `Marl-Factory-Grid-0.0.7/mfg_package/environment/groups/global_entities.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from collections import defaultdict
 from operator import itemgetter
 from typing import Dict
 
-from environment.groups.objects import Objects
-from environment.entity.entity import Entity
-from environment.utils.helpers import POS_MASK
+from mfg_package.environment.groups.objects import Objects
+from mfg_package.utils.helpers import POS_MASK
 
 
 class Entities(Objects):
     _entity = Objects
 
     @staticmethod
     def neighboring_positions(pos):
```

### Comparing `Marl-Factory-Grid-0.0.6/environment/groups/mixins.py` & `Marl-Factory-Grid-0.0.7/mfg_package/environment/groups/mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,10 @@
-from abc import ABC
-from typing import Tuple
+from mfg_package.environment import constants as c
 
-import numpy as np
-
-from environment import constants as c
-
-from environment.entity.entity import Entity
+from mfg_package.environment.entity.entity import Entity
 
 
 # noinspection PyUnresolvedReferences,PyTypeChecker,PyArgumentList
 class PositionMixin:
 
     _entity = Entity
     is_blocking_light: bool = True
```

### Comparing `Marl-Factory-Grid-0.0.6/environment/groups/objects.py` & `Marl-Factory-Grid-0.0.7/mfg_package/environment/groups/objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from collections import defaultdict
 from typing import List
 
 import numpy as np
 
-from environment.entity.object import Object
+from mfg_package.environment.entity.object import Object
 
 
 class Objects:
     _entity = Object
 
     @property
     def observers(self):
```

### Comparing `Marl-Factory-Grid-0.0.6/environment/groups/utils.py` & `Marl-Factory-Grid-0.0.7/mfg_package/environment/groups/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-import numbers
-from typing import List, Union, Dict
+from typing import List, Union
 
 import numpy as np
 
-from environment.groups.env_objects import EnvObjects
-from environment.groups.objects import Objects
-from environment.groups.mixins import HasBoundedMixin, PositionMixin
-from environment.entity.util import PlaceHolder, GlobalPosition
-from environment.utils import helpers as h
-from environment import constants as c
+from mfg_package.environment.groups.env_objects import EnvObjects
+from mfg_package.environment.groups.objects import Objects
+from mfg_package.environment.groups.mixins import HasBoundedMixin, PositionMixin
+from mfg_package.environment.entity.util import GlobalPosition
+from mfg_package.utils import helpers as h
+from mfg_package.environment import constants as c
 
 
 class Combined(PositionMixin, EnvObjects):
 
     @property
     def name(self):
         return f'{super().name}({self._ident or self._names})'
```

### Comparing `Marl-Factory-Grid-0.0.6/environment/groups/wall_n_floors.py` & `Marl-Factory-Grid-0.0.7/mfg_package/environment/groups/wall_n_floors.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import random
 from typing import List
 
-import numpy as np
-
-from environment import constants as c
-from environment.groups.env_objects import EnvObjects
-from environment.groups.mixins import PositionMixin
-from environment.entity.wall_floor import Wall, Floor
+from mfg_package.environment import constants as c
+from mfg_package.environment.groups.env_objects import EnvObjects
+from mfg_package.environment.groups.mixins import PositionMixin
+from mfg_package.environment.entity.wall_floor import Wall, Floor
 
 
 class Walls(PositionMixin, EnvObjects):
     _entity = Wall
     symbol = c.SYMBOL_WALL
 
     def __init__(self, *args, **kwargs):
```

### Comparing `Marl-Factory-Grid-0.0.6/environment/logging/envmonitor.py` & `Marl-Factory-Grid-0.0.7/mfg_package/logging/envmonitor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import pickle
 from os import PathLike
 from pathlib import Path
 from typing import Union
 
 from gymnasium import Wrapper
 
-from environment.utils.helpers import IGNORED_DF_COLUMNS
-from environment.factory import REC_TAC
+from mfg_package.utils.helpers import IGNORED_DF_COLUMNS
+from mfg_package.environment.factory import REC_TAC
 
 import pandas as pd
 
-from plotting.compare_runs import plot_single_run
+from mfg_package.plotting.compare_runs import plot_single_run
 
 
 class EnvMonitor(Wrapper):
 
     ext = 'png'
 
     def __init__(self, env, filepath: Union[str, PathLike] = None):
```

### Comparing `Marl-Factory-Grid-0.0.6/environment/logging/recorder.py` & `Marl-Factory-Grid-0.0.7/mfg_package/logging/recorder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import warnings
 from collections import defaultdict
 from os import PathLike
 from pathlib import Path
 from typing import Union
 
+import yaml
 from gymnasium import Wrapper
 
 import numpy as np
 import pandas as pd
-import simplejson
 
-from environment.factory import REC_TAC
+from mfg_package.environment.factory import REC_TAC
 
 
 class EnvRecorder(Wrapper):
 
     def __init__(self, env, entities: str = 'all', filepath: Union[str, PathLike] = None, freq: int = 0):
         super(EnvRecorder, self).__init__(env)
         self.filepath = filepath
@@ -77,29 +77,29 @@
                      save_trajectory_map=False,
                      ):
         filepath = Path(filepath or self.filepath)
         filepath.parent.mkdir(exist_ok=True, parents=True)
         # cls.out_file.unlink(missing_ok=True)
         with filepath.open('w') as f:
             if only_deltas:
-                from deepdiff import DeepDiff, Delta
+                from deepdiff import DeepDiff
                 diff_dict = [DeepDiff(t1,t2, ignore_order=True)
                              for t1, t2 in zip(self._recorder_out_list, self._recorder_out_list[1:])
                              ]
                 out_dict = {'episodes': diff_dict}
 
             else:
                 out_dict = {'episodes': self._recorder_out_list}
             out_dict.update(
                 {'n_episodes': self._episode_counter,
                  'env_params': self.env.params,
                  'header': self.env.summarize_header
                  })
             try:
-                simplejson.dump(out_dict, f, indent=4)
+                yaml.dump(out_dict, f, indent=4)
             except TypeError:
                 print('Shit')
 
         if save_occupation_map:
             a = np.zeros((15, 15))
             # noinspection PyTypeChecker
             for episode in out_dict['episodes']:
```

### Comparing `Marl-Factory-Grid-0.0.6/environment/rules.py` & `Marl-Factory-Grid-0.0.7/mfg_package/environment/rules.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import abc
-from typing import Union, List
+from typing import List
 
-from environment.utils.results import Result, TickResult, DoneResult, ActionResult
-from environment import constants as c
-from environment import rewards as r
+from mfg_package.utils.results import TickResult, DoneResult
+from mfg_package.environment import rewards as r, constants as c
 
 
 class Rule(abc.ABC):
 
     @property
     def name(self):
         return self.__class__.__name__
```

### Comparing `Marl-Factory-Grid-0.0.6/environment/utils/config_parser.py` & `Marl-Factory-Grid-0.0.7/mfg_package/utils/config_parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from os import PathLike
 from pathlib import Path
 from typing import Union
 
 import yaml
 
-from environment.groups.global_entities import Entities
-from environment.groups.agents import Agents
-from environment.entity.agent import Agent
-from environment.utils.helpers import locate_and_import_class
-from environment import constants as c
-
+from mfg_package.environment.groups.agents import Agents
+from mfg_package.environment.entity.agent import Agent
+from mfg_package.utils.helpers import locate_and_import_class
+from mfg_package.environment import constants as c
 
 DEFAULT_PATH = 'environment'
 MODULE_PATH = 'modules'
 
 
 class FactoryConfigParser(object):
 
@@ -90,14 +88,15 @@
             actions = list()
             if c.DEFAULTS in self.agents[name]['Actions']:
                 actions.extend(self.default_actions)
             actions.extend(x for x in self.agents[name]['Actions'] if x != c.DEFAULTS)
             parsed_actions = list()
             for action in actions:
                 folder_path = MODULE_PATH if action not in base_env_actions else DEFAULT_PATH
+                folder_path = (Path(__file__) / '..' / '..' / '..' / folder_path)
                 try:
                     class_or_classes = locate_and_import_class(action, folder_path)
                 except AttributeError:
                     class_or_classes = locate_and_import_class(action, self.custom_modules_path)
                 try:
                     parsed_actions.extend(class_or_classes)
                 except TypeError:
@@ -122,14 +121,15 @@
             for rule in self.default_rules:
                 if rule not in rules:
                     rules.append(rule)
         rules.extend(x for x in self.rules if x != c.DEFAULTS)
 
         for rule in rules:
             folder_path = MODULE_PATH if rule not in self.default_rules else DEFAULT_PATH
+            folder_path = (Path(__file__) / '..' / '..' / '..' / folder_path)
             try:
                 rule_class = locate_and_import_class(rule, folder_path)
             except AttributeError:
                 rule_class = locate_and_import_class(rule, self.custom_modules_path)
             rule_kwargs = self.rules.get(rule, {})
             rules_classes.update({rule: {'class': rule_class, 'kwargs': rule_kwargs}})
         return rules_classes
```

### Comparing `Marl-Factory-Grid-0.0.6/environment/utils/helpers.py` & `Marl-Factory-Grid-0.0.7/mfg_package/utils/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from collections import defaultdict
 from pathlib import PurePath, Path
 from typing import Union, Dict, List
 
 import numpy as np
 from numpy.typing import ArrayLike
 
-from environment import constants as c
+from mfg_package.environment import constants as c
 
 """
 This file is used for:
     1. string based definition
         Use a class like `Constants`, to define attributes, which then reveal strings.
         These can be used for naming convention along the environments as well as keys for mappings such as dicts etc.
         When defining new envs, use class inheritance. 
@@ -208,30 +208,31 @@
     else:
         return c.AGENT, 'idle'
 
 
 def locate_and_import_class(class_name, folder_path: Union[str, PurePath] = ''):
     """Locate an object by name or dotted path, importing as necessary."""
     import sys
-    sys.path.append("..")
+    sys.path.append("../../environment")
     folder_path = Path(folder_path).resolve()
     module_paths = [x.resolve() for x in folder_path.rglob('*.py') if x.is_file() and '__init__' not in x.name]
     # possible_package_path = folder_path / '__init__.py'
     # package = str(possible_package_path) if possible_package_path.exists() else None
     all_found_modules = list()
-    package_pos = next(idx for idx, x in enumerate(Path(__file__).resolve().parts) if x == 'environment')
+    package_pos = next(idx for idx, x in enumerate(Path(__file__).resolve().parts) if x == 'mfg_package')
     for module_path in module_paths:
         module_parts = [x.replace('.py', '') for idx, x in enumerate(module_path.parts) if idx >= package_pos]
         mod = importlib.import_module('.'.join(module_parts))
         all_found_modules.extend([x for x in dir(mod) if not(x.startswith('__') or len(x) < 2 or x.isupper())
                                   and x not in ['Entity',  'NamedTuple', 'List', 'Rule', 'Union', 'random', 'Floor'
                                                 'TickResult', 'ActionResult', 'Action', 'Agent', 'deque',
                                                 'BoundEntityMixin', 'RenderEntity', 'TemplateRule', 'defaultdict',
                                                 'is_move', 'Objects', 'PositionMixin', 'IsBoundMixin', 'EnvObject',
-                                                'EnvObjects']])
+                                                'EnvObjects', 'Dict', 'locate_and_import_class', 'yaml', 'Any',
+                                                'inspect']])
         try:
             model_class = mod.__getattribute__(class_name)
             return model_class
         except AttributeError:
             continue
     raise AttributeError(f'Class "{class_name}" was not found!!!"\n'
                          f'Check the {folder_path.name} name.\n'
```

### Comparing `Marl-Factory-Grid-0.0.6/environment/utils/level_parser.py` & `Marl-Factory-Grid-0.0.7/mfg_package/utils/level_parser.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from os import PathLike
 from pathlib import Path
 from typing import Dict
 
 import numpy as np
 
-from environment.groups.global_entities import Entities
-from environment.groups.wall_n_floors import Walls, Floors
-from environment.utils import helpers as h
-from environment import constants as c
+from mfg_package.environment.groups.global_entities import Entities
+from mfg_package.environment.groups.wall_n_floors import Walls, Floors
+from mfg_package.utils import helpers as h
+from mfg_package.environment import constants as c
 
 
 class LevelParser(object):
 
     @property
     def pomdp_d(self):
         return self.pomdp_r * 2 + 1
```

### Comparing `Marl-Factory-Grid-0.0.6/environment/utils/observation_builder.py` & `Marl-Factory-Grid-0.0.7/mfg_package/utils/observation_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 from collections import defaultdict
 from itertools import product
 from typing import Dict, List
 
 import numpy as np
 from numba import njit
 
-from environment.groups.utils import Combined
-from environment.utils.states import Gamestate
+from mfg_package.environment.groups.utils import Combined
+from mfg_package.utils.states import Gamestate
 
-from environment import constants as c
+from mfg_package.environment import constants as c
 
 
 class OBSBuilder(object):
 
     default_obs = [c.WALLS, c.OTHERS]
 
     @property
```

### Comparing `Marl-Factory-Grid-0.0.6/environment/utils/renderer.py` & `Marl-Factory-Grid-0.0.7/mfg_package/utils/renderer.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from itertools import product
 
 import numpy as np
 import pygame
 from typing import Tuple, Union
 import time
 
-from environment.utils.render import RenderEntity
+from mfg_package.utils.render import RenderEntity
 
 AGENT: str = 'agent'
 STATE_IDLE: str = 'idle'
 STATE_MOVE: str = 'move'
 STATE_VALID: str = 'valid'
 STATE_INVALID: str = 'invalid'
 STATE_COLLISION: str = 'agent_collision'
```

### Comparing `Marl-Factory-Grid-0.0.6/environment/utils/results.py` & `Marl-Factory-Grid-0.0.7/mfg_package/utils/results.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Union
-from dataclasses import dataclass, asdict
+from dataclasses import dataclass
 
-from environment.entity.entity import Entity
+from mfg_package.environment.entity.entity import Entity
 
 TYPE_VALUE  = 'value'
 TYPE_REWARD = 'reward'
 types = [TYPE_VALUE, TYPE_REWARD]
 
 @dataclass
 class InfoObject:
```

### Comparing `Marl-Factory-Grid-0.0.6/environment/utils/states.py` & `Marl-Factory-Grid-0.0.7/mfg_package/utils/states.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List, Dict
 
 import numpy as np
 
-from environment.entity.wall_floor import Floor
-from environment.rules import Rule
-from environment.utils.results import Result
-from environment import constants as c
+from mfg_package.environment.entity.wall_floor import Floor
+from mfg_package.environment.rules import Rule
+from mfg_package.utils.results import Result
+from mfg_package.environment import constants as c
 
 
 class StepRules:
     def __init__(self, *args):
         if args:
             self.rules = list(args)
         else:
```

### Comparing `Marl-Factory-Grid-0.0.6/environment/utils/utility_classes.py` & `Marl-Factory-Grid-0.0.7/mfg_package/utils/utility_classes.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.6/modules/_template/rules.py` & `Marl-Factory-Grid-0.0.7/mfg_package/modules/_template/rules.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
-from environment.rules import Rule
-from environment.utils.results import TickResult, DoneResult
+from mfg_package.environment.rules import Rule
+from mfg_package.utils.results import TickResult, DoneResult
 
 
 class TemplateRule(Rule):
 
     def __init__(self, *args, **kwargs):
         super(TemplateRule, self).__init__(*args, **kwargs)
```

### Comparing `Marl-Factory-Grid-0.0.6/modules/batteries/actions.py` & `Marl-Factory-Grid-0.0.7/mfg_package/modules/batteries/actions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Union
 
-from environment.actions import Action
-from environment.utils.results import ActionResult
+from mfg_package.environment.actions import Action
+from mfg_package.utils.results import ActionResult
 
-from modules.batteries import constants as b, rewards as r
-from environment import constants as c
+from mfg_package.modules.batteries import constants as b, rewards as r
+from mfg_package.environment import constants as c
 
 
 class BtryCharge(Action):
 
     def __init__(self):
         super().__init__(b.CHARGE)
```

### Comparing `Marl-Factory-Grid-0.0.6/modules/batteries/constants.py` & `Marl-Factory-Grid-0.0.7/mfg_package/modules/batteries/constants.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.6/modules/batteries/entitites.py` & `Marl-Factory-Grid-0.0.7/mfg_package/modules/batteries/entitites.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from environment.entity.mixin import BoundEntityMixin
-from environment.entity.object import EnvObject
-from environment.entity.entity import Entity
-from environment import constants as c
-from environment.utils.render import RenderEntity
+from mfg_package.environment.entity.mixin import BoundEntityMixin
+from mfg_package.environment.entity.object import EnvObject
+from mfg_package.environment.entity.entity import Entity
+from mfg_package.environment import constants as c
+from mfg_package.utils.render import RenderEntity
 
-from modules.batteries import constants as b
+from mfg_package.modules.batteries import constants as b
 
 
 class Battery(BoundEntityMixin, EnvObject):
 
     @property
     def is_discharged(self):
         return self.charge_level == 0
```

### Comparing `Marl-Factory-Grid-0.0.6/modules/batteries/rules.py` & `Marl-Factory-Grid-0.0.7/mfg_package/modules/batteries/rules.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List, Union
-from environment.rules import Rule
-from environment.utils.results import TickResult, DoneResult
+from mfg_package.environment.rules import Rule
+from mfg_package.utils.results import TickResult, DoneResult
 
-from environment import constants as c
-from modules.batteries import constants as b, rewards as r
+from mfg_package.environment import constants as c
+from mfg_package.modules.batteries import constants as b, rewards as r
 
 
 class Btry(Rule):
 
     def __init__(self, initial_charge: float = 0.8, per_action_costs: Union[dict, float] = 0.02):
         super().__init__()
         self.per_action_costs = per_action_costs
```

### Comparing `Marl-Factory-Grid-0.0.6/modules/clean_up/actions.py` & `Marl-Factory-Grid-0.0.7/mfg_package/modules/clean_up/actions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Union
 
-from environment.actions import Action
-from environment.utils.results import ActionResult
+from mfg_package.environment.actions import Action
+from mfg_package.utils.results import ActionResult
 
-from modules.clean_up import constants as d, rewards as r
+from mfg_package.modules.clean_up import constants as d, rewards as r
 
-from environment import constants as c
+from mfg_package.environment import constants as c
 
 
 class CleanUp(Action):
 
     def __init__(self):
         super().__init__(d.CLEAN_UP)
```

### Comparing `Marl-Factory-Grid-0.0.6/modules/clean_up/dirtpiles.png` & `Marl-Factory-Grid-0.0.7/mfg_package/modules/clean_up/dirtpiles.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.6/modules/clean_up/entitites.py` & `Marl-Factory-Grid-0.0.7/mfg_package/modules/clean_up/entitites.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from numpy import random
 
-from environment.entity.entity import Entity
-from environment.utils.render import RenderEntity
-from modules.clean_up import constants as d
+from mfg_package.environment.entity.entity import Entity
+from mfg_package.utils.render import RenderEntity
+from mfg_package.modules.clean_up import constants as d
 
 
 class DirtPile(Entity):
 
     @property
     def amount(self):
         return self._amount
```

### Comparing `Marl-Factory-Grid-0.0.6/modules/clean_up/groups.py` & `Marl-Factory-Grid-0.0.7/mfg_package/modules/clean_up/groups.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from environment.groups.env_objects import EnvObjects
-from environment.groups.mixins import PositionMixin
-from environment.entity.wall_floor import Floor
-from modules.clean_up.entitites import DirtPile
+from mfg_package.environment.groups.env_objects import EnvObjects
+from mfg_package.environment.groups.mixins import PositionMixin
+from mfg_package.environment.entity.wall_floor import Floor
+from mfg_package.modules.clean_up.entitites import DirtPile
 
-from environment import constants as c
+from mfg_package.environment import constants as c
 
 
 class DirtPiles(PositionMixin, EnvObjects):
 
     _entity = DirtPile
     is_blocking_light: bool = False
     can_collide: bool = False
```

### Comparing `Marl-Factory-Grid-0.0.6/modules/clean_up/rule_done_on_all_clean.py` & `Marl-Factory-Grid-0.0.7/mfg_package/modules/clean_up/rule_done_on_all_clean.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from environment import constants as c
-from environment.rules import Rule
-from environment.utils.results import DoneResult
-from modules.clean_up import constants as d, rewards as r
+from mfg_package.environment import constants as c
+from mfg_package.environment.rules import Rule
+from mfg_package.utils.results import DoneResult
+from mfg_package.modules.clean_up import constants as d, rewards as r
 
 
 class DirtAllCleanDone(Rule):
 
     def __init__(self):
         super().__init__()
```

### Comparing `Marl-Factory-Grid-0.0.6/modules/destinations/actions.py` & `Marl-Factory-Grid-0.0.7/mfg_package/modules/items/actions.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,37 @@
 from typing import Union
 
-from environment.actions import Action
-from environment.utils.results import ActionResult
+from mfg_package.environment.actions import Action
+from mfg_package.utils.results import ActionResult
 
-from modules.destinations import constants as d, rewards as r
-from environment import constants as c
+from mfg_package.modules.items import constants as i, rewards as r
+from mfg_package.environment import constants as c
 
 
-class DestAction(Action):
+class ItemAction(Action):
 
     def __init__(self):
-        super().__init__(d.DESTINATION)
+        super().__init__(i.ITEM_ACTION)
 
     def do(self, entity, state) -> Union[None, ActionResult]:
-        if destination := state[d.DESTINATION].by_pos(entity.pos):
-            valid = destination.do_wait_action(entity)
-            state.print(f'{entity.name} just waited at {entity.pos}')
+        inventory = state[i.INVENTORY].by_entity(entity)
+        if drop_off := state[i.DROP_OFF].by_pos(entity.pos):
+            if inventory:
+                valid = drop_off.place_item(inventory.pop())
+            else:
+                valid = c.NOT_VALID
+            if valid:
+                state.print(f'{entity.name} just dropped of an item at {drop_off.pos}.')
+            else:
+                state.print(f'{entity.name} just tried to drop off at {entity.pos}, but failed.')
+            reward = r.DROP_OFF_VALID if valid else r.DROP_OFF_FAIL
+            return ActionResult(entity=entity, identifier=self._identifier, validity=valid, reward=reward)
+
+        elif item := state[i.ITEM].by_pos(entity.pos):
+            item.change_parent_collection(inventory)
+            item.set_tile_to(state.NO_POS_TILE)
+            state.print(f'{entity.name} just picked up an item at {entity.pos}')
+            return ActionResult(entity=entity, identifier=self._identifier, validity=c.VALID, reward=r.PICK_UP_VALID)
+
         else:
-            valid = c.NOT_VALID
-            state.print(f'{entity.name} just tried to do_wait_action do_wait_action at {entity.pos} but failed')
-        return ActionResult(entity=entity, identifier=self._identifier, validity=valid,
-                            reward=r.WAIT_VALID if valid else r.WAIT_FAIL)
+            state.print(f'{entity.name} just tried to pick up an item at {entity.pos}, but failed.')
+            return ActionResult(entity=entity, identifier=self._identifier, validity=c.NOT_VALID, reward=r.PICK_UP_FAIL)
```

### Comparing `Marl-Factory-Grid-0.0.6/modules/destinations/destinations.png` & `Marl-Factory-Grid-0.0.7/mfg_package/modules/destinations/destinations.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.6/modules/destinations/entitites.py` & `Marl-Factory-Grid-0.0.7/mfg_package/modules/destinations/entitites.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from collections import defaultdict
 
-from environment.entity.agent import Agent
-from environment.entity.entity import Entity
-from environment import constants as c
-from environment.utils.render import RenderEntity
-from modules.destinations import constants as d
+from mfg_package.environment.entity.agent import Agent
+from mfg_package.environment.entity.entity import Entity
+from mfg_package.environment import constants as c
+from mfg_package.utils.render import RenderEntity
+from mfg_package.modules.destinations import constants as d
 
 
 class Destination(Entity):
 
     @property
     def any_agent_has_dwelled(self):
         return bool(len(self._per_agent_times))
```

### Comparing `Marl-Factory-Grid-0.0.6/modules/destinations/rules.py` & `Marl-Factory-Grid-0.0.7/mfg_package/modules/destinations/rules.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import List, Union
-from environment.rules import Rule
-from environment.utils.results import TickResult, DoneResult
-from environment import constants as c
+from mfg_package.environment.rules import Rule
+from mfg_package.utils.results import TickResult, DoneResult
+from mfg_package.environment import constants as c
 
-from modules.destinations import constants as d, rewards as r
-from modules.destinations.entitites import Destination
+from mfg_package.modules.destinations import constants as d, rewards as r
+from mfg_package.modules.destinations.entitites import Destination
 
 
 class DestinationReach(Rule):
 
     def __init__(self, n_dests: int = 1, tiles: Union[List, None] = None):
         super(DestinationReach, self).__init__()
         self.n_dests = n_dests or len(tiles)
```

### Comparing `Marl-Factory-Grid-0.0.6/modules/doors/actions.py` & `Marl-Factory-Grid-0.0.7/mfg_package/modules/doors/actions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Union
 
-from environment.actions import Action
-from environment.utils.results import ActionResult
+from mfg_package.environment.actions import Action
+from mfg_package.utils.results import ActionResult
 
-from modules.doors import constants as d, rewards as r
-from environment import constants as c
+from mfg_package.modules.doors import constants as d, rewards as r
+from mfg_package.environment import constants as c
 
 
 class DoorUse(Action):
 
     def __init__(self):
         super().__init__(d.ACTION_DOOR_USE)
```

### Comparing `Marl-Factory-Grid-0.0.6/modules/doors/constants.py` & `Marl-Factory-Grid-0.0.7/mfg_package/modules/doors/constants.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.6/modules/doors/door_closed.png` & `Marl-Factory-Grid-0.0.7/mfg_package/modules/doors/door_closed.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.6/modules/doors/door_open.png` & `Marl-Factory-Grid-0.0.7/mfg_package/modules/doors/door_open.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.6/modules/doors/entitites.py` & `Marl-Factory-Grid-0.0.7/mfg_package/modules/doors/entitites.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from environment.entity.entity import Entity
-from environment.utils.render import RenderEntity
-from environment import constants as c
+from mfg_package.environment.entity.entity import Entity
+from mfg_package.utils.render import RenderEntity
+from mfg_package.environment import constants as c
 
-from modules.doors import constants as d
+from mfg_package.modules.doors import constants as d
 
 
 class DoorIndicator(Entity):
 
     @property
     def encoding(self):
         return d.VALUE_ACCESS_INDICATOR
```

### Comparing `Marl-Factory-Grid-0.0.6/modules/doors/groups.py` & `Marl-Factory-Grid-0.0.7/mfg_package/modules/doors/groups.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Union
 
-from environment.groups.env_objects import EnvObjects
-from environment.groups.mixins import PositionMixin
-from modules.doors import constants as d
-from modules.doors.entitites import Door
+from mfg_package.environment.groups.env_objects import EnvObjects
+from mfg_package.environment.groups.mixins import PositionMixin
+from mfg_package.modules.doors import constants as d
+from mfg_package.modules.doors.entitites import Door
 
 
 class Doors(PositionMixin, EnvObjects):
 
     symbol = d.SYMBOL_DOOR
     _entity = Door
```

### Comparing `Marl-Factory-Grid-0.0.6/modules/items/assets/charge_pod.png` & `Marl-Factory-Grid-0.0.7/mfg_package/modules/items/assets/charge_pod.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.6/modules/items/assets/dropofflocations.png` & `Marl-Factory-Grid-0.0.7/mfg_package/modules/items/assets/dropofflocations.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.6/modules/items/assets/items.png` & `Marl-Factory-Grid-0.0.7/mfg_package/modules/items/assets/items.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.6/modules/items/entitites.py` & `Marl-Factory-Grid-0.0.7/mfg_package/modules/items/entitites.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from collections import deque
 
-from environment.entity.entity import Entity
-from environment import constants as c
-from environment.utils.render import RenderEntity
-from modules.items import constants as i
+from mfg_package.environment.entity.entity import Entity
+from mfg_package.environment import constants as c
+from mfg_package.utils.render import RenderEntity
+from mfg_package.modules.items import constants as i
 
 
 class Item(Entity):
 
     def render(self):
         return RenderEntity(i.ITEM, self.tile.pos) if self.pos != c.VALUE_NO_POS else None
```

### Comparing `Marl-Factory-Grid-0.0.6/modules/items/rules.py` & `Marl-Factory-Grid-0.0.7/mfg_package/modules/items/rules.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import List
 
-from environment.rules import Rule
-from environment import constants as c
-from environment.utils.results import TickResult
-from modules.items import constants as i
-from modules.items.entitites import DropOffLocation
+from mfg_package.environment.rules import Rule
+from mfg_package.environment import constants as c
+from mfg_package.utils.results import TickResult
+from mfg_package.modules.items import constants as i
+from mfg_package.modules.items.entitites import DropOffLocation
 
 
 class ItemRules(Rule):
 
     def __init__(self, n_items: int = 5, spawn_frequency: int = 15,
                  n_locations: int = 5, max_dropoff_storage_size: int = 0):
         super().__init__()
```

### Comparing `Marl-Factory-Grid-0.0.6/modules/machines/entitites.py` & `Marl-Factory-Grid-0.0.7/mfg_package/modules/machines/entitites.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from environment.entity.entity import Entity
-from environment.utils.render import RenderEntity
-from environment import constants as c
-from environment.utils.results import TickResult
-from modules.machines import constants as m, rewards as r
+from mfg_package.environment.entity.entity import Entity
+from mfg_package.utils.render import RenderEntity
+from mfg_package.environment import constants as c
+from mfg_package.utils.results import TickResult
+from mfg_package.modules.machines import constants as m, rewards as r
 
 
 class Machine(Entity):
 
     @property
     def encoding(self):
         return self._encodings[self.state]
```

### Comparing `Marl-Factory-Grid-0.0.6/plotting/compare_runs.py` & `Marl-Factory-Grid-0.0.7/mfg_package/plotting/compare_runs.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import re
 from os import PathLike
 from pathlib import Path
 from typing import Union, List
 
 import pandas as pd
 
-from environment.utils.helpers import IGNORED_DF_COLUMNS
-from plotting.plotting import prepare_plot
+from mfg_package.utils.helpers import IGNORED_DF_COLUMNS
+from mfg_package.plotting.plotting import prepare_plot
 
 MODEL_MAP = None
 
 
 def plot_single_run(run_path: Union[str, PathLike], use_tex: bool = False, column_keys=None):
     run_path = Path(run_path)
     df_list = list()
```

### Comparing `Marl-Factory-Grid-0.0.6/plotting/plotting.py` & `Marl-Factory-Grid-0.0.7/mfg_package/plotting/plotting.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.6/quickstart/all_test_config.yaml` & `Marl-Factory-Grid-0.0.7/quickstart/all_test_config.yaml`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.6/quickstart/default_config.yaml` & `Marl-Factory-Grid-0.0.7/quickstart/default_config.yaml`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.6/setup.py` & `Marl-Factory-Grid-0.0.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(name='Marl-Factory-Grid',
-      version='0.0.6',
+      version='0.0.7',
       description='A framework to research MARL agents in various setings.',
       author='Steffen Illium',
       author_email='steffen.illium@ifi.lmu.de',
       url='https://github.com/illiumst/marl-factory-grid/import',
       license='MIT',
       keywords=[
             'artificial intelligence',
             'pytorch',
             'multiagent reinforcement learning',
             'simulation',
             'emergence',
             'gymnasium',
-            'environment'
+            'environment',
+            'deepdiff',
+            'natsort',
+
       ],
       classifiers=[
             'Development Status :: 4 - Beta',
             'Intended Audience :: Developers',
             'Topic :: Scientific/Engineering :: Artificial Intelligence',
             'License :: OSI Approved :: MIT License',
             'Programming Language :: Python :: 3.11',
```

