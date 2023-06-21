# Comparing `tmp/cell-tracking-bc-2023.5.tar.gz` & `tmp/cell-tracking-bc-2023.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cell-tracking-bc-2023.5.tar", last modified: Mon Mar  6 15:39:15 2023, max compression
+gzip compressed data, was "cell-tracking-bc-2023.6.tar", last modified: Wed Jun 21 15:04:36 2023, max compression
```

## Comparing `cell-tracking-bc-2023.5.tar` & `cell-tracking-bc-2023.6.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-06 15:39:15.370250 cell-tracking-bc-2023.5/
--rw-r--r--   0 eric      (1000) users      (984)       61 2021-12-01 17:53:11.000000 cell-tracking-bc-2023.5/MANIFEST.in
--rw-r--r--   0 eric      (1000) users      (984)     3114 2023-03-06 15:39:15.370250 cell-tracking-bc-2023.5/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)      636 2021-02-02 12:30:22.000000 cell-tracking-bc-2023.5/README-COPYRIGHT.txt
--rw-r--r--   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 cell-tracking-bc-2023.5/README-LICENCE-utf8.txt
--rw-r--r--   0 eric      (1000) users      (984)     2286 2022-02-03 09:12:09.000000 cell-tracking-bc-2023.5/README.rst
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-06 15:39:15.346917 cell-tracking-bc-2023.5/cell_tracking_BC/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-06 15:39:15.346917 cell-tracking-bc-2023.5/cell_tracking_BC/catalog/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-06 15:39:15.346917 cell-tracking-bc-2023.5/cell_tracking_BC/catalog/channel/
--rw-r--r--   0 eric      (1000) users      (984)     1969 2023-02-13 12:56:29.000000 cell-tracking-bc-2023.5/cell_tracking_BC/catalog/channel/ratio.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-06 15:39:15.343583 cell-tracking-bc-2023.5/cell_tracking_BC/catalog/feature/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-06 15:39:15.346917 cell-tracking-bc-2023.5/cell_tracking_BC/catalog/feature/geometrical/
--rw-r--r--   0 eric      (1000) users      (984)        0 2023-02-15 15:28:16.000000 cell-tracking-bc-2023.5/cell_tracking_BC/catalog/feature/geometrical/dummy.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-06 15:39:15.346917 cell-tracking-bc-2023.5/cell_tracking_BC/catalog/feature/radiometric/
--rw-r--r--   0 eric      (1000) users      (984)     2574 2023-02-10 13:45:02.000000 cell-tracking-bc-2023.5/cell_tracking_BC/catalog/feature/radiometric/entropy.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-06 15:39:15.346917 cell-tracking-bc-2023.5/cell_tracking_BC/catalog/feature/set/
--rw-r--r--   0 eric      (1000) users      (984)     2532 2023-02-10 15:24:31.000000 cell-tracking-bc-2023.5/cell_tracking_BC/catalog/feature/set/numpy_.py
--rw-r--r--   0 eric      (1000) users      (984)     4169 2023-02-10 15:24:31.000000 cell-tracking-bc-2023.5/cell_tracking_BC/catalog/feature/set/skimage_.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-06 15:39:15.346917 cell-tracking-bc-2023.5/cell_tracking_BC/catalog/feature/temporal/
--rw-r--r--   0 eric      (1000) users      (984)     2140 2023-02-10 15:02:24.000000 cell-tracking-bc-2023.5/cell_tracking_BC/catalog/feature/temporal/shift.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-06 15:39:15.346917 cell-tracking-bc-2023.5/cell_tracking_BC/catalog/matching/
--rw-r--r--   0 eric      (1000) users      (984)     1985 2021-09-08 16:51:38.000000 cell-tracking-bc-2023.5/cell_tracking_BC/catalog/matching/jaccard.py
--rw-r--r--   0 eric      (1000) users      (984)     3209 2023-02-17 09:35:42.000000 cell-tracking-bc-2023.5/cell_tracking_BC/catalog/parser.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-06 15:39:15.350250 cell-tracking-bc-2023.5/cell_tracking_BC/catalog/processing/
--rw-r--r--   0 eric      (1000) users      (984)     3866 2023-02-10 13:53:35.000000 cell-tracking-bc-2023.5/cell_tracking_BC/catalog/processing/background.py
--rw-r--r--   0 eric      (1000) users      (984)     1976 2023-02-10 13:53:54.000000 cell-tracking-bc-2023.5/cell_tracking_BC/catalog/processing/contrast.py
--rw-r--r--   0 eric      (1000) users      (984)     2503 2023-02-10 13:54:29.000000 cell-tracking-bc-2023.5/cell_tracking_BC/catalog/processing/geometry.py
--rw-r--r--   0 eric      (1000) users      (984)     2991 2023-02-10 13:55:52.000000 cell-tracking-bc-2023.5/cell_tracking_BC/catalog/processing/registration.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-06 15:39:15.350250 cell-tracking-bc-2023.5/cell_tracking_BC/catalog/segmentation/
--rw-r--r--   0 eric      (1000) users      (984)     4374 2023-02-17 09:35:42.000000 cell-tracking-bc-2023.5/cell_tracking_BC/catalog/segmentation/tf_network.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-06 15:39:15.350250 cell-tracking-bc-2023.5/cell_tracking_BC/catalog/tracking/
--rw-r--r--   0 eric      (1000) users      (984)     5631 2023-02-10 13:58:46.000000 cell-tracking-bc-2023.5/cell_tracking_BC/catalog/tracking/gmb_tracker.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-06 15:39:15.343583 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-06 15:39:15.350250 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/file/
--rw-r--r--   0 eric      (1000) users      (984)    10676 2023-02-17 09:35:42.000000 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/file/event.py
--rw-r--r--   0 eric      (1000) users      (984)     6728 2023-02-17 09:35:42.000000 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/file/feature.py
--rw-r--r--   0 eric      (1000) users      (984)     4916 2023-02-17 09:35:42.000000 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/file/path.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-06 15:39:15.353583 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/file/table/
--rw-r--r--   0 eric      (1000) users      (984)     3076 2023-02-08 13:52:59.000000 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/file/table/cell.py
--rw-r--r--   0 eric      (1000) users      (984)     3480 2023-02-08 13:56:27.000000 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/file/table/chart.py
--rw-r--r--   0 eric      (1000) users      (984)     2388 2023-02-08 13:57:24.000000 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/file/table/column.py
--rw-r--r--   0 eric      (1000) users      (984)     2208 2023-02-11 18:31:12.000000 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/file/table/sheet.py
--rw-r--r--   0 eric      (1000) users      (984)     5734 2023-02-17 09:35:42.000000 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/file/track.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-06 15:39:15.353583 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/
--rw-r--r--   0 eric      (1000) users      (984)     7863 2023-01-24 09:27:19.000000 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/annotations.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-06 15:39:15.343583 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/dbe/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-06 15:39:15.356917 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/dbe/matplotlib/
--rw-r--r--   0 eric      (1000) users      (984)     2754 2022-02-17 13:49:51.000000 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/dbe/matplotlib/context.py
--rw-r--r--   0 eric      (1000) users      (984)     9151 2023-01-18 14:25:10.000000 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/dbe/matplotlib/d_2.py
--rw-r--r--   0 eric      (1000) users      (984)     7982 2022-07-09 12:00:34.000000 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/dbe/matplotlib/d_3.py
--rw-r--r--   0 eric      (1000) users      (984)     8450 2023-02-17 09:42:06.000000 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/dbe/matplotlib/d_any.py
--rw-r--r--   0 eric      (1000) users      (984)     6053 2022-05-31 12:24:19.000000 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/dbe/matplotlib/event.py
--rw-r--r--   0 eric      (1000) users      (984)     2798 2021-11-10 10:18:31.000000 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/dbe/matplotlib/style.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-06 15:39:15.356917 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/dbe/vedo/
--rw-r--r--   0 eric      (1000) users      (984)     1891 2022-02-01 15:12:55.000000 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/dbe/vedo/context.py
--rw-r--r--   0 eric      (1000) users      (984)     8915 2022-02-01 15:14:31.000000 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/dbe/vedo/d_3.py
--rw-r--r--   0 eric      (1000) users      (984)     5376 2022-02-23 16:34:49.000000 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/dbe/vedo/d_any.py
--rw-r--r--   0 eric      (1000) users      (984)     1873 2022-02-01 15:24:42.000000 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/dbe/vedo/missing.py
--rw-r--r--   0 eric      (1000) users      (984)     3207 2022-02-01 15:15:32.000000 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/dbe/vedo/style.py
--rw-r--r--   0 eric      (1000) users      (984)    14278 2023-02-17 09:35:42.000000 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/event.py
--rw-r--r--   0 eric      (1000) users      (984)     3736 2023-01-11 13:41:46.000000 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/feature.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-06 15:39:15.356917 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/generic/
--rw-r--r--   0 eric      (1000) users      (984)     4751 2023-01-18 14:26:08.000000 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/generic/d_2.py
--rw-r--r--   0 eric      (1000) users      (984)     4918 2023-01-11 13:38:38.000000 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/generic/d_3.py
--rw-r--r--   0 eric      (1000) users      (984)     2642 2023-01-20 16:01:30.000000 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/generic/d_any.py
--rw-r--r--   0 eric      (1000) users      (984)     4832 2023-01-17 13:23:40.000000 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/segmentation.py
--rw-r--r--   0 eric      (1000) users      (984)     7538 2023-01-13 14:12:23.000000 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/sequence.py
--rw-r--r--   0 eric      (1000) users      (984)    14093 2023-01-17 15:32:43.000000 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/tracking.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-06 15:39:15.360250 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/type/
--rw-r--r--   0 eric      (1000) users      (984)     1693 2022-01-25 19:46:56.000000 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/type/annotation.py
--rw-r--r--   0 eric      (1000) users      (984)     9774 2023-02-08 13:59:20.000000 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/type/axes.py
--rw-r--r--   0 eric      (1000) users      (984)     3564 2022-01-25 18:39:23.000000 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/type/color.py
--rw-r--r--   0 eric      (1000) users      (984)     3104 2022-02-17 13:51:26.000000 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/type/context.py
--rw-r--r--   0 eric      (1000) users      (984)    13212 2022-06-01 07:11:21.000000 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/type/e_viewer_2d_t.py
--rw-r--r--   0 eric      (1000) users      (984)     1590 2022-01-25 18:11:16.000000 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/type/event.py
--rw-r--r--   0 eric      (1000) users      (984)     3100 2022-05-31 12:20:28.000000 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/type/figure.py
--rw-r--r--   0 eric      (1000) users      (984)    12951 2023-01-20 16:01:59.000000 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/type/s_drawer_2d.py
--rw-r--r--   0 eric      (1000) users      (984)     7915 2023-01-18 14:30:43.000000 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/type/s_viewer_2d.py
--rw-r--r--   0 eric      (1000) users      (984)     3060 2022-01-26 09:00:12.000000 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/type/signatures.py
--rw-r--r--   0 eric      (1000) users      (984)     5295 2023-01-18 14:24:16.000000 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/type/t_explorer_2d.py
--rw-r--r--   0 eric      (1000) users      (984)    11377 2023-02-17 09:35:42.000000 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/type/t_viewer_2d.py
--rw-r--r--   0 eric      (1000) users      (984)     3190 2023-01-10 16:09:45.000000 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/type/track.py
--rw-r--r--   0 eric      (1000) users      (984)     1645 2022-01-26 08:45:06.000000 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/type/widget.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-06 15:39:15.363583 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/text/
--rw-r--r--   0 eric      (1000) users      (984)     1675 2021-11-25 09:11:46.000000 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/text/dev.py
--rw-r--r--   0 eric      (1000) users      (984)     4191 2023-02-10 15:18:51.000000 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/text/plot.py
--rw-r--r--   0 eric      (1000) users      (984)     4074 2022-01-25 09:33:16.000000 cell-tracking-bc-2023.5/cell_tracking_BC/in_out/text/progress.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-06 15:39:15.363583 cell-tracking-bc-2023.5/cell_tracking_BC/standard/
--rw-r--r--   0 eric      (1000) users      (984)     2899 2023-01-13 14:44:24.000000 cell-tracking-bc-2023.5/cell_tracking_BC/standard/issue.py
--rw-r--r--   0 eric      (1000) users      (984)     1632 2021-12-16 15:05:53.000000 cell-tracking-bc-2023.5/cell_tracking_BC/standard/number.py
--rw-r--r--   0 eric      (1000) users      (984)     1791 2023-02-11 18:22:01.000000 cell-tracking-bc-2023.5/cell_tracking_BC/standard/path.py
--rw-r--r--   0 eric      (1000) users      (984)     2450 2023-02-08 13:56:27.000000 cell-tracking-bc-2023.5/cell_tracking_BC/standard/uid.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-06 15:39:15.343583 cell-tracking-bc-2023.5/cell_tracking_BC/task/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-06 15:39:15.363583 cell-tracking-bc-2023.5/cell_tracking_BC/task/channel/
--rw-r--r--   0 eric      (1000) users      (984)     1690 2023-02-10 14:28:42.000000 cell-tracking-bc-2023.5/cell_tracking_BC/task/channel/base.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-06 15:39:15.363583 cell-tracking-bc-2023.5/cell_tracking_BC/task/feature/
--rw-r--r--   0 eric      (1000) users      (984)     2433 2023-02-10 14:12:05.000000 cell-tracking-bc-2023.5/cell_tracking_BC/task/feature/base.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-06 15:39:15.363583 cell-tracking-bc-2023.5/cell_tracking_BC/task/matching/
--rw-r--r--   0 eric      (1000) users      (984)     6346 2023-02-17 09:35:42.000000 cell-tracking-bc-2023.5/cell_tracking_BC/task/matching/pattern.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-06 15:39:15.363583 cell-tracking-bc-2023.5/cell_tracking_BC/task/processing/
--rw-r--r--   0 eric      (1000) users      (984)     1664 2023-02-10 11:25:18.000000 cell-tracking-bc-2023.5/cell_tracking_BC/task/processing/base.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-06 15:39:15.363583 cell-tracking-bc-2023.5/cell_tracking_BC/task/registration/
--rw-r--r--   0 eric      (1000) users      (984)     4710 2023-02-10 11:32:54.000000 cell-tracking-bc-2023.5/cell_tracking_BC/task/registration/rigid.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-06 15:39:15.366917 cell-tracking-bc-2023.5/cell_tracking_BC/task/segmentation/
--rw-r--r--   0 eric      (1000) users      (984)    20183 2023-02-17 09:35:42.000000 cell-tracking-bc-2023.5/cell_tracking_BC/task/segmentation/frame.py
--rw-r--r--   0 eric      (1000) users      (984)     5269 2023-02-10 14:19:32.000000 cell-tracking-bc-2023.5/cell_tracking_BC/task/segmentation/sequence.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-06 15:39:15.366917 cell-tracking-bc-2023.5/cell_tracking_BC/task/tracking/
--rw-r--r--   0 eric      (1000) users      (984)     6615 2023-01-13 15:07:41.000000 cell-tracking-bc-2023.5/cell_tracking_BC/task/tracking/base.py
--rw-r--r--   0 eric      (1000) users      (984)     1647 2022-05-13 07:50:37.000000 cell-tracking-bc-2023.5/cell_tracking_BC/task/tracking/constant.py
--rw-r--r--   0 eric      (1000) users      (984)     2399 2022-06-28 12:49:37.000000 cell-tracking-bc-2023.5/cell_tracking_BC/track_finder.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-06 15:39:15.366917 cell-tracking-bc-2023.5/cell_tracking_BC/type/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-06 15:39:15.366917 cell-tracking-bc-2023.5/cell_tracking_BC/type/acquisition/
--rw-r--r--   0 eric      (1000) users      (984)     2006 2023-01-20 09:44:08.000000 cell-tracking-bc-2023.5/cell_tracking_BC/type/acquisition/frame.py
--rw-r--r--   0 eric      (1000) users      (984)    12594 2023-02-17 09:35:42.000000 cell-tracking-bc-2023.5/cell_tracking_BC/type/acquisition/sequence.py
--rw-r--r--   0 eric      (1000) users      (984)     2076 2023-02-13 09:18:21.000000 cell-tracking-bc-2023.5/cell_tracking_BC/type/analysis.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-06 15:39:15.366917 cell-tracking-bc-2023.5/cell_tracking_BC/type/compartment/
--rw-r--r--   0 eric      (1000) users      (984)     7392 2023-01-20 15:29:49.000000 cell-tracking-bc-2023.5/cell_tracking_BC/type/compartment/base.py
--rw-r--r--   0 eric      (1000) users      (984)     6955 2023-01-20 15:39:59.000000 cell-tracking-bc-2023.5/cell_tracking_BC/type/compartment/cell.py
--rw-r--r--   0 eric      (1000) users      (984)     1632 2023-01-10 16:10:01.000000 cell-tracking-bc-2023.5/cell_tracking_BC/type/compartment/cytoplasm.py
--rw-r--r--   0 eric      (1000) users      (984)     1630 2023-01-10 16:10:01.000000 cell-tracking-bc-2023.5/cell_tracking_BC/type/compartment/nucleus.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-06 15:39:15.366917 cell-tracking-bc-2023.5/cell_tracking_BC/type/segmentation/
--rw-r--r--   0 eric      (1000) users      (984)     7207 2023-01-20 15:57:41.000000 cell-tracking-bc-2023.5/cell_tracking_BC/type/segmentation/frame.py
--rw-r--r--   0 eric      (1000) users      (984)    12053 2023-02-10 14:24:32.000000 cell-tracking-bc-2023.5/cell_tracking_BC/type/segmentation/sequence.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-06 15:39:15.343583 cell-tracking-bc-2023.5/cell_tracking_BC/type/track/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-06 15:39:15.370250 cell-tracking-bc-2023.5/cell_tracking_BC/type/track/multiple/
--rw-r--r--   0 eric      (1000) users      (984)    14463 2023-01-19 16:02:16.000000 cell-tracking-bc-2023.5/cell_tracking_BC/type/track/multiple/structured.py
--rw-r--r--   0 eric      (1000) users      (984)     2777 2023-01-17 12:16:47.000000 cell-tracking-bc-2023.5/cell_tracking_BC/type/track/multiple/unstructured.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-06 15:39:15.370250 cell-tracking-bc-2023.5/cell_tracking_BC/type/track/single/
--rw-r--r--   0 eric      (1000) users      (984)    16776 2023-02-17 09:35:42.000000 cell-tracking-bc-2023.5/cell_tracking_BC/type/track/single/forking.py
--rw-r--r--   0 eric      (1000) users      (984)    20885 2023-02-17 09:35:42.000000 cell-tracking-bc-2023.5/cell_tracking_BC/type/track/single/structured.py
--rw-r--r--   0 eric      (1000) users      (984)    10343 2023-02-17 09:35:42.000000 cell-tracking-bc-2023.5/cell_tracking_BC/type/track/single/thread.py
--rw-r--r--   0 eric      (1000) users      (984)     5380 2023-01-17 13:16:57.000000 cell-tracking-bc-2023.5/cell_tracking_BC/type/track/single/unstructured.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-03-06 15:39:15.370250 cell-tracking-bc-2023.5/cell_tracking_bc.egg-info/
--rw-r--r--   0 eric      (1000) users      (984)     3114 2023-03-06 15:39:15.000000 cell-tracking-bc-2023.5/cell_tracking_bc.egg-info/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)     4407 2023-03-06 15:39:15.000000 cell-tracking-bc-2023.5/cell_tracking_bc.egg-info/SOURCES.txt
--rw-r--r--   0 eric      (1000) users      (984)        1 2023-03-06 15:39:15.000000 cell-tracking-bc-2023.5/cell_tracking_bc.egg-info/dependency_links.txt
--rw-r--r--   0 eric      (1000) users      (984)       66 2023-03-06 15:39:15.000000 cell-tracking-bc-2023.5/cell_tracking_bc.egg-info/entry_points.txt
--rw-r--r--   0 eric      (1000) users      (984)      149 2023-03-06 15:39:15.000000 cell-tracking-bc-2023.5/cell_tracking_bc.egg-info/requires.txt
--rw-r--r--   0 eric      (1000) users      (984)       17 2023-03-06 15:39:15.000000 cell-tracking-bc-2023.5/cell_tracking_bc.egg-info/top_level.txt
--rw-r--r--   0 eric      (1000) users      (984)      104 2022-01-13 17:58:27.000000 cell-tracking-bc-2023.5/pyproject.toml
--rw-r--r--   0 eric      (1000) users      (984)       38 2023-03-06 15:39:15.370250 cell-tracking-bc-2023.5/setup.cfg
--rw-r--r--   0 eric      (1000) users      (984)     5766 2023-03-01 10:53:05.000000 cell-tracking-bc-2023.5/setup.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.903556 cell-tracking-bc-2023.6/
+-rw-r--r--   0 eric      (1000) users      (984)       61 2023-06-21 15:02:20.000000 cell-tracking-bc-2023.6/MANIFEST.in
+-rw-r--r--   0 eric      (1000) users      (984)     3114 2023-06-21 15:04:36.903556 cell-tracking-bc-2023.6/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)      636 2021-02-02 12:30:22.000000 cell-tracking-bc-2023.6/README-COPYRIGHT.txt
+-rw-r--r--   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 cell-tracking-bc-2023.6/README-LICENCE-utf8.txt
+-rw-r--r--   0 eric      (1000) users      (984)     2286 2022-02-03 09:12:09.000000 cell-tracking-bc-2023.6/README.rst
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.896889 cell-tracking-bc-2023.6/cell_tracking_BC/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.896889 cell-tracking-bc-2023.6/cell_tracking_BC/catalog/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.896889 cell-tracking-bc-2023.6/cell_tracking_BC/catalog/channel/
+-rw-r--r--   0 eric      (1000) users      (984)     1969 2023-02-13 12:56:29.000000 cell-tracking-bc-2023.6/cell_tracking_BC/catalog/channel/ratio.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.896889 cell-tracking-bc-2023.6/cell_tracking_BC/catalog/feature/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.896889 cell-tracking-bc-2023.6/cell_tracking_BC/catalog/feature/geometrical/
+-rw-r--r--   0 eric      (1000) users      (984)        0 2023-02-15 15:28:16.000000 cell-tracking-bc-2023.6/cell_tracking_BC/catalog/feature/geometrical/dummy.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.896889 cell-tracking-bc-2023.6/cell_tracking_BC/catalog/feature/radiometric/
+-rw-r--r--   0 eric      (1000) users      (984)     2574 2023-02-10 13:45:02.000000 cell-tracking-bc-2023.6/cell_tracking_BC/catalog/feature/radiometric/entropy.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.896889 cell-tracking-bc-2023.6/cell_tracking_BC/catalog/feature/set/
+-rw-r--r--   0 eric      (1000) users      (984)     2532 2023-02-10 15:24:31.000000 cell-tracking-bc-2023.6/cell_tracking_BC/catalog/feature/set/numpy_.py
+-rw-r--r--   0 eric      (1000) users      (984)     4169 2023-02-10 15:24:31.000000 cell-tracking-bc-2023.6/cell_tracking_BC/catalog/feature/set/skimage_.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.896889 cell-tracking-bc-2023.6/cell_tracking_BC/catalog/feature/temporal/
+-rw-r--r--   0 eric      (1000) users      (984)     2140 2023-02-10 15:02:24.000000 cell-tracking-bc-2023.6/cell_tracking_BC/catalog/feature/temporal/shift.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.896889 cell-tracking-bc-2023.6/cell_tracking_BC/catalog/matching/
+-rw-r--r--   0 eric      (1000) users      (984)     1985 2021-09-08 16:51:38.000000 cell-tracking-bc-2023.6/cell_tracking_BC/catalog/matching/jaccard.py
+-rw-r--r--   0 eric      (1000) users      (984)     3209 2023-02-17 09:35:42.000000 cell-tracking-bc-2023.6/cell_tracking_BC/catalog/parser.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.896889 cell-tracking-bc-2023.6/cell_tracking_BC/catalog/processing/
+-rw-r--r--   0 eric      (1000) users      (984)     3866 2023-02-10 13:53:35.000000 cell-tracking-bc-2023.6/cell_tracking_BC/catalog/processing/background.py
+-rw-r--r--   0 eric      (1000) users      (984)     1976 2023-02-10 13:53:54.000000 cell-tracking-bc-2023.6/cell_tracking_BC/catalog/processing/contrast.py
+-rw-r--r--   0 eric      (1000) users      (984)     2503 2023-02-10 13:54:29.000000 cell-tracking-bc-2023.6/cell_tracking_BC/catalog/processing/geometry.py
+-rw-r--r--   0 eric      (1000) users      (984)     2991 2023-02-10 13:55:52.000000 cell-tracking-bc-2023.6/cell_tracking_BC/catalog/processing/registration.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.896889 cell-tracking-bc-2023.6/cell_tracking_BC/catalog/segmentation/
+-rw-r--r--   0 eric      (1000) users      (984)     4782 2023-06-12 11:59:41.000000 cell-tracking-bc-2023.6/cell_tracking_BC/catalog/segmentation/tf_network.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.900223 cell-tracking-bc-2023.6/cell_tracking_BC/catalog/tracking/
+-rw-r--r--   0 eric      (1000) users      (984)     5631 2023-02-10 13:58:46.000000 cell-tracking-bc-2023.6/cell_tracking_BC/catalog/tracking/gmb_tracker.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.896889 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.900223 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/file/
+-rw-r--r--   0 eric      (1000) users      (984)    10676 2023-02-17 09:35:42.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/file/event.py
+-rw-r--r--   0 eric      (1000) users      (984)     6728 2023-02-17 09:35:42.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/file/feature.py
+-rw-r--r--   0 eric      (1000) users      (984)     4916 2023-02-17 09:35:42.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/file/path.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.900223 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/file/table/
+-rw-r--r--   0 eric      (1000) users      (984)     3076 2023-02-08 13:52:59.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/file/table/cell.py
+-rw-r--r--   0 eric      (1000) users      (984)     3480 2023-02-08 13:56:27.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/file/table/chart.py
+-rw-r--r--   0 eric      (1000) users      (984)     2388 2023-02-08 13:57:24.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/file/table/column.py
+-rw-r--r--   0 eric      (1000) users      (984)     2208 2023-02-11 18:31:12.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/file/table/sheet.py
+-rw-r--r--   0 eric      (1000) users      (984)     5734 2023-02-17 09:35:42.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/file/track.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.900223 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/
+-rw-r--r--   0 eric      (1000) users      (984)     7863 2023-01-24 09:27:19.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/annotations.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.896889 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/dbe/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.900223 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/dbe/matplotlib/
+-rw-r--r--   0 eric      (1000) users      (984)     2754 2022-02-17 13:49:51.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/dbe/matplotlib/context.py
+-rw-r--r--   0 eric      (1000) users      (984)     9151 2023-01-18 14:25:10.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/dbe/matplotlib/d_2.py
+-rw-r--r--   0 eric      (1000) users      (984)     7982 2022-07-09 12:00:34.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/dbe/matplotlib/d_3.py
+-rw-r--r--   0 eric      (1000) users      (984)     8450 2023-02-17 09:42:06.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/dbe/matplotlib/d_any.py
+-rw-r--r--   0 eric      (1000) users      (984)     6053 2022-05-31 12:24:19.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/dbe/matplotlib/event.py
+-rw-r--r--   0 eric      (1000) users      (984)     2798 2021-11-10 10:18:31.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/dbe/matplotlib/style.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.900223 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/dbe/vedo/
+-rw-r--r--   0 eric      (1000) users      (984)     1891 2022-02-01 15:12:55.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/dbe/vedo/context.py
+-rw-r--r--   0 eric      (1000) users      (984)     8915 2022-02-01 15:14:31.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/dbe/vedo/d_3.py
+-rw-r--r--   0 eric      (1000) users      (984)     5376 2022-02-23 16:34:49.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/dbe/vedo/d_any.py
+-rw-r--r--   0 eric      (1000) users      (984)     1873 2022-02-01 15:24:42.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/dbe/vedo/missing.py
+-rw-r--r--   0 eric      (1000) users      (984)     3207 2022-02-01 15:15:32.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/dbe/vedo/style.py
+-rw-r--r--   0 eric      (1000) users      (984)    14278 2023-02-17 09:35:42.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/event.py
+-rw-r--r--   0 eric      (1000) users      (984)     3736 2023-01-11 13:41:46.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/feature.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.900223 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/generic/
+-rw-r--r--   0 eric      (1000) users      (984)     4751 2023-01-18 14:26:08.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/generic/d_2.py
+-rw-r--r--   0 eric      (1000) users      (984)     4918 2023-01-11 13:38:38.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/generic/d_3.py
+-rw-r--r--   0 eric      (1000) users      (984)     2642 2023-01-20 16:01:30.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/generic/d_any.py
+-rw-r--r--   0 eric      (1000) users      (984)     4832 2023-01-17 13:23:40.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/segmentation.py
+-rw-r--r--   0 eric      (1000) users      (984)     7538 2023-01-13 14:12:23.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/sequence.py
+-rw-r--r--   0 eric      (1000) users      (984)    14093 2023-01-17 15:32:43.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/tracking.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.900223 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/
+-rw-r--r--   0 eric      (1000) users      (984)     1693 2022-01-25 19:46:56.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/annotation.py
+-rw-r--r--   0 eric      (1000) users      (984)     9774 2023-02-08 13:59:20.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/axes.py
+-rw-r--r--   0 eric      (1000) users      (984)     3564 2022-01-25 18:39:23.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/color.py
+-rw-r--r--   0 eric      (1000) users      (984)     3104 2022-02-17 13:51:26.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/context.py
+-rw-r--r--   0 eric      (1000) users      (984)    13212 2022-06-01 07:11:21.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/e_viewer_2d_t.py
+-rw-r--r--   0 eric      (1000) users      (984)     1590 2022-01-25 18:11:16.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/event.py
+-rw-r--r--   0 eric      (1000) users      (984)     3100 2022-05-31 12:20:28.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/figure.py
+-rw-r--r--   0 eric      (1000) users      (984)    12951 2023-01-20 16:01:59.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/s_drawer_2d.py
+-rw-r--r--   0 eric      (1000) users      (984)     7915 2023-01-18 14:30:43.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/s_viewer_2d.py
+-rw-r--r--   0 eric      (1000) users      (984)     3060 2022-01-26 09:00:12.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/signatures.py
+-rw-r--r--   0 eric      (1000) users      (984)     5295 2023-01-18 14:24:16.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/t_explorer_2d.py
+-rw-r--r--   0 eric      (1000) users      (984)    11377 2023-02-17 09:35:42.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/t_viewer_2d.py
+-rw-r--r--   0 eric      (1000) users      (984)     3190 2023-01-10 16:09:45.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/track.py
+-rw-r--r--   0 eric      (1000) users      (984)     1645 2022-01-26 08:45:06.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/widget.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.903556 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/text/
+-rw-r--r--   0 eric      (1000) users      (984)     1675 2021-11-25 09:11:46.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/text/dev.py
+-rw-r--r--   0 eric      (1000) users      (984)     4191 2023-02-10 15:18:51.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/text/plot.py
+-rw-r--r--   0 eric      (1000) users      (984)     4074 2022-01-25 09:33:16.000000 cell-tracking-bc-2023.6/cell_tracking_BC/in_out/text/progress.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.903556 cell-tracking-bc-2023.6/cell_tracking_BC/standard/
+-rw-r--r--   0 eric      (1000) users      (984)     2899 2023-01-13 14:44:24.000000 cell-tracking-bc-2023.6/cell_tracking_BC/standard/issue.py
+-rw-r--r--   0 eric      (1000) users      (984)     1632 2021-12-16 15:05:53.000000 cell-tracking-bc-2023.6/cell_tracking_BC/standard/number.py
+-rw-r--r--   0 eric      (1000) users      (984)     1791 2023-02-11 18:22:01.000000 cell-tracking-bc-2023.6/cell_tracking_BC/standard/path.py
+-rw-r--r--   0 eric      (1000) users      (984)     2450 2023-02-08 13:56:27.000000 cell-tracking-bc-2023.6/cell_tracking_BC/standard/uid.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.896889 cell-tracking-bc-2023.6/cell_tracking_BC/task/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.903556 cell-tracking-bc-2023.6/cell_tracking_BC/task/channel/
+-rw-r--r--   0 eric      (1000) users      (984)     1690 2023-02-10 14:28:42.000000 cell-tracking-bc-2023.6/cell_tracking_BC/task/channel/base.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.903556 cell-tracking-bc-2023.6/cell_tracking_BC/task/feature/
+-rw-r--r--   0 eric      (1000) users      (984)     2433 2023-02-10 14:12:05.000000 cell-tracking-bc-2023.6/cell_tracking_BC/task/feature/base.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.903556 cell-tracking-bc-2023.6/cell_tracking_BC/task/matching/
+-rw-r--r--   0 eric      (1000) users      (984)     6346 2023-02-17 09:35:42.000000 cell-tracking-bc-2023.6/cell_tracking_BC/task/matching/pattern.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.903556 cell-tracking-bc-2023.6/cell_tracking_BC/task/processing/
+-rw-r--r--   0 eric      (1000) users      (984)     1664 2023-02-10 11:25:18.000000 cell-tracking-bc-2023.6/cell_tracking_BC/task/processing/base.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.903556 cell-tracking-bc-2023.6/cell_tracking_BC/task/registration/
+-rw-r--r--   0 eric      (1000) users      (984)     4710 2023-02-10 11:32:54.000000 cell-tracking-bc-2023.6/cell_tracking_BC/task/registration/rigid.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.903556 cell-tracking-bc-2023.6/cell_tracking_BC/task/segmentation/
+-rw-r--r--   0 eric      (1000) users      (984)    20183 2023-02-17 09:35:42.000000 cell-tracking-bc-2023.6/cell_tracking_BC/task/segmentation/frame.py
+-rw-r--r--   0 eric      (1000) users      (984)     5269 2023-02-10 14:19:32.000000 cell-tracking-bc-2023.6/cell_tracking_BC/task/segmentation/sequence.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.903556 cell-tracking-bc-2023.6/cell_tracking_BC/task/tracking/
+-rw-r--r--   0 eric      (1000) users      (984)     6615 2023-01-13 15:07:41.000000 cell-tracking-bc-2023.6/cell_tracking_BC/task/tracking/base.py
+-rw-r--r--   0 eric      (1000) users      (984)     1647 2022-05-13 07:50:37.000000 cell-tracking-bc-2023.6/cell_tracking_BC/task/tracking/constant.py
+-rw-r--r--   0 eric      (1000) users      (984)     2399 2022-06-28 12:49:37.000000 cell-tracking-bc-2023.6/cell_tracking_BC/track_finder.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.903556 cell-tracking-bc-2023.6/cell_tracking_BC/type/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.903556 cell-tracking-bc-2023.6/cell_tracking_BC/type/acquisition/
+-rw-r--r--   0 eric      (1000) users      (984)     2006 2023-01-20 09:44:08.000000 cell-tracking-bc-2023.6/cell_tracking_BC/type/acquisition/frame.py
+-rw-r--r--   0 eric      (1000) users      (984)    12594 2023-02-17 09:35:42.000000 cell-tracking-bc-2023.6/cell_tracking_BC/type/acquisition/sequence.py
+-rw-r--r--   0 eric      (1000) users      (984)     2076 2023-02-13 09:18:21.000000 cell-tracking-bc-2023.6/cell_tracking_BC/type/analysis.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.903556 cell-tracking-bc-2023.6/cell_tracking_BC/type/compartment/
+-rw-r--r--   0 eric      (1000) users      (984)     7392 2023-01-20 15:29:49.000000 cell-tracking-bc-2023.6/cell_tracking_BC/type/compartment/base.py
+-rw-r--r--   0 eric      (1000) users      (984)     6955 2023-01-20 15:39:59.000000 cell-tracking-bc-2023.6/cell_tracking_BC/type/compartment/cell.py
+-rw-r--r--   0 eric      (1000) users      (984)     1632 2023-01-10 16:10:01.000000 cell-tracking-bc-2023.6/cell_tracking_BC/type/compartment/cytoplasm.py
+-rw-r--r--   0 eric      (1000) users      (984)     1630 2023-01-10 16:10:01.000000 cell-tracking-bc-2023.6/cell_tracking_BC/type/compartment/nucleus.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.903556 cell-tracking-bc-2023.6/cell_tracking_BC/type/segmentation/
+-rw-r--r--   0 eric      (1000) users      (984)     7207 2023-01-20 15:57:41.000000 cell-tracking-bc-2023.6/cell_tracking_BC/type/segmentation/frame.py
+-rw-r--r--   0 eric      (1000) users      (984)    12053 2023-02-10 14:24:32.000000 cell-tracking-bc-2023.6/cell_tracking_BC/type/segmentation/sequence.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.896889 cell-tracking-bc-2023.6/cell_tracking_BC/type/track/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.903556 cell-tracking-bc-2023.6/cell_tracking_BC/type/track/multiple/
+-rw-r--r--   0 eric      (1000) users      (984)    14508 2023-06-21 08:59:52.000000 cell-tracking-bc-2023.6/cell_tracking_BC/type/track/multiple/structured.py
+-rw-r--r--   0 eric      (1000) users      (984)     2777 2023-01-17 12:16:47.000000 cell-tracking-bc-2023.6/cell_tracking_BC/type/track/multiple/unstructured.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.903556 cell-tracking-bc-2023.6/cell_tracking_BC/type/track/single/
+-rw-r--r--   0 eric      (1000) users      (984)    16776 2023-02-17 09:35:42.000000 cell-tracking-bc-2023.6/cell_tracking_BC/type/track/single/forking.py
+-rw-r--r--   0 eric      (1000) users      (984)    23416 2023-06-21 13:14:27.000000 cell-tracking-bc-2023.6/cell_tracking_BC/type/track/single/structured.py
+-rw-r--r--   0 eric      (1000) users      (984)    10343 2023-02-17 09:35:42.000000 cell-tracking-bc-2023.6/cell_tracking_BC/type/track/single/thread.py
+-rw-r--r--   0 eric      (1000) users      (984)     5380 2023-01-17 13:16:57.000000 cell-tracking-bc-2023.6/cell_tracking_BC/type/track/single/unstructured.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-21 15:04:36.903556 cell-tracking-bc-2023.6/cell_tracking_bc.egg-info/
+-rw-r--r--   0 eric      (1000) users      (984)     3114 2023-06-21 15:04:36.000000 cell-tracking-bc-2023.6/cell_tracking_bc.egg-info/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)     4407 2023-06-21 15:04:36.000000 cell-tracking-bc-2023.6/cell_tracking_bc.egg-info/SOURCES.txt
+-rw-r--r--   0 eric      (1000) users      (984)        1 2023-06-21 15:04:36.000000 cell-tracking-bc-2023.6/cell_tracking_bc.egg-info/dependency_links.txt
+-rw-r--r--   0 eric      (1000) users      (984)       66 2023-06-21 15:04:36.000000 cell-tracking-bc-2023.6/cell_tracking_bc.egg-info/entry_points.txt
+-rw-r--r--   0 eric      (1000) users      (984)      149 2023-06-21 15:04:36.000000 cell-tracking-bc-2023.6/cell_tracking_bc.egg-info/requires.txt
+-rw-r--r--   0 eric      (1000) users      (984)       17 2023-06-21 15:04:36.000000 cell-tracking-bc-2023.6/cell_tracking_bc.egg-info/top_level.txt
+-rw-r--r--   0 eric      (1000) users      (984)      104 2022-01-13 17:58:27.000000 cell-tracking-bc-2023.6/pyproject.toml
+-rw-r--r--   0 eric      (1000) users      (984)       38 2023-06-21 15:04:36.903556 cell-tracking-bc-2023.6/setup.cfg
+-rw-r--r--   0 eric      (1000) users      (984)     5694 2023-06-21 15:02:38.000000 cell-tracking-bc-2023.6/setup.py
```

### Comparing `cell-tracking-bc-2023.5/PKG-INFO` & `cell-tracking-bc-2023.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cell-tracking-bc
-Version: 2023.5
+Version: 2023.6
 Summary: Base Classes for Cell Tracking in Microscopy
 Home-page: https://gitlab.inria.fr/edebreuv/cell-tracking-bc
 Author: Eric Debreuve
 Author-email: eric.debreuve@univ-cotedazur.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://gitlab.inria.fr/edebreuv/cell-tracking-bc
 Project-URL: Source, https://gitlab.inria.fr/edebreuv/cell-tracking-bc
```

### Comparing `cell-tracking-bc-2023.5/README-COPYRIGHT.txt` & `cell-tracking-bc-2023.6/README-COPYRIGHT.txt`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/README-LICENCE-utf8.txt` & `cell-tracking-bc-2023.6/README-LICENCE-utf8.txt`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/README.rst` & `cell-tracking-bc-2023.6/README.rst`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/catalog/channel/ratio.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/catalog/channel/ratio.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/catalog/feature/radiometric/entropy.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/catalog/feature/radiometric/entropy.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/catalog/feature/set/numpy_.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/catalog/feature/set/numpy_.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/catalog/feature/set/skimage_.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/catalog/feature/set/skimage_.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/catalog/feature/temporal/shift.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/catalog/feature/temporal/shift.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/catalog/matching/jaccard.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/catalog/matching/jaccard.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/catalog/parser.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/catalog/parser.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/catalog/processing/background.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/catalog/processing/background.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/catalog/processing/contrast.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/catalog/processing/contrast.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/catalog/processing/geometry.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/catalog/processing/geometry.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/catalog/processing/registration.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/catalog/processing/registration.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/catalog/segmentation/tf_network.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/catalog/segmentation/tf_network.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,18 +32,18 @@
 from pathlib import Path as path_t
 from typing import Sequence, Tuple, Union
 
 import numpy as nmpy
 import tensorflow as tsfl
 import tensorflow.keras.models as modl
 import tensorrt as tsrt
-
+from config.unet import UNetInstance
 from logger_36 import LOGGER
-from cell_tracking_BC.task.processing.base import processing_h
 
+from cell_tracking_BC.task.processing.base import processing_h
 
 array_t = nmpy.ndarray
 
 
 def InputSizeOfTFNetwork(
     network_path: Union[str, path_t],
     /,
@@ -80,15 +80,18 @@
     if PostProcessed is None:
         PostProcessed = lambda _prm: _prm
 
     frames = nmpy.array(frames, dtype=nmpy.float32)
     if frames.ndim == 3:
         frames = nmpy.expand_dims(frames, axis=3)
 
-    network = modl.load_model(network_path)
+    if network_path.suffix.lower() == ".h5":
+        network = UNetInstance(*frames.shape[1:], network_path)
+    else:
+        network = modl.load_model(network_path)
     # network.summary()
     predictions = network.predict(frames, verbose=1)
     # First dimension is time (needs to be removed for single frame reshape below), last dimension is channels
     # (equal to one, thus removed).
     shape = network.layers[0].input_shape[0][1:-1]
 
     for t_idx, prediction in enumerate(predictions):
@@ -105,12 +108,15 @@
 
 
 def LogTensorflowDetailsDetails() -> None:
     """"""
     system_details = tsfl.sysconfig.get_build_info()
     LOGGER.info(
         f"TENSORFLOW DETAILS\n"
-        f"    Tensorflow: {tsfl.version.VERSION}\n"
-        f"      TensorRT: {tsrt.__version__}\n"
-        f"          Cuda: {system_details['cuda_version']}\n"
-        f"         CuDNN: {system_details['cudnn_version']}"
+        f"          Tensorflow: {tsfl.version.VERSION}\n"
+        f"    Tensorflow Build: {tsfl.sysconfig.get_build_info()}\n"
+        f"            TensorRT: {tsrt.__version__}\n"
+        f"                Cuda: {system_details['cuda_version']}\n"
+        f"               CuDNN: {system_details['cudnn_version']}\n"
+        f"                CPUs: {tsfl.config.list_physical_devices('CPU')}\n"
+        f"                GPUs: {tsfl.config.list_physical_devices('GPU')}"
     )
```

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/catalog/tracking/gmb_tracker.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/catalog/tracking/gmb_tracker.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/in_out/file/event.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/file/event.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/in_out/file/feature.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/file/feature.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/in_out/file/path.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/file/path.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/in_out/file/table/cell.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/file/table/cell.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/in_out/file/table/chart.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/file/table/chart.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/in_out/file/table/column.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/file/table/column.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/in_out/file/table/sheet.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/file/table/sheet.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/in_out/file/track.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/file/track.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/annotations.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/annotations.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/dbe/matplotlib/context.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/dbe/matplotlib/context.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/dbe/matplotlib/d_2.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/dbe/matplotlib/d_2.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/dbe/matplotlib/d_3.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/dbe/matplotlib/d_3.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/dbe/matplotlib/d_any.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/dbe/matplotlib/d_any.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/dbe/matplotlib/event.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/dbe/matplotlib/event.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/dbe/matplotlib/style.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/dbe/matplotlib/style.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/dbe/vedo/context.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/dbe/vedo/context.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/dbe/vedo/d_3.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/dbe/vedo/d_3.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/dbe/vedo/d_any.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/dbe/vedo/d_any.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/dbe/vedo/missing.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/dbe/vedo/missing.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/dbe/vedo/style.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/dbe/vedo/style.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/event.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/event.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/feature.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/feature.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/generic/d_2.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/generic/d_2.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/generic/d_3.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/generic/d_3.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/generic/d_any.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/generic/d_any.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/segmentation.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/segmentation.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/sequence.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/sequence.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/tracking.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/tracking.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/type/annotation.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/annotation.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/type/axes.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/axes.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/type/color.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/color.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/type/context.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/context.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/type/e_viewer_2d_t.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/e_viewer_2d_t.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/type/event.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/event.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/type/figure.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/figure.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/type/s_drawer_2d.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/s_drawer_2d.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/type/s_viewer_2d.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/s_viewer_2d.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/type/signatures.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/signatures.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/type/t_explorer_2d.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/t_explorer_2d.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/type/t_viewer_2d.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/t_viewer_2d.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/type/track.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/track.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/in_out/graphics/type/widget.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/graphics/type/widget.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/in_out/text/dev.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/text/dev.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/in_out/text/plot.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/text/plot.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/in_out/text/progress.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/in_out/text/progress.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/standard/issue.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/standard/issue.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/standard/number.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/standard/number.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/standard/path.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/standard/path.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/standard/uid.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/standard/uid.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/task/channel/base.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/task/channel/base.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/task/feature/base.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/task/feature/base.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/task/matching/pattern.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/task/matching/pattern.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/task/processing/base.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/task/processing/base.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/task/registration/rigid.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/task/registration/rigid.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/task/segmentation/frame.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/task/segmentation/frame.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/task/segmentation/sequence.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/task/segmentation/sequence.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/task/tracking/base.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/task/tracking/base.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/task/tracking/constant.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/task/tracking/constant.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/track_finder.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/track_finder.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/type/acquisition/frame.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/type/acquisition/frame.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/type/acquisition/sequence.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/type/acquisition/sequence.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/type/analysis.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/type/analysis.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/type/compartment/base.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/type/compartment/base.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/type/compartment/cell.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/type/compartment/cell.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/type/compartment/cytoplasm.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/type/compartment/cytoplasm.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/type/compartment/nucleus.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/type/compartment/nucleus.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/type/segmentation/frame.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/type/segmentation/frame.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/type/segmentation/sequence.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/type/segmentation/sequence.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/type/track/multiple/structured.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/type/track/multiple/structured.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,28 +203,30 @@
         return output
 
     def MarkDeadCells(
         self,
         death_responses: Dict[int, Optional[Sequence[float]]],
         lower_bound: float,
         after_divisions: bool,
+        method: str,
         /,
         *,
         CombinedResponse: Callable[[Iterable], float] = max,
     ) -> None:
         """
         A death is set if the highest response at a cell among the adjacent threads is above the threshold.
         """
         t_idx = 0
         while t_idx < self.__len__():
             track = self[t_idx]
             fully_pruned = track.MarkDeadCells(
                 death_responses,
                 lower_bound,
                 after_divisions,
+                method,
                 CombinedResponse=CombinedResponse,
                 called_from_educated_code=True,
             )
             if fully_pruned:
                 self.fully_pruned.append(track)
                 del self[t_idx]
             else:
```

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/type/track/multiple/unstructured.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/type/track/multiple/unstructured.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/type/track/single/forking.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/type/track/single/forking.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/type/track/single/structured.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/type/track/single/structured.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     Optional,
     Sequence,
     Tuple,
     Union,
 )
 
 import networkx as grph
+import numpy as nmpy
 
 from logger_36 import LOGGER
 from cell_tracking_BC.standard.issue import ISSUE_SEPARATOR
 from cell_tracking_BC.standard.number import INFINITY_MINUS, MAX_INT
 from cell_tracking_BC.standard.uid import Identity
 from cell_tracking_BC.type.compartment.cell import cell_t, state_e
 
@@ -167,14 +168,15 @@
         return {}  # Used to be (-1,), then None
 
     def MarkDeadCells(
         self,
         death_responses: Dict[int, Optional[Sequence[float]]],
         lower_bound: float,
         after_divisions: bool,
+        method: str,
         /,
         *,
         CombinedResponse: Callable[[Iterable], float] = max,
         called_from_educated_code: bool = False,
     ) -> bool:
         """
         A death is set if the highest response at a cell among the adjacent threads is above the threshold.
@@ -208,44 +210,93 @@
             return False
 
         if after_divisions:
             dividing_cells = self.DividingCells()
         else:
             dividing_cells = ()
 
-        # This loop must not prune cells or modify leaves since it could change the sibling labels to labels of leaves
-        # that have been pruned in a prior step (e.g. when validating divisions). For example, behind a cell are 2
-        # leaves with labels 1 and 2. Suppose that the leaf with label 1 has been pruned in a prior step. So the cell
-        # has 2 as its sibling labels. So has the cell before it. If the cell is marked dead, and the leaf with label 2
-        # is pruned, the previous cell will now receive the label min(1,2), which is different from what it had.
-        dead_cells = []
-        if isinstance(self, list):
-            cells = self
+        sibling_labels = self.TrackLabelsContainingCell(self.root)
+        sibling_responses = {}
+        for label in sibling_labels:
+            if death_responses[label] is None:
+                sibling_responses[label] = nmpy.array(
+                    [lower_bound - 1.0], dtype=nmpy.float64
+                )
+            else:
+                sibling_responses[label] = nmpy.array(
+                    death_responses[label], dtype=nmpy.float64
+                )
+        # TODO: Use the above variable of "first above" also.
+        # TODO: Note that global max and first max ignore the CombinedResponse option.
+        if method == "global max":
+            where_maxes = {}
+            for label, sibling_response in sibling_responses.items():
+                where_max = nmpy.nonzero(
+                    sibling_response == nmpy.amax(sibling_response)
+                )[0][0]
+                if sibling_response[where_max] >= lower_bound:
+                    where_maxes[label] = where_max
+        elif method == "first max":
+            where_maxes = {}
+            for label, sibling_response in sibling_responses.items():
+                where_above = nmpy.nonzero(sibling_response >= lower_bound)[0]
+                if where_above.size == 0:
+                    continue
+                where_above = where_above[0]
+                while (where_above + 1 < sibling_response.size) and (
+                    sibling_response[where_above + 1] >= sibling_response[where_above]
+                ):
+                    where_above += 1
+                where_maxes[label] = where_above
         else:
-            cells = grph.dfs_preorder_nodes(self, source=self.topologic_root)
-        for cell in cells:
-            if cell.state in (state_e.dividing, state_e.discarded):
-                continue
-            if after_divisions and any(
-                self.ConfirmCellLineage(cell, _dvd) for _dvd in dividing_cells
-            ):
-                continue
-
-            time_point = self.CellTimePoint(cell)
-            sibling_labels = self.TrackLabelsContainingCell(cell)
-            combined = CombinedResponse(
-                death_responses[_lbl][time_point]
-                if (death_responses[_lbl] is not None)
-                and (death_responses[_lbl][time_point] is not None)
-                else INFINITY_MINUS
-                for _lbl in sibling_labels
-            )
-            if combined >= lower_bound:
-                # Note: The cell can be a leaf (see new_leaves below)
-                dead_cells.append(cell)
+            where_maxes = None
+        if method in ("global max", "first max"):
+            dead_cells = []
+            # Threads must be iterated over in topologic mode since death responses cover the whole cell range.
+            for thread, label in self.LabeledThreadIterator(topologic_mode=True):
+                if label in where_maxes:
+                    cell = thread[where_maxes[label]]
+                    if after_divisions and any(
+                        self.ConfirmCellLineage(cell, _dvd) for _dvd in dividing_cells
+                    ):
+                        continue
+                    dead_cells.append(cell)
+        elif method == "first above":
+            # This loop must not prune cells or modify leaves since it could change the sibling labels to labels of leaves
+            # that have been pruned in a prior step (e.g. when validating divisions). For example, behind a cell are 2
+            # leaves with labels 1 and 2. Suppose that the leaf with label 1 has been pruned in a prior step. So the cell
+            # has 2 as its sibling labels. So has the cell before it. If the cell is marked dead, and the leaf with label 2
+            # is pruned, the previous cell will now receive the label min(1,2), which is different from what it had.
+            dead_cells = []
+            if isinstance(self, list):
+                cells = self
+            else:
+                cells = grph.dfs_preorder_nodes(self, source=self.topologic_root)
+            for cell in cells:
+                if cell.state in (state_e.dividing, state_e.discarded):
+                    continue
+                if after_divisions and any(
+                    self.ConfirmCellLineage(cell, _dvd) for _dvd in dividing_cells
+                ):
+                    continue
+
+                time_point = self.CellTimePoint(cell)
+                sibling_labels = self.TrackLabelsContainingCell(cell)
+                combined = CombinedResponse(
+                    death_responses[_lbl][time_point]
+                    if (death_responses[_lbl] is not None)
+                    and (death_responses[_lbl][time_point] is not None)
+                    else INFINITY_MINUS
+                    for _lbl in sibling_labels
+                )
+                if combined >= lower_bound:
+                    # Note: The cell can be a leaf (see new_leaves below)
+                    dead_cells.append(cell)
+        else:
+            raise ValueError(f"{method}: Invalid method for marking dead cells.")
 
         # Do not log inside the loop on dead_cells since it does not update leaves (update is done after the loop),
         # leaving the track in a transient state not suitable for TrackLabelsContainingCell.
         summary = {}
         max_duration = max(self.durations)
         for cell in dead_cells:
             labels = self.TrackLabelsContainingCell(cell)
```

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/type/track/single/thread.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/type/track/single/thread.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_BC/type/track/single/unstructured.py` & `cell-tracking-bc-2023.6/cell_tracking_BC/type/track/single/unstructured.py`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/cell_tracking_bc.egg-info/PKG-INFO` & `cell-tracking-bc-2023.6/cell_tracking_bc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cell-tracking-bc
-Version: 2023.5
+Version: 2023.6
 Summary: Base Classes for Cell Tracking in Microscopy
 Home-page: https://gitlab.inria.fr/edebreuv/cell-tracking-bc
 Author: Eric Debreuve
 Author-email: eric.debreuve@univ-cotedazur.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://gitlab.inria.fr/edebreuv/cell-tracking-bc
 Project-URL: Source, https://gitlab.inria.fr/edebreuv/cell-tracking-bc
```

### Comparing `cell-tracking-bc-2023.5/cell_tracking_bc.egg-info/SOURCES.txt` & `cell-tracking-bc-2023.6/cell_tracking_bc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cell-tracking-bc-2023.5/setup.py` & `cell-tracking-bc-2023.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 
 AUTHOR = "Eric Debreuve"
 E_MAIL = "eric.debreuve@univ-cotedazur.fr"
 
 PYPI_NAME = "cell-tracking-bc"
 DESCRIPTION = "Base Classes for Cell Tracking in Microscopy"
-VERSION = (2023, 5)  # /!\ str(2021.10) -> "2021.1"
+version = "2023.6"
 PY_VERSION = "3.8"
 
 REPOSITORY_NAME = "cell-tracking-bc"
 REPOSITORY_USER = "edebreuv"
 REPOSITORY_SITE = "gitlab.inria.fr"
 DOCUMENTATION_SITE = f"{REPOSITORY_USER}.gitlabpages.inria.fr"
 
@@ -91,15 +91,14 @@
 
 HERE = Path(__file__).parent.resolve()
 
 
 long_description = (HERE / "README.rst").read_text(encoding="utf-8")
 repository_url = f"https://{REPOSITORY_SITE}/{REPOSITORY_USER}/{REPOSITORY_NAME}"
 documentation_url = repository_url
-version = f"{VERSION[0]}.{VERSION[1]}"
 
 folders = [IMPORT_NAME]
 for node in (HERE / IMPORT_NAME).rglob("*"):
     if node.is_dir():
         node = node.relative_to(HERE)
         node = ".".join(node.parts)
         folders.append(node)
```

