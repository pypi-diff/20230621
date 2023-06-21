# Comparing `tmp/arena-py-0.4.0.tar.gz` & `tmp/arena-py-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/arena-py-0.4.0.tar", last modified: Thu May 25 14:39:26 2023, max compression
+gzip compressed data, was "dist/arena-py-0.4.2.tar", last modified: Wed Jun 21 17:29:11 2023, max compression
```

## Comparing `arena-py-0.4.0.tar` & `arena-py-0.4.2.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 mwfarb     (501) staff       (20)        0 2023-05-25 14:39:26.195154 arena-py-0.4.0/
--rw-r--r--   0 mwfarb     (501) staff       (20)     1533 2020-12-01 18:59:55.000000 arena-py-0.4.0/LICENSE
--rw-r--r--   0 mwfarb     (501) staff       (20)     4346 2023-05-25 14:39:26.194939 arena-py-0.4.0/PKG-INFO
--rw-r--r--   0 mwfarb     (501) staff       (20)     3842 2023-02-02 16:06:13.000000 arena-py-0.4.0/README.md
-drwxr-xr-x   0 mwfarb     (501) staff       (20)        0 2023-05-25 14:39:26.178776 arena-py-0.4.0/arena/
--rw-r--r--   0 mwfarb     (501) staff       (20)      280 2022-06-06 21:30:11.000000 arena-py-0.4.0/arena/__init__.py
--rwxr-xr-x   0 mwfarb     (501) staff       (20)     3142 2022-06-24 16:57:42.000000 arena-py-0.4.0/arena/__main__.py
--rw-r--r--   0 mwfarb     (501) staff       (20)    12383 2023-05-25 14:11:15.000000 arena-py-0.4.0/arena/arena_mqtt.py
-drwxr-xr-x   0 mwfarb     (501) staff       (20)        0 2023-05-25 14:39:26.182245 arena-py-0.4.0/arena/attributes/
--rw-r--r--   0 mwfarb     (501) staff       (20)     1022 2023-04-11 20:21:11.000000 arena-py-0.4.0/arena/attributes/__init__.py
--rw-r--r--   0 mwfarb     (501) staff       (20)     1031 2021-03-01 16:34:58.000000 arena-py-0.4.0/arena/attributes/animation.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      139 2021-03-01 16:34:58.000000 arena-py-0.4.0/arena/attributes/animation_mixer.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      175 2021-01-22 22:37:37.000000 arena-py-0.4.0/arena/attributes/attribute.py
--rw-r--r--   0 mwfarb     (501) staff       (20)     1135 2021-06-28 19:02:43.000000 arena-py-0.4.0/arena/attributes/color.py
--rw-r--r--   0 mwfarb     (501) staff       (20)     4974 2023-04-11 16:20:00.000000 arena-py-0.4.0/arena/attributes/data.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      362 2023-04-11 17:08:06.000000 arena-py-0.4.0/arena/attributes/goto_url.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      764 2023-04-11 16:29:38.000000 arena-py-0.4.0/arena/attributes/impulse.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      503 2021-10-12 18:10:25.000000 arena-py-0.4.0/arena/attributes/jitsi_video.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      811 2022-03-22 01:57:06.000000 arena-py-0.4.0/arena/attributes/landmark.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      611 2023-04-11 20:36:06.000000 arena-py-0.4.0/arena/attributes/material.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      237 2023-04-12 12:33:13.000000 arena-py-0.4.0/arena/attributes/morph.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      357 2023-04-11 20:36:06.000000 arena-py-0.4.0/arena/attributes/physics.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      496 2021-01-22 22:37:37.000000 arena-py-0.4.0/arena/attributes/position.py
--rw-r--r--   0 mwfarb     (501) staff       (20)     1616 2023-03-15 15:58:06.000000 arena-py-0.4.0/arena/attributes/rotation.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      355 2021-01-22 22:37:37.000000 arena-py-0.4.0/arena/attributes/scale.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      247 2023-04-11 20:36:06.000000 arena-py-0.4.0/arena/attributes/sound.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      475 2023-04-11 20:22:33.000000 arena-py-0.4.0/arena/attributes/text_input.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      152 2023-04-11 20:33:16.000000 arena-py-0.4.0/arena/attributes/video_control.py
--rw-r--r--   0 mwfarb     (501) staff       (20)    16321 2023-04-14 11:40:07.000000 arena-py-0.4.0/arena/auth.py
--rw-r--r--   0 mwfarb     (501) staff       (20)     1127 2021-09-15 13:49:45.000000 arena-py-0.4.0/arena/base_object.py
--rw-r--r--   0 mwfarb     (501) staff       (20)     2762 2023-04-25 14:16:16.000000 arena-py-0.4.0/arena/device.py
-drwxr-xr-x   0 mwfarb     (501) staff       (20)        0 2023-05-25 14:39:26.183686 arena-py-0.4.0/arena/event_loop/
--rw-r--r--   0 mwfarb     (501) staff       (20)      267 2021-03-08 20:18:41.000000 arena-py-0.4.0/arena/event_loop/__init__.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      419 2021-01-22 22:37:37.000000 arena-py-0.4.0/arena/event_loop/async_worker.py
--rw-r--r--   0 mwfarb     (501) staff       (20)     1690 2021-06-28 19:02:43.000000 arena-py-0.4.0/arena/event_loop/asyncio_mqtt.py
--rw-r--r--   0 mwfarb     (501) staff       (20)     1749 2023-03-15 15:59:58.000000 arena-py-0.4.0/arena/event_loop/event_loop.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      651 2021-06-28 19:02:43.000000 arena-py-0.4.0/arena/event_loop/lazy_worker.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      841 2021-06-28 19:02:43.000000 arena-py-0.4.0/arena/event_loop/persistent_worker.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      129 2021-01-22 22:37:37.000000 arena-py-0.4.0/arena/event_loop/single_worker.py
--rw-r--r--   0 mwfarb     (501) staff       (20)     1171 2021-06-28 19:02:43.000000 arena-py-0.4.0/arena/event_loop/worker.py
-drwxr-xr-x   0 mwfarb     (501) staff       (20)        0 2023-05-25 14:39:26.184053 arena-py-0.4.0/arena/events/
--rw-r--r--   0 mwfarb     (501) staff       (20)       25 2021-01-22 22:37:37.000000 arena-py-0.4.0/arena/events/__init__.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      984 2021-01-22 22:37:37.000000 arena-py-0.4.0/arena/events/event.py
-drwxr-xr-x   0 mwfarb     (501) staff       (20)        0 2023-05-25 14:39:26.189096 arena-py-0.4.0/arena/objects/
--rw-r--r--   0 mwfarb     (501) staff       (20)     1289 2023-04-17 16:31:41.000000 arena-py-0.4.0/arena/objects/__init__.py
--rw-r--r--   0 mwfarb     (501) staff       (20)     6766 2023-04-25 13:54:03.000000 arena-py-0.4.0/arena/objects/arena_object.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      516 2021-03-03 22:16:46.000000 arena-py-0.4.0/arena/objects/box.py
--rw-r--r--   0 mwfarb     (501) staff       (20)     1569 2021-03-03 22:16:46.000000 arena-py-0.4.0/arena/objects/camera.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      236 2023-04-12 18:42:29.000000 arena-py-0.4.0/arena/objects/circle.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      228 2021-03-03 22:16:46.000000 arena-py-0.4.0/arena/objects/cone.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      243 2021-03-03 22:16:46.000000 arena-py-0.4.0/arena/objects/cylinder.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      260 2021-03-03 22:16:46.000000 arena-py-0.4.0/arena/objects/dodecahedron.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      236 2023-04-17 18:03:03.000000 arena-py-0.4.0/arena/objects/entity.py
--rw-r--r--   0 mwfarb     (501) staff       (20)     1320 2021-09-15 13:49:45.000000 arena-py-0.4.0/arena/objects/gltf.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      256 2021-03-03 22:16:46.000000 arena-py-0.4.0/arena/objects/icosahedron.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      249 2021-03-03 22:16:46.000000 arena-py-0.4.0/arena/objects/image.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      232 2021-03-03 22:16:46.000000 arena-py-0.4.0/arena/objects/light.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      332 2021-03-03 22:16:46.000000 arena-py-0.4.0/arena/objects/line.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      252 2021-03-03 22:16:46.000000 arena-py-0.4.0/arena/objects/octahedron.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      244 2023-04-17 16:28:29.000000 arena-py-0.4.0/arena/objects/particle.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      232 2021-03-03 22:16:46.000000 arena-py-0.4.0/arena/objects/plane.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      228 2021-03-03 22:16:46.000000 arena-py-0.4.0/arena/objects/ring.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      236 2021-03-03 22:16:46.000000 arena-py-0.4.0/arena/objects/sphere.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      256 2021-03-03 22:16:46.000000 arena-py-0.4.0/arena/objects/tetrahedron.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      264 2021-03-03 22:16:46.000000 arena-py-0.4.0/arena/objects/text.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      968 2021-04-07 22:02:00.000000 arena-py-0.4.0/arena/objects/thickline.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      232 2021-03-03 22:16:46.000000 arena-py-0.4.0/arena/objects/torus.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      248 2021-03-03 22:16:46.000000 arena-py-0.4.0/arena/objects/torus_knot.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      244 2021-03-03 22:16:46.000000 arena-py-0.4.0/arena/objects/triangle.py
--rw-r--r--   0 mwfarb     (501) staff       (20)    16310 2023-05-25 14:06:53.000000 arena-py-0.4.0/arena/scene.py
-drwxr-xr-x   0 mwfarb     (501) staff       (20)        0 2023-05-25 14:39:26.191537 arena-py-0.4.0/arena/scripts/
--rw-r--r--   0 mwfarb     (501) staff       (20)        0 2021-10-12 18:10:25.000000 arena-py-0.4.0/arena/scripts/__init__.py
--rwxr-xr-x   0 mwfarb     (501) staff       (20)      122 2021-10-12 18:10:25.000000 arena-py-0.4.0/arena/scripts/arena_py_permissions.py
--rwxr-xr-x   0 mwfarb     (501) staff       (20)      557 2021-10-12 18:10:25.000000 arena-py-0.4.0/arena/scripts/arena_py_pub.py
--rwxr-xr-x   0 mwfarb     (501) staff       (20)      118 2021-10-12 18:10:25.000000 arena-py-0.4.0/arena/scripts/arena_py_signout.py
--rwxr-xr-x   0 mwfarb     (501) staff       (20)      559 2021-10-12 18:10:25.000000 arena-py-0.4.0/arena/scripts/arena_py_sub.py
--rwxr-xr-x   0 mwfarb     (501) staff       (20)      229 2021-10-12 18:10:25.000000 arena-py-0.4.0/arena/scripts/arena_py_token.py
-drwxr-xr-x   0 mwfarb     (501) staff       (20)        0 2023-05-25 14:39:26.193594 arena-py-0.4.0/arena/utils/
--rw-r--r--   0 mwfarb     (501) staff       (20)       25 2021-01-22 22:37:37.000000 arena-py-0.4.0/arena/utils/__init__.py
--rw-r--r--   0 mwfarb     (501) staff       (20)      781 2021-03-01 16:34:58.000000 arena-py-0.4.0/arena/utils/utils.py
-drwxr-xr-x   0 mwfarb     (501) staff       (20)        0 2023-05-25 14:39:26.194652 arena-py-0.4.0/arena_py.egg-info/
--rw-r--r--   0 mwfarb     (501) staff       (20)     4346 2023-05-25 14:39:25.000000 arena-py-0.4.0/arena_py.egg-info/PKG-INFO
--rw-r--r--   0 mwfarb     (501) staff       (20)     2057 2023-05-25 14:39:26.000000 arena-py-0.4.0/arena_py.egg-info/SOURCES.txt
--rw-r--r--   0 mwfarb     (501) staff       (20)        1 2023-05-25 14:39:25.000000 arena-py-0.4.0/arena_py.egg-info/dependency_links.txt
--rw-r--r--   0 mwfarb     (501) staff       (20)      308 2023-05-25 14:39:25.000000 arena-py-0.4.0/arena_py.egg-info/entry_points.txt
--rw-r--r--   0 mwfarb     (501) staff       (20)      150 2023-05-25 14:39:26.000000 arena-py-0.4.0/arena_py.egg-info/requires.txt
--rw-r--r--   0 mwfarb     (501) staff       (20)        6 2023-05-25 14:39:26.000000 arena-py-0.4.0/arena_py.egg-info/top_level.txt
--rw-r--r--   0 mwfarb     (501) staff       (20)       38 2023-05-25 14:39:26.195227 arena-py-0.4.0/setup.cfg
--rw-r--r--   0 mwfarb     (501) staff       (20)     1451 2023-05-25 14:36:07.000000 arena-py-0.4.0/setup.py
+drwxr-xr-x   0 mwfarb     (501) staff       (20)        0 2023-06-21 17:29:11.867573 arena-py-0.4.2/
+-rw-r--r--   0 mwfarb     (501) staff       (20)     1533 2020-12-01 18:59:55.000000 arena-py-0.4.2/LICENSE
+-rw-r--r--   0 mwfarb     (501) staff       (20)     4326 2023-06-21 17:29:11.867343 arena-py-0.4.2/PKG-INFO
+-rw-r--r--   0 mwfarb     (501) staff       (20)     3822 2023-05-26 19:27:46.000000 arena-py-0.4.2/README.md
+drwxr-xr-x   0 mwfarb     (501) staff       (20)        0 2023-06-21 17:29:11.852867 arena-py-0.4.2/arena/
+-rw-r--r--   0 mwfarb     (501) staff       (20)      280 2022-06-06 21:30:11.000000 arena-py-0.4.2/arena/__init__.py
+-rwxr-xr-x   0 mwfarb     (501) staff       (20)     3148 2023-05-26 19:27:46.000000 arena-py-0.4.2/arena/__main__.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)    12634 2023-05-26 19:27:46.000000 arena-py-0.4.2/arena/arena_mqtt.py
+drwxr-xr-x   0 mwfarb     (501) staff       (20)        0 2023-06-21 17:29:11.857177 arena-py-0.4.2/arena/attributes/
+-rw-r--r--   0 mwfarb     (501) staff       (20)     1022 2023-04-11 20:21:11.000000 arena-py-0.4.2/arena/attributes/__init__.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)     1031 2021-03-01 16:34:58.000000 arena-py-0.4.2/arena/attributes/animation.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      139 2021-03-01 16:34:58.000000 arena-py-0.4.2/arena/attributes/animation_mixer.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      175 2021-01-22 22:37:37.000000 arena-py-0.4.2/arena/attributes/attribute.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)     1135 2021-06-28 19:02:43.000000 arena-py-0.4.2/arena/attributes/color.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)     4974 2023-04-11 16:20:00.000000 arena-py-0.4.2/arena/attributes/data.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      362 2023-04-11 17:08:06.000000 arena-py-0.4.2/arena/attributes/goto_url.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      764 2023-04-11 16:29:38.000000 arena-py-0.4.2/arena/attributes/impulse.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      503 2021-10-12 18:10:25.000000 arena-py-0.4.2/arena/attributes/jitsi_video.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      811 2022-03-22 01:57:06.000000 arena-py-0.4.2/arena/attributes/landmark.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      611 2023-04-11 20:36:06.000000 arena-py-0.4.2/arena/attributes/material.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      237 2023-04-12 12:33:13.000000 arena-py-0.4.2/arena/attributes/morph.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      357 2023-04-11 20:36:06.000000 arena-py-0.4.2/arena/attributes/physics.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      496 2021-01-22 22:37:37.000000 arena-py-0.4.2/arena/attributes/position.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)     1616 2023-03-15 15:58:06.000000 arena-py-0.4.2/arena/attributes/rotation.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      355 2021-01-22 22:37:37.000000 arena-py-0.4.2/arena/attributes/scale.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      247 2023-04-11 20:36:06.000000 arena-py-0.4.2/arena/attributes/sound.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      475 2023-04-11 20:22:33.000000 arena-py-0.4.2/arena/attributes/text_input.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      152 2023-04-11 20:33:16.000000 arena-py-0.4.2/arena/attributes/video_control.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)    16461 2023-05-26 19:27:46.000000 arena-py-0.4.2/arena/auth.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)     1127 2021-09-15 13:49:45.000000 arena-py-0.4.2/arena/base_object.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)     2837 2023-05-26 19:27:46.000000 arena-py-0.4.2/arena/device.py
+drwxr-xr-x   0 mwfarb     (501) staff       (20)        0 2023-06-21 17:29:11.858691 arena-py-0.4.2/arena/event_loop/
+-rw-r--r--   0 mwfarb     (501) staff       (20)      267 2021-03-08 20:18:41.000000 arena-py-0.4.2/arena/event_loop/__init__.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      419 2021-01-22 22:37:37.000000 arena-py-0.4.2/arena/event_loop/async_worker.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)     1690 2021-06-28 19:02:43.000000 arena-py-0.4.2/arena/event_loop/asyncio_mqtt.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)     1749 2023-03-15 15:59:58.000000 arena-py-0.4.2/arena/event_loop/event_loop.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      651 2021-06-28 19:02:43.000000 arena-py-0.4.2/arena/event_loop/lazy_worker.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      841 2021-06-28 19:02:43.000000 arena-py-0.4.2/arena/event_loop/persistent_worker.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      129 2021-01-22 22:37:37.000000 arena-py-0.4.2/arena/event_loop/single_worker.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)     1171 2021-06-28 19:02:43.000000 arena-py-0.4.2/arena/event_loop/worker.py
+drwxr-xr-x   0 mwfarb     (501) staff       (20)        0 2023-06-21 17:29:11.858988 arena-py-0.4.2/arena/events/
+-rw-r--r--   0 mwfarb     (501) staff       (20)       25 2021-01-22 22:37:37.000000 arena-py-0.4.2/arena/events/__init__.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      984 2021-01-22 22:37:37.000000 arena-py-0.4.2/arena/events/event.py
+drwxr-xr-x   0 mwfarb     (501) staff       (20)        0 2023-06-21 17:29:11.864178 arena-py-0.4.2/arena/objects/
+-rw-r--r--   0 mwfarb     (501) staff       (20)     1289 2023-04-17 16:31:41.000000 arena-py-0.4.2/arena/objects/__init__.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)     6766 2023-04-25 13:54:03.000000 arena-py-0.4.2/arena/objects/arena_object.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      516 2021-03-03 22:16:46.000000 arena-py-0.4.2/arena/objects/box.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)     1569 2021-03-03 22:16:46.000000 arena-py-0.4.2/arena/objects/camera.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      236 2023-04-12 18:42:29.000000 arena-py-0.4.2/arena/objects/circle.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      228 2021-03-03 22:16:46.000000 arena-py-0.4.2/arena/objects/cone.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      243 2021-03-03 22:16:46.000000 arena-py-0.4.2/arena/objects/cylinder.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      260 2021-03-03 22:16:46.000000 arena-py-0.4.2/arena/objects/dodecahedron.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      236 2023-04-17 18:03:03.000000 arena-py-0.4.2/arena/objects/entity.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)     1320 2021-09-15 13:49:45.000000 arena-py-0.4.2/arena/objects/gltf.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      256 2021-03-03 22:16:46.000000 arena-py-0.4.2/arena/objects/icosahedron.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      249 2021-03-03 22:16:46.000000 arena-py-0.4.2/arena/objects/image.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      232 2021-03-03 22:16:46.000000 arena-py-0.4.2/arena/objects/light.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      332 2021-03-03 22:16:46.000000 arena-py-0.4.2/arena/objects/line.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      252 2021-03-03 22:16:46.000000 arena-py-0.4.2/arena/objects/octahedron.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      244 2023-04-17 16:28:29.000000 arena-py-0.4.2/arena/objects/particle.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      232 2021-03-03 22:16:46.000000 arena-py-0.4.2/arena/objects/plane.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      228 2021-03-03 22:16:46.000000 arena-py-0.4.2/arena/objects/ring.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      236 2021-03-03 22:16:46.000000 arena-py-0.4.2/arena/objects/sphere.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      256 2021-03-03 22:16:46.000000 arena-py-0.4.2/arena/objects/tetrahedron.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      264 2021-03-03 22:16:46.000000 arena-py-0.4.2/arena/objects/text.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      968 2021-04-07 22:02:00.000000 arena-py-0.4.2/arena/objects/thickline.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      232 2021-03-03 22:16:46.000000 arena-py-0.4.2/arena/objects/torus.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      248 2021-03-03 22:16:46.000000 arena-py-0.4.2/arena/objects/torus_knot.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      244 2021-03-03 22:16:46.000000 arena-py-0.4.2/arena/objects/triangle.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)    16309 2023-05-26 19:27:46.000000 arena-py-0.4.2/arena/scene.py
+drwxr-xr-x   0 mwfarb     (501) staff       (20)        0 2023-06-21 17:29:11.865216 arena-py-0.4.2/arena/scripts/
+-rw-r--r--   0 mwfarb     (501) staff       (20)        0 2021-10-12 18:10:25.000000 arena-py-0.4.2/arena/scripts/__init__.py
+-rwxr-xr-x   0 mwfarb     (501) staff       (20)      122 2021-10-12 18:10:25.000000 arena-py-0.4.2/arena/scripts/arena_py_permissions.py
+-rwxr-xr-x   0 mwfarb     (501) staff       (20)      557 2021-10-12 18:10:25.000000 arena-py-0.4.2/arena/scripts/arena_py_pub.py
+-rwxr-xr-x   0 mwfarb     (501) staff       (20)      118 2021-10-12 18:10:25.000000 arena-py-0.4.2/arena/scripts/arena_py_signout.py
+-rwxr-xr-x   0 mwfarb     (501) staff       (20)      559 2021-10-12 18:10:25.000000 arena-py-0.4.2/arena/scripts/arena_py_sub.py
+-rwxr-xr-x   0 mwfarb     (501) staff       (20)      229 2021-10-12 18:10:25.000000 arena-py-0.4.2/arena/scripts/arena_py_token.py
+drwxr-xr-x   0 mwfarb     (501) staff       (20)        0 2023-06-21 17:29:11.865599 arena-py-0.4.2/arena/utils/
+-rw-r--r--   0 mwfarb     (501) staff       (20)       25 2021-01-22 22:37:37.000000 arena-py-0.4.2/arena/utils/__init__.py
+-rw-r--r--   0 mwfarb     (501) staff       (20)      781 2021-03-01 16:34:58.000000 arena-py-0.4.2/arena/utils/utils.py
+drwxr-xr-x   0 mwfarb     (501) staff       (20)        0 2023-06-21 17:29:11.866867 arena-py-0.4.2/arena_py.egg-info/
+-rw-r--r--   0 mwfarb     (501) staff       (20)     4326 2023-06-21 17:29:11.000000 arena-py-0.4.2/arena_py.egg-info/PKG-INFO
+-rw-r--r--   0 mwfarb     (501) staff       (20)     2057 2023-06-21 17:29:11.000000 arena-py-0.4.2/arena_py.egg-info/SOURCES.txt
+-rw-r--r--   0 mwfarb     (501) staff       (20)        1 2023-06-21 17:29:11.000000 arena-py-0.4.2/arena_py.egg-info/dependency_links.txt
+-rw-r--r--   0 mwfarb     (501) staff       (20)      308 2023-06-21 17:29:11.000000 arena-py-0.4.2/arena_py.egg-info/entry_points.txt
+-rw-r--r--   0 mwfarb     (501) staff       (20)      150 2023-06-21 17:29:11.000000 arena-py-0.4.2/arena_py.egg-info/requires.txt
+-rw-r--r--   0 mwfarb     (501) staff       (20)        6 2023-06-21 17:29:11.000000 arena-py-0.4.2/arena_py.egg-info/top_level.txt
+-rw-r--r--   0 mwfarb     (501) staff       (20)       38 2023-06-21 17:29:11.867644 arena-py-0.4.2/setup.cfg
+-rw-r--r--   0 mwfarb     (501) staff       (20)     1451 2023-06-21 17:28:15.000000 arena-py-0.4.2/setup.py
```

### Comparing `arena-py-0.4.0/LICENSE` & `arena-py-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.0/PKG-INFO` & `arena-py-0.4.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arena-py
-Version: 0.4.0
+Version: 0.4.2
 Summary: Draw objects and run programs in the ARENA using Python!
 Home-page: https://github.com/arenaxr/ARENA-py
 Author: Conix Research Center
 Author-email: info@conix.io
 License: BSD 3-clause "New" or "Revised License"
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
@@ -33,15 +33,15 @@
 python hello.py
 ```
 
 `hello.py`
 ```python
 from arena import *
 
-scene = Scene(host="mqtt.arenaxr.org", scene="example")
+scene = Scene(host="arenaxr.org", scene="example")
 
 @scene.run_once
 def make_box():
     scene.add_object(Box())
 
 scene.run_tasks()
 ```
@@ -69,23 +69,23 @@
 ```
 ### Show Permissions
 ```bash
 arena-py-permissions
 ```
 ### CLI Subscribe to Scene Messages
 ```bash
-arena-py-sub -mh mqtt.arenaxr.org -s example
+arena-py-sub -mh arenaxr.org -s example
 ```
 ### CLI Subscribe to Custom Topic
 ```bash
-arena-py-sub -mh mqtt.arenaxr.org -t realm/g/a
+arena-py-sub -mh arenaxr.org -t realm/g/a
 ```
 ### CLI Publish a Scene Object Message
 ```bash
-arena-py-pub -mh mqtt.arenaxr.org -s example -m '{"object_id": "gltf-model_Earth", "action": "create", "type": "object", "data": {"object_type": "gltf-model", "position": {"x":0, "y": 0.1, "z": 0}, "url": "store/models/Earth.glb", "scale": {"x": 5, "y": 5, "z": 5}}}'
+arena-py-pub -mh arenaxr.org -s example -m '{"object_id": "gltf-model_Earth", "action": "create", "type": "object", "data": {"object_type": "gltf-model", "position": {"x":0, "y": 0.1, "z": 0}, "url": "store/models/Earth.glb", "scale": {"x": 5, "y": 5, "z": 5}}}'
 ```
 ### CLI Help
 ```bash
 arena-py-pub --help
 arena-py-sub --help
 ```
```

### Comparing `arena-py-0.4.0/README.md` & `arena-py-0.4.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 python hello.py
 ```
 
 `hello.py`
 ```python
 from arena import *
 
-scene = Scene(host="mqtt.arenaxr.org", scene="example")
+scene = Scene(host="arenaxr.org", scene="example")
 
 @scene.run_once
 def make_box():
     scene.add_object(Box())
 
 scene.run_tasks()
 ```
@@ -54,23 +54,23 @@
 ```
 ### Show Permissions
 ```bash
 arena-py-permissions
 ```
 ### CLI Subscribe to Scene Messages
 ```bash
-arena-py-sub -mh mqtt.arenaxr.org -s example
+arena-py-sub -mh arenaxr.org -s example
 ```
 ### CLI Subscribe to Custom Topic
 ```bash
-arena-py-sub -mh mqtt.arenaxr.org -t realm/g/a
+arena-py-sub -mh arenaxr.org -t realm/g/a
 ```
 ### CLI Publish a Scene Object Message
 ```bash
-arena-py-pub -mh mqtt.arenaxr.org -s example -m '{"object_id": "gltf-model_Earth", "action": "create", "type": "object", "data": {"object_type": "gltf-model", "position": {"x":0, "y": 0.1, "z": 0}, "url": "store/models/Earth.glb", "scale": {"x": 5, "y": 5, "z": 5}}}'
+arena-py-pub -mh arenaxr.org -s example -m '{"object_id": "gltf-model_Earth", "action": "create", "type": "object", "data": {"object_type": "gltf-model", "position": {"x":0, "y": 0.1, "z": 0}, "url": "store/models/Earth.glb", "scale": {"x": 5, "y": 5, "z": 5}}}'
 ```
 ### CLI Help
 ```bash
 arena-py-pub --help
 arena-py-sub --help
 ```
```

### Comparing `arena-py-0.4.0/arena/__main__.py` & `arena-py-0.4.2/arena/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import argparse
 import json
 
 from arena import *
 
 # define defaults
-DEFAULT_MQTT_HOST = "mqtt.arenaxr.org"
+DEFAULT_WEB_HOST = "arenaxr.org"
 PUBLISH = "pub"
 SUBSCRIBE = "sub"
 
 
 def on_msg_callback(scene, obj, msg):
     print(f"<{scene.root_topic}> \"{msg}\"")
 
@@ -42,16 +42,16 @@
         print(f"Publishing to topic: <{topic}>... ", end="")
         scene.mqttc.publish(topic, msg)
     print("done!")
 
     scene.stop_tasks()
 
 
-def main(mqtth, realm, scene, namespace, action, topic, message):
-    scene = Scene(host=mqtth, realm=realm, scene=scene, namespace=namespace)
+def main(host, realm, scene, namespace, action, topic, message):
+    scene = Scene(host=host, realm=realm, scene=scene, namespace=namespace)
 
     if action == SUBSCRIBE:
         if topic is None:
             print(f"Subscribing to topic: <{scene.subscribe_topic}>... ", end="")
             scene.on_msg_callback = on_msg_callback
         else:
             print(f"Subscribing to topic: <{topic}>... ", end="")
@@ -66,18 +66,18 @@
 
     scene.run_tasks()
 
 
 def cli():
     parser = argparse.ArgumentParser(description=("ARENA-py MQTT CLI"))
 
-    parser.add_argument("-mh", "--mqtth",
+    parser.add_argument("-mh", "--host",
                         type=str,
-                        help="MQTT host to connect to",
-                        default=DEFAULT_MQTT_HOST)
+                        help="ARENA webserver main host to connect to",
+                        default=DEFAULT_WEB_HOST)
     parser.add_argument("-r", "--realm",
                         type=str,
                         help="Realm to listen to",
                         default="realm")
     parser.add_argument("-s", "--scene",
                         type=str,
                         help="Scene to listen to")
```

### Comparing `arena-py-0.4.0/arena/arena_mqtt.py` & `arena-py-0.4.2/arena/arena_mqtt.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,26 +29,28 @@
                 on_msg_callback = None,
                 end_program_callback = None,
                 video = False,
                 debug = False,
                 **kwargs
             ):
         if os.environ.get("MQTTH"):
-            self.host = os.environ["MQTTH"]
+            self.web_host = os.environ["MQTTH"]
+            print(f"Using Host from 'MQTTH' env variable: {self.web_host}")
         elif "host" in kwargs and kwargs["host"]:
-            self.host = kwargs["host"]
-            print("Cannot find MQTTH environmental variable, using input parameter instead.")
+            self.web_host = kwargs["host"]
+            print(f"Using Host from 'host' input parameter: {self.web_host}")
         else:
-            sys.exit("mqtt host argument (host) is unspecified or None, aborting...")
+            sys.exit("ARENA webserver host argument (host) is unspecified or None, aborting...")
 
         if os.environ.get("REALM"):
             self.realm = os.environ["REALM"]
+            print(f"Using Realm from 'REALM' env variable: {self.realm}")
         elif "realm" in kwargs and kwargs["realm"]:
             self.realm = kwargs["realm"]
-            print("Cannot find REALM environmental variable, using input parameter instead.")
+            print(f"Using Realm from 'realm' input parameter: {self.realm}")
         else:
             # Use default "realm" until multiple realms exist, avoids user confusion.
             self.realm = realm
 
         self.debug = debug
 
         print("=====")
@@ -62,39 +64,41 @@
             self.username = os.environ["ARENA_USERNAME"]
             token = os.environ["ARENA_PASSWORD"]
             self.auth.store_environment_auth(self.username, token)
         else:
             if self.scene:
                 local = self.auth.check_local_auth()
             elif self.device:
-                local = self.auth.authenticate_device(self.host)
+                local = self.auth.authenticate_device(self.web_host)
             if local and "username" in local and "token" in local:
                 # auth 2nd: use locally saved token
                 self.username = local["username"]
                 token = local["token"]
             else:
                 if self.scene:
                     # auth 3rd: use the user account online
-                    self.username = self.auth.authenticate_user(self.host)
+                    self.username = self.auth.authenticate_user(self.web_host)
 
         if os.environ.get("NAMESPACE"):
             self.namespace = os.environ["NAMESPACE"]
         elif "namespace" not in kwargs or ("namespace" in kwargs and kwargs["namespace"] is None):
             self.namespace = self.username
         else:
             self.namespace = kwargs["namespace"]
 
         # Always use the the hostname specified by the user, or defaults.
         self.mqttc_id = "pyClient-" + self.generate_client_id()
 
         # fetch host config
         print("Fetching ARENA configuration...")
-        self.config_url = f"https://{self.host}/conf/defaults.json"
+        self.config_url = f"https://{self.web_host}/conf/defaults.json"
         self.config_data = json.loads(self.auth.urlopen(self.config_url))
 
+        self.mqtt_host = self.config_data["ARENADefaults"]["mqttHost"]
+
         # set up topic variables
         if self.scene:
             self.namespaced_target =  f"{self.namespace}/{self.scene}"
             self.root_topic = f"{self.realm}/s/{self.namespaced_target}"
         elif self.device:
             self.namespaced_target =  f"{self.namespace}/{self.device}"
             self.root_topic = f"{self.realm}/d/{self.namespaced_target}"
@@ -105,15 +109,15 @@
         self.mqttc = mqtt.Client(
             self.mqttc_id, clean_session=True
         )
 
         if self.scene and (not self.username or not token):
             # do scene auth by user
             data = self.auth.authenticate_scene(
-                self.host, self.realm, self.namespaced_target, self.username, video)
+                self.web_host, self.realm, self.namespaced_target, self.username, video)
             if "username" in data and "token" in data:
                 self.username = data["username"]
                 token = data["token"]
                 self.remote_auth_token = data
         self.mqttc.username_pw_set(username=self.username, password=token)
         print("=====")
 
@@ -143,33 +147,33 @@
         self.msg_queue = asyncio.Queue()
 
         # connect to mqtt broker
         if "port" in kwargs:
             port = kwargs["port"]
         else:
             port = 8883 # ARENA broker TLS 1.2 connection port
-        if self.auth.verify(self.host):
+        if self.auth.verify(self.web_host):
             self.mqttc.tls_set()
         else:
             self.mqttc.tls_set_context(ssl._create_unverified_context())
             self.mqttc.tls_insecure_set(True)
         try:
-            self.mqttc.connect(self.host, port=port)
+            self.mqttc.connect(self.mqtt_host, port=port)
         except Exception as err:
-            print(f'MQTT connect error to {self.host}, port={port}: {err}')
+            print(f'MQTT connect error to {self.mqtt_host}, port={port}: {err}')
         self.mqttc.socket().setsockopt(socket.SOL_SOCKET, socket.SO_SNDBUF, 2048)
 
 
     def parse_cli(self):
         """
         Reusable command-line options to give apps flexible options to avoid hard-coding locations.
         """
         parser = argparse.ArgumentParser(description=("ARENA-py Application CLI"))
-        parser.add_argument("-mh", "--mqtth", type=str,
-                            help="MQTT host to connect to")
+        parser.add_argument("-mh", "--host", type=str,
+                            help="ARENA webserver main host to connect to")
         parser.add_argument("-n", "--namespace", type=str,
                             help="Namespace of scene")
         parser.add_argument("-s", "--scene", type=str,
                             help="Scene to publish and listen to")
         parser.add_argument("-d", "--device", type=str,
                             help="Device to publish and listen to")
         parser.add_argument("-p", "--position", nargs=3, type=float, default=(0, 0, 0),
@@ -180,15 +184,15 @@
                             help="App scale in meters")
         parser.add_argument("-D", "--debug", action='store_true', help='Debug mode.', default=False)
         args = parser.parse_args()
         app_position = tuple(args.position)
         app_rotation = tuple(args.rotation)
         app_scale = tuple(args.scale)
         return {
-            "mqtth": args.mqtth,
+            "host": args.host,
             "namespace": args.namespace,
             "scene": args.scene,
             "device": args.device,
             "position": app_position,
             "rotation": app_rotation,
             "scale": app_scale,
             "debug": args.debug,
```

### Comparing `arena-py-0.4.0/arena/attributes/__init__.py` & `arena-py-0.4.2/arena/attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.0/arena/attributes/animation.py` & `arena-py-0.4.2/arena/attributes/animation.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.0/arena/attributes/color.py` & `arena-py-0.4.2/arena/attributes/color.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.0/arena/attributes/data.py` & `arena-py-0.4.2/arena/attributes/data.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.0/arena/attributes/impulse.py` & `arena-py-0.4.2/arena/attributes/impulse.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.0/arena/attributes/landmark.py` & `arena-py-0.4.2/arena/attributes/landmark.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.0/arena/attributes/material.py` & `arena-py-0.4.2/arena/attributes/material.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.0/arena/attributes/rotation.py` & `arena-py-0.4.2/arena/attributes/rotation.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.0/arena/auth.py` & `arena-py-0.4.2/arena/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,25 +34,25 @@
                "https://www.googleapis.com/auth/userinfo.email"]
 
     def __init__(self):
         self._csrftoken = None
         self._mqtt_token = None
         self._id_token = None
 
-    def authenticate_user(self, host):
+    def authenticate_user(self, web_host):
         """
         Begins authentication flow, getting Google auth, opening web browser if
         needed, getting username and state from ARENA server.
-        host: The hostname of the ARENA webserver.
+        web_host: The hostname of the ARENA webserver.
         Returns: Username from arena-account, or None.
         """
         print("Signing in to the ARENA...")
-        gauth_json = self._get_gauthid(host)
+        gauth_json = self._get_gauthid(web_host)
         creds = None
-        scene_auth_dir = self._get_scene_auth_path(host)
+        scene_auth_dir = self._get_scene_auth_path(web_host)
         scene_gauth_path = f"{scene_auth_dir}/{_gauth_file}"
 
         if not os.path.exists(scene_auth_dir):
             os.makedirs(scene_auth_dir)
 
         # store the user's access and refresh tokens
         if os.path.exists(scene_gauth_path):
@@ -102,91 +102,91 @@
             with open(scene_gauth_path, "wb") as token:
                 # save the credentials for the next run
                 pickle.dump(creds, token)
             os.chmod(scene_gauth_path, 0o600)  # set user-only perms.
 
         username = None
         self._id_token = creds.id_token
-        user_info = self._get_user_state(host, self._id_token)
+        user_info = self._get_user_state(web_host, self._id_token)
         _user_info = json.loads(user_info)
         if "authenticated" in _user_info and "username" in _user_info:
             username = _user_info["username"]
         profile_info = session.get(
             "https://www.googleapis.com/userinfo/v2/me").json()
         if profile_info:
             print(f"Authenticated Google account: {profile_info['email']}")
         return username
 
-    def authenticate_scene(self, host, realm, scene, username, video=False):
+    def authenticate_scene(self, web_host, realm, scene, username, video=False):
         """ End authentication flow, requesting permissions may change by owner
         or admin, for now, get a fresh mqtt_token each time.
-        host: The hostname of the ARENA webserver.
+        web_host: The hostname of the ARENA webserver.
         realm: The topic realm name.
         scene: The namespace/scene name combination.
         username: The ARENA username for the user.
         video: If Jitsi video conference is requested.
         Returns: username and mqtt_token from arena-account.
         """
-        scene_auth_dir = self._get_scene_auth_path(host)
+        scene_auth_dir = self._get_scene_auth_path(web_host)
         scene_mqtt_path = f"{scene_auth_dir}/{_mqtt_token_file}"
 
         print("Using remote-authenticated MQTT token.")
         mqtt_json = self._get_mqtt_token(
-            host, realm, scene, username, self._id_token, video)
+            web_host, realm, scene, username, self._id_token, video)
         # save mqtt_token
         with open(scene_mqtt_path, mode="w") as d:
             d.write(mqtt_json)
         os.chmod(scene_mqtt_path, 0o600)  # set user-only perms.
 
         self._mqtt_token = json.loads(mqtt_json)
         self._log_token()
         return self._mqtt_token
 
-    def authenticate_device(self, host):
+    def authenticate_device(self, web_host):
         """
         Check for device mqtt_token, ask for a missing one, and save to local memory.
         """
-        device_auth_dir = self._get_device_auth_path(host)
+        device_auth_dir = self._get_device_auth_path(web_host)
         device_mqtt_path = f"{device_auth_dir}/{_mqtt_token_file}"
         # check token expiration
         _remove_credentials(device_auth_dir, expire=True)
         # load device token if valid
         if os.path.exists(device_mqtt_path):
             print("Using user long-term device MQTT token.")
             f = open(device_mqtt_path, "r")
             mqtt_json = f.read()
             f.close()
         else:
             if not os.path.exists(device_auth_dir):
                 os.makedirs(device_auth_dir)
             print(
-                f"Generate a token for this device at https://{host}/user/profile")
+                f"Generate a token for this device at https://{web_host}/user/profile")
             mqtt_json = input(
                 "Paste auth MQTT full JSON here for this device: ")
             # save mqtt_token
             with open(device_mqtt_path, mode="w") as d:
                 d.write(mqtt_json)
             os.chmod(device_mqtt_path, 0o600)  # set user-only perms.
 
         self._mqtt_token = json.loads(mqtt_json)
         self._log_token()
         return self._mqtt_token
 
-    def _get_scene_auth_path(self, host):
-        return f"{_arena_user_dir}/python/{host}/s"
+    def _get_scene_auth_path(self, web_host):
+        return f"{_arena_user_dir}/python/{web_host}/s"
 
-    def _get_device_auth_path(self, host):
-        return f"{_arena_user_dir}/python/{host}/d"
+    def _get_device_auth_path(self, web_host):
+        return f"{_arena_user_dir}/python/{web_host}/d"
 
-    def get_writable_scenes(self, host):
+    def get_writable_scenes(self, web_host):
         """ Request list of scene names for logged in user that user has publish permission for.
-        host: The hostname of the ARENA webserver.
+        web_host: The hostname of the ARENA webserver.
         Returns: list of scenes.
         """
-        my_scenes = self._get_my_scenes(host, self._id_token)
+        my_scenes = self._get_my_scenes(web_host, self._id_token)
         return json.loads(my_scenes)
 
     def _is_headless_client(self):
         """ Determine headless or headed console.
         """
         if "SSH_TTY" in os.environ or "SSH_CLIENT" in os.environ:
             print("SSH connection detected, using headless auth.")
@@ -240,68 +240,68 @@
             mqtt_json = f.read()
             f.close()
             self._mqtt_token = json.loads(mqtt_json)
             self._log_token()
             return self._mqtt_token
         return None
 
-    def _get_csrftoken(self, host):
+    def _get_csrftoken(self, web_host):
         # get the csrftoken for django
-        csrf_url = f"https://{host}/user/login"
+        csrf_url = f"https://{web_host}/user/login"
         client = requests.session()
-        client.get(csrf_url, verify=self.verify(host))  # sets cookie
+        client.get(csrf_url, verify=self.verify(web_host))  # sets cookie
         if "csrftoken" in client.cookies:
             self._csrftoken = client.cookies["csrftoken"]
         elif "csrf" in client.cookies:
             self._csrftoken = client.cookies["csrf"]
         else:
             self._csrftoken = None
         return self._csrftoken
 
-    def _get_gauthid(self, host):
-        url = f"https://{host}/conf/gauth.json"
+    def _get_gauthid(self, web_host):
+        url = f"https://{web_host}/conf/gauth.json"
         return self.urlopen(url)
 
-    def _get_my_scenes(self, host, id_token):
-        url = f"https://{host}/user/my_scenes"
+    def _get_my_scenes(self, web_host, id_token):
+        url = f"https://{web_host}/user/my_scenes"
         if not self._csrftoken:
-            self._csrftoken = self._get_csrftoken(host)
+            self._csrftoken = self._get_csrftoken(web_host)
         params = {"id_token": id_token}
         query_string = parse.urlencode(params)
         data = query_string.encode("ascii")
         return self.urlopen(url, data=data, csrf=self._csrftoken)
 
-    def _get_user_state(self, host, id_token):
-        url = f"https://{host}/user/user_state"
+    def _get_user_state(self, web_host, id_token):
+        url = f"https://{web_host}/user/user_state"
         if not self._csrftoken:
-            self._csrftoken = self._get_csrftoken(host)
+            self._csrftoken = self._get_csrftoken(web_host)
         params = {"id_token": id_token}
         query_string = parse.urlencode(params)
         data = query_string.encode("ascii")
         return self.urlopen(url, data=data, csrf=self._csrftoken)
 
-    def _get_mqtt_token(self, host, realm, scene, username, id_token, video):
-        url = f"https://{host}/user/mqtt_auth"
+    def _get_mqtt_token(self, web_host, realm, scene, username, id_token, video):
+        url = f"https://{web_host}/user/mqtt_auth"
         if not self._csrftoken:
-            self._csrftoken = self._get_csrftoken(host)
+            self._csrftoken = self._get_csrftoken(web_host)
         params = {
             "id_auth": "google-installed",
             "username": username,
             "id_token": id_token,
             "realm": realm,
             "scene": scene
         }
         if video:
             params["camid"] = True
         query_string = parse.urlencode(params)
         data = query_string.encode("ascii")
         return self.urlopen(url, data=data, csrf=self._csrftoken)
 
-    def verify(self, host):
-        return host != "localhost"
+    def verify(self, web_host):
+        return web_host != "localhost"
 
     def urlopen(self, url, data=None, creds=False, csrf=None):
         """ urlopen is for ARENA URL connections.
         url: the url to POST/GET.
         data: None for GET, add params for POST.
         creds: True to pass the MQTT token as a cookie.
         csrf: The csrftoken.
```

### Comparing `arena-py-0.4.0/arena/base_object.py` & `arena-py-0.4.2/arena/base_object.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.0/arena/device.py` & `arena-py-0.4.2/arena/device.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 class Device(ArenaMQTT):
     """
     Gives access to an ARENA device.
     Can create and execute various user-defined functions/tasks.
 
-    :param str host: Hostname of the MQTT broker (required).
+    :param str host: Hostname of the ARENA webserver (required).
     :param str realm: Reserved topic fork for future use (optional).
     :param str namespace: Username of authenticated user or other namespace (automatic).
     :param str device: The name of the device, without namespace (required).
     """
 
     def __init__(
                 self,
@@ -25,41 +25,43 @@
                 end_program_callback = None,
                 debug = False,
                 cli_args = False,
                 **kwargs
             ):
         if cli_args:
             self.args = self.parse_cli()
-            if self.args["mqtth"]:
-                kwargs["host"] = self.args["mqtth"]
+            if self.args["host"]:
+                kwargs["host"] = self.args["host"]
             if self.args["namespace"]:
                 kwargs["namespace"] = self.args["namespace"]
             if self.args["device"]:
                 kwargs["device"] = self.args["device"]
             if self.args["debug"]:
                 debug = self.args["debug"]
 
         if os.environ.get("DEVICE"):
             self.device = os.environ["DEVICE"]
+            print(f"Using Device from 'DEVICE' env variable: {self.device}")
         elif "device" in kwargs and kwargs["device"]:
             if re.search("/", kwargs["device"]):
-                sys.exit("device argument (device) cannot include '/', aborting...")
+                sys.exit("Device argument (device) cannot include '/', aborting...")
             self.device = kwargs["device"]
-            print("Cannot find DEVICE environmental variable, using input parameter instead.")
+            print(f"Using Device from 'device' input parameter: {self.device}")
         else:
-            sys.exit("device argument (device) is unspecified or None, aborting...")
+            sys.exit("Device argument (device) is unspecified or None, aborting...")
+
         super().__init__(
             realm,
             network_latency_interval,
             on_msg_callback,
             end_program_callback,
             debug,
             **kwargs
         )
-        print(f"Device topic ready: {self.realm}/d/{self.namespace}/{self.device}, host={self.host}")
+        print(f"Device topic ready: {self.realm}/d/{self.namespace}/{self.device}, mqtt_host={self.mqtt_host}")
 
     async def process_message(self):
         while True:
             msg = await self.msg_queue.get()
             # extract payload
             try:
                 payload_str = msg.payload.decode("utf-8", "ignore")
```

### Comparing `arena-py-0.4.0/arena/event_loop/asyncio_mqtt.py` & `arena-py-0.4.2/arena/event_loop/asyncio_mqtt.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.0/arena/event_loop/event_loop.py` & `arena-py-0.4.2/arena/event_loop/event_loop.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.0/arena/event_loop/lazy_worker.py` & `arena-py-0.4.2/arena/event_loop/lazy_worker.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.0/arena/event_loop/persistent_worker.py` & `arena-py-0.4.2/arena/event_loop/persistent_worker.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.0/arena/event_loop/worker.py` & `arena-py-0.4.2/arena/event_loop/worker.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.0/arena/events/event.py` & `arena-py-0.4.2/arena/events/event.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.0/arena/objects/__init__.py` & `arena-py-0.4.2/arena/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.0/arena/objects/arena_object.py` & `arena-py-0.4.2/arena/objects/arena_object.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.0/arena/objects/box.py` & `arena-py-0.4.2/arena/objects/box.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.0/arena/objects/camera.py` & `arena-py-0.4.2/arena/objects/camera.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.0/arena/objects/gltf.py` & `arena-py-0.4.2/arena/objects/gltf.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.0/arena/objects/thickline.py` & `arena-py-0.4.2/arena/objects/thickline.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.0/arena/scene.py` & `arena-py-0.4.2/arena/scene.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 class Scene(ArenaMQTT):
     """
     Gives access to an ARENA scene.
     Can create and execute various user-defined functions/tasks.
 
-    :param str host: Hostname of the MQTT broker (required).
+    :param str host: Hostname of the ARENA webserver (required).
     :param str realm: Reserved topic fork for future use (optional).
     :param str namespace: Username of authenticated user or other namespace (automatic).
     :param str scene: The name of the scene, without namespace (required).
     """
 
     def __init__(
                 self,
@@ -36,43 +36,44 @@
                 video = False,
                 debug = False,
                 cli_args = False,
                 **kwargs
             ):
         if cli_args:
             self.args = self.parse_cli()
-            if self.args["mqtth"]:
-                kwargs["host"] = self.args["mqtth"]
+            if self.args["host"]:
+                kwargs["host"] = self.args["host"]
             if self.args["namespace"]:
                 kwargs["namespace"] = self.args["namespace"]
             if self.args["scene"]:
                 kwargs["scene"] = self.args["scene"]
             if self.args["debug"]:
                 debug = self.args["debug"]
 
         if os.environ.get("SCENE"):
             self.scene = os.environ["SCENE"]
+            print(f"Using Scene from 'SCENE' env variable: {self.scene}")
         elif "scene" in kwargs and kwargs["scene"]:
             if re.search("/", kwargs["scene"]):
-                sys.exit("scene argument (scene) cannot include '/', aborting...")
+                sys.exit("Scene argument (scene) cannot include '/', aborting...")
             self.scene = kwargs["scene"]
-            print("Cannot find SCENE environmental variable, using input parameter instead.")
+            print(f"Using Scene from 'scene' input parameter: {self.scene}")
         else:
-            sys.exit("scene argument (scene) is unspecified or None, aborting...")
+            sys.exit("Scene argument (scene) is unspecified or None, aborting...")
+
         super().__init__(
             realm,
             network_latency_interval,
             on_msg_callback,
             end_program_callback,
             video,
             debug,
             **kwargs
         )
 
-        self.jitsi_host = self.config_data["ARENADefaults"]["jitsiHost"]
         self.persist_host = self.config_data["ARENADefaults"]["persistHost"]
         self.persist_path = self.config_data["ARENADefaults"]["persistPath"]
 
         self.persist_url = f"https://{self.persist_host}{self.persist_path}{self.namespaced_target}"
 
         # set up callbacks
         self.new_obj_callback = new_obj_callback
@@ -82,15 +83,15 @@
 
         self.unspecified_object_ids = set() # objects that exist in the scene,
                                             # but this scene instance does not
                                             # have a reference to
         self.users = {} # dict of all users
 
         # Always use the the hostname specified by the user, or defaults.
-        print(f"Loading: https://{self.host}/{self.namespace}/{self.scene}, realm={self.realm}")
+        print(f"Loading: https://{self.web_host}/{self.namespace}/{self.scene}, realm={self.realm}")
 
     def on_connect(self, client, userdata, flags, rc):
         super().on_connect(client, userdata, flags, rc)
         if rc == 0:
             # create ARENA-py Objects from persist server
             # no need to return anything here
             self.get_persisted_objs()
@@ -396,15 +397,15 @@
         output = json.loads(data)
         return output
 
     def get_writable_scenes(self):
         """ Request list of scene names for logged in user account that user has publish permission for.
         Returns: list of scenes.
         """
-        return self.auth.get_writable_scenes(host=self.host)
+        return self.auth.get_writable_scenes(web_host=self.web_host)
 
     def get_user_list(self):
         """Returns a list of users"""
         return self.users.values()
 
 class Arena(Scene):
     """
```

### Comparing `arena-py-0.4.0/arena/scripts/arena_py_pub.py` & `arena-py-0.4.2/arena/scripts/arena_py_pub.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.0/arena/scripts/arena_py_sub.py` & `arena-py-0.4.2/arena/scripts/arena_py_sub.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.0/arena/utils/utils.py` & `arena-py-0.4.2/arena/utils/utils.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.0/arena_py.egg-info/PKG-INFO` & `arena-py-0.4.2/arena_py.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arena-py
-Version: 0.4.0
+Version: 0.4.2
 Summary: Draw objects and run programs in the ARENA using Python!
 Home-page: https://github.com/arenaxr/ARENA-py
 Author: Conix Research Center
 Author-email: info@conix.io
 License: BSD 3-clause "New" or "Revised License"
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
@@ -33,15 +33,15 @@
 python hello.py
 ```
 
 `hello.py`
 ```python
 from arena import *
 
-scene = Scene(host="mqtt.arenaxr.org", scene="example")
+scene = Scene(host="arenaxr.org", scene="example")
 
 @scene.run_once
 def make_box():
     scene.add_object(Box())
 
 scene.run_tasks()
 ```
@@ -69,23 +69,23 @@
 ```
 ### Show Permissions
 ```bash
 arena-py-permissions
 ```
 ### CLI Subscribe to Scene Messages
 ```bash
-arena-py-sub -mh mqtt.arenaxr.org -s example
+arena-py-sub -mh arenaxr.org -s example
 ```
 ### CLI Subscribe to Custom Topic
 ```bash
-arena-py-sub -mh mqtt.arenaxr.org -t realm/g/a
+arena-py-sub -mh arenaxr.org -t realm/g/a
 ```
 ### CLI Publish a Scene Object Message
 ```bash
-arena-py-pub -mh mqtt.arenaxr.org -s example -m '{"object_id": "gltf-model_Earth", "action": "create", "type": "object", "data": {"object_type": "gltf-model", "position": {"x":0, "y": 0.1, "z": 0}, "url": "store/models/Earth.glb", "scale": {"x": 5, "y": 5, "z": 5}}}'
+arena-py-pub -mh arenaxr.org -s example -m '{"object_id": "gltf-model_Earth", "action": "create", "type": "object", "data": {"object_type": "gltf-model", "position": {"x":0, "y": 0.1, "z": 0}, "url": "store/models/Earth.glb", "scale": {"x": 5, "y": 5, "z": 5}}}'
 ```
 ### CLI Help
 ```bash
 arena-py-pub --help
 arena-py-sub --help
 ```
```

### Comparing `arena-py-0.4.0/arena_py.egg-info/SOURCES.txt` & `arena-py-0.4.2/arena_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arena-py-0.4.0/setup.py` & `arena-py-0.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as readme:
     long_description = readme.read()
 
 setuptools.setup(
     name="arena-py",
-    version="0.4.0",
+    version="0.4.2",
     author="Conix Research Center",
     author_email="info@conix.io",
     license="BSD 3-clause \"New\" or \"Revised License\"",
     description="Draw objects and run programs in the ARENA using Python!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/arenaxr/ARENA-py",
```

