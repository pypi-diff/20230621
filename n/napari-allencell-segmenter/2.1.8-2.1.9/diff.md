# Comparing `tmp/napari-allencell-segmenter-2.1.8.tar.gz` & `tmp/napari-allencell-segmenter-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-allencell-segmenter-2.1.8.tar", last modified: Wed Jan 11 19:05:19 2023, max compression
+gzip compressed data, was "napari-allencell-segmenter-2.1.9.tar", last modified: Fri Feb  3 18:20:23 2023, max compression
```

## Comparing `napari-allencell-segmenter-2.1.8.tar` & `napari-allencell-segmenter-2.1.9.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 19:05:19.620468 napari-allencell-segmenter-2.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-01-11 19:05:19.624468 napari-allencell-segmenter-2.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 19:05:19.612468 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_dock_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_style.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 19:05:19.612468 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 19:05:19.612468 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/controller/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/controller/batch_processing_controller_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/controller/workflow_select_controller_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    25061 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/controller/workflow_steps_controller_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 19:05:19.616468 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/core/application_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/core/controller_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/core/layer_reader_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/core/router_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/core/state_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/core/view_manager_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/core/view_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/core/viewer_abstraction_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/mocks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 19:05:19.616468 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/model/segmenter_model_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/style_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 19:05:19.616468 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/util/convert_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/util/lazy_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 19:05:19.616468 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/view/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/view/_main_template_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/view/batch_processing_view_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/view/workflow_select_view_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/view/workflow_steps_view_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 19:05:19.616468 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/widgets/collapsible_box_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/widgets/file_input_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/widgets/warning_message_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/widgets/workflow_step_widget_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/widgets/workflow_thumbnails_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 19:05:19.612468 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 19:05:19.616468 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/assets/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/assets/icons/expand_less_black_24dp.svg
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/assets/icons/expand_more_black_24dp.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/assets/icons/gear.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/assets/icons/icon-parameter-sweep.svg
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/assets/icons/warning.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 19:05:19.616468 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/controller/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/controller/_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/controller/batch_processing_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/controller/workflow_select_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    25183 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/controller/workflow_steps_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 19:05:19.620468 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/core/_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/core/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/core/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/core/layer_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/core/router.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/core/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/core/view.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/core/view_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/core/viewer_abstraction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 19:05:19.620468 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/model/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/model/segmenter_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 19:05:19.620468 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/styles/
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/styles/main.qss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 19:05:19.620468 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/util/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/util/debug_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/util/directories.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/util/lazy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/util/ui_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 19:05:19.620468 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/view/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/view/_main_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/view/batch_processing_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/view/workflow_select_view.py
--rw-r--r--   0 runner    (1001) docker     (123)    10297 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/view/workflow_steps_view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 19:05:19.620468 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/widgets/batch_complete_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/widgets/collapsible_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/widgets/file_input.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/widgets/float_slider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/widgets/form.py
--rw-r--r--   0 runner    (1001) docker     (123)    18618 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/widgets/param_sweep_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/widgets/warning_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/widgets/workflow_step_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/widgets/workflow_thumbnails.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 19:05:19.612468 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-01-11 19:05:19.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-01-11 19:05:19.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 19:05:19.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-01-11 19:05:19.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 19:05:19.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-01-11 19:05:19.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-01-11 19:05:19.000000 napari-allencell-segmenter-2.1.8/napari_allencell_segmenter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-01-11 19:05:19.624468 napari-allencell-segmenter-2.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-01-11 19:05:15.000000 napari-allencell-segmenter-2.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 18:20:23.714202 napari-allencell-segmenter-2.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-02-03 18:20:23.714202 napari-allencell-segmenter-2.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 18:20:23.710202 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_dock_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_style.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 18:20:23.710202 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 18:20:23.710202 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/controller/batch_processing_controller_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/controller/workflow_select_controller_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25061 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/controller/workflow_steps_controller_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 18:20:23.710202 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/core/application_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/core/controller_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/core/layer_reader_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/core/router_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/core/state_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/core/view_manager_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/core/view_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/core/viewer_abstraction_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/mocks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 18:20:23.710202 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/model/segmenter_model_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/style_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 18:20:23.710202 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/util/convert_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/util/lazy_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 18:20:23.710202 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/view/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/view/_main_template_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/view/batch_processing_view_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/view/workflow_select_view_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/view/workflow_steps_view_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 18:20:23.710202 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/widgets/collapsible_box_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/widgets/file_input_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/widgets/warning_message_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/widgets/workflow_step_widget_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/widgets/workflow_thumbnails_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 18:20:23.706202 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 18:20:23.710202 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/assets/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/assets/icons/expand_less_black_24dp.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/assets/icons/expand_more_black_24dp.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/assets/icons/gear.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/assets/icons/icon-parameter-sweep.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/assets/icons/warning.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 18:20:23.714202 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/controller/_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/controller/batch_processing_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/controller/workflow_select_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25183 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/controller/workflow_steps_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 18:20:23.714202 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/core/_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/core/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/core/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/core/layer_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/core/router.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/core/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/core/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/core/view_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/core/viewer_abstraction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 18:20:23.714202 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/model/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/model/segmenter_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 18:20:23.714202 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/styles/main.qss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 18:20:23.714202 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/util/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/util/debug_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/util/directories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/util/lazy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/util/ui_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 18:20:23.714202 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/view/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/view/_main_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/view/batch_processing_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/view/workflow_select_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10297 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/view/workflow_steps_view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 18:20:23.714202 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/widgets/batch_complete_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/widgets/collapsible_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/widgets/file_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/widgets/float_slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/widgets/form.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18867 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/widgets/param_sweep_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/widgets/warning_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/widgets/workflow_step_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/widgets/workflow_thumbnails.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 18:20:23.710202 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-02-03 18:20:23.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-02-03 18:20:23.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 18:20:23.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-02-03 18:20:23.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 18:20:23.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-02-03 18:20:23.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-03 18:20:23.000000 napari-allencell-segmenter-2.1.9/napari_allencell_segmenter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-02-03 18:20:23.718202 napari-allencell-segmenter-2.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-02-03 18:20:18.000000 napari-allencell-segmenter-2.1.9/setup.py
```

### Comparing `napari-allencell-segmenter-2.1.8/LICENSE` & `napari-allencell-segmenter-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/PKG-INFO` & `napari-allencell-segmenter-2.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-allencell-segmenter
-Version: 2.1.8
+Version: 2.1.9
 Summary: A plugin that enables 3D image segmentation provided by Allen Institute for Cell Science
 Home-page: https://github.com/AllenCell/napari-allencell-segmenter
 Author: Allen Institute for Cell Science
 License: BSD-3
 Project-URL: Bug Tracker, https://github.com/AllenCell/napari-allencell-segmenter/issues
 Project-URL: Documentation, https://github.com/AllenCell/napari-allencell-segmenter#README.md
 Project-URL: Source Code, https://github.com/AllenCell/napari-allencell-segmenter
```

### Comparing `napari-allencell-segmenter-2.1.8/README.md` & `napari-allencell-segmenter-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_dock_widget.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_dock_widget.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_style.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_style.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/conftest.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/controller/batch_processing_controller_test.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/controller/batch_processing_controller_test.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/controller/workflow_select_controller_test.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/controller/workflow_select_controller_test.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/controller/workflow_steps_controller_test.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/controller/workflow_steps_controller_test.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/core/application_test.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/core/application_test.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/core/controller_test.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/core/controller_test.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/core/layer_reader_test.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/core/layer_reader_test.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/core/router_test.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/core/router_test.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/core/view_manager_test.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/core/view_manager_test.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/core/view_test.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/core/view_test.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/core/viewer_abstraction_test.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/core/viewer_abstraction_test.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/mocks.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/mocks.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/model/segmenter_model_test.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/model/segmenter_model_test.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/style_test.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/style_test.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/util/convert_test.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/util/convert_test.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/view/batch_processing_view_test.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/view/batch_processing_view_test.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/view/workflow_select_view_test.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/view/workflow_select_view_test.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/view/workflow_steps_view_test.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/view/workflow_steps_view_test.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/widgets/collapsible_box_test.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/widgets/collapsible_box_test.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/widgets/warning_message_test.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/widgets/warning_message_test.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/widgets/workflow_step_widget_test.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/widgets/workflow_step_widget_test.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/_tests/widgets/workflow_thumbnails_test.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/_tests/widgets/workflow_thumbnails_test.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/assets/icons/gear.svg` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/assets/icons/gear.svg`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/assets/icons/icon-parameter-sweep.svg` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/assets/icons/icon-parameter-sweep.svg`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/assets/icons/warning.png` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/assets/icons/warning.png`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/controller/_interfaces.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/controller/_interfaces.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/controller/batch_processing_controller.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/controller/batch_processing_controller.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/controller/workflow_select_controller.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/controller/workflow_select_controller.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/controller/workflow_steps_controller.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/controller/workflow_steps_controller.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/core/_interfaces.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/core/_interfaces.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/core/application.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/core/application.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/core/controller.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/core/controller.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/core/layer_reader.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/core/layer_reader.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/core/router.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/core/router.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/core/view.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/core/view.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/core/view_manager.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/core/view_manager.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/core/viewer_abstraction.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/core/viewer_abstraction.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/model/segmenter_model.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/model/segmenter_model.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/styles/main.qss` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/styles/main.qss`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/util/convert.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/util/convert.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/util/debug_utils.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/util/debug_utils.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/util/directories.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/util/directories.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/util/ui_utils.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/util/ui_utils.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/view/_main_template.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/view/_main_template.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/view/batch_processing_view.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/view/batch_processing_view.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/view/workflow_select_view.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/view/workflow_select_view.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/view/workflow_steps_view.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/view/workflow_steps_view.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/widgets/batch_complete_dialog.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/widgets/batch_complete_dialog.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/widgets/collapsible_box.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/widgets/collapsible_box.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/widgets/file_input.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/widgets/file_input.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/widgets/float_slider.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/widgets/float_slider.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/widgets/form.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/widgets/form.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/widgets/param_sweep_widget.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/widgets/param_sweep_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     QComboBox,
 )
 from qtpy.QtCore import Qt
 from typing import Dict, Any, List
 from napari_allencell_segmenter.widgets.form import Form, FormRow
 from functools import partial
 from napari.qt import get_stylesheet
+from napari_allencell_segmenter.widgets.warning_message import WarningMessage
 
 
 class ParamSweepWidget(QDialog):
     """
     A dialog box containing a workflow finished message. Also includes a button to open the output folder
     and a button to close the dialog box
 
@@ -195,14 +196,19 @@
         """
         Initiate a sweep (called when run sweep button is pressed) with the values provided in the UI
 
         Params:
            none
         """
         inputs: List[List[str]] = self.grab_ui_values(grab_combo=False)
+        try:
+            self.sanitize_ui_inputs(inputs)
+        except ValueError:
+            WarningMessage("Please enter valid numbers for sweep parameters.").show()
+
         count: int = self.get_live_count(inputs)
         if count > 20:
             # warn if too many images will be generated
             if self.warn_images_created(count) == 1024:
                 self.set_run_in_progress()
                 self.controller.run_step_sweep(self, self.grab_ui_values())
         else:
```

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/widgets/warning_message.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/widgets/warning_message.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/widgets/workflow_step_widget.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/widgets/workflow_step_widget.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter/widgets/workflow_thumbnails.py` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter/widgets/workflow_thumbnails.py`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter.egg-info/PKG-INFO` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-allencell-segmenter
-Version: 2.1.8
+Version: 2.1.9
 Summary: A plugin that enables 3D image segmentation provided by Allen Institute for Cell Science
 Home-page: https://github.com/AllenCell/napari-allencell-segmenter
 Author: Allen Institute for Cell Science
 License: BSD-3
 Project-URL: Bug Tracker, https://github.com/AllenCell/napari-allencell-segmenter/issues
 Project-URL: Documentation, https://github.com/AllenCell/napari-allencell-segmenter#README.md
 Project-URL: Source Code, https://github.com/AllenCell/napari-allencell-segmenter
```

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter.egg-info/SOURCES.txt` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari-allencell-segmenter-2.1.8/napari_allencell_segmenter.egg-info/requires.txt` & `napari-allencell-segmenter-2.1.9/napari_allencell_segmenter.egg-info/requires.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,25 @@
-napari
-napari-plugin-engine
+napari>=0.4.9
+napari-plugin-engine>=0.1.4
 numpy
-aicssegmentation>=0.5.2
+aicssegmentation>=0.5.0
 magicgui>=0.2.9
-aicsimageio~=4.0.9
-qtpy
-skimage
+aicsimageio~=4.0.5
 opencv-python-headless>=4.5.1
+importlib-metadata==4.11.4
 
 [all]
-napari
-napari-plugin-engine
+napari>=0.4.9
+napari-plugin-engine>=0.1.4
 numpy
-aicssegmentation>=0.5.2
+aicssegmentation>=0.5.0
 magicgui>=0.2.9
-aicsimageio~=4.0.9
-qtpy
-skimage
+aicsimageio~=4.0.5
 opencv-python-headless>=4.5.1
+importlib-metadata==4.11.4
 black>=19.10b0
 codecov>=2.0.22
 docutils<0.16,>=0.10
 flake8>=3.7.7
 psutil>=5.7.0
 pytest>=4.3.0
 pytest-cov==2.6.1
```

### Comparing `napari-allencell-segmenter-2.1.8/setup.cfg` & `napari-allencell-segmenter-2.1.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 2.1.8
+current_version = 2.1.9
 commit = True
 tag = True
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\-(?P<release>[a-z]+)(?P<build>\d+))?
 serialize = 
 	{major}.{minor}.{patch}-{release}{build}
 	{major}.{minor}.{patch}
```

### Comparing `napari-allencell-segmenter-2.1.8/setup.py` & `napari-allencell-segmenter-2.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,25 +10,25 @@
     file_path = os.path.join(os.path.dirname(__file__), fname)
     return codecs.open(file_path, encoding="utf-8").read()
 
 
 # Add your dependencies in requirements.txt
 # Note: you can add test-specific requirements in tox.ini
 requirements = [
-    "napari",
-    "napari-plugin-engine",
+    "napari>=0.4.9",
+    "napari-plugin-engine>=0.1.4",
     "numpy",
-    "aicssegmentation >= 0.5.2",
+    "aicssegmentation >= 0.5.0",
     "magicgui >= 0.2.9",
-    "aicsimageio ~= 4.0.9",
-    "qtpy",
-    "skimage",
+    "aicsimageio ~= 4.0.5",
     "opencv-python-headless>=4.5.1",
+    "importlib-metadata==4.11.4",
 ]
 
+
 test_requirements = [
     "black>=19.10b0",
     "codecov>=2.0.22",
     "docutils>=0.10,<0.16",
     "flake8>=3.7.7",
     "psutil>=5.7.0",
     "pytest>=4.3.0",
@@ -122,10 +122,10 @@
         "Bug Tracker": "https://github.com/AllenCell/napari-allencell-segmenter/issues",
         "Documentation": "https://github.com/AllenCell/napari-allencell-segmenter#README.md",
         "Source Code": "https://github.com/AllenCell/napari-allencell-segmenter",
         "User Support": "https://github.com/AllenCell/napari-allencell-segmenter/issues",
     },
     # Do not edit this string manually, always use bumpversion
     # Details in CONTRIBUTING.rst
-    version="2.1.8",
+    version="2.1.9",
     zip_safe=False,
 )
```

