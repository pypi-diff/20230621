# Comparing `tmp/Marl-Factory-Grid-0.0.8.tar.gz` & `tmp/Marl-Factory-Grid-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Marl-Factory-Grid-0.0.8.tar", last modified: Wed Jun 21 09:29:12 2023, max compression
+gzip compressed data, was "Marl-Factory-Grid-0.0.9.tar", last modified: Wed Jun 21 09:40:11 2023, max compression
```

## Comparing `Marl-Factory-Grid-0.0.8.tar` & `Marl-Factory-Grid-0.0.9.tar`

### file list

```diff
@@ -1,169 +1,167 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.097490 Marl-Factory-Grid-0.0.8/
--rw-rw-rw-   0 root         (0) root         (0)      453 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)       45 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/MANIFEST.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.085491 Marl-Factory-Grid-0.0.8/Marl_Factory_Grid.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4376 2023-06-21 09:29:12.000000 Marl-Factory-Grid-0.0.8/Marl_Factory_Grid.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6265 2023-06-21 09:29:12.000000 Marl-Factory-Grid-0.0.8/Marl_Factory_Grid.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 09:29:12.000000 Marl-Factory-Grid-0.0.8/Marl_Factory_Grid.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-21 09:29:12.000000 Marl-Factory-Grid-0.0.8/Marl_Factory_Grid.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-21 09:29:12.000000 Marl-Factory-Grid-0.0.8/Marl_Factory_Grid.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     4376 2023-06-21 09:29:12.097490 Marl-Factory-Grid-0.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3673 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.085491 Marl-Factory-Grid-0.0.8/images/
--rw-rw-rw-   0 root         (0) root         (0)   303396 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/images/Hooks_FIKS.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.089491 Marl-Factory-Grid-0.0.8/marl_factory_grid/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.089491 Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.089491 Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/marl/
--rw-rw-rw-   0 root         (0) root         (0)       74 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/marl/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8710 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/marl/base_ac.py
--rw-rw-rw-   0 root         (0) root         (0)      636 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/marl/example_config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2125 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/marl/iac.py
--rw-rw-rw-   0 root         (0) root         (0)     3208 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/marl/mappo.py
--rw-rw-rw-   0 root         (0) root         (0)     7763 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/marl/memory.py
--rw-rw-rw-   0 root         (0) root         (0)     4784 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/marl/networks.py
--rw-rw-rw-   0 root         (0) root         (0)     2279 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/marl/seac.py
--rw-rw-rw-   0 root         (0) root         (0)     1305 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/marl/snac.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.089491 Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/static/
--rw-rw-rw-   0 root         (0) root         (0)     5337 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/static/TSP_base_agent.py
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/static/TSP_dirt_agent.py
--rw-rw-rw-   0 root         (0) root         (0)     2387 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/static/TSP_item_agent.py
--rw-rw-rw-   0 root         (0) root         (0)     1115 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/static/TSP_target_agent.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/static/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      391 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/static/random_agent.py
--rw-rw-rw-   0 root         (0) root         (0)     2687 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.089491 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2633 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/actions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.089491 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/assets/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/assets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.089491 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/assets/agent/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/assets/agent/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8521 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/assets/agent/adversary.png
--rw-rw-rw-   0 root         (0) root         (0)     3402 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/assets/agent/agent.png
--rw-rw-rw-   0 root         (0) root         (0)    18857 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/assets/agent/agent_collision.png
--rw-rw-rw-   0 root         (0) root         (0)     1631 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/assets/agent/idle.png
--rw-rw-rw-   0 root         (0) root         (0)     1599 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/assets/agent/invalid.png
--rw-rw-rw-   0 root         (0) root         (0)     5933 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/assets/agent/move.png
--rw-rw-rw-   0 root         (0) root         (0)     5717 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/assets/agent/valid.png
--rw-rw-rw-   0 root         (0) root         (0)     1415 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/assets/wall.png
--rw-rw-rw-   0 root         (0) root         (0)     2766 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.089491 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/entity/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/entity/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2380 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/entity/agent.py
--rw-rw-rw-   0 root         (0) root         (0)     2175 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/entity/entity.py
--rw-rw-rw-   0 root         (0) root         (0)      400 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/entity/mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     3320 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/entity/object.py
--rw-rw-rw-   0 root         (0) root         (0)     1240 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/entity/util.py
--rw-rw-rw-   0 root         (0) root         (0)     3123 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/entity/wall_floor.py
--rw-rw-rw-   0 root         (0) root         (0)     6943 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.093490 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/groups/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/groups/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      895 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/groups/agents.py
--rw-rw-rw-   0 root         (0) root         (0)      957 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/groups/env_objects.py
--rw-rw-rw-   0 root         (0) root         (0)     2056 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/groups/global_entities.py
--rw-rw-rw-   0 root         (0) root         (0)     2910 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/groups/mixins.py
--rw-rw-rw-   0 root         (0) root         (0)     3902 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/groups/objects.py
--rw-rw-rw-   0 root         (0) root         (0)     2399 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/groups/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1586 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/groups/wall_n_floors.py
--rw-rw-rw-   0 root         (0) root         (0)      124 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/rewards.py
--rw-rw-rw-   0 root         (0) root         (0)     2537 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/rules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.093490 Marl-Factory-Grid-0.0.8/marl_factory_grid/logging/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/logging/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2244 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/logging/envmonitor.py
--rw-rw-rw-   0 root         (0) root         (0)     5474 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/logging/recorder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.093490 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.093490 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/_template/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/_template/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      319 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/_template/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      595 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/_template/rules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.093490 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/batteries/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/batteries/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1103 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/batteries/actions.py
--rw-rw-rw-   0 root         (0) root         (0)      523 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/batteries/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2426 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/batteries/entitites.py
--rw-rw-rw-   0 root         (0) root         (0)     1073 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/batteries/groups.py
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/batteries/rewards.py
--rw-rw-rw-   0 root         (0) root         (0)     2135 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/batteries/rules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.093490 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/clean_up/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/clean_up/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1319 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/clean_up/actions.py
--rw-rw-rw-   0 root         (0) root         (0)      150 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/clean_up/constants.py
--rw-rw-rw-   0 root         (0) root         (0)    39296 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/clean_up/dirtpiles.png
--rw-rw-rw-   0 root         (0) root         (0)     1180 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/clean_up/entitites.py
--rw-rw-rw-   0 root         (0) root         (0)     2611 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/clean_up/groups.py
--rw-rw-rw-   0 root         (0) root         (0)       82 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/clean_up/rewards.py
--rw-rw-rw-   0 root         (0) root         (0)      611 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/clean_up/rule_done_on_all_clean.py
--rw-rw-rw-   0 root         (0) root         (0)      967 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/clean_up/rule_respawn.py
--rw-rw-rw-   0 root         (0) root         (0)     1072 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/clean_up/rule_smear_on_move.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.093490 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/destinations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/destinations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      948 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/destinations/actions.py
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/destinations/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     7037 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/destinations/destinations.png
--rw-rw-rw-   0 root         (0) root         (0)     1813 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/destinations/entitites.py
--rw-rw-rw-   0 root         (0) root         (0)      834 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/destinations/groups.py
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/destinations/rewards.py
--rw-rw-rw-   0 root         (0) root         (0)     3728 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/destinations/rules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.093490 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/doors/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/doors/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1164 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/doors/actions.py
--rw-rw-rw-   0 root         (0) root         (0)      793 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/doors/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      699 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/doors/door_closed.png
--rw-rw-rw-   0 root         (0) root         (0)     4224 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/doors/door_open.png
--rw-rw-rw-   0 root         (0) root         (0)     2740 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/doors/entitites.py
--rw-rw-rw-   0 root         (0) root         (0)      924 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/doors/groups.py
--rw-rw-rw-   0 root         (0) root         (0)       58 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/doors/rewards.py
--rw-rw-rw-   0 root         (0) root         (0)      900 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/doors/rule_door_auto_close.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.093490 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/items/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/items/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1681 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/items/actions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.093490 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/items/assets/
--rw-rw-rw-   0 root         (0) root         (0)     6610 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/items/assets/charge_pod.png
--rw-rw-rw-   0 root         (0) root         (0)     2318 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/items/assets/dropofflocations.png
--rw-rw-rw-   0 root         (0) root         (0)     3102 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/items/assets/items.png
--rw-rw-rw-   0 root         (0) root         (0)      234 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/items/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2074 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/items/entitites.py
--rw-rw-rw-   0 root         (0) root         (0)     3173 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/items/groups.py
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/items/rewards.py
--rw-rw-rw-   0 root         (0) root         (0)     3153 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/items/rules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.097490 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/levels/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/levels/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1511 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/levels/large.txt
--rw-rw-rw-   0 root         (0) root         (0)     5827 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/levels/large_qquad.txt
--rw-rw-rw-   0 root         (0) root         (0)      207 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/levels/rooms.txt
--rw-rw-rw-   0 root         (0) root         (0)      168 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/levels/shelves.txt
--rw-rw-rw-   0 root         (0) root         (0)      155 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/levels/simple.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.097490 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/machines/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/machines/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      178 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/machines/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1898 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/machines/entitites.py
--rw-rw-rw-   0 root         (0) root         (0)      439 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/machines/groups.py
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/machines/rewards.py
--rw-rw-rw-   0 root         (0) root         (0)      932 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/machines/rules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.097490 Marl-Factory-Grid-0.0.8/marl_factory_grid/plotting/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/plotting/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8652 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/plotting/compare_runs.py
--rw-rw-rw-   0 root         (0) root         (0)     2967 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/plotting/plotting.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.097490 Marl-Factory-Grid-0.0.8/marl_factory_grid/quickstart/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/quickstart/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1381 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/quickstart/default_config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      413 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/quickstart/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.097490 Marl-Factory-Grid-0.0.8/marl_factory_grid/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5309 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/utils/config_parser.py
--rw-rw-rw-   0 root         (0) root         (0)    10888 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/utils/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     2260 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/utils/level_parser.py
--rw-rw-rw-   0 root         (0) root         (0)    12499 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/utils/observation_builder.py
--rw-rw-rw-   0 root         (0) root         (0)      283 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/utils/render.py
--rw-rw-rw-   0 root         (0) root         (0)     5765 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/utils/renderer.py
--rw-rw-rw-   0 root         (0) root         (0)     1114 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/utils/results.py
--rw-rw-rw-   0 root         (0) root         (0)     3625 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/utils/states.py
--rw-rw-rw-   0 root         (0) root         (0)     5673 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/utils/tools.py
--rw-rw-rw-   0 root         (0) root         (0)      811 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/marl_factory_grid/utils/utility_classes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:29:12.097490 Marl-Factory-Grid-0.0.8/quickstart/
--rw-rw-rw-   0 root         (0) root         (0)     2129 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/quickstart/all_test_config.yaml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-21 09:29:12.097490 Marl-Factory-Grid-0.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1415 2023-06-21 09:29:05.000000 Marl-Factory-Grid-0.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.927360 Marl-Factory-Grid-0.0.9/
+-rw-rw-rw-   0 root         (0) root         (0)      453 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)       45 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/MANIFEST.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.919360 Marl-Factory-Grid-0.0.9/Marl_Factory_Grid.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4376 2023-06-21 09:40:11.000000 Marl-Factory-Grid-0.0.9/Marl_Factory_Grid.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6209 2023-06-21 09:40:11.000000 Marl-Factory-Grid-0.0.9/Marl_Factory_Grid.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 09:40:11.000000 Marl-Factory-Grid-0.0.9/Marl_Factory_Grid.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-21 09:40:11.000000 Marl-Factory-Grid-0.0.9/Marl_Factory_Grid.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-21 09:40:11.000000 Marl-Factory-Grid-0.0.9/Marl_Factory_Grid.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     4376 2023-06-21 09:40:11.927360 Marl-Factory-Grid-0.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3673 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.919360 Marl-Factory-Grid-0.0.9/_quickstart/
+-rw-rw-rw-   0 root         (0) root         (0)     2129 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/_quickstart/all_test_config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.919360 Marl-Factory-Grid-0.0.9/images/
+-rw-rw-rw-   0 root         (0) root         (0)   303396 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/images/Hooks_FIKS.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.919360 Marl-Factory-Grid-0.0.9/marl_factory_grid/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.919360 Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.919360 Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/marl/
+-rw-rw-rw-   0 root         (0) root         (0)       74 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/marl/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8710 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/marl/base_ac.py
+-rw-rw-rw-   0 root         (0) root         (0)      636 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/marl/example_config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2125 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/marl/iac.py
+-rw-rw-rw-   0 root         (0) root         (0)     3208 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/marl/mappo.py
+-rw-rw-rw-   0 root         (0) root         (0)     7763 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/marl/memory.py
+-rw-rw-rw-   0 root         (0) root         (0)     4784 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/marl/networks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2279 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/marl/seac.py
+-rw-rw-rw-   0 root         (0) root         (0)     1305 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/marl/snac.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.919360 Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/static/
+-rw-rw-rw-   0 root         (0) root         (0)     5337 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/static/TSP_base_agent.py
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/static/TSP_dirt_agent.py
+-rw-rw-rw-   0 root         (0) root         (0)     2387 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/static/TSP_item_agent.py
+-rw-rw-rw-   0 root         (0) root         (0)     1115 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/static/TSP_target_agent.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/static/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      391 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/static/random_agent.py
+-rw-rw-rw-   0 root         (0) root         (0)     2687 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1381 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/default_config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.919360 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2633 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/actions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.919360 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/assets/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/assets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.919360 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/assets/agent/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/assets/agent/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8521 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/assets/agent/adversary.png
+-rw-rw-rw-   0 root         (0) root         (0)     3402 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/assets/agent/agent.png
+-rw-rw-rw-   0 root         (0) root         (0)    18857 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/assets/agent/agent_collision.png
+-rw-rw-rw-   0 root         (0) root         (0)     1631 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/assets/agent/idle.png
+-rw-rw-rw-   0 root         (0) root         (0)     1599 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/assets/agent/invalid.png
+-rw-rw-rw-   0 root         (0) root         (0)     5933 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/assets/agent/move.png
+-rw-rw-rw-   0 root         (0) root         (0)     5717 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/assets/agent/valid.png
+-rw-rw-rw-   0 root         (0) root         (0)     1415 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/assets/wall.png
+-rw-rw-rw-   0 root         (0) root         (0)     2766 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.923360 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/entity/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/entity/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2380 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/entity/agent.py
+-rw-rw-rw-   0 root         (0) root         (0)     2175 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/entity/entity.py
+-rw-rw-rw-   0 root         (0) root         (0)      400 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/entity/mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     3320 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/entity/object.py
+-rw-rw-rw-   0 root         (0) root         (0)     1240 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/entity/util.py
+-rw-rw-rw-   0 root         (0) root         (0)     3123 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/entity/wall_floor.py
+-rw-rw-rw-   0 root         (0) root         (0)     6943 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.923360 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/groups/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/groups/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      895 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/groups/agents.py
+-rw-rw-rw-   0 root         (0) root         (0)      957 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/groups/env_objects.py
+-rw-rw-rw-   0 root         (0) root         (0)     2056 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/groups/global_entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     2910 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/groups/mixins.py
+-rw-rw-rw-   0 root         (0) root         (0)     3902 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/groups/objects.py
+-rw-rw-rw-   0 root         (0) root         (0)     2399 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/groups/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1586 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/groups/wall_n_floors.py
+-rw-rw-rw-   0 root         (0) root         (0)      124 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/rewards.py
+-rw-rw-rw-   0 root         (0) root         (0)     2537 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/rules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.923360 Marl-Factory-Grid-0.0.9/marl_factory_grid/logging/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/logging/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2244 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/logging/envmonitor.py
+-rw-rw-rw-   0 root         (0) root         (0)     5474 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/logging/recorder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.923360 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.923360 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/_template/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/_template/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      319 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/_template/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      595 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/_template/rules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.923360 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/batteries/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/batteries/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1103 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/batteries/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)      523 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/batteries/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2426 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/batteries/entitites.py
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/batteries/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/batteries/rewards.py
+-rw-rw-rw-   0 root         (0) root         (0)     2135 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/batteries/rules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.923360 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/clean_up/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/clean_up/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1319 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/clean_up/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)      150 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/clean_up/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)    39296 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/clean_up/dirtpiles.png
+-rw-rw-rw-   0 root         (0) root         (0)     1180 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/clean_up/entitites.py
+-rw-rw-rw-   0 root         (0) root         (0)     2611 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/clean_up/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)       82 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/clean_up/rewards.py
+-rw-rw-rw-   0 root         (0) root         (0)      611 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/clean_up/rule_done_on_all_clean.py
+-rw-rw-rw-   0 root         (0) root         (0)      967 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/clean_up/rule_respawn.py
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/clean_up/rule_smear_on_move.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.923360 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/destinations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/destinations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      948 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/destinations/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/destinations/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     7037 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/destinations/destinations.png
+-rw-rw-rw-   0 root         (0) root         (0)     1813 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/destinations/entitites.py
+-rw-rw-rw-   0 root         (0) root         (0)      834 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/destinations/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/destinations/rewards.py
+-rw-rw-rw-   0 root         (0) root         (0)     3728 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/destinations/rules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.923360 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/doors/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/doors/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1164 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/doors/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)      793 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/doors/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      699 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/doors/door_closed.png
+-rw-rw-rw-   0 root         (0) root         (0)     4224 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/doors/door_open.png
+-rw-rw-rw-   0 root         (0) root         (0)     2740 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/doors/entitites.py
+-rw-rw-rw-   0 root         (0) root         (0)      924 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/doors/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/doors/rewards.py
+-rw-rw-rw-   0 root         (0) root         (0)      900 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/doors/rule_door_auto_close.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.927360 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/items/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/items/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1681 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/items/actions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.927360 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/items/assets/
+-rw-rw-rw-   0 root         (0) root         (0)     6610 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/items/assets/charge_pod.png
+-rw-rw-rw-   0 root         (0) root         (0)     2318 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/items/assets/dropofflocations.png
+-rw-rw-rw-   0 root         (0) root         (0)     3102 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/items/assets/items.png
+-rw-rw-rw-   0 root         (0) root         (0)      234 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/items/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2074 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/items/entitites.py
+-rw-rw-rw-   0 root         (0) root         (0)     3173 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/items/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/items/rewards.py
+-rw-rw-rw-   0 root         (0) root         (0)     3153 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/items/rules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.927360 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/levels/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/levels/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1511 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/levels/large.txt
+-rw-rw-rw-   0 root         (0) root         (0)     5827 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/levels/large_qquad.txt
+-rw-rw-rw-   0 root         (0) root         (0)      207 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/levels/rooms.txt
+-rw-rw-rw-   0 root         (0) root         (0)      168 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/levels/shelves.txt
+-rw-rw-rw-   0 root         (0) root         (0)      155 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/levels/simple.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.927360 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/machines/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/machines/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      178 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/machines/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1898 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/machines/entitites.py
+-rw-rw-rw-   0 root         (0) root         (0)      439 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/machines/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/machines/rewards.py
+-rw-rw-rw-   0 root         (0) root         (0)      932 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/machines/rules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.927360 Marl-Factory-Grid-0.0.9/marl_factory_grid/plotting/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/plotting/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8652 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/plotting/compare_runs.py
+-rw-rw-rw-   0 root         (0) root         (0)     2967 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/plotting/plotting.py
+-rw-rw-rw-   0 root         (0) root         (0)      634 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/quickstart.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:40:11.927360 Marl-Factory-Grid-0.0.9/marl_factory_grid/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5309 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/utils/config_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)    10888 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/utils/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2260 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/utils/level_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)    12499 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/utils/observation_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)      283 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/utils/render.py
+-rw-rw-rw-   0 root         (0) root         (0)     5765 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/utils/renderer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1114 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/utils/results.py
+-rw-rw-rw-   0 root         (0) root         (0)     3625 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/utils/states.py
+-rw-rw-rw-   0 root         (0) root         (0)     5673 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/utils/tools.py
+-rw-rw-rw-   0 root         (0) root         (0)      811 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/marl_factory_grid/utils/utility_classes.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-21 09:40:11.927360 Marl-Factory-Grid-0.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1415 2023-06-21 09:40:05.000000 Marl-Factory-Grid-0.0.9/setup.py
```

### Comparing `Marl-Factory-Grid-0.0.8/Marl_Factory_Grid.egg-info/PKG-INFO` & `Marl-Factory-Grid-0.0.9/Marl_Factory_Grid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Marl-Factory-Grid
-Version: 0.0.8
+Version: 0.0.9
 Summary: A framework to research MARL agents in various setings.
 Home-page: https://github.com/illiumst/marl-factory-grid/import
 Author: Steffen Illium
 Author-email: steffen.illium@ifi.lmu.de
 License: MIT
 Keywords: artificial intelligence,pytorch,multiagent reinforcement learning,simulation,emergence,gymnasium,environment,deepdiff,natsort
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Marl-Factory-Grid-0.0.8/Marl_Factory_Grid.egg-info/SOURCES.txt` & `Marl-Factory-Grid-0.0.9/Marl_Factory_Grid.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,19 @@
 README.md
 setup.py
 Marl_Factory_Grid.egg-info/PKG-INFO
 Marl_Factory_Grid.egg-info/SOURCES.txt
 Marl_Factory_Grid.egg-info/dependency_links.txt
 Marl_Factory_Grid.egg-info/requires.txt
 Marl_Factory_Grid.egg-info/top_level.txt
+_quickstart/all_test_config.yaml
 images/Hooks_FIKS.png
 marl_factory_grid/__init__.py
+marl_factory_grid/default_config.yaml
+marl_factory_grid/quickstart.py
 marl_factory_grid/algorithms/__init__.py
 marl_factory_grid/algorithms/utils.py
 marl_factory_grid/algorithms/marl/__init__.py
 marl_factory_grid/algorithms/marl/base_ac.py
 marl_factory_grid/algorithms/marl/example_config.yaml
 marl_factory_grid/algorithms/marl/iac.py
 marl_factory_grid/algorithms/marl/mappo.py
@@ -119,22 +122,18 @@
 marl_factory_grid/modules/machines/entitites.py
 marl_factory_grid/modules/machines/groups.py
 marl_factory_grid/modules/machines/rewards.py
 marl_factory_grid/modules/machines/rules.py
 marl_factory_grid/plotting/__init__.py
 marl_factory_grid/plotting/compare_runs.py
 marl_factory_grid/plotting/plotting.py
-marl_factory_grid/quickstart/__init__.py
-marl_factory_grid/quickstart/default_config.yaml
-marl_factory_grid/quickstart/init.py
 marl_factory_grid/utils/__init__.py
 marl_factory_grid/utils/config_parser.py
 marl_factory_grid/utils/helpers.py
 marl_factory_grid/utils/level_parser.py
 marl_factory_grid/utils/observation_builder.py
 marl_factory_grid/utils/render.py
 marl_factory_grid/utils/renderer.py
 marl_factory_grid/utils/results.py
 marl_factory_grid/utils/states.py
 marl_factory_grid/utils/tools.py
-marl_factory_grid/utils/utility_classes.py
-quickstart/all_test_config.yaml
+marl_factory_grid/utils/utility_classes.py
```

### Comparing `Marl-Factory-Grid-0.0.8/PKG-INFO` & `Marl-Factory-Grid-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Marl-Factory-Grid
-Version: 0.0.8
+Version: 0.0.9
 Summary: A framework to research MARL agents in various setings.
 Home-page: https://github.com/illiumst/marl-factory-grid/import
 Author: Steffen Illium
 Author-email: steffen.illium@ifi.lmu.de
 License: MIT
 Keywords: artificial intelligence,pytorch,multiagent reinforcement learning,simulation,emergence,gymnasium,environment,deepdiff,natsort
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Marl-Factory-Grid-0.0.8/README.md` & `Marl-Factory-Grid-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/images/Hooks_FIKS.png` & `Marl-Factory-Grid-0.0.9/images/Hooks_FIKS.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/marl/base_ac.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/marl/base_ac.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/marl/example_config.yaml` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/marl/example_config.yaml`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/marl/iac.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/marl/iac.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/marl/mappo.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/marl/mappo.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/marl/memory.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/marl/memory.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/marl/networks.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/marl/networks.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/marl/seac.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/marl/seac.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/marl/snac.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/marl/snac.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/static/TSP_base_agent.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/static/TSP_base_agent.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/static/TSP_dirt_agent.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/static/TSP_dirt_agent.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/static/TSP_item_agent.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/static/TSP_item_agent.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/static/TSP_target_agent.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/static/TSP_target_agent.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/algorithms/utils.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/algorithms/utils.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/actions.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/actions.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/assets/agent/adversary.png` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/assets/agent/adversary.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/assets/agent/agent.png` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/assets/agent/agent.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/assets/agent/agent_collision.png` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/assets/agent/agent_collision.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/assets/agent/idle.png` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/assets/agent/idle.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/assets/agent/invalid.png` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/assets/agent/invalid.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/assets/agent/move.png` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/assets/agent/move.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/assets/agent/valid.png` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/assets/agent/valid.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/assets/wall.png` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/assets/wall.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/constants.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/constants.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/entity/agent.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/entity/agent.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/entity/entity.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/entity/entity.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/entity/object.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/entity/object.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/entity/util.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/entity/util.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/entity/wall_floor.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/entity/wall_floor.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/factory.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/factory.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/groups/agents.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/groups/agents.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/groups/env_objects.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/groups/env_objects.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/groups/global_entities.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/groups/global_entities.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/groups/mixins.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/groups/mixins.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/groups/objects.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/groups/objects.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/groups/utils.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/groups/utils.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/groups/wall_n_floors.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/groups/wall_n_floors.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/environment/rules.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/environment/rules.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/logging/envmonitor.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/logging/envmonitor.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/logging/recorder.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/logging/recorder.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/_template/rules.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/_template/rules.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/batteries/actions.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/batteries/actions.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/batteries/constants.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/batteries/constants.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/batteries/entitites.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/batteries/entitites.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/batteries/groups.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/batteries/groups.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/batteries/rules.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/batteries/rules.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/clean_up/actions.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/clean_up/actions.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/clean_up/dirtpiles.png` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/clean_up/dirtpiles.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/clean_up/entitites.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/clean_up/entitites.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/clean_up/groups.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/clean_up/groups.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/clean_up/rule_done_on_all_clean.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/clean_up/rule_done_on_all_clean.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/clean_up/rule_respawn.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/clean_up/rule_respawn.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/clean_up/rule_smear_on_move.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/clean_up/rule_smear_on_move.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/destinations/actions.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/destinations/actions.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/destinations/destinations.png` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/destinations/destinations.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/destinations/entitites.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/destinations/entitites.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/destinations/groups.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/destinations/groups.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/destinations/rules.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/destinations/rules.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/doors/actions.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/doors/actions.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/doors/constants.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/doors/constants.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/doors/door_closed.png` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/doors/door_closed.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/doors/door_open.png` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/doors/door_open.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/doors/entitites.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/doors/entitites.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/doors/groups.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/doors/groups.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/doors/rule_door_auto_close.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/doors/rule_door_auto_close.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/items/actions.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/items/actions.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/items/assets/charge_pod.png` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/items/assets/charge_pod.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/items/assets/dropofflocations.png` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/items/assets/dropofflocations.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/items/assets/items.png` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/items/assets/items.png`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/items/entitites.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/items/entitites.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/items/groups.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/items/groups.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/items/rules.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/items/rules.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/machines/entitites.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/machines/entitites.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/modules/machines/rules.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/modules/machines/rules.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/plotting/compare_runs.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/plotting/compare_runs.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/plotting/plotting.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/plotting/plotting.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/quickstart/default_config.yaml` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/default_config.yaml`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/utils/config_parser.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/utils/config_parser.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/utils/helpers.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/utils/level_parser.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/utils/level_parser.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/utils/observation_builder.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/utils/observation_builder.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/utils/renderer.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/utils/renderer.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/utils/results.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/utils/results.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/utils/states.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/utils/states.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/utils/tools.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/utils/tools.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/marl_factory_grid/utils/utility_classes.py` & `Marl-Factory-Grid-0.0.9/marl_factory_grid/utils/utility_classes.py`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/quickstart/all_test_config.yaml` & `Marl-Factory-Grid-0.0.9/_quickstart/all_test_config.yaml`

 * *Files identical despite different names*

### Comparing `Marl-Factory-Grid-0.0.8/setup.py` & `Marl-Factory-Grid-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(name='Marl-Factory-Grid',
-      version='0.0.8',
+      version='0.0.9',
       description='A framework to research MARL agents in various setings.',
       author='Steffen Illium',
       author_email='steffen.illium@ifi.lmu.de',
       url='https://github.com/illiumst/marl-factory-grid/import',
       license='MIT',
       keywords=[
             'artificial intelligence',
```

