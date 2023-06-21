# Comparing `tmp/qudi-core-1.3.0.tar.gz` & `tmp/qudi-core-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qudi-core-1.3.0.tar", last modified: Tue Dec 20 15:28:10 2022, max compression
+gzip compressed data, was "qudi-core-1.4.0.tar", last modified: Wed Jun 21 08:59:58 2023, max compression
```

## Comparing `qudi-core-1.3.0.tar` & `qudi-core-1.4.0.tar`

### file list

```diff
@@ -1,259 +1,260 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:28:10.689189 qudi-core-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3649 2022-12-20 15:28:01.000000 qudi-core-1.3.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2022-12-20 15:28:01.000000 qudi-core-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2022-12-20 15:28:01.000000 qudi-core-1.3.0/LICENSE.LESSER
--rw-r--r--   0 runner    (1001) docker     (123)     5952 2022-12-20 15:28:10.689189 qudi-core-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2022-12-20 15:28:01.000000 qudi-core-1.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2022-12-20 15:28:01.000000 qudi-core-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-20 15:28:10.689189 qudi-core-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4151 2022-12-20 15:28:01.000000 qudi-core-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:28:10.657189 qudi-core-1.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:28:10.657189 qudi-core-1.3.0/src/qudi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:28:10.653189 qudi-core-1.3.0/src/qudi/artwork/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:28:10.669189 qudi-core-1.3.0/src/qudi/artwork/icons/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:28:10.669189 qudi-core-1.3.0/src/qudi/artwork/icons/LICENSE/
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/LICENSE/Oxygen.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/LICENSE/qudi.txt
--rw-r--r--   0 runner    (1001) docker     (123)    78804 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/accessories-calculator.svg
--rw-r--r--   0 runner    (1001) docker     (123)    36694 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/application-exit.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/auto_pois.svg
--rw-r--r--   0 runner    (1001) docker     (123)    69533 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/camera-photo.svg
--rw-r--r--   0 runner    (1001) docker     (123)   175679 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/configure.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6085 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/correct-tilt.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/dialog-warning.svgz
--rw-r--r--   0 runner    (1001) docker     (123)    18333 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/document-new.svg
--rw-r--r--   0 runner    (1001) docker     (123)    92192 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/document-open.svgz
--rw-r--r--   0 runner    (1001) docker     (123)  1116723 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/document-save.svg
--rw-r--r--   0 runner    (1001) docker     (123)    36808 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/edit-clear.svgz
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/edit-copy.svgz
--rw-r--r--   0 runner    (1001) docker     (123)     8439 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/edit-cut.svgz
--rw-r--r--   0 runner    (1001) docker     (123)    42294 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/edit-delete-shred.svgz
--rw-r--r--   0 runner    (1001) docker     (123)    21905 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/edit-delete.svgz
--rw-r--r--   0 runner    (1001) docker     (123)    35135 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/go-home.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6149 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/go-next.svgz
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/go-previous.svgz
--rw-r--r--   0 runner    (1001) docker     (123)     6759 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/goto-poi.svgz
--rw-r--r--   0 runner    (1001) docker     (123)    21650 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/list-add.svg
--rw-r--r--   0 runner    (1001) docker     (123)    14594 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/list-remove.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/media-playback-pause.svgz
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/media-playback-start.svgz
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/media-playback-stop.svgz
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/media-record.svgz
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/mouse_pointer.svg
--rw-r--r--   0 runner    (1001) docker     (123)    62089 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/network-connect.svg
--rw-r--r--   0 runner    (1001) docker     (123)    44593 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/network-disconnect.svg
--rw-r--r--   0 runner    (1001) docker     (123)  1308331 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/new_poi_crosshair.svg
--rw-r--r--   0 runner    (1001) docker     (123)  1304944 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/new_poi_mouse.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/object-rotate-left.svgz
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/object-rotate-right.svgz
--rw-r--r--   0 runner    (1001) docker     (123)     4116 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/optimize-position-poi.svgz
--rw-r--r--   0 runner    (1001) docker     (123)    13543 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/optimize-position.svg
--rw-r--r--   0 runner    (1001) docker     (123)    24755 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/periodic-refind-poi.svgz
--rw-r--r--   0 runner    (1001) docker     (123)  1308267 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/poi-new.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/record-counter.svgz
--rw-r--r--   0 runner    (1001) docker     (123)    24473 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/restart-counter.svg
--rw-r--r--   0 runner    (1001) docker     (123)    19409 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/scan-depth-loop.svg
--rw-r--r--   0 runner    (1001) docker     (123)    24941 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/scan-depth-restart.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15203 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/scan-depth-start.svg
--rw-r--r--   0 runner    (1001) docker     (123)    33779 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/scan-stop.svg
--rw-r--r--   0 runner    (1001) docker     (123)    19411 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/scan-xy-loop.svg
--rw-r--r--   0 runner    (1001) docker     (123)    24941 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/scan-xy-restart.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15203 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/scan-xy-start.svg
--rw-r--r--   0 runner    (1001) docker     (123)    14736 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/start-counter.svg
--rw-r--r--   0 runner    (1001) docker     (123)    33505 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/stop-counter.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8434 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/utilities-terminal.svgz
--rw-r--r--   0 runner    (1001) docker     (123)    29805 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/view-filter.svg
--rw-r--r--   0 runner    (1001) docker     (123)    58775 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/view-refresh.svg
--rw-r--r--   0 runner    (1001) docker     (123)    41078 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/zoom-fit-best.svg
--rw-r--r--   0 runner    (1001) docker     (123)    31740 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/icons/zoom-select.svgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:28:10.669189 qudi-core-1.3.0/src/qudi/artwork/logo/
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/logo/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10735 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/logo/logo-qudi.svg
--rw-r--r--   0 runner    (1001) docker     (123)   324299 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/logo/logo_qudi.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:28:10.669189 qudi-core-1.3.0/src/qudi/artwork/styles/
--rw-r--r--   0 runner    (1001) docker     (123)    17494 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/dracula.qss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:28:10.673189 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/Hmovetoolbar.png
--rw-r--r--   0 runner    (1001) docker     (123)      172 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/Hsepartoolbar.png
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      228 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/Vmovetoolbar.png
--rw-r--r--   0 runner    (1001) docker     (123)      187 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/Vsepartoolbar.png
--rw-r--r--   0 runner    (1001) docker     (123)      147 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/branch_closed-on.png
--rw-r--r--   0 runner    (1001) docker     (123)      160 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/branch_closed.png
--rw-r--r--   0 runner    (1001) docker     (123)      150 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/branch_open-on.png
--rw-r--r--   0 runner    (1001) docker     (123)      166 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/branch_open.png
--rw-r--r--   0 runner    (1001) docker     (123)      492 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/checkbox_checked.png
--rw-r--r--   0 runner    (1001) docker     (123)      491 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/checkbox_checked_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)      512 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/checkbox_checked_focus.png
--rw-r--r--   0 runner    (1001) docker     (123)      493 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/checkbox_indeterminate.png
--rw-r--r--   0 runner    (1001) docker     (123)      492 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/checkbox_indeterminate_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)      514 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/checkbox_indeterminate_focus.png
--rw-r--r--   0 runner    (1001) docker     (123)      464 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/checkbox_unchecked.png
--rw-r--r--   0 runner    (1001) docker     (123)      464 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/checkbox_unchecked_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)      483 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/checkbox_unchecked_focus.png
--rw-r--r--   0 runner    (1001) docker     (123)      598 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/close-hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      598 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/close-pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)      586 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/close.png
--rw-r--r--   0 runner    (1001) docker     (123)      165 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/down_arrow.png
--rw-r--r--   0 runner    (1001) docker     (123)      166 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/down_arrow_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)      166 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/left_arrow.png
--rw-r--r--   0 runner    (1001) docker     (123)      166 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/left_arrow_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)      940 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/radio_checked.png
--rw-r--r--   0 runner    (1001) docker     (123)      972 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/radio_checked_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)      933 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/radio_checked_focus.png
--rw-r--r--   0 runner    (1001) docker     (123)      728 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/radio_unchecked.png
--rw-r--r--   0 runner    (1001) docker     (123)      760 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/radio_unchecked_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)      724 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/radio_unchecked_focus.png
--rw-r--r--   0 runner    (1001) docker     (123)      160 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/right_arrow.png
--rw-r--r--   0 runner    (1001) docker     (123)      160 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/right_arrow_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)      129 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/sizegrip.png
--rw-r--r--   0 runner    (1001) docker     (123)      224 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/stylesheet-branch-end.png
--rw-r--r--   0 runner    (1001) docker     (123)      182 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/stylesheet-branch-more.png
--rw-r--r--   0 runner    (1001) docker     (123)      239 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/stylesheet-vline.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:28:10.677189 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/svg/
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/svg/checkbox_checked.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/svg/checkbox_checked_disabled.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/svg/checkbox_checked_focus.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2898 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/svg/checkbox_indeterminate.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/svg/checkbox_indeterminate_disabled.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/svg/checkbox_indeterminate_focus.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/svg/checkbox_unchecked.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/svg/checkbox_unchecked_disabled.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/svg/checkbox_unchecked_focus.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/svg/radio_checked.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/svg/radio_checked_disabled.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/svg/radio_checked_focus.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/svg/radio_unchecked.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/svg/radio_unchecked_disabled.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/svg/radio_unchecked_focus.svg
--rw-r--r--   0 runner    (1001) docker     (123)      195 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/transparent.png
--rw-r--r--   0 runner    (1001) docker     (123)      578 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/undock.png
--rw-r--r--   0 runner    (1001) docker     (123)      158 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/up_arrow.png
--rw-r--r--   0 runner    (1001) docker     (123)      159 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark/up_arrow_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)    24763 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qdark.qss
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/artwork/styles/qtdark.qss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:28:10.677189 qudi-core-1.3.0/src/qudi/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/core/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18352 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/core/application.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:28:10.681189 qudi-core-1.3.0/src/qudi/core/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/core/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14026 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/core/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5949 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/core/config/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7566 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/core/config/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3828 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/core/config/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5006 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/core/configoption.py
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/core/connector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:28:10.681189 qudi-core-1.3.0/src/qudi/core/gui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/core/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15742 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/core/gui/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:28:10.681189 qudi-core-1.3.0/src/qudi/core/gui/main_gui/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/core/gui/main_gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11242 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/core/gui/main_gui/aboutqudidialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/core/gui/main_gui/configwidget.py
--rw-r--r--   0 runner    (1001) docker     (123)     7670 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/core/gui/main_gui/errordialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     9839 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/core/gui/main_gui/logwidget.py
--rw-r--r--   0 runner    (1001) docker     (123)    18527 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/core/gui/main_gui/main_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)    11719 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/core/gui/main_gui/mainwindow.py
--rw-r--r--   0 runner    (1001) docker     (123)    13920 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/core/gui/main_gui/modulewidget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/core/gui/main_gui/remotewidget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/core/gui/main_gui/settingsdialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/core/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:28:10.681189 qudi-core-1.3.0/src/qudi/core/logger/
--rw-r--r--   0 runner    (1001) docker     (123)     7194 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/core/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/core/logger/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6413 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/core/logger/records_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/core/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    18830 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/core/module.py
--rw-r--r--   0 runner    (1001) docker     (123)    29893 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/core/modulemanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5199 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/core/parentpoller.py
--rw-r--r--   0 runner    (1001) docker     (123)     7251 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/core/qudikernel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:28:10.681189 qudi-core-1.3.0/src/qudi/core/scripting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/core/scripting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10363 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/core/scripting/modulescript.py
--rw-r--r--   0 runner    (1001) docker     (123)     8609 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/core/scripting/moduletask.py
--rw-r--r--   0 runner    (1001) docker     (123)    10711 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/core/servers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12452 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/core/services.py
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/core/statusvariable.py
--rw-r--r--   0 runner    (1001) docker     (123)     8438 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/core/threadmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/core/watchdog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:28:10.657189 qudi-core-1.3.0/src/qudi/gui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:28:10.681189 qudi-core-1.3.0/src/qudi/gui/taskrunner/
--rw-r--r--   0 runner    (1001) docker     (123)     5307 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/gui/taskrunner/main_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/gui/taskrunner/task_runner_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     9154 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/gui/taskrunner/taskwidget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:28:10.681189 qudi-core-1.3.0/src/qudi/logic/
--rw-r--r--   0 runner    (1001) docker     (123)     8642 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/logic/taskrunner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/runnable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:28:10.681189 qudi-core-1.3.0/src/qudi/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/tasks/test_tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:28:10.657189 qudi-core-1.3.0/src/qudi/tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:28:10.685189 qudi-core-1.3.0/src/qudi/tools/config_editor/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/tools/config_editor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/tools/config_editor/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15413 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/tools/config_editor/config_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8464 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/tools/config_editor/custom_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/tools/config_editor/global_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    15978 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/tools/config_editor/global_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5984 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/tools/config_editor/module_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4467 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/tools/config_editor/module_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6161 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/tools/config_editor/module_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)    21476 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/tools/config_editor/module_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     8965 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/tools/config_editor/tree_widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:28:10.685189 qudi-core-1.3.0/src/qudi/util/
--rw-r--r--   0 runner    (1001) docker     (123)    52734 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/util/colordefs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5318 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/util/constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)    13319 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/util/datafitting.py
--rw-r--r--   0 runner    (1001) docker     (123)    34037 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/util/datastorage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/util/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:28:10.685189 qudi-core-1.3.0/src/qudi/util/fit_models/
--rw-r--r--   0 runner    (1001) docker     (123)     6657 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/util/fit_models/exp_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)    18864 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/util/fit_models/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     9529 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/util/fit_models/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/util/fit_models/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)    17273 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/util/fit_models/lorentzian.py
--rw-r--r--   0 runner    (1001) docker     (123)     6009 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/util/fit_models/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6737 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/util/fit_models/poissonian.py
--rw-r--r--   0 runner    (1001) docker     (123)    18926 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/util/fit_models/sine.py
--rw-r--r--   0 runner    (1001) docker     (123)     7962 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/util/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18996 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/util/mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7277 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/util/math.py
--rw-r--r--   0 runner    (1001) docker     (123)    11382 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/util/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/util/mutex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/util/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     8192 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/util/overload.py
--rw-r--r--   0 runner    (1001) docker     (123)     7299 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/util/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6085 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/util/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     5617 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/util/uic.py
--rw-r--r--   0 runner    (1001) docker     (123)    13072 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/util/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:28:10.689189 qudi-core-1.3.0/src/qudi/util/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/util/widgets/advanced_dockwidget.py
--rw-r--r--   0 runner    (1001) docker     (123)     5388 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/util/widgets/collapsible.py
--rw-r--r--   0 runner    (1001) docker     (123)    17380 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/util/widgets/fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     9851 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/util/widgets/literal_lineedit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5303 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/util/widgets/loading_indicator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/util/widgets/parameter_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4836 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/util/widgets/path_line_edit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:28:10.689189 qudi-core-1.3.0/src/qudi/util/widgets/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/util/widgets/plotting/axis.py
--rw-r--r--   0 runner    (1001) docker     (123)    11664 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/util/widgets/plotting/colorbar.py
--rw-r--r--   0 runner    (1001) docker     (123)    10292 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/util/widgets/plotting/image_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    30567 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/util/widgets/plotting/interactive_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)    34463 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/util/widgets/plotting/marker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5035 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/util/widgets/plotting/plot_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    10206 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/util/widgets/plotting/plot_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     8942 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/util/widgets/plotting/roi.py
--rw-r--r--   0 runner    (1001) docker     (123)    25078 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/util/widgets/plotting/view_box.py
--rw-r--r--   0 runner    (1001) docker     (123)    61278 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/util/widgets/scientific_spinbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/util/widgets/separator_lines.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/util/widgets/slider.py
--rw-r--r--   0 runner    (1001) docker     (123)    11177 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/util/widgets/toggle_switch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11313 2022-12-20 15:28:01.000000 qudi-core-1.3.0/src/qudi/util/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:28:10.689189 qudi-core-1.3.0/src/qudi_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5952 2022-12-20 15:28:10.000000 qudi-core-1.3.0/src/qudi_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9359 2022-12-20 15:28:10.000000 qudi-core-1.3.0/src/qudi_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-20 15:28:10.000000 qudi-core-1.3.0/src/qudi_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      229 2022-12-20 15:28:10.000000 qudi-core-1.3.0/src/qudi_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-20 15:28:10.000000 qudi-core-1.3.0/src/qudi_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      186 2022-12-20 15:28:10.000000 qudi-core-1.3.0/src/qudi_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2022-12-20 15:28:10.000000 qudi-core-1.3.0/src/qudi_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:59:58.601395 qudi-core-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-06-21 08:59:43.000000 qudi-core-1.4.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-21 08:59:43.000000 qudi-core-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-21 08:59:43.000000 qudi-core-1.4.0/LICENSE.LESSER
+-rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-06-21 08:59:58.601395 qudi-core-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-06-21 08:59:43.000000 qudi-core-1.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-21 08:59:43.000000 qudi-core-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 08:59:58.601395 qudi-core-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-06-21 08:59:43.000000 qudi-core-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:59:58.533396 qudi-core-1.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:59:58.537396 qudi-core-1.4.0/src/qudi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:59:58.533396 qudi-core-1.4.0/src/qudi/artwork/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:59:58.557396 qudi-core-1.4.0/src/qudi/artwork/icons/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:59:58.557396 qudi-core-1.4.0/src/qudi/artwork/icons/LICENSE/
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/LICENSE/Oxygen.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/LICENSE/qudi.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    78804 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/accessories-calculator.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    36694 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/application-exit.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/auto_pois.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    69533 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/camera-photo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   175679 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/configure.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/correct-tilt.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/dialog-warning.svgz
+-rw-r--r--   0 runner    (1001) docker     (123)    18333 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/document-new.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    92192 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/document-open.svgz
+-rw-r--r--   0 runner    (1001) docker     (123)  1116723 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/document-save.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    36808 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/edit-clear.svgz
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/edit-copy.svgz
+-rw-r--r--   0 runner    (1001) docker     (123)     8439 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/edit-cut.svgz
+-rw-r--r--   0 runner    (1001) docker     (123)    42294 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/edit-delete-shred.svgz
+-rw-r--r--   0 runner    (1001) docker     (123)    21905 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/edit-delete.svgz
+-rw-r--r--   0 runner    (1001) docker     (123)    35135 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/go-home.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/go-next.svgz
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/go-previous.svgz
+-rw-r--r--   0 runner    (1001) docker     (123)     6759 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/goto-poi.svgz
+-rw-r--r--   0 runner    (1001) docker     (123)    21650 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/list-add.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14594 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/list-remove.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/media-playback-pause.svgz
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/media-playback-start.svgz
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/media-playback-stop.svgz
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/media-record.svgz
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/mouse_pointer.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    62089 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/network-connect.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    44593 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/network-disconnect.svg
+-rw-r--r--   0 runner    (1001) docker     (123)  1308331 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/new_poi_crosshair.svg
+-rw-r--r--   0 runner    (1001) docker     (123)  1304944 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/new_poi_mouse.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/object-rotate-left.svgz
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/object-rotate-right.svgz
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/optimize-position-poi.svgz
+-rw-r--r--   0 runner    (1001) docker     (123)    13543 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/optimize-position.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    24755 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/periodic-refind-poi.svgz
+-rw-r--r--   0 runner    (1001) docker     (123)  1308267 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/poi-new.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/record-counter.svgz
+-rw-r--r--   0 runner    (1001) docker     (123)    24473 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/restart-counter.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    19409 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/scan-depth-loop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    24941 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/scan-depth-restart.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15203 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/scan-depth-start.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    33779 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/scan-stop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    19411 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/scan-xy-loop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    24941 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/scan-xy-restart.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15203 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/scan-xy-start.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14736 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/start-counter.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    33505 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/stop-counter.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/utilities-terminal.svgz
+-rw-r--r--   0 runner    (1001) docker     (123)    29805 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/view-filter.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    58775 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/view-refresh.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    41078 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/zoom-fit-best.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    31740 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/icons/zoom-select.svgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:59:58.557396 qudi-core-1.4.0/src/qudi/artwork/logo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/logo/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/logo/logo-qudi.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   324299 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/logo/logo_qudi.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:59:58.557396 qudi-core-1.4.0/src/qudi/artwork/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)    17494 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/dracula.qss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:59:58.569396 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/Hmovetoolbar.png
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/Hsepartoolbar.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/Vmovetoolbar.png
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/Vsepartoolbar.png
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/branch_closed-on.png
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/branch_closed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/branch_open-on.png
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/branch_open.png
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/checkbox_checked.png
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/checkbox_checked_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/checkbox_checked_focus.png
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/checkbox_indeterminate.png
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/checkbox_indeterminate_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/checkbox_indeterminate_focus.png
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/checkbox_unchecked.png
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/checkbox_unchecked_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/checkbox_unchecked_focus.png
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/close-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/close-pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/close.png
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/down_arrow.png
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/down_arrow_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/left_arrow.png
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/left_arrow_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/radio_checked.png
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/radio_checked_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/radio_checked_focus.png
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/radio_unchecked.png
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/radio_unchecked_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/radio_unchecked_focus.png
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/right_arrow.png
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/right_arrow_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/sizegrip.png
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/stylesheet-branch-end.png
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/stylesheet-branch-more.png
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/stylesheet-vline.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:59:58.573396 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/svg/
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/svg/checkbox_checked.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/svg/checkbox_checked_disabled.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/svg/checkbox_checked_focus.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/svg/checkbox_indeterminate.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/svg/checkbox_indeterminate_disabled.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/svg/checkbox_indeterminate_focus.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/svg/checkbox_unchecked.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/svg/checkbox_unchecked_disabled.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/svg/checkbox_unchecked_focus.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/svg/radio_checked.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/svg/radio_checked_disabled.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/svg/radio_checked_focus.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/svg/radio_unchecked.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/svg/radio_unchecked_disabled.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/svg/radio_unchecked_focus.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/transparent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/undock.png
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/up_arrow.png
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark/up_arrow_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24763 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qdark.qss
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/artwork/styles/qtdark.qss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:59:58.577396 qudi-core-1.4.0/src/qudi/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/core/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18352 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/core/application.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:59:58.577396 qudi-core-1.4.0/src/qudi/core/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/core/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14026 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/core/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/core/config/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/core/config/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/core/config/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/core/configoption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/core/connector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:59:58.577396 qudi-core-1.4.0/src/qudi/core/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/core/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15742 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/core/gui/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:59:58.581396 qudi-core-1.4.0/src/qudi/core/gui/main_gui/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/core/gui/main_gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/core/gui/main_gui/aboutqudidialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/core/gui/main_gui/configwidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7670 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/core/gui/main_gui/errordialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9839 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/core/gui/main_gui/logwidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18527 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/core/gui/main_gui/main_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11719 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/core/gui/main_gui/mainwindow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13920 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/core/gui/main_gui/modulewidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/core/gui/main_gui/remotewidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/core/gui/main_gui/settingsdialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/core/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:59:58.581396 qudi-core-1.4.0/src/qudi/core/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/core/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/core/logger/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/core/logger/records_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/core/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18830 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/core/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29893 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/core/modulemanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5199 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/core/parentpoller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/core/qudikernel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:59:58.581396 qudi-core-1.4.0/src/qudi/core/scripting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/core/scripting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10363 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/core/scripting/modulescript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8609 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/core/scripting/moduletask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10711 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/core/servers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12452 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/core/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/core/statusvariable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/core/threadmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/core/watchdog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:59:58.533396 qudi-core-1.4.0/src/qudi/gui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:59:58.581396 qudi-core-1.4.0/src/qudi/gui/taskrunner/
+-rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/gui/taskrunner/main_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/gui/taskrunner/task_runner_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9154 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/gui/taskrunner/taskwidget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:59:58.585396 qudi-core-1.4.0/src/qudi/logic/
+-rw-r--r--   0 runner    (1001) docker     (123)     8642 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/logic/taskrunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/runnable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:59:58.585396 qudi-core-1.4.0/src/qudi/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/tasks/test_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:59:58.533396 qudi-core-1.4.0/src/qudi/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:59:58.585396 qudi-core-1.4.0/src/qudi/tools/config_editor/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/tools/config_editor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/tools/config_editor/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15413 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/tools/config_editor/config_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8464 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/tools/config_editor/custom_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/tools/config_editor/global_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15978 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/tools/config_editor/global_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5984 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/tools/config_editor/module_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/tools/config_editor/module_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6161 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/tools/config_editor/module_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21476 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/tools/config_editor/module_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8965 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/tools/config_editor/tree_widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:59:58.589396 qudi-core-1.4.0/src/qudi/util/
+-rw-r--r--   0 runner    (1001) docker     (123)    52734 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/util/colordefs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/util/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13319 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/util/datafitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34037 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/util/datastorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10951 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/util/descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/util/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:59:58.593396 qudi-core-1.4.0/src/qudi/util/fit_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/util/fit_models/exp_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18864 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/util/fit_models/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9529 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/util/fit_models/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/util/fit_models/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17273 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/util/fit_models/lorentzian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/util/fit_models/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6737 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/util/fit_models/poissonian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18926 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/util/fit_models/sine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7962 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/util/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18996 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/util/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/util/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11382 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/util/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/util/mutex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/util/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/util/overload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/util/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/util/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/util/uic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13072 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/util/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:59:58.597396 qudi-core-1.4.0/src/qudi/util/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/util/widgets/advanced_dockwidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/util/widgets/collapsible.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17380 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/util/widgets/fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9851 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/util/widgets/literal_lineedit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/util/widgets/loading_indicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/util/widgets/parameter_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/util/widgets/path_line_edit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:59:58.597396 qudi-core-1.4.0/src/qudi/util/widgets/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/util/widgets/plotting/axis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11664 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/util/widgets/plotting/colorbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10292 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/util/widgets/plotting/image_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30567 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/util/widgets/plotting/interactive_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34463 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/util/widgets/plotting/marker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/util/widgets/plotting/plot_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10206 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/util/widgets/plotting/plot_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8942 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/util/widgets/plotting/roi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25078 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/util/widgets/plotting/view_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61278 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/util/widgets/scientific_spinbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/util/widgets/separator_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/util/widgets/slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11177 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/util/widgets/toggle_switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11313 2023-06-21 08:59:43.000000 qudi-core-1.4.0/src/qudi/util/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:59:58.601395 qudi-core-1.4.0/src/qudi_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-06-21 08:59:58.000000 qudi-core-1.4.0/src/qudi_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-06-21 08:59:58.000000 qudi-core-1.4.0/src/qudi_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 08:59:58.000000 qudi-core-1.4.0/src/qudi_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-21 08:59:58.000000 qudi-core-1.4.0/src/qudi_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 08:59:58.000000 qudi-core-1.4.0/src/qudi_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-21 08:59:58.000000 qudi-core-1.4.0/src/qudi_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-21 08:59:58.000000 qudi-core-1.4.0/src/qudi_core.egg-info/top_level.txt
```

### Comparing `qudi-core-1.3.0/AUTHORS.md` & `qudi-core-1.4.0/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/LICENSE` & `qudi-core-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/LICENSE.LESSER` & `qudi-core-1.4.0/LICENSE.LESSER`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/PKG-INFO` & `qudi-core-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: qudi-core
-Version: 1.3.0
+Version: 1.4.0
 Summary: A modular measurement application framework
 Home-page: https://github.com/Ulm-IQO/qudi-core
 License: LGPLv3
 Project-URL: Documentation, https://ulm-iqo.github.io/qudi-core/
 Project-URL: Source Code, https://github.com/Ulm-IQO/qudi-core/
 Project-URL: Bug Tracker, https://github.com/Ulm-IQO/qudi-core/issues/
-Keywords: qudi,diamond,quantum,confocal,experiment,measurement,framework,lab,laboratory,instrumentation,instrument,modular
+Keywords: qudi,diamond,quantum,confocal,automation,experiment,measurement,framework,lab,laboratory,instrumentation,instrument,modular
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: X11 Applications
 Classifier: Environment :: MacOS X
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: End Users/Desktop
@@ -21,18 +21,19 @@
 Classifier: Operating System :: Microsoft :: Windows :: Windows 8.1
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: User Interfaces
-Requires-Python: >=3.8, <3.10
+Requires-Python: >=3.8, <3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.LESSER
 License-File: AUTHORS.md
 
 # qudi-core
 [![License: LGPL v3](https://img.shields.io/badge/License-LGPL%20v3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0)
```

### Comparing `qudi-core-1.3.0/README.md` & `qudi-core-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/setup.py` & `qudi-core-1.4.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,26 +71,27 @@
                   'Source Code': 'https://github.com/Ulm-IQO/qudi-core/',
                   'Bug Tracker': 'https://github.com/Ulm-IQO/qudi-core/issues/',
                   },
     keywords=['qudi',
               'diamond',
               'quantum',
               'confocal',
+              'automation',
               'experiment',
               'measurement',
               'framework',
               'lab',
               'laboratory',
               'instrumentation',
               'instrument',
               'modular'
               ],
     license='LGPLv3',
     install_requires=windows_dep if sys.platform == 'win32' else unix_dep,
-    python_requires='>=3.8, <3.10',
+    python_requires='>=3.8, <3.11',
     classifiers=['Development Status :: 5 - Production/Stable',
 
                  'Environment :: Win32 (MS Windows)',
                  'Environment :: X11 Applications',
                  'Environment :: MacOS X',
 
                  'Intended Audience :: Developers',
@@ -106,14 +107,15 @@
                  'Operating System :: Microsoft :: Windows :: Windows 10',
                  'Operating System :: MacOS :: MacOS X',
                  'Operating System :: Unix',
                  'Operating System :: POSIX :: Linux',
 
                  'Programming Language :: Python :: 3.8',
                  'Programming Language :: Python :: 3.9',
+                 'Programming Language :: Python :: 3.10',
 
                  'Topic :: Scientific/Engineering',
                  'Topic :: Software Development :: Libraries :: Application Frameworks',
                  'Topic :: Software Development :: User Interfaces',
                  ],
     entry_points={
         'console_scripts': ['qudi=qudi.runnable:main',
```

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/LICENSE/Oxygen.txt` & `qudi-core-1.4.0/src/qudi/artwork/icons/LICENSE/Oxygen.txt`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/LICENSE/qudi.txt` & `qudi-core-1.4.0/src/qudi/artwork/icons/LICENSE/qudi.txt`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/accessories-calculator.svg` & `qudi-core-1.4.0/src/qudi/artwork/icons/accessories-calculator.svg`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/application-exit.svg` & `qudi-core-1.4.0/src/qudi/artwork/icons/application-exit.svg`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/auto_pois.svg` & `qudi-core-1.4.0/src/qudi/artwork/icons/auto_pois.svg`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/camera-photo.svg` & `qudi-core-1.4.0/src/qudi/artwork/icons/camera-photo.svg`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/configure.svg` & `qudi-core-1.4.0/src/qudi/artwork/icons/configure.svg`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/correct-tilt.svg` & `qudi-core-1.4.0/src/qudi/artwork/icons/correct-tilt.svg`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/dialog-warning.svgz` & `qudi-core-1.4.0/src/qudi/artwork/icons/dialog-warning.svgz`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/document-new.svg` & `qudi-core-1.4.0/src/qudi/artwork/icons/document-new.svg`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/document-open.svgz` & `qudi-core-1.4.0/src/qudi/artwork/icons/document-open.svgz`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/document-save.svg` & `qudi-core-1.4.0/src/qudi/artwork/icons/document-save.svg`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/edit-clear.svgz` & `qudi-core-1.4.0/src/qudi/artwork/icons/edit-clear.svgz`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/edit-copy.svgz` & `qudi-core-1.4.0/src/qudi/artwork/icons/edit-copy.svgz`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/edit-cut.svgz` & `qudi-core-1.4.0/src/qudi/artwork/icons/edit-cut.svgz`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/edit-delete-shred.svgz` & `qudi-core-1.4.0/src/qudi/artwork/icons/edit-delete-shred.svgz`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/edit-delete.svgz` & `qudi-core-1.4.0/src/qudi/artwork/icons/edit-delete.svgz`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/go-home.svg` & `qudi-core-1.4.0/src/qudi/artwork/icons/go-home.svg`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/go-next.svgz` & `qudi-core-1.4.0/src/qudi/artwork/icons/go-next.svgz`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/go-previous.svgz` & `qudi-core-1.4.0/src/qudi/artwork/icons/go-previous.svgz`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/goto-poi.svgz` & `qudi-core-1.4.0/src/qudi/artwork/icons/goto-poi.svgz`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/list-add.svg` & `qudi-core-1.4.0/src/qudi/artwork/icons/list-add.svg`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/list-remove.svg` & `qudi-core-1.4.0/src/qudi/artwork/icons/list-remove.svg`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/media-playback-pause.svgz` & `qudi-core-1.4.0/src/qudi/artwork/icons/media-playback-pause.svgz`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/media-playback-start.svgz` & `qudi-core-1.4.0/src/qudi/artwork/icons/media-playback-start.svgz`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/media-playback-stop.svgz` & `qudi-core-1.4.0/src/qudi/artwork/icons/media-playback-stop.svgz`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/media-record.svgz` & `qudi-core-1.4.0/src/qudi/artwork/icons/media-record.svgz`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/mouse_pointer.svg` & `qudi-core-1.4.0/src/qudi/artwork/icons/mouse_pointer.svg`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/network-connect.svg` & `qudi-core-1.4.0/src/qudi/artwork/icons/network-connect.svg`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/network-disconnect.svg` & `qudi-core-1.4.0/src/qudi/artwork/icons/network-disconnect.svg`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/new_poi_crosshair.svg` & `qudi-core-1.4.0/src/qudi/artwork/icons/new_poi_crosshair.svg`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/new_poi_mouse.svg` & `qudi-core-1.4.0/src/qudi/artwork/icons/new_poi_mouse.svg`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/object-rotate-left.svgz` & `qudi-core-1.4.0/src/qudi/artwork/icons/object-rotate-left.svgz`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/object-rotate-right.svgz` & `qudi-core-1.4.0/src/qudi/artwork/icons/object-rotate-right.svgz`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/optimize-position-poi.svgz` & `qudi-core-1.4.0/src/qudi/artwork/icons/optimize-position-poi.svgz`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/optimize-position.svg` & `qudi-core-1.4.0/src/qudi/artwork/icons/optimize-position.svg`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/periodic-refind-poi.svgz` & `qudi-core-1.4.0/src/qudi/artwork/icons/periodic-refind-poi.svgz`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/poi-new.svg` & `qudi-core-1.4.0/src/qudi/artwork/icons/poi-new.svg`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/record-counter.svgz` & `qudi-core-1.4.0/src/qudi/artwork/icons/record-counter.svgz`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/restart-counter.svg` & `qudi-core-1.4.0/src/qudi/artwork/icons/restart-counter.svg`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/scan-depth-loop.svg` & `qudi-core-1.4.0/src/qudi/artwork/icons/scan-depth-loop.svg`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/scan-depth-restart.svg` & `qudi-core-1.4.0/src/qudi/artwork/icons/scan-depth-restart.svg`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/scan-depth-start.svg` & `qudi-core-1.4.0/src/qudi/artwork/icons/scan-depth-start.svg`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/scan-stop.svg` & `qudi-core-1.4.0/src/qudi/artwork/icons/scan-stop.svg`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/scan-xy-loop.svg` & `qudi-core-1.4.0/src/qudi/artwork/icons/scan-xy-loop.svg`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/scan-xy-restart.svg` & `qudi-core-1.4.0/src/qudi/artwork/icons/scan-xy-restart.svg`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/scan-xy-start.svg` & `qudi-core-1.4.0/src/qudi/artwork/icons/scan-xy-start.svg`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/start-counter.svg` & `qudi-core-1.4.0/src/qudi/artwork/icons/start-counter.svg`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/stop-counter.svg` & `qudi-core-1.4.0/src/qudi/artwork/icons/stop-counter.svg`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/utilities-terminal.svgz` & `qudi-core-1.4.0/src/qudi/artwork/icons/utilities-terminal.svgz`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/view-filter.svg` & `qudi-core-1.4.0/src/qudi/artwork/icons/view-filter.svg`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/view-refresh.svg` & `qudi-core-1.4.0/src/qudi/artwork/icons/view-refresh.svg`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/zoom-fit-best.svg` & `qudi-core-1.4.0/src/qudi/artwork/icons/zoom-fit-best.svg`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/icons/zoom-select.svgz` & `qudi-core-1.4.0/src/qudi/artwork/icons/zoom-select.svgz`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/logo/LICENSE.txt` & `qudi-core-1.4.0/src/qudi/artwork/logo/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/logo/logo-qudi.svg` & `qudi-core-1.4.0/src/qudi/artwork/logo/logo-qudi.svg`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/logo/logo_qudi.ico` & `qudi-core-1.4.0/src/qudi/artwork/logo/logo_qudi.ico`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/styles/dracula.qss` & `qudi-core-1.4.0/src/qudi/artwork/styles/dracula.qss`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/styles/qdark/LICENSE.txt` & `qudi-core-1.4.0/src/qudi/artwork/styles/qdark/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/styles/qdark/checkbox_checked_focus.png` & `qudi-core-1.4.0/src/qudi/artwork/styles/qdark/checkbox_checked_focus.png`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/styles/qdark/checkbox_indeterminate_focus.png` & `qudi-core-1.4.0/src/qudi/artwork/styles/qdark/checkbox_indeterminate_focus.png`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/styles/qdark/close-hover.png` & `qudi-core-1.4.0/src/qudi/artwork/styles/qdark/close-hover.png`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/styles/qdark/close-pressed.png` & `qudi-core-1.4.0/src/qudi/artwork/styles/qdark/close-pressed.png`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/styles/qdark/close.png` & `qudi-core-1.4.0/src/qudi/artwork/styles/qdark/close.png`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/styles/qdark/radio_checked.png` & `qudi-core-1.4.0/src/qudi/artwork/styles/qdark/radio_checked.png`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/styles/qdark/radio_checked_disabled.png` & `qudi-core-1.4.0/src/qudi/artwork/styles/qdark/radio_checked_disabled.png`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/styles/qdark/radio_checked_focus.png` & `qudi-core-1.4.0/src/qudi/artwork/styles/qdark/radio_checked_focus.png`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/styles/qdark/radio_unchecked.png` & `qudi-core-1.4.0/src/qudi/artwork/styles/qdark/radio_unchecked.png`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/styles/qdark/radio_unchecked_disabled.png` & `qudi-core-1.4.0/src/qudi/artwork/styles/qdark/radio_unchecked_disabled.png`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/styles/qdark/radio_unchecked_focus.png` & `qudi-core-1.4.0/src/qudi/artwork/styles/qdark/radio_unchecked_focus.png`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/styles/qdark/svg/checkbox_checked.svg` & `qudi-core-1.4.0/src/qudi/artwork/styles/qdark/svg/checkbox_checked.svg`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/styles/qdark/svg/checkbox_checked_disabled.svg` & `qudi-core-1.4.0/src/qudi/artwork/styles/qdark/svg/checkbox_checked_disabled.svg`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/styles/qdark/svg/checkbox_checked_focus.svg` & `qudi-core-1.4.0/src/qudi/artwork/styles/qdark/svg/checkbox_checked_focus.svg`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/styles/qdark/svg/checkbox_indeterminate.svg` & `qudi-core-1.4.0/src/qudi/artwork/styles/qdark/svg/checkbox_indeterminate.svg`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/styles/qdark/svg/checkbox_indeterminate_disabled.svg` & `qudi-core-1.4.0/src/qudi/artwork/styles/qdark/svg/checkbox_indeterminate_disabled.svg`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/styles/qdark/svg/checkbox_indeterminate_focus.svg` & `qudi-core-1.4.0/src/qudi/artwork/styles/qdark/svg/checkbox_indeterminate_focus.svg`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/styles/qdark/svg/checkbox_unchecked.svg` & `qudi-core-1.4.0/src/qudi/artwork/styles/qdark/svg/checkbox_unchecked.svg`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/styles/qdark/svg/checkbox_unchecked_disabled.svg` & `qudi-core-1.4.0/src/qudi/artwork/styles/qdark/svg/checkbox_unchecked_disabled.svg`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/styles/qdark/svg/checkbox_unchecked_focus.svg` & `qudi-core-1.4.0/src/qudi/artwork/styles/qdark/svg/checkbox_unchecked_focus.svg`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/styles/qdark/svg/radio_checked.svg` & `qudi-core-1.4.0/src/qudi/artwork/styles/qdark/svg/radio_checked.svg`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/styles/qdark/svg/radio_checked_disabled.svg` & `qudi-core-1.4.0/src/qudi/artwork/styles/qdark/svg/radio_checked_disabled.svg`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/styles/qdark/svg/radio_checked_focus.svg` & `qudi-core-1.4.0/src/qudi/artwork/styles/qdark/svg/radio_checked_focus.svg`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/styles/qdark/svg/radio_unchecked.svg` & `qudi-core-1.4.0/src/qudi/artwork/styles/qdark/svg/radio_unchecked.svg`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/styles/qdark/svg/radio_unchecked_disabled.svg` & `qudi-core-1.4.0/src/qudi/artwork/styles/qdark/svg/radio_unchecked_disabled.svg`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/styles/qdark/svg/radio_unchecked_focus.svg` & `qudi-core-1.4.0/src/qudi/artwork/styles/qdark/svg/radio_unchecked_focus.svg`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/styles/qdark/undock.png` & `qudi-core-1.4.0/src/qudi/artwork/styles/qdark/undock.png`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/styles/qdark.qss` & `qudi-core-1.4.0/src/qudi/artwork/styles/qdark.qss`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/artwork/styles/qtdark.qss` & `qudi-core-1.4.0/src/qudi/artwork/styles/qtdark.qss`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/core/__init__.py` & `qudi-core-1.4.0/src/qudi/core/__init__.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/core/__main__.py` & `qudi-core-1.4.0/src/qudi/core/__main__.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/core/application.py` & `qudi-core-1.4.0/src/qudi/core/application.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/core/config/__init__.py` & `qudi-core-1.4.0/src/qudi/core/config/__init__.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/core/config/config.py` & `qudi-core-1.4.0/src/qudi/core/config/config.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/core/config/file_handler.py` & `qudi-core-1.4.0/src/qudi/core/config/file_handler.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/core/config/schema.py` & `qudi-core-1.4.0/src/qudi/core/config/schema.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/core/config/validator.py` & `qudi-core-1.4.0/src/qudi/core/config/validator.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/core/configoption.py` & `qudi-core-1.4.0/src/qudi/core/configoption.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/core/connector.py` & `qudi-core-1.4.0/src/qudi/core/connector.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/core/gui/gui.py` & `qudi-core-1.4.0/src/qudi/core/gui/gui.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/core/gui/main_gui/aboutqudidialog.py` & `qudi-core-1.4.0/src/qudi/core/gui/main_gui/aboutqudidialog.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/core/gui/main_gui/configwidget.py` & `qudi-core-1.4.0/src/qudi/core/gui/main_gui/configwidget.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/core/gui/main_gui/errordialog.py` & `qudi-core-1.4.0/src/qudi/core/gui/main_gui/errordialog.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/core/gui/main_gui/logwidget.py` & `qudi-core-1.4.0/src/qudi/core/gui/main_gui/logwidget.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/core/gui/main_gui/main_gui.py` & `qudi-core-1.4.0/src/qudi/core/gui/main_gui/main_gui.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/core/gui/main_gui/mainwindow.py` & `qudi-core-1.4.0/src/qudi/core/gui/main_gui/mainwindow.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/core/gui/main_gui/modulewidget.py` & `qudi-core-1.4.0/src/qudi/core/gui/main_gui/modulewidget.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/core/gui/main_gui/remotewidget.py` & `qudi-core-1.4.0/src/qudi/core/gui/main_gui/remotewidget.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/core/gui/main_gui/settingsdialog.py` & `qudi-core-1.4.0/src/qudi/core/gui/main_gui/settingsdialog.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/core/interface.py` & `qudi-core-1.4.0/src/qudi/core/interface.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/core/logger/__init__.py` & `qudi-core-1.4.0/src/qudi/core/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/core/logger/handlers.py` & `qudi-core-1.4.0/src/qudi/core/logger/handlers.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/core/logger/records_model.py` & `qudi-core-1.4.0/src/qudi/core/logger/records_model.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/core/meta.py` & `qudi-core-1.4.0/src/qudi/core/meta.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/core/module.py` & `qudi-core-1.4.0/src/qudi/core/module.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/core/modulemanager.py` & `qudi-core-1.4.0/src/qudi/core/modulemanager.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/core/parentpoller.py` & `qudi-core-1.4.0/src/qudi/core/parentpoller.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/core/qudikernel.py` & `qudi-core-1.4.0/src/qudi/core/qudikernel.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/core/scripting/modulescript.py` & `qudi-core-1.4.0/src/qudi/core/scripting/modulescript.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/core/scripting/moduletask.py` & `qudi-core-1.4.0/src/qudi/core/scripting/moduletask.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/core/servers.py` & `qudi-core-1.4.0/src/qudi/core/servers.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/core/services.py` & `qudi-core-1.4.0/src/qudi/core/services.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/core/statusvariable.py` & `qudi-core-1.4.0/src/qudi/core/statusvariable.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/core/threadmanager.py` & `qudi-core-1.4.0/src/qudi/core/threadmanager.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/core/watchdog.py` & `qudi-core-1.4.0/src/qudi/core/watchdog.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/gui/taskrunner/main_window.py` & `qudi-core-1.4.0/src/qudi/gui/taskrunner/main_window.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/gui/taskrunner/task_runner_gui.py` & `qudi-core-1.4.0/src/qudi/gui/taskrunner/task_runner_gui.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/gui/taskrunner/taskwidget.py` & `qudi-core-1.4.0/src/qudi/gui/taskrunner/taskwidget.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/logic/taskrunner.py` & `qudi-core-1.4.0/src/qudi/logic/taskrunner.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/runnable.py` & `qudi-core-1.4.0/src/qudi/runnable.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/tasks/test_tasks.py` & `qudi-core-1.4.0/src/qudi/tasks/test_tasks.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/tools/config_editor/__init__.py` & `qudi-core-1.4.0/src/qudi/tools/config_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/tools/config_editor/__main__.py` & `qudi-core-1.4.0/src/qudi/tools/config_editor/__main__.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/tools/config_editor/config_editor.py` & `qudi-core-1.4.0/src/qudi/tools/config_editor/config_editor.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/tools/config_editor/custom_widgets.py` & `qudi-core-1.4.0/src/qudi/tools/config_editor/custom_widgets.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/tools/config_editor/global_editor.py` & `qudi-core-1.4.0/src/qudi/tools/config_editor/global_editor.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/tools/config_editor/global_widgets.py` & `qudi-core-1.4.0/src/qudi/tools/config_editor/global_widgets.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/tools/config_editor/module_editor.py` & `qudi-core-1.4.0/src/qudi/tools/config_editor/module_editor.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/tools/config_editor/module_finder.py` & `qudi-core-1.4.0/src/qudi/tools/config_editor/module_finder.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/tools/config_editor/module_selector.py` & `qudi-core-1.4.0/src/qudi/tools/config_editor/module_selector.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/tools/config_editor/module_widgets.py` & `qudi-core-1.4.0/src/qudi/tools/config_editor/module_widgets.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/tools/config_editor/tree_widgets.py` & `qudi-core-1.4.0/src/qudi/tools/config_editor/tree_widgets.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/util/colordefs.py` & `qudi-core-1.4.0/src/qudi/util/colordefs.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/util/constraints.py` & `qudi-core-1.4.0/src/qudi/util/constraints.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,22 +34,22 @@
                  increment: Optional[Union[int, float]] = None,
                  enforce_int: Optional[bool] = False,
                  checker: Optional[Callable[[Union[int, float]], bool]] = None
                  ) -> None:
         """
         """
         self._enforce_int = bool(enforce_int)
-        self._check_value_type(default)
+        self.check_value_type(default)
         for value in bounds:
-            self._check_value_type(value)
+            self.check_value_type(value)
         if increment is not None:
-            self._check_value_type(increment)
+            self.check_value_type(increment)
         if checker is not None and not callable(checker):
-            raise TypeError('checker must be eithe None or a callable accepting a single scalar '
-                            'and returning a bool.')
+            raise TypeError('checker must be either None or a callable accepting a single scalar '
+                            'and returning a valid-flag bool or raising ValueError')
         self._default = default
         self._minimum, self._maximum = sorted(bounds)
         self._increment = increment
         self._checker = checker
 
         if not self.is_valid(self._default):
             raise ValueError(f'invalid default value ({self._default}) encountered')
@@ -74,38 +74,45 @@
     def increment(self) -> Union[None, int, float]:
         return self._increment
 
     @property
     def enforce_int(self) -> bool:
         return self._enforce_int
 
+    def check(self, value: Union[int, float]) -> None:
+        self.check_value_type(value)
+        self.check_value_range(value)
+        self.check_custom(value)
+
     def is_valid(self, value: Union[int, float]) -> bool:
         try:
-            self._check_value_type(value)
-        except TypeError:
+            self.check(value)
+        except (ValueError, TypeError):
             return False
-
-        if self._minimum <= value <= self._maximum:
-            if self._checker is None:
-                return True
-            else:
-                return self._checker(value)
-        return False
+        return True
 
     def clip(self, value: Union[int, float]) -> Union[int, float]:
         return min(self._maximum, max(self._minimum, value))
 
     def copy(self) -> object:
         return ScalarConstraint(default=self.default,
                                 bounds=self.bounds,
                                 increment=self.increment,
                                 enforce_int=self.enforce_int,
                                 checker=self._checker)
 
-    def _check_value_type(self, value: Any) -> None:
+    def check_custom(self, value: Any) -> None:
+        if (self._checker is not None) and (not self._checker(value)):
+            raise ValueError(f'Custom checker failed to validate value "{value}"')
+
+    def check_value_range(self, value: Union[int, float]) -> None:
+        if not (self._minimum <= value <= self._maximum):
+            raise ValueError(f'Value "{value}" is out of bounds {self.bounds}')
+
+    def check_value_type(self, value: Any) -> None:
         if self._enforce_int:
             if not is_integer(value):
                 raise TypeError(f'values must be int type (received {value})')
         else:
             if not (is_integer(value) or is_float(value)):
                 raise TypeError(f'values must be int or float type (received {value})')
```

### Comparing `qudi-core-1.3.0/src/qudi/util/datafitting.py` & `qudi-core-1.4.0/src/qudi/util/datafitting.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/util/datastorage.py` & `qudi-core-1.4.0/src/qudi/util/datastorage.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/util/filters.py` & `qudi-core-1.4.0/src/qudi/util/filters.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/util/fit_models/exp_decay.py` & `qudi-core-1.4.0/src/qudi/util/fit_models/exp_decay.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/util/fit_models/gaussian.py` & `qudi-core-1.4.0/src/qudi/util/fit_models/gaussian.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/util/fit_models/helpers.py` & `qudi-core-1.4.0/src/qudi/util/fit_models/helpers.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/util/fit_models/linear.py` & `qudi-core-1.4.0/src/qudi/util/fit_models/linear.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/util/fit_models/lorentzian.py` & `qudi-core-1.4.0/src/qudi/util/fit_models/lorentzian.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/util/fit_models/model.py` & `qudi-core-1.4.0/src/qudi/util/fit_models/model.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/util/fit_models/poissonian.py` & `qudi-core-1.4.0/src/qudi/util/fit_models/poissonian.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/util/fit_models/sine.py` & `qudi-core-1.4.0/src/qudi/util/fit_models/sine.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/util/helpers.py` & `qudi-core-1.4.0/src/qudi/util/helpers.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/util/mapper.py` & `qudi-core-1.4.0/src/qudi/util/mapper.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/util/math.py` & `qudi-core-1.4.0/src/qudi/util/math.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/util/models.py` & `qudi-core-1.4.0/src/qudi/util/models.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/util/mutex.py` & `qudi-core-1.4.0/src/qudi/util/mutex.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/util/network.py` & `qudi-core-1.4.0/src/qudi/util/network.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/util/overload.py` & `qudi-core-1.4.0/src/qudi/util/overload.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/util/parameters.py` & `qudi-core-1.4.0/src/qudi/util/parameters.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/util/paths.py` & `qudi-core-1.4.0/src/qudi/util/paths.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/util/uic.py` & `qudi-core-1.4.0/src/qudi/util/uic.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/util/units.py` & `qudi-core-1.4.0/src/qudi/util/units.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/util/widgets/advanced_dockwidget.py` & `qudi-core-1.4.0/src/qudi/util/widgets/advanced_dockwidget.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/util/widgets/collapsible.py` & `qudi-core-1.4.0/src/qudi/util/widgets/collapsible.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/util/widgets/fitting.py` & `qudi-core-1.4.0/src/qudi/util/widgets/fitting.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/util/widgets/literal_lineedit.py` & `qudi-core-1.4.0/src/qudi/util/widgets/literal_lineedit.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/util/widgets/loading_indicator.py` & `qudi-core-1.4.0/src/qudi/util/widgets/loading_indicator.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/util/widgets/parameter_editor.py` & `qudi-core-1.4.0/src/qudi/util/widgets/parameter_editor.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/util/widgets/path_line_edit.py` & `qudi-core-1.4.0/src/qudi/util/widgets/path_line_edit.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/util/widgets/plotting/axis.py` & `qudi-core-1.4.0/src/qudi/util/widgets/plotting/axis.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/util/widgets/plotting/colorbar.py` & `qudi-core-1.4.0/src/qudi/util/widgets/plotting/colorbar.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/util/widgets/plotting/image_widget.py` & `qudi-core-1.4.0/src/qudi/util/widgets/plotting/image_widget.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/util/widgets/plotting/interactive_curve.py` & `qudi-core-1.4.0/src/qudi/util/widgets/plotting/interactive_curve.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/util/widgets/plotting/marker.py` & `qudi-core-1.4.0/src/qudi/util/widgets/plotting/marker.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/util/widgets/plotting/plot_item.py` & `qudi-core-1.4.0/src/qudi/util/widgets/plotting/plot_item.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/util/widgets/plotting/plot_widget.py` & `qudi-core-1.4.0/src/qudi/util/widgets/plotting/plot_widget.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/util/widgets/plotting/roi.py` & `qudi-core-1.4.0/src/qudi/util/widgets/plotting/roi.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/util/widgets/plotting/view_box.py` & `qudi-core-1.4.0/src/qudi/util/widgets/plotting/view_box.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/util/widgets/scientific_spinbox.py` & `qudi-core-1.4.0/src/qudi/util/widgets/scientific_spinbox.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/util/widgets/separator_lines.py` & `qudi-core-1.4.0/src/qudi/util/widgets/separator_lines.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/util/widgets/slider.py` & `qudi-core-1.4.0/src/qudi/util/widgets/slider.py`

 * *Files 7% similar despite different names*

```diff
@@ -64,17 +64,19 @@
         return self._maximum_value
 
     def value(self):
         int_val = super().value()
         return self.minimum() + (self.maximum() - self.minimum()) * (int_val / self._step_number)
 
     def setValue(self, val):
-        int_val = round((val - self.minimum()) * self._step_number / (self.maximum() - self.minimum()))
+        max_val = self.maximum()
+        min_val = self.minimum()
+        val = max(min_val, min(max_val, val))
+        int_val = int(round((val - min_val) * self._step_number / (max_val - min_val)))
         super().setValue(int_val)
-        return
 
     @property
     def granularity(self) -> int:
         return self._step_number + 1
 
     def set_granularity(self, number_of_steps):
         """
```

### Comparing `qudi-core-1.3.0/src/qudi/util/widgets/toggle_switch.py` & `qudi-core-1.4.0/src/qudi/util/widgets/toggle_switch.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi/util/yaml.py` & `qudi-core-1.4.0/src/qudi/util/yaml.py`

 * *Files identical despite different names*

### Comparing `qudi-core-1.3.0/src/qudi_core.egg-info/PKG-INFO` & `qudi-core-1.4.0/src/qudi_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: qudi-core
-Version: 1.3.0
+Version: 1.4.0
 Summary: A modular measurement application framework
 Home-page: https://github.com/Ulm-IQO/qudi-core
 License: LGPLv3
 Project-URL: Documentation, https://ulm-iqo.github.io/qudi-core/
 Project-URL: Source Code, https://github.com/Ulm-IQO/qudi-core/
 Project-URL: Bug Tracker, https://github.com/Ulm-IQO/qudi-core/issues/
-Keywords: qudi,diamond,quantum,confocal,experiment,measurement,framework,lab,laboratory,instrumentation,instrument,modular
+Keywords: qudi,diamond,quantum,confocal,automation,experiment,measurement,framework,lab,laboratory,instrumentation,instrument,modular
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: X11 Applications
 Classifier: Environment :: MacOS X
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: End Users/Desktop
@@ -21,18 +21,19 @@
 Classifier: Operating System :: Microsoft :: Windows :: Windows 8.1
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: User Interfaces
-Requires-Python: >=3.8, <3.10
+Requires-Python: >=3.8, <3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.LESSER
 License-File: AUTHORS.md
 
 # qudi-core
 [![License: LGPL v3](https://img.shields.io/badge/License-LGPL%20v3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0)
```

### Comparing `qudi-core-1.3.0/src/qudi_core.egg-info/SOURCES.txt` & `qudi-core-1.4.0/src/qudi_core.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -176,14 +176,15 @@
 src/qudi/tools/config_editor/module_selector.py
 src/qudi/tools/config_editor/module_widgets.py
 src/qudi/tools/config_editor/tree_widgets.py
 src/qudi/util/colordefs.py
 src/qudi/util/constraints.py
 src/qudi/util/datafitting.py
 src/qudi/util/datastorage.py
+src/qudi/util/descriptors.py
 src/qudi/util/filters.py
 src/qudi/util/helpers.py
 src/qudi/util/mapper.py
 src/qudi/util/math.py
 src/qudi/util/models.py
 src/qudi/util/mutex.py
 src/qudi/util/network.py
```

