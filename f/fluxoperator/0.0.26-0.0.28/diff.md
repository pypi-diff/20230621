# Comparing `tmp/fluxoperator-0.0.26.tar.gz` & `tmp/fluxoperator-0.0.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluxoperator-0.0.26.tar", last modified: Mon Jun  5 22:27:40 2023, max compression
+gzip compressed data, was "fluxoperator-0.0.28.tar", last modified: Wed Jun 21 05:22:20 2023, max compression
```

## Comparing `fluxoperator-0.0.26.tar` & `fluxoperator-0.0.28.tar`

### file list

```diff
@@ -1,69 +1,71 @@
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-05 22:27:40.706054 fluxoperator-0.0.26/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2694 2023-06-05 22:27:40.706054 fluxoperator-0.0.26/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      391 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/README.md
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-05 22:27:40.694054 fluxoperator-0.0.26/fluxoperator/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1957 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/fluxoperator/__init__.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-05 22:27:40.698054 fluxoperator-0.0.26/fluxoperator/api/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       87 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/fluxoperator/api/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    27361 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/fluxoperator/api_client.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    13596 2023-06-02 23:35:12.000000 fluxoperator-0.0.26/fluxoperator/client.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    16066 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/fluxoperator/configuration.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      756 2023-04-07 19:58:49.000000 fluxoperator-0.0.26/fluxoperator/decorator.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       75 2023-04-07 19:58:49.000000 fluxoperator-0.0.26/fluxoperator/defaults.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5061 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/fluxoperator/exceptions.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-05 22:27:40.698054 fluxoperator-0.0.26/fluxoperator/models/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1481 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/fluxoperator/models/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8452 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/fluxoperator/models/commands.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4338 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/fluxoperator/models/container_resources.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4322 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/fluxoperator/models/container_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6774 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/fluxoperator/models/flux_restful.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8265 2023-06-05 22:23:54.000000 fluxoperator-0.0.26/fluxoperator/models/flux_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4119 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/fluxoperator/models/flux_user.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4402 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/fluxoperator/models/life_cycle.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6622 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/fluxoperator/models/logging_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7375 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/fluxoperator/models/mini_cluster.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3612 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/fluxoperator/models/mini_cluster_archive.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    23480 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/fluxoperator/models/mini_cluster_container.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6217 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/fluxoperator/models/mini_cluster_existing_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6969 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/fluxoperator/models/mini_cluster_list.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    16292 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/fluxoperator/models/mini_cluster_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7727 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/fluxoperator/models/mini_cluster_status.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4434 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/fluxoperator/models/mini_cluster_user.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    13029 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/fluxoperator/models/mini_cluster_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7124 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/fluxoperator/models/pod_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3683 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/fluxoperator/models/security_context.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-05 22:27:40.698054 fluxoperator-0.0.26/fluxoperator/resource/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2023-04-07 19:58:49.000000 fluxoperator-0.0.26/fluxoperator/resource/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1910 2023-04-07 19:58:49.000000 fluxoperator-0.0.26/fluxoperator/resource/network.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5913 2023-05-10 21:19:30.000000 fluxoperator-0.0.26/fluxoperator/resource/pods.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    12590 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/fluxoperator/rest.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-05 22:27:40.698054 fluxoperator-0.0.26/fluxoperator.egg-info/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2694 2023-06-05 22:27:40.000000 fluxoperator-0.0.26/fluxoperator.egg-info/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1923 2023-06-05 22:27:40.000000 fluxoperator-0.0.26/fluxoperator.egg-info/SOURCES.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-06-05 22:27:40.000000 fluxoperator-0.0.26/fluxoperator.egg-info/dependency_links.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-02-25 05:06:19.000000 fluxoperator-0.0.26/fluxoperator.egg-info/not-zip-safe
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       20 2023-06-05 22:27:40.000000 fluxoperator-0.0.26/fluxoperator.egg-info/requires.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       18 2023-06-05 22:27:40.000000 fluxoperator-0.0.26/fluxoperator.egg-info/top_level.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       69 2023-06-05 22:27:40.706054 fluxoperator-0.0.26/setup.cfg
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2153 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/setup.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-05 22:27:40.706054 fluxoperator-0.0.26/test/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2023-06-05 22:00:46.000000 fluxoperator-0.0.26/test/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1224 2023-04-07 19:58:49.000000 fluxoperator-0.0.26/test/test_commands.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1351 2023-04-07 19:58:49.000000 fluxoperator-0.0.26/test/test_container_resources.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1335 2023-04-07 19:58:49.000000 fluxoperator-0.0.26/test/test_container_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1271 2023-04-07 19:58:49.000000 fluxoperator-0.0.26/test/test_flux_restful.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1307 2023-05-10 21:19:30.000000 fluxoperator-0.0.26/test/test_flux_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1212 2023-04-07 19:58:49.000000 fluxoperator-0.0.26/test/test_flux_user.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1226 2023-04-07 19:58:49.000000 fluxoperator-0.0.26/test/test_life_cycle.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1277 2023-04-07 19:58:49.000000 fluxoperator-0.0.26/test/test_logging_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8175 2023-06-02 23:35:12.000000 fluxoperator-0.0.26/test/test_mini_cluster.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1370 2023-06-02 23:35:12.000000 fluxoperator-0.0.26/test/test_mini_cluster_archive.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3559 2023-05-10 23:12:41.000000 fluxoperator-0.0.26/test/test_mini_cluster_container.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1578 2023-06-02 23:35:12.000000 fluxoperator-0.0.26/test/test_mini_cluster_existing_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    17767 2023-06-02 23:35:12.000000 fluxoperator-0.0.26/test/test_mini_cluster_list.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    12352 2023-05-10 23:12:41.000000 fluxoperator-0.0.26/test/test_mini_cluster_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1539 2023-06-02 23:35:12.000000 fluxoperator-0.0.26/test/test_mini_cluster_status.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1396 2023-06-02 23:35:12.000000 fluxoperator-0.0.26/test/test_mini_cluster_user.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1990 2023-06-02 23:35:12.000000 fluxoperator-0.0.26/test/test_mini_cluster_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1284 2023-04-07 19:58:49.000000 fluxoperator-0.0.26/test/test_pod_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1289 2023-04-07 19:58:49.000000 fluxoperator-0.0.26/test/test_security_context.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-21 05:22:20.689673 fluxoperator-0.0.28/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2719 2023-06-21 05:22:20.689673 fluxoperator-0.0.28/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      391 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/README.md
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-21 05:22:20.681672 fluxoperator-0.0.28/fluxoperator/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2005 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/__init__.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-21 05:22:20.685672 fluxoperator-0.0.28/fluxoperator/api/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       87 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/api/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    27361 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/api_client.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    13616 2023-06-21 05:22:14.000000 fluxoperator-0.0.28/fluxoperator/client.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    16066 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/configuration.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      756 2023-04-07 19:58:49.000000 fluxoperator-0.0.28/fluxoperator/decorator.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       75 2023-04-07 19:58:49.000000 fluxoperator-0.0.28/fluxoperator/defaults.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5061 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/exceptions.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-21 05:22:20.685672 fluxoperator-0.0.28/fluxoperator/models/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1529 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/models/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8452 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/models/commands.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4338 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/models/container_resources.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4322 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/models/container_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6774 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/models/flux_restful.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8265 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/models/flux_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4119 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/models/flux_user.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4402 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/models/life_cycle.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6622 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/models/logging_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7375 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/models/mini_cluster.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3612 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/models/mini_cluster_archive.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    23480 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/models/mini_cluster_container.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8150 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/models/mini_cluster_existing_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6969 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/models/mini_cluster_list.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    16961 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/models/mini_cluster_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7727 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/models/mini_cluster_status.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4434 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/models/mini_cluster_user.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    13029 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/models/mini_cluster_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3714 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/models/network.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7124 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/models/pod_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3683 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/models/security_context.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-21 05:22:20.685672 fluxoperator-0.0.28/fluxoperator/resource/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2023-04-07 19:58:49.000000 fluxoperator-0.0.28/fluxoperator/resource/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1910 2023-04-07 19:58:49.000000 fluxoperator-0.0.28/fluxoperator/resource/network.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6151 2023-06-21 05:22:14.000000 fluxoperator-0.0.28/fluxoperator/resource/pods.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    12590 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/fluxoperator/rest.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-21 05:22:20.685672 fluxoperator-0.0.28/fluxoperator.egg-info/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2719 2023-06-21 05:22:20.000000 fluxoperator-0.0.28/fluxoperator.egg-info/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1975 2023-06-21 05:22:20.000000 fluxoperator-0.0.28/fluxoperator.egg-info/SOURCES.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-06-21 05:22:20.000000 fluxoperator-0.0.28/fluxoperator.egg-info/dependency_links.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-02-25 05:06:19.000000 fluxoperator-0.0.28/fluxoperator.egg-info/not-zip-safe
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       20 2023-06-21 05:22:20.000000 fluxoperator-0.0.28/fluxoperator.egg-info/requires.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       18 2023-06-21 05:22:20.000000 fluxoperator-0.0.28/fluxoperator.egg-info/top_level.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       69 2023-06-21 05:22:20.689673 fluxoperator-0.0.28/setup.cfg
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2153 2023-06-21 05:22:14.000000 fluxoperator-0.0.28/setup.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-21 05:22:20.689673 fluxoperator-0.0.28/test/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2023-06-21 04:57:23.000000 fluxoperator-0.0.28/test/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1224 2023-04-07 19:58:49.000000 fluxoperator-0.0.28/test/test_commands.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1351 2023-04-07 19:58:49.000000 fluxoperator-0.0.28/test/test_container_resources.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1335 2023-04-07 19:58:49.000000 fluxoperator-0.0.28/test/test_container_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1271 2023-04-07 19:58:49.000000 fluxoperator-0.0.28/test/test_flux_restful.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1307 2023-06-14 19:07:03.000000 fluxoperator-0.0.28/test/test_flux_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1212 2023-04-07 19:58:49.000000 fluxoperator-0.0.28/test/test_flux_user.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1226 2023-04-07 19:58:49.000000 fluxoperator-0.0.28/test/test_life_cycle.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1277 2023-04-07 19:58:49.000000 fluxoperator-0.0.28/test/test_logging_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8175 2023-06-14 19:07:03.000000 fluxoperator-0.0.28/test/test_mini_cluster.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1370 2023-06-14 19:07:03.000000 fluxoperator-0.0.28/test/test_mini_cluster_archive.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3559 2023-06-14 19:07:03.000000 fluxoperator-0.0.28/test/test_mini_cluster_container.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1578 2023-06-14 19:07:03.000000 fluxoperator-0.0.28/test/test_mini_cluster_existing_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    17767 2023-06-14 19:07:03.000000 fluxoperator-0.0.28/test/test_mini_cluster_list.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    12352 2023-06-14 19:07:03.000000 fluxoperator-0.0.28/test/test_mini_cluster_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1539 2023-06-14 19:07:03.000000 fluxoperator-0.0.28/test/test_mini_cluster_status.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1396 2023-06-14 19:07:03.000000 fluxoperator-0.0.28/test/test_mini_cluster_user.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1990 2023-06-14 19:07:03.000000 fluxoperator-0.0.28/test/test_mini_cluster_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1266 2023-06-14 19:07:03.000000 fluxoperator-0.0.28/test/test_network.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1284 2023-04-07 19:58:49.000000 fluxoperator-0.0.28/test/test_pod_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1289 2023-04-07 19:58:49.000000 fluxoperator-0.0.28/test/test_security_context.py
```

### Comparing `fluxoperator-0.0.26/PKG-INFO` & `fluxoperator-0.0.28/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluxoperator
-Version: 0.0.26
+Version: 0.0.28
 Summary: Python SDK for the Flux Operator
 Home-page: https://github.com/flux-framework/flux-operator/tree/main/python-sdk/v1alpha1
 Author: Vanessasaurus
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessasaurus
 License: Apache 2.0
 Keywords: flux-operator,flux-framework,kubernetes,workflows,jobs-api
@@ -91,14 +91,15 @@
  - [MiniClusterContainer](MiniClusterContainer.md)
  - [MiniClusterList](MiniClusterList.md)
  - [MiniClusterSpec](MiniClusterSpec.md)
  - [MiniClusterStatus](MiniClusterStatus.md)
  - [MiniClusterUser](MiniClusterUser.md)
  - [MiniClusterExistingVolume](MiniClusterExistingVolume.md)
  - [MiniClusterVolume](MiniClusterVolume.md)
+ - [Network](Network.md)
  - [PodSpec](PodSpec.md)
  - [SecurityContext](SecurityContext.md)
 
 ## Documentation For Authorization
 
  All endpoints do not require authorization (but they do require you have permission via your kubernetes config)
```

### Comparing `fluxoperator-0.0.26/fluxoperator/__init__.py` & `fluxoperator-0.0.28/fluxoperator/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,10 +41,11 @@
 from fluxoperator.models.mini_cluster_container import MiniClusterContainer
 from fluxoperator.models.mini_cluster_existing_volume import MiniClusterExistingVolume
 from fluxoperator.models.mini_cluster_list import MiniClusterList
 from fluxoperator.models.mini_cluster_spec import MiniClusterSpec
 from fluxoperator.models.mini_cluster_status import MiniClusterStatus
 from fluxoperator.models.mini_cluster_user import MiniClusterUser
 from fluxoperator.models.mini_cluster_volume import MiniClusterVolume
+from fluxoperator.models.network import Network
 from fluxoperator.models.pod_spec import PodSpec
 from fluxoperator.models.security_context import SecurityContext
```

### Comparing `fluxoperator-0.0.26/fluxoperator/api_client.py` & `fluxoperator-0.0.28/fluxoperator/api_client.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.26/fluxoperator/client.py` & `fluxoperator-0.0.28/fluxoperator/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -358,20 +358,20 @@
             if len(pod_list.items) == 0:
                 ready = True
                 break
             time.sleep(retry_seconds)
         if not quiet:
             print("All pods are terminated.")
 
-    def delete_minicluster(self, name=None, namespace=None):
+    def delete_minicluster(self, name=None, namespace=None, **kwargs):
         """
         Deletion (and time the deletion of) the MiniCluster
         """
         namespace = namespace or self.namespace
-        res = delete_minicluster(name, namespace)
+        res = delete_minicluster(name, namespace, **kwargs)
         self.wait_termination_pods(name, namespace)
         return res
 
     def wait_pods(
         self,
         size=None,
         name=None,
```

### Comparing `fluxoperator-0.0.26/fluxoperator/configuration.py` & `fluxoperator-0.0.28/fluxoperator/configuration.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.26/fluxoperator/decorator.py` & `fluxoperator-0.0.28/fluxoperator/decorator.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.26/fluxoperator/exceptions.py` & `fluxoperator-0.0.28/fluxoperator/exceptions.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.26/fluxoperator/models/__init__.py` & `fluxoperator-0.0.28/fluxoperator/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,9 +27,10 @@
 from fluxoperator.models.mini_cluster_container import MiniClusterContainer
 from fluxoperator.models.mini_cluster_existing_volume import MiniClusterExistingVolume
 from fluxoperator.models.mini_cluster_list import MiniClusterList
 from fluxoperator.models.mini_cluster_spec import MiniClusterSpec
 from fluxoperator.models.mini_cluster_status import MiniClusterStatus
 from fluxoperator.models.mini_cluster_user import MiniClusterUser
 from fluxoperator.models.mini_cluster_volume import MiniClusterVolume
+from fluxoperator.models.network import Network
 from fluxoperator.models.pod_spec import PodSpec
 from fluxoperator.models.security_context import SecurityContext
```

### Comparing `fluxoperator-0.0.26/fluxoperator/models/commands.py` & `fluxoperator-0.0.28/fluxoperator/models/commands.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.26/fluxoperator/models/container_resources.py` & `fluxoperator-0.0.28/fluxoperator/models/container_resources.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.26/fluxoperator/models/container_volume.py` & `fluxoperator-0.0.28/fluxoperator/models/container_volume.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.26/fluxoperator/models/flux_restful.py` & `fluxoperator-0.0.28/fluxoperator/models/flux_restful.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.26/fluxoperator/models/flux_spec.py` & `fluxoperator-0.0.28/fluxoperator/models/flux_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.26/fluxoperator/models/flux_user.py` & `fluxoperator-0.0.28/fluxoperator/models/flux_user.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.26/fluxoperator/models/life_cycle.py` & `fluxoperator-0.0.28/fluxoperator/models/life_cycle.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.26/fluxoperator/models/logging_spec.py` & `fluxoperator-0.0.28/fluxoperator/models/logging_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.26/fluxoperator/models/mini_cluster.py` & `fluxoperator-0.0.28/fluxoperator/models/mini_cluster.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.26/fluxoperator/models/mini_cluster_archive.py` & `fluxoperator-0.0.28/fluxoperator/models/mini_cluster_archive.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.26/fluxoperator/models/mini_cluster_container.py` & `fluxoperator-0.0.28/fluxoperator/models/mini_cluster_container.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.26/fluxoperator/models/mini_cluster_existing_volume.py` & `fluxoperator-0.0.28/fluxoperator/models/mini_cluster_list.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,152 +14,151 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from fluxoperator.configuration import Configuration
 
 
-class MiniClusterExistingVolume(object):
+class MiniClusterList(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'claim_name': 'str',
-        'path': 'str',
-        'read_only': 'bool',
-        'secret_name': 'str'
+        'api_version': 'str',
+        'items': 'list[MiniCluster]',
+        'kind': 'str',
+        'metadata': 'V1ListMeta'
     }
 
     attribute_map = {
-        'claim_name': 'claimName',
-        'path': 'path',
-        'read_only': 'readOnly',
-        'secret_name': 'secretName'
+        'api_version': 'apiVersion',
+        'items': 'items',
+        'kind': 'kind',
+        'metadata': 'metadata'
     }
 
-    def __init__(self, claim_name=None, path=None, read_only=False, secret_name=None, local_vars_configuration=None):  # noqa: E501
-        """MiniClusterExistingVolume - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, api_version=None, items=None, kind=None, metadata=None, local_vars_configuration=None):  # noqa: E501
+        """MiniClusterList - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
-        self._claim_name = None
-        self._path = None
-        self._read_only = None
-        self._secret_name = None
+        self._api_version = None
+        self._items = None
+        self._kind = None
+        self._metadata = None
         self.discriminator = None
 
-        if claim_name is not None:
-            self.claim_name = claim_name
-        if path is not None:
-            self.path = path
-        if read_only is not None:
-            self.read_only = read_only
-        if secret_name is not None:
-            self.secret_name = secret_name
+        if api_version is not None:
+            self.api_version = api_version
+        self.items = items
+        if kind is not None:
+            self.kind = kind
+        if metadata is not None:
+            self.metadata = metadata
 
     @property
-    def claim_name(self):
-        """Gets the claim_name of this MiniClusterExistingVolume.  # noqa: E501
+    def api_version(self):
+        """Gets the api_version of this MiniClusterList.  # noqa: E501
 
-        Claim name if the existing volume is a PVC  # noqa: E501
+        APIVersion defines the versioned schema of this representation of an object. Servers should convert recognized schemas to the latest internal value, and may reject unrecognized values. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources  # noqa: E501
 
-        :return: The claim_name of this MiniClusterExistingVolume.  # noqa: E501
+        :return: The api_version of this MiniClusterList.  # noqa: E501
         :rtype: str
         """
-        return self._claim_name
+        return self._api_version
 
-    @claim_name.setter
-    def claim_name(self, claim_name):
-        """Sets the claim_name of this MiniClusterExistingVolume.
+    @api_version.setter
+    def api_version(self, api_version):
+        """Sets the api_version of this MiniClusterList.
 
-        Claim name if the existing volume is a PVC  # noqa: E501
+        APIVersion defines the versioned schema of this representation of an object. Servers should convert recognized schemas to the latest internal value, and may reject unrecognized values. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources  # noqa: E501
 
-        :param claim_name: The claim_name of this MiniClusterExistingVolume.  # noqa: E501
-        :type claim_name: str
+        :param api_version: The api_version of this MiniClusterList.  # noqa: E501
+        :type api_version: str
         """
 
-        self._claim_name = claim_name
+        self._api_version = api_version
 
     @property
-    def path(self):
-        """Gets the path of this MiniClusterExistingVolume.  # noqa: E501
+    def items(self):
+        """Gets the items of this MiniClusterList.  # noqa: E501
 
-        Path and claim name are always required if a secret isn't defined  # noqa: E501
 
-        :return: The path of this MiniClusterExistingVolume.  # noqa: E501
-        :rtype: str
+        :return: The items of this MiniClusterList.  # noqa: E501
+        :rtype: list[MiniCluster]
         """
-        return self._path
+        return self._items
 
-    @path.setter
-    def path(self, path):
-        """Sets the path of this MiniClusterExistingVolume.
+    @items.setter
+    def items(self, items):
+        """Sets the items of this MiniClusterList.
 
-        Path and claim name are always required if a secret isn't defined  # noqa: E501
 
-        :param path: The path of this MiniClusterExistingVolume.  # noqa: E501
-        :type path: str
+        :param items: The items of this MiniClusterList.  # noqa: E501
+        :type items: list[MiniCluster]
         """
+        if self.local_vars_configuration.client_side_validation and items is None:  # noqa: E501
+            raise ValueError("Invalid value for `items`, must not be `None`")  # noqa: E501
 
-        self._path = path
+        self._items = items
 
     @property
-    def read_only(self):
-        """Gets the read_only of this MiniClusterExistingVolume.  # noqa: E501
+    def kind(self):
+        """Gets the kind of this MiniClusterList.  # noqa: E501
 
+        Kind is a string value representing the REST resource this object represents. Servers may infer this from the endpoint the client submits requests to. Cannot be updated. In CamelCase. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds  # noqa: E501
 
-        :return: The read_only of this MiniClusterExistingVolume.  # noqa: E501
-        :rtype: bool
+        :return: The kind of this MiniClusterList.  # noqa: E501
+        :rtype: str
         """
-        return self._read_only
+        return self._kind
 
-    @read_only.setter
-    def read_only(self, read_only):
-        """Sets the read_only of this MiniClusterExistingVolume.
+    @kind.setter
+    def kind(self, kind):
+        """Sets the kind of this MiniClusterList.
 
+        Kind is a string value representing the REST resource this object represents. Servers may infer this from the endpoint the client submits requests to. Cannot be updated. In CamelCase. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds  # noqa: E501
 
-        :param read_only: The read_only of this MiniClusterExistingVolume.  # noqa: E501
-        :type read_only: bool
+        :param kind: The kind of this MiniClusterList.  # noqa: E501
+        :type kind: str
         """
 
-        self._read_only = read_only
+        self._kind = kind
 
     @property
-    def secret_name(self):
-        """Gets the secret_name of this MiniClusterExistingVolume.  # noqa: E501
+    def metadata(self):
+        """Gets the metadata of this MiniClusterList.  # noqa: E501
 
-        An existing secret  # noqa: E501
 
-        :return: The secret_name of this MiniClusterExistingVolume.  # noqa: E501
-        :rtype: str
+        :return: The metadata of this MiniClusterList.  # noqa: E501
+        :rtype: V1ListMeta
         """
-        return self._secret_name
+        return self._metadata
 
-    @secret_name.setter
-    def secret_name(self, secret_name):
-        """Sets the secret_name of this MiniClusterExistingVolume.
+    @metadata.setter
+    def metadata(self, metadata):
+        """Sets the metadata of this MiniClusterList.
 
-        An existing secret  # noqa: E501
 
-        :param secret_name: The secret_name of this MiniClusterExistingVolume.  # noqa: E501
-        :type secret_name: str
+        :param metadata: The metadata of this MiniClusterList.  # noqa: E501
+        :type metadata: V1ListMeta
         """
 
-        self._secret_name = secret_name
+        self._metadata = metadata
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
@@ -195,18 +194,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, MiniClusterExistingVolume):
+        if not isinstance(other, MiniClusterList):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, MiniClusterExistingVolume):
+        if not isinstance(other, MiniClusterList):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `fluxoperator-0.0.26/fluxoperator/models/mini_cluster_spec.py` & `fluxoperator-0.0.28/fluxoperator/models/mini_cluster_spec.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,14 +39,15 @@
         'deadline_seconds': 'int',
         'flux': 'FluxSpec',
         'flux_restful': 'FluxRestful',
         'interactive': 'bool',
         'job_labels': 'dict(str, str)',
         'logging': 'LoggingSpec',
         'max_size': 'int',
+        'network': 'Network',
         'pod': 'PodSpec',
         'services': 'list[MiniClusterContainer]',
         'size': 'int',
         'tasks': 'int',
         'users': 'list[MiniClusterUser]',
         'volumes': 'dict(str, MiniClusterVolume)'
     }
@@ -58,23 +59,24 @@
         'deadline_seconds': 'deadlineSeconds',
         'flux': 'flux',
         'flux_restful': 'fluxRestful',
         'interactive': 'interactive',
         'job_labels': 'jobLabels',
         'logging': 'logging',
         'max_size': 'maxSize',
+        'network': 'network',
         'pod': 'pod',
         'services': 'services',
         'size': 'size',
         'tasks': 'tasks',
         'users': 'users',
         'volumes': 'volumes'
     }
 
-    def __init__(self, archive=None, cleanup=False, containers=None, deadline_seconds=31500000, flux=None, flux_restful=None, interactive=False, job_labels=None, logging=None, max_size=None, pod=None, services=None, size=1, tasks=1, users=None, volumes=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, archive=None, cleanup=False, containers=None, deadline_seconds=31500000, flux=None, flux_restful=None, interactive=False, job_labels=None, logging=None, max_size=None, network=None, pod=None, services=None, size=1, tasks=1, users=None, volumes=None, local_vars_configuration=None):  # noqa: E501
         """MiniClusterSpec - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._archive = None
         self._cleanup = None
@@ -82,14 +84,15 @@
         self._deadline_seconds = None
         self._flux = None
         self._flux_restful = None
         self._interactive = None
         self._job_labels = None
         self._logging = None
         self._max_size = None
+        self._network = None
         self._pod = None
         self._services = None
         self._size = None
         self._tasks = None
         self._users = None
         self._volumes = None
         self.discriminator = None
@@ -109,14 +112,16 @@
             self.interactive = interactive
         if job_labels is not None:
             self.job_labels = job_labels
         if logging is not None:
             self.logging = logging
         if max_size is not None:
             self.max_size = max_size
+        if network is not None:
+            self.network = network
         if pod is not None:
             self.pod = pod
         if services is not None:
             self.services = services
         if size is not None:
             self.size = size
         if tasks is not None:
@@ -347,14 +352,35 @@
         :param max_size: The max_size of this MiniClusterSpec.  # noqa: E501
         :type max_size: int
         """
 
         self._max_size = max_size
 
     @property
+    def network(self):
+        """Gets the network of this MiniClusterSpec.  # noqa: E501
+
+
+        :return: The network of this MiniClusterSpec.  # noqa: E501
+        :rtype: Network
+        """
+        return self._network
+
+    @network.setter
+    def network(self, network):
+        """Sets the network of this MiniClusterSpec.
+
+
+        :param network: The network of this MiniClusterSpec.  # noqa: E501
+        :type network: Network
+        """
+
+        self._network = network
+
+    @property
     def pod(self):
         """Gets the pod of this MiniClusterSpec.  # noqa: E501
 
 
         :return: The pod of this MiniClusterSpec.  # noqa: E501
         :rtype: PodSpec
         """
```

### Comparing `fluxoperator-0.0.26/fluxoperator/models/mini_cluster_status.py` & `fluxoperator-0.0.28/fluxoperator/models/mini_cluster_status.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.26/fluxoperator/models/mini_cluster_user.py` & `fluxoperator-0.0.28/fluxoperator/models/mini_cluster_user.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.26/fluxoperator/models/mini_cluster_volume.py` & `fluxoperator-0.0.28/fluxoperator/models/mini_cluster_volume.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.26/fluxoperator/models/pod_spec.py` & `fluxoperator-0.0.28/fluxoperator/models/pod_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.26/fluxoperator/models/security_context.py` & `fluxoperator-0.0.28/fluxoperator/models/security_context.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.26/fluxoperator/resource/network.py` & `fluxoperator-0.0.28/fluxoperator/resource/network.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.26/fluxoperator/resource/pods.py` & `fluxoperator-0.0.28/fluxoperator/resource/pods.py`

 * *Files 7% similar despite different names*

```diff
@@ -131,17 +131,19 @@
             sys.exit(f'A "{required}" field is required as a keyword argument.')
 
     container = kwargs["container"]
     namespace = kwargs["namespace"]
     name = kwargs["name"]
     del kwargs["container"]
 
-    # The cluster should be running with the operator installed
-    config.load_kube_config()
-    crd_api = client.CustomObjectsApi()
+    # This allows the client to provide a custom crd that already has credentials
+    crd_api = kwargs.get('crd_api')
+    if not crd_api:
+        config.load_kube_config()
+        crd_api = client.CustomObjectsApi()
 
     # We assume that this is a single container to run flux
     # Multi-container support can eventually be added.
     # TODO when requested, add pod resources
     container = _get_container_spec(container)
 
     flux_spec = _get_flux_spec(kwargs.get("flux"))
@@ -172,20 +174,23 @@
         version=defaults.flux_operator_api_version,
         namespace=namespace,
         plural="miniclusters",
         body=minicluster,
     )
 
 
-def delete_minicluster(name, namespace):
+def delete_minicluster(name, namespace, **kwargs):
     """
     Delete a named MiniCluster.
     """
-    config.load_kube_config()
-    crd_api = client.CustomObjectsApi()
+    # This allows the client to provide a custom crd that already has credentials
+    crd_api = kwargs.get('crd_api')
+    if not crd_api:
+        config.load_kube_config()
+        crd_api = client.CustomObjectsApi()
 
     return crd_api.delete_namespaced_custom_object(
         group="flux-framework.org",
         version=defaults.flux_operator_api_version,
         namespace=namespace,
         plural="miniclusters",
         name=name,
```

### Comparing `fluxoperator-0.0.26/fluxoperator/rest.py` & `fluxoperator-0.0.28/fluxoperator/rest.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.26/fluxoperator.egg-info/PKG-INFO` & `fluxoperator-0.0.28/fluxoperator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluxoperator
-Version: 0.0.26
+Version: 0.0.28
 Summary: Python SDK for the Flux Operator
 Home-page: https://github.com/flux-framework/flux-operator/tree/main/python-sdk/v1alpha1
 Author: Vanessasaurus
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessasaurus
 License: Apache 2.0
 Keywords: flux-operator,flux-framework,kubernetes,workflows,jobs-api
@@ -91,14 +91,15 @@
  - [MiniClusterContainer](MiniClusterContainer.md)
  - [MiniClusterList](MiniClusterList.md)
  - [MiniClusterSpec](MiniClusterSpec.md)
  - [MiniClusterStatus](MiniClusterStatus.md)
  - [MiniClusterUser](MiniClusterUser.md)
  - [MiniClusterExistingVolume](MiniClusterExistingVolume.md)
  - [MiniClusterVolume](MiniClusterVolume.md)
+ - [Network](Network.md)
  - [PodSpec](PodSpec.md)
  - [SecurityContext](SecurityContext.md)
 
 ## Documentation For Authorization
 
  All endpoints do not require authorization (but they do require you have permission via your kubernetes config)
```

### Comparing `fluxoperator-0.0.26/fluxoperator.egg-info/SOURCES.txt` & `fluxoperator-0.0.28/fluxoperator.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 fluxoperator/models/mini_cluster_container.py
 fluxoperator/models/mini_cluster_existing_volume.py
 fluxoperator/models/mini_cluster_list.py
 fluxoperator/models/mini_cluster_spec.py
 fluxoperator/models/mini_cluster_status.py
 fluxoperator/models/mini_cluster_user.py
 fluxoperator/models/mini_cluster_volume.py
+fluxoperator/models/network.py
 fluxoperator/models/pod_spec.py
 fluxoperator/models/security_context.py
 fluxoperator/resource/__init__.py
 fluxoperator/resource/network.py
 fluxoperator/resource/pods.py
 test/__init__.py
 test/test_commands.py
@@ -53,9 +54,10 @@
 test/test_mini_cluster_container.py
 test/test_mini_cluster_existing_volume.py
 test/test_mini_cluster_list.py
 test/test_mini_cluster_spec.py
 test/test_mini_cluster_status.py
 test/test_mini_cluster_user.py
 test/test_mini_cluster_volume.py
+test/test_network.py
 test/test_pod_spec.py
 test/test_security_context.py
```

### Comparing `fluxoperator-0.0.26/setup.py` & `fluxoperator-0.0.28/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 ################################################################################
 # MAIN #########################################################################
 ################################################################################
 
 if __name__ == "__main__":
     setup(
         name="fluxoperator",
-        version="0.0.26",
+        version="0.0.28",
         author="Vanessasaurus",
         author_email="vsoch@users.noreply.github.com",
         maintainer="Vanessasaurus",
         packages=find_packages(),
         include_package_data=True,
         zip_safe=False,
         url="https://github.com/flux-framework/flux-operator/tree/main/python-sdk/v1alpha1",
```

### Comparing `fluxoperator-0.0.26/test/test_commands.py` & `fluxoperator-0.0.28/test/test_commands.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.26/test/test_container_resources.py` & `fluxoperator-0.0.28/test/test_container_resources.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.26/test/test_container_volume.py` & `fluxoperator-0.0.28/test/test_container_volume.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.26/test/test_flux_restful.py` & `fluxoperator-0.0.28/test/test_flux_restful.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.26/test/test_flux_spec.py` & `fluxoperator-0.0.28/test/test_flux_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.26/test/test_flux_user.py` & `fluxoperator-0.0.28/test/test_flux_user.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.26/test/test_life_cycle.py` & `fluxoperator-0.0.28/test/test_life_cycle.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.26/test/test_logging_spec.py` & `fluxoperator-0.0.28/test/test_logging_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.26/test/test_mini_cluster.py` & `fluxoperator-0.0.28/test/test_mini_cluster.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.26/test/test_mini_cluster_archive.py` & `fluxoperator-0.0.28/test/test_mini_cluster_archive.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.26/test/test_mini_cluster_container.py` & `fluxoperator-0.0.28/test/test_mini_cluster_container.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.26/test/test_mini_cluster_existing_volume.py` & `fluxoperator-0.0.28/test/test_mini_cluster_existing_volume.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.26/test/test_mini_cluster_list.py` & `fluxoperator-0.0.28/test/test_mini_cluster_list.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.26/test/test_mini_cluster_spec.py` & `fluxoperator-0.0.28/test/test_mini_cluster_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.26/test/test_mini_cluster_status.py` & `fluxoperator-0.0.28/test/test_mini_cluster_status.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.26/test/test_mini_cluster_user.py` & `fluxoperator-0.0.28/test/test_mini_cluster_user.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.26/test/test_mini_cluster_volume.py` & `fluxoperator-0.0.28/test/test_mini_cluster_volume.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.26/test/test_pod_spec.py` & `fluxoperator-0.0.28/test/test_pod_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.26/test/test_security_context.py` & `fluxoperator-0.0.28/test/test_security_context.py`

 * *Files identical despite different names*

