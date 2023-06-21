# Comparing `tmp/nonebot_plugin_l4d2_server-0.5.6.4.tar.gz` & `tmp/nonebot_plugin_l4d2_server-0.5.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_l4d2_server-0.5.6.4.tar", max compression
+gzip compressed data, was "nonebot_plugin_l4d2_server-0.5.6.5.tar", max compression
```

## Comparing `nonebot_plugin_l4d2_server-0.5.6.4.tar` & `nonebot_plugin_l4d2_server-0.5.6.5.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0    35149 2023-06-21 03:31:12.856099 nonebot_plugin_l4d2_server-0.5.6.4/LICENSE
--rw-r--r--   0        0        0     5683 2023-06-21 03:31:12.856099 nonebot_plugin_l4d2_server-0.5.6.4/README.md
--rw-r--r--   0        0        0    16860 2023-06-21 03:31:12.856099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/__init__.py
--rw-r--r--   0        0        0   158357 2023-06-21 03:31:12.860099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
--rw-r--r--   0        0        0   631630 2023-06-21 03:31:12.860099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
--rw-r--r--   0        0        0   405369 2023-06-21 03:31:12.860099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
--rw-r--r--   0        0        0     1590 2023-06-21 03:31:12.860099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
--rw-r--r--   0        0        0   242997 2023-06-21 03:31:12.860099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
--rw-r--r--   0        0        0     2135 2023-06-21 03:31:12.864099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
--rw-r--r--   0        0        0     6135 2023-06-21 03:31:12.864099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
--rw-r--r--   0        0        0     6170 2023-06-21 03:31:12.864099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
--rw-r--r--   0        0        0     1523 2023-06-21 03:31:12.864099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
--rw-r--r--   0        0        0     5506 2023-06-21 03:31:12.864099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg
--rw-r--r--   0        0        0     2408 2023-06-21 03:31:12.864099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg
--rw-r--r--   0        0        0     7874 2023-06-21 03:31:12.864099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
--rw-r--r--   0        0        0      486 2023-06-21 03:31:12.864099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/w.svg
--rw-r--r--   0        0        0     1350 2023-06-21 03:31:12.864099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/data/img/white.png
--rw-r--r--   0        0        0     8734 2023-06-21 03:31:12.864099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
--rw-r--r--   0        0        0     1610 2023-06-21 03:31:12.864099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
--rw-r--r--   0        0        0     3010 2023-06-21 03:31:12.864099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
--rw-r--r--   0        0        0     1694 2023-06-21 03:31:12.864099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_anne/server.py
--rw-r--r--   0        0        0      359 2023-06-21 03:31:12.864099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
--rw-r--r--   0        0        0     3252 2023-06-21 03:31:12.864099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
--rw-r--r--   0        0        0      468 2023-06-21 03:31:12.864099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_data/config.py
--rw-r--r--   0        0        0        0 2023-06-21 03:31:12.864099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_data/database.py
--rw-r--r--   0        0        0     3232 2023-06-21 03:31:12.864099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_data/players.py
--rw-r--r--   0        0        0     1295 2023-06-21 03:31:12.864099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
--rw-r--r--   0        0        0     4097 2023-06-21 03:31:12.864099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
--rw-r--r--   0        0        0     1714 2023-06-21 03:31:12.864099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py
--rw-r--r--   0        0        0     1860 2023-06-21 03:31:12.864099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_file/input_json.py
--rw-r--r--   0        0        0     2688 2023-06-21 03:31:12.864099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_file/remote.py
--rw-r--r--   0        0        0     4148 2023-06-21 03:31:12.864099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
--rw-r--r--   0        0        0     4007 2023-06-21 03:31:12.864099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_image/download.py
--rw-r--r--   0        0        0     1038 2023-06-21 03:31:12.864099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
--rw-r--r--   0        0        0     9524 2023-06-21 03:31:12.864099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_image/image.py
--rw-r--r--   0        0        0     1073 2023-06-21 03:31:12.864099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_image/one.py
--rw-r--r--   0        0        0      936 2023-06-21 03:31:12.864099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
--rw-r--r--   0        0        0     3799 2023-06-21 03:31:12.864099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_image/steam.py
--rw-r--r--   0        0        0     1387 2023-06-21 03:31:12.864099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
--rw-r--r--   0        0        0     7415 2023-06-21 03:31:12.864099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_push/__init__.py
--rw-r--r--   0        0        0     3735 2023-06-21 03:31:12.864099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
--rw-r--r--   0        0        0     1157 2023-06-21 03:31:12.864099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_queries/api.py
--rw-r--r--   0        0        0     1191 2023-06-21 03:31:12.864099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py
--rw-r--r--   0        0        0    10855 2023-06-21 03:31:12.864099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
--rw-r--r--   0        0        0     1615 2023-06-21 03:31:12.864099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
--rw-r--r--   0        0        0        0 2023-06-21 03:31:12.864099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_server/index.py
--rw-r--r--   0        0        0     1248 2023-06-21 03:31:12.864099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
--rw-r--r--   0        0        0     1359 2023-06-21 03:31:12.864099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
--rw-r--r--   0        0        0     4113 2023-06-21 03:31:12.864099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_update/__init__.py
--rw-r--r--   0        0        0     1175 2023-06-21 03:31:12.864099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py
--rw-r--r--   0        0        0     2024 2023-06-21 03:31:12.864099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_update/restart.py
--rw-r--r--   0        0        0     1434 2023-06-21 03:31:12.864099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_update/update.py
--rw-r--r--   0        0        0     9342 2023-06-21 03:31:12.864099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_utils/command.py
--rw-r--r--   0        0        0     5813 2023-06-21 03:31:12.864099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_utils/config.py
--rw-r--r--   0        0        0     1620 2023-06-21 03:31:12.864099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_utils/message.py
--rw-r--r--   0        0        0      337 2023-06-21 03:31:12.864099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_utils/rule.py
--rw-r--r--   0        0        0      992 2023-06-21 03:31:12.864099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_utils/seach.py
--rw-r--r--   0        0        0     2133 2023-06-21 03:31:12.864099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py
--rw-r--r--   0        0        0     8928 2023-06-21 03:31:12.868099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_utils/utils.py
--rw-r--r--   0        0        0     8575 2023-06-21 03:31:12.868099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_web/web.py
--rw-r--r--   0        0        0    14650 2023-06-21 03:31:12.868099 nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
--rw-r--r--   0        0        0     1496 2023-06-21 03:31:12.868099 nonebot_plugin_l4d2_server-0.5.6.4/pyproject.toml
--rw-r--r--   0        0        0     7549 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.5.6.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-21 09:56:32.772747 nonebot_plugin_l4d2_server-0.5.6.5/LICENSE
+-rw-r--r--   0        0        0     5683 2023-06-21 09:56:32.772747 nonebot_plugin_l4d2_server-0.5.6.5/README.md
+-rw-r--r--   0        0        0    19652 2023-06-21 09:56:32.776748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/__init__.py
+-rw-r--r--   0        0        0   158357 2023-06-21 09:56:32.776748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
+-rw-r--r--   0        0        0   631630 2023-06-21 09:56:32.780748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
+-rw-r--r--   0        0        0   405369 2023-06-21 09:56:32.780748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
+-rw-r--r--   0        0        0     1590 2023-06-21 09:56:32.780748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
+-rw-r--r--   0        0        0   242997 2023-06-21 09:56:32.780748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
+-rw-r--r--   0        0        0     2135 2023-06-21 09:56:32.780748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
+-rw-r--r--   0        0        0     6135 2023-06-21 09:56:32.780748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
+-rw-r--r--   0        0        0     6170 2023-06-21 09:56:32.780748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
+-rw-r--r--   0        0        0     1523 2023-06-21 09:56:32.780748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
+-rw-r--r--   0        0        0     5506 2023-06-21 09:56:32.780748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg
+-rw-r--r--   0        0        0     2408 2023-06-21 09:56:32.780748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg
+-rw-r--r--   0        0        0     7874 2023-06-21 09:56:32.780748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
+-rw-r--r--   0        0        0      486 2023-06-21 09:56:32.780748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/w.svg
+-rw-r--r--   0        0        0     1350 2023-06-21 09:56:32.784748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/data/img/white.png
+-rw-r--r--   0        0        0     8734 2023-06-21 09:56:32.784748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
+-rw-r--r--   0        0        0     1610 2023-06-21 09:56:32.784748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
+-rw-r--r--   0        0        0     3010 2023-06-21 09:56:32.784748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
+-rw-r--r--   0        0        0     1694 2023-06-21 09:56:32.784748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_anne/server.py
+-rw-r--r--   0        0        0      359 2023-06-21 09:56:32.784748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
+-rw-r--r--   0        0        0     3252 2023-06-21 09:56:32.784748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
+-rw-r--r--   0        0        0      468 2023-06-21 09:56:32.784748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_data/config.py
+-rw-r--r--   0        0        0        0 2023-06-21 09:56:32.784748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_data/database.py
+-rw-r--r--   0        0        0     3232 2023-06-21 09:56:32.784748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_data/players.py
+-rw-r--r--   0        0        0     1295 2023-06-21 09:56:32.784748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
+-rw-r--r--   0        0        0     4097 2023-06-21 09:56:32.784748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
+-rw-r--r--   0        0        0     1714 2023-06-21 09:56:32.784748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py
+-rw-r--r--   0        0        0     1860 2023-06-21 09:56:32.784748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_file/input_json.py
+-rw-r--r--   0        0        0     2688 2023-06-21 09:56:32.784748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_file/remote.py
+-rw-r--r--   0        0        0     4148 2023-06-21 09:56:32.784748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
+-rw-r--r--   0        0        0     4007 2023-06-21 09:56:32.784748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_image/download.py
+-rw-r--r--   0        0        0     1038 2023-06-21 09:56:32.784748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
+-rw-r--r--   0        0        0     9524 2023-06-21 09:56:32.784748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_image/image.py
+-rw-r--r--   0        0        0     1073 2023-06-21 09:56:32.784748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_image/one.py
+-rw-r--r--   0        0        0      936 2023-06-21 09:56:32.784748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
+-rw-r--r--   0        0        0     3799 2023-06-21 09:56:32.784748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_image/steam.py
+-rw-r--r--   0        0        0     1387 2023-06-21 09:56:32.784748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
+-rw-r--r--   0        0        0     7415 2023-06-21 09:56:32.784748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_push/__init__.py
+-rw-r--r--   0        0        0     3735 2023-06-21 09:56:32.784748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
+-rw-r--r--   0        0        0     1157 2023-06-21 09:56:32.784748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_queries/api.py
+-rw-r--r--   0        0        0     1191 2023-06-21 09:56:32.784748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py
+-rw-r--r--   0        0        0    10990 2023-06-21 09:56:32.784748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
+-rw-r--r--   0        0        0     1615 2023-06-21 09:56:32.784748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-21 09:56:32.784748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_server/index.py
+-rw-r--r--   0        0        0     1248 2023-06-21 09:56:32.784748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
+-rw-r--r--   0        0        0     1359 2023-06-21 09:56:32.784748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
+-rw-r--r--   0        0        0     4113 2023-06-21 09:56:32.784748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_update/__init__.py
+-rw-r--r--   0        0        0     1175 2023-06-21 09:56:32.784748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py
+-rw-r--r--   0        0        0     2024 2023-06-21 09:56:32.784748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_update/restart.py
+-rw-r--r--   0        0        0     1434 2023-06-21 09:56:32.784748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_update/update.py
+-rw-r--r--   0        0        0     9345 2023-06-21 09:56:32.784748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_utils/command.py
+-rw-r--r--   0        0        0     5875 2023-06-21 09:56:32.784748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_utils/config.py
+-rw-r--r--   0        0        0     1620 2023-06-21 09:56:32.784748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_utils/message.py
+-rw-r--r--   0        0        0      337 2023-06-21 09:56:32.784748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_utils/rule.py
+-rw-r--r--   0        0        0      992 2023-06-21 09:56:32.784748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_utils/seach.py
+-rw-r--r--   0        0        0     2133 2023-06-21 09:56:32.784748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py
+-rw-r--r--   0        0        0     8928 2023-06-21 09:56:32.784748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_utils/utils.py
+-rw-r--r--   0        0        0     8575 2023-06-21 09:56:32.784748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_web/web.py
+-rw-r--r--   0        0        0    15044 2023-06-21 09:56:32.784748 nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
+-rw-r--r--   0        0        0     1496 2023-06-21 09:56:32.784748 nonebot_plugin_l4d2_server-0.5.6.5/pyproject.toml
+-rw-r--r--   0        0        0     7549 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.5.6.5/PKG-INFO
```

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/LICENSE` & `nonebot_plugin_l4d2_server-0.5.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/README.md` & `nonebot_plugin_l4d2_server-0.5.6.5/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 from typing import Tuple,Union,List
 from time import sleep
 
 from nonebot.matcher import Matcher
 from nonebot.typing import T_State
 from nonebot.params import CommandArg,ArgPlainText,RegexGroup,Arg
 from nonebot import get_driver, require
+from typing import Annotated
+from nonebot.params import Keyword
 
 from .l4d2_utils.config import *
 from .l4d2_utils.utils import *
 from .l4d2_utils.command import *
 from .l4d2_image.steam import url_to_byte,url_to_byte_name
 
 from .l4d2_data import sq_L4D2
@@ -35,23 +37,56 @@
 from .l4d2_file import updown_l4d2_vpk,all_zip_to_one
 from .l4d2_file.input_json import *
 from .l4d2_utils.txt_to_img import mode_txt_to_img
 scheduler = require("nonebot_plugin_apscheduler").scheduler
 from nonebot.plugin import PluginMetadata
 
 driver = get_driver()
+logo ="""
+    ......                  ` .]]@@@@@@@@@@@@@@@@@@@@@@@@@@@@@OO^       
+    ......                ,/@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@OO^       
+    ......            /O@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@OO^       
+    `.....           ,@^=.OOO\/\@@@@@@@@@@@@@@@@@@@@OO//@@@@@/OO\]]]OO\]
+    ``....          ,@@/=^OOOOOOOO@@@@@@@@@@@\]OOOOOOO^^=@@@@OOOOOOOOOOO
+    `.....          O@O^==OOOOOOOO@@@/.,@@@OOOOOOOOOOO\O,@@@@OOOOOOOOO@@
+    ......    ,    .@@@^=`OOOOOOOOO/  ,O@@OOOOOOOOOOOOOO.O@@@OO/[[[[[[[.
+    ......    =..,//@@@^=`OOOOOOOOO@.*=@@@OOOOOOOOOOOOOO]@@@OOO.     ,/`
+    ......    =.\O]`,@O^\=OOOO@@@@@@O`=@@@@@@@OOOOOOOO*O,OO^....[[``]./]
+    ......    ,^.oOoO@O^=,OO@@@@@OoO`\O\OO@@@@OOOOOOOOO]@@^.]]]/OOOo.,OO
+    ......     =.=OOOO@@@@/[[=/.^,/....*.=^,[O@@@@OOOO.@@OOOOOOOOO/..OOO
+    ......      \.\OO`.,....*`.=.^.......=....=@O[\@@O@@[^ ,`.=Oo*.,OOO/
+    ......       ,@,`...  ....=^/......../....=/O^....\..O]/[\O[*]/OOO. 
+    ......       ]@^.,....*..=O\^........^..*.O.\O.^..=^\..,\/\@OOO[.   
+    ......    ,,`O^.,..../.,O`//........=..=`=^.=O`O..=^..OOO*/OOO.     
+    ......   .=.=@..^...=^/O`*OO.]...o**\.,/=^...O^@^..^...OO^=`OOO`    
+    ......  `=.,O^./.*.,OO`,.,/@/.*,O`,O*/@/`....\O\^......Oo^.^,OOO.   
+    ...... .,`.o=^=^.../`...]/`***/O^/@oO@`..[[[[\/=\......O^^...=OO^   
+    ......  ^.=`O^O.*.=\],]]]/\O/\@O[=O/`        =.=O....=^O^*....OOO.  
+    ...... =../=OO^.*.=@@[[,@@@\ .. ..    ,\@@@@@] =O...`=^@`.....=OO^  
+    ...... `..^=OO^.^,@`  ^ =oO\          .O\O@\.,\@@..,^OoO......=OOO. 
+    ...... ^...=OO^.^.@^ =^*=^,O          \..Ooo^  ,@..=OOOO..*....OOO. 
+    ...... ^...=o@^.`.O@. .  ... .. ....  ^.*`.*^  =^..o@oO@*.=....OOO^ 
+    ...... ^...=oOO.*.\O   ... .......... .\   ` ,=^*.,OOOO@^.=`^..=OO\ 
+    ...... ^...*`OO.*.=O ........          ......,`*^.=OOOo@^.=^^..=OOO.
+    ...... \....*oO^..*O^ ....... @OO[[[`  ......../.,@OOOo@^..OO...OOO`
+    ...... =.....*.=`..,O`       .O.....=   ... ^.=..OOOOO=O@..=O^..OOO^
+    ...... .^...**.O@...\O^ .     \.....`   .^ /.,^.=O@OO`=O@^..OO`.=OO\
+    ...... .^...,.=O=@...OO@\      ,[O\=.    ./`.*.*OOOOO..OOO*..OO.,OOO
+    ....../O....../^=O@`..O@@@@@]`    .* .,/@@/..../OOOOO*.,OOO..,OO`=OO
+    @OO\ooO....,*/@^,@@@\..@^[\@@@@@@O]*]//[`@^*^*=OOOOOO^..=OO\...\^.\@
+    OOooo^..`./oOO@/ =^\/^.^\\....=]......,/@@^O^*O.... .,][],OO\....\`.
+    @Oooo\/]OOOOOO/  .  \.=^....,..........[.,OO^=^.    /    ,`\OO`.....
+    """
 
 
 __version__ = "0.5.6"
 __plugin_meta__ = PluginMetadata(
     name="求生之路小助手",
     description='群内对有关求生之路的查询和操作',
-    usage="""
-    查询：【关键词】([序号])
-    """,
+    usage=logo,
     type="application",
     homepage="https://github.com/Agnes4m/nonebot_plugin_l4d2_server",
     supported_adapters={"~onebot.v11"},
     extra={
         "version": __version__,
         "author": "Agnes4m <Z735803792@163.com>",
     },
@@ -81,17 +116,22 @@
     vpk_files = await updown_l4d2_vpk(map_path,name,url)
     if vpk_files:
         mes = "解压成功，新增以下几个vpk文件"
         await matcher.finish(mes_list(mes,vpk_files))
     else:
         await matcher.finish("你可能上传了相同的文件，或者解压失败了捏")
 
-
-
-@up.got("is_sure", prompt="请选择上传位置（输入阿拉伯数字)")    
+path_list:str = '请选择上传位置（输入阿拉伯数字)'
+times = 0
+for one_path in l4_config.l4_ipall:
+    times += 1
+    path_msg = one_path['location']
+    path_list += f'\n {str(times)} | {path_msg}'
+    
+@up.got("is_sure", prompt=path_list)    
 async def _(matcher: Matcher):
     args = matcher.get_arg('txt')
     l4_file = l4_config.l4_ipall
     if not args:
         await matcher.finish('获取文件出错辣，再试一次吧')
 
     is_sure = str(matcher.get_arg('is_sure')).strip()
@@ -235,24 +275,27 @@
             await matcher.send(f'已经切换路径为\n{str(l4_config.l4_number+1)}、{now_path}')
             config_manager.save()
     else: 
         now_path = l4_config.l4_ipall[l4_config.l4_number]['location']
         await matcher.send(f'当前的路径为\n{str(l4_config.l4_number+1)}、{now_path}')
         
         
-@queries.handle()
-async def _(matcher:Matcher,args:Message = CommandArg()):
-    msg = args.extract_plain_text()
-    if msg:
-        matcher.set_arg("ip",args)
-
-@queries.got("ip",prompt="请输入ip,格式如中括号内【127.0.0.1】【114.51.49.19:1810】")
-async def _(matcher:Matcher,tag:str = ArgPlainText("ip")):
-    ip = split_maohao(tag)
-    msg = await queries_server(ip)
+@queries_comm.handle()
+async def _(matcher:Matcher,event:MessageEvent,keyword:str = Keyword()):
+    msg = event.get_plaintext()
+    if not msg:
+        await matcher.finish('ip格式如中括号内【127.0.0.1】【114.51.49.19:1810】')
+    ip = msg.split(keyword)[-1].split('\r')[0].split(' ')
+    for one_msg in ip:
+        if one_msg and one_msg[-1].isdigit():
+            break
+    if not one_msg:
+        await matcher.finish()
+    ip_list = split_maohao(one_msg)
+    msg = await queries_server(ip_list)
     await matcher.finish(msg)
     
 
 @add_queries.handle()
 async def _(matcher:Matcher,event:GroupMessageEvent,args:Message = CommandArg()):
     msg = args.extract_plain_text()
     if len(msg)==0:
```

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/data/img/white.png` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/data/img/white.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_anne/server.py` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_anne/server.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_data/__init__.py` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_data/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_data/players.py` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_data/players.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_data/serverip.py` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_data/serverip.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_file/__init__.py` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_file/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_file/input_json.py` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_file/input_json.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_file/remote.py` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_file/remote.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_image/__init__.py` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_image/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_image/download.py` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_image/download.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_image/image.py` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_image/image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_image/one.py` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_image/one.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_image/steam.py` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_image/steam.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_push/__init__.py` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_push/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_queries/api.py` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_queries/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py`

 * *Files 2% similar despite different names*

```diff
@@ -217,16 +217,23 @@
     try:
         return str(host) + ':' + str(port)
     except TypeError:
         return None
 
 def split_maohao(msg:str) -> list:
     """分割大小写冒号"""
-    msg:list = re.split(":|：",msg.strip())
-    mse = [msg[0],msg[-1]] if len(msg)==2 else [msg[0],20715]
+    if ':' in msg:
+        msg:list = msg.split(':')
+    elif '：' in msg:
+        msg:list = msg.split('：')
+    elif msg.replace('.','').isdigit():
+        msg:List[str] = [msg,'20715']
+    else:
+        pass  
+    mse = [msg[0],msg[-1]]
     return mse
 
 async def write_json(data_str: str):
     """
     添加数据或者删除数据
      - 【求生更新 添加 腐竹 ip 模式 序号】
      - 【求生更新 添加 腐竹 ip 模式】
```

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_server/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_server/rcon.py` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_server/rcon.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_server/workshop.py` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_server/workshop.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_update/__init__.py` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_update/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_update/restart.py` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_update/restart.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_update/update.py` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_update/update.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_utils/command.py` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_utils/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 import asyncio
 from typing import Type
 from time import sleep
 
-from nonebot import on_notice,on_command,on_regex,on_keyword,MatcherGroup
+from nonebot import on_notice,on_command,on_regex,on_keyword
 from nonebot.params import CommandArg,RawCommand,CommandStart
 from nonebot.matcher import Matcher
 import nonebot
 from nonebot.adapters.onebot.v11 import (
     GroupUploadNoticeEvent,
     NoticeEvent,
     MessageEvent,
@@ -75,15 +75,15 @@
 prison = on_command('zl',aliases={'坐牢'},priority=20,block=True)
 open_prison = on_command('kl',aliases={'开牢'},priority=20,block=True)
 
 # updata = on_command('updata',aliases={'求生更新'},priority=20,block=True,permission= Master)
 tan_jian = on_command('tj',aliases={'探监'},priority=20,block=True)
 
 # 查询
-queries = on_command('queries',aliases={'求生ip','求生IP'},priority=20,block=True)
+queries_comm = on_keyword(keywords={'queries','求生ip','求生IP','connect'},priority=20,block=True)
 add_queries = on_command('addq',aliases={"求生添加订阅"},priority=20,block=True,permission= Master)
 del_queries = on_command('delq',aliases={"求生取消订阅"},priority=20,block=True,permission= Master)
 show_queries = on_command('showq',aliases={"求生订阅"},priority=20,block=True)
 join_server = on_command('ld_jr',aliases={"求生加入"},priority=20,block=True)
 connect_rcon = on_command("Rrcon", aliases={"求生连接", '求生链接','求生rcon'}, priority=50, block=False)
 end_connect = ['stop', '结束', '连接结束', '结束连接']
 search_api = on_command('search',aliases={'求生三方'}, priority=20, block=True,permission= Master)
```

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_utils/config.py` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_utils/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         'port':'20715',
         'rcon':'9191810',
         'account':'root',
         'password':'114514',
         'server_id':'远程地图',
         }],
           alias='l4服务器ip集合')
-    
+    l4_zl_tag :List[str] = Field(['云'], alias='坐牢三指令')
     l4_number :int = Field(1,alias='第几个地图路径')
     web_secret_key: str = Field('49c294d32f69b732ef6447c18379451ce1738922a75cd1d4812ef150318a2ed0',
                                 alias='后台管理token密钥')
     l4_master: List[str] = Field(['114514919'], alias='求生地图全局管理员qq')
     # l4_ip:bool = Field(False, alias='查询地图是否显示ip')
     l4_font: str = Field('simsun.ttc', alias='字体')
     l4_only:bool = Field(False, alias='下载地图是是否阻碍其他指令')
```

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_utils/message.py` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_utils/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_utils/seach.py` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_utils/seach.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_utils/utils.py` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_utils/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_web/web.py` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_web/web.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/nonebot_plugin_l4d2_server/l4d2_web/webUI.py` & `nonebot_plugin_l4d2_server-0.5.6.5/nonebot_plugin_l4d2_server/l4d2_web/webUI.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,15 +72,20 @@
                   labelRemark=Remark(shape='circle',
                                      content='设置好后，使用推送服务器定时指令，将以x分钟为间隔推送一次')),
         InputNumber(label='定时推次数', name='l4_push_times', value='${l4_push_times}',
                   labelRemark=Remark(shape='circle',
                                      content='设置好后，将按照推送间隔时间推送x此')),        
         InputNumber(label='当前路径序号', name='l4_number', value='${l4_number}',
                   labelRemark=Remark(shape='circle',
-                                     content='如果选定了路径，则上传地图优先传这个路径')),        
+                                     content='如果选定了路径，则上传地图优先传这个路径')),     
+        InputTag(label='求生上传地图用户', name='l4_master', value='${l4_master}',
+                 enableBatchAdd=True,
+                 placeholder='添加qq号', visibleOn='${total_enable}', joinValues=False, extractValue=True,
+                 labelRemark=Remark(shape='circle',
+                                    content='在这里加入的用户，才能上传地图')),           
 
         InputTag(label='求生上传地图用户', name='l4_master', value='${l4_master}',
                  enableBatchAdd=True,
                  placeholder='添加qq号', visibleOn='${total_enable}', joinValues=False, extractValue=True,
                  labelRemark=Remark(shape='circle',
                                     content='在这里加入的用户，才能上传地图')),
```

#### html2text {}

```diff
@@ -49,14 +49,18 @@
 content='è®¾ç½®å¥½åï¼å°æç§æ¨éé´éæ¶é´æ¨éxæ­¤')), InputNumber
 (label='å½åè·¯å¾åºå·', name='l4_number', value='${l4_number}',
 labelRemark=Remark(shape='circle',
 content='å¦æéå®äºè·¯å¾ï¼åä¸ä¼ å°å¾ä¼åä¼ è¿ä¸ªè·¯å¾')),
 InputTag(label='æ±çä¸ä¼ å°å¾ç¨æ·', name='l4_master', value='$
 {l4_master}', enableBatchAdd=True, placeholder='æ·»å qqå·', visibleOn='$
 {total_enable}', joinValues=False, extractValue=True, labelRemark=Remark
+(shape='circle', content='å¨è¿éå å¥çç¨æ·ï¼æè½ä¸ä¼ å°å¾')),
+InputTag(label='æ±çä¸ä¼ å°å¾ç¨æ·', name='l4_master', value='$
+{l4_master}', enableBatchAdd=True, placeholder='æ·»å qqå·', visibleOn='$
+{total_enable}', joinValues=False, extractValue=True, labelRemark=Remark
 (shape='circle', content='å¨è¿éå å¥çç¨æ·ï¼æè½ä¸ä¼ å°å¾')), ],
 actions=[Action(label='ä¿å­', level=LevelEnum.success, type='submit'), Action
 (label='éç½®', level=LevelEnum.warning, type='reset')] ) upload_map_form =
 Form( title='å¨å±éç½®', name='global_config', api='post:/l4d2/api/
 l4d2_map_config', body=[ InputText(label='æå¡å¨host', name='web_username',
 value='${web_username}', labelRemark=Remark(shape='circle',
 content='127.0.0.1')), InputPassword(label='æå¡å¨', name='web_password',
```

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/pyproject.toml` & `nonebot_plugin_l4d2_server-0.5.6.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-l4d2-server"
-version = "0.5.6.4"
+version = "0.5.6.5"
 description = "L4D2 server related operations plugin for NoneBot2"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 repository = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 keywords = ["steam", "game", "l4d2", "nonebot2", "plugin"]
```

### Comparing `nonebot_plugin_l4d2_server-0.5.6.4/PKG-INFO` & `nonebot_plugin_l4d2_server-0.5.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-l4d2-server
-Version: 0.5.6.4
+Version: 0.5.6.5
 Summary: L4D2 server related operations plugin for NoneBot2
 Home-page: https://github.com/Agnes4m/nonebot_plugin_l4d2_server
 License: GPLv3
 Keywords: steam,game,l4d2,nonebot2,plugin
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.9,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.5.6.4
+Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.5.6.5
 Summary: L4D2 server related operations plugin for NoneBot2 Home-page: https://
 github.com/Agnes4m/nonebot_plugin_l4d2_server License: GPLv3 Keywords:
 steam,game,l4d2,nonebot2,plugin Author: Agnes_Digital Author-email:
 Z735803792@163.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
```

