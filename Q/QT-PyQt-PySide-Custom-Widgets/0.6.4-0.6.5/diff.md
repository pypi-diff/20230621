# Comparing `tmp/QT-PyQt-PySide-Custom-Widgets-0.6.4.tar.gz` & `tmp/QT-PyQt-PySide-Custom-Widgets-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QT-PyQt-PySide-Custom-Widgets-0.6.4.tar", last modified: Mon Jan  9 16:49:37 2023, max compression
+gzip compressed data, was "dist\QT-PyQt-PySide-Custom-Widgets-0.6.5.tar", last modified: Wed Jun 21 21:13:08 2023, max compression
```

## Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4.tar` & `QT-PyQt-PySide-Custom-Widgets-0.6.5.tar`

### file list

```diff
@@ -1,389 +1,389 @@
-drwxrwxrwx   0 spinn     (1000) spinn     (1001)        0 2023-01-09 16:49:37.604900 QT-PyQt-PySide-Custom-Widgets-0.6.4/
-drwxrwxrwx   0 spinn     (1000) spinn     (1001)        0 2023-01-09 16:49:37.081146 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)    66370 2023-01-07 14:59:52.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/AnalogGaugeWidget.py
-drwxrwxrwx   0 spinn     (1000) spinn     (1001)        0 2023-01-09 16:49:37.085507 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/ProgressIndicator/
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)        0 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/ProgressIndicator/__init__.py
-drwxrwxrwx   0 spinn     (1000) spinn     (1001)        0 2023-01-09 16:49:37.093453 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/ProgressIndicator/__pycache__/
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      185 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/ProgressIndicator/__pycache__/__init__.cpython-310.pyc
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      178 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/ProgressIndicator/__pycache__/__init__.cpython-38.pyc
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     3840 2023-01-08 10:24:42.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/ProgressIndicator/__pycache__/test.cpython-310.pyc
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     3794 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/ProgressIndicator/__pycache__/test.cpython-38.pyc
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     5285 2023-01-08 10:14:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/ProgressIndicator/__pycache__/ui_interface.cpython-310.pyc
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     5276 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/ProgressIndicator/__pycache__/ui_interface.cpython-38.pyc
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     5297 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/ProgressIndicator/__pycache__/ui_interface.cpython-39.pyc
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     8502 2023-01-08 10:13:43.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/ProgressIndicator/interface.ui
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     9452 2023-01-08 10:24:24.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/ProgressIndicator/test.py
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     9629 2023-01-08 10:13:49.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/ProgressIndicator/ui_interface.py
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)    14071 2023-01-07 14:56:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/ProjectMaker.py
-drwxrwxrwx   0 spinn     (1000) spinn     (1001)        0 2023-01-09 16:49:37.104405 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)    39288 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/QSS_Resources.qrc
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     5505 2023-01-07 15:08:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/SassCompiler.py
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)    14615 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/SvgToPngIcons.py
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)       39 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/__init__.py
-drwxrwxrwx   0 spinn     (1000) spinn     (1001)        0 2023-01-09 16:49:37.134668 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/__pycache__/
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)   630113 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/__pycache__/QSS_Resources.cpython-39.pyc
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     3122 2023-01-07 15:21:54.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/__pycache__/SassCompiler.cpython-310.pyc
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     3029 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/__pycache__/SassCompiler.cpython-38.pyc
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     6895 2023-01-07 13:20:07.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/__pycache__/SvgToPngIcons.cpython-310.pyc
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     6525 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/__pycache__/SvgToPngIcons.cpython-38.pyc
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     3158 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/__pycache__/SvgToPngIcons.cpython-39.pyc
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      192 2023-01-07 13:20:07.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/__pycache__/__init__.cpython-310.pyc
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      177 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/__pycache__/__init__.cpython-37.pyc
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      164 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/__pycache__/__init__.cpython-38.pyc
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      188 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/__pycache__/__init__.cpython-39.pyc
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     6166 2023-01-07 15:21:54.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/__pycache__/colorsystem.cpython-310.pyc
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     6168 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/__pycache__/colorsystem.cpython-37.pyc
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     6106 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/__pycache__/colorsystem.cpython-38.pyc
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     6064 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/__pycache__/colorsystem.cpython-39.pyc
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)   630112 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/__pycache__/resources_rc.cpython-39.pyc
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     2764 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/__pycache__/sassCompiler.cpython-39.pyc
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)    60079 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/_styles.scss
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)    10630 2023-01-07 15:11:36.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/colorsystem.py
-drwxrwxrwx   0 spinn     (1000) spinn     (1001)        0 2023-01-09 16:49:37.059942 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/
-drwxrwxrwx   0 spinn     (1000) spinn     (1001)        0 2023-01-09 16:49:37.580901 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      276 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/activity.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      356 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/airplay.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      350 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/alert-circle.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      410 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/alert-octagon.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      418 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/alert-triangle.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      392 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/align-center.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      393 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/align-justify.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      390 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/align-left.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      391 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/align-right.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      339 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/anchor.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      562 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/aperture.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      355 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/archive.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      354 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/arrow-down-circle.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      309 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/arrow-down-left.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      311 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/arrow-down-right.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      307 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/arrow-down.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      353 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/arrow-left-circle.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      306 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/arrow-left.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      355 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/arrow-right-circle.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      308 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/arrow-right.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      351 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/arrow-up-circle.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      306 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/arrow-up-left.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      308 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/arrow-up-right.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      304 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/arrow-up.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     3022 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/arrow_down.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     3023 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/arrow_left.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     3026 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/arrow_right.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     3021 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/arrow_up.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      316 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/at-sign.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      319 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/award.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      349 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/bar-chart-2.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      347 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/bar-chart.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     7594 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/base_icon.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)    33666 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/base_palette.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      421 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/battery-charging.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      320 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/battery.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      454 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/bell-off.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      315 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/bell.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      292 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/bluetooth.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      321 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/bold.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      333 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/book-open.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      339 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/book.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      281 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/bookmark.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      456 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/box.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     2755 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/branch_closed.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     2902 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/branch_end.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     3508 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/branch_line.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     2678 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/branch_more.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     2711 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/branch_open.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      337 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/briefcase.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      404 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/calendar.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      379 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/camera-off.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      350 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/camera.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      381 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/cast.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      322 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/check-circle.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      339 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/check-square.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      256 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/check.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     2799 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/checkbox_checked.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     2781 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/checkbox_indeterminate.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     2598 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/checkbox_unchecked.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      263 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/chevron-down.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      264 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/chevron-left.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      264 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/chevron-right.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      262 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/chevron-up.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      311 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/chevrons-down.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      312 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/chevrons-left.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      312 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/chevrons-right.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      310 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/chevrons-up.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      442 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/chrome.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      252 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/circle.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      365 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/clipboard.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      298 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/clock.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      551 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/cloud-drizzle.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      339 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/cloud-lightning.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      365 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/cloud-off.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      415 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/cloud-rain.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      566 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/cloud-snow.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      274 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/cloud.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      301 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/code.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      480 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/codepen.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      632 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/codesandbox.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      441 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/coffee.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      320 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/columns.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      415 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/command.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      336 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/compass.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      345 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/copy.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      308 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/corner-down-left.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      312 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/corner-down-right.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      311 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/corner-left-down.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      306 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/corner-left-up.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      312 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/corner-right-down.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      307 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/corner-right-up.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      306 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/corner-up-left.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      310 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/corner-up-right.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      661 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/cpu.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      323 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/credit-card.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      304 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/crop.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      431 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/crosshair.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      366 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/database.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      368 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/delete.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      289 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/disc.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      391 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/divide-circle.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      413 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/divide-square.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      333 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/divide.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      328 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/dollar-sign.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      381 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/download-cloud.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      364 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/download.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      418 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/dribbble.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      268 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/droplet.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      285 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/edit-2.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      311 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/edit-3.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      359 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/edit.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      382 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/external-link.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      454 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/eye-off.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      310 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/eye.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      297 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/facebook.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      317 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/fast-forward.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      367 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/feather.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      547 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/figma.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      381 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/file-minus.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      425 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/file-plus.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      467 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/file-text.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      331 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/file.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      580 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/film.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      284 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/filter.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      328 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/flag.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      355 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/folder-minus.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      399 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/folder-plus.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      305 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/folder.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      272 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/framer.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      384 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/frown.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      475 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/gift.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      371 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/git-branch.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      352 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/git-commit.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      330 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/git-merge.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      381 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/git-pull-request.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      521 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/github.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      484 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/gitlab.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      403 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/globe.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      398 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/grid.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      478 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/hard-drive.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      383 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/hash.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      389 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/headphones.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      365 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/heart.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      359 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/help-circle.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      352 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/hexagon.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      326 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/home.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      363 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/image.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      399 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/inbox.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      341 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/info.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      394 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/instagram.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      342 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/italic.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      346 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/key.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      359 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/layers.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      358 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/layout.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      569 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/life-buoy.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     2445 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/line_horizontal.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     2454 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/line_vertical.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      349 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/link-2.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      365 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/link.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      394 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/linkedin.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      476 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/list.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      608 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/loader.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      315 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/lock.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      362 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/log-in.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      361 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/log-out.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      348 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/mail.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      316 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/map-pin.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      367 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/map.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      394 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/maximize-2.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      325 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/maximize.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      383 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/meh.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      340 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/menu.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      422 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/message-circle.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      299 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/message-square.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      488 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/mic-off.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      412 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/mic.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      398 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/minimize-2.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      325 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/minimize.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      302 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/minus-circle.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      324 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/minus-square.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      255 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/minus.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      364 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/monitor.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      275 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/moon.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      337 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/more-horizontal.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      335 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/more-vertical.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      305 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/mouse-pointer.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      480 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/move.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      321 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/music.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      273 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/navigation-2.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      271 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/navigation.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      312 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/octagon.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      511 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/package.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      346 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/paperclip.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      346 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/pause-circle.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      306 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/pause.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      385 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/pen-tool.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      344 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/percent.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      570 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/phone-call.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      612 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/phone-forwarded.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      611 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/phone-incoming.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      607 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/phone-missed.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      585 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/phone-off.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      611 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/phone-outgoing.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      514 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/phone.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      309 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/pie-chart.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      307 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/play-circle.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      257 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/play.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      345 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/plus-circle.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      367 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/plus-square.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      298 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/plus.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      352 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/pocket.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      302 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/power.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      401 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/printer.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      383 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/radio.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     2714 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/radio_checked.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     2419 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/radio_unchecked.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      394 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/refresh-ccw.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      394 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/refresh-cw.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      386 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/repeat.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      313 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/rewind.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      311 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/rotate-ccw.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      315 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/rotate-cw.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      324 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/rss.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      386 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/save.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      438 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/scissors.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      302 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/search.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      308 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/send.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      425 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/server.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     1005 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/settings.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      439 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/share-2.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      358 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/share.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      399 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/shield-off.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      273 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/shield.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      366 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/shopping-bag.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      377 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/shopping-cart.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      435 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/shuffle.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      317 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/sidebar.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      307 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/skip-back.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      309 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/skip-forward.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      993 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/slack.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      306 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/slash.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      605 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/sliders.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      326 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/smartphone.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      382 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/smile.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      360 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/speaker.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      274 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/square.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      333 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/star.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      303 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/stop-circle.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      644 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/sun.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      583 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/sunrise.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      582 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/sunset.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      322 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/tablet.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      349 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/tag.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      330 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/target.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      304 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/terminal.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      291 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/thermometer.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      368 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/thumbs-down.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      348 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/thumbs-up.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      317 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/toggle-left.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      319 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/toggle-right.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      380 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/tool.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     2703 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/toolbar_move_horizontal.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     2710 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/toolbar_move_vertical.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     2464 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/toolbar_separator_horizontal.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     2463 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/toolbar_separator_vertical.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     2347 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/transparent.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      442 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/trash-2.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      350 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/trash.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      367 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/trello.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      325 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/trending-down.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      322 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/trending-up.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      320 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/triangle.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      409 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/truck.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      314 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/tv.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      271 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/twitch.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      402 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/twitter.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      346 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/type.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      284 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/umbrella.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      313 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/underline.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      316 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/unlock.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      425 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/upload-cloud.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      359 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/upload.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      361 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/user-check.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      359 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/user-minus.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      402 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/user-plus.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      398 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/user-x.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      307 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/user.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      394 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/users.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      373 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/video-off.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      323 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/video.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      352 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/voicemail.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      322 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/volume-1.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      353 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/volume-2.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      364 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/volume-x.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      274 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/volume.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      456 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/watch.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      563 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/wifi-off.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      395 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/wifi.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      320 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/wind.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     2953 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/window_close.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     3018 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/window_grip.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     2465 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/window_minimize.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     2979 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/window_undock.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      340 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/x-circle.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      400 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/x-octagon.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      362 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/x-square.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      293 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/x.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      559 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/youtube.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      427 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/zap-off.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      276 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/zap.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      391 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/zoom-in.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      348 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/zoom-out.svg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      134 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/main.scss
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)    30871 2023-01-07 14:55:55.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/RoundProgressBar.py
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)    40717 2023-01-07 13:43:08.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/SpiralProgressBar.py
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)   156605 2023-01-07 13:33:04.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Widgets.py
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     4824 2023-01-07 13:42:01.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/WidgetsWorker.py
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)       39 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/__init__.py
-drwxrwxrwx   0 spinn     (1000) spinn     (1001)        0 2023-01-09 16:49:37.062128 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/components/
-drwxrwxrwx   0 spinn     (1000) spinn     (1001)        0 2023-01-09 16:49:37.583903 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/components/json/
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      344 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/components/json/style.json
-drwxrwxrwx   0 spinn     (1000) spinn     (1001)        0 2023-01-09 16:49:37.587017 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/components/python/
-drwxrwxrwx   0 spinn     (1000) spinn     (1001)        0 2023-01-09 16:49:37.593898 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/components/python/__pycache__/
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      853 2023-01-07 13:20:07.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/components/python/__pycache__/main.cpython-310.pyc
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)      836 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/components/python/__pycache__/main.cpython-38.pyc
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     2561 2023-01-07 13:20:07.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/components/python/__pycache__/ui_interface.cpython-310.pyc
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     2552 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/components/python/__pycache__/ui_interface.cpython-38.pyc
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     2679 2023-01-07 15:20:25.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/components/python/main.py
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     3127 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/components/python/ui_interface.py
-drwxrwxrwx   0 spinn     (1000) spinn     (1001)        0 2023-01-09 16:49:37.595503 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/components/uis/
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     2691 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/components/uis/interface.ui
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     1242 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/interface.ui
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     2368 2023-01-07 13:20:06.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/main.py
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)    35149 2021-06-11 19:06:36.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/LICENSE
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)       82 2022-02-17 19:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/MANIFEST.in
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     4030 2023-01-09 16:49:37.604336 QT-PyQt-PySide-Custom-Widgets-0.6.4/PKG-INFO
-drwxrwxrwx   0 spinn     (1000) spinn     (1001)        0 2023-01-09 16:49:37.602424 QT-PyQt-PySide-Custom-Widgets-0.6.4/QT_PyQt_PySide_Custom_Widgets.egg-info/
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     4030 2023-01-09 16:49:36.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/QT_PyQt_PySide_Custom_Widgets.egg-info/PKG-INFO
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)    19073 2023-01-09 16:49:36.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/QT_PyQt_PySide_Custom_Widgets.egg-info/SOURCES.txt
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)        1 2023-01-09 16:49:36.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/QT_PyQt_PySide_Custom_Widgets.egg-info/dependency_links.txt
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)       45 2023-01-09 16:49:36.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/QT_PyQt_PySide_Custom_Widgets.egg-info/requires.txt
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)       15 2023-01-09 16:49:36.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/QT_PyQt_PySide_Custom_Widgets.egg-info/top_level.txt
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     3169 2022-08-11 03:08:01.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/README.md
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)       38 2023-01-09 16:49:37.605116 QT-PyQt-PySide-Custom-Widgets-0.6.4/setup.cfg
--rwxrwxrwx   0 spinn     (1000) spinn     (1001)     2253 2023-01-09 16:35:45.000000 QT-PyQt-PySide-Custom-Widgets-0.6.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 21:13:08.168026 QT-PyQt-PySide-Custom-Widgets-0.6.5/
+drwxrwxrwx   0        0        0        0 2023-06-21 21:13:06.819338 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/
+-rw-rw-rw-   0        0        0    66370 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/AnalogGaugeWidget.py
+drwxrwxrwx   0        0        0        0 2023-06-21 21:13:06.828332 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/ProgressIndicator/
+-rw-rw-rw-   0        0        0        0 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/ProgressIndicator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 21:13:06.881634 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/ProgressIndicator/__pycache__/
+-rw-rw-rw-   0        0        0      185 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/ProgressIndicator/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      178 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/ProgressIndicator/__pycache__/__init__.cpython-38.pyc
+-rw-rw-rw-   0        0        0     3840 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/ProgressIndicator/__pycache__/test.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3948 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/ProgressIndicator/__pycache__/test.cpython-38.pyc
+-rw-rw-rw-   0        0        0     5285 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/ProgressIndicator/__pycache__/ui_interface.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5276 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/ProgressIndicator/__pycache__/ui_interface.cpython-38.pyc
+-rw-rw-rw-   0        0        0     5297 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/ProgressIndicator/__pycache__/ui_interface.cpython-39.pyc
+-rw-rw-rw-   0        0        0     8502 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/ProgressIndicator/interface.ui
+-rw-rw-rw-   0        0        0     9452 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/ProgressIndicator/test.py
+-rw-rw-rw-   0        0        0     9629 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/ProgressIndicator/ui_interface.py
+-rw-rw-rw-   0        0        0    14071 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/ProjectMaker.py
+drwxrwxrwx   0        0        0        0 2023-06-21 21:13:06.949614 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/
+-rw-rw-rw-   0        0        0    39288 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/QSS_Resources.qrc
+-rw-rw-rw-   0        0        0     5505 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/SassCompiler.py
+-rw-rw-rw-   0        0        0    14615 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/SvgToPngIcons.py
+-rw-rw-rw-   0        0        0       39 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 21:13:07.072648 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/
+-rw-rw-rw-   0        0        0   630113 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/QSS_Resources.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3122 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/SassCompiler.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3089 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/SassCompiler.cpython-38.pyc
+-rw-rw-rw-   0        0        0     6895 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/SvgToPngIcons.cpython-310.pyc
+-rw-rw-rw-   0        0        0     6680 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/SvgToPngIcons.cpython-38.pyc
+-rw-rw-rw-   0        0        0     3158 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/SvgToPngIcons.cpython-39.pyc
+-rw-rw-rw-   0        0        0      192 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      177 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0      185 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/__init__.cpython-38.pyc
+-rw-rw-rw-   0        0        0      188 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     6166 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/colorsystem.cpython-310.pyc
+-rw-rw-rw-   0        0        0     6168 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/colorsystem.cpython-37.pyc
+-rw-rw-rw-   0        0        0     6481 2023-06-21 21:05:22.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/colorsystem.cpython-38.pyc
+-rw-rw-rw-   0        0        0     6064 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/colorsystem.cpython-39.pyc
+-rw-rw-rw-   0        0        0   630112 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/resources_rc.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2764 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/sassCompiler.cpython-39.pyc
+-rw-rw-rw-   0        0        0    60079 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/_styles.scss
+-rw-rw-rw-   0        0        0    10048 2023-06-21 21:05:04.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/colorsystem.py
+drwxrwxrwx   0        0        0        0 2023-06-21 21:13:06.736609 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/
+drwxrwxrwx   0        0        0        0 2023-06-21 21:13:07.997122 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/
+-rw-rw-rw-   0        0        0      276 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/activity.svg
+-rw-rw-rw-   0        0        0      356 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/airplay.svg
+-rw-rw-rw-   0        0        0      350 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/alert-circle.svg
+-rw-rw-rw-   0        0        0      410 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/alert-octagon.svg
+-rw-rw-rw-   0        0        0      418 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/alert-triangle.svg
+-rw-rw-rw-   0        0        0      392 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/align-center.svg
+-rw-rw-rw-   0        0        0      393 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/align-justify.svg
+-rw-rw-rw-   0        0        0      390 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/align-left.svg
+-rw-rw-rw-   0        0        0      391 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/align-right.svg
+-rw-rw-rw-   0        0        0      339 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/anchor.svg
+-rw-rw-rw-   0        0        0      562 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/aperture.svg
+-rw-rw-rw-   0        0        0      355 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/archive.svg
+-rw-rw-rw-   0        0        0      354 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/arrow-down-circle.svg
+-rw-rw-rw-   0        0        0      309 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/arrow-down-left.svg
+-rw-rw-rw-   0        0        0      311 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/arrow-down-right.svg
+-rw-rw-rw-   0        0        0      307 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/arrow-down.svg
+-rw-rw-rw-   0        0        0      353 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/arrow-left-circle.svg
+-rw-rw-rw-   0        0        0      306 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/arrow-left.svg
+-rw-rw-rw-   0        0        0      355 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/arrow-right-circle.svg
+-rw-rw-rw-   0        0        0      308 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/arrow-right.svg
+-rw-rw-rw-   0        0        0      351 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/arrow-up-circle.svg
+-rw-rw-rw-   0        0        0      306 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/arrow-up-left.svg
+-rw-rw-rw-   0        0        0      308 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/arrow-up-right.svg
+-rw-rw-rw-   0        0        0      304 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/arrow-up.svg
+-rw-rw-rw-   0        0        0     3022 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/arrow_down.svg
+-rw-rw-rw-   0        0        0     3023 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/arrow_left.svg
+-rw-rw-rw-   0        0        0     3026 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/arrow_right.svg
+-rw-rw-rw-   0        0        0     3021 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/arrow_up.svg
+-rw-rw-rw-   0        0        0      316 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/at-sign.svg
+-rw-rw-rw-   0        0        0      319 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/award.svg
+-rw-rw-rw-   0        0        0      349 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/bar-chart-2.svg
+-rw-rw-rw-   0        0        0      347 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/bar-chart.svg
+-rw-rw-rw-   0        0        0     7594 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/base_icon.svg
+-rw-rw-rw-   0        0        0    33666 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/base_palette.svg
+-rw-rw-rw-   0        0        0      421 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/battery-charging.svg
+-rw-rw-rw-   0        0        0      320 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/battery.svg
+-rw-rw-rw-   0        0        0      454 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/bell-off.svg
+-rw-rw-rw-   0        0        0      315 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/bell.svg
+-rw-rw-rw-   0        0        0      292 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/bluetooth.svg
+-rw-rw-rw-   0        0        0      321 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/bold.svg
+-rw-rw-rw-   0        0        0      333 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/book-open.svg
+-rw-rw-rw-   0        0        0      339 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/book.svg
+-rw-rw-rw-   0        0        0      281 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/bookmark.svg
+-rw-rw-rw-   0        0        0      456 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/box.svg
+-rw-rw-rw-   0        0        0     2755 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/branch_closed.svg
+-rw-rw-rw-   0        0        0     2902 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/branch_end.svg
+-rw-rw-rw-   0        0        0     3508 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/branch_line.svg
+-rw-rw-rw-   0        0        0     2678 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/branch_more.svg
+-rw-rw-rw-   0        0        0     2711 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/branch_open.svg
+-rw-rw-rw-   0        0        0      337 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/briefcase.svg
+-rw-rw-rw-   0        0        0      404 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/calendar.svg
+-rw-rw-rw-   0        0        0      379 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/camera-off.svg
+-rw-rw-rw-   0        0        0      350 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/camera.svg
+-rw-rw-rw-   0        0        0      381 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/cast.svg
+-rw-rw-rw-   0        0        0      322 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/check-circle.svg
+-rw-rw-rw-   0        0        0      339 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/check-square.svg
+-rw-rw-rw-   0        0        0      256 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/check.svg
+-rw-rw-rw-   0        0        0     2799 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/checkbox_checked.svg
+-rw-rw-rw-   0        0        0     2781 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/checkbox_indeterminate.svg
+-rw-rw-rw-   0        0        0     2598 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/checkbox_unchecked.svg
+-rw-rw-rw-   0        0        0      263 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/chevron-down.svg
+-rw-rw-rw-   0        0        0      264 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/chevron-left.svg
+-rw-rw-rw-   0        0        0      264 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/chevron-right.svg
+-rw-rw-rw-   0        0        0      262 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/chevron-up.svg
+-rw-rw-rw-   0        0        0      311 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/chevrons-down.svg
+-rw-rw-rw-   0        0        0      312 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/chevrons-left.svg
+-rw-rw-rw-   0        0        0      312 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/chevrons-right.svg
+-rw-rw-rw-   0        0        0      310 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/chevrons-up.svg
+-rw-rw-rw-   0        0        0      442 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/chrome.svg
+-rw-rw-rw-   0        0        0      252 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/circle.svg
+-rw-rw-rw-   0        0        0      365 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/clipboard.svg
+-rw-rw-rw-   0        0        0      298 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/clock.svg
+-rw-rw-rw-   0        0        0      551 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/cloud-drizzle.svg
+-rw-rw-rw-   0        0        0      339 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/cloud-lightning.svg
+-rw-rw-rw-   0        0        0      365 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/cloud-off.svg
+-rw-rw-rw-   0        0        0      415 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/cloud-rain.svg
+-rw-rw-rw-   0        0        0      566 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/cloud-snow.svg
+-rw-rw-rw-   0        0        0      274 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/cloud.svg
+-rw-rw-rw-   0        0        0      301 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/code.svg
+-rw-rw-rw-   0        0        0      480 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/codepen.svg
+-rw-rw-rw-   0        0        0      632 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/codesandbox.svg
+-rw-rw-rw-   0        0        0      441 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/coffee.svg
+-rw-rw-rw-   0        0        0      320 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/columns.svg
+-rw-rw-rw-   0        0        0      415 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/command.svg
+-rw-rw-rw-   0        0        0      336 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/compass.svg
+-rw-rw-rw-   0        0        0      345 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/copy.svg
+-rw-rw-rw-   0        0        0      308 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/corner-down-left.svg
+-rw-rw-rw-   0        0        0      312 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/corner-down-right.svg
+-rw-rw-rw-   0        0        0      311 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/corner-left-down.svg
+-rw-rw-rw-   0        0        0      306 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/corner-left-up.svg
+-rw-rw-rw-   0        0        0      312 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/corner-right-down.svg
+-rw-rw-rw-   0        0        0      307 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/corner-right-up.svg
+-rw-rw-rw-   0        0        0      306 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/corner-up-left.svg
+-rw-rw-rw-   0        0        0      310 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/corner-up-right.svg
+-rw-rw-rw-   0        0        0      661 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/cpu.svg
+-rw-rw-rw-   0        0        0      323 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/credit-card.svg
+-rw-rw-rw-   0        0        0      304 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/crop.svg
+-rw-rw-rw-   0        0        0      431 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/crosshair.svg
+-rw-rw-rw-   0        0        0      366 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/database.svg
+-rw-rw-rw-   0        0        0      368 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/delete.svg
+-rw-rw-rw-   0        0        0      289 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/disc.svg
+-rw-rw-rw-   0        0        0      391 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/divide-circle.svg
+-rw-rw-rw-   0        0        0      413 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/divide-square.svg
+-rw-rw-rw-   0        0        0      333 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/divide.svg
+-rw-rw-rw-   0        0        0      328 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/dollar-sign.svg
+-rw-rw-rw-   0        0        0      381 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/download-cloud.svg
+-rw-rw-rw-   0        0        0      364 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/download.svg
+-rw-rw-rw-   0        0        0      418 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/dribbble.svg
+-rw-rw-rw-   0        0        0      268 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/droplet.svg
+-rw-rw-rw-   0        0        0      285 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/edit-2.svg
+-rw-rw-rw-   0        0        0      311 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/edit-3.svg
+-rw-rw-rw-   0        0        0      359 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/edit.svg
+-rw-rw-rw-   0        0        0      382 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/external-link.svg
+-rw-rw-rw-   0        0        0      454 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/eye-off.svg
+-rw-rw-rw-   0        0        0      310 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/eye.svg
+-rw-rw-rw-   0        0        0      297 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/facebook.svg
+-rw-rw-rw-   0        0        0      317 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/fast-forward.svg
+-rw-rw-rw-   0        0        0      367 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/feather.svg
+-rw-rw-rw-   0        0        0      547 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/figma.svg
+-rw-rw-rw-   0        0        0      381 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/file-minus.svg
+-rw-rw-rw-   0        0        0      425 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/file-plus.svg
+-rw-rw-rw-   0        0        0      467 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/file-text.svg
+-rw-rw-rw-   0        0        0      331 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/file.svg
+-rw-rw-rw-   0        0        0      580 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/film.svg
+-rw-rw-rw-   0        0        0      284 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/filter.svg
+-rw-rw-rw-   0        0        0      328 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/flag.svg
+-rw-rw-rw-   0        0        0      355 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/folder-minus.svg
+-rw-rw-rw-   0        0        0      399 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/folder-plus.svg
+-rw-rw-rw-   0        0        0      305 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/folder.svg
+-rw-rw-rw-   0        0        0      272 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/framer.svg
+-rw-rw-rw-   0        0        0      384 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/frown.svg
+-rw-rw-rw-   0        0        0      475 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/gift.svg
+-rw-rw-rw-   0        0        0      371 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/git-branch.svg
+-rw-rw-rw-   0        0        0      352 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/git-commit.svg
+-rw-rw-rw-   0        0        0      330 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/git-merge.svg
+-rw-rw-rw-   0        0        0      381 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/git-pull-request.svg
+-rw-rw-rw-   0        0        0      521 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/github.svg
+-rw-rw-rw-   0        0        0      484 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/gitlab.svg
+-rw-rw-rw-   0        0        0      403 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/globe.svg
+-rw-rw-rw-   0        0        0      398 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/grid.svg
+-rw-rw-rw-   0        0        0      478 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/hard-drive.svg
+-rw-rw-rw-   0        0        0      383 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/hash.svg
+-rw-rw-rw-   0        0        0      389 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/headphones.svg
+-rw-rw-rw-   0        0        0      365 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/heart.svg
+-rw-rw-rw-   0        0        0      359 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/help-circle.svg
+-rw-rw-rw-   0        0        0      352 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/hexagon.svg
+-rw-rw-rw-   0        0        0      326 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/home.svg
+-rw-rw-rw-   0        0        0      363 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/image.svg
+-rw-rw-rw-   0        0        0      399 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/inbox.svg
+-rw-rw-rw-   0        0        0      341 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/info.svg
+-rw-rw-rw-   0        0        0      394 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/instagram.svg
+-rw-rw-rw-   0        0        0      342 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/italic.svg
+-rw-rw-rw-   0        0        0      346 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/key.svg
+-rw-rw-rw-   0        0        0      359 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/layers.svg
+-rw-rw-rw-   0        0        0      358 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/layout.svg
+-rw-rw-rw-   0        0        0      569 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/life-buoy.svg
+-rw-rw-rw-   0        0        0     2445 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/line_horizontal.svg
+-rw-rw-rw-   0        0        0     2454 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/line_vertical.svg
+-rw-rw-rw-   0        0        0      349 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/link-2.svg
+-rw-rw-rw-   0        0        0      365 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/link.svg
+-rw-rw-rw-   0        0        0      394 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/linkedin.svg
+-rw-rw-rw-   0        0        0      476 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/list.svg
+-rw-rw-rw-   0        0        0      608 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/loader.svg
+-rw-rw-rw-   0        0        0      315 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/lock.svg
+-rw-rw-rw-   0        0        0      362 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/log-in.svg
+-rw-rw-rw-   0        0        0      361 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/log-out.svg
+-rw-rw-rw-   0        0        0      348 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/mail.svg
+-rw-rw-rw-   0        0        0      316 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/map-pin.svg
+-rw-rw-rw-   0        0        0      367 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/map.svg
+-rw-rw-rw-   0        0        0      394 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/maximize-2.svg
+-rw-rw-rw-   0        0        0      325 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/maximize.svg
+-rw-rw-rw-   0        0        0      383 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/meh.svg
+-rw-rw-rw-   0        0        0      340 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/menu.svg
+-rw-rw-rw-   0        0        0      422 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/message-circle.svg
+-rw-rw-rw-   0        0        0      299 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/message-square.svg
+-rw-rw-rw-   0        0        0      488 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/mic-off.svg
+-rw-rw-rw-   0        0        0      412 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/mic.svg
+-rw-rw-rw-   0        0        0      398 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/minimize-2.svg
+-rw-rw-rw-   0        0        0      325 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/minimize.svg
+-rw-rw-rw-   0        0        0      302 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/minus-circle.svg
+-rw-rw-rw-   0        0        0      324 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/minus-square.svg
+-rw-rw-rw-   0        0        0      255 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/minus.svg
+-rw-rw-rw-   0        0        0      364 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/monitor.svg
+-rw-rw-rw-   0        0        0      275 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/moon.svg
+-rw-rw-rw-   0        0        0      337 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/more-horizontal.svg
+-rw-rw-rw-   0        0        0      335 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/more-vertical.svg
+-rw-rw-rw-   0        0        0      305 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/mouse-pointer.svg
+-rw-rw-rw-   0        0        0      480 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/move.svg
+-rw-rw-rw-   0        0        0      321 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/music.svg
+-rw-rw-rw-   0        0        0      273 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/navigation-2.svg
+-rw-rw-rw-   0        0        0      271 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/navigation.svg
+-rw-rw-rw-   0        0        0      312 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/octagon.svg
+-rw-rw-rw-   0        0        0      511 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/package.svg
+-rw-rw-rw-   0        0        0      346 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/paperclip.svg
+-rw-rw-rw-   0        0        0      346 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/pause-circle.svg
+-rw-rw-rw-   0        0        0      306 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/pause.svg
+-rw-rw-rw-   0        0        0      385 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/pen-tool.svg
+-rw-rw-rw-   0        0        0      344 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/percent.svg
+-rw-rw-rw-   0        0        0      570 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/phone-call.svg
+-rw-rw-rw-   0        0        0      612 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/phone-forwarded.svg
+-rw-rw-rw-   0        0        0      611 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/phone-incoming.svg
+-rw-rw-rw-   0        0        0      607 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/phone-missed.svg
+-rw-rw-rw-   0        0        0      585 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/phone-off.svg
+-rw-rw-rw-   0        0        0      611 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/phone-outgoing.svg
+-rw-rw-rw-   0        0        0      514 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/phone.svg
+-rw-rw-rw-   0        0        0      309 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/pie-chart.svg
+-rw-rw-rw-   0        0        0      307 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/play-circle.svg
+-rw-rw-rw-   0        0        0      257 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/play.svg
+-rw-rw-rw-   0        0        0      345 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/plus-circle.svg
+-rw-rw-rw-   0        0        0      367 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/plus-square.svg
+-rw-rw-rw-   0        0        0      298 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/plus.svg
+-rw-rw-rw-   0        0        0      352 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/pocket.svg
+-rw-rw-rw-   0        0        0      302 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/power.svg
+-rw-rw-rw-   0        0        0      401 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/printer.svg
+-rw-rw-rw-   0        0        0      383 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/radio.svg
+-rw-rw-rw-   0        0        0     2714 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/radio_checked.svg
+-rw-rw-rw-   0        0        0     2419 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/radio_unchecked.svg
+-rw-rw-rw-   0        0        0      394 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/refresh-ccw.svg
+-rw-rw-rw-   0        0        0      394 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/refresh-cw.svg
+-rw-rw-rw-   0        0        0      386 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/repeat.svg
+-rw-rw-rw-   0        0        0      313 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/rewind.svg
+-rw-rw-rw-   0        0        0      311 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/rotate-ccw.svg
+-rw-rw-rw-   0        0        0      315 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/rotate-cw.svg
+-rw-rw-rw-   0        0        0      324 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/rss.svg
+-rw-rw-rw-   0        0        0      386 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/save.svg
+-rw-rw-rw-   0        0        0      438 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/scissors.svg
+-rw-rw-rw-   0        0        0      302 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/search.svg
+-rw-rw-rw-   0        0        0      308 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/send.svg
+-rw-rw-rw-   0        0        0      425 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/server.svg
+-rw-rw-rw-   0        0        0     1005 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/settings.svg
+-rw-rw-rw-   0        0        0      439 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/share-2.svg
+-rw-rw-rw-   0        0        0      358 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/share.svg
+-rw-rw-rw-   0        0        0      399 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/shield-off.svg
+-rw-rw-rw-   0        0        0      273 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/shield.svg
+-rw-rw-rw-   0        0        0      366 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/shopping-bag.svg
+-rw-rw-rw-   0        0        0      377 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/shopping-cart.svg
+-rw-rw-rw-   0        0        0      435 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/shuffle.svg
+-rw-rw-rw-   0        0        0      317 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/sidebar.svg
+-rw-rw-rw-   0        0        0      307 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/skip-back.svg
+-rw-rw-rw-   0        0        0      309 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/skip-forward.svg
+-rw-rw-rw-   0        0        0      993 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/slack.svg
+-rw-rw-rw-   0        0        0      306 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/slash.svg
+-rw-rw-rw-   0        0        0      605 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/sliders.svg
+-rw-rw-rw-   0        0        0      326 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/smartphone.svg
+-rw-rw-rw-   0        0        0      382 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/smile.svg
+-rw-rw-rw-   0        0        0      360 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/speaker.svg
+-rw-rw-rw-   0        0        0      274 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/square.svg
+-rw-rw-rw-   0        0        0      333 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/star.svg
+-rw-rw-rw-   0        0        0      303 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/stop-circle.svg
+-rw-rw-rw-   0        0        0      644 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/sun.svg
+-rw-rw-rw-   0        0        0      583 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/sunrise.svg
+-rw-rw-rw-   0        0        0      582 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/sunset.svg
+-rw-rw-rw-   0        0        0      322 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/tablet.svg
+-rw-rw-rw-   0        0        0      349 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/tag.svg
+-rw-rw-rw-   0        0        0      330 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/target.svg
+-rw-rw-rw-   0        0        0      304 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/terminal.svg
+-rw-rw-rw-   0        0        0      291 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/thermometer.svg
+-rw-rw-rw-   0        0        0      368 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/thumbs-down.svg
+-rw-rw-rw-   0        0        0      348 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/thumbs-up.svg
+-rw-rw-rw-   0        0        0      317 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/toggle-left.svg
+-rw-rw-rw-   0        0        0      319 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/toggle-right.svg
+-rw-rw-rw-   0        0        0      380 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/tool.svg
+-rw-rw-rw-   0        0        0     2703 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/toolbar_move_horizontal.svg
+-rw-rw-rw-   0        0        0     2710 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/toolbar_move_vertical.svg
+-rw-rw-rw-   0        0        0     2464 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/toolbar_separator_horizontal.svg
+-rw-rw-rw-   0        0        0     2463 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/toolbar_separator_vertical.svg
+-rw-rw-rw-   0        0        0     2347 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/transparent.svg
+-rw-rw-rw-   0        0        0      442 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/trash-2.svg
+-rw-rw-rw-   0        0        0      350 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/trash.svg
+-rw-rw-rw-   0        0        0      367 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/trello.svg
+-rw-rw-rw-   0        0        0      325 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/trending-down.svg
+-rw-rw-rw-   0        0        0      322 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/trending-up.svg
+-rw-rw-rw-   0        0        0      320 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/triangle.svg
+-rw-rw-rw-   0        0        0      409 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/truck.svg
+-rw-rw-rw-   0        0        0      314 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/tv.svg
+-rw-rw-rw-   0        0        0      271 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/twitch.svg
+-rw-rw-rw-   0        0        0      402 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/twitter.svg
+-rw-rw-rw-   0        0        0      346 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/type.svg
+-rw-rw-rw-   0        0        0      284 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/umbrella.svg
+-rw-rw-rw-   0        0        0      313 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/underline.svg
+-rw-rw-rw-   0        0        0      316 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/unlock.svg
+-rw-rw-rw-   0        0        0      425 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/upload-cloud.svg
+-rw-rw-rw-   0        0        0      359 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/upload.svg
+-rw-rw-rw-   0        0        0      361 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/user-check.svg
+-rw-rw-rw-   0        0        0      359 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/user-minus.svg
+-rw-rw-rw-   0        0        0      402 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/user-plus.svg
+-rw-rw-rw-   0        0        0      398 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/user-x.svg
+-rw-rw-rw-   0        0        0      307 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/user.svg
+-rw-rw-rw-   0        0        0      394 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/users.svg
+-rw-rw-rw-   0        0        0      373 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/video-off.svg
+-rw-rw-rw-   0        0        0      323 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/video.svg
+-rw-rw-rw-   0        0        0      352 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/voicemail.svg
+-rw-rw-rw-   0        0        0      322 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/volume-1.svg
+-rw-rw-rw-   0        0        0      353 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/volume-2.svg
+-rw-rw-rw-   0        0        0      364 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/volume-x.svg
+-rw-rw-rw-   0        0        0      274 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/volume.svg
+-rw-rw-rw-   0        0        0      456 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/watch.svg
+-rw-rw-rw-   0        0        0      563 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/wifi-off.svg
+-rw-rw-rw-   0        0        0      395 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/wifi.svg
+-rw-rw-rw-   0        0        0      320 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/wind.svg
+-rw-rw-rw-   0        0        0     2953 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/window_close.svg
+-rw-rw-rw-   0        0        0     3018 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/window_grip.svg
+-rw-rw-rw-   0        0        0     2465 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/window_minimize.svg
+-rw-rw-rw-   0        0        0     2979 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/window_undock.svg
+-rw-rw-rw-   0        0        0      340 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/x-circle.svg
+-rw-rw-rw-   0        0        0      400 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/x-octagon.svg
+-rw-rw-rw-   0        0        0      362 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/x-square.svg
+-rw-rw-rw-   0        0        0      293 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/x.svg
+-rw-rw-rw-   0        0        0      559 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/youtube.svg
+-rw-rw-rw-   0        0        0      427 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/zap-off.svg
+-rw-rw-rw-   0        0        0      276 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/zap.svg
+-rw-rw-rw-   0        0        0      391 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/zoom-in.svg
+-rw-rw-rw-   0        0        0      348 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/zoom-out.svg
+-rw-rw-rw-   0        0        0      134 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/main.scss
+-rw-rw-rw-   0        0        0    30871 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/RoundProgressBar.py
+-rw-rw-rw-   0        0        0    40717 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/SpiralProgressBar.py
+-rw-rw-rw-   0        0        0   156605 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Widgets.py
+-rw-rw-rw-   0        0        0     4824 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/WidgetsWorker.py
+-rw-rw-rw-   0        0        0       39 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 21:13:06.739545 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/components/
+drwxrwxrwx   0        0        0        0 2023-06-21 21:13:08.003119 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/components/json/
+-rw-rw-rw-   0        0        0      344 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/components/json/style.json
+drwxrwxrwx   0        0        0        0 2023-06-21 21:13:08.025113 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/components/python/
+drwxrwxrwx   0        0        0        0 2023-06-21 21:13:08.062085 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/components/python/__pycache__/
+-rw-rw-rw-   0        0        0      853 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/components/python/__pycache__/main.cpython-310.pyc
+-rw-rw-rw-   0        0        0      836 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/components/python/__pycache__/main.cpython-38.pyc
+-rw-rw-rw-   0        0        0     2561 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/components/python/__pycache__/ui_interface.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2552 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/components/python/__pycache__/ui_interface.cpython-38.pyc
+-rw-rw-rw-   0        0        0     2679 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/components/python/main.py
+-rw-rw-rw-   0        0        0     3127 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/components/python/ui_interface.py
+drwxrwxrwx   0        0        0        0 2023-06-21 21:13:08.067082 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/components/uis/
+-rw-rw-rw-   0        0        0     2691 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/components/uis/interface.ui
+-rw-rw-rw-   0        0        0     1242 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/interface.ui
+-rw-rw-rw-   0        0        0     2368 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/main.py
+-rw-rw-rw-   0        0        0    35149 2021-06-11 19:06:36.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/LICENSE
+-rw-rw-rw-   0        0        0       82 2022-02-17 19:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     4158 2023-06-21 21:13:08.167031 QT-PyQt-PySide-Custom-Widgets-0.6.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-21 21:13:08.163028 QT-PyQt-PySide-Custom-Widgets-0.6.5/QT_PyQt_PySide_Custom_Widgets.egg-info/
+-rw-rw-rw-   0        0        0     4158 2023-06-21 21:13:03.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/QT_PyQt_PySide_Custom_Widgets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    19073 2023-06-21 21:13:04.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/QT_PyQt_PySide_Custom_Widgets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 21:13:03.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/QT_PyQt_PySide_Custom_Widgets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-06-21 21:13:03.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/QT_PyQt_PySide_Custom_Widgets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-21 21:13:03.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/QT_PyQt_PySide_Custom_Widgets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3169 2022-08-11 03:08:01.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-21 21:13:08.169023 QT-PyQt-PySide-Custom-Widgets-0.6.5/setup.cfg
+-rw-rw-rw-   0        0        0     2253 2023-06-21 21:09:53.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/setup.py
```

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/AnalogGaugeWidget.py` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/AnalogGaugeWidget.py`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/ProgressIndicator/__pycache__/test.cpython-310.pyc` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/ProgressIndicator/__pycache__/test.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/ProgressIndicator/__pycache__/test.cpython-38.pyc` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/ProgressIndicator/__pycache__/test.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Mar  4 16:18:45 2022 UTC, .py size: 9242 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,238 +1,247 @@
-00000000: 550d 0d0a 0000 0000 e53b 2262 1a24 0000  U........;"b.$..
+00000000: 550d 0d0a 0000 0000 6a61 9364 ec24 0000  U.......ja.d.$..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 5000 0000 6400  .....@...sP...d.
-00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
-00000040: 0100 6400 6403 6c03 5400 6400 6401 6c04  ..d.d.l.T.d.d.l.
-00000050: 5a04 6400 6403 6c05 5400 6400 6403 6c06  Z.d.d.l.T.d.d.l.
-00000060: 5400 4700 6404 6405 8400 6405 6507 8303  T.G.d.d...d.e...
-00000070: 5a08 6406 6407 8400 5a09 6401 5300 2908  Z.d.d...Z.d.S.).
-00000080: e900 0000 004e 2901 da06 5174 436f 7265  .....N)...QtCore
-00000090: 2901 da01 2a63 0000 0000 0000 0000 0000  )...*c..........
-000000a0: 0000 0000 0000 0300 0000 4000 0000 731e  ..........@...s.
-000000b0: 0000 0065 005a 0164 005a 0264 0664 0264  ...e.Z.d.Z.d.d.d
-000000c0: 0384 015a 0364 0464 0584 005a 0464 0153  ...Z.d.d...Z.d.S
-000000d0: 0029 07da 0a4d 6169 6e57 696e 646f 774e  .)...MainWindowN
-000000e0: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-000000f0: 0006 0000 0003 0000 0073 ea01 0000 7400  .........s....t.
-00000100: a001 8800 a101 0100 7402 8300 8800 5f03  ........t....._.
-00000110: 8800 6a03 a004 8800 a101 0100 8800 6a03  ..j...........j.
-00000120: 6a05 6a06 6401 6402 6403 6404 8d03 0100  j.j.d.d.d.d.....
-00000130: 8800 6a03 6a07 6a06 6405 6406 6402 6407  ..j.j.j.d.d.d.d.
-00000140: 8d03 0100 8800 6a03 6a05 a008 6408 a101  ......j.j...d...
-00000150: 0100 8800 6a03 6a07 a008 6409 a101 0100  ....j.j...d.....
-00000160: 8800 6a03 6a07 a009 640a a101 0100 8800  ..j.j...d.......
-00000170: 6a03 6a0a 6a06 6405 6406 6402 6403 640b  j.j.j.d.d.d.d.d.
-00000180: 8d04 0100 8800 6a03 6a0a a008 640c a101  ......j.j...d...
-00000190: 0100 8800 6a03 6a0a a009 640a a101 0100  ....j.j...d.....
-000001a0: 8800 6a03 6a0b 6a0c a00d 8700 6601 640d  ..j.j.j.....f.d.
-000001b0: 640e 8408 a101 0100 8800 6a03 6a0e 6a0c  d.........j.j.j.
-000001c0: a00d 8700 6601 640f 640e 8408 a101 0100  ....f.d.d.......
-000001d0: 8800 6a03 6a0f 6a0c a00d 8700 6601 6410  ..j.j.j.....f.d.
-000001e0: 640e 8408 a101 0100 8800 6a03 6a10 6a0c  d.........j.j.j.
-000001f0: a00d 8700 6601 6411 640e 8408 a101 0100  ....f.d.d.......
-00000200: 8800 6a03 6a11 6a0c a00d 8700 6601 6412  ..j.j.j.....f.d.
-00000210: 640e 8408 a101 0100 8800 6a03 6a07 6a12  d.........j.j.j.
-00000220: 6413 6413 6413 6414 8d03 0100 8800 6a03  d.d.d.d.......j.
-00000230: 6a05 6a12 6413 6413 6413 6415 8d03 0100  j.j.d.d.d.d.....
-00000240: 8800 6a03 6a13 6a0c a00d 8700 6601 6416  ..j.j.j.....f.d.
-00000250: 640e 8408 a101 0100 8800 6a03 6a14 6a0c  d.........j.j.j.
-00000260: a00d 8700 6601 6417 640e 8408 a101 0100  ....f.d.d.......
-00000270: 8800 6a03 6a15 6a0c a00d 8700 6601 6418  ..j.j.j.....f.d.
-00000280: 640e 8408 a101 0100 8800 6a03 6a16 6a0c  d.........j.j.j.
-00000290: a00d 8700 6601 6419 640e 8408 a101 0100  ....f.d.d.......
-000002a0: 8800 6a03 6a17 6a0c a00d 8700 6601 641a  ..j.j.j.....f.d.
-000002b0: 640e 8408 a101 0100 641b 8800 5f18 7419  d.......d..._.t.
-000002c0: a01a a100 8800 5f1b 8800 6a1b 6a1c a00d  ......_...j.j...
-000002d0: 8800 6a1d a101 0100 8800 6a1b a01e 641c  ..j.......j...d.
-000002e0: a101 0100 6400 5300 291d 4e5a 0a49 6e4f  ....d.S.).NZ.InO
-000002f0: 7574 5175 696e 74e9 5000 0000 69f4 0100  utQuint.P...i...
-00000300: 0029 035a 2066 6f72 6d50 726f 6772 6573  .).Z formProgres
-00000310: 7341 6e69 6d61 7469 6f6e 4561 7369 6e67  sAnimationEasing
-00000320: 4375 7276 65da 0668 6569 6768 74da 0577  Curve..height..w
-00000330: 6964 7468 e90a 0000 0069 d007 0000 2903  idth.....i....).
-00000340: da11 666f 726d 5072 6f67 7265 7373 436f  ..formProgressCo
-00000350: 756e 74da 1d66 6f72 6d50 726f 6772 6573  unt..formProgres
-00000360: 7341 6e69 6d61 7469 6f6e 4475 7261 7469  sAnimationDurati
-00000370: 6f6e 7206 0000 00e9 0400 0000 e902 0000  onr.............
-00000380: 00e9 3c00 0000 2904 7209 0000 0072 0a00  ..<...).r....r..
-00000390: 0000 7206 0000 0072 0700 0000 e903 0000  ..r....r........
-000003a0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-000003b0: 0000 0300 0000 1300 0000 730e 0000 0088  ..........s.....
-000003c0: 006a 006a 01a0 0264 01a1 0153 00a9 024e  .j.j...d...S...N
-000003d0: e914 0000 00a9 03da 0275 69da 0877 6964  .........ui..wid
-000003e0: 6765 745f 32da 1361 6e69 6d61 7465 466f  get_2..animateFo
-000003f0: 726d 5072 6f67 7265 7373 a900 a901 da04  rmProgress......
-00000400: 7365 6c66 7215 0000 00fa 5363 3a5c 7573  selfr.....Sc:\us
-00000410: 6572 735c 6b69 6265 745c 616e 6163 6f6e  ers\kibet\anacon
-00000420: 6461 335c 4c69 625c 7369 7465 2d70 6163  da3\Lib\site-pac
-00000430: 6b61 6765 735c 4375 7374 6f6d 5f57 6964  kages\Custom_Wid
-00000440: 6765 7473 2f50 726f 6772 6573 7349 6e64  gets/ProgressInd
-00000450: 6963 6174 6f72 2f74 6573 742e 7079 da08  icator/test.py..
-00000460: 3c6c 616d 6264 613e 7a00 0000 f300 0000  <lambda>z.......
-00000470: 007a 254d 6169 6e57 696e 646f 772e 5f5f  .z%MainWindow.__
-00000480: 696e 6974 5f5f 2e3c 6c6f 6361 6c73 3e2e  init__.<locals>.
-00000490: 3c6c 616d 6264 613e 6300 0000 0000 0000  <lambda>c.......
-000004a0: 0000 0000 0000 0000 0003 0000 0013 0000  ................
-000004b0: 0073 0e00 0000 8800 6a00 6a01 a002 6401  .s......j.j...d.
-000004c0: a101 5300 a902 4ee9 2800 0000 7211 0000  ..S...N.(...r...
-000004d0: 0072 1500 0000 7216 0000 0072 1500 0000  .r....r....r....
-000004e0: 7218 0000 0072 1900 0000 7c00 0000 721a  r....r....|...r.
-000004f0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00000500: 0000 0000 0300 0000 1300 0000 730e 0000  ............s...
-00000510: 0088 006a 006a 01a0 0264 01a1 0153 00a9  ...j.j...d...S..
-00000520: 024e 720d 0000 0072 1100 0000 7215 0000  .Nr....r....r...
-00000530: 0072 1600 0000 7215 0000 0072 1800 0000  .r....r....r....
-00000540: 7219 0000 007e 0000 0072 1a00 0000 6300  r....~...r....c.
-00000550: 0000 0000 0000 0000 0000 0000 0000 0003  ................
-00000560: 0000 0013 0000 0073 0e00 0000 8800 6a00  .......s......j.
-00000570: 6a01 a002 6401 a101 5300 a902 4e72 0500  j...d...S...Nr..
-00000580: 0000 7211 0000 0072 1500 0000 7216 0000  ..r....r....r...
-00000590: 0072 1500 0000 7218 0000 0072 1900 0000  .r....r....r....
-000005a0: 8000 0000 721a 0000 0063 0000 0000 0000  ....r....c......
-000005b0: 0000 0000 0000 0000 0000 0300 0000 1300  ................
-000005c0: 0000 730e 0000 0088 006a 006a 01a0 0264  ..s......j.j...d
-000005d0: 01a1 0153 00a9 024e e964 0000 0072 1100  ...S...N.d...r..
-000005e0: 0000 7215 0000 0072 1600 0000 7215 0000  ..r....r....r...
-000005f0: 0072 1800 0000 7219 0000 0082 0000 0072  .r....r........r
-00000600: 1a00 0000 5429 03da 0c73 7465 705f 355f  ....T)...step_5_
-00000610: 6572 726f 725a 0e73 7465 705f 335f 7761  errorZ.step_3_wa
-00000620: 726e 696e 675a 0e73 7465 705f 385f 7375  rningZ.step_8_su
-00000630: 6363 6573 7329 0372 2100 0000 5a0e 7374  ccess).r!...Z.st
-00000640: 6570 5f32 5f77 6172 6e69 6e67 5a0e 7374  ep_2_warningZ.st
-00000650: 6570 5f33 5f73 7563 6365 7373 6300 0000  ep_3_successc...
-00000660: 0000 0000 0000 0000 0000 0000 0003 0000  ................
-00000670: 0013 0000 0073 0e00 0000 8800 6a00 6a01  .....s......j.j.
-00000680: a002 6401 a101 5300 720f 0000 00a9 0372  ..d...S.r......r
-00000690: 1200 0000 da06 7769 6467 6574 7214 0000  ......widgetr...
-000006a0: 0072 1500 0000 7216 0000 0072 1500 0000  .r....r....r....
-000006b0: 7218 0000 0072 1900 0000 9a00 0000 721a  r....r........r.
-000006c0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-000006d0: 0000 0000 0300 0000 1300 0000 730e 0000  ............s...
-000006e0: 0088 006a 006a 01a0 0264 01a1 0153 0072  ...j.j...d...S.r
-000006f0: 1b00 0000 7222 0000 0072 1500 0000 7216  ....r"...r....r.
-00000700: 0000 0072 1500 0000 7218 0000 0072 1900  ...r....r....r..
-00000710: 0000 9c00 0000 721a 0000 0063 0000 0000  ......r....c....
-00000720: 0000 0000 0000 0000 0000 0000 0300 0000  ................
-00000730: 1300 0000 730e 0000 0088 006a 006a 01a0  ....s......j.j..
-00000740: 0264 01a1 0153 0072 1d00 0000 7222 0000  .d...S.r....r"..
-00000750: 0072 1500 0000 7216 0000 0072 1500 0000  .r....r....r....
-00000760: 7218 0000 0072 1900 0000 9e00 0000 721a  r....r........r.
-00000770: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00000780: 0000 0000 0300 0000 1300 0000 730e 0000  ............s...
-00000790: 0088 006a 006a 01a0 0264 01a1 0153 0072  ...j.j...d...S.r
-000007a0: 1e00 0000 7222 0000 0072 1500 0000 7216  ....r"...r....r.
-000007b0: 0000 0072 1500 0000 7218 0000 0072 1900  ...r....r....r..
-000007c0: 0000 a000 0000 721a 0000 0063 0000 0000  ......r....c....
-000007d0: 0000 0000 0000 0000 0000 0000 0300 0000  ................
-000007e0: 1300 0000 730e 0000 0088 006a 006a 01a0  ....s......j.j..
-000007f0: 0264 01a1 0153 0072 1f00 0000 7222 0000  .d...S.r....r"..
-00000800: 0072 1500 0000 7216 0000 0072 1500 0000  .r....r....r....
-00000810: 7218 0000 0072 1900 0000 a200 0000 721a  r....r........r.
-00000820: 0000 0072 0100 0000 7220 0000 0029 1fda  ...r....r ...)..
-00000830: 0b51 4d61 696e 5769 6e64 6f77 da08 5f5f  .QMainWindow..__
-00000840: 696e 6974 5f5f 5a0d 5569 5f4d 6169 6e57  init__Z.Ui_MainW
-00000850: 696e 646f 7772 1200 0000 5a07 7365 7475  indowr....Z.setu
-00000860: 7055 6972 2300 0000 da1b 7570 6461 7465  pUir#.....update
-00000870: 466f 726d 5072 6f67 7265 7373 496e 6469  FormProgressIndi
-00000880: 6361 746f 7272 1300 0000 da20 7365 6c65  catorr..... sele
-00000890: 6374 466f 726d 5072 6f67 7265 7373 496e  ctFormProgressIn
-000008a0: 6469 6361 746f 7254 6865 6d65 7214 0000  dicatorThemer...
-000008b0: 00da 0877 6964 6765 745f 335a 0673 7465  ...widget_3Z.ste
-000008c0: 705f 365a 0763 6c69 636b 6564 da07 636f  p_6Z.clicked..co
-000008d0: 6e6e 6563 745a 0673 7465 705f 375a 0673  nnectZ.step_7Z.s
-000008e0: 7465 705f 385a 0673 7465 705f 395a 0773  tep_8Z.step_9Z.s
-000008f0: 7465 705f 3130 da0d 7365 7453 7465 7053  tep_10..setStepS
-00000900: 7461 7475 735a 0673 7465 705f 315a 0673  tatusZ.step_1Z.s
-00000910: 7465 705f 325a 0673 7465 705f 335a 0673  tep_2Z.step_3Z.s
-00000920: 7465 705f 345a 0673 7465 705f 35da 0864  tep_4Z.step_5..d
-00000930: 6f77 6e6c 6f61 6472 0200 0000 5a06 5154  ownloadr....Z.QT
-00000940: 696d 6572 da05 7469 6d65 72da 0774 696d  imer..timer..tim
-00000950: 656f 7574 da10 646f 776e 6c6f 6164 5072  eout..downloadPr
-00000960: 6f67 7265 7373 da05 7374 6172 7429 0272  ogress..start).r
-00000970: 1700 0000 da06 7061 7265 6e74 7215 0000  ......parentr...
-00000980: 0072 1600 0000 7218 0000 0072 2500 0000  .r....r....r%...
-00000990: 1d00 0000 7360 0000 0000 010a 0108 010c  ....s`..........
-000009a0: 0408 1002 0202 0202 ec06 1a08 0c02 0202  ................
-000009b0: 0402 ee06 190e 010e 010e 0308 0c02 0202  ................
-000009c0: 0402 0202 ec06 190e 010e 0418 0218 0218  ................
-000009d0: 0218 0218 0308 0202 0202 0202 fa06 0a08  ................
-000009e0: 0202 0202 0202 fa06 0b18 0218 0218 0218  ................
-000009f0: 0218 0406 010a 0110 017a 134d 6169 6e57  .........z.MainW
-00000a00: 696e 646f 772e 5f5f 696e 6974 5f5f 6301  indow.__init__c.
-00000a10: 0000 0000 0000 0000 0000 0008 0000 0007  ................
-00000a20: 0000 0043 0000 0073 4401 0000 6401 6402  ...C...sD...d.d.
-00000a30: 6403 6703 7d01 7c00 6a00 6404 6b00 7224  d.g.}.|.j.d.k.r$
-00000a40: 7c00 0400 6a00 6405 3700 0200 5f00 6ec8  |...j.d.7..._.n.
-00000a50: 6406 7c00 5f00 7401 6405 6407 8302 4400  d.|._.t.d.d...D.
-00000a60: 5d26 7d02 7c01 4400 5d1c 7d03 7c00 6a02  ]&}.|.D.].}.|.j.
-00000a70: 6a03 6a04 7405 7c02 8301 7c03 6408 6409  j.j.t.|...|.d.d.
-00000a80: 8d03 0100 713c 7134 7406 a007 640a 640b  ....q<q4t...d.d.
-00000a90: 640c 640d 640e 6705 a101 7d04 7406 a007  d.d.d.g...}.t...
-00000aa0: 640f 6410 6411 6412 6704 a101 7d05 7406  d.d.d.d.g...}.t.
-00000ab0: a007 6405 6413 640c 6414 640b 6705 a101  ..d.d.d.d.d.g...
-00000ac0: 7d06 7c00 6a02 6a03 6a08 7c04 7c05 6415  }.|.j.j.j.|.|.d.
-00000ad0: 8d02 0100 7c00 6a02 6a03 a009 7c06 a101  ....|.j.j...|...
-00000ae0: 0100 7c00 6a02 6a0a a00b 740c 7c06 8301  ..|.j.j...t.|...
-00000af0: a101 0100 7c00 6a02 6a0d a00b 740c 7c05  ....|.j.j...t.|.
-00000b00: 8301 a101 0100 7c00 6a02 6a0e a00b 740c  ......|.j.j...t.
-00000b10: 7c04 8301 a101 0100 7c00 6a02 6a03 a00f  |.......|.j.j...
-00000b20: 7c00 6a00 a101 0100 7406 a007 7c01 a101  |.j.....t...|...
-00000b30: 7d07 7c00 6a00 7c00 6a02 6a03 6a10 1600  }.|.j.|.j.j.j...
-00000b40: 6406 6b02 9001 7240 7c00 6a02 6a03 6a04  d.k...r@|.j.j.j.
-00000b50: 7405 7c00 6a00 7c00 6a02 6a03 6a10 1b00  t.|.j.|.j.j.j...
-00000b60: 8301 7c07 6416 6409 8d03 0100 6400 5300  ..|.d.d.....d.S.
-00000b70: 2917 4eda 0777 6172 6e69 6e67 da05 6572  ).N..warning..er
-00000b80: 726f 72da 0773 7563 6365 7373 e965 0000  ror..success.e..
-00000b90: 00e9 0100 0000 7201 0000 00e9 0b00 0000  ......r.........
-00000ba0: 4629 03da 0473 7465 70da 0673 7461 7475  F)...step..statu
-00000bb0: 73da 0576 616c 7565 7208 0000 00e9 0500  s..valuer.......
-00000bc0: 0000 720e 0000 00e9 0700 0000 e90f 0000  ..r.............
-00000bd0: 0072 1000 0000 721c 0000 00e9 3200 0000  .r....r.....2...
-00000be0: 720d 0000 0072 0c00 0000 720b 0000 0029  r....r....r....)
-00000bf0: 0272 0900 0000 7206 0000 0054 2911 722b  .r....r....T).r+
-00000c00: 0000 00da 0572 616e 6765 7212 0000 0072  .....ranger....r
-00000c10: 2800 0000 722a 0000 00da 0369 6e74 da06  (...r*.....int..
-00000c20: 7261 6e64 6f6d da06 6368 6f69 6365 7226  random..choicer&
-00000c30: 0000 0072 2700 0000 da05 7468 656d 655a  ...r'.....themeZ
-00000c40: 0773 6574 5465 7874 da03 7374 7272 0600  .setText..strr..
-00000c50: 0000 5a05 7374 6570 7372 1400 0000 7209  ..Z.stepsr....r.
-00000c60: 0000 0029 0872 1700 0000 5a08 7374 6174  ...).r....Z.stat
-00000c70: 7573 6573 da01 78da 0179 7209 0000 0072  uses..x..yr....r
-00000c80: 0600 0000 7242 0000 005a 0a72 616e 6453  ....rB...Z.randS
-00000c90: 7461 7475 7372 1500 0000 7215 0000 0072  tatusr....r....r
-00000ca0: 1800 0000 722e 0000 00af 0000 0073 3c00  ....r........s<.
-00000cb0: 0000 0002 0a01 0a01 1003 0602 0e02 0801  ................
-00000cc0: 0801 0602 0202 02fb 0a09 1401 1201 1402  ................
-00000cd0: 0802 0202 02fc 0607 0e03 1201 1201 1204  ................
-00000ce0: 1003 0a01 1601 0801 1202 0202 02fb 7a1b  ..............z.
-00000cf0: 4d61 696e 5769 6e64 6f77 2e64 6f77 6e6c  MainWindow.downl
-00000d00: 6f61 6450 726f 6772 6573 7329 014e 2905  oadProgress).N).
-00000d10: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-00000d20: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-00000d30: 6d65 5f5f 7225 0000 0072 2e00 0000 7215  me__r%...r....r.
-00000d40: 0000 0072 1500 0000 7215 0000 0072 1800  ...r....r....r..
-00000d50: 0000 7204 0000 001c 0000 0073 0600 0000  ..r........s....
-00000d60: 0801 0a7f 0013 7204 0000 0063 0000 0000  ......r....c....
-00000d70: 0000 0000 0000 0000 0200 0000 0400 0000  ................
-00000d80: 4300 0000 732a 0000 0074 0074 016a 0283  C...s*...t.t.j..
-00000d90: 017d 0074 0383 007d 017c 01a0 04a1 0001  .}.t...}.|......
-00000da0: 0074 01a0 057c 00a0 06a1 00a1 0101 0064  .t...|.........d
-00000db0: 0053 0029 014e 2907 5a0c 5141 7070 6c69  .S.).N).Z.QAppli
-00000dc0: 6361 7469 6f6e da03 7379 73da 0461 7267  cation..sys..arg
-00000dd0: 7672 0400 0000 da04 7368 6f77 da04 6578  vr......show..ex
-00000de0: 6974 da05 6578 6563 5f29 025a 0361 7070  it..exec_).Z.app
-00000df0: 5a06 7769 6e64 6f77 7215 0000 0072 1500  Z.windowr....r..
-00000e00: 0000 7218 0000 00da 046d 6169 6eea 0000  ..r......main...
-00000e10: 0073 0800 0000 0001 0a04 0601 0801 724e  .s............rN
-00000e20: 0000 0029 0a72 4900 0000 5a07 5079 5369  ...).rI...Z.PySi
-00000e30: 6465 3272 0200 0000 5a0e 5079 5369 6465  de2r....Z.PySide
-00000e40: 322e 5174 436f 7265 7240 0000 005a 2d43  2.QtCorer@...Z-C
-00000e50: 7573 746f 6d5f 5769 6467 6574 732e 5072  ustom_Widgets.Pr
-00000e60: 6f67 7265 7373 496e 6469 6361 746f 722e  ogressIndicator.
-00000e70: 7569 5f69 6e74 6572 6661 6365 5a0e 4375  ui_interfaceZ.Cu
-00000e80: 7374 6f6d 5f57 6964 6765 7473 7224 0000  stom_Widgetsr$..
-00000e90: 0072 0400 0000 724e 0000 0072 1500 0000  .r....rN...r....
-00000ea0: 7215 0000 0072 1500 0000 7218 0000 00da  r....r....r.....
-00000eb0: 083c 6d6f 6475 6c65 3e0a 0000 0073 1000  .<module>....s..
-00000ec0: 0000 0801 0c01 0801 0803 0806 0806 107f  ................
-00000ed0: 004f                                     .O
+00000020: 0009 0000 0040 0000 0073 9800 0000 6400  .....@...s....d.
+00000030: 6401 6c00 5a00 7a18 6400 6402 6c01 6d02  d.l.Z.z.d.d.l.m.
+00000040: 5a02 0100 6400 6403 6c03 5400 5700 6e42  Z...d.d.l.T.W.nB
+00000050: 0100 0100 0100 7a18 6400 6402 6c04 6d02  ......z.d.d.l.m.
+00000060: 5a02 0100 6400 6403 6c05 5400 5700 6e1c  Z...d.d.l.T.W.n.
+00000070: 0100 0100 0100 6506 6404 8301 0100 6500  ......e.d.....e.
+00000080: a007 a100 0100 5900 6e02 5800 5900 6e02  ......Y.n.X.Y.n.
+00000090: 5800 6400 6401 6c08 5a08 6400 6403 6c09  X.d.d.l.Z.d.d.l.
+000000a0: 5400 6400 6403 6c0a 5400 4700 6405 6406  T.d.d.l.T.G.d.d.
+000000b0: 8400 6406 650b 8303 5a0c 6407 6408 8400  ..d.e...Z.d.d...
+000000c0: 5a0d 6401 5300 2909 e900 0000 004e 2901  Z.d.S.)......N).
+000000d0: da06 5174 436f 7265 2901 da01 2a7a 1b4e  ..QtCore)...*z.N
+000000e0: 6f20 5079 5369 6465 3220 6f72 2050 7953  o PySide2 or PyS
+000000f0: 6964 6536 2066 6f75 6e64 6300 0000 0000  ide6 foundc.....
+00000100: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
+00000110: 0000 0073 1e00 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
+00000120: 6406 6402 6403 8401 5a03 6404 6405 8400  d.d.d...Z.d.d...
+00000130: 5a04 6401 5300 2907 da0a 4d61 696e 5769  Z.d.S.)...MainWi
+00000140: 6e64 6f77 4e63 0200 0000 0000 0000 0000  ndowNc..........
+00000150: 0000 0200 0000 0600 0000 0300 0000 73ea  ..............s.
+00000160: 0100 0074 00a0 0188 00a1 0101 0074 0283  ...t.........t..
+00000170: 0088 005f 0388 006a 03a0 0488 00a1 0101  ..._...j........
+00000180: 0088 006a 036a 056a 0664 0164 0264 0364  ...j.j.j.d.d.d.d
+00000190: 048d 0301 0088 006a 036a 076a 0664 0564  .......j.j.j.d.d
+000001a0: 0664 0264 078d 0301 0088 006a 036a 05a0  .d.d.......j.j..
+000001b0: 0864 08a1 0101 0088 006a 036a 07a0 0864  .d.......j.j...d
+000001c0: 09a1 0101 0088 006a 036a 07a0 0964 0aa1  .......j.j...d..
+000001d0: 0101 0088 006a 036a 0a6a 0664 0564 0664  .....j.j.j.d.d.d
+000001e0: 0264 0364 0b8d 0401 0088 006a 036a 0aa0  .d.d.......j.j..
+000001f0: 0864 0ca1 0101 0088 006a 036a 0aa0 0964  .d.......j.j...d
+00000200: 0aa1 0101 0088 006a 036a 0b6a 0ca0 0d87  .......j.j.j....
+00000210: 0066 0164 0d64 0e84 08a1 0101 0088 006a  .f.d.d.........j
+00000220: 036a 0e6a 0ca0 0d87 0066 0164 0f64 0e84  .j.j.....f.d.d..
+00000230: 08a1 0101 0088 006a 036a 0f6a 0ca0 0d87  .......j.j.j....
+00000240: 0066 0164 1064 0e84 08a1 0101 0088 006a  .f.d.d.........j
+00000250: 036a 106a 0ca0 0d87 0066 0164 1164 0e84  .j.j.....f.d.d..
+00000260: 08a1 0101 0088 006a 036a 116a 0ca0 0d87  .......j.j.j....
+00000270: 0066 0164 1264 0e84 08a1 0101 0088 006a  .f.d.d.........j
+00000280: 036a 076a 1264 1364 1364 1364 148d 0301  .j.j.d.d.d.d....
+00000290: 0088 006a 036a 056a 1264 1364 1364 1364  ...j.j.j.d.d.d.d
+000002a0: 158d 0301 0088 006a 036a 136a 0ca0 0d87  .......j.j.j....
+000002b0: 0066 0164 1664 0e84 08a1 0101 0088 006a  .f.d.d.........j
+000002c0: 036a 146a 0ca0 0d87 0066 0164 1764 0e84  .j.j.....f.d.d..
+000002d0: 08a1 0101 0088 006a 036a 156a 0ca0 0d87  .......j.j.j....
+000002e0: 0066 0164 1864 0e84 08a1 0101 0088 006a  .f.d.d.........j
+000002f0: 036a 166a 0ca0 0d87 0066 0164 1964 0e84  .j.j.....f.d.d..
+00000300: 08a1 0101 0088 006a 036a 176a 0ca0 0d87  .......j.j.j....
+00000310: 0066 0164 1a64 0e84 08a1 0101 0064 1b88  .f.d.d.......d..
+00000320: 005f 1874 19a0 1aa1 0088 005f 1b88 006a  ._.t......._...j
+00000330: 1b6a 1ca0 0d88 006a 1da1 0101 0088 006a  .j.....j.......j
+00000340: 1ba0 1e64 1ca1 0101 0064 0053 0029 1d4e  ...d.....d.S.).N
+00000350: 5a0a 496e 4f75 7451 7569 6e74 e950 0000  Z.InOutQuint.P..
+00000360: 0069 f401 0000 2903 5a20 666f 726d 5072  .i....).Z formPr
+00000370: 6f67 7265 7373 416e 696d 6174 696f 6e45  ogressAnimationE
+00000380: 6173 696e 6743 7572 7665 da06 6865 6967  asingCurve..heig
+00000390: 6874 da05 7769 6474 68e9 0a00 0000 69d0  ht..width.....i.
+000003a0: 0700 0029 03da 1166 6f72 6d50 726f 6772  ...)...formProgr
+000003b0: 6573 7343 6f75 6e74 da1d 666f 726d 5072  essCount..formPr
+000003c0: 6f67 7265 7373 416e 696d 6174 696f 6e44  ogressAnimationD
+000003d0: 7572 6174 696f 6e72 0600 0000 e904 0000  urationr........
+000003e0: 00e9 0200 0000 e93c 0000 0029 0472 0900  .......<...).r..
+000003f0: 0000 720a 0000 0072 0600 0000 7207 0000  ..r....r....r...
+00000400: 00e9 0300 0000 6300 0000 0000 0000 0000  ......c.........
+00000410: 0000 0000 0000 0003 0000 0013 0000 0073  ...............s
+00000420: 0e00 0000 8800 6a00 6a01 a002 6401 a101  ......j.j...d...
+00000430: 5300 a902 4ee9 1400 0000 a903 da02 7569  S...N.........ui
+00000440: da08 7769 6467 6574 5f32 da13 616e 696d  ..widget_2..anim
+00000450: 6174 6546 6f72 6d50 726f 6772 6573 73a9  ateFormProgress.
+00000460: 00a9 01da 0473 656c 6672 1500 0000 fa53  .....selfr.....S
+00000470: 633a 5c75 7365 7273 5c6b 6962 6574 5c61  c:\users\kibet\a
+00000480: 6e61 636f 6e64 6133 5c4c 6962 5c73 6974  naconda3\Lib\sit
+00000490: 652d 7061 636b 6167 6573 5c43 7573 746f  e-packages\Custo
+000004a0: 6d5f 5769 6467 6574 732f 5072 6f67 7265  m_Widgets/Progre
+000004b0: 7373 496e 6469 6361 746f 722f 7465 7374  ssIndicator/test
+000004c0: 2e70 79da 083c 6c61 6d62 6461 3e8a 0000  .py..<lambda>...
+000004d0: 00f3 0000 0000 7a25 4d61 696e 5769 6e64  ......z%MainWind
+000004e0: 6f77 2e5f 5f69 6e69 745f 5f2e 3c6c 6f63  ow.__init__.<loc
+000004f0: 616c 733e 2e3c 6c61 6d62 6461 3e63 0000  als>.<lambda>c..
+00000500: 0000 0000 0000 0000 0000 0000 0000 0300  ................
+00000510: 0000 1300 0000 730e 0000 0088 006a 006a  ......s......j.j
+00000520: 01a0 0264 01a1 0153 00a9 024e e928 0000  ...d...S...N.(..
+00000530: 0072 1100 0000 7215 0000 0072 1600 0000  .r....r....r....
+00000540: 7215 0000 0072 1800 0000 7219 0000 008c  r....r....r.....
+00000550: 0000 0072 1a00 0000 6300 0000 0000 0000  ...r....c.......
+00000560: 0000 0000 0000 0000 0003 0000 0013 0000  ................
+00000570: 0073 0e00 0000 8800 6a00 6a01 a002 6401  .s......j.j...d.
+00000580: a101 5300 a902 4e72 0d00 0000 7211 0000  ..S...Nr....r...
+00000590: 0072 1500 0000 7216 0000 0072 1500 0000  .r....r....r....
+000005a0: 7218 0000 0072 1900 0000 8e00 0000 721a  r....r........r.
+000005b0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+000005c0: 0000 0000 0300 0000 1300 0000 730e 0000  ............s...
+000005d0: 0088 006a 006a 01a0 0264 01a1 0153 00a9  ...j.j...d...S..
+000005e0: 024e 7205 0000 0072 1100 0000 7215 0000  .Nr....r....r...
+000005f0: 0072 1600 0000 7215 0000 0072 1800 0000  .r....r....r....
+00000600: 7219 0000 0090 0000 0072 1a00 0000 6300  r........r....c.
+00000610: 0000 0000 0000 0000 0000 0000 0000 0003  ................
+00000620: 0000 0013 0000 0073 0e00 0000 8800 6a00  .......s......j.
+00000630: 6a01 a002 6401 a101 5300 a902 4ee9 6400  j...d...S...N.d.
+00000640: 0000 7211 0000 0072 1500 0000 7216 0000  ..r....r....r...
+00000650: 0072 1500 0000 7218 0000 0072 1900 0000  .r....r....r....
+00000660: 9200 0000 721a 0000 0054 2903 da0c 7374  ....r....T)...st
+00000670: 6570 5f35 5f65 7272 6f72 5a0e 7374 6570  ep_5_errorZ.step
+00000680: 5f33 5f77 6172 6e69 6e67 5a0e 7374 6570  _3_warningZ.step
+00000690: 5f38 5f73 7563 6365 7373 2903 7221 0000  _8_success).r!..
+000006a0: 005a 0e73 7465 705f 325f 7761 726e 696e  .Z.step_2_warnin
+000006b0: 675a 0e73 7465 705f 335f 7375 6363 6573  gZ.step_3_succes
+000006c0: 7363 0000 0000 0000 0000 0000 0000 0000  sc..............
+000006d0: 0000 0300 0000 1300 0000 730e 0000 0088  ..........s.....
+000006e0: 006a 006a 01a0 0264 01a1 0153 0072 0f00  .j.j...d...S.r..
+000006f0: 0000 a903 7212 0000 00da 0677 6964 6765  ....r......widge
+00000700: 7472 1400 0000 7215 0000 0072 1600 0000  tr....r....r....
+00000710: 7215 0000 0072 1800 0000 7219 0000 00aa  r....r....r.....
+00000720: 0000 0072 1a00 0000 6300 0000 0000 0000  ...r....c.......
+00000730: 0000 0000 0000 0000 0003 0000 0013 0000  ................
+00000740: 0073 0e00 0000 8800 6a00 6a01 a002 6401  .s......j.j...d.
+00000750: a101 5300 721b 0000 0072 2200 0000 7215  ..S.r....r"...r.
+00000760: 0000 0072 1600 0000 7215 0000 0072 1800  ...r....r....r..
+00000770: 0000 7219 0000 00ac 0000 0072 1a00 0000  ..r........r....
+00000780: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000790: 0003 0000 0013 0000 0073 0e00 0000 8800  .........s......
+000007a0: 6a00 6a01 a002 6401 a101 5300 721d 0000  j.j...d...S.r...
+000007b0: 0072 2200 0000 7215 0000 0072 1600 0000  .r"...r....r....
+000007c0: 7215 0000 0072 1800 0000 7219 0000 00ae  r....r....r.....
+000007d0: 0000 0072 1a00 0000 6300 0000 0000 0000  ...r....c.......
+000007e0: 0000 0000 0000 0000 0003 0000 0013 0000  ................
+000007f0: 0073 0e00 0000 8800 6a00 6a01 a002 6401  .s......j.j...d.
+00000800: a101 5300 721e 0000 0072 2200 0000 7215  ..S.r....r"...r.
+00000810: 0000 0072 1600 0000 7215 0000 0072 1800  ...r....r....r..
+00000820: 0000 7219 0000 00b0 0000 0072 1a00 0000  ..r........r....
+00000830: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000840: 0003 0000 0013 0000 0073 0e00 0000 8800  .........s......
+00000850: 6a00 6a01 a002 6401 a101 5300 721f 0000  j.j...d...S.r...
+00000860: 0072 2200 0000 7215 0000 0072 1600 0000  .r"...r....r....
+00000870: 7215 0000 0072 1800 0000 7219 0000 00b2  r....r....r.....
+00000880: 0000 0072 1a00 0000 7201 0000 0072 2000  ...r....r....r .
+00000890: 0000 291f da0b 514d 6169 6e57 696e 646f  ..)...QMainWindo
+000008a0: 77da 085f 5f69 6e69 745f 5f5a 0d55 695f  w..__init__Z.Ui_
+000008b0: 4d61 696e 5769 6e64 6f77 7212 0000 005a  MainWindowr....Z
+000008c0: 0773 6574 7570 5569 7223 0000 00da 1b75  .setupUir#.....u
+000008d0: 7064 6174 6546 6f72 6d50 726f 6772 6573  pdateFormProgres
+000008e0: 7349 6e64 6963 6174 6f72 7213 0000 00da  sIndicatorr.....
+000008f0: 2073 656c 6563 7446 6f72 6d50 726f 6772   selectFormProgr
+00000900: 6573 7349 6e64 6963 6174 6f72 5468 656d  essIndicatorThem
+00000910: 6572 1400 0000 da08 7769 6467 6574 5f33  er......widget_3
+00000920: 5a06 7374 6570 5f36 5a07 636c 6963 6b65  Z.step_6Z.clicke
+00000930: 64da 0763 6f6e 6e65 6374 5a06 7374 6570  d..connectZ.step
+00000940: 5f37 5a06 7374 6570 5f38 5a06 7374 6570  _7Z.step_8Z.step
+00000950: 5f39 5a07 7374 6570 5f31 30da 0d73 6574  _9Z.step_10..set
+00000960: 5374 6570 5374 6174 7573 5a06 7374 6570  StepStatusZ.step
+00000970: 5f31 5a06 7374 6570 5f32 5a06 7374 6570  _1Z.step_2Z.step
+00000980: 5f33 5a06 7374 6570 5f34 5a06 7374 6570  _3Z.step_4Z.step
+00000990: 5f35 da08 646f 776e 6c6f 6164 7202 0000  _5..downloadr...
+000009a0: 005a 0651 5469 6d65 72da 0574 696d 6572  .Z.QTimer..timer
+000009b0: da07 7469 6d65 6f75 74da 1064 6f77 6e6c  ..timeout..downl
+000009c0: 6f61 6450 726f 6772 6573 73da 0573 7461  oadProgress..sta
+000009d0: 7274 2902 7217 0000 00da 0670 6172 656e  rt).r......paren
+000009e0: 7472 1500 0000 7216 0000 0072 1800 0000  tr....r....r....
+000009f0: 7225 0000 002d 0000 0073 6000 0000 0001  r%...-...s`.....
+00000a00: 0a01 0801 0c04 0810 0202 0202 02ec 061a  ................
+00000a10: 080c 0202 0204 02ee 0619 0e01 0e01 0e03  ................
+00000a20: 080c 0202 0204 0202 02ec 0619 0e01 0e04  ................
+00000a30: 1802 1802 1802 1802 1803 0802 0202 0202  ................
+00000a40: 02fa 060a 0802 0202 0202 02fa 060b 1802  ................
+00000a50: 1802 1802 1802 1804 0601 0a01 1001 7a13  ..............z.
+00000a60: 4d61 696e 5769 6e64 6f77 2e5f 5f69 6e69  MainWindow.__ini
+00000a70: 745f 5f63 0100 0000 0000 0000 0000 0000  t__c............
+00000a80: 0800 0000 0700 0000 4300 0000 7344 0100  ........C...sD..
+00000a90: 0064 0164 0264 0367 037d 017c 006a 0064  .d.d.d.g.}.|.j.d
+00000aa0: 046b 0072 247c 0004 006a 0064 0537 0002  .k.r$|...j.d.7..
+00000ab0: 005f 006e c864 067c 005f 0074 0164 0564  ._.n.d.|._.t.d.d
+00000ac0: 0783 0244 005d 267d 027c 0144 005d 1c7d  ...D.]&}.|.D.].}
+00000ad0: 037c 006a 026a 036a 0474 057c 0283 017c  .|.j.j.j.t.|...|
+00000ae0: 0364 0864 098d 0301 0071 3c71 3474 06a0  .d.d.....q<q4t..
+00000af0: 0764 0a64 0b64 0c64 0d64 0e67 05a1 017d  .d.d.d.d.d.g...}
+00000b00: 0474 06a0 0764 0f64 1064 1164 1267 04a1  .t...d.d.d.d.g..
+00000b10: 017d 0574 06a0 0764 0564 1364 0c64 1464  .}.t...d.d.d.d.d
+00000b20: 0b67 05a1 017d 067c 006a 026a 036a 087c  .g...}.|.j.j.j.|
+00000b30: 047c 0564 158d 0201 007c 006a 026a 03a0  .|.d.....|.j.j..
+00000b40: 097c 06a1 0101 007c 006a 026a 0aa0 0b74  .|.....|.j.j...t
+00000b50: 0c7c 0683 01a1 0101 007c 006a 026a 0da0  .|.......|.j.j..
+00000b60: 0b74 0c7c 0583 01a1 0101 007c 006a 026a  .t.|.......|.j.j
+00000b70: 0ea0 0b74 0c7c 0483 01a1 0101 007c 006a  ...t.|.......|.j
+00000b80: 026a 03a0 0f7c 006a 00a1 0101 0074 06a0  .j...|.j.....t..
+00000b90: 077c 01a1 017d 077c 006a 007c 006a 026a  .|...}.|.j.|.j.j
+00000ba0: 036a 1016 0064 066b 0290 0172 407c 006a  .j...d.k...r@|.j
+00000bb0: 026a 036a 0474 057c 006a 007c 006a 026a  .j.j.t.|.j.|.j.j
+00000bc0: 036a 101b 0083 017c 0764 1664 098d 0301  .j.....|.d.d....
+00000bd0: 0064 0053 0029 174e da07 7761 726e 696e  .d.S.).N..warnin
+00000be0: 67da 0565 7272 6f72 da07 7375 6363 6573  g..error..succes
+00000bf0: 73e9 6500 0000 e901 0000 0072 0100 0000  s.e........r....
+00000c00: e90b 0000 0046 2903 da04 7374 6570 da06  .....F)...step..
+00000c10: 7374 6174 7573 da05 7661 6c75 6572 0800  status..valuer..
+00000c20: 0000 e905 0000 0072 0e00 0000 e907 0000  .......r........
+00000c30: 00e9 0f00 0000 7210 0000 0072 1c00 0000  ......r....r....
+00000c40: e932 0000 0072 0d00 0000 720c 0000 0072  .2...r....r....r
+00000c50: 0b00 0000 2902 7209 0000 0072 0600 0000  ....).r....r....
+00000c60: 5429 1172 2b00 0000 da05 7261 6e67 6572  T).r+.....ranger
+00000c70: 1200 0000 7228 0000 0072 2a00 0000 da03  ....r(...r*.....
+00000c80: 696e 74da 0672 616e 646f 6dda 0663 686f  int..random..cho
+00000c90: 6963 6572 2600 0000 7227 0000 00da 0574  icer&...r'.....t
+00000ca0: 6865 6d65 5a07 7365 7454 6578 74da 0373  hemeZ.setText..s
+00000cb0: 7472 7206 0000 005a 0573 7465 7073 7214  trr....Z.stepsr.
+00000cc0: 0000 0072 0900 0000 2908 7217 0000 005a  ...r....).r....Z
+00000cd0: 0873 7461 7475 7365 73da 0178 da01 7972  .statuses..x..yr
+00000ce0: 0900 0000 7206 0000 0072 4200 0000 5a0a  ....r....rB...Z.
+00000cf0: 7261 6e64 5374 6174 7573 7215 0000 0072  randStatusr....r
+00000d00: 1500 0000 7218 0000 0072 2e00 0000 bf00  ....r....r......
+00000d10: 0000 733c 0000 0000 020a 010a 0110 0306  ..s<............
+00000d20: 020e 0208 0108 0106 0202 0202 fb0a 0914  ................
+00000d30: 0112 0114 0208 0202 0202 fc06 070e 0312  ................
+00000d40: 0112 0112 0410 030a 0116 0108 0112 0202  ................
+00000d50: 0202 fb7a 1b4d 6169 6e57 696e 646f 772e  ...z.MainWindow.
+00000d60: 646f 776e 6c6f 6164 5072 6f67 7265 7373  downloadProgress
+00000d70: 2901 4e29 05da 085f 5f6e 616d 655f 5fda  ).N)...__name__.
+00000d80: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+00000d90: 7561 6c6e 616d 655f 5f72 2500 0000 722e  ualname__r%...r.
+00000da0: 0000 0072 1500 0000 7215 0000 0072 1500  ...r....r....r..
+00000db0: 0000 7218 0000 0072 0400 0000 2c00 0000  ..r....r....,...
+00000dc0: 7306 0000 0008 010a 7f00 1372 0400 0000  s..........r....
+00000dd0: 6300 0000 0000 0000 0000 0000 0002 0000  c...............
+00000de0: 0004 0000 0043 0000 0073 2a00 0000 7400  .....C...s*...t.
+00000df0: 7401 6a02 8301 7d00 7403 8300 7d01 7c01  t.j...}.t...}.|.
+00000e00: a004 a100 0100 7401 a005 7c00 a006 a100  ......t...|.....
+00000e10: a101 0100 6400 5300 2901 4e29 075a 0c51  ....d.S.).N).Z.Q
+00000e20: 4170 706c 6963 6174 696f 6eda 0373 7973  Application..sys
+00000e30: da04 6172 6776 7204 0000 00da 0473 686f  ..argvr......sho
+00000e40: 77da 0465 7869 74da 0565 7865 635f 2902  w..exit..exec_).
+00000e50: 5a03 6170 705a 0677 696e 646f 7772 1500  Z.appZ.windowr..
+00000e60: 0000 7215 0000 0072 1800 0000 da04 6d61  ..r....r......ma
+00000e70: 696e fa00 0000 7308 0000 0000 010a 0406  in....s.........
+00000e80: 0108 0172 4e00 0000 290e 7249 0000 005a  ...rN...).rI...Z
+00000e90: 0750 7953 6964 6532 7202 0000 005a 0e50  .PySide2r....Z.P
+00000ea0: 7953 6964 6532 2e51 7443 6f72 655a 0750  ySide2.QtCoreZ.P
+00000eb0: 7953 6964 6536 5a0e 5079 5369 6465 362e  ySide6Z.PySide6.
+00000ec0: 5174 436f 7265 da05 7072 696e 7472 4c00  QtCore..printrL.
+00000ed0: 0000 7240 0000 005a 2d43 7573 746f 6d5f  ..r@...Z-Custom_
+00000ee0: 5769 6467 6574 732e 5072 6f67 7265 7373  Widgets.Progress
+00000ef0: 496e 6469 6361 746f 722e 7569 5f69 6e74  Indicator.ui_int
+00000f00: 6572 6661 6365 5a0e 4375 7374 6f6d 5f57  erfaceZ.Custom_W
+00000f10: 6964 6765 7473 7224 0000 0072 0400 0000  idgetsr$...r....
+00000f20: 724e 0000 0072 1500 0000 7215 0000 0072  rN...r....r....r
+00000f30: 1500 0000 7218 0000 00da 083c 6d6f 6475  ....r......<modu
+00000f40: 6c65 3e0a 0000 0073 2000 0000 0802 0201  le>....s .......
+00000f50: 0c01 0c02 0601 0201 0c01 0c02 0601 0802  ................
+00000f60: 1405 0803 0806 0806 107f 004f            ...........O
```

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/ProgressIndicator/__pycache__/ui_interface.cpython-310.pyc` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/ProgressIndicator/__pycache__/ui_interface.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/ProgressIndicator/__pycache__/ui_interface.cpython-38.pyc` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/ProgressIndicator/__pycache__/ui_interface.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Mar  4 16:18:45 2022 UTC, .py size: 9581 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 e53b 2262 6d25 0000  U........;"bm%..
+00000000: 550d 0d0a 0000 0000 6a61 9364 9d25 0000  U.......ja.d.%..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3800 0000 6400  .....@...s8...d.
 00000030: 6401 6c00 5400 6400 6401 6c01 5400 6400  d.l.T.d.d.l.T.d.
 00000040: 6401 6c02 5400 6400 6402 6c03 6d04 5a04  d.l.T.d.d.l.m.Z.
 00000050: 0100 4700 6403 6404 8400 6404 6505 8303  ..G.d.d...d.e...
 00000060: 5a06 6405 5300 2906 e900 0000 0029 01da  Z.d.S.)......)..
 00000070: 012a 2901 da15 466f 726d 5072 6f67 7265  .*)...FormProgre
```

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/ProgressIndicator/__pycache__/ui_interface.cpython-39.pyc` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/ProgressIndicator/__pycache__/ui_interface.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/ProgressIndicator/interface.ui` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/ProgressIndicator/interface.ui`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/ProgressIndicator/test.py` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/ProgressIndicator/test.py`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/ProgressIndicator/ui_interface.py` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/ProgressIndicator/ui_interface.py`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/ProjectMaker.py` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/ProjectMaker.py`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/QSS_Resources.qrc` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/QSS_Resources.qrc`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/SassCompiler.py` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/SassCompiler.py`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/SvgToPngIcons.py` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/SvgToPngIcons.py`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/__pycache__/QSS_Resources.cpython-39.pyc` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/QSS_Resources.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/__pycache__/SassCompiler.cpython-310.pyc` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/SassCompiler.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/__pycache__/SassCompiler.cpython-38.pyc` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/SassCompiler.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon Mar 14 09:36:36 2022 UTC, .py size: 4818 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,190 +1,194 @@
-00000000: 550d 0d0a 0000 0000 a40c 2f62 d212 0000  U........./b....
+00000000: 550d 0d0a 0000 0000 6a61 9364 8115 0000  U.......ja.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 7800 0000 6400  .....@...sx...d.
-00000030: 6401 6c00 5400 6400 6401 6c01 5400 6400  d.l.T.d.d.l.T.d.
-00000040: 6401 6c02 5400 6400 6402 6c03 5a03 6400  d.l.T.d.d.l.Z.d.
-00000050: 6402 6c04 5a04 6400 6402 6c05 5a05 6403  d.l.Z.d.d.l.Z.d.
-00000060: 6404 6c06 6d07 5a07 6d08 5a08 6d09 5a09  d.l.m.Z.m.Z.m.Z.
-00000070: 0100 6403 6405 6c0a 6d0b 5a0b 0100 6406  ..d.d.l.m.Z...d.
-00000080: 6407 6c0c 6d0d 5a0d 6d0e 5a0e 0100 650f  d.l.m.Z.m.Z...e.
-00000090: 8300 5a10 4700 6408 6409 8400 6409 8302  ..Z.G.d.d...d...
-000000a0: 5a11 6402 5300 290a e900 0000 0029 01da  Z.d.S.)......)..
-000000b0: 012a 4ee9 0100 0000 2903 da13 4372 6561  .*N.....)...Crea
-000000c0: 7465 436f 6c6f 7256 6172 6961 626c 65da  teColorVariable.
-000000d0: 0444 6172 6bda 054c 6967 6874 2901 da11  .Dark..Light)...
-000000e0: 4e65 7749 636f 6e73 4765 6e65 7261 746f  NewIconsGenerato
-000000f0: 72e9 0200 0000 2902 da06 576f 726b 6572  r.....)...Worker
-00000100: da0e 576f 726b 6572 5265 7370 6f6e 7365  ..WorkerResponse
-00000110: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000120: 0004 0000 0000 0000 0073 2600 0000 6500  .........s&...e.
-00000130: 5a01 6400 5a02 6406 8700 6601 6402 6403  Z.d.Z.d...f.d.d.
-00000140: 8409 5a03 6404 6405 8400 5a04 8700 0400  ..Z.d.d...Z.....
-00000150: 5a05 5300 2907 da11 436f 6d70 696c 6553  Z.S.)...CompileS
-00000160: 7479 6c65 5368 6565 744e 6302 0000 0000  tyleSheetNc.....
-00000170: 0000 0000 0000 0002 0000 0003 0000 0003  ................
-00000180: 0000 0073 1400 0000 7400 7401 7c00 8302  ...s....t.t.|...
-00000190: a002 7c01 a101 0100 6400 5300 2901 4e29  ..|.....d.S.).N)
-000001a0: 03da 0573 7570 6572 720b 0000 00da 085f  ...superr......_
-000001b0: 5f69 6e69 745f 5f29 02da 0473 656c 66da  _init__)...self.
-000001c0: 0670 6172 656e 74a9 01da 095f 5f63 6c61  .parent....__cla
-000001d0: 7373 5f5f a900 fa38 453a 5c53 7069 6e6e  ss__...8E:\Spinn
-000001e0: 2054 5620 5475 745c 3232 2d55 495c 4375   TV Tut\22-UI\Cu
-000001f0: 7374 6f6d 5f57 6964 6765 7473 5c51 7373  stom_Widgets\Qss
-00000200: 5c53 6173 7343 6f6d 7069 6c65 722e 7079  \SassCompiler.py
-00000210: 720d 0000 0022 0000 0073 0200 0000 0001  r...."...s......
-00000220: 7a1a 436f 6d70 696c 6553 7479 6c65 5368  z.CompileStyleSh
-00000230: 6565 742e 5f5f 696e 6974 5f5f 6301 0000  eet.__init__c...
-00000240: 0000 0000 0000 0000 000e 0000 0009 0000  ................
-00000250: 0043 0000 0073 5e02 0000 7400 8300 7d01  .C...s^...t...}.
-00000260: 7401 6a02 a003 7401 6a02 a004 7401 a005  t.j...t.j...t...
-00000270: a100 6401 a102 a101 7d02 7401 6a02 a006  ..d.....}.t.j...
-00000280: 7c02 a101 7336 7401 a007 7c02 a101 0100  |...s6t...|.....
-00000290: 7401 6a02 a003 7401 6a02 a004 7401 a005  t.j...t.j...t...
-000002a0: a100 6402 a102 a101 7d03 7401 6a02 a003  ..d.....}.t.j...
-000002b0: 7401 6a02 a004 7401 a005 a100 6403 a102  t.j...t.....d...
-000002c0: a101 7d04 7401 6a02 a003 7401 6a02 a004  ..}.t.j...t.j...
-000002d0: 7401 a005 a100 6404 a102 a101 7d05 7408  t.....d.....}.t.
-000002e0: a009 7c00 a101 7d06 7401 6a02 a006 7c03  ..|...}.t.j...|.
-000002f0: a101 73d6 740a a00b 7401 6a02 a003 7401  ..s.t...t.j...t.
-00000300: 6a02 a004 7401 6a02 a00c 740d a101 6405  j...t.j...t...d.
-00000310: a102 a101 7401 6a02 a003 7401 6a02 a004  ....t.j...t.j...
-00000320: 7401 a005 a100 6401 a102 a101 a102 0100  t.....d.........
-00000330: 7401 6a02 a006 7c04 a101 9001 7320 740a  t.j...|.....s t.
-00000340: a00b 7401 6a02 a003 7401 6a02 a004 7401  ..t.j...t.j...t.
-00000350: 6a02 a00c 740d a101 6406 a102 a101 7401  j...t...d.....t.
-00000360: 6a02 a003 7401 6a02 a004 7401 a005 a100  j...t.j...t.....
-00000370: 6401 a102 a101 a102 0100 7401 6a02 a003  d.........t.j...
-00000380: 7401 6a02 a004 7401 a005 a100 6407 a102  t.j...t.....d...
-00000390: a101 7d07 7401 6a02 a006 7c07 a101 9001  ..}.t.j...|.....
-000003a0: 7366 740e 7c07 6408 8302 7d08 740f 6409  sft.|.d...}.t.d.
-000003b0: 7c08 640a 8d02 0100 7c08 a010 a100 0100  |.d.....|.......
-000003c0: 7411 a012 7c03 7c05 a102 0100 740e 7c05  t...|.|.....t.|.
-000003d0: 640b 8302 8f14 7d09 7c00 a013 7c09 a014  d.....}.|...|...
-000003e0: a100 a101 0100 5700 3500 5100 5200 5800  ......W.5.Q.R.X.
-000003f0: 7415 7c00 6a16 8301 7d0a 7c0a 6a17 6a18  t.|.j...}.|.j.j.
-00000400: a019 741a 6a1b a101 0100 7c0a 6a17 6a1c  ..t.j.....|.j.j.
-00000410: a019 7c00 6a1d a101 0100 7c0a 6a17 6a1e  ..|.j.....|.j.j.
-00000420: a019 7c00 6a1f a101 0100 7415 7c00 6a20  ..|.j.....t.|.j 
-00000430: 8301 7d0b 7c0b 6a17 6a18 a019 741a 6a1b  ..}.|.j.j...t.j.
-00000440: a101 0100 7c0b 6a17 6a1c a019 640c 640d  ....|.j.j...d.d.
-00000450: 8400 a101 0100 7c0b 6a17 6a1e a019 7c00  ......|.j.j...|.
-00000460: 6a1f a101 0100 7408 a021 7c00 a101 7d0c  j.....t..!|...}.
-00000470: 7422 7c0c 640e 1900 8301 7d0d 7c01 a023  t"|.d.....}.|..#
-00000480: 640f a101 7c0d 6b02 9002 734e 7c0c 640e  d...|.k...sN|.d.
-00000490: 1900 6400 6b09 9002 724e 7c00 6a24 a025  ..d.k...rN|.j$.%
-000004a0: 7c0a a101 0100 6e0c 7c00 6a24 a025 7c0b  |.....n.|.j$.%|.
-000004b0: a101 0100 6400 5300 2910 4e5a 0351 5353  ....d.S.).NZ.QSS
-000004c0: 7a0d 5153 532f 6d61 696e 2e73 6373 737a  z.QSS/main.scssz
-000004d0: 1051 5353 2f5f 7374 796c 6573 2e73 6373  .QSS/_styles.scs
-000004e0: 737a 0c51 5353 2f6d 6169 6e2e 6373 737a  sz.QSS/main.cssz
-000004f0: 096d 6169 6e2e 7363 7373 7a0c 5f73 7479  .main.scssz._sty
-00000500: 6c65 732e 7363 7373 7a15 5153 532f 6465  les.scssz.QSS/de
-00000510: 6661 756c 7453 7479 6c65 2e73 6373 73da  faultStyle.scss.
-00000520: 0177 61bf 0100 000a 2020 2020 2020 2020  .wa.....        
-00000530: 2020 2020 2f2f 3d3d 3d3d 3d3d 3d3d 3d3d      //==========
-00000540: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000550: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000560: 3d3d 3d3d 3d3d 3d3d 3d2f 2f0a 2020 2020  =========//.    
-00000570: 2020 2020 2020 2020 2f2f 2046 494c 4520          // FILE 
-00000580: 4155 544f 2d47 454e 4552 4154 4544 2e20  AUTO-GENERATED. 
-00000590: 5055 5420 594f 5552 2044 4546 4155 4c54  PUT YOUR DEFAULT
-000005a0: 2053 5459 4c45 5320 4845 5245 2e20 0a20   STYLES HERE. . 
-000005b0: 2020 2020 2020 2020 2020 202f 2f20 5448             // TH
-000005c0: 4553 4520 5354 594c 4553 2057 494c 4c20  ESE STYLES WILL 
-000005d0: 4f56 4552 4944 4520 5448 4520 5448 454d  OVERIDE THE THEM
-000005e0: 4520 5354 594c 4553 0a20 2020 2020 2020  E STYLES.       
-000005f0: 2020 2020 202f 2f3d 3d3d 3d3d 3d3d 3d3d       //=========
-00000600: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000610: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000620: 3d3d 3d3d 3d3d 3d3d 3d3d 3d2f 2f0a 2020  ===========//.  
-00000630: 2020 2020 2020 2020 2020 0a20 2020 2020            .     
-00000640: 2020 2020 2020 202f 2f3d 3d3d 3d3d 3d3d         //=======
-00000650: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000660: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000670: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 2f2f 0a20  ============//. 
-00000680: 2020 2020 2020 2020 2020 202f 2f20 454e             // EN
-00000690: 4420 2f2f 0a20 2020 2020 2020 2020 2020  D //.           
-000006a0: 202f 2f3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d   //=============
-000006b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000006c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000006d0: 3d3d 3d3d 3d3d 3d2f 2f0a 2020 2020 2020  =======//.      
-000006e0: 2020 2020 2020 2901 da04 6669 6c65 da01        )...file..
-000006f0: 7263 0000 0000 0000 0000 0000 0000 0000  rc..............
-00000700: 0000 0200 0000 5300 0000 7308 0000 0074  ......S...s....t
-00000710: 0064 0183 0153 0029 024e 7a38 616c 6c20  .d...S.).Nz8all 
-00000720: 6963 6f6e 7320 6861 7665 2062 6565 6e20  icons have been 
-00000730: 6368 6563 6b65 6420 616e 6420 6d69 7373  checked and miss
-00000740: 696e 6720 6963 6f6e 7320 6765 6e65 7261  ing icons genera
-00000750: 7465 6421 2901 da05 7072 696e 7472 1200  ted!)...printr..
-00000760: 0000 7212 0000 0072 1200 0000 7213 0000  ..r....r....r...
-00000770: 00da 083c 6c61 6d62 6461 3e62 0000 00f3  ...<lambda>b....
-00000780: 0000 0000 7a35 436f 6d70 696c 6553 7479  ....z5CompileSty
-00000790: 6c65 5368 6565 742e 6170 706c 7943 6f6d  leSheet.applyCom
-000007a0: 7069 6c65 6453 6173 732e 3c6c 6f63 616c  piledSass.<local
-000007b0: 733e 2e3c 6c61 6d62 6461 3e7a 0b69 636f  s>.<lambda>z.ico
-000007c0: 6e73 2d63 6f6c 6f72 7a0b 4943 4f4e 532d  ns-colorz.ICONS-
-000007d0: 434f 4c4f 5229 26da 0951 5365 7474 696e  COLOR)&..QSettin
-000007e0: 6773 da02 6f73 da04 7061 7468 da07 6162  gs..os..path..ab
-000007f0: 7370 6174 68da 046a 6f69 6eda 0667 6574  spath..join..get
-00000800: 6377 64da 0665 7869 7374 73da 086d 616b  cwd..exists..mak
-00000810: 6564 6972 7372 0400 0000 5a0f 4372 6561  edirsr....Z.Crea
-00000820: 7465 5661 7269 6162 6c65 73da 0673 6875  teVariables..shu
-00000830: 7469 6cda 0463 6f70 79da 0764 6972 6e61  til..copy..dirna
-00000840: 6d65 da08 5f5f 6669 6c65 5f5f da04 6f70  me..__file__..op
-00000850: 656e 7217 0000 00da 0563 6c6f 7365 da06  enr......close..
-00000860: 7174 7361 7373 5a10 636f 6d70 696c 655f  qtsassZ.compile_
-00000870: 6669 6c65 6e61 6d65 da0d 7365 7453 7479  filename..setSty
-00000880: 6c65 5368 6565 74da 0472 6561 6472 0900  leSheet..readr..
-00000890: 0000 da10 636f 6d70 696c 6553 6173 7354  ....compileSassT
-000008a0: 6865 6d65 5a07 7369 676e 616c 73da 0672  hemeZ.signals..r
-000008b0: 6573 756c 74da 0763 6f6e 6e65 6374 720a  esult..connectr.
-000008c0: 0000 005a 0c70 7269 6e74 5f6f 7574 7075  ...Z.print_outpu
-000008d0: 74da 0866 696e 6973 6865 64da 0772 6573  t..finished..res
-000008e0: 7461 7274 da08 7072 6f67 7265 7373 da17  tart..progress..
-000008f0: 7361 7373 436f 6d70 696c 6174 696f 6e50  sassCompilationP
-00000900: 726f 6772 6573 73da 0c6d 616b 6541 6c6c  rogress..makeAll
-00000910: 4963 6f6e 735a 1367 6574 4375 7272 656e  IconsZ.getCurren
-00000920: 7454 6865 6d65 496e 666f da03 7374 72da  tThemeInfo..str.
-00000930: 0576 616c 7565 da17 6375 7374 6f6d 5769  .value..customWi
-00000940: 6467 6574 7354 6872 6561 6470 6f6f 6cda  dgetsThreadpool.
-00000950: 0573 7461 7274 290e 720e 0000 00da 0873  .start).r......s
-00000960: 6574 7469 6e67 735a 0b71 6373 735f 666f  ettingsZ.qcss_fo
-00000970: 6c64 6572 5a0e 6d61 696e 5f73 6173 735f  lderZ.main_sass_
-00000980: 7061 7468 5a10 7374 796c 6573 5f73 6173  pathZ.styles_sas
-00000990: 735f 7061 7468 da08 6373 735f 7061 7468  s_path..css_path
-000009a0: 5a0d 7661 7269 6162 6c65 7346 696c 655a  Z.variablesFileZ
-000009b0: 1164 6566 6175 6c74 5f73 6373 735f 7061  .default_scss_pa
-000009c0: 7468 da01 66da 0363 7373 5a0b 6963 6f6e  th..f..cssZ.icon
-000009d0: 7357 6f72 6b65 725a 0e61 6c6c 4963 6f6e  sWorkerZ.allIcon
-000009e0: 7357 6f72 6b65 72da 0563 6f6c 6f72 5a0c  sWorker..colorZ.
-000009f0: 6e6f 726d 616c 5f63 6f6c 6f72 7212 0000  normal_colorr...
-00000a00: 0072 1200 0000 7213 0000 00da 1161 7070  .r....r......app
-00000a10: 6c79 436f 6d70 696c 6564 5361 7373 2d00  lyCompiledSass-.
-00000a20: 0000 7346 0000 0000 0106 021a 010c 010a  ..sF............
-00000a30: 021a 011a 011a 020a 020c 013c 020e 013c  ...........<...<
-00000a40: 021a 010e 010a 0104 0902 f706 0b08 020c  ................
-00000a50: 020c 0118 070a 0110 0110 0110 030a 0110  ................
-00000a60: 0112 0110 020a 010c 021e 020e 027a 2343  .............z#C
-00000a70: 6f6d 7069 6c65 5374 796c 6553 6865 6574  ompileStyleSheet
-00000a80: 2e61 7070 6c79 436f 6d70 696c 6564 5361  .applyCompiledSa
-00000a90: 7373 2901 4e29 06da 085f 5f6e 616d 655f  ss).N)...__name_
-00000aa0: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-00000ab0: 5f71 7561 6c6e 616d 655f 5f72 0d00 0000  _qualname__r....
-00000ac0: 723c 0000 00da 0d5f 5f63 6c61 7373 6365  r<.....__classce
-00000ad0: 6c6c 5f5f 7212 0000 0072 1200 0000 7210  ll__r....r....r.
-00000ae0: 0000 0072 1300 0000 720b 0000 0021 0000  ...r....r....!..
-00000af0: 0073 0400 0000 0801 0e0b 720b 0000 0029  .s........r....)
-00000b00: 12da 0e50 7953 6964 6532 2e51 7443 6f72  ...PySide2.QtCor
-00000b10: 65da 0d50 7953 6964 6532 2e51 7447 7569  e..PySide2.QtGui
-00000b20: da11 5079 5369 6465 322e 5174 5769 6467  ..PySide2.QtWidg
-00000b30: 6574 7372 2800 0000 721b 0000 0072 2200  etsr(...r....r".
-00000b40: 0000 5a0b 636f 6c6f 7273 7973 7465 6d72  ..Z.colorsystemr
-00000b50: 0400 0000 7205 0000 0072 0600 0000 5a0d  ....r....r....Z.
-00000b60: 5376 6754 6f50 6e67 4963 6f6e 7372 0700  SvgToPngIconsr..
-00000b70: 0000 da0d 5769 6467 6574 7357 6f72 6b65  ....WidgetsWorke
-00000b80: 7272 0900 0000 720a 0000 0072 1a00 0000  rr....r....r....
-00000b90: 7237 0000 0072 0b00 0000 7212 0000 0072  r7...r....r....r
-00000ba0: 1200 0000 7212 0000 0072 1300 0000 da08  ....r....r......
-00000bb0: 3c6d 6f64 756c 653e 0900 0000 7314 0000  <module>....s...
-00000bc0: 0008 0108 0108 0208 0308 0108 0214 010c  ................
-00000bd0: 0410 0206 07                             .....
+00000020: 0003 0000 0040 0000 0073 8000 0000 6400  .....@...s....d.
+00000030: 6401 6c00 5a00 6400 6402 6c01 5400 6400  d.l.Z.d.d.l.T.d.
+00000040: 6402 6c02 5400 6400 6402 6c03 5400 6400  d.l.T.d.d.l.T.d.
+00000050: 6401 6c04 5a04 6400 6401 6c05 5a05 6400  d.l.Z.d.d.l.Z.d.
+00000060: 6401 6c06 5a06 6403 6404 6c07 6d08 5a08  d.l.Z.d.d.l.m.Z.
+00000070: 6d09 5a09 6d0a 5a0a 0100 6403 6405 6c0b  m.Z.m.Z...d.d.l.
+00000080: 6d0c 5a0c 0100 6406 6407 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
+00000090: 6d0f 5a0f 0100 6510 8300 5a11 4700 6408  m.Z...e...Z.G.d.
+000000a0: 6409 8400 6409 8302 5a12 6401 5300 290a  d...d...Z.d.S.).
+000000b0: e900 0000 004e 2901 da01 2ae9 0100 0000  .....N)...*.....
+000000c0: 2903 da13 4372 6561 7465 436f 6c6f 7256  )...CreateColorV
+000000d0: 6172 6961 626c 65da 0444 6172 6bda 054c  ariable..Dark..L
+000000e0: 6967 6874 2901 da11 4e65 7749 636f 6e73  ight)...NewIcons
+000000f0: 4765 6e65 7261 746f 72e9 0200 0000 2902  Generator.....).
+00000100: da06 576f 726b 6572 da0e 576f 726b 6572  ..Worker..Worker
+00000110: 5265 7370 6f6e 7365 6300 0000 0000 0000  Responsec.......
+00000120: 0000 0000 0000 0000 0004 0000 0000 0000  ................
+00000130: 0073 2600 0000 6500 5a01 6400 5a02 6406  .s&...e.Z.d.Z.d.
+00000140: 8700 6601 6402 6403 8409 5a03 6404 6405  ..f.d.d...Z.d.d.
+00000150: 8400 5a04 8700 0400 5a05 5300 2907 da11  ..Z.....Z.S.)...
+00000160: 436f 6d70 696c 6553 7479 6c65 5368 6565  CompileStyleShee
+00000170: 744e 6302 0000 0000 0000 0000 0000 0002  tNc.............
+00000180: 0000 0003 0000 0003 0000 0073 1400 0000  ...........s....
+00000190: 7400 7401 7c00 8302 a002 7c01 a101 0100  t.t.|.....|.....
+000001a0: 6400 5300 2901 4e29 03da 0573 7570 6572  d.S.).N)...super
+000001b0: 720b 0000 00da 085f 5f69 6e69 745f 5f29  r......__init__)
+000001c0: 02da 0473 656c 66da 0670 6172 656e 74a9  ...self..parent.
+000001d0: 01da 095f 5f63 6c61 7373 5f5f a900 fa4d  ...__class__...M
+000001e0: 633a 5c75 7365 7273 5c6b 6962 6574 5c61  c:\users\kibet\a
+000001f0: 6e61 636f 6e64 6133 5c4c 6962 5c73 6974  naconda3\Lib\sit
+00000200: 652d 7061 636b 6167 6573 5c43 7573 746f  e-packages\Custo
+00000210: 6d5f 5769 6467 6574 732f 5173 732f 5361  m_Widgets/Qss/Sa
+00000220: 7373 436f 6d70 696c 6572 2e70 7972 0d00  ssCompiler.pyr..
+00000230: 0000 3500 0000 7302 0000 0000 017a 1a43  ..5...s......z.C
+00000240: 6f6d 7069 6c65 5374 796c 6553 6865 6574  ompileStyleSheet
+00000250: 2e5f 5f69 6e69 745f 5f63 0100 0000 0000  .__init__c......
+00000260: 0000 0000 0000 0e00 0000 0900 0000 4300  ..............C.
+00000270: 0000 7366 0200 0074 0083 007d 0174 016a  ..sf...t...}.t.j
+00000280: 02a0 0374 016a 02a0 0474 01a0 05a1 0064  ...t.j...t.....d
+00000290: 01a1 02a1 017d 0274 016a 02a0 067c 02a1  .....}.t.j...|..
+000002a0: 0173 3674 01a0 077c 02a1 0101 0074 016a  .s6t...|.....t.j
+000002b0: 02a0 0374 016a 02a0 0474 01a0 05a1 0064  ...t.j...t.....d
+000002c0: 02a1 02a1 017d 0374 016a 02a0 0374 016a  .....}.t.j...t.j
+000002d0: 02a0 0474 01a0 05a1 0064 03a1 02a1 017d  ...t.....d.....}
+000002e0: 0474 016a 02a0 0374 016a 02a0 0474 01a0  .t.j...t.j...t..
+000002f0: 05a1 0064 04a1 02a1 017d 0574 08a0 097c  ...d.....}.t...|
+00000300: 00a1 017d 0674 016a 02a0 067c 03a1 0173  ...}.t.j...|...s
+00000310: d674 0aa0 0b74 016a 02a0 0374 016a 02a0  .t...t.j...t.j..
+00000320: 0474 016a 02a0 0c74 0da1 0164 05a1 02a1  .t.j...t...d....
+00000330: 0174 016a 02a0 0374 016a 02a0 0474 01a0  .t.j...t.j...t..
+00000340: 05a1 0064 01a1 02a1 01a1 0201 0074 016a  ...d.........t.j
+00000350: 02a0 067c 04a1 0190 0173 2074 0aa0 0b74  ...|.....s t...t
+00000360: 016a 02a0 0374 016a 02a0 0474 016a 02a0  .j...t.j...t.j..
+00000370: 0c74 0da1 0164 06a1 02a1 0174 016a 02a0  .t...d.....t.j..
+00000380: 0374 016a 02a0 0474 01a0 05a1 0064 01a1  .t.j...t.....d..
+00000390: 02a1 01a1 0201 0074 016a 02a0 0374 016a  .......t.j...t.j
+000003a0: 02a0 0474 01a0 05a1 0064 07a1 02a1 017d  ...t.....d.....}
+000003b0: 0774 016a 02a0 067c 07a1 0190 0173 6674  .t.j...|.....sft
+000003c0: 0e7c 0764 0883 027d 0874 0f64 097c 0864  .|.d...}.t.d.|.d
+000003d0: 0a8d 0201 007c 08a0 10a1 0001 0074 11a0  .....|.......t..
+000003e0: 127c 037c 05a1 0201 0074 0e7c 0564 0b83  .|.|.....t.|.d..
+000003f0: 028f 147d 097c 00a0 137c 09a0 14a1 00a1  ...}.|...|......
+00000400: 0101 0057 0035 0051 0052 0058 0074 157c  ...W.5.Q.R.X.t.|
+00000410: 006a 1683 017d 0a7c 0a6a 176a 18a0 1974  .j...}.|.j.j...t
+00000420: 1a6a 1ba1 0101 007c 0a6a 176a 1ca0 197c  .j.....|.j.j...|
+00000430: 006a 1da1 0101 007c 0a6a 176a 1ea0 197c  .j.....|.j.j...|
+00000440: 006a 1fa1 0101 0074 157c 006a 2083 017d  .j.....t.|.j ..}
+00000450: 0b7c 0b6a 176a 18a0 1974 1a6a 1ba1 0101  .|.j.j...t.j....
+00000460: 007c 006a 2190 0272 047c 0b6a 176a 1ca0  .|.j!..r.|.j.j..
+00000470: 1964 0c64 0d84 00a1 0101 007c 0b6a 176a  .d.d.......|.j.j
+00000480: 1ea0 197c 006a 1fa1 0101 0074 08a0 227c  ...|.j.....t.."|
+00000490: 00a1 017d 0c74 237c 0c64 0e19 0083 017d  ...}.t#|.d.....}
+000004a0: 0d7c 01a0 2464 0fa1 017c 0d6b 0290 0273  .|..$d...|.k...s
+000004b0: 567c 0c64 0e19 0064 006b 0990 0272 567c  V|.d...d.k...rV|
+000004c0: 006a 25a0 267c 0aa1 0101 006e 0c7c 006a  .j%.&|.....n.|.j
+000004d0: 25a0 267c 0ba1 0101 0064 0053 0029 104e  %.&|.....d.S.).N
+000004e0: 5a03 5153 537a 0d51 5353 2f6d 6169 6e2e  Z.QSSz.QSS/main.
+000004f0: 7363 7373 7a10 5153 532f 5f73 7479 6c65  scssz.QSS/_style
+00000500: 732e 7363 7373 7a0c 5153 532f 6d61 696e  s.scssz.QSS/main
+00000510: 2e63 7373 7a09 6d61 696e 2e73 6373 737a  .cssz.main.scssz
+00000520: 0c5f 7374 796c 6573 2e73 6373 737a 1551  ._styles.scssz.Q
+00000530: 5353 2f64 6566 6175 6c74 5374 796c 652e  SS/defaultStyle.
+00000540: 7363 7373 da01 7761 bf01 0000 0a20 2020  scss..wa.....   
+00000550: 2020 2020 2020 2020 202f 2f3d 3d3d 3d3d           //=====
+00000560: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000570: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000580: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 2f2f  ==============//
+00000590: 0a20 2020 2020 2020 2020 2020 202f 2f20  .            // 
+000005a0: 4649 4c45 2041 5554 4f2d 4745 4e45 5241  FILE AUTO-GENERA
+000005b0: 5445 442e 2050 5554 2059 4f55 5220 4445  TED. PUT YOUR DE
+000005c0: 4641 554c 5420 5354 594c 4553 2048 4552  FAULT STYLES HER
+000005d0: 452e 200a 2020 2020 2020 2020 2020 2020  E. .            
+000005e0: 2f2f 2054 4845 5345 2053 5459 4c45 5320  // THESE STYLES 
+000005f0: 5749 4c4c 204f 5645 5249 4445 2054 4845  WILL OVERIDE THE
+00000600: 2054 4845 4d45 2053 5459 4c45 530a 2020   THEME STYLES.  
+00000610: 2020 2020 2020 2020 2020 2f2f 3d3d 3d3d            //====
+00000620: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000630: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000640: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000650: 2f2f 0a20 2020 2020 2020 2020 2020 200a  //.            .
+00000660: 2020 2020 2020 2020 2020 2020 2f2f 3d3d              //==
+00000670: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000680: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000690: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000006a0: 3d2f 2f0a 2020 2020 2020 2020 2020 2020  =//.            
+000006b0: 2f2f 2045 4e44 202f 2f0a 2020 2020 2020  // END //.      
+000006c0: 2020 2020 2020 2f2f 3d3d 3d3d 3d3d 3d3d        //========
+000006d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000006e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000006f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 2f2f 0a20  ============//. 
+00000700: 2020 2020 2020 2020 2020 2029 01da 0466             )...f
+00000710: 696c 65da 0172 6300 0000 0000 0000 0000  ile..rc.........
+00000720: 0000 0000 0000 0002 0000 0053 0000 0073  ...........S...s
+00000730: 0800 0000 7400 6401 8301 5300 2902 4e7a  ....t.d...S.).Nz
+00000740: 3861 6c6c 2069 636f 6e73 2068 6176 6520  8all icons have 
+00000750: 6265 656e 2063 6865 636b 6564 2061 6e64  been checked and
+00000760: 206d 6973 7369 6e67 2069 636f 6e73 2067   missing icons g
+00000770: 656e 6572 6174 6564 2129 01da 0570 7269  enerated!)...pri
+00000780: 6e74 7212 0000 0072 1200 0000 7212 0000  ntr....r....r...
+00000790: 0072 1300 0000 da08 3c6c 616d 6264 613e  .r......<lambda>
+000007a0: 7600 0000 f300 0000 007a 3543 6f6d 7069  v........z5Compi
+000007b0: 6c65 5374 796c 6553 6865 6574 2e61 7070  leStyleSheet.app
+000007c0: 6c79 436f 6d70 696c 6564 5361 7373 2e3c  lyCompiledSass.<
+000007d0: 6c6f 6361 6c73 3e2e 3c6c 616d 6264 613e  locals>.<lambda>
+000007e0: 7a0b 6963 6f6e 732d 636f 6c6f 727a 0b49  z.icons-colorz.I
+000007f0: 434f 4e53 2d43 4f4c 4f52 2927 da09 5153  CONS-COLOR)'..QS
+00000800: 6574 7469 6e67 73da 026f 73da 0470 6174  ettings..os..pat
+00000810: 68da 0761 6273 7061 7468 da04 6a6f 696e  h..abspath..join
+00000820: da06 6765 7463 7764 da06 6578 6973 7473  ..getcwd..exists
+00000830: da08 6d61 6b65 6469 7273 7204 0000 005a  ..makedirsr....Z
+00000840: 0f43 7265 6174 6556 6172 6961 626c 6573  .CreateVariables
+00000850: da06 7368 7574 696c da04 636f 7079 da07  ..shutil..copy..
+00000860: 6469 726e 616d 65da 085f 5f66 696c 655f  dirname..__file_
+00000870: 5fda 046f 7065 6e72 1700 0000 da05 636c  _..openr......cl
+00000880: 6f73 65da 0671 7473 6173 735a 1063 6f6d  ose..qtsassZ.com
+00000890: 7069 6c65 5f66 696c 656e 616d 655a 0d73  pile_filenameZ.s
+000008a0: 6574 5374 796c 6553 6865 6574 da04 7265  etStyleSheet..re
+000008b0: 6164 7209 0000 005a 1063 6f6d 7069 6c65  adr....Z.compile
+000008c0: 5361 7373 5468 656d 655a 0773 6967 6e61  SassThemeZ.signa
+000008d0: 6c73 da06 7265 7375 6c74 da07 636f 6e6e  ls..result..conn
+000008e0: 6563 7472 0a00 0000 5a0c 7072 696e 745f  ectr....Z.print_
+000008f0: 6f75 7470 7574 da08 6669 6e69 7368 6564  output..finished
+00000900: 5a07 7265 7374 6172 74da 0870 726f 6772  Z.restart..progr
+00000910: 6573 735a 1773 6173 7343 6f6d 7069 6c61  essZ.sassCompila
+00000920: 7469 6f6e 5072 6f67 7265 7373 5a0c 6d61  tionProgressZ.ma
+00000930: 6b65 416c 6c49 636f 6e73 5a15 7368 6f77  keAllIconsZ.show
+00000940: 4375 7374 6f6d 5769 6467 6574 734c 6f67  CustomWidgetsLog
+00000950: 735a 1367 6574 4375 7272 656e 7454 6865  sZ.getCurrentThe
+00000960: 6d65 496e 666f da03 7374 72da 0576 616c  meInfo..str..val
+00000970: 7565 5a17 6375 7374 6f6d 5769 6467 6574  ueZ.customWidget
+00000980: 7354 6872 6561 6470 6f6f 6cda 0573 7461  sThreadpool..sta
+00000990: 7274 290e 720e 0000 00da 0873 6574 7469  rt).r......setti
+000009a0: 6e67 735a 0b71 6373 735f 666f 6c64 6572  ngsZ.qcss_folder
+000009b0: 5a0e 6d61 696e 5f73 6173 735f 7061 7468  Z.main_sass_path
+000009c0: 5a10 7374 796c 6573 5f73 6173 735f 7061  Z.styles_sass_pa
+000009d0: 7468 5a08 6373 735f 7061 7468 5a0d 7661  thZ.css_pathZ.va
+000009e0: 7269 6162 6c65 7346 696c 655a 1164 6566  riablesFileZ.def
+000009f0: 6175 6c74 5f73 6373 735f 7061 7468 da01  ault_scss_path..
+00000a00: 66da 0363 7373 5a0b 6963 6f6e 7357 6f72  f..cssZ.iconsWor
+00000a10: 6b65 725a 0e61 6c6c 4963 6f6e 7357 6f72  kerZ.allIconsWor
+00000a20: 6b65 72da 0563 6f6c 6f72 5a0c 6e6f 726d  ker..colorZ.norm
+00000a30: 616c 5f63 6f6c 6f72 7212 0000 0072 1200  al_colorr....r..
+00000a40: 0000 7213 0000 00da 1161 7070 6c79 436f  ..r......applyCo
+00000a50: 6d70 696c 6564 5361 7373 4000 0000 7348  mpiledSass@...sH
+00000a60: 0000 0000 0106 021a 010c 010a 021a 011a  ................
+00000a70: 011a 020a 020c 013c 020e 013c 021a 010e  .......<...<....
+00000a80: 010a 0104 0902 f706 0b08 020c 020c 0118  ................
+00000a90: 070a 0110 0110 0110 030a 0110 0108 0112  ................
+00000aa0: 0110 020a 010c 011e 020e 027a 2343 6f6d  ...........z#Com
+00000ab0: 7069 6c65 5374 796c 6553 6865 6574 2e61  pileStyleSheet.a
+00000ac0: 7070 6c79 436f 6d70 696c 6564 5361 7373  pplyCompiledSass
+00000ad0: 2901 4e29 06da 085f 5f6e 616d 655f 5fda  ).N)...__name__.
+00000ae0: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+00000af0: 7561 6c6e 616d 655f 5f72 0d00 0000 7235  ualname__r....r5
+00000b00: 0000 00da 0d5f 5f63 6c61 7373 6365 6c6c  .....__classcell
+00000b10: 5f5f 7212 0000 0072 1200 0000 7210 0000  __r....r....r...
+00000b20: 0072 1300 0000 720b 0000 0034 0000 0073  .r....r....4...s
+00000b30: 0400 0000 0801 0e0b 720b 0000 0029 13da  ........r....)..
+00000b40: 0373 7973 5a0b 7174 7079 2e51 7443 6f72  .sysZ.qtpy.QtCor
+00000b50: 655a 0a71 7470 792e 5174 4775 695a 0e71  eZ.qtpy.QtGuiZ.q
+00000b60: 7470 792e 5174 5769 6467 6574 7372 2800  tpy.QtWidgetsr(.
+00000b70: 0000 721b 0000 0072 2200 0000 5a0b 636f  ..r....r"...Z.co
+00000b80: 6c6f 7273 7973 7465 6d72 0400 0000 7205  lorsystemr....r.
+00000b90: 0000 0072 0600 0000 5a0d 5376 6754 6f50  ...r....Z.SvgToP
+00000ba0: 6e67 4963 6f6e 7372 0700 0000 5a0d 5769  ngIconsr....Z.Wi
+00000bb0: 6467 6574 7357 6f72 6b65 7272 0900 0000  dgetsWorkerr....
+00000bc0: 720a 0000 0072 1a00 0000 7231 0000 0072  r....r....r1...r
+00000bd0: 0b00 0000 7212 0000 0072 1200 0000 7212  ....r....r....r.
+00000be0: 0000 0072 1300 0000 da08 3c6d 6f64 756c  ...r......<modul
+00000bf0: 653e 0800 0000 7316 0000 0008 1208 0108  e>....s.........
+00000c00: 0108 0408 0308 0108 0214 010c 0410 0206  ................
+00000c10: 07                                       .
```

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/__pycache__/SvgToPngIcons.cpython-310.pyc` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/SvgToPngIcons.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/__pycache__/SvgToPngIcons.cpython-38.pyc` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/SvgToPngIcons.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon Mar 14 10:11:12 2022 UTC, .py size: 14374 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c014 2f62 2638 0000  U........./b&8..
+00000000: 550d 0d0a 0000 0000 6a61 9364 1739 0000  U.......ja.d.9..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 6800 0000 6400  .....@...sh...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6402 6c05 6d06 5a06  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6400 6403 6c07 6d08 5a08 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6401 6c09 5a09 6404 6405 6c0a 5400 650b  d.l.Z.d.d.l.T.e.
@@ -21,388 +21,398 @@
 00000140: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
 00000150: 0003 0000 0003 0000 0073 1800 0000 7400  .........s....t.
 00000160: 7401 7c00 8302 a002 a100 0100 7c01 7c00  t.|.........|.|.
 00000170: 5f03 6400 5300 2901 4e29 04da 0573 7570  _.d.S.).N)...sup
 00000180: 6572 7206 0000 00da 085f 5f69 6e69 745f  err......__init_
 00000190: 5fda 0361 7267 2902 da04 7365 6c66 7209  _..arg)...selfr.
 000001a0: 0000 00a9 01da 095f 5f63 6c61 7373 5f5f  .......__class__
-000001b0: a900 fa39 453a 5c53 7069 6e6e 2054 5620  ...9E:\Spinn TV 
-000001c0: 5475 745c 3232 2d55 495c 4375 7374 6f6d  Tut\22-UI\Custom
-000001d0: 5f57 6964 6765 7473 5c51 7373 5c53 7667  _Widgets\Qss\Svg
-000001e0: 546f 506e 6749 636f 6e73 2e70 7972 0800  ToPngIcons.pyr..
-000001f0: 0000 1100 0000 7304 0000 0000 010e 017a  ......s........z
-00000200: 1a4e 6577 4963 6f6e 7347 656e 6572 6174  .NewIconsGenerat
-00000210: 6f72 2e5f 5f69 6e69 745f 5f63 0200 0000  or.__init__c....
-00000220: 0000 0000 0000 0000 2300 0000 0c00 0000  ........#.......
-00000230: 4300 0000 73fe 0600 0074 0083 007d 0274  C...s....t...}.t
-00000240: 016a 02a0 0374 04a1 017d 0374 016a 02a0  .j...t...}.t.j..
-00000250: 057c 0364 01a1 027d 0467 007d 0574 06a0  .|.d...}.g.}.t..
-00000260: 077c 00a1 017d 0664 027d 0774 087c 0664  .|...}.d.}.t.|.d
-00000270: 0319 0083 017d 0874 097c 0864 0483 027d  .....}.t.|.d...}
-00000280: 0974 097c 0864 0583 027d 0a7c 08a0 0a64  .t.|.d...}.|...d
-00000290: 0664 07a1 027d 0b74 016a 02a0 0b74 016a  .d...}.t.j...t.j
-000002a0: 02a0 0574 01a0 0ca1 0064 087c 0b17 00a1  ...t.....d.|....
-000002b0: 02a1 017d 0c74 016a 02a0 0b74 016a 02a0  ...}.t.j...t.j..
-000002c0: 0574 01a0 0ca1 0064 09a1 02a1 017d 0d7c  .t.....d.....}.|
-000002d0: 02a0 0d64 0aa1 0164 006b 0872 da74 06a0  ...d...d.k.r.t..
-000002e0: 077c 00a1 017d 0e74 016a 02a0 0b74 016a  .|...}.t.j...t.j
-000002f0: 02a0 0574 01a0 0ca1 0064 087c 0e64 0319  ...t.....d.|.d..
-00000300: 00a0 0a64 0664 07a1 0217 00a1 02a1 017d  ...d.d.........}
-00000310: 0f6e 2c74 016a 02a0 0b74 016a 02a0 0574  .n,t.j...t.j...t
-00000320: 01a0 0ca1 0064 087c 02a0 0d64 0aa1 01a0  .....d.|...d....
-00000330: 0a64 0664 07a1 0217 00a1 02a1 017d 0f7c  .d.d.........}.|
-00000340: 02a0 0d64 0aa1 017c 086b 0290 0673 ee7c  ...d...|.k...s.|
-00000350: 0664 0319 0064 006b 0990 0672 ee74 0e64  .d...d.k...r.t.d
-00000360: 0b7c 02a0 0d64 0aa1 0164 0c7c 0883 0401  .|...d...d.|....
-00000370: 0074 0e64 0d83 0101 0074 01a0 0f7c 04a1  .t.d.....t...|..
-00000380: 0144 005d 2c5c 037d 107d 117d 127c 1244  .D.],\.}.}.}.|.D
-00000390: 005d 1a7d 137c 05a0 1074 016a 02a0 057c  .].}.|...t.j...|
-000003a0: 107c 13a1 02a1 0101 0090 0171 5890 0171  .|.........qX..q
-000003b0: 4a74 117c 0583 017d 147c 0544 0090 015d  Jt.|...}.|.D...]
-000003c0: 267d 1574 016a 02a0 1274 137c 1583 016a  &}.t.j...t.|...j
-000003d0: 02a1 01a0 0a64 0e64 0fa1 027d 1674 016a  .....d.d...}.t.j
-000003e0: 02a0 1474 016a 02a0 057c 0d7c 16a1 02a1  ...t.j...|.|....
-000003f0: 0190 0172 ea74 016a 02a0 1474 016a 02a0  ...r.t.j...t.j..
-00000400: 057c 0f7c 16a1 02a1 0190 0173 ea74 15a0  .|.|.......s.t..
-00000410: 1674 016a 02a0 057c 0d7c 16a1 027c 0fa1  .t.j...|.|...|..
-00000420: 0201 0074 016a 02a0 1274 137c 1583 016a  ...t.j...t.|...j
-00000430: 02a1 01a0 0a64 0e64 10a1 027d 1674 016a  .....d.d...}.t.j
-00000440: 02a0 1474 016a 02a0 057c 0d7c 16a1 02a1  ...t.j...|.|....
-00000450: 0190 0272 4a74 016a 02a0 1474 016a 02a0  ...rJt.j...t.j..
-00000460: 057c 0f7c 16a1 02a1 0190 0273 4a74 15a0  .|.|.......sJt..
-00000470: 1674 016a 02a0 057c 0d7c 16a1 027c 0fa1  .t.j...|.|...|..
-00000480: 0201 0074 016a 02a0 1274 137c 1583 016a  ...t.j...t.|...j
-00000490: 02a1 01a0 0a64 0e64 11a1 027d 1674 016a  .....d.d...}.t.j
-000004a0: 02a0 1474 016a 02a0 057c 0d7c 16a1 02a1  ...t.j...|.|....
-000004b0: 0190 0172 8474 016a 02a0 1474 016a 02a0  ...r.t.j...t.j..
-000004c0: 057c 0f7c 16a1 02a1 0190 0173 8474 15a0  .|.|.......s.t..
-000004d0: 1674 016a 02a0 057c 0d7c 16a1 027c 0fa1  .t.j...|.|...|..
-000004e0: 0201 0090 0171 847c 0544 0090 025d 927d  .....q.|.D...].}
-000004f0: 1574 176a 187c 1564 1264 1364 148d 038f  .t.j.|.d.d.d....
-00000500: ba7d 177c 17a0 19a1 007d 187c 18a0 0a7c  .}.|.....}.|...|
-00000510: 077c 08a1 027d 1974 08a0 1a7c 19a1 017d  .|...}.t...|...}
-00000520: 1a74 016a 02a0 1274 137c 1583 016a 02a1  .t.j...t.|...j..
-00000530: 01a0 0a64 0e64 0fa1 027d 1674 016a 02a0  ...d.d...}.t.j..
-00000540: 0b74 016a 02a0 057c 0c7c 16a1 02a1 017d  .t.j...|.|.....}
-00000550: 0474 016a 02a0 147c 0ca1 0190 0373 3074  .t.j...|.....s0t
-00000560: 01a0 1b7c 0ca1 0101 0074 016a 02a0 147c  ...|.....t.j...|
-00000570: 04a1 0190 0373 7e7a 1274 1c6a 1d7c 1a7c  .....s~z.t.j.|.|
-00000580: 0464 158d 0201 0057 006e 2c04 0074 1e6b  .d.....W.n,..t.k
-00000590: 0a90 0372 7c01 007d 1b01 007a 0c74 0e7c  ...r|..}...z.t.|
-000005a0: 1b83 0101 0057 0035 0064 007d 1b7e 1b58  .....W.5.d.}.~.X
-000005b0: 0059 006e 0258 0057 0035 0051 0052 0058  .Y.n.X.W.5.Q.R.X
-000005c0: 0074 176a 187c 1564 1264 1364 148d 038f  .t.j.|.d.d.d....
-000005d0: ba7d 177c 17a0 19a1 007d 187c 18a0 0a7c  .}.|.....}.|...|
-000005e0: 077c 09a1 027d 1974 08a0 1a7c 19a1 017d  .|...}.t...|...}
-000005f0: 1a74 016a 02a0 1274 137c 1583 016a 02a1  .t.j...t.|...j..
-00000600: 01a0 0a64 0e64 10a1 027d 1674 016a 02a0  ...d.d...}.t.j..
-00000610: 0b74 016a 02a0 057c 0c7c 16a1 02a1 017d  .t.j...|.|.....}
-00000620: 0474 016a 02a0 147c 0ca1 0190 0473 0074  .t.j...|.....s.t
-00000630: 01a0 1b7c 0ca1 0101 0074 016a 02a0 147c  ...|.....t.j...|
-00000640: 04a1 0190 0473 4e7a 1274 1c6a 1d7c 1a7c  .....sNz.t.j.|.|
-00000650: 0464 158d 0201 0057 006e 2c04 0074 1e6b  .d.....W.n,..t.k
-00000660: 0a90 0472 4c01 007d 1b01 007a 0c74 0e7c  ...rL..}...z.t.|
-00000670: 1b83 0101 0057 0035 0064 007d 1b7e 1b58  .....W.5.d.}.~.X
-00000680: 0059 006e 0258 0057 0035 0051 0052 0058  .Y.n.X.W.5.Q.R.X
-00000690: 0074 176a 187c 1564 1264 1364 148d 038f  .t.j.|.d.d.d....
-000006a0: ba7d 177c 17a0 19a1 007d 187c 18a0 0a7c  .}.|.....}.|...|
-000006b0: 077c 0aa1 027d 1974 08a0 1a7c 19a1 017d  .|...}.t...|...}
-000006c0: 1a74 016a 02a0 1274 137c 1583 016a 02a1  .t.j...t.|...j..
-000006d0: 01a0 0a64 0e64 11a1 027d 1674 016a 02a0  ...d.d...}.t.j..
-000006e0: 0b74 016a 02a0 057c 0c7c 16a1 02a1 017d  .t.j...|.|.....}
-000006f0: 0474 016a 02a0 147c 0ca1 0190 0473 d074  .t.j...|.....s.t
-00000700: 01a0 1b7c 0ca1 0101 0074 016a 02a0 147c  ...|.....t.j...|
-00000710: 04a1 0190 0573 1e7a 1274 1c6a 1d7c 1a7c  .....s.z.t.j.|.|
-00000720: 0464 158d 0201 0057 006e 2c04 0074 1e6b  .d.....W.n,..t.k
-00000730: 0a90 0572 1c01 007d 1b01 007a 0c74 0e7c  ...r...}...z.t.|
-00000740: 1b83 0101 0057 0035 0064 007d 1b7e 1b58  .....W.5.d.}.~.X
-00000750: 0059 006e 0258 0057 0035 0051 0052 0058  .Y.n.X.W.5.Q.R.X
-00000760: 007c 01a0 1f74 207c 05a0 217c 15a1 017c  .|...t |..!|...|
-00000770: 141b 0064 1614 0083 01a1 0101 0090 0271  ...d...........q
-00000780: b27c 0c7d 1c7c 0d7d 1d74 01a0 227c 1ca1  .|.}.|.}.t.."|..
-00000790: 017d 1e74 016a 02a0 147c 0da1 0190 0573  .}.t.j...|.....s
-000007a0: 7474 01a0 1b7c 0da1 0101 006e 1874 016a  tt...|.....n.t.j
-000007b0: 02a0 147c 0da1 0190 0573 8c74 01a0 1b7c  ...|.....s.t...|
-000007c0: 0da1 0101 0064 177d 1f7c 1e44 005d 5e7d  .....d.}.|.D.]^}
-000007d0: 2074 016a 2364 186b 0290 0572 bc74 15a0   t.j#d.k...r.t..
-000007e0: 2474 016a 02a0 057c 1c7c 20a1 027c 1da1  $t.j...|.| ..|..
-000007f0: 0201 006e 1674 15a0 1674 016a 02a0 057c  ...n.t...t.j...|
-00000800: 1c7c 20a1 027c 1da1 0201 007c 1f64 1937  .| ..|.....|.d.7
-00000810: 007d 1f7c 01a0 1f74 207c 1f7c 141b 0064  .}.|...t |.|...d
-00000820: 1614 0083 01a1 0101 0090 0571 9474 016a  ...........q.t.j
-00000830: 02a0 0b74 016a 02a0 0574 01a0 0ca1 0064  ...t.j...t.....d
-00000840: 1aa1 02a1 017d 2174 016a 02a0 147c 21a1  .....}!t.j...|!.
-00000850: 0190 0673 5874 15a0 2474 016a 02a0 0b74  ...sXt..$t.j...t
-00000860: 016a 02a0 0574 016a 02a0 0374 04a1 0164  .j...t.j...t...d
-00000870: 1ba1 02a1 0174 016a 02a0 0b74 016a 02a0  .....t.j...t.j..
-00000880: 0574 01a0 0ca1 0064 1ca1 02a1 01a1 0201  .t.....d........
-00000890: 007c 21a0 0a64 1d64 1ea1 027d 227c 22a0  .|!..d.d...}"|".
-000008a0: 0a64 0864 07a1 027d 227c 22a0 0a64 1f64  .d.d...}"|"..d.d
-000008b0: 07a1 027d 227c 22a0 0a64 2064 21a1 027d  ...}"|"..d d!..}
-000008c0: 227a 367c 02a0 2564 0a7c 08a1 0201 0074  "z6|..%d.|.....t
-000008d0: 01a0 2664 227c 2117 0064 2317 007c 2217  ..&d"|!..d#..|".
-000008e0: 0064 2417 00a1 0101 007c 02a0 2564 0a7c  .d$......|..%d.|
-000008f0: 08a1 0201 0057 006e 2c04 0074 1e6b 0a90  .....W.n,..t.k..
-00000900: 0672 ea01 007d 1b01 007a 0c74 0e64 2583  .r...}...z.t.d%.
-00000910: 0101 0057 0035 0064 007d 1b7e 1b58 0059  ...W.5.d.}.~.X.Y
-00000920: 006e 0258 006e 0c74 27a0 287c 007c 01a1  .n.X.n.t'.(|.|..
-00000930: 0201 0064 0053 0029 264e fa12 6963 6f6e  ...d.S.)&N..icon
-00000940: 732f 6f72 6967 696e 616c 5f73 7667 fa04  s/original_svg..
-00000950: 2366 6666 7a0b 6963 6f6e 732d 636f 6c6f  #fffz.icons-colo
-00000960: 72e7 0000 0000 0000 f83f e700 0000 0000  r........?......
-00000970: 00e0 3ffa 0123 da00 fa04 5153 532f fa09  ..?..#....QSS/..
-00000980: 5153 532f 4963 6f6e 73fa 0b49 434f 4e53  QSS/Icons..ICONS
-00000990: 2d43 4f4c 4f52 7a14 4375 7272 656e 7420  -COLORz.Current 
-000009a0: 6963 6f6e 7320 636f 6c6f 7220 7a0f 4e65  icons color z.Ne
-000009b0: 7720 6963 6f6e 7320 636f 6c6f 727a 4047  w icons colorz@G
-000009c0: 656e 6572 6174 696e 6720 6963 6f6e 7320  enerating icons 
-000009d0: 666f 7220 796f 7572 2074 6865 6d65 2c20  for your theme, 
-000009e0: 706c 6561 7365 2077 6169 742e 2054 6869  please wait. Thi
-000009f0: 7320 6d61 7920 7461 6b65 206c 6f6e 67fa  s may take long.
-00000a00: 042e 7376 67fa 042e 706e 67fa 0a5f 666f  ..svg...png.._fo
-00000a10: 6375 732e 706e 67fa 0d5f 6469 7361 626c  cus.png.._disabl
-00000a20: 6564 2e70 6e67 fa05 7574 662d 38da 0669  ed.png..utf-8..i
-00000a30: 676e 6f72 65a9 02da 0865 6e63 6f64 696e  gnore....encodin
-00000a40: 67da 0665 7272 6f72 73a9 025a 0a62 7974  g..errors..Z.byt
-00000a50: 6573 7472 696e 675a 0877 7269 7465 5f74  estringZ.write_t
-00000a60: 6fe9 6400 0000 7201 0000 00da 026e 7472  o.d...r......ntr
-00000a70: 0400 0000 7a15 5153 532f 5153 535f 5265  ....z.QSS/QSS_Re
-00000a80: 736f 7572 6365 732e 7172 637a 1151 5353  sources.qrcz.QSS
-00000a90: 5f52 6573 6f75 7263 6573 2e71 7263 da03  _Resources.qrc..
-00000aa0: 5153 537a 042e 7172 637a 032e 7079 7a04  QSSz..qrcz..pyz.
-00000ab0: 5153 535c 5a0d 5153 535f 5265 736f 7572  QSS\Z.QSS_Resour
-00000ac0: 6365 73da 1051 5353 5f52 6573 6f75 7263  ces..QSS_Resourc
-00000ad0: 6573 5f72 637a 0870 7972 6363 3520 227a  es_rcz.pyrcc5 "z
-00000ae0: 0622 202d 6f20 22fa 0122 7a24 6572 726f  ." -o ".."z$erro
-00000af0: 7220 7768 696c 6520 636f 6e76 6572 7469  r while converti
-00000b00: 6e67 2072 6573 6f75 7263 6520 6669 6c65  ng resource file
-00000b10: 2929 da09 5153 6574 7469 6e67 73da 026f  ))..QSettings..o
-00000b20: 73da 0470 6174 68da 0764 6972 6e61 6d65  s..path..dirname
-00000b30: da08 5f5f 6669 6c65 5f5f da04 6a6f 696e  ..__file__..join
-00000b40: da13 4372 6561 7465 436f 6c6f 7256 6172  ..CreateColorVar
-00000b50: 6961 626c 65da 1367 6574 4375 7272 656e  iable..getCurren
-00000b60: 7454 6865 6d65 496e 666f da03 7374 72da  tThemeInfo..str.
-00000b70: 1061 646a 7573 745f 6c69 6768 746e 6573  .adjust_lightnes
-00000b80: 73da 0772 6570 6c61 6365 da07 6162 7370  s..replace..absp
-00000b90: 6174 68da 0667 6574 6377 64da 0576 616c  ath..getcwd..val
-00000ba0: 7565 da05 7072 696e 74da 0477 616c 6bda  ue..print..walk.
-00000bb0: 0661 7070 656e 64da 036c 656e da08 6261  .append..len..ba
-00000bc0: 7365 6e61 6d65 7202 0000 00da 0665 7869  senamer......exi
-00000bd0: 7374 73da 0673 6875 7469 6cda 046d 6f76  sts..shutil..mov
-00000be0: 65da 0663 6f64 6563 73da 046f 7065 6eda  e..codecs..open.
-00000bf0: 0472 6561 64da 0665 6e63 6f64 65da 086d  .read..encode..m
-00000c00: 616b 6564 6972 73da 0863 6169 726f 7376  akedirs..cairosv
-00000c10: 67da 0773 7667 3270 6e67 da09 4578 6365  g..svg2png..Exce
-00000c20: 7074 696f 6eda 0465 6d69 74da 0369 6e74  ption..emit..int
-00000c30: da05 696e 6465 78da 076c 6973 7464 6972  ..index..listdir
-00000c40: da04 6e61 6d65 da04 636f 7079 da08 7365  ..name..copy..se
-00000c50: 7456 616c 7565 da06 7379 7374 656d 7206  tValue..systemr.
-00000c60: 0000 00da 1067 656e 6572 6174 6541 6c6c  .....generateAll
-00000c70: 4963 6f6e 7329 2372 0a00 0000 da11 7072  Icons)#r......pr
-00000c80: 6f67 7265 7373 5f63 616c 6c62 6163 6bda  ogress_callback.
-00000c90: 0873 6574 7469 6e67 7372 2a00 0000 da08  .settingsr*.....
-00000ca0: 6669 6c65 6e61 6d65 da0d 6c69 7374 5f6f  filename..list_o
-00000cb0: 665f 6669 6c65 73da 0563 6f6c 6f72 da09  f_files..color..
-00000cc0: 7376 675f 636f 6c6f 72da 0c6e 6f72 6d61  svg_color..norma
-00000cd0: 6c5f 636f 6c6f 72da 0d66 6f63 7573 6564  l_color..focused
-00000ce0: 5f63 6f6c 6f72 da0e 6469 7361 626c 6564  _color..disabled
-00000cf0: 5f63 6f6c 6f72 da0f 6963 6f6e 7346 6f6c  _color..iconsFol
-00000d00: 6465 724e 616d 65da 0b69 636f 6e73 466f  derName..iconsFo
-00000d10: 6c64 6572 da0e 6f6c 6449 636f 6e73 466f  lder..oldIconsFo
-00000d20: 6c64 6572 da0d 7661 7269 6162 6c65 7346  lder..variablesF
-00000d30: 696c 655a 196f 6c64 4963 6f6e 7344 6573  ileZ.oldIconsDes
-00000d40: 7469 6e61 7469 6f6e 466f 6c64 6572 da04  tinationFolder..
-00000d50: 726f 6f74 da04 6469 7273 da05 6669 6c65  root..dirs..file
-00000d60: 73da 0466 696c 65da 0a74 6f74 616c 4963  s..file..totalIc
-00000d70: 6f6e 7372 4900 0000 da06 6e61 6d65 5f32  onsrI.....name_2
-00000d80: da01 66da 0763 6f6e 7465 6e74 da06 6e65  ..f..content..ne
-00000d90: 7753 5647 da08 6e65 7742 7974 6573 da01  wSVG..newBytes..
-00000da0: 655a 0a73 6f75 7263 655f 6469 725a 0a74  eZ.source_dirZ.t
-00000db0: 6172 6765 745f 6469 725a 0a66 696c 655f  arget_dirZ.file_
-00000dc0: 6e61 6d65 735a 0a66 696c 6573 4d6f 7665  namesZ.filesMove
-00000dd0: 64da 0966 696c 655f 6e61 6d65 da0d 7265  d..file_name..re
-00000de0: 736f 7572 6365 5f70 6174 685a 1070 795f  source_pathZ.py_
-00000df0: 7265 736f 7572 6365 5f70 6174 6872 0d00  resource_pathr..
-00000e00: 0000 720d 0000 0072 0e00 0000 da10 6765  ..r....r......ge
-00000e10: 6e65 7261 7465 4e65 7749 636f 6e73 1500  nerateNewIcons..
-00000e20: 0000 73cc 0000 0000 0106 020c 010e 0104  ..s.............
-00000e30: 020a 0104 010c 020a 010a 020c 011e 021a  ................
-00000e40: 020e 010a 012c 022c 021e 0114 0108 0214  .....,.,........
-00000e50: 0108 011c 0208 020a 021a 0130 0116 021a  ...........0....
-00000e60: 0130 0116 021a 0130 011a 030a 0212 0108  .0.....0........
-00000e70: 020c 010a 021a 0116 020e 010a 020e 0102  ................
-00000e80: 0212 0112 0124 0312 0108 020c 010a 021a  .....$..........
-00000e90: 0116 020e 010a 020e 0102 0212 0112 0124  ...............$
-00000ea0: 0312 0108 020c 010a 021a 0116 020e 010a  ................
-00000eb0: 020e 0102 0212 0112 0124 0420 0304 0104  .........$. ....
-00000ec0: 020a 020e 010c 020e 010a 0204 0108 010c  ................
-00000ed0: 0118 0216 0208 021a 041a 010e 013c 010c  .............<..
-00000ee0: 010c 010c 010c 0202 010c 011a 0110 0112  ................
-00000ef0: 021c 037a 224e 6577 4963 6f6e 7347 656e  ...z"NewIconsGen
-00000f00: 6572 6174 6f72 2e67 656e 6572 6174 654e  erator.generateN
-00000f10: 6577 4963 6f6e 7363 0200 0000 0000 0000  ewIconsc........
-00000f20: 0000 0000 1c00 0000 0d00 0000 4300 0000  ............C...
-00000f30: 73a6 0500 0074 0083 007d 0274 016a 02a0  s....t...}.t.j..
-00000f40: 0374 04a1 017d 0374 016a 02a0 057c 0364  .t...}.t.j...|.d
-00000f50: 01a1 027d 0467 007d 0564 027d 067c 006a  ...}.g.}.d.}.|.j
-00000f60: 066a 0744 0090 055d 6e7d 077c 02a0 0864  .j.D...]n}.|...d
-00000f70: 03a1 017d 0874 0964 047c 076a 0a17 0083  ...}.t.d.|.j....
-00000f80: 0101 0074 0b7c 0764 0583 0272 7a7c 076a  ...t.|.d...rz|.j
-00000f90: 0c64 066b 0372 6e74 0d7c 076a 0c83 017d  .d.k.rnt.|.j...}
-00000fa0: 0971 e874 0d7c 076a 0e83 017d 096e 6e7c  .q.t.|.j...}.nn|
-00000fb0: 0864 076b 0272 aa74 0f83 007d 0a7c 0a6a  .d.k.r.t...}.|.j
-00000fc0: 1064 066b 0272 9e74 0d7c 0a6a 1183 017d  .d.k.r.t.|.j...}
-00000fd0: 0971 e874 0d7c 0a6a 1083 017d 096e 3e7c  .q.t.|.j...}.n>|
-00000fe0: 0864 086b 0272 da74 1283 007d 0a7c 0a6a  .d.k.r.t...}.|.j
-00000ff0: 1064 066b 0272 ce74 0d7c 0a6a 1183 017d  .d.k.r.t.|.j...}
-00001000: 0971 e874 0d7c 0a6a 1083 017d 096e 0e74  .q.t.|.j...}.n.t
-00001010: 0964 097c 076a 0a83 0201 0071 3074 137c  .d.|.j.....q0t.|
-00001020: 0964 0a83 027d 0b74 137c 0964 0b83 027d  .d...}.t.|.d...}
-00001030: 0c7c 09a0 1464 0c64 06a1 027d 0d74 016a  .|...d.d...}.t.j
-00001040: 02a0 1574 016a 02a0 0574 01a0 16a1 0064  ...t.j...t.....d
-00001050: 0d7c 0d17 00a1 02a1 017d 0e74 0964 0e7c  .|.......}.t.d.|
-00001060: 0964 0f83 0301 0074 01a0 177c 04a1 0144  .d.....t...|...D
-00001070: 005d 2c5c 037d 0f7d 107d 117c 1144 005d  .],\.}.}.}.|.D.]
-00001080: 1a7d 127c 05a0 1874 016a 02a0 057c 0f7c  .}.|...t.j...|.|
-00001090: 12a1 02a1 0101 0090 0171 4a90 0171 3c74  .........qJ..q<t
-000010a0: 197c 0583 017d 137c 0544 0090 045d 267d  .|...}.|.D...]&}
-000010b0: 1474 1a6a 1b7c 1464 1064 1164 128d 0390  .t.j.|.d.d.d....
-000010c0: 018f 007d 157c 15a0 1ca1 007d 167c 16a0  ...}.|.....}.|..
-000010d0: 147c 067c 09a1 027d 1774 0da0 1d7c 17a1  .|.|...}.t...|..
-000010e0: 017d 1874 016a 02a0 1e74 1f7c 1483 016a  .}.t.j...t.|...j
-000010f0: 02a1 01a0 1464 1364 14a1 027d 1974 016a  .....d.d...}.t.j
-00001100: 02a0 1574 016a 02a0 057c 0e7c 19a1 02a1  ...t.j...|.|....
-00001110: 017d 0474 016a 02a0 207c 0ea1 0190 0173  .}.t.j.. |.....s
-00001120: f674 01a0 217c 0ea1 0101 0074 016a 02a0  .t..!|.....t.j..
-00001130: 207c 04a1 0190 0272 1457 0035 0051 0052   |.....r.W.5.Q.R
-00001140: 00a3 0090 0171 766e 367c 02a0 0864 15a1  .....qvn6|...d..
-00001150: 0164 006b 0990 0272 4a7c 02a0 0864 15a1  .d.k...rJ|...d..
-00001160: 01a0 1464 0c64 06a1 027c 0d6b 0290 0272  ...d.d...|.k...r
-00001170: 4a57 0035 0051 0052 00a3 0090 0171 767a  JW.5.Q.R.....qvz
-00001180: 1274 226a 237c 187c 0464 168d 0201 0057  .t"j#|.|.d.....W
-00001190: 006e 2c04 0074 246b 0a90 0272 8801 007d  .n,..t$k...r...}
-000011a0: 1a01 007a 0c74 097c 1a83 0101 0057 0035  ...z.t.|.....W.5
-000011b0: 0064 007d 1a7e 1a58 0059 006e 0258 0057  .d.}.~.X.Y.n.X.W
-000011c0: 0035 0051 0052 0058 0074 1a6a 1b7c 1464  .5.Q.R.X.t.j.|.d
-000011d0: 1064 1164 128d 0390 018f 5e7d 157c 15a0  .d.d......^}.|..
-000011e0: 1ca1 007d 167c 16a0 147c 067c 0ba1 027d  ...}.|...|.|...}
-000011f0: 1774 0da0 1d7c 17a1 017d 1874 016a 02a0  .t...|...}.t.j..
-00001200: 1e74 1f7c 1483 016a 02a1 01a0 1464 1364  .t.|...j.....d.d
-00001210: 17a1 027d 1974 016a 02a0 1574 016a 02a0  ...}.t.j...t.j..
-00001220: 057c 0e7c 19a1 02a1 017d 0474 016a 02a0  .|.|.....}.t.j..
-00001230: 207c 0ea1 0190 0373 0e74 01a0 217c 0ea1   |.....s.t..!|..
-00001240: 0101 0074 016a 02a0 207c 04a1 0190 0372  ...t.j.. |.....r
-00001250: 2c57 0035 0051 0052 00a3 0090 0171 766e  ,W.5.Q.R.....qvn
-00001260: 7e7c 02a0 0864 15a1 0164 006b 0990 0372  ~|...d...d.k...r
-00001270: aa7c 02a0 0864 15a1 01a0 1464 0c64 06a1  .|...d.....d.d..
-00001280: 027c 0d6b 0290 0372 aa74 016a 02a0 1574  .|.k...r.t.j...t
-00001290: 016a 02a0 0574 01a0 16a1 0064 18a1 02a1  .j...t.....d....
-000012a0: 017d 1b74 016a 02a0 2074 016a 02a0 057c  .}.t.j.. t.j...|
-000012b0: 1b7c 19a1 02a1 0190 0372 aa74 25a0 2674  .|.......r.t%.&t
-000012c0: 016a 02a0 057c 1b7c 19a1 027c 0ea1 0201  .j...|.|...|....
-000012d0: 0057 0035 0051 0052 00a3 0090 0171 7674  .W.5.Q.R.....qvt
-000012e0: 016a 02a0 1574 016a 02a0 057c 0e7c 19a1  .j...t.j...|.|..
-000012f0: 02a1 017d 047a 1274 226a 237c 187c 0464  ...}.z.t"j#|.|.d
-00001300: 168d 0201 0057 006e 2c04 0074 246b 0a90  .....W.n,..t$k..
-00001310: 0372 fe01 007d 1a01 007a 0c74 097c 1a83  .r...}...z.t.|..
-00001320: 0101 0057 0035 0064 007d 1a7e 1a58 0059  ...W.5.d.}.~.X.Y
-00001330: 006e 0258 0057 0035 0051 0052 0058 0074  .n.X.W.5.Q.R.X.t
-00001340: 1a6a 1b7c 1464 1064 1164 128d 0390 018f  .j.|.d.d.d......
-00001350: 5e7d 157c 15a0 1ca1 007d 167c 16a0 147c  ^}.|.....}.|...|
-00001360: 067c 0ca1 027d 1774 0da0 1d7c 17a1 017d  .|...}.t...|...}
-00001370: 1874 016a 02a0 1e74 1f7c 1483 016a 02a1  .t.j...t.|...j..
-00001380: 01a0 1464 1364 19a1 027d 1974 016a 02a0  ...d.d...}.t.j..
-00001390: 1574 016a 02a0 057c 0e7c 19a1 02a1 017d  .t.j...|.|.....}
-000013a0: 0474 016a 02a0 207c 0ea1 0190 0473 8474  .t.j.. |.....s.t
-000013b0: 01a0 217c 0ea1 0101 0074 016a 02a0 207c  ..!|.....t.j.. |
-000013c0: 04a1 0190 0472 a257 0035 0051 0052 00a3  .....r.W.5.Q.R..
-000013d0: 0090 0171 766e 7e7c 02a0 0864 15a1 0164  ...qvn~|...d...d
-000013e0: 006b 0990 0572 207c 02a0 0864 15a1 01a0  .k...r |...d....
-000013f0: 1464 0c64 06a1 027c 0d6b 0290 0572 2074  .d.d...|.k...r t
-00001400: 016a 02a0 1574 016a 02a0 0574 01a0 16a1  .j...t.j...t....
-00001410: 0064 18a1 02a1 017d 1b74 016a 02a0 2074  .d.....}.t.j.. t
-00001420: 016a 02a0 057c 1b7c 19a1 02a1 0190 0572  .j...|.|.......r
-00001430: 2074 25a0 2674 016a 02a0 057c 1b7c 19a1   t%.&t.j...|.|..
-00001440: 027c 0ea1 0201 0057 0035 0051 0052 00a3  .|.....W.5.Q.R..
-00001450: 0090 0171 7674 016a 02a0 1574 016a 02a0  ...qvt.j...t.j..
-00001460: 057c 0e7c 19a1 02a1 017d 047a 1274 226a  .|.|.....}.z.t"j
-00001470: 237c 187c 0464 168d 0201 0057 006e 2c04  #|.|.d.....W.n,.
-00001480: 0074 246b 0a90 0572 7401 007d 1a01 007a  .t$k...rt..}...z
-00001490: 0c74 097c 1a83 0101 0057 0035 0064 007d  .t.|.....W.5.d.}
-000014a0: 1a7e 1a58 0059 006e 0258 0057 0035 0051  .~.X.Y.n.X.W.5.Q
-000014b0: 0052 0058 007c 01a0 2774 287c 05a0 297c  .R.X.|..'t(|..)|
-000014c0: 14a1 017c 131b 0064 1a14 0083 01a1 0101  ...|...d........
-000014d0: 0090 0171 7671 3064 0053 0029 1b4e 720f  ...qvq0d.S.).Nr.
-000014e0: 0000 0072 1000 0000 da05 5448 454d 457a  ...r......THEMEz
-000014f0: 1343 6865 636b 696e 6720 6963 6f6e 7320  .Checking icons 
-00001500: 666f 7220 da0a 6963 6f6e 7343 6f6c 6f72  for ..iconsColor
-00001510: 7214 0000 00da 054c 4947 4854 da04 4441  r......LIGHT..DA
-00001520: 524b 7a22 4e6f 2069 636f 6e73 2063 6f6c  RKz"No icons col
-00001530: 6f72 2073 7065 6369 6669 6564 2066 6f72  or specified for
-00001540: 2074 6865 6d65 7211 0000 0072 1200 0000   themer....r....
-00001550: 7213 0000 0072 1500 0000 7a27 4765 6e65  r....r....z'Gene
-00001560: 7261 7469 6e67 206d 6973 7369 6e67 2069  rating missing i
-00001570: 636f 6e73 2066 6f72 2079 6f75 7220 7468  cons for your th
-00001580: 656d 657a 1f70 6c65 6173 6520 7761 6974  emez.please wait
-00001590: 2e20 5468 6973 206d 6179 2074 616b 6520  . This may take 
-000015a0: 6c6f 6e67 721c 0000 0072 1d00 0000 721e  longr....r....r.
-000015b0: 0000 0072 1800 0000 7219 0000 0072 1700  ...r....r....r..
-000015c0: 0000 7221 0000 0072 1a00 0000 7216 0000  ..r!...r....r...
-000015d0: 0072 1b00 0000 7222 0000 0029 2a72 2700  .r....r"...)*r'.
-000015e0: 0000 7228 0000 0072 2900 0000 722a 0000  ..r(...r)...r*..
-000015f0: 0072 2b00 0000 722c 0000 00da 0275 69da  .r+...r,.....ui.
-00001600: 0674 6865 6d65 7372 3400 0000 7235 0000  .themesr4...r5..
-00001610: 0072 4900 0000 da07 6861 7361 7474 7272  .rI.....hasattrr
-00001620: 6a00 0000 722f 0000 00da 0b61 6363 656e  j...r/.....accen
-00001630: 7443 6f6c 6f72 da05 4c69 6768 74da 0b69  tColor..Light..i
-00001640: 636f 6e73 5f63 6f6c 6f72 da0c 6163 6365  cons_color..acce
-00001650: 6e74 5f63 6f6c 6f72 da04 4461 726b 7230  nt_color..Darkr0
-00001660: 0000 0072 3100 0000 7232 0000 0072 3300  ...r1...r2...r3.
-00001670: 0000 7236 0000 0072 3700 0000 7238 0000  ..r6...r7...r8..
-00001680: 0072 3d00 0000 723e 0000 0072 3f00 0000  .r=...r>...r?...
-00001690: 7240 0000 0072 3900 0000 7202 0000 0072  r@...r9...r....r
-000016a0: 3a00 0000 7241 0000 0072 4200 0000 7243  :...rA...rB...rC
-000016b0: 0000 0072 4400 0000 723b 0000 0072 3c00  ...rD...r;...r<.
-000016c0: 0000 7245 0000 0072 4600 0000 7247 0000  ..rE...rF...rG..
-000016d0: 0029 1c72 0a00 0000 724e 0000 0072 4f00  .).r....rN...rO.
-000016e0: 0000 722a 0000 0072 5000 0000 7251 0000  ..r*...rP...rQ..
-000016f0: 0072 5300 0000 da05 7468 656d 6572 6900  .rS.....themeri.
-00001700: 0000 7254 0000 005a 0d74 6865 6d65 5072  ..rT...Z.themePr
-00001710: 6f70 6572 7479 7255 0000 0072 5600 0000  opertyrU...rV...
-00001720: 7257 0000 0072 5800 0000 725b 0000 0072  rW...rX...r[...r
-00001730: 5c00 0000 725d 0000 0072 5e00 0000 725f  \...r]...r^...r_
-00001740: 0000 0072 4900 0000 7261 0000 0072 6200  ...rI...ra...rb.
-00001750: 0000 7263 0000 0072 6400 0000 7260 0000  ..rc...rd...r`..
-00001760: 0072 6500 0000 7259 0000 0072 0d00 0000  .re...rY...r....
-00001770: 720d 0000 0072 0e00 0000 724d 0000 00b4  r....r....rM....
-00001780: 0000 0073 b600 0000 0001 0602 0c01 0e01  ...s............
-00001790: 0402 0402 0e01 0a04 0e03 0a01 0a01 0c02  ................
-000017a0: 0c02 0801 0601 0a01 0c02 0c02 0801 0601  ................
-000017b0: 0a01 0c02 0c03 0c01 0202 0a01 0a02 0c02  ................
-000017c0: 1e02 0c02 1401 0801 1c02 0801 0a02 1401  ................
-000017d0: 0802 0c01 0a02 1a01 1602 0e01 0a02 0e01  ................
-000017e0: 1002 2801 0e01 0202 1201 1201 2403 1401  ..(.........$...
-000017f0: 0802 0c01 0a02 1a01 1602 0e01 0a02 0e01  ................
-00001800: 1002 2802 1a02 1801 1601 0e02 1601 0202  ..(.............
-00001810: 1201 1201 2403 1401 0802 0c01 0a02 1a01  ....$...........
-00001820: 1602 0e01 0a02 0e01 1002 2802 1a02 1801  ..........(.....
-00001830: 1601 0e02 1601 0201 1201 1201 2404 7a22  ............$.z"
-00001840: 4e65 7749 636f 6e73 4765 6e65 7261 746f  NewIconsGenerato
-00001850: 722e 6765 6e65 7261 7465 416c 6c49 636f  r.generateAllIco
-00001860: 6e73 2908 da08 5f5f 6e61 6d65 5f5f da0a  ns)...__name__..
-00001870: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
-00001880: 616c 6e61 6d65 5f5f da07 5f5f 646f 635f  alname__..__doc_
-00001890: 5f72 0800 0000 7268 0000 0072 4d00 0000  _r....rh...rM...
-000018a0: da0d 5f5f 636c 6173 7363 656c 6c5f 5f72  ..__classcell__r
-000018b0: 0d00 0000 720d 0000 0072 0b00 0000 720e  ....r....r....r.
-000018c0: 0000 0072 0600 0000 0f00 0000 730a 0000  ...r........s...
-000018d0: 0008 0104 010c 0408 7f00 2072 0600 0000  .......... r....
-000018e0: 290e 7242 0000 0072 3d00 0000 7228 0000  ).rB...r=...r(..
-000018f0: 00da 0373 7973 723b 0000 00da 0c75 726c  ...sysr;.....url
-00001900: 6c69 622e 7061 7273 6572 0200 0000 da07  lib.parser......
-00001910: 7061 7468 6c69 6272 0300 0000 da08 5f5f  pathlibr......__
-00001920: 6d61 696e 5f5f da0b 636f 6c6f 7273 7973  main__..colorsys
-00001930: 7465 6d72 2700 0000 724f 0000 0072 0600  temr'...rO...r..
-00001940: 0000 720d 0000 0072 0d00 0000 720d 0000  ..r....r....r...
-00001950: 0072 0e00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-00001960: 0100 0000 7314 0000 0008 0108 0108 0108  ....s...........
-00001970: 0108 010c 010c 0108 0308 0206 02         .............
+000001b0: a900 fa4e 633a 5c75 7365 7273 5c6b 6962  ...Nc:\users\kib
+000001c0: 6574 5c61 6e61 636f 6e64 6133 5c4c 6962  et\anaconda3\Lib
+000001d0: 5c73 6974 652d 7061 636b 6167 6573 5c43  \site-packages\C
+000001e0: 7573 746f 6d5f 5769 6467 6574 732f 5173  ustom_Widgets/Qs
+000001f0: 732f 5376 6754 6f50 6e67 4963 6f6e 732e  s/SvgToPngIcons.
+00000200: 7079 7208 0000 0011 0000 0073 0400 0000  pyr........s....
+00000210: 0001 0e01 7a1a 4e65 7749 636f 6e73 4765  ....z.NewIconsGe
+00000220: 6e65 7261 746f 722e 5f5f 696e 6974 5f5f  nerator.__init__
+00000230: 6302 0000 0000 0000 0000 0000 0023 0000  c............#..
+00000240: 000c 0000 0043 0000 0073 4607 0000 7400  .....C...sF...t.
+00000250: 8300 7d02 7401 6a02 a003 7404 a101 7d03  ..}.t.j...t...}.
+00000260: 7401 6a02 a005 7c03 6401 a102 7d04 6700  t.j...|.d...}.g.
+00000270: 7d05 7406 a007 7c00 a101 7d06 6402 7d07  }.t...|...}.d.}.
+00000280: 7408 7c06 6403 1900 8301 7d08 7409 7c08  t.|.d.....}.t.|.
+00000290: 6404 8302 7d09 7409 7c08 6405 8302 7d0a  d...}.t.|.d...}.
+000002a0: 7c08 a00a 6406 6407 a102 7d0b 7401 6a02  |...d.d...}.t.j.
+000002b0: a00b 7401 6a02 a005 7401 a00c a100 6408  ..t.j...t.....d.
+000002c0: 7c0b 1700 a102 a101 7d0c 7401 6a02 a00b  |.......}.t.j...
+000002d0: 7401 6a02 a005 7401 a00c a100 6409 a102  t.j...t.....d...
+000002e0: a101 7d0d 7c02 a00d 640a a101 6400 6b08  ..}.|...d...d.k.
+000002f0: 72da 7406 a007 7c00 a101 7d0e 7401 6a02  r.t...|...}.t.j.
+00000300: a00b 7401 6a02 a005 7401 a00c a100 6408  ..t.j...t.....d.
+00000310: 7c0e 6403 1900 a00a 6406 6407 a102 1700  |.d.....d.d.....
+00000320: a102 a101 7d0f 6e2c 7401 6a02 a00b 7401  ....}.n,t.j...t.
+00000330: 6a02 a005 7401 a00c a100 6408 7c02 a00d  j...t.....d.|...
+00000340: 640a a101 a00a 6406 6407 a102 1700 a102  d.....d.d.......
+00000350: a101 7d0f 7c02 a00d 640a a101 7c08 6b02  ..}.|...d...|.k.
+00000360: 9007 7336 7c06 6403 1900 6400 6b09 9007  ..s6|.d...d.k...
+00000370: 7236 7c00 6a0e 9001 7248 740f 640b 7c02  r6|.j...rHt.d.|.
+00000380: a00d 640a a101 640c 7c08 8304 0100 740f  ..d...d.|.....t.
+00000390: 640d 8301 0100 7401 a010 7c04 a101 4400  d.....t...|...D.
+000003a0: 5d2c 5c03 7d10 7d11 7d12 7c12 4400 5d1a  ],\.}.}.}.|.D.].
+000003b0: 7d13 7c05 a011 7401 6a02 a005 7c10 7c13  }.|...t.j...|.|.
+000003c0: a102 a101 0100 9001 7160 9001 7152 7412  ........q`..qRt.
+000003d0: 7c05 8301 7d14 7c05 4400 9001 5d26 7d15  |...}.|.D...]&}.
+000003e0: 7401 6a02 a013 7414 7c15 8301 6a02 a101  t.j...t.|...j...
+000003f0: a00a 640e 640f a102 7d16 7401 6a02 a015  ..d.d...}.t.j...
+00000400: 7401 6a02 a005 7c0d 7c16 a102 a101 9001  t.j...|.|.......
+00000410: 72f2 7401 6a02 a015 7401 6a02 a005 7c0f  r.t.j...t.j...|.
+00000420: 7c16 a102 a101 9001 73f2 7416 a017 7401  |.......s.t...t.
+00000430: 6a02 a005 7c0d 7c16 a102 7c0f a102 0100  j...|.|...|.....
+00000440: 7401 6a02 a013 7414 7c15 8301 6a02 a101  t.j...t.|...j...
+00000450: a00a 640e 6410 a102 7d16 7401 6a02 a015  ..d.d...}.t.j...
+00000460: 7401 6a02 a005 7c0d 7c16 a102 a101 9002  t.j...|.|.......
+00000470: 7252 7401 6a02 a015 7401 6a02 a005 7c0f  rRt.j...t.j...|.
+00000480: 7c16 a102 a101 9002 7352 7416 a017 7401  |.......sRt...t.
+00000490: 6a02 a005 7c0d 7c16 a102 7c0f a102 0100  j...|.|...|.....
+000004a0: 7401 6a02 a013 7414 7c15 8301 6a02 a101  t.j...t.|...j...
+000004b0: a00a 640e 6411 a102 7d16 7401 6a02 a015  ..d.d...}.t.j...
+000004c0: 7401 6a02 a005 7c0d 7c16 a102 a101 9001  t.j...|.|.......
+000004d0: 728c 7401 6a02 a015 7401 6a02 a005 7c0f  r.t.j...t.j...|.
+000004e0: 7c16 a102 a101 9001 738c 7416 a017 7401  |.......s.t...t.
+000004f0: 6a02 a005 7c0d 7c16 a102 7c0f a102 0100  j...|.|...|.....
+00000500: 9001 718c 7c05 4400 9002 5d92 7d15 7418  ..q.|.D...].}.t.
+00000510: 6a19 7c15 6412 6413 6414 8d03 8fba 7d17  j.|.d.d.d.....}.
+00000520: 7c17 a01a a100 7d18 7c18 a00a 7c07 7c08  |.....}.|...|.|.
+00000530: a102 7d19 7408 a01b 7c19 a101 7d1a 7401  ..}.t...|...}.t.
+00000540: 6a02 a013 7414 7c15 8301 6a02 a101 a00a  j...t.|...j.....
+00000550: 640e 640f a102 7d16 7401 6a02 a00b 7401  d.d...}.t.j...t.
+00000560: 6a02 a005 7c0c 7c16 a102 a101 7d04 7401  j...|.|.....}.t.
+00000570: 6a02 a015 7c0c a101 9003 7338 7401 a01c  j...|.....s8t...
+00000580: 7c0c a101 0100 7401 6a02 a015 7c04 a101  |.....t.j...|...
+00000590: 9003 7386 7a12 741d 6a1e 7c1a 7c04 6415  ..s.z.t.j.|.|.d.
+000005a0: 8d02 0100 5700 6e2c 0400 741f 6b0a 9003  ....W.n,..t.k...
+000005b0: 7284 0100 7d1b 0100 7a0c 740f 7c1b 8301  r...}...z.t.|...
+000005c0: 0100 5700 3500 6400 7d1b 7e1b 5800 5900  ..W.5.d.}.~.X.Y.
+000005d0: 6e02 5800 5700 3500 5100 5200 5800 7418  n.X.W.5.Q.R.X.t.
+000005e0: 6a19 7c15 6412 6413 6414 8d03 8fba 7d17  j.|.d.d.d.....}.
+000005f0: 7c17 a01a a100 7d18 7c18 a00a 7c07 7c09  |.....}.|...|.|.
+00000600: a102 7d19 7408 a01b 7c19 a101 7d1a 7401  ..}.t...|...}.t.
+00000610: 6a02 a013 7414 7c15 8301 6a02 a101 a00a  j...t.|...j.....
+00000620: 640e 6410 a102 7d16 7401 6a02 a00b 7401  d.d...}.t.j...t.
+00000630: 6a02 a005 7c0c 7c16 a102 a101 7d04 7401  j...|.|.....}.t.
+00000640: 6a02 a015 7c0c a101 9004 7308 7401 a01c  j...|.....s.t...
+00000650: 7c0c a101 0100 7401 6a02 a015 7c04 a101  |.....t.j...|...
+00000660: 9004 7356 7a12 741d 6a1e 7c1a 7c04 6415  ..sVz.t.j.|.|.d.
+00000670: 8d02 0100 5700 6e2c 0400 741f 6b0a 9004  ....W.n,..t.k...
+00000680: 7254 0100 7d1b 0100 7a0c 740f 7c1b 8301  rT..}...z.t.|...
+00000690: 0100 5700 3500 6400 7d1b 7e1b 5800 5900  ..W.5.d.}.~.X.Y.
+000006a0: 6e02 5800 5700 3500 5100 5200 5800 7418  n.X.W.5.Q.R.X.t.
+000006b0: 6a19 7c15 6412 6413 6414 8d03 8fba 7d17  j.|.d.d.d.....}.
+000006c0: 7c17 a01a a100 7d18 7c18 a00a 7c07 7c0a  |.....}.|...|.|.
+000006d0: a102 7d19 7408 a01b 7c19 a101 7d1a 7401  ..}.t...|...}.t.
+000006e0: 6a02 a013 7414 7c15 8301 6a02 a101 a00a  j...t.|...j.....
+000006f0: 640e 6411 a102 7d16 7401 6a02 a00b 7401  d.d...}.t.j...t.
+00000700: 6a02 a005 7c0c 7c16 a102 a101 7d04 7401  j...|.|.....}.t.
+00000710: 6a02 a015 7c0c a101 9004 73d8 7401 a01c  j...|.....s.t...
+00000720: 7c0c a101 0100 7401 6a02 a015 7c04 a101  |.....t.j...|...
+00000730: 9005 7326 7a12 741d 6a1e 7c1a 7c04 6415  ..s&z.t.j.|.|.d.
+00000740: 8d02 0100 5700 6e2c 0400 741f 6b0a 9005  ....W.n,..t.k...
+00000750: 7224 0100 7d1b 0100 7a0c 740f 7c1b 8301  r$..}...z.t.|...
+00000760: 0100 5700 3500 6400 7d1b 7e1b 5800 5900  ..W.5.d.}.~.X.Y.
+00000770: 6e02 5800 5700 3500 5100 5200 5800 7c01  n.X.W.5.Q.R.X.|.
+00000780: a020 7421 7c05 a022 7c15 a101 7c14 1b00  . t!|.."|...|...
+00000790: 6416 1400 8301 a101 0100 9002 71ba 7c0c  d...........q.|.
+000007a0: 7d1c 7c0d 7d1d 7401 a023 7c1c a101 7d1e  }.|.}.t..#|...}.
+000007b0: 7401 6a02 a015 7c0d a101 9005 737c 7401  t.j...|.....s|t.
+000007c0: a01c 7c0d a101 0100 6e18 7401 6a02 a015  ..|.....n.t.j...
+000007d0: 7c0d a101 9005 7394 7401 a01c 7c0d a101  |.....s.t...|...
+000007e0: 0100 6417 7d1f 7c1e 4400 5d9e 7d20 7401  ..d.}.|.D.].} t.
+000007f0: 6a24 6418 6b02 9005 72c4 7416 a025 7401  j$d.k...r.t..%t.
+00000800: 6a02 a005 7c1c 7c20 a102 7c1d a102 0100  j...|.| ..|.....
+00000810: 6e56 7a1a 7416 a017 7401 6a02 a005 7c1c  nVz.t...t.j...|.
+00000820: 7c20 a102 7c1d a102 0100 5700 6e3a 0400  | ..|.....W.n:..
+00000830: 741f 6b0a 9006 7218 0100 7d1b 0100 7a1a  t.k...r...}...z.
+00000840: 7416 a025 7401 6a02 a005 7c1c 7c20 a102  t..%t.j...|.| ..
+00000850: 7c1d a102 0100 5700 3500 6400 7d1b 7e1b  |.....W.5.d.}.~.
+00000860: 5800 5900 6e02 5800 7c1f 6419 3700 7d1f  X.Y.n.X.|.d.7.}.
+00000870: 7c01 a020 7421 7c1f 7c14 1b00 6416 1400  |.. t!|.|...d...
+00000880: 8301 a101 0100 9005 719c 7401 6a02 a00b  ........q.t.j...
+00000890: 7401 6a02 a005 7401 a00c a100 641a a102  t.j...t.....d...
+000008a0: a101 7d21 7401 6a02 a015 7c21 a101 9006  ..}!t.j...|!....
+000008b0: 73a0 7416 a025 7401 6a02 a00b 7401 6a02  s.t..%t.j...t.j.
+000008c0: a005 7401 6a02 a003 7404 a101 641b a102  ..t.j...t...d...
+000008d0: a101 7401 6a02 a00b 7401 6a02 a005 7401  ..t.j...t.j...t.
+000008e0: a00c a100 641c a102 a101 a102 0100 7c21  ....d.........|!
+000008f0: a00a 641d 641e a102 7d22 7c22 a00a 6408  ..d.d...}"|"..d.
+00000900: 6407 a102 7d22 7c22 a00a 641f 6407 a102  d...}"|"..d.d...
+00000910: 7d22 7c22 a00a 6420 6421 a102 7d22 7a36  }"|"..d d!..}"z6
+00000920: 7c02 a026 640a 7c08 a102 0100 7401 a027  |..&d.|.....t..'
+00000930: 6422 7c21 1700 6423 1700 7c22 1700 6424  d"|!..d#..|"..d$
+00000940: 1700 a101 0100 7c02 a026 640a 7c08 a102  ......|..&d.|...
+00000950: 0100 5700 6e2c 0400 741f 6b0a 9007 7232  ..W.n,..t.k...r2
+00000960: 0100 7d1b 0100 7a0c 740f 6425 8301 0100  ..}...z.t.d%....
+00000970: 5700 3500 6400 7d1b 7e1b 5800 5900 6e02  W.5.d.}.~.X.Y.n.
+00000980: 5800 6e0c 7428 a029 7c00 7c01 a102 0100  X.n.t(.)|.|.....
+00000990: 6400 5300 2926 4efa 1269 636f 6e73 2f6f  d.S.)&N..icons/o
+000009a0: 7269 6769 6e61 6c5f 7376 67fa 0423 6666  riginal_svg..#ff
+000009b0: 667a 0b69 636f 6e73 2d63 6f6c 6f72 e700  fz.icons-color..
+000009c0: 0000 0000 00f8 3fe7 0000 0000 0000 e03f  ......?........?
+000009d0: fa01 23da 00fa 0451 5353 2ffa 0951 5353  ..#....QSS/..QSS
+000009e0: 2f49 636f 6e73 fa0b 4943 4f4e 532d 434f  /Icons..ICONS-CO
+000009f0: 4c4f 527a 1443 7572 7265 6e74 2069 636f  LORz.Current ico
+00000a00: 6e73 2063 6f6c 6f72 207a 0f4e 6577 2069  ns color z.New i
+00000a10: 636f 6e73 2063 6f6c 6f72 7a40 4765 6e65  cons colorz@Gene
+00000a20: 7261 7469 6e67 2069 636f 6e73 2066 6f72  rating icons for
+00000a30: 2079 6f75 7220 7468 656d 652c 2070 6c65   your theme, ple
+00000a40: 6173 6520 7761 6974 2e20 5468 6973 206d  ase wait. This m
+00000a50: 6179 2074 616b 6520 6c6f 6e67 fa04 2e73  ay take long...s
+00000a60: 7667 fa04 2e70 6e67 fa0a 5f66 6f63 7573  vg...png.._focus
+00000a70: 2e70 6e67 fa0d 5f64 6973 6162 6c65 642e  .png.._disabled.
+00000a80: 706e 67fa 0575 7466 2d38 da06 6967 6e6f  png..utf-8..igno
+00000a90: 7265 a902 da08 656e 636f 6469 6e67 da06  re....encoding..
+00000aa0: 6572 726f 7273 a902 5a0a 6279 7465 7374  errors..Z.bytest
+00000ab0: 7269 6e67 5a08 7772 6974 655f 746f e964  ringZ.write_to.d
+00000ac0: 0000 0072 0100 0000 da02 6e74 7204 0000  ...r......ntr...
+00000ad0: 007a 1551 5353 2f51 5353 5f52 6573 6f75  .z.QSS/QSS_Resou
+00000ae0: 7263 6573 2e71 7263 7a11 5153 535f 5265  rces.qrcz.QSS_Re
+00000af0: 736f 7572 6365 732e 7172 635a 0351 5353  sources.qrcZ.QSS
+00000b00: 7a04 2e71 7263 7a03 2e70 797a 0451 5353  z..qrcz..pyz.QSS
+00000b10: 5c5a 0d51 5353 5f52 6573 6f75 7263 6573  \Z.QSS_Resources
+00000b20: 5a10 5153 535f 5265 736f 7572 6365 735f  Z.QSS_Resources_
+00000b30: 7263 7a08 7079 7263 6335 2022 7a06 2220  rcz.pyrcc5 "z." 
+00000b40: 2d6f 2022 fa01 227a 2465 7272 6f72 2077  -o ".."z$error w
+00000b50: 6869 6c65 2063 6f6e 7665 7274 696e 6720  hile converting 
+00000b60: 7265 736f 7572 6365 2066 696c 6529 2ada  resource file)*.
+00000b70: 0951 5365 7474 696e 6773 da02 6f73 da04  .QSettings..os..
+00000b80: 7061 7468 da07 6469 726e 616d 65da 085f  path..dirname.._
+00000b90: 5f66 696c 655f 5fda 046a 6f69 6e5a 1343  _file__..joinZ.C
+00000ba0: 7265 6174 6543 6f6c 6f72 5661 7269 6162  reateColorVariab
+00000bb0: 6c65 5a13 6765 7443 7572 7265 6e74 5468  leZ.getCurrentTh
+00000bc0: 656d 6549 6e66 6fda 0373 7472 da10 6164  emeInfo..str..ad
+00000bd0: 6a75 7374 5f6c 6967 6874 6e65 7373 da07  just_lightness..
+00000be0: 7265 706c 6163 65da 0761 6273 7061 7468  replace..abspath
+00000bf0: da06 6765 7463 7764 da05 7661 6c75 65da  ..getcwd..value.
+00000c00: 1573 686f 7743 7573 746f 6d57 6964 6765  .showCustomWidge
+00000c10: 7473 4c6f 6773 da05 7072 696e 74da 0477  tsLogs..print..w
+00000c20: 616c 6bda 0661 7070 656e 64da 036c 656e  alk..append..len
+00000c30: da08 6261 7365 6e61 6d65 7202 0000 00da  ..basenamer.....
+00000c40: 0665 7869 7374 73da 0673 6875 7469 6cda  .exists..shutil.
+00000c50: 046d 6f76 65da 0663 6f64 6563 73da 046f  .move..codecs..o
+00000c60: 7065 6eda 0472 6561 64da 0665 6e63 6f64  pen..read..encod
+00000c70: 65da 086d 616b 6564 6972 73da 0863 6169  e..makedirs..cai
+00000c80: 726f 7376 67da 0773 7667 3270 6e67 da09  rosvg..svg2png..
+00000c90: 4578 6365 7074 696f 6eda 0465 6d69 74da  Exception..emit.
+00000ca0: 0369 6e74 da05 696e 6465 78da 076c 6973  .int..index..lis
+00000cb0: 7464 6972 da04 6e61 6d65 da04 636f 7079  tdir..name..copy
+00000cc0: 5a08 7365 7456 616c 7565 da06 7379 7374  Z.setValue..syst
+00000cd0: 656d 7206 0000 00da 1067 656e 6572 6174  emr......generat
+00000ce0: 6541 6c6c 4963 6f6e 7329 2372 0a00 0000  eAllIcons)#r....
+00000cf0: da11 7072 6f67 7265 7373 5f63 616c 6c62  ..progress_callb
+00000d00: 6163 6bda 0873 6574 7469 6e67 7372 2800  ack..settingsr(.
+00000d10: 0000 da08 6669 6c65 6e61 6d65 da0d 6c69  ....filename..li
+00000d20: 7374 5f6f 665f 6669 6c65 73da 0563 6f6c  st_of_files..col
+00000d30: 6f72 da09 7376 675f 636f 6c6f 72da 0c6e  or..svg_color..n
+00000d40: 6f72 6d61 6c5f 636f 6c6f 72da 0d66 6f63  ormal_color..foc
+00000d50: 7573 6564 5f63 6f6c 6f72 da0e 6469 7361  used_color..disa
+00000d60: 626c 6564 5f63 6f6c 6f72 da0f 6963 6f6e  bled_color..icon
+00000d70: 7346 6f6c 6465 724e 616d 65da 0b69 636f  sFolderName..ico
+00000d80: 6e73 466f 6c64 6572 da0e 6f6c 6449 636f  nsFolder..oldIco
+00000d90: 6e73 466f 6c64 6572 5a0d 7661 7269 6162  nsFolderZ.variab
+00000da0: 6c65 7346 696c 655a 196f 6c64 4963 6f6e  lesFileZ.oldIcon
+00000db0: 7344 6573 7469 6e61 7469 6f6e 466f 6c64  sDestinationFold
+00000dc0: 6572 da04 726f 6f74 da04 6469 7273 da05  er..root..dirs..
+00000dd0: 6669 6c65 73da 0466 696c 65da 0a74 6f74  files..file..tot
+00000de0: 616c 4963 6f6e 7372 4600 0000 da06 6e61  alIconsrF.....na
+00000df0: 6d65 5f32 da01 66da 0763 6f6e 7465 6e74  me_2..f..content
+00000e00: da06 6e65 7753 5647 da08 6e65 7742 7974  ..newSVG..newByt
+00000e10: 6573 da01 65da 0a73 6f75 7263 655f 6469  es..e..source_di
+00000e20: 72da 0a74 6172 6765 745f 6469 725a 0a66  r..target_dirZ.f
+00000e30: 696c 655f 6e61 6d65 735a 0a66 696c 6573  ile_namesZ.files
+00000e40: 4d6f 7665 64da 0966 696c 655f 6e61 6d65  Moved..file_name
+00000e50: da0d 7265 736f 7572 6365 5f70 6174 685a  ..resource_pathZ
+00000e60: 1070 795f 7265 736f 7572 6365 5f70 6174  .py_resource_pat
+00000e70: 6872 0d00 0000 720d 0000 0072 0e00 0000  hr....r....r....
+00000e80: da10 6765 6e65 7261 7465 4e65 7749 636f  ..generateNewIco
+00000e90: 6e73 1500 0000 73d4 0000 0000 0106 020c  ns....s.........
+00000ea0: 010e 0104 020a 0104 010c 020a 010a 020c  ................
+00000eb0: 011e 021a 020e 010a 012c 022c 021e 0108  .........,.,....
+00000ec0: 0114 0108 0214 0108 011c 0208 020a 021a  ................
+00000ed0: 0130 0116 021a 0130 0116 021a 0130 011a  .0.....0.....0..
+00000ee0: 020a 0212 0108 020c 010a 021a 0116 020e  ................
+00000ef0: 010a 020e 0102 0212 0112 0124 0312 0108  ...........$....
+00000f00: 020c 010a 021a 0116 020e 010a 020e 0102  ................
+00000f10: 0212 0112 0124 0312 0108 020c 010a 021a  .....$..........
+00000f20: 0116 020e 010a 020e 0102 0212 0112 0124  ...............$
+00000f30: 0420 0304 0104 020a 020e 010c 020e 010a  . ..............
+00000f40: 0204 0108 010c 0118 0202 011a 0112 0128  ...............(
+00000f50: 0308 021a 041a 010e 013c 010c 010c 010c  .........<......
+00000f60: 010c 0202 010c 011a 0110 0112 021c 037a  ...............z
+00000f70: 224e 6577 4963 6f6e 7347 656e 6572 6174  "NewIconsGenerat
+00000f80: 6f72 2e67 656e 6572 6174 654e 6577 4963  or.generateNewIc
+00000f90: 6f6e 7363 0200 0000 0000 0000 0000 0000  onsc............
+00000fa0: 1c00 0000 0d00 0000 4300 0000 73ba 0500  ........C...s...
+00000fb0: 0074 0083 007d 0274 016a 02a0 0374 04a1  .t...}.t.j...t..
+00000fc0: 017d 0374 016a 02a0 057c 0364 01a1 027d  .}.t.j...|.d...}
+00000fd0: 0467 007d 0564 027d 067c 006a 066a 0744  .g.}.d.}.|.j.j.D
+00000fe0: 0090 055d 827d 077c 02a0 0864 03a1 017d  ...].}.|...d...}
+00000ff0: 087c 006a 0972 5474 0a64 047c 076a 0b17  .|.j.rTt.d.|.j..
+00001000: 0083 0101 0074 0c7c 0764 0583 0272 807c  .....t.|.d...r.|
+00001010: 076a 0d64 066b 0372 7474 0e7c 076a 0d83  .j.d.k.rtt.|.j..
+00001020: 017d 0971 f474 0e7c 076a 0f83 017d 096e  .}.q.t.|.j...}.n
+00001030: 747c 0864 076b 0272 b074 1083 007d 0a7c  t|.d.k.r.t...}.|
+00001040: 0a6a 1164 066b 0272 a474 0e7c 0a6a 1283  .j.d.k.r.t.|.j..
+00001050: 017d 0971 f474 0e7c 0a6a 1183 017d 096e  .}.q.t.|.j...}.n
+00001060: 447c 0864 086b 0272 e074 1383 007d 0a7c  D|.d.k.r.t...}.|
+00001070: 0a6a 1164 066b 0272 d474 0e7c 0a6a 1283  .j.d.k.r.t.|.j..
+00001080: 017d 0971 f474 0e7c 0a6a 1183 017d 096e  .}.q.t.|.j...}.n
+00001090: 147c 006a 0972 3074 0a64 097c 076a 0b83  .|.j.r0t.d.|.j..
+000010a0: 0201 0071 3074 147c 0964 0a83 027d 0b74  ...q0t.|.d...}.t
+000010b0: 147c 0964 0b83 027d 0c7c 09a0 1564 0c64  .|.d...}.|...d.d
+000010c0: 06a1 027d 0d74 016a 02a0 1674 016a 02a0  ...}.t.j...t.j..
+000010d0: 0574 01a0 17a1 0064 0d7c 0d17 00a1 02a1  .t.....d.|......
+000010e0: 017d 0e7c 006a 0990 0172 4674 0a64 0e7c  .}.|.j...rFt.d.|
+000010f0: 0964 0f83 0301 0074 01a0 187c 04a1 0144  .d.....t...|...D
+00001100: 005d 2c5c 037d 0f7d 107d 117c 1144 005d  .],\.}.}.}.|.D.]
+00001110: 1a7d 127c 05a0 1974 016a 02a0 057c 0f7c  .}.|...t.j...|.|
+00001120: 12a1 02a1 0101 0090 0171 5e90 0171 5074  .........q^..qPt
+00001130: 1a7c 0583 017d 137c 0544 0090 045d 267d  .|...}.|.D...]&}
+00001140: 1474 1b6a 1c7c 1464 1064 1164 128d 0390  .t.j.|.d.d.d....
+00001150: 018f 007d 157c 15a0 1da1 007d 167c 16a0  ...}.|.....}.|..
+00001160: 157c 067c 09a1 027d 1774 0ea0 1e7c 17a1  .|.|...}.t...|..
+00001170: 017d 1874 016a 02a0 1f74 207c 1483 016a  .}.t.j...t |...j
+00001180: 02a1 01a0 1564 1364 14a1 027d 1974 016a  .....d.d...}.t.j
+00001190: 02a0 1674 016a 02a0 057c 0e7c 19a1 02a1  ...t.j...|.|....
+000011a0: 017d 0474 016a 02a0 217c 0ea1 0190 0273  .}.t.j..!|.....s
+000011b0: 0a74 01a0 227c 0ea1 0101 0074 016a 02a0  .t.."|.....t.j..
+000011c0: 217c 04a1 0190 0272 2857 0035 0051 0052  !|.....r(W.5.Q.R
+000011d0: 00a3 0090 0171 8a6e 367c 02a0 0864 15a1  .....q.n6|...d..
+000011e0: 0164 006b 0990 0272 5e7c 02a0 0864 15a1  .d.k...r^|...d..
+000011f0: 01a0 1564 0c64 06a1 027c 0d6b 0290 0272  ...d.d...|.k...r
+00001200: 5e57 0035 0051 0052 00a3 0090 0171 8a7a  ^W.5.Q.R.....q.z
+00001210: 1274 236a 247c 187c 0464 168d 0201 0057  .t#j$|.|.d.....W
+00001220: 006e 2c04 0074 256b 0a90 0272 9c01 007d  .n,..t%k...r...}
+00001230: 1a01 007a 0c74 0a7c 1a83 0101 0057 0035  ...z.t.|.....W.5
+00001240: 0064 007d 1a7e 1a58 0059 006e 0258 0057  .d.}.~.X.Y.n.X.W
+00001250: 0035 0051 0052 0058 0074 1b6a 1c7c 1464  .5.Q.R.X.t.j.|.d
+00001260: 1064 1164 128d 0390 018f 5e7d 157c 15a0  .d.d......^}.|..
+00001270: 1da1 007d 167c 16a0 157c 067c 0ba1 027d  ...}.|...|.|...}
+00001280: 1774 0ea0 1e7c 17a1 017d 1874 016a 02a0  .t...|...}.t.j..
+00001290: 1f74 207c 1483 016a 02a1 01a0 1564 1364  .t |...j.....d.d
+000012a0: 17a1 027d 1974 016a 02a0 1674 016a 02a0  ...}.t.j...t.j..
+000012b0: 057c 0e7c 19a1 02a1 017d 0474 016a 02a0  .|.|.....}.t.j..
+000012c0: 217c 0ea1 0190 0373 2274 01a0 227c 0ea1  !|.....s"t.."|..
+000012d0: 0101 0074 016a 02a0 217c 04a1 0190 0372  ...t.j..!|.....r
+000012e0: 4057 0035 0051 0052 00a3 0090 0171 8a6e  @W.5.Q.R.....q.n
+000012f0: 7e7c 02a0 0864 15a1 0164 006b 0990 0372  ~|...d...d.k...r
+00001300: be7c 02a0 0864 15a1 01a0 1564 0c64 06a1  .|...d.....d.d..
+00001310: 027c 0d6b 0290 0372 be74 016a 02a0 1674  .|.k...r.t.j...t
+00001320: 016a 02a0 0574 01a0 17a1 0064 18a1 02a1  .j...t.....d....
+00001330: 017d 1b74 016a 02a0 2174 016a 02a0 057c  .}.t.j..!t.j...|
+00001340: 1b7c 19a1 02a1 0190 0372 be74 26a0 2774  .|.......r.t&.'t
+00001350: 016a 02a0 057c 1b7c 19a1 027c 0ea1 0201  .j...|.|...|....
+00001360: 0057 0035 0051 0052 00a3 0090 0171 8a74  .W.5.Q.R.....q.t
+00001370: 016a 02a0 1674 016a 02a0 057c 0e7c 19a1  .j...t.j...|.|..
+00001380: 02a1 017d 047a 1274 236a 247c 187c 0464  ...}.z.t#j$|.|.d
+00001390: 168d 0201 0057 006e 2c04 0074 256b 0a90  .....W.n,..t%k..
+000013a0: 0472 1201 007d 1a01 007a 0c74 0a7c 1a83  .r...}...z.t.|..
+000013b0: 0101 0057 0035 0064 007d 1a7e 1a58 0059  ...W.5.d.}.~.X.Y
+000013c0: 006e 0258 0057 0035 0051 0052 0058 0074  .n.X.W.5.Q.R.X.t
+000013d0: 1b6a 1c7c 1464 1064 1164 128d 0390 018f  .j.|.d.d.d......
+000013e0: 5e7d 157c 15a0 1da1 007d 167c 16a0 157c  ^}.|.....}.|...|
+000013f0: 067c 0ca1 027d 1774 0ea0 1e7c 17a1 017d  .|...}.t...|...}
+00001400: 1874 016a 02a0 1f74 207c 1483 016a 02a1  .t.j...t |...j..
+00001410: 01a0 1564 1364 19a1 027d 1974 016a 02a0  ...d.d...}.t.j..
+00001420: 1674 016a 02a0 057c 0e7c 19a1 02a1 017d  .t.j...|.|.....}
+00001430: 0474 016a 02a0 217c 0ea1 0190 0473 9874  .t.j..!|.....s.t
+00001440: 01a0 227c 0ea1 0101 0074 016a 02a0 217c  .."|.....t.j..!|
+00001450: 04a1 0190 0472 b657 0035 0051 0052 00a3  .....r.W.5.Q.R..
+00001460: 0090 0171 8a6e 7e7c 02a0 0864 15a1 0164  ...q.n~|...d...d
+00001470: 006b 0990 0572 347c 02a0 0864 15a1 01a0  .k...r4|...d....
+00001480: 1564 0c64 06a1 027c 0d6b 0290 0572 3474  .d.d...|.k...r4t
+00001490: 016a 02a0 1674 016a 02a0 0574 01a0 17a1  .j...t.j...t....
+000014a0: 0064 18a1 02a1 017d 1b74 016a 02a0 2174  .d.....}.t.j..!t
+000014b0: 016a 02a0 057c 1b7c 19a1 02a1 0190 0572  .j...|.|.......r
+000014c0: 3474 26a0 2774 016a 02a0 057c 1b7c 19a1  4t&.'t.j...|.|..
+000014d0: 027c 0ea1 0201 0057 0035 0051 0052 00a3  .|.....W.5.Q.R..
+000014e0: 0090 0171 8a74 016a 02a0 1674 016a 02a0  ...q.t.j...t.j..
+000014f0: 057c 0e7c 19a1 02a1 017d 047a 1274 236a  .|.|.....}.z.t#j
+00001500: 247c 187c 0464 168d 0201 0057 006e 2c04  $|.|.d.....W.n,.
+00001510: 0074 256b 0a90 0572 8801 007d 1a01 007a  .t%k...r...}...z
+00001520: 0c74 0a7c 1a83 0101 0057 0035 0064 007d  .t.|.....W.5.d.}
+00001530: 1a7e 1a58 0059 006e 0258 0057 0035 0051  .~.X.Y.n.X.W.5.Q
+00001540: 0052 0058 007c 01a0 2874 297c 05a0 2a7c  .R.X.|..(t)|..*|
+00001550: 14a1 017c 131b 0064 1a14 0083 01a1 0101  ...|...d........
+00001560: 0090 0171 8a71 3064 0053 0029 1b4e 720f  ...q.q0d.S.).Nr.
+00001570: 0000 0072 1000 0000 da05 5448 454d 457a  ...r......THEMEz
+00001580: 1343 6865 636b 696e 6720 6963 6f6e 7320  .Checking icons 
+00001590: 666f 7220 da0a 6963 6f6e 7343 6f6c 6f72  for ..iconsColor
+000015a0: 7214 0000 005a 054c 4947 4854 5a04 4441  r....Z.LIGHTZ.DA
+000015b0: 524b 7a22 4e6f 2069 636f 6e73 2063 6f6c  RKz"No icons col
+000015c0: 6f72 2073 7065 6369 6669 6564 2066 6f72  or specified for
+000015d0: 2074 6865 6d65 7211 0000 0072 1200 0000   themer....r....
+000015e0: 7213 0000 0072 1500 0000 7a27 4765 6e65  r....r....z'Gene
+000015f0: 7261 7469 6e67 206d 6973 7369 6e67 2069  rating missing i
+00001600: 636f 6e73 2066 6f72 2079 6f75 7220 7468  cons for your th
+00001610: 656d 657a 1f70 6c65 6173 6520 7761 6974  emez.please wait
+00001620: 2e20 5468 6973 206d 6179 2074 616b 6520  . This may take 
+00001630: 6c6f 6e67 721c 0000 0072 1d00 0000 721e  longr....r....r.
+00001640: 0000 0072 1800 0000 7219 0000 0072 1700  ...r....r....r..
+00001650: 0000 7221 0000 0072 1a00 0000 7216 0000  ..r!...r....r...
+00001660: 0072 1b00 0000 7222 0000 0029 2b72 2500  .r....r"...)+r%.
+00001670: 0000 7226 0000 0072 2700 0000 7228 0000  ..r&...r'...r(..
+00001680: 0072 2900 0000 722a 0000 005a 0275 69da  .r)...r*...Z.ui.
+00001690: 0674 6865 6d65 7372 3000 0000 7231 0000  .themesr0...r1..
+000016a0: 0072 3200 0000 7246 0000 00da 0768 6173  .r2...rF.....has
+000016b0: 6174 7472 7267 0000 0072 2b00 0000 5a0b  attrrg...r+...Z.
+000016c0: 6163 6365 6e74 436f 6c6f 725a 054c 6967  accentColorZ.Lig
+000016d0: 6874 5a0b 6963 6f6e 735f 636f 6c6f 725a  htZ.icons_colorZ
+000016e0: 0c61 6363 656e 745f 636f 6c6f 725a 0444  .accent_colorZ.D
+000016f0: 6172 6b72 2c00 0000 722d 0000 0072 2e00  arkr,...r-...r..
+00001700: 0000 722f 0000 0072 3300 0000 7234 0000  ..r/...r3...r4..
+00001710: 0072 3500 0000 723a 0000 0072 3b00 0000  .r5...r:...r;...
+00001720: 723c 0000 0072 3d00 0000 7236 0000 0072  r<...r=...r6...r
+00001730: 0200 0000 7237 0000 0072 3e00 0000 723f  ....r7...r>...r?
+00001740: 0000 0072 4000 0000 7241 0000 0072 3800  ...r@...rA...r8.
+00001750: 0000 7239 0000 0072 4200 0000 7243 0000  ..r9...rB...rC..
+00001760: 0072 4400 0000 291c 720a 0000 0072 4a00  .rD...).r....rJ.
+00001770: 0000 724b 0000 0072 2800 0000 724c 0000  ..rK...r(...rL..
+00001780: 0072 4d00 0000 724f 0000 00da 0574 6865  .rM...rO.....the
+00001790: 6d65 7266 0000 0072 5000 0000 5a0d 7468  merf...rP...Z.th
+000017a0: 656d 6550 726f 7065 7274 7972 5100 0000  emePropertyrQ...
+000017b0: 7252 0000 0072 5300 0000 7254 0000 0072  rR...rS...rT...r
+000017c0: 5600 0000 7257 0000 0072 5800 0000 7259  V...rW...rX...rY
+000017d0: 0000 0072 5a00 0000 7246 0000 0072 5c00  ...rZ...rF...r\.
+000017e0: 0000 725d 0000 0072 5e00 0000 725f 0000  ..r]...r^...r_..
+000017f0: 0072 5b00 0000 7260 0000 0072 5500 0000  .r[...r`...rU...
+00001800: 720d 0000 0072 0d00 0000 720e 0000 0072  r....r....r....r
+00001810: 4900 0000 b800 0000 73bc 0000 0000 0106  I.......s.......
+00001820: 020c 010e 0104 0204 020e 010a 0406 010e  ................
+00001830: 030a 010a 010c 020c 0208 0106 010a 010c  ................
+00001840: 020c 0208 0106 010a 010c 020c 0306 010c  ................
+00001850: 0102 020a 010a 020c 021e 0208 010c 0214  ................
+00001860: 0108 011c 0208 010a 0214 0108 020c 010a  ................
+00001870: 021a 0116 020e 010a 020e 0110 0228 010e  .............(..
+00001880: 0102 0212 0112 0124 0314 0108 020c 010a  .......$........
+00001890: 021a 0116 020e 010a 020e 0110 0228 021a  .............(..
+000018a0: 0218 0116 010e 0216 0102 0212 0112 0124  ...............$
+000018b0: 0314 0108 020c 010a 021a 0116 020e 010a  ................
+000018c0: 020e 0110 0228 021a 0218 0116 010e 0216  .....(..........
+000018d0: 0102 0112 0112 0124 047a 224e 6577 4963  .......$.z"NewIc
+000018e0: 6f6e 7347 656e 6572 6174 6f72 2e67 656e  onsGenerator.gen
+000018f0: 6572 6174 6541 6c6c 4963 6f6e 7329 08da  erateAllIcons)..
+00001900: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
+00001910: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
+00001920: 655f 5fda 075f 5f64 6f63 5f5f 7208 0000  e__..__doc__r...
+00001930: 0072 6500 0000 7249 0000 00da 0d5f 5f63  .re...rI.....__c
+00001940: 6c61 7373 6365 6c6c 5f5f 720d 0000 0072  lasscell__r....r
+00001950: 0d00 0000 720b 0000 0072 0e00 0000 7206  ....r....r....r.
+00001960: 0000 000f 0000 0073 0a00 0000 0801 0401  .......s........
+00001970: 0c04 087f 0024 7206 0000 0029 0e72 3f00  .....$r....).r?.
+00001980: 0000 723a 0000 0072 2600 0000 da03 7379  ..r:...r&.....sy
+00001990: 7372 3800 0000 da0c 7572 6c6c 6962 2e70  sr8.....urllib.p
+000019a0: 6172 7365 7202 0000 00da 0770 6174 686c  arser......pathl
+000019b0: 6962 7203 0000 00da 085f 5f6d 6169 6e5f  ibr......__main_
+000019c0: 5f5a 0b63 6f6c 6f72 7379 7374 656d 7225  _Z.colorsystemr%
+000019d0: 0000 0072 4b00 0000 7206 0000 0072 0d00  ...rK...r....r..
+000019e0: 0000 720d 0000 0072 0d00 0000 720e 0000  ..r....r....r...
+000019f0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+00001a00: 1400 0000 0801 0801 0801 0801 0801 0c01  ................
+00001a10: 0c01 0803 0802 0602                      ........
```

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/__pycache__/SvgToPngIcons.cpython-39.pyc` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/SvgToPngIcons.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/__pycache__/colorsystem.cpython-310.pyc` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/colorsystem.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/__pycache__/colorsystem.cpython-37.pyc` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/colorsystem.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/__pycache__/colorsystem.cpython-38.pyc` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/colorsystem.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Sun Mar 13 13:50:54 2022 UTC, .py size: 10193 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,382 +1,406 @@
-00000000: 550d 0d0a 0000 0000 bef6 2d62 d127 0000  U.........-b.'..
+00000000: 550d 0d0a 0000 0000 0066 9364 4027 0000  U........f.d@'..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 8200 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 9400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 5400 6400 6401 6c03 6d04 5a05  d.l.T.d.d.l.m.Z.
 00000050: 0100 6400 6401 6c06 5a06 6507 8300 5a08  ..d.d.l.Z.e...Z.
-00000060: 6410 6404 6405 8401 5a09 6406 6407 8400  d.d.d...Z.d.d...
+00000060: 6412 6404 6405 8401 5a09 6406 6407 8400  d.d.d...Z.d.d...
 00000070: 5a0a 4700 6408 6409 8400 6409 8302 5a0b  Z.G.d.d...d...Z.
-00000080: 4700 640a 640b 8400 640b 8302 5a0c 4700  G.d.d...d...Z.G.
-00000090: 640c 640d 8400 640d 8302 5a0d 4700 640e  d.d...d...Z.G.d.
-000000a0: 640f 8400 640f 650e 8303 5a0f 6401 5300  d...d.e...Z.d.S.
-000000b0: 2911 e900 0000 004e 2901 da01 2ae7 0000  )......N)...*...
-000000c0: 0000 0000 e03f 6302 0000 0000 0000 0000  .....?c.........
-000000d0: 0000 0005 0000 0006 0000 0043 0000 0073  ...........C...s
-000000e0: b000 0000 7a0e 7400 6a01 7c00 1900 7d02  ....z.t.j.|...}.
-000000f0: 5700 6e10 0100 0100 0100 7c00 7d02 5900  W.n.......|.}.Y.
-00000100: 6e02 5800 7402 6a03 7400 a004 7c02 a101  n.X.t.j.t...|...
-00000110: 8e00 7d02 7c02 6401 1900 6402 6b04 725c  ..}.|.d...d.k.r\
-00000120: 7402 a005 7c02 6402 1900 7c01 7c02 6401  t...|.d...|.|.d.
-00000130: 1900 1400 7c02 6403 1900 a103 7d03 6e1e  ....|.d.....}.n.
-00000140: 7402 a005 7c02 6402 1900 6401 7c01 6401  t...|.d...d.|.d.
-00000150: 1400 1800 7c02 6403 1900 a103 7d03 7406  ....|.d.....}.t.
-00000160: 7407 7c03 6402 1900 6404 1400 8301 7407  t.|.d...d.....t.
-00000170: 7c03 6401 1900 6404 1400 8301 7407 7c03  |.d...d.....t.|.
-00000180: 6403 1900 6404 1400 8301 6603 8301 7d04  d...d.....f...}.
-00000190: 7c04 5300 2905 4ee9 0100 0000 7201 0000  |.S.).N.....r...
-000001a0: 00e9 0200 0000 e9fa 0000 0029 08da 026d  ...........)...m
-000001b0: 635a 0663 6e61 6d65 73da 0863 6f6c 6f72  cZ.cnames..color
-000001c0: 7379 735a 0a72 6762 5f74 6f5f 686c 735a  sysZ.rgb_to_hlsZ
-000001d0: 0674 6f5f 7267 625a 0a68 6c73 5f74 6f5f  .to_rgbZ.hls_to_
-000001e0: 7267 62da 0a72 6762 5f74 6f5f 6865 78da  rgb..rgb_to_hex.
-000001f0: 0369 6e74 2905 da05 636f 6c6f 72da 0661  .int)...color..a
-00000200: 6d6f 756e 74da 0163 da03 7267 625a 086e  mount..c..rgbZ.n
-00000210: 6577 436f 6c6f 72a9 0072 0f00 0000 fa37  ewColor..r.....7
-00000220: 453a 5c53 7069 6e6e 2054 5620 5475 745c  E:\Spinn TV Tut\
-00000230: 3232 2d55 495c 4375 7374 6f6d 5f57 6964  22-UI\Custom_Wid
-00000240: 6765 7473 5c51 7373 5c63 6f6c 6f72 7379  gets\Qss\colorsy
-00000250: 7374 656d 2e70 79da 1061 646a 7573 745f  stem.py..adjust_
-00000260: 6c69 6768 746e 6573 7318 0000 0073 1400  lightness....s..
-00000270: 0000 0001 0201 0e01 0601 0a01 1002 0c01  ................
-00000280: 2002 1e02 3201 7211 0000 0063 0100 0000   ...2.r....c....
-00000290: 0000 0000 0000 0000 0200 0000 0300 0000  ................
-000002a0: 4300 0000 7314 0000 0064 017c 0016 007d  C...s....d.|...}
-000002b0: 0164 0274 007c 0183 0117 0053 0029 034e  .d.t.|.....S.).N
-000002c0: 7a0c 2530 3278 2530 3278 2530 3278 fa01  z.%02x%02x%02x..
-000002d0: 2329 01da 0373 7472 2902 720e 0000 005a  #)...str).r....Z
-000002e0: 0868 6578 436f 6c6f 7272 0f00 0000 720f  .hexColorr....r.
-000002f0: 0000 0072 1000 0000 7209 0000 0027 0000  ...r....r....'..
-00000300: 0073 0400 0000 0002 0801 7209 0000 0063  .s........r....c
-00000310: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000320: 0300 0000 4000 0000 73ac 0000 0065 005a  ....@...s....e.Z
-00000330: 0164 005a 0264 015a 0364 025a 0464 035a  .d.Z.d.Z.d.Z.d.Z
-00000340: 0564 025a 0665 0765 0364 0483 025a 0865  .d.Z.e.e.d...Z.e
-00000350: 0765 0364 0583 025a 0965 0765 0364 0683  .e.d...Z.e.e.d..
-00000360: 025a 0a65 0765 0364 0783 025a 0b65 0765  .Z.e.e.d...Z.e.e
-00000370: 0364 0883 025a 0c65 0765 0364 0983 025a  .d...Z.e.e.d...Z
-00000380: 0d65 0765 0464 0483 025a 0e65 0765 0464  .e.e.d...Z.e.e.d
-00000390: 0583 025a 0f65 0765 0464 0683 025a 1065  ...Z.e.e.d...Z.e
-000003a0: 0765 0464 0783 025a 1165 0765 0564 0483  .e.d...Z.e.e.d..
-000003b0: 025a 1265 0765 0564 0683 025a 1365 0765  .Z.e.e.d...Z.e.e
-000003c0: 0564 0a83 025a 1465 0765 0564 0983 025a  .d...Z.e.e.d...Z
-000003d0: 1564 0b5a 1664 0c53 0029 0dda 0444 6172  .d.Z.d.S.)...Dar
-000003e0: 6b7a 0723 3044 3044 3134 fa04 2366 6666  kz.#0D0D14..#fff
-000003f0: 7a07 2341 3842 3942 4472 0400 0000 e7cd  z.#A8B9BDr......
-00000400: cccc cccc ccec 3fe7 9a99 9999 9999 e93f  ......?........?
-00000410: e766 6666 6666 66e6 3f72 0300 0000 e79a  .ffffff.?r......
-00000420: 9999 9999 99d9 3fe7 3333 3333 3333 e33f  ......?.333333.?
-00000430: fa0e 3a2f 6963 6f6e 732f 4963 6f6e 732f  ..:/icons/Icons/
-00000440: 4ea9 17da 085f 5f6e 616d 655f 5fda 0a5f  N....__name__.._
-00000450: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
-00000460: 6c6e 616d 655f 5fda 0862 675f 636f 6c6f  lname__..bg_colo
-00000470: 72da 0974 7874 5f63 6f6c 6f72 da0c 6163  r..txt_color..ac
-00000480: 6365 6e74 5f63 6f6c 6f72 da0b 6963 6f6e  cent_color..icon
-00000490: 735f 636f 6c6f 7272 1100 0000 da04 4247  s_colorr......BG
-000004a0: 5f31 da04 4247 5f32 da04 4247 5f33 da04  _1..BG_2..BG_3..
-000004b0: 4247 5f34 da04 4247 5f35 da04 4247 5f36  BG_4..BG_5..BG_6
-000004c0: da04 4354 5f31 da04 4354 5f32 da04 4354  ..CT_1..CT_2..CT
-000004d0: 5f33 da04 4354 5f34 da04 4341 5f31 da04  _3..CT_4..CA_1..
-000004e0: 4341 5f32 da04 4341 5f33 da04 4341 5f34  CA_2..CA_3..CA_4
-000004f0: da05 4943 4f4e 5372 0f00 0000 720f 0000  ..ICONSr....r...
-00000500: 0072 0f00 0000 7210 0000 0072 1400 0000  .r....r....r....
-00000510: 2f00 0000 7326 0000 0008 0104 0104 0104  /...s&..........
-00000520: 0104 020a 010a 010a 010a 010a 010a 020a  ................
-00000530: 010a 010a 010a 020a 010a 010a 010a 0272  ...............r
-00000540: 1400 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00000550: 0000 0000 0003 0000 0040 0000 0073 ac00  .........@...s..
-00000560: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
-00000570: 5a04 6403 5a05 6404 5a06 6507 6503 6405  Z.d.Z.d.Z.e.e.d.
-00000580: 8302 5a08 6507 6503 6406 8302 5a09 6507  ..Z.e.e.d...Z.e.
-00000590: 6503 6407 8302 5a0a 6507 6503 6408 8302  e.d...Z.e.e.d...
-000005a0: 5a0b 6507 6503 6409 8302 5a0c 6507 6503  Z.e.e.d...Z.e.e.
-000005b0: 640a 8302 5a0d 6507 6504 6405 8302 5a0e  d...Z.e.e.d...Z.
-000005c0: 6507 6504 6408 8302 5a0f 6507 6504 640a  e.e.d...Z.e.e.d.
-000005d0: 8302 5a10 6507 6504 640b 8302 5a11 6507  ..Z.e.e.d...Z.e.
-000005e0: 6505 6405 8302 5a12 6507 6505 640a 8302  e.d...Z.e.e.d...
-000005f0: 5a13 6507 6505 640c 8302 5a14 6507 6505  Z.e.e.d...Z.e.e.
-00000600: 640d 8302 5a15 640e 5a16 640f 5300 2910  d...Z.d.Z.d.S.).
-00000610: da05 4c69 6768 7472 1500 0000 7a04 2330  ..Lightr....z.#0
-00000620: 3030 7a07 2330 3062 6366 66da 0072 0400  00z.#00bcff..r..
-00000630: 0000 67ae 47e1 7a14 aeef 3f67 6666 6666  ..g.G.z...?gffff
-00000640: 6666 ee3f 7216 0000 0067 3333 3333 3333  ff.?r....g333333
-00000650: eb3f 7217 0000 0072 1800 0000 721a 0000  .?r....r....r...
-00000660: 0072 1900 0000 721b 0000 004e 721c 0000  .r....r....Nr...
-00000670: 0072 0f00 0000 720f 0000 0072 0f00 0000  .r....r....r....
-00000680: 7210 0000 0072 3300 0000 4a00 0000 7326  r....r3...J...s&
-00000690: 0000 0008 0104 0104 0104 0104 020a 010a  ................
-000006a0: 010a 010a 010a 010a 020a 010a 010a 010a  ................
-000006b0: 020a 010a 010a 010a 0272 3300 0000 6300  .........r3...c.
-000006c0: 0000 0000 0000 0000 0000 0000 0000 0004  ................
-000006d0: 0000 0000 0000 0073 2e00 0000 6500 5a01  .......s....e.Z.
-000006e0: 6400 5a02 6408 8700 6601 6402 6403 8409  d.Z.d...f.d.d...
-000006f0: 5a03 6404 6405 8400 5a04 6406 6407 8400  Z.d.d...Z.d.d...
-00000700: 5a05 8700 0400 5a06 5300 2909 da13 4372  Z.....Z.S.)...Cr
-00000710: 6561 7465 436f 6c6f 7256 6172 6961 626c  eateColorVariabl
-00000720: 654e 6302 0000 0000 0000 0000 0000 0002  eNc.............
-00000730: 0000 0003 0000 0003 0000 0073 1400 0000  ...........s....
-00000740: 7400 7401 7c00 8302 a002 7c01 a101 0100  t.t.|.....|.....
-00000750: 6400 5300 2901 4e29 03da 0573 7570 6572  d.S.).N)...super
-00000760: 7235 0000 00da 085f 5f69 6e69 745f 5f29  r5.....__init__)
-00000770: 02da 0473 656c 66da 0670 6172 656e 74a9  ...self..parent.
-00000780: 01da 095f 5f63 6c61 7373 5f5f 720f 0000  ...__class__r...
-00000790: 0072 1000 0000 7237 0000 006b 0000 0073  .r....r7...k...s
-000007a0: 0200 0000 0001 7a1c 4372 6561 7465 436f  ......z.CreateCo
-000007b0: 6c6f 7256 6172 6961 626c 652e 5f5f 696e  lorVariable.__in
-000007c0: 6974 5f5f 6301 0000 0000 0000 0000 0000  it__c...........
-000007d0: 0009 0000 0006 0000 0043 0000 0073 5001  .........C...sP.
-000007e0: 0000 7400 8300 7d01 7c01 a001 6401 a101  ..t...}.|...d...
-000007f0: 7d02 6900 7d03 7c02 6402 6b02 7258 7402  }.i.}.|.d.k.rXt.
-00000800: 8300 7d04 7c04 6a03 6403 6b02 723c 7c04  ..}.|.j.d.k.r<|.
-00000810: 6a04 7d05 7c04 6a04 7c04 5f03 6e06 7c04  j.}.|.j.|._.n.|.
-00000820: 6a03 7d05 7c04 6a05 7c04 6a06 7c04 6a04  j.}.|.j.|.j.|.j.
-00000830: 7c05 6404 9c04 7d03 6eb2 7c02 6405 6b02  |.d...}.n.|.d.k.
-00000840: 729c 7407 8300 7d04 7c04 6a03 6403 6b02  r.t...}.|.j.d.k.
-00000850: 7280 7c04 6a04 7d05 7c04 6a04 7c04 5f03  r.|.j.}.|.j.|._.
-00000860: 6e06 7c04 6a03 7d05 7c04 6a05 7c04 6a06  n.|.j.}.|.j.|.j.
-00000870: 7c04 6a04 7c05 6404 9c04 7d03 6e6e 7c00  |.j.|.d...}.nn|.
-00000880: 6a08 6a09 4400 5d64 7d04 7c04 6a0a 73b8  j.j.D.]d}.|.j.s.
-00000890: 7c04 6a0b 7c02 6b02 72a4 7c01 a00c 6401  |.j.|.k.r.|...d.
-000008a0: 7c04 6a0b a102 0100 7c04 6a0d 7d06 7c04  |.j.....|.j.}.|.
-000008b0: 6a0e 7d07 7c04 6a0f 7d08 7c04 6a10 72f6  j.}.|.j.}.|.j.r.
-000008c0: 7c04 6a11 6403 6b02 72ee 7c08 7d05 71fa  |.j.d.k.r.|.}.q.
-000008d0: 7c04 6a11 7d05 6e04 6400 7d05 7c06 7c07  |.j.}.n.d.}.|.|.
-000008e0: 7c08 7c05 6404 9c04 7d03 71a4 7412 7c03  |.|.d...}.q.t.|.
-000008f0: 8301 6406 6b02 9001 724c 7402 8300 7d04  ..d.k...rLt...}.
-00000900: 7c04 6a03 6403 6b02 9001 7232 7c04 6a04  |.j.d.k...r2|.j.
-00000910: 7d05 6e06 7c04 6a03 7d05 7c04 6a05 7c04  }.n.|.j.}.|.j.|.
-00000920: 6a06 7c04 6a04 7c05 6404 9c04 7d03 7c03  j.|.j.|.d...}.|.
-00000930: 5300 2907 4eda 0554 4845 4d45 da05 4c49  S.).N..THEME..LI
-00000940: 4748 5472 3400 0000 2904 7a10 6261 636b  GHTr4...).z.back
-00000950: 6772 6f75 6e64 2d63 6f6c 6f72 7a0a 7465  ground-colorz.te
-00000960: 7874 2d63 6f6c 6f72 7a0c 6163 6365 6e74  xt-colorz.accent
-00000970: 2d63 6f6c 6f72 7a0b 6963 6f6e 732d 636f  -colorz.icons-co
-00000980: 6c6f 72da 0444 4152 4b72 0100 0000 2913  lor..DARKr....).
-00000990: da09 5153 6574 7469 6e67 73da 0576 616c  ..QSettings..val
-000009a0: 7565 7233 0000 0072 2300 0000 7222 0000  uer3...r#...r"..
-000009b0: 0072 2000 0000 7221 0000 0072 1400 0000  .r ...r!...r....
-000009c0: da02 7569 da06 7468 656d 6573 da0c 6465  ..ui..themes..de
-000009d0: 6661 756c 7454 6865 6d65 da04 6e61 6d65  faultTheme..name
-000009e0: da08 7365 7456 616c 7565 da0f 6261 636b  ..setValue..back
-000009f0: 6772 6f75 6e64 436f 6c6f 72da 0974 6578  groundColor..tex
-00000a00: 7443 6f6c 6f72 da0b 6163 6365 6e74 436f  tColor..accentCo
-00000a10: 6c6f 72da 0e63 7265 6174 654e 6577 4963  lor..createNewIc
-00000a20: 6f6e 73da 0a69 636f 6e73 436f 6c6f 72da  ons..iconsColor.
-00000a30: 036c 656e 2909 7238 0000 00da 0873 6574  .len).r8.....set
-00000a40: 7469 6e67 7372 3c00 0000 5a10 6375 7272  tingsr<...Z.curr
-00000a50: 656e 7454 6865 6d65 496e 666f da05 7468  entThemeInfo..th
-00000a60: 656d 6572 4a00 0000 7220 0000 0072 2100  emerJ...r ...r!.
-00000a70: 0000 7222 0000 0072 0f00 0000 720f 0000  ..r"...r....r...
-00000a80: 0072 1000 0000 da13 6765 7443 7572 7265  .r......getCurre
-00000a90: 6e74 5468 656d 6549 6e66 6f6e 0000 0073  ntThemeInfon...s
-00000aa0: 4800 0000 0001 0602 0a02 0402 0801 0601  H...............
-00000ab0: 0a01 0601 0a02 0602 1602 0801 0601 0a01  ................
-00000ac0: 0601 0a02 0602 1603 0c01 1002 0e01 0601  ................
-00000ad0: 0601 0602 0601 0a01 0602 0802 0402 1002  ................
-00000ae0: 0e01 0601 0c01 0802 0602 1402 7a27 4372  ............z'Cr
-00000af0: 6561 7465 436f 6c6f 7256 6172 6961 626c  eateColorVariabl
-00000b00: 652e 6765 7443 7572 7265 6e74 5468 656d  e.getCurrentThem
-00000b10: 6549 6e66 6f63 0100 0000 0000 0000 0000  eInfoc..........
-00000b20: 0000 0900 0000 2000 0000 4300 0000 73e2  ...... ...C...s.
-00000b30: 0200 0074 0083 007d 017c 01a0 0164 01a1  ...t...}.|...d..
-00000b40: 017d 0264 027d 037c 0264 036b 0272 2674  .}.d.}.|.d.k.r&t
-00000b50: 0283 007d 0490 016e 3a7c 0264 046b 0272  ...}...n:|.d.k.r
-00000b60: 3874 0383 007d 0490 016e 287c 006a 046a  8t...}...n(|.j.j
-00000b70: 0544 005d 4a7d 057c 056a 0673 547c 056a  .D.]J}.|.j.sT|.j
-00000b80: 077c 026b 0272 407c 01a0 0864 017c 056a  .|.k.r@|...d.|.j
-00000b90: 07a1 0201 007c 057d 047c 056a 097c 045f  .....|.}.|.j.|._
-00000ba0: 0a7c 056a 0b7c 045f 0c7c 056a 0d7c 045f  .|.j.|._.|.j.|._
-00000bb0: 0e7c 046a 0f7c 045f 1064 057d 0371 407c  .|.j.|._.d.}.q@|
-00000bc0: 0373 9674 0283 007d 0474 117c 046a 0a64  .s.t...}.t.|.j.d
-00000bd0: 0683 027c 045f 1274 117c 046a 0a64 0783  ...|._.t.|.j.d..
-00000be0: 027c 045f 1374 117c 046a 0a64 0883 027c  .|._.t.|.j.d...|
-00000bf0: 045f 1474 117c 046a 0a64 0983 027c 045f  ._.t.|.j.d...|._
-00000c00: 1574 117c 046a 0a64 0a83 027c 045f 1674  .t.|.j.d...|._.t
-00000c10: 117c 046a 0a64 0b83 027c 045f 1774 117c  .|.j.d...|._.t.|
-00000c20: 046a 0c64 0683 027c 045f 1874 117c 046a  .j.d...|._.t.|.j
-00000c30: 0c64 0783 027c 045f 1974 117c 046a 0c64  .d...|._.t.|.j.d
-00000c40: 0883 027c 045f 1a74 117c 046a 0c64 0c83  ...|._.t.|.j.d..
-00000c50: 027c 045f 1b74 117c 046a 0e64 0683 027c  .|._.t.|.j.d...|
-00000c60: 045f 1c74 117c 046a 0e64 0883 027c 045f  ._.t.|.j.d...|._
-00000c70: 1d74 117c 046a 0e64 0983 027c 045f 1e74  .t.|.j.d...|._.t
-00000c80: 117c 046a 0e64 0b83 027c 045f 1f64 0d7c  .|.j.d...|._.d.|
-00000c90: 045f 2074 2183 007c 005f 227c 046a 127c  ._ t!..|._"|.j.|
-00000ca0: 006a 225f 237c 046a 137c 006a 225f 247c  .j"_#|.j.|.j"_$|
-00000cb0: 046a 147c 006a 225f 257c 046a 157c 006a  .j.|.j"_%|.j.|.j
-00000cc0: 225f 267c 046a 167c 006a 225f 277c 046a  "_&|.j.|.j"_'|.j
-00000cd0: 177c 006a 225f 287c 046a 187c 006a 225f  .|.j"_(|.j.|.j"_
-00000ce0: 297c 046a 197c 006a 225f 2a7c 046a 1a7c  )|.j.|.j"_*|.j.|
-00000cf0: 006a 225f 2b7c 046a 1b7c 006a 225f 2c7c  .j"_+|.j.|.j"_,|
-00000d00: 046a 1c7c 006a 225f 2d7c 046a 1d7c 006a  .j.|.j"_-|.j.|.j
-00000d10: 225f 2e7c 046a 1e7c 006a 225f 2f7c 046a  "_.|.j.|.j"_/|.j
-00000d20: 1f7c 006a 225f 307c 046a 207c 006a 225f  .|.j"_0|.j |.j"_
-00000d30: 3174 326a 33a0 3474 326a 33a0 3574 32a0  1t2j3.4t2j3.5t2.
-00000d40: 36a1 0064 0ea1 02a1 017d 0674 326a 33a0  6..d.....}.t2j3.
-00000d50: 377c 06a1 0190 0273 3074 32a0 387c 06a1  7|.....s0t2.8|..
-00000d60: 0101 0074 326a 33a0 3474 326a 33a0 357c  ...t2j3.4t2j3.5|
-00000d70: 0664 0fa1 02a1 017d 0774 397c 0764 1083  .d.....}.t9|.d..
-00000d80: 027d 0874 3a64 117c 046a 129b 0064 127c  .}.t:d.|.j...d.|
-00000d90: 046a 139b 0064 137c 046a 149b 0064 147c  .j...d.|.j...d.|
-00000da0: 046a 159b 0064 157c 046a 169b 0064 167c  .j...d.|.j...d.|
-00000db0: 046a 179b 0064 177c 046a 189b 0064 187c  .j...d.|.j...d.|
-00000dc0: 046a 199b 0064 197c 046a 1a9b 0064 1a7c  .j...d.|.j...d.|
-00000dd0: 046a 1b9b 0064 1b7c 046a 1c9b 0064 1c7c  .j...d.|.j...d.|
-00000de0: 046a 1d9b 0064 1d7c 046a 1e9b 0064 1e7c  .j...d.|.j...d.|
-00000df0: 046a 1f9b 0064 1f7c 046a 209b 0064 209d  .j...d.|.j ..d .
-00000e00: 1f7c 0864 218d 0201 007c 08a0 3ba1 0001  .|.d!....|..;...
-00000e10: 0064 0053 0029 224e 723c 0000 0046 723d  .d.S.)"Nr<...Fr=
-00000e20: 0000 0072 3e00 0000 5472 0400 0000 7216  ...r>...Tr....r.
-00000e30: 0000 0072 1700 0000 721a 0000 0072 0300  ...r....r....r..
-00000e40: 0000 7219 0000 0072 1800 0000 721b 0000  ..r....r....r...
-00000e50: 00da 0351 5353 7a0f 5f76 6172 6961 626c  ...QSSz._variabl
-00000e60: 6573 2e73 6373 73da 0177 7ae0 0a20 2020  es.scss..wz..   
-00000e70: 2020 2020 202f 2f3d 3d3d 3d3d 3d3d 3d3d       //=========
-00000e80: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000e90: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000ea0: 3d3d 3d3d 3d3d 3d3d 3d3d 2f2f 0a20 2020  ==========//.   
-00000eb0: 2020 2020 202f 2f20 4649 4c45 2041 5554       // FILE AUT
-00000ec0: 4f2d 4745 4e45 5241 5445 442c 2041 4e59  O-GENERATED, ANY
-00000ed0: 2043 4841 4e47 4553 204d 4144 4520 5749   CHANGES MADE WI
-00000ee0: 4c4c 2042 4520 4c4f 5354 202f 2f0a 2020  LL BE LOST //.  
-00000ef0: 2020 2020 2020 2f2f 3d3d 3d3d 3d3d 3d3d        //========
-00000f00: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000f10: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000f20: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 2f2f 0a20  ============//. 
-00000f30: 2020 2020 2020 2024 434f 4c4f 525f 4241         $COLOR_BA
-00000f40: 434b 4752 4f55 4e44 5f31 3a20 7a1f 3b0a  CKGROUND_1: z.;.
-00000f50: 2020 2020 2020 2020 2443 4f4c 4f52 5f42          $COLOR_B
-00000f60: 4143 4b47 524f 554e 445f 323a 207a 1f3b  ACKGROUND_2: z.;
-00000f70: 0a20 2020 2020 2020 2024 434f 4c4f 525f  .        $COLOR_
-00000f80: 4241 434b 4752 4f55 4e44 5f33 3a20 7a20  BACKGROUND_3: z 
-00000f90: 3b20 0a20 2020 2020 2020 2024 434f 4c4f  ; .        $COLO
-00000fa0: 525f 4241 434b 4752 4f55 4e44 5f34 3a20  R_BACKGROUND_4: 
-00000fb0: 7a20 3b20 0a20 2020 2020 2020 2024 434f  z ; .        $CO
-00000fc0: 4c4f 525f 4241 434b 4752 4f55 4e44 5f35  LOR_BACKGROUND_5
-00000fd0: 3a20 7a20 3b20 0a20 2020 2020 2020 2024  : z ; .        $
-00000fe0: 434f 4c4f 525f 4241 434b 4752 4f55 4e44  COLOR_BACKGROUND
-00000ff0: 5f36 3a20 7a1a 3b20 0a20 2020 2020 2020  _6: z.; .       
-00001000: 2024 434f 4c4f 525f 5445 5854 5f31 3a20   $COLOR_TEXT_1: 
-00001010: 7a19 3b0a 2020 2020 2020 2020 2443 4f4c  z.;.        $COL
-00001020: 4f52 5f54 4558 545f 323a 207a 193b 0a20  OR_TEXT_2: z.;. 
-00001030: 2020 2020 2020 2024 434f 4c4f 525f 5445         $COLOR_TE
-00001040: 5854 5f33 3a20 7a19 3b0a 2020 2020 2020  XT_3: z.;.      
-00001050: 2020 2443 4f4c 4f52 5f54 4558 545f 343a    $COLOR_TEXT_4:
-00001060: 207a 1b3b 0a20 2020 2020 2020 2024 434f   z.;.        $CO
-00001070: 4c4f 525f 4143 4345 4e54 5f31 3a20 7a1b  LOR_ACCENT_1: z.
-00001080: 3b0a 2020 2020 2020 2020 2443 4f4c 4f52  ;.        $COLOR
-00001090: 5f41 4343 454e 545f 323a 207a 1b3b 0a20  _ACCENT_2: z.;. 
-000010a0: 2020 2020 2020 2024 434f 4c4f 525f 4143         $COLOR_AC
-000010b0: 4345 4e54 5f33 3a20 7a1b 3b0a 2020 2020  CENT_3: z.;.    
-000010c0: 2020 2020 2443 4f4c 4f52 5f41 4343 454e      $COLOR_ACCEN
-000010d0: 545f 343a 2061 9b01 0000 3b0a 2020 2020  T_4: a....;.    
-000010e0: 2020 2020 244f 5041 4349 5459 5f54 4f4f      $OPACITY_TOO
-000010f0: 4c54 4950 3a20 3233 303b 0a20 2020 2020  LTIP: 230;.     
-00001100: 2020 2024 5349 5a45 5f42 4f52 4445 525f     $SIZE_BORDER_
-00001110: 5241 4449 5553 3a20 3470 783b 0a20 2020  RADIUS: 4px;.   
-00001120: 2020 2020 2024 424f 5244 4552 5f31 3a20       $BORDER_1: 
-00001130: 3170 7820 736f 6c69 6420 2443 4f4c 4f52  1px solid $COLOR
-00001140: 5f42 4143 4b47 524f 554e 445f 313b 0a20  _BACKGROUND_1;. 
-00001150: 2020 2020 2020 2024 424f 5244 4552 5f32         $BORDER_2
-00001160: 3a20 3170 7820 736f 6c69 6420 2443 4f4c  : 1px solid $COL
-00001170: 4f52 5f42 4143 4b47 524f 554e 445f 343b  OR_BACKGROUND_4;
-00001180: 0a20 2020 2020 2020 2024 424f 5244 4552  .        $BORDER
-00001190: 5f33 3a20 3170 7820 736f 6c69 6420 2443  _3: 1px solid $C
-000011a0: 4f4c 4f52 5f42 4143 4b47 524f 554e 445f  OLOR_BACKGROUND_
-000011b0: 363b 0a20 2020 2020 2020 2024 424f 5244  6;.        $BORD
-000011c0: 4552 5f53 454c 4543 5449 4f4e 5f33 3a20  ER_SELECTION_3: 
-000011d0: 3170 7820 736f 6c69 6420 2443 4f4c 4f52  1px solid $COLOR
-000011e0: 5f41 4343 454e 545f 333b 0a20 2020 2020  _ACCENT_3;.     
-000011f0: 2020 2024 424f 5244 4552 5f53 454c 4543     $BORDER_SELEC
-00001200: 5449 4f4e 5f32 3a20 3170 7820 736f 6c69  TION_2: 1px soli
-00001210: 6420 2443 4f4c 4f52 5f41 4343 454e 545f  d $COLOR_ACCENT_
-00001220: 323b 0a20 2020 2020 2020 2024 424f 5244  2;.        $BORD
-00001230: 4552 5f53 454c 4543 5449 4f4e 5f31 3a20  ER_SELECTION_1: 
-00001240: 3170 7820 736f 6c69 6420 2443 4f4c 4f52  1px solid $COLOR
-00001250: 5f41 4343 454e 545f 313b 0a20 2020 2020  _ACCENT_1;.     
-00001260: 2020 2024 5041 5448 5f52 4553 4f55 5243     $PATH_RESOURC
-00001270: 4553 3a20 277a 9e27 3b0a 2020 2020 2020  ES: 'z.';.      
-00001280: 2020 2f2f 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d    //============
-00001290: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000012a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000012b0: 3d3d 3d3d 3d3d 3d2f 2f0a 2020 2020 2020  =======//.      
-000012c0: 2020 2f2f 2045 4e44 202f 2f0a 2020 2020    // END //.    
-000012d0: 2020 2020 2f2f 3d3d 3d3d 3d3d 3d3d 3d3d      //==========
-000012e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000012f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00001300: 3d3d 3d3d 3d3d 3d3d 3d3d 2f2f 0a20 2020  ==========//.   
-00001310: 2020 2020 2029 01da 0466 696c 6529 3c72       )...file)<r
-00001320: 3f00 0000 7240 0000 0072 3300 0000 7214  ?...r@...r3...r.
-00001330: 0000 0072 4100 0000 7242 0000 0072 4300  ...rA...rB...rC.
-00001340: 0000 7244 0000 0072 4500 0000 7246 0000  ..rD...rE...rF..
-00001350: 0072 2000 0000 7247 0000 0072 2100 0000  .r ...rG...r!...
-00001360: 7248 0000 0072 2200 0000 724a 0000 0072  rH...r"...rJ...r
-00001370: 2300 0000 7211 0000 0072 2400 0000 7225  #...r....r$...r%
-00001380: 0000 0072 2600 0000 7227 0000 0072 2800  ...r&...r'...r(.
-00001390: 0000 7229 0000 0072 2a00 0000 722b 0000  ..r)...r*...r+..
-000013a0: 0072 2c00 0000 722d 0000 0072 2e00 0000  .r,...r-...r....
-000013b0: 722f 0000 0072 3000 0000 7231 0000 0072  r/...r0...r1...r
-000013c0: 3200 0000 da06 4f62 6a65 6374 724d 0000  2.....ObjectrM..
-000013d0: 005a 1243 4f4c 4f52 5f42 4143 4b47 524f  .Z.COLOR_BACKGRO
-000013e0: 554e 445f 315a 1243 4f4c 4f52 5f42 4143  UND_1Z.COLOR_BAC
-000013f0: 4b47 524f 554e 445f 32da 1243 4f4c 4f52  KGROUND_2..COLOR
-00001400: 5f42 4143 4b47 524f 554e 445f 33da 1243  _BACKGROUND_3..C
-00001410: 4f4c 4f52 5f42 4143 4b47 524f 554e 445f  OLOR_BACKGROUND_
-00001420: 345a 1243 4f4c 4f52 5f42 4143 4b47 524f  4Z.COLOR_BACKGRO
-00001430: 554e 445f 355a 1243 4f4c 4f52 5f42 4143  UND_5Z.COLOR_BAC
-00001440: 4b47 524f 554e 445f 36da 0c43 4f4c 4f52  KGROUND_6..COLOR
-00001450: 5f54 4558 545f 315a 0c43 4f4c 4f52 5f54  _TEXT_1Z.COLOR_T
-00001460: 4558 545f 325a 0c43 4f4c 4f52 5f54 4558  EXT_2Z.COLOR_TEX
-00001470: 545f 335a 0c43 4f4c 4f52 5f54 4558 545f  T_3Z.COLOR_TEXT_
-00001480: 34da 0e43 4f4c 4f52 5f41 4343 454e 545f  4..COLOR_ACCENT_
-00001490: 31da 0e43 4f4c 4f52 5f41 4343 454e 545f  1..COLOR_ACCENT_
-000014a0: 32da 0e43 4f4c 4f52 5f41 4343 454e 545f  2..COLOR_ACCENT_
-000014b0: 33da 0e43 4f4c 4f52 5f41 4343 454e 545f  3..COLOR_ACCENT_
-000014c0: 345a 0e50 4154 485f 5245 534f 5552 4345  4Z.PATH_RESOURCE
-000014d0: 53da 026f 73da 0470 6174 68da 0761 6273  S..os..path..abs
-000014e0: 7061 7468 da04 6a6f 696e da06 6765 7463  path..join..getc
-000014f0: 7764 da06 6578 6973 7473 da08 6d61 6b65  wd..exists..make
-00001500: 6469 7273 da04 6f70 656e da05 7072 696e  dirs..open..prin
-00001510: 74da 0563 6c6f 7365 2909 7238 0000 0072  t..close).r8...r
-00001520: 4c00 0000 723c 0000 005a 0a74 6865 6d65  L...r<...Z.theme
-00001530: 466f 756e 6472 4d00 0000 7242 0000 005a  FoundrM...rB...Z
-00001540: 0b73 6373 735f 666f 6c64 6572 da09 7363  .scss_folder..sc
-00001550: 7373 5f70 6174 68da 0166 720f 0000 0072  ss_path..fr....r
-00001560: 0f00 0000 7210 0000 00da 0f43 7265 6174  ....r......Creat
-00001570: 6556 6172 6961 626c 6573 a700 0000 73b0  eVariables....s.
-00001580: 0000 0000 0106 020a 0104 0108 010a 0208  ................
-00001590: 010a 030c 0110 020e 0204 0108 0108 0108  ................
-000015a0: 0108 0106 0204 0106 030e 010e 010e 010e  ................
-000015b0: 010e 010e 020e 010e 010e 010e 020e 010e  ................
-000015c0: 010e 010e 0206 0308 010a 010a 010a 010a  ................
-000015d0: 010a 010a 020a 010a 010a 010a 020a 010a  ................
-000015e0: 010a 010a 020a 031a 010e 010a 0216 010a  ................
-000015f0: 0104 0404 fc04 0504 fb04 0604 fa04 0704  ................
-00001600: f904 0804 f804 0904 f704 0a04 f604 0b04  ................
-00001610: f504 0c04 f404 0d04 f304 0e04 f204 0f04  ................
-00001620: f104 1004 f004 1104 ef04 1a04 e606 1e02  ................
-00001630: e206 207a 2343 7265 6174 6543 6f6c 6f72  .. z#CreateColor
-00001640: 5661 7269 6162 6c65 2e43 7265 6174 6556  Variable.CreateV
-00001650: 6172 6961 626c 6573 2901 4e29 0772 1d00  ariables).N).r..
-00001660: 0000 721e 0000 0072 1f00 0000 7237 0000  ..r....r....r7..
-00001670: 0072 4e00 0000 7266 0000 00da 0d5f 5f63  .rN...rf.....__c
-00001680: 6c61 7373 6365 6c6c 5f5f 720f 0000 0072  lasscell__r....r
-00001690: 0f00 0000 723a 0000 0072 1000 0000 7235  ....r:...r....r5
-000016a0: 0000 006a 0000 0073 0600 0000 0801 0e03  ...j...s........
-000016b0: 0839 7235 0000 0063 0000 0000 0000 0000  .9r5...c........
-000016c0: 0000 0000 0000 0000 0100 0000 4000 0000  ............@...
-000016d0: 730c 0000 0065 005a 0164 005a 0264 0153  s....e.Z.d.Z.d.S
-000016e0: 0029 0272 5200 0000 4e29 0372 1d00 0000  .).rR...N).r....
-000016f0: 721e 0000 0072 1f00 0000 720f 0000 0072  r....r....r....r
-00001700: 0f00 0000 720f 0000 0072 1000 0000 7252  ....r....r....rR
-00001710: 0000 0017 0100 0073 0200 0000 0801 7252  .......s......rR
-00001720: 0000 0029 0172 0300 0000 2910 725a 0000  ...).r....).rZ..
-00001730: 00da 0373 7973 da0e 5079 5369 6465 322e  ...sys..PySide2.
-00001740: 5174 436f 7265 5a11 6d61 7470 6c6f 746c  QtCoreZ.matplotl
-00001750: 6962 2e63 6f6c 6f72 73da 0663 6f6c 6f72  ib.colors..color
-00001760: 7372 0700 0000 7208 0000 0072 3f00 0000  sr....r....r?...
-00001770: 724c 0000 0072 1100 0000 7209 0000 0072  rL...r....r....r
-00001780: 1400 0000 7233 0000 0072 3500 0000 da06  ....r3...r5.....
-00001790: 6f62 6a65 6374 7252 0000 0072 0f00 0000  objectrR...r....
-000017a0: 720f 0000 0072 0f00 0000 7210 0000 00da  r....r....r.....
-000017b0: 083c 6d6f 6475 6c65 3e08 0000 0073 1800  .<module>....s..
-000017c0: 0000 0801 0804 0802 0c01 0802 0606 0a0f  ................
-000017d0: 0808 0e1b 0e20 0e7f 002e                 ..... ....
+00000080: 4700 640a 640b 8400 640b 650b 8303 5a0c  G.d.d...d.e...Z.
+00000090: 4700 640c 640d 8400 640d 650b 8303 5a0d  G.d.d...d.e...Z.
+000000a0: 4700 640e 640f 8400 640f 8302 5a0e 4700  G.d.d...d...Z.G.
+000000b0: 6410 6411 8400 6411 650f 8303 5a10 6401  d.d...d.e...Z.d.
+000000c0: 5300 2913 e900 0000 004e 2901 da01 2ae7  S.)......N)...*.
+000000d0: 0000 0000 0000 e03f 6302 0000 0000 0000  .......?c.......
+000000e0: 0000 0000 0005 0000 0008 0000 0043 0000  .............C..
+000000f0: 0073 c800 0000 7a0e 7400 6a01 7c00 1900  .s....z.t.j.|...
+00000100: 7d02 5700 6e18 0400 7402 6b0a 7226 0100  }.W.n...t.k.r&..
+00000110: 0100 0100 7c00 7d02 5900 6e02 5800 7403  ....|.}.Y.n.X.t.
+00000120: 6a04 7400 a005 7c02 a101 8e00 7d02 7406  j.t...|.....}.t.
+00000130: 7c02 8301 0100 7c02 6401 1900 6402 6b04  |.....|.d...d.k.
+00000140: 726c 7403 a007 7c02 6402 1900 7c01 7c02  rlt...|.d...|.|.
+00000150: 6401 1900 1400 7c02 6403 1900 a103 7d03  d.....|.d.....}.
+00000160: 6e26 7403 a007 7c02 6402 1900 6401 7c01  n&t...|.d...d.|.
+00000170: 6401 7c02 6401 1900 1800 1400 1800 7c02  d.|.d.........|.
+00000180: 6403 1900 a103 7d03 7408 7409 7c03 6402  d.....}.t.t.|.d.
+00000190: 1900 6404 1400 8301 7409 7c03 6401 1900  ..d.....t.|.d...
+000001a0: 6404 1400 8301 7409 7c03 6403 1900 6404  d.....t.|.d...d.
+000001b0: 1400 8301 6603 8301 7d04 7c04 5300 2905  ....f...}.|.S.).
+000001c0: 4ee9 0100 0000 7201 0000 00e9 0200 0000  N.....r.........
+000001d0: e9fa 0000 0029 0ada 026d 635a 0663 6e61  .....)...mcZ.cna
+000001e0: 6d65 73da 084b 6579 4572 726f 72da 0863  mes..KeyError..c
+000001f0: 6f6c 6f72 7379 735a 0a72 6762 5f74 6f5f  olorsysZ.rgb_to_
+00000200: 686c 735a 0674 6f5f 7267 62da 0570 7269  hlsZ.to_rgb..pri
+00000210: 6e74 5a0a 686c 735f 746f 5f72 6762 da0a  ntZ.hls_to_rgb..
+00000220: 7267 625f 746f 5f68 6578 da03 696e 7429  rgb_to_hex..int)
+00000230: 05da 0563 6f6c 6f72 da06 616d 6f75 6e74  ...color..amount
+00000240: da01 63da 0372 6762 5a09 6e65 775f 636f  ..c..rgbZ.new_co
+00000250: 6c6f 72a9 0072 1100 0000 fa46 653a 5c53  lor..r.....Fe:\S
+00000260: 7069 6e6e 2054 6173 6b5c 3070 6173 735c  pinn Task\0pass\
+00000270: 3070 6173 732d 6170 702d 6d61 7374 6572  0pass-app-master
+00000280: 5c43 7573 746f 6d5f 5769 6467 6574 735c  \Custom_Widgets\
+00000290: 5173 735c 636f 6c6f 7273 7973 7465 6d2e  Qss\colorsystem.
+000002a0: 7079 da10 6164 6a75 7374 5f6c 6967 6874  py..adjust_light
+000002b0: 6e65 7373 1e00 0000 7316 0000 0000 0102  ness....s.......
+000002c0: 010e 010e 010a 0110 0108 020c 0120 0226  ............. .&
+000002d0: 0232 0172 1300 0000 6301 0000 0000 0000  .2.r....c.......
+000002e0: 0000 0000 0002 0000 0002 0000 0043 0000  .............C..
+000002f0: 0073 1000 0000 6401 7c00 1600 7d01 6402  .s....d.|...}.d.
+00000300: 7c01 1700 5300 2903 4e7a 0c25 3032 7825  |...S.).Nz.%02x%
+00000310: 3032 7825 3032 78fa 0123 7211 0000 0029  02x%02x..#r....)
+00000320: 0272 1000 0000 5a09 6865 785f 636f 6c6f  .r....Z.hex_colo
+00000330: 7272 1100 0000 7211 0000 0072 1200 0000  rr....r....r....
+00000340: 720b 0000 002f 0000 0073 0400 0000 0001  r..../...s......
+00000350: 0801 720b 0000 0063 0000 0000 0000 0000  ..r....c........
+00000360: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
+00000370: 7316 0000 0065 005a 0164 005a 0264 0564  s....e.Z.d.Z.d.d
+00000380: 0264 0384 015a 0364 0453 0029 06da 0554  .d...Z.d.S.)...T
+00000390: 6865 6d65 da00 6305 0000 0000 0000 0000  heme..c.........
+000003a0: 0000 0005 0000 0003 0000 0043 0000 0073  ...........C...s
+000003b0: ca00 0000 7c01 7c00 5f00 7c02 7c00 5f01  ....|.|._.|.|._.
+000003c0: 7c03 7c00 5f02 7c04 7c00 5f03 7404 7c01  |.|._.|.|._.t.|.
+000003d0: 6401 8302 7c00 5f05 7404 7c01 6402 8302  d...|._.t.|.d...
+000003e0: 7c00 5f06 7404 7c01 6403 8302 7c00 5f07  |._.t.|.d...|._.
+000003f0: 7404 7c01 6404 8302 7c00 5f08 7404 7c01  t.|.d...|._.t.|.
+00000400: 6405 8302 7c00 5f09 7404 7c01 6406 8302  d...|._.t.|.d...
+00000410: 7c00 5f0a 7404 7c02 6401 8302 7c00 5f0b  |._.t.|.d...|._.
+00000420: 7404 7c02 6407 8302 7c00 5f0c 7404 7c02  t.|.d...|._.t.|.
+00000430: 6403 8302 7c00 5f0d 7404 7c02 6408 8302  d...|._.t.|.d...
+00000440: 7c00 5f0e 7404 7c03 6401 8302 7c00 5f0f  |._.t.|.d...|._.
+00000450: 7404 7c03 6407 8302 7c00 5f10 7404 7c03  t.|.d...|._.t.|.
+00000460: 6403 8302 7c00 5f11 7404 7c03 6408 8302  d...|._.t.|.d...
+00000470: 7c00 5f12 6409 7c00 5f13 6400 5300 290a  |._.d.|._.d.S.).
+00000480: 4e72 0400 0000 6766 6666 6666 66ee 3fe7  Nr....gffffff.?.
+00000490: 9a99 9999 9999 e93f 6700 0000 0000 00e8  .......?g.......
+000004a0: 3fe7 3333 3333 3333 e33f 679a 9999 9999  ?.333333.?g.....
+000004b0: 99e1 3fe7 cdcc cccc cccc ec3f e766 6666  ..?........?.fff
+000004c0: 6666 66e6 3ffa 0e3a 2f69 636f 6e73 2f49  fff.?..:/icons/I
+000004d0: 636f 6e73 2f29 14da 0862 675f 636f 6c6f  cons/)...bg_colo
+000004e0: 72da 0974 7874 5f63 6f6c 6f72 da0c 6163  r..txt_color..ac
+000004f0: 6365 6e74 5f63 6f6c 6f72 da0b 6963 6f6e  cent_color..icon
+00000500: 735f 636f 6c6f 7272 1300 0000 da04 4247  s_colorr......BG
+00000510: 5f31 da04 4247 5f32 da04 4247 5f33 da04  _1..BG_2..BG_3..
+00000520: 4247 5f34 da04 4247 5f35 da04 4247 5f36  BG_4..BG_5..BG_6
+00000530: da04 4354 5f31 da04 4354 5f32 da04 4354  ..CT_1..CT_2..CT
+00000540: 5f33 da04 4354 5f34 da04 4341 5f31 da04  _3..CT_4..CA_1..
+00000550: 4341 5f32 da04 4341 5f33 da04 4341 5f34  CA_2..CA_3..CA_4
+00000560: da05 4943 4f4e 5329 05da 0473 656c 6672  ..ICONS)...selfr
+00000570: 1c00 0000 721d 0000 0072 1e00 0000 721f  ....r....r....r.
+00000580: 0000 0072 1100 0000 7211 0000 0072 1200  ...r....r....r..
+00000590: 0000 da08 5f5f 696e 6974 5f5f 3400 0000  ....__init__4...
+000005a0: 7326 0000 0000 0106 0106 0106 0106 020c  s&..............
+000005b0: 010c 010c 010c 010c 010c 020c 010c 010c  ................
+000005c0: 010c 020c 010c 010c 010c 027a 0e54 6865  ...........z.The
+000005d0: 6d65 2e5f 5f69 6e69 745f 5f4e 2901 7216  me.__init__N).r.
+000005e0: 0000 0029 04da 085f 5f6e 616d 655f 5fda  ...)...__name__.
+000005f0: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+00000600: 7561 6c6e 616d 655f 5f72 3000 0000 7211  ualname__r0...r.
+00000610: 0000 0072 1100 0000 7211 0000 0072 1200  ...r....r....r..
+00000620: 0000 7215 0000 0033 0000 0073 0200 0000  ..r....3...s....
+00000630: 0801 7215 0000 0063 0000 0000 0000 0000  ..r....c........
+00000640: 0000 0000 0000 0000 0300 0000 0000 0000  ................
+00000650: 731c 0000 0065 005a 0164 005a 0287 0066  s....e.Z.d.Z...f
+00000660: 0164 0164 0284 085a 0387 0004 005a 0453  .d.d...Z.....Z.S
+00000670: 0029 03da 0444 6172 6b63 0100 0000 0000  .)...Darkc......
+00000680: 0000 0000 0000 0100 0000 0500 0000 0300  ................
+00000690: 0000 7314 0000 0074 0083 00a0 0164 0164  ..s....t.....d.d
+000006a0: 0264 03a1 0301 0064 0053 0029 044e 7a07  .d.....d.S.).Nz.
+000006b0: 2330 4430 4431 34fa 0423 6666 667a 0723  #0D0D14..#fffz.#
+000006c0: 4138 4239 4244 a902 da05 7375 7065 7272  A8B9BD....superr
+000006d0: 3000 0000 a901 722f 0000 00a9 01da 095f  0.....r/......._
+000006e0: 5f63 6c61 7373 5f5f 7211 0000 0072 1200  _class__r....r..
+000006f0: 0000 7230 0000 004e 0000 0073 0200 0000  ..r0...N...s....
+00000700: 0001 7a0d 4461 726b 2e5f 5f69 6e69 745f  ..z.Dark.__init_
+00000710: 5fa9 0572 3100 0000 7232 0000 0072 3300  _..r1...r2...r3.
+00000720: 0000 7230 0000 00da 0d5f 5f63 6c61 7373  ..r0.....__class
+00000730: 6365 6c6c 5f5f 7211 0000 0072 1100 0000  cell__r....r....
+00000740: 7239 0000 0072 1200 0000 7234 0000 004d  r9...r....r4...M
+00000750: 0000 0073 0200 0000 0801 7234 0000 0063  ...s......r4...c
+00000760: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000770: 0300 0000 0000 0000 731c 0000 0065 005a  ........s....e.Z
+00000780: 0164 005a 0287 0066 0164 0164 0284 085a  .d.Z...f.d.d...Z
+00000790: 0387 0004 005a 0453 0029 03da 054c 6967  .....Z.S.)...Lig
+000007a0: 6874 6301 0000 0000 0000 0000 0000 0001  htc.............
+000007b0: 0000 0005 0000 0003 0000 0073 1400 0000  ...........s....
+000007c0: 7400 8300 a001 6401 6402 6403 a103 0100  t.....d.d.d.....
+000007d0: 6400 5300 2904 4e72 3500 0000 7a04 2330  d.S.).Nr5...z.#0
+000007e0: 3030 7a07 2330 3062 6366 6672 3600 0000  00z.#00bcffr6...
+000007f0: 7238 0000 0072 3900 0000 7211 0000 0072  r8...r9...r....r
+00000800: 1200 0000 7230 0000 0052 0000 0073 0200  ....r0...R...s..
+00000810: 0000 0001 7a0e 4c69 6768 742e 5f5f 696e  ....z.Light.__in
+00000820: 6974 5f5f 723b 0000 0072 1100 0000 7211  it__r;...r....r.
+00000830: 0000 0072 3900 0000 7212 0000 0072 3d00  ...r9...r....r=.
+00000840: 0000 5100 0000 7302 0000 0008 0172 3d00  ..Q...s......r=.
+00000850: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00000860: 0000 0004 0000 0000 0000 0073 2e00 0000  ...........s....
+00000870: 6500 5a01 6400 5a02 6408 8700 6601 6402  e.Z.d.Z.d...f.d.
+00000880: 6403 8409 5a03 6404 6405 8400 5a04 6406  d...Z.d.d...Z.d.
+00000890: 6407 8400 5a05 8700 0400 5a06 5300 2909  d...Z.....Z.S.).
+000008a0: da13 4372 6561 7465 436f 6c6f 7256 6172  ..CreateColorVar
+000008b0: 6961 626c 654e 6302 0000 0000 0000 0000  iableNc.........
+000008c0: 0000 0002 0000 0003 0000 0003 0000 0073  ...............s
+000008d0: 1400 0000 7400 7401 7c00 8302 a002 7c01  ....t.t.|.....|.
+000008e0: a101 0100 6400 5300 2901 4e29 0372 3700  ....d.S.).N).r7.
+000008f0: 0000 723e 0000 0072 3000 0000 2902 722f  ..r>...r0...).r/
+00000900: 0000 00da 0670 6172 656e 7472 3900 0000  .....parentr9...
+00000910: 7211 0000 0072 1200 0000 7230 0000 005e  r....r....r0...^
+00000920: 0000 0073 0200 0000 0001 7a1c 4372 6561  ...s......z.Crea
+00000930: 7465 436f 6c6f 7256 6172 6961 626c 652e  teColorVariable.
+00000940: 5f5f 696e 6974 5f5f 6301 0000 0000 0000  __init__c.......
+00000950: 0000 0000 0009 0000 0006 0000 0043 0000  .............C..
+00000960: 0073 5001 0000 7400 8300 7d01 7c01 a001  .sP...t...}.|...
+00000970: 6401 a101 7d02 6900 7d03 7c02 6402 6b02  d...}.i.}.|.d.k.
+00000980: 7258 7402 8300 7d04 7c04 6a03 6403 6b02  rXt...}.|.j.d.k.
+00000990: 723c 7c04 6a04 7d05 7c04 6a04 7c04 5f03  r<|.j.}.|.j.|._.
+000009a0: 6e06 7c04 6a03 7d05 7c04 6a05 7c04 6a06  n.|.j.}.|.j.|.j.
+000009b0: 7c04 6a04 7c05 6404 9c04 7d03 6eb2 7c02  |.j.|.d...}.n.|.
+000009c0: 6405 6b02 729c 7407 8300 7d04 7c04 6a03  d.k.r.t...}.|.j.
+000009d0: 6403 6b02 7280 7c04 6a04 7d05 7c04 6a04  d.k.r.|.j.}.|.j.
+000009e0: 7c04 5f03 6e06 7c04 6a03 7d05 7c04 6a05  |._.n.|.j.}.|.j.
+000009f0: 7c04 6a06 7c04 6a04 7c05 6404 9c04 7d03  |.j.|.j.|.d...}.
+00000a00: 6e6e 7c00 6a08 6a09 4400 5d64 7d04 7c04  nn|.j.j.D.]d}.|.
+00000a10: 6a0a 73b8 7c04 6a0b 7c02 6b02 72a4 7c01  j.s.|.j.|.k.r.|.
+00000a20: a00c 6401 7c04 6a0b a102 0100 7c04 6a0d  ..d.|.j.....|.j.
+00000a30: 7d06 7c04 6a0e 7d07 7c04 6a0f 7d08 7c04  }.|.j.}.|.j.}.|.
+00000a40: 6a10 72f6 7c04 6a11 6403 6b02 72ee 7c08  j.r.|.j.d.k.r.|.
+00000a50: 7d05 71fa 7c04 6a11 7d05 6e04 6400 7d05  }.q.|.j.}.n.d.}.
+00000a60: 7c06 7c07 7c08 7c05 6404 9c04 7d03 71a4  |.|.|.|.d...}.q.
+00000a70: 7412 7c03 8301 6406 6b02 9001 724c 7402  t.|...d.k...rLt.
+00000a80: 8300 7d04 7c04 6a03 6403 6b02 9001 7232  ..}.|.j.d.k...r2
+00000a90: 7c04 6a04 7d05 6e06 7c04 6a03 7d05 7c04  |.j.}.n.|.j.}.|.
+00000aa0: 6a05 7c04 6a06 7c04 6a04 7c05 6404 9c04  j.|.j.|.j.|.d...
+00000ab0: 7d03 7c03 5300 2907 4eda 0554 4845 4d45  }.|.S.).N..THEME
+00000ac0: da05 4c49 4748 5472 1600 0000 2904 7a10  ..LIGHTr....).z.
+00000ad0: 6261 636b 6772 6f75 6e64 2d63 6f6c 6f72  background-color
+00000ae0: 7a0a 7465 7874 2d63 6f6c 6f72 7a0c 6163  z.text-colorz.ac
+00000af0: 6365 6e74 2d63 6f6c 6f72 7a0b 6963 6f6e  cent-colorz.icon
+00000b00: 732d 636f 6c6f 72da 0444 4152 4b72 0100  s-color..DARKr..
+00000b10: 0000 2913 da09 5153 6574 7469 6e67 73da  ..)...QSettings.
+00000b20: 0576 616c 7565 723d 0000 0072 1f00 0000  .valuer=...r....
+00000b30: 721e 0000 0072 1c00 0000 721d 0000 0072  r....r....r....r
+00000b40: 3400 0000 da02 7569 da06 7468 656d 6573  4.....ui..themes
+00000b50: da0c 6465 6661 756c 7454 6865 6d65 da04  ..defaultTheme..
+00000b60: 6e61 6d65 da08 7365 7456 616c 7565 da0f  name..setValue..
+00000b70: 6261 636b 6772 6f75 6e64 436f 6c6f 72da  backgroundColor.
+00000b80: 0974 6578 7443 6f6c 6f72 da0b 6163 6365  .textColor..acce
+00000b90: 6e74 436f 6c6f 72da 0e63 7265 6174 654e  ntColor..createN
+00000ba0: 6577 4963 6f6e 73da 0a69 636f 6e73 436f  ewIcons..iconsCo
+00000bb0: 6c6f 72da 036c 656e 2909 722f 0000 00da  lor..len).r/....
+00000bc0: 0873 6574 7469 6e67 7372 4000 0000 5a10  .settingsr@...Z.
+00000bd0: 6375 7272 656e 7454 6865 6d65 496e 666f  currentThemeInfo
+00000be0: da05 7468 656d 6572 4e00 0000 721c 0000  ..themerN...r...
+00000bf0: 0072 1d00 0000 721e 0000 0072 1100 0000  .r....r....r....
+00000c00: 7211 0000 0072 1200 0000 da13 6765 7443  r....r......getC
+00000c10: 7572 7265 6e74 5468 656d 6549 6e66 6f61  urrentThemeInfoa
+00000c20: 0000 0073 4800 0000 0001 0602 0a02 0402  ...sH...........
+00000c30: 0801 0601 0a01 0601 0a02 0602 1602 0801  ................
+00000c40: 0601 0a01 0601 0a02 0602 1603 0c01 1002  ................
+00000c50: 0e01 0601 0601 0602 0601 0a01 0602 0802  ................
+00000c60: 0402 1002 0e01 0601 0c01 0802 0602 1402  ................
+00000c70: 7a27 4372 6561 7465 436f 6c6f 7256 6172  z'CreateColorVar
+00000c80: 6961 626c 652e 6765 7443 7572 7265 6e74  iable.getCurrent
+00000c90: 5468 656d 6549 6e66 6f63 0100 0000 0000  ThemeInfoc......
+00000ca0: 0000 0000 0000 0900 0000 2000 0000 4300  .......... ...C.
+00000cb0: 0000 73e2 0200 0074 0083 007d 017c 01a0  ..s....t...}.|..
+00000cc0: 0164 01a1 017d 0264 027d 037c 0264 036b  .d...}.d.}.|.d.k
+00000cd0: 0272 2674 0283 007d 0490 016e 3a7c 0264  .r&t...}...n:|.d
+00000ce0: 046b 0272 3874 0383 007d 0490 016e 287c  .k.r8t...}...n(|
+00000cf0: 006a 046a 0544 005d 4a7d 057c 056a 0673  .j.j.D.]J}.|.j.s
+00000d00: 547c 056a 077c 026b 0272 407c 01a0 0864  T|.j.|.k.r@|...d
+00000d10: 017c 056a 07a1 0201 007c 057d 047c 056a  .|.j.....|.}.|.j
+00000d20: 097c 045f 0a7c 056a 0b7c 045f 0c7c 056a  .|._.|.j.|._.|.j
+00000d30: 0d7c 045f 0e7c 046a 0f7c 045f 1064 057d  .|._.|.j.|._.d.}
+00000d40: 0371 407c 0373 9674 0283 007d 0474 117c  .q@|.s.t...}.t.|
+00000d50: 046a 0a64 0683 027c 045f 1274 117c 046a  .j.d...|._.t.|.j
+00000d60: 0a64 0783 027c 045f 1374 117c 046a 0a64  .d...|._.t.|.j.d
+00000d70: 0883 027c 045f 1474 117c 046a 0a64 0983  ...|._.t.|.j.d..
+00000d80: 027c 045f 1574 117c 046a 0a64 0a83 027c  .|._.t.|.j.d...|
+00000d90: 045f 1674 117c 046a 0a64 0b83 027c 045f  ._.t.|.j.d...|._
+00000da0: 1774 117c 046a 0c64 0683 027c 045f 1874  .t.|.j.d...|._.t
+00000db0: 117c 046a 0c64 0783 027c 045f 1974 117c  .|.j.d...|._.t.|
+00000dc0: 046a 0c64 0883 027c 045f 1a74 117c 046a  .j.d...|._.t.|.j
+00000dd0: 0c64 0983 027c 045f 1b74 117c 046a 0e64  .d...|._.t.|.j.d
+00000de0: 0683 027c 045f 1c74 117c 046a 0e64 0783  ...|._.t.|.j.d..
+00000df0: 027c 045f 1d74 117c 046a 0e64 0883 027c  .|._.t.|.j.d...|
+00000e00: 045f 1e74 117c 046a 0e64 0983 027c 045f  ._.t.|.j.d...|._
+00000e10: 1f64 0c7c 045f 2074 2183 007c 005f 227c  .d.|._ t!..|._"|
+00000e20: 046a 127c 006a 225f 237c 046a 137c 006a  .j.|.j"_#|.j.|.j
+00000e30: 225f 247c 046a 147c 006a 225f 257c 046a  "_$|.j.|.j"_%|.j
+00000e40: 157c 006a 225f 267c 046a 167c 006a 225f  .|.j"_&|.j.|.j"_
+00000e50: 277c 046a 177c 006a 225f 287c 046a 187c  '|.j.|.j"_(|.j.|
+00000e60: 006a 225f 297c 046a 197c 006a 225f 2a7c  .j"_)|.j.|.j"_*|
+00000e70: 046a 1a7c 006a 225f 2b7c 046a 1b7c 006a  .j.|.j"_+|.j.|.j
+00000e80: 225f 2c7c 046a 1c7c 006a 225f 2d7c 046a  "_,|.j.|.j"_-|.j
+00000e90: 1d7c 006a 225f 2e7c 046a 1e7c 006a 225f  .|.j"_.|.j.|.j"_
+00000ea0: 2f7c 046a 1f7c 006a 225f 307c 046a 207c  /|.j.|.j"_0|.j |
+00000eb0: 006a 225f 3174 326a 33a0 3474 326a 33a0  .j"_1t2j3.4t2j3.
+00000ec0: 3574 32a0 36a1 0064 0da1 02a1 017d 0674  5t2.6..d.....}.t
+00000ed0: 326a 33a0 377c 06a1 0190 0273 3074 32a0  2j3.7|.....s0t2.
+00000ee0: 387c 06a1 0101 0074 326a 33a0 3474 326a  8|.....t2j3.4t2j
+00000ef0: 33a0 357c 0664 0ea1 02a1 017d 0774 397c  3.5|.d.....}.t9|
+00000f00: 0764 0f83 027d 0874 3a64 107c 046a 129b  .d...}.t:d.|.j..
+00000f10: 0064 117c 046a 139b 0064 127c 046a 149b  .d.|.j...d.|.j..
+00000f20: 0064 137c 046a 159b 0064 147c 046a 169b  .d.|.j...d.|.j..
+00000f30: 0064 157c 046a 179b 0064 167c 046a 189b  .d.|.j...d.|.j..
+00000f40: 0064 177c 046a 199b 0064 187c 046a 1a9b  .d.|.j...d.|.j..
+00000f50: 0064 197c 046a 1b9b 0064 1a7c 046a 1c9b  .d.|.j...d.|.j..
+00000f60: 0064 1b7c 046a 1d9b 0064 1c7c 046a 1e9b  .d.|.j...d.|.j..
+00000f70: 0064 1d7c 046a 1f9b 0064 1e7c 046a 209b  .d.|.j...d.|.j .
+00000f80: 0064 1f9d 1f7c 0864 208d 0201 007c 08a0  .d...|.d ....|..
+00000f90: 3ba1 0001 0064 0053 0029 214e 7240 0000  ;....d.S.)!Nr@..
+00000fa0: 0046 7241 0000 0072 4200 0000 5472 0400  .FrA...rB...Tr..
+00000fb0: 0000 7219 0000 0072 1700 0000 721a 0000  ..r....r....r...
+00000fc0: 0072 1800 0000 7203 0000 0072 1b00 0000  .r....r....r....
+00000fd0: da03 5153 537a 0f5f 7661 7269 6162 6c65  ..QSSz._variable
+00000fe0: 732e 7363 7373 da01 777a e00a 2020 2020  s.scss..wz..    
+00000ff0: 2020 2020 2f2f 3d3d 3d3d 3d3d 3d3d 3d3d      //==========
+00001000: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00001010: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00001020: 3d3d 3d3d 3d3d 3d3d 3d2f 2f0a 2020 2020  =========//.    
+00001030: 2020 2020 2f2f 2046 494c 4520 4155 544f      // FILE AUTO
+00001040: 2d47 454e 4552 4154 4544 2c20 414e 5920  -GENERATED, ANY 
+00001050: 4348 414e 4745 5320 4d41 4445 2057 494c  CHANGES MADE WIL
+00001060: 4c20 4245 204c 4f53 5420 2f2f 0a20 2020  L BE LOST //.   
+00001070: 2020 2020 202f 2f3d 3d3d 3d3d 3d3d 3d3d       //=========
+00001080: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00001090: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000010a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d2f 2f0a 2020  ===========//.  
+000010b0: 2020 2020 2020 2443 4f4c 4f52 5f42 4143        $COLOR_BAC
+000010c0: 4b47 524f 554e 445f 313a 207a 1f3b 0a20  KGROUND_1: z.;. 
+000010d0: 2020 2020 2020 2024 434f 4c4f 525f 4241         $COLOR_BA
+000010e0: 434b 4752 4f55 4e44 5f32 3a20 7a1f 3b0a  CKGROUND_2: z.;.
+000010f0: 2020 2020 2020 2020 2443 4f4c 4f52 5f42          $COLOR_B
+00001100: 4143 4b47 524f 554e 445f 333a 207a 203b  ACKGROUND_3: z ;
+00001110: 200a 2020 2020 2020 2020 2443 4f4c 4f52   .        $COLOR
+00001120: 5f42 4143 4b47 524f 554e 445f 343a 207a  _BACKGROUND_4: z
+00001130: 203b 200a 2020 2020 2020 2020 2443 4f4c   ; .        $COL
+00001140: 4f52 5f42 4143 4b47 524f 554e 445f 353a  OR_BACKGROUND_5:
+00001150: 207a 203b 200a 2020 2020 2020 2020 2443   z ; .        $C
+00001160: 4f4c 4f52 5f42 4143 4b47 524f 554e 445f  OLOR_BACKGROUND_
+00001170: 363a 207a 1a3b 200a 2020 2020 2020 2020  6: z.; .        
+00001180: 2443 4f4c 4f52 5f54 4558 545f 313a 207a  $COLOR_TEXT_1: z
+00001190: 193b 0a20 2020 2020 2020 2024 434f 4c4f  .;.        $COLO
+000011a0: 525f 5445 5854 5f32 3a20 7a19 3b0a 2020  R_TEXT_2: z.;.  
+000011b0: 2020 2020 2020 2443 4f4c 4f52 5f54 4558        $COLOR_TEX
+000011c0: 545f 333a 207a 193b 0a20 2020 2020 2020  T_3: z.;.       
+000011d0: 2024 434f 4c4f 525f 5445 5854 5f34 3a20   $COLOR_TEXT_4: 
+000011e0: 7a1b 3b0a 2020 2020 2020 2020 2443 4f4c  z.;.        $COL
+000011f0: 4f52 5f41 4343 454e 545f 313a 207a 1b3b  OR_ACCENT_1: z.;
+00001200: 0a20 2020 2020 2020 2024 434f 4c4f 525f  .        $COLOR_
+00001210: 4143 4345 4e54 5f32 3a20 7a1b 3b0a 2020  ACCENT_2: z.;.  
+00001220: 2020 2020 2020 2443 4f4c 4f52 5f41 4343        $COLOR_ACC
+00001230: 454e 545f 333a 207a 1b3b 0a20 2020 2020  ENT_3: z.;.     
+00001240: 2020 2024 434f 4c4f 525f 4143 4345 4e54     $COLOR_ACCENT
+00001250: 5f34 3a20 619b 0100 003b 0a20 2020 2020  _4: a....;.     
+00001260: 2020 2024 4f50 4143 4954 595f 544f 4f4c     $OPACITY_TOOL
+00001270: 5449 503a 2032 3330 3b0a 2020 2020 2020  TIP: 230;.      
+00001280: 2020 2453 495a 455f 424f 5244 4552 5f52    $SIZE_BORDER_R
+00001290: 4144 4955 533a 2034 7078 3b0a 2020 2020  ADIUS: 4px;.    
+000012a0: 2020 2020 2442 4f52 4445 525f 313a 2031      $BORDER_1: 1
+000012b0: 7078 2073 6f6c 6964 2024 434f 4c4f 525f  px solid $COLOR_
+000012c0: 4241 434b 4752 4f55 4e44 5f31 3b0a 2020  BACKGROUND_1;.  
+000012d0: 2020 2020 2020 2442 4f52 4445 525f 323a        $BORDER_2:
+000012e0: 2031 7078 2073 6f6c 6964 2024 434f 4c4f   1px solid $COLO
+000012f0: 525f 4241 434b 4752 4f55 4e44 5f34 3b0a  R_BACKGROUND_4;.
+00001300: 2020 2020 2020 2020 2442 4f52 4445 525f          $BORDER_
+00001310: 333a 2031 7078 2073 6f6c 6964 2024 434f  3: 1px solid $CO
+00001320: 4c4f 525f 4241 434b 4752 4f55 4e44 5f36  LOR_BACKGROUND_6
+00001330: 3b0a 2020 2020 2020 2020 2442 4f52 4445  ;.        $BORDE
+00001340: 525f 5345 4c45 4354 494f 4e5f 333a 2031  R_SELECTION_3: 1
+00001350: 7078 2073 6f6c 6964 2024 434f 4c4f 525f  px solid $COLOR_
+00001360: 4143 4345 4e54 5f33 3b0a 2020 2020 2020  ACCENT_3;.      
+00001370: 2020 2442 4f52 4445 525f 5345 4c45 4354    $BORDER_SELECT
+00001380: 494f 4e5f 323a 2031 7078 2073 6f6c 6964  ION_2: 1px solid
+00001390: 2024 434f 4c4f 525f 4143 4345 4e54 5f32   $COLOR_ACCENT_2
+000013a0: 3b0a 2020 2020 2020 2020 2442 4f52 4445  ;.        $BORDE
+000013b0: 525f 5345 4c45 4354 494f 4e5f 313a 2031  R_SELECTION_1: 1
+000013c0: 7078 2073 6f6c 6964 2024 434f 4c4f 525f  px solid $COLOR_
+000013d0: 4143 4345 4e54 5f31 3b0a 2020 2020 2020  ACCENT_1;.      
+000013e0: 2020 2450 4154 485f 5245 534f 5552 4345    $PATH_RESOURCE
+000013f0: 533a 2027 7a9e 273b 0a20 2020 2020 2020  S: 'z.';.       
+00001400: 202f 2f3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d   //=============
+00001410: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00001420: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00001430: 3d3d 3d3d 3d3d 2f2f 0a20 2020 2020 2020  ======//.       
+00001440: 202f 2f20 454e 4420 2f2f 0a20 2020 2020   // END //.     
+00001450: 2020 202f 2f3d 3d3d 3d3d 3d3d 3d3d 3d3d     //===========
+00001460: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00001470: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00001480: 3d3d 3d3d 3d3d 3d3d 3d2f 2f0a 2020 2020  =========//.    
+00001490: 2020 2020 2901 da04 6669 6c65 293c 7243      )...file)<rC
+000014a0: 0000 0072 4400 0000 723d 0000 0072 3400  ...rD...r=...r4.
+000014b0: 0000 7245 0000 0072 4600 0000 7247 0000  ..rE...rF...rG..
+000014c0: 0072 4800 0000 7249 0000 0072 4a00 0000  .rH...rI...rJ...
+000014d0: 721c 0000 0072 4b00 0000 721d 0000 0072  r....rK...r....r
+000014e0: 4c00 0000 721e 0000 0072 4e00 0000 721f  L...r....rN...r.
+000014f0: 0000 0072 1300 0000 7220 0000 0072 2100  ...r....r ...r!.
+00001500: 0000 7222 0000 0072 2300 0000 7224 0000  ..r"...r#...r$..
+00001510: 0072 2500 0000 7226 0000 0072 2700 0000  .r%...r&...r'...
+00001520: 7228 0000 0072 2900 0000 722a 0000 0072  r(...r)...r*...r
+00001530: 2b00 0000 722c 0000 0072 2d00 0000 722e  +...r,...r-...r.
+00001540: 0000 00da 064f 626a 6563 7472 5100 0000  .....ObjectrQ...
+00001550: 5a12 434f 4c4f 525f 4241 434b 4752 4f55  Z.COLOR_BACKGROU
+00001560: 4e44 5f31 5a12 434f 4c4f 525f 4241 434b  ND_1Z.COLOR_BACK
+00001570: 4752 4f55 4e44 5f32 5a12 434f 4c4f 525f  GROUND_2Z.COLOR_
+00001580: 4241 434b 4752 4f55 4e44 5f33 5a12 434f  BACKGROUND_3Z.CO
+00001590: 4c4f 525f 4241 434b 4752 4f55 4e44 5f34  LOR_BACKGROUND_4
+000015a0: 5a12 434f 4c4f 525f 4241 434b 4752 4f55  Z.COLOR_BACKGROU
+000015b0: 4e44 5f35 5a12 434f 4c4f 525f 4241 434b  ND_5Z.COLOR_BACK
+000015c0: 4752 4f55 4e44 5f36 5a0c 434f 4c4f 525f  GROUND_6Z.COLOR_
+000015d0: 5445 5854 5f31 5a0c 434f 4c4f 525f 5445  TEXT_1Z.COLOR_TE
+000015e0: 5854 5f32 5a0c 434f 4c4f 525f 5445 5854  XT_2Z.COLOR_TEXT
+000015f0: 5f33 5a0c 434f 4c4f 525f 5445 5854 5f34  _3Z.COLOR_TEXT_4
+00001600: 5a0e 434f 4c4f 525f 4143 4345 4e54 5f31  Z.COLOR_ACCENT_1
+00001610: 5a0e 434f 4c4f 525f 4143 4345 4e54 5f32  Z.COLOR_ACCENT_2
+00001620: 5a0e 434f 4c4f 525f 4143 4345 4e54 5f33  Z.COLOR_ACCENT_3
+00001630: 5a0e 434f 4c4f 525f 4143 4345 4e54 5f34  Z.COLOR_ACCENT_4
+00001640: 5a0e 5041 5448 5f52 4553 4f55 5243 4553  Z.PATH_RESOURCES
+00001650: da02 6f73 da04 7061 7468 da07 6162 7370  ..os..path..absp
+00001660: 6174 68da 046a 6f69 6eda 0667 6574 6377  ath..join..getcw
+00001670: 64da 0665 7869 7374 73da 086d 616b 6564  d..exists..maked
+00001680: 6972 73da 046f 7065 6e72 0a00 0000 da05  irs..openr......
+00001690: 636c 6f73 6529 0972 2f00 0000 7250 0000  close).r/...rP..
+000016a0: 0072 4000 0000 5a0a 7468 656d 6546 6f75  .r@...Z.themeFou
+000016b0: 6e64 7251 0000 0072 4600 0000 5a0b 7363  ndrQ...rF...Z.sc
+000016c0: 7373 5f66 6f6c 6465 72da 0973 6373 735f  ss_folder..scss_
+000016d0: 7061 7468 da01 6672 1100 0000 7211 0000  path..fr....r...
+000016e0: 0072 1200 0000 da0f 4372 6561 7465 5661  .r......CreateVa
+000016f0: 7269 6162 6c65 739a 0000 0073 b000 0000  riables....s....
+00001700: 0001 0602 0a01 0401 0801 0a02 0801 0a03  ................
+00001710: 0c01 1002 0e02 0401 0801 0801 0801 0801  ................
+00001720: 0602 0401 0603 0e01 0e01 0e01 0e01 0e01  ................
+00001730: 0e02 0e01 0e01 0e01 0e02 0e01 0e01 0e01  ................
+00001740: 0e02 0603 0801 0a01 0a01 0a01 0a01 0a01  ................
+00001750: 0a02 0a01 0a01 0a01 0a02 0a01 0a01 0a01  ................
+00001760: 0a02 0a03 1a01 0e01 0a02 1601 0a01 0404  ................
+00001770: 04fc 0405 04fb 0406 04fa 0407 04f9 0408  ................
+00001780: 04f8 0409 04f7 040a 04f6 040b 04f5 040c  ................
+00001790: 04f4 040d 04f3 040e 04f2 040f 04f1 0410  ................
+000017a0: 04f0 0411 04ef 041a 04e6 061e 02e2 0620  ............... 
+000017b0: 7a23 4372 6561 7465 436f 6c6f 7256 6172  z#CreateColorVar
+000017c0: 6961 626c 652e 4372 6561 7465 5661 7269  iable.CreateVari
+000017d0: 6162 6c65 7329 014e 2907 7231 0000 0072  ables).N).r1...r
+000017e0: 3200 0000 7233 0000 0072 3000 0000 7252  2...r3...r0...rR
+000017f0: 0000 0072 6200 0000 723c 0000 0072 1100  ...rb...r<...r..
+00001800: 0000 7211 0000 0072 3900 0000 7212 0000  ..r....r9...r...
+00001810: 0072 3e00 0000 5d00 0000 7306 0000 0008  .r>...]...s.....
+00001820: 010e 0308 3972 3e00 0000 6300 0000 0000  ....9r>...c.....
+00001830: 0000 0000 0000 0000 0000 0001 0000 0040  ...............@
+00001840: 0000 0073 0c00 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
+00001850: 6401 5300 2902 7256 0000 004e 2903 7231  d.S.).rV...N).r1
+00001860: 0000 0072 3200 0000 7233 0000 0072 1100  ...r2...r3...r..
+00001870: 0000 7211 0000 0072 1100 0000 7212 0000  ..r....r....r...
+00001880: 0072 5600 0000 0a01 0000 7302 0000 0008  .rV.......s.....
+00001890: 0172 5600 0000 2901 7203 0000 0029 1172  .rV...).r....).r
+000018a0: 5700 0000 da03 7379 73da 0b71 7470 792e  W.....sys..qtpy.
+000018b0: 5174 436f 7265 5a11 6d61 7470 6c6f 746c  QtCoreZ.matplotl
+000018c0: 6962 2e63 6f6c 6f72 73da 0663 6f6c 6f72  ib.colors..color
+000018d0: 7372 0700 0000 7209 0000 0072 4300 0000  sr....r....rC...
+000018e0: 7250 0000 0072 1300 0000 720b 0000 0072  rP...r....r....r
+000018f0: 1500 0000 7234 0000 0072 3d00 0000 723e  ....r4...r=...r>
+00001900: 0000 00da 066f 626a 6563 7472 5600 0000  .....objectrV...
+00001910: 7211 0000 0072 1100 0000 7211 0000 0072  r....r....r....r
+00001920: 1200 0000 da08 3c6d 6f64 756c 653e 0800  ......<module>..
+00001930: 0000 731a 0000 0008 0108 0d08 030c 0108  ..s.............
+00001940: 0206 020a 1108 040e 1a10 0410 0c0e 7f00  ................
+00001950: 2e                                       .
```

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/__pycache__/colorsystem.cpython-39.pyc` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/colorsystem.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/__pycache__/resources_rc.cpython-39.pyc` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/resources_rc.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/__pycache__/sassCompiler.cpython-39.pyc` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/sassCompiler.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/_styles.scss` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/_styles.scss`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/colorsystem.py` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/colorsystem.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,91 +23,69 @@
 ########################################################################
 
 import matplotlib.colors as mc
 import colorsys
 ########################################################################
 settings = QSettings()
 
-
-########################################################################
-## 
-########################################################################
 def adjust_lightness(color, amount=0.5):
     try:
         c = mc.cnames[color]
-    except:
+    except KeyError:
         c = color
     c = colorsys.rgb_to_hls(*mc.to_rgb(c))
+    print(c)
 
     if c[1] > 0:
-        rgb = colorsys.hls_to_rgb(c[0], amount * c[1], c[2])
+        rgb = colorsys.hls_to_rgb(c[0] , amount * c[1], c[2])
     else:
-        rgb = colorsys.hls_to_rgb(c[0], 1 - (amount * 1), c[2])
-
-    newColor = rgb_to_hex((int(rgb[0] * 250), int(rgb[1] * 250), int(rgb[2] * 250)))
-    return newColor
+        rgb = colorsys.hls_to_rgb(c[0], 1 - (amount *  (1 - c[1])), c[2])
 
-def rgb_to_hex(rgb):
-    hexColor = '%02x%02x%02x' % rgb
-    return "#"+str(hexColor)
-
-########################################################################
-## THEMES
-########################################################################
-class Dark:
-    bg_color = "#0D0D14"
-    txt_color = "#fff"
-    accent_color = "#A8B9BD"
-    icons_color = "#fff"
-
-    BG_1 = adjust_lightness(bg_color, 1)
-    BG_2 = adjust_lightness(bg_color, 0.9)
-    BG_3 = adjust_lightness(bg_color, 0.8)
-    BG_4 = adjust_lightness(bg_color, 0.7)
-    BG_5 = adjust_lightness(bg_color, 0.5)
-    BG_6 = adjust_lightness(bg_color, 0.4)
-
-    CT_1 = adjust_lightness(txt_color, 1)
-    CT_2 = adjust_lightness(txt_color, 0.9)
-    CT_3 = adjust_lightness(txt_color, 0.8)
-    CT_4 = adjust_lightness(txt_color, 0.7)
-
-    CA_1 = adjust_lightness(accent_color, 1)
-    CA_2 = adjust_lightness(accent_color, .8)
-    CA_3 = adjust_lightness(accent_color, .6)
-    CA_4 = adjust_lightness(accent_color, .4)
-    
-    ICONS = ":/icons/Icons/"
+    new_color = rgb_to_hex((int(rgb[0] * 250), int(rgb[1] * 250), int(rgb[2] * 250)))
+    return new_color
 
 
+def rgb_to_hex(rgb):
+    hex_color = '%02x%02x%02x' % rgb
+    return "#" + hex_color
 
-class Light:
-    bg_color = "#fff"
-    txt_color = "#000"
-    accent_color = "#00bcff"
-    icons_color = ""
-    
-    BG_1 = adjust_lightness(bg_color, 1)
-    BG_2 = adjust_lightness(bg_color, 0.99)
-    BG_3 = adjust_lightness(bg_color, 0.95)
-    BG_4 = adjust_lightness(bg_color, 0.90)
-    BG_5 = adjust_lightness(bg_color, 0.85)
-    BG_6 = adjust_lightness(bg_color, 0.80)
-
-    CT_1 = adjust_lightness(txt_color, 1)
-    CT_2 = adjust_lightness(txt_color, 0.9)
-    CT_3 = adjust_lightness(txt_color, 0.8)
-    CT_4 = adjust_lightness(txt_color, 0.7)
-
-    CA_1 = adjust_lightness(accent_color, 1)
-    CA_2 = adjust_lightness(accent_color, .8)
-    CA_3 = adjust_lightness(accent_color, .6)
-    CA_4 = adjust_lightness(accent_color, .4)
+class Theme:
+    def __init__(self, bg_color, txt_color, accent_color, icons_color=""):
+        self.bg_color = bg_color
+        self.txt_color = txt_color
+        self.accent_color = accent_color
+        self.icons_color = icons_color
+
+        self.BG_1 = adjust_lightness(bg_color, 1)
+        self.BG_2 = adjust_lightness(bg_color, 0.95)
+        self.BG_3 = adjust_lightness(bg_color, 0.8)
+        self.BG_4 = adjust_lightness(bg_color, 0.75)
+        self.BG_5 = adjust_lightness(bg_color, 0.6)
+        self.BG_6 = adjust_lightness(bg_color, 0.55)
+
+        self.CT_1 = adjust_lightness(txt_color, 1)
+        self.CT_2 = adjust_lightness(txt_color, 0.9)
+        self.CT_3 = adjust_lightness(txt_color, 0.8)
+        self.CT_4 = adjust_lightness(txt_color, 0.7)
+
+        self.CA_1 = adjust_lightness(accent_color, 1)
+        self.CA_2 = adjust_lightness(accent_color, 0.9)
+        self.CA_3 = adjust_lightness(accent_color, 0.8)
+        self.CA_4 = adjust_lightness(accent_color, 0.7)
+
+        self.ICONS = ":/icons/Icons/"
+
+class Dark(Theme):
+    def __init__(self):
+        super().__init__("#0D0D14", "#fff", "#A8B9BD")
+
+class Light(Theme):
+    def __init__(self):
+        super().__init__("#fff", "#000", "#00bcff")
 
-    ICONS = ":/icons/Icons/"
 
 ########################################################################
 ## 
 ########################################################################
 
 ########################################################################
 ## CREATE COLOR VARIABLES
@@ -200,27 +178,27 @@
             if not themeFound:
                 theme = Light()
 
 
             theme.BG_1 = adjust_lightness(theme.bg_color, 1)
             theme.BG_2 = adjust_lightness(theme.bg_color, 0.90)
             theme.BG_3 = adjust_lightness(theme.bg_color, 0.80)
-            theme.BG_4 = adjust_lightness(theme.bg_color, 0.60)
-            theme.BG_5 = adjust_lightness(theme.bg_color, 0.50)
-            theme.BG_6 = adjust_lightness(theme.bg_color, 0.40)
+            theme.BG_4 = adjust_lightness(theme.bg_color, 0.70)
+            theme.BG_5 = adjust_lightness(theme.bg_color, 0.60)
+            theme.BG_6 = adjust_lightness(theme.bg_color, 0.50)
 
             theme.CT_1 = adjust_lightness(theme.txt_color, 1)
             theme.CT_2 = adjust_lightness(theme.txt_color, 0.9)
             theme.CT_3 = adjust_lightness(theme.txt_color, 0.8)
             theme.CT_4 = adjust_lightness(theme.txt_color, 0.7)
 
             theme.CA_1 = adjust_lightness(theme.accent_color, 1)
-            theme.CA_2 = adjust_lightness(theme.accent_color, .8)
-            theme.CA_3 = adjust_lightness(theme.accent_color, .6)
-            theme.CA_4 = adjust_lightness(theme.accent_color, .4)
+            theme.CA_2 = adjust_lightness(theme.accent_color, .9)
+            theme.CA_3 = adjust_lightness(theme.accent_color, .8)
+            theme.CA_4 = adjust_lightness(theme.accent_color, .7)
 
             theme.ICONS = ":/icons/Icons/"
 
         # Create global color variables
         self.theme = Object()
         self.theme.COLOR_BACKGROUND_1 = theme.BG_1
         self.theme.COLOR_BACKGROUND_2 = theme.BG_2
```

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/aperture.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/aperture.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/arrow_down.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/arrow_down.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/arrow_left.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/arrow_left.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/arrow_right.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/arrow_right.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/arrow_up.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/arrow_up.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/base_icon.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/base_icon.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/base_palette.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/base_palette.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/branch_closed.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/branch_closed.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/branch_end.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/branch_end.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/branch_line.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/branch_line.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/branch_more.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/branch_more.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/branch_open.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/branch_open.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/checkbox_checked.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/checkbox_checked.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/checkbox_indeterminate.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/checkbox_indeterminate.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/checkbox_unchecked.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/checkbox_unchecked.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/cloud-drizzle.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/cloud-drizzle.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/cloud-snow.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/cloud-snow.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/codesandbox.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/codesandbox.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/cpu.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/cpu.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/figma.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/figma.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/film.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/film.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/github.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/github.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/life-buoy.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/life-buoy.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/line_horizontal.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/line_horizontal.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/line_vertical.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/line_vertical.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/loader.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/loader.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/phone-call.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/phone-call.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/phone-forwarded.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/phone-forwarded.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/phone-incoming.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/phone-incoming.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/phone-missed.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/phone-missed.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/phone-off.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/phone-off.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/phone-outgoing.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/phone-outgoing.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/phone.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/phone.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/radio_checked.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/radio_checked.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/radio_unchecked.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/radio_unchecked.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/settings.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/settings.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/slack.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/slack.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/sliders.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/sliders.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/sun.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/sun.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/sunrise.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/sunrise.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/sunset.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/sunset.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/toolbar_move_horizontal.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/toolbar_move_horizontal.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/toolbar_move_vertical.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/toolbar_move_vertical.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/toolbar_separator_horizontal.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/toolbar_separator_horizontal.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/toolbar_separator_vertical.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/toolbar_separator_vertical.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/transparent.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/transparent.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/wifi-off.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/wifi-off.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/window_close.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/window_close.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/window_grip.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/window_grip.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/window_minimize.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/window_minimize.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/window_undock.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/window_undock.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Qss/icons/original_svg/youtube.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/youtube.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/RoundProgressBar.py` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/RoundProgressBar.py`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/SpiralProgressBar.py` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/SpiralProgressBar.py`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/Widgets.py` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Widgets.py`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/WidgetsWorker.py` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/WidgetsWorker.py`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/components/python/__pycache__/main.cpython-310.pyc` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/components/python/__pycache__/main.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/components/python/__pycache__/main.cpython-38.pyc` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/components/python/__pycache__/main.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Mar  4 16:18:45 2022 UTC, .py size: 2368 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 e53b 2262 4009 0000  U........;"b@...
+00000000: 550d 0d0a 0000 0000 6b61 9364 770a 0000  U.......ka.dw...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6800 0000 6400  .....@...sh...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 5400 6400 6402 6c03 5400 6504  d.l.T.d.d.l.T.e.
 00000050: 8300 5a05 4700 6403 6404 8400 6404 6506  ..Z.G.d.d...d.e.
 00000060: 8303 5a07 6508 6405 6b02 7264 6509 6501  ..Z.e.d.k.rde.e.
 00000070: 6a0a 8301 5a0b 6507 8300 5a0c 650c a00d  j...Z.e...Z.e...
@@ -26,15 +26,15 @@
 00000190: 0670 6172 656e 74a9 0072 0900 0000 fa53  .parent..r.....S
 000001a0: 633a 5c75 7365 7273 5c6b 6962 6574 5c61  c:\users\kibet\a
 000001b0: 6e61 636f 6e64 6133 5c4c 6962 5c73 6974  naconda3\Lib\sit
 000001c0: 652d 7061 636b 6167 6573 5c43 7573 746f  e-packages\Custo
 000001d0: 6d5f 5769 6467 6574 732f 636f 6d70 6f6e  m_Widgets/compon
 000001e0: 656e 7473 2f70 7974 686f 6e2f 6d61 696e  ents/python/main
 000001f0: 2e70 7972 0500 0000 1c00 0000 730a 0000  .pyr........s...
-00000200: 0000 010a 0108 010c 070c 067a 134d 6169  ...........z.Mai
+00000200: 0000 010a 0108 010c 080c 0c7a 134d 6169  ...........z.Mai
 00000210: 6e57 696e 646f 772e 5f5f 696e 6974 5f5f  nWindow.__init__
 00000220: 2901 4e29 04da 085f 5f6e 616d 655f 5fda  ).N)...__name__.
 00000230: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
 00000240: 7561 6c6e 616d 655f 5f72 0500 0000 7209  ualname__r....r.
 00000250: 0000 0072 0900 0000 7209 0000 0072 0a00  ...r....r....r..
 00000260: 0000 7203 0000 001b 0000 0073 0200 0000  ..r........s....
 00000270: 0801 7203 0000 00da 085f 5f6d 6169 6e5f  ..r......__main_
@@ -45,9 +45,9 @@
 000002c0: 6574 7469 6e67 7372 0400 0000 7203 0000  ettingsr....r...
 000002d0: 0072 0b00 0000 5a0c 5141 7070 6c69 6361  .r....Z.QApplica
 000002e0: 7469 6f6e da04 6172 6776 5a03 6170 705a  tion..argvZ.appZ
 000002f0: 0677 696e 646f 7772 0600 0000 da04 6578  .windowr......ex
 00000300: 6974 da05 6578 6563 5f72 0900 0000 7209  it..exec_r....r.
 00000310: 0000 0072 0900 0000 720a 0000 00da 083c  ...r....r......<
 00000320: 6d6f 6475 6c65 3e08 0000 0073 1400 0000  module>....s....
-00000330: 0801 0803 0805 0802 0608 101b 0801 0a04  ................
+00000330: 0801 0803 0805 0802 0608 1022 0801 0a04  ..........."....
 00000340: 0601 0801                                ....
```

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/components/python/__pycache__/ui_interface.cpython-310.pyc` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/components/python/__pycache__/ui_interface.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/components/python/__pycache__/ui_interface.cpython-38.pyc` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/components/python/__pycache__/ui_interface.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Mar  4 16:18:45 2022 UTC, .py size: 3127 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 e53b 2262 370c 0000  U........;"b7...
+00000000: 550d 0d0a 0000 0000 6b61 9364 370c 0000  U.......ka.d7...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3400 0000 6400  .....@...s4...d.
 00000030: 6401 6c00 5400 6400 6401 6c01 5400 6400  d.l.T.d.d.l.T.d.
 00000040: 6401 6c02 5400 6400 6402 6c03 5a03 4700  d.l.T.d.d.l.Z.G.
 00000050: 6403 6404 8400 6404 6504 8303 5a05 6402  d.d...d.e...Z.d.
 00000060: 5300 2905 e900 0000 0029 01da 012a 4e63  S.)......)...*Nc
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/components/python/main.py` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/components/python/main.py`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/components/python/ui_interface.py` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/components/python/ui_interface.py`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/components/uis/interface.ui` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/components/uis/interface.ui`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/interface.ui` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/interface.ui`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/Custom_Widgets/main.py` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/main.py`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/LICENSE` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/PKG-INFO` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,107 +1,109 @@
-Metadata-Version: 2.1
-Name: QT-PyQt-PySide-Custom-Widgets
-Version: 0.6.4
-Summary: Custom widgets and widget animations made for QT applications
-Home-page: https://github.com/KhamisiKibet/QT-PyQt-PySide-Custom-Widgets
-Author: Khamisi Kibet
-Author-email: kibetkhamisi@gmail.com
-License: GNU General Public License v3.0
-Keywords: PySide,PyQt,animation,custom,widgets,QML,C++,QT Creator
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# QT-PyQt-PySide-Custom-Widgets
-Awesome custom widgets made for QT Desktop Applications. Simplify your UI development process. These widgets can be used in QT Designer then imported to PySide code.
-
-# Installation 
-First time installer:
-```
-pip install QT-PyQt-PySide-Custom-Widgets
-```
-Upgrade/install the latest version:
-```
-pip install --upgrade QT-PyQt-PySide-Custom-Widgets
-```
-
-# Installation Testing
-Run the following code to see if the installation was successful.
-
-```python
-# Run this from your terminal or create a python file, 
-# paste this code, then run
-from Custom_Widgets.ProgressIndicator import test
-test.main()
-```
-
-You should see the following interface:
-![Custom Progress bar](https://github.com/KhamisiKibet/QT-PyQt-PySide-Custom-Widgets/blob/main/images/Screenshot.png?raw=true)
-
-# How to use it.
-- Read the full documentation plus video guides [here](https://khamisikibet.github.io/QT-PyQt-PySide-Custom-Widgets/) 
-
-[Watch the tutorial videos here](https://www.youtube.com/watch?v=21Qt9p_F7Ts&list=PLJ8t3BKaQLhPKj9Mx08WAwvz7TGskefbK)
-
-# What is new?
-## Version 0.6.2:
-- Added support for loading multiple ``JSON Stylesheets``
-    By default, the json file named ``style.json`` will be loaded, so no need to specify. The file must me inside the root directory of your project, ``json`` directory, or ``jsonstyles`` directory inside your project folder for it to be automatically loaded.
-    
-    If you have multiple JSON stylesheet files, then you can apply them to your GUI like this:
-    ```python
-        ########################################################################
-        # APPLY JSON STYLESHEET
-        ########################################################################
-        # self = QMainWindow class
-        # self.ui = Ui_MainWindow / user interface class
-        loadJsonStyle(self, self.ui, jsonFiles = {
-            "mystyle.json",
-            "mydirectory/myJsonStyle.json"
-            })
-        ########################################################################
-    ```
-    This feature is helpful especially when you have multiple windows files that will share only some parts of the stylesheet shuch app app title, settings etc.
-    
-- Toggle logs:
-    You can now switch app logs on or off.
-    This can be done from a python file:
-    ```python
-    # Show Logs
-    self.showCustomWidgetsLogs = True
-    ```
-    ```python
-    # Hide Logs
-    self.showCustomWidgetsLogs = False
-    ```
-    From the JSON file:
-    ```json
-    {
-    "ShowLogs": true,
-    ```
-    ```json
-    {
-    "ShowLogs": false,
-    ```
-
-# Sample Images
-
-Analog Gauge Widget
-
-![Analog Gauge Widget](https://github.com/KhamisiKibet/QT-PyQt-PySide-Custom-Widgets/blob/main/images/analog_qt_widget.png?raw=true)
-
-Responsive Animated GUI
-
-![Resposive PyQt PySide GUI](https://github.com/KhamisiKibet/QT-PyQt-PySide-Custom-Widgets/blob/main/images/responsive-qt-gui-python-intarface.png?raw=true)
-
-Animated QStacked Widget
-
-![Custom QStacked Widgets](https://github.com/KhamisiKibet/QT-PyQt-PySide-Custom-Widgets/blob/main/images/qstacked.png?raw=true)
+Metadata-Version: 2.1
+Name: QT-PyQt-PySide-Custom-Widgets
+Version: 0.6.5
+Summary: Custom widgets and widget animations made for QT applications
+Home-page: https://github.com/KhamisiKibet/QT-PyQt-PySide-Custom-Widgets
+Author: Khamisi Kibet
+Author-email: kibetkhamisi@gmail.com
+License: GNU General Public License v3.0
+Keywords: PySide,PyQt,animation,custom,widgets,QML,C++,QT Creator
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# QT-PyQt-PySide-Custom-Widgets
+Awesome custom widgets made for QT Desktop Applications. Simplify your UI development process. These widgets can be used in QT Designer then imported to PySide code.
+
+# Installation 
+First time installer:
+```
+pip install QT-PyQt-PySide-Custom-Widgets
+```
+Upgrade/install the latest version:
+```
+pip install --upgrade QT-PyQt-PySide-Custom-Widgets
+```
+
+# Installation Testing
+Run the following code to see if the installation was successful.
+
+```python
+# Run this from your terminal or create a python file, 
+# paste this code, then run
+from Custom_Widgets.ProgressIndicator import test
+test.main()
+```
+
+You should see the following interface:
+![Custom Progress bar](https://github.com/KhamisiKibet/QT-PyQt-PySide-Custom-Widgets/blob/main/images/Screenshot.png?raw=true)
+
+# How to use it.
+- Read the full documentation plus video guides [here](https://khamisikibet.github.io/QT-PyQt-PySide-Custom-Widgets/) 
+
+[Watch the tutorial videos here](https://www.youtube.com/watch?v=21Qt9p_F7Ts&list=PLJ8t3BKaQLhPKj9Mx08WAwvz7TGskefbK)
+
+# What is new?
+## Version 0.6.2:
+- Added support for loading multiple ``JSON Stylesheets``
+    By default, the json file named ``style.json`` will be loaded, so no need to specify. The file must me inside the root directory of your project, ``json`` directory, or ``jsonstyles`` directory inside your project folder for it to be automatically loaded.
+    
+    If you have multiple JSON stylesheet files, then you can apply them to your GUI like this:
+    ```python
+        ########################################################################
+        # APPLY JSON STYLESHEET
+        ########################################################################
+        # self = QMainWindow class
+        # self.ui = Ui_MainWindow / user interface class
+        loadJsonStyle(self, self.ui, jsonFiles = {
+            "mystyle.json",
+            "mydirectory/myJsonStyle.json"
+            })
+        ########################################################################
+    ```
+    This feature is helpful especially when you have multiple windows files that will share only some parts of the stylesheet shuch app app title, settings etc.
+    
+- Toggle logs:
+    You can now switch app logs on or off.
+    This can be done from a python file:
+    ```python
+    # Show Logs
+    self.showCustomWidgetsLogs = True
+    ```
+    ```python
+    # Hide Logs
+    self.showCustomWidgetsLogs = False
+    ```
+    From the JSON file:
+    ```json
+    {
+    "ShowLogs": true,
+    ```
+    ```json
+    {
+    "ShowLogs": false,
+    ```
+
+# Sample Images
+
+Analog Gauge Widget
+
+![Analog Gauge Widget](https://github.com/KhamisiKibet/QT-PyQt-PySide-Custom-Widgets/blob/main/images/analog_qt_widget.png?raw=true)
+
+Responsive Animated GUI
+
+![Resposive PyQt PySide GUI](https://github.com/KhamisiKibet/QT-PyQt-PySide-Custom-Widgets/blob/main/images/responsive-qt-gui-python-intarface.png?raw=true)
+
+Animated QStacked Widget
+
+![Custom QStacked Widgets](https://github.com/KhamisiKibet/QT-PyQt-PySide-Custom-Widgets/blob/main/images/qstacked.png?raw=true)
+
```

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/QT_PyQt_PySide_Custom_Widgets.egg-info/PKG-INFO` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/QT_PyQt_PySide_Custom_Widgets.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,107 +1,109 @@
-Metadata-Version: 2.1
-Name: QT-PyQt-PySide-Custom-Widgets
-Version: 0.6.4
-Summary: Custom widgets and widget animations made for QT applications
-Home-page: https://github.com/KhamisiKibet/QT-PyQt-PySide-Custom-Widgets
-Author: Khamisi Kibet
-Author-email: kibetkhamisi@gmail.com
-License: GNU General Public License v3.0
-Keywords: PySide,PyQt,animation,custom,widgets,QML,C++,QT Creator
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# QT-PyQt-PySide-Custom-Widgets
-Awesome custom widgets made for QT Desktop Applications. Simplify your UI development process. These widgets can be used in QT Designer then imported to PySide code.
-
-# Installation 
-First time installer:
-```
-pip install QT-PyQt-PySide-Custom-Widgets
-```
-Upgrade/install the latest version:
-```
-pip install --upgrade QT-PyQt-PySide-Custom-Widgets
-```
-
-# Installation Testing
-Run the following code to see if the installation was successful.
-
-```python
-# Run this from your terminal or create a python file, 
-# paste this code, then run
-from Custom_Widgets.ProgressIndicator import test
-test.main()
-```
-
-You should see the following interface:
-![Custom Progress bar](https://github.com/KhamisiKibet/QT-PyQt-PySide-Custom-Widgets/blob/main/images/Screenshot.png?raw=true)
-
-# How to use it.
-- Read the full documentation plus video guides [here](https://khamisikibet.github.io/QT-PyQt-PySide-Custom-Widgets/) 
-
-[Watch the tutorial videos here](https://www.youtube.com/watch?v=21Qt9p_F7Ts&list=PLJ8t3BKaQLhPKj9Mx08WAwvz7TGskefbK)
-
-# What is new?
-## Version 0.6.2:
-- Added support for loading multiple ``JSON Stylesheets``
-    By default, the json file named ``style.json`` will be loaded, so no need to specify. The file must me inside the root directory of your project, ``json`` directory, or ``jsonstyles`` directory inside your project folder for it to be automatically loaded.
-    
-    If you have multiple JSON stylesheet files, then you can apply them to your GUI like this:
-    ```python
-        ########################################################################
-        # APPLY JSON STYLESHEET
-        ########################################################################
-        # self = QMainWindow class
-        # self.ui = Ui_MainWindow / user interface class
-        loadJsonStyle(self, self.ui, jsonFiles = {
-            "mystyle.json",
-            "mydirectory/myJsonStyle.json"
-            })
-        ########################################################################
-    ```
-    This feature is helpful especially when you have multiple windows files that will share only some parts of the stylesheet shuch app app title, settings etc.
-    
-- Toggle logs:
-    You can now switch app logs on or off.
-    This can be done from a python file:
-    ```python
-    # Show Logs
-    self.showCustomWidgetsLogs = True
-    ```
-    ```python
-    # Hide Logs
-    self.showCustomWidgetsLogs = False
-    ```
-    From the JSON file:
-    ```json
-    {
-    "ShowLogs": true,
-    ```
-    ```json
-    {
-    "ShowLogs": false,
-    ```
-
-# Sample Images
-
-Analog Gauge Widget
-
-![Analog Gauge Widget](https://github.com/KhamisiKibet/QT-PyQt-PySide-Custom-Widgets/blob/main/images/analog_qt_widget.png?raw=true)
-
-Responsive Animated GUI
-
-![Resposive PyQt PySide GUI](https://github.com/KhamisiKibet/QT-PyQt-PySide-Custom-Widgets/blob/main/images/responsive-qt-gui-python-intarface.png?raw=true)
-
-Animated QStacked Widget
-
-![Custom QStacked Widgets](https://github.com/KhamisiKibet/QT-PyQt-PySide-Custom-Widgets/blob/main/images/qstacked.png?raw=true)
+Metadata-Version: 2.1
+Name: QT-PyQt-PySide-Custom-Widgets
+Version: 0.6.5
+Summary: Custom widgets and widget animations made for QT applications
+Home-page: https://github.com/KhamisiKibet/QT-PyQt-PySide-Custom-Widgets
+Author: Khamisi Kibet
+Author-email: kibetkhamisi@gmail.com
+License: GNU General Public License v3.0
+Keywords: PySide,PyQt,animation,custom,widgets,QML,C++,QT Creator
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# QT-PyQt-PySide-Custom-Widgets
+Awesome custom widgets made for QT Desktop Applications. Simplify your UI development process. These widgets can be used in QT Designer then imported to PySide code.
+
+# Installation 
+First time installer:
+```
+pip install QT-PyQt-PySide-Custom-Widgets
+```
+Upgrade/install the latest version:
+```
+pip install --upgrade QT-PyQt-PySide-Custom-Widgets
+```
+
+# Installation Testing
+Run the following code to see if the installation was successful.
+
+```python
+# Run this from your terminal or create a python file, 
+# paste this code, then run
+from Custom_Widgets.ProgressIndicator import test
+test.main()
+```
+
+You should see the following interface:
+![Custom Progress bar](https://github.com/KhamisiKibet/QT-PyQt-PySide-Custom-Widgets/blob/main/images/Screenshot.png?raw=true)
+
+# How to use it.
+- Read the full documentation plus video guides [here](https://khamisikibet.github.io/QT-PyQt-PySide-Custom-Widgets/) 
+
+[Watch the tutorial videos here](https://www.youtube.com/watch?v=21Qt9p_F7Ts&list=PLJ8t3BKaQLhPKj9Mx08WAwvz7TGskefbK)
+
+# What is new?
+## Version 0.6.2:
+- Added support for loading multiple ``JSON Stylesheets``
+    By default, the json file named ``style.json`` will be loaded, so no need to specify. The file must me inside the root directory of your project, ``json`` directory, or ``jsonstyles`` directory inside your project folder for it to be automatically loaded.
+    
+    If you have multiple JSON stylesheet files, then you can apply them to your GUI like this:
+    ```python
+        ########################################################################
+        # APPLY JSON STYLESHEET
+        ########################################################################
+        # self = QMainWindow class
+        # self.ui = Ui_MainWindow / user interface class
+        loadJsonStyle(self, self.ui, jsonFiles = {
+            "mystyle.json",
+            "mydirectory/myJsonStyle.json"
+            })
+        ########################################################################
+    ```
+    This feature is helpful especially when you have multiple windows files that will share only some parts of the stylesheet shuch app app title, settings etc.
+    
+- Toggle logs:
+    You can now switch app logs on or off.
+    This can be done from a python file:
+    ```python
+    # Show Logs
+    self.showCustomWidgetsLogs = True
+    ```
+    ```python
+    # Hide Logs
+    self.showCustomWidgetsLogs = False
+    ```
+    From the JSON file:
+    ```json
+    {
+    "ShowLogs": true,
+    ```
+    ```json
+    {
+    "ShowLogs": false,
+    ```
+
+# Sample Images
+
+Analog Gauge Widget
+
+![Analog Gauge Widget](https://github.com/KhamisiKibet/QT-PyQt-PySide-Custom-Widgets/blob/main/images/analog_qt_widget.png?raw=true)
+
+Responsive Animated GUI
+
+![Resposive PyQt PySide GUI](https://github.com/KhamisiKibet/QT-PyQt-PySide-Custom-Widgets/blob/main/images/responsive-qt-gui-python-intarface.png?raw=true)
+
+Animated QStacked Widget
+
+![Custom QStacked Widgets](https://github.com/KhamisiKibet/QT-PyQt-PySide-Custom-Widgets/blob/main/images/qstacked.png?raw=true)
+
```

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/QT_PyQt_PySide_Custom_Widgets.egg-info/SOURCES.txt` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/QT_PyQt_PySide_Custom_Widgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/README.md` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.4/setup.py` & `QT-PyQt-PySide-Custom-Widgets-0.6.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     name = 'QT-PyQt-PySide-Custom-Widgets',         # How you named your package folder (MyLib)
     packages = [
         'Custom_Widgets',
         'Custom_Widgets.ProgressIndicator',
         'Custom_Widgets.Qss',
     ],
     include_package_data=True,
-    version = '0.6.4',      # Start with a small number and increase it with every change you make
+    version = '0.6.5',      # Start with a small number and increase it with every change you make
     license="GNU General Public License v3.0",        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description = 'Custom widgets and widget animations made for QT applications',   # Give a short description about your library
     long_description=README,
     long_description_content_type="text/markdown",
     author = 'Khamisi Kibet',                   # Type in your name
     author_email = 'kibetkhamisi@gmail.com',      # Type in your E-Mail
     url = 'https://github.com/KhamisiKibet/QT-PyQt-PySide-Custom-Widgets',   # Provide either the link to your github or to your website
```

