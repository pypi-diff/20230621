# Comparing `tmp/vedo-2023.4.5.tar.gz` & `tmp/vedo-2023.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vedo-2023.4.5.tar", last modified: Sun Jun 18 15:36:43 2023, max compression
+gzip compressed data, was "vedo-2023.4.6.tar", last modified: Wed Jun 21 17:43:43 2023, max compression
```

## Comparing `vedo-2023.4.5.tar` & `vedo-2023.4.6.tar`

### file list

```diff
@@ -1,458 +1,459 @@
-drwxr-x---   0 musy      (8766) sharpe    (4311)        0 2023-06-18 15:36:43.424368 vedo-2023.4.5/
--rw-r-----   0 musy      (8766) sharpe    (4311)     7617 2022-03-01 14:15:57.000000 vedo-2023.4.5/FONT.LICENSE
--rw-r--r--   0 musy      (8766) sharpe    (4311)     1067 2022-02-27 13:43:39.000000 vedo-2023.4.5/LICENSE
--rw-r--r--   0 musy      (8766) sharpe    (4311)      267 2022-03-01 12:22:11.000000 vedo-2023.4.5/MANIFEST.in
--rw-r-----   0 musy      (8766) sharpe    (4311)     1249 2023-06-18 15:36:43.424368 vedo-2023.4.5/PKG-INFO
--rw-rw-r--   0 musy      (8766) sharpe    (4311)    10862 2023-06-02 16:59:49.000000 vedo-2023.4.5/README.md
-drwxr-x---   0 musy      (8766) sharpe    (4311)        0 2023-06-18 15:36:43.376367 vedo-2023.4.5/examples/
-drwxr-x---   0 musy      (8766) sharpe    (4311)        0 2023-06-18 15:36:43.380367 vedo-2023.4.5/examples/advanced/
--rw-rw-r--   0 musy      (8766) sharpe    (4311)        3 2021-03-06 18:50:54.000000 vedo-2023.4.5/examples/advanced/__init__.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1467 2023-02-02 17:56:11.000000 vedo-2023.4.5/examples/advanced/capping_mesh.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      559 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/advanced/contours2mesh.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      281 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/advanced/convex_hull.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      422 2023-02-03 19:31:48.000000 vedo-2023.4.5/examples/advanced/cut_and_cap.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      582 2023-02-17 17:24:05.000000 vedo-2023.4.5/examples/advanced/cut_with_mesh1.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      440 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/advanced/cut_with_points1.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      498 2023-06-18 13:10:42.000000 vedo-2023.4.5/examples/advanced/cut_with_points2.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      941 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/advanced/fitline.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      683 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/advanced/fitplanes.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      949 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/advanced/fitspheres1.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      972 2023-02-17 17:16:26.000000 vedo-2023.4.5/examples/advanced/fitspheres2.py
--rw-rw-r--   0 musy      (8766) sharpe    (4311)      546 2022-02-25 12:03:56.000000 vedo-2023.4.5/examples/advanced/geodesic.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     5443 2022-11-06 15:19:38.000000 vedo-2023.4.5/examples/advanced/geological_model.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      824 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/advanced/gyroid.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     2153 2023-06-18 13:14:58.000000 vedo-2023.4.5/examples/advanced/interpolate_field.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      672 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/advanced/interpolate_scalar1.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1129 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/advanced/interpolate_scalar2.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      680 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/advanced/interpolate_scalar3.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      996 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/advanced/interpolate_scalar4.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      680 2023-01-20 17:20:50.000000 vedo-2023.4.5/examples/advanced/line2mesh_quads.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      731 2023-01-20 17:20:32.000000 vedo-2023.4.5/examples/advanced/line2mesh_tri.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1416 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/advanced/measure_curvature.py
--rw-rw-r--   0 musy      (8766) sharpe    (4311)      461 2022-12-07 17:35:32.000000 vedo-2023.4.5/examples/advanced/mesh_smoother1.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      536 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/advanced/mesh_smoother2.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1074 2023-02-17 14:59:48.000000 vedo-2023.4.5/examples/advanced/meshquality.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      919 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/advanced/moving_least_squares1D.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1676 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/advanced/moving_least_squares2D.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     2182 2023-03-23 11:00:46.000000 vedo-2023.4.5/examples/advanced/multi_viewer2.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1123 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/advanced/recosurface.py
--rwxr-x---   0 musy      (8766) sharpe    (4311)      347 2022-11-14 13:08:27.000000 vedo-2023.4.5/examples/advanced/run_all.sh
--rw-r-----   0 musy      (8766) sharpe    (4311)      395 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/advanced/skeletonize.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     2197 2023-03-23 11:07:23.000000 vedo-2023.4.5/examples/advanced/spline_draw.py
--rw-rw-r--   0 musy      (8766) sharpe    (4311)      316 2022-02-25 12:11:18.000000 vedo-2023.4.5/examples/advanced/splitmesh.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      333 2023-03-14 16:58:51.000000 vedo-2023.4.5/examples/advanced/timer_callback0.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1232 2023-04-13 17:24:04.000000 vedo-2023.4.5/examples/advanced/timer_callback1.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     2299 2023-02-17 15:55:08.000000 vedo-2023.4.5/examples/advanced/timer_callback2.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1708 2023-04-13 17:20:56.000000 vedo-2023.4.5/examples/advanced/timer_callback3.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      526 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/advanced/voronoi2.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      990 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/advanced/warp1.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      887 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/advanced/warp2.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     3663 2023-01-07 21:26:46.000000 vedo-2023.4.5/examples/advanced/warp3.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     6776 2023-03-23 11:06:49.000000 vedo-2023.4.5/examples/advanced/warp4.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     4991 2023-01-07 21:26:46.000000 vedo-2023.4.5/examples/advanced/warp5.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1033 2023-04-03 14:27:35.000000 vedo-2023.4.5/examples/advanced/warp6.py
-drwxr-x---   0 musy      (8766) sharpe    (4311)        0 2023-06-18 15:36:43.388367 vedo-2023.4.5/examples/basic/
--rw-r-----   0 musy      (8766) sharpe    (4311)      682 2023-03-14 19:19:18.000000 vedo-2023.4.5/examples/basic/.vedo_pipeline_graphviz
--rw-r-----   0 musy      (8766) sharpe    (4311)    19278 2023-03-14 19:19:18.000000 vedo-2023.4.5/examples/basic/.vedo_pipeline_graphviz.pdf
--rw-r-----   0 musy      (8766) sharpe    (4311)     2518 2023-06-18 15:14:33.000000 vedo-2023.4.5/examples/basic/.vedo_recorded_events.log
--rw-rw-r--   0 musy      (8766) sharpe    (4311)        3 2021-03-06 18:56:56.000000 vedo-2023.4.5/examples/basic/__init__.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      838 2023-04-13 17:38:35.000000 vedo-2023.4.5/examples/basic/align1.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1027 2023-04-13 17:44:46.000000 vedo-2023.4.5/examples/basic/align2.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1164 2023-04-13 17:57:24.000000 vedo-2023.4.5/examples/basic/align3.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1079 2023-04-13 18:00:42.000000 vedo-2023.4.5/examples/basic/align4.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1148 2023-04-13 18:02:59.000000 vedo-2023.4.5/examples/basic/align5.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      883 2023-04-13 18:05:19.000000 vedo-2023.4.5/examples/basic/align6.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      849 2023-04-13 18:11:41.000000 vedo-2023.4.5/examples/basic/background_image.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1377 2023-04-13 18:14:10.000000 vedo-2023.4.5/examples/basic/boolean.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      719 2023-04-13 18:16:55.000000 vedo-2023.4.5/examples/basic/boundaries.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      782 2023-04-13 18:19:56.000000 vedo-2023.4.5/examples/basic/buildmesh.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1204 2023-04-13 18:22:38.000000 vedo-2023.4.5/examples/basic/buttons.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1495 2023-04-13 18:26:44.000000 vedo-2023.4.5/examples/basic/cartoony.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      731 2023-04-13 18:28:57.000000 vedo-2023.4.5/examples/basic/cells_within_bounds.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1322 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/basic/closewindow.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      931 2023-04-13 18:30:21.000000 vedo-2023.4.5/examples/basic/clustering.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      688 2023-04-13 18:38:32.000000 vedo-2023.4.5/examples/basic/color_mesh_cells1.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      768 2023-04-13 18:40:16.000000 vedo-2023.4.5/examples/basic/color_mesh_cells2.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1680 2023-04-13 18:32:30.000000 vedo-2023.4.5/examples/basic/colorcubes.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1322 2023-04-13 18:34:38.000000 vedo-2023.4.5/examples/basic/colorlines.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1213 2023-04-13 18:36:50.000000 vedo-2023.4.5/examples/basic/colormap_list.py
--rw-rw-r--   0 musy      (8766) sharpe    (4311)      703 2023-02-17 15:06:20.000000 vedo-2023.4.5/examples/basic/colormaps.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      709 2023-04-13 18:42:02.000000 vedo-2023.4.5/examples/basic/connected_vtx.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     2847 2023-04-17 09:34:03.000000 vedo-2023.4.5/examples/basic/cut_freehand.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      630 2023-06-15 12:11:15.000000 vedo-2023.4.5/examples/basic/cut_interactive.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      772 2023-04-13 18:49:28.000000 vedo-2023.4.5/examples/basic/delaunay2d.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1003 2023-04-13 18:51:43.000000 vedo-2023.4.5/examples/basic/delete_mesh_pts.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      678 2023-04-13 18:53:42.000000 vedo-2023.4.5/examples/basic/distance2mesh.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      574 2023-04-13 18:55:44.000000 vedo-2023.4.5/examples/basic/extrude.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      380 2023-04-13 18:57:36.000000 vedo-2023.4.5/examples/basic/fillholes.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      418 2023-04-13 18:58:26.000000 vedo-2023.4.5/examples/basic/flatarrow.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1058 2023-04-13 19:01:49.000000 vedo-2023.4.5/examples/basic/glyphs1.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1415 2023-04-13 19:03:46.000000 vedo-2023.4.5/examples/basic/glyphs_arrows.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      765 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/basic/hover_legend.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1103 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/basic/input_box.py
--rw-rw-r--   0 musy      (8766) sharpe    (4311)      523 2023-04-05 18:39:17.000000 vedo-2023.4.5/examples/basic/interaction_modes.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      810 2023-03-23 11:19:03.000000 vedo-2023.4.5/examples/basic/keypress.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      435 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/basic/largestregion.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      623 2022-12-07 16:21:23.000000 vedo-2023.4.5/examples/basic/legendbox.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      359 2022-03-17 20:05:40.000000 vedo-2023.4.5/examples/basic/lightings.py
--rw-rw-r--   0 musy      (8766) sharpe    (4311)      799 2021-05-04 16:06:12.000000 vedo-2023.4.5/examples/basic/lights.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      651 2022-10-23 14:51:55.000000 vedo-2023.4.5/examples/basic/lin_interpolate.py
--rw-rw-r--   0 musy      (8766) sharpe    (4311)      463 2023-04-27 17:09:43.000000 vedo-2023.4.5/examples/basic/manypoints.py
--rw-rw-r--   0 musy      (8766) sharpe    (4311)      684 2022-06-06 19:09:50.000000 vedo-2023.4.5/examples/basic/manyspheres.py
--rw-rw-r--   0 musy      (8766) sharpe    (4311)      531 2021-09-08 14:00:59.000000 vedo-2023.4.5/examples/basic/mesh_alphas.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1133 2023-05-28 11:38:19.000000 vedo-2023.4.5/examples/basic/mesh_coloring.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      957 2023-02-17 17:32:23.000000 vedo-2023.4.5/examples/basic/mesh_custom.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1374 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/basic/mesh_lut.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      683 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/basic/mesh_map2cell.py
--rw-rw-r--   0 musy      (8766) sharpe    (4311)     1537 2021-03-06 18:56:56.000000 vedo-2023.4.5/examples/basic/mesh_merge_vs_assembly.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      356 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/basic/mesh_modify.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      545 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/basic/mesh_sharemap.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      548 2023-02-17 15:02:14.000000 vedo-2023.4.5/examples/basic/mesh_threshold.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      323 2023-02-02 21:20:57.000000 vedo-2023.4.5/examples/basic/mirror.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      813 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/basic/mouseclick.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      705 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/basic/mousehighlight.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      766 2023-02-27 11:30:28.000000 vedo-2023.4.5/examples/basic/mousehover0.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1460 2023-03-23 11:21:41.000000 vedo-2023.4.5/examples/basic/mousehover1.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      805 2023-03-23 11:22:10.000000 vedo-2023.4.5/examples/basic/mousehover2.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1300 2023-03-23 11:23:21.000000 vedo-2023.4.5/examples/basic/mousehover3.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1110 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/basic/multirenderers.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1523 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/basic/multiwindows1.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      839 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/basic/multiwindows2.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      563 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/basic/pca_ellipse.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1336 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/basic/pca_ellipsoid.py
--rw-rw-r--   0 musy      (8766) sharpe    (4311)      495 2022-01-27 19:58:01.000000 vedo-2023.4.5/examples/basic/record_play.py
--rw-rw-r--   0 musy      (8766) sharpe    (4311)      532 2022-03-19 14:51:42.000000 vedo-2023.4.5/examples/basic/ribbon.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      388 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/basic/rotate_image.py
--rwxr-x---   0 musy      (8766) sharpe    (4311)      182 2023-01-18 12:46:24.000000 vedo-2023.4.5/examples/basic/run_all.sh
--rw-r-----   0 musy      (8766) sharpe    (4311)      859 2023-05-28 11:39:11.000000 vedo-2023.4.5/examples/basic/scalarbars.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      353 2023-05-26 16:18:15.000000 vedo-2023.4.5/examples/basic/shadow1.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      564 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/basic/shadow2.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      505 2023-01-09 14:44:11.000000 vedo-2023.4.5/examples/basic/shadow3.py
--rw-rw-r--   0 musy      (8766) sharpe    (4311)      207 2021-05-04 16:06:12.000000 vedo-2023.4.5/examples/basic/shrink.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      478 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/basic/silhouette1.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1561 2023-02-16 17:23:28.000000 vedo-2023.4.5/examples/basic/silhouette2.py
--rw-rw-r--   0 musy      (8766) sharpe    (4311)      349 2022-02-24 21:54:41.000000 vedo-2023.4.5/examples/basic/silhouette3.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      474 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/basic/skybox.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      971 2023-03-23 11:24:13.000000 vedo-2023.4.5/examples/basic/slider_browser.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      614 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/basic/sliders1.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1432 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/basic/sliders2.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      513 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/basic/sliders3d.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1661 2023-02-17 15:13:17.000000 vedo-2023.4.5/examples/basic/sliders_hsv.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      897 2023-04-05 13:32:34.000000 vedo-2023.4.5/examples/basic/sliders_range.py
--rw-rw-r--   0 musy      (8766) sharpe    (4311)      649 2022-01-27 20:22:57.000000 vedo-2023.4.5/examples/basic/specular.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      667 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/basic/spline_tool.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      536 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/basic/ssao.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      348 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/basic/surf_intersect.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      776 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/basic/texture_coords.py
--rw-rw-r--   0 musy      (8766) sharpe    (4311)      504 2022-06-06 19:09:50.000000 vedo-2023.4.5/examples/basic/texturecubes.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      773 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/basic/tube_radii.py
--rw-rw-r--   0 musy      (8766) sharpe    (4311)      429 2022-10-18 18:03:39.000000 vedo-2023.4.5/examples/basic/voronoi1.py
-drwxr-x---   0 musy      (8766) sharpe    (4311)        0 2023-06-18 15:36:43.392367 vedo-2023.4.5/examples/other/
--rw-rw-r--   0 musy      (8766) sharpe    (4311)        5 2022-06-06 19:09:50.000000 vedo-2023.4.5/examples/other/__init__.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      669 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/other/clone2d.py
-drwxr-x---   0 musy      (8766) sharpe    (4311)        0 2023-06-18 15:36:43.400367 vedo-2023.4.5/examples/other/dolfin/
--rw-r-----   0 musy      (8766) sharpe    (4311)      504 2023-02-03 17:02:08.000000 vedo-2023.4.5/examples/other/dolfin/README.md
--rw-rw-r--   0 musy      (8766) sharpe    (4311)        3 2021-03-06 19:00:03.000000 vedo-2023.4.5/examples/other/dolfin/__init__.py
--rw-r--r--   0 musy      (8766) sharpe    (4311)      446 2021-03-06 19:00:03.000000 vedo-2023.4.5/examples/other/dolfin/ascalarbar.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     3266 2023-01-27 15:42:02.000000 vedo-2023.4.5/examples/other/dolfin/awefem.py
--rw-r--r--   0 musy      (8766) sharpe    (4311)     1135 2021-03-06 19:00:03.000000 vedo-2023.4.5/examples/other/dolfin/calc_surface_area.py
--rw-r--r--   0 musy      (8766) sharpe    (4311)     1072 2021-03-06 19:00:03.000000 vedo-2023.4.5/examples/other/dolfin/collisions.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1024 2023-01-27 15:42:02.000000 vedo-2023.4.5/examples/other/dolfin/demo_eigenvalue.py
--rw-r--r--   0 musy      (8766) sharpe    (4311)     1035 2021-03-06 19:00:03.000000 vedo-2023.4.5/examples/other/dolfin/demo_submesh.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1845 2023-01-27 15:42:02.000000 vedo-2023.4.5/examples/other/dolfin/elasticbeam.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     6528 2023-01-27 15:42:02.000000 vedo-2023.4.5/examples/other/dolfin/elastodynamics.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1385 2022-05-08 22:18:28.000000 vedo-2023.4.5/examples/other/dolfin/ex03_poisson.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1977 2023-01-27 15:42:02.000000 vedo-2023.4.5/examples/other/dolfin/ex04_mixed-poisson.py
--rw-r--r--   0 musy      (8766) sharpe    (4311)     1575 2021-03-06 19:00:03.000000 vedo-2023.4.5/examples/other/dolfin/ex06_elasticity1.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1064 2023-03-14 18:26:09.000000 vedo-2023.4.5/examples/other/dolfin/ex06_elasticity2.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     3431 2023-01-20 17:19:50.000000 vedo-2023.4.5/examples/other/dolfin/ex06_elasticity3.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     2415 2023-03-02 20:08:18.000000 vedo-2023.4.5/examples/other/dolfin/ex06_elasticity4.py
--rw-r--r--   0 musy      (8766) sharpe    (4311)     2070 2022-05-08 22:20:34.000000 vedo-2023.4.5/examples/other/dolfin/ex07_stokes-iterative.py
--rw-r--r--   0 musy      (8766) sharpe    (4311)     1580 2021-03-06 19:00:03.000000 vedo-2023.4.5/examples/other/dolfin/ft02_poisson_membrane.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1537 2022-03-17 20:16:09.000000 vedo-2023.4.5/examples/other/dolfin/ft04_heat_gaussian.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     2943 2023-01-27 15:42:02.000000 vedo-2023.4.5/examples/other/dolfin/ft09_reaction_system.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     2622 2023-01-27 15:42:02.000000 vedo-2023.4.5/examples/other/dolfin/heatconv.py
--rw-r--r--   0 musy      (8766) sharpe    (4311)     2916 2021-03-06 19:00:03.000000 vedo-2023.4.5/examples/other/dolfin/magnetostatics.py
--rw-r--r--   0 musy      (8766) sharpe    (4311)      455 2021-03-06 19:00:03.000000 vedo-2023.4.5/examples/other/dolfin/markmesh.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     2899 2023-01-27 15:42:02.000000 vedo-2023.4.5/examples/other/dolfin/navier-stokes_lshape.py
--rw-r--r--   0 musy      (8766) sharpe    (4311)      462 2021-03-06 19:00:03.000000 vedo-2023.4.5/examples/other/dolfin/nodal_u.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      630 2023-01-27 15:42:02.000000 vedo-2023.4.5/examples/other/dolfin/pi_estimate.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1532 2023-01-27 15:42:02.000000 vedo-2023.4.5/examples/other/dolfin/pointLoad.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1120 2023-01-27 15:42:02.000000 vedo-2023.4.5/examples/other/dolfin/read_image.py
--rwxr-xr-x   0 musy      (8766) sharpe    (4311)     2130 2022-04-05 19:56:37.000000 vedo-2023.4.5/examples/other/dolfin/run_all.sh
--rw-r-----   0 musy      (8766) sharpe    (4311)      670 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/other/dolfin/scalemesh.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     2549 2023-01-27 15:42:02.000000 vedo-2023.4.5/examples/other/dolfin/stokes1.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1246 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/other/dolfin/stokes2.py
--rw-r--r--   0 musy      (8766) sharpe    (4311)      818 2021-03-06 19:00:03.000000 vedo-2023.4.5/examples/other/dolfin/submesh_boundary.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     2471 2023-01-27 15:42:02.000000 vedo-2023.4.5/examples/other/dolfin/turing_2d.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     2461 2023-04-17 12:22:50.000000 vedo-2023.4.5/examples/other/dolfin/turing_3d.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      774 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/other/ellipt_fourier_desc.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      474 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/other/export_numpy.py
--rw-r--r--   0 musy      (8766) sharpe    (4311)      653 2022-04-05 19:15:36.000000 vedo-2023.4.5/examples/other/export_x3d.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      939 2022-12-09 20:52:34.000000 vedo-2023.4.5/examples/other/flag_labels1.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      422 2022-12-07 20:53:49.000000 vedo-2023.4.5/examples/other/flag_labels2.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      330 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/other/icon.py
--rw-rw-r--   0 musy      (8766) sharpe    (4311)      841 2021-05-04 16:06:12.000000 vedo-2023.4.5/examples/other/iminuit1.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1127 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/other/inset.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1797 2023-02-27 12:54:07.000000 vedo-2023.4.5/examples/other/make_video.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      398 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/other/meshio_read.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1900 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/other/morphomatics_regression.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1328 2022-10-21 13:11:03.000000 vedo-2023.4.5/examples/other/morphomatics_tube.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      791 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/other/napari1.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      907 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/other/nevergrad_opt.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1190 2023-03-23 15:07:49.000000 vedo-2023.4.5/examples/other/printc.py
--rw-rw-r--   0 musy      (8766) sharpe    (4311)      529 2022-06-06 19:09:50.000000 vedo-2023.4.5/examples/other/pygeodesic1.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1030 2023-06-15 12:18:25.000000 vedo-2023.4.5/examples/other/pygmsh_cut.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      958 2023-01-08 20:24:11.000000 vedo-2023.4.5/examples/other/pymeshlab1.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      609 2023-01-08 20:24:00.000000 vedo-2023.4.5/examples/other/pymeshlab2.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1743 2023-06-15 12:22:12.000000 vedo-2023.4.5/examples/other/qt_cutter.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     4000 2023-01-09 14:49:35.000000 vedo-2023.4.5/examples/other/qt_tabs.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1984 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/other/qt_window1.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1819 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/other/qt_window2.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1713 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/other/qt_window3.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      508 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/other/remesh_ACVD.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1095 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/other/remesh_meshfix.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1563 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/other/remesh_tetgen.py
--rwxrwxr-x   0 musy      (8766) sharpe    (4311)     1040 2022-12-15 17:42:58.000000 vedo-2023.4.5/examples/other/run_all.sh
--rw-r-----   0 musy      (8766) sharpe    (4311)   155200 2023-06-18 15:27:07.000000 vedo-2023.4.5/examples/other/scene.npz
--rw-r-----   0 musy      (8766) sharpe    (4311)     3119 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/other/spherical_harmonics1.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     3023 2023-05-26 16:42:50.000000 vedo-2023.4.5/examples/other/spherical_harmonics2.py
--rw-rw-r--   0 musy      (8766) sharpe    (4311)      217 2022-11-27 17:34:53.000000 vedo-2023.4.5/examples/other/tensor_grid1.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     4769 2023-04-17 17:54:59.000000 vedo-2023.4.5/examples/other/tensor_grid2.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      770 2023-02-02 19:37:56.000000 vedo-2023.4.5/examples/other/trame_ex1.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      878 2023-02-02 21:28:33.000000 vedo-2023.4.5/examples/other/trame_ex2.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     2285 2023-02-02 21:16:56.000000 vedo-2023.4.5/examples/other/trame_ex3.py
-drwxr-x---   0 musy      (8766) sharpe    (4311)        0 2023-06-18 15:36:43.400367 vedo-2023.4.5/examples/other/trimesh/
--rw-r-----   0 musy      (8766) sharpe    (4311)     1832 2022-11-07 13:12:03.000000 vedo-2023.4.5/examples/other/trimesh/README.md
--rw-rw-r--   0 musy      (8766) sharpe    (4311)        5 2022-06-06 19:09:50.000000 vedo-2023.4.5/examples/other/trimesh/__init__.py
--rw-rw-r--   0 musy      (8766) sharpe    (4311)     1193 2022-06-06 19:09:50.000000 vedo-2023.4.5/examples/other/trimesh/nearest.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1164 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/other/trimesh/ray.py
--rwxrwxr-x   0 musy      (8766) sharpe    (4311)      254 2022-08-14 19:31:52.000000 vedo-2023.4.5/examples/other/trimesh/run_all.sh
--rw-r-----   0 musy      (8766) sharpe    (4311)     1628 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/other/trimesh/section.py
--rw-rw-r--   0 musy      (8766) sharpe    (4311)     1193 2022-06-06 19:09:50.000000 vedo-2023.4.5/examples/other/trimesh/shortest.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      688 2023-04-03 11:58:30.000000 vedo-2023.4.5/examples/other/vpolyscope.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1610 2023-05-26 16:42:31.000000 vedo-2023.4.5/examples/other/wx_window1.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1726 2022-12-07 19:20:10.000000 vedo-2023.4.5/examples/other/wx_window2.py
-drwxr-x---   0 musy      (8766) sharpe    (4311)        0 2023-06-18 15:36:43.408367 vedo-2023.4.5/examples/pyplot/
--rw-rw-r--   0 musy      (8766) sharpe    (4311)        3 2021-01-14 20:43:53.000000 vedo-2023.4.5/examples/pyplot/__init__.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     2684 2023-02-16 17:49:40.000000 vedo-2023.4.5/examples/pyplot/anim_lines.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      663 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/pyplot/caption.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     2059 2023-02-16 17:43:20.000000 vedo-2023.4.5/examples/pyplot/custom_axes1.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      987 2023-02-16 17:44:53.000000 vedo-2023.4.5/examples/pyplot/custom_axes2.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      779 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/pyplot/custom_axes3.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1078 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/pyplot/custom_axes4.py
--rw-rw-r--   0 musy      (8766) sharpe    (4311)      280 2022-02-25 13:08:22.000000 vedo-2023.4.5/examples/pyplot/donut.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     2167 2023-04-17 13:00:20.000000 vedo-2023.4.5/examples/pyplot/earthquake_browser.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      561 2023-03-09 15:49:39.000000 vedo-2023.4.5/examples/pyplot/embed_matplotlib.py
--rw-rw-r--   0 musy      (8766) sharpe    (4311)     1896 2023-04-27 17:11:39.000000 vedo-2023.4.5/examples/pyplot/explore5d.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      827 2022-11-17 21:02:52.000000 vedo-2023.4.5/examples/pyplot/fill_gap.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      848 2023-03-10 19:38:14.000000 vedo-2023.4.5/examples/pyplot/fit_circle.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      944 2022-10-26 16:27:11.000000 vedo-2023.4.5/examples/pyplot/fit_curve.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1126 2023-04-30 20:06:51.000000 vedo-2023.4.5/examples/pyplot/fit_erf.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1477 2023-02-17 15:30:35.000000 vedo-2023.4.5/examples/pyplot/fit_polynomial1.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1955 2023-02-17 15:31:18.000000 vedo-2023.4.5/examples/pyplot/fit_polynomial2.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     3836 2023-02-16 17:41:47.000000 vedo-2023.4.5/examples/pyplot/fonts3d.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     2341 2023-03-23 11:26:07.000000 vedo-2023.4.5/examples/pyplot/fourier_epicycles.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      801 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/pyplot/glyphs3.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      948 2023-02-17 15:33:49.000000 vedo-2023.4.5/examples/pyplot/goniometer.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1001 2023-06-18 13:16:30.000000 vedo-2023.4.5/examples/pyplot/graph_lineage.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1662 2023-06-18 13:18:08.000000 vedo-2023.4.5/examples/pyplot/graph_network.py
--rw-r-----   0 musy      (8766) sharpe    (4311)       98 2022-04-06 10:06:05.000000 vedo-2023.4.5/examples/pyplot/histo_1d_a.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      947 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/pyplot/histo_1d_b.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      881 2023-02-17 15:35:41.000000 vedo-2023.4.5/examples/pyplot/histo_1d_c.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1120 2023-04-30 20:16:33.000000 vedo-2023.4.5/examples/pyplot/histo_1d_d.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      797 2023-04-13 15:13:03.000000 vedo-2023.4.5/examples/pyplot/histo_1d_e.py
--rw-rw-r--   0 musy      (8766) sharpe    (4311)      597 2022-03-29 11:28:28.000000 vedo-2023.4.5/examples/pyplot/histo_2d_a.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      550 2022-11-08 11:49:50.000000 vedo-2023.4.5/examples/pyplot/histo_2d_b.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      547 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/pyplot/histo_3d.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      798 2022-11-17 21:03:22.000000 vedo-2023.4.5/examples/pyplot/histo_gauss.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      575 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/pyplot/histo_hexagonal.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     2599 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/pyplot/histo_manual.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1166 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/pyplot/histo_pca.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1332 2023-02-17 17:17:57.000000 vedo-2023.4.5/examples/pyplot/histo_polar.py
--rw-rw-r--   0 musy      (8766) sharpe    (4311)      364 2022-10-28 11:18:51.000000 vedo-2023.4.5/examples/pyplot/histo_spheric.py
--rw-rw-r--   0 musy      (8766) sharpe    (4311)      583 2022-03-21 12:35:17.000000 vedo-2023.4.5/examples/pyplot/histo_violin.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1143 2023-02-16 17:46:00.000000 vedo-2023.4.5/examples/pyplot/intersect2d.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1159 2023-03-10 19:39:34.000000 vedo-2023.4.5/examples/pyplot/isolines.py
--rw-rw-r--   0 musy      (8766) sharpe    (4311)      652 2022-04-04 18:51:43.000000 vedo-2023.4.5/examples/pyplot/latex.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      906 2023-03-14 18:39:00.000000 vedo-2023.4.5/examples/pyplot/lines_intersect.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      415 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/pyplot/markers.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      413 2023-02-02 19:24:07.000000 vedo-2023.4.5/examples/pyplot/markpoint.py
--rw-rw-r--   0 musy      (8766) sharpe    (4311)      556 2023-02-17 15:38:52.000000 vedo-2023.4.5/examples/pyplot/np_matrix.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      946 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/pyplot/plot_bars.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      804 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/pyplot/plot_density2d.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      577 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/pyplot/plot_density3d.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1012 2023-03-23 11:26:39.000000 vedo-2023.4.5/examples/pyplot/plot_density4d.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1049 2023-04-30 20:19:11.000000 vedo-2023.4.5/examples/pyplot/plot_empty.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1371 2023-05-30 16:11:07.000000 vedo-2023.4.5/examples/pyplot/plot_errband.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1147 2023-02-17 15:40:26.000000 vedo-2023.4.5/examples/pyplot/plot_errbars.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1792 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/pyplot/plot_extra_yaxis.py
--rw-rw-r--   0 musy      (8766) sharpe    (4311)     1350 2023-03-14 18:37:56.000000 vedo-2023.4.5/examples/pyplot/plot_fxy.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      692 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/pyplot/plot_hexcells.py
--rw-rw-r--   0 musy      (8766) sharpe    (4311)      537 2022-04-04 19:10:12.000000 vedo-2023.4.5/examples/pyplot/plot_multi.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      877 2022-11-18 17:33:00.000000 vedo-2023.4.5/examples/pyplot/plot_pip.py
--rw-rw-r--   0 musy      (8766) sharpe    (4311)      586 2022-03-21 12:35:46.000000 vedo-2023.4.5/examples/pyplot/plot_polar.py
--rw-rw-r--   0 musy      (8766) sharpe    (4311)      761 2021-05-04 16:06:12.000000 vedo-2023.4.5/examples/pyplot/plot_spheric.py
--rw-rw-r--   0 musy      (8766) sharpe    (4311)      624 2023-06-18 13:19:08.000000 vedo-2023.4.5/examples/pyplot/plot_stream.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      256 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/pyplot/quiver.py
--rwxr-xr-x   0 musy      (8766) sharpe    (4311)      279 2021-10-05 17:36:39.000000 vedo-2023.4.5/examples/pyplot/run_all.sh
--rw-rw-r--   0 musy      (8766) sharpe    (4311)      397 2022-03-29 23:31:38.000000 vedo-2023.4.5/examples/pyplot/scatter1.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1312 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/pyplot/scatter2.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1003 2023-04-30 20:26:37.000000 vedo-2023.4.5/examples/pyplot/scatter3.py
--rw-rw-r--   0 musy      (8766) sharpe    (4311)      501 2022-06-06 19:09:50.000000 vedo-2023.4.5/examples/pyplot/scatter_large.py
--rw-rw-r--   0 musy      (8766) sharpe    (4311)      421 2022-03-20 22:00:43.000000 vedo-2023.4.5/examples/pyplot/triangulate2d.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1476 2023-02-16 17:50:52.000000 vedo-2023.4.5/examples/pyplot/whiskers.py
-drwxr-x---   0 musy      (8766) sharpe    (4311)        0 2023-06-18 15:36:43.408367 vedo-2023.4.5/examples/simulations/
--rw-rw-r--   0 musy      (8766) sharpe    (4311)        3 2021-03-06 18:59:20.000000 vedo-2023.4.5/examples/simulations/__init__.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      556 2023-06-18 13:45:53.000000 vedo-2023.4.5/examples/simulations/airplane1.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      876 2023-06-18 13:50:37.000000 vedo-2023.4.5/examples/simulations/airplane2.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1189 2023-06-02 13:45:59.000000 vedo-2023.4.5/examples/simulations/aspring1.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1570 2023-06-05 14:34:00.000000 vedo-2023.4.5/examples/simulations/aspring2_player.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     4596 2023-02-05 18:12:21.000000 vedo-2023.4.5/examples/simulations/brownian2d.py
--rw-rw-r--   0 musy      (8766) sharpe    (4311)     2125 2022-02-24 19:44:14.000000 vedo-2023.4.5/examples/simulations/doubleslit.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      721 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/simulations/drag_chain.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     4999 2023-06-15 17:09:37.000000 vedo-2023.4.5/examples/simulations/gas.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     2889 2023-01-07 21:26:46.000000 vedo-2023.4.5/examples/simulations/grayscott.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     2440 2023-02-16 19:03:31.000000 vedo-2023.4.5/examples/simulations/gyroscope1.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     2896 2023-03-23 11:27:28.000000 vedo-2023.4.5/examples/simulations/gyroscope2.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     2113 2023-01-30 20:16:44.000000 vedo-2023.4.5/examples/simulations/hanoi3d.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      994 2023-01-20 17:18:38.000000 vedo-2023.4.5/examples/simulations/koch_fractal.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1103 2023-05-26 16:37:59.000000 vedo-2023.4.5/examples/simulations/lorenz.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     2120 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/simulations/mag_field1.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      781 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/simulations/mag_field2.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     4367 2023-02-16 18:41:40.000000 vedo-2023.4.5/examples/simulations/multiple_pendulum.py
--rw-r-----   0 musy      (8766) sharpe    (4311)    11430 2023-01-18 12:46:24.000000 vedo-2023.4.5/examples/simulations/optics_base.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     4261 2022-10-26 14:34:00.000000 vedo-2023.4.5/examples/simulations/optics_main1.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     2124 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/simulations/optics_main2.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1423 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/simulations/optics_main3.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     4194 2023-06-18 13:29:08.000000 vedo-2023.4.5/examples/simulations/particle_simulator.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1155 2023-06-18 14:08:54.000000 vedo-2023.4.5/examples/simulations/pendulum_3d.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1886 2023-02-05 18:10:20.000000 vedo-2023.4.5/examples/simulations/pendulum_ode.py
--rwxr-xr-x   0 musy      (8766) sharpe    (4311)      279 2021-10-05 17:36:43.000000 vedo-2023.4.5/examples/simulations/run_all.sh
--rw-r-----   0 musy      (8766) sharpe    (4311)     2697 2023-05-26 16:41:55.000000 vedo-2023.4.5/examples/simulations/self_org_maps2d.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      859 2023-02-17 17:01:30.000000 vedo-2023.4.5/examples/simulations/spline_ease.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      564 2023-06-18 13:24:19.000000 vedo-2023.4.5/examples/simulations/trail.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1665 2022-11-18 16:09:52.000000 vedo-2023.4.5/examples/simulations/tunnelling1.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     2800 2023-05-26 16:39:36.000000 vedo-2023.4.5/examples/simulations/tunnelling2.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     4456 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/simulations/value_iteration.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     2121 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/simulations/volterra.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     3610 2023-02-05 18:08:51.000000 vedo-2023.4.5/examples/simulations/wave_equation1d.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1656 2023-01-07 21:26:46.000000 vedo-2023.4.5/examples/simulations/wave_equation2d.py
-drwxr-x---   0 musy      (8766) sharpe    (4311)        0 2023-06-18 15:36:43.416367 vedo-2023.4.5/examples/volumetric/
--rw-rw-r--   0 musy      (8766) sharpe    (4311)        3 2021-03-06 19:00:26.000000 vedo-2023.4.5/examples/volumetric/__init__.py
--rw-rw-r--   0 musy      (8766) sharpe    (4311)      244 2023-03-15 13:47:09.000000 vedo-2023.4.5/examples/volumetric/app_isobrowser.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      273 2022-02-09 17:33:21.000000 vedo-2023.4.5/examples/volumetric/app_raycaster.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      919 2023-03-10 19:37:32.000000 vedo-2023.4.5/examples/volumetric/colorize_volume.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      564 2023-02-23 20:04:44.000000 vedo-2023.4.5/examples/volumetric/delaunay3d.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      689 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/volumetric/densifycloud.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     2032 2023-05-28 11:39:57.000000 vedo-2023.4.5/examples/volumetric/earth_model.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      376 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/volumetric/erode_dilate.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      290 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/volumetric/euclidian_dist.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      950 2023-02-23 19:58:20.000000 vedo-2023.4.5/examples/volumetric/image_false_colors.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      652 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/volumetric/image_fft.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1432 2022-11-20 18:06:50.000000 vedo-2023.4.5/examples/volumetric/image_mask.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1387 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/volumetric/image_probe.py
--rw-rw-r--   0 musy      (8766) sharpe    (4311)      795 2022-12-15 15:46:00.000000 vedo-2023.4.5/examples/volumetric/image_rgba.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      805 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/volumetric/image_to_mesh.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1484 2023-05-28 11:40:21.000000 vedo-2023.4.5/examples/volumetric/interpolate_volume.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      436 2023-06-15 12:19:51.000000 vedo-2023.4.5/examples/volumetric/isosurfaces.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      451 2023-02-17 17:06:54.000000 vedo-2023.4.5/examples/volumetric/legosurface.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      616 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/volumetric/lowpassfilter.py
--rw-rw-r--   0 musy      (8766) sharpe    (4311)      462 2022-03-19 15:00:10.000000 vedo-2023.4.5/examples/volumetric/mesh2volume.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1208 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/volumetric/multiscalars.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      608 2023-02-23 13:22:42.000000 vedo-2023.4.5/examples/volumetric/numpy2volume1.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      539 2023-02-14 15:11:12.000000 vedo-2023.4.5/examples/volumetric/numpy2volume2.py
--rw-rw-r--   0 musy      (8766) sharpe    (4311)      521 2022-08-14 19:31:52.000000 vedo-2023.4.5/examples/volumetric/numpy_imread.py
--rw-r--r--   0 musy      (8766) sharpe    (4311)    10019 2021-03-06 19:00:26.000000 vedo-2023.4.5/examples/volumetric/off_furniture.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      780 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/volumetric/office.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      346 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/volumetric/point_density.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      590 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/volumetric/probe_line1.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      732 2023-02-23 11:27:44.000000 vedo-2023.4.5/examples/volumetric/probe_line2.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      540 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/volumetric/probe_points.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      614 2022-12-15 18:13:49.000000 vedo-2023.4.5/examples/volumetric/read_volume1.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1196 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/volumetric/read_volume2.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1272 2023-05-30 16:00:02.000000 vedo-2023.4.5/examples/volumetric/read_volume3.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      593 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/volumetric/read_vts.py
--rwxr-xr-x   0 musy      (8766) sharpe    (4311)      281 2021-10-05 17:36:48.000000 vedo-2023.4.5/examples/volumetric/run_all.sh
--rw-r-----   0 musy      (8766) sharpe    (4311)      299 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/volumetric/slice_mesh.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1037 2023-03-23 11:34:02.000000 vedo-2023.4.5/examples/volumetric/slice_plane1.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      540 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/volumetric/slice_plane2.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      576 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/volumetric/slicer1.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1298 2023-02-03 14:25:42.000000 vedo-2023.4.5/examples/volumetric/slicer2.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      898 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/volumetric/streamlines1.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      781 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/volumetric/streamlines2.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      895 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/volumetric/streamlines3.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      612 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/volumetric/streamlines4.py
--rw-rw-r--   0 musy      (8766) sharpe    (4311)      811 2022-05-08 19:29:44.000000 vedo-2023.4.5/examples/volumetric/streamribbons.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      615 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/volumetric/tensors.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      619 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/volumetric/tet_astyle.py
--rw-rw-r--   0 musy      (8766) sharpe    (4311)      936 2021-09-20 16:16:08.000000 vedo-2023.4.5/examples/volumetric/tet_build.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      332 2023-02-16 17:47:52.000000 vedo-2023.4.5/examples/volumetric/tet_cutMesh1.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1002 2023-02-23 15:08:37.000000 vedo-2023.4.5/examples/volumetric/tet_cutMesh2.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1216 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/volumetric/tet_explode.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      485 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/volumetric/tet_isos_slice.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      433 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/volumetric/tet_threshold.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      964 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/volumetric/tetralize_surface.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      201 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/volumetric/ugrid1.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      274 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/volumetric/ugrid2.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      285 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/volumetric/vol2points.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      422 2022-11-14 13:08:27.000000 vedo-2023.4.5/examples/volumetric/volumeFromMesh.py
--rw-r-----   0 musy      (8766) sharpe    (4311)     1930 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/volumetric/volume_operations.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      769 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/volumetric/volume_sharemap.py
--rw-r-----   0 musy      (8766) sharpe    (4311)      369 2022-10-17 16:29:31.000000 vedo-2023.4.5/examples/volumetric/warp_scalars.py
--rw-r-----   0 musy      (8766) sharpe    (4311)       75 2023-06-18 15:36:43.424368 vedo-2023.4.5/setup.cfg
--rwxr-x---   0 musy      (8766) sharpe    (4311)     2767 2023-01-18 12:46:24.000000 vedo-2023.4.5/setup.py
-drwxr-x---   0 musy      (8766) sharpe    (4311)        0 2023-06-18 15:36:43.416367 vedo-2023.4.5/vedo/
--rw-r-----   0 musy      (8766) sharpe    (4311)     3676 2023-06-15 15:37:21.000000 vedo-2023.4.5/vedo/__init__.py
--rw-r-----   0 musy      (8766) sharpe    (4311)   154478 2023-06-18 15:13:17.000000 vedo-2023.4.5/vedo/addons.py
--rw-r-----   0 musy      (8766) sharpe    (4311)    67553 2023-06-16 16:53:14.000000 vedo-2023.4.5/vedo/applications.py
--rw-r-----   0 musy      (8766) sharpe    (4311)    12563 2023-04-28 15:16:08.000000 vedo-2023.4.5/vedo/assembly.py
--rw-r-----   0 musy      (8766) sharpe    (4311)    14266 2023-06-13 15:58:10.000000 vedo-2023.4.5/vedo/backends.py
--rw-r-----   0 musy      (8766) sharpe    (4311)    91529 2023-05-28 11:19:54.000000 vedo-2023.4.5/vedo/base.py
--rw-r-----   0 musy      (8766) sharpe    (4311)    34983 2023-05-30 15:52:32.000000 vedo-2023.4.5/vedo/cli.py
--rw-rw-r--   0 musy      (8766) sharpe    (4311)   304787 2023-01-27 09:58:59.000000 vedo-2023.4.5/vedo/cmaps.py
--rw-r-----   0 musy      (8766) sharpe    (4311)    34673 2023-05-01 10:25:38.000000 vedo-2023.4.5/vedo/colors.py
--rw-r-----   0 musy      (8766) sharpe    (4311)    31736 2023-04-28 15:30:53.000000 vedo-2023.4.5/vedo/dolfin.py
--rw-r-----   0 musy      (8766) sharpe    (4311)    71310 2023-05-25 11:09:42.000000 vedo-2023.4.5/vedo/file_io.py
-drwxr-x---   0 musy      (8766) sharpe    (4311)        0 2023-06-18 15:36:43.424368 vedo-2023.4.5/vedo/fonts/
--rw-r-----   0 musy      (8766) sharpe    (4311)    65008 2023-02-08 19:31:34.000000 vedo-2023.4.5/vedo/fonts/Bongas.npz
--rw-r--r--   0 musy      (8766) sharpe    (4311)    33928 2014-01-28 02:04:38.000000 vedo-2023.4.5/vedo/fonts/Bongas.ttf
--rw-r-----   0 musy      (8766) sharpe    (4311)    65491 2023-02-08 19:33:53.000000 vedo-2023.4.5/vedo/fonts/Calco.npz
--rw-r--r--   0 musy      (8766) sharpe    (4311)    65528 2020-06-13 19:22:59.000000 vedo-2023.4.5/vedo/fonts/Calco.ttf
--rw-r-----   0 musy      (8766) sharpe    (4311)   127729 2023-02-08 19:34:41.000000 vedo-2023.4.5/vedo/fonts/Comae.npz
--rw-r--r--   0 musy      (8766) sharpe    (4311)    98408 2014-01-28 02:09:20.000000 vedo-2023.4.5/vedo/fonts/Comae.ttf
--rw-r-----   0 musy      (8766) sharpe    (4311)   153242 2023-02-08 19:37:52.000000 vedo-2023.4.5/vedo/fonts/Glasgo.npz
--rw-rw-r--   0 musy      (8766) sharpe    (4311)   144352 2017-09-01 17:37:42.000000 vedo-2023.4.5/vedo/fonts/Glasgo.ttf
--rw-r-----   0 musy      (8766) sharpe    (4311)   196983 2023-02-08 19:52:45.000000 vedo-2023.4.5/vedo/fonts/Kanopus.npz
--rw-r--r--   0 musy      (8766) sharpe    (4311)   901240 2020-08-12 13:11:07.000000 vedo-2023.4.5/vedo/fonts/Kanopus.ttf
--rw-r-----   0 musy      (8766) sharpe    (4311)   111014 2023-02-08 19:25:41.000000 vedo-2023.4.5/vedo/fonts/Normografo.npz
--rw-rw-r--   0 musy      (8766) sharpe    (4311)    52460 2017-08-03 01:32:10.000000 vedo-2023.4.5/vedo/fonts/Normografo.ttf
--rw-r-----   0 musy      (8766) sharpe    (4311)    95884 2023-02-08 19:50:37.000000 vedo-2023.4.5/vedo/fonts/Quikhand.npz
--rw-rw-r--   0 musy      (8766) sharpe    (4311)    79328 2020-06-22 00:16:11.000000 vedo-2023.4.5/vedo/fonts/Quikhand.ttf
--rw-r-----   0 musy      (8766) sharpe    (4311)    91962 2023-02-08 19:47:39.000000 vedo-2023.4.5/vedo/fonts/SmartCouric.npz
--rw-r--r--   0 musy      (8766) sharpe    (4311)    98156 2020-07-27 12:20:22.000000 vedo-2023.4.5/vedo/fonts/SmartCouric.ttf
--rw-r-----   0 musy      (8766) sharpe    (4311)   110904 2023-02-08 19:45:55.000000 vedo-2023.4.5/vedo/fonts/Theemim.npz
--rw-r--r--   0 musy      (8766) sharpe    (4311)   169668 2013-06-04 12:17:38.000000 vedo-2023.4.5/vedo/fonts/Theemim.ttf
--rw-r-----   0 musy      (8766) sharpe    (4311)   134429 2023-02-08 19:55:49.000000 vedo-2023.4.5/vedo/fonts/VictorMono.npz
--rw-r--r--   0 musy      (8766) sharpe    (4311)   153724 2020-06-29 16:12:20.000000 vedo-2023.4.5/vedo/fonts/VictorMono.ttf
--rw-r-----   0 musy      (8766) sharpe    (4311)    46534 2023-06-16 16:54:47.000000 vedo-2023.4.5/vedo/interactor_modes.py
--rw-r-----   0 musy      (8766) sharpe    (4311)   104013 2023-06-16 14:53:23.000000 vedo-2023.4.5/vedo/mesh.py
--rw-r-----   0 musy      (8766) sharpe    (4311)    51186 2023-05-25 18:17:11.000000 vedo-2023.4.5/vedo/picture.py
--rw-r-----   0 musy      (8766) sharpe    (4311)   151871 2023-06-18 15:08:45.000000 vedo-2023.4.5/vedo/plotter.py
--rw-r-----   0 musy      (8766) sharpe    (4311)   184341 2023-06-18 13:52:48.000000 vedo-2023.4.5/vedo/pointcloud.py
--rw-r-----   0 musy      (8766) sharpe    (4311)   145381 2023-05-30 16:09:41.000000 vedo-2023.4.5/vedo/pyplot.py
--rw-r-----   0 musy      (8766) sharpe    (4311)    23633 2023-06-13 18:44:02.000000 vedo-2023.4.5/vedo/settings.py
--rw-r-----   0 musy      (8766) sharpe    (4311)   160688 2023-06-16 12:40:01.000000 vedo-2023.4.5/vedo/shapes.py
--rw-r-----   0 musy      (8766) sharpe    (4311)    17315 2023-05-01 09:58:04.000000 vedo-2023.4.5/vedo/tetmesh.py
--rw-r-----   0 musy      (8766) sharpe    (4311)    12955 2023-05-01 09:57:55.000000 vedo-2023.4.5/vedo/ugrid.py
--rw-r-----   0 musy      (8766) sharpe    (4311)    88404 2023-05-19 15:16:12.000000 vedo-2023.4.5/vedo/utils.py
--rw-r-----   0 musy      (8766) sharpe    (4311)       22 2023-06-18 15:35:54.000000 vedo-2023.4.5/vedo/version.py
--rw-r-----   0 musy      (8766) sharpe    (4311)    61918 2023-05-25 18:42:54.000000 vedo-2023.4.5/vedo/volume.py
--rw-r-----   0 musy      (8766) sharpe    (4311)    13196 2023-06-15 11:20:58.000000 vedo-2023.4.5/vedo/vtkclasses.py
-drwxr-x---   0 musy      (8766) sharpe    (4311)        0 2023-06-18 15:36:43.420367 vedo-2023.4.5/vedo.egg-info/
--rw-r-----   0 musy      (8766) sharpe    (4311)     1249 2023-06-18 15:36:43.000000 vedo-2023.4.5/vedo.egg-info/PKG-INFO
--rw-r-----   0 musy      (8766) sharpe    (4311)    13783 2023-06-18 15:36:43.000000 vedo-2023.4.5/vedo.egg-info/SOURCES.txt
--rw-r-----   0 musy      (8766) sharpe    (4311)        1 2023-06-18 15:36:43.000000 vedo-2023.4.5/vedo.egg-info/dependency_links.txt
--rw-r-----   0 musy      (8766) sharpe    (4311)       46 2023-06-18 15:36:43.000000 vedo-2023.4.5/vedo.egg-info/entry_points.txt
--rw-r-----   0 musy      (8766) sharpe    (4311)       30 2023-06-18 15:36:43.000000 vedo-2023.4.5/vedo.egg-info/requires.txt
--rw-r-----   0 musy      (8766) sharpe    (4311)        5 2023-06-18 15:36:43.000000 vedo-2023.4.5/vedo.egg-info/top_level.txt
+drwxr-x---   0 musy      (8766) sharpe    (4311)        0 2023-06-21 17:43:43.576463 vedo-2023.4.6/
+-rw-r-----   0 musy      (8766) sharpe    (4311)     7617 2022-03-01 14:15:57.000000 vedo-2023.4.6/FONT.LICENSE
+-rw-r--r--   0 musy      (8766) sharpe    (4311)     1067 2022-02-27 13:43:39.000000 vedo-2023.4.6/LICENSE
+-rw-r--r--   0 musy      (8766) sharpe    (4311)      267 2022-03-01 12:22:11.000000 vedo-2023.4.6/MANIFEST.in
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1249 2023-06-21 17:43:43.576463 vedo-2023.4.6/PKG-INFO
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)    10862 2023-06-02 16:59:49.000000 vedo-2023.4.6/README.md
+drwxr-x---   0 musy      (8766) sharpe    (4311)        0 2023-06-21 17:43:43.528463 vedo-2023.4.6/examples/
+drwxr-x---   0 musy      (8766) sharpe    (4311)        0 2023-06-21 17:43:43.532463 vedo-2023.4.6/examples/advanced/
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)        3 2021-03-06 18:50:54.000000 vedo-2023.4.6/examples/advanced/__init__.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1467 2023-02-02 17:56:11.000000 vedo-2023.4.6/examples/advanced/capping_mesh.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      559 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/advanced/contours2mesh.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      281 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/advanced/convex_hull.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      422 2023-02-03 19:31:48.000000 vedo-2023.4.6/examples/advanced/cut_and_cap.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      582 2023-02-17 17:24:05.000000 vedo-2023.4.6/examples/advanced/cut_with_mesh1.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      440 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/advanced/cut_with_points1.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      498 2023-06-18 13:10:42.000000 vedo-2023.4.6/examples/advanced/cut_with_points2.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      941 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/advanced/fitline.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      683 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/advanced/fitplanes.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      949 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/advanced/fitspheres1.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      972 2023-02-17 17:16:26.000000 vedo-2023.4.6/examples/advanced/fitspheres2.py
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)      546 2022-02-25 12:03:56.000000 vedo-2023.4.6/examples/advanced/geodesic.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     5443 2022-11-06 15:19:38.000000 vedo-2023.4.6/examples/advanced/geological_model.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      824 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/advanced/gyroid.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     2153 2023-06-18 13:14:58.000000 vedo-2023.4.6/examples/advanced/interpolate_field.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      672 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/advanced/interpolate_scalar1.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1129 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/advanced/interpolate_scalar2.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      680 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/advanced/interpolate_scalar3.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      996 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/advanced/interpolate_scalar4.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      680 2023-01-20 17:20:50.000000 vedo-2023.4.6/examples/advanced/line2mesh_quads.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      731 2023-01-20 17:20:32.000000 vedo-2023.4.6/examples/advanced/line2mesh_tri.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1416 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/advanced/measure_curvature.py
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)      461 2022-12-07 17:35:32.000000 vedo-2023.4.6/examples/advanced/mesh_smoother1.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      536 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/advanced/mesh_smoother2.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1074 2023-02-17 14:59:48.000000 vedo-2023.4.6/examples/advanced/meshquality.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      919 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/advanced/moving_least_squares1D.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1676 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/advanced/moving_least_squares2D.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     2182 2023-03-23 11:00:46.000000 vedo-2023.4.6/examples/advanced/multi_viewer2.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1123 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/advanced/recosurface.py
+-rwxr-x---   0 musy      (8766) sharpe    (4311)      347 2022-11-14 13:08:27.000000 vedo-2023.4.6/examples/advanced/run_all.sh
+-rw-r-----   0 musy      (8766) sharpe    (4311)      395 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/advanced/skeletonize.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     2197 2023-03-23 11:07:23.000000 vedo-2023.4.6/examples/advanced/spline_draw.py
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)      316 2022-02-25 12:11:18.000000 vedo-2023.4.6/examples/advanced/splitmesh.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      333 2023-03-14 16:58:51.000000 vedo-2023.4.6/examples/advanced/timer_callback0.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1232 2023-04-13 17:24:04.000000 vedo-2023.4.6/examples/advanced/timer_callback1.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     2299 2023-02-17 15:55:08.000000 vedo-2023.4.6/examples/advanced/timer_callback2.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1708 2023-04-13 17:20:56.000000 vedo-2023.4.6/examples/advanced/timer_callback3.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      526 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/advanced/voronoi2.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      990 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/advanced/warp1.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      887 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/advanced/warp2.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     3663 2023-01-07 21:26:46.000000 vedo-2023.4.6/examples/advanced/warp3.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     6776 2023-03-23 11:06:49.000000 vedo-2023.4.6/examples/advanced/warp4.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     4991 2023-01-07 21:26:46.000000 vedo-2023.4.6/examples/advanced/warp5.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1033 2023-04-03 14:27:35.000000 vedo-2023.4.6/examples/advanced/warp6.py
+drwxr-x---   0 musy      (8766) sharpe    (4311)        0 2023-06-21 17:43:43.544463 vedo-2023.4.6/examples/basic/
+-rw-r-----   0 musy      (8766) sharpe    (4311)      682 2023-03-14 19:19:18.000000 vedo-2023.4.6/examples/basic/.vedo_pipeline_graphviz
+-rw-r-----   0 musy      (8766) sharpe    (4311)    19278 2023-03-14 19:19:18.000000 vedo-2023.4.6/examples/basic/.vedo_pipeline_graphviz.pdf
+-rw-r-----   0 musy      (8766) sharpe    (4311)     2420 2023-06-21 16:23:31.000000 vedo-2023.4.6/examples/basic/.vedo_recorded_events.log
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)        3 2021-03-06 18:56:56.000000 vedo-2023.4.6/examples/basic/__init__.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      838 2023-04-13 17:38:35.000000 vedo-2023.4.6/examples/basic/align1.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1027 2023-04-13 17:44:46.000000 vedo-2023.4.6/examples/basic/align2.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1164 2023-04-13 17:57:24.000000 vedo-2023.4.6/examples/basic/align3.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1079 2023-04-13 18:00:42.000000 vedo-2023.4.6/examples/basic/align4.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1148 2023-04-13 18:02:59.000000 vedo-2023.4.6/examples/basic/align5.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      883 2023-04-13 18:05:19.000000 vedo-2023.4.6/examples/basic/align6.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      849 2023-04-13 18:11:41.000000 vedo-2023.4.6/examples/basic/background_image.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1377 2023-04-13 18:14:10.000000 vedo-2023.4.6/examples/basic/boolean.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      719 2023-04-13 18:16:55.000000 vedo-2023.4.6/examples/basic/boundaries.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      782 2023-06-21 15:04:01.000000 vedo-2023.4.6/examples/basic/buildmesh.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1204 2023-04-13 18:22:38.000000 vedo-2023.4.6/examples/basic/buttons.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1495 2023-04-13 18:26:44.000000 vedo-2023.4.6/examples/basic/cartoony.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      731 2023-04-13 18:28:57.000000 vedo-2023.4.6/examples/basic/cells_within_bounds.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1322 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/basic/closewindow.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      931 2023-04-13 18:30:21.000000 vedo-2023.4.6/examples/basic/clustering.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      688 2023-04-13 18:38:32.000000 vedo-2023.4.6/examples/basic/color_mesh_cells1.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      768 2023-04-13 18:40:16.000000 vedo-2023.4.6/examples/basic/color_mesh_cells2.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1680 2023-04-13 18:32:30.000000 vedo-2023.4.6/examples/basic/colorcubes.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1322 2023-04-13 18:34:38.000000 vedo-2023.4.6/examples/basic/colorlines.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1213 2023-04-13 18:36:50.000000 vedo-2023.4.6/examples/basic/colormap_list.py
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)      703 2023-02-17 15:06:20.000000 vedo-2023.4.6/examples/basic/colormaps.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      709 2023-04-13 18:42:02.000000 vedo-2023.4.6/examples/basic/connected_vtx.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     2847 2023-04-17 09:34:03.000000 vedo-2023.4.6/examples/basic/cut_freehand.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      630 2023-06-15 12:11:15.000000 vedo-2023.4.6/examples/basic/cut_interactive.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      772 2023-04-13 18:49:28.000000 vedo-2023.4.6/examples/basic/delaunay2d.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1003 2023-04-13 18:51:43.000000 vedo-2023.4.6/examples/basic/delete_mesh_pts.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      678 2023-04-13 18:53:42.000000 vedo-2023.4.6/examples/basic/distance2mesh.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      574 2023-04-13 18:55:44.000000 vedo-2023.4.6/examples/basic/extrude.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      380 2023-04-13 18:57:36.000000 vedo-2023.4.6/examples/basic/fillholes.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      418 2023-04-13 18:58:26.000000 vedo-2023.4.6/examples/basic/flatarrow.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1058 2023-04-13 19:01:49.000000 vedo-2023.4.6/examples/basic/glyphs1.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1415 2023-04-13 19:03:46.000000 vedo-2023.4.6/examples/basic/glyphs_arrows.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      765 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/basic/hover_legend.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1103 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/basic/input_box.py
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)      523 2023-04-05 18:39:17.000000 vedo-2023.4.6/examples/basic/interaction_modes.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      810 2023-03-23 11:19:03.000000 vedo-2023.4.6/examples/basic/keypress.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      435 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/basic/largestregion.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      623 2022-12-07 16:21:23.000000 vedo-2023.4.6/examples/basic/legendbox.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      359 2022-03-17 20:05:40.000000 vedo-2023.4.6/examples/basic/lightings.py
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)      799 2021-05-04 16:06:12.000000 vedo-2023.4.6/examples/basic/lights.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      651 2022-10-23 14:51:55.000000 vedo-2023.4.6/examples/basic/lin_interpolate.py
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)      463 2023-04-27 17:09:43.000000 vedo-2023.4.6/examples/basic/manypoints.py
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)      684 2022-06-06 19:09:50.000000 vedo-2023.4.6/examples/basic/manyspheres.py
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)      531 2021-09-08 14:00:59.000000 vedo-2023.4.6/examples/basic/mesh_alphas.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1133 2023-05-28 11:38:19.000000 vedo-2023.4.6/examples/basic/mesh_coloring.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      957 2023-02-17 17:32:23.000000 vedo-2023.4.6/examples/basic/mesh_custom.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1374 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/basic/mesh_lut.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      683 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/basic/mesh_map2cell.py
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)     1537 2021-03-06 18:56:56.000000 vedo-2023.4.6/examples/basic/mesh_merge_vs_assembly.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      356 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/basic/mesh_modify.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      545 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/basic/mesh_sharemap.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      548 2023-02-17 15:02:14.000000 vedo-2023.4.6/examples/basic/mesh_threshold.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      323 2023-02-02 21:20:57.000000 vedo-2023.4.6/examples/basic/mirror.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      813 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/basic/mouseclick.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      705 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/basic/mousehighlight.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      766 2023-02-27 11:30:28.000000 vedo-2023.4.6/examples/basic/mousehover0.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1460 2023-03-23 11:21:41.000000 vedo-2023.4.6/examples/basic/mousehover1.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      805 2023-03-23 11:22:10.000000 vedo-2023.4.6/examples/basic/mousehover2.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1300 2023-03-23 11:23:21.000000 vedo-2023.4.6/examples/basic/mousehover3.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1110 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/basic/multirenderers.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1523 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/basic/multiwindows1.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      839 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/basic/multiwindows2.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      563 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/basic/pca_ellipse.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1336 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/basic/pca_ellipsoid.py
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)      495 2022-01-27 19:58:01.000000 vedo-2023.4.6/examples/basic/record_play.py
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)      532 2022-03-19 14:51:42.000000 vedo-2023.4.6/examples/basic/ribbon.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      388 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/basic/rotate_image.py
+-rwxr-x---   0 musy      (8766) sharpe    (4311)      182 2023-01-18 12:46:24.000000 vedo-2023.4.6/examples/basic/run_all.sh
+-rw-r-----   0 musy      (8766) sharpe    (4311)      859 2023-05-28 11:39:11.000000 vedo-2023.4.6/examples/basic/scalarbars.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      353 2023-05-26 16:18:15.000000 vedo-2023.4.6/examples/basic/shadow1.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      564 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/basic/shadow2.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      505 2023-01-09 14:44:11.000000 vedo-2023.4.6/examples/basic/shadow3.py
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)      207 2021-05-04 16:06:12.000000 vedo-2023.4.6/examples/basic/shrink.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      478 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/basic/silhouette1.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1561 2023-02-16 17:23:28.000000 vedo-2023.4.6/examples/basic/silhouette2.py
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)      349 2022-02-24 21:54:41.000000 vedo-2023.4.6/examples/basic/silhouette3.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      474 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/basic/skybox.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      971 2023-03-23 11:24:13.000000 vedo-2023.4.6/examples/basic/slider_browser.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      614 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/basic/sliders1.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1432 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/basic/sliders2.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      513 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/basic/sliders3d.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1661 2023-02-17 15:13:17.000000 vedo-2023.4.6/examples/basic/sliders_hsv.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      897 2023-04-05 13:32:34.000000 vedo-2023.4.6/examples/basic/sliders_range.py
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)      649 2022-01-27 20:22:57.000000 vedo-2023.4.6/examples/basic/specular.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      667 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/basic/spline_tool.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      536 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/basic/ssao.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      348 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/basic/surf_intersect.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      776 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/basic/texture_coords.py
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)      504 2022-06-06 19:09:50.000000 vedo-2023.4.6/examples/basic/texturecubes.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      773 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/basic/tube_radii.py
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)      429 2022-10-18 18:03:39.000000 vedo-2023.4.6/examples/basic/voronoi1.py
+drwxr-x---   0 musy      (8766) sharpe    (4311)        0 2023-06-21 17:43:43.544463 vedo-2023.4.6/examples/other/
+-rw-r-----   0 musy      (8766) sharpe    (4311)       97 2023-06-21 16:52:34.000000 vedo-2023.4.6/examples/other/.polyscope.ini
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)        5 2022-06-06 19:09:50.000000 vedo-2023.4.6/examples/other/__init__.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      669 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/other/clone2d.py
+drwxr-x---   0 musy      (8766) sharpe    (4311)        0 2023-06-21 17:43:43.548463 vedo-2023.4.6/examples/other/dolfin/
+-rw-r-----   0 musy      (8766) sharpe    (4311)      504 2023-02-03 17:02:08.000000 vedo-2023.4.6/examples/other/dolfin/README.md
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)        3 2021-03-06 19:00:03.000000 vedo-2023.4.6/examples/other/dolfin/__init__.py
+-rw-r--r--   0 musy      (8766) sharpe    (4311)      446 2021-03-06 19:00:03.000000 vedo-2023.4.6/examples/other/dolfin/ascalarbar.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     3266 2023-01-27 15:42:02.000000 vedo-2023.4.6/examples/other/dolfin/awefem.py
+-rw-r--r--   0 musy      (8766) sharpe    (4311)     1135 2021-03-06 19:00:03.000000 vedo-2023.4.6/examples/other/dolfin/calc_surface_area.py
+-rw-r--r--   0 musy      (8766) sharpe    (4311)     1072 2021-03-06 19:00:03.000000 vedo-2023.4.6/examples/other/dolfin/collisions.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1024 2023-01-27 15:42:02.000000 vedo-2023.4.6/examples/other/dolfin/demo_eigenvalue.py
+-rw-r--r--   0 musy      (8766) sharpe    (4311)     1035 2021-03-06 19:00:03.000000 vedo-2023.4.6/examples/other/dolfin/demo_submesh.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1845 2023-01-27 15:42:02.000000 vedo-2023.4.6/examples/other/dolfin/elasticbeam.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     6528 2023-01-27 15:42:02.000000 vedo-2023.4.6/examples/other/dolfin/elastodynamics.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1385 2022-05-08 22:18:28.000000 vedo-2023.4.6/examples/other/dolfin/ex03_poisson.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1977 2023-01-27 15:42:02.000000 vedo-2023.4.6/examples/other/dolfin/ex04_mixed-poisson.py
+-rw-r--r--   0 musy      (8766) sharpe    (4311)     1575 2021-03-06 19:00:03.000000 vedo-2023.4.6/examples/other/dolfin/ex06_elasticity1.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1064 2023-03-14 18:26:09.000000 vedo-2023.4.6/examples/other/dolfin/ex06_elasticity2.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     3431 2023-01-20 17:19:50.000000 vedo-2023.4.6/examples/other/dolfin/ex06_elasticity3.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     2415 2023-03-02 20:08:18.000000 vedo-2023.4.6/examples/other/dolfin/ex06_elasticity4.py
+-rw-r--r--   0 musy      (8766) sharpe    (4311)     2070 2022-05-08 22:20:34.000000 vedo-2023.4.6/examples/other/dolfin/ex07_stokes-iterative.py
+-rw-r--r--   0 musy      (8766) sharpe    (4311)     1580 2021-03-06 19:00:03.000000 vedo-2023.4.6/examples/other/dolfin/ft02_poisson_membrane.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1537 2022-03-17 20:16:09.000000 vedo-2023.4.6/examples/other/dolfin/ft04_heat_gaussian.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     2943 2023-01-27 15:42:02.000000 vedo-2023.4.6/examples/other/dolfin/ft09_reaction_system.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     2622 2023-01-27 15:42:02.000000 vedo-2023.4.6/examples/other/dolfin/heatconv.py
+-rw-r--r--   0 musy      (8766) sharpe    (4311)     2916 2021-03-06 19:00:03.000000 vedo-2023.4.6/examples/other/dolfin/magnetostatics.py
+-rw-r--r--   0 musy      (8766) sharpe    (4311)      455 2021-03-06 19:00:03.000000 vedo-2023.4.6/examples/other/dolfin/markmesh.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     2899 2023-01-27 15:42:02.000000 vedo-2023.4.6/examples/other/dolfin/navier-stokes_lshape.py
+-rw-r--r--   0 musy      (8766) sharpe    (4311)      462 2021-03-06 19:00:03.000000 vedo-2023.4.6/examples/other/dolfin/nodal_u.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      630 2023-01-27 15:42:02.000000 vedo-2023.4.6/examples/other/dolfin/pi_estimate.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1532 2023-01-27 15:42:02.000000 vedo-2023.4.6/examples/other/dolfin/pointLoad.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1120 2023-01-27 15:42:02.000000 vedo-2023.4.6/examples/other/dolfin/read_image.py
+-rwxr-xr-x   0 musy      (8766) sharpe    (4311)     1968 2023-06-21 10:21:22.000000 vedo-2023.4.6/examples/other/dolfin/run_all.sh
+-rw-r-----   0 musy      (8766) sharpe    (4311)      670 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/other/dolfin/scalemesh.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     2549 2023-01-27 15:42:02.000000 vedo-2023.4.6/examples/other/dolfin/stokes1.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1246 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/other/dolfin/stokes2.py
+-rw-r--r--   0 musy      (8766) sharpe    (4311)      818 2021-03-06 19:00:03.000000 vedo-2023.4.6/examples/other/dolfin/submesh_boundary.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     2471 2023-01-27 15:42:02.000000 vedo-2023.4.6/examples/other/dolfin/turing_2d.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     2461 2023-04-17 12:22:50.000000 vedo-2023.4.6/examples/other/dolfin/turing_3d.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      774 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/other/ellipt_fourier_desc.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      474 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/other/export_numpy.py
+-rw-r--r--   0 musy      (8766) sharpe    (4311)      653 2022-04-05 19:15:36.000000 vedo-2023.4.6/examples/other/export_x3d.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      939 2022-12-09 20:52:34.000000 vedo-2023.4.6/examples/other/flag_labels1.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      422 2022-12-07 20:53:49.000000 vedo-2023.4.6/examples/other/flag_labels2.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      330 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/other/icon.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      175 2023-06-21 16:52:33.000000 vedo-2023.4.6/examples/other/imgui.ini
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)      841 2021-05-04 16:06:12.000000 vedo-2023.4.6/examples/other/iminuit1.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1127 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/other/inset.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1797 2023-02-27 12:54:07.000000 vedo-2023.4.6/examples/other/make_video.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      398 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/other/meshio_read.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1900 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/other/morphomatics_regression.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1328 2022-10-21 13:11:03.000000 vedo-2023.4.6/examples/other/morphomatics_tube.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      791 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/other/napari1.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      907 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/other/nevergrad_opt.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1190 2023-03-23 15:07:49.000000 vedo-2023.4.6/examples/other/printc.py
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)      529 2022-06-06 19:09:50.000000 vedo-2023.4.6/examples/other/pygeodesic1.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1030 2023-06-15 12:18:25.000000 vedo-2023.4.6/examples/other/pygmsh_cut.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      958 2023-01-08 20:24:11.000000 vedo-2023.4.6/examples/other/pymeshlab1.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      609 2023-01-08 20:24:00.000000 vedo-2023.4.6/examples/other/pymeshlab2.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1743 2023-06-15 12:22:12.000000 vedo-2023.4.6/examples/other/qt_cutter.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     4000 2023-01-09 14:49:35.000000 vedo-2023.4.6/examples/other/qt_tabs.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1984 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/other/qt_window1.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1819 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/other/qt_window2.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1713 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/other/qt_window3.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      508 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/other/remesh_ACVD.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1095 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/other/remesh_meshfix.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1563 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/other/remesh_tetgen.py
+-rwxrwxr-x   0 musy      (8766) sharpe    (4311)     1040 2022-12-15 17:42:58.000000 vedo-2023.4.6/examples/other/run_all.sh
+-rw-r-----   0 musy      (8766) sharpe    (4311)   156522 2023-06-21 16:53:07.000000 vedo-2023.4.6/examples/other/scene.npz
+-rw-r-----   0 musy      (8766) sharpe    (4311)     3119 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/other/spherical_harmonics1.py
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)      217 2022-11-27 17:34:53.000000 vedo-2023.4.6/examples/other/tensor_grid1.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     4769 2023-04-17 17:54:59.000000 vedo-2023.4.6/examples/other/tensor_grid2.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      770 2023-02-02 19:37:56.000000 vedo-2023.4.6/examples/other/trame_ex1.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      878 2023-02-02 21:28:33.000000 vedo-2023.4.6/examples/other/trame_ex2.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     2285 2023-02-02 21:16:56.000000 vedo-2023.4.6/examples/other/trame_ex3.py
+drwxr-x---   0 musy      (8766) sharpe    (4311)        0 2023-06-21 17:43:43.552463 vedo-2023.4.6/examples/other/trimesh/
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1832 2022-11-07 13:12:03.000000 vedo-2023.4.6/examples/other/trimesh/README.md
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)        5 2022-06-06 19:09:50.000000 vedo-2023.4.6/examples/other/trimesh/__init__.py
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)     1193 2022-06-06 19:09:50.000000 vedo-2023.4.6/examples/other/trimesh/nearest.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1164 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/other/trimesh/ray.py
+-rwxrwxr-x   0 musy      (8766) sharpe    (4311)      254 2022-08-14 19:31:52.000000 vedo-2023.4.6/examples/other/trimesh/run_all.sh
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1628 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/other/trimesh/section.py
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)     1193 2022-06-06 19:09:50.000000 vedo-2023.4.6/examples/other/trimesh/shortest.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      688 2023-04-03 11:58:30.000000 vedo-2023.4.6/examples/other/vpolyscope.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1610 2023-05-26 16:42:31.000000 vedo-2023.4.6/examples/other/wx_window1.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1726 2022-12-07 19:20:10.000000 vedo-2023.4.6/examples/other/wx_window2.py
+drwxr-x---   0 musy      (8766) sharpe    (4311)        0 2023-06-21 17:43:43.556463 vedo-2023.4.6/examples/pyplot/
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)        3 2021-01-14 20:43:53.000000 vedo-2023.4.6/examples/pyplot/__init__.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     2684 2023-02-16 17:49:40.000000 vedo-2023.4.6/examples/pyplot/anim_lines.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      663 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/pyplot/caption.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     2059 2023-02-16 17:43:20.000000 vedo-2023.4.6/examples/pyplot/custom_axes1.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      987 2023-02-16 17:44:53.000000 vedo-2023.4.6/examples/pyplot/custom_axes2.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      779 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/pyplot/custom_axes3.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1078 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/pyplot/custom_axes4.py
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)      280 2022-02-25 13:08:22.000000 vedo-2023.4.6/examples/pyplot/donut.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     2167 2023-04-17 13:00:20.000000 vedo-2023.4.6/examples/pyplot/earthquake_browser.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      561 2023-03-09 15:49:39.000000 vedo-2023.4.6/examples/pyplot/embed_matplotlib.py
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)     1896 2023-04-27 17:11:39.000000 vedo-2023.4.6/examples/pyplot/explore5d.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      827 2022-11-17 21:02:52.000000 vedo-2023.4.6/examples/pyplot/fill_gap.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      848 2023-03-10 19:38:14.000000 vedo-2023.4.6/examples/pyplot/fit_circle.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      944 2022-10-26 16:27:11.000000 vedo-2023.4.6/examples/pyplot/fit_curve.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1126 2023-04-30 20:06:51.000000 vedo-2023.4.6/examples/pyplot/fit_erf.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1477 2023-02-17 15:30:35.000000 vedo-2023.4.6/examples/pyplot/fit_polynomial1.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1955 2023-02-17 15:31:18.000000 vedo-2023.4.6/examples/pyplot/fit_polynomial2.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     3836 2023-02-16 17:41:47.000000 vedo-2023.4.6/examples/pyplot/fonts3d.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     2341 2023-03-23 11:26:07.000000 vedo-2023.4.6/examples/pyplot/fourier_epicycles.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      801 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/pyplot/glyphs3.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      948 2023-02-17 15:33:49.000000 vedo-2023.4.6/examples/pyplot/goniometer.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1001 2023-06-18 13:16:30.000000 vedo-2023.4.6/examples/pyplot/graph_lineage.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1662 2023-06-18 13:18:08.000000 vedo-2023.4.6/examples/pyplot/graph_network.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)       98 2022-04-06 10:06:05.000000 vedo-2023.4.6/examples/pyplot/histo_1d_a.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      947 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/pyplot/histo_1d_b.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      881 2023-02-17 15:35:41.000000 vedo-2023.4.6/examples/pyplot/histo_1d_c.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1120 2023-04-30 20:16:33.000000 vedo-2023.4.6/examples/pyplot/histo_1d_d.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      797 2023-04-13 15:13:03.000000 vedo-2023.4.6/examples/pyplot/histo_1d_e.py
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)      597 2022-03-29 11:28:28.000000 vedo-2023.4.6/examples/pyplot/histo_2d_a.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      550 2022-11-08 11:49:50.000000 vedo-2023.4.6/examples/pyplot/histo_2d_b.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      547 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/pyplot/histo_3d.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      798 2022-11-17 21:03:22.000000 vedo-2023.4.6/examples/pyplot/histo_gauss.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      575 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/pyplot/histo_hexagonal.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     2599 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/pyplot/histo_manual.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1166 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/pyplot/histo_pca.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1332 2023-02-17 17:17:57.000000 vedo-2023.4.6/examples/pyplot/histo_polar.py
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)      364 2022-10-28 11:18:51.000000 vedo-2023.4.6/examples/pyplot/histo_spheric.py
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)      583 2022-03-21 12:35:17.000000 vedo-2023.4.6/examples/pyplot/histo_violin.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1143 2023-02-16 17:46:00.000000 vedo-2023.4.6/examples/pyplot/intersect2d.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1159 2023-03-10 19:39:34.000000 vedo-2023.4.6/examples/pyplot/isolines.py
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)      652 2022-04-04 18:51:43.000000 vedo-2023.4.6/examples/pyplot/latex.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      906 2023-03-14 18:39:00.000000 vedo-2023.4.6/examples/pyplot/lines_intersect.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      415 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/pyplot/markers.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      413 2023-02-02 19:24:07.000000 vedo-2023.4.6/examples/pyplot/markpoint.py
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)      556 2023-02-17 15:38:52.000000 vedo-2023.4.6/examples/pyplot/np_matrix.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      946 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/pyplot/plot_bars.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      804 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/pyplot/plot_density2d.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      577 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/pyplot/plot_density3d.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1012 2023-03-23 11:26:39.000000 vedo-2023.4.6/examples/pyplot/plot_density4d.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1049 2023-04-30 20:19:11.000000 vedo-2023.4.6/examples/pyplot/plot_empty.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1371 2023-05-30 16:11:07.000000 vedo-2023.4.6/examples/pyplot/plot_errband.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1147 2023-02-17 15:40:26.000000 vedo-2023.4.6/examples/pyplot/plot_errbars.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1792 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/pyplot/plot_extra_yaxis.py
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)     1350 2023-03-14 18:37:56.000000 vedo-2023.4.6/examples/pyplot/plot_fxy.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      692 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/pyplot/plot_hexcells.py
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)      537 2022-04-04 19:10:12.000000 vedo-2023.4.6/examples/pyplot/plot_multi.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      877 2022-11-18 17:33:00.000000 vedo-2023.4.6/examples/pyplot/plot_pip.py
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)      586 2022-03-21 12:35:46.000000 vedo-2023.4.6/examples/pyplot/plot_polar.py
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)      761 2021-05-04 16:06:12.000000 vedo-2023.4.6/examples/pyplot/plot_spheric.py
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)      624 2023-06-18 13:19:08.000000 vedo-2023.4.6/examples/pyplot/plot_stream.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      256 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/pyplot/quiver.py
+-rwxr-xr-x   0 musy      (8766) sharpe    (4311)      279 2021-10-05 17:36:39.000000 vedo-2023.4.6/examples/pyplot/run_all.sh
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)      397 2022-03-29 23:31:38.000000 vedo-2023.4.6/examples/pyplot/scatter1.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1312 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/pyplot/scatter2.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1003 2023-04-30 20:26:37.000000 vedo-2023.4.6/examples/pyplot/scatter3.py
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)      501 2022-06-06 19:09:50.000000 vedo-2023.4.6/examples/pyplot/scatter_large.py
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)      421 2022-03-20 22:00:43.000000 vedo-2023.4.6/examples/pyplot/triangulate2d.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1476 2023-02-16 17:50:52.000000 vedo-2023.4.6/examples/pyplot/whiskers.py
+drwxr-x---   0 musy      (8766) sharpe    (4311)        0 2023-06-21 17:43:43.560463 vedo-2023.4.6/examples/simulations/
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)        3 2021-03-06 18:59:20.000000 vedo-2023.4.6/examples/simulations/__init__.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      556 2023-06-18 13:45:53.000000 vedo-2023.4.6/examples/simulations/airplane1.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      876 2023-06-18 13:50:37.000000 vedo-2023.4.6/examples/simulations/airplane2.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1189 2023-06-02 13:45:59.000000 vedo-2023.4.6/examples/simulations/aspring1.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1570 2023-06-05 14:34:00.000000 vedo-2023.4.6/examples/simulations/aspring2_player.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     4596 2023-02-05 18:12:21.000000 vedo-2023.4.6/examples/simulations/brownian2d.py
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)     2125 2022-02-24 19:44:14.000000 vedo-2023.4.6/examples/simulations/doubleslit.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      721 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/simulations/drag_chain.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     4999 2023-06-15 17:09:37.000000 vedo-2023.4.6/examples/simulations/gas.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     2889 2023-01-07 21:26:46.000000 vedo-2023.4.6/examples/simulations/grayscott.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     2440 2023-02-16 19:03:31.000000 vedo-2023.4.6/examples/simulations/gyroscope1.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     2896 2023-03-23 11:27:28.000000 vedo-2023.4.6/examples/simulations/gyroscope2.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     2113 2023-01-30 20:16:44.000000 vedo-2023.4.6/examples/simulations/hanoi3d.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      994 2023-01-20 17:18:38.000000 vedo-2023.4.6/examples/simulations/koch_fractal.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1103 2023-05-26 16:37:59.000000 vedo-2023.4.6/examples/simulations/lorenz.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     2120 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/simulations/mag_field1.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      781 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/simulations/mag_field2.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     4367 2023-02-16 18:41:40.000000 vedo-2023.4.6/examples/simulations/multiple_pendulum.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)    11430 2023-01-18 12:46:24.000000 vedo-2023.4.6/examples/simulations/optics_base.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     4261 2022-10-26 14:34:00.000000 vedo-2023.4.6/examples/simulations/optics_main1.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     2124 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/simulations/optics_main2.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1423 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/simulations/optics_main3.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     4194 2023-06-18 13:29:08.000000 vedo-2023.4.6/examples/simulations/particle_simulator.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1155 2023-06-18 14:08:54.000000 vedo-2023.4.6/examples/simulations/pendulum_3d.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1886 2023-02-05 18:10:20.000000 vedo-2023.4.6/examples/simulations/pendulum_ode.py
+-rwxr-xr-x   0 musy      (8766) sharpe    (4311)      279 2021-10-05 17:36:43.000000 vedo-2023.4.6/examples/simulations/run_all.sh
+-rw-r-----   0 musy      (8766) sharpe    (4311)     2697 2023-05-26 16:41:55.000000 vedo-2023.4.6/examples/simulations/self_org_maps2d.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      859 2023-02-17 17:01:30.000000 vedo-2023.4.6/examples/simulations/spline_ease.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      564 2023-06-18 13:24:19.000000 vedo-2023.4.6/examples/simulations/trail.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1665 2022-11-18 16:09:52.000000 vedo-2023.4.6/examples/simulations/tunnelling1.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     2800 2023-05-26 16:39:36.000000 vedo-2023.4.6/examples/simulations/tunnelling2.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     4456 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/simulations/value_iteration.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     2121 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/simulations/volterra.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     3610 2023-02-05 18:08:51.000000 vedo-2023.4.6/examples/simulations/wave_equation1d.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1656 2023-01-07 21:26:46.000000 vedo-2023.4.6/examples/simulations/wave_equation2d.py
+drwxr-x---   0 musy      (8766) sharpe    (4311)        0 2023-06-21 17:43:43.564463 vedo-2023.4.6/examples/volumetric/
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)        3 2021-03-06 19:00:26.000000 vedo-2023.4.6/examples/volumetric/__init__.py
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)      244 2023-03-15 13:47:09.000000 vedo-2023.4.6/examples/volumetric/app_isobrowser.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      273 2022-02-09 17:33:21.000000 vedo-2023.4.6/examples/volumetric/app_raycaster.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      919 2023-03-10 19:37:32.000000 vedo-2023.4.6/examples/volumetric/colorize_volume.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      564 2023-02-23 20:04:44.000000 vedo-2023.4.6/examples/volumetric/delaunay3d.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      689 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/volumetric/densifycloud.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     2032 2023-05-28 11:39:57.000000 vedo-2023.4.6/examples/volumetric/earth_model.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      376 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/volumetric/erode_dilate.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      290 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/volumetric/euclidian_dist.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      950 2023-02-23 19:58:20.000000 vedo-2023.4.6/examples/volumetric/image_false_colors.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      652 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/volumetric/image_fft.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1432 2022-11-20 18:06:50.000000 vedo-2023.4.6/examples/volumetric/image_mask.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1387 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/volumetric/image_probe.py
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)      795 2022-12-15 15:46:00.000000 vedo-2023.4.6/examples/volumetric/image_rgba.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      805 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/volumetric/image_to_mesh.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1484 2023-05-28 11:40:21.000000 vedo-2023.4.6/examples/volumetric/interpolate_volume.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      436 2023-06-15 12:19:51.000000 vedo-2023.4.6/examples/volumetric/isosurfaces.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      451 2023-02-17 17:06:54.000000 vedo-2023.4.6/examples/volumetric/legosurface.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      616 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/volumetric/lowpassfilter.py
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)      462 2022-03-19 15:00:10.000000 vedo-2023.4.6/examples/volumetric/mesh2volume.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1208 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/volumetric/multiscalars.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      608 2023-02-23 13:22:42.000000 vedo-2023.4.6/examples/volumetric/numpy2volume1.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      539 2023-02-14 15:11:12.000000 vedo-2023.4.6/examples/volumetric/numpy2volume2.py
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)      521 2022-08-14 19:31:52.000000 vedo-2023.4.6/examples/volumetric/numpy_imread.py
+-rw-r--r--   0 musy      (8766) sharpe    (4311)    10019 2021-03-06 19:00:26.000000 vedo-2023.4.6/examples/volumetric/off_furniture.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      780 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/volumetric/office.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      346 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/volumetric/point_density.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      590 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/volumetric/probe_line1.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      732 2023-02-23 11:27:44.000000 vedo-2023.4.6/examples/volumetric/probe_line2.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      540 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/volumetric/probe_points.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      614 2022-12-15 18:13:49.000000 vedo-2023.4.6/examples/volumetric/read_volume1.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1196 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/volumetric/read_volume2.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1272 2023-05-30 16:00:02.000000 vedo-2023.4.6/examples/volumetric/read_volume3.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      593 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/volumetric/read_vts.py
+-rwxr-xr-x   0 musy      (8766) sharpe    (4311)      281 2021-10-05 17:36:48.000000 vedo-2023.4.6/examples/volumetric/run_all.sh
+-rw-r-----   0 musy      (8766) sharpe    (4311)      299 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/volumetric/slice_mesh.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1037 2023-03-23 11:34:02.000000 vedo-2023.4.6/examples/volumetric/slice_plane1.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      540 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/volumetric/slice_plane2.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      576 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/volumetric/slicer1.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1298 2023-02-03 14:25:42.000000 vedo-2023.4.6/examples/volumetric/slicer2.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      898 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/volumetric/streamlines1.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      781 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/volumetric/streamlines2.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      895 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/volumetric/streamlines3.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      612 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/volumetric/streamlines4.py
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)      811 2022-05-08 19:29:44.000000 vedo-2023.4.6/examples/volumetric/streamribbons.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      615 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/volumetric/tensors.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      619 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/volumetric/tet_astyle.py
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)      936 2021-09-20 16:16:08.000000 vedo-2023.4.6/examples/volumetric/tet_build.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      332 2023-02-16 17:47:52.000000 vedo-2023.4.6/examples/volumetric/tet_cut1.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1002 2023-02-23 15:08:37.000000 vedo-2023.4.6/examples/volumetric/tet_cut2.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1216 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/volumetric/tet_explode.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      485 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/volumetric/tet_isos_slice.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      433 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/volumetric/tet_threshold.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      964 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/volumetric/tetralize_surface.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      201 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/volumetric/ugrid1.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      274 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/volumetric/ugrid2.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      285 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/volumetric/vol2points.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      422 2022-11-14 13:08:27.000000 vedo-2023.4.6/examples/volumetric/volumeFromMesh.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1930 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/volumetric/volume_operations.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      769 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/volumetric/volume_sharemap.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)      369 2022-10-17 16:29:31.000000 vedo-2023.4.6/examples/volumetric/warp_scalars.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)       75 2023-06-21 17:43:43.576463 vedo-2023.4.6/setup.cfg
+-rwxr-x---   0 musy      (8766) sharpe    (4311)     2767 2023-01-18 12:46:24.000000 vedo-2023.4.6/setup.py
+drwxr-x---   0 musy      (8766) sharpe    (4311)        0 2023-06-21 17:43:43.568463 vedo-2023.4.6/vedo/
+-rw-r-----   0 musy      (8766) sharpe    (4311)     3676 2023-06-15 15:37:21.000000 vedo-2023.4.6/vedo/__init__.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)   154478 2023-06-18 15:13:17.000000 vedo-2023.4.6/vedo/addons.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)    67687 2023-06-21 16:14:00.000000 vedo-2023.4.6/vedo/applications.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)    12563 2023-04-28 15:16:08.000000 vedo-2023.4.6/vedo/assembly.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)    14266 2023-06-13 15:58:10.000000 vedo-2023.4.6/vedo/backends.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)    91587 2023-06-20 15:41:29.000000 vedo-2023.4.6/vedo/base.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)    34979 2023-06-20 14:38:02.000000 vedo-2023.4.6/vedo/cli.py
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)   304787 2023-01-27 09:58:59.000000 vedo-2023.4.6/vedo/cmaps.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)    34673 2023-05-01 10:25:38.000000 vedo-2023.4.6/vedo/colors.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)    31737 2023-06-20 16:42:23.000000 vedo-2023.4.6/vedo/dolfin.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)    71365 2023-06-20 11:06:23.000000 vedo-2023.4.6/vedo/file_io.py
+drwxr-x---   0 musy      (8766) sharpe    (4311)        0 2023-06-21 17:43:43.576463 vedo-2023.4.6/vedo/fonts/
+-rw-r-----   0 musy      (8766) sharpe    (4311)    65008 2023-02-08 19:31:34.000000 vedo-2023.4.6/vedo/fonts/Bongas.npz
+-rw-r--r--   0 musy      (8766) sharpe    (4311)    33928 2014-01-28 02:04:38.000000 vedo-2023.4.6/vedo/fonts/Bongas.ttf
+-rw-r-----   0 musy      (8766) sharpe    (4311)    65491 2023-02-08 19:33:53.000000 vedo-2023.4.6/vedo/fonts/Calco.npz
+-rw-r--r--   0 musy      (8766) sharpe    (4311)    65528 2020-06-13 19:22:59.000000 vedo-2023.4.6/vedo/fonts/Calco.ttf
+-rw-r-----   0 musy      (8766) sharpe    (4311)   127729 2023-02-08 19:34:41.000000 vedo-2023.4.6/vedo/fonts/Comae.npz
+-rw-r--r--   0 musy      (8766) sharpe    (4311)    98408 2014-01-28 02:09:20.000000 vedo-2023.4.6/vedo/fonts/Comae.ttf
+-rw-r-----   0 musy      (8766) sharpe    (4311)   153242 2023-02-08 19:37:52.000000 vedo-2023.4.6/vedo/fonts/Glasgo.npz
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)   144352 2017-09-01 17:37:42.000000 vedo-2023.4.6/vedo/fonts/Glasgo.ttf
+-rw-r-----   0 musy      (8766) sharpe    (4311)   196983 2023-02-08 19:52:45.000000 vedo-2023.4.6/vedo/fonts/Kanopus.npz
+-rw-r--r--   0 musy      (8766) sharpe    (4311)   901240 2020-08-12 13:11:07.000000 vedo-2023.4.6/vedo/fonts/Kanopus.ttf
+-rw-r-----   0 musy      (8766) sharpe    (4311)   111014 2023-02-08 19:25:41.000000 vedo-2023.4.6/vedo/fonts/Normografo.npz
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)    52460 2017-08-03 01:32:10.000000 vedo-2023.4.6/vedo/fonts/Normografo.ttf
+-rw-r-----   0 musy      (8766) sharpe    (4311)    95884 2023-02-08 19:50:37.000000 vedo-2023.4.6/vedo/fonts/Quikhand.npz
+-rw-rw-r--   0 musy      (8766) sharpe    (4311)    79328 2020-06-22 00:16:11.000000 vedo-2023.4.6/vedo/fonts/Quikhand.ttf
+-rw-r-----   0 musy      (8766) sharpe    (4311)    91962 2023-02-08 19:47:39.000000 vedo-2023.4.6/vedo/fonts/SmartCouric.npz
+-rw-r--r--   0 musy      (8766) sharpe    (4311)    98156 2020-07-27 12:20:22.000000 vedo-2023.4.6/vedo/fonts/SmartCouric.ttf
+-rw-r-----   0 musy      (8766) sharpe    (4311)   110904 2023-02-08 19:45:55.000000 vedo-2023.4.6/vedo/fonts/Theemim.npz
+-rw-r--r--   0 musy      (8766) sharpe    (4311)   169668 2013-06-04 12:17:38.000000 vedo-2023.4.6/vedo/fonts/Theemim.ttf
+-rw-r-----   0 musy      (8766) sharpe    (4311)   134429 2023-02-08 19:55:49.000000 vedo-2023.4.6/vedo/fonts/VictorMono.npz
+-rw-r--r--   0 musy      (8766) sharpe    (4311)   153724 2020-06-29 16:12:20.000000 vedo-2023.4.6/vedo/fonts/VictorMono.ttf
+-rw-r-----   0 musy      (8766) sharpe    (4311)    46534 2023-06-16 16:54:47.000000 vedo-2023.4.6/vedo/interactor_modes.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)   104013 2023-06-16 14:53:23.000000 vedo-2023.4.6/vedo/mesh.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)    51186 2023-05-25 18:17:11.000000 vedo-2023.4.6/vedo/picture.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)   152097 2023-06-21 09:02:58.000000 vedo-2023.4.6/vedo/plotter.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)   184341 2023-06-18 13:52:48.000000 vedo-2023.4.6/vedo/pointcloud.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)   145381 2023-05-30 16:09:41.000000 vedo-2023.4.6/vedo/pyplot.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)    23633 2023-06-13 18:44:02.000000 vedo-2023.4.6/vedo/settings.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)   160688 2023-06-16 12:40:01.000000 vedo-2023.4.6/vedo/shapes.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)    17315 2023-05-01 09:58:04.000000 vedo-2023.4.6/vedo/tetmesh.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)    12955 2023-05-01 09:57:55.000000 vedo-2023.4.6/vedo/ugrid.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)    88404 2023-05-19 15:16:12.000000 vedo-2023.4.6/vedo/utils.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)       22 2023-06-21 17:42:43.000000 vedo-2023.4.6/vedo/version.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)    61924 2023-06-19 12:39:31.000000 vedo-2023.4.6/vedo/volume.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)    13196 2023-06-15 11:20:58.000000 vedo-2023.4.6/vedo/vtkclasses.py
+drwxr-x---   0 musy      (8766) sharpe    (4311)        0 2023-06-21 17:43:43.568463 vedo-2023.4.6/vedo.egg-info/
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1249 2023-06-21 17:43:43.000000 vedo-2023.4.6/vedo.egg-info/PKG-INFO
+-rw-r-----   0 musy      (8766) sharpe    (4311)    13791 2023-06-21 17:43:43.000000 vedo-2023.4.6/vedo.egg-info/SOURCES.txt
+-rw-r-----   0 musy      (8766) sharpe    (4311)        1 2023-06-21 17:43:43.000000 vedo-2023.4.6/vedo.egg-info/dependency_links.txt
+-rw-r-----   0 musy      (8766) sharpe    (4311)       46 2023-06-21 17:43:43.000000 vedo-2023.4.6/vedo.egg-info/entry_points.txt
+-rw-r-----   0 musy      (8766) sharpe    (4311)       30 2023-06-21 17:43:43.000000 vedo-2023.4.6/vedo.egg-info/requires.txt
+-rw-r-----   0 musy      (8766) sharpe    (4311)        5 2023-06-21 17:43:43.000000 vedo-2023.4.6/vedo.egg-info/top_level.txt
```

### Comparing `vedo-2023.4.5/FONT.LICENSE` & `vedo-2023.4.6/FONT.LICENSE`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/LICENSE` & `vedo-2023.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/PKG-INFO` & `vedo-2023.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vedo
-Version: 2023.4.5
+Version: 2023.4.6
 Summary: A python module for scientific analysis and visualization of 3D objects and point clouds based on VTK.
 Home-page: https://github.com/marcomusy/vedo
 Author: Marco Musy
 Author-email: marco.musy@embl.es
 Maintainer: Marco Musy
 License: MIT
 Keywords: vtk 3D science analysis visualization mesh numpy
```

### Comparing `vedo-2023.4.5/README.md` & `vedo-2023.4.6/README.md`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/advanced/capping_mesh.py` & `vedo-2023.4.6/examples/advanced/capping_mesh.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/advanced/contours2mesh.py` & `vedo-2023.4.6/examples/advanced/contours2mesh.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/advanced/cut_with_mesh1.py` & `vedo-2023.4.6/examples/advanced/cut_with_mesh1.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/advanced/fitline.py` & `vedo-2023.4.6/examples/advanced/fitline.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/advanced/fitplanes.py` & `vedo-2023.4.6/examples/advanced/fitplanes.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/advanced/fitspheres1.py` & `vedo-2023.4.6/examples/advanced/fitspheres1.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/advanced/fitspheres2.py` & `vedo-2023.4.6/examples/advanced/fitspheres2.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/advanced/geodesic.py` & `vedo-2023.4.6/examples/advanced/geodesic.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/advanced/geological_model.py` & `vedo-2023.4.6/examples/advanced/geological_model.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/advanced/gyroid.py` & `vedo-2023.4.6/examples/advanced/gyroid.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/advanced/interpolate_field.py` & `vedo-2023.4.6/examples/advanced/interpolate_field.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/advanced/interpolate_scalar1.py` & `vedo-2023.4.6/examples/advanced/interpolate_scalar1.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/advanced/interpolate_scalar2.py` & `vedo-2023.4.6/examples/advanced/interpolate_scalar2.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/advanced/interpolate_scalar3.py` & `vedo-2023.4.6/examples/advanced/interpolate_scalar3.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/advanced/interpolate_scalar4.py` & `vedo-2023.4.6/examples/advanced/interpolate_scalar4.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/advanced/line2mesh_quads.py` & `vedo-2023.4.6/examples/advanced/line2mesh_quads.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/advanced/line2mesh_tri.py` & `vedo-2023.4.6/examples/advanced/line2mesh_tri.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/advanced/measure_curvature.py` & `vedo-2023.4.6/examples/advanced/measure_curvature.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/advanced/mesh_smoother2.py` & `vedo-2023.4.6/examples/advanced/mesh_smoother2.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/advanced/meshquality.py` & `vedo-2023.4.6/examples/advanced/meshquality.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/advanced/moving_least_squares1D.py` & `vedo-2023.4.6/examples/advanced/moving_least_squares1D.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/advanced/moving_least_squares2D.py` & `vedo-2023.4.6/examples/advanced/moving_least_squares2D.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/advanced/multi_viewer2.py` & `vedo-2023.4.6/examples/advanced/multi_viewer2.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/advanced/recosurface.py` & `vedo-2023.4.6/examples/advanced/recosurface.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/advanced/spline_draw.py` & `vedo-2023.4.6/examples/advanced/spline_draw.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/advanced/timer_callback1.py` & `vedo-2023.4.6/examples/advanced/timer_callback1.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/advanced/timer_callback2.py` & `vedo-2023.4.6/examples/advanced/timer_callback2.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/advanced/timer_callback3.py` & `vedo-2023.4.6/examples/advanced/timer_callback3.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/advanced/voronoi2.py` & `vedo-2023.4.6/examples/advanced/voronoi2.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/advanced/warp1.py` & `vedo-2023.4.6/examples/advanced/warp1.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/advanced/warp2.py` & `vedo-2023.4.6/examples/advanced/warp2.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/advanced/warp3.py` & `vedo-2023.4.6/examples/advanced/warp3.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/advanced/warp4.py` & `vedo-2023.4.6/examples/advanced/warp4.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/advanced/warp5.py` & `vedo-2023.4.6/examples/advanced/warp5.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/advanced/warp6.py` & `vedo-2023.4.6/examples/advanced/warp6.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/.vedo_pipeline_graphviz` & `vedo-2023.4.6/examples/basic/.vedo_pipeline_graphviz`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/.vedo_pipeline_graphviz.pdf` & `vedo-2023.4.6/examples/basic/.vedo_pipeline_graphviz.pdf`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/.vedo_recorded_events.log` & `vedo-2023.4.6/examples/basic/.vedo_recorded_events.log`

 * *Files 16% similar despite different names*

```diff
@@ -1,77 +1,74 @@
 # StreamVersion 1.2
 ExposeEvent 0 959 0 0 0 0 0
 RenderEvent 0 959 0 0 0 0 0
-LeftButtonPressEvent 434 672 0 0 0 0 0
-StartInteractionEvent 434 672 0 0 0 0 0
-MouseMoveEvent 434 672 0 0 0 0 0
-RenderEvent 434 672 0 0 0 0 0
-InteractionEvent 434 672 0 0 0 0 0
-MouseMoveEvent 434 668 0 0 0 0 0
-RenderEvent 434 668 0 0 0 0 0
-InteractionEvent 434 668 0 0 0 0 0
-MouseMoveEvent 434 663 0 0 0 0 0
-RenderEvent 434 663 0 0 0 0 0
-InteractionEvent 434 663 0 0 0 0 0
-MouseMoveEvent 434 654 0 0 0 0 0
-RenderEvent 434 654 0 0 0 0 0
-InteractionEvent 434 654 0 0 0 0 0
-MouseMoveEvent 434 635 0 0 0 0 0
-RenderEvent 434 635 0 0 0 0 0
-InteractionEvent 434 635 0 0 0 0 0
-MouseMoveEvent 434 614 0 0 0 0 0
-RenderEvent 434 614 0 0 0 0 0
-InteractionEvent 434 614 0 0 0 0 0
-MouseMoveEvent 434 591 0 0 0 0 0
-RenderEvent 434 591 0 0 0 0 0
-InteractionEvent 434 591 0 0 0 0 0
-MouseMoveEvent 434 573 0 0 0 0 0
-RenderEvent 434 573 0 0 0 0 0
-InteractionEvent 434 573 0 0 0 0 0
-MouseMoveEvent 434 550 0 0 0 0 0
-RenderEvent 434 550 0 0 0 0 0
-InteractionEvent 434 550 0 0 0 0 0
-MouseMoveEvent 434 535 0 0 0 0 0
-RenderEvent 434 535 0 0 0 0 0
-InteractionEvent 434 535 0 0 0 0 0
-MouseMoveEvent 432 525 0 0 0 0 0
-RenderEvent 432 525 0 0 0 0 0
-InteractionEvent 432 525 0 0 0 0 0
-MouseMoveEvent 431 518 0 0 0 0 0
-RenderEvent 431 518 0 0 0 0 0
-InteractionEvent 431 518 0 0 0 0 0
-MouseMoveEvent 431 515 0 0 0 0 0
-RenderEvent 431 515 0 0 0 0 0
-InteractionEvent 431 515 0 0 0 0 0
-MouseMoveEvent 431 517 0 0 0 0 0
-RenderEvent 431 517 0 0 0 0 0
-InteractionEvent 431 517 0 0 0 0 0
-MouseMoveEvent 436 526 0 0 0 0 0
-RenderEvent 436 526 0 0 0 0 0
-InteractionEvent 436 526 0 0 0 0 0
-MouseMoveEvent 443 540 0 0 0 0 0
-RenderEvent 443 540 0 0 0 0 0
-InteractionEvent 443 540 0 0 0 0 0
-MouseMoveEvent 457 570 0 0 0 0 0
-RenderEvent 457 570 0 0 0 0 0
-InteractionEvent 457 570 0 0 0 0 0
-MouseMoveEvent 469 597 0 0 0 0 0
-RenderEvent 469 597 0 0 0 0 0
-InteractionEvent 469 597 0 0 0 0 0
-MouseMoveEvent 476 618 0 0 0 0 0
-RenderEvent 476 618 0 0 0 0 0
-InteractionEvent 476 618 0 0 0 0 0
-MouseMoveEvent 479 629 0 0 0 0 0
-RenderEvent 479 629 0 0 0 0 0
-InteractionEvent 479 629 0 0 0 0 0
-MouseMoveEvent 482 637 0 0 0 0 0
-RenderEvent 482 637 0 0 0 0 0
-InteractionEvent 482 637 0 0 0 0 0
-MouseMoveEvent 482 639 0 0 0 0 0
-RenderEvent 482 639 0 0 0 0 0
-InteractionEvent 482 639 0 0 0 0 0
-MouseMoveEvent 483 640 0 0 0 0 0
-RenderEvent 483 640 0 0 0 0 0
-InteractionEvent 483 640 0 0 0 0 0
-LeftButtonReleaseEvent 483 640 0 0 0 0 0
-EndInteractionEvent 483 640 0 0 0 0 0
-RenderEvent 483 640 0 0 0 0 0
+LeftButtonPressEvent 444 571 0 0 0 0 0
+StartInteractionEvent 444 571 0 0 0 0 0
+MouseMoveEvent 444 571 0 0 0 0 0
+RenderEvent 444 571 0 0 0 0 0
+InteractionEvent 444 571 0 0 0 0 0
+MouseMoveEvent 444 569 0 0 0 0 0
+RenderEvent 444 569 0 0 0 0 0
+InteractionEvent 444 569 0 0 0 0 0
+MouseMoveEvent 444 565 0 0 0 0 0
+RenderEvent 444 565 0 0 0 0 0
+InteractionEvent 444 565 0 0 0 0 0
+MouseMoveEvent 444 562 0 0 0 0 0
+RenderEvent 444 562 0 0 0 0 0
+InteractionEvent 444 562 0 0 0 0 0
+MouseMoveEvent 444 558 0 0 0 0 0
+RenderEvent 444 558 0 0 0 0 0
+InteractionEvent 444 558 0 0 0 0 0
+MouseMoveEvent 444 544 0 0 0 0 0
+RenderEvent 444 544 0 0 0 0 0
+InteractionEvent 444 544 0 0 0 0 0
+MouseMoveEvent 444 520 0 0 0 0 0
+RenderEvent 444 520 0 0 0 0 0
+InteractionEvent 444 520 0 0 0 0 0
+MouseMoveEvent 442 498 0 0 0 0 0
+RenderEvent 442 498 0 0 0 0 0
+InteractionEvent 442 498 0 0 0 0 0
+MouseMoveEvent 440 485 0 0 0 0 0
+RenderEvent 440 485 0 0 0 0 0
+InteractionEvent 440 485 0 0 0 0 0
+MouseMoveEvent 437 478 0 0 0 0 0
+RenderEvent 437 478 0 0 0 0 0
+InteractionEvent 437 478 0 0 0 0 0
+MouseMoveEvent 437 477 0 0 0 0 0
+RenderEvent 437 477 0 0 0 0 0
+InteractionEvent 437 477 0 0 0 0 0
+MouseMoveEvent 436 473 0 0 0 0 0
+RenderEvent 436 473 0 0 0 0 0
+InteractionEvent 436 473 0 0 0 0 0
+MouseMoveEvent 434 467 0 0 0 0 0
+RenderEvent 434 467 0 0 0 0 0
+InteractionEvent 434 467 0 0 0 0 0
+MouseMoveEvent 432 459 0 0 0 0 0
+RenderEvent 432 459 0 0 0 0 0
+InteractionEvent 432 459 0 0 0 0 0
+MouseMoveEvent 430 451 0 0 0 0 0
+RenderEvent 430 451 0 0 0 0 0
+InteractionEvent 430 451 0 0 0 0 0
+MouseMoveEvent 429 446 0 0 0 0 0
+RenderEvent 429 446 0 0 0 0 0
+InteractionEvent 429 446 0 0 0 0 0
+MouseMoveEvent 427 442 0 0 0 0 0
+RenderEvent 427 442 0 0 0 0 0
+InteractionEvent 427 442 0 0 0 0 0
+MouseMoveEvent 427 439 0 0 0 0 0
+RenderEvent 427 439 0 0 0 0 0
+InteractionEvent 427 439 0 0 0 0 0
+MouseMoveEvent 426 435 0 0 0 0 0
+RenderEvent 426 435 0 0 0 0 0
+InteractionEvent 426 435 0 0 0 0 0
+MouseMoveEvent 426 434 0 0 0 0 0
+RenderEvent 426 434 0 0 0 0 0
+InteractionEvent 426 434 0 0 0 0 0
+MouseMoveEvent 426 431 0 0 0 0 0
+RenderEvent 426 431 0 0 0 0 0
+InteractionEvent 426 431 0 0 0 0 0
+MouseMoveEvent 426 430 0 0 0 0 0
+RenderEvent 426 430 0 0 0 0 0
+InteractionEvent 426 430 0 0 0 0 0
+LeftButtonReleaseEvent 426 430 0 0 0 0 0
+EndInteractionEvent 426 430 0 0 0 0 0
+RenderEvent 426 430 0 0 0 0 0
```

### Comparing `vedo-2023.4.5/examples/basic/align1.py` & `vedo-2023.4.6/examples/basic/align1.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/align2.py` & `vedo-2023.4.6/examples/basic/align2.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/align3.py` & `vedo-2023.4.6/examples/basic/align3.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/align4.py` & `vedo-2023.4.6/examples/basic/align4.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/align5.py` & `vedo-2023.4.6/examples/basic/align5.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/align6.py` & `vedo-2023.4.6/examples/basic/align6.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/background_image.py` & `vedo-2023.4.6/examples/basic/background_image.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/boolean.py` & `vedo-2023.4.6/examples/basic/boolean.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/boundaries.py` & `vedo-2023.4.6/examples/basic/boundaries.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/buildmesh.py` & `vedo-2023.4.6/examples/basic/buildmesh.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/buttons.py` & `vedo-2023.4.6/examples/basic/buttons.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/cartoony.py` & `vedo-2023.4.6/examples/basic/cartoony.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/cells_within_bounds.py` & `vedo-2023.4.6/examples/basic/cells_within_bounds.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/closewindow.py` & `vedo-2023.4.6/examples/basic/closewindow.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/clustering.py` & `vedo-2023.4.6/examples/basic/clustering.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/color_mesh_cells1.py` & `vedo-2023.4.6/examples/basic/color_mesh_cells1.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/color_mesh_cells2.py` & `vedo-2023.4.6/examples/basic/color_mesh_cells2.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/colorcubes.py` & `vedo-2023.4.6/examples/basic/colorcubes.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/colorlines.py` & `vedo-2023.4.6/examples/basic/colorlines.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/colormap_list.py` & `vedo-2023.4.6/examples/basic/colormap_list.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/colormaps.py` & `vedo-2023.4.6/examples/basic/colormaps.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/connected_vtx.py` & `vedo-2023.4.6/examples/basic/connected_vtx.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/cut_freehand.py` & `vedo-2023.4.6/examples/basic/cut_freehand.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/cut_interactive.py` & `vedo-2023.4.6/examples/basic/cut_interactive.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/delaunay2d.py` & `vedo-2023.4.6/examples/basic/delaunay2d.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/delete_mesh_pts.py` & `vedo-2023.4.6/examples/basic/delete_mesh_pts.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/distance2mesh.py` & `vedo-2023.4.6/examples/basic/distance2mesh.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/extrude.py` & `vedo-2023.4.6/examples/basic/extrude.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/glyphs1.py` & `vedo-2023.4.6/examples/basic/glyphs1.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/glyphs_arrows.py` & `vedo-2023.4.6/examples/basic/glyphs_arrows.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/hover_legend.py` & `vedo-2023.4.6/examples/basic/hover_legend.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/input_box.py` & `vedo-2023.4.6/examples/basic/input_box.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/interaction_modes.py` & `vedo-2023.4.6/examples/basic/interaction_modes.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/keypress.py` & `vedo-2023.4.6/examples/basic/keypress.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/legendbox.py` & `vedo-2023.4.6/examples/basic/legendbox.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/lights.py` & `vedo-2023.4.6/examples/basic/lights.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/lin_interpolate.py` & `vedo-2023.4.6/examples/basic/lin_interpolate.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/manyspheres.py` & `vedo-2023.4.6/examples/basic/manyspheres.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/mesh_alphas.py` & `vedo-2023.4.6/examples/basic/mesh_alphas.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/mesh_coloring.py` & `vedo-2023.4.6/examples/basic/mesh_coloring.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/mesh_custom.py` & `vedo-2023.4.6/examples/basic/mesh_custom.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/mesh_lut.py` & `vedo-2023.4.6/examples/basic/mesh_lut.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/mesh_map2cell.py` & `vedo-2023.4.6/examples/basic/mesh_map2cell.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/mesh_merge_vs_assembly.py` & `vedo-2023.4.6/examples/basic/mesh_merge_vs_assembly.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/mesh_sharemap.py` & `vedo-2023.4.6/examples/basic/mesh_sharemap.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/mesh_threshold.py` & `vedo-2023.4.6/examples/basic/mesh_threshold.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/mouseclick.py` & `vedo-2023.4.6/examples/basic/mouseclick.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/mousehighlight.py` & `vedo-2023.4.6/examples/basic/mousehighlight.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/mousehover0.py` & `vedo-2023.4.6/examples/basic/mousehover0.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/mousehover1.py` & `vedo-2023.4.6/examples/basic/mousehover1.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/mousehover2.py` & `vedo-2023.4.6/examples/basic/mousehover2.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/mousehover3.py` & `vedo-2023.4.6/examples/basic/mousehover3.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/multirenderers.py` & `vedo-2023.4.6/examples/basic/multirenderers.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/multiwindows1.py` & `vedo-2023.4.6/examples/basic/multiwindows1.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/multiwindows2.py` & `vedo-2023.4.6/examples/basic/multiwindows2.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/pca_ellipse.py` & `vedo-2023.4.6/examples/basic/pca_ellipse.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/pca_ellipsoid.py` & `vedo-2023.4.6/examples/basic/pca_ellipsoid.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/ribbon.py` & `vedo-2023.4.6/examples/basic/ribbon.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/scalarbars.py` & `vedo-2023.4.6/examples/basic/scalarbars.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/shadow2.py` & `vedo-2023.4.6/examples/basic/shadow2.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/silhouette2.py` & `vedo-2023.4.6/examples/basic/silhouette2.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/slider_browser.py` & `vedo-2023.4.6/examples/basic/slider_browser.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/sliders1.py` & `vedo-2023.4.6/examples/basic/sliders1.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/sliders2.py` & `vedo-2023.4.6/examples/basic/sliders2.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/sliders3d.py` & `vedo-2023.4.6/examples/basic/sliders3d.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/sliders_hsv.py` & `vedo-2023.4.6/examples/basic/sliders_hsv.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/sliders_range.py` & `vedo-2023.4.6/examples/basic/sliders_range.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/specular.py` & `vedo-2023.4.6/examples/basic/specular.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/spline_tool.py` & `vedo-2023.4.6/examples/basic/spline_tool.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/ssao.py` & `vedo-2023.4.6/examples/basic/ssao.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/texture_coords.py` & `vedo-2023.4.6/examples/basic/texture_coords.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/basic/tube_radii.py` & `vedo-2023.4.6/examples/basic/tube_radii.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/clone2d.py` & `vedo-2023.4.6/examples/other/clone2d.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/dolfin/awefem.py` & `vedo-2023.4.6/examples/other/dolfin/awefem.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/dolfin/calc_surface_area.py` & `vedo-2023.4.6/examples/other/dolfin/calc_surface_area.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/dolfin/collisions.py` & `vedo-2023.4.6/examples/other/dolfin/collisions.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/dolfin/demo_eigenvalue.py` & `vedo-2023.4.6/examples/other/dolfin/demo_eigenvalue.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/dolfin/demo_submesh.py` & `vedo-2023.4.6/examples/other/dolfin/demo_submesh.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/dolfin/elasticbeam.py` & `vedo-2023.4.6/examples/other/dolfin/elasticbeam.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/dolfin/elastodynamics.py` & `vedo-2023.4.6/examples/other/dolfin/elastodynamics.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/dolfin/ex03_poisson.py` & `vedo-2023.4.6/examples/other/dolfin/ex03_poisson.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/dolfin/ex04_mixed-poisson.py` & `vedo-2023.4.6/examples/other/dolfin/ex04_mixed-poisson.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/dolfin/ex06_elasticity1.py` & `vedo-2023.4.6/examples/other/dolfin/ex06_elasticity1.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/dolfin/ex06_elasticity2.py` & `vedo-2023.4.6/examples/other/dolfin/ex06_elasticity2.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/dolfin/ex06_elasticity3.py` & `vedo-2023.4.6/examples/other/dolfin/ex06_elasticity3.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/dolfin/ex06_elasticity4.py` & `vedo-2023.4.6/examples/other/dolfin/ex06_elasticity4.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/dolfin/ex07_stokes-iterative.py` & `vedo-2023.4.6/examples/other/dolfin/ex07_stokes-iterative.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/dolfin/ft02_poisson_membrane.py` & `vedo-2023.4.6/examples/other/dolfin/ft02_poisson_membrane.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/dolfin/ft04_heat_gaussian.py` & `vedo-2023.4.6/examples/other/dolfin/ft04_heat_gaussian.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/dolfin/ft09_reaction_system.py` & `vedo-2023.4.6/examples/other/dolfin/ft09_reaction_system.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/dolfin/heatconv.py` & `vedo-2023.4.6/examples/other/dolfin/heatconv.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/dolfin/magnetostatics.py` & `vedo-2023.4.6/examples/other/dolfin/magnetostatics.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/dolfin/navier-stokes_lshape.py` & `vedo-2023.4.6/examples/other/dolfin/navier-stokes_lshape.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/dolfin/pi_estimate.py` & `vedo-2023.4.6/examples/other/dolfin/pi_estimate.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/dolfin/pointLoad.py` & `vedo-2023.4.6/examples/other/dolfin/pointLoad.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/dolfin/read_image.py` & `vedo-2023.4.6/examples/other/dolfin/read_image.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/dolfin/run_all.sh` & `vedo-2023.4.6/examples/other/dolfin/run_all.sh`

 * *Files 17% similar despite different names*

```diff
@@ -10,44 +10,38 @@
 
 echo Running calc_surface_area.py
 python3 calc_surface_area.py
 
 echo Running markmesh.py
 python3 markmesh.py
 
-echo Running scalemesh.py
-python3 scalemesh.py
+# echo Running scalemesh.py
+# python3 scalemesh.py
 
-echo Running pi_estimate.py
-python3 pi_estimate.py
+# echo Running pi_estimate.py
+# python3 pi_estimate.py
 
-echo Running submesh_boundary.py
-python3 submesh_boundary.py
+# echo Running submesh_boundary.py
+# python3 submesh_boundary.py
 
 echo Running demo_submesh.py
 python3 demo_submesh.py
 
 echo Running elastodynamics.py
 python3 elastodynamics.py
 
 echo Running elasticbeam.py
 python3 elasticbeam.py
 
 echo Running magnetostatics.py
 python3 magnetostatics.py
 
-echo Running curl2d.py
-python3 curl2d.py
-
 echo Running pointLoad.py
 python3 pointLoad.py
 
-echo Running meshEditor.py
-python3 meshEditor.py
-
 echo Running nodal_u.py
 python3 nodal_u.py
 
 echo Running read_image.py
 python3 read_image.py
 
 
@@ -69,16 +63,16 @@
 python3 ex06_elasticity2.py
 
 echo Running ex07_stokes-iterative.py
 python3 ex07_stokes-iterative.py
 
 
 ######################################
-echo Running ft02_poisson_membrane.py
-python3 ft02_poisson_membrane.py
+# echo Running ft02_poisson_membrane.py
+# python3 ft02_poisson_membrane.py
 
 echo Running ft04_heat_gaussian.py
 python3 ft04_heat_gaussian.py
 
 echo Running navier-stokes_lshape.py
 python3 navier-stokes_lshape.py
 
@@ -105,14 +99,7 @@
 
 echo Running awefem.py
 python3 awefem.py
 
 echo Running demo_eigenvalue.py
 python3 demo_eigenvalue.py
 
-echo Running demo_auto-adaptive-poisson.py
-python3 demo_auto-adaptive-poisson.py
-
-
-
-
-
```

### Comparing `vedo-2023.4.5/examples/other/dolfin/scalemesh.py` & `vedo-2023.4.6/examples/other/dolfin/scalemesh.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/dolfin/stokes1.py` & `vedo-2023.4.6/examples/other/dolfin/stokes1.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/dolfin/stokes2.py` & `vedo-2023.4.6/examples/other/dolfin/stokes2.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/dolfin/submesh_boundary.py` & `vedo-2023.4.6/examples/other/dolfin/submesh_boundary.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/dolfin/turing_2d.py` & `vedo-2023.4.6/examples/other/dolfin/turing_2d.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/dolfin/turing_3d.py` & `vedo-2023.4.6/examples/other/dolfin/turing_3d.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/ellipt_fourier_desc.py` & `vedo-2023.4.6/examples/other/ellipt_fourier_desc.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/export_x3d.py` & `vedo-2023.4.6/examples/other/export_x3d.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/flag_labels1.py` & `vedo-2023.4.6/examples/other/flag_labels1.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/iminuit1.py` & `vedo-2023.4.6/examples/other/iminuit1.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/inset.py` & `vedo-2023.4.6/examples/other/inset.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/make_video.py` & `vedo-2023.4.6/examples/other/make_video.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/morphomatics_regression.py` & `vedo-2023.4.6/examples/other/morphomatics_regression.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/morphomatics_tube.py` & `vedo-2023.4.6/examples/other/morphomatics_tube.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/napari1.py` & `vedo-2023.4.6/examples/other/napari1.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/nevergrad_opt.py` & `vedo-2023.4.6/examples/other/nevergrad_opt.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/printc.py` & `vedo-2023.4.6/examples/other/printc.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/pygeodesic1.py` & `vedo-2023.4.6/examples/other/pygeodesic1.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/pygmsh_cut.py` & `vedo-2023.4.6/examples/other/pygmsh_cut.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/pymeshlab1.py` & `vedo-2023.4.6/examples/other/pymeshlab1.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/pymeshlab2.py` & `vedo-2023.4.6/examples/other/pymeshlab2.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/qt_cutter.py` & `vedo-2023.4.6/examples/other/qt_cutter.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/qt_tabs.py` & `vedo-2023.4.6/examples/other/qt_tabs.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/qt_window1.py` & `vedo-2023.4.6/examples/other/qt_window1.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/qt_window2.py` & `vedo-2023.4.6/examples/other/qt_window2.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/qt_window3.py` & `vedo-2023.4.6/examples/other/qt_window3.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/remesh_meshfix.py` & `vedo-2023.4.6/examples/other/remesh_meshfix.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/remesh_tetgen.py` & `vedo-2023.4.6/examples/other/remesh_tetgen.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/run_all.sh` & `vedo-2023.4.6/examples/other/run_all.sh`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/spherical_harmonics1.py` & `vedo-2023.4.6/examples/other/spherical_harmonics1.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/tensor_grid2.py` & `vedo-2023.4.6/examples/other/tensor_grid2.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/trame_ex1.py` & `vedo-2023.4.6/examples/other/trame_ex1.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/trame_ex2.py` & `vedo-2023.4.6/examples/other/trame_ex2.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/trame_ex3.py` & `vedo-2023.4.6/examples/other/trame_ex3.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/trimesh/README.md` & `vedo-2023.4.6/examples/other/trimesh/README.md`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/trimesh/nearest.py` & `vedo-2023.4.6/examples/other/trimesh/nearest.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/trimesh/ray.py` & `vedo-2023.4.6/examples/other/trimesh/ray.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/trimesh/section.py` & `vedo-2023.4.6/examples/other/trimesh/section.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/trimesh/shortest.py` & `vedo-2023.4.6/examples/other/trimesh/shortest.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/vpolyscope.py` & `vedo-2023.4.6/examples/other/vpolyscope.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/wx_window1.py` & `vedo-2023.4.6/examples/other/wx_window1.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/other/wx_window2.py` & `vedo-2023.4.6/examples/other/wx_window2.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/anim_lines.py` & `vedo-2023.4.6/examples/pyplot/anim_lines.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/caption.py` & `vedo-2023.4.6/examples/pyplot/caption.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/custom_axes1.py` & `vedo-2023.4.6/examples/pyplot/custom_axes1.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/custom_axes2.py` & `vedo-2023.4.6/examples/pyplot/custom_axes2.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/custom_axes3.py` & `vedo-2023.4.6/examples/pyplot/custom_axes3.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/custom_axes4.py` & `vedo-2023.4.6/examples/pyplot/custom_axes4.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/earthquake_browser.py` & `vedo-2023.4.6/examples/pyplot/earthquake_browser.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/embed_matplotlib.py` & `vedo-2023.4.6/examples/pyplot/embed_matplotlib.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/explore5d.py` & `vedo-2023.4.6/examples/pyplot/explore5d.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/fill_gap.py` & `vedo-2023.4.6/examples/pyplot/fill_gap.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/fit_circle.py` & `vedo-2023.4.6/examples/pyplot/fit_circle.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/fit_curve.py` & `vedo-2023.4.6/examples/pyplot/fit_curve.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/fit_erf.py` & `vedo-2023.4.6/examples/pyplot/fit_erf.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/fit_polynomial1.py` & `vedo-2023.4.6/examples/pyplot/fit_polynomial1.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/fit_polynomial2.py` & `vedo-2023.4.6/examples/pyplot/fit_polynomial2.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/fonts3d.py` & `vedo-2023.4.6/examples/pyplot/fonts3d.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/fourier_epicycles.py` & `vedo-2023.4.6/examples/pyplot/fourier_epicycles.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/glyphs3.py` & `vedo-2023.4.6/examples/pyplot/glyphs3.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/goniometer.py` & `vedo-2023.4.6/examples/pyplot/goniometer.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/graph_lineage.py` & `vedo-2023.4.6/examples/pyplot/graph_lineage.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/graph_network.py` & `vedo-2023.4.6/examples/pyplot/graph_network.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/histo_1d_b.py` & `vedo-2023.4.6/examples/pyplot/histo_1d_b.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/histo_1d_c.py` & `vedo-2023.4.6/examples/pyplot/histo_1d_c.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/histo_1d_d.py` & `vedo-2023.4.6/examples/pyplot/histo_1d_d.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/histo_1d_e.py` & `vedo-2023.4.6/examples/pyplot/histo_1d_e.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/histo_2d_a.py` & `vedo-2023.4.6/examples/pyplot/histo_2d_a.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/histo_2d_b.py` & `vedo-2023.4.6/examples/pyplot/histo_2d_b.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/histo_3d.py` & `vedo-2023.4.6/examples/pyplot/histo_3d.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/histo_gauss.py` & `vedo-2023.4.6/examples/pyplot/histo_gauss.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/histo_hexagonal.py` & `vedo-2023.4.6/examples/pyplot/histo_hexagonal.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/histo_manual.py` & `vedo-2023.4.6/examples/pyplot/histo_manual.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/histo_pca.py` & `vedo-2023.4.6/examples/pyplot/histo_pca.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/histo_polar.py` & `vedo-2023.4.6/examples/pyplot/histo_polar.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/histo_violin.py` & `vedo-2023.4.6/examples/pyplot/histo_violin.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/intersect2d.py` & `vedo-2023.4.6/examples/pyplot/intersect2d.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/isolines.py` & `vedo-2023.4.6/examples/pyplot/isolines.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/latex.py` & `vedo-2023.4.6/examples/pyplot/latex.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/lines_intersect.py` & `vedo-2023.4.6/examples/pyplot/lines_intersect.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/np_matrix.py` & `vedo-2023.4.6/examples/pyplot/np_matrix.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/plot_bars.py` & `vedo-2023.4.6/examples/pyplot/plot_bars.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/plot_density2d.py` & `vedo-2023.4.6/examples/pyplot/plot_density2d.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/plot_density3d.py` & `vedo-2023.4.6/examples/pyplot/plot_density3d.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/plot_density4d.py` & `vedo-2023.4.6/examples/pyplot/plot_density4d.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/plot_empty.py` & `vedo-2023.4.6/examples/pyplot/plot_empty.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/plot_errband.py` & `vedo-2023.4.6/examples/pyplot/plot_errband.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/plot_errbars.py` & `vedo-2023.4.6/examples/pyplot/plot_errbars.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/plot_extra_yaxis.py` & `vedo-2023.4.6/examples/pyplot/plot_extra_yaxis.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/plot_fxy.py` & `vedo-2023.4.6/examples/pyplot/plot_fxy.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/plot_hexcells.py` & `vedo-2023.4.6/examples/pyplot/plot_hexcells.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/plot_multi.py` & `vedo-2023.4.6/examples/pyplot/plot_multi.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/plot_pip.py` & `vedo-2023.4.6/examples/pyplot/plot_pip.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/plot_polar.py` & `vedo-2023.4.6/examples/pyplot/plot_polar.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/plot_spheric.py` & `vedo-2023.4.6/examples/pyplot/plot_spheric.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/plot_stream.py` & `vedo-2023.4.6/examples/pyplot/plot_stream.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/scatter2.py` & `vedo-2023.4.6/examples/pyplot/scatter2.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/scatter3.py` & `vedo-2023.4.6/examples/pyplot/scatter3.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/pyplot/whiskers.py` & `vedo-2023.4.6/examples/pyplot/whiskers.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/simulations/airplane1.py` & `vedo-2023.4.6/examples/simulations/airplane1.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/simulations/airplane2.py` & `vedo-2023.4.6/examples/simulations/airplane2.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/simulations/aspring1.py` & `vedo-2023.4.6/examples/simulations/aspring1.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/simulations/aspring2_player.py` & `vedo-2023.4.6/examples/simulations/aspring2_player.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/simulations/brownian2d.py` & `vedo-2023.4.6/examples/simulations/brownian2d.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/simulations/doubleslit.py` & `vedo-2023.4.6/examples/simulations/doubleslit.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/simulations/drag_chain.py` & `vedo-2023.4.6/examples/simulations/drag_chain.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/simulations/gas.py` & `vedo-2023.4.6/examples/simulations/gas.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/simulations/grayscott.py` & `vedo-2023.4.6/examples/simulations/grayscott.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/simulations/gyroscope1.py` & `vedo-2023.4.6/examples/simulations/gyroscope1.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/simulations/gyroscope2.py` & `vedo-2023.4.6/examples/simulations/gyroscope2.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/simulations/hanoi3d.py` & `vedo-2023.4.6/examples/simulations/hanoi3d.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/simulations/koch_fractal.py` & `vedo-2023.4.6/examples/simulations/koch_fractal.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/simulations/lorenz.py` & `vedo-2023.4.6/examples/simulations/lorenz.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/simulations/mag_field1.py` & `vedo-2023.4.6/examples/simulations/mag_field1.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/simulations/mag_field2.py` & `vedo-2023.4.6/examples/simulations/mag_field2.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/simulations/multiple_pendulum.py` & `vedo-2023.4.6/examples/simulations/multiple_pendulum.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/simulations/optics_base.py` & `vedo-2023.4.6/examples/simulations/optics_base.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/simulations/optics_main1.py` & `vedo-2023.4.6/examples/simulations/optics_main1.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/simulations/optics_main2.py` & `vedo-2023.4.6/examples/simulations/optics_main2.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/simulations/optics_main3.py` & `vedo-2023.4.6/examples/simulations/optics_main3.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/simulations/particle_simulator.py` & `vedo-2023.4.6/examples/simulations/particle_simulator.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/simulations/pendulum_3d.py` & `vedo-2023.4.6/examples/simulations/pendulum_3d.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/simulations/pendulum_ode.py` & `vedo-2023.4.6/examples/simulations/pendulum_ode.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/simulations/self_org_maps2d.py` & `vedo-2023.4.6/examples/simulations/self_org_maps2d.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/simulations/spline_ease.py` & `vedo-2023.4.6/examples/simulations/spline_ease.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/simulations/trail.py` & `vedo-2023.4.6/examples/simulations/trail.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/simulations/tunnelling1.py` & `vedo-2023.4.6/examples/simulations/tunnelling1.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/simulations/tunnelling2.py` & `vedo-2023.4.6/examples/simulations/tunnelling2.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/simulations/value_iteration.py` & `vedo-2023.4.6/examples/simulations/value_iteration.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/simulations/volterra.py` & `vedo-2023.4.6/examples/simulations/volterra.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/simulations/wave_equation1d.py` & `vedo-2023.4.6/examples/simulations/wave_equation1d.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/simulations/wave_equation2d.py` & `vedo-2023.4.6/examples/simulations/wave_equation2d.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/volumetric/colorize_volume.py` & `vedo-2023.4.6/examples/volumetric/colorize_volume.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/volumetric/delaunay3d.py` & `vedo-2023.4.6/examples/volumetric/delaunay3d.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/volumetric/densifycloud.py` & `vedo-2023.4.6/examples/volumetric/densifycloud.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/volumetric/earth_model.py` & `vedo-2023.4.6/examples/volumetric/earth_model.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/volumetric/image_false_colors.py` & `vedo-2023.4.6/examples/volumetric/image_false_colors.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/volumetric/image_fft.py` & `vedo-2023.4.6/examples/volumetric/image_fft.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/volumetric/image_mask.py` & `vedo-2023.4.6/examples/volumetric/image_mask.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/volumetric/image_probe.py` & `vedo-2023.4.6/examples/volumetric/image_probe.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/volumetric/image_rgba.py` & `vedo-2023.4.6/examples/volumetric/image_rgba.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/volumetric/image_to_mesh.py` & `vedo-2023.4.6/examples/volumetric/image_to_mesh.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/volumetric/interpolate_volume.py` & `vedo-2023.4.6/examples/volumetric/interpolate_volume.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/volumetric/lowpassfilter.py` & `vedo-2023.4.6/examples/volumetric/lowpassfilter.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/volumetric/multiscalars.py` & `vedo-2023.4.6/examples/volumetric/multiscalars.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/volumetric/numpy2volume1.py` & `vedo-2023.4.6/examples/volumetric/numpy2volume1.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/volumetric/numpy2volume2.py` & `vedo-2023.4.6/examples/volumetric/numpy2volume2.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/volumetric/numpy_imread.py` & `vedo-2023.4.6/examples/volumetric/numpy_imread.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/volumetric/off_furniture.py` & `vedo-2023.4.6/examples/volumetric/off_furniture.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/volumetric/office.py` & `vedo-2023.4.6/examples/volumetric/office.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/volumetric/probe_line1.py` & `vedo-2023.4.6/examples/volumetric/probe_line1.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/volumetric/probe_line2.py` & `vedo-2023.4.6/examples/volumetric/probe_line2.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/volumetric/probe_points.py` & `vedo-2023.4.6/examples/volumetric/probe_points.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/volumetric/read_volume1.py` & `vedo-2023.4.6/examples/volumetric/read_volume1.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/volumetric/read_volume2.py` & `vedo-2023.4.6/examples/volumetric/read_volume2.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/volumetric/read_volume3.py` & `vedo-2023.4.6/examples/volumetric/read_volume3.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/volumetric/read_vts.py` & `vedo-2023.4.6/examples/volumetric/read_vts.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/volumetric/slice_plane1.py` & `vedo-2023.4.6/examples/volumetric/slice_plane1.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/volumetric/slice_plane2.py` & `vedo-2023.4.6/examples/volumetric/slice_plane2.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/volumetric/slicer1.py` & `vedo-2023.4.6/examples/volumetric/slicer1.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/volumetric/slicer2.py` & `vedo-2023.4.6/examples/volumetric/slicer2.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/volumetric/streamlines1.py` & `vedo-2023.4.6/examples/volumetric/streamlines1.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/volumetric/streamlines2.py` & `vedo-2023.4.6/examples/volumetric/streamlines2.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/volumetric/streamlines3.py` & `vedo-2023.4.6/examples/volumetric/streamlines3.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/volumetric/streamlines4.py` & `vedo-2023.4.6/examples/volumetric/streamlines4.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/volumetric/streamribbons.py` & `vedo-2023.4.6/examples/volumetric/streamribbons.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/volumetric/tensors.py` & `vedo-2023.4.6/examples/volumetric/tensors.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/volumetric/tet_astyle.py` & `vedo-2023.4.6/examples/volumetric/tet_astyle.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/volumetric/tet_build.py` & `vedo-2023.4.6/examples/volumetric/tet_build.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/volumetric/tet_cutMesh2.py` & `vedo-2023.4.6/examples/volumetric/tet_cut2.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/volumetric/tet_explode.py` & `vedo-2023.4.6/examples/volumetric/tet_explode.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/volumetric/tetralize_surface.py` & `vedo-2023.4.6/examples/volumetric/tetralize_surface.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/volumetric/volume_operations.py` & `vedo-2023.4.6/examples/volumetric/volume_operations.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/examples/volumetric/volume_sharemap.py` & `vedo-2023.4.6/examples/volumetric/volume_sharemap.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/setup.py` & `vedo-2023.4.6/setup.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/vedo/__init__.py` & `vedo-2023.4.6/vedo/__init__.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/vedo/addons.py` & `vedo-2023.4.6/vedo/addons.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/vedo/applications.py` & `vedo-2023.4.6/vedo/applications.py`

 * *Files 0% similar despite different names*

```diff
@@ -759,14 +759,17 @@
             plt.close()
             ```
 
         - [morphomatics_tube.py](https://github.com/marcomusy/vedo/tree/master/examples/other/morphomatics_tube.py)
         """
         Plotter.__init__(self, axes=axes, **kwargs)
 
+        if isinstance(objects, str):
+            objects = vedo.file_io.load(objects)
+
         self += objects
 
         self.slider = None
         self.timer_callback_id = None
 
         # define the slider func ##########################
         def slider_function(widget=None, event=None):
@@ -949,14 +952,15 @@
                 self.remove([self.spline, self.jline])
                 if self.splined:  # show the spline closed
                     self.spline = Spline(self.cpoints, closed=True, res=len(self.cpoints) * 4)
                 else:
                     self.spline = Line(self.cpoints, closed=True)
                 self.spline.lw(self.linewidth).c(self.linecolor).pickable(False)
                 self.add(self.spline)
+        self.render()
 
     def _on_mouse_move(self, evt):
         if self.drawmode:
             cpt = self.compute_world_coordinate(evt.picked2d)  # make this 2d-screen point 3d
             if self.cpoints and mag(cpt - self.cpoints[-1]) < self.mesh.diagonal_size() * self.tol:
                 return  # new point is too close to the last one. skip
             self.cpoints.append(cpt)
@@ -1009,15 +1013,15 @@
             mcut = self.mesh.extract_largest_region()
             mcut.filename = self.mesh.filename  # copy over various properties
             mcut.name = self.mesh.name
             mcut.scalarbar = self.mesh.scalarbar
             mcut.info = self.mesh.info
             self.mesh = mcut                            # discard old mesh by overwriting it
             self.txt2d.text(self.msg).background(self.color)   # put back original message
-            self.add(mcut)
+            self.add(mcut).render()
 
         elif evt.keypress == 'u':                       # Undo last action
             if self.drawmode:
                 self._on_right_click(evt)               # toggle mode to normal
             else:
                 self.txt2d.background(self.color, self.alpha)
             self.remove([self.mesh, self.spline, self.jline, self.points, self.topline])
@@ -1032,17 +1036,17 @@
             self.cpoints, self.points, self.spline = [], None, None
             self.top_pts, self.topline = [], None
 
         elif evt.keypress == "r":  # reset camera and axes
             try:
                 self.remove(self.axes_instances[0])
                 self.axes_instances[0] = None
-                self.add_global_axes(axtype=1, c=None)
+                self.add_global_axes(axtype=1, c=None, bounds=self.mesh.bounds())
                 self.renderer.ResetCamera()
-                self.interactor.Render()
+                self.render()
             except:
                 pass
 
         elif evt.keypress == "s":
             if self.mesh.filename:
                 fname = os.path.basename(self.mesh.filename)
                 fname, extension = os.path.splitext(fname)
```

### Comparing `vedo-2023.4.5/vedo/assembly.py` & `vedo-2023.4.6/vedo/assembly.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/vedo/backends.py` & `vedo-2023.4.6/vedo/backends.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/vedo/base.py` & `vedo-2023.4.6/vedo/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -2038,14 +2038,18 @@
                 use a list to specify transparencies along the scalar range
             vmin : (float)
                 force the min of the scalar range to be this value
             vmax : (float)
                 force the max of the scalar range to be this value
         """
         # supersedes method in Points, Mesh
+
+        if col is None:
+            return self
+        
         if vmin is None:
             vmin, _ = self._data.GetScalarRange()
         if vmax is None:
             _, vmax = self._data.GetScalarRange()
         ctf = self.GetProperty().GetRGBTransferFunction()
         ctf.RemoveAllPoints()
         self._color = col
```

### Comparing `vedo-2023.4.5/vedo/cli.py` & `vedo-2023.4.6/vedo/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
     pr.add_argument("-x", "--axes-type", type=int,  help="specify axes type [0-14]", default=1, metavar='')
     pr.add_argument("-i", "--no-camera-share",      help="do not share camera in renderers", action="store_true")
     pr.add_argument("-f", "--full-screen",          help="full screen mode", action="store_true")
     pr.add_argument("-bg","--background", type=str, help="background color [integer or color name]", default='', metavar='')
     pr.add_argument("-bg2", "--background-grad",    help="use background color gradient", default='', metavar='')
     pr.add_argument("-z", "--zoom", type=float,     help="zooming factor", default=1, metavar='')
     pr.add_argument("-n", "--multirenderer-mode",   help="multi renderer mode: files go to separate renderers", action="store_true")
-    pr.add_argument("-s", "--scrolling-mode",       help="scrolling Mode: use slider to scroll files", action="store_true")
+    pr.add_argument("-s", "--sequence-mode",        help="sequence mode: use slider to browse files", action="store_true")
     pr.add_argument("-g", "--ray-cast-mode",        help="GPU Ray-casting Mode for 3D image files", action="store_true")
     pr.add_argument("-gx", "--x-spacing", type=float, help="volume x-spacing factor [1]", default=1, metavar='')
     pr.add_argument("-gy", "--y-spacing", type=float, help="volume y-spacing factor [1]", default=1, metavar='')
     pr.add_argument("-gz", "--z-spacing", type=float, help="volume z-spacing factor [1]", default=1, metavar='')
     pr.add_argument("--mode",                       help="volume rendering style (composite/maxproj/...)", default=0, metavar='')
     pr.add_argument("--cmap",                       help="volume rendering color map name", default='jet', metavar='')
     pr.add_argument("-e", "--edit",                 help="free-hand edit the input Mesh", action="store_true")
@@ -679,15 +679,15 @@
         args.background_grad = get_color(args.background_grad)
 
     if nfiles == 1 and args.files[0].endswith(".gif"):  ###can be improved
         frames = load(args.files[0])
         applications.Browser(frames).show(bg=args.background, bg2=args.background_grad)
         return  ##########################################################
 
-    if args.scrolling_mode:
+    if args.sequence_mode:
         args.multirenderer_mode = False
     settings.default_font = args.font
 
     sharecam = args.no_camera_share
 
     N = None
     if args.multirenderer_mode:
@@ -828,15 +828,15 @@
             precompute=False, progress=True, use_gpu=True,
         )
         plt.show(zoom=args.zoom, viewup="z")
         return
 
     ########################################################################
     # NORMAL mode for single or multiple files, or multiren mode, or numpy scene
-    elif nfiles == 1 or (not args.scrolling_mode):
+    elif nfiles == 1 or (not args.sequence_mode):
         # print('DEBUG NORMAL mode for single or multiple files, or multiren mode')
 
         interactor_mode = 0
         if args.image:
             interactor_mode = "image"
 
         ##########################################################
@@ -914,15 +914,15 @@
             if all(a is None for a in actors):
                 vedo.logger.error("Could not load file(s). Quit.")
                 return
             plt.show(actors, interactive=True, zoom=args.zoom, mode=interactor_mode)
         return
 
     ########################################################################
-    # scrolling mode  -s
+    # sequence mode  -s
     else:
         # print("DEBUG simple browser mode  -s")
         if plt.axes == 4:
             plt.axes = 1
 
         acts = load(args.files, force=args.reload)
         plt += acts
```

### Comparing `vedo-2023.4.5/vedo/cmaps.py` & `vedo-2023.4.6/vedo/cmaps.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/vedo/colors.py` & `vedo-2023.4.6/vedo/colors.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/vedo/dolfin.py` & `vedo-2023.4.6/vedo/dolfin.py`

 * *Files 0% similar despite different names*

```diff
@@ -465,15 +465,15 @@
             actor.alpha(alpha * alpha)
         if lw:
             actor.linewidth(lw)
             if wire and alpha:
                 lw1 = min(lw, 1)
                 actor.alpha(alpha * lw1)
         if ps:
-            actor.pointSize(ps)
+            actor.point_size(ps)
         if shading:
             if shading == "phong":
                 actor.phong()
             elif shading == "flat":
                 actor.flat()
             elif shading[0] == "g":
                 actor.gouraud()
```

### Comparing `vedo-2023.4.5/vedo/file_io.py` & `vedo-2023.4.6/vedo/file_io.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,15 +205,16 @@
     """
     acts = []
     if utils.is_sequence(inputobj):
         flist = inputobj
     elif isinstance(inputobj, str) and inputobj.startswith("https://"):
         flist = [inputobj]
     else:
-        flist = sorted(glob.glob(inputobj))
+        # flist = sorted(glob.glob(inputobj))
+        flist = utils.humansort(glob.glob(inputobj))
 
     for fod in flist:
 
         if fod.startswith("https://"):
             fod = download(fod, force=force, verbose=False)
 
         if os.path.isfile(fod):  ### it's a file
```

### Comparing `vedo-2023.4.5/vedo/fonts/Bongas.npz` & `vedo-2023.4.6/vedo/fonts/Bongas.npz`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/vedo/fonts/Bongas.ttf` & `vedo-2023.4.6/vedo/fonts/Bongas.ttf`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/vedo/fonts/Calco.npz` & `vedo-2023.4.6/vedo/fonts/Calco.npz`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/vedo/fonts/Calco.ttf` & `vedo-2023.4.6/vedo/fonts/Calco.ttf`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/vedo/fonts/Comae.npz` & `vedo-2023.4.6/vedo/fonts/Comae.npz`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/vedo/fonts/Comae.ttf` & `vedo-2023.4.6/vedo/fonts/Comae.ttf`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/vedo/fonts/Glasgo.npz` & `vedo-2023.4.6/vedo/fonts/Glasgo.npz`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/vedo/fonts/Glasgo.ttf` & `vedo-2023.4.6/vedo/fonts/Glasgo.ttf`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/vedo/fonts/Kanopus.npz` & `vedo-2023.4.6/vedo/fonts/Kanopus.npz`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/vedo/fonts/Kanopus.ttf` & `vedo-2023.4.6/vedo/fonts/Kanopus.ttf`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/vedo/fonts/Normografo.npz` & `vedo-2023.4.6/vedo/fonts/Normografo.npz`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/vedo/fonts/Normografo.ttf` & `vedo-2023.4.6/vedo/fonts/Normografo.ttf`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/vedo/fonts/Quikhand.npz` & `vedo-2023.4.6/vedo/fonts/Quikhand.npz`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/vedo/fonts/Quikhand.ttf` & `vedo-2023.4.6/vedo/fonts/Quikhand.ttf`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/vedo/fonts/SmartCouric.npz` & `vedo-2023.4.6/vedo/fonts/SmartCouric.npz`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/vedo/fonts/SmartCouric.ttf` & `vedo-2023.4.6/vedo/fonts/SmartCouric.ttf`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/vedo/fonts/Theemim.npz` & `vedo-2023.4.6/vedo/fonts/Theemim.npz`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/vedo/fonts/Theemim.ttf` & `vedo-2023.4.6/vedo/fonts/Theemim.ttf`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/vedo/fonts/VictorMono.npz` & `vedo-2023.4.6/vedo/fonts/VictorMono.npz`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/vedo/fonts/VictorMono.ttf` & `vedo-2023.4.6/vedo/fonts/VictorMono.ttf`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/vedo/interactor_modes.py` & `vedo-2023.4.6/vedo/interactor_modes.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/vedo/mesh.py` & `vedo-2023.4.6/vedo/mesh.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/vedo/picture.py` & `vedo-2023.4.6/vedo/picture.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/vedo/plotter.py` & `vedo-2023.4.6/vedo/plotter.py`

 * *Files 0% similar despite different names*

```diff
@@ -9002,491 +9002,506 @@
 00023290: 2061 6e64 2073 656c 662e 6178 6573 203d   and self.axes =
 000232a0: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
 000232b0: 2020 2020 2020 2020 2073 656c 662e 6178           self.ax
 000232c0: 6573 202d 3d20 3120 2023 206a 756d 7020  es -= 1  # jump 
 000232d0: 7275 6c65 7220 646f 6573 6e74 206d 616b  ruler doesnt mak
 000232e0: 6520 7365 6e73 6520 696e 2070 6572 7370  e sense in persp
 000232f0: 6563 7469 7665 206d 6f64 650a 2020 2020  ective mode.    
-00023300: 2020 2020 2020 2020 2020 2020 6164 646f              addo
-00023310: 6e73 2e61 6464 5f67 6c6f 6261 6c5f 6178  ns.add_global_ax
-00023320: 6573 2861 7874 7970 653d 2873 656c 662e  es(axtype=(self.
-00023330: 6178 6573 202d 2031 2920 2520 3135 2c20  axes - 1) % 15, 
-00023340: 633d 4e6f 6e65 290a 2020 2020 2020 2020  c=None).        
-00023350: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00023360: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-00023370: 2073 6574 7469 6e67 732e 7573 655f 7061   settings.use_pa
-00023380: 7261 6c6c 656c 5f70 726f 6a65 6374 696f  rallel_projectio
-00023390: 6e20 616e 6420 7365 6c66 2e61 7865 7320  n and self.axes 
-000233a0: 3d3d 2031 323a 0a20 2020 2020 2020 2020  == 12:.         
-000233b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000233c0: 6178 6573 202b 3d20 3120 2023 206a 756d  axes += 1  # jum
-000233d0: 7020 7275 6c65 7220 646f 6573 6e74 206d  p ruler doesnt m
-000233e0: 616b 6520 7365 6e73 6520 696e 2070 6572  ake sense in per
-000233f0: 7370 6563 7469 7665 206d 6f64 650a 2020  spective mode.  
-00023400: 2020 2020 2020 2020 2020 2020 2020 6164                ad
-00023410: 646f 6e73 2e61 6464 5f67 6c6f 6261 6c5f  dons.add_global_
-00023420: 6178 6573 2861 7874 7970 653d 2873 656c  axes(axtype=(sel
-00023430: 662e 6178 6573 202b 2031 2920 2520 3135  f.axes + 1) % 15
-00023440: 2c20 633d 4e6f 6e65 290a 2020 2020 2020  , c=None).      
-00023450: 2020 2020 2020 7365 6c66 2e69 6e74 6572        self.inter
-00023460: 6163 746f 722e 5265 6e64 6572 2829 0a0a  actor.Render()..
-00023470: 2020 2020 2020 2020 656c 6966 2022 4b50          elif "KP
-00023480: 5f22 2069 6e20 6b65 7920 6f72 206b 6579  _" in key or key
-00023490: 2069 6e20 5b0a 2020 2020 2020 2020 2020   in [.          
-000234a0: 2020 2249 6e73 6572 7422 2c0a 2020 2020    "Insert",.    
-000234b0: 2020 2020 2020 2020 2245 6e64 222c 0a20          "End",. 
-000234c0: 2020 2020 2020 2020 2020 2022 446f 776e             "Down
-000234d0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-000234e0: 4e65 7874 222c 0a20 2020 2020 2020 2020  Next",.         
-000234f0: 2020 2022 4c65 6674 222c 0a20 2020 2020     "Left",.     
-00023500: 2020 2020 2020 2022 4265 6769 6e22 2c0a         "Begin",.
-00023510: 2020 2020 2020 2020 2020 2020 2252 6967              "Rig
-00023520: 6874 222c 0a20 2020 2020 2020 2020 2020  ht",.           
-00023530: 2022 486f 6d65 222c 0a20 2020 2020 2020   "Home",.       
-00023540: 2020 2020 2022 5570 222c 0a20 2020 2020       "Up",.     
-00023550: 2020 2020 2020 2022 5072 696f 7222 2c0a         "Prior",.
-00023560: 2020 2020 2020 2020 5d3a 0a20 2020 2020          ]:.     
-00023570: 2020 2020 2020 2023 2063 6861 6e67 6520         # change 
-00023580: 6178 6573 2073 7479 6c65 0a20 2020 2020  axes style.     
-00023590: 2020 2020 2020 2061 7373 6f20 3d20 7b0a         asso = {.
-000235a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000235b0: 224b 505f 496e 7365 7274 223a 2030 2c0a  "KP_Insert": 0,.
-000235c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000235d0: 224b 505f 3022 3a20 302c 0a20 2020 2020  "KP_0": 0,.     
-000235e0: 2020 2020 2020 2020 2020 2022 4b50 5f45             "KP_E
-000235f0: 6e64 223a 2031 2c0a 2020 2020 2020 2020  nd": 1,.        
-00023600: 2020 2020 2020 2020 224b 505f 3122 3a20          "KP_1": 
-00023610: 312c 0a20 2020 2020 2020 2020 2020 2020  1,.             
-00023620: 2020 2022 4b50 5f44 6f77 6e22 3a20 322c     "KP_Down": 2,
-00023630: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00023640: 2022 4b50 5f32 223a 2032 2c0a 2020 2020   "KP_2": 2,.    
-00023650: 2020 2020 2020 2020 2020 2020 224b 505f              "KP_
-00023660: 4e65 7874 223a 2033 2c0a 2020 2020 2020  Next": 3,.      
-00023670: 2020 2020 2020 2020 2020 224b 505f 3322            "KP_3"
-00023680: 3a20 332c 0a20 2020 2020 2020 2020 2020  : 3,.           
-00023690: 2020 2020 2022 4b50 5f4c 6566 7422 3a20       "KP_Left": 
-000236a0: 342c 0a20 2020 2020 2020 2020 2020 2020  4,.             
-000236b0: 2020 2022 4b50 5f34 223a 2034 2c0a 2020     "KP_4": 4,.  
-000236c0: 2020 2020 2020 2020 2020 2020 2020 224b                "K
-000236d0: 505f 4265 6769 6e22 3a20 352c 0a20 2020  P_Begin": 5,.   
-000236e0: 2020 2020 2020 2020 2020 2020 2022 4b50               "KP
-000236f0: 5f35 223a 2035 2c0a 2020 2020 2020 2020  _5": 5,.        
-00023700: 2020 2020 2020 2020 224b 505f 5269 6768          "KP_Righ
-00023710: 7422 3a20 362c 0a20 2020 2020 2020 2020  t": 6,.         
-00023720: 2020 2020 2020 2022 4b50 5f36 223a 2036         "KP_6": 6
-00023730: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00023740: 2020 224b 505f 486f 6d65 223a 2037 2c0a    "KP_Home": 7,.
-00023750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023760: 224b 505f 3722 3a20 372c 0a20 2020 2020  "KP_7": 7,.     
-00023770: 2020 2020 2020 2020 2020 2022 4b50 5f55             "KP_U
-00023780: 7022 3a20 382c 0a20 2020 2020 2020 2020  p": 8,.         
-00023790: 2020 2020 2020 2022 4b50 5f38 223a 2038         "KP_8": 8
-000237a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000237b0: 2020 2250 7269 6f72 223a 2039 2c20 2023    "Prior": 9,  #
-000237c0: 206f 6e20 7769 6e64 6f77 7320 4f53 0a20   on windows OS. 
-000237d0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000237e0: 496e 7365 7274 223a 2030 2c0a 2020 2020  Insert": 0,.    
-000237f0: 2020 2020 2020 2020 2020 2020 2245 6e64              "End
-00023800: 223a 2031 2c0a 2020 2020 2020 2020 2020  ": 1,.          
-00023810: 2020 2020 2020 2244 6f77 6e22 3a20 322c        "Down": 2,
-00023820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00023830: 2022 4e65 7874 223a 2033 2c0a 2020 2020   "Next": 3,.    
-00023840: 2020 2020 2020 2020 2020 2020 224c 6566              "Lef
-00023850: 7422 3a20 342c 0a20 2020 2020 2020 2020  t": 4,.         
-00023860: 2020 2020 2020 2022 4265 6769 6e22 3a20         "Begin": 
-00023870: 352c 0a20 2020 2020 2020 2020 2020 2020  5,.             
-00023880: 2020 2022 5269 6768 7422 3a20 362c 0a20     "Right": 6,. 
-00023890: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000238a0: 486f 6d65 223a 2037 2c0a 2020 2020 2020  Home": 7,.      
-000238b0: 2020 2020 2020 2020 2020 2255 7022 3a20            "Up": 
-000238c0: 382c 0a20 2020 2020 2020 2020 2020 2020  8,.             
-000238d0: 2020 2022 5072 696f 7222 3a20 392c 0a20     "Prior": 9,. 
-000238e0: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-000238f0: 2020 2020 2020 2020 2063 6c69 636b 6564           clicked
-00023900: 7220 3d20 7365 6c66 2e72 656e 6465 7265  r = self.rendere
-00023910: 7273 2e69 6e64 6578 2872 656e 6465 7265  rs.index(rendere
-00023920: 7229 0a20 2020 2020 2020 2020 2020 2069  r).            i
-00023930: 6620 6b65 7920 696e 2061 7373 6f3a 0a20  f key in asso:. 
-00023940: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00023950: 6620 7365 6c66 2e61 7865 735f 696e 7374  f self.axes_inst
-00023960: 616e 6365 735b 636c 6963 6b65 6472 5d3a  ances[clickedr]:
-00023970: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00023980: 2020 2020 2069 6620 6861 7361 7474 7228       if hasattr(
-00023990: 7365 6c66 2e61 7865 735f 696e 7374 616e  self.axes_instan
-000239a0: 6365 735b 636c 6963 6b65 6472 5d2c 2022  ces[clickedr], "
-000239b0: 456e 6162 6c65 644f 6666 2229 3a20 2023  EnabledOff"):  #
-000239c0: 2077 6964 6765 740a 2020 2020 2020 2020   widget.        
-000239d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000239e0: 7365 6c66 2e61 7865 735f 696e 7374 616e  self.axes_instan
-000239f0: 6365 735b 636c 6963 6b65 6472 5d2e 456e  ces[clickedr].En
-00023a00: 6162 6c65 644f 6666 2829 0a20 2020 2020  abledOff().     
-00023a10: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00023a20: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00023a30: 2020 2020 2020 2020 2020 2020 2074 7279               try
-00023a40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00023a50: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00023a60: 6e64 6572 6572 2e52 656d 6f76 6541 6374  nderer.RemoveAct
-00023a70: 6f72 2873 656c 662e 6178 6573 5f69 6e73  or(self.axes_ins
-00023a80: 7461 6e63 6573 5b63 6c69 636b 6564 725d  tances[clickedr]
-00023a90: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00023aa0: 2020 2020 2020 2020 2020 6578 6365 7074            except
-00023ab0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00023ac0: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-00023ad0: 7373 0a20 2020 2020 2020 2020 2020 2020  ss.             
-00023ae0: 2020 2020 2020 2073 656c 662e 6178 6573         self.axes
-00023af0: 5f69 6e73 7461 6e63 6573 5b63 6c69 636b  _instances[click
-00023b00: 6564 725d 203d 204e 6f6e 650a 2020 2020  edr] = None.    
-00023b10: 2020 2020 2020 2020 2020 2020 6164 646f              addo
-00023b20: 6e73 2e61 6464 5f67 6c6f 6261 6c5f 6178  ns.add_global_ax
-00023b30: 6573 2861 7874 7970 653d 6173 736f 5b6b  es(axtype=asso[k
-00023b40: 6579 5d2c 2063 3d4e 6f6e 6529 0a20 2020  ey], c=None).   
-00023b50: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00023b60: 662e 696e 7465 7261 6374 6f72 2e52 656e  f.interactor.Ren
-00023b70: 6465 7228 290a 0a20 2020 2020 2020 2069  der()..        i
-00023b80: 6620 6b65 7920 3d3d 2022 4f22 3a0a 2020  f key == "O":.  
-00023b90: 2020 2020 2020 2020 2020 7265 6e64 6572            render
-00023ba0: 6572 2e52 656d 6f76 654c 6967 6874 2873  er.RemoveLight(s
-00023bb0: 656c 662e 5f65 7874 7261 6c69 6768 7429  elf._extralight)
-00023bc0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00023bd0: 662e 5f65 7874 7261 6c69 6768 7420 3d20  f._extralight = 
-00023be0: 4e6f 6e65 0a0a 2020 2020 2020 2020 656c  None..        el
-00023bf0: 6966 206b 6579 203d 3d20 226f 223a 0a20  if key == "o":. 
-00023c00: 2020 2020 2020 2020 2020 2076 6262 2c20             vbb, 
-00023c10: 7369 7a65 732c 205f 2c20 5f20 3d20 6164  sizes, _, _ = ad
-00023c20: 646f 6e73 2e63 6f6d 7075 7465 5f76 6973  dons.compute_vis
-00023c30: 6962 6c65 5f62 6f75 6e64 7328 290a 2020  ible_bounds().  
-00023c40: 2020 2020 2020 2020 2020 636d 203d 2075            cm = u
-00023c50: 7469 6c73 2e76 6563 746f 7228 2876 6262  tils.vector((vbb
-00023c60: 5b30 5d20 2b20 7662 625b 315d 2920 2f20  [0] + vbb[1]) / 
-00023c70: 322c 2028 7662 625b 325d 202b 2076 6262  2, (vbb[2] + vbb
-00023c80: 5b33 5d29 202f 2032 2c20 2876 6262 5b34  [3]) / 2, (vbb[4
-00023c90: 5d20 2b20 7662 625b 355d 2920 2f20 3229  ] + vbb[5]) / 2)
-00023ca0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00023cb0: 6e6f 7420 7365 6c66 2e5f 6578 7472 616c  not self._extral
-00023cc0: 6967 6874 3a0a 2020 2020 2020 2020 2020  ight:.          
-00023cd0: 2020 2020 2020 7675 7020 3d20 7265 6e64        vup = rend
-00023ce0: 6572 6572 2e47 6574 4163 7469 7665 4361  erer.GetActiveCa
-00023cf0: 6d65 7261 2829 2e47 6574 5669 6577 5570  mera().GetViewUp
-00023d00: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-00023d10: 2020 2070 6f73 203d 2063 6d20 2b20 7574     pos = cm + ut
-00023d20: 696c 732e 7665 6374 6f72 2876 7570 2920  ils.vector(vup) 
-00023d30: 2a20 7574 696c 732e 6d61 6728 7369 7a65  * utils.mag(size
-00023d40: 7329 0a20 2020 2020 2020 2020 2020 2020  s).             
-00023d50: 2020 2073 656c 662e 5f65 7874 7261 6c69     self._extrali
-00023d60: 6768 7420 3d20 6164 646f 6e73 2e4c 6967  ght = addons.Lig
-00023d70: 6874 2870 6f73 2c20 666f 6361 6c5f 706f  ht(pos, focal_po
-00023d80: 696e 743d 636d 290a 2020 2020 2020 2020  int=cm).        
-00023d90: 2020 2020 2020 2020 7265 6e64 6572 6572          renderer
-00023da0: 2e41 6464 4c69 6768 7428 7365 6c66 2e5f  .AddLight(self._
-00023db0: 6578 7472 616c 6967 6874 290a 2020 2020  extralight).    
-00023dc0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00023dd0: 7428 2250 7265 7373 2061 6761 696e 206f  t("Press again o
-00023de0: 2074 6f20 726f 7461 7465 206c 6967 6874   to rotate light
-00023df0: 2073 6f75 7263 652c 206f 7220 4f20 746f   source, or O to
-00023e00: 2072 656d 6f76 6520 6974 2e22 290a 2020   remove it.").  
-00023e10: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-00023e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023e30: 6370 6f73 203d 2075 7469 6c73 2e76 6563  cpos = utils.vec
-00023e40: 746f 7228 7365 6c66 2e5f 6578 7472 616c  tor(self._extral
-00023e50: 6967 6874 2e47 6574 506f 7369 7469 6f6e  ight.GetPosition
-00023e60: 2829 290a 2020 2020 2020 2020 2020 2020  ()).            
-00023e70: 2020 2020 782c 2079 2c20 7a20 3d20 7365      x, y, z = se
-00023e80: 6c66 2e5f 6578 7472 616c 6967 6874 2e47  lf._extralight.G
-00023e90: 6574 506f 7369 7469 6f6e 2829 202d 2063  etPosition() - c
-00023ea0: 6d0a 2020 2020 2020 2020 2020 2020 2020  m.              
-00023eb0: 2020 722c 2074 682c 2070 6820 3d20 7574    r, th, ph = ut
-00023ec0: 696c 732e 6361 7274 3273 7068 6572 2878  ils.cart2spher(x
-00023ed0: 2c20 792c 207a 290a 2020 2020 2020 2020  , y, z).        
-00023ee0: 2020 2020 2020 2020 7468 202b 3d20 302e          th += 0.
-00023ef0: 320a 2020 2020 2020 2020 2020 2020 2020  2.              
-00023f00: 2020 6966 2074 6820 3e20 6e70 2e70 693a    if th > np.pi:
-00023f10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00023f20: 2020 2020 2074 6820 3d20 6e70 2e72 616e       th = np.ran
-00023f30: 646f 6d2e 7261 6e64 6f6d 2829 202a 206e  dom.random() * n
-00023f40: 702e 7069 202f 2032 0a20 2020 2020 2020  p.pi / 2.       
-00023f50: 2020 2020 2020 2020 2070 6820 2b3d 2030           ph += 0
-00023f60: 2e33 0a20 2020 2020 2020 2020 2020 2020  .3.             
-00023f70: 2020 2063 706f 7320 3d20 7574 696c 732e     cpos = utils.
-00023f80: 7370 6865 7232 6361 7274 2872 2c20 7468  spher2cart(r, th
-00023f90: 2c20 7068 2920 2b20 636d 0a20 2020 2020  , ph) + cm.     
-00023fa0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00023fb0: 5f65 7874 7261 6c69 6768 742e 5365 7450  _extralight.SetP
-00023fc0: 6f73 6974 696f 6e28 6370 6f73 290a 0a20  osition(cpos).. 
-00023fd0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00023fe0: 7769 6e64 6f77 2e52 656e 6465 7228 290a  window.Render().
-00023ff0: 0a20 2020 2020 2020 2065 6c69 6620 6b65  .        elif ke
-00024000: 7920 3d3d 2022 6c22 3a0a 2020 2020 2020  y == "l":.      
-00024010: 2020 2020 2020 6966 2073 656c 662e 636c        if self.cl
-00024020: 6963 6b65 645f 6163 746f 7220 696e 2073  icked_actor in s
-00024030: 656c 662e 6765 745f 6d65 7368 6573 2829  elf.get_meshes()
-00024040: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00024050: 2020 6163 7473 203d 205b 7365 6c66 2e63    acts = [self.c
-00024060: 6c69 636b 6564 5f61 6374 6f72 5d0a 2020  licked_actor].  
-00024070: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-00024080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024090: 6163 7473 203d 2073 656c 662e 6765 745f  acts = self.get_
-000240a0: 6d65 7368 6573 2829 0a20 2020 2020 2020  meshes().       
-000240b0: 2020 2020 2066 6f72 2069 6120 696e 2061       for ia in a
-000240c0: 6374 733a 0a20 2020 2020 2020 2020 2020  cts:.           
-000240d0: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-000240e0: 2020 2020 2020 2020 2020 2020 2020 6576                ev
-000240f0: 203d 2069 612e 4765 7450 726f 7065 7274   = ia.GetPropert
-00024100: 7928 292e 4765 7445 6467 6556 6973 6962  y().GetEdgeVisib
-00024110: 696c 6974 7928 290a 2020 2020 2020 2020  ility().        
-00024120: 2020 2020 2020 2020 2020 2020 6961 2e47              ia.G
-00024130: 6574 5072 6f70 6572 7479 2829 2e53 6574  etProperty().Set
-00024140: 4564 6765 5669 7369 6269 6c69 7479 286e  EdgeVisibility(n
-00024150: 6f74 2065 7629 0a20 2020 2020 2020 2020  ot ev).         
-00024160: 2020 2020 2020 2020 2020 2069 612e 4765             ia.Ge
-00024170: 7450 726f 7065 7274 7928 292e 5365 7452  tProperty().SetR
-00024180: 6570 7265 7365 6e74 6174 696f 6e54 6f53  epresentationToS
-00024190: 7572 6661 6365 2829 0a20 2020 2020 2020  urface().       
-000241a0: 2020 2020 2020 2020 2020 2020 2069 612e               ia.
-000241b0: 4765 7450 726f 7065 7274 7928 292e 5365  GetProperty().Se
-000241c0: 744c 696e 6557 6964 7468 2830 2e31 290a  tLineWidth(0.1).
-000241d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000241e0: 6578 6365 7074 2041 7474 7269 6275 7465  except Attribute
-000241f0: 4572 726f 723a 0a20 2020 2020 2020 2020  Error:.         
-00024200: 2020 2020 2020 2020 2020 2070 6173 730a             pass.
-00024210: 0a20 2020 2020 2020 2065 6c69 6620 6b65  .        elif ke
-00024220: 7920 3d3d 2022 6b22 3a20 2023 206c 6967  y == "k":  # lig
-00024230: 6874 696e 6773 0a20 2020 2020 2020 2020  htings.         
-00024240: 2020 2069 6620 7365 6c66 2e63 6c69 636b     if self.click
-00024250: 6564 5f61 6374 6f72 2069 6e20 7365 6c66  ed_actor in self
-00024260: 2e67 6574 5f6d 6573 6865 7328 293a 0a20  .get_meshes():. 
-00024270: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00024280: 6374 7320 3d20 5b73 656c 662e 636c 6963  cts = [self.clic
-00024290: 6b65 645f 6163 746f 725d 0a20 2020 2020  ked_actor].     
-000242a0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-000242b0: 2020 2020 2020 2020 2020 2020 2061 6374               act
-000242c0: 7320 3d20 7365 6c66 2e67 6574 5f6d 6573  s = self.get_mes
-000242d0: 6865 7328 290a 2020 2020 2020 2020 2020  hes().          
-000242e0: 2020 7368 6473 203d 2028 2264 6566 6175    shds = ("defau
-000242f0: 6c74 222c 2022 6d65 7461 6c6c 6963 222c  lt", "metallic",
-00024300: 2022 706c 6173 7469 6322 2c20 2273 6869   "plastic", "shi
-00024310: 6e79 222c 2022 676c 6f73 7379 222c 2022  ny", "glossy", "
-00024320: 6f66 6622 290a 2020 2020 2020 2020 2020  off").          
-00024330: 2020 666f 7220 6961 2069 6e20 6163 7473    for ia in acts
-00024340: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00024350: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-00024360: 2020 2020 2020 2020 2020 206c 6e72 203d             lnr =
-00024370: 2028 6961 2e5f 6c69 6774 6869 6e67 6e72   (ia._ligthingnr
-00024380: 202b 2031 2920 2520 360a 2020 2020 2020   + 1) % 6.      
-00024390: 2020 2020 2020 2020 2020 2020 2020 6961                ia
-000243a0: 2e6c 6967 6874 696e 6728 7368 6473 5b6c  .lighting(shds[l
-000243b0: 6e72 5d29 0a20 2020 2020 2020 2020 2020  nr]).           
-000243c0: 2020 2020 2020 2020 2069 612e 5f6c 6967           ia._lig
-000243d0: 7468 696e 676e 7220 3d20 6c6e 720a 2020  thingnr = lnr.  
-000243e0: 2020 2020 2020 2020 2020 2020 2020 6578                ex
-000243f0: 6365 7074 2041 7474 7269 6275 7465 4572  cept AttributeEr
-00024400: 726f 723a 0a20 2020 2020 2020 2020 2020  ror:.           
-00024410: 2020 2020 2020 2020 2070 6173 730a 0a20           pass.. 
-00024420: 2020 2020 2020 2065 6c69 6620 6b65 7920         elif key 
-00024430: 3d3d 2022 4b22 3a20 2023 2073 6861 6469  == "K":  # shadi
-00024440: 6e67 0a20 2020 2020 2020 2020 2020 2069  ng.            i
-00024450: 6620 7365 6c66 2e63 6c69 636b 6564 5f61  f self.clicked_a
-00024460: 6374 6f72 2069 6e20 7365 6c66 2e67 6574  ctor in self.get
-00024470: 5f6d 6573 6865 7328 293a 0a20 2020 2020  _meshes():.     
-00024480: 2020 2020 2020 2020 2020 2061 6374 7320             acts 
-00024490: 3d20 5b73 656c 662e 636c 6963 6b65 645f  = [self.clicked_
-000244a0: 6163 746f 725d 0a20 2020 2020 2020 2020  actor].         
-000244b0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000244c0: 2020 2020 2020 2020 2061 6374 7320 3d20           acts = 
-000244d0: 7365 6c66 2e67 6574 5f6d 6573 6865 7328  self.get_meshes(
-000244e0: 290a 2020 2020 2020 2020 2020 2020 666f  ).            fo
-000244f0: 7220 6961 2069 6e20 6163 7473 3a0a 2020  r ia in acts:.  
-00024500: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00024510: 2069 7369 6e73 7461 6e63 6528 6961 2c20   isinstance(ia, 
-00024520: 7665 646f 2e4d 6573 6829 3a0a 2020 2020  vedo.Mesh):.    
-00024530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024540: 6961 2e63 6f6d 7075 7465 5f6e 6f72 6d61  ia.compute_norma
-00024550: 6c73 2863 656c 6c73 3d46 616c 7365 290a  ls(cells=False).
-00024560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024570: 2020 2020 696e 7472 7020 3d20 6961 2e47      intrp = ia.G
-00024580: 6574 5072 6f70 6572 7479 2829 2e47 6574  etProperty().Get
-00024590: 496e 7465 7270 6f6c 6174 696f 6e28 290a  Interpolation().
-000245a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000245b0: 2020 2020 2320 7072 696e 7428 696e 7472      # print(intr
-000245c0: 702c 2069 612e 4765 7450 726f 7065 7274  p, ia.GetPropert
-000245d0: 7928 292e 4765 7449 6e74 6572 706f 6c61  y().GetInterpola
-000245e0: 7469 6f6e 4173 5374 7269 6e67 2829 290a  tionAsString()).
-000245f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024600: 2020 2020 6966 2069 6e74 7270 203e 2030      if intrp > 0
-00024610: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00024620: 2020 2020 2020 2020 2020 6961 2e47 6574            ia.Get
-00024630: 5072 6f70 6572 7479 2829 2e53 6574 496e  Property().SetIn
-00024640: 7465 7270 6f6c 6174 696f 6e28 3029 2020  terpolation(0)  
-00024650: 2320 666c 6174 0a20 2020 2020 2020 2020  # flat.         
-00024660: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00024670: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00024680: 2020 2020 2020 2020 2069 612e 4765 7450           ia.GetP
-00024690: 726f 7065 7274 7928 292e 5365 7449 6e74  roperty().SetInt
-000246a0: 6572 706f 6c61 7469 6f6e 2832 2920 2023  erpolation(2)  #
-000246b0: 2070 686f 6e67 0a0a 2020 2020 2020 2020   phong..        
-000246c0: 656c 6966 206b 6579 203d 3d20 226e 223a  elif key == "n":
-000246d0: 2020 2320 7368 6f77 206e 6f72 6d61 6c73    # show normals
-000246e0: 2074 6f20 616e 2061 6374 6f72 0a20 2020   to an actor.   
-000246f0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-00024700: 2e63 6c69 636b 6564 5f61 6374 6f72 2069  .clicked_actor i
-00024710: 6e20 7365 6c66 2e67 6574 5f6d 6573 6865  n self.get_meshe
-00024720: 7328 293a 0a20 2020 2020 2020 2020 2020  s():.           
-00024730: 2020 2020 2069 6620 7365 6c66 2e63 6c69       if self.cli
-00024740: 636b 6564 5f61 6374 6f72 2e47 6574 5069  cked_actor.GetPi
-00024750: 636b 6162 6c65 2829 3a0a 2020 2020 2020  ckable():.      
-00024760: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00024770: 6c66 2e72 656e 6465 7265 722e 4164 6441  lf.renderer.AddA
-00024780: 6374 6f72 2876 6564 6f2e 7368 6170 6573  ctor(vedo.shapes
-00024790: 2e4e 6f72 6d61 6c4c 696e 6573 2873 656c  .NormalLines(sel
-000247a0: 662e 636c 6963 6b65 645f 6163 746f 7229  f.clicked_actor)
-000247b0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000247c0: 2020 2020 2020 6972 656e 2e52 656e 6465        iren.Rende
-000247d0: 7228 290a 2020 2020 2020 2020 2020 2020  r().            
-000247e0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-000247f0: 2020 2020 2020 7072 696e 7428 2243 6c69        print("Cli
-00024800: 636b 2061 6e20 6163 746f 7220 616e 6420  ck an actor and 
-00024810: 7072 6573 7320 6e20 746f 2061 6464 206e  press n to add n
-00024820: 6f72 6d61 6c73 2e22 290a 0a20 2020 2020  ormals.")..     
-00024830: 2020 2065 6c69 6620 6b65 7920 3d3d 2022     elif key == "
-00024840: 7822 3a0a 2020 2020 2020 2020 2020 2020  x":.            
-00024850: 6966 2073 656c 662e 6a75 7374 7265 6d6f  if self.justremo
-00024860: 7665 6420 6973 204e 6f6e 653a 0a20 2020  ved is None:.   
-00024870: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00024880: 7365 6c66 2e63 6c69 636b 6564 5f61 6374  self.clicked_act
-00024890: 6f72 2069 6e20 7365 6c66 2e67 6574 5f6d  or in self.get_m
-000248a0: 6573 6865 7328 2920 6f72 2069 7369 6e73  eshes() or isins
-000248b0: 7461 6e63 6528 0a20 2020 2020 2020 2020  tance(.         
-000248c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000248d0: 636c 6963 6b65 645f 6163 746f 722c 2076  clicked_actor, v
-000248e0: 746b 2e76 746b 4173 7365 6d62 6c79 0a20  tk.vtkAssembly. 
-000248f0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00024900: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00024910: 2020 2020 2020 7365 6c66 2e6a 7573 7472        self.justr
-00024920: 656d 6f76 6564 203d 2073 656c 662e 636c  emoved = self.cl
-00024930: 6963 6b65 645f 6163 746f 720a 2020 2020  icked_actor.    
-00024940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024950: 7365 6c66 2e72 656e 6465 7265 722e 5265  self.renderer.Re
-00024960: 6d6f 7665 4163 746f 7228 7365 6c66 2e63  moveActor(self.c
-00024970: 6c69 636b 6564 5f61 6374 6f72 290a 2020  licked_actor).  
-00024980: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-00024990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000249a0: 7365 6c66 2e72 656e 6465 7265 722e 4164  self.renderer.Ad
-000249b0: 6441 6374 6f72 2873 656c 662e 6a75 7374  dActor(self.just
-000249c0: 7265 6d6f 7665 6429 0a20 2020 2020 2020  removed).       
-000249d0: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
-000249e0: 6e64 6572 6572 2e52 656e 6465 7228 290a  nderer.Render().
-000249f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024a00: 7365 6c66 2e6a 7573 7472 656d 6f76 6564  self.justremoved
-00024a10: 203d 204e 6f6e 650a 0a20 2020 2020 2020   = None..       
-00024a20: 2065 6c69 6620 6b65 7920 3d3d 2022 5822   elif key == "X"
-00024a30: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00024a40: 2073 656c 662e 636c 6963 6b65 645f 6163   self.clicked_ac
-00024a50: 746f 723a 0a20 2020 2020 2020 2020 2020  tor:.           
-00024a60: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
-00024a70: 2e63 7574 7465 725f 7769 6467 6574 3a0a  .cutter_widget:.
-00024a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024a90: 2020 2020 7365 6c66 2e63 7574 7465 725f      self.cutter_
-00024aa0: 7769 6467 6574 203d 2061 6464 6f6e 732e  widget = addons.
-00024ab0: 426f 7843 7574 7465 7228 7365 6c66 2e63  BoxCutter(self.c
-00024ac0: 6c69 636b 6564 5f61 6374 6f72 290a 2020  licked_actor).  
-00024ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024ae0: 2020 7365 6c66 2e61 6464 2873 656c 662e    self.add(self.
-00024af0: 6375 7474 6572 5f77 6964 6765 7429 0a20  cutter_widget). 
-00024b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024b10: 2020 2070 7269 6e74 2822 5072 6573 7320     print("Press 
-00024b20: 5368 6966 742b 5820 746f 2063 6c6f 7365  Shift+X to close
-00024b30: 2074 6865 2063 7574 7465 7220 626f 7820   the cutter box 
-00024b40: 7769 6467 6574 2c20 4374 726c 2b73 2074  widget, Ctrl+s t
-00024b50: 6f20 7361 7665 2074 6865 2063 7574 2073  o save the cut s
-00024b60: 6563 7469 6f6e 2e22 290a 2020 2020 2020  ection.").      
-00024b70: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-00024b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024b90: 2020 2020 7365 6c66 2e72 656d 6f76 6528      self.remove(
-00024ba0: 7365 6c66 2e63 7574 7465 725f 7769 6467  self.cutter_widg
-00024bb0: 6574 290a 2020 2020 2020 2020 2020 2020  et).            
-00024bc0: 2020 2020 2020 2020 7365 6c66 2e63 7574          self.cut
-00024bd0: 7465 725f 7769 6467 6574 203d 204e 6f6e  ter_widget = Non
-00024be0: 650a 2020 2020 2020 2020 2020 2020 656c  e.            el
-00024bf0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00024c00: 2020 2020 666f 7220 6120 696e 2073 656c      for a in sel
-00024c10: 662e 6163 746f 7273 3a0a 2020 2020 2020  f.actors:.      
-00024c20: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00024c30: 2069 7369 6e73 7461 6e63 6528 612c 2076   isinstance(a, v
-00024c40: 746b 2e76 746b 566f 6c75 6d65 293a 0a20  tk.vtkVolume):. 
-00024c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024c60: 2020 2020 2020 2061 6464 6f6e 732e 6164         addons.ad
-00024c70: 645f 6375 7474 6572 5f74 6f6f 6c28 6129  d_cutter_tool(a)
-00024c80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00024c90: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
-00024ca0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00024cb0: 2076 6564 6f2e 7072 696e 7463 2822 436c   vedo.printc("Cl
-00024cc0: 6963 6b20 6f62 6a65 6374 2061 6e64 2070  ick object and p
-00024cd0: 7265 7373 2058 2074 6f20 6f70 656e 2074  ress X to open t
-00024ce0: 6865 2063 7574 7465 7220 626f 7820 7769  he cutter box wi
-00024cf0: 6467 6574 2e22 2c20 633d 3429 0a0a 2020  dget.", c=4)..  
-00024d00: 2020 2020 2020 656c 6966 206b 6579 203d        elif key =
-00024d10: 3d20 2245 223a 0a20 2020 2020 2020 2020  = "E":.         
-00024d20: 2020 2076 6564 6f2e 7072 696e 7463 2872     vedo.printc(r
-00024d30: 223a 6361 6d65 7261 3a20 4578 706f 7274  ":camera: Export
-00024d40: 696e 6720 3344 2077 696e 646f 7720 746f  ing 3D window to
-00024d50: 2066 696c 6522 2c20 633d 2262 6c75 6522   file", c="blue"
-00024d60: 2c20 656e 643d 2222 290a 2020 2020 2020  , end="").      
-00024d70: 2020 2020 2020 7665 646f 2e66 696c 655f        vedo.file_
-00024d80: 696f 2e65 7870 6f72 745f 7769 6e64 6f77  io.export_window
-00024d90: 2822 7363 656e 652e 6e70 7a22 290a 2020  ("scene.npz").  
-00024da0: 2020 2020 2020 2020 2020 7665 646f 2e70            vedo.p
-00024db0: 7269 6e74 6328 222e 2054 7279 3a5c 6e3e  rintc(". Try:\n>
-00024dc0: 2076 6564 6f20 7363 656e 652e 6e70 7a22   vedo scene.npz"
-00024dd0: 2c20 633d 2262 6c75 6522 290a 0a20 2020  , c="blue")..   
-00024de0: 2020 2020 2065 6c69 6620 6b65 7920 3d3d       elif key ==
-00024df0: 2022 4622 3a0a 2020 2020 2020 2020 2020   "F":.          
-00024e00: 2020 7665 646f 2e66 696c 655f 696f 2e65    vedo.file_io.e
-00024e10: 7870 6f72 745f 7769 6e64 6f77 2822 7363  xport_window("sc
-00024e20: 656e 652e 7833 6422 290a 2020 2020 2020  ene.x3d").      
-00024e30: 2020 2020 2020 7665 646f 2e70 7269 6e74        vedo.print
-00024e40: 6328 223a 6964 6561 3a20 5472 793a 2066  c(":idea: Try: f
-00024e50: 6972 6566 6f78 2073 6365 6e65 2e68 746d  irefox scene.htm
-00024e60: 6c22 2c20 633d 2262 6c75 6522 290a 0a20  l", c="blue").. 
-00024e70: 2020 2020 2020 2065 6c69 6620 6b65 7920         elif key 
-00024e80: 3d3d 2022 6922 3a20 2023 2070 7269 6e74  == "i":  # print
-00024e90: 2069 6e66 6f0a 2020 2020 2020 2020 2020   info.          
-00024ea0: 2020 6966 2073 656c 662e 636c 6963 6b65    if self.clicke
-00024eb0: 645f 6163 746f 723a 0a20 2020 2020 2020  d_actor:.       
-00024ec0: 2020 2020 2020 2020 2075 7469 6c73 2e70           utils.p
-00024ed0: 7269 6e74 5f69 6e66 6f28 7365 6c66 2e63  rint_info(self.c
-00024ee0: 6c69 636b 6564 5f61 6374 6f72 290a 2020  licked_actor).  
-00024ef0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-00024f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024f10: 7574 696c 732e 7072 696e 745f 696e 666f  utils.print_info
-00024f20: 2873 656c 6629 0a0a 2020 2020 2020 2020  (self)..        
-00024f30: 656c 6966 206b 6579 203d 3d20 2249 223a  elif key == "I":
-00024f40: 2020 2320 7072 696e 7420 636f 6c6f 7220    # print color 
-00024f50: 756e 6465 7220 7468 6520 6d6f 7573 650a  under the mouse.
-00024f60: 2020 2020 2020 2020 2020 2020 782c 2079              x, y
-00024f70: 203d 2069 7265 6e2e 4765 7445 7665 6e74   = iren.GetEvent
-00024f80: 506f 7369 7469 6f6e 2829 0a20 2020 2020  Position().     
-00024f90: 2020 2020 2020 2073 656c 662e 636f 6c6f         self.colo
-00024fa0: 725f 7069 636b 6572 285b 782c 2079 5d2c  r_picker([x, y],
-00024fb0: 2076 6572 626f 7365 3d54 7275 6529 0a0a   verbose=True)..
-00024fc0: 2020 2020 2020 2020 656c 6966 206b 6579          elif key
-00024fd0: 203d 3d20 2279 223a 0a20 2020 2020 2020   == "y":.       
-00024fe0: 2020 2020 2069 6620 7365 6c66 2e63 6c69       if self.cli
-00024ff0: 636b 6564 5f61 6374 6f72 2061 6e64 2073  cked_actor and s
-00025000: 656c 662e 636c 6963 6b65 645f 6163 746f  elf.clicked_acto
-00025010: 722e 7069 7065 6c69 6e65 3a0a 2020 2020  r.pipeline:.    
-00025020: 2020 2020 2020 2020 2020 2020 2320 7365              # se
-00025030: 6c66 2e63 6c69 636b 6564 5f61 6374 6f72  lf.clicked_actor
-00025040: 2e70 6970 656c 696e 6520 3d20 2075 7469  .pipeline =  uti
-00025050: 6c73 2e4f 7065 7261 7469 6f6e 4e6f 6465  ls.OperationNode
-00025060: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00025070: 2020 2320 2020 2020 2020 2020 2273 686f    #         "sho
-00025080: 7722 2c20 7061 7265 6e74 733d 5b73 656c  w", parents=[sel
-00025090: 662e 636c 6963 6b65 645f 6163 746f 725d  f.clicked_actor]
-000250a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000250b0: 2020 2320 2020 2020 2020 2020 7368 6170    #         shap
-000250c0: 653d 2263 6972 636c 6522 2c0a 2020 2020  e="circle",.    
-000250d0: 2020 2020 2020 2020 2020 2020 2320 290a              # ).
-000250e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000250f0: 7365 6c66 2e63 6c69 636b 6564 5f61 6374  self.clicked_act
-00025100: 6f72 2e70 6970 656c 696e 652e 7368 6f77  or.pipeline.show
-00025110: 2829 0a0a 2020 2020 2020 2020 6966 2069  ()..        if i
-00025120: 7265 6e3a 0a20 2020 2020 2020 2020 2020  ren:.           
-00025130: 2069 7265 6e2e 5265 6e64 6572 2829 0a     iren.Render().
+00023300: 2020 2020 2020 2020 2020 2020 626e 7320              bns 
+00023310: 3d20 7365 6c66 2e72 656e 6465 7265 722e  = self.renderer.
+00023320: 436f 6d70 7574 6556 6973 6962 6c65 5072  ComputeVisiblePr
+00023330: 6f70 426f 756e 6473 2829 0a20 2020 2020  opBounds().     
+00023340: 2020 2020 2020 2020 2020 2061 6464 6f6e             addon
+00023350: 732e 6164 645f 676c 6f62 616c 5f61 7865  s.add_global_axe
+00023360: 7328 6178 7479 7065 3d28 7365 6c66 2e61  s(axtype=(self.a
+00023370: 7865 7320 2d20 3129 2025 2031 352c 2063  xes - 1) % 15, c
+00023380: 3d4e 6f6e 652c 2062 6f75 6e64 733d 626e  =None, bounds=bn
+00023390: 7329 0a20 2020 2020 2020 2020 2020 2065  s).            e
+000233a0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+000233b0: 2020 2020 2069 6620 6e6f 7420 7365 7474       if not sett
+000233c0: 696e 6773 2e75 7365 5f70 6172 616c 6c65  ings.use_paralle
+000233d0: 6c5f 7072 6f6a 6563 7469 6f6e 2061 6e64  l_projection and
+000233e0: 2073 656c 662e 6178 6573 203d 3d20 3132   self.axes == 12
+000233f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00023400: 2020 2020 2020 7365 6c66 2e61 7865 7320        self.axes 
+00023410: 2b3d 2031 2020 2320 6a75 6d70 2072 756c  += 1  # jump rul
+00023420: 6572 2064 6f65 736e 7420 6d61 6b65 2073  er doesnt make s
+00023430: 656e 7365 2069 6e20 7065 7273 7065 6374  ense in perspect
+00023440: 6976 6520 6d6f 6465 0a20 2020 2020 2020  ive mode.       
+00023450: 2020 2020 2020 2020 2062 6e73 203d 2073           bns = s
+00023460: 656c 662e 7265 6e64 6572 6572 2e43 6f6d  elf.renderer.Com
+00023470: 7075 7465 5669 7369 626c 6550 726f 7042  puteVisiblePropB
+00023480: 6f75 6e64 7328 290a 2020 2020 2020 2020  ounds().        
+00023490: 2020 2020 2020 2020 6164 646f 6e73 2e61          addons.a
+000234a0: 6464 5f67 6c6f 6261 6c5f 6178 6573 2861  dd_global_axes(a
+000234b0: 7874 7970 653d 2873 656c 662e 6178 6573  xtype=(self.axes
+000234c0: 202b 2031 2920 2520 3135 2c20 633d 4e6f   + 1) % 15, c=No
+000234d0: 6e65 2c20 626f 756e 6473 3d62 6e73 290a  ne, bounds=bns).
+000234e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000234f0: 2e69 6e74 6572 6163 746f 722e 5265 6e64  .interactor.Rend
+00023500: 6572 2829 0a0a 2020 2020 2020 2020 656c  er()..        el
+00023510: 6966 2022 4b50 5f22 2069 6e20 6b65 7920  if "KP_" in key 
+00023520: 6f72 206b 6579 2069 6e20 5b0a 2020 2020  or key in [.    
+00023530: 2020 2020 2020 2020 2249 6e73 6572 7422          "Insert"
+00023540: 2c0a 2020 2020 2020 2020 2020 2020 2245  ,.            "E
+00023550: 6e64 222c 0a20 2020 2020 2020 2020 2020  nd",.           
+00023560: 2022 446f 776e 222c 0a20 2020 2020 2020   "Down",.       
+00023570: 2020 2020 2022 4e65 7874 222c 0a20 2020       "Next",.   
+00023580: 2020 2020 2020 2020 2022 4c65 6674 222c           "Left",
+00023590: 0a20 2020 2020 2020 2020 2020 2022 4265  .            "Be
+000235a0: 6769 6e22 2c0a 2020 2020 2020 2020 2020  gin",.          
+000235b0: 2020 2252 6967 6874 222c 0a20 2020 2020    "Right",.     
+000235c0: 2020 2020 2020 2022 486f 6d65 222c 0a20         "Home",. 
+000235d0: 2020 2020 2020 2020 2020 2022 5570 222c             "Up",
+000235e0: 0a20 2020 2020 2020 2020 2020 2022 5072  .            "Pr
+000235f0: 696f 7222 2c0a 2020 2020 2020 2020 5d3a  ior",.        ]:
+00023600: 0a20 2020 2020 2020 2020 2020 2023 2063  .            # c
+00023610: 6861 6e67 6520 6178 6573 2073 7479 6c65  hange axes style
+00023620: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
+00023630: 6f20 3d20 7b0a 2020 2020 2020 2020 2020  o = {.          
+00023640: 2020 2020 2020 224b 505f 496e 7365 7274        "KP_Insert
+00023650: 223a 2030 2c0a 2020 2020 2020 2020 2020  ": 0,.          
+00023660: 2020 2020 2020 224b 505f 3022 3a20 302c        "KP_0": 0,
+00023670: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00023680: 2022 4b50 5f45 6e64 223a 2031 2c0a 2020   "KP_End": 1,.  
+00023690: 2020 2020 2020 2020 2020 2020 2020 224b                "K
+000236a0: 505f 3122 3a20 312c 0a20 2020 2020 2020  P_1": 1,.       
+000236b0: 2020 2020 2020 2020 2022 4b50 5f44 6f77           "KP_Dow
+000236c0: 6e22 3a20 322c 0a20 2020 2020 2020 2020  n": 2,.         
+000236d0: 2020 2020 2020 2022 4b50 5f32 223a 2032         "KP_2": 2
+000236e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000236f0: 2020 224b 505f 4e65 7874 223a 2033 2c0a    "KP_Next": 3,.
+00023700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023710: 224b 505f 3322 3a20 332c 0a20 2020 2020  "KP_3": 3,.     
+00023720: 2020 2020 2020 2020 2020 2022 4b50 5f4c             "KP_L
+00023730: 6566 7422 3a20 342c 0a20 2020 2020 2020  eft": 4,.       
+00023740: 2020 2020 2020 2020 2022 4b50 5f34 223a           "KP_4":
+00023750: 2034 2c0a 2020 2020 2020 2020 2020 2020   4,.            
+00023760: 2020 2020 224b 505f 4265 6769 6e22 3a20      "KP_Begin": 
+00023770: 352c 0a20 2020 2020 2020 2020 2020 2020  5,.             
+00023780: 2020 2022 4b50 5f35 223a 2035 2c0a 2020     "KP_5": 5,.  
+00023790: 2020 2020 2020 2020 2020 2020 2020 224b                "K
+000237a0: 505f 5269 6768 7422 3a20 362c 0a20 2020  P_Right": 6,.   
+000237b0: 2020 2020 2020 2020 2020 2020 2022 4b50               "KP
+000237c0: 5f36 223a 2036 2c0a 2020 2020 2020 2020  _6": 6,.        
+000237d0: 2020 2020 2020 2020 224b 505f 486f 6d65          "KP_Home
+000237e0: 223a 2037 2c0a 2020 2020 2020 2020 2020  ": 7,.          
+000237f0: 2020 2020 2020 224b 505f 3722 3a20 372c        "KP_7": 7,
+00023800: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00023810: 2022 4b50 5f55 7022 3a20 382c 0a20 2020   "KP_Up": 8,.   
+00023820: 2020 2020 2020 2020 2020 2020 2022 4b50               "KP
+00023830: 5f38 223a 2038 2c0a 2020 2020 2020 2020  _8": 8,.        
+00023840: 2020 2020 2020 2020 2250 7269 6f72 223a          "Prior":
+00023850: 2039 2c20 2023 206f 6e20 7769 6e64 6f77   9,  # on window
+00023860: 7320 4f53 0a20 2020 2020 2020 2020 2020  s OS.           
+00023870: 2020 2020 2022 496e 7365 7274 223a 2030       "Insert": 0
+00023880: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00023890: 2020 2245 6e64 223a 2031 2c0a 2020 2020    "End": 1,.    
+000238a0: 2020 2020 2020 2020 2020 2020 2244 6f77              "Dow
+000238b0: 6e22 3a20 322c 0a20 2020 2020 2020 2020  n": 2,.         
+000238c0: 2020 2020 2020 2022 4e65 7874 223a 2033         "Next": 3
+000238d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000238e0: 2020 224c 6566 7422 3a20 342c 0a20 2020    "Left": 4,.   
+000238f0: 2020 2020 2020 2020 2020 2020 2022 4265               "Be
+00023900: 6769 6e22 3a20 352c 0a20 2020 2020 2020  gin": 5,.       
+00023910: 2020 2020 2020 2020 2022 5269 6768 7422           "Right"
+00023920: 3a20 362c 0a20 2020 2020 2020 2020 2020  : 6,.           
+00023930: 2020 2020 2022 486f 6d65 223a 2037 2c0a       "Home": 7,.
+00023940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023950: 2255 7022 3a20 382c 0a20 2020 2020 2020  "Up": 8,.       
+00023960: 2020 2020 2020 2020 2022 5072 696f 7222           "Prior"
+00023970: 3a20 392c 0a20 2020 2020 2020 2020 2020  : 9,.           
+00023980: 207d 0a20 2020 2020 2020 2020 2020 2063   }.            c
+00023990: 6c69 636b 6564 7220 3d20 7365 6c66 2e72  lickedr = self.r
+000239a0: 656e 6465 7265 7273 2e69 6e64 6578 2872  enderers.index(r
+000239b0: 656e 6465 7265 7229 0a20 2020 2020 2020  enderer).       
+000239c0: 2020 2020 2069 6620 6b65 7920 696e 2061       if key in a
+000239d0: 7373 6f3a 0a20 2020 2020 2020 2020 2020  sso:.           
+000239e0: 2020 2020 2069 6620 7365 6c66 2e61 7865       if self.axe
+000239f0: 735f 696e 7374 616e 6365 735b 636c 6963  s_instances[clic
+00023a00: 6b65 6472 5d3a 0a20 2020 2020 2020 2020  kedr]:.         
+00023a10: 2020 2020 2020 2020 2020 2069 6620 6861             if ha
+00023a20: 7361 7474 7228 7365 6c66 2e61 7865 735f  sattr(self.axes_
+00023a30: 696e 7374 616e 6365 735b 636c 6963 6b65  instances[clicke
+00023a40: 6472 5d2c 2022 456e 6162 6c65 644f 6666  dr], "EnabledOff
+00023a50: 2229 3a20 2023 2077 6964 6765 740a 2020  "):  # widget.  
+00023a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023a70: 2020 2020 2020 7365 6c66 2e61 7865 735f        self.axes_
+00023a80: 696e 7374 616e 6365 735b 636c 6963 6b65  instances[clicke
+00023a90: 6472 5d2e 456e 6162 6c65 644f 6666 2829  dr].EnabledOff()
+00023aa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00023ab0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00023ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023ad0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+00023ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023af0: 2020 2020 7265 6e64 6572 6572 2e52 656d      renderer.Rem
+00023b00: 6f76 6541 6374 6f72 2873 656c 662e 6178  oveActor(self.ax
+00023b10: 6573 5f69 6e73 7461 6e63 6573 5b63 6c69  es_instances[cli
+00023b20: 636b 6564 725d 290a 2020 2020 2020 2020  ckedr]).        
+00023b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023b40: 6578 6365 7074 3a0a 2020 2020 2020 2020  except:.        
+00023b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023b60: 2020 2020 7061 7373 0a20 2020 2020 2020      pass.       
+00023b70: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00023b80: 662e 6178 6573 5f69 6e73 7461 6e63 6573  f.axes_instances
+00023b90: 5b63 6c69 636b 6564 725d 203d 204e 6f6e  [clickedr] = Non
+00023ba0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00023bb0: 2020 626f 756e 6473 203d 2072 656e 6465    bounds = rende
+00023bc0: 7265 722e 436f 6d70 7574 6556 6973 6962  rer.ComputeVisib
+00023bd0: 6c65 5072 6f70 426f 756e 6473 2829 0a20  lePropBounds(). 
+00023be0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00023bf0: 6464 6f6e 732e 6164 645f 676c 6f62 616c  ddons.add_global
+00023c00: 5f61 7865 7328 6178 7479 7065 3d61 7373  _axes(axtype=ass
+00023c10: 6f5b 6b65 795d 2c20 633d 4e6f 6e65 2c20  o[key], c=None, 
+00023c20: 626f 756e 6473 3d62 6f75 6e64 7329 0a20  bounds=bounds). 
+00023c30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00023c40: 656c 662e 696e 7465 7261 6374 6f72 2e52  elf.interactor.R
+00023c50: 656e 6465 7228 290a 0a20 2020 2020 2020  ender()..       
+00023c60: 2069 6620 6b65 7920 3d3d 2022 4f22 3a0a   if key == "O":.
+00023c70: 2020 2020 2020 2020 2020 2020 7265 6e64              rend
+00023c80: 6572 6572 2e52 656d 6f76 654c 6967 6874  erer.RemoveLight
+00023c90: 2873 656c 662e 5f65 7874 7261 6c69 6768  (self._extraligh
+00023ca0: 7429 0a20 2020 2020 2020 2020 2020 2073  t).            s
+00023cb0: 656c 662e 5f65 7874 7261 6c69 6768 7420  elf._extralight 
+00023cc0: 3d20 4e6f 6e65 0a0a 2020 2020 2020 2020  = None..        
+00023cd0: 656c 6966 206b 6579 203d 3d20 226f 223a  elif key == "o":
+00023ce0: 0a20 2020 2020 2020 2020 2020 2076 6262  .            vbb
+00023cf0: 2c20 7369 7a65 732c 205f 2c20 5f20 3d20  , sizes, _, _ = 
+00023d00: 6164 646f 6e73 2e63 6f6d 7075 7465 5f76  addons.compute_v
+00023d10: 6973 6962 6c65 5f62 6f75 6e64 7328 290a  isible_bounds().
+00023d20: 2020 2020 2020 2020 2020 2020 636d 203d              cm =
+00023d30: 2075 7469 6c73 2e76 6563 746f 7228 2876   utils.vector((v
+00023d40: 6262 5b30 5d20 2b20 7662 625b 315d 2920  bb[0] + vbb[1]) 
+00023d50: 2f20 322c 2028 7662 625b 325d 202b 2076  / 2, (vbb[2] + v
+00023d60: 6262 5b33 5d29 202f 2032 2c20 2876 6262  bb[3]) / 2, (vbb
+00023d70: 5b34 5d20 2b20 7662 625b 355d 2920 2f20  [4] + vbb[5]) / 
+00023d80: 3229 0a20 2020 2020 2020 2020 2020 2069  2).            i
+00023d90: 6620 6e6f 7420 7365 6c66 2e5f 6578 7472  f not self._extr
+00023da0: 616c 6967 6874 3a0a 2020 2020 2020 2020  alight:.        
+00023db0: 2020 2020 2020 2020 7675 7020 3d20 7265          vup = re
+00023dc0: 6e64 6572 6572 2e47 6574 4163 7469 7665  nderer.GetActive
+00023dd0: 4361 6d65 7261 2829 2e47 6574 5669 6577  Camera().GetView
+00023de0: 5570 2829 0a20 2020 2020 2020 2020 2020  Up().           
+00023df0: 2020 2020 2070 6f73 203d 2063 6d20 2b20       pos = cm + 
+00023e00: 7574 696c 732e 7665 6374 6f72 2876 7570  utils.vector(vup
+00023e10: 2920 2a20 7574 696c 732e 6d61 6728 7369  ) * utils.mag(si
+00023e20: 7a65 7329 0a20 2020 2020 2020 2020 2020  zes).           
+00023e30: 2020 2020 2073 656c 662e 5f65 7874 7261       self._extra
+00023e40: 6c69 6768 7420 3d20 6164 646f 6e73 2e4c  light = addons.L
+00023e50: 6967 6874 2870 6f73 2c20 666f 6361 6c5f  ight(pos, focal_
+00023e60: 706f 696e 743d 636d 290a 2020 2020 2020  point=cm).      
+00023e70: 2020 2020 2020 2020 2020 7265 6e64 6572            render
+00023e80: 6572 2e41 6464 4c69 6768 7428 7365 6c66  er.AddLight(self
+00023e90: 2e5f 6578 7472 616c 6967 6874 290a 2020  ._extralight).  
+00023ea0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00023eb0: 696e 7428 2250 7265 7373 2061 6761 696e  int("Press again
+00023ec0: 206f 2074 6f20 726f 7461 7465 206c 6967   o to rotate lig
+00023ed0: 6874 2073 6f75 7263 652c 206f 7220 4f20  ht source, or O 
+00023ee0: 746f 2072 656d 6f76 6520 6974 2e22 290a  to remove it.").
+00023ef0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00023f00: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00023f10: 2020 6370 6f73 203d 2075 7469 6c73 2e76    cpos = utils.v
+00023f20: 6563 746f 7228 7365 6c66 2e5f 6578 7472  ector(self._extr
+00023f30: 616c 6967 6874 2e47 6574 506f 7369 7469  alight.GetPositi
+00023f40: 6f6e 2829 290a 2020 2020 2020 2020 2020  on()).          
+00023f50: 2020 2020 2020 782c 2079 2c20 7a20 3d20        x, y, z = 
+00023f60: 7365 6c66 2e5f 6578 7472 616c 6967 6874  self._extralight
+00023f70: 2e47 6574 506f 7369 7469 6f6e 2829 202d  .GetPosition() -
+00023f80: 2063 6d0a 2020 2020 2020 2020 2020 2020   cm.            
+00023f90: 2020 2020 722c 2074 682c 2070 6820 3d20      r, th, ph = 
+00023fa0: 7574 696c 732e 6361 7274 3273 7068 6572  utils.cart2spher
+00023fb0: 2878 2c20 792c 207a 290a 2020 2020 2020  (x, y, z).      
+00023fc0: 2020 2020 2020 2020 2020 7468 202b 3d20            th += 
+00023fd0: 302e 320a 2020 2020 2020 2020 2020 2020  0.2.            
+00023fe0: 2020 2020 6966 2074 6820 3e20 6e70 2e70      if th > np.p
+00023ff0: 693a 0a20 2020 2020 2020 2020 2020 2020  i:.             
+00024000: 2020 2020 2020 2074 6820 3d20 6e70 2e72         th = np.r
+00024010: 616e 646f 6d2e 7261 6e64 6f6d 2829 202a  andom.random() *
+00024020: 206e 702e 7069 202f 2032 0a20 2020 2020   np.pi / 2.     
+00024030: 2020 2020 2020 2020 2020 2070 6820 2b3d             ph +=
+00024040: 2030 2e33 0a20 2020 2020 2020 2020 2020   0.3.           
+00024050: 2020 2020 2063 706f 7320 3d20 7574 696c       cpos = util
+00024060: 732e 7370 6865 7232 6361 7274 2872 2c20  s.spher2cart(r, 
+00024070: 7468 2c20 7068 2920 2b20 636d 0a20 2020  th, ph) + cm.   
+00024080: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00024090: 662e 5f65 7874 7261 6c69 6768 742e 5365  f._extralight.Se
+000240a0: 7450 6f73 6974 696f 6e28 6370 6f73 290a  tPosition(cpos).
+000240b0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000240c0: 662e 7769 6e64 6f77 2e52 656e 6465 7228  f.window.Render(
+000240d0: 290a 0a20 2020 2020 2020 2065 6c69 6620  )..        elif 
+000240e0: 6b65 7920 3d3d 2022 6c22 3a0a 2020 2020  key == "l":.    
+000240f0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00024100: 636c 6963 6b65 645f 6163 746f 7220 696e  clicked_actor in
+00024110: 2073 656c 662e 6765 745f 6d65 7368 6573   self.get_meshes
+00024120: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00024130: 2020 2020 6163 7473 203d 205b 7365 6c66      acts = [self
+00024140: 2e63 6c69 636b 6564 5f61 6374 6f72 5d0a  .clicked_actor].
+00024150: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00024160: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00024170: 2020 6163 7473 203d 2073 656c 662e 6765    acts = self.ge
+00024180: 745f 6d65 7368 6573 2829 0a20 2020 2020  t_meshes().     
+00024190: 2020 2020 2020 2066 6f72 2069 6120 696e         for ia in
+000241a0: 2061 6374 733a 0a20 2020 2020 2020 2020   acts:.         
+000241b0: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+000241c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000241d0: 6576 203d 2069 612e 4765 7450 726f 7065  ev = ia.GetPrope
+000241e0: 7274 7928 292e 4765 7445 6467 6556 6973  rty().GetEdgeVis
+000241f0: 6962 696c 6974 7928 290a 2020 2020 2020  ibility().      
+00024200: 2020 2020 2020 2020 2020 2020 2020 6961                ia
+00024210: 2e47 6574 5072 6f70 6572 7479 2829 2e53  .GetProperty().S
+00024220: 6574 4564 6765 5669 7369 6269 6c69 7479  etEdgeVisibility
+00024230: 286e 6f74 2065 7629 0a20 2020 2020 2020  (not ev).       
+00024240: 2020 2020 2020 2020 2020 2020 2069 612e               ia.
+00024250: 4765 7450 726f 7065 7274 7928 292e 5365  GetProperty().Se
+00024260: 7452 6570 7265 7365 6e74 6174 696f 6e54  tRepresentationT
+00024270: 6f53 7572 6661 6365 2829 0a20 2020 2020  oSurface().     
+00024280: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00024290: 612e 4765 7450 726f 7065 7274 7928 292e  a.GetProperty().
+000242a0: 5365 744c 696e 6557 6964 7468 2830 2e31  SetLineWidth(0.1
+000242b0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000242c0: 2020 6578 6365 7074 2041 7474 7269 6275    except Attribu
+000242d0: 7465 4572 726f 723a 0a20 2020 2020 2020  teError:.       
+000242e0: 2020 2020 2020 2020 2020 2020 2070 6173               pas
+000242f0: 730a 0a20 2020 2020 2020 2065 6c69 6620  s..        elif 
+00024300: 6b65 7920 3d3d 2022 6b22 3a20 2023 206c  key == "k":  # l
+00024310: 6967 6874 696e 6773 0a20 2020 2020 2020  ightings.       
+00024320: 2020 2020 2069 6620 7365 6c66 2e63 6c69       if self.cli
+00024330: 636b 6564 5f61 6374 6f72 2069 6e20 7365  cked_actor in se
+00024340: 6c66 2e67 6574 5f6d 6573 6865 7328 293a  lf.get_meshes():
+00024350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00024360: 2061 6374 7320 3d20 5b73 656c 662e 636c   acts = [self.cl
+00024370: 6963 6b65 645f 6163 746f 725d 0a20 2020  icked_actor].   
+00024380: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+00024390: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+000243a0: 6374 7320 3d20 7365 6c66 2e67 6574 5f6d  cts = self.get_m
+000243b0: 6573 6865 7328 290a 2020 2020 2020 2020  eshes().        
+000243c0: 2020 2020 7368 6473 203d 2028 2264 6566      shds = ("def
+000243d0: 6175 6c74 222c 2022 6d65 7461 6c6c 6963  ault", "metallic
+000243e0: 222c 2022 706c 6173 7469 6322 2c20 2273  ", "plastic", "s
+000243f0: 6869 6e79 222c 2022 676c 6f73 7379 222c  hiny", "glossy",
+00024400: 2022 6f66 6622 290a 2020 2020 2020 2020   "off").        
+00024410: 2020 2020 666f 7220 6961 2069 6e20 6163      for ia in ac
+00024420: 7473 3a0a 2020 2020 2020 2020 2020 2020  ts:.            
+00024430: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+00024440: 2020 2020 2020 2020 2020 2020 206c 6e72               lnr
+00024450: 203d 2028 6961 2e5f 6c69 6774 6869 6e67   = (ia._ligthing
+00024460: 6e72 202b 2031 2920 2520 360a 2020 2020  nr + 1) % 6.    
+00024470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024480: 6961 2e6c 6967 6874 696e 6728 7368 6473  ia.lighting(shds
+00024490: 5b6c 6e72 5d29 0a20 2020 2020 2020 2020  [lnr]).         
+000244a0: 2020 2020 2020 2020 2020 2069 612e 5f6c             ia._l
+000244b0: 6967 7468 696e 676e 7220 3d20 6c6e 720a  igthingnr = lnr.
+000244c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000244d0: 6578 6365 7074 2041 7474 7269 6275 7465  except Attribute
+000244e0: 4572 726f 723a 0a20 2020 2020 2020 2020  Error:.         
+000244f0: 2020 2020 2020 2020 2020 2070 6173 730a             pass.
+00024500: 0a20 2020 2020 2020 2065 6c69 6620 6b65  .        elif ke
+00024510: 7920 3d3d 2022 4b22 3a20 2023 2073 6861  y == "K":  # sha
+00024520: 6469 6e67 0a20 2020 2020 2020 2020 2020  ding.           
+00024530: 2069 6620 7365 6c66 2e63 6c69 636b 6564   if self.clicked
+00024540: 5f61 6374 6f72 2069 6e20 7365 6c66 2e67  _actor in self.g
+00024550: 6574 5f6d 6573 6865 7328 293a 0a20 2020  et_meshes():.   
+00024560: 2020 2020 2020 2020 2020 2020 2061 6374               act
+00024570: 7320 3d20 5b73 656c 662e 636c 6963 6b65  s = [self.clicke
+00024580: 645f 6163 746f 725d 0a20 2020 2020 2020  d_actor].       
+00024590: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+000245a0: 2020 2020 2020 2020 2020 2061 6374 7320             acts 
+000245b0: 3d20 7365 6c66 2e67 6574 5f6d 6573 6865  = self.get_meshe
+000245c0: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
+000245d0: 666f 7220 6961 2069 6e20 6163 7473 3a0a  for ia in acts:.
+000245e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000245f0: 6966 2069 7369 6e73 7461 6e63 6528 6961  if isinstance(ia
+00024600: 2c20 7665 646f 2e4d 6573 6829 3a0a 2020  , vedo.Mesh):.  
+00024610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024620: 2020 6961 2e63 6f6d 7075 7465 5f6e 6f72    ia.compute_nor
+00024630: 6d61 6c73 2863 656c 6c73 3d46 616c 7365  mals(cells=False
+00024640: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00024650: 2020 2020 2020 696e 7472 7020 3d20 6961        intrp = ia
+00024660: 2e47 6574 5072 6f70 6572 7479 2829 2e47  .GetProperty().G
+00024670: 6574 496e 7465 7270 6f6c 6174 696f 6e28  etInterpolation(
+00024680: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00024690: 2020 2020 2020 2320 7072 696e 7428 696e        # print(in
+000246a0: 7472 702c 2069 612e 4765 7450 726f 7065  trp, ia.GetPrope
+000246b0: 7274 7928 292e 4765 7449 6e74 6572 706f  rty().GetInterpo
+000246c0: 6c61 7469 6f6e 4173 5374 7269 6e67 2829  lationAsString()
+000246d0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000246e0: 2020 2020 2020 6966 2069 6e74 7270 203e        if intrp >
+000246f0: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
+00024700: 2020 2020 2020 2020 2020 2020 6961 2e47              ia.G
+00024710: 6574 5072 6f70 6572 7479 2829 2e53 6574  etProperty().Set
+00024720: 496e 7465 7270 6f6c 6174 696f 6e28 3029  Interpolation(0)
+00024730: 2020 2320 666c 6174 0a20 2020 2020 2020    # flat.       
+00024740: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00024750: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00024760: 2020 2020 2020 2020 2020 2069 612e 4765             ia.Ge
+00024770: 7450 726f 7065 7274 7928 292e 5365 7449  tProperty().SetI
+00024780: 6e74 6572 706f 6c61 7469 6f6e 2832 2920  nterpolation(2) 
+00024790: 2023 2070 686f 6e67 0a0a 2020 2020 2020   # phong..      
+000247a0: 2020 656c 6966 206b 6579 203d 3d20 226e    elif key == "n
+000247b0: 223a 2020 2320 7368 6f77 206e 6f72 6d61  ":  # show norma
+000247c0: 6c73 2074 6f20 616e 2061 6374 6f72 0a20  ls to an actor. 
+000247d0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+000247e0: 6c66 2e63 6c69 636b 6564 5f61 6374 6f72  lf.clicked_actor
+000247f0: 2069 6e20 7365 6c66 2e67 6574 5f6d 6573   in self.get_mes
+00024800: 6865 7328 293a 0a20 2020 2020 2020 2020  hes():.         
+00024810: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
+00024820: 6c69 636b 6564 5f61 6374 6f72 2e47 6574  licked_actor.Get
+00024830: 5069 636b 6162 6c65 2829 3a0a 2020 2020  Pickable():.    
+00024840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024850: 7365 6c66 2e72 656e 6465 7265 722e 4164  self.renderer.Ad
+00024860: 6441 6374 6f72 2876 6564 6f2e 7368 6170  dActor(vedo.shap
+00024870: 6573 2e4e 6f72 6d61 6c4c 696e 6573 2873  es.NormalLines(s
+00024880: 656c 662e 636c 6963 6b65 645f 6163 746f  elf.clicked_acto
+00024890: 7229 290a 2020 2020 2020 2020 2020 2020  r)).            
+000248a0: 2020 2020 2020 2020 6972 656e 2e52 656e          iren.Ren
+000248b0: 6465 7228 290a 2020 2020 2020 2020 2020  der().          
+000248c0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+000248d0: 2020 2020 2020 2020 7072 696e 7428 2243          print("C
+000248e0: 6c69 636b 2061 6e20 6163 746f 7220 616e  lick an actor an
+000248f0: 6420 7072 6573 7320 6e20 746f 2061 6464  d press n to add
+00024900: 206e 6f72 6d61 6c73 2e22 290a 0a20 2020   normals.")..   
+00024910: 2020 2020 2065 6c69 6620 6b65 7920 3d3d       elif key ==
+00024920: 2022 7822 3a0a 2020 2020 2020 2020 2020   "x":.          
+00024930: 2020 6966 2073 656c 662e 6a75 7374 7265    if self.justre
+00024940: 6d6f 7665 6420 6973 204e 6f6e 653a 0a20  moved is None:. 
+00024950: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00024960: 6620 7365 6c66 2e63 6c69 636b 6564 5f61  f self.clicked_a
+00024970: 6374 6f72 2069 6e20 7365 6c66 2e67 6574  ctor in self.get
+00024980: 5f6d 6573 6865 7328 2920 6f72 2069 7369  _meshes() or isi
+00024990: 6e73 7461 6e63 6528 0a20 2020 2020 2020  nstance(.       
+000249a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000249b0: 662e 636c 6963 6b65 645f 6163 746f 722c  f.clicked_actor,
+000249c0: 2076 746b 2e76 746b 4173 7365 6d62 6c79   vtk.vtkAssembly
+000249d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000249e0: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
+000249f0: 2020 2020 2020 2020 7365 6c66 2e6a 7573          self.jus
+00024a00: 7472 656d 6f76 6564 203d 2073 656c 662e  tremoved = self.
+00024a10: 636c 6963 6b65 645f 6163 746f 720a 2020  clicked_actor.  
+00024a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024a30: 2020 7365 6c66 2e72 656e 6465 7265 722e    self.renderer.
+00024a40: 5265 6d6f 7665 4163 746f 7228 7365 6c66  RemoveActor(self
+00024a50: 2e63 6c69 636b 6564 5f61 6374 6f72 290a  .clicked_actor).
+00024a60: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00024a70: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00024a80: 2020 7365 6c66 2e72 656e 6465 7265 722e    self.renderer.
+00024a90: 4164 6441 6374 6f72 2873 656c 662e 6a75  AddActor(self.ju
+00024aa0: 7374 7265 6d6f 7665 6429 0a20 2020 2020  stremoved).     
+00024ab0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00024ac0: 7265 6e64 6572 6572 2e52 656e 6465 7228  renderer.Render(
+00024ad0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00024ae0: 2020 7365 6c66 2e6a 7573 7472 656d 6f76    self.justremov
+00024af0: 6564 203d 204e 6f6e 650a 0a20 2020 2020  ed = None..     
+00024b00: 2020 2065 6c69 6620 6b65 7920 3d3d 2022     elif key == "
+00024b10: 5822 3a0a 2020 2020 2020 2020 2020 2020  X":.            
+00024b20: 6966 2073 656c 662e 636c 6963 6b65 645f  if self.clicked_
+00024b30: 6163 746f 723a 0a20 2020 2020 2020 2020  actor:.         
+00024b40: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
+00024b50: 6c66 2e63 7574 7465 725f 7769 6467 6574  lf.cutter_widget
+00024b60: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00024b70: 2020 2020 2020 7365 6c66 2e63 7574 7465        self.cutte
+00024b80: 725f 7769 6467 6574 203d 2061 6464 6f6e  r_widget = addon
+00024b90: 732e 426f 7843 7574 7465 7228 7365 6c66  s.BoxCutter(self
+00024ba0: 2e63 6c69 636b 6564 5f61 6374 6f72 290a  .clicked_actor).
+00024bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024bc0: 2020 2020 7365 6c66 2e61 6464 2873 656c      self.add(sel
+00024bd0: 662e 6375 7474 6572 5f77 6964 6765 7429  f.cutter_widget)
+00024be0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00024bf0: 2020 2020 2070 7269 6e74 2822 5072 6573       print("Pres
+00024c00: 7320 5368 6966 742b 5820 746f 2063 6c6f  s Shift+X to clo
+00024c10: 7365 2074 6865 2063 7574 7465 7220 626f  se the cutter bo
+00024c20: 7820 7769 6467 6574 2c20 4374 726c 2b73  x widget, Ctrl+s
+00024c30: 2074 6f20 7361 7665 2074 6865 2063 7574   to save the cut
+00024c40: 2073 6563 7469 6f6e 2e22 290a 2020 2020   section.").    
+00024c50: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00024c60: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00024c70: 2020 2020 2020 7365 6c66 2e72 656d 6f76        self.remov
+00024c80: 6528 7365 6c66 2e63 7574 7465 725f 7769  e(self.cutter_wi
+00024c90: 6467 6574 290a 2020 2020 2020 2020 2020  dget).          
+00024ca0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00024cb0: 7574 7465 725f 7769 6467 6574 203d 204e  utter_widget = N
+00024cc0: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+00024cd0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00024ce0: 2020 2020 2020 666f 7220 6120 696e 2073        for a in s
+00024cf0: 656c 662e 6163 746f 7273 3a0a 2020 2020  elf.actors:.    
+00024d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024d10: 6966 2069 7369 6e73 7461 6e63 6528 612c  if isinstance(a,
+00024d20: 2076 746b 2e76 746b 566f 6c75 6d65 293a   vtk.vtkVolume):
+00024d30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00024d40: 2020 2020 2020 2020 2061 6464 6f6e 732e           addons.
+00024d50: 6164 645f 6375 7474 6572 5f74 6f6f 6c28  add_cutter_tool(
+00024d60: 6129 0a20 2020 2020 2020 2020 2020 2020  a).             
+00024d70: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00024d80: 6e0a 0a20 2020 2020 2020 2020 2020 2020  n..             
+00024d90: 2020 2076 6564 6f2e 7072 696e 7463 2822     vedo.printc("
+00024da0: 436c 6963 6b20 6f62 6a65 6374 2061 6e64  Click object and
+00024db0: 2070 7265 7373 2058 2074 6f20 6f70 656e   press X to open
+00024dc0: 2074 6865 2063 7574 7465 7220 626f 7820   the cutter box 
+00024dd0: 7769 6467 6574 2e22 2c20 633d 3429 0a0a  widget.", c=4)..
+00024de0: 2020 2020 2020 2020 656c 6966 206b 6579          elif key
+00024df0: 203d 3d20 2245 223a 0a20 2020 2020 2020   == "E":.       
+00024e00: 2020 2020 2076 6564 6f2e 7072 696e 7463       vedo.printc
+00024e10: 2872 223a 6361 6d65 7261 3a20 4578 706f  (r":camera: Expo
+00024e20: 7274 696e 6720 3344 2077 696e 646f 7720  rting 3D window 
+00024e30: 746f 2066 696c 6522 2c20 633d 2262 6c75  to file", c="blu
+00024e40: 6522 2c20 656e 643d 2222 290a 2020 2020  e", end="").    
+00024e50: 2020 2020 2020 2020 7665 646f 2e66 696c          vedo.fil
+00024e60: 655f 696f 2e65 7870 6f72 745f 7769 6e64  e_io.export_wind
+00024e70: 6f77 2822 7363 656e 652e 6e70 7a22 290a  ow("scene.npz").
+00024e80: 2020 2020 2020 2020 2020 2020 7665 646f              vedo
+00024e90: 2e70 7269 6e74 6328 222e 2054 7279 3a5c  .printc(". Try:\
+00024ea0: 6e3e 2076 6564 6f20 7363 656e 652e 6e70  n> vedo scene.np
+00024eb0: 7a22 2c20 633d 2262 6c75 6522 290a 0a20  z", c="blue").. 
+00024ec0: 2020 2020 2020 2065 6c69 6620 6b65 7920         elif key 
+00024ed0: 3d3d 2022 4622 3a0a 2020 2020 2020 2020  == "F":.        
+00024ee0: 2020 2020 7665 646f 2e66 696c 655f 696f      vedo.file_io
+00024ef0: 2e65 7870 6f72 745f 7769 6e64 6f77 2822  .export_window("
+00024f00: 7363 656e 652e 7833 6422 290a 2020 2020  scene.x3d").    
+00024f10: 2020 2020 2020 2020 7665 646f 2e70 7269          vedo.pri
+00024f20: 6e74 6328 223a 6964 6561 3a20 5472 793a  ntc(":idea: Try:
+00024f30: 2066 6972 6566 6f78 2073 6365 6e65 2e68   firefox scene.h
+00024f40: 746d 6c22 2c20 633d 2262 6c75 6522 290a  tml", c="blue").
+00024f50: 0a20 2020 2020 2020 2065 6c69 6620 6b65  .        elif ke
+00024f60: 7920 3d3d 2022 6922 3a20 2023 2070 7269  y == "i":  # pri
+00024f70: 6e74 2069 6e66 6f0a 2020 2020 2020 2020  nt info.        
+00024f80: 2020 2020 6966 2073 656c 662e 636c 6963      if self.clic
+00024f90: 6b65 645f 6163 746f 723a 0a20 2020 2020  ked_actor:.     
+00024fa0: 2020 2020 2020 2020 2020 2075 7469 6c73             utils
+00024fb0: 2e70 7269 6e74 5f69 6e66 6f28 7365 6c66  .print_info(self
+00024fc0: 2e63 6c69 636b 6564 5f61 6374 6f72 290a  .clicked_actor).
+00024fd0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00024fe0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00024ff0: 2020 7574 696c 732e 7072 696e 745f 696e    utils.print_in
+00025000: 666f 2873 656c 6629 0a0a 2020 2020 2020  fo(self)..      
+00025010: 2020 656c 6966 206b 6579 203d 3d20 2249    elif key == "I
+00025020: 223a 2020 2320 7072 696e 7420 636f 6c6f  ":  # print colo
+00025030: 7220 756e 6465 7220 7468 6520 6d6f 7573  r under the mous
+00025040: 650a 2020 2020 2020 2020 2020 2020 782c  e.            x,
+00025050: 2079 203d 2069 7265 6e2e 4765 7445 7665   y = iren.GetEve
+00025060: 6e74 506f 7369 7469 6f6e 2829 0a20 2020  ntPosition().   
+00025070: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+00025080: 6c6f 725f 7069 636b 6572 285b 782c 2079  lor_picker([x, y
+00025090: 5d2c 2076 6572 626f 7365 3d54 7275 6529  ], verbose=True)
+000250a0: 0a0a 2020 2020 2020 2020 656c 6966 206b  ..        elif k
+000250b0: 6579 203d 3d20 2279 223a 0a20 2020 2020  ey == "y":.     
+000250c0: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
+000250d0: 6c69 636b 6564 5f61 6374 6f72 2061 6e64  licked_actor and
+000250e0: 2073 656c 662e 636c 6963 6b65 645f 6163   self.clicked_ac
+000250f0: 746f 722e 7069 7065 6c69 6e65 3a0a 2020  tor.pipeline:.  
+00025100: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00025110: 7365 6c66 2e63 6c69 636b 6564 5f61 6374  self.clicked_act
+00025120: 6f72 2e70 6970 656c 696e 6520 3d20 2075  or.pipeline =  u
+00025130: 7469 6c73 2e4f 7065 7261 7469 6f6e 4e6f  tils.OperationNo
+00025140: 6465 280a 2020 2020 2020 2020 2020 2020  de(.            
+00025150: 2020 2020 2320 2020 2020 2020 2020 2273      #         "s
+00025160: 686f 7722 2c20 7061 7265 6e74 733d 5b73  how", parents=[s
+00025170: 656c 662e 636c 6963 6b65 645f 6163 746f  elf.clicked_acto
+00025180: 725d 2c0a 2020 2020 2020 2020 2020 2020  r],.            
+00025190: 2020 2020 2320 2020 2020 2020 2020 7368      #         sh
+000251a0: 6170 653d 2263 6972 636c 6522 2c0a 2020  ape="circle",.  
+000251b0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+000251c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000251d0: 2020 7365 6c66 2e63 6c69 636b 6564 5f61    self.clicked_a
+000251e0: 6374 6f72 2e70 6970 656c 696e 652e 7368  ctor.pipeline.sh
+000251f0: 6f77 2829 0a0a 2020 2020 2020 2020 6966  ow()..        if
+00025200: 2069 7265 6e3a 0a20 2020 2020 2020 2020   iren:.         
+00025210: 2020 2069 7265 6e2e 5265 6e64 6572 2829     iren.Render()
+00025220: 0a                                       .
```

### Comparing `vedo-2023.4.5/vedo/pointcloud.py` & `vedo-2023.4.6/vedo/pointcloud.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/vedo/pyplot.py` & `vedo-2023.4.6/vedo/pyplot.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/vedo/settings.py` & `vedo-2023.4.6/vedo/settings.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/vedo/shapes.py` & `vedo-2023.4.6/vedo/shapes.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/vedo/tetmesh.py` & `vedo-2023.4.6/vedo/tetmesh.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/vedo/ugrid.py` & `vedo-2023.4.6/vedo/ugrid.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/vedo/utils.py` & `vedo-2023.4.6/vedo/utils.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/vedo/volume.py` & `vedo-2023.4.6/vedo/volume.py`

 * *Files 0% similar despite different names*

```diff
@@ -428,15 +428,15 @@
             voxels : (int, list)
                 number of voxels to be added (or a list of length 4)
             value : (int)
                 intensity value (gray-scale color) of the padding
         
         Example:
             ```python
-            from vedo import Volume, dataurl
+            from vedo import Volume, dataurl, show
             iso = Volume(dataurl+'embryo.tif').isosurface()
             vol = iso.binarize(spacing=(100, 100, 100)).pad(10)
             vol.dilate([15,15,15])
             show(iso, vol.isosurface(), N=2, axes=1)
             ```
             ![](https://vedo.embl.es/images/volumetric/volume_pad.png)
         """
```

### Comparing `vedo-2023.4.5/vedo/vtkclasses.py` & `vedo-2023.4.6/vedo/vtkclasses.py`

 * *Files identical despite different names*

### Comparing `vedo-2023.4.5/vedo.egg-info/PKG-INFO` & `vedo-2023.4.6/vedo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vedo
-Version: 2023.4.5
+Version: 2023.4.6
 Summary: A python module for scientific analysis and visualization of 3D objects and point clouds based on VTK.
 Home-page: https://github.com/marcomusy/vedo
 Author: Marco Musy
 Author-email: marco.musy@embl.es
 Maintainer: Marco Musy
 License: MIT
 Keywords: vtk 3D science analysis visualization mesh numpy
```

### Comparing `vedo-2023.4.5/vedo.egg-info/SOURCES.txt` & `vedo-2023.4.6/vedo.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -140,22 +140,24 @@
 examples/basic/spline_tool.py
 examples/basic/ssao.py
 examples/basic/surf_intersect.py
 examples/basic/texture_coords.py
 examples/basic/texturecubes.py
 examples/basic/tube_radii.py
 examples/basic/voronoi1.py
+examples/other/.polyscope.ini
 examples/other/__init__.py
 examples/other/clone2d.py
 examples/other/ellipt_fourier_desc.py
 examples/other/export_numpy.py
 examples/other/export_x3d.py
 examples/other/flag_labels1.py
 examples/other/flag_labels2.py
 examples/other/icon.py
+examples/other/imgui.ini
 examples/other/iminuit1.py
 examples/other/inset.py
 examples/other/make_video.py
 examples/other/meshio_read.py
 examples/other/morphomatics_regression.py
 examples/other/morphomatics_tube.py
 examples/other/napari1.py
@@ -172,15 +174,14 @@
 examples/other/qt_window3.py
 examples/other/remesh_ACVD.py
 examples/other/remesh_meshfix.py
 examples/other/remesh_tetgen.py
 examples/other/run_all.sh
 examples/other/scene.npz
 examples/other/spherical_harmonics1.py
-examples/other/spherical_harmonics2.py
 examples/other/tensor_grid1.py
 examples/other/tensor_grid2.py
 examples/other/trame_ex1.py
 examples/other/trame_ex2.py
 examples/other/trame_ex3.py
 examples/other/vpolyscope.py
 examples/other/wx_window1.py
@@ -374,16 +375,16 @@
 examples/volumetric/streamlines2.py
 examples/volumetric/streamlines3.py
 examples/volumetric/streamlines4.py
 examples/volumetric/streamribbons.py
 examples/volumetric/tensors.py
 examples/volumetric/tet_astyle.py
 examples/volumetric/tet_build.py
-examples/volumetric/tet_cutMesh1.py
-examples/volumetric/tet_cutMesh2.py
+examples/volumetric/tet_cut1.py
+examples/volumetric/tet_cut2.py
 examples/volumetric/tet_explode.py
 examples/volumetric/tet_isos_slice.py
 examples/volumetric/tet_threshold.py
 examples/volumetric/tetralize_surface.py
 examples/volumetric/ugrid1.py
 examples/volumetric/ugrid2.py
 examples/volumetric/vol2points.py
```

