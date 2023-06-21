# Comparing `tmp/acconeer-exptool-7.0.2.tar.gz` & `tmp/acconeer-exptool-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acconeer-exptool-7.0.2.tar", last modified: Thu Jun  1 13:03:48 2023, max compression
+gzip compressed data, was "acconeer-exptool-7.1.0.tar", last modified: Wed Jun 21 08:08:36 2023, max compression
```

## Comparing `acconeer-exptool-7.0.2.tar` & `acconeer-exptool-7.1.0.tar`

### file list

```diff
@@ -1,609 +1,621 @@
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.774839 acconeer-exptool-7.0.2/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       91 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/.gitattributes
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.722839 acconeer-exptool-7.0.2/.github/
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.730839 acconeer-exptool-7.0.2/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      877 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      368 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/.gitignore
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      158 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/.readthedocs.yaml
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14372 2023-06-01 12:49:58.000000 acconeer-exptool-7.0.2/CHANGELOG.md
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    13663 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/Jenkinsfile
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1881 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/LICENSE.md
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      217 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/MANIFEST.in
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8990 2023-06-01 13:03:48.774839 acconeer-exptool-7.0.2/PKG-INFO
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7948 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/README.md
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       73 2023-05-31 10:00:02.000000 acconeer-exptool-7.0.2/UNRELEASED_CHANGELOG.md
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.730839 acconeer-exptool-7.0.2/docker/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1865 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/docker/Dockerfile
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       82 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/docker/requirements-dev.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1604 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/dodo.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.726839 acconeer-exptool-7.0.2/examples/
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.730839 acconeer-exptool-7.0.2/examples/a111/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3247 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/examples/a111/basic.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1819 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/examples/a111/basic_continuous.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2657 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/examples/a111/load_record.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1273 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/examples/a111/load_record_h5.m
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.730839 acconeer-exptool-7.0.2/examples/a111/plotting/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1999 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/examples/a111/plotting/plot_with_matplotlib.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2551 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/examples/a111/plotting/plot_with_pyqtgraph.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.730839 acconeer-exptool-7.0.2/examples/a111/record_data/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1156 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/examples/a111/record_data/barebones.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2541 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/examples/a111/record_data/long_duration_split_files.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1958 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/examples/a111/record_data/with_cli.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.734839 acconeer-exptool-7.0.2/examples/a111/services/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2251 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/examples/a111/services/envelope.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3013 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/examples/a111/services/iq.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2277 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/examples/a111/services/power_bins.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2861 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/examples/a111/services/sparse.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.734839 acconeer-exptool-7.0.2/examples/a111/utils/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      802 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/examples/a111/utils/ping.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      805 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/examples/a111/utils/test_throughput.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.734839 acconeer-exptool-7.0.2/examples/a121/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1222 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/examples/a121/basic.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.734839 acconeer-exptool-7.0.2/examples/a121/bilateration/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8174 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/examples/a121/bilateration/bilaterator.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.734839 acconeer-exptool-7.0.2/examples/a121/breathing/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6340 2023-06-01 11:00:34.000000 acconeer-exptool-7.0.2/examples/a121/breathing/breathing.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.734839 acconeer-exptool-7.0.2/examples/a121/distance/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4522 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/examples/a121/distance/detector.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5053 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/examples/a121/distance/processor.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      776 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/examples/a121/extended_config.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1518 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/examples/a121/load_record.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1405 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/examples/a121/load_record_h5.m
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.734839 acconeer-exptool-7.0.2/examples/a121/phase_tracking/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5808 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/examples/a121/phase_tracking/phase_tracking.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4538 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/examples/a121/plot.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.734839 acconeer-exptool-7.0.2/examples/a121/presence/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11241 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/examples/a121/presence/detector.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11026 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/examples/a121/presence/processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.734839 acconeer-exptool-7.0.2/examples/a121/record_data/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      975 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/examples/a121/record_data/barebones.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1017 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/examples/a121/record_data/with_cli.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1140 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/examples/a121/reuse_calibration.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.734839 acconeer-exptool-7.0.2/examples/a121/smart_presence/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    10430 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/examples/a121/smart_presence/processor.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     9497 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/examples/a121/smart_presence/ref_app.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4253 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/examples/a121/stress.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      946 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/examples/a121/subsweeps.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.734839 acconeer-exptool-7.0.2/examples/a121/surface_velocity/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8515 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/examples/a121/surface_velocity/example_app.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8864 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/examples/a121/surface_velocity/processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.734839 acconeer-exptool-7.0.2/examples/a121/touchless_button/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3927 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/examples/a121/touchless_button/processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.734839 acconeer-exptool-7.0.2/examples/a121/vibration/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4410 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/examples/a121/vibration/vibration.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.734839 acconeer-exptool-7.0.2/gui/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1254 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/gui/main.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7005 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/noxfile.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.734839 acconeer-exptool-7.0.2/portable/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       27 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/portable/.gitignore
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1571 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/portable/make.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.734839 acconeer-exptool-7.0.2/portable/package/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      108 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/portable/package/cmd_with_path.bat
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      346 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/portable/package/run_app.bat
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.734839 acconeer-exptool-7.0.2/portable/package/tools/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      989 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/portable/package/tools/update.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      168 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/portable/package/update.bat
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2515 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/pyproject.toml
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2433 2023-06-01 13:03:48.774839 acconeer-exptool-7.0.2/setup.cfg
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.730839 acconeer-exptool-7.0.2/src/
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.726839 acconeer-exptool-7.0.2/src/acconeer/
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.734839 acconeer-exptool-7.0.2/src/acconeer/exptool/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      295 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3212 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/_bs_thread.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.734839 acconeer-exptool-7.0.2/src/acconeer/exptool/_pyusb/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      100 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/_pyusb/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5890 2023-01-24 10:54:24.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/_pyusb/pyusbcomm.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.734839 acconeer-exptool-7.0.2/src/acconeer/exptool/_structs/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/_structs/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15542 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/_structs/configbase.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15673 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/_structs/qtpidgets.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.734839 acconeer-exptool-7.0.2/src/acconeer/exptool/_tests/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/_tests/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4259 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/_tests/test_rig.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       22 2023-06-01 13:03:48.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/_version.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.738839 acconeer-exptool-7.0.2/src/acconeer/exptool/_winusbcdc/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1071 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/_winusbcdc/LICENSE
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      190 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/_winusbcdc/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2847 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/_winusbcdc/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6837 2023-01-24 14:05:20.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/_winusbcdc/usb_cdc.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2021 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/_winusbcdc/winusb.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3466 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/_winusbcdc/winusbclasses.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      231 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/_winusbcdc/winusberror.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10029 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/_winusbcdc/winusbpy.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12307 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/_winusbcdc/winusbutils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.738839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      438 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/__init__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.738839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      119 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7940 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/base.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5916 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/client.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5513 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/client_factory.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      517 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/common.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.738839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/json/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/json/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18330 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/json/client.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14209 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/links.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.738839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/mock/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/mock/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7621 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/mock/client.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1496 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/multiwrap.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.738839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/reg/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/reg/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    24884 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/reg/client.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.738839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/reg/data/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/reg/data/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8068 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/reg/data/regmap.yaml
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6351 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/reg/protocol.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     9853 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/reg/regmap.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7176 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_conf_to_rss_sdk.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    28007 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_configs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      587 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_modes.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3710 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.738839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      242 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/__init__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.738839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/_base/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2708 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/_base/calibration.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      860 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/_base/module_info.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1695 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/_standalone_main.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.738839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/breathing/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/breathing/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/breathing/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      538 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/breathing/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7469 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/breathing/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4554 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/breathing/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.738839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/button_press/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/button_press/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/button_press/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      618 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/button_press/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6054 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/button_press/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       79 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/button_press/constants.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5308 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/button_press/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.742839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/button_press_sparse/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/button_press_sparse/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/button_press_sparse/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      552 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/button_press_sparse/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11319 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/button_press_sparse/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       79 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/button_press_sparse/constants.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4931 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/button_press_sparse/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.742839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/distance_detector/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/distance_detector/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/distance_detector/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      948 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/distance_detector/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    21416 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/distance_detector/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2204 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/distance_detector/calibration.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6126 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/distance_detector/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.742839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/envelope/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/envelope/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/envelope/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      862 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/envelope/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3943 2022-12-29 10:02:50.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/envelope/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1517 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/envelope/calibration.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5280 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/envelope/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.742839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/iq/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/iq/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/iq/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      565 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/iq/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1985 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/iq/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3928 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/iq/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.742839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/obstacle_detection/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/obstacle_detection/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/obstacle_detection/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      939 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/obstacle_detection/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    27784 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/obstacle_detection/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9166 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/obstacle_detection/calibration.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      104 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/obstacle_detection/constants.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    16847 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/obstacle_detection/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.742839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/parking/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/parking/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/parking/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      890 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/parking/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9162 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/parking/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8503 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/parking/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.742839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/phase_tracking/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      110 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/phase_tracking/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/phase_tracking/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      576 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/phase_tracking/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2599 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/phase_tracking/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4172 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/phase_tracking/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.742839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/power_bins/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       99 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/power_bins/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/power_bins/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      612 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/power_bins/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      175 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/power_bins/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1400 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/power_bins/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.742839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/presence_detect_human_only/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2023-02-23 12:52:28.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/presence_detect_human_only/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2023-02-23 12:52:28.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/presence_detect_human_only/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      577 2023-02-23 12:52:28.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/presence_detect_human_only/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15250 2023-02-23 12:52:28.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/presence_detect_human_only/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    13885 2023-02-23 12:52:28.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/presence_detect_human_only/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.746839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/presence_detection_sparse/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/presence_detection_sparse/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/presence_detection_sparse/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      917 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/presence_detection_sparse/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14079 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/presence_detection_sparse/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10519 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/presence_detection_sparse/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.746839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sleep_breathing/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sleep_breathing/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sleep_breathing/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      615 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sleep_breathing/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10381 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sleep_breathing/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4623 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sleep_breathing/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.746839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      577 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2880 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5079 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.746839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse_fft/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse_fft/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse_fft/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      552 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse_fft/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1341 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse_fft/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4454 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse_fft/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.746839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse_inter_fft/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse_inter_fft/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse_inter_fft/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      557 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse_inter_fft/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5185 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse_inter_fft/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5472 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse_inter_fft/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.746839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/speed_sparse/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/speed_sparse/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/speed_sparse/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      824 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/speed_sparse/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12380 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/speed_sparse/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      186 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/speed_sparse/constants.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7812 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/speed_sparse/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.746839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/tank_level_short/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/tank_level_short/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/tank_level_short/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      840 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/tank_level_short/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10409 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/tank_level_short/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1517 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/tank_level_short/calibration.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3125 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/tank_level_short/ui.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2560 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.746839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/wave_to_exit/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/wave_to_exit/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/wave_to_exit/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      545 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/wave_to_exit/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4662 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/wave_to_exit/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6099 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/wave_to_exit/ui.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9009 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/recording.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.746839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1136 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1790 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_cli.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.746839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      989 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/__init__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.750839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      690 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/__init__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.750839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/configs/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      329 2023-02-08 08:58:10.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/configs/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4195 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/configs/config_enums.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    22033 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/configs/sensor_config.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    10267 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/configs/session_config.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11137 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/configs/subsweep_config.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1035 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/configs/validation_error.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.750839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/containers/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      607 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/containers/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8821 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/containers/client_info.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4798 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/containers/metadata.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8216 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/containers/record.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2192 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/containers/result.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1351 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/containers/sensor_calibration.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2906 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/containers/server_info.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      187 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/containers/server_log_message.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2189 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/containers/stacked_results.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1675 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/containers/utils.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      144 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/dtypes.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.750839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/mediators/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      150 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/mediators/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      931 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/mediators/link.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1265 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/mediators/recorder.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.750839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      401 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/__init__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.750839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      439 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7119 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/client.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5053 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/common_client.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1324 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/communication_protocol.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    15568 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_client.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.750839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      403 2023-02-13 09:23:57.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1023 2023-02-13 09:23:57.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_factory.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6512 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_latest.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      985 2023-02-13 09:23:57.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_15_6_mhz.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1037 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_5_2_mhz.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      840 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_calibration_reuse.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.750839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      521 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      687 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/erroneus_message.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1150 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/log_message.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       96 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/parse_error.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4314 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/result_message.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1123 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/sensor_info_response.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      752 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/set_baudrate_response.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2836 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/setup_response.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1045 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/streaming_responses.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      791 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/system_info_response.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       97 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/server_error.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1998 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/links.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      643 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/message.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11369 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/mock_client.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3996 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.754839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/h5_record/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      276 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/h5_record/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8225 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/h5_record/record.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3012 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/h5_record/record_io.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    12719 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/h5_record/recorder.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1526 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/h5_record/session_schema.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      928 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/h5_record/utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.754839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/im_record/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       95 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/im_record/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3543 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/im_record/im_record.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18035 2023-04-28 09:00:18.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.754839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core_ext/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      118 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core_ext/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4868 2023-05-31 21:00:21.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core_ext/_replaying_client.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      318 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_h5_utils.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4840 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_perf_calc.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2516 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_rate_calc.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.754839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      681 2023-06-01 09:17:45.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4086 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/_base.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.754839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/_plugins/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      367 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/_plugins/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7933 2023-06-01 12:45:39.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/_plugins/_a121.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      434 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/_plugins/_detector.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      617 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/_plugins/_null_app_model.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3783 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/_plugins/_processor_main.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.754839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/_plugins/processor/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      446 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/_plugins/processor/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8320 2023-06-01 12:00:03.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/_plugins/processor/backend_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1388 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/_plugins/processor/plot_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1276 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/_plugins/processor/plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6579 2023-06-01 12:00:03.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/_plugins/processor/view_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10386 2023-06-01 11:00:34.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/_utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.754839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/bilateration/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      175 2023-02-06 10:51:29.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/bilateration/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      395 2023-03-28 07:00:16.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/bilateration/_configs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    24946 2023-06-01 12:00:03.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/bilateration/_plugin.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    17474 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/bilateration/_processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.754839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/breathing/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      192 2023-06-01 11:00:34.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/breathing/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      376 2023-06-01 11:00:34.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/breathing/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8723 2023-06-01 11:00:34.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/breathing/_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7401 2023-06-01 11:00:34.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/breathing/_processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.754839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/distance/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      507 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/distance/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      855 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/distance/__main__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5471 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/distance/_aggregator.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      307 2023-03-28 07:00:16.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/distance/_configs.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    59448 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/distance/_detector.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    24079 2023-06-01 12:00:03.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/distance/_detector_plugin.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    30450 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/distance/_processors.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    15812 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/distance/_serializers.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.754839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/phase_tracking/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      187 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/phase_tracking/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      376 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/phase_tracking/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7575 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/phase_tracking/_plugin.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7141 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/phase_tracking/_processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.758839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/presence/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      213 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/presence/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2175 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/presence/_configs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    13856 2023-06-01 11:00:34.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/presence/_detector.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    25707 2023-06-01 12:48:59.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/presence/_detector_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18288 2023-04-28 09:00:18.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/presence/_processors.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4717 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/presence/_serializers.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.758839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/smart_presence/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      182 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/smart_presence/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2223 2023-05-31 10:00:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/smart_presence/_configs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6607 2023-04-03 13:53:22.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/smart_presence/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7165 2023-05-31 10:00:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/smart_presence/_ref_app.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    21729 2023-06-01 12:48:59.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/smart_presence/_ref_app_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6835 2023-05-31 10:00:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/smart_presence/_serializer.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.758839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/sparse_iq/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      220 2023-02-06 16:11:19.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/sparse_iq/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      376 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/sparse_iq/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8167 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/sparse_iq/_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3116 2023-02-06 16:11:19.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/sparse_iq/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7245 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/sparse_iq/_serializers.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.758839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/surface_velocity/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      130 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/surface_velocity/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11611 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/surface_velocity/_example_app.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    21732 2023-06-01 12:00:03.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/surface_velocity/_example_app_plugin.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    14090 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/surface_velocity/_processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.758839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/tank_level/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      219 2023-04-03 13:53:22.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/tank_level/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1658 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/tank_level/_configs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    27152 2023-06-01 12:00:03.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/tank_level/_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7290 2023-04-03 13:53:22.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/tank_level/_processor.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     6265 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/tank_level/_ref_app.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4229 2023-04-03 13:53:22.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/tank_level/_serializer.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.758839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/touchless_button/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      306 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/touchless_button/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      486 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/touchless_button/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1100 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/touchless_button/_blinkstick_updater.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1738 2023-01-24 14:05:20.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/touchless_button/_configs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7687 2023-03-31 08:16:11.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/touchless_button/_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14754 2023-06-01 09:17:45.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/touchless_button/_processor.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2896 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/touchless_button/_serializers.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.758839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/vibration/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      187 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/vibration/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      376 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/vibration/__main__,py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8514 2023-04-28 09:00:18.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/vibration/_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7628 2023-06-01 09:17:45.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/vibration/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/py.typed
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.758839 acconeer-exptool-7.0.2/src/acconeer/exptool/app/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      333 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/__main__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4475 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/launcher.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.758839 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      959 2023-06-01 12:00:03.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      116 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      994 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/_argument_parser.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1718 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/_enums.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      102 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/_exceptions.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      983 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/_version_checker.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2698 2022-12-29 10:02:50.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/app.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.762839 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/app_model/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      239 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/app_model/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    27076 2023-06-01 12:00:03.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/app_model/app_model.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1404 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/app_model/app_model_listener.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      981 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/app_model/file_detective.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      428 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/app_model/plugin_protocols.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2074 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/app_model/port_updater.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.762839 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/backend/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      478 2023-06-01 12:00:03.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/backend/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2737 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/backend/_application_client.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4985 2023-06-01 12:00:03.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/backend/_backend.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1610 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/backend/_backend_logger.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2040 2023-06-01 12:00:03.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/backend/_backend_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1559 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/backend/_message.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4770 2023-06-01 12:00:03.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/backend/_model.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2786 2023-06-01 12:00:03.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/backend/_tasks.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1558 2023-06-01 11:00:34.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/plugin_loader.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.762839 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/pluginbase/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      241 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/pluginbase/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      973 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/pluginbase/plot_plugin_base.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      431 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/pluginbase/plugin_preset_base.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1404 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/pluginbase/plugin_spec_base.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1024 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/pluginbase/ui_plugin_base.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1836 2023-06-01 12:00:03.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/pluginbase/view_plugin_base.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/py.typed
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      470 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/qt_subclasses.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      804 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/storage.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.762839 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      495 2023-06-01 12:00:03.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2141 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/app_model_viewer.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2641 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/device_comboboxes.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.762839 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/flash_tab/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       94 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/flash_tab/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    14023 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/flash_tab/dialogs.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4635 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/flash_tab/threads.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15274 2023-06-01 12:00:03.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/flash_tab/widgets.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1802 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/help_tab.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2052 2023-06-01 12:00:03.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/icons.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3600 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/main_window.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1968 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/misc.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.762839 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      783 2023-06-01 12:00:03.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6615 2023-06-01 12:00:03.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/attrs_config_editor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1290 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/collapsible_widget.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1026 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/data_editor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6166 2023-06-01 12:00:03.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/metadata_view.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1432 2023-03-27 09:23:51.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/misc_error_view.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3557 2023-06-01 12:00:03.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/perf_calc_view.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.766839 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      769 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      499 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/common.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3814 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/hooks.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2082 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidget_groups.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    25494 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidgets.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2004 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/range_help_view.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12975 2023-06-01 12:00:03.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/sensor_config_editor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6474 2023-06-01 12:00:03.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/session_config_editor.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7963 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/subsweep_config_editor.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1887 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/two_sensor_ids_editor.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      294 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/types.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      865 2023-06-01 12:00:03.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/utils.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     9480 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/status_bar.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.766839 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/stream_tab/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       98 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/stream_tab/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    10441 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/stream_tab/connection_widget.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5853 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/stream_tab/hints.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12245 2023-06-01 12:00:03.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/stream_tab/plugin_widget.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4551 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/stream_tab/recording_widget.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2636 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/stream_tab/widgets.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1382 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.766839 acconeer-exptool-7.0.2/src/acconeer/exptool/app/old/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       79 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/old/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      116 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/old/__main__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    84006 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/old/app.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4735 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/old/data_processing.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.766839 acconeer-exptool-7.0.2/src/acconeer/exptool/app/old/elements/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/old/elements/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8476 2022-12-29 10:02:50.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/old/elements/helper.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2346 2023-02-23 12:52:28.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/old/elements/modules.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    10745 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/old/elements/qt_subclasses.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.766839 acconeer-exptool-7.0.2/src/acconeer/exptool/app/resources/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/resources/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    90184 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/resources/a111_gui.png
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    57036 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/resources/a121_gui.png
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4162 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/resources/icon-black.svg
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    35706 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/resources/icon.png
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3208 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/resources/loader.gif
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.730839 acconeer-exptool-7.0.2/src/acconeer/exptool/data/
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.766839 acconeer-exptool-7.0.2/src/acconeer/exptool/data/libft4222/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1245 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/data/libft4222/LICENSE.txt
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.766839 acconeer-exptool-7.0.2/src/acconeer/exptool/data/libft4222/aarch64/
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   513305 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/data/libft4222/aarch64/libft4222.so.1.4.4.44
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.766839 acconeer-exptool-7.0.2/src/acconeer/exptool/data/libft4222/amd64/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   209008 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/data/libft4222/amd64/LibFT4222.dll
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   314552 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/data/libft4222/amd64/ftd2xx.dll
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.766839 acconeer-exptool-7.0.2/src/acconeer/exptool/data/libft4222/armv6/
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   484176 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/data/libft4222/armv6/libft4222.so.1.4.4.44
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.766839 acconeer-exptool-7.0.2/src/acconeer/exptool/data/libft4222/armv7/
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   399731 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/data/libft4222/armv7/libft4222.so.1.4.4.44
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.770839 acconeer-exptool-7.0.2/src/acconeer/exptool/data/libft4222/i386/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   160256 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/data/libft4222/i386/LibFT4222.dll
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   271672 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/data/libft4222/i386/ftd2xx.dll
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.770839 acconeer-exptool-7.0.2/src/acconeer/exptool/data/libft4222/x86_64/
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   504389 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/data/libft4222/x86_64/libft4222.so.1.4.4.44
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.770839 acconeer-exptool-7.0.2/src/acconeer/exptool/flash/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      338 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/flash/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      115 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/flash/__main__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5844 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/flash/_bin_fetcher.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3625 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/flash/_dev_license.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4284 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/flash/_dev_license_tui.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      416 2023-04-03 13:53:22.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/flash/_device_flasher_base.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    12868 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/flash/_flasher.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      828 2023-01-24 14:05:20.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/flash/_products.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.770839 acconeer-exptool-7.0.2/src/acconeer/exptool/flash/_stm32uart/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      150 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/flash/_stm32uart/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      274 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/flash/_stm32uart/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6665 2023-04-03 13:53:22.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/flash/_stm32uart/_stm32flasher.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.770839 acconeer-exptool-7.0.2/src/acconeer/exptool/flash/_xc120/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      258 2023-01-24 14:05:20.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/flash/_xc120/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9147 2023-01-24 14:05:20.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/flash/_xc120/_bootloader_comm.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     9417 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/flash/_xc120/_bootloader_tool.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      224 2023-01-24 14:05:20.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/flash/_xc120/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11051 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/libft4222.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3338 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/mpl_process.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3185 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/pg_process.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.770839 acconeer-exptool-7.0.2/src/acconeer/exptool/setup/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/setup/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1191 2022-12-22 15:03:13.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/setup/__main__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.770839 acconeer-exptool-7.0.2/src/acconeer/exptool/setup/base/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      244 2022-12-22 15:03:13.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/setup/base/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1431 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/setup/base/platform_install.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      980 2022-12-22 15:03:13.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/setup/base/prompts.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      690 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/setup/base/setup_group.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2880 2022-12-22 15:03:13.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/setup/base/setup_step.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      520 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/setup/base/utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.770839 acconeer-exptool-7.0.2/src/acconeer/exptool/setup/cli/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      106 2022-12-22 15:03:13.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/setup/cli/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      684 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/setup/cli/argument_parser.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.770839 acconeer-exptool-7.0.2/src/acconeer/exptool/setup/platforms/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       91 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/setup/platforms/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      329 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/setup/platforms/how_to.txt
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1867 2022-12-22 15:03:13.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/setup/platforms/linux.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1191 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/setup/platforms/ubuntu_20_04.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/setup/py.typed
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    21469 2023-04-03 13:53:22.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.770839 acconeer-exptool-7.0.2/src/acconeer_exptool.egg-info/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8990 2023-06-01 13:03:48.000000 acconeer-exptool-7.0.2/src/acconeer_exptool.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    25530 2023-06-01 13:03:48.000000 acconeer-exptool-7.0.2/src/acconeer_exptool.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-06-01 13:03:48.000000 acconeer-exptool-7.0.2/src/acconeer_exptool.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-06-01 13:03:48.000000 acconeer-exptool-7.0.2/src/acconeer_exptool.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      475 2023-06-01 13:03:48.000000 acconeer-exptool-7.0.2/src/acconeer_exptool.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        9 2023-06-01 13:03:48.000000 acconeer-exptool-7.0.2/src/acconeer_exptool.egg-info/top_level.txt
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.774839 acconeer-exptool-7.0.2/tools/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3943 2023-06-01 09:17:45.000000 acconeer-exptool-7.0.2/tools/check_changelog.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12005 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/tools/check_copyright.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1388 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/tools/check_line_length.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1495 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/tools/check_permissions.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4237 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/tools/check_sdk_mentions.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1801 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/tools/check_whitespace.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2064 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/tools/update_regmap.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.774839 acconeer-exptool-7.0.2/utils/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14756 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/utils/convert_to_csv.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.701143 acconeer-exptool-7.1.0/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       91 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/.gitattributes
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.633143 acconeer-exptool-7.1.0/.github/
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.641143 acconeer-exptool-7.1.0/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      877 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      368 2023-03-03 12:25:40.000000 acconeer-exptool-7.1.0/.gitignore
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      158 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/.readthedocs.yaml
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14786 2023-06-21 08:08:21.000000 acconeer-exptool-7.1.0/CHANGELOG.md
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    13663 2023-04-03 10:32:44.000000 acconeer-exptool-7.1.0/Jenkinsfile
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1881 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/LICENSE.md
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      217 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/MANIFEST.in
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8990 2023-06-21 08:08:36.701143 acconeer-exptool-7.1.0/PKG-INFO
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7948 2023-04-04 08:04:50.000000 acconeer-exptool-7.1.0/README.md
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       86 2023-06-21 08:08:21.000000 acconeer-exptool-7.1.0/UNRELEASED_CHANGELOG.md
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.641143 acconeer-exptool-7.1.0/docker/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1865 2023-03-03 13:14:28.000000 acconeer-exptool-7.1.0/docker/Dockerfile
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       82 2023-03-03 12:25:40.000000 acconeer-exptool-7.1.0/docker/requirements-dev.txt
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1604 2023-03-27 08:58:09.000000 acconeer-exptool-7.1.0/dodo.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.633143 acconeer-exptool-7.1.0/examples/
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.641143 acconeer-exptool-7.1.0/examples/a111/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3247 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/examples/a111/basic.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1819 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/examples/a111/basic_continuous.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2657 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/examples/a111/load_record.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1273 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/examples/a111/load_record_h5.m
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.641143 acconeer-exptool-7.1.0/examples/a111/plotting/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1999 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/examples/a111/plotting/plot_with_matplotlib.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2551 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/examples/a111/plotting/plot_with_pyqtgraph.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.641143 acconeer-exptool-7.1.0/examples/a111/record_data/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1156 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/examples/a111/record_data/barebones.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2541 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/examples/a111/record_data/long_duration_split_files.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1958 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/examples/a111/record_data/with_cli.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.641143 acconeer-exptool-7.1.0/examples/a111/services/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2251 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/examples/a111/services/envelope.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3013 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/examples/a111/services/iq.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2277 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/examples/a111/services/power_bins.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2861 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/examples/a111/services/sparse.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.641143 acconeer-exptool-7.1.0/examples/a111/utils/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      802 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/examples/a111/utils/ping.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      805 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/examples/a111/utils/test_throughput.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.645143 acconeer-exptool-7.1.0/examples/a121/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1222 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/examples/a121/basic.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.645143 acconeer-exptool-7.1.0/examples/a121/bilateration/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8174 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/examples/a121/bilateration/bilaterator.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.645143 acconeer-exptool-7.1.0/examples/a121/distance/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4522 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/examples/a121/distance/detector.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5053 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/examples/a121/distance/processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      776 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/examples/a121/extended_config.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1518 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/examples/a121/load_record.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1405 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/examples/a121/load_record_h5.m
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.645143 acconeer-exptool-7.1.0/examples/a121/phase_tracking/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5808 2023-04-11 13:56:57.000000 acconeer-exptool-7.1.0/examples/a121/phase_tracking/phase_tracking.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4538 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/examples/a121/plot.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.645143 acconeer-exptool-7.1.0/examples/a121/presence/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11241 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/examples/a121/presence/detector.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11026 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/examples/a121/presence/processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.645143 acconeer-exptool-7.1.0/examples/a121/record_data/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      975 2023-05-15 07:29:55.000000 acconeer-exptool-7.1.0/examples/a121/record_data/barebones.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1017 2023-05-15 07:29:55.000000 acconeer-exptool-7.1.0/examples/a121/record_data/with_cli.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1140 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/examples/a121/reuse_calibration.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.645143 acconeer-exptool-7.1.0/examples/a121/smart_presence/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10430 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/examples/a121/smart_presence/processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9497 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/examples/a121/smart_presence/ref_app.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4253 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/examples/a121/stress.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      946 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/examples/a121/subsweeps.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.645143 acconeer-exptool-7.1.0/examples/a121/surface_velocity/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8515 2023-04-17 09:00:31.000000 acconeer-exptool-7.1.0/examples/a121/surface_velocity/example_app.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8864 2023-04-17 09:00:31.000000 acconeer-exptool-7.1.0/examples/a121/surface_velocity/processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.645143 acconeer-exptool-7.1.0/examples/a121/touchless_button/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3927 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/examples/a121/touchless_button/processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.645143 acconeer-exptool-7.1.0/examples/a121/vibration/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4410 2023-04-28 14:58:15.000000 acconeer-exptool-7.1.0/examples/a121/vibration/vibration.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.645143 acconeer-exptool-7.1.0/gui/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1254 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/gui/main.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6585 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/noxfile.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.645143 acconeer-exptool-7.1.0/portable/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       27 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/portable/.gitignore
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1571 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/portable/make.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.645143 acconeer-exptool-7.1.0/portable/package/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      108 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/portable/package/cmd_with_path.bat
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      346 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/portable/package/run_app.bat
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.649143 acconeer-exptool-7.1.0/portable/package/tools/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      989 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/portable/package/tools/update.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      168 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/portable/package/update.bat
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2361 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/pyproject.toml
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2433 2023-06-21 08:08:36.705143 acconeer-exptool-7.1.0/setup.cfg
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.637143 acconeer-exptool-7.1.0/src/
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.633143 acconeer-exptool-7.1.0/src/acconeer/
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.649143 acconeer-exptool-7.1.0/src/acconeer/exptool/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      295 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3212 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/_bs_thread.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.649143 acconeer-exptool-7.1.0/src/acconeer/exptool/_pyusb/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      100 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/_pyusb/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5890 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/_pyusb/pyusbcomm.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.649143 acconeer-exptool-7.1.0/src/acconeer/exptool/_structs/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/_structs/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15542 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/_structs/configbase.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15673 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/_structs/qtpidgets.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.649143 acconeer-exptool-7.1.0/src/acconeer/exptool/_tests/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/_tests/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4259 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/_tests/test_rig.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       22 2023-06-21 08:08:36.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/_version.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.649143 acconeer-exptool-7.1.0/src/acconeer/exptool/_winusbcdc/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1071 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/_winusbcdc/LICENSE
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      190 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/_winusbcdc/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2847 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/_winusbcdc/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6837 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/_winusbcdc/usb_cdc.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2021 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/_winusbcdc/winusb.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3466 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/_winusbcdc/winusbclasses.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      231 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/_winusbcdc/winusberror.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10029 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/_winusbcdc/winusbpy.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12307 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/_winusbcdc/winusbutils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.649143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      438 2023-04-03 10:32:44.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/__init__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.653143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      119 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7940 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/base.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5916 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5513 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/client_factory.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      517 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/common.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.653143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/json/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/json/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18330 2023-03-03 12:25:40.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/json/client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14209 2023-03-03 12:25:40.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/links.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.653143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/mock/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/mock/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7621 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/mock/client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1496 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/multiwrap.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.653143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/reg/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/reg/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    24884 2023-05-12 09:53:24.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/reg/client.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.653143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/reg/data/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/reg/data/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8068 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/reg/data/regmap.yaml
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6351 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/reg/protocol.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9853 2023-04-03 10:32:44.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/reg/regmap.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7176 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_conf_to_rss_sdk.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    28007 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      587 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_modes.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3710 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.653143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      242 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/__init__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.653143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/_base/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2708 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/_base/calibration.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      860 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/_base/module_info.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1695 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/_standalone_main.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.653143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/breathing/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/breathing/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/breathing/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      538 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/breathing/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7469 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/breathing/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4554 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/breathing/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.653143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/button_press/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/button_press/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/button_press/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      618 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/button_press/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6054 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/button_press/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       79 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/button_press/constants.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5308 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/button_press/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.657143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/button_press_sparse/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/button_press_sparse/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/button_press_sparse/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      552 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/button_press_sparse/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11319 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/button_press_sparse/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       79 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/button_press_sparse/constants.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4931 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/button_press_sparse/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.657143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/distance_detector/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/distance_detector/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/distance_detector/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      948 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/distance_detector/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    21416 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/distance_detector/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2204 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/distance_detector/calibration.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6126 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/distance_detector/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.657143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/envelope/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/envelope/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/envelope/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      862 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/envelope/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3943 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/envelope/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1517 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/envelope/calibration.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5280 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/envelope/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.657143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/iq/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/iq/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/iq/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      565 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/iq/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1985 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/iq/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3928 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/iq/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.657143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/obstacle_detection/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/obstacle_detection/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/obstacle_detection/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      939 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/obstacle_detection/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    27784 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/obstacle_detection/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9166 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/obstacle_detection/calibration.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      104 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/obstacle_detection/constants.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    16847 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/obstacle_detection/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.661143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/parking/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/parking/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/parking/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      890 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/parking/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9162 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/parking/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8503 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/parking/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.661143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/phase_tracking/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      110 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/phase_tracking/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/phase_tracking/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      576 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/phase_tracking/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2599 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/phase_tracking/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4172 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/phase_tracking/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.661143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/power_bins/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       99 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/power_bins/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/power_bins/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      612 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/power_bins/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      175 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/power_bins/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1400 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/power_bins/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.661143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      577 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15250 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    13885 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.661143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      917 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14079 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10519 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.661143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sleep_breathing/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sleep_breathing/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sleep_breathing/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      615 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sleep_breathing/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10381 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sleep_breathing/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4623 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sleep_breathing/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.665143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      577 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2880 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5079 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.665143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse_fft/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse_fft/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse_fft/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      552 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse_fft/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1341 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse_fft/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4454 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse_fft/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.665143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      557 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5185 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5472 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.665143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/speed_sparse/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/speed_sparse/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/speed_sparse/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      824 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/speed_sparse/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12380 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/speed_sparse/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      186 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/speed_sparse/constants.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7812 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/speed_sparse/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.665143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/tank_level_short/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/tank_level_short/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/tank_level_short/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      840 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/tank_level_short/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10409 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/tank_level_short/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1517 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/tank_level_short/calibration.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3125 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/tank_level_short/ui.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2560 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.669143 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/wave_to_exit/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/wave_to_exit/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/wave_to_exit/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      545 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/wave_to_exit/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4662 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/wave_to_exit/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6099 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/wave_to_exit/ui.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9009 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a111/recording.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.669143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1207 2023-06-09 13:10:48.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1790 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_cli.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.669143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      989 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/__init__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.669143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      690 2023-05-15 07:29:55.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/__init__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.669143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/configs/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      329 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/configs/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4195 2023-03-29 12:24:17.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/configs/config_enums.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    22075 2023-06-20 07:07:07.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/configs/sensor_config.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10223 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/configs/session_config.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11207 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/configs/subsweep_config.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1035 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/configs/validation_error.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.669143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/containers/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      607 2023-05-15 07:29:55.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/containers/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8821 2023-04-17 09:35:06.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/containers/client_info.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4798 2023-03-06 09:22:45.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/containers/metadata.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8216 2023-05-15 07:29:55.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/containers/record.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2192 2023-03-06 09:22:45.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/containers/result.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1351 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/containers/sensor_calibration.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2906 2023-03-06 09:22:45.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/containers/server_info.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      187 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/containers/server_log_message.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2189 2023-03-06 09:22:45.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/containers/stacked_results.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1675 2023-03-06 09:22:45.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/containers/utils.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      144 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/dtypes.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.669143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/mediators/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      150 2023-05-15 07:29:55.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/mediators/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      931 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/mediators/link.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1265 2023-05-15 11:16:12.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/mediators/recorder.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.669143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      401 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/__init__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.669143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      439 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7119 2023-05-15 11:16:12.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5053 2023-05-15 11:16:12.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/common_client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1324 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/communication_protocol.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15568 2023-05-15 07:29:55.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_client.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.673143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      403 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1023 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_factory.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6512 2023-03-06 09:22:45.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_latest.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      985 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_15_6_mhz.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1037 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_5_2_mhz.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      840 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_calibration_reuse.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.673143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      521 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      687 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/erroneus_message.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1150 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/log_message.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       96 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/parse_error.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4314 2023-03-06 09:22:45.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/result_message.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1123 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/sensor_info_response.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      752 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/set_baudrate_response.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2836 2023-02-27 12:43:10.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/setup_response.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1045 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/streaming_responses.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      791 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/system_info_response.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       97 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/server_error.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1998 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/links.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      643 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/message.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11369 2023-05-15 07:29:55.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/mock_client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3996 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.673143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      276 2023-05-15 07:29:55.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8225 2023-05-15 07:29:55.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/record.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3012 2023-05-15 07:29:55.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/record_io.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12719 2023-05-15 11:16:12.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/recorder.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1526 2023-05-15 07:29:55.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/session_schema.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      928 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.673143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/im_record/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       95 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/im_record/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3543 2023-05-15 07:29:55.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/im_record/im_record.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18924 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.673143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core_ext/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      118 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core_ext/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4868 2023-05-29 14:09:50.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core_ext/_replaying_client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      318 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_h5_utils.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7945 2023-06-09 13:10:48.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_perf_calc.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2516 2023-02-27 12:43:10.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_rate_calc.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.673143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      720 2023-06-12 13:00:08.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4086 2023-04-17 09:23:23.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/_base.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.673143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/_plugins/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      367 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/_plugins/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7933 2023-06-02 14:43:08.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/_plugins/_a121.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      434 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/_plugins/_detector.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      617 2023-03-06 09:22:45.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/_plugins/_null_app_model.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3783 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/_plugins/_processor_main.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.673143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/_plugins/processor/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      446 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/_plugins/processor/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8320 2023-06-02 14:43:08.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/_plugins/processor/backend_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1388 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/_plugins/processor/plot_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1276 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/_plugins/processor/plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6615 2023-06-09 13:10:48.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/_plugins/processor/view_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10729 2023-06-12 13:00:08.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/_utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.673143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/bilateration/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      175 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/bilateration/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      395 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/bilateration/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    24992 2023-06-09 13:10:48.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/bilateration/_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    17474 2023-03-29 12:24:17.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/bilateration/_processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.677143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/breathing/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      303 2023-06-12 13:00:08.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/breathing/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      759 2023-06-12 13:00:08.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/breathing/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    20031 2023-06-12 13:00:08.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/breathing/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8542 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/breathing/_ref_app.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    31517 2023-06-12 13:00:08.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/breathing/_ref_app_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6541 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/breathing/_serializer.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.677143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/distance/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      507 2023-03-29 12:24:17.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/distance/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      855 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/distance/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5471 2023-03-29 12:24:17.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/distance/_aggregator.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      307 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/distance/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    59448 2023-06-20 13:22:54.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/distance/_detector.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    26179 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/distance/_detector_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    30450 2023-06-20 13:22:54.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/distance/_processors.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15812 2023-03-29 12:24:17.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/distance/_serializers.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.677143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/phase_tracking/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      187 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/phase_tracking/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      376 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/phase_tracking/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7575 2023-03-03 13:14:28.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/phase_tracking/_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7141 2023-06-20 13:22:54.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/phase_tracking/_processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.677143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/presence/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      235 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/presence/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2175 2023-03-13 14:50:09.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/presence/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14812 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/presence/_detector.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    29697 2023-06-21 08:00:20.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/presence/_detector_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18288 2023-06-20 13:22:54.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/presence/_processors.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4717 2023-03-06 09:22:45.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/presence/_serializers.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.677143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/smart_presence/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      182 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/smart_presence/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2223 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/smart_presence/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6607 2023-03-23 08:31:28.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/smart_presence/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7165 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/smart_presence/_ref_app.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    21790 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/smart_presence/_ref_app_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6835 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/smart_presence/_serializer.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.677143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/sparse_iq/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      220 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/sparse_iq/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      376 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/sparse_iq/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8167 2023-03-06 09:22:45.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/sparse_iq/_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3116 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/sparse_iq/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7245 2023-03-06 09:22:45.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/sparse_iq/_serializers.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.677143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/speed/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      213 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/speed/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      347 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/speed/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14231 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/speed/_detector.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    21150 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/speed/_detector_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4909 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/speed/_processors.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.681143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/surface_velocity/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      130 2023-03-24 13:36:14.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/surface_velocity/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11611 2023-05-16 12:47:42.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/surface_velocity/_example_app.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    21732 2023-06-09 13:10:48.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/surface_velocity/_example_app_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14090 2023-06-20 13:22:54.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/surface_velocity/_processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.681143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/tank_level/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      219 2023-03-22 21:29:48.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/tank_level/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1658 2023-03-29 12:24:17.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/tank_level/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    29464 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/tank_level/_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7290 2023-06-20 13:22:54.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/tank_level/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6265 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/tank_level/_ref_app.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4229 2023-03-22 21:29:48.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/tank_level/_serializer.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.681143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/touchless_button/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      306 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/touchless_button/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      486 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/touchless_button/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1100 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/touchless_button/_blinkstick_updater.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1738 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/touchless_button/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7687 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/touchless_button/_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14754 2023-06-01 09:22:41.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/touchless_button/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2896 2023-03-29 12:24:17.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/touchless_button/_serializers.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.681143 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/vibration/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      187 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/vibration/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      376 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/vibration/__main__,py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8514 2023-04-28 14:58:15.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/vibration/_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7628 2023-06-20 13:22:54.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/vibration/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/a121/py.typed
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.681143 acconeer-exptool-7.1.0/src/acconeer/exptool/app/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      333 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4475 2023-03-31 10:16:50.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/launcher.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.681143 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      909 2023-06-09 13:10:48.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      116 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      994 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/_argument_parser.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1718 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/_enums.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      102 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/_exceptions.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      983 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/_version_checker.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2698 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/app.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.681143 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/app_model/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      239 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/app_model/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    27095 2023-06-21 08:08:21.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/app_model/app_model.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1404 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/app_model/app_model_listener.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      981 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/app_model/file_detective.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      428 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/app_model/plugin_protocols.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2074 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/app_model/port_updater.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.685143 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/backend/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      478 2023-06-02 14:43:08.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/backend/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2737 2023-05-15 07:29:55.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/backend/_application_client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4985 2023-06-02 14:43:08.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/backend/_backend.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1610 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/backend/_backend_logger.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2040 2023-06-02 14:43:08.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/backend/_backend_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1559 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/backend/_message.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4770 2023-06-02 14:43:08.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/backend/_model.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2786 2023-06-02 14:43:08.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/backend/_tasks.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1685 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/plugin_loader.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.685143 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/pluginbase/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      241 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/pluginbase/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      973 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/pluginbase/plot_plugin_base.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      431 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/pluginbase/plugin_preset_base.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1404 2023-03-06 09:22:45.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/pluginbase/plugin_spec_base.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1024 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/pluginbase/ui_plugin_base.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1836 2023-06-02 14:43:08.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/pluginbase/view_plugin_base.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/py.typed
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      470 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/qt_subclasses.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      804 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/storage.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.685143 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      445 2023-06-09 13:10:48.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2141 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/app_model_viewer.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2641 2023-04-11 13:56:57.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/device_comboboxes.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.685143 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/flash_tab/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       94 2023-04-21 06:43:18.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/flash_tab/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14023 2023-04-21 06:43:18.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/flash_tab/dialogs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4635 2023-04-19 09:25:35.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/flash_tab/threads.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15274 2023-06-09 13:10:48.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/flash_tab/widgets.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1802 2023-04-21 06:43:18.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/help_tab.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2142 2023-06-09 13:10:48.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/icons.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3910 2023-06-09 13:10:48.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/main_window.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1968 2023-04-11 13:56:57.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/misc.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.685143 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      798 2023-06-14 14:27:03.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7130 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/attrs_config_editor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1290 2023-03-13 14:50:09.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/collapsible_widget.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1026 2023-04-19 09:25:35.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/data_editor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6271 2023-06-14 14:27:03.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/json_save_load_buttons.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6159 2023-06-09 13:10:48.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/metadata_view.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1432 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/misc_error_view.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3612 2023-06-09 13:10:48.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/perf_calc_view.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.689143 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      769 2023-03-03 13:14:28.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      499 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/common.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3814 2023-04-19 09:25:35.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/hooks.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2082 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidget_groups.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    27081 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidgets.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2004 2023-04-28 14:58:15.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/range_help_view.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.689143 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/save_dialog/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      227 2023-06-14 14:27:03.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/save_dialog/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1757 2023-06-14 14:27:03.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/save_dialog/dialog.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6112 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/save_dialog/preview.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4004 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/save_dialog/set_config_presenter.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    13043 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/sensor_config_editor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6682 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/session_config_editor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7963 2023-04-19 09:25:35.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/subsweep_config_editor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1887 2023-04-19 09:25:35.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/two_sensor_ids_editor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      294 2023-04-19 09:25:35.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/types.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3848 2023-06-09 13:10:48.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/utils.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9480 2023-04-11 13:26:50.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/status_bar.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.689143 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/stream_tab/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       98 2023-04-11 13:56:57.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/stream_tab/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10441 2023-04-11 13:56:57.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/stream_tab/connection_widget.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5853 2023-04-11 13:56:57.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/stream_tab/hints.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12509 2023-06-09 13:10:48.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/stream_tab/plugin_widget.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4551 2023-04-11 13:56:57.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/stream_tab/recording_widget.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2636 2023-04-21 06:43:18.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/stream_tab/widgets.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1382 2023-04-21 06:43:18.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.689143 acconeer-exptool-7.1.0/src/acconeer/exptool/app/old/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       79 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/old/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      116 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/old/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    84005 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/old/app.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4735 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/old/data_processing.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.689143 acconeer-exptool-7.1.0/src/acconeer/exptool/app/old/elements/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/old/elements/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8476 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/old/elements/helper.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2346 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/old/elements/modules.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10745 2023-05-12 09:53:24.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/old/elements/qt_subclasses.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.689143 acconeer-exptool-7.1.0/src/acconeer/exptool/app/resources/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/resources/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    90184 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/resources/a111_gui.png
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    57036 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/resources/a121_gui.png
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4162 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/resources/icon-black.svg
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    35706 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/resources/icon.png
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3208 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/app/resources/loader.gif
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.637143 acconeer-exptool-7.1.0/src/acconeer/exptool/data/
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.689143 acconeer-exptool-7.1.0/src/acconeer/exptool/data/libft4222/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1245 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/data/libft4222/LICENSE.txt
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.693143 acconeer-exptool-7.1.0/src/acconeer/exptool/data/libft4222/aarch64/
+-rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   513305 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/data/libft4222/aarch64/libft4222.so.1.4.4.44
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.693143 acconeer-exptool-7.1.0/src/acconeer/exptool/data/libft4222/amd64/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   209008 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/data/libft4222/amd64/LibFT4222.dll
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   314552 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/data/libft4222/amd64/ftd2xx.dll
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.693143 acconeer-exptool-7.1.0/src/acconeer/exptool/data/libft4222/armv6/
+-rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   484176 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/data/libft4222/armv6/libft4222.so.1.4.4.44
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.693143 acconeer-exptool-7.1.0/src/acconeer/exptool/data/libft4222/armv7/
+-rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   399731 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/data/libft4222/armv7/libft4222.so.1.4.4.44
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.697143 acconeer-exptool-7.1.0/src/acconeer/exptool/data/libft4222/i386/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   160256 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/data/libft4222/i386/LibFT4222.dll
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   271672 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/data/libft4222/i386/ftd2xx.dll
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.697143 acconeer-exptool-7.1.0/src/acconeer/exptool/data/libft4222/x86_64/
+-rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   504389 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/data/libft4222/x86_64/libft4222.so.1.4.4.44
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.697143 acconeer-exptool-7.1.0/src/acconeer/exptool/flash/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      338 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/flash/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      115 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/flash/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5843 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/flash/_bin_fetcher.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3629 2023-06-21 07:39:31.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/flash/_dev_license.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4284 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/flash/_dev_license_tui.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      416 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/flash/_device_flasher_base.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12868 2023-04-04 08:04:50.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/flash/_flasher.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      828 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/flash/_products.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.697143 acconeer-exptool-7.1.0/src/acconeer/exptool/flash/_stm32uart/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      150 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/flash/_stm32uart/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      274 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/flash/_stm32uart/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6665 2023-03-30 21:08:35.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/flash/_stm32uart/_stm32flasher.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.697143 acconeer-exptool-7.1.0/src/acconeer/exptool/flash/_xc120/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      258 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/flash/_xc120/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9147 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/flash/_xc120/_bootloader_comm.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9417 2023-04-21 13:00:24.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/flash/_xc120/_bootloader_tool.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      224 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/flash/_xc120/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11051 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/libft4222.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3338 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/mpl_process.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3185 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/pg_process.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.697143 acconeer-exptool-7.1.0/src/acconeer/exptool/setup/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/setup/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1191 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/setup/__main__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.701143 acconeer-exptool-7.1.0/src/acconeer/exptool/setup/base/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      244 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/setup/base/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1431 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/setup/base/platform_install.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      980 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/setup/base/prompts.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      690 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/setup/base/setup_group.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2880 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/setup/base/setup_step.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      520 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/setup/base/utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.701143 acconeer-exptool-7.1.0/src/acconeer/exptool/setup/cli/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      106 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/setup/cli/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      684 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/setup/cli/argument_parser.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.701143 acconeer-exptool-7.1.0/src/acconeer/exptool/setup/platforms/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       91 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/setup/platforms/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      329 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/setup/platforms/how_to.txt
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1867 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/setup/platforms/linux.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1191 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/setup/platforms/ubuntu_20_04.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/setup/py.typed
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    21469 2023-03-22 21:29:48.000000 acconeer-exptool-7.1.0/src/acconeer/exptool/utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.701143 acconeer-exptool-7.1.0/src/acconeer_exptool.egg-info/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8990 2023-06-21 08:08:36.000000 acconeer-exptool-7.1.0/src/acconeer_exptool.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    26248 2023-06-21 08:08:36.000000 acconeer-exptool-7.1.0/src/acconeer_exptool.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-06-21 08:08:36.000000 acconeer-exptool-7.1.0/src/acconeer_exptool.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-06-21 08:08:36.000000 acconeer-exptool-7.1.0/src/acconeer_exptool.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      475 2023-06-21 08:08:36.000000 acconeer-exptool-7.1.0/src/acconeer_exptool.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        9 2023-06-21 08:08:36.000000 acconeer-exptool-7.1.0/src/acconeer_exptool.egg-info/top_level.txt
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.701143 acconeer-exptool-7.1.0/tools/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3930 2023-06-21 08:08:21.000000 acconeer-exptool-7.1.0/tools/check_changelog.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12005 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/tools/check_copyright.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1388 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/tools/check_line_length.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1495 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/tools/check_permissions.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4237 2023-04-03 10:32:44.000000 acconeer-exptool-7.1.0/tools/check_sdk_mentions.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1801 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/tools/check_whitespace.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2064 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/tools/update_regmap.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-21 08:08:36.701143 acconeer-exptool-7.1.0/utils/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14756 2023-02-16 14:46:04.000000 acconeer-exptool-7.1.0/utils/convert_to_csv.py
```

### Comparing `acconeer-exptool-7.0.2/.github/ISSUE_TEMPLATE/bug_report.md` & `acconeer-exptool-7.1.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/CHANGELOG.md` & `acconeer-exptool-7.1.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,24 @@
 # Changelog
 
+## v7.1.0
+
+### Added
+- New algorithm: Speed detector
+- Config load- & save for the majority of configs in the A121 App.
+- Export some configurations to C via the config save buttons.
+  + Sparse IQ
+  + Distance detector
+  + Presence detector
+  + Tank level
+- A121: Presence: Add context with estimated frame rate to presence detector
+
+### Changed
+- Breathing is now a reference application instead of an example
+
 ## v7.0.2
 
 ### Fixed
 - A121: Fix replaying issues in apps
 
 ## v7.0.1
 
@@ -73,15 +88,15 @@
 - A121: Tank level reference app
 - A121: Distance: Add recalibration functionality.
 - A121: Distance: Add calibration needed and temperature to API.
 - A121: Add surface velocity example app.
 - A121: Distance: Add reflector shape to detector config.
 - A121: Distance: Update peak sorting strategy selections.
 
-# Changed
+### Changed
 - Documentation structure
 - Client interface
 - Setting up instructions
 - Drop beta for A121 Application
 
 ## v5.9.2
```

### Comparing `acconeer-exptool-7.0.2/Jenkinsfile` & `acconeer-exptool-7.1.0/Jenkinsfile`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/LICENSE.md` & `acconeer-exptool-7.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/PKG-INFO` & `acconeer-exptool-7.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acconeer-exptool
-Version: 7.0.2
+Version: 7.1.0
 Summary: Acconeer Exploration Tool
 Home-page: https://github.com/acconeer/acconeer-python-exploration
 Author: Acconeer AB
 Author-email: tools@acconeer.com
 License: BSD 3-Clause Clear License
 Project-URL: Tracker, https://github.com/acconeer/acconeer-python-exploration/issues
 Project-URL: Documentation, https://acconeer-python-exploration.readthedocs.io
```

### Comparing `acconeer-exptool-7.0.2/README.md` & `acconeer-exptool-7.1.0/README.md`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/docker/Dockerfile` & `acconeer-exptool-7.1.0/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/dodo.py` & `acconeer-exptool-7.1.0/dodo.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/examples/a111/basic.py` & `acconeer-exptool-7.1.0/examples/a111/basic.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/examples/a111/basic_continuous.py` & `acconeer-exptool-7.1.0/examples/a111/basic_continuous.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/examples/a111/load_record.py` & `acconeer-exptool-7.1.0/examples/a111/load_record.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/examples/a111/load_record_h5.m` & `acconeer-exptool-7.1.0/examples/a111/load_record_h5.m`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/examples/a111/plotting/plot_with_matplotlib.py` & `acconeer-exptool-7.1.0/examples/a111/plotting/plot_with_matplotlib.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/examples/a111/plotting/plot_with_pyqtgraph.py` & `acconeer-exptool-7.1.0/examples/a111/plotting/plot_with_pyqtgraph.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/examples/a111/record_data/barebones.py` & `acconeer-exptool-7.1.0/examples/a111/record_data/barebones.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/examples/a111/record_data/long_duration_split_files.py` & `acconeer-exptool-7.1.0/examples/a111/record_data/long_duration_split_files.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/examples/a111/record_data/with_cli.py` & `acconeer-exptool-7.1.0/examples/a111/record_data/with_cli.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/examples/a111/services/envelope.py` & `acconeer-exptool-7.1.0/examples/a111/services/envelope.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/examples/a111/services/iq.py` & `acconeer-exptool-7.1.0/examples/a111/services/iq.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/examples/a111/services/power_bins.py` & `acconeer-exptool-7.1.0/examples/a111/services/power_bins.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/examples/a111/services/sparse.py` & `acconeer-exptool-7.1.0/examples/a111/services/sparse.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/examples/a111/utils/ping.py` & `acconeer-exptool-7.1.0/examples/a111/utils/ping.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/examples/a111/utils/test_throughput.py` & `acconeer-exptool-7.1.0/examples/a111/utils/test_throughput.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/examples/a121/basic.py` & `acconeer-exptool-7.1.0/examples/a121/basic.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/examples/a121/bilateration/bilaterator.py` & `acconeer-exptool-7.1.0/examples/a121/bilateration/bilaterator.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/examples/a121/breathing/breathing.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/distance_detector/ui.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,182 +1,180 @@
-# Copyright (c) Acconeer AB, 2022-2023
+# Copyright (c) Acconeer AB, 2022
 # All rights reserved
 
-from __future__ import annotations
-
-import time
-
 import numpy as np
 
-# Added here to force pyqtgraph to choose PySide
-import PySide6  # noqa: F401
-from PySide6.QtGui import QFont
-
 import pyqtgraph as pg
 
 import acconeer.exptool as et
-from acconeer.exptool import a121
-from acconeer.exptool.a121.algo.breathing import Processor, ProcessorConfig, get_sensor_config
-
-
-sensor_config = get_sensor_config()
-
 
-def main():
-    args = a121.ExampleArgumentParser().parse_args()
-    et.utils.config_logging(args)
 
-    client = a121.Client.open(**a121.get_client_args(args))
-    metadata = client.setup_session(sensor_config)
-
-    processor = Processor(
-        sensor_config=sensor_config, processor_config=ProcessorConfig(), metadata=metadata
-    )
-
-    pg_updater = PGUpdater(sensor_config, metadata)
-    pg_process = et.PGProcess(pg_updater)
-    pg_process.start()
-
-    client.start_session()
-    interrupt_handler = et.utils.ExampleInterruptHandler()
-    print("Press Ctrl-C to end session")
+class PGUpdater:
+    def __init__(self, sensor_config, processing_config, session_info):
+        self.sensor_config = sensor_config
+        self.processing_config = processing_config
+
+        self.r = et.a111.get_range_depths(sensor_config, session_info)
+
+        self.setup_is_done = False
+
+    def update_processing_config(self, processing_config=None):
+        if processing_config is None:
+            processing_config = self.processing_config
+        else:
+            self.processing_config = processing_config
+
+        if not self.setup_is_done:
+            return
+
+        # Hide the first_distance_above_threshold data
+        self.first_distance_above_threshold.setVisible(
+            processing_config.show_first_above_threshold
+        )
 
-    while not interrupt_handler.got_signal:
-        result = client.get_next()
+        # ...and hide the marker and text in the legend.
+        self.hist_plot.legend.items[2][0].setVisible(processing_config.show_first_above_threshold)
+        self.hist_plot.legend.items[2][1].setVisible(processing_config.show_first_above_threshold)
 
-        processor_result = processor.process(result)
+        self.hist_plot.setXRange(-processing_config.history_length_s, 0)
 
-        try:
-            pg_process.put_data(processor_result)
-        except et.PGProccessDiedException:
-            break
+    def setup(self, win):
+        win.setWindowTitle("Acconeer Distance Detector")
 
-    print("Disconnecting...")
-    client.close()
+        # Sweep Plot
+        self.sweep_plot = win.addPlot(title="Sweep and threshold")
+        self.sweep_plot.setMenuEnabled(False)
+        self.sweep_plot.setMouseEnabled(x=False, y=False)
+        self.sweep_plot.hideButtons()
+        self.sweep_plot.showGrid(x=True, y=True)
+        self.sweep_plot.addLegend()
+        self.sweep_plot.setLabel("bottom", "Distance (mm)")
+        self.sweep_plot.setYRange(0, 20000)
+        self.sweep_plot.setXRange(1000.0 * self.r[0], 1000.0 * self.r[-1])
+
+        self.sweep_curve = self.sweep_plot.plot(
+            pen=et.utils.pg_pen_cycler(5),
+            name="Envelope sweep",
+        )
 
+        self.mean_sweep_curve = self.sweep_plot.plot(
+            pen=et.utils.pg_pen_cycler(0, width=3),
+            name="Mean Envelope sweep",
+        )
 
-class PGUpdater:
+        self.threshold_curve = self.sweep_plot.plot(
+            pen=et.utils.pg_pen_cycler(1),
+            name="Threshold",
+        )
 
-    _TIME_SERIES_Y_SCALE_MARGIN_M = 0.0025
-    _DATA_INIT_DURATION = 5.0
+        self.smooth_max_sweep = et.utils.SmoothMax(
+            self.sensor_config.update_rate,
+            hysteresis=0.6,
+            tau_decay=3,
+        )
 
-    def __init__(self, sensor_config: a121.SensorConfig, metadata: a121.Metadata):
-        ...
+        self.peak_lines = []
+        for i in range(3):
+            color_idx = 1 if i > 0 else 0
+            width = 2 if i == 0 else 1
+            color_tuple = et.utils.hex_to_rgb_tuple(et.utils.color_cycler(color_idx))
+            line = pg.InfiniteLine(pen=pg.mkPen(pg.mkColor(*color_tuple, 150), width=width))
+            self.sweep_plot.addItem(line)
+            self.peak_lines.append(line)
+
+        self.peak_text = pg.TextItem(
+            anchor=(0, 1),
+            color=et.utils.color_cycler(0),
+            fill=pg.mkColor(0xFF, 0xFF, 0xFF, 150),
+        )
+        self.peak_text.setPos(self.r[0] * 1000, 0)
+        self.peak_text.setZValue(100)
+        self.sweep_plot.addItem(self.peak_text)
+
+        win.nextRow()
+
+        # Detection history Plot
+        self.hist_plot = win.addPlot(title="Detected peaks")
+        self.hist_plot.setMenuEnabled(False)
+        self.hist_plot.setMouseEnabled(x=False, y=False)
+        self.hist_plot.hideButtons()
+        self.hist_plot.showGrid(x=True, y=True)
+        self.hist_plot.addLegend()
+        self.hist_plot.setLabel("bottom", "Time history (s)")
+        self.hist_plot.setLabel("left", "Distance (mm)")
+        self.hist_plot.setXRange(-10, 0)
+        self.hist_plot.setYRange(1000.0 * self.r[0], 1000.0 * self.r[-1])
+
+        self.main_peak = self.hist_plot.plot(
+            pen=None,
+            symbol="o",
+            symbolSize=8,
+            symbolPen="k",
+            symbolBrush=et.utils.color_cycler(0),
+            name="Main peak",
+        )
 
-    def setup(self, win):
+        self.minor_peaks = self.hist_plot.plot(
+            pen=None,
+            symbol="o",
+            symbolSize=5,
+            symbolPen="k",
+            symbolBrush=et.utils.color_cycler(1),
+            name="Minor peaks",
+        )
 
-        pens = [et.utils.pg_pen_cycler(i) for i in range(5)]
-        brush = et.utils.pg_brush_cycler(0)
-        symbol_kw = dict(symbol="o", symbolSize=1, symbolBrush=brush, symbolPen="k")
-        feat_kws = [dict(pen=pen, **symbol_kw) for pen in pens]
-
-        font = QFont()
-        font.setPixelSize(16.0)
-
-        # time series plot
-        self.time_series_plot = win.addPlot(row=0, col=0)
-        self.time_series_plot.setMenuEnabled(False)
-        self.time_series_plot.showGrid(x=True, y=True)
-        self.time_series_plot.addLegend()
-        self.time_series_plot.setLabel("left", "Displacement (m)")
-        self.time_series_plot.setLabel("bottom", "Time")
-        self.time_series_plot.addItem(pg.PlotDataItem())
-        self.time_series_curve = []
-        self.time_series_curve.append(self.time_series_plot.plot(**feat_kws[0]))
-        self.time_series_curve.append(self.time_series_plot.plot(**feat_kws[1]))
-
-        self.time_series_smooth_limits = et.utils.SmoothLimits()
-
-        self.time_series_text_item = pg.TextItem(
-            fill=pg.mkColor(0xFF, 0x7F, 0x0E, 200),
-            anchor=(0.5, 0),
-            color=pg.mkColor(0xFF, 0xFF, 0xFF, 200),
-        )
-        self.time_series_text_item.setFont(font)
-        self.time_series_text_item.show()
-        self.time_series_plot.addItem(self.time_series_text_item)
-
-        # fft plot
-        self.fft_plot = win.addPlot(row=1, col=0)
-        self.fft_plot.setMenuEnabled(False)
-        self.fft_plot.showGrid(x=True, y=True)
-        self.fft_plot.addLegend()
-        self.fft_plot.setLabel("left", "Power")
-        self.fft_plot.setLabel("bottom", "Frequency (Hz)")
-        self.fft_plot.addItem(pg.PlotDataItem())
-        self.fft_curve = self.fft_plot.plot(**feat_kws[0])
-        self.fft_vert_line = pg.InfiniteLine(pen=pens[1])
-        self.fft_plot.addItem(self.fft_vert_line)
-
-        self.fft_smooth_max = et.utils.SmoothMax(tau_grow=0.5, tau_decay=2.0)
-
-        self.fft_text_item = pg.TextItem(
-            fill=pg.mkColor(0xFF, 0x7F, 0x0E, 200),
-            anchor=(0.5, 0),
-            color=pg.mkColor(0xFF, 0xFF, 0xFF, 200),
-        )
-        self.fft_text_item.setFont(font)
-        self.fft_text_item.show()
-        self.fft_plot.addItem(self.fft_text_item)
-
-        self.start_time = time.time()
-
-    def update(self, processor_result):
-        time_series = processor_result.time_series
-        distance_to_analyze_m = processor_result.distance_to_analyze_m
-        z_abs_lp = processor_result.lp_psd
-        freqs = processor_result.freqs
-        breathing_rate = processor_result.breathing_rate
-        fft_peak_location = processor_result.fft_peak_location
-
-        # time series plot
-        self.time_series_curve[0].setData(time_series)
-        lim = self.time_series_smooth_limits.update(time_series)
-
-        self.time_series_plot.setYRange(
-            lim[0] - self._TIME_SERIES_Y_SCALE_MARGIN_M,
-            lim[1] + self._TIME_SERIES_Y_SCALE_MARGIN_M,
-        )
-        text_y_pos = self.time_series_plot.getAxis("left").range[1] * 0.95
-        text_x_pos = self.time_series_plot.getAxis("bottom").range[1] / 2.0
-        self.time_series_text_item.setPos(text_x_pos, text_y_pos)
-        self.time_series_text_item.setHtml(
-            "Distance being visualized: " + "{:.2f}".format(distance_to_analyze_m) + " (m)"
-        )
-
-        # fft plot
-        if (time.time() - self.start_time) < self._DATA_INIT_DURATION:
-            self.fft_curve.setData(freqs, np.zeros_like(freqs))
-            self.fft_plot.setYRange(0.0, 1.0)
-
-            text_y_pos = self.fft_plot.getAxis("left").range[1] * 0.95
-            text_x_pos = self.fft_plot.getAxis("bottom").range[1] / 2.0
-            self.fft_text_item.setHtml("Acquiring data.")
-        elif freqs is not None:
-            assert z_abs_lp is not None
-            assert breathing_rate is not None
-            assert fft_peak_location is not None
-
-            self.fft_curve.setData(freqs, z_abs_lp)
-            self.fft_vert_line.setValue(fft_peak_location)
-            lim = self.fft_smooth_max.update(z_abs_lp)
-            self.fft_plot.setYRange(0.0, lim * 1.2)
+        self.first_distance_above_threshold = self.hist_plot.plot(
+            pen=None,
+            symbol="o",
+            symbolSize=3,
+            symbolPen="k",
+            symbolBrush=et.utils.color_cycler(2),
+            name="First distance above threshold",
+            visible=False,
+        )
 
-            text_y_pos = self.fft_plot.getAxis("left").range[1] * 0.95
-            text_x_pos = self.fft_plot.getAxis("bottom").range[1] / 2.0
+        self.setup_is_done = True
+        self.update_processing_config()
 
-            self.fft_text_item.setHtml(
-                "Breathing rate: " + "{:.1f}".format(breathing_rate) + " per minute"
+    def update(self, data):
+        self.sweep_curve.setData(1000.0 * self.r, data["sweep"])
+        self.mean_sweep_curve.setData(1000.0 * self.r, data["last_mean_sweep"])
+        self.threshold_curve.setData(1000.0 * self.r, data["threshold"])
+
+        m = np.nanmax(
+            np.concatenate(
+                [
+                    2 * data["threshold"],
+                    data["sweep"],
+                    data["last_mean_sweep"],
+                ]
             )
-        self.fft_text_item.setPos(text_x_pos, text_y_pos)
+        )
+        ymax = self.smooth_max_sweep.update(m)
+        self.sweep_plot.setYRange(0, ymax)
 
-    @staticmethod
-    def _format_string(string_to_display: str) -> str:
-        return (
-            '<div style="text-align: center">'
-            '<span style="color: #FFFFFF;font-size:15pt;">'
-            "{}</span></div>".format(string_to_display)
+        self.main_peak.setData(data["main_peak_hist_sweep_s"], 1000 * data["main_peak_hist_dist"])
+        self.minor_peaks.setData(
+            data["minor_peaks_hist_sweep_s"], 1000 * data["minor_peaks_hist_dist"]
+        )
+        self.first_distance_above_threshold.setData(
+            data["above_thres_hist_sweep_s"], 1000 * data["above_thres_hist_dist"]
         )
 
+        if data["found_peaks"] is not None:
+            peaks = np.take(self.r, data["found_peaks"]) * 1000.0
+            for i, line in enumerate(self.peak_lines):
+                try:
+                    peak = peaks[i]
+                except (TypeError, IndexError):
+                    line.hide()
+                else:
+                    line.setPos(peak)
+                    line.show()
+
+            if data["found_peaks"]:
+                amplitude = data["sweep"][data["found_peaks"][0]]
+                text = "{:.2f} mm, {:.1f}".format(peaks[0], amplitude)
+            else:
+                text = "-"
 
-if __name__ == "__main__":
-    main()
+            self.peak_text.setText(text)
```

### Comparing `acconeer-exptool-7.0.2/examples/a121/distance/detector.py` & `acconeer-exptool-7.1.0/examples/a121/distance/detector.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/examples/a121/distance/processor.py` & `acconeer-exptool-7.1.0/examples/a121/distance/processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/examples/a121/extended_config.py` & `acconeer-exptool-7.1.0/examples/a121/extended_config.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/examples/a121/load_record.py` & `acconeer-exptool-7.1.0/examples/a121/load_record.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/examples/a121/load_record_h5.m` & `acconeer-exptool-7.1.0/examples/a121/load_record_h5.m`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/examples/a121/phase_tracking/phase_tracking.py` & `acconeer-exptool-7.1.0/examples/a121/phase_tracking/phase_tracking.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/examples/a121/plot.py` & `acconeer-exptool-7.1.0/examples/a121/plot.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/examples/a121/presence/detector.py` & `acconeer-exptool-7.1.0/examples/a121/presence/detector.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/examples/a121/presence/processor.py` & `acconeer-exptool-7.1.0/examples/a121/presence/processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/examples/a121/record_data/barebones.py` & `acconeer-exptool-7.1.0/examples/a121/record_data/barebones.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/examples/a121/record_data/with_cli.py` & `acconeer-exptool-7.1.0/examples/a121/record_data/with_cli.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/examples/a121/reuse_calibration.py` & `acconeer-exptool-7.1.0/examples/a121/reuse_calibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/examples/a121/smart_presence/processor.py` & `acconeer-exptool-7.1.0/examples/a121/smart_presence/processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/examples/a121/smart_presence/ref_app.py` & `acconeer-exptool-7.1.0/examples/a121/smart_presence/ref_app.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/examples/a121/stress.py` & `acconeer-exptool-7.1.0/examples/a121/stress.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/examples/a121/subsweeps.py` & `acconeer-exptool-7.1.0/examples/a121/subsweeps.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/examples/a121/surface_velocity/example_app.py` & `acconeer-exptool-7.1.0/examples/a121/surface_velocity/example_app.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/examples/a121/surface_velocity/processor.py` & `acconeer-exptool-7.1.0/examples/a121/surface_velocity/processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/examples/a121/touchless_button/processor.py` & `acconeer-exptool-7.1.0/examples/a121/touchless_button/processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/examples/a121/vibration/vibration.py` & `acconeer-exptool-7.1.0/examples/a121/vibration/vibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/gui/main.py` & `acconeer-exptool-7.1.0/gui/main.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/noxfile.py` & `acconeer-exptool-7.1.0/noxfile.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,17 +10,16 @@
 py_ver = ".".join(map(str, sys.version_info[:2]))
 nox.options.sessions = ["lint", "docs", f"test(python='{py_ver}')"]
 nox.options.stop_on_first_error = True
 nox.options.reuse_existing_virtualenvs = True
 
 
 BLACK_SPEC = "black==22.12.0"
-ISORT_SPEC = "isort==5.6.3"
-RUFF_SPEC = "ruff==0.0.260"
-MYPY_SPEC = "mypy==1.2.0"
+RUFF_SPEC = "ruff==0.0.270"
+MYPY_SPEC = "mypy==1.3.0"
 PIP_SPEC = "pip>=21.3"
 PYTEST_MOCK_SPEC = "pytest-mock==3.3.1"
 PYTEST_SPEC = "pytest==7.2"
 PYTEST_XDIST_SPEC = "pytest-xdist==3.1.0"
 DIRTY_EQUALS_SPEC = "dirty-equals==0.5.0"
 
 SPHINX_SOURCE_DIR = "docs"
@@ -69,47 +68,33 @@
             choices=self.KNOWN_DOCS_BUILDERS,
             default=self.DEFAULT_DOCS_BUILDERS,
         )
 
 
 @nox.session
 def lint(session):
-    session.install(
-        BLACK_SPEC,
-        ISORT_SPEC,
-        RUFF_SPEC,
-        "flake8",
-        "flake8-future-annotations",
-        "packaging",
-    )
-    FUTURE_ANNOTATIONS_ERRORS = "FA10"
+    session.install(BLACK_SPEC, RUFF_SPEC, "packaging")
 
     session.run("python", "tools/check_permissions.py")
     session.run("python", "tools/check_whitespace.py")
     session.run("python", "tools/check_line_length.py")
     session.run("python", "tools/check_sdk_mentions.py")
     session.run("python", "tools/check_changelog.py")
     session.run("python", "tools/check_copyright.py")
     session.run("python", "-m", "ruff", ".")
-    session.run("python", "-m", "flake8", "--select", FUTURE_ANNOTATIONS_ERRORS)
     session.run("python", "-m", "black", "--check", "--diff", "--quiet", ".")
-    session.run("python", "-m", "isort", "--check", "--diff", "--quiet", ".")
 
 
 @nox.session
 def reformat(session):
-    session.install(
-        BLACK_SPEC,
-        ISORT_SPEC,
-        RUFF_SPEC,
-    )
+    session.install(BLACK_SPEC, RUFF_SPEC)
+
     session.run("python", "tools/check_copyright.py", "--update-year")
     session.run("python", "-m", "black", ".")
     session.run("python", "-m", "ruff", "--fix", ".")
-    session.run("python", "-m", "isort", ".")
 
 
 @nox.session
 @nox.parametrize("python", ["3.7"])
 def mypy(session):
     session.install("-e", ".", MYPY_SPEC, PYTEST_SPEC)
     session.run("python", "-m", "mypy")
```

### Comparing `acconeer-exptool-7.0.2/portable/make.py` & `acconeer-exptool-7.1.0/portable/make.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/portable/package/tools/update.py` & `acconeer-exptool-7.1.0/portable/package/tools/update.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/pyproject.toml` & `acconeer-exptool-7.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -12,40 +12,39 @@
 write_to_template = "__version__ = \"{version}\"\n"
 
 [tool.black]
 line-length = 99
 
 [tool.ruff]
 # "extend" here adds to the ruff defaults, rather than replacing.
-extend-select = ["Q", "TID"]  # Q = flake8-quotes, TID = flake8-tidy-imports
-extend-ignore = ["E741"]  # Ambiguous variable names, e.g. I vs l
+# Q = flake8-quotes, TID = flake8-tidy-imports, I = isort, FA = flake8-future-annotations
+extend-select = ["Q", "TID", "I", "FA"]
+# E741 = Ambiguous variable names, e.g. I vs l
+# E501 = "line too long". Handled by black.
+extend-ignore = ["E741", "E501"]
 
 line-length = 100
 
 show-fixes = true
 show-source = true
 
-src = ["src"]
+src = ["src", "tests"]
 namespace-packages = ["src/acconeer"]
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401", "E402"]
 "src/acconeer/exptool/_winusbcdc/*" = ["F40", "E501"]
 
 [tool.ruff.flake8-tidy-imports]
 ban-relative-imports = "parents"
 
-[tool.isort]
-line_length = 99
-lines_after_imports = 2
-multi_line_output = 3
-indent = 4
-default_section = "FIRSTPARTY"
-include_trailing_comma = true
-known_third_party = [
+[tool.ruff.isort]
+lines-after-imports = 2
+
+known-third-party = [
     "numpy",
     "scipy",
     "serial",
     "matplotlib",
     "h5py",
     "flask",
     "yaml",
@@ -60,43 +59,29 @@
     "attrs",
     "typing_extensions",
     "qdarktheme",
     "qtawesome",
     "pyperclip",
     "psutil",
 ]
-known_qt = "PySide6"
-known_plotting = "pyqtgraph"
-known_acconeer = "acconeer"
-sections = [
-    "FUTURE",
-    "STDLIB",
-    "THIRDPARTY",
-    "QT",
-    "PLOTTING",
-    "ACCONEER",
-    "FIRSTPARTY",
-    "LOCALFOLDER",
-]
-skip = [
-    ".git",
-    "__pycache__",
-    "build",
-    "dist",
-    "*.egg-info",
-    "env",
-    "venv",
-    "stash",
-    ".tox",
-    ".nox",
-    ".mypy_cache",
-    ".pytest_cache",
-    "get-pip.py",
+section-order = [
+    "future",
+    "standard-library",
+    "third-party",
+    "PySide6",
+    "pyqtgraph",
+    "acconeer",
+    "first-party",
+    "local-folder",
 ]
-profile = "black"
+
+[tool.ruff.isort.sections]
+"PySide6" = ["PySide6"]
+"pyqtgraph" = ["pyqtgraph"]
+"acconeer" = ["acconeer"]
 
 [tool.mypy]
 packages = [
     "acconeer.exptool.a121",
     "acconeer.exptool.app.new",
     "acconeer.exptool.setup",
     "tests.unit.a121",
```

### Comparing `acconeer-exptool-7.0.2/setup.cfg` & `acconeer-exptool-7.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/_bs_thread.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/_bs_thread.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/_pyusb/pyusbcomm.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/_pyusb/pyusbcomm.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/_structs/configbase.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/_structs/configbase.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/_structs/qtpidgets.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/_structs/qtpidgets.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/_tests/test_rig.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/_tests/test_rig.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/_winusbcdc/LICENSE` & `acconeer-exptool-7.1.0/src/acconeer/exptool/_winusbcdc/LICENSE`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/_winusbcdc/__main__.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/_winusbcdc/__main__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/_winusbcdc/usb_cdc.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/_winusbcdc/usb_cdc.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/_winusbcdc/winusb.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/_winusbcdc/winusb.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/_winusbcdc/winusbclasses.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/_winusbcdc/winusbclasses.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/_winusbcdc/winusbpy.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/_winusbcdc/winusbpy.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/_winusbcdc/winusbutils.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/_winusbcdc/winusbutils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/base.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/base.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/client.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/client_factory.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/client_factory.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/common.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/common.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/json/client.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/json/client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/links.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/links.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/mock/client.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/mock/client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/multiwrap.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/multiwrap.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/reg/client.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/reg/client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/reg/data/regmap.yaml` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/reg/data/regmap.yaml`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/reg/protocol.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/reg/protocol.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/reg/regmap.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_clients/reg/regmap.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_conf_to_rss_sdk.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_conf_to_rss_sdk.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_configs.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_configs.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_modes.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_modes.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_utils.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/_utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/_base/calibration.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/_base/calibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/_base/module_info.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/_base/module_info.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/_standalone_main.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/_standalone_main.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/breathing/_meta.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/breathing/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/breathing/_processor.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/breathing/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/breathing/ui.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/breathing/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/button_press/_meta.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/button_press/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/button_press/_processor.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/button_press/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/button_press/ui.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/button_press/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/button_press_sparse/_meta.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/button_press_sparse/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/button_press_sparse/_processor.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/button_press_sparse/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/button_press_sparse/ui.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/button_press_sparse/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/distance_detector/_meta.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/distance_detector/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/distance_detector/_processor.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/distance_detector/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/distance_detector/calibration.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/distance_detector/calibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/distance_detector/ui.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/_processor.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,180 +1,177 @@
 # Copyright (c) Acconeer AB, 2022
 # All rights reserved
 
 import numpy as np
 
-import pyqtgraph as pg
-
 import acconeer.exptool as et
 
 
-class PGUpdater:
-    def __init__(self, sensor_config, processing_config, session_info):
-        self.sensor_config = sensor_config
-        self.processing_config = processing_config
-
-        self.r = et.a111.get_range_depths(sensor_config, session_info)
-
-        self.setup_is_done = False
-
-    def update_processing_config(self, processing_config=None):
-        if processing_config is None:
-            processing_config = self.processing_config
-        else:
-            self.processing_config = processing_config
-
-        if not self.setup_is_done:
-            return
-
-        # Hide the first_distance_above_threshold data
-        self.first_distance_above_threshold.setVisible(
-            processing_config.show_first_above_threshold
+def get_sensor_config():
+    config = et.a111.SparseServiceConfig()
+    config.profile = et.a111.SparseServiceConfig.Profile.PROFILE_3
+    config.range_interval = [0.48, 0.72]
+    config.sweeps_per_frame = 16
+    config.hw_accelerated_average_samples = 60
+    config.update_rate = 60
+    return config
+
+
+class ProcessingConfiguration(et.configbase.ProcessingConfig):
+    VERSION = 1
+    WINDOW_SIZE_POW_OF_2_MAX = 12
+    ROLLING_HISTORY_SIZE_MAX = 1000
+
+    show_time_domain = et.configbase.BoolParameter(
+        label="Show data in time domain",
+        default_value=True,
+        updateable=True,
+        order=0,
+    )
+
+    show_spect_history = et.configbase.BoolParameter(
+        label="Show spectrum history",
+        default_value=False,
+        updateable=True,
+        order=10,
+    )
+
+    show_depthwise_spect = et.configbase.BoolParameter(
+        label="Show depthwise spectrum",
+        default_value=False,
+        updateable=True,
+        order=20,
+    )
+
+    window_size_pow_of_2 = et.configbase.FloatParameter(
+        label="Window size, power of 2",
+        default_value=8,
+        limits=(3, WINDOW_SIZE_POW_OF_2_MAX),
+        decimals=0,
+        updateable=True,
+        order=100,
+    )
+
+    _window_size = et.configbase.get_virtual_parameter_class(et.configbase.IntParameter)(
+        label="Window size",
+        get_fun=lambda conf: 2 ** int(conf.window_size_pow_of_2),
+        visible=False,
+    )
+
+    overlap = et.configbase.FloatParameter(
+        label="Overlap",
+        default_value=0.95,
+        limits=(0, 1),
+        updateable=True,
+        order=200,
+    )
+
+    rolling_history_size = et.configbase.FloatParameter(
+        label="Rolling history size",
+        default_value=100,
+        decimals=0,
+        logscale=True,
+        limits=(10, ROLLING_HISTORY_SIZE_MAX),
+        updateable=True,
+        order=300,
+    )
+
+    def check(self):
+        alerts = super().check()
+
+        msg = "{}".format(self._window_size)
+        alerts.append(et.configbase.Info("window_size_pow_of_2", msg))
+
+        return alerts
+
+
+class Processor:
+    def __init__(self, sensor_config, processing_config, session_info, calibration=None):
+        self.f = sensor_config.update_rate
+        depths = et.a111.get_range_depths(sensor_config, session_info)
+        self.num_depths = depths.size
+
+        max_window_size = 2**ProcessingConfiguration.WINDOW_SIZE_POW_OF_2_MAX
+        self.sweep_history = np.full([max_window_size, self.num_depths], np.nan)
+
+        self.collapsed_asd = None
+        self.collapsed_asd_history = None
+
+        self.window_size = None
+        self.frames_between_updates = None
+        self.rolling_history_size = None
+
+        self.tick_idx = 0
+        self.last_update_tick = 0
+
+        self.update_processing_config(processing_config)
+
+    def update_processing_config(self, processing_config):
+        invalid = self.window_size != processing_config._window_size
+
+        self.window_size = processing_config._window_size
+        self.frames_between_updates = int(
+            round(self.window_size * (1 - processing_config.overlap))
         )
 
-        # ...and hide the marker and text in the legend.
-        self.hist_plot.legend.items[2][0].setVisible(processing_config.show_first_above_threshold)
-        self.hist_plot.legend.items[2][1].setVisible(processing_config.show_first_above_threshold)
-
-        self.hist_plot.setXRange(-processing_config.history_length_s, 0)
-
-    def setup(self, win):
-        win.setWindowTitle("Acconeer Distance Detector")
-
-        # Sweep Plot
-        self.sweep_plot = win.addPlot(title="Sweep and threshold")
-        self.sweep_plot.setMenuEnabled(False)
-        self.sweep_plot.setMouseEnabled(x=False, y=False)
-        self.sweep_plot.hideButtons()
-        self.sweep_plot.showGrid(x=True, y=True)
-        self.sweep_plot.addLegend()
-        self.sweep_plot.setLabel("bottom", "Distance (mm)")
-        self.sweep_plot.setYRange(0, 20000)
-        self.sweep_plot.setXRange(1000.0 * self.r[0], 1000.0 * self.r[-1])
-
-        self.sweep_curve = self.sweep_plot.plot(
-            pen=et.utils.pg_pen_cycler(5),
-            name="Envelope sweep",
-        )
+        self.rolling_history_size = int(processing_config.rolling_history_size)
 
-        self.mean_sweep_curve = self.sweep_plot.plot(
-            pen=et.utils.pg_pen_cycler(0, width=3),
-            name="Mean Envelope sweep",
-        )
+        if invalid:
+            self.collapsed_asd_history = np.zeros(
+                [
+                    ProcessingConfiguration.ROLLING_HISTORY_SIZE_MAX,
+                    self.window_size // 2,
+                ]
+            )
 
-        self.threshold_curve = self.sweep_plot.plot(
-            pen=et.utils.pg_pen_cycler(1),
-            name="Threshold",
-        )
+        if invalid and self.tick_idx > 0:
+            self.update_spect()
 
-        self.smooth_max_sweep = et.utils.SmoothMax(
-            self.sensor_config.update_rate,
-            hysteresis=0.6,
-            tau_decay=3,
-        )
+    def process(self, data, data_info):
+        frame = data
 
-        self.peak_lines = []
-        for i in range(3):
-            color_idx = 1 if i > 0 else 0
-            width = 2 if i == 0 else 1
-            color_tuple = et.utils.hex_to_rgb_tuple(et.utils.color_cycler(color_idx))
-            line = pg.InfiniteLine(pen=pg.mkPen(pg.mkColor(*color_tuple, 150), width=width))
-            self.sweep_plot.addItem(line)
-            self.peak_lines.append(line)
-
-        self.peak_text = pg.TextItem(
-            anchor=(0, 1),
-            color=et.utils.color_cycler(0),
-            fill=pg.mkColor(0xFF, 0xFF, 0xFF, 150),
-        )
-        self.peak_text.setPos(self.r[0] * 1000, 0)
-        self.peak_text.setZValue(100)
-        self.sweep_plot.addItem(self.peak_text)
-
-        win.nextRow()
-
-        # Detection history Plot
-        self.hist_plot = win.addPlot(title="Detected peaks")
-        self.hist_plot.setMenuEnabled(False)
-        self.hist_plot.setMouseEnabled(x=False, y=False)
-        self.hist_plot.hideButtons()
-        self.hist_plot.showGrid(x=True, y=True)
-        self.hist_plot.addLegend()
-        self.hist_plot.setLabel("bottom", "Time history (s)")
-        self.hist_plot.setLabel("left", "Distance (mm)")
-        self.hist_plot.setXRange(-10, 0)
-        self.hist_plot.setYRange(1000.0 * self.r[0], 1000.0 * self.r[-1])
-
-        self.main_peak = self.hist_plot.plot(
-            pen=None,
-            symbol="o",
-            symbolSize=8,
-            symbolPen="k",
-            symbolBrush=et.utils.color_cycler(0),
-            name="Main peak",
-        )
+        mean_sweep = frame.mean(axis=0)
 
-        self.minor_peaks = self.hist_plot.plot(
-            pen=None,
-            symbol="o",
-            symbolSize=5,
-            symbolPen="k",
-            symbolBrush=et.utils.color_cycler(1),
-            name="Minor peaks",
-        )
+        self.sweep_history = np.roll(self.sweep_history, -1, axis=0)
+        self.sweep_history[-1] = mean_sweep
 
-        self.first_distance_above_threshold = self.hist_plot.plot(
-            pen=None,
-            symbol="o",
-            symbolSize=3,
-            symbolPen="k",
-            symbolBrush=et.utils.color_cycler(2),
-            name="First distance above threshold",
-            visible=False,
-        )
+        outdated = (self.tick_idx - self.last_update_tick) > self.frames_between_updates
+        if self.tick_idx == 0 or outdated:
+            self.update_spect()
 
-        self.setup_is_done = True
-        self.update_processing_config()
+        self.tick_idx += 1
 
-    def update(self, data):
-        self.sweep_curve.setData(1000.0 * self.r, data["sweep"])
-        self.mean_sweep_curve.setData(1000.0 * self.r, data["last_mean_sweep"])
-        self.threshold_curve.setData(1000.0 * self.r, data["threshold"])
+        return self.gather_result()
 
-        m = np.nanmax(
-            np.concatenate(
-                [
-                    2 * data["threshold"],
-                    data["sweep"],
-                    data["last_mean_sweep"],
-                ]
-            )
-        )
-        ymax = self.smooth_max_sweep.update(m)
-        self.sweep_plot.setYRange(0, ymax)
+    def update_spect(self):
+        x = self.sweep_history[-self.window_size :]
+        x = x - np.nanmean(x, axis=0, keepdims=True)
+        x = np.nan_to_num(x)
+        fft = np.fft.rfft(x.T * np.hanning(x.shape[0]), axis=1)
+        asd = np.abs(fft)[:, 1:]
 
-        self.main_peak.setData(data["main_peak_hist_sweep_s"], 1000 * data["main_peak_hist_dist"])
-        self.minor_peaks.setData(
-            data["minor_peaks_hist_sweep_s"], 1000 * data["minor_peaks_hist_dist"]
-        )
-        self.first_distance_above_threshold.setData(
-            data["above_thres_hist_sweep_s"], 1000 * data["above_thres_hist_dist"]
-        )
+        self.collapsed_asd = asd.sum(axis=0)
+        self.dw_asd = asd
+
+        self.collapsed_asd_history = np.roll(self.collapsed_asd_history, -1, axis=0)
+        self.collapsed_asd_history[-1] = self.collapsed_asd
+
+        self.last_update_tick = self.tick_idx
+
+    def gather_result(self):
+        ts = np.arange(-self.window_size, 0, dtype="float") + 1
+        fs = np.arange(self.window_size // 2, dtype="float") + 1
+
+        if self.f:
+            ts *= 1 / self.f
+            fs *= 0.5 * self.f / fs[-1]
 
-        if data["found_peaks"] is not None:
-            peaks = np.take(self.r, data["found_peaks"]) * 1000.0
-            for i, line in enumerate(self.peak_lines):
-                try:
-                    peak = peaks[i]
-                except (TypeError, IndexError):
-                    line.hide()
-                else:
-                    line.setPos(peak)
-                    line.show()
-
-            if data["found_peaks"]:
-                amplitude = data["sweep"][data["found_peaks"][0]]
-                text = "{:.2f} mm, {:.1f}".format(peaks[0], amplitude)
-            else:
-                text = "-"
+        cropped_history = self.collapsed_asd_history[-self.rolling_history_size :]
 
-            self.peak_text.setText(text)
+        return {
+            "ts": ts,
+            "sweep_history": self.sweep_history[-self.window_size :],
+            "fs": fs,
+            "collapsed_asd": self.collapsed_asd,
+            "collapsed_asd_history": cropped_history,
+            "dw_asd": self.dw_asd,
+        }
```

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/envelope/_meta.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/envelope/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/envelope/_processor.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/envelope/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/envelope/calibration.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/envelope/calibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/envelope/ui.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/envelope/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/iq/_meta.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/iq/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/iq/_processor.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/iq/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/iq/ui.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/iq/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/obstacle_detection/_meta.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/obstacle_detection/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/obstacle_detection/_processor.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/obstacle_detection/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/obstacle_detection/calibration.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/obstacle_detection/calibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/obstacle_detection/ui.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/obstacle_detection/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/parking/_meta.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/parking/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/parking/_processor.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/parking/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/parking/ui.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/parking/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/phase_tracking/_meta.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/phase_tracking/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/phase_tracking/_processor.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/phase_tracking/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/phase_tracking/ui.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/phase_tracking/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/power_bins/_meta.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/power_bins/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/power_bins/ui.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/power_bins/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/presence_detect_human_only/_meta.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/presence_detect_human_only/_processor.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/presence_detect_human_only/ui.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/presence_detection_sparse/_meta.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/presence_detection_sparse/_processor.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/presence_detection_sparse/ui.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sleep_breathing/_meta.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sleep_breathing/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sleep_breathing/_processor.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sleep_breathing/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sleep_breathing/ui.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sleep_breathing/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse/_meta.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse/_processor.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse/ui.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse_fft/_meta.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse_fft/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse_fft/_processor.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse_fft/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse_fft/ui.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse_fft/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse_inter_fft/_meta.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse_inter_fft/ui.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/speed_sparse/_meta.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/speed_sparse/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/speed_sparse/_processor.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/speed_sparse/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/speed_sparse/ui.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/speed_sparse/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/tank_level_short/_meta.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/tank_level_short/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/tank_level_short/_processor.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/tank_level_short/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/tank_level_short/calibration.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/tank_level_short/calibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/tank_level_short/ui.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/tank_level_short/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/utils.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/wave_to_exit/_meta.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/wave_to_exit/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/wave_to_exit/_processor.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/wave_to_exit/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/wave_to_exit/ui.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/algo/wave_to_exit/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/recording.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a111/recording.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/__init__.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,9 +44,14 @@
     open_record,
     save_record,
     save_record_to_h5,
     zip3_extended_structures,
     zip_extended_structures,
 )
 from ._core_ext import _ReplayingClient, _StopReplay
-from ._perf_calc import _SensorPerformanceCalc, _SessionPerformanceCalc
+from ._perf_calc import (
+    _SensorPerformanceCalc,
+    _SessionPerformanceCalc,
+    get_point_overhead_duration,
+    get_sample_duration,
+)
 from ._rate_calc import _RateCalculator, _RateStats
```

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_cli.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_cli.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/__init__.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/__init__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/__init__.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/configs/config_enums.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/configs/config_enums.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/configs/sensor_config.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/configs/sensor_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,14 +123,16 @@
     :param num_subsweeps:
         Initialize with a given number of subsweeps. May not be combined with ``subsweeps``.
     :raises ValueError: If ``subsweeps`` and ``num_subsweeps`` are both given.
     :raises ValueError: If the given list of ``subsweeps`` is empty.
     :raises ValueError: If subsweeps parameters are both given implicitly and via ``subsweeps``.
     """
 
+    MAX_HWAAS = SubsweepConfig.MAX_HWAAS
+
     _subsweeps: list[SubsweepConfig]
 
     _sweeps_per_frame: int
     _sweep_rate: Optional[float]
     _frame_rate: Optional[float]
     _continuous_sweep_mode: bool
     _double_buffering: bool
```

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/configs/session_config.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/configs/session_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,16 +73,14 @@
         Forces whether to use the extended format or not. If not given (``= None``), the extended
         format will be used automatically if multiple sensor configs are given.
     :param update_rate:
         The update rate limit on the server. Defaults to None, not limiting the rate.
     :raises ValueError: If the session config must be extended but ``extended=False``.
     """
 
-    _groups: list[dict[int, SensorConfig]]
-
     def __init__(
         self,
         arg: Optional[
             Union[SensorConfig, dict[int, SensorConfig], list[dict[int, SensorConfig]]]
         ] = None,
         *,
         extended: Optional[bool] = None,
```

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/configs/subsweep_config.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/configs/subsweep_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,16 @@
     """Subsweep configuration
 
     The subsweep config represents a 1-1 mapping to the RSS service subsweep config.
 
     Normally used as a part of the :attr:`SensorConfig`.
     """
 
+    MAX_HWAAS = 511
+
     _start_point: int = attrs.field(
         default=80,
         converter=int_converter,
     )
     _num_points: int = attrs.field(
         default=160,
         converter=int_converter,
@@ -226,16 +228,17 @@
 
         return self._step_length
 
     @step_length.setter
     def step_length(self, value: int) -> None:
         self._step_length = value
 
+    @staticmethod
     @_step_length.validator
-    def _(self, _: t.Any, step_length: int) -> None:
+    def step_length_validator(instance: t.Any, _: t.Any, step_length: int) -> None:
         if not (
             is_divisor_of(SPARSE_IQ_PPC, step_length) or is_multiple_of(SPARSE_IQ_PPC, step_length)
         ):
             raise ValueError(f"Step length must be a divisor or multiple of {SPARSE_IQ_PPC}")
 
     @property
     def profile(self) -> Profile:
```

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/configs/validation_error.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/configs/validation_error.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/containers/__init__.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/containers/client_info.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/containers/client_info.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/containers/metadata.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/containers/metadata.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/containers/record.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/containers/record.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/containers/result.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/containers/result.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/containers/sensor_calibration.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/containers/sensor_calibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/containers/server_info.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/containers/server_info.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/containers/stacked_results.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/containers/stacked_results.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/containers/utils.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/entities/containers/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/mediators/link.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/mediators/link.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/mediators/recorder.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/mediators/recorder.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/client.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/common_client.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/common_client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/communication_protocol.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/communication_protocol.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_client.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_factory.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_factory.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_latest.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_latest.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_15_6_mhz.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_15_6_mhz.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_5_2_mhz.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_5_2_mhz.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_calibration_reuse.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_calibration_reuse.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/__init__.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/erroneus_message.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/erroneus_message.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/log_message.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/log_message.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/result_message.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/result_message.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/sensor_info_response.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/sensor_info_response.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/set_baudrate_response.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/set_baudrate_response.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/setup_response.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/setup_response.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/streaming_responses.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/streaming_responses.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/system_info_response.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/system_info_response.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/links.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/links.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/message.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/message.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/mock_client.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/mock_client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/utils.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/communication/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/h5_record/record.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/record.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/h5_record/record_io.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/record_io.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/h5_record/recorder.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/recorder.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/h5_record/session_schema.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/session_schema.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/h5_record/utils.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/im_record/im_record.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/peripherals/im_record/im_record.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/utils.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     TypeVar,
     Union,
     overload,
 )
 
 import attrs
 import numpy as np
+import numpy.typing as npt
 import packaging.version
 
 
 S = TypeVar("S")
 T = TypeVar("T")
 U = TypeVar("U")
 
@@ -536,16 +537,46 @@
     return lines
 
 
 def indent_strs(strs: list[str], level: int) -> list[str]:
     return ["  " * level + s for s in strs]
 
 
+def ndarray_isclose(a: npt.ArrayLike, b: npt.ArrayLike) -> bool:
+    return bool(np.isclose(a, b).all())
+
+
+def _dict_wrapper(f: Callable[[S, T], bool]) -> Callable[[dict[U, S], dict[U, T]], bool]:
+    def wrapper(a: dict[U, S], b: dict[U, T]) -> bool:
+        if a.keys() != b.keys():
+            return False
+
+        for key in a:
+            if not f(a[key], b[key]):
+                return False
+
+        return True
+
+    return wrapper
+
+
+def _optional_wrapper(f: Callable[[S, T], bool]) -> Callable[[Optional[S], Optional[T]], bool]:
+    def wrapper(a: Optional[S], b: Optional[T]) -> bool:
+        if a is None or b is None:
+            return a is b
+        else:
+            return f(a, b)
+
+    return wrapper
+
+
 attrs_ndarray_eq = attrs.cmp_using(eq=np.array_equal)
-attrs_ndarray_isclose = attrs.cmp_using(eq=lambda a, b: bool(np.isclose(a, b).all()))
+attrs_ndarray_isclose = attrs.cmp_using(eq=ndarray_isclose)
+attrs_optional_ndarray_isclose = attrs.cmp_using(eq=_optional_wrapper(ndarray_isclose))
+attrs_dict_ndarray_isclose = attrs.cmp_using(eq=_dict_wrapper(ndarray_isclose))
 
 
 def no_dynamic_member_creation(cls: Type[T]) -> Type[T]:
     """
     Class annotation that prevents setting any attributes that does not exist
     after the object have been created (the __init__ function have executed).
     """
```

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core_ext/_replaying_client.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_core_ext/_replaying_client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_rate_calc.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/_rate_calc.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/__init__.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from ._utils import (
     APPROX_BASE_STEP_LENGTH_M,
     ENVELOPE_FWHM_M,
     NOISE_TEMPERATURE_MODEL_PARAMETER,
     PERCEIVED_WAVELENGTH,
     SIGNAL_TEMPERATURE_MODEL_PARAMETER,
     double_buffering_frame_filter,
+    exponential_smoothing_coefficient,
     find_peaks,
     get_approx_fft_vels,
     get_distance_filter_coeffs,
     get_distance_filter_edge_margin,
     get_distances_m,
     get_temperature_adjustment_factors,
     interpolate_peaks,
```

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/_base.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/_base.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/_plugins/_a121.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/_plugins/_a121.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/_plugins/_null_app_model.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/_plugins/_null_app_model.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/_plugins/_processor_main.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/_plugins/_processor_main.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/_plugins/processor/backend_plugin.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/_plugins/processor/backend_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/_plugins/processor/plot_plugin.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/_plugins/processor/plot_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/_plugins/processor/plugin.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/_plugins/processor/plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/_plugins/processor/view_plugin.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/_plugins/processor/view_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from acconeer.exptool import a121
 from acconeer.exptool.a121.algo._base import ProcessorConfigT
 from acconeer.exptool.a121.algo._plugins._a121 import A121ViewPluginBase
 from acconeer.exptool.app.new import (
     AppModel,
     AttrsConfigEditor,
-    GridGroupBox,
+    GroupBox,
     MiscErrorView,
     PidgetFactoryMapping,
     PluginState,
     SessionConfigEditor,
     SmartMetadataView,
     SmartPerfCalcView,
     icons,
@@ -46,28 +46,29 @@
         self.stop_button.clicked.connect(self._send_stop_request)
 
         self.start_button.setShortcut("space")
         self.start_button.setToolTip("Starts the session.\n\nShortcut: Space")
         self.stop_button.setShortcut("space")
         self.stop_button.setToolTip("Stops the session.\n\nShortcut: Space")
 
-        button_group = GridGroupBox("Controls", parent=self.sticky_widget)
+        button_group = GroupBox.grid("Controls", parent=self.sticky_widget)
         button_group.layout().addWidget(self.start_button, 0, 0)
         button_group.layout().addWidget(self.stop_button, 0, 1)
         sticky_layout.addWidget(button_group)
 
         self.metadata_view = SmartMetadataView(parent=self.scrolly_widget)
         scrolly_layout.addWidget(self.metadata_view)
 
         self.perf_calc_view = SmartPerfCalcView(parent=self.scrolly_widget)
         scrolly_layout.addWidget(self.perf_calc_view)
 
-        self.processor_config_editor = AttrsConfigEditor[ProcessorConfigT](
+        self.processor_config_editor = AttrsConfigEditor(
             title="Processor parameters",
             factory_mapping=self.get_pidget_mapping(),
+            config_type=self.get_processor_config_cls(),
             parent=self.scrolly_widget,
         )
         self.processor_config_editor.sig_update.connect(self._on_processor_config_update)
         scrolly_layout.addWidget(self.processor_config_editor)
 
         self.misc_error_view = MiscErrorView(self.scrolly_widget)
         scrolly_layout.addWidget(self.misc_error_view)
```

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/_utils.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -281,13 +281,27 @@
         delta_times[-1] = delta
 
     client.stop_session()
 
     return float(1.0 / np.nanmean(delta_times))
 
 
+def exponential_smoothing_coefficient(fs: float, time_constant: float) -> float:
+    """Calculate the exponential smoothing coefficient.
+
+    Typical usage:
+
+    y = y * coeff + x * (1 - coeff)
+
+    :param fs: Sampling frequency.
+    :param time_constant: Time constant.
+    """
+    dt = 1 / fs
+    return float(np.exp(-dt / time_constant))
+
+
 def _safe_ceil(x: float) -> float:
     """Perform safe ceil.
 
     Implementation of ceil function, compatible with float representation in C.
     """
     return float(f"{x:.16g}")
```

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/bilateration/_plugin.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/bilateration/_plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from acconeer.exptool.a121.algo.distance._detector import _load_algo_data
 from acconeer.exptool.a121.algo.distance._detector_plugin import ViewPlugin as DistanceViewPlugin
 from acconeer.exptool.app.new import (
     AppModel,
     AttrsConfigEditor,
     ConnectionState,
     GeneralMessage,
-    GridGroupBox,
+    GroupBox,
     HandledException,
     Message,
     PidgetFactoryMapping,
     PluginFamily,
     PluginGeneration,
     PluginPresetBase,
     PluginSpecBase,
@@ -466,39 +466,41 @@
 
         self.defaults_button = QPushButton(icons.RESTORE(), "Reset settings and calibrations")
         self.defaults_button.clicked.connect(self._send_defaults_request)
 
         self.message_box = QLabel(self.sticky_widget)
         self.message_box.setWordWrap(True)
 
-        button_group = GridGroupBox("Controls", parent=self.sticky_widget)
+        button_group = GroupBox.grid("Controls", parent=self.sticky_widget)
         button_group.layout().addWidget(self.start_button, 0, 0)
         button_group.layout().addWidget(self.stop_button, 0, 1)
         button_group.layout().addWidget(self.calibrate_detector_button, 1, 0, 1, -1)
         button_group.layout().addWidget(self.defaults_button, 3, 0, 1, -1)
         button_group.layout().addWidget(self.message_box, 4, 0, 1, -1)
 
         sticky_layout.addWidget(button_group)
 
-        sensor_selection_group = GridGroupBox("Sensor selection", parent=self.scrolly_widget)
+        sensor_selection_group = GroupBox.grid("Sensor selection", parent=self.scrolly_widget)
         self.two_sensor_id_editor = TwoSensorIdsEditor(name_label_texts=["Left", "Right"])
         sensor_selection_group.layout().addWidget(self.two_sensor_id_editor, 0, 0)
         scrolly_layout.addWidget(sensor_selection_group)
 
-        self.bilateration_config_editor = AttrsConfigEditor[ProcessorConfig](
+        self.bilateration_config_editor = AttrsConfigEditor(
             title="Bilateration parameters",
             factory_mapping=self._get_processor_pidget_mapping(),
+            config_type=ProcessorConfig,
             parent=self.scrolly_widget,
         )
         self.bilateration_config_editor.sig_update.connect(self._on_processor_config_update)
         scrolly_layout.addWidget(self.bilateration_config_editor)
 
-        self.config_editor = AttrsConfigEditor[DetectorConfig](
+        self.config_editor = AttrsConfigEditor(
             title="Distance detector parameters",
             factory_mapping=self._get_pidget_mapping(),
+            config_type=DetectorConfig,
             parent=self.scrolly_widget,
         )
         self.config_editor.sig_update.connect(self._on_config_update)
         scrolly_layout.addWidget(self.config_editor)
 
         self.two_sensor_id_editor.sig_update.connect(self._on_sensor_ids_update)
         self.sticky_widget.setLayout(sticky_layout)
```

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/bilateration/_processor.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/bilateration/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/breathing/_plugin.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/vibration/_plugin.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,31 @@
-# Copyright (c) Acconeer AB, 2022-2023
+# Copyright (c) Acconeer AB, 2023
 # All rights reserved
 
 from __future__ import annotations
 
-import time
 from enum import Enum, auto
 from typing import Callable, Type
 
 import numpy as np
 
-from PySide6.QtGui import QFont
 from PySide6.QtWidgets import QWidget
 
 import pyqtgraph as pg
 
 import acconeer.exptool as et
 from acconeer.exptool import a121
 from acconeer.exptool.a121.algo._plugins import (
     ProcessorBackendPluginBase,
     ProcessorPlotPluginBase,
     ProcessorPluginPreset,
     ProcessorViewPluginBase,
 )
-from acconeer.exptool.a121.algo.breathing import (
+from acconeer.exptool.a121.algo._utils import APPROX_BASE_STEP_LENGTH_M
+from acconeer.exptool.a121.algo.vibration import (
     Processor,
     ProcessorConfig,
     ProcessorResult,
     get_sensor_config,
 )
 from acconeer.exptool.app.new import (
     AppModel,
@@ -73,157 +72,142 @@
         return {
             "time_series_length": pidgets.IntPidgetFactory(
                 name_label_text="Time series length",
                 limits=(0, None),
             ),
             "lp_coeff": pidgets.FloatSliderPidgetFactory(
                 name_label_text="Time filtering coefficient",
+                suffix="",
                 limits=(0, 1),
                 decimals=2,
             ),
-            "min_freq": pidgets.FloatSliderPidgetFactory(
-                name_label_text="Lower frequency of bandpass filter",
-                limits=(0, 1.0),
+            "sensitivity": pidgets.FloatSliderPidgetFactory(
+                name_label_text="Threshold sensitivity",
+                suffix="dB",
+                limits=(0, 30),
                 decimals=1,
             ),
-            "max_freq": pidgets.FloatSliderPidgetFactory(
-                name_label_text="Upper frequency of bandpass filter",
-                limits=(2.0, 10.0),
-                decimals=1,
+            "amplitude_threshold": pidgets.FloatPidgetFactory(
+                name_label_text="Minimum amplitude",
+                decimals=0,
+                limits=(0, None),
             ),
         }
 
     @classmethod
     def get_processor_config_cls(cls) -> Type[ProcessorConfig]:
         return ProcessorConfig
 
 
 class PlotPlugin(ProcessorPlotPluginBase[ProcessorResult]):
-
-    _TIME_SERIES_Y_SCALE_MARGIN_M = 0.0025
-    _DATA_INIT_DURATION = 5.0
-
     def __init__(self, *, plot_layout: pg.GraphicsLayout, app_model: AppModel) -> None:
         super().__init__(plot_layout=plot_layout, app_model=app_model)
 
     def setup(self, metadata: a121.Metadata, sensor_config: a121.SensorConfig) -> None:
 
-        pens = [et.utils.pg_pen_cycler(i) for i in range(5)]
+        self.meas_dist_m = sensor_config.start_point * APPROX_BASE_STEP_LENGTH_M
+
+        pen = et.utils.pg_pen_cycler(0)
         brush = et.utils.pg_brush_cycler(0)
+        brush_dot = et.utils.pg_brush_cycler(1)
         symbol_kw = dict(symbol="o", symbolSize=1, symbolBrush=brush, symbolPen="k")
-        feat_kws = [dict(pen=pen, **symbol_kw) for pen in pens]
+        feat_kw = dict(pen=pen, **symbol_kw)
+        symbol_dot_kw = dict(symbol="o", symbolSize=10, symbolBrush=brush_dot, symbolPen="k")
+
+        # presence plot
+        self.presence_plot = pg.PlotItem()
+        self.presence_plot.setMenuEnabled(False)
+        self.presence_plot.showGrid(x=False, y=True)
+        self.presence_plot.setLabel("left", "Max amplitude")
+        self.presence_plot.setLabel("bottom", "Distance (m)")
+        self.presence_plot.setXRange(self.meas_dist_m - 0.001, self.meas_dist_m + 0.001)
+        self.presence_curve = self.presence_plot.plot(**dict(pen=pen, **symbol_dot_kw))
+
+        self.presence_threshold = pg.InfiniteLine(pen=pen, angle=0)
+        self.presence_plot.addItem(self.presence_threshold)
+        self.presence_threshold.show()
 
-        font = QFont()
-        font.setPixelSize(16.0)
+        self.smooth_max_presence = et.utils.SmoothMax(tau_decay=10.0)
 
-        # time series plot
-        self.time_series_plot = self.plot_layout.addPlot(row=0, col=0)
+        # sweep and threshold plot
+        self.time_series_plot = pg.PlotItem()
         self.time_series_plot.setMenuEnabled(False)
         self.time_series_plot.showGrid(x=True, y=True)
-        self.time_series_plot.addLegend()
-        self.time_series_plot.setLabel("left", "Displacement (m)")
-        self.time_series_plot.setLabel("bottom", "Time")
-        self.time_series_plot.addItem(pg.PlotDataItem())
-        self.time_series_curve = []
-        self.time_series_curve.append(self.time_series_plot.plot(**feat_kws[0]))
-        self.time_series_curve.append(self.time_series_plot.plot(**feat_kws[1]))
+        self.time_series_plot.setLabel("left", "Displacement (mm)")
+        self.time_series_plot.setLabel("bottom", "History")
+        self.time_series_curve = self.time_series_plot.plot(**feat_kw)
+
+        sublayout = self.plot_layout.addLayout(row=0, col=0)
+        sublayout.layout.setColumnStretchFactor(1, 5)
+        sublayout.addItem(self.presence_plot, row=0, col=0)
+        sublayout.addItem(self.time_series_plot, row=0, col=1)
 
-        self.time_series_smooth_limits = et.utils.SmoothLimits()
-
-        self.time_series_text_item = pg.TextItem(
-            fill=pg.mkColor(0xFF, 0x7F, 0x0E, 200),
-            anchor=(0.5, 0),
-            color=pg.mkColor(0xFF, 0xFF, 0xFF, 200),
-        )
-        self.time_series_text_item.setFont(font)
-        self.time_series_text_item.show()
-        self.time_series_plot.addItem(self.time_series_text_item)
+        self.smooth_lim_time_series = et.utils.SmoothLimits(tau_decay=0.5, tau_grow=0.1)
 
-        # fft plot
-        self.fft_plot = self.plot_layout.addPlot(row=1, col=0)
+        self.fft_plot = self.plot_layout.addPlot(col=0, row=1)
         self.fft_plot.setMenuEnabled(False)
         self.fft_plot.showGrid(x=True, y=True)
-        self.fft_plot.addLegend()
-        self.fft_plot.setLabel("left", "Power")
+        self.fft_plot.setLabel("left", "Power (dB)")
         self.fft_plot.setLabel("bottom", "Frequency (Hz)")
         self.fft_plot.addItem(pg.PlotDataItem())
-        self.fft_curve = self.fft_plot.plot(**feat_kws[0])
-        self.fft_vert_line = pg.InfiniteLine(pen=pens[1])
-        self.fft_plot.addItem(self.fft_vert_line)
+        self.fft_curve = [
+            self.fft_plot.plot(**feat_kw),
+            self.fft_plot.plot(**dict(pen=pen, **symbol_dot_kw)),
+        ]
 
-        self.fft_smooth_max = et.utils.SmoothMax(tau_grow=0.5, tau_decay=2.0)
-
-        self.fft_text_item = pg.TextItem(
+        self.text_item = pg.TextItem(
             fill=pg.mkColor(0xFF, 0x7F, 0x0E, 200),
             anchor=(0.5, 0),
-            color=pg.mkColor(0xFF, 0xFF, 0xFF, 200),
         )
-        self.fft_text_item.setFont(font)
-        self.fft_text_item.show()
-        self.fft_plot.addItem(self.fft_text_item)
+        self.text_item.hide()
+        self.fft_plot.addItem(self.text_item)
 
-        self.start_time = time.time()
+        self.smooth_max_fft = et.utils.SmoothMax()
 
     def update(self, processor_result: ProcessorResult) -> None:
 
         time_series = processor_result.time_series
-        distance_to_analyze_m = processor_result.distance_to_analyze_m
-        z_abs_lp = processor_result.lp_psd
+        z_abs_db = processor_result.lp_z_abs_db
         freqs = processor_result.freqs
-        breathing_rate = processor_result.breathing_rate
-        fft_peak_location = processor_result.fft_peak_location
-
-        # time series plot
-        self.time_series_curve[0].setData(time_series)
-        lim = self.time_series_smooth_limits.update(time_series)
-
-        self.time_series_plot.setYRange(
-            lim[0] - self._TIME_SERIES_Y_SCALE_MARGIN_M,
-            lim[1] + self._TIME_SERIES_Y_SCALE_MARGIN_M,
-        )
-        text_y_pos = self.time_series_plot.getAxis("left").range[1] * 0.95
-        text_x_pos = self.time_series_plot.getAxis("bottom").range[1] / 2.0
-        self.time_series_text_item.setPos(text_x_pos, text_y_pos)
-        self.time_series_text_item.setHtml(
-            "Distance being visualized: " + "{:.2f}".format(distance_to_analyze_m) + " (m)"
-        )
-
-        # fft plot
-        if (time.time() - self.start_time) < self._DATA_INIT_DURATION:
-            self.fft_curve.setData(freqs, np.zeros_like(freqs))
-            self.fft_plot.setYRange(0.0, 1.0)
-
-            text_y_pos = self.fft_plot.getAxis("left").range[1] * 0.95
-            text_x_pos = self.fft_plot.getAxis("bottom").range[1] / 2.0
-            self.fft_text_item.setHtml("Acquiring data.")
-        elif freqs is not None:
-            assert z_abs_lp is not None
-            assert breathing_rate is not None
-            assert fft_peak_location is not None
-
-            self.fft_curve.setData(freqs, z_abs_lp)
-            self.fft_vert_line.setValue(fft_peak_location)
-            lim = self.fft_smooth_max.update(z_abs_lp)
-            self.fft_plot.setYRange(0.0, lim * 1.2)
-
-            text_y_pos = self.fft_plot.getAxis("left").range[1] * 0.95
-            text_x_pos = self.fft_plot.getAxis("bottom").range[1] / 2.0
-
-            self.fft_text_item.setHtml(
-                "Breathing rate: " + "{:.1f}".format(breathing_rate) + " per minute"
-            )
-        self.fft_text_item.setPos(text_x_pos, text_y_pos)
-
-    @staticmethod
-    def _format_string(string_to_display: str) -> str:
-        return (
-            '<div style="text-align: center">'
-            '<span style="color: #FFFFFF;font-size:15pt;">'
-            "{}</span></div>".format(string_to_display)
-        )
+        max_amplitude = processor_result.max_amplitude
+        amplitude_threshold = processor_result.amplitude_threshold
+        max_psd_ampl = processor_result.max_psd_ampl
+        max_psd_ampl_freq = processor_result.max_psd_ampl_freq
+
+        # plot object presence metric.
+        self.presence_curve.setData([self.meas_dist_m], [max_amplitude])
+        self.presence_threshold.setValue(amplitude_threshold)
+        lim = self.smooth_max_presence.update(max_amplitude)
+        self.presence_plot.setYRange(0, max(1000.0, lim))
+
+        if processor_result.result_available:
+            # plot time series and psd as object is present.
+            self.time_series_curve.setData(time_series)
+            lim = self.smooth_lim_time_series.update(time_series)
+            self.time_series_plot.setYRange(lim[0], lim[1])
+
+            assert z_abs_db is not None
+            self.fft_curve[0].setData(freqs, z_abs_db)
+            lim = self.smooth_max_fft.update(np.max(z_abs_db))
+            self.fft_plot.setYRange(0, lim)
+
+            if max_psd_ampl_freq is not None:
+                self.fft_curve[1].setData([max_psd_ampl_freq], [max_psd_ampl])
+                # Place text box centered at the top of the plotting window.
+                self.text_item.setPos(max(freqs) / 2, lim * 0.95)
+                html_format = (
+                    '<div style="text-align: center">'
+                    '<span style="color: #FFFFFF;font-size:15pt;">'
+                    "{}</span></div>".format("Detected Frequency: " + str(int(max_psd_ampl_freq)))
+                )
+                self.text_item.setHtml(html_format)
+                self.text_item.show()
+            else:
+                self.fft_curve[1].setData([], [])
+                self.text_item.hide()
 
 
 class PluginSpec(PluginSpecBase):
     def create_backend_plugin(
         self, callback: Callable[[Message], None], key: str
     ) -> BackendPlugin:
         return BackendPlugin(callback=callback, generation=self.generation, key=key)
@@ -233,18 +217,18 @@
 
     def create_plot_plugin(
         self, app_model: AppModel, plot_layout: pg.GraphicsLayout
     ) -> PlotPlugin:
         return PlotPlugin(app_model=app_model, plot_layout=plot_layout)
 
 
-BREATHING_PLUGIN = PluginSpec(
+VIBRATION_PLUGIN = PluginSpec(
     generation=PluginGeneration.A121,
-    key="breathing",
-    title="Breathing",
-    description="Measure breathing rate.",
+    key="vibration",
+    title="Vibration measurement",
+    description="Quantify the frequency content of vibrating object.",
     family=PluginFamily.EXAMPLE_APP,
     presets=[
         PluginPresetBase(name="Default", preset_id=PluginPresetId.DEFAULT),
     ],
     default_preset_id=PluginPresetId.DEFAULT,
 )
```

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/breathing/_processor.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/vibration/_processor.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,220 +1,229 @@
-# Copyright (c) Acconeer AB, 2022-2023
+# Copyright (c) Acconeer AB, 2023
 # All rights reserved
 
 from __future__ import annotations
 
 from typing import Optional
 
 import attrs
 import numpy as np
 import numpy.typing as npt
-from scipy import signal
 
 from acconeer.exptool import a121
 from acconeer.exptool.a121.algo import (
     APPROX_BASE_STEP_LENGTH_M,
     AlgoProcessorConfigBase,
     ProcessorBase,
+    double_buffering_frame_filter,
 )
 
 
 @attrs.mutable(kw_only=True)
 class ProcessorConfig(AlgoProcessorConfigBase):
     time_series_length: int = attrs.field(default=1024)
     """Length of time series."""
 
-    lp_coeff: float = attrs.field(default=0.75)
-    """Specify filter coefficient for exponential filter of psd over time."""
+    lp_coeff: float = attrs.field(default=0.95)
+    """Specify filter coefficient of exponential filter."""
 
-    min_freq: float = attrs.field(default=0.2)
-    """Lower limit of bandpass filter."""
+    sensitivity: float = attrs.field(default=10.0)
+    """Specify threshold sensitivity."""
 
-    max_freq: float = attrs.field(default=3.0)
-    """Upper limit of bandpass filter."""
+    amplitude_threshold: float = attrs.field(default=100.0)
+    """Specify minimum amplitude for calculating vibration."""
 
     def _collect_validation_results(
         self, config: a121.SessionConfig
     ) -> list[a121.ValidationResult]:
         validation_results: list[a121.ValidationResult] = []
 
-        if config.sensor_config.frame_rate is None:
+        if config.sensor_config.sweep_rate is None:
             validation_results.append(
                 a121.ValidationError(
                     config.sensor_config,
-                    "frame_rate",
+                    "sweep_rate",
                     "Must be set",
                 )
             )
 
-        if config.sensor_config.sweeps_per_frame != 1:
+        if config.sensor_config.num_points != 1:
+            validation_results.append(
+                a121.ValidationError(
+                    config.sensor_config.subsweep,
+                    "num_points",
+                    "Must be set to 1",
+                )
+            )
+
+        if not config.sensor_config.double_buffering:
             validation_results.append(
                 a121.ValidationError(
                     config.sensor_config,
-                    "sweeps_per_frame",
-                    "Must be equal to 1",
+                    "double_buffering",
+                    "Must be enabled",
+                )
+            )
+
+        if not config.sensor_config.continuous_sweep_mode:
+            validation_results.append(
+                a121.ValidationError(
+                    config.sensor_config,
+                    "continuous_sweep_mode",
+                    "Must be enabled",
                 )
             )
 
         return validation_results
 
 
 @attrs.frozen(kw_only=True)
 class ProcessorContext:
     ...
 
 
 @attrs.frozen(kw_only=True)
 class ProcessorResult:
-    time_series: npt.NDArray[np.float_]
-    distance_to_analyze_m: float
+    result_available: bool
+    time_series: Optional[npt.NDArray[np.float_]] = attrs.field(default=None)
+    lp_z_abs_db: Optional[npt.NDArray[np.float_]] = attrs.field(default=None)
     freqs: npt.NDArray[np.float_]
-    lp_psd: Optional[npt.NDArray[np.float_]] = attrs.field(default=None)
-    breathing_rate: Optional[float] = attrs.field(default=None)
-    fft_peak_location: Optional[float] = attrs.field(default=None)
+    max_amplitude: float
+    amplitude_threshold: float
+    max_psd_ampl: Optional[float] = attrs.field(default=None)
+    max_psd_ampl_freq: Optional[float] = attrs.field(default=None)
 
 
 class Processor(ProcessorBase[ProcessorConfig, ProcessorResult]):
 
-    _IIR_INIT_LENGTH: int = 200
-    _OVER_SAMPLING_FACTOR: int = 5
-    _PHASE_TO_MM: float = APPROX_BASE_STEP_LENGTH_M / (np.pi * 2.0)
-    _SECONDS_PER_MINUTE: float = 60.0
-    _SECONDS_PER_FFT_WINDOW: float = 10.0
-    _AMPL_LP_COEFF: float = 0.99
+    _OVER_SAMPLING_FACTOR = 2
+    _WINDOW_BASE_LENGTH = 10
+    _HALF_GUARD_BASE_LENGTH = 5
 
     def __init__(
         self,
         *,
         sensor_config: a121.SensorConfig,
         metadata: a121.Metadata,
         processor_config: ProcessorConfig,
         subsweep_indexes: Optional[list[int]] = None,
         context: Optional[ProcessorContext] = None,
     ) -> None:
+
         processor_config.validate(sensor_config)
 
-        assert sensor_config.frame_rate is not None
-        self.frame_rate = sensor_config.frame_rate
-        self.start_point = sensor_config.start_point
-        self.step_length = sensor_config.step_length
-        self.spf = sensor_config.sweeps_per_frame
+        # Should never happen, checked in validate
+        assert sensor_config.sweep_rate is not None
 
-        self.time_series_len = processor_config.time_series_length
-        self.max_freq = processor_config.max_freq
-        self.lp_coeff = processor_config.lp_coeff
-
-        self.time_series = np.zeros(
-            shape=(
-                processor_config.time_series_length + self._IIR_INIT_LENGTH,
-                sensor_config.num_points,
-            )
-        )
+        self.double_buffering = sensor_config.double_buffering
+        self.spf = sensor_config.sweeps_per_frame
+        self.lp_coeffs = processor_config.lp_coeff
+        self.sensitivity = processor_config.sensitivity
+        self.time_series_length = processor_config.time_series_length
+        self.amplitude_threshold = processor_config.amplitude_threshold
+
+        self.time_series = np.zeros(shape=processor_config.time_series_length)
+        self.freq = np.fft.rfftfreq(
+            self._OVER_SAMPLING_FACTOR * processor_config.time_series_length,
+            1 / sensor_config.sweep_rate,
+        )[1:]
+        self.lp_z_abs_db = np.zeros_like(self.freq)
+        self.window_length = self._WINDOW_BASE_LENGTH * self._OVER_SAMPLING_FACTOR
+        self.half_guard_length = self._HALF_GUARD_BASE_LENGTH * self._OVER_SAMPLING_FACTOR
 
-        self.has_init = False
+    def process(self, result: a121.Result) -> ProcessorResult:
 
-        self.ampl_lp_filt = np.zeros(shape=sensor_config.num_points)
+        if self.double_buffering:
+            frame = double_buffering_frame_filter(result.frame)
+        else:
+            frame = result.frame
 
-        self.lp_psd = None
-        self.window_length = self._SECONDS_PER_FFT_WINDOW * self.frame_rate
-        (self.B, self.A) = signal.butter(
-            N=2,
-            Wn=[processor_config.min_freq, processor_config.max_freq],
-            fs=sensor_config.frame_rate,
-            btype="bandpass",
-        )
+        max_amplitude = float(np.max(np.abs(frame)))
 
-    def process(self, result: a121.Result) -> ProcessorResult:
-        # Add new data to fifo buffer, unwrap and filter.
-        self.time_series = np.roll(self.time_series, -self.spf, axis=0)
-        self.time_series[-self.spf :] = np.angle(result.frame)
-        time_series_unwrapped = np.unwrap(self.time_series, axis=0) * self._PHASE_TO_MM
-        time_series_filt = signal.lfilter(self.B, self.A, time_series_unwrapped, axis=0)[
-            self._IIR_INIT_LENGTH :
-        ]
-
-        # Filter amplitudes and determine at what distance to plot time series.
-        self.ampl_lp_filt = self._AMPL_LP_COEFF * self.ampl_lp_filt + (
-            1 - self._AMPL_LP_COEFF
-        ) * np.abs(result.frame)
-        distance_to_plot = np.argmax(self.ampl_lp_filt)
-        distance_to_plot_m = (
-            float(self.start_point + distance_to_plot * self.step_length)
-            * APPROX_BASE_STEP_LENGTH_M
-        )
+        if max_amplitude < self.amplitude_threshold:
+            return ProcessorResult(
+                result_available=False,
+                max_amplitude=max_amplitude,
+                amplitude_threshold=self.amplitude_threshold,
+                freqs=self.freq,
+            )
 
-        # Calculate psd.
-        freqs, psd = signal.welch(
-            x=time_series_filt,
-            fs=self.frame_rate,
-            window="hann",
-            nperseg=self.window_length,
-            nfft=self.time_series_len * self._OVER_SAMPLING_FACTOR,
-            axis=0,
-            average="mean",
-        )
+        new_data_segment = np.angle(frame.squeeze(axis=1))
 
-        # Weigh psd with filtered amplitude and psd over distances.
-        psd = np.mean(psd * self.ampl_lp_filt, axis=1)
+        self.time_series = np.roll(self.time_series, -self.spf)
+        self.time_series[-self.spf :] = new_data_segment
+        self.time_series = np.unwrap(self.time_series)
 
-        if not self.has_init:
-            self.lp_psd = psd
-            self.ampl_lp_filt = np.abs(result.frame)
-            self.has_init = True
-
-        assert self.lp_psd is not None
-        self.lp_psd = self.lp_psd * self.lp_coeff + psd * (1 - self.lp_coeff)
-
-        idx_to_analyze = np.where(freqs < self.max_freq)[0]
-        freqs_to_analyze = freqs[idx_to_analyze]
-        psd_to_analyze = self.lp_psd[idx_to_analyze]
-        fft_peak_loc_idx = np.argmax(psd_to_analyze)
-
-        # Make sure max value is not first or last element in psd.
-        if (fft_peak_loc_idx != 0) & (fft_peak_loc_idx != (freqs_to_analyze.shape[0] - 1)):
-            fft_interpolated_freq = self.interpolate_peaks(
-                psd_to_analyze[fft_peak_loc_idx - 1 : fft_peak_loc_idx + 2],
-                freqs_to_analyze[fft_peak_loc_idx - 1 : fft_peak_loc_idx + 2],
+        z_abs = np.abs(
+            np.fft.rfft(
+                self.time_series - np.mean(self.time_series),
+                n=self.time_series_length * self._OVER_SAMPLING_FACTOR,
             )
-            breathing_rate = fft_interpolated_freq * self._SECONDS_PER_MINUTE
+        )[1:]
+        z_abs_db = 20 * np.log10(z_abs)
+        self.lp_z_abs_db = self.lp_z_abs_db * self.lp_coeffs + z_abs_db * (1 - self.lp_coeffs)
 
-            return ProcessorResult(
-                time_series=time_series_filt[:, distance_to_plot],
-                distance_to_analyze_m=distance_to_plot_m,
-                lp_psd=psd_to_analyze,
-                freqs=freqs_to_analyze,
-                breathing_rate=breathing_rate,
-                fft_peak_location=fft_interpolated_freq,
-            )
+        presented_time_series = (
+            (self.time_series - np.mean(self.time_series)) * APPROX_BASE_STEP_LENGTH_M * 1000
+        )
 
+        threshold = self._calculate_cfar_threshold(
+            self.lp_z_abs_db, self.sensitivity, self.window_length, self.half_guard_length
+        )
+        # Find index of values over threshold
+        idx_over_threshold = np.where(threshold < self.lp_z_abs_db)[0]
+        if idx_over_threshold.shape[0] != 0:
+            psd_ampls_over_threshold = self.lp_z_abs_db[idx_over_threshold]
+            max_psd_ampl = np.max(psd_ampls_over_threshold)
+            max_psd_ampl_freq = self.freq[idx_over_threshold[np.argmax(psd_ampls_over_threshold)]]
         else:
-            return ProcessorResult(
-                time_series=time_series_filt[:, distance_to_plot],
-                distance_to_analyze_m=distance_to_plot_m,
-                freqs=freqs_to_analyze,
-            )
+            max_psd_ampl = None
+            max_psd_ampl_freq = None
 
-    @staticmethod
-    def interpolate_peaks(ampls: npt.NDArray[np.float_], freqs: npt.NDArray[np.float_]) -> float:
-        x = freqs
-        y = ampls
-        a = (x[0] * (y[2] - y[1]) + x[1] * (y[0] - y[2]) + x[2] * (y[1] - y[0])) / (
-            (x[0] - x[1]) * (x[0] - x[2]) * (x[1] - x[2])
+        return ProcessorResult(
+            result_available=True,
+            time_series=presented_time_series,
+            lp_z_abs_db=self.lp_z_abs_db,
+            freqs=self.freq,
+            max_amplitude=max_amplitude,
+            amplitude_threshold=self.amplitude_threshold,
+            max_psd_ampl=max_psd_ampl,
+            max_psd_ampl_freq=max_psd_ampl_freq,
         )
-        b = (y[1] - y[0]) / (x[1] - x[0]) - a * (x[0] + x[1])
-        return float(-b / (2 * a))
+
+    @staticmethod
+    def _calculate_cfar_threshold(
+        psd: npt.NDArray[np.float_],
+        sensitivity: float,
+        window_length: int,
+        half_guard_length: int,
+    ) -> npt.NDArray[np.float_]:
+        threshold = np.full(psd.shape, np.nan)
+        margin = window_length + half_guard_length
+        length_after_filtering = psd.shape[0] - 2 * margin
+
+        filt_psd = np.convolve(psd, np.ones(window_length), "valid") / window_length
+        threshold[margin:-margin] = (
+            filt_psd[:length_after_filtering] + filt_psd[-length_after_filtering:]
+        ) / 2 + sensitivity
+
+        return threshold
 
     def update_config(self, config: ProcessorConfig) -> None:
         ...
 
 
 def get_sensor_config() -> a121.SensorConfig:
     return a121.SensorConfig(
         profile=a121.Profile.PROFILE_3,
         hwaas=16,
-        num_points=10,
-        step_length=24,
-        start_point=150,
-        receiver_gain=12,
-        sweeps_per_frame=1,
-        frame_rate=50,
+        num_points=1,
+        step_length=1,
+        start_point=80,
+        receiver_gain=10,
+        sweep_rate=2000,
+        sweeps_per_frame=50,
+        double_buffering=True,
+        continuous_sweep_mode=True,
+        inter_frame_idle_state=a121.IdleState.READY,
+        inter_sweep_idle_state=a121.IdleState.READY,
     )
```

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/distance/__main__.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/distance/__main__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/distance/_aggregator.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/distance/_aggregator.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/distance/_detector.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/distance/_detector.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/distance/_detector_plugin.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/distance/_detector_plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) Acconeer AB, 2022-2023
 # All rights reserved
 
 from __future__ import annotations
 
 import logging
 from enum import Enum, auto
-from typing import Callable, Mapping, Optional, cast
+from typing import Any, Callable, Mapping, Optional, cast
 
 import attrs
 import h5py
 import numpy as np
 
 from PySide6.QtWidgets import QLabel, QPushButton, QTabWidget, QVBoxLayout, QWidget
 
@@ -24,36 +24,36 @@
     DetectorViewPluginBase,
 )
 from acconeer.exptool.app.new import (
     AppModel,
     AttrsConfigEditor,
     BackendLogger,
     GeneralMessage,
-    GridGroupBox,
+    GroupBox,
     HandledException,
     Message,
     MiscErrorView,
     PidgetFactoryMapping,
     PluginFamily,
     PluginGeneration,
     PluginPresetBase,
     PluginSpecBase,
     PluginState,
     PluginStateMessage,
-    VerticalGroupBox,
     icons,
     is_task,
     pidgets,
 )
 from acconeer.exptool.app.new.ui.plugin_components import CollapsibleWidget, SensorConfigEditor
 from acconeer.exptool.app.new.ui.plugin_components.pidgets.hooks import (
     disable_if,
     enable_if,
     parameter_is,
 )
+from acconeer.exptool.app.new.ui.plugin_components.save_dialog import PresentationType
 
 from ._configs import get_high_accuracy_detector_config
 from ._detector import (
     DetailedStatus,
     Detector,
     DetectorConfig,
     DetectorContext,
@@ -347,37 +347,39 @@
 
         self.defaults_button = QPushButton(icons.RESTORE(), "Reset settings and calibrations")
         self.defaults_button.clicked.connect(self._send_defaults_request)
 
         self.message_box = QLabel(self.sticky_widget)
         self.message_box.setWordWrap(True)
 
-        button_group = GridGroupBox("Controls", parent=self.sticky_widget)
+        button_group = GroupBox.grid("Controls", parent=self.sticky_widget)
         button_group.layout().addWidget(self.start_button, 0, 0)
         button_group.layout().addWidget(self.stop_button, 0, 1)
         button_group.layout().addWidget(self.calibrate_detector_button, 1, 0, 1, -1)
         button_group.layout().addWidget(self.defaults_button, 3, 0, 1, -1)
         button_group.layout().addWidget(self.message_box, 4, 0, 1, -1)
 
         sticky_layout.addWidget(button_group)
 
         self.misc_error_view = MiscErrorView(self.scrolly_widget)
         scrolly_layout.addWidget(self.misc_error_view)
 
-        sensor_selection_group = VerticalGroupBox("Sensor selection", parent=self.scrolly_widget)
+        sensor_selection_group = GroupBox.vertical("Sensor selection", parent=self.scrolly_widget)
         self.sensor_id_pidget = pidgets.SensorIdPidgetFactory(items=[]).create(
             parent=sensor_selection_group
         )
         self.sensor_id_pidget.sig_update.connect(self._on_sensor_id_update)
         sensor_selection_group.layout().addWidget(self.sensor_id_pidget)
         scrolly_layout.addWidget(sensor_selection_group)
 
-        self.config_editor = AttrsConfigEditor[DetectorConfig](
+        self.config_editor = AttrsConfigEditor(
             title="Detector parameters",
             factory_mapping=self.get_pidget_mapping(),
+            config_type=DetectorConfig,
+            extra_presenter=_detector_config_presenter,
             parent=self.scrolly_widget,
         )
         self.config_editor.sig_update.connect(self._on_config_update)
         scrolly_layout.addWidget(self.config_editor)
 
         self.sensor_config_editor_tabs = QTabWidget()
         self.sensor_config_editor_tabs.setStyleSheet("QTabWidget::pane { padding: 5px;}")
@@ -580,14 +582,49 @@
     def _on_calibrate_detector(self) -> None:
         BackendPlugin.calibrate_detector.rpc(self.app_model.put_task)
 
     def _send_defaults_request(self) -> None:
         BackendPlugin.restore_defaults.rpc(self.app_model.put_task)
 
 
+def _detector_config_presenter(config: Any, presentation_type: PresentationType) -> Optional[str]:
+    if isinstance(config, DetectorConfig) and presentation_type is PresentationType.C_SET_CONFIG:
+        max_step_length = 0 if config.max_step_length is None else config.max_step_length
+
+        return f"""
+static void set_config(acc_detector_distance_config_t *config, distance_preset_config_t preset)
+{{
+    // This snippet is generated to be compatible with RSS A121 v1.0.0
+    // If there is a version missmatch the snippet might need some modification
+
+    (void)preset;
+
+    acc_detector_distance_config_sensor_set(config, SENSOR_ID);
+
+    acc_detector_distance_config_start_set(config, {config.start_m:.3f}f);
+    acc_detector_distance_config_end_set(config, {config.end_m:.3f}f);
+    acc_detector_distance_config_max_step_length_set(config, {max_step_length}U);
+
+    acc_detector_distance_config_signal_quality_set(config, {float(config.signal_quality):.3f}f);
+    acc_detector_distance_config_max_profile_set(config, ACC_CONFIG_{config.max_profile.name});
+    acc_detector_distance_config_peak_sorting_set(config, ACC_DETECTOR_DISTANCE_PEAK_SORTING_{config.peaksorting_method.name});
+    acc_detector_distance_config_reflector_shape_set(config, ACC_DETECTOR_DISTANCE_REFLECTOR_SHAPE_{config.reflector_shape.name});
+
+    acc_detector_distance_config_threshold_method_set(config, ACC_DETECTOR_DISTANCE_THRESHOLD_METHOD_{config.threshold_method.name});
+    acc_detector_distance_config_num_frames_recorded_threshold_set(config, {config.num_frames_in_recorded_threshold}U);
+    acc_detector_distance_config_fixed_threshold_value_set(config, {config.fixed_threshold_value:.3f}f);
+    acc_detector_distance_config_threshold_sensitivity_set(config, {config.threshold_sensitivity:.3f}f);
+
+    acc_detector_distance_config_close_range_leakage_cancellation_set(config, {str(config.close_range_leakage_cancellation).lower()});
+}}
+"""
+
+    return None
+
+
 class PluginSpec(PluginSpecBase):
     def create_backend_plugin(
         self, callback: Callable[[Message], None], key: str
     ) -> BackendPlugin:
         return BackendPlugin(callback, generation=self.generation, key=key)
 
     def create_view_plugin(self, app_model: AppModel, view_widget: QWidget) -> ViewPlugin:
```

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/distance/_processors.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/distance/_processors.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/distance/_serializers.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/distance/_serializers.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/phase_tracking/_plugin.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/phase_tracking/_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/phase_tracking/_processor.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/phase_tracking/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/presence/_configs.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/presence/_configs.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/presence/_detector.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/presence/_detector.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,21 @@
 import numpy as np
 import numpy.typing as npt
 
 from acconeer.exptool import a121
 from acconeer.exptool.a121._core.entities.configs.config_enums import IdleState, Profile
 from acconeer.exptool.a121._core.utils import is_divisor_of, is_multiple_of
 from acconeer.exptool.a121._h5_utils import _create_h5_string_dataset
-from acconeer.exptool.a121.algo import ENVELOPE_FWHM_M, AlgoConfigBase, Controller, select_prf
+from acconeer.exptool.a121.algo import (
+    ENVELOPE_FWHM_M,
+    AlgoBase,
+    AlgoConfigBase,
+    Controller,
+    select_prf,
+)
 from acconeer.exptool.a121.algo._utils import estimate_frame_rate
 
 from ._processors import Processor, ProcessorConfig, ProcessorContext, ProcessorExtraResult
 
 
 SPARSE_IQ_PPC = 24
 
@@ -139,14 +145,19 @@
                     f"Must be greater than {Processor.NOISE_ESTIMATION_DIFF_ORDER}",
                 )
             )
 
         return validation_results
 
 
+@attrs.mutable(kw_only=True)
+class DetectorContext(AlgoBase):
+    estimated_frame_rate: float = attrs.field(default=None)
+
+
 @attrs.frozen(kw_only=True)
 class DetectorMetadata:
     start_m: float = attrs.field()
     """Actual start point of measurement in meters"""
 
     step_length_m: float = attrs.field()
     """Actual step length between each data point of the measurement in meters"""
@@ -193,42 +204,52 @@
 
     def __init__(
         self,
         *,
         client: a121.Client,
         sensor_id: int,
         detector_config: DetectorConfig,
+        detector_context: Optional[DetectorContext] = None,
     ) -> None:
         super().__init__(client=client, config=detector_config)
         self.sensor_id = sensor_id
         self.detector_metadata: Optional[DetectorMetadata] = None
+        self.detector_context = detector_context
 
         self.started = False
 
     def start(
-        self, recorder: Optional[a121.Recorder] = None, _algo_group: Optional[h5py.Group] = None
+        self,
+        recorder: Optional[a121.Recorder] = None,
+        _algo_group: Optional[h5py.Group] = None,
     ) -> None:
         if self.started:
             raise RuntimeError("Already started")
 
         sensor_config = self._get_sensor_config(self.config)
         self.session_config = a121.SessionConfig(
             {self.sensor_id: sensor_config},
             extended=False,
         )
 
-        self.estimated_frame_rate = estimate_frame_rate(self.client, self.session_config)
-        # Add estimated frame rate to context if it differs more than 10% from the set frame rate
+        if self.detector_context is None:
+            self.estimated_frame_rate = estimate_frame_rate(self.client, self.session_config)
+            self.detector_context = DetectorContext(estimated_frame_rate=self.estimated_frame_rate)
+        else:
+            self.estimated_frame_rate = self.detector_context.estimated_frame_rate
+
+        # Add estimated frame rate to context if it differs more than
+        # 10% from the set frame rate
         if (
             np.abs(self.config.frame_rate - self.estimated_frame_rate) / self.config.frame_rate
             > 0.1
         ):
-            context = ProcessorContext(estimated_frame_rate=self.estimated_frame_rate)
+            processor_context = ProcessorContext(estimated_frame_rate=self.estimated_frame_rate)
         else:
-            context = ProcessorContext(estimated_frame_rate=None)
+            processor_context = ProcessorContext(estimated_frame_rate=None)
 
         metadata = self.client.setup_session(self.session_config)
         assert isinstance(metadata, a121.Metadata)
 
         processor_config = self._get_processor_config(self.config)
 
         self.detector_metadata = DetectorMetadata(
@@ -238,25 +259,26 @@
             profile=sensor_config.profile,
         )
 
         self.processor = Processor(
             sensor_config=sensor_config,
             metadata=metadata,
             processor_config=processor_config,
-            context=context,
+            context=processor_context,
         )
 
         if recorder is not None:
             if isinstance(recorder, a121.H5Recorder):
                 if _algo_group is None:
                     _algo_group = recorder.require_algo_group("presence_detector")
                 _record_algo_data(
                     _algo_group,
                     self.sensor_id,
                     self.config,
+                    self.detector_context,
                 )
             else:
                 # Should never happen as we currently only have the H5Recorder
                 warnings.warn("Will not save algo data")
 
             self.client.attach_recorder(recorder)
 
@@ -363,20 +385,29 @@
         return recorder_result
 
 
 def _record_algo_data(
     algo_group: h5py.Group,
     sensor_id: int,
     config: DetectorConfig,
+    context: DetectorContext,
 ) -> None:
     algo_group.create_dataset(
         "sensor_id",
         data=sensor_id,
         track_times=False,
     )
     _create_h5_string_dataset(algo_group, "detector_config", config.to_json())
+    _create_h5_string_dataset(algo_group, "detector_context", context.to_json())
 
 
-def _load_algo_data(algo_group: h5py.Group) -> Tuple[int, DetectorConfig]:
+def _load_algo_data(
+    algo_group: h5py.Group,
+) -> Tuple[int, DetectorConfig, Optional[DetectorContext]]:
     sensor_id = algo_group["sensor_id"][()]
     config = DetectorConfig.from_json(algo_group["detector_config"][()])
-    return sensor_id, config
+    context_data_set = algo_group.get("detector_context")
+    if context_data_set is None:
+        context = None
+    else:
+        context = DetectorContext.from_json(context_data_set[()])
+    return sensor_id, config, context
```

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/presence/_detector_plugin.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/smart_presence/_ref_app_plugin.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Acconeer AB, 2022-2023
+# Copyright (c) Acconeer AB, 2023
 # All rights reserved
 
 from __future__ import annotations
 
 import logging
 from enum import Enum, auto
 from typing import Callable, Mapping, Optional
@@ -15,396 +15,389 @@
 from PySide6.QtWidgets import QPushButton, QVBoxLayout, QWidget
 
 import pyqtgraph as pg
 
 import acconeer.exptool as et
 from acconeer.exptool import a121
 from acconeer.exptool.a121._h5_utils import _create_h5_string_dataset
+from acconeer.exptool.a121.algo._base import AlgoBase
 from acconeer.exptool.a121.algo._plugins import (
     DetectorBackendPluginBase,
     DetectorPlotPluginBase,
     DetectorViewPluginBase,
 )
+from acconeer.exptool.a121.algo.presence._detector import Detector
+from acconeer.exptool.a121.algo.presence._detector_plugin import ViewPlugin as PresenceViewPlugin
 from acconeer.exptool.app.new import (
     AppModel,
     AttrsConfigEditor,
     BackendLogger,
     GeneralMessage,
-    GridGroupBox,
+    GroupBox,
     Message,
     MiscErrorView,
     PidgetGroupFactoryMapping,
     PluginFamily,
     PluginGeneration,
     PluginPresetBase,
     PluginSpecBase,
     PluginState,
-    VerticalGroupBox,
     icons,
     is_task,
     pidgets,
 )
-from acconeer.exptool.app.new.ui.plugin_components.pidgets.hooks import disable_if, parameter_is
 
 from ._configs import get_long_range_config, get_medium_range_config, get_short_range_config
-from ._detector import Detector, DetectorConfig, DetectorMetadata, DetectorResult, _load_algo_data
+from ._ref_app import RefApp, RefAppConfig, RefAppResult, _load_algo_data
+
+
+@attrs.mutable(kw_only=True)
+class PlotConfig(AlgoBase):
+    show_all_detected_zones: bool = attrs.field(default=False)
 
 
 @attrs.mutable(kw_only=True)
 class SharedState:
     sensor_id: int = attrs.field(default=1)
-    config: DetectorConfig = attrs.field(factory=DetectorConfig)
+    config: RefAppConfig = attrs.field(factory=RefAppConfig)
+    plot_config: PlotConfig = attrs.field(factory=PlotConfig)
 
 
 class PluginPresetId(Enum):
     SHORT_RANGE = auto()
     MEDIUM_RANGE = auto()
     LONG_RANGE = auto()
 
 
 class BackendPlugin(DetectorBackendPluginBase[SharedState]):
-    PLUGIN_PRESETS: Mapping[int, Callable[[], DetectorConfig]] = {
+
+    PLUGIN_PRESETS: Mapping[int, Callable[[], RefAppConfig]] = {
         PluginPresetId.SHORT_RANGE.value: lambda: get_short_range_config(),
         PluginPresetId.MEDIUM_RANGE.value: lambda: get_medium_range_config(),
         PluginPresetId.LONG_RANGE.value: lambda: get_long_range_config(),
     }
 
     def __init__(
         self, callback: Callable[[Message], None], generation: PluginGeneration, key: str
     ) -> None:
         super().__init__(callback=callback, generation=generation, key=key)
 
         self._recorder: Optional[a121.H5Recorder] = None
-        self._detector_instance: Optional[Detector] = None
+        self._ref_app_instance: Optional[RefApp] = None
         self._log = BackendLogger.getLogger(__name__)
 
         self.restore_defaults()
 
     def _load_from_cache(self, file: h5py.File) -> None:
-        self.shared_state.config = DetectorConfig.from_json(file["config"][()])
+        self.shared_state.config = RefAppConfig.from_json(file["config"][()])
+        self.shared_state.plot_config = PlotConfig.from_json(file["plot_config"][()])
+
+        show_all_detected_zones = self.shared_state.plot_config.show_all_detected_zones
+        self.shared_state.config.show_all_detected_zones = show_all_detected_zones
 
     @is_task
     def restore_defaults(self) -> None:
         self.shared_state = SharedState()
         self.broadcast()
 
     @is_task
     def update_sensor_id(self, *, sensor_id: int) -> None:
         self.shared_state.sensor_id = sensor_id
         self.broadcast()
 
+    @is_task
+    def update_plot_config(self, *, config: PlotConfig) -> None:
+        self.shared_state.plot_config = config
+        self.broadcast()
+
     def _sync_sensor_ids(self) -> None:
         if self.client is not None:
             sensor_ids = self.client.server_info.connected_sensors
 
             if len(sensor_ids) > 0 and self.shared_state.sensor_id not in sensor_ids:
                 self.shared_state.sensor_id = sensor_ids[0]
 
     @is_task
-    def update_config(self, *, config: DetectorConfig) -> None:
+    def update_config(self, *, config: RefAppConfig) -> None:
         self.shared_state.config = config
         self.broadcast()
 
     def save_to_cache(self, file: h5py.File) -> None:
         _create_h5_string_dataset(file, "config", self.shared_state.config.to_json())
+        _create_h5_string_dataset(file, "plot_config", self.shared_state.plot_config.to_json())
 
     @is_task
     def set_preset(self, preset_id: int) -> None:
         preset_config = self.PLUGIN_PRESETS[preset_id]
         self.shared_state.config = preset_config()
+        self.shared_state.plot_config = PlotConfig()
         self.broadcast()
 
     def load_from_record_setup(self, *, record: a121.H5Record) -> None:
         algo_group = record.get_algo_group(self.key)
         _, config = _load_algo_data(algo_group)
         self.shared_state.config = config
         self.shared_state.sensor_id = record.sensor_id
 
     def _start_session(self, recorder: Optional[a121.H5Recorder]) -> None:
         assert self.client
-        self._detector_instance = Detector(
+        self._ref_app_instance = RefApp(
             client=self.client,
             sensor_id=self.shared_state.sensor_id,
-            detector_config=self.shared_state.config,
+            ref_app_config=self.shared_state.config,
         )
-        self._detector_instance.start(recorder)
+        self._ref_app_instance.start(recorder)
         self.callback(
             GeneralMessage(
                 name="setup",
                 kwargs=dict(
-                    detector_config=self.shared_state.config,
-                    detector_metadata=self._detector_instance.detector_metadata,
-                    estimated_frame_rate=self._detector_instance.estimated_frame_rate,
+                    ref_app_config=self.shared_state.config,
+                    sensor_config=Detector._get_sensor_config(
+                        self._ref_app_instance.detector.config
+                    ),
+                    plot_config=self.shared_state.plot_config,
+                    estimated_frame_rate=self._ref_app_instance.detector.estimated_frame_rate,
                 ),
                 recipient="plot_plugin",
             )
         )
 
     def end_session(self) -> None:
-        if self._detector_instance is None:
+        if self._ref_app_instance is None:
             raise RuntimeError
         if self._recorder is not None:
             self._recorder.close()
-        self._detector_instance.stop()
+        self._ref_app_instance.stop()
 
     def get_next(self) -> None:
         assert self.client
-        if self._detector_instance is None:
+        if self._ref_app_instance is None:
             raise RuntimeError
-        result = self._detector_instance.get_next()
+        result = self._ref_app_instance.get_next()
 
         self.callback(GeneralMessage(name="plot", data=result, recipient="plot_plugin"))
 
 
 class PlotPlugin(DetectorPlotPluginBase):
     def __init__(self, *, plot_layout: pg.GraphicsLayout, app_model: AppModel) -> None:
         super().__init__(plot_layout=plot_layout, app_model=app_model)
 
     def setup_from_message(self, message: GeneralMessage) -> None:
         assert message.kwargs is not None
         self.setup(**message.kwargs)
 
     def update_from_message(self, message: GeneralMessage) -> None:
-        assert isinstance(message.data, DetectorResult)
+        assert isinstance(message.data, RefAppResult)
         self.update(message.data)
 
     def setup(
         self,
-        detector_config: DetectorConfig,
-        detector_metadata: DetectorMetadata,
+        ref_app_config: RefAppConfig,
+        sensor_config: a121.SensorConfig,
+        plot_config: PlotConfig,
         estimated_frame_rate: float,
     ) -> None:
-        self.detector_config = detector_config
+        self.ref_app_config = ref_app_config
         self.distances = np.linspace(
-            detector_metadata.start_m,
-            detector_config.end_m,
-            detector_metadata.num_points,
+            ref_app_config.start_m, ref_app_config.end_m, sensor_config.num_points
         )
 
+        self.show_all_detected_zones = plot_config.show_all_detected_zones
+
         self.history_length_s = 5
         self.history_length_n = int(round(self.history_length_s * estimated_frame_rate))
         self.intra_history = np.zeros(self.history_length_n)
         self.inter_history = np.zeros(self.history_length_n)
 
+        self.num_sectors = min(ref_app_config.num_zones, self.distances.size)
+        self.sector_size = max(1, -(-self.distances.size // self.num_sectors))
+
+        self.sector_offset = (self.num_sectors * self.sector_size - self.distances.size) // 2
         win = self.plot_layout
 
         self.intra_limit_lines = []
         self.inter_limit_lines = []
 
-        # Noise estimation plot
-
-        self.noise_plot = win.addPlot(
-            row=0,
-            col=0,
-            title="Noise",
-        )
-        self.noise_plot.setMenuEnabled(False)
-        self.noise_plot.setMouseEnabled(x=False, y=False)
-        self.noise_plot.hideButtons()
-        self.noise_plot.showGrid(x=True, y=True)
-        self.noise_plot.setLabel("bottom", "Distance (m)")
-        self.noise_plot.setLabel("left", "Amplitude")
-        self.noise_plot.setVisible(False)
-        self.noise_curve = self.noise_plot.plot(pen=et.utils.pg_pen_cycler())
-        self.noise_smooth_max = et.utils.SmoothMax(self.detector_config.frame_rate)
-
-        # Depthwise presence plot
-
-        self.move_plot = pg.PlotItem(title="Depthwise presence")
-        self.move_plot.setMenuEnabled(False)
-        self.move_plot.setMouseEnabled(x=False, y=False)
-        self.move_plot.hideButtons()
-        self.move_plot.showGrid(x=True, y=True)
-        self.move_plot.setLabel("bottom", "Distance (m)")
-        self.move_plot.setLabel("left", "Norm. ampl.")
-        self.move_plot.setXRange(self.distances[0], self.distances[-1])
-        self.intra_curve = self.move_plot.plot(pen=et.utils.pg_pen_cycler(1))
-        if not self.detector_config.intra_enable:
-            self.intra_curve.hide()
-
-        self.inter_curve = self.move_plot.plot(pen=et.utils.pg_pen_cycler(0))
-        if not self.detector_config.inter_enable:
-            self.inter_curve.hide()
-
-        self.move_smooth_max = et.utils.SmoothMax(
-            self.detector_config.frame_rate,
-            tau_decay=1.0,
-            tau_grow=0.25,
-        )
-
-        self.move_depth_line = pg.InfiniteLine(pen=pg.mkPen("k", width=1.5))
-        self.move_depth_line.hide()
-        self.move_plot.addItem(self.move_depth_line)
-
-        self.present_html_format = (
-            '<div style="text-align: center">'
-            '<span style="color: #FFFFFF;font-size:15pt;">'
-            "{}</span></div>"
-        )
-        not_present_html = (
-            '<div style="text-align: center">'
-            '<span style="color: #FFFFFF;font-size:15pt;">'
-            "{}</span></div>".format("No presence detected")
-        )
-        self.present_text_item = pg.TextItem(
-            fill=pg.mkColor(0xFF, 0x7F, 0x0E, 200),
-            anchor=(0.5, 0),
-        )
-        self.not_present_text_item = pg.TextItem(
-            html=not_present_html,
-            fill=pg.mkColor(0x1F, 0x77, 0xB4, 180),
-            anchor=(0.5, 0),
-        )
-
-        self.move_plot.addItem(self.present_text_item)
-        self.move_plot.addItem(self.not_present_text_item)
-        self.present_text_item.hide()
-        self.not_present_text_item.hide()
-
         # Intra presence history plot
 
         self.intra_hist_plot = win.addPlot(
-            row=1,
+            row=0,
             col=0,
             title="Intra presence history (fast motions)",
         )
         self.intra_hist_plot.setMenuEnabled(False)
         self.intra_hist_plot.setMouseEnabled(x=False, y=False)
         self.intra_hist_plot.hideButtons()
         self.intra_hist_plot.showGrid(x=True, y=True)
         self.intra_hist_plot.setLabel("bottom", "Time (s)")
         self.intra_hist_plot.setLabel("left", "Score")
         self.intra_hist_plot.setXRange(-self.history_length_s, 0)
-        self.intra_history_smooth_max = et.utils.SmoothMax(self.detector_config.frame_rate)
+        self.intra_history_smooth_max = et.utils.SmoothMax(estimated_frame_rate)
         self.intra_hist_plot.setYRange(0, 10)
-        if not self.detector_config.intra_enable:
+        if not self.ref_app_config.intra_enable:
             intra_color = et.utils.color_cycler(1)
             intra_color = f"{intra_color}50"
             intra_dashed_pen = pg.mkPen(intra_color, width=2.5, style=QtCore.Qt.DashLine)
             intra_pen = pg.mkPen(intra_color, width=2)
         else:
             intra_dashed_pen = et.utils.pg_pen_cycler(1, width=2.5, style="--")
             intra_pen = et.utils.pg_pen_cycler(1)
 
         self.intra_hist_curve = self.intra_hist_plot.plot(pen=intra_pen)
         limit_line = pg.InfiniteLine(angle=0, pen=intra_dashed_pen)
         self.intra_hist_plot.addItem(limit_line)
         self.intra_limit_lines.append(limit_line)
 
         for line in self.intra_limit_lines:
-            line.setPos(self.detector_config.intra_detection_threshold)
+            line.setPos(self.ref_app_config.intra_detection_threshold)
 
         # Inter presence history plot
 
         self.inter_hist_plot = win.addPlot(
-            row=1,
+            row=0,
             col=1,
             title="Inter presence history (slow motions)",
         )
         self.inter_hist_plot.setMenuEnabled(False)
         self.inter_hist_plot.setMouseEnabled(x=False, y=False)
         self.inter_hist_plot.hideButtons()
         self.inter_hist_plot.showGrid(x=True, y=True)
         self.inter_hist_plot.setLabel("bottom", "Time (s)")
         self.inter_hist_plot.setLabel("left", "Score")
         self.inter_hist_plot.setXRange(-self.history_length_s, 0)
-        self.inter_history_smooth_max = et.utils.SmoothMax(self.detector_config.frame_rate)
+        self.inter_history_smooth_max = et.utils.SmoothMax(estimated_frame_rate)
         self.inter_hist_plot.setYRange(0, 10)
-        if not self.detector_config.inter_enable:
+        if not self.ref_app_config.inter_enable:
             inter_color = et.utils.color_cycler(0)
             inter_color = f"{inter_color}50"
             inter_dashed_pen = pg.mkPen(inter_color, width=2.5, style=QtCore.Qt.DashLine)
             inter_pen = pg.mkPen(inter_color, width=2)
         else:
             inter_pen = et.utils.pg_pen_cycler(0)
             inter_dashed_pen = et.utils.pg_pen_cycler(0, width=2.5, style="--")
 
         self.inter_hist_curve = self.inter_hist_plot.plot(pen=inter_pen)
         limit_line = pg.InfiniteLine(angle=0, pen=inter_dashed_pen)
         self.inter_hist_plot.addItem(limit_line)
         self.inter_limit_lines.append(limit_line)
 
         for line in self.inter_limit_lines:
-            line.setPos(self.detector_config.inter_detection_threshold)
+            line.setPos(self.ref_app_config.inter_detection_threshold)
 
-        sublayout = win.addLayout(row=2, col=0, colspan=2)
-        sublayout.layout.setColumnStretchFactor(0, 2)
-        sublayout.addItem(self.move_plot, row=0, col=0)
+        # Sector plot
 
-    def update(self, data: DetectorResult) -> None:
-        noise = data.processor_extra_result.lp_noise
-        self.noise_curve.setData(self.distances, noise)
-        self.noise_plot.setYRange(0, self.noise_smooth_max.update(noise))
-
-        movement_x = data.presence_distance
-
-        self.inter_curve.setData(self.distances, data.inter_depthwise_scores)
-        self.intra_curve.setData(self.distances, data.intra_depthwise_scores)
-        m = self.move_smooth_max.update(
-            np.max(np.maximum(data.inter_depthwise_scores, data.intra_depthwise_scores))
-        )
-        m = max(
-            m,
-            2
-            * np.maximum(
-                self.detector_config.intra_detection_threshold,
-                self.detector_config.inter_detection_threshold,
-            ),
-        )
-        self.move_plot.setYRange(0, m)
-        self.move_depth_line.setPos(movement_x)
-        self.move_depth_line.setVisible(bool(data.presence_detected))
+        self.sector_plot = pg.PlotItem(
+            title="Detection zone<br>Detection type: fast (orange), slow (blue), both (green)"
+        )
+        self.sector_plot.setAspectLocked()
+        self.sector_plot.hideAxis("left")
+        self.sector_plot.hideAxis("bottom")
+        self.sectors = []
+        self.limit_text = []
 
-        self.set_present_text_y_pos(m)
+        self.range_html = (
+            '<div style="text-align: center">'
+            '<span style="color: #000000;font-size:12pt;">'
+            "{}</span></div>"
+        )
 
-        if data.presence_detected:
-            present_text = "Presence detected at {:.0f} cm".format(movement_x * 100)
-            present_html = self.present_html_format.format(present_text)
-            self.present_text_item.setHtml(present_html)
+        pen = pg.mkPen("k", width=1)
+        span_deg = 25
+        for r in np.flip(np.arange(self.num_sectors) + 1):
+            sector = pg.QtWidgets.QGraphicsEllipseItem(-r, -r, r * 2, r * 2)
+            sector.setStartAngle(-16 * span_deg)
+            sector.setSpanAngle(16 * span_deg * 2)
+            sector.setPen(pen)
+            self.sector_plot.addItem(sector)
+            self.sectors.append(sector)
+
+            limit = pg.TextItem(html=self.range_html, anchor=(0.5, 0.5), angle=25)
+            x = r * np.cos(np.radians(span_deg))
+            y = r * np.sin(np.radians(span_deg))
+            limit.setPos(x, y + 0.25)
+            self.sector_plot.addItem(limit)
+            self.limit_text.append(limit)
+
+        self.sectors.reverse()
+
+        start_limit_text = pg.TextItem(html=self.range_html, anchor=(0.5, 0.5), angle=25)
+        range_html = self.range_html.format(f"{ref_app_config.start_m}")
+        start_limit_text.setHtml(range_html)
+        start_limit_text.setPos(0, 0.25)
+        self.sector_plot.addItem(start_limit_text)
+
+        unit_text = pg.TextItem(html=self.range_html, anchor=(0.5, 0.5))
+        unit_html = self.range_html.format("[m]")
+        unit_text.setHtml(unit_html)
+        unit_text.setPos(
+            self.num_sectors + 0.5, (self.num_sectors + 1) * np.sin(np.radians(span_deg))
+        )
+        self.sector_plot.addItem(unit_text)
 
-            self.present_text_item.show()
-            self.not_present_text_item.hide()
-        else:
-            self.present_text_item.hide()
-            self.not_present_text_item.show()
+        sublayout = win.addLayout(row=1, col=0, colspan=2)
+        sublayout.layout.setColumnStretchFactor(0, 2)
+        sublayout.addItem(self.sector_plot, row=0, col=0)
+
+    def update(self, data: RefAppResult) -> None:
 
         # Intra presence
 
         move_hist_xs = np.linspace(-self.history_length_s, 0, self.history_length_n)
 
         self.intra_history = np.roll(self.intra_history, -1)
         self.intra_history[-1] = data.intra_presence_score
 
         m_hist = max(
-            float(np.max(self.intra_history)),
-            self.detector_config.intra_detection_threshold * 1.05,
+            float(np.max(self.intra_history)), self.ref_app_config.intra_detection_threshold * 1.05
         )
         m_hist = self.intra_history_smooth_max.update(m_hist)
 
         self.intra_hist_plot.setYRange(0, m_hist)
         self.intra_hist_curve.setData(move_hist_xs, self.intra_history)
 
         # Inter presence
 
         self.inter_history = np.roll(self.inter_history, -1)
         self.inter_history[-1] = data.inter_presence_score
 
         m_hist = max(
-            float(np.max(self.inter_history)),
-            self.detector_config.inter_detection_threshold * 1.05,
+            float(np.max(self.inter_history)), self.ref_app_config.inter_detection_threshold * 1.05
         )
         m_hist = self.inter_history_smooth_max.update(m_hist)
 
         self.inter_hist_plot.setYRange(0, m_hist)
         self.inter_hist_curve.setData(move_hist_xs, self.inter_history)
 
-    def set_present_text_y_pos(self, y: float) -> None:
-        x_pos = self.distances[0] + (self.distances[-1] - self.distances[0]) / 2
-        self.present_text_item.setPos(x_pos, 0.95 * y)
-        self.not_present_text_item.setPos(x_pos, 0.95 * y)
+        # Sector
+
+        brush = et.utils.pg_brush_cycler(7)
+        for sector in self.sectors:
+            sector.setBrush(brush)
+
+        if data.presence_detected:
+            if self.show_all_detected_zones:
+                for zone, (inter_value, intra_value) in enumerate(
+                    zip(data.inter_zone_detections, data.intra_zone_detections)
+                ):
+                    if inter_value + intra_value == 2:
+                        self.sectors[zone].setBrush(et.utils.pg_brush_cycler(2))
+                    elif inter_value == 1:
+                        self.sectors[zone].setBrush(et.utils.pg_brush_cycler(0))
+                    elif intra_value == 1:
+                        self.sectors[zone].setBrush(et.utils.pg_brush_cycler(1))
+            else:
+                assert data.max_presence_zone is not None
+                if data.max_presence_zone == data.max_intra_zone:
+                    self.sectors[data.max_presence_zone].setBrush(et.utils.pg_brush_cycler(1))
+                else:
+                    self.sectors[data.max_presence_zone].setBrush(et.utils.pg_brush_cycler(0))
+
+        for (text_item, limit) in zip(self.limit_text, np.flip(data.zone_limits)):
+            range_html = self.range_html.format(np.around(limit, 1))
+            text_item.setHtml(range_html)
 
 
 class ViewPlugin(DetectorViewPluginBase):
     def __init__(self, app_model: AppModel, view_widget: QWidget) -> None:
         super().__init__(app_model=app_model, view_widget=view_widget)
         self._log = logging.getLogger(__name__)
 
@@ -419,181 +412,71 @@
         self.start_button.clicked.connect(self._send_start_request)
 
         self.stop_button = QPushButton(icons.STOP(), "Stop")
         self.stop_button.setShortcut("space")
         self.stop_button.setToolTip("Stops the session.\n\nShortcut: Space")
         self.stop_button.clicked.connect(self._send_stop_request)
 
-        button_group = GridGroupBox("Controls", parent=self.sticky_widget)
+        button_group = GroupBox.grid("Controls", parent=self.sticky_widget)
         button_group.layout().addWidget(self.start_button, 0, 0)
         button_group.layout().addWidget(self.stop_button, 0, 1)
 
         sticky_layout.addWidget(button_group)
 
         self.misc_error_view = MiscErrorView(self.scrolly_widget)
         scrolly_layout.addWidget(self.misc_error_view)
 
-        sensor_selection_group = VerticalGroupBox("Sensor selection", parent=self.scrolly_widget)
+        sensor_selection_group = GroupBox.vertical("Sensor selection", parent=self.scrolly_widget)
         self.sensor_id_pidget = pidgets.SensorIdPidgetFactory(items=[]).create(
             parent=sensor_selection_group
         )
         self.sensor_id_pidget.sig_update.connect(self._on_sensor_id_update)
         sensor_selection_group.layout().addWidget(self.sensor_id_pidget)
         scrolly_layout.addWidget(sensor_selection_group)
 
-        self.config_editor = AttrsConfigEditor[DetectorConfig](
-            title="Detector parameters",
+        self.config_editor = AttrsConfigEditor(
+            title="Ref App parameters",
             factory_mapping=self._get_pidget_mapping(),
+            config_type=RefAppConfig,
             parent=self.scrolly_widget,
         )
         self.config_editor.sig_update.connect(self._on_config_update)
         scrolly_layout.addWidget(self.config_editor)
 
+        self.plot_config_editor = AttrsConfigEditor(
+            title="Plot parameters",
+            factory_mapping={
+                "show_all_detected_zones": pidgets.CheckboxPidgetFactory(
+                    name_label_text="Show all detected zones",
+                )
+            },
+            config_type=PlotConfig,
+            save_load_buttons=False,
+            parent=self.scrolly_widget,
+        )
+        self.plot_config_editor.sig_update.connect(self._on_plot_config_update)
+        scrolly_layout.addWidget(self.plot_config_editor)
+
         self.sticky_widget.setLayout(sticky_layout)
         self.scrolly_widget.setLayout(scrolly_layout)
 
     @classmethod
     def _get_pidget_mapping(cls) -> PidgetGroupFactoryMapping:
-        service_parameters = {
-            "start_m": pidgets.FloatPidgetFactory(
-                name_label_text="Range start",
-                suffix=" m",
-                decimals=3,
-            ),
-            "end_m": pidgets.FloatPidgetFactory(
-                name_label_text="Range end",
-                suffix=" m",
-                decimals=3,
-            ),
-            "profile": pidgets.OptionalEnumPidgetFactory(
-                name_label_text="Profile",
-                checkbox_label_text="Override",
-                enum_type=a121.Profile,
-                label_mapping={
-                    a121.Profile.PROFILE_1: "1 (shortest)",
-                    a121.Profile.PROFILE_2: "2",
-                    a121.Profile.PROFILE_3: "3",
-                    a121.Profile.PROFILE_4: "4",
-                    a121.Profile.PROFILE_5: "5 (longest)",
-                },
-            ),
-            "step_length": pidgets.OptionalIntPidgetFactory(
-                name_label_text="Step length",
-                checkbox_label_text="Override",
-                limits=(1, None),
-                init_set_value=24,
-            ),
-            "frame_rate": pidgets.FloatPidgetFactory(
-                name_label_text="Frame rate",
-                suffix=" Hz",
-                decimals=1,
-                limits=(1, 100),
-            ),
-            "sweeps_per_frame": pidgets.IntPidgetFactory(
-                name_label_text="Sweeps per frame",
-                limits=(1, 4095),
-            ),
-            "hwaas": pidgets.IntPidgetFactory(
-                name_label_text="HWAAS",
-                limits=(1, 511),
-            ),
-            "inter_frame_idle_state": pidgets.EnumPidgetFactory(
-                enum_type=a121.IdleState,
-                name_label_text="Inter frame idle state",
-                label_mapping={
-                    a121.IdleState.DEEP_SLEEP: "Deep sleep",
-                    a121.IdleState.SLEEP: "Sleep",
-                    a121.IdleState.READY: "Ready",
-                },
-            ),
-        }
-        intra_parameters = {
-            "intra_detection_threshold": pidgets.FloatSliderPidgetFactory(
-                name_label_text="Intra detection threshold",
-                decimals=2,
-                limits=(0, 5),
-            ),
-            "intra_frame_time_const": pidgets.FloatSliderPidgetFactory(
-                name_label_text="Intra time constant",
-                suffix=" s",
-                decimals=2,
-                limits=(0, 1),
-            ),
-            "intra_output_time_const": pidgets.FloatSliderPidgetFactory(
-                name_label_text="Intra output time constant",
-                suffix=" s",
-                decimals=2,
-                limits=(0.01, 20),
-                log_scale=True,
-            ),
-        }
-        inter_parameters = {
-            "inter_phase_boost": pidgets.CheckboxPidgetFactory(
-                name_label_text="Enable phase boost"
-            ),
-            "inter_detection_threshold": pidgets.FloatSliderPidgetFactory(
-                name_label_text="Inter detection threshold",
-                decimals=2,
-                limits=(0, 5),
-            ),
-            "inter_frame_fast_cutoff": pidgets.FloatSliderPidgetFactory(
-                name_label_text="Inter fast cutoff freq.",
-                suffix=" Hz",
-                decimals=2,
-                limits=(1, 50),
-                log_scale=True,
-            ),
-            "inter_frame_slow_cutoff": pidgets.FloatSliderPidgetFactory(
-                name_label_text="Inter slow cutoff freq.",
-                suffix=" Hz",
-                decimals=2,
-                limits=(0.01, 1),
-                log_scale=True,
-            ),
-            "inter_frame_deviation_time_const": pidgets.FloatSliderPidgetFactory(
-                name_label_text="Inter time constant",
-                suffix=" s",
-                decimals=2,
-                limits=(0.01, 20),
-                log_scale=True,
-            ),
-            "inter_output_time_const": pidgets.FloatSliderPidgetFactory(
-                name_label_text="Inter output time constant",
-                suffix=" s",
-                decimals=2,
-                limits=(0.01, 20),
-                log_scale=True,
-            ),
-            "inter_frame_presence_timeout": pidgets.OptionalIntPidgetFactory(
-                name_label_text="Presence timeout",
-                checkbox_label_text="Enable",
-                suffix=" s",
-                limits=(1, 30),
-                init_set_value=5,
-            ),
-        }
-        return {
-            pidgets.FlatPidgetGroup(): service_parameters,
-            pidgets.FlatPidgetGroup(): {
-                "intra_enable": pidgets.CheckboxPidgetFactory(
-                    name_label_text="Enable intra (fast) motion detection"
-                ),
-            },
-            pidgets.FlatPidgetGroup(
-                hooks=disable_if(parameter_is("intra_enable", False)),
-            ): intra_parameters,
-            pidgets.FlatPidgetGroup(): {
-                "inter_enable": pidgets.CheckboxPidgetFactory(
-                    name_label_text="Enable inter (slow) motion detection"
-                ),
-            },
-            pidgets.FlatPidgetGroup(
-                hooks=disable_if(parameter_is("inter_enable", False)),
-            ): inter_parameters,
-        }
+        presence_pidget_mapping = dict(PresenceViewPlugin._get_pidget_mapping())
+        presence_pidget_mapping.update(
+            {
+                pidgets.FlatPidgetGroup(): {
+                    "num_zones": pidgets.IntPidgetFactory(
+                        name_label_text="Number of zones",
+                        limits=(1, None),
+                    ),
+                }
+            }
+        )
+        return presence_pidget_mapping
 
     def on_backend_state_update(self, backend_plugin_state: Optional[SharedState]) -> None:
         if backend_plugin_state is not None and backend_plugin_state.config is not None:
             results = backend_plugin_state.config._collect_validation_results()
 
             not_handled = self.config_editor.handle_validation_results(results)
 
@@ -614,25 +497,30 @@
 
             return
 
         assert isinstance(state, SharedState)
 
         self.config_editor.setEnabled(app_model.plugin_state == PluginState.LOADED_IDLE)
         self.config_editor.set_data(state.config)
+        self.plot_config_editor.setEnabled(app_model.plugin_state == PluginState.LOADED_IDLE)
+        self.plot_config_editor.set_data(state.plot_config)
         self.sensor_id_pidget.set_selected_sensor(state.sensor_id, app_model.connected_sensors)
         self.sensor_id_pidget.setEnabled(app_model.plugin_state.is_steady)
 
         self.start_button.setEnabled(
             app_model.is_ready_for_session() and self.config_editor.is_ready
         )
         self.stop_button.setEnabled(app_model.plugin_state == PluginState.LOADED_BUSY)
 
-    def _on_config_update(self, config: DetectorConfig) -> None:
+    def _on_config_update(self, config: RefAppConfig) -> None:
         BackendPlugin.update_config.rpc(self.app_model.put_task, config=config)
 
+    def _on_plot_config_update(self, config: PlotConfig) -> None:
+        BackendPlugin.update_plot_config.rpc(self.app_model.put_task, config=config)
+
     def _send_defaults_request(self) -> None:
         BackendPlugin.restore_defaults.rpc(self.app_model.put_task)
 
     def _on_sensor_id_update(self, sensor_id: int) -> None:
         BackendPlugin.update_sensor_id.rpc(self.app_model.put_task, sensor_id=sensor_id)
 
 
@@ -647,20 +535,20 @@
 
     def create_plot_plugin(
         self, app_model: AppModel, plot_layout: pg.GraphicsLayout
     ) -> PlotPlugin:
         return PlotPlugin(app_model=app_model, plot_layout=plot_layout)
 
 
-PRESENCE_DETECTOR_PLUGIN = PluginSpec(
+SMART_PRESENCE_PLUGIN = PluginSpec(
     generation=PluginGeneration.A121,
-    key="presence_detector",
-    title="Presence detector",
-    description="Detect human presence.",
-    family=PluginFamily.DETECTOR,
+    key="smart_presence",
+    title="Smart presence",
+    description="Split presence detection range into zones.",
+    family=PluginFamily.REF_APP,
     presets=[
         PluginPresetBase(
             name="Short range",
             description="Short range",
             preset_id=PluginPresetId.SHORT_RANGE,
         ),
         PluginPresetBase(
```

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/presence/_processors.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/presence/_processors.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/presence/_serializers.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/presence/_serializers.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/smart_presence/_configs.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/smart_presence/_configs.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/smart_presence/_processor.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/smart_presence/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/smart_presence/_ref_app.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/smart_presence/_ref_app.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/smart_presence/_ref_app_plugin.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/surface_velocity/_example_app_plugin.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,398 +7,326 @@
 from enum import Enum, auto
 from typing import Callable, Mapping, Optional
 
 import attrs
 import h5py
 import numpy as np
 
-from PySide6 import QtCore
 from PySide6.QtWidgets import QPushButton, QVBoxLayout, QWidget
 
 import pyqtgraph as pg
 
 import acconeer.exptool as et
 from acconeer.exptool import a121
 from acconeer.exptool.a121._h5_utils import _create_h5_string_dataset
-from acconeer.exptool.a121.algo._base import AlgoBase
 from acconeer.exptool.a121.algo._plugins import (
     DetectorBackendPluginBase,
     DetectorPlotPluginBase,
     DetectorViewPluginBase,
 )
-from acconeer.exptool.a121.algo.presence._detector import Detector
-from acconeer.exptool.a121.algo.presence._detector_plugin import ViewPlugin as PresenceViewPlugin
 from acconeer.exptool.app.new import (
     AppModel,
     AttrsConfigEditor,
     BackendLogger,
     GeneralMessage,
-    GridGroupBox,
+    GroupBox,
     Message,
     MiscErrorView,
-    PidgetGroupFactoryMapping,
+    PidgetFactoryMapping,
     PluginFamily,
     PluginGeneration,
     PluginPresetBase,
     PluginSpecBase,
     PluginState,
-    VerticalGroupBox,
     icons,
     is_task,
     pidgets,
 )
+from acconeer.exptool.app.new.ui.plugin_components.range_help_view import RangeHelpView
 
-from ._configs import get_long_range_config, get_medium_range_config, get_short_range_config
-from ._ref_app import RefApp, RefAppConfig, RefAppResult, _load_algo_data
-
-
-@attrs.mutable(kw_only=True)
-class PlotConfig(AlgoBase):
-    show_all_detected_zones: bool = attrs.field(default=False)
+from ._example_app import ExampleApp, ExampleAppConfig, ExampleAppResult, _load_algo_data
 
 
 @attrs.mutable(kw_only=True)
 class SharedState:
     sensor_id: int = attrs.field(default=1)
-    config: RefAppConfig = attrs.field(factory=RefAppConfig)
-    plot_config: PlotConfig = attrs.field(factory=PlotConfig)
+    config: ExampleAppConfig = attrs.field(factory=ExampleAppConfig)
 
 
 class PluginPresetId(Enum):
-    SHORT_RANGE = auto()
-    MEDIUM_RANGE = auto()
-    LONG_RANGE = auto()
+    DEFAULT = auto()
 
 
 class BackendPlugin(DetectorBackendPluginBase[SharedState]):
 
-    PLUGIN_PRESETS: Mapping[int, Callable[[], RefAppConfig]] = {
-        PluginPresetId.SHORT_RANGE.value: lambda: get_short_range_config(),
-        PluginPresetId.MEDIUM_RANGE.value: lambda: get_medium_range_config(),
-        PluginPresetId.LONG_RANGE.value: lambda: get_long_range_config(),
+    PLUGIN_PRESETS: Mapping[int, Callable[[], ExampleAppConfig]] = {
+        PluginPresetId.DEFAULT.value: lambda: ExampleAppConfig()
     }
 
     def __init__(
         self, callback: Callable[[Message], None], generation: PluginGeneration, key: str
     ) -> None:
         super().__init__(callback=callback, generation=generation, key=key)
 
         self._recorder: Optional[a121.H5Recorder] = None
-        self._ref_app_instance: Optional[RefApp] = None
+        self._exempel_app_instance: Optional[ExampleApp] = None
         self._log = BackendLogger.getLogger(__name__)
 
         self.restore_defaults()
 
     def _load_from_cache(self, file: h5py.File) -> None:
-        self.shared_state.config = RefAppConfig.from_json(file["config"][()])
-        self.shared_state.plot_config = PlotConfig.from_json(file["plot_config"][()])
-
-        show_all_detected_zones = self.shared_state.plot_config.show_all_detected_zones
-        self.shared_state.config.show_all_detected_zones = show_all_detected_zones
+        self.shared_state.config = ExampleAppConfig.from_json(file["config"][()])
 
     @is_task
     def restore_defaults(self) -> None:
         self.shared_state = SharedState()
         self.broadcast()
 
     @is_task
     def update_sensor_id(self, *, sensor_id: int) -> None:
         self.shared_state.sensor_id = sensor_id
         self.broadcast()
 
-    @is_task
-    def update_plot_config(self, *, config: PlotConfig) -> None:
-        self.shared_state.plot_config = config
-        self.broadcast()
-
     def _sync_sensor_ids(self) -> None:
         if self.client is not None:
             sensor_ids = self.client.server_info.connected_sensors
 
             if len(sensor_ids) > 0 and self.shared_state.sensor_id not in sensor_ids:
                 self.shared_state.sensor_id = sensor_ids[0]
 
     @is_task
-    def update_config(self, *, config: RefAppConfig) -> None:
+    def update_config(self, *, config: ExampleAppConfig) -> None:
         self.shared_state.config = config
         self.broadcast()
 
     def save_to_cache(self, file: h5py.File) -> None:
         _create_h5_string_dataset(file, "config", self.shared_state.config.to_json())
-        _create_h5_string_dataset(file, "plot_config", self.shared_state.plot_config.to_json())
 
     @is_task
     def set_preset(self, preset_id: int) -> None:
         preset_config = self.PLUGIN_PRESETS[preset_id]
         self.shared_state.config = preset_config()
-        self.shared_state.plot_config = PlotConfig()
         self.broadcast()
 
     def load_from_record_setup(self, *, record: a121.H5Record) -> None:
         algo_group = record.get_algo_group(self.key)
         _, config = _load_algo_data(algo_group)
         self.shared_state.config = config
         self.shared_state.sensor_id = record.sensor_id
 
     def _start_session(self, recorder: Optional[a121.H5Recorder]) -> None:
         assert self.client
-        self._ref_app_instance = RefApp(
+        self._example_app_instance = ExampleApp(
             client=self.client,
             sensor_id=self.shared_state.sensor_id,
-            ref_app_config=self.shared_state.config,
+            example_app_config=self.shared_state.config,
         )
-        self._ref_app_instance.start(recorder)
+        self._example_app_instance.start(recorder)
         self.callback(
             GeneralMessage(
                 name="setup",
                 kwargs=dict(
-                    ref_app_config=self.shared_state.config,
-                    sensor_config=Detector._get_sensor_config(
-                        self._ref_app_instance.detector.config
-                    ),
-                    plot_config=self.shared_state.plot_config,
-                    estimated_frame_rate=self._ref_app_instance.detector.estimated_frame_rate,
+                    example_app_config=self.shared_state.config,
                 ),
                 recipient="plot_plugin",
             )
         )
 
     def end_session(self) -> None:
-        if self._ref_app_instance is None:
+        if self._example_app_instance is None:
             raise RuntimeError
         if self._recorder is not None:
             self._recorder.close()
-        self._ref_app_instance.stop()
+        self._example_app_instance.stop()
 
     def get_next(self) -> None:
         assert self.client
-        if self._ref_app_instance is None:
+        if self._example_app_instance is None:
             raise RuntimeError
-        result = self._ref_app_instance.get_next()
+        result = self._example_app_instance.get_next()
 
         self.callback(GeneralMessage(name="plot", data=result, recipient="plot_plugin"))
 
 
 class PlotPlugin(DetectorPlotPluginBase):
+
+    _VELOCITY_Y_SCALE_MARGIN_M = 0.25
+
     def __init__(self, *, plot_layout: pg.GraphicsLayout, app_model: AppModel) -> None:
         super().__init__(plot_layout=plot_layout, app_model=app_model)
 
     def setup_from_message(self, message: GeneralMessage) -> None:
         assert message.kwargs is not None
         self.setup(**message.kwargs)
 
     def update_from_message(self, message: GeneralMessage) -> None:
-        assert isinstance(message.data, RefAppResult)
+        assert isinstance(message.data, ExampleAppResult)
         self.update(message.data)
 
     def setup(
         self,
-        ref_app_config: RefAppConfig,
-        sensor_config: a121.SensorConfig,
-        plot_config: PlotConfig,
-        estimated_frame_rate: float,
+        example_app_config: ExampleAppConfig,
     ) -> None:
-        self.ref_app_config = ref_app_config
-        self.distances = np.linspace(
-            ref_app_config.start_m, ref_app_config.end_m, sensor_config.num_points
-        )
-
-        self.show_all_detected_zones = plot_config.show_all_detected_zones
-
-        self.history_length_s = 5
-        self.history_length_n = int(round(self.history_length_s * estimated_frame_rate))
-        self.intra_history = np.zeros(self.history_length_n)
-        self.inter_history = np.zeros(self.history_length_n)
-
-        self.num_sectors = min(ref_app_config.num_zones, self.distances.size)
-        self.sector_size = max(1, -(-self.distances.size // self.num_sectors))
-
-        self.sector_offset = (self.num_sectors * self.sector_size - self.distances.size) // 2
-        win = self.plot_layout
-
-        self.intra_limit_lines = []
-        self.inter_limit_lines = []
-
-        # Intra presence history plot
-
-        self.intra_hist_plot = win.addPlot(
-            row=0,
-            col=0,
-            title="Intra presence history (fast motions)",
-        )
-        self.intra_hist_plot.setMenuEnabled(False)
-        self.intra_hist_plot.setMouseEnabled(x=False, y=False)
-        self.intra_hist_plot.hideButtons()
-        self.intra_hist_plot.showGrid(x=True, y=True)
-        self.intra_hist_plot.setLabel("bottom", "Time (s)")
-        self.intra_hist_plot.setLabel("left", "Score")
-        self.intra_hist_plot.setXRange(-self.history_length_s, 0)
-        self.intra_history_smooth_max = et.utils.SmoothMax(estimated_frame_rate)
-        self.intra_hist_plot.setYRange(0, 10)
-        if not self.ref_app_config.intra_enable:
-            intra_color = et.utils.color_cycler(1)
-            intra_color = f"{intra_color}50"
-            intra_dashed_pen = pg.mkPen(intra_color, width=2.5, style=QtCore.Qt.DashLine)
-            intra_pen = pg.mkPen(intra_color, width=2)
-        else:
-            intra_dashed_pen = et.utils.pg_pen_cycler(1, width=2.5, style="--")
-            intra_pen = et.utils.pg_pen_cycler(1)
 
-        self.intra_hist_curve = self.intra_hist_plot.plot(pen=intra_pen)
-        limit_line = pg.InfiniteLine(angle=0, pen=intra_dashed_pen)
-        self.intra_hist_plot.addItem(limit_line)
-        self.intra_limit_lines.append(limit_line)
-
-        for line in self.intra_limit_lines:
-            line.setPos(self.ref_app_config.intra_detection_threshold)
-
-        # Inter presence history plot
-
-        self.inter_hist_plot = win.addPlot(
-            row=0,
-            col=1,
-            title="Inter presence history (slow motions)",
-        )
-        self.inter_hist_plot.setMenuEnabled(False)
-        self.inter_hist_plot.setMouseEnabled(x=False, y=False)
-        self.inter_hist_plot.hideButtons()
-        self.inter_hist_plot.showGrid(x=True, y=True)
-        self.inter_hist_plot.setLabel("bottom", "Time (s)")
-        self.inter_hist_plot.setLabel("left", "Score")
-        self.inter_hist_plot.setXRange(-self.history_length_s, 0)
-        self.inter_history_smooth_max = et.utils.SmoothMax(estimated_frame_rate)
-        self.inter_hist_plot.setYRange(0, 10)
-        if not self.ref_app_config.inter_enable:
-            inter_color = et.utils.color_cycler(0)
-            inter_color = f"{inter_color}50"
-            inter_dashed_pen = pg.mkPen(inter_color, width=2.5, style=QtCore.Qt.DashLine)
-            inter_pen = pg.mkPen(inter_color, width=2)
+        self.slow_zone = example_app_config.slow_zone
+        self.history_length_s = 10
+        if example_app_config.frame_rate is None:
+            estimated_frame_rate = (
+                example_app_config.sweep_rate / example_app_config.sweeps_per_frame
+            )
         else:
-            inter_pen = et.utils.pg_pen_cycler(0)
-            inter_dashed_pen = et.utils.pg_pen_cycler(0, width=2.5, style="--")
+            estimated_frame_rate = example_app_config.frame_rate
+
+        self.history_length_n = int(np.around(self.history_length_s * estimated_frame_rate))
 
-        self.inter_hist_curve = self.inter_hist_plot.plot(pen=inter_pen)
-        limit_line = pg.InfiniteLine(angle=0, pen=inter_dashed_pen)
-        self.inter_hist_plot.addItem(limit_line)
-        self.inter_limit_lines.append(limit_line)
+        c0_dashed_pen = et.utils.pg_pen_cycler(0, width=2.5, style="--")
 
-        for line in self.inter_limit_lines:
-            line.setPos(self.ref_app_config.inter_detection_threshold)
+        # Velocity plot
 
-        # Sector plot
+        self.velocity_history_plot = self._create_plot(self.plot_layout, row=0, col=0)
+        self.velocity_history_plot.setTitle("Estimated velocity")
+        self.velocity_history_plot.setLabel(axis="left", text="Velocity", units="m/s")
+        self.velocity_history_plot.setLabel(axis="bottom", text="Time", units="s")
+        self.velocity_history_plot.addLegend(labelTextSize="10pt")
+        self.velocity_smooth_limits = et.utils.SmoothLimits()
 
-        self.sector_plot = pg.PlotItem(
-            title="Detection zone<br>Detection type: fast (orange), slow (blue), both (green)"
+        self.velocity_curve = self.velocity_history_plot.plot(
+            pen=et.utils.pg_pen_cycler(0), name="Estimated velocity"
         )
-        self.sector_plot.setAspectLocked()
-        self.sector_plot.hideAxis("left")
-        self.sector_plot.hideAxis("bottom")
-        self.sectors = []
-        self.limit_text = []
 
-        self.range_html = (
+        self.psd_html = (
             '<div style="text-align: center">'
-            '<span style="color: #000000;font-size:12pt;">'
+            '<span style="color: #FFFFFF;font-size:13pt;">'
             "{}</span></div>"
         )
 
-        pen = pg.mkPen("k", width=1)
-        span_deg = 25
-        for r in np.flip(np.arange(self.num_sectors) + 1):
-            sector = pg.QtWidgets.QGraphicsEllipseItem(-r, -r, r * 2, r * 2)
-            sector.setStartAngle(-16 * span_deg)
-            sector.setSpanAngle(16 * span_deg * 2)
-            sector.setPen(pen)
-            self.sector_plot.addItem(sector)
-            self.sectors.append(sector)
-
-            limit = pg.TextItem(html=self.range_html, anchor=(0.5, 0.5), angle=25)
-            x = r * np.cos(np.radians(span_deg))
-            y = r * np.sin(np.radians(span_deg))
-            limit.setPos(x, y + 0.25)
-            self.sector_plot.addItem(limit)
-            self.limit_text.append(limit)
-
-        self.sectors.reverse()
-
-        start_limit_text = pg.TextItem(html=self.range_html, anchor=(0.5, 0.5), angle=25)
-        range_html = self.range_html.format(f"{ref_app_config.start_m}")
-        start_limit_text.setHtml(range_html)
-        start_limit_text.setPos(0, 0.25)
-        self.sector_plot.addItem(start_limit_text)
-
-        unit_text = pg.TextItem(html=self.range_html, anchor=(0.5, 0.5))
-        unit_html = self.range_html.format("[m]")
-        unit_text.setHtml(unit_html)
-        unit_text.setPos(
-            self.num_sectors + 0.5, (self.num_sectors + 1) * np.sin(np.radians(span_deg))
-        )
-        self.sector_plot.addItem(unit_text)
-
-        sublayout = win.addLayout(row=1, col=0, colspan=2)
-        sublayout.layout.setColumnStretchFactor(0, 2)
-        sublayout.addItem(self.sector_plot, row=0, col=0)
-
-    def update(self, data: RefAppResult) -> None:
-
-        # Intra presence
-
-        move_hist_xs = np.linspace(-self.history_length_s, 0, self.history_length_n)
-
-        self.intra_history = np.roll(self.intra_history, -1)
-        self.intra_history[-1] = data.intra_presence_score
-
-        m_hist = max(
-            float(np.max(self.intra_history)), self.ref_app_config.intra_detection_threshold * 1.05
-        )
-        m_hist = self.intra_history_smooth_max.update(m_hist)
-
-        self.intra_hist_plot.setYRange(0, m_hist)
-        self.intra_hist_curve.setData(move_hist_xs, self.intra_history)
-
-        # Inter presence
-
-        self.inter_history = np.roll(self.inter_history, -1)
-        self.inter_history[-1] = data.inter_presence_score
-
-        m_hist = max(
-            float(np.max(self.inter_history)), self.ref_app_config.inter_detection_threshold * 1.05
-        )
-        m_hist = self.inter_history_smooth_max.update(m_hist)
-
-        self.inter_hist_plot.setYRange(0, m_hist)
-        self.inter_hist_curve.setData(move_hist_xs, self.inter_history)
-
-        # Sector
-
-        brush = et.utils.pg_brush_cycler(7)
-        for sector in self.sectors:
-            sector.setBrush(brush)
-
-        if data.presence_detected:
-            if self.show_all_detected_zones:
-                for zone, (inter_value, intra_value) in enumerate(
-                    zip(data.inter_zone_detections, data.intra_zone_detections)
-                ):
-                    if inter_value + intra_value == 2:
-                        self.sectors[zone].setBrush(et.utils.pg_brush_cycler(2))
-                    elif inter_value == 1:
-                        self.sectors[zone].setBrush(et.utils.pg_brush_cycler(0))
-                    elif intra_value == 1:
-                        self.sectors[zone].setBrush(et.utils.pg_brush_cycler(1))
-            else:
-                assert data.max_presence_zone is not None
-                if data.max_presence_zone == data.max_intra_zone:
-                    self.sectors[data.max_presence_zone].setBrush(et.utils.pg_brush_cycler(1))
-                else:
-                    self.sectors[data.max_presence_zone].setBrush(et.utils.pg_brush_cycler(0))
-
-        for (text_item, limit) in zip(self.limit_text, np.flip(data.zone_limits)):
-            range_html = self.range_html.format(np.around(limit, 1))
-            text_item.setHtml(range_html)
+        self.distance_text_item = pg.TextItem(
+            html=self.psd_html,
+            fill=pg.mkColor(0x1F, 0x77, 0xB4, 180),
+            anchor=(0.5, 0),
+        )
+
+        self.velocity_history_plot.addItem(self.distance_text_item)
+
+        self.velocity_history = np.zeros(self.history_length_n)
+
+        self.lower_std_history = np.zeros(self.history_length_n)
+        self.upper_std_history = np.zeros(self.history_length_n)
+
+        self.lower_std_curve = self.velocity_history_plot.plot()
+        self.upper_std_curve = self.velocity_history_plot.plot()
+
+        fbi = pg.FillBetweenItem(
+            self.lower_std_curve,
+            self.upper_std_curve,
+            brush=pg.mkBrush(f"{et.utils.color_cycler(0)}50"),
+        )
+
+        self.velocity_history_plot.addItem(fbi)
+
+        # PSD plot
+
+        self.psd_plot = self._create_plot(self.plot_layout, row=1, col=0)
+        self.psd_plot.setTitle("PSD<br>(colored area represents the slow zone)")
+        self.psd_plot.setLabel(axis="left", text="Power")
+        self.psd_plot.setLabel(axis="bottom", text="Velocity", units="m/s")
+        self.psd_plot.addLegend(labelTextSize="10pt")
+
+        self.psd_smooth_max = et.utils.SmoothMax(tau_grow=0.5, tau_decay=2.0)
+        self.psd_curve = self.psd_plot.plot(pen=et.utils.pg_pen_cycler(0), name="PSD")
+        self.psd_threshold = self.psd_plot.plot(pen=c0_dashed_pen, name="Threshold")
+
+        psd_slow_zone_color = et.utils.color_cycler(0)
+        psd_slow_zone_color = f"{psd_slow_zone_color}50"
+        psd_slow_zone_brush = pg.mkBrush(psd_slow_zone_color)
+
+        self.psd_slow_zone = pg.LinearRegionItem(brush=psd_slow_zone_brush, movable=False)
+        self.psd_plot.addItem(self.psd_slow_zone)
+
+        brush = et.utils.pg_brush_cycler(0)
+        self.psd_peak_plot_item = pg.PlotDataItem(
+            pen=None, symbol="o", symbolSize=8, symbolBrush=brush, symbolPen="k"
+        )
+        self.psd_plot.addItem(self.psd_peak_plot_item)
+
+        self.psd_plot.setLogMode(x=False, y=True)
+
+    def update(self, example_app_result: ExampleAppResult) -> None:
+        processor_extra_result = example_app_result.processor_extra_result
+
+        lim = self.velocity_smooth_limits.update(example_app_result.velocity)
+
+        self.velocity_history_plot.setYRange(
+            lim[0] - self._VELOCITY_Y_SCALE_MARGIN_M, lim[1] + self._VELOCITY_Y_SCALE_MARGIN_M
+        )
+        self.velocity_history_plot.setXRange(-self.history_length_s, 0)
+
+        xs = np.linspace(-self.history_length_s, 0, self.history_length_n)
+
+        self.velocity_history = np.roll(self.velocity_history, -1)
+        self.velocity_history[-1] = example_app_result.velocity
+        self.velocity_curve.setData(xs, self.velocity_history)
+
+        velocity_html = self.psd_html.format(
+            f"Distance {np.around(example_app_result.distance_m, 2)} m"
+        )
+        self.distance_text_item.setHtml(velocity_html)
+        self.distance_text_item.setPos(
+            -self.history_length_s / 2, lim[1] + self._VELOCITY_Y_SCALE_MARGIN_M
+        )
+
+        self.lower_std_history = np.roll(self.lower_std_history, -1)
+        self.lower_std_history[-1] = (
+            example_app_result.velocity + 0.5 * processor_extra_result.peak_width
+        )
+        self.lower_std_curve.setData(xs, self.lower_std_history)
+
+        self.upper_std_history = np.roll(self.upper_std_history, -1)
+        self.upper_std_history[-1] = (
+            example_app_result.velocity - 0.5 * processor_extra_result.peak_width
+        )
+        self.upper_std_curve.setData(xs, self.upper_std_history)
+
+        lim = self.psd_smooth_max.update(processor_extra_result.psd_threshold)
+        self.psd_plot.setYRange(np.log10(0.2), np.log10(lim))
+        self.psd_plot.setXRange(
+            processor_extra_result.max_bin_vertical_vs[0],
+            processor_extra_result.max_bin_vertical_vs[-1],
+        )
+        self.psd_curve.setData(
+            processor_extra_result.vertical_velocities, processor_extra_result.psd
+        )
+        self.psd_threshold.setData(
+            processor_extra_result.vertical_velocities, processor_extra_result.psd_threshold
+        )
+        if processor_extra_result.peak_idx is not None:
+            self.psd_peak_plot_item.setData(
+                [processor_extra_result.vertical_velocities[processor_extra_result.peak_idx]],
+                [processor_extra_result.psd[processor_extra_result.peak_idx]],
+            )
+        else:
+            self.psd_peak_plot_item.clear()
+
+        middle_idx = int(np.around(processor_extra_result.vertical_velocities.shape[0] / 2))
+        self.psd_slow_zone.setRegion(
+            [
+                processor_extra_result.vertical_velocities[middle_idx - self.slow_zone],
+                processor_extra_result.vertical_velocities[middle_idx + self.slow_zone],
+            ]
+        )
+
+    @staticmethod
+    def _create_plot(parent: pg.GraphicsLayout, row: int, col: int) -> pg.PlotItem:
+        velocity_history_plot = parent.addPlot(row=row, col=col)
+        velocity_history_plot.setMenuEnabled(False)
+        velocity_history_plot.setMouseEnabled(x=False, y=False)
+        velocity_history_plot.hideButtons()
+        velocity_history_plot.showGrid(x=True, y=True, alpha=0.5)
+
+        return velocity_history_plot
 
 
 class ViewPlugin(DetectorViewPluginBase):
     def __init__(self, app_model: AppModel, view_widget: QWidget) -> None:
         super().__init__(app_model=app_model, view_widget=view_widget)
         self._log = logging.getLogger(__name__)
 
@@ -413,79 +341,180 @@
         self.start_button.clicked.connect(self._send_start_request)
 
         self.stop_button = QPushButton(icons.STOP(), "Stop")
         self.stop_button.setShortcut("space")
         self.stop_button.setToolTip("Stops the session.\n\nShortcut: Space")
         self.stop_button.clicked.connect(self._send_stop_request)
 
-        button_group = GridGroupBox("Controls", parent=self.sticky_widget)
+        button_group = GroupBox.grid("Controls", parent=self.sticky_widget)
         button_group.layout().addWidget(self.start_button, 0, 0)
         button_group.layout().addWidget(self.stop_button, 0, 1)
 
         sticky_layout.addWidget(button_group)
 
         self.misc_error_view = MiscErrorView(self.scrolly_widget)
         scrolly_layout.addWidget(self.misc_error_view)
 
-        sensor_selection_group = VerticalGroupBox("Sensor selection", parent=self.scrolly_widget)
+        sensor_selection_group = GroupBox.vertical("Sensor selection", parent=self.scrolly_widget)
         self.sensor_id_pidget = pidgets.SensorIdPidgetFactory(items=[]).create(
             parent=sensor_selection_group
         )
         self.sensor_id_pidget.sig_update.connect(self._on_sensor_id_update)
         sensor_selection_group.layout().addWidget(self.sensor_id_pidget)
         scrolly_layout.addWidget(sensor_selection_group)
 
-        self.config_editor = AttrsConfigEditor[RefAppConfig](
-            title="Ref App parameters",
+        self.range_helper = RangeHelpView()
+        scrolly_layout.addWidget(self.range_helper)
+
+        self.config_editor = AttrsConfigEditor(
+            title="Example app parameters",
             factory_mapping=self._get_pidget_mapping(),
+            config_type=ExampleAppConfig,
             parent=self.scrolly_widget,
         )
         self.config_editor.sig_update.connect(self._on_config_update)
         scrolly_layout.addWidget(self.config_editor)
 
-        self.plot_config_editor = AttrsConfigEditor[PlotConfig](
-            title="Plot parameters",
-            factory_mapping={
-                "show_all_detected_zones": pidgets.CheckboxPidgetFactory(
-                    name_label_text="Show all detected zones",
-                )
-            },
-            parent=self.scrolly_widget,
-        )
-        self.plot_config_editor.sig_update.connect(self._on_plot_config_update)
-        scrolly_layout.addWidget(self.plot_config_editor)
-
         self.sticky_widget.setLayout(sticky_layout)
         self.scrolly_widget.setLayout(scrolly_layout)
 
     @classmethod
-    def _get_pidget_mapping(cls) -> PidgetGroupFactoryMapping:
-        presence_pidget_mapping = dict(PresenceViewPlugin._get_pidget_mapping())
-        presence_pidget_mapping.update(
-            {
-                pidgets.FlatPidgetGroup(): {
-                    "num_zones": pidgets.IntPidgetFactory(
-                        name_label_text="Number of zones",
-                        limits=(1, None),
-                    ),
-                }
-            }
-        )
-        return presence_pidget_mapping
+    def _get_pidget_mapping(cls) -> PidgetFactoryMapping:
+        return {
+            "surface_distance": pidgets.FloatPidgetFactory(
+                name_label_text="Surface distance",
+                suffix=" m",
+                decimals=2,
+                limits=(0.1, 3),
+            ),
+            "sensor_angle": pidgets.FloatPidgetFactory(
+                name_label_text="Sensor angle",
+                suffix=" degrees",
+                decimals=1,
+                limits=(0, 89),
+            ),
+            "num_points": pidgets.IntPidgetFactory(
+                name_label_text="Number of distance points",
+                limits=(1, None),
+            ),
+            "sweep_rate": pidgets.FloatPidgetFactory(
+                name_label_text="Sweep rate",
+                suffix=" Hz",
+                decimals=1,
+                limits=(100, None),
+            ),
+            "sweeps_per_frame": pidgets.IntPidgetFactory(
+                name_label_text="Sweeps per frame",
+                limits=(64, 2048),
+            ),
+            "hwaas": pidgets.IntPidgetFactory(
+                name_label_text="HWAAS",
+                limits=(1, 511),
+            ),
+            "profile": pidgets.OptionalEnumPidgetFactory(
+                name_label_text="Profile",
+                checkbox_label_text="Override",
+                enum_type=a121.Profile,
+                label_mapping={
+                    a121.Profile.PROFILE_1: "1 (shortest)",
+                    a121.Profile.PROFILE_2: "2",
+                    a121.Profile.PROFILE_3: "3",
+                    a121.Profile.PROFILE_4: "4",
+                    a121.Profile.PROFILE_5: "5 (longest)",
+                },
+            ),
+            "step_length": pidgets.IntPidgetFactory(
+                name_label_text="Step length:",
+                limits=(1, None),
+            ),
+            "frame_rate": pidgets.OptionalFloatPidgetFactory(
+                name_label_text="Frame rate",
+                checkbox_label_text="Limit",
+                suffix=" Hz",
+                decimals=1,
+                limits=(1, None),
+                init_set_value=10,
+            ),
+            "continuous_sweep_mode": pidgets.CheckboxPidgetFactory(
+                name_label_text="Continuos sweep mode",
+            ),
+            "double_buffering": pidgets.CheckboxPidgetFactory(
+                name_label_text="Double buffering",
+            ),
+            "inter_frame_idle_state": pidgets.EnumPidgetFactory(
+                enum_type=a121.IdleState,
+                name_label_text="Inter frame idle state",
+                label_mapping={
+                    a121.IdleState.DEEP_SLEEP: "Deep sleep",
+                    a121.IdleState.SLEEP: "Sleep",
+                    a121.IdleState.READY: "Ready",
+                },
+            ),
+            "inter_sweep_idle_state": pidgets.EnumPidgetFactory(
+                enum_type=a121.IdleState,
+                name_label_text="Inter sweep idle state",
+                label_mapping={
+                    a121.IdleState.DEEP_SLEEP: "Deep sleep",
+                    a121.IdleState.SLEEP: "Sleep",
+                    a121.IdleState.READY: "Ready",
+                },
+            ),
+            "time_series_length": pidgets.IntPidgetFactory(
+                name_label_text="Time series length",
+                limits=(64, None),
+            ),
+            "psd_lp_coeff": pidgets.FloatSliderPidgetFactory(
+                name_label_text="PSD time filtering coeff.",
+                limits=(0, 1),
+                decimals=3,
+            ),
+            "slow_zone": pidgets.IntPidgetFactory(
+                name_label_text="Slow zone half length",
+                limits=(0, 20),
+            ),
+            "velocity_lp_coeff": pidgets.FloatSliderPidgetFactory(
+                name_label_text="Velocity time filtering coeff.\nper time series",
+                limits=(0, 1),
+                decimals=3,
+            ),
+            "cfar_win": pidgets.IntPidgetFactory(
+                name_label_text="CFAR window length",
+                limits=(0, 20),
+            ),
+            "cfar_guard": pidgets.IntPidgetFactory(
+                name_label_text="CFAR guard length",
+                limits=(0, 20),
+            ),
+            "cfar_sensitivity": pidgets.FloatSliderPidgetFactory(
+                name_label_text="Threshold sensitivity",
+                decimals=2,
+                limits=(0.01, 1),
+            ),
+            "max_peak_interval_s": pidgets.FloatPidgetFactory(
+                name_label_text="Max peak interval",
+                decimals=1,
+                limits=(0, 20),
+                suffix=" s",
+            ),
+        }
 
     def on_backend_state_update(self, backend_plugin_state: Optional[SharedState]) -> None:
         if backend_plugin_state is not None and backend_plugin_state.config is not None:
             results = backend_plugin_state.config._collect_validation_results()
 
             not_handled = self.config_editor.handle_validation_results(results)
 
             not_handled = self.misc_error_view.handle_validation_results(not_handled)
 
             assert not_handled == []
 
+            self.range_helper.update(
+                ExampleApp._get_sensor_config(backend_plugin_state.config).subsweep
+            )
+
     def on_app_model_update(self, app_model: AppModel) -> None:
         state = app_model.backend_plugin_state
 
         if state is None:
             self.start_button.setEnabled(False)
             self.stop_button.setEnabled(False)
 
@@ -495,30 +524,25 @@
 
             return
 
         assert isinstance(state, SharedState)
 
         self.config_editor.setEnabled(app_model.plugin_state == PluginState.LOADED_IDLE)
         self.config_editor.set_data(state.config)
-        self.plot_config_editor.setEnabled(app_model.plugin_state == PluginState.LOADED_IDLE)
-        self.plot_config_editor.set_data(state.plot_config)
         self.sensor_id_pidget.set_selected_sensor(state.sensor_id, app_model.connected_sensors)
         self.sensor_id_pidget.setEnabled(app_model.plugin_state.is_steady)
 
         self.start_button.setEnabled(
             app_model.is_ready_for_session() and self.config_editor.is_ready
         )
         self.stop_button.setEnabled(app_model.plugin_state == PluginState.LOADED_BUSY)
 
-    def _on_config_update(self, config: RefAppConfig) -> None:
+    def _on_config_update(self, config: ExampleAppConfig) -> None:
         BackendPlugin.update_config.rpc(self.app_model.put_task, config=config)
 
-    def _on_plot_config_update(self, config: PlotConfig) -> None:
-        BackendPlugin.update_plot_config.rpc(self.app_model.put_task, config=config)
-
     def _send_defaults_request(self) -> None:
         BackendPlugin.restore_defaults.rpc(self.app_model.put_task)
 
     def _on_sensor_id_update(self, sensor_id: int) -> None:
         BackendPlugin.update_sensor_id.rpc(self.app_model.put_task, sensor_id=sensor_id)
 
 
@@ -533,32 +557,18 @@
 
     def create_plot_plugin(
         self, app_model: AppModel, plot_layout: pg.GraphicsLayout
     ) -> PlotPlugin:
         return PlotPlugin(app_model=app_model, plot_layout=plot_layout)
 
 
-SMART_PRESENCE_PLUGIN = PluginSpec(
+SURFACE_VELOCITY_PLUGIN = PluginSpec(
     generation=PluginGeneration.A121,
-    key="smart_presence",
-    title="Smart presence",
-    description="Split presence detection range into zones.",
-    family=PluginFamily.REF_APP,
+    key="surface_velocity",
+    title="Surface velocity",
+    description="Estimate surface speed and direction of streaming water.",
+    family=PluginFamily.EXAMPLE_APP,
     presets=[
-        PluginPresetBase(
-            name="Short range",
-            description="Short range",
-            preset_id=PluginPresetId.SHORT_RANGE,
-        ),
-        PluginPresetBase(
-            name="Medium range",
-            description="Medium range",
-            preset_id=PluginPresetId.MEDIUM_RANGE,
-        ),
-        PluginPresetBase(
-            name="Long range",
-            description="Long range",
-            preset_id=PluginPresetId.LONG_RANGE,
-        ),
+        PluginPresetBase(name="Default", preset_id=PluginPresetId.DEFAULT),
     ],
-    default_preset_id=PluginPresetId.MEDIUM_RANGE,
+    default_preset_id=PluginPresetId.DEFAULT,
 )
```

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/smart_presence/_serializer.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/smart_presence/_serializer.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/sparse_iq/_plugin.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/sparse_iq/_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/sparse_iq/_processor.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/sparse_iq/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/sparse_iq/_serializers.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/sparse_iq/_serializers.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/surface_velocity/_example_app.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/surface_velocity/_example_app.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/surface_velocity/_example_app_plugin.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/speed/_detector_plugin.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Acconeer AB, 2023
+# Copyright (c) Acconeer AB, 2022-2023
 # All rights reserved
 
 from __future__ import annotations
 
 import logging
 from enum import Enum, auto
 from typing import Callable, Mapping, Optional
@@ -19,67 +19,72 @@
 from acconeer.exptool import a121
 from acconeer.exptool.a121._h5_utils import _create_h5_string_dataset
 from acconeer.exptool.a121.algo._plugins import (
     DetectorBackendPluginBase,
     DetectorPlotPluginBase,
     DetectorViewPluginBase,
 )
+from acconeer.exptool.a121.algo._utils import estimate_frame_rate
 from acconeer.exptool.app.new import (
     AppModel,
     AttrsConfigEditor,
     BackendLogger,
     GeneralMessage,
-    GridGroupBox,
+    GroupBox,
     Message,
     MiscErrorView,
-    PidgetFactoryMapping,
+    PidgetGroupFactoryMapping,
     PluginFamily,
     PluginGeneration,
     PluginPresetBase,
     PluginSpecBase,
     PluginState,
-    VerticalGroupBox,
     icons,
     is_task,
     pidgets,
 )
+from acconeer.exptool.app.new.ui.plugin_components import CollapsibleWidget, SensorConfigEditor
 from acconeer.exptool.app.new.ui.plugin_components.range_help_view import RangeHelpView
+from acconeer.exptool.app.new.ui.stream_tab.plugin_widget import PluginPlotArea
 
-from ._example_app import ExampleApp, ExampleAppConfig, ExampleAppResult, _load_algo_data
+from ._configs import get_default_config, get_traffic_config
+from ._detector import Detector, DetectorConfig, DetectorMetadata, DetectorResult, _load_algo_data
 
 
 @attrs.mutable(kw_only=True)
 class SharedState:
     sensor_id: int = attrs.field(default=1)
-    config: ExampleAppConfig = attrs.field(factory=ExampleAppConfig)
+    config: DetectorConfig = attrs.field(factory=DetectorConfig)
 
 
 class PluginPresetId(Enum):
     DEFAULT = auto()
+    TRAFFIC = auto()
 
 
 class BackendPlugin(DetectorBackendPluginBase[SharedState]):
 
-    PLUGIN_PRESETS: Mapping[int, Callable[[], ExampleAppConfig]] = {
-        PluginPresetId.DEFAULT.value: lambda: ExampleAppConfig()
+    PLUGIN_PRESETS: Mapping[int, Callable[[], DetectorConfig]] = {
+        PluginPresetId.DEFAULT.value: lambda: get_default_config(),
+        PluginPresetId.TRAFFIC.value: lambda: get_traffic_config(),
     }
 
     def __init__(
         self, callback: Callable[[Message], None], generation: PluginGeneration, key: str
     ) -> None:
         super().__init__(callback=callback, generation=generation, key=key)
 
         self._recorder: Optional[a121.H5Recorder] = None
-        self._exempel_app_instance: Optional[ExampleApp] = None
+        self._detector_instance: Optional[Detector] = None
         self._log = BackendLogger.getLogger(__name__)
 
         self.restore_defaults()
 
     def _load_from_cache(self, file: h5py.File) -> None:
-        self.shared_state.config = ExampleAppConfig.from_json(file["config"][()])
+        self.shared_state.config = DetectorConfig.from_json(file["config"][()])
 
     @is_task
     def restore_defaults(self) -> None:
         self.shared_state = SharedState()
         self.broadcast()
 
     @is_task
@@ -91,15 +96,15 @@
         if self.client is not None:
             sensor_ids = self.client.server_info.connected_sensors
 
             if len(sensor_ids) > 0 and self.shared_state.sensor_id not in sensor_ids:
                 self.shared_state.sensor_id = sensor_ids[0]
 
     @is_task
-    def update_config(self, *, config: ExampleAppConfig) -> None:
+    def update_config(self, *, config: DetectorConfig) -> None:
         self.shared_state.config = config
         self.broadcast()
 
     def save_to_cache(self, file: h5py.File) -> None:
         _create_h5_string_dataset(file, "config", self.shared_state.config.to_json())
 
     @is_task
@@ -112,222 +117,234 @@
         algo_group = record.get_algo_group(self.key)
         _, config = _load_algo_data(algo_group)
         self.shared_state.config = config
         self.shared_state.sensor_id = record.sensor_id
 
     def _start_session(self, recorder: Optional[a121.H5Recorder]) -> None:
         assert self.client
-        self._example_app_instance = ExampleApp(
+        self._detector_instance = Detector(
             client=self.client,
             sensor_id=self.shared_state.sensor_id,
-            example_app_config=self.shared_state.config,
+            detector_config=self.shared_state.config,
         )
-        self._example_app_instance.start(recorder)
+        sensor_config = self._detector_instance._get_sensor_config(self._detector_instance.config)
+        session_config = a121.SessionConfig(
+            {self.shared_state.sensor_id: sensor_config},
+            extended=False,
+        )
+
+        estimated_frame_rate = estimate_frame_rate(self.client, session_config)
+
+        self._detector_instance.start(recorder)
         self.callback(
             GeneralMessage(
                 name="setup",
                 kwargs=dict(
-                    example_app_config=self.shared_state.config,
+                    detector_config=self.shared_state.config,
+                    detector_metadata=self._detector_instance.detector_metadata,
+                    estimated_frame_rate=estimated_frame_rate,
                 ),
                 recipient="plot_plugin",
             )
         )
 
     def end_session(self) -> None:
-        if self._example_app_instance is None:
+        if self._detector_instance is None:
             raise RuntimeError
-        if self._recorder is not None:
-            self._recorder.close()
-        self._example_app_instance.stop()
+        self._detector_instance.stop()
 
     def get_next(self) -> None:
         assert self.client
-        if self._example_app_instance is None:
+        if self._detector_instance is None:
             raise RuntimeError
-        result = self._example_app_instance.get_next()
+        result = self._detector_instance.get_next()
 
         self.callback(GeneralMessage(name="plot", data=result, recipient="plot_plugin"))
 
 
 class PlotPlugin(DetectorPlotPluginBase):
-
-    _VELOCITY_Y_SCALE_MARGIN_M = 0.25
-
     def __init__(self, *, plot_layout: pg.GraphicsLayout, app_model: AppModel) -> None:
         super().__init__(plot_layout=plot_layout, app_model=app_model)
 
     def setup_from_message(self, message: GeneralMessage) -> None:
         assert message.kwargs is not None
         self.setup(**message.kwargs)
 
     def update_from_message(self, message: GeneralMessage) -> None:
-        assert isinstance(message.data, ExampleAppResult)
+        assert isinstance(message.data, DetectorResult)
         self.update(message.data)
 
     def setup(
         self,
-        example_app_config: ExampleAppConfig,
+        detector_config: DetectorConfig,
+        detector_metadata: DetectorMetadata,
+        estimated_frame_rate: float,
     ) -> None:
+        self.detector_config = detector_config
 
-        self.slow_zone = example_app_config.slow_zone
-        self.history_length_s = 10
-        if example_app_config.frame_rate is None:
-            estimated_frame_rate = (
-                example_app_config.sweep_rate / example_app_config.sweeps_per_frame
-            )
-        else:
-            estimated_frame_rate = example_app_config.frame_rate
+        self.n_depths = detector_metadata.num_points
 
-        self.history_length_n = int(np.around(self.history_length_s * estimated_frame_rate))
+        max_update_rate = PluginPlotArea._FPS
 
-        c0_dashed_pen = et.utils.pg_pen_cycler(0, width=2.5, style="--")
+        if estimated_frame_rate > max_update_rate:
+            plugin_frame_rate = float(max_update_rate)
+        else:
+            plugin_frame_rate = estimated_frame_rate
 
-        # Velocity plot
+        self.history_length_s = 10.0
+        self.history_length = int(self.history_length_s * plugin_frame_rate)
 
-        self.velocity_history_plot = self._create_plot(self.plot_layout, row=0, col=0)
-        self.velocity_history_plot.setTitle("Estimated velocity")
-        self.velocity_history_plot.setLabel(axis="left", text="Velocity", units="m/s")
-        self.velocity_history_plot.setLabel(axis="bottom", text="Time", units="s")
-        self.velocity_history_plot.addLegend(labelTextSize="10pt")
-        self.velocity_smooth_limits = et.utils.SmoothLimits()
+        self.time_window_length_s = 3.0
+        self.time_window_length_n = int(self.time_window_length_s * plugin_frame_rate)
 
-        self.velocity_curve = self.velocity_history_plot.plot(
-            pen=et.utils.pg_pen_cycler(0), name="Estimated velocity"
-        )
+        self.speed_history = np.zeros(self.history_length)
+        self.speed_history_xs = np.array([i for i in range(-self.history_length, 0)])
+
+        n_ticks_to_display = 10
+        x_labels = np.linspace(-self.history_length_s, 0, self.history_length)
+        all_ticks = [
+            (t, "{:.0f}".format(label)) for t, label in zip(self.speed_history_xs, x_labels)
+        ]
+        subsample_step = self.history_length // n_ticks_to_display
+        display_ticks = [all_ticks[::subsample_step]]
+
+        win = self.plot_layout
+
+        # FFT plot
+
+        self.raw_fft_plot = win.addPlot(row=1, col=0)
+        self.raw_fft_plot.setTitle("Frequency data")
+        self.raw_fft_plot.setLabel(axis="left", text="Amplitude")
+        self.raw_fft_plot.setLabel(axis="bottom", text="Frequency", units="Hz")
+        self.raw_fft_plot.addLegend(labelTextSize="10pt")
+        self.raw_fft_limits = et.utils.SmoothLimits()
+        self.raw_fft_plot.setMenuEnabled(False)
+        self.raw_fft_plot.setMouseEnabled(x=False, y=False)
+        self.raw_fft_plot.hideButtons()
+        self.raw_fft_plot.showGrid(x=True, y=True)
+        self.raw_fft_plot.setLogMode(x=False, y=True)
+        self.raw_fft_curves = []
+        self.raw_fft_smooth_max = et.utils.SmoothMax(self.detector_config.frame_rate)
+        self.raw_thresholds_curves = []
+
+        for i in range(self.n_depths):
+            raw_fft_curve = self.raw_fft_plot.plot(pen=et.utils.pg_pen_cycler(i), name="Fft")
+            threshold_curve = self.raw_fft_plot.plot(
+                pen=et.utils.pg_pen_cycler(i), name="Threshold"
+            )
+            self.raw_fft_curves.append(raw_fft_curve)
+            self.raw_thresholds_curves.append(threshold_curve)
 
-        self.psd_html = (
+        self.speed_history_plot = win.addPlot(row=0, col=0)
+        self.speed_history_plot.setTitle("Speed history")
+        self.speed_history_plot.setLabel(axis="left", text="Speed", units="m/s")
+        self.speed_history_plot.setLabel(axis="bottom", text="Time", units="Seconds")
+        self.speed_history_plot.addLegend(labelTextSize="10pt")
+        self.speed_history_curve = self.speed_history_plot.plot(
+            pen=None,
+            name="speed",
+            symbol="o",
+            symbolsize=3,
+        )
+
+        if detector_config.sweep_rate is not None:
+            actual_max_speed = detector_config._get_max_speed(detector_config.sweep_rate)
+            self.speed_history_plot.setYRange(-actual_max_speed, actual_max_speed)
+        else:
+            self.speed_history_plot.setYRange(
+                -detector_config.max_speed, detector_config.max_speed
+            )
+        self.speed_history_plot.setXRange(-self.history_length, 0)
+        ay = self.speed_history_plot.getAxis("bottom")
+        ay.setTicks(display_ticks)
+
+        self.speed_html_format = (
             '<div style="text-align: center">'
-            '<span style="color: #FFFFFF;font-size:13pt;">'
+            '<span style="color: #FFFFFF;font-size:15pt;">'
             "{}</span></div>"
         )
 
-        self.distance_text_item = pg.TextItem(
-            html=self.psd_html,
-            fill=pg.mkColor(0x1F, 0x77, 0xB4, 180),
-            anchor=(0.5, 0),
-        )
-
-        self.velocity_history_plot.addItem(self.distance_text_item)
-
-        self.velocity_history = np.zeros(self.history_length_n)
-
-        self.lower_std_history = np.zeros(self.history_length_n)
-        self.upper_std_history = np.zeros(self.history_length_n)
-
-        self.lower_std_curve = self.velocity_history_plot.plot()
-        self.upper_std_curve = self.velocity_history_plot.plot()
-
-        fbi = pg.FillBetweenItem(
-            self.lower_std_curve,
-            self.upper_std_curve,
-            brush=pg.mkBrush(f"{et.utils.color_cycler(0)}50"),
+        self.speed_text_item = pg.TextItem(
+            fill=pg.mkColor(0xFF, 0x7F, 0x0E, 200),
+            anchor=(0.5, 0.5),
         )
 
-        self.velocity_history_plot.addItem(fbi)
-
-        # PSD plot
-
-        self.psd_plot = self._create_plot(self.plot_layout, row=1, col=0)
-        self.psd_plot.setTitle("PSD<br>(colored area represents the slow zone)")
-        self.psd_plot.setLabel(axis="left", text="Power")
-        self.psd_plot.setLabel(axis="bottom", text="Velocity", units="m/s")
-        self.psd_plot.addLegend(labelTextSize="10pt")
-
-        self.psd_smooth_max = et.utils.SmoothMax(tau_grow=0.5, tau_decay=2.0)
-        self.psd_curve = self.psd_plot.plot(pen=et.utils.pg_pen_cycler(0), name="PSD")
-        self.psd_threshold = self.psd_plot.plot(pen=c0_dashed_pen, name="Threshold")
-
-        psd_slow_zone_color = et.utils.color_cycler(0)
-        psd_slow_zone_color = f"{psd_slow_zone_color}50"
-        psd_slow_zone_brush = pg.mkBrush(psd_slow_zone_color)
-
-        self.psd_slow_zone = pg.LinearRegionItem(brush=psd_slow_zone_brush, movable=False)
-        self.psd_plot.addItem(self.psd_slow_zone)
-
-        brush = et.utils.pg_brush_cycler(0)
-        self.psd_peak_plot_item = pg.PlotDataItem(
+        self.speed_text_item.setPos(-self.history_length / 2, -detector_config.max_speed / 2)
+        brush = et.utils.pg_brush_cycler(1)
+        self.speed_history_peak_plot_item = pg.PlotDataItem(
             pen=None, symbol="o", symbolSize=8, symbolBrush=brush, symbolPen="k"
         )
-        self.psd_plot.addItem(self.psd_peak_plot_item)
-
-        self.psd_plot.setLogMode(x=False, y=True)
+        self.speed_history_plot.addItem(self.speed_history_peak_plot_item)
+        self.speed_history_plot.addItem(self.speed_text_item)
 
-    def update(self, example_app_result: ExampleAppResult) -> None:
-        processor_extra_result = example_app_result.processor_extra_result
+        self.speed_text_item.hide()
 
-        lim = self.velocity_smooth_limits.update(example_app_result.velocity)
+    def update(self, data: DetectorResult) -> None:
 
-        self.velocity_history_plot.setYRange(
-            lim[0] - self._VELOCITY_Y_SCALE_MARGIN_M, lim[1] + self._VELOCITY_Y_SCALE_MARGIN_M
-        )
-        self.velocity_history_plot.setXRange(-self.history_length_s, 0)
-
-        xs = np.linspace(-self.history_length_s, 0, self.history_length_n)
-
-        self.velocity_history = np.roll(self.velocity_history, -1)
-        self.velocity_history[-1] = example_app_result.velocity
-        self.velocity_curve.setData(xs, self.velocity_history)
-
-        velocity_html = self.psd_html.format(
-            f"Distance {np.around(example_app_result.distance_m, 2)} m"
-        )
-        self.distance_text_item.setHtml(velocity_html)
-        self.distance_text_item.setPos(
-            -self.history_length_s / 2, lim[1] + self._VELOCITY_Y_SCALE_MARGIN_M
-        )
-
-        self.lower_std_history = np.roll(self.lower_std_history, -1)
-        self.lower_std_history[-1] = (
-            example_app_result.velocity + 0.5 * processor_extra_result.peak_width
-        )
-        self.lower_std_curve.setData(xs, self.lower_std_history)
-
-        self.upper_std_history = np.roll(self.upper_std_history, -1)
-        self.upper_std_history[-1] = (
-            example_app_result.velocity - 0.5 * processor_extra_result.peak_width
-        )
-        self.upper_std_curve.setData(xs, self.upper_std_history)
+        psd = data.extra_result.psd
+        speed_guess = data.max_speed
+        x_speeds = data.extra_result.velocities
+        thresholds = data.extra_result.actual_thresholds
+
+        self.speed_history = np.roll(self.speed_history, -1)
+
+        self.speed_history[-1] = speed_guess
+
+        if self.time_window_length_n > 0:
+            pos_speed = np.max(self.speed_history[-self.time_window_length_n :])
+            pos_ind = int(np.argmax(self.speed_history[-self.time_window_length_n :]))
+            neg_speed = np.min(self.speed_history[-self.time_window_length_n :])
+            neg_ind = int(np.argmin(self.speed_history[-self.time_window_length_n :]))
+
+            if abs(neg_speed) > abs(pos_speed):
+                max_display_speed = neg_speed
+                max_display_ind = neg_ind
+            else:
+                max_display_speed = pos_speed
+                max_display_ind = pos_ind
+        else:
+            max_display_speed = self.speed_history[-1]
+            max_display_ind = -1
 
-        lim = self.psd_smooth_max.update(processor_extra_result.psd_threshold)
-        self.psd_plot.setYRange(np.log10(0.2), np.log10(lim))
-        self.psd_plot.setXRange(
-            processor_extra_result.max_bin_vertical_vs[0],
-            processor_extra_result.max_bin_vertical_vs[-1],
-        )
-        self.psd_curve.setData(
-            processor_extra_result.vertical_velocities, processor_extra_result.psd
-        )
-        self.psd_threshold.setData(
-            processor_extra_result.vertical_velocities, processor_extra_result.psd_threshold
-        )
-        if processor_extra_result.peak_idx is not None:
-            self.psd_peak_plot_item.setData(
-                [processor_extra_result.vertical_velocities[processor_extra_result.peak_idx]],
-                [processor_extra_result.psd[processor_extra_result.peak_idx]],
+        if max_display_speed != 0.0:
+            speed_text = "Max speed estimate {:.4f} m/s".format(max_display_speed)
+            speed_html = self.speed_html_format.format(speed_text)
+
+            self.speed_text_item.setHtml(speed_html)
+            self.speed_text_item.show()
+
+            sub_xs = self.speed_history_xs[-self.time_window_length_n :]
+            self.speed_history_peak_plot_item.setData(
+                [sub_xs[max_display_ind]], [max_display_speed]
             )
         else:
-            self.psd_peak_plot_item.clear()
+            self.speed_history_peak_plot_item.clear()
+            self.speed_text_item.hide()
 
-        middle_idx = int(np.around(processor_extra_result.vertical_velocities.shape[0] / 2))
-        self.psd_slow_zone.setRegion(
-            [
-                processor_extra_result.vertical_velocities[middle_idx - self.slow_zone],
-                processor_extra_result.vertical_velocities[middle_idx + self.slow_zone],
-            ]
-        )
-
-    @staticmethod
-    def _create_plot(parent: pg.GraphicsLayout, row: int, col: int) -> pg.PlotItem:
-        velocity_history_plot = parent.addPlot(row=row, col=col)
-        velocity_history_plot.setMenuEnabled(False)
-        velocity_history_plot.setMouseEnabled(x=False, y=False)
-        velocity_history_plot.hideButtons()
-        velocity_history_plot.showGrid(x=True, y=True, alpha=0.5)
+        display_inds = np.array([i for i, x in enumerate(self.speed_history) if x != 0.0])
+        if len(display_inds) > 0:
+            display_xs = self.speed_history_xs[display_inds]
+            display_data = self.speed_history[display_inds]
+        else:
+            display_xs = []
+            display_data = []
+        self.speed_history_curve.setData(display_xs, display_data)
+
+        assert psd is not None
+        assert thresholds is not None
+
+        top_max = max(np.max(psd), np.max(thresholds))
+
+        smooth_max_val = np.log10(self.raw_fft_smooth_max.update(top_max))
+        self.raw_fft_plot.setYRange(-2, smooth_max_val)
+        for i in range(psd.shape[1]):
+            self.raw_fft_curves[i].setData(x_speeds, psd[:, i])
 
-        return velocity_history_plot
+            threshold_line = np.full(x_speeds.shape[0], thresholds[i])
+            self.raw_thresholds_curves[i].setData(x_speeds, threshold_line)
 
 
 class ViewPlugin(DetectorViewPluginBase):
     def __init__(self, app_model: AppModel, view_widget: QWidget) -> None:
         super().__init__(app_model=app_model, view_widget=view_widget)
         self._log = logging.getLogger(__name__)
 
@@ -342,179 +359,136 @@
         self.start_button.clicked.connect(self._send_start_request)
 
         self.stop_button = QPushButton(icons.STOP(), "Stop")
         self.stop_button.setShortcut("space")
         self.stop_button.setToolTip("Stops the session.\n\nShortcut: Space")
         self.stop_button.clicked.connect(self._send_stop_request)
 
-        button_group = GridGroupBox("Controls", parent=self.sticky_widget)
+        button_group = GroupBox.grid("Controls", parent=self.sticky_widget)
         button_group.layout().addWidget(self.start_button, 0, 0)
         button_group.layout().addWidget(self.stop_button, 0, 1)
 
         sticky_layout.addWidget(button_group)
 
         self.misc_error_view = MiscErrorView(self.scrolly_widget)
         scrolly_layout.addWidget(self.misc_error_view)
 
-        sensor_selection_group = VerticalGroupBox("Sensor selection", parent=self.scrolly_widget)
+        sensor_selection_group = GroupBox.vertical("Sensor selection", parent=self.scrolly_widget)
         self.sensor_id_pidget = pidgets.SensorIdPidgetFactory(items=[]).create(
             parent=sensor_selection_group
         )
         self.sensor_id_pidget.sig_update.connect(self._on_sensor_id_update)
         sensor_selection_group.layout().addWidget(self.sensor_id_pidget)
         scrolly_layout.addWidget(sensor_selection_group)
 
-        self.range_helper = RangeHelpView()
-        scrolly_layout.addWidget(self.range_helper)
-
-        self.config_editor = AttrsConfigEditor[ExampleAppConfig](
-            title="Example app parameters",
+        self.config_editor = AttrsConfigEditor[DetectorConfig](
+            title="Detector parameters",
             factory_mapping=self._get_pidget_mapping(),
+            config_type=DetectorConfig,
             parent=self.scrolly_widget,
         )
         self.config_editor.sig_update.connect(self._on_config_update)
+
+        self.range_help_view = RangeHelpView()
+        scrolly_layout.addWidget(self.range_help_view)
+
         scrolly_layout.addWidget(self.config_editor)
 
+        self.sensor_config_status = SensorConfigEditor()
+        self.sensor_config_status.set_read_only(True)
+        collapsible_widget = CollapsibleWidget(
+            "Current sensor settings", self.sensor_config_status, self.scrolly_widget
+        )
+        scrolly_layout.addWidget(collapsible_widget)
+
         self.sticky_widget.setLayout(sticky_layout)
         self.scrolly_widget.setLayout(scrolly_layout)
 
     @classmethod
-    def _get_pidget_mapping(cls) -> PidgetFactoryMapping:
-        return {
-            "surface_distance": pidgets.FloatPidgetFactory(
-                name_label_text="Surface distance",
-                suffix=" m",
-                decimals=2,
-                limits=(0.1, 3),
-            ),
-            "sensor_angle": pidgets.FloatPidgetFactory(
-                name_label_text="Sensor angle",
-                suffix=" degrees",
-                decimals=1,
-                limits=(0, 89),
+    def _get_pidget_mapping(cls) -> PidgetGroupFactoryMapping:
+        service_parameters = {
+            "start_point": pidgets.IntPidgetFactory(
+                name_label_text="Start point",
             ),
             "num_points": pidgets.IntPidgetFactory(
-                name_label_text="Number of distance points",
-                limits=(1, None),
-            ),
-            "sweep_rate": pidgets.FloatPidgetFactory(
-                name_label_text="Sweep rate",
-                suffix=" Hz",
-                decimals=1,
-                limits=(100, None),
-            ),
-            "sweeps_per_frame": pidgets.IntPidgetFactory(
-                name_label_text="Sweeps per frame",
-                limits=(64, 2048),
+                name_label_text="Number of points",
+                limits=(1, 100),
             ),
-            "hwaas": pidgets.IntPidgetFactory(
-                name_label_text="HWAAS",
-                limits=(1, 511),
+            "step_length": pidgets.OptionalIntPidgetFactory(
+                name_label_text="Step length",
+                checkbox_label_text="Override",
+                limits=(1, None),
+                init_set_value=72,
             ),
             "profile": pidgets.OptionalEnumPidgetFactory(
                 name_label_text="Profile",
                 checkbox_label_text="Override",
                 enum_type=a121.Profile,
                 label_mapping={
                     a121.Profile.PROFILE_1: "1 (shortest)",
                     a121.Profile.PROFILE_2: "2",
                     a121.Profile.PROFILE_3: "3",
                     a121.Profile.PROFILE_4: "4",
                     a121.Profile.PROFILE_5: "5 (longest)",
                 },
             ),
-            "step_length": pidgets.IntPidgetFactory(
-                name_label_text="Step length:",
-                limits=(1, None),
+            "sweep_rate": pidgets.OptionalIntPidgetFactory(
+                name_label_text="Sweep rate",
+                suffix=" Hz",
+                checkbox_label_text="Override",
+                limits=(1, 134000),
+                init_set_value=10000,
             ),
             "frame_rate": pidgets.OptionalFloatPidgetFactory(
                 name_label_text="Frame rate",
-                checkbox_label_text="Limit",
                 suffix=" Hz",
-                decimals=1,
-                limits=(1, None),
-                init_set_value=10,
-            ),
-            "continuous_sweep_mode": pidgets.CheckboxPidgetFactory(
-                name_label_text="Continuos sweep mode",
-            ),
-            "double_buffering": pidgets.CheckboxPidgetFactory(
-                name_label_text="Double buffering",
-            ),
-            "inter_frame_idle_state": pidgets.EnumPidgetFactory(
-                enum_type=a121.IdleState,
-                name_label_text="Inter frame idle state",
-                label_mapping={
-                    a121.IdleState.DEEP_SLEEP: "Deep sleep",
-                    a121.IdleState.SLEEP: "Sleep",
-                    a121.IdleState.READY: "Ready",
-                },
-            ),
-            "inter_sweep_idle_state": pidgets.EnumPidgetFactory(
-                enum_type=a121.IdleState,
-                name_label_text="Inter sweep idle state",
-                label_mapping={
-                    a121.IdleState.DEEP_SLEEP: "Deep sleep",
-                    a121.IdleState.SLEEP: "Sleep",
-                    a121.IdleState.READY: "Ready",
-                },
-            ),
-            "time_series_length": pidgets.IntPidgetFactory(
-                name_label_text="Time series length",
-                limits=(64, None),
-            ),
-            "psd_lp_coeff": pidgets.FloatSliderPidgetFactory(
-                name_label_text="PSD time filtering coeff.",
-                limits=(0, 1),
-                decimals=3,
-            ),
-            "slow_zone": pidgets.IntPidgetFactory(
-                name_label_text="Slow zone half length",
-                limits=(0, 20),
-            ),
-            "velocity_lp_coeff": pidgets.FloatSliderPidgetFactory(
-                name_label_text="Velocity time filtering coeff.\nper time series",
-                limits=(0, 1),
-                decimals=3,
-            ),
-            "cfar_win": pidgets.IntPidgetFactory(
-                name_label_text="CFAR window length",
-                limits=(0, 20),
+                checkbox_label_text="Override",
+                limits=(1, 200),
+                init_set_value=20.0,
             ),
-            "cfar_guard": pidgets.IntPidgetFactory(
-                name_label_text="CFAR guard length",
-                limits=(0, 20),
+            "hwaas": pidgets.OptionalIntPidgetFactory(
+                name_label_text="HWAAS",
+                checkbox_label_text="Override",
+                limits=(1, 511),
+                init_set_value=4,
             ),
-            "cfar_sensitivity": pidgets.FloatSliderPidgetFactory(
-                name_label_text="Threshold sensitivity",
-                decimals=2,
-                limits=(0.01, 1),
+            "num_bins": pidgets.IntPidgetFactory(
+                name_label_text="Number of bins",
+                limits=(3, 4095),
             ),
-            "max_peak_interval_s": pidgets.FloatPidgetFactory(
-                name_label_text="Max peak interval",
-                decimals=1,
-                limits=(0, 20),
-                suffix=" s",
+        }
+        processing_parameters = {
+            "max_speed": pidgets.FloatPidgetFactory(
+                name_label_text="Max speed",
+                suffix=" m/s",
+                limits=(0, 150.0),
+            ),
+            "threshold": pidgets.FloatPidgetFactory(
+                name_label_text="Detection threshold",
+                limits=(1.0, 10000.0),
             ),
         }
+        return {
+            pidgets.FlatPidgetGroup(): service_parameters,
+            pidgets.FlatPidgetGroup(): processing_parameters,
+        }
 
     def on_backend_state_update(self, backend_plugin_state: Optional[SharedState]) -> None:
         if backend_plugin_state is not None and backend_plugin_state.config is not None:
             results = backend_plugin_state.config._collect_validation_results()
 
             not_handled = self.config_editor.handle_validation_results(results)
 
             not_handled = self.misc_error_view.handle_validation_results(not_handled)
 
+            sensor_config = Detector._get_sensor_config(backend_plugin_state.config)
+            self.range_help_view.update(sensor_config.subsweep)
+            self.sensor_config_status.set_data(sensor_config)
             assert not_handled == []
 
-            self.range_helper.update(
-                ExampleApp._get_sensor_config(backend_plugin_state.config).subsweep
-            )
-
     def on_app_model_update(self, app_model: AppModel) -> None:
         state = app_model.backend_plugin_state
 
         if state is None:
             self.start_button.setEnabled(False)
             self.stop_button.setEnabled(False)
 
@@ -532,15 +506,15 @@
         self.sensor_id_pidget.setEnabled(app_model.plugin_state.is_steady)
 
         self.start_button.setEnabled(
             app_model.is_ready_for_session() and self.config_editor.is_ready
         )
         self.stop_button.setEnabled(app_model.plugin_state == PluginState.LOADED_BUSY)
 
-    def _on_config_update(self, config: ExampleAppConfig) -> None:
+    def _on_config_update(self, config: DetectorConfig) -> None:
         BackendPlugin.update_config.rpc(self.app_model.put_task, config=config)
 
     def _send_defaults_request(self) -> None:
         BackendPlugin.restore_defaults.rpc(self.app_model.put_task)
 
     def _on_sensor_id_update(self, sensor_id: int) -> None:
         BackendPlugin.update_sensor_id.rpc(self.app_model.put_task, sensor_id=sensor_id)
@@ -557,18 +531,27 @@
 
     def create_plot_plugin(
         self, app_model: AppModel, plot_layout: pg.GraphicsLayout
     ) -> PlotPlugin:
         return PlotPlugin(app_model=app_model, plot_layout=plot_layout)
 
 
-SURFACE_VELOCITY_PLUGIN = PluginSpec(
+SPEED_DETECTOR_PLUGIN = PluginSpec(
     generation=PluginGeneration.A121,
-    key="surface_velocity",
-    title="Surface velocity",
-    description="Estimate surface speed and direction of streaming water.",
-    family=PluginFamily.EXAMPLE_APP,
+    key="speed_detector",
+    title="Speed detector",
+    description="Measure speed.",
+    family=PluginFamily.DETECTOR,
     presets=[
-        PluginPresetBase(name="Default", preset_id=PluginPresetId.DEFAULT),
+        PluginPresetBase(
+            name="Default",
+            description="Default settings to validate functionality",
+            preset_id=PluginPresetId.DEFAULT,
+        ),
+        PluginPresetBase(
+            name="Traffic",
+            description="Settings to validate fast traffic",
+            preset_id=PluginPresetId.TRAFFIC,
+        ),
     ],
     default_preset_id=PluginPresetId.DEFAULT,
 )
```

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/surface_velocity/_processor.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/surface_velocity/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/tank_level/_configs.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/tank_level/_configs.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/tank_level/_plugin.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/tank_level/_plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) Acconeer AB, 2023
 # All rights reserved
 
 from __future__ import annotations
 
 import logging
 from enum import Enum, auto
-from typing import Callable, Mapping, Optional
+from typing import Any, Callable, Mapping, Optional
 
 import attrs
 import h5py
 import numpy as np
 
 from PySide6.QtWidgets import QLabel, QPushButton, QVBoxLayout, QWidget
 
@@ -38,30 +38,30 @@
     RefAppResult,
     _load_algo_data,
 )
 from acconeer.exptool.app.new import (
     AppModel,
     BackendLogger,
     GeneralMessage,
+    GroupBox,
     HandledException,
     Message,
     PluginFamily,
     PluginGeneration,
     PluginPresetBase,
     PluginSpecBase,
     PluginState,
     PluginStateMessage,
-    VerticalGroupBox,
     icons,
     is_task,
 )
 from acconeer.exptool.app.new.ui.plugin_components import (
     AttrsConfigEditor,
-    GridGroupBox,
     PidgetFactoryMapping,
+    PresentationType,
     pidgets,
 )
 
 
 NO_DETECTION_TIMEOUT = 50
 TIME_HISTORY_S = 30
 
@@ -514,42 +514,46 @@
 
         self.defaults_button = QPushButton(icons.RESTORE(), "Reset settings and calibrations")
         self.defaults_button.clicked.connect(self._send_defaults_request)
 
         self.message_box = QLabel(self.sticky_widget)
         self.message_box.setWordWrap(True)
 
-        button_group = GridGroupBox("Controls", parent=self.sticky_widget)
+        button_group = GroupBox.grid("Controls", parent=self.sticky_widget)
         button_group.layout().addWidget(self.start_button, 0, 0)
         button_group.layout().addWidget(self.stop_button, 0, 1)
         button_group.layout().addWidget(self.calibrate_detector_button, 1, 0, 1, -1)
         button_group.layout().addWidget(self.defaults_button, 3, 0, 1, -1)
         button_group.layout().addWidget(self.message_box, 4, 0, 1, -1)
 
         sticky_layout.addWidget(button_group)
 
-        sensor_selection_group = VerticalGroupBox("Sensor selection", parent=self.scrolly_widget)
+        sensor_selection_group = GroupBox.vertical("Sensor selection", parent=self.scrolly_widget)
         self.sensor_id_pidget = pidgets.SensorIdPidgetFactory(items=[]).create(
             parent=sensor_selection_group
         )
         self.sensor_id_pidget.sig_update.connect(self._on_sensor_id_update)
         sensor_selection_group.layout().addWidget(self.sensor_id_pidget)
         scrolly_layout.addWidget(sensor_selection_group)
 
-        self.tank_level_config_editor = AttrsConfigEditor[RefAppConfig](
+        self.tank_level_config_editor = AttrsConfigEditor(
             title="Tank level indicator parameters",
             factory_mapping=self._get_processor_pidget_mapping(),
+            config_type=RefAppConfig,
+            extra_presenter=_set_config_presenter,
             parent=self.scrolly_widget,
         )
         self.tank_level_config_editor.sig_update.connect(self._on_config_update)
         scrolly_layout.addWidget(self.tank_level_config_editor)
 
-        self.config_editor = AttrsConfigEditor[RefAppConfig](
+        self.config_editor = AttrsConfigEditor(
             title="Detector parameters",
             factory_mapping=self._get_detector_pidget_mapping(),
+            config_type=RefAppConfig,
+            save_load_buttons=False,
             parent=self.scrolly_widget,
         )
         self.config_editor.sig_update.connect(self._on_config_update)
         scrolly_layout.addWidget(self.config_editor)
 
         self.sticky_widget.setLayout(sticky_layout)
         self.scrolly_widget.setLayout(scrolly_layout)
@@ -695,14 +699,48 @@
     def _on_calibrate_detector(self) -> None:
         BackendPlugin.calibrate_detector.rpc(self.app_model.put_task)
 
     def _send_defaults_request(self) -> None:
         BackendPlugin.restore_defaults.rpc(self.app_model.put_task)
 
 
+def _set_config_presenter(instance: Any, presentation_type: PresentationType) -> Optional[str]:
+    if isinstance(instance, RefAppConfig) and presentation_type is PresentationType.C_SET_CONFIG:
+        config: RefAppConfig = instance
+        distance_config = config.to_detector_config()
+
+        return f"""
+static void set_config(acc_ref_app_tank_level_config_t *config, tank_level_preset_config_t preset)
+{{
+    // This snippet is generated to be compatible with RSS A121 v1.0.0
+    // If there is a version missmatch the snippet might need some modification
+
+    (void)preset;
+
+    config->tank_range_start_m     = {config.start_m:.3f}f;
+    config->tank_range_end_m       = {config.end_m:.3f}f;
+    config->median_filter_length   = {config.median_filter_length}U;
+    config->num_medians_to_average = {config.num_medians_to_average}U;
+
+    acc_detector_distance_config_start_set(config->distance_config, {distance_config.start_m:.3f}f);
+    acc_detector_distance_config_end_set(config->distance_config, {distance_config.end_m:.3f}f);
+    acc_detector_distance_config_max_step_length_set(config->distance_config, {distance_config.max_step_length or 0}U);
+    acc_detector_distance_config_max_profile_set(config->distance_config, ACC_CONFIG_{distance_config.max_profile.name});
+    acc_detector_distance_config_num_frames_recorded_threshold_set(config->distance_config, {distance_config.num_frames_in_recorded_threshold}U);
+    acc_detector_distance_config_peak_sorting_set(config->distance_config, ACC_DETECTOR_DISTANCE_PEAK_SORTING_{distance_config.peaksorting_method.name});
+    acc_detector_distance_config_reflector_shape_set(config->distance_config, ACC_DETECTOR_DISTANCE_REFLECTOR_SHAPE_{distance_config.reflector_shape.name});
+    acc_detector_distance_config_threshold_sensitivity_set(config->distance_config, {distance_config.threshold_sensitivity:.3f}f);
+    acc_detector_distance_config_signal_quality_set(config->distance_config, {distance_config.signal_quality:.3f}f);
+    acc_detector_distance_config_close_range_leakage_cancellation_set(config->distance_config, {str(distance_config.close_range_leakage_cancellation).lower()});
+}}
+"""
+
+    return None
+
+
 class PluginSpec(PluginSpecBase):
     def create_backend_plugin(
         self, callback: Callable[[Message], None], key: str
     ) -> BackendPlugin:
         return BackendPlugin(callback, generation=self.generation, key=key)
 
     def create_view_plugin(self, app_model: AppModel, view_widget: QWidget) -> ViewPlugin:
```

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/tank_level/_processor.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/tank_level/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/tank_level/_ref_app.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/tank_level/_ref_app.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/tank_level/_serializer.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/tank_level/_serializer.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/touchless_button/_blinkstick_updater.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/touchless_button/_blinkstick_updater.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/touchless_button/_configs.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/touchless_button/_configs.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/touchless_button/_plugin.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/touchless_button/_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/touchless_button/_processor.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/touchless_button/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/touchless_button/_serializers.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/a121/algo/touchless_button/_serializers.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/launcher.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/launcher.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/__init__.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,20 +21,18 @@
     PluginStateMessage,
     is_task,
 )
 from .pluginbase import PlotPluginBase, PluginPresetBase, PluginSpecBase, ViewPluginBase
 from .storage import get_temp_dir, get_temp_h5_path
 from .ui import (
     AttrsConfigEditor,
-    GridGroupBox,
-    HorizontalGroupBox,
+    GroupBox,
     MiscErrorView,
     PidgetFactoryMapping,
     PidgetGroupFactoryMapping,
     SessionConfigEditor,
     SmartMetadataView,
     SmartPerfCalcView,
     TwoSensorIdsEditor,
-    VerticalGroupBox,
     icons,
     pidgets,
 )
```

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/_argument_parser.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/_argument_parser.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/_enums.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/_enums.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/_version_checker.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/_version_checker.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/app.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/app.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/app_model/app_model.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/app_model/app_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -311,15 +311,15 @@
         *,
         on_ok: Optional[Callable[[], None]] = None,
         on_error: Optional[Callable[[Exception, Optional[str]], None]] = None,
     ) -> None:
         key = self._backend.put_task(task)
         self._backend_task_callbacks[key] = {
             "on_ok": on_ok,
-            "on_error": on_error,
+            "on_error": on_error or self.emit_error,
         }
 
         (name, _) = task
         log.debug(f"Put backend task with name: '{name}', key: {key.time_low}")
 
     def _handle_backend_closed_task(self, closed_task: ClosedTask) -> None:
         log.debug(f"Got backend closed task: {closed_task.key.time_low}")
```

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/app_model/app_model_listener.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/app_model/app_model_listener.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/app_model/file_detective.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/app_model/file_detective.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/app_model/port_updater.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/app_model/port_updater.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/backend/_application_client.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/backend/_application_client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/backend/_backend.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/backend/_backend.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/backend/_backend_logger.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/backend/_backend_logger.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/backend/_backend_plugin.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/backend/_backend_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/backend/_message.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/backend/_message.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/backend/_model.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/backend/_model.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/backend/_tasks.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/backend/_tasks.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/plugin_loader.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/plugin_loader.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,20 +4,21 @@
 from __future__ import annotations
 
 from .app_model import PluginSpec
 
 
 def load_default_plugins() -> list[PluginSpec]:
     from acconeer.exptool.a121.algo.bilateration._plugin import BILATERATION_PLUGIN
-    from acconeer.exptool.a121.algo.breathing._plugin import BREATHING_PLUGIN
+    from acconeer.exptool.a121.algo.breathing._ref_app_plugin import BREATHING_PLUGIN
     from acconeer.exptool.a121.algo.distance._detector_plugin import DISTANCE_DETECTOR_PLUGIN
     from acconeer.exptool.a121.algo.phase_tracking._plugin import PHASE_TRACKING_PLUGIN
     from acconeer.exptool.a121.algo.presence._detector_plugin import PRESENCE_DETECTOR_PLUGIN
     from acconeer.exptool.a121.algo.smart_presence._ref_app_plugin import SMART_PRESENCE_PLUGIN
     from acconeer.exptool.a121.algo.sparse_iq._plugin import SPARSE_IQ_PLUGIN
+    from acconeer.exptool.a121.algo.speed._detector_plugin import SPEED_DETECTOR_PLUGIN
     from acconeer.exptool.a121.algo.surface_velocity._example_app_plugin import (
         SURFACE_VELOCITY_PLUGIN,
     )
     from acconeer.exptool.a121.algo.tank_level._plugin import TANK_LEVEL_PLUGIN
     from acconeer.exptool.a121.algo.touchless_button._plugin import TOUCHLESS_BUTTON_PLUGIN
     from acconeer.exptool.a121.algo.vibration._plugin import VIBRATION_PLUGIN
 
@@ -30,8 +31,9 @@
         PRESENCE_DETECTOR_PLUGIN,
         SMART_PRESENCE_PLUGIN,
         SPARSE_IQ_PLUGIN,
         SURFACE_VELOCITY_PLUGIN,
         TANK_LEVEL_PLUGIN,
         TOUCHLESS_BUTTON_PLUGIN,
         VIBRATION_PLUGIN,
+        SPEED_DETECTOR_PLUGIN,
     ]
```

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/pluginbase/plot_plugin_base.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/pluginbase/plot_plugin_base.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/pluginbase/plugin_spec_base.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/pluginbase/plugin_spec_base.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/pluginbase/ui_plugin_base.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/pluginbase/ui_plugin_base.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/pluginbase/view_plugin_base.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/pluginbase/view_plugin_base.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/storage.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/storage.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/app_model_viewer.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/app_model_viewer.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/device_comboboxes.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/device_comboboxes.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/flash_tab/dialogs.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/flash_tab/dialogs.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/flash_tab/threads.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/flash_tab/threads.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/flash_tab/widgets.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/flash_tab/widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 )
 
 from acconeer.exptool.app import resources  # type: ignore[attr-defined]
 from acconeer.exptool.app.new._enums import ConnectionInterface
 from acconeer.exptool.app.new.app_model import AppModel
 from acconeer.exptool.app.new.ui import utils as ui_utils
 from acconeer.exptool.app.new.ui.device_comboboxes import SerialPortComboBox, USBDeviceComboBox
-from acconeer.exptool.app.new.ui.plugin_components.utils import VerticalGroupBox
+from acconeer.exptool.app.new.ui.plugin_components.utils import GroupBox
 from acconeer.exptool.flash import (  # type: ignore[import]
     DevLicense,
     clear_cookies,
     get_flash_download_name,
     get_flash_known_devices,
 )
 from acconeer.exptool.flash._products import (  # type: ignore[import]
@@ -138,15 +138,15 @@
         button_layout.addWidget(self.flash_button,             3,   0,   1,    12)    # noqa: E241
         button_layout.addWidget(self.logged_in_label,          4,   0,   1,     8)    # noqa: E241
         button_layout.addWidget(self.logout_button,            4,   8,   1,     4)    # noqa: E241
         button_layout.addWidget(self.download_spinner,         5,   0,   1,     1)    # noqa: E241
         button_layout.addWidget(self.download_status_label,    5,   1,   1,    11)    # noqa: E241
         # fmt: on
 
-        box = VerticalGroupBox("", self)
+        box = GroupBox.vertical("", parent=self)
         box.setSizePolicy(QSizePolicy.Policy.Fixed, QSizePolicy.Policy.Fixed)
         box.layout().addWidget(ui_utils.LayoutWrapper(button_layout))
 
         layout = QVBoxLayout()
         layout.setAlignment(Qt.AlignmentFlag.AlignCenter)
         layout.addWidget(box)
```

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/help_tab.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/help_tab.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/icons.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/icons.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 # A nice side-effect is that the "color" of the icon can be overridden by the caller
 #
 #     QLabel(ARROW_LEFT_BOLD(color="<my custom color>"), ...)
 #
 # fmt: off
 ARROW_LEFT_BOLD = partial(qta.icon, "ph.arrow-left-bold",        color=BUTTON_ICON_COLOR)
 CALIBRATE       = partial(qta.icon, "fa.circle",                 color=BUTTON_ICON_COLOR)
+CHECKMARK       = partial(qta.icon, "fa5s.check",                color=BUTTON_ICON_COLOR)
 COG             = partial(qta.icon, "fa5s.cog",                  color=BUTTON_ICON_COLOR)
 EXTERNAL_LINK   = partial(qta.icon, "fa5s.external-link-alt",    color=BUTTON_ICON_COLOR)
 FLASH           = partial(qta.icon, "mdi.flash",                 color=BUTTON_ICON_COLOR)
 FOLDER_OPEN     = partial(qta.icon, "fa.folder-open",            color=BUTTON_ICON_COLOR)
 HELP            = partial(qta.icon, "mdi6.help-circle",          color=BUTTON_ICON_COLOR)
 LINK            = partial(qta.icon, "fa5s.link",                 color=BUTTON_ICON_COLOR)
 PLAY            = partial(qta.icon, "fa5s.play-circle",          color=BUTTON_ICON_COLOR)
```

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/main_window.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/main_window.py`

 * *Files 7% similar despite different names*

```diff
@@ -65,51 +65,61 @@
         |B|      Page A      |
         +-+                  |
         | |                  |
         +-+------------------+
     """
 
     def __init__(
-        self, pages: t.Iterable[t.Tuple[QIcon, str, QWidget]], *, index_button_width: int = 60
+        self,
+        app_model: AppModel,
+        pages: t.Iterable[t.Tuple[QIcon, str, QWidget]],
+        *,
+        index_button_width: int = 60,
     ) -> None:
         super().__init__()
+        app_model.sig_notify.connect(self._on_app_model_update)
+
         self._index_button_group = QButtonGroup()
         self._index_button_layout = QVBoxLayout()
         self._index_button_layout.setContentsMargins(0, 0, 0, 0)
 
         self._page_widget = QStackedWidget()
 
         for i, (icon, text, page) in enumerate(pages):
             index_button = _IconButton(icon, text, is_active=i == 0)
 
             self._index_button_group.addButton(index_button, id=i)
             self._index_button_layout.addWidget(index_button)
             self._page_widget.addWidget(page)
 
         self._index_button_group.idClicked.connect(self._page_widget.setCurrentIndex)
-        index_button_widget = TopAlignDecorator(LayoutWrapper(self._index_button_layout))
-        index_button_widget.setFixedWidth(index_button_width)
-        self.addWidget(index_button_widget)
+        self._index_button_widget = TopAlignDecorator(LayoutWrapper(self._index_button_layout))
+        self._index_button_widget.setFixedWidth(index_button_width)
+        self.addWidget(self._index_button_widget)
         self.addWidget(self._page_widget)
         self.setCollapsible(1, False)
 
+    def _on_app_model_update(self, app_model: AppModel) -> None:
+        self._index_button_widget.setEnabled(app_model.plugin_state.is_steady)
+
 
 class MainWindow(QMainWindow):
     def __init__(self, app_model: AppModel) -> None:
         super().__init__()
 
         self.resize(1280, 720)
 
         self.setCentralWidget(
             _PagedLayout(
+                app_model,
                 [
                     (RECORD(), "Stream", StreamingMainWidget(app_model, self)),
                     (FLASH(), "Flash", FlashMainWidget(app_model, self)),
                     (HELP(), "Help", HelpMainWidget(self)),
-                ]
+                ],
             )
         )
 
         self.setStatusBar(StatusBar(app_model, self))
         self.setWindowTitle("Acconeer Exploration Tool")
         self.moveEvent = lambda _: self.saveGeometry()
```

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/misc.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/misc.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/__init__.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,13 +4,14 @@
 from . import pidgets
 from .attrs_config_editor import AttrsConfigEditor
 from .collapsible_widget import CollapsibleWidget
 from .data_editor import DataEditor
 from .metadata_view import ExtendedMetadataView, MetadataView, SmartMetadataView
 from .misc_error_view import MiscErrorView
 from .perf_calc_view import ExtendedPerfCalcView, PerfCalcView, SmartPerfCalcView
+from .save_dialog import PresentationType, PresenterFunc
 from .sensor_config_editor import SensorConfigEditor
 from .session_config_editor import SessionConfigEditor
 from .subsweep_config_editor import SubsweepConfigEditor
 from .two_sensor_ids_editor import TwoSensorIdsEditor
 from .types import PidgetFactoryMapping, PidgetGroupFactoryMapping
-from .utils import GridGroupBox, HorizontalGroupBox, VerticalGroupBox
+from .utils import GroupBox
```

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/attrs_config_editor.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/attrs_config_editor.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 # Copyright (c) Acconeer AB, 2022-2023
 # All rights reserved
 
 from __future__ import annotations
 
 import copy
 from functools import partial
-from typing import Any, Optional, Sequence, TypeVar, Union, cast
+from typing import Any, Optional, Sequence, Type, TypeVar, Union, cast
 
 import attrs
 
 from PySide6.QtCore import Signal
 from PySide6.QtWidgets import QVBoxLayout, QWidget
 
 from acconeer.exptool import a121
 from acconeer.exptool.a121._core import Criticality
 
 from .data_editor import DataEditor
+from .json_save_load_buttons import JsonPresentable, JsonSaveLoadButtons
 from .pidgets import FlatPidgetGroup, Pidget, PidgetGroup, PidgetGroupHook, PidgetHook
+from .save_dialog import PresenterFunc
 from .types import PidgetFactoryMapping, PidgetGroupFactoryMapping
-from .utils import VerticalGroupBox
+from .utils import GroupBox
 
 
-T = TypeVar("T")
+T = TypeVar("T", bound=JsonPresentable)
 
 
 def _to_group_factory_mapping(
     factory_mapping: Union[PidgetFactoryMapping, PidgetGroupFactoryMapping]
 ) -> PidgetGroupFactoryMapping:
     if factory_mapping == {}:
         return {}
@@ -55,22 +57,34 @@
 
     sig_update = Signal(object)
 
     def __init__(
         self,
         title: str,
         factory_mapping: Union[PidgetFactoryMapping, PidgetGroupFactoryMapping],
+        config_type: Type[T],
+        *,
+        save_load_buttons: bool = True,
+        extra_presenter: PresenterFunc = lambda i, t: None,
         parent: Optional[QWidget] = None,
     ) -> None:
         super().__init__(parent=parent)
         self._config = None
         self.setLayout(QVBoxLayout(self))
         self.layout().setContentsMargins(0, 0, 0, 0)
         self.layout().setSpacing(11)
-        group_box = VerticalGroupBox(title, parent=self)
+        group_box = GroupBox.vertical(
+            title,
+            right_header=(
+                JsonSaveLoadButtons.from_editor_and_config_type(self, config_type, extra_presenter)
+                if save_load_buttons
+                else None
+            ),
+            parent=self,
+        )
         self.layout().addWidget(group_box)
 
         self._pidget_mapping: dict[str, Pidget] = {}
         self._pidget_hooks: dict[str, Sequence[PidgetHook]] = {}
         self._group_widgets: list[QWidget] = []
         self._group_hooks: list[Sequence[PidgetGroupHook]] = []
         self._erroneous_aspects = set()
```

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/collapsible_widget.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/collapsible_widget.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/data_editor.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/data_editor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/metadata_view.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/metadata_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     QVBoxLayout,
     QWidget,
 )
 
 from acconeer.exptool import a121
 from acconeer.exptool.a121 import _core
 
-from .utils import VerticalGroupBox
+from .utils import GroupBox
 
 
 _WIDGET_WIDTH = 125
 
 
 class SmartMetadataView(QWidget):
     def __init__(self, parent: QWidget) -> None:
@@ -54,15 +54,15 @@
 
 
 class ExtendedMetadataView(QWidget):
     def __init__(self, parent: QWidget) -> None:
         super().__init__(parent)
         self.setLayout(QVBoxLayout(self))
 
-        group_box = VerticalGroupBox("Metadata", parent=self)
+        group_box = GroupBox.vertical("Metadata", parent=self)
         self.layout().addWidget(group_box)
 
         self._tab_widget = QTabWidget(parent=self)
         self._tab_widget.setStyleSheet(
             """
             QTabWidget::pane { border: none; }
             * {margin: 0;}
```

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/misc_error_view.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/misc_error_view.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/perf_calc_view.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/perf_calc_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,28 @@
-# Copyright (c) Acconeer AB, 2022
+# Copyright (c) Acconeer AB, 2022-2023
 # All rights reserved
 
 from __future__ import annotations
 
 from typing import Optional, Union
 
 from PySide6 import QtCore
-from PySide6.QtWidgets import QGridLayout, QGroupBox, QLabel, QLineEdit, QStackedLayout, QWidget
+from PySide6.QtWidgets import (
+    QGridLayout,
+    QGroupBox,
+    QLabel,
+    QLineEdit,
+    QStackedLayout,
+    QVBoxLayout,
+    QWidget,
+)
 
 from acconeer.exptool import a121
 
-from .utils import VerticalGroupBox
+from .utils import GroupBox
 
 
 _WIDGET_WIDTH = 125
 
 
 class SmartPerfCalcView(QWidget):
     def __init__(self, parent: QWidget) -> None:
@@ -37,17 +45,17 @@
             self._layout.setCurrentIndex(1)
             self._extended_perf_calc_view.update(session_config, metadata)
         else:
             self._layout.setCurrentIndex(0)
             self._perf_calc_view.update(session_config, metadata)
 
 
-class ExtendedPerfCalcView(VerticalGroupBox):
+class ExtendedPerfCalcView(GroupBox):
     def __init__(self, parent: QWidget) -> None:
-        super().__init__("Performance calculations", parent)
+        super().__init__("Performance calculations", QVBoxLayout, parent=parent)
 
         label = QLabel("No estimates available", self)
         label.setEnabled(False)
         label.setAlignment(QtCore.Qt.AlignCenter)
         self.layout().addWidget(label)
 
     def update(
```

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/__init__.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/__init__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/hooks.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/hooks.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidget_groups.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidget_groups.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidgets.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     QDoubleSpinBox,
     QGridLayout,
     QHBoxLayout,
     QLabel,
     QLayout,
     QSlider,
     QSpinBox,
+    QStackedWidget,
     QVBoxLayout,
     QWidget,
 )
 
 from acconeer.exptool.a121._core.entities import Criticality
 from acconeer.exptool.app.new.ui.plugin_components.data_editor import DataEditor
 
@@ -386,53 +387,86 @@
         else:
             return int(self._spin_box.value())
 
 
 @attrs.frozen(kw_only=True, slots=False)
 class OptionalFloatPidgetFactory(OptionalPidgetFactory, FloatPidgetFactory):
     init_set_value: Optional[float] = None
+    """
+    The initial value of the spinbox (ignoring the None-ness of the pidget)
+    """
+
+    placeholder_text: Optional[str] = None
+    """
+    Text that will be displayed when the checkbox is unchecked (and data is None).
+    placeholder_text = None disables the placeholder text entierly
+    """
 
     def create(self, parent: QWidget) -> OptionalFloatPidget:
         return OptionalFloatPidget(self, parent)
 
 
 class OptionalFloatPidget(OptionalPidget):
+    _SPINBOX_INDEX = 0
+    _DUMMY_INDEX = 1
+
     def __init__(self, factory: OptionalFloatPidgetFactory, parent: QWidget) -> None:
         super().__init__(factory, parent)
 
+        self._container = QStackedWidget()
         self._spin_box = _PidgetDoubleSpinBox(
-            self._optional_widget,
+            self._container,
             decimals=factory.decimals,
             limits=factory.limits,
             suffix=factory.suffix,
             init_set_value=factory.init_set_value,
         )
-        self._optional_layout.addWidget(self._spin_box)
 
+        self._container.addWidget(self._spin_box)
+
+        if factory.placeholder_text is None:
+            self._dummy_spin_box = None
+        else:
+            self._dummy_spin_box = _PidgetDoubleSpinBox.placeholder_dummy(
+                self._container, factory.placeholder_text
+            )
+            self._dummy_spin_box.setEnabled(False)
+            self._container.addWidget(self._dummy_spin_box)
+
+        self._optional_layout.addWidget(self._container)
         self._none_checkbox.stateChanged.connect(self.__on_changed)
         self._spin_box.valueChanged.connect(self.__on_changed)
 
     def __on_changed(self) -> None:
         checked = self._none_checkbox.isChecked()
 
         with QtCore.QSignalBlocker(self):
-            self._spin_box.setEnabled(checked)
+            if self._dummy_spin_box is None:
+                self._spin_box.setEnabled(checked)
+            else:
+                self._container.setCurrentIndex(
+                    self._SPINBOX_INDEX if checked else self._DUMMY_INDEX
+                )
 
         value = self._spin_box.value() if checked else None
         self.sig_update.emit(value)
 
     def set_data(self, value: Any) -> None:
         super().set_data(value)
 
-        with QtCore.QSignalBlocker(self):
-            if value is None:
-                self._spin_box.setEnabled(False)
-            else:
+        if value is not None:
+            with QtCore.QSignalBlocker(self):
                 self._spin_box.setValue(value)
-                self._spin_box.setEnabled(True)
+
+        if self._dummy_spin_box is None:
+            self._spin_box.setEnabled(value is not None)
+        else:
+            self._container.setCurrentIndex(
+                self._SPINBOX_INDEX if value is not None else self._DUMMY_INDEX
+            )
 
     def get_data(self) -> Optional[float]:
         if not self._none_checkbox.isChecked():
             return None
         else:
             return float(self._spin_box.value())
 
@@ -700,14 +734,26 @@
 
         if suffix:
             self.setSuffix(f" {suffix}")
 
         if init_set_value is not None:
             self.setValue(init_set_value)
 
+    @classmethod
+    def placeholder_dummy(cls, parent: QWidget, placeholder_text: str) -> _PidgetDoubleSpinBox:
+        """
+        Create a spinbox that only displays a placeholder text
+        """
+        spin_box = _PidgetDoubleSpinBox(parent)
+        spin_box.setSpecialValueText(placeholder_text)
+        spin_box.setRange(0, 1)
+        spin_box.setValue(0)
+        spin_box.setReadOnly(True)
+        return spin_box
+
     def wheelEvent(self, event: QtGui.QWheelEvent) -> None:
         if self.hasFocus():
             super().wheelEvent(event)
         else:
             event.ignore()
```

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/range_help_view.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/range_help_view.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/sensor_config_editor.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/sensor_config_editor.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from acconeer.exptool import a121
 from acconeer.exptool.a121._core import Criticality
 
 from . import pidgets
 from .data_editor import DataEditor
 from .subsweep_config_editor import SubsweepConfigEditor
 from .types import PidgetFactoryMapping
-from .utils import VerticalGroupBox
+from .utils import GroupBox
 
 
 log = logging.getLogger(__name__)
 
 
 class SensorConfigEditor(DataEditor[Optional[a121.SensorConfig]]):
     sig_update = Signal(object)
@@ -53,26 +53,28 @@
             name_label_tooltip=(
                 "The sweep rate for sweeps in a frame (measurement).\n"
                 "If 'Limit' is unchecked, the sweep rate will be as fast as possible."
             ),
             limits=(1, 1e6),
             decimals=0,
             init_set_value=1000.0,
+            placeholder_text="- Hz",
             suffix="Hz",
             checkbox_label_text="Limit",
         ),
         "frame_rate": pidgets.OptionalFloatPidgetFactory(
             name_label_text="Frame rate:",
             name_label_tooltip=(
                 "Frame rate.\nIf 'Limit' is unchecked, the rate is not limited by the sensor "
                 "but by the rate that the server acknowledge and reads out the frame."
             ),
             limits=(0.1, 1e4),
             decimals=1,
             init_set_value=10.0,
+            placeholder_text="- Hz",
             suffix="Hz",
             checkbox_label_text="Limit",
         ),
         "inter_sweep_idle_state": pidgets.EnumPidgetFactory(
             enum_type=a121.IdleState,
             name_label_text="Inter sweep idle state:",
             name_label_tooltip=(
@@ -139,27 +141,27 @@
 
         self._read_only = False
         self._supports_multiple_subsweeps = supports_multiple_subsweeps
 
         self.setLayout(QVBoxLayout(self))
         self.layout().setContentsMargins(0, 0, 0, 0)
 
-        self.sensor_group_box = VerticalGroupBox("Sensor parameters", parent=self)
+        self.sensor_group_box = GroupBox.vertical("Sensor parameters", parent=self)
         self.sensor_group_box.layout().setSpacing(self.SPACING)
         self.layout().addWidget(self.sensor_group_box)
 
         for aspect, factory in self.SENSOR_CONFIG_FACTORIES.items():
             pidget = factory.create(self.sensor_group_box)
             self.sensor_group_box.layout().addWidget(pidget)
 
             pidget.sig_update.connect(partial(self._update_sensor_config_aspect, aspect))
 
             self._sensor_config_pidgets[aspect] = pidget
 
-        self.subsweep_group_box = VerticalGroupBox("Subsweep parameters", parent=self)
+        self.subsweep_group_box = GroupBox.vertical("Subsweep parameters", parent=self)
         self.subsweep_group_box.layout().setSpacing(self.SPACING)
         self.layout().addWidget(self.subsweep_group_box)
 
         self._tab_widget = QTabWidget(self)
         self._tab_widget.setStyleSheet("QTabWidget::pane { padding: 5px;}")
         self.subsweep_group_box.layout().addWidget(self._tab_widget)
```

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/session_config_editor.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/session_config_editor.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,16 +11,17 @@
 from PySide6.QtWidgets import QVBoxLayout, QWidget
 
 from acconeer.exptool import a121
 from acconeer.exptool.a121._core import Criticality
 
 from . import pidgets
 from .data_editor import DataEditor
+from .json_save_load_buttons import JsonSaveLoadButtons
 from .sensor_config_editor import SensorConfigEditor
-from .utils import VerticalGroupBox
+from .utils import GroupBox
 
 
 log = logging.getLogger(__name__)
 
 
 class SessionConfigEditor(DataEditor[Optional[a121.SessionConfig]]):
     _session_config: Optional[a121.SessionConfig]
@@ -42,15 +43,19 @@
 
         self._session_config = None
         self._update_rate_erroneous = False
 
         self.setLayout(QVBoxLayout(self))
         self.layout().setContentsMargins(0, 0, 0, 0)
 
-        self.session_group_box = VerticalGroupBox("Session parameters", parent=self)
+        self.session_group_box = GroupBox.vertical(
+            "Session parameters",
+            JsonSaveLoadButtons.from_editor_and_config_type(self, a121.SessionConfig),
+            parent=self,
+        )
         self.session_group_box.layout().setSpacing(self.SPACING)
         self.layout().addWidget(self.session_group_box)
 
         self._sensor_id_pidget = pidgets.SensorIdPidgetFactory(items=[]).create(self)
         self._sensor_id_pidget.sig_update.connect(self._update_sole_sensor_id)
         self.session_group_box.layout().addWidget(self._sensor_id_pidget)
 
@@ -59,14 +64,15 @@
             name_label_tooltip=(
                 "Set an update rate limit on the server.\n"
                 "If 'Limit' is unchecked, the server will run as fast as possible."
             ),
             limits=(0.1, 1e4),
             decimals=1,
             init_set_value=10.0,
+            placeholder_text="- Hz",
             suffix="Hz",
             checkbox_label_text="Limit",
         ).create(self)
         self._update_rate_pidget.sig_update.connect(self._update_update_rate)
         self.session_group_box.layout().addWidget(self._update_rate_pidget)
 
         self._sensor_config_editor = SensorConfigEditor(supports_multiple_subsweeps, self)
```

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/subsweep_config_editor.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/subsweep_config_editor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/two_sensor_ids_editor.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/plugin_components/two_sensor_ids_editor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/status_bar.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/status_bar.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/stream_tab/connection_widget.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/stream_tab/connection_widget.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/stream_tab/hints.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/stream_tab/hints.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/stream_tab/plugin_widget.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/stream_tab/plugin_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,19 +25,19 @@
     QVBoxLayout,
     QWidget,
 )
 
 import pyqtgraph as pg
 
 from acconeer.exptool.app import resources  # type: ignore[attr-defined]
-from acconeer.exptool.app.new._enums import PluginFamily
+from acconeer.exptool.app.new._enums import PluginFamily, PluginState
 from acconeer.exptool.app.new.app_model import AppModel, PluginPresetSpec, PluginSpec
 from acconeer.exptool.app.new.pluginbase import PlotPluginBase, PluginSpecBase
 from acconeer.exptool.app.new.ui.icons import ARROW_LEFT_BOLD
-from acconeer.exptool.app.new.ui.plugin_components.utils import VerticalGroupBox
+from acconeer.exptool.app.new.ui.plugin_components.utils import GroupBox
 from acconeer.exptool.app.new.ui.utils import (
     HorizontalSeparator,
     ScrollAreaDecorator,
     TopAlignDecorator,
 )
 
 
@@ -77,34 +77,37 @@
         assert all(isinstance(e, PluginSelectionButton) for e in buttons)
         return buttons
 
 
 class PluginPresetButton(QPushButton):
     def __init__(self, plugin_preset: PluginPresetSpec, default: bool, parent: QWidget) -> None:
         super().__init__(parent)
+
         if default:
             self.setText(f"{plugin_preset.name} (default)")
         else:
             self.setText(plugin_preset.name)
         if plugin_preset.description is not None:
             self.setToolTip(plugin_preset.description)
         self.setStyleSheet("text-align: left; font-weight: bold;")
 
 
 class PluginPresetPlaceholder(QWidget):
     def __init__(self, app_model: AppModel, parent: Optional[QWidget] = None) -> None:
         super().__init__(parent)
 
-        app_model.sig_load_plugin.connect(self._on_load_plugin)
+        self.app_model = app_model
+        self.app_model.sig_load_plugin.connect(self._on_load_plugin)
+        self.app_model.sig_notify.connect(self._on_app_model_update)
 
         self.app_model = app_model
         self.setLayout(QVBoxLayout(self))
         self.layout().setContentsMargins(0, 0, 0, 0)
         self.layout().setSpacing(11)
-        self.group_box = VerticalGroupBox("Preset Configurations", self)
+        self.group_box = GroupBox.vertical("Preset Configurations", parent=self)
         self.layout().addWidget(self.group_box)
         self.preset_buttons_widget: Optional[QWidget] = None
 
     def _clear(self) -> None:
         if self.preset_buttons_widget is not None:
             self.preset_buttons_widget.deleteLater()
             self.preset_buttons_widget = None
@@ -126,14 +129,17 @@
                     and preset.preset_id == plugin_spec.default_preset_id
                     and preset.name.lower() != "default"
                 )
                 button = PluginPresetButton(preset, default_preset, self)
                 self.preset_buttons_widget.layout().addWidget(button)
                 button.clicked.connect(partial(self._on_preset_click, preset.preset_id))
 
+    def _on_app_model_update(self, app_model: AppModel) -> None:
+        self.setEnabled(app_model.plugin_state == PluginState.LOADED_IDLE)
+
 
 class PluginSelection(QWidget):
     def __init__(self, app_model: AppModel, parent: QWidget) -> None:
         super().__init__(parent)
 
         self.app_model = app_model
```

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/stream_tab/recording_widget.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/stream_tab/recording_widget.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/stream_tab/widgets.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/stream_tab/widgets.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/utils.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/new/ui/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/old/app.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/old/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import time
 import traceback
 import warnings
 import webbrowser
 from typing import Any, Optional, Tuple
 
 import numpy as np
+import platformdirs
 from packaging import version
 
 from PySide6 import QtCore, QtWidgets
 from PySide6.QtCore import Signal
 from PySide6.QtGui import QFont, QIcon
 from PySide6.QtWidgets import (
     QApplication,
@@ -39,16 +40,14 @@
 import pyqtgraph as pg
 
 import acconeer.exptool as et
 from acconeer.exptool.a111 import _conf_to_rss_sdk
 from acconeer.exptool.a111.algo import Calibration, ModuleInfo
 from acconeer.exptool.app import resources
 
-import platformdirs
-
 from . import data_processing
 from .elements.helper import (
     CalibrationStatus,
     CalibrationUiState,
     Count,
     ExptoolArgumentParser,
     LoadState,
```

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/old/data_processing.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/old/data_processing.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/old/elements/helper.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/old/elements/helper.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/old/elements/modules.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/old/elements/modules.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/old/elements/qt_subclasses.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/old/elements/qt_subclasses.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/resources/a111_gui.png` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/resources/a111_gui.png`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/resources/a121_gui.png` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/resources/a121_gui.png`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/resources/icon-black.svg` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/resources/icon-black.svg`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/resources/icon.png` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/resources/icon.png`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/app/resources/loader.gif` & `acconeer-exptool-7.1.0/src/acconeer/exptool/app/resources/loader.gif`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/data/libft4222/LICENSE.txt` & `acconeer-exptool-7.1.0/src/acconeer/exptool/data/libft4222/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/data/libft4222/aarch64/libft4222.so.1.4.4.44` & `acconeer-exptool-7.1.0/src/acconeer/exptool/data/libft4222/aarch64/libft4222.so.1.4.4.44`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/data/libft4222/amd64/LibFT4222.dll` & `acconeer-exptool-7.1.0/src/acconeer/exptool/data/libft4222/amd64/LibFT4222.dll`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/data/libft4222/amd64/ftd2xx.dll` & `acconeer-exptool-7.1.0/src/acconeer/exptool/data/libft4222/amd64/ftd2xx.dll`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/data/libft4222/armv6/libft4222.so.1.4.4.44` & `acconeer-exptool-7.1.0/src/acconeer/exptool/data/libft4222/armv6/libft4222.so.1.4.4.44`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/data/libft4222/armv7/libft4222.so.1.4.4.44` & `acconeer-exptool-7.1.0/src/acconeer/exptool/data/libft4222/armv7/libft4222.so.1.4.4.44`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/data/libft4222/i386/LibFT4222.dll` & `acconeer-exptool-7.1.0/src/acconeer/exptool/data/libft4222/i386/LibFT4222.dll`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/data/libft4222/i386/ftd2xx.dll` & `acconeer-exptool-7.1.0/src/acconeer/exptool/data/libft4222/i386/ftd2xx.dll`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/data/libft4222/x86_64/libft4222.so.1.4.4.44` & `acconeer-exptool-7.1.0/src/acconeer/exptool/data/libft4222/x86_64/libft4222.so.1.4.4.44`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/flash/_bin_fetcher.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/flash/_bin_fetcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,17 +9,16 @@
 import pickle
 import shutil
 import tempfile
 import zipfile
 from pathlib import Path
 from typing import Optional, Tuple
 
-import requests
-
 import platformdirs
+import requests
 from bs4 import BeautifulSoup
 
 
 ET_DIR = Path(platformdirs.user_data_dir(appname="acconeer_exptool", appauthor="Acconeer AB"))
 CODENAME = "plugoneer"
 COOKIE_DIR = ET_DIR / CODENAME / "cookies"
 COOKIE_FILEPATH = COOKIE_DIR / "developer_page.pickle"
```

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/flash/_dev_license.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/flash/_dev_license.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-# Copyright (c) Acconeer AB, 2022
+# Copyright (c) Acconeer AB, 2022-2023
 # All rights reserved
 
 from __future__ import annotations
 
 import logging
 from typing import List
 
 import requests
-
 from bs4 import BeautifulSoup
 
 
 DEV_LICENSE_URL = "https://developer.acconeer.com/software-license-agreement/"
 
 DEV_LICENSE_DEFAULT_HEADER = "SOFTWARE LICENSE AGREEMENT"
 DEV_LICENSE_DEFAULT_SUBHEADER = "LIMITED LICENSE AGREEMENT FOR Acconeer MATERIALS"
```

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/flash/_dev_license_tui.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/flash/_dev_license_tui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/flash/_flasher.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/flash/_flasher.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/flash/_products.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/flash/_products.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/flash/_stm32uart/_stm32flasher.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/flash/_stm32uart/_stm32flasher.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/flash/_xc120/_bootloader_comm.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/flash/_xc120/_bootloader_comm.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/flash/_xc120/_bootloader_tool.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/flash/_xc120/_bootloader_tool.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/libft4222.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/libft4222.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/mpl_process.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/mpl_process.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/pg_process.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/pg_process.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/setup/__main__.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/setup/__main__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/setup/base/platform_install.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/setup/base/platform_install.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/setup/base/prompts.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/setup/base/prompts.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/setup/base/setup_group.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/setup/base/setup_group.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/setup/base/setup_step.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/setup/base/setup_step.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/setup/base/utils.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/setup/base/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/setup/cli/argument_parser.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/setup/cli/argument_parser.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/setup/platforms/linux.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/setup/platforms/linux.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/setup/platforms/ubuntu_20_04.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/setup/platforms/ubuntu_20_04.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer/exptool/utils.py` & `acconeer-exptool-7.1.0/src/acconeer/exptool/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/src/acconeer_exptool.egg-info/PKG-INFO` & `acconeer-exptool-7.1.0/src/acconeer_exptool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acconeer-exptool
-Version: 7.0.2
+Version: 7.1.0
 Summary: Acconeer Exploration Tool
 Home-page: https://github.com/acconeer/acconeer-python-exploration
 Author: Acconeer AB
 Author-email: tools@acconeer.com
 License: BSD 3-Clause Clear License
 Project-URL: Tracker, https://github.com/acconeer/acconeer-python-exploration/issues
 Project-URL: Documentation, https://acconeer-python-exploration.readthedocs.io
```

### Comparing `acconeer-exptool-7.0.2/src/acconeer_exptool.egg-info/SOURCES.txt` & `acconeer-exptool-7.1.0/src/acconeer_exptool.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 examples/a121/load_record.py
 examples/a121/load_record_h5.m
 examples/a121/plot.py
 examples/a121/reuse_calibration.py
 examples/a121/stress.py
 examples/a121/subsweeps.py
 examples/a121/bilateration/bilaterator.py
-examples/a121/breathing/breathing.py
 examples/a121/distance/detector.py
 examples/a121/distance/processor.py
 examples/a121/phase_tracking/phase_tracking.py
 examples/a121/presence/detector.py
 examples/a121/presence/processor.py
 examples/a121/record_data/barebones.py
 examples/a121/record_data/with_cli.py
@@ -293,17 +292,19 @@
 src/acconeer/exptool/a121/algo/_plugins/processor/plugin.py
 src/acconeer/exptool/a121/algo/_plugins/processor/view_plugin.py
 src/acconeer/exptool/a121/algo/bilateration/__init__.py
 src/acconeer/exptool/a121/algo/bilateration/_configs.py
 src/acconeer/exptool/a121/algo/bilateration/_plugin.py
 src/acconeer/exptool/a121/algo/bilateration/_processor.py
 src/acconeer/exptool/a121/algo/breathing/__init__.py
-src/acconeer/exptool/a121/algo/breathing/__main__.py
-src/acconeer/exptool/a121/algo/breathing/_plugin.py
+src/acconeer/exptool/a121/algo/breathing/_configs.py
 src/acconeer/exptool/a121/algo/breathing/_processor.py
+src/acconeer/exptool/a121/algo/breathing/_ref_app.py
+src/acconeer/exptool/a121/algo/breathing/_ref_app_plugin.py
+src/acconeer/exptool/a121/algo/breathing/_serializer.py
 src/acconeer/exptool/a121/algo/distance/__init__.py
 src/acconeer/exptool/a121/algo/distance/__main__.py
 src/acconeer/exptool/a121/algo/distance/_aggregator.py
 src/acconeer/exptool/a121/algo/distance/_configs.py
 src/acconeer/exptool/a121/algo/distance/_detector.py
 src/acconeer/exptool/a121/algo/distance/_detector_plugin.py
 src/acconeer/exptool/a121/algo/distance/_processors.py
@@ -325,14 +326,19 @@
 src/acconeer/exptool/a121/algo/smart_presence/_ref_app_plugin.py
 src/acconeer/exptool/a121/algo/smart_presence/_serializer.py
 src/acconeer/exptool/a121/algo/sparse_iq/__init__.py
 src/acconeer/exptool/a121/algo/sparse_iq/__main__.py
 src/acconeer/exptool/a121/algo/sparse_iq/_plugin.py
 src/acconeer/exptool/a121/algo/sparse_iq/_processor.py
 src/acconeer/exptool/a121/algo/sparse_iq/_serializers.py
+src/acconeer/exptool/a121/algo/speed/__init__.py
+src/acconeer/exptool/a121/algo/speed/_configs.py
+src/acconeer/exptool/a121/algo/speed/_detector.py
+src/acconeer/exptool/a121/algo/speed/_detector_plugin.py
+src/acconeer/exptool/a121/algo/speed/_processors.py
 src/acconeer/exptool/a121/algo/surface_velocity/__init__.py
 src/acconeer/exptool/a121/algo/surface_velocity/_example_app.py
 src/acconeer/exptool/a121/algo/surface_velocity/_example_app_plugin.py
 src/acconeer/exptool/a121/algo/surface_velocity/_processor.py
 src/acconeer/exptool/a121/algo/tank_level/__init__.py
 src/acconeer/exptool/a121/algo/tank_level/_configs.py
 src/acconeer/exptool/a121/algo/tank_level/_plugin.py
@@ -397,14 +403,15 @@
 src/acconeer/exptool/app/new/ui/flash_tab/dialogs.py
 src/acconeer/exptool/app/new/ui/flash_tab/threads.py
 src/acconeer/exptool/app/new/ui/flash_tab/widgets.py
 src/acconeer/exptool/app/new/ui/plugin_components/__init__.py
 src/acconeer/exptool/app/new/ui/plugin_components/attrs_config_editor.py
 src/acconeer/exptool/app/new/ui/plugin_components/collapsible_widget.py
 src/acconeer/exptool/app/new/ui/plugin_components/data_editor.py
+src/acconeer/exptool/app/new/ui/plugin_components/json_save_load_buttons.py
 src/acconeer/exptool/app/new/ui/plugin_components/metadata_view.py
 src/acconeer/exptool/app/new/ui/plugin_components/misc_error_view.py
 src/acconeer/exptool/app/new/ui/plugin_components/perf_calc_view.py
 src/acconeer/exptool/app/new/ui/plugin_components/range_help_view.py
 src/acconeer/exptool/app/new/ui/plugin_components/sensor_config_editor.py
 src/acconeer/exptool/app/new/ui/plugin_components/session_config_editor.py
 src/acconeer/exptool/app/new/ui/plugin_components/subsweep_config_editor.py
@@ -412,14 +419,18 @@
 src/acconeer/exptool/app/new/ui/plugin_components/types.py
 src/acconeer/exptool/app/new/ui/plugin_components/utils.py
 src/acconeer/exptool/app/new/ui/plugin_components/pidgets/__init__.py
 src/acconeer/exptool/app/new/ui/plugin_components/pidgets/common.py
 src/acconeer/exptool/app/new/ui/plugin_components/pidgets/hooks.py
 src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidget_groups.py
 src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidgets.py
+src/acconeer/exptool/app/new/ui/plugin_components/save_dialog/__init__.py
+src/acconeer/exptool/app/new/ui/plugin_components/save_dialog/dialog.py
+src/acconeer/exptool/app/new/ui/plugin_components/save_dialog/preview.py
+src/acconeer/exptool/app/new/ui/plugin_components/save_dialog/set_config_presenter.py
 src/acconeer/exptool/app/new/ui/stream_tab/__init__.py
 src/acconeer/exptool/app/new/ui/stream_tab/connection_widget.py
 src/acconeer/exptool/app/new/ui/stream_tab/hints.py
 src/acconeer/exptool/app/new/ui/stream_tab/plugin_widget.py
 src/acconeer/exptool/app/new/ui/stream_tab/recording_widget.py
 src/acconeer/exptool/app/new/ui/stream_tab/widgets.py
 src/acconeer/exptool/app/old/__init__.py
```

### Comparing `acconeer-exptool-7.0.2/tools/check_changelog.py` & `acconeer-exptool-7.1.0/tools/check_changelog.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,26 @@
 from pathlib import Path
 from typing import Optional
 
 from packaging.version import Version
 
 
 VERSION_PATTERN = r"v?\d+\.\d+\.\d+"
+EMPTY_UNRELEASED_CHANGELOG = """# Unreleased Changelog
+
+## Unreleased
+
+### Added
+
+### Changed
+
+### Fixed
+
+### Removed
+"""
 
 
 def utf8_subprocess_output(*args: str) -> str:
     return subprocess.check_output(args, encoding="utf-8").strip()
 
 
 def get_commit_sha_of_git_tag(git_tag: str) -> str:
@@ -110,19 +122,15 @@
 
     if first_match == version_tag:
         print(f"Which matches {version_tag} exactly.")
     else:
         print(f'Which does not match "{version_tag}".')
         status = False
 
-    empty_unreleased_changelog = (
-        "# Unreleased Changelog\n\n## Unreleased\n\n### Added\n\n### Changed\n\n### Fixed\n"
-    )
-
-    if unreleased_changelog.read_text() != empty_unreleased_changelog:
+    if unreleased_changelog.read_text() != EMPTY_UNRELEASED_CHANGELOG:
         print("Unreleased changelog is not cleared")
         status = False
 
     exit(0 if status else 1)
 
 
 if __name__ == "__main__":
```

### Comparing `acconeer-exptool-7.0.2/tools/check_copyright.py` & `acconeer-exptool-7.1.0/tools/check_copyright.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/tools/check_line_length.py` & `acconeer-exptool-7.1.0/tools/check_line_length.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/tools/check_permissions.py` & `acconeer-exptool-7.1.0/tools/check_permissions.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/tools/check_sdk_mentions.py` & `acconeer-exptool-7.1.0/tools/check_sdk_mentions.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/tools/check_whitespace.py` & `acconeer-exptool-7.1.0/tools/check_whitespace.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/tools/update_regmap.py` & `acconeer-exptool-7.1.0/tools/update_regmap.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.2/utils/convert_to_csv.py` & `acconeer-exptool-7.1.0/utils/convert_to_csv.py`

 * *Files identical despite different names*

