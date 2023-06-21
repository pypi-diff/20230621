# Comparing `tmp/esphome-dashboard-20230516.0.tar.gz` & `tmp/esphome-dashboard-20230621.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esphome-dashboard-20230516.0.tar", last modified: Mon May 15 20:28:38 2023, max compression
+gzip compressed data, was "esphome-dashboard-20230621.0.tar", last modified: Wed Jun 21 01:56:10 2023, max compression
```

## Comparing `esphome-dashboard-20230516.0.tar` & `esphome-dashboard-20230621.0.tar`

### file list

```diff
@@ -1,521 +1,521 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:28:38.587113 esphome-dashboard-20230516.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-15 20:27:39.000000 esphome-dashboard-20230516.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-15 20:27:39.000000 esphome-dashboard-20230516.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-15 20:28:38.587113 esphome-dashboard-20230516.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-15 20:27:39.000000 esphome-dashboard-20230516.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:28:38.539114 esphome-dashboard-20230516.0/esphome_dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-15 20:27:57.000000 esphome-dashboard-20230516.0/esphome_dashboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-15 20:27:57.000000 esphome-dashboard-20230516.0/esphome_dashboard/base.template.html
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-15 20:27:57.000000 esphome-dashboard-20230516.0/esphome_dashboard/base_with_header_footer.template.html
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-15 20:27:57.000000 esphome-dashboard-20230516.0/esphome_dashboard/index.template.html
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-15 20:27:57.000000 esphome-dashboard-20230516.0/esphome_dashboard/login.template.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:28:38.531114 esphome-dashboard-20230516.0/esphome_dashboard/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:28:38.539114 esphome-dashboard-20230516.0/esphome_dashboard/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-15 20:27:57.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/css/esphome-2.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:28:38.539114 esphome-dashboard-20230516.0/esphome_dashboard/static/firmware/
--rw-r--r--   0 runner    (1001) docker     (123)    15872 2023-05-15 20:27:57.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/firmware/bootloader.bin
--rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-05-15 20:27:57.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/firmware/ota.bin
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-05-15 20:27:57.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/firmware/partitions.bin
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:28:38.539114 esphome-dashboard-20230516.0/esphome_dashboard/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    72504 2023-05-15 20:28:13.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/fonts/codicon.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:28:38.539114 esphome-dashboard-20230516.0/esphome_dashboard/static/fonts/material-icons/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-15 20:27:57.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/fonts/material-icons/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    57620 2023-05-15 20:27:57.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/fonts/material-icons/MaterialIcons-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    44300 2023-05-15 20:27:57.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/fonts/material-icons/MaterialIcons-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-15 20:27:57.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/fonts/material-icons/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-15 20:27:57.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/fonts/material-icons/material-icons.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:28:38.539114 esphome-dashboard-20230516.0/esphome_dashboard/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-05-15 20:27:57.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-05-15 20:27:57.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/images/logo-text.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:28:38.531114 esphome-dashboard-20230516.0/esphome_dashboard/static/js/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:28:38.547114 esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/
--rw-r--r--   0 runner    (1001) docker     (123)     7876 2023-05-15 20:28:37.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.1bc018ae.js
--rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-05-15 20:28:37.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.1c31574e.js
--rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-05-15 20:28:37.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.286ad693.js
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-05-15 20:28:37.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.29c28c21.js
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-05-15 20:28:37.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.2b18cdda.js
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-15 20:28:37.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.363ea4b9.js
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-15 20:28:37.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.3b4072f5.js
--rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-05-15 20:28:37.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.417d3d2d.js
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-15 20:28:37.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.440fff61.js
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-15 20:28:37.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.45f3bfa8.js
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-15 20:28:37.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.52f07dd8.js
--rw-r--r--   0 runner    (1001) docker     (123)  2790314 2023-05-15 20:28:37.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.5cae2e65.js
--rw-r--r--   0 runner    (1001) docker     (123)   233918 2023-05-15 20:28:37.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.5cd5d307.js
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-05-15 20:28:37.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.61332c08.js
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-15 20:28:37.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.6d280f04.js
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-05-15 20:28:37.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.6eebcb7a.js
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-15 20:28:37.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.734d4b21.js
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-15 20:28:37.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.78cf8c6e.js
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-15 20:28:37.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.7d2e85dd.js
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-15 20:28:37.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.7e8b4fbe.js
--rw-r--r--   0 runner    (1001) docker     (123)    83074 2023-05-15 20:28:37.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.834bbab0.js
--rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-05-15 20:28:37.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.98e8e8d2.js
--rw-r--r--   0 runner    (1001) docker     (123)    16777 2023-05-15 20:28:37.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.9e5eaea1.js
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-15 20:28:37.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.a613b168.js
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-15 20:28:37.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.a6e96e5a.js
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-05-15 20:28:37.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.b9286028.js
--rw-r--r--   0 runner    (1001) docker     (123)    77094 2023-05-15 20:28:37.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.bff582f5.js
--rw-r--r--   0 runner    (1001) docker     (123)    14078 2023-05-15 20:28:37.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.c0a69417.js
--rw-r--r--   0 runner    (1001) docker     (123)    58068 2023-05-15 20:28:37.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.c2d1f4be.js
--rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-05-15 20:28:37.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.c74d5ae3.js
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-15 20:28:37.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.d408ba9c.js
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-15 20:28:37.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.db573db5.js
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-15 20:28:37.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.dde41422.js
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-15 20:28:37.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.e1319253.js
--rw-r--r--   0 runner    (1001) docker     (123)    41533 2023-05-15 20:28:37.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.e4466087.js
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-15 20:28:37.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.e683a7a9.js
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-15 20:28:37.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.e6db31ca.js
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-15 20:28:37.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.ed145062.js
--rw-r--r--   0 runner    (1001) docker     (123)     8648 2023-05-15 20:28:37.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.f4034d2e.js
--rw-r--r--   0 runner    (1001) docker     (123)   318847 2023-05-15 20:28:37.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/index-d3dd97b9.js
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-15 20:28:37.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/manifest.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:28:38.531114 esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/monaco-editor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:28:38.531114 esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/monaco-editor/esm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:28:38.531114 esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/monaco-editor/esm/vs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:28:38.547114 esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/monaco-editor/esm/vs/editor/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-15 20:28:37.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/monaco-editor/esm/vs/editor/editor.worker.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:28:38.587113 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/a4988.json
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/absolute_humidity.json
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ac_dimmer.json
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/adalight.json
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/adc.json
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/adc128s102.json
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/addressable_light.json
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ade7953.json
--rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ads1115.json
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/aht10.json
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/airthings_ble.json
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/airthings_wave_mini.json
--rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/airthings_wave_plus.json
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/am2320.json
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/am43.json
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/analog_threshold.json
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/animation.json
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/anova.json
--rw-r--r--   0 runner    (1001) docker     (123)     7100 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/apds9960.json
--rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/api.json
--rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/as3935.json
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/as3935_i2c.json
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/as3935_spi.json
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/as7341.json
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/async_tcp.json
--rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/atc_mithermometer.json
--rw-r--r--   0 runner    (1001) docker     (123)    16157 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/atm90e32.json
--rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/b_parasite.json
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ballu.json
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/bang_bang.json
--rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/bedjet.json
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/bh1750.json
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/binary.json
--rw-r--r--   0 runner    (1001) docker     (123)    28755 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/binary_sensor.json
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/binary_sensor_map.json
--rw-r--r--   0 runner    (1001) docker     (123)     9157 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/bl0939.json
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/bl0940.json
--rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/bl0942.json
--rw-r--r--   0 runner    (1001) docker     (123)    18543 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ble_client.json
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ble_presence.json
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ble_rssi.json
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ble_scanner.json
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/bluetooth_proxy.json
--rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/bme280.json
--rw-r--r--   0 runner    (1001) docker     (123)    11912 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/bme680.json
--rw-r--r--   0 runner    (1001) docker     (123)    18394 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/bme680_bsec.json
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/bmp085.json
--rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/bmp280.json
--rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/bmp3xx.json
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/bp1658cj.json
--rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/bp5758d.json
--rw-r--r--   0 runner    (1001) docker     (123)     5386 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/button.json
--rw-r--r--   0 runner    (1001) docker     (123)     8742 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/canbus.json
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/cap1188.json
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/captive_portal.json
--rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ccs811.json
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/cd74hc4067.json
--rw-r--r--   0 runner    (1001) docker     (123)    21700 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/climate.json
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/climate_ir.json
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/climate_ir_lg.json
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/color.json
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/color_temperature.json
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/component.json
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/coolix.json
--rw-r--r--   0 runner    (1001) docker     (123)     9813 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/copy.json
--rw-r--r--   0 runner    (1001) docker     (123)    10873 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/cover.json
--rw-r--r--   0 runner    (1001) docker     (123)    10920 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/cs5460a.json
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/cse7761.json
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/cse7766.json
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ct_clamp.json
--rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/current_based.json
--rw-r--r--   0 runner    (1001) docker     (123)    13964 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/custom.json
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/custom_component.json
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/cwww.json
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/dac7678.json
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/daikin.json
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/daikin_brc.json
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/dallas.json
--rw-r--r--   0 runner    (1001) docker     (123)    28349 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/daly_bms.json
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/dashboard_import.json
--rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/debug.json
--rw-r--r--   0 runner    (1001) docker     (123)    10662 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/deep_sleep.json
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/delonghi.json
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/demo.json
--rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/dfplayer.json
--rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/dht.json
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/dht12.json
--rw-r--r--   0 runner    (1001) docker     (123)    14252 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/display.json
--rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/display_menu.json
--rw-r--r--   0 runner    (1001) docker     (123)    24685 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/display_menu_base.json
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/dps310.json
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ds1307.json
--rw-r--r--   0 runner    (1001) docker     (123)    51328 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/dsmr.json
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/duty_cycle.json
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/e131.json
--rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ee895.json
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ektf2232.json
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/endstop.json
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ens210.json
--rw-r--r--   0 runner    (1001) docker     (123)    32029 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/esp32.json
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/esp32_ble.json
--rw-r--r--   0 runner    (1001) docker     (123)     5447 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/esp32_ble_beacon.json
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/esp32_ble_server.json
--rw-r--r--   0 runner    (1001) docker     (123)    13007 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/esp32_ble_tracker.json
--rw-r--r--   0 runner    (1001) docker     (123)    19956 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/esp32_camera.json
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/esp32_camera_web_server.json
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/esp32_can.json
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/esp32_dac.json
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/esp32_hall.json
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/esp32_improv.json
--rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/esp32_touch.json
--rw-r--r--   0 runner    (1001) docker     (123)    13930 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/esp8266.json
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/esp8266_pwm.json
--rw-r--r--   0 runner    (1001) docker     (123)    87963 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/esphome.json
--rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ethernet.json
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ethernet_info.json
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/exposure_notifications.json
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/external_components.json
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ezo.json
--rw-r--r--   0 runner    (1001) docker     (123)    21627 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ezo_pmp.json
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/factory_reset.json
--rw-r--r--   0 runner    (1001) docker     (123)    11926 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/fan.json
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/fastled_base.json
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/fastled_clockless.json
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/fastled_spi.json
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/feedback.json
--rw-r--r--   0 runner    (1001) docker     (123)    18007 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/fingerprint_grow.json
--rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/font.json
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/fs3000.json
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/fujitsu_general.json
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/globals.json
--rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/gpio.json
--rw-r--r--   0 runner    (1001) docker     (123)     7610 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/gps.json
--rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/graph.json
--rw-r--r--   0 runner    (1001) docker     (123)    16922 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/growatt_solar.json
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/haier.json
--rw-r--r--   0 runner    (1001) docker     (123)    25645 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/havells_solar.json
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/hbridge.json
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/hdc1080.json
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/heatpumpir.json
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/hitachi_ac344.json
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/hitachi_ac424.json
--rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/hlw8012.json
--rw-r--r--   0 runner    (1001) docker     (123)     6964 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/hm3301.json
--rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/hmc5883l.json
--rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/homeassistant.json
--rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/honeywellabp.json
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/hrxl_maxsonar_wr.json
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/hte501.json
--rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/http_request.json
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/htu21d.json
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/hx711.json
--rw-r--r--   0 runner    (1001) docker     (123)    13066 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/hydreon_rgxx.json
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/hyt271.json
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/i2c.json
--rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/i2s_audio.json
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ili9xxx.json
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/image.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/improv_base.json
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/improv_serial.json
--rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ina219.json
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ina226.json
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ina260.json
--rw-r--r--   0 runner    (1001) docker     (123)     8315 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ina3221.json
--rw-r--r--   0 runner    (1001) docker     (123)     6082 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/inkbird_ibsth1_mini.json
--rw-r--r--   0 runner    (1001) docker     (123)    12726 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/inkplate6.json
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/integration.json
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/internal_temperature.json
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/interval.json
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/json.json
--rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/kalman_combinator.json
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/key_collector.json
--rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/kuntze.json
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/lcd_base.json
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/lcd_gpio.json
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/lcd_menu.json
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/lcd_pcf8574.json
--rw-r--r--   0 runner    (1001) docker     (123)    11517 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ld2410.json
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ledc.json
--rw-r--r--   0 runner    (1001) docker     (123)    80866 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/light.json
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/lilygo_t5_47.json
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/lock.json
--rw-r--r--   0 runner    (1001) docker     (123)   238272 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/logger.json
--rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ltr390.json
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/matrix_keypad.json
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/max31855.json
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/max31856.json
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/max31865.json
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/max44009.json
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/max6675.json
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/max6956.json
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/max7219.json
--rw-r--r--   0 runner    (1001) docker     (123)     8560 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/max7219digit.json
--rw-r--r--   0 runner    (1001) docker     (123)     6456 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/max9611.json
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mcp23008.json
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mcp23016.json
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mcp23017.json
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mcp23s08.json
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mcp23s17.json
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mcp23xxx.json
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mcp23xxx_base.json
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mcp2515.json
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mcp3008.json
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mcp3204.json
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mcp4725.json
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mcp4728.json
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mcp47a1.json
--rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mcp9600.json
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mcp9808.json
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mdns.json
--rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/media_player.json
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mhz19.json
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/microphone.json
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mics_4514.json
--rw-r--r--   0 runner    (1001) docker     (123)    10822 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/midea.json
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/midea_ac.json
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/midea_ir.json
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mitsubishi.json
--rw-r--r--   0 runner    (1001) docker     (123)    11764 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mlx90393.json
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mlx90614.json
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mmc5603.json
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/modbus.json
--rw-r--r--   0 runner    (1001) docker     (123)    49191 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/modbus_controller.json
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/monochromatic.json
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mopeka_ble.json
--rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mopeka_pro_check.json
--rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mopeka_std_check.json
--rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mpl3115a2.json
--rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mpr121.json
--rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mpu6050.json
--rw-r--r--   0 runner    (1001) docker     (123)     6959 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mpu6886.json
--rw-r--r--   0 runner    (1001) docker     (123)    22240 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mqtt.json
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mqtt_subscribe.json
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ms5611.json
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/my9231.json
--rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/neopixelbus.json
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/network.json
--rw-r--r--   0 runner    (1001) docker     (123)    20223 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/nextion.json
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ntc.json
--rw-r--r--   0 runner    (1001) docker     (123)    15235 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/number.json
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ota.json
--rw-r--r--   0 runner    (1001) docker     (123)    20277 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/output.json
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/packages.json
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/page.json
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/partition.json
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/pca6416a.json
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/pca9554.json
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/pca9685.json
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/pcd8544.json
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/pcf85063.json
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/pcf8574.json
--rw-r--r--   0 runner    (1001) docker     (123)    20589 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/pid.json
--rw-r--r--   0 runner    (1001) docker     (123)    73941 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/pipsolar.json
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/pm1006.json
--rw-r--r--   0 runner    (1001) docker     (123)    11184 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/pmsa003i.json
--rw-r--r--   0 runner    (1001) docker     (123)    16777 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/pmsx003.json
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/pn532.json
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/pn532_i2c.json
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/pn532_spi.json
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/power_supply.json
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/preferences.json
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/prometheus.json
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/psram.json
--rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/pulse_counter.json
--rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/pulse_meter.json
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/pulse_width.json
--rw-r--r--   0 runner    (1001) docker     (123)     8096 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/pvvx_mithermometer.json
--rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/pzem004t.json
--rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/pzemac.json
--rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/pzemdc.json
--rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/qmc5883l.json
--rw-r--r--   0 runner    (1001) docker     (123)     6620 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/qmp6988.json
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/qr_code.json
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/radon_eye_ble.json
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/radon_eye_rd200.json
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/rc522.json
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/rc522_i2c.json
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/rc522_spi.json
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/rdm6300.json
--rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/remote_base.json
--rw-r--r--   0 runner    (1001) docker     (123)    47870 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/remote_receiver.json
--rw-r--r--   0 runner    (1001) docker     (123)    47223 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/remote_transmitter.json
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/resistance.json
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/restart.json
--rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/rf_bridge.json
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/rgb.json
--rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/rgbct.json
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/rgbw.json
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/rgbww.json
--rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/rotary_encoder.json
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/rp2040.json
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/rp2040_pwm.json
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/rtttl.json
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ruuvi_ble.json
--rw-r--r--   0 runner    (1001) docker     (123)    14474 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ruuvitag.json
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/safe_mode.json
--rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/scd30.json
--rw-r--r--   0 runner    (1001) docker     (123)    11509 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/scd4x.json
--rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/script.json
--rw-r--r--   0 runner    (1001) docker     (123)    16724 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sdm_meter.json
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sdp3x.json
--rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sds011.json
--rw-r--r--   0 runner    (1001) docker     (123)    17512 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/selec_meter.json
--rw-r--r--   0 runner    (1001) docker     (123)    10334 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/select.json
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sen21231.json
--rw-r--r--   0 runner    (1001) docker     (123)    25256 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sen5x.json
--rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/senseair.json
--rw-r--r--   0 runner    (1001) docker     (123)   106836 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sensor.json
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/servo.json
--rw-r--r--   0 runner    (1001) docker     (123)    10669 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sgp30.json
--rw-r--r--   0 runner    (1001) docker     (123)    15212 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sgp4x.json
--rw-r--r--   0 runner    (1001) docker     (123)     9201 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/shelly_dimmer.json
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sht3xd.json
--rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sht4x.json
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/shtcx.json
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/shutdown.json
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sigma_delta_output.json
--rw-r--r--   0 runner    (1001) docker     (123)    10343 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sim800l.json
--rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/slow_pwm.json
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sm10bit_base.json
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sm16716.json
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sm2135.json
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sm2235.json
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sm2335.json
--rw-r--r--   0 runner    (1001) docker     (123)    10974 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sm300d2.json
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sml.json
--rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/smt100.json
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sn74hc165.json
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sn74hc595.json
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sntp.json
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/socket.json
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sonoff_d1.json
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/speed.json
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/spi.json
--rw-r--r--   0 runner    (1001) docker     (123)    53606 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sprinkler.json
--rw-r--r--   0 runner    (1001) docker     (123)    15586 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sps30.json
--rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ssd1306_base.json
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ssd1306_i2c.json
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ssd1306_spi.json
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ssd1322_base.json
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ssd1322_spi.json
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ssd1325_base.json
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ssd1325_spi.json
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ssd1327_base.json
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ssd1327_i2c.json
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ssd1327_spi.json
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ssd1331_base.json
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ssd1331_spi.json
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ssd1351_base.json
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ssd1351_spi.json
--rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/st7735.json
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/st7789v.json
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/st7920.json
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/status.json
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/status_led.json
--rw-r--r--   0 runner    (1001) docker     (123)     8316 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/stepper.json
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sts3x.json
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/substitutions.json
--rw-r--r--   0 runner    (1001) docker     (123)     8353 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sun.json
--rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/switch.json
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sx1509.json
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/t6615.json
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/tca9548a.json
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/tcl112.json
--rw-r--r--   0 runner    (1001) docker     (123)     8310 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/tcs34725.json
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/tee501.json
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/teleinfo.json
--rw-r--r--   0 runner    (1001) docker     (123)    38023 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/template.json
--rw-r--r--   0 runner    (1001) docker     (123)    11115 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/text_sensor.json
--rw-r--r--   0 runner    (1001) docker     (123)    11486 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/thermostat.json
--rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/time.json
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/time_based.json
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/tlc59208f.json
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/tlc5947.json
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/tm1621.json
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/tm1637.json
--rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/tm1638.json
--rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/tm1651.json
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/tmp102.json
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/tmp117.json
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/tof10120.json
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/toshiba.json
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/total_daily_energy.json
--rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/touchscreen.json
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/tsl2561.json
--rw-r--r--   0 runner    (1001) docker     (123)    10223 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/tsl2591.json
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ttp229_bsf.json
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ttp229_lsf.json
--rw-r--r--   0 runner    (1001) docker     (123)    33914 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/tuya.json
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/tx20.json
--rw-r--r--   0 runner    (1001) docker     (123)     7313 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/uart.json
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ufire_ec.json
--rw-r--r--   0 runner    (1001) docker     (123)     6987 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ufire_ise.json
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/uln2003.json
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ultrasonic.json
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/uptime.json
--rw-r--r--   0 runner    (1001) docker     (123)    55804 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/vbus.json
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/version.json
--rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/vl53l0x.json
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/voice_assistant.json
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/wake_on_lan.json
--rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/waveshare_epaper.json
--rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/web_server.json
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/web_server_base.json
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/whirlpool.json
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/whynter.json
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/wiegand.json
--rw-r--r--   0 runner    (1001) docker     (123)    15821 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/wifi.json
--rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/wifi_info.json
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/wifi_signal.json
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/wl_134.json
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/wled.json
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/x9c.json
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/xiaomi_ble.json
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/xiaomi_cgd1.json
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/xiaomi_cgdk2.json
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/xiaomi_cgg1.json
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/xiaomi_cgpr1.json
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/xiaomi_gcls002.json
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/xiaomi_hhccjcy01.json
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/xiaomi_hhccpot002.json
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/xiaomi_jqjcy01ym.json
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/xiaomi_lywsd02.json
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/xiaomi_lywsd03mmc.json
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/xiaomi_lywsdcgq.json
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/xiaomi_mhoc303.json
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/xiaomi_mhoc401.json
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/xiaomi_miscale.json
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/xiaomi_mjyd02yla.json
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/xiaomi_mue4094rt.json
--rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/xiaomi_rtcgq02lm.json
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/xiaomi_wx08zm.json
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/xpt2046.json
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/yashima.json
--rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-05-15 20:28:18.000000 esphome-dashboard-20230516.0/esphome_dashboard/static/schema/zyaura.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:28:38.539114 esphome-dashboard-20230516.0/esphome_dashboard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-15 20:28:38.000000 esphome-dashboard-20230516.0/esphome_dashboard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23547 2023-05-15 20:28:38.000000 esphome-dashboard-20230516.0/esphome_dashboard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 20:28:38.000000 esphome-dashboard-20230516.0/esphome_dashboard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 20:28:38.000000 esphome-dashboard-20230516.0/esphome_dashboard.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-15 20:28:38.000000 esphome-dashboard-20230516.0/esphome_dashboard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 20:28:38.587113 esphome-dashboard-20230516.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-15 20:27:39.000000 esphome-dashboard-20230516.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:56:10.062827 esphome-dashboard-20230621.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-21 01:55:06.000000 esphome-dashboard-20230621.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-21 01:55:06.000000 esphome-dashboard-20230621.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-21 01:56:10.062827 esphome-dashboard-20230621.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-21 01:55:06.000000 esphome-dashboard-20230621.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:56:10.014827 esphome-dashboard-20230621.0/esphome_dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-21 01:55:26.000000 esphome-dashboard-20230621.0/esphome_dashboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-21 01:55:26.000000 esphome-dashboard-20230621.0/esphome_dashboard/base.template.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-21 01:55:26.000000 esphome-dashboard-20230621.0/esphome_dashboard/base_with_header_footer.template.html
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-21 01:55:26.000000 esphome-dashboard-20230621.0/esphome_dashboard/index.template.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-21 01:55:26.000000 esphome-dashboard-20230621.0/esphome_dashboard/login.template.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:56:10.014827 esphome-dashboard-20230621.0/esphome_dashboard/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:56:10.014827 esphome-dashboard-20230621.0/esphome_dashboard/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-06-21 01:55:26.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/css/esphome-2.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:56:10.014827 esphome-dashboard-20230621.0/esphome_dashboard/static/firmware/
+-rw-r--r--   0 runner    (1001) docker     (123)    15872 2023-06-21 01:55:26.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/firmware/bootloader.bin
+-rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-06-21 01:55:26.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/firmware/ota.bin
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-06-21 01:55:26.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/firmware/partitions.bin
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:56:10.014827 esphome-dashboard-20230621.0/esphome_dashboard/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    72504 2023-06-21 01:55:43.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/fonts/codicon.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:56:10.018827 esphome-dashboard-20230621.0/esphome_dashboard/static/fonts/material-icons/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-21 01:55:26.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/fonts/material-icons/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    57620 2023-06-21 01:55:26.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/fonts/material-icons/MaterialIcons-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    44300 2023-06-21 01:55:26.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/fonts/material-icons/MaterialIcons-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-21 01:55:26.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/fonts/material-icons/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-21 01:55:26.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/fonts/material-icons/material-icons.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:56:10.018827 esphome-dashboard-20230621.0/esphome_dashboard/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-06-21 01:55:26.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-06-21 01:55:26.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/images/logo-text.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:56:10.014827 esphome-dashboard-20230621.0/esphome_dashboard/static/js/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:56:10.022827 esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/
+-rw-r--r--   0 runner    (1001) docker     (123)    83075 2023-06-21 01:56:08.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.1107b6f0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-06-21 01:56:08.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.11743138.js
+-rw-r--r--   0 runner    (1001) docker     (123)    77094 2023-06-21 01:56:08.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.17838855.js
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-21 01:56:08.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.1fccc3bb.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7876 2023-06-21 01:56:08.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.22fb066b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-21 01:56:08.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.25394cef.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-06-21 01:56:08.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.286ad693.js
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-21 01:56:08.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.2d34b51a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-06-21 01:56:08.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.323af3d2.js
+-rw-r--r--   0 runner    (1001) docker     (123)    58095 2023-06-21 01:56:08.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.3bbbdf4b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16738 2023-06-21 01:56:08.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.3f59652f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-21 01:56:08.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.40278fa0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-06-21 01:56:08.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.417d3d2d.js
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-21 01:56:08.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.440fff61.js
+-rw-r--r--   0 runner    (1001) docker     (123)    41533 2023-06-21 01:56:08.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.4971d925.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-06-21 01:56:08.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.4c0eda7e.js
+-rw-r--r--   0 runner    (1001) docker     (123)   233918 2023-06-21 01:56:08.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.5cd5d307.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-06-21 01:56:08.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.64ac3748.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-21 01:56:08.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.670cd819.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-21 01:56:08.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.6951bded.js
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-21 01:56:08.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.7e8b4fbe.js
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-21 01:56:08.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.884f2894.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-06-21 01:56:08.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.8ab91975.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-06-21 01:56:08.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.90e5e76e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-21 01:56:08.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.9d543f02.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-06-21 01:56:08.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.9f55698d.js
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-21 01:56:08.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.9fa8c472.js
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-21 01:56:08.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.a6e96e5a.js
+-rw-r--r--   0 runner    (1001) docker     (123)  2790638 2023-06-21 01:56:08.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.a94304a8.js
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-21 01:56:08.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.b545a09c.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14078 2023-06-21 01:56:08.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.c0a69417.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-06-21 01:56:08.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.c74d5ae3.js
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-21 01:56:08.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.c84471ef.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-21 01:56:08.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.cce2f2f7.js
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-21 01:56:08.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.cd26dc5d.js
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-21 01:56:08.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.d861da54.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-06-21 01:56:08.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.f0358a8b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8648 2023-06-21 01:56:08.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.f4034d2e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-06-21 01:56:08.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.fadc3045.js
+-rw-r--r--   0 runner    (1001) docker     (123)   319198 2023-06-21 01:56:08.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/index-bfcf9cd9.js
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-21 01:56:08.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/manifest.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:56:10.014827 esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/monaco-editor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:56:10.014827 esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/monaco-editor/esm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:56:10.014827 esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/monaco-editor/esm/vs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:56:10.022827 esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/monaco-editor/esm/vs/editor/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-21 01:56:08.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/monaco-editor/esm/vs/editor/editor.worker.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:56:10.062827 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/a4988.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/absolute_humidity.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ac_dimmer.json
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/adalight.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/adc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/adc128s102.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/addressable_light.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ade7953.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ads1115.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/aht10.json
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/airthings_ble.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/airthings_wave_mini.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/airthings_wave_plus.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/am2320.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/am43.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/analog_threshold.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/animation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/anova.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7100 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/apds9960.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/api.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/as3935.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/as3935_i2c.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/as3935_spi.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/as7341.json
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/async_tcp.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/atc_mithermometer.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16157 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/atm90e32.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/b_parasite.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ballu.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/bang_bang.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/bedjet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/bh1750.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/binary.json
+-rw-r--r--   0 runner    (1001) docker     (123)    28755 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/binary_sensor.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/binary_sensor_map.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9157 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/bl0939.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/bl0940.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/bl0942.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18543 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ble_client.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ble_presence.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ble_rssi.json
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ble_scanner.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/bluetooth_proxy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/bme280.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11912 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/bme680.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18394 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/bme680_bsec.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/bmp085.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/bmp280.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/bmp3xx.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/bp1658cj.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/bp5758d.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5386 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/button.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8742 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/canbus.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/cap1188.json
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/captive_portal.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ccs811.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/cd74hc4067.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21700 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/climate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/climate_ir.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/climate_ir_lg.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/color.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/color_temperature.json
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/component.json
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/coolix.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9813 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/copy.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10873 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/cover.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10920 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/cs5460a.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/cse7761.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/cse7766.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ct_clamp.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/current_based.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13964 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/custom.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/custom_component.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/cwww.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/dac7678.json
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/daikin.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/daikin_brc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/dallas.json
+-rw-r--r--   0 runner    (1001) docker     (123)    28349 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/daly_bms.json
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/dashboard_import.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/debug.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10662 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/deep_sleep.json
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/delonghi.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/demo.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/dfplayer.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/dht.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/dht12.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14252 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/display.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/display_menu.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24685 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/display_menu_base.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/dps310.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ds1307.json
+-rw-r--r--   0 runner    (1001) docker     (123)    51328 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/dsmr.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/duty_cycle.json
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/e131.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ee895.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ektf2232.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/endstop.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ens210.json
+-rw-r--r--   0 runner    (1001) docker     (123)    32029 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/esp32.json
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/esp32_ble.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5447 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/esp32_ble_beacon.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/esp32_ble_server.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13007 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/esp32_ble_tracker.json
+-rw-r--r--   0 runner    (1001) docker     (123)    19956 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/esp32_camera.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/esp32_camera_web_server.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/esp32_can.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/esp32_dac.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/esp32_hall.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/esp32_improv.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/esp32_touch.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13930 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/esp8266.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/esp8266_pwm.json
+-rw-r--r--   0 runner    (1001) docker     (123)    87963 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/esphome.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ethernet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ethernet_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/exposure_notifications.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/external_components.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ezo.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21627 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ezo_pmp.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/factory_reset.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11926 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/fan.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/fastled_base.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/fastled_clockless.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/fastled_spi.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/feedback.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18007 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/fingerprint_grow.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/font.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/fs3000.json
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/fujitsu_general.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/globals.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/gpio.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7610 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/gps.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/graph.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16922 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/growatt_solar.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/haier.json
+-rw-r--r--   0 runner    (1001) docker     (123)    25645 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/havells_solar.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/hbridge.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/hdc1080.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/heatpumpir.json
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/hitachi_ac344.json
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/hitachi_ac424.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/hlw8012.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6964 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/hm3301.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/hmc5883l.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/homeassistant.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/honeywellabp.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/hrxl_maxsonar_wr.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/hte501.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/http_request.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/htu21d.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/hx711.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13066 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/hydreon_rgxx.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/hyt271.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/i2c.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/i2s_audio.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ili9xxx.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/image.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/improv_base.json
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/improv_serial.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ina219.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ina226.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ina260.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8315 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ina3221.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6082 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/inkbird_ibsth1_mini.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12726 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/inkplate6.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/integration.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/internal_temperature.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/interval.json
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/json.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/kalman_combinator.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/key_collector.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/kuntze.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/lcd_base.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/lcd_gpio.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/lcd_menu.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/lcd_pcf8574.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11517 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ld2410.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ledc.json
+-rw-r--r--   0 runner    (1001) docker     (123)    80866 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/light.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/lilygo_t5_47.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)   238272 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/logger.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ltr390.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/matrix_keypad.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/max31855.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/max31856.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/max31865.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/max44009.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/max6675.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/max6956.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/max7219.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8560 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/max7219digit.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6456 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/max9611.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mcp23008.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mcp23016.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mcp23017.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mcp23s08.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mcp23s17.json
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mcp23xxx.json
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mcp23xxx_base.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mcp2515.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mcp3008.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mcp3204.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mcp4725.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mcp4728.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mcp47a1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mcp9600.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mcp9808.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mdns.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/media_player.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mhz19.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/microphone.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mics_4514.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10822 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/midea.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/midea_ac.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/midea_ir.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mitsubishi.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11764 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mlx90393.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mlx90614.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mmc5603.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/modbus.json
+-rw-r--r--   0 runner    (1001) docker     (123)    49191 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/modbus_controller.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/monochromatic.json
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mopeka_ble.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mopeka_pro_check.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mopeka_std_check.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mpl3115a2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mpr121.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mpu6050.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6959 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mpu6886.json
+-rw-r--r--   0 runner    (1001) docker     (123)    22240 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mqtt.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mqtt_subscribe.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ms5611.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/my9231.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/neopixelbus.json
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/network.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20223 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/nextion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ntc.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15235 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/number.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ota.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20277 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/output.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/packages.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/page.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/partition.json
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/pca6416a.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/pca9554.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/pca9685.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/pcd8544.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/pcf85063.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/pcf8574.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20589 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/pid.json
+-rw-r--r--   0 runner    (1001) docker     (123)    73941 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/pipsolar.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/pm1006.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11184 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/pmsa003i.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16777 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/pmsx003.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/pn532.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/pn532_i2c.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/pn532_spi.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/power_supply.json
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/preferences.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/prometheus.json
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/psram.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/pulse_counter.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/pulse_meter.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/pulse_width.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8096 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/pvvx_mithermometer.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/pzem004t.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/pzemac.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/pzemdc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/qmc5883l.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6620 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/qmp6988.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/qr_code.json
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/radon_eye_ble.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/radon_eye_rd200.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/rc522.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/rc522_i2c.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/rc522_spi.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/rdm6300.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/remote_base.json
+-rw-r--r--   0 runner    (1001) docker     (123)    47870 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/remote_receiver.json
+-rw-r--r--   0 runner    (1001) docker     (123)    47223 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/remote_transmitter.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/resistance.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/restart.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/rf_bridge.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/rgb.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/rgbct.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/rgbw.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/rgbww.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/rotary_encoder.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/rp2040.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/rp2040_pwm.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/rtttl.json
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ruuvi_ble.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14474 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ruuvitag.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/safe_mode.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/scd30.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11509 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/scd4x.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/script.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16724 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sdm_meter.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sdp3x.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sds011.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17512 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/selec_meter.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10334 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/select.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sen21231.json
+-rw-r--r--   0 runner    (1001) docker     (123)    25256 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sen5x.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/senseair.json
+-rw-r--r--   0 runner    (1001) docker     (123)   106836 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sensor.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/servo.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10669 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sgp30.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15212 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sgp4x.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9201 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/shelly_dimmer.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sht3xd.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sht4x.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/shtcx.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/shutdown.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sigma_delta_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10343 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sim800l.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/slow_pwm.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sm10bit_base.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sm16716.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sm2135.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sm2235.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sm2335.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10974 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sm300d2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sml.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/smt100.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sn74hc165.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sn74hc595.json
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sntp.json
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/socket.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sonoff_d1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/speed.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/spi.json
+-rw-r--r--   0 runner    (1001) docker     (123)    53606 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sprinkler.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15586 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sps30.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ssd1306_base.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ssd1306_i2c.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ssd1306_spi.json
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ssd1322_base.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ssd1322_spi.json
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ssd1325_base.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ssd1325_spi.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ssd1327_base.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ssd1327_i2c.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ssd1327_spi.json
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ssd1331_base.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ssd1331_spi.json
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ssd1351_base.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ssd1351_spi.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/st7735.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/st7789v.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/st7920.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/status.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/status_led.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8316 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/stepper.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sts3x.json
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/substitutions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8353 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sun.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/switch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sx1509.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/t6615.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/tca9548a.json
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/tcl112.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8310 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/tcs34725.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/tee501.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/teleinfo.json
+-rw-r--r--   0 runner    (1001) docker     (123)    38023 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/template.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11115 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/text_sensor.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11486 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/thermostat.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/time.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/time_based.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/tlc59208f.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/tlc5947.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/tm1621.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/tm1637.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/tm1638.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/tm1651.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/tmp102.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/tmp117.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/tof10120.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/toshiba.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/total_daily_energy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/touchscreen.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/tsl2561.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10223 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/tsl2591.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ttp229_bsf.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ttp229_lsf.json
+-rw-r--r--   0 runner    (1001) docker     (123)    33914 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/tuya.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/tx20.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7313 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/uart.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ufire_ec.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6987 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ufire_ise.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/uln2003.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ultrasonic.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/uptime.json
+-rw-r--r--   0 runner    (1001) docker     (123)    55804 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/vbus.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/version.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/vl53l0x.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/voice_assistant.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/wake_on_lan.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/waveshare_epaper.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/web_server.json
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/web_server_base.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/whirlpool.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/whynter.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/wiegand.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15821 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/wifi.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/wifi_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/wifi_signal.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/wl_134.json
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/wled.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/x9c.json
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/xiaomi_ble.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/xiaomi_cgd1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/xiaomi_cgdk2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/xiaomi_cgg1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/xiaomi_cgpr1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/xiaomi_gcls002.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/xiaomi_hhccjcy01.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/xiaomi_hhccpot002.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/xiaomi_jqjcy01ym.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/xiaomi_lywsd02.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/xiaomi_lywsd03mmc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/xiaomi_lywsdcgq.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/xiaomi_mhoc303.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/xiaomi_mhoc401.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/xiaomi_miscale.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/xiaomi_mjyd02yla.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/xiaomi_mue4094rt.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/xiaomi_rtcgq02lm.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/xiaomi_wx08zm.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/xpt2046.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/yashima.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-06-21 01:55:48.000000 esphome-dashboard-20230621.0/esphome_dashboard/static/schema/zyaura.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:56:10.014827 esphome-dashboard-20230621.0/esphome_dashboard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-21 01:56:09.000000 esphome-dashboard-20230621.0/esphome_dashboard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23547 2023-06-21 01:56:09.000000 esphome-dashboard-20230621.0/esphome_dashboard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 01:56:09.000000 esphome-dashboard-20230621.0/esphome_dashboard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 01:56:09.000000 esphome-dashboard-20230621.0/esphome_dashboard.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 01:56:09.000000 esphome-dashboard-20230621.0/esphome_dashboard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 01:56:10.062827 esphome-dashboard-20230621.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-21 01:55:06.000000 esphome-dashboard-20230621.0/setup.py
```

### Comparing `esphome-dashboard-20230516.0/LICENSE` & `esphome-dashboard-20230621.0/LICENSE`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/README.md` & `esphome-dashboard-20230621.0/README.md`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/base.template.html` & `esphome-dashboard-20230621.0/esphome_dashboard/base.template.html`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/base_with_header_footer.template.html` & `esphome-dashboard-20230621.0/esphome_dashboard/base_with_header_footer.template.html`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/login.template.html` & `esphome-dashboard-20230621.0/esphome_dashboard/login.template.html`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/firmware/bootloader.bin` & `esphome-dashboard-20230621.0/esphome_dashboard/static/firmware/bootloader.bin`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/firmware/partitions.bin` & `esphome-dashboard-20230621.0/esphome_dashboard/static/firmware/partitions.bin`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/fonts/codicon.ttf` & `esphome-dashboard-20230621.0/esphome_dashboard/static/fonts/codicon.ttf`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/fonts/material-icons/LICENSE` & `esphome-dashboard-20230621.0/esphome_dashboard/static/fonts/material-icons/LICENSE`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/fonts/material-icons/MaterialIcons-Regular.woff` & `esphome-dashboard-20230621.0/esphome_dashboard/static/fonts/material-icons/MaterialIcons-Regular.woff`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/fonts/material-icons/MaterialIcons-Regular.woff2` & `esphome-dashboard-20230621.0/esphome_dashboard/static/fonts/material-icons/MaterialIcons-Regular.woff2`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/fonts/material-icons/material-icons.css` & `esphome-dashboard-20230621.0/esphome_dashboard/static/fonts/material-icons/material-icons.css`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/images/favicon.ico` & `esphome-dashboard-20230621.0/esphome_dashboard/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/images/logo-text.svg` & `esphome-dashboard-20230621.0/esphome_dashboard/static/images/logo-text.svg`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.1bc018ae.js` & `esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.22fb066b.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,21 +1,21 @@
 import {
     b as e,
     n as t,
-    a6 as o,
+    a7 as o,
     h as s,
     G as r,
     r as n,
     d as a,
     l,
     s as i,
     y as c,
-    a4 as d
-} from "./index-d3dd97b9.js";
-import "./c.e4466087.js";
+    a5 as d
+} from "./index-bfcf9cd9.js";
+import "./c.4971d925.js";
 class g {
     constructor(e) {
         this.targetElement = e, this.state = {
             bold: !1,
             italic: !1,
             underline: !1,
             strikethrough: !1,
```

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.1c31574e.js` & `esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.fadc3045.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -4,27 +4,27 @@
     b as i,
     d as s,
     l as o,
     i as a,
     n,
     s as r,
     y as d,
-    U as l,
+    V as l,
     h as c,
     C as h
-} from "./index-d3dd97b9.js";
-import "./c.e4466087.js";
-import "./c.834bbab0.js";
+} from "./index-bfcf9cd9.js";
+import "./c.4971d925.js";
+import "./c.1107b6f0.js";
 import {
     c as p,
     s as m
-} from "./c.dde41422.js";
+} from "./c.2d34b51a.js";
 import {
     o as u
-} from "./c.45f3bfa8.js";
+} from "./c.d861da54.js";
 import {
     c as y
 } from "./c.440fff61.js";
 import {
     s as _
 } from "./c.a6e96e5a.js";
 let f = class extends r {
```

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.286ad693.js` & `esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.286ad693.js`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.29c28c21.js` & `esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.8ab91975.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,55 +1,56 @@
 import {
-    r as o,
-    b as e,
-    d as t,
-    i as n,
-    l as i,
-    n as s,
-    s as c,
-    y as a,
-    P as l,
-    H as r,
-    a4 as d
-} from "./index-d3dd97b9.js";
-import "./c.e4466087.js";
+    G as o,
+    r as e,
+    b as t,
+    d as n,
+    i,
+    l as s,
+    n as c,
+    s as a,
+    y as l,
+    Q as r,
+    I as d,
+    a5 as h
+} from "./index-bfcf9cd9.js";
+import "./c.4971d925.js";
 import {
-    c as h,
-    C as p,
-    b as u
-} from "./c.1bc018ae.js";
+    c as p,
+    C as u,
+    b as g
+} from "./c.22fb066b.js";
 import {
-    s as g
+    s as w
 } from "./c.a6e96e5a.js";
-class w {
+class m {
     constructor() {
         this.chunks = ""
     }
     transform(o, e) {
         this.chunks += o;
         const t = this.chunks.split("\r\n");
         this.chunks = t.pop(), t.forEach((o => e.enqueue(o + "\r\n")))
     }
     flush(o) {
         o.enqueue(this.chunks)
     }
 }
-class m extends HTMLElement {
+class f extends HTMLElement {
     constructor() {
         super(...arguments), this.allowInput = !0
     }
     logs() {
         var o;
         return (null === (o = this._console) || void 0 === o ? void 0 : o.logs()) || ""
     }
     connectedCallback() {
         if (this._console) return;
         if (this.attachShadow({
                 mode: "open"
-            }).innerHTML = `\n      <style>\n        :host, input {\n          background-color: #1c1c1c;\n          color: #ddd;\n          font-family: "SFMono-Regular", Consolas, "Liberation Mono", Menlo, Courier,\n            monospace;\n          line-height: 1.45;\n          display: flex;\n          flex-direction: column;\n        }\n        form {\n          display: flex;\n          align-items: center;\n          padding: 0 8px 0 16px;\n        }\n        input {\n          flex: 1;\n          padding: 4px;\n          margin: 0 8px;\n          border: 0;\n          outline: none;\n        }\n        ${h}\n      </style>\n      <div class="log"></div>\n      ${this.allowInput?"<form>\n                >\n                <input autofocus>\n              </form>\n            ":""}\n    `, this._console = new p(this.shadowRoot.querySelector("div")), this.allowInput) {
+            }).innerHTML = `\n      <style>\n        :host, input {\n          background-color: #1c1c1c;\n          color: #ddd;\n          font-family: "SFMono-Regular", Consolas, "Liberation Mono", Menlo, Courier,\n            monospace;\n          line-height: 1.45;\n          display: flex;\n          flex-direction: column;\n        }\n        form {\n          display: flex;\n          align-items: center;\n          padding: 0 8px 0 16px;\n        }\n        input {\n          flex: 1;\n          padding: 4px;\n          margin: 0 8px;\n          border: 0;\n          outline: none;\n        }\n        ${p}\n      </style>\n      <div class="log"></div>\n      ${this.allowInput?"<form>\n                >\n                <input autofocus>\n              </form>\n            ":""}\n    `, this._console = new u(this.shadowRoot.querySelector("div")), this.allowInput) {
             const o = this.shadowRoot.querySelector("input");
             this.addEventListener("click", (() => {
                 var e;
                 "" === (null === (e = getSelection()) || void 0 === e ? void 0 : e.toString()) && o.focus()
             })), o.addEventListener("keydown", (o => {
                 "Enter" === o.key && (o.preventDefault(), o.stopPropagation(), this._sendCommand())
             }))
@@ -59,23 +60,23 @@
         this._cancelConnection = () => (o.abort(), e)
     }
     async _connect(o) {
         this.logger.debug("Starting console read loop");
         try {
             await this.port.readable.pipeThrough(new TextDecoderStream, {
                 signal: o
-            }).pipeThrough(new TransformStream(new w)).pipeTo(new WritableStream({
+            }).pipeThrough(new TransformStream(new m)).pipeTo(new WritableStream({
                 write: o => {
                     this._console.addLine(o.replace("\r", ""))
                 }
             })), o.aborted || (this._console.addLine(""), this._console.addLine(""), this._console.addLine("Terminal disconnected"))
         } catch (o) {
             this._console.addLine(""), this._console.addLine(""), this._console.addLine(`Terminal disconnected: ${o}`)
         } finally {
-            await g(100), this.logger.debug("Finished console read loop")
+            await w(100), this.logger.debug("Finished console read loop")
         }
     }
     async _sendCommand() {
         const o = this.shadowRoot.querySelector("input"),
             e = o.value,
             t = new TextEncoder,
             n = this.port.writable.getWriter();
@@ -95,21 +96,21 @@
             requestToSend: !0
         }), await this.port.setSignals({
             dataTerminalReady: !1,
             requestToSend: !1
         }), await new Promise((o => setTimeout(o, 1e3)))
     }
 }
-customElements.define("ewt-console", m);
-let f = class extends c {
+customElements.define("ewt-console", f);
+let _ = class extends a {
     constructor() {
         super(...arguments), this._isPico = !1
     }
     render() {
-        return a`
+        return l`
       <mwc-dialog
         open
         .heading=${this.configuration?`Logs ${this.configuration}`:"Logs"}
         scrimClickAction
         @closed=${this._handleClose}
       >
         <ewt-console
@@ -118,23 +119,23 @@
           .allowInput=${!1}
         ></ewt-console>
         <mwc-button
           slot="secondaryAction"
           label="Download Logs"
           @click=${this._downloadLogs}
         ></mwc-button>
-        ${this.configuration?a`
+        ${this.configuration?l`
               <mwc-button
                 slot="secondaryAction"
                 dialogAction="close"
                 label="Edit"
                 @click=${this._openEdit}
               ></mwc-button>
             `:""}
-        ${this._isPico?"":a`
+        ${this._isPico?"":l`
               <mwc-button
                 slot="secondaryAction"
                 label="Reset Device"
                 @click=${this._resetDevice}
               ></mwc-button>
             `}
         <mwc-button
@@ -142,33 +143,33 @@
           dialogAction="close"
           label="Close"
         ></mwc-button>
       </mwc-dialog>
     `
     }
     firstUpdated(o) {
-        super.firstUpdated(o), this.configuration && l(this.configuration).then((o => {
+        super.firstUpdated(o), this.configuration && r(this.configuration).then((o => {
             this._isPico = "RP2040" === o.esp_platform
         }))
     }
     async _openEdit() {
-        this.configuration && r(this.configuration)
+        this.configuration && d(this.configuration)
     }
     async _handleClose() {
         await this._console.disconnect(), this.closePortOnClose && await this.port.close(), this.parentNode.removeChild(this)
     }
     async _resetDevice() {
         await this._console.reset()
     }
     _downloadLogs() {
-        d(this._console.logs(), (this.configuration ? `${u(this.configuration)}_logs` : "logs") + ".txt")
+        h(this._console.logs(), (this.configuration ? `${g(this.configuration)}_logs` : "logs") + ".txt")
     }
 };
-f.styles = o`
-    mwc-dialog {
-      --mdc-dialog-max-width: 90vw;
-    }
-    ewt-console {
-      width: calc(80vw - 48px);
-      height: calc(90vh - 128px);
-    }
-  `, e([t()], f.prototype, "configuration", void 0), e([t()], f.prototype, "port", void 0), e([t()], f.prototype, "closePortOnClose", void 0), e([n("ewt-console")], f.prototype, "_console", void 0), e([i()], f.prototype, "_isPico", void 0), f = e([s("esphome-logs-webserial-dialog")], f);
+_.styles = [o, e`
+      mwc-dialog {
+        --mdc-dialog-max-width: 90vw;
+      }
+      ewt-console {
+        width: calc(80vw - 48px);
+        height: calc(90vh - 128px);
+      }
+    `], t([n()], _.prototype, "configuration", void 0), t([n()], _.prototype, "port", void 0), t([n()], _.prototype, "closePortOnClose", void 0), t([i("ewt-console")], _.prototype, "_console", void 0), t([s()], _.prototype, "_isPico", void 0), _ = t([c("esphome-logs-webserial-dialog")], _);
```

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.2b18cdda.js` & `esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.323af3d2.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 import {
     m as e
-} from "./c.5cae2e65.js";
-import "./index-d3dd97b9.js";
+} from "./c.a94304a8.js";
+import "./index-bfcf9cd9.js";
 import "./c.5cd5d307.js";
-import "./c.e4466087.js";
+import "./c.4971d925.js";
 var n, t, r = Object.defineProperty,
     o = Object.getOwnPropertyDescriptor,
     l = Object.getOwnPropertyNames,
     i = Object.prototype.hasOwnProperty,
     a = (e, n, t, a) => {
         if (n && "object" == typeof n || "function" == typeof n)
             for (let c of l(n)) i.call(e, c) || c === t || r(e, c, {
```

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.363ea4b9.js` & `esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.9fa8c472.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
 import {
     b as e,
     d as o,
     n as s,
     s as i,
     y as t
-} from "./index-d3dd97b9.js";
-import "./c.1bc018ae.js";
-import "./c.e4466087.js";
+} from "./index-bfcf9cd9.js";
+import "./c.22fb066b.js";
+import "./c.4971d925.js";
 let a = class extends i {
     render() {
         return t`
       <esphome-process-dialog
         .heading=${`Clean MQTT discovery topics for ${this.configuration}`}
         .type=${"clean-mqtt"}
         .spawnParams=${{configuration:this.configuration}}
```

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.3b4072f5.js` & `esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.cd26dc5d.js`

 * *Files 24% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 import {
-    Q as a
-} from "./index-d3dd97b9.js";
+    S as a
+} from "./index-bfcf9cd9.js";
 import {
     s as t
 } from "./c.a6e96e5a.js";
 const e = async t => {
     let e;
     try {
         e = await fetch(a(t, !0))
```

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.417d3d2d.js` & `esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.417d3d2d.js`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.52f07dd8.js` & `esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.cce2f2f7.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -1,19 +1,19 @@
 import {
     b as o,
     d as i,
     l as t,
     n as s,
     s as e,
     y as a,
-    H as n,
+    I as n,
     j as l
-} from "./index-d3dd97b9.js";
-import "./c.1bc018ae.js";
-import "./c.e4466087.js";
+} from "./index-bfcf9cd9.js";
+import "./c.22fb066b.js";
+import "./c.4971d925.js";
 let d = class extends e {
     render() {
         const o = void 0 === this._valid ? "" : this._valid ? "✅" : "❌";
         return a`
       <esphome-process-dialog
         .heading=${`Validate ${this.configuration} ${o}`}
         .type=${"validate"}
```

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.5cae2e65.js` & `esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.a94304a8.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -17,15 +17,15 @@
     r as m,
     n as f,
     s as _,
     h as v,
     j as b,
     w,
     k as C
-} from "./index-d3dd97b9.js";
+} from "./index-bfcf9cd9.js";
 import {
     m as y,
     D as S,
     a as k,
     i as x,
     b as L,
     K as D,
@@ -265,15 +265,15 @@
     cW as $n,
     cX as qn,
     cY as Gn,
     cZ as Zn,
     c_ as Yn,
     c$ as Qn
 } from "./c.5cd5d307.js";
-import "./c.e4466087.js";
+import "./c.4971d925.js";
 
 function Xn(e, t) {
     void 0 === t && (t = {});
     var i = t.insertAt;
     if (e && "undefined" != typeof document) {
         var n = document.head || document.getElementsByTagName("head")[0],
             o = document.createElement("style");
@@ -79225,15 +79225,15 @@
     }))
 }
 E4({
     id: "yaml",
     extensions: [".yaml", ".yml"],
     aliases: ["YAML", "yaml", "YML", "yml"],
     mimetypes: ["application/x-yaml", "text/x-yaml"],
-    loader: () => import("./c.2b18cdda.js")
+    loader: () => import("./c.323af3d2.js")
 });
 var M4 = Object.freeze({
         __proto__: null,
         CancellationTokenSource: u4,
         Emitter: g4,
         KeyCode: p4,
         KeyMod: m4,
@@ -84584,20 +84584,32 @@
         token: "type",
         foreground: "000099",
         fontStyle: ""
     }],
     colors: {
         "editor.foreground": "#000000"
     }
+}), k4.defineTheme("esphome-dark", {
+    base: "vs-dark",
+    inherit: !0,
+    rules: [{
+        token: "type",
+        foreground: "E8E8E9",
+        fontStyle: ""
+    }],
+    colors: {
+        "editor.foreground": "#E8E8E9"
+    }
 });
 const u7 = window.location,
     g7 = new URL("./", `${u7.protocol}//${u7.host}${u7.pathname}`);
 g7.protocol = "ws:", "https:" === u7.protocol && (g7.protocol = "wss:");
-const p7 = g7.href;
-let m7 = class extends _ {
+const p7 = g7.href,
+    m7 = window.matchMedia("(prefers-color-scheme: dark)");
+let f7 = class extends _ {
     constructor() {
         super(...arguments), this.editorActiveWebSocket = null, this.editorValidationScheduled = !1, this.editorValidationRunning = !1, this.editorActiveSecrets = !1, this._handleResize = () => {
             var e;
             null === (e = this.editor) || void 0 === e || e.layout(this.calcEditorSize())
         }
     }
     createRenderRoot() {
@@ -84614,31 +84626,31 @@
         }
         .esphome-header {
           display: flex;
           justify-content: space-between;
           align-items: center;
           align-content: stretch;
         }
-        .esphome-header mwc-button {
-          --mdc-theme-primary: black;
-        }
         h2 {
           line-height: 100%;
           /* this margin, padding stretches the container, offsetHeight does not calculate margin of .editor-header */
           padding: 0.8rem 0.5rem 1rem 0.5rem;
           margin: 0px;
           font-size: 1.4rem;
           flex: 1 1 auto;
           overflow: hidden;
           white-space: nowrap;
           text-overflow: ellipsis;
         }
         mwc-icon-button {
           --mdc-icon-button-size: 32px;
         }
+        mwc-button {
+          --mdc-theme-primary: var(--primary-text-color);
+        }
       </style>
       <mwc-snackbar leading></mwc-snackbar>
 
       <div class="esphome-header">
         <mwc-icon-button
           icon="clear"
           @click=${this._handleClose}
@@ -84684,29 +84696,31 @@
     }
     firstUpdated() {
         var e;
         self.MonacoEnvironment = {
             getWorkerUrl: function(e, t) {
                 return "./static/js/esphome/monaco-editor/esm/vs/editor/editor.worker.js"
             }
-        }, this.editor = k4.create(this.container, {
+        }, m7.addEventListener("change", (() => {
+            k4.setTheme(m7.matches ? "esphome-dark" : "esphome")
+        })), this.editor = k4.create(this.container, {
             value: "",
             language: "yaml",
-            theme: "esphome",
+            theme: m7.matches ? "esphome-dark" : "esphome",
             minimap: {
                 enabled: !1
             },
             tabSize: 2,
             dimension: this.calcEditorSize(),
             fontFamily: 'ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,"Liberation Mono","Courier New",monospace'
         });
         const t = "secrets.yaml" === this.fileName || "secrets.yml" === this.fileName;
         C(this.fileName).then((e => {
             var i;
-            null === e && t && (e = f7), null === (i = this.editor) || void 0 === i || i.setValue(null != e ? e : ""), this.startAceWebsocket()
+            null === e && t && (e = _7), null === (i = this.editor) || void 0 === i || i.setValue(null != e ? e : ""), this.startAceWebsocket()
         })), this.editor.focus(), null === (e = this.editor.getModel()) || void 0 === e || e.onDidChangeContent(Y4((() => {
             this.editorValidationScheduled = !this.editorActiveSecrets
         }), 250)), this.editor.addAction({
             id: "action-save-file",
             label: "Save file",
             keybindings: [m4.CtrlCmd | p4.KeyS],
             run: () => {
@@ -84785,15 +84799,15 @@
     connectedCallback() {
         super.connectedCallback(), window.addEventListener("resize", this._handleResize)
     }
     disconnectedCallback() {
         window.removeEventListener("resize", this._handleResize), super.disconnectedCallback()
     }
 };
-l([c()], m7.prototype, "fileName", void 0), l([d("mwc-snackbar", !0)], m7.prototype, "_snackbar", void 0), l([d("main", !0)], m7.prototype, "container", void 0), l([d(".esphome-header", !0)], m7.prototype, "editor_header", void 0), m7 = l([f("esphome-editor")], m7);
-const f7 = '# Your Wi-Fi SSID and password\nwifi_ssid: "REPLACEME"\nwifi_password: "REPLACEME"\n';
-var _7 = Object.freeze({
+l([c()], f7.prototype, "fileName", void 0), l([d("mwc-snackbar", !0)], f7.prototype, "_snackbar", void 0), l([d("main", !0)], f7.prototype, "container", void 0), l([d(".esphome-header", !0)], f7.prototype, "editor_header", void 0), f7 = l([f("esphome-editor")], f7);
+const _7 = '# Your Wi-Fi SSID and password\nwifi_ssid: "REPLACEME"\nwifi_password: "REPLACEME"\n';
+var v7 = Object.freeze({
     __proto__: null
 });
 export {
-    _7 as e, M4 as m
+    v7 as e, M4 as m
 };
```

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.5cd5d307.js` & `esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.5cd5d307.js`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.61332c08.js` & `esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.f0358a8b.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,83 +1,84 @@
 import {
     G as t,
-    r as o,
-    b as e,
-    d as s,
-    l as i,
-    n as r,
-    s as n,
-    y as a
-} from "./index-d3dd97b9.js";
-import "./c.e4466087.js";
-import "./c.1bc018ae.js";
+    H as o,
+    r as e,
+    b as s,
+    d as i,
+    l as r,
+    n,
+    s as a,
+    y as c
+} from "./index-bfcf9cd9.js";
+import "./c.4971d925.js";
+import "./c.22fb066b.js";
 import {
-    g as c
-} from "./c.7d2e85dd.js";
+    g as l
+} from "./c.c84471ef.js";
 import {
-    m as l,
-    s as p,
-    b as m
-} from "./c.e683a7a9.js";
-const h = (t, o) => {
-        import("./c.e6db31ca.js");
+    m as p,
+    s as m,
+    b as h
+} from "./c.884f2894.js";
+const d = (t, o) => {
+        import("./c.40278fa0.js");
         const e = document.createElement("esphome-logs-dialog");
         e.configuration = t, e.target = o, document.body.append(e)
     },
-    d = (t, o, e) => {
-        import("./c.29c28c21.js");
+    w = (t, o, e) => {
+        import("./c.8ab91975.js");
         const s = document.createElement("esphome-logs-webserial-dialog");
         s.configuration = e, s.port = t, s.closePortOnClose = o, document.body.append(s)
     };
-let w = class extends n {
+let u = class extends a {
     constructor() {
         super(...arguments), this._show = "options"
     }
     render() {
         let t, o;
-        return "options" === this._show ? (t = "How to get the logs for your device?", o = a`
+        return "options" === this._show ? (t = "How to get the logs for your device?", o = c`
         <mwc-list-item
           twoline
           hasMeta
           dialogAction="close"
           .port=${"OTA"}
           @click=${this._pickPort}
         >
           <span>Wirelessly</span>
           <span slot="secondary">Requires the device to be online</span>
-          ${l}
+          ${p}
         </mwc-list-item>
 
         <mwc-list-item
           twoline
           hasMeta
           .port=${"WEBSERIAL"}
           @click=${this._pickWebSerial}
         >
           <span>Plug into this computer</span>
           <span slot="secondary">
             For devices connected via USB to this computer
           </span>
-          ${l}
+          ${p}
         </mwc-list-item>
 
         <mwc-list-item twoline hasMeta @click=${this._showServerPorts}>
           <span>Plug into computer running ESPHome Dashboard</span>
           <span slot="secondary">
             For devices connected via USB to the server
           </span>
-          ${l}
+          ${p}
         </mwc-list-item>
         <mwc-button
           no-attention
           slot="primaryAction"
           dialogAction="close"
           label="Cancel"
         ></mwc-button>
-      `) : "web_instructions" === this._show ? (t = "View logs in the browser", o = a`
+      `) : "web_instructions" === this._show ? (t = "View logs in the browser", o = c`
         <div>
           ESPHome can view the logs of your device via the browser if certain
           requirements are met:
         </div>
         <ul>
           <li>ESPHome is visited over HTTPS</li>
           <li>Your browser supports WebSerial</li>
@@ -101,81 +102,81 @@
         </a>
         <mwc-button
           no-attention
           slot="secondaryAction"
           label="Back"
           @click=${()=>{this._show="options"}}
         ></mwc-button>
-      `) : (t = "Pick server port", o = a`${void 0===this._ports?a`
+      `) : (t = "Pick server port", o = c`${void 0===this._ports?c`
               <mwc-list-item>
                 <span>Loading ports…</span>
               </mwc-list-item>
-            `:0===this._ports.length?a`
+            `:0===this._ports.length?c`
               <mwc-list-item>
                 <span>No serial ports found.</span>
               </mwc-list-item>
-            `:this._ports.map((t=>a`
+            `:this._ports.map((t=>c`
                 <mwc-list-item
                   twoline
                   hasMeta
                   dialogAction="close"
                   .port=${t.port}
                   @click=${this._pickPort}
                 >
                   <span>${t.desc}</span>
                   <span slot="secondary">${t.port}</span>
-                  ${l}
+                  ${p}
                 </mwc-list-item>
               `))}
 
         <mwc-button
           no-attention
           slot="primaryAction"
           label="Back"
           @click=${()=>{this._show="options"}}
-        ></mwc-button>`), a`
+        ></mwc-button>`), c`
       <mwc-dialog
         open
         heading=${t}
         scrimClickAction
         @closed=${this._handleClose}
       >
         ${o}
       </mwc-dialog>
     `
     }
     firstUpdated(t) {
-        super.firstUpdated(t), c().then((t => {
-            0 !== t.length || p ? this._ports = t : (this._handleClose(), h(this.configuration, "OTA"))
+        super.firstUpdated(t), l().then((t => {
+            0 !== t.length || m ? this._ports = t : (this._handleClose(), d(this.configuration, "OTA"))
         }))
     }
     _showServerPorts() {
         this._show = "server_ports"
     }
     _pickPort(t) {
-        h(this.configuration, t.currentTarget.port)
+        d(this.configuration, t.currentTarget.port)
     }
     async _pickWebSerial(t) {
-        if (p && m) try {
+        if (m && h) try {
             const t = await navigator.serial.requestPort();
             await t.open({
                 baudRate: 115200
-            }), this.shadowRoot.querySelector("mwc-dialog").close(), d(t, !0, this.configuration)
+            }), this.shadowRoot.querySelector("mwc-dialog").close(), w(t, !0, this.configuration)
         } catch (t) {
             console.error(t)
         } else this._show = "web_instructions"
     }
     _handleClose() {
         this.parentNode.removeChild(this)
     }
 };
-w.styles = [t, o`
+u.styles = [t, o, e`
       mwc-list-item {
         margin: 0 -20px;
       }
-    `], e([s()], w.prototype, "configuration", void 0), e([i()], w.prototype, "_ports", void 0), e([i()], w.prototype, "_show", void 0), w = e([r("esphome-logs-target-dialog")], w);
-var u = Object.freeze({
+    `], s([i()], u.prototype, "configuration", void 0), s([r()], u.prototype, "_ports", void 0), s([r()], u.prototype, "_show", void 0), u = s([n("esphome-logs-target-dialog")], u);
+var g = Object.freeze({
     __proto__: null
 });
 export {
-    u as l, h as o
+    g as l, d as o
 };
```

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.6d280f04.js` & `esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.64ac3748.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -4,18 +4,18 @@
     b as o,
     d as a,
     l as r,
     i,
     n as s,
     s as n,
     y as l
-} from "./index-d3dd97b9.js";
-import "./c.834bbab0.js";
-import "./c.e4466087.js";
-const c = () => import("./c.ed145062.js");
+} from "./index-bfcf9cd9.js";
+import "./c.1107b6f0.js";
+import "./c.4971d925.js";
+const c = () => import("./c.25394cef.js");
 let m = class extends n {
     constructor() {
         super(...arguments), this._cleanNameInput = e => {
             this._error = void 0;
             const t = e.target;
             t.value = t.value.toLowerCase().replace(/[ \._]/g, "-").replace(/[^a-z0-9-]/g, "")
         }, this._cleanNameBlur = e => {
```

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.6eebcb7a.js` & `esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.4c0eda7e.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,17 +1,17 @@
 import {
     G as e,
     r as t,
     b as o,
     n as l,
     s as i,
     y as s,
-    T as n
-} from "./index-d3dd97b9.js";
-import "./c.e4466087.js";
+    U as n
+} from "./index-bfcf9cd9.js";
+import "./c.4971d925.js";
 const a = n`
   <svg
     version="1.1"
     id="Capa_1"
     xmlns="http://www.w3.org/2000/svg"
     xmlns:xlink="http://www.w3.org/1999/xlink"
     x="0px"
```

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.734d4b21.js` & `esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.b545a09c.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,18 +1,18 @@
 import {
     b as o,
     d as t,
     n as i,
     s as n,
     y as e,
-    H as s,
+    I as s,
     j as a
-} from "./index-d3dd97b9.js";
-import "./c.1bc018ae.js";
-import "./c.e4466087.js";
+} from "./index-bfcf9cd9.js";
+import "./c.22fb066b.js";
+import "./c.4971d925.js";
 let l = class extends n {
     render() {
         return e`
       <esphome-process-dialog
         .heading=${`Clean ${this.configuration}`}
         .type=${"clean"}
         .spawnParams=${{configuration:this.configuration}}
```

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.78cf8c6e.js` & `esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.9d543f02.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -3,16 +3,16 @@
     d as t,
     n as o,
     s as a,
     y as i,
     F as n,
     h as l,
     r as s
-} from "./index-d3dd97b9.js";
-import "./c.e4466087.js";
+} from "./index-bfcf9cd9.js";
+import "./c.4971d925.js";
 let r = class extends a {
     render() {
         return i`
       <mwc-dialog
         .heading=${`Delete ${this.name}`}
         @closed=${this._handleClose}
         open
```

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.834bbab0.js` & `esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.1107b6f0.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -7,27 +7,27 @@
     d as n,
     B as o,
     f as a,
     y as r,
     r as c,
     n as s,
     e as m,
-    X as f,
+    Y as f,
     t as p,
-    Y as h,
-    $ as u,
-    I as x,
-    a0 as g,
-    a1 as b,
+    $ as h,
+    a0 as u,
+    J as x,
+    a1 as g,
+    a2 as b,
     o as v,
     l as _,
     q as y,
     u as w,
     g as E
-} from "./index-d3dd97b9.js";
+} from "./index-bfcf9cd9.js";
 var I = {
         NOTCH_ELEMENT_SELECTOR: ".mdc-notched-outline__notch"
     },
     L = {
         NOTCH_ELEMENT_PADDING: 8
     },
     C = {
```

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.98e8e8d2.js` & `esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.11743138.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,36 +1,36 @@
 import {
     s as t,
     y as e,
-    P as r,
+    Q as r,
     D as i,
     G as s,
     r as o,
     b as a,
     d as n,
     l,
     n as c
-} from "./index-d3dd97b9.js";
-import "./c.e4466087.js";
-import "./c.bff582f5.js";
+} from "./index-bfcf9cd9.js";
+import "./c.4971d925.js";
+import "./c.17838855.js";
 import {
     f as d,
     r as p,
     g as h
-} from "./c.3b4072f5.js";
+} from "./c.cd26dc5d.js";
 import {
     o as _,
     a as g
-} from "./c.9e5eaea1.js";
+} from "./c.3f59652f.js";
 import {
     c as m
-} from "./c.e683a7a9.js";
+} from "./c.884f2894.js";
 import "./c.a6e96e5a.js";
-import "./c.7d2e85dd.js";
-import "./c.45f3bfa8.js";
+import "./c.c84471ef.js";
+import "./c.d861da54.js";
 let u = class extends t {
     constructor() {
         super(...arguments), this._state = "connecting_webserial"
     }
     render() {
         let t, r = !1;
         return "connecting_webserial" === this._state ? (t = this._renderProgress("Connecting"), r = !0) : "prepare_installation" === this._state ? (t = this._renderProgress("Preparing installation"), r = !0) : "installing" === this._state ? (t = void 0 === this._writeProgress ? this._renderProgress("Erasing") : this._renderProgress(e`
```

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.9e5eaea1.js` & `esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.3f59652f.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,60 +1,61 @@
 import {
     e as t,
     c as e,
-    I as o,
-    J as i,
+    J as o,
+    K as i,
     r as s,
     b as r,
     d as a,
     n,
     s as l,
     y as c,
     f as d,
-    K as p,
-    L as h,
-    N as m,
-    O as u,
+    L as p,
+    N as h,
+    O as m,
+    P as u,
     G as w,
-    l as _,
-    P as v,
-    D as g,
-    Q as y
-} from "./index-d3dd97b9.js";
+    H as _,
+    l as v,
+    Q as g,
+    D as y,
+    S as f
+} from "./index-bfcf9cd9.js";
 import {
-    g as f
-} from "./c.7d2e85dd.js";
-import "./c.e4466087.js";
+    g as b
+} from "./c.c84471ef.js";
+import "./c.4971d925.js";
 import {
-    o as b,
-    c as $
-} from "./c.bff582f5.js";
+    o as $,
+    c as P
+} from "./c.17838855.js";
 import {
-    m as P,
-    s as S,
-    b as k
-} from "./c.e683a7a9.js";
+    m as S,
+    s as k,
+    b as x
+} from "./c.884f2894.js";
 import {
-    o as x
-} from "./c.45f3bfa8.js";
-class C {
+    o as C
+} from "./c.d861da54.js";
+class E {
     constructor(t) {
         this.Y = t
     }
     disconnect() {
         this.Y = void 0
     }
     reconnect(t) {
         this.Y = t
     }
     deref() {
         return this.Y
     }
 }
-class E {
+class H {
     constructor() {
         this.Z = void 0, this.q = void 0
     }
     get() {
         return this.Z
     }
     pause() {
@@ -62,33 +63,33 @@
         null !== (t = this.Z) && void 0 !== t || (this.Z = new Promise((t => this.q = t)))
     }
     resume() {
         var t;
         null === (t = this.q) || void 0 === t || t.call(this), this.Z = this.q = void 0
     }
 }
-const H = t => !i(t) && "function" == typeof t.then;
-const W = t(class extends e {
+const W = t => !i(t) && "function" == typeof t.then;
+const j = t(class extends e {
         constructor() {
-            super(...arguments), this._$Cwt = 1073741823, this._$Cyt = [], this._$CK = new C(this), this._$CX = new E
+            super(...arguments), this._$Cwt = 1073741823, this._$Cyt = [], this._$CK = new E(this), this._$CX = new H
         }
         render(...t) {
             var e;
-            return null !== (e = t.find((t => !H(t)))) && void 0 !== e ? e : o
+            return null !== (e = t.find((t => !W(t)))) && void 0 !== e ? e : o
         }
         update(t, e) {
             const i = this._$Cyt;
             let s = i.length;
             this._$Cyt = e;
             const r = this._$CK,
                 a = this._$CX;
             this.isConnected || this.disconnected();
             for (let t = 0; t < e.length && !(t > this._$Cwt); t++) {
                 const o = e[t];
-                if (!H(o)) return this._$Cwt = t, o;
+                if (!W(o)) return this._$Cwt = t, o;
                 t < s && o === i[t] || (this._$Cwt = 1073741823, s = 0, Promise.resolve(o).then((async t => {
                     for (; a.get();) await a.get();
                     const e = r.deref();
                     if (void 0 !== e) {
                         const i = e._$Cyt.indexOf(o);
                         i > -1 && i < e._$Cwt && (e._$Cwt = i, e.setValue(t))
                     }
@@ -99,52 +100,52 @@
         disconnected() {
             this._$CK.disconnect(), this._$CX.pause()
         }
         reconnected() {
             this._$CK.reconnect(this), this._$CX.resume()
         }
     }),
-    j = (t, e) => {
-        import("./c.e1319253.js");
+    A = (t, e) => {
+        import("./c.6951bded.js");
         const o = document.createElement("esphome-compile-dialog");
         o.configuration = t, o.downloadFactoryFirmware = e, document.body.append(o)
     },
     I = async (t, e) => {
-        import("./c.98e8e8d2.js");
+        import("./c.11743138.js");
         let o = t.port;
         if (o) await o.close();
         else try {
             o = await navigator.serial.requestPort()
         } catch (o) {
-            return void("NotFoundError" === o.name ? b((() => I(t, e))) : alert(`Unable to connect: ${o.message}`))
+            return void("NotFoundError" === o.name ? $((() => I(t, e))) : alert(`Unable to connect: ${o.message}`))
         }
-        const i = $(o);
+        const i = P(o);
         e && e();
         const s = document.createElement("esphome-install-web-dialog");
         s.params = t, s.esploader = i, document.body.append(s)
-    }, A = {
+    }, T = {
         info: p,
         warning: h,
         error: m,
         success: u
     };
-let T = class extends l {
+let D = class extends l {
     constructor() {
         super(...arguments), this.title = "", this.alertType = "info", this.rtl = !1
     }
     render() {
         return c`
       <div
         class="issue-type ${d({rtl:this.rtl,[this.alertType]:!0})}"
         role="alert"
       >
         <div class="icon ${this.title?"":"no-title"}">
           <slot name="icon">
             <esphome-svg-icon
-              .path=${A[this.alertType]}
+              .path=${T[this.alertType]}
             ></esphome-svg-icon>
           </slot>
         </div>
         <div class="content">
           <div class="main-content">
             ${this.title?c`<div class="title">${this.title}</div>`:""}
             <slot></slot>
@@ -153,15 +154,15 @@
             <slot name="action"> </slot>
           </div>
         </div>
       </div>
     `
     }
 };
-T.styles = s`
+D.styles = s`
     .issue-type {
       position: relative;
       padding: 8px;
       display: flex;
       padding-left: var(--esphome-alert-padding-left, 8px);
     }
     .issue-type.rtl {
@@ -241,20 +242,20 @@
 
     .issue-type.success > .icon {
       color: var(--alert-success-color);
     }
     .issue-type.success::after {
       background-color: var(--alert-success-color);
     }
-  `, r([a()], T.prototype, "title", void 0), r([a({
+  `, r([a()], D.prototype, "title", void 0), r([a({
     attribute: "alert-type"
-})], T.prototype, "alertType", void 0), r([a({
+})], D.prototype, "alertType", void 0), r([a({
     type: Boolean
-})], T.prototype, "rtl", void 0), T = r([n("esphome-alert")], T);
-let D = class extends l {
+})], D.prototype, "rtl", void 0), D = r([n("esphome-alert")], D);
+let B = class extends l {
     constructor() {
         super(...arguments), this._ethernet = !1, this._isPico = !1, this._state = "pick_option"
     }
     get _platformSupportsWebSerial() {
         return !this._isPico
     }
     render() {
@@ -264,51 +265,51 @@
           twoline
           hasMeta
           .port=${"OTA"}
           @click=${this._handleLegacyOption}
         >
           <span>${this._ethernet?"Via the network":"Wirelessly"}</span>
           <span slot="secondary">Requires the device to be online</span>
-          ${P}
+          ${S}
         </mwc-list-item>
 
         ${this._error?c`<div class="error">${this._error}</div>`:""}
 
         <mwc-list-item
           twoline
           hasMeta
           ?disabled=${!this._platformSupportsWebSerial}
           @click=${this._handleBrowserInstall}
         >
           <span>Plug into this computer</span>
           <span slot="secondary">
             ${this._platformSupportsWebSerial?"For devices connected via USB to this computer":"Installing this via the web is not supported yet for this device"}
           </span>
-          ${P}
+          ${S}
         </mwc-list-item>
 
         <mwc-list-item twoline hasMeta @click=${this._handleServerInstall}>
           <span>Plug into the computer running ESPHome Dashboard</span>
           <span slot="secondary">
             ${"For devices connected via USB to the server"+(this._isPico?" and running ESPHome":"")}
           </span>
-          ${P}
+          ${S}
         </mwc-list-item>
 
         <mwc-list-item
           twoline
           hasMeta
           @click=${()=>{this._state=this._isPico?"download_instructions":"pick_download_type"}}
         >
           <span>Manual download</span>
           <span slot="secondary">
             Install it yourself
             ${this._isPico?"by copying it to the Pico USB drive":"using ESPHome Web or other tools"}
           </span>
-          ${P}
+          ${S}
         </mwc-list-item>
 
         <mwc-button
           no-attention
           slot="secondaryAction"
           dialogAction="close"
           label="Cancel"
@@ -331,15 +332,15 @@
                           twoline
                           hasMeta
                           .port=${t.port}
                           @click=${this._handleLegacyOption}
                         >
                           <span>${t.desc}</span>
                           <span slot="secondary">${t.port}</span>
-                          ${P}
+                          ${S}
                         </mwc-list-item>
                       `))}
                   `}
               <mwc-button
                 no-attention
                 slot="primaryAction"
                 label="Back"
@@ -353,26 +354,26 @@
           dialogAction="close"
           @click=${this._handleWebDownload}
         >
           <span>Modern format</span>
           <span slot="secondary">
             For use with ESPHome Web and other tools.
           </span>
-          ${P}
+          ${S}
         </mwc-list-item>
 
         <mwc-list-item
           twoline
           hasMeta
           dialogAction="close"
           @click=${this._handleManualDownload}
         >
           <span>Legacy format</span>
           <span slot="secondary">For use with ESPHome Flasher.</span>
-          ${P}
+          ${S}
         </mwc-list-item>
 
         ${this._platformSupportsWebSerial?c`
               <a
                 href="https://web.esphome.io"
                 target="_blank"
                 rel="noopener noreferrer"
@@ -385,15 +386,15 @@
           slot="primaryAction"
           label="Back"
           @click=${()=>{this._state="pick_option"}}
         ></mwc-button>
       `;
         else if ("download_instructions" === this._state) {
             let o;
-            const i = W(this._compileConfiguration, c`<a download disabled href="#">Download project</a>
+            const i = j(this._compileConfiguration, c`<a download disabled href="#">Download project</a>
           preparing&nbsp;download…
           <mwc-circular-progress
             density="-8"
             indeterminate
           ></mwc-circular-progress>`);
             this._isPico ? (t = "Install ESPHome via the USB drive", o = c`
           <div>
@@ -493,35 +494,35 @@
               dialogAction="ok"
               label="Close"
             ></mwc-button>
           `:""}
     `
     }
     firstUpdated(t) {
-        super.firstUpdated(t), this._updateSerialPorts(), v(this.configuration).then((t => {
+        super.firstUpdated(t), this._updateSerialPorts(), g(this.configuration).then((t => {
             this._ethernet = t.loaded_integrations.includes("ethernet"), this._isPico = "RP2040" === t.esp_platform
         }))
     }
     async _updateSerialPorts() {
-        this._ports = await f()
+        this._ports = await b()
     }
     willUpdate(t) {
-        super.willUpdate(t), t.has("_state") && "download_instructions" === this._state && !this._compileConfiguration && (this._abortCompilation = new AbortController, this._compileConfiguration = g(this.configuration).then((() => c`
+        super.willUpdate(t), t.has("_state") && "download_instructions" === this._state && !this._compileConfiguration && (this._abortCompilation = new AbortController, this._compileConfiguration = y(this.configuration).then((() => c`
             <a
               download
-              href="${y(this.configuration,!this._isPico)}"
+              href="${f(this.configuration,!this._isPico)}"
               >Download project</a
             >
           `), (() => c`
             <a download disabled href="#">Download project</a>
             <span class="prepare-error">preparation failed:</span>
             <button
               class="link"
               dialogAction="close"
-              @click=${()=>{j(this.configuration,!this._isPico)}}
+              @click=${()=>{A(this.configuration,!this._isPico)}}
             >
               see what went wrong
             </button>
           `)).finally((() => {
             this._abortCompilation = void 0
         })))
     }
@@ -539,43 +540,40 @@
     _storeDialogWidth() {
         this.style.setProperty("--mdc-dialog-min-width", `${this.shadowRoot.querySelector("mwc-list-item").clientWidth+4}px`)
     }
     _handleServerInstall() {
         this._storeDialogWidth(), this._state = "pick_server_port"
     }
     _handleManualDownload() {
-        j(this.configuration, !1)
+        A(this.configuration, !1)
     }
     _handleWebDownload() {
-        j(this.configuration, !0)
+        A(this.configuration, !0)
     }
     _handleLegacyOption(t) {
-        x(this.configuration, t.currentTarget.port), this._close()
+        C(this.configuration, t.currentTarget.port), this._close()
     }
     _handleBrowserInstall() {
-        if (!S || !k) return this._storeDialogWidth(), void(this._state = "download_instructions");
+        if (!k || !x) return this._storeDialogWidth(), void(this._state = "download_instructions");
         I({
             configuration: this.configuration
         }, (() => this._close()))
     }
     _close() {
         this.shadowRoot.querySelector("mwc-dialog").close()
     }
     async _handleClose() {
         var t;
         null === (t = this._abortCompilation) || void 0 === t || t.abort(), this._updateSerialInterval && (clearTimeout(this._updateSerialInterval), this._updateSerialInterval = void 0), this.parentNode.removeChild(this)
     }
 };
-D.styles = [w, s`
+B.styles = [w, _, s`
       mwc-list-item {
         margin: 0 -20px;
       }
-      svg {
-        fill: currentColor;
-      }
       .center {
         text-align: center;
       }
       mwc-circular-progress {
         margin-bottom: 16px;
       }
       li mwc-circular-progress {
@@ -629,14 +627,14 @@
       }
       esphome-alert {
         color: black;
         margin: 0 -24px;
         display: block;
         --esphome-alert-padding-left: 20px;
       }
-    `], r([a()], D.prototype, "configuration", void 0), r([_()], D.prototype, "_ethernet", void 0), r([_()], D.prototype, "_isPico", void 0), r([_()], D.prototype, "_ports", void 0), r([_()], D.prototype, "_state", void 0), r([_()], D.prototype, "_error", void 0), D = r([n("esphome-install-choose-dialog")], D);
-var B = Object.freeze({
+    `], r([a()], B.prototype, "configuration", void 0), r([v()], B.prototype, "_ethernet", void 0), r([v()], B.prototype, "_isPico", void 0), r([v()], B.prototype, "_ports", void 0), r([v()], B.prototype, "_state", void 0), r([v()], B.prototype, "_error", void 0), B = r([n("esphome-install-choose-dialog")], B);
+var M = Object.freeze({
     __proto__: null
 });
 export {
-    I as a, B as i, j as o
+    I as a, M as i, A as o
 };
```

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.a613b168.js` & `esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.670cd819.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -2,17 +2,17 @@
     b as t,
     l as s,
     n as e,
     s as i,
     y as o,
     f as a,
     r
-} from "./index-d3dd97b9.js";
-import "./c.e4466087.js";
-let l = class extends i {
+} from "./index-bfcf9cd9.js";
+import "./c.4971d925.js";
+let m = class extends i {
     async showDialog(t, s) {
         this._params = t, this._resolve = s
     }
     render() {
         return this._params ? o`
       <mwc-dialog
         .heading=${this._params.title||""}
@@ -36,14 +36,18 @@
     ` : o``
     }
     _handleClose(t) {
         this._resolve("confirm" === t.detail.action), this.parentNode.removeChild(this)
     }
     static get styles() {
         return r`
+      mwc-button {
+        --mdc-theme-primary: var(--primary-text-color);
+      }
+
       .destructive {
         --mdc-theme-primary: var(--alert-error-color);
       }
     `
     }
 };
-t([s()], l.prototype, "_params", void 0), t([s()], l.prototype, "_resolve", void 0), l = t([e("esphome-confirmation-dialog")], l);
+t([s()], m.prototype, "_params", void 0), t([s()], m.prototype, "_resolve", void 0), m = t([e("esphome-confirmation-dialog")], m);
```

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.b9286028.js` & `esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.9f55698d.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -4,17 +4,17 @@
     b as t,
     d as e,
     l as s,
     n as a,
     s as n,
     y as c,
     C as d,
-    H as l
-} from "./index-d3dd97b9.js";
-import "./c.e4466087.js";
+    I as l
+} from "./index-bfcf9cd9.js";
+import "./c.4971d925.js";
 import {
     c as r
 } from "./c.440fff61.js";
 let p = class extends n {
     constructor() {
         super(...arguments), this._showCopied = !1
     }
```

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.bff582f5.js` & `esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.17838855.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,19 +1,19 @@
 import {
     b as t,
     d as e,
     p as i,
     s as r,
     y as a,
     f as s,
-    S as n,
+    T as n,
     u as o,
     r as h,
     n as _
-} from "./index-d3dd97b9.js";
+} from "./index-bfcf9cd9.js";
 class l extends r {
     constructor() {
         super(...arguments), this.indeterminate = !1, this.progress = 0, this.density = 0, this.closed = !1
     }
     open() {
         this.closed = !1
     }
@@ -129,15 +129,15 @@
     type: String,
     attribute: "aria-label"
 })], l.prototype, "ariaLabel", void 0);
 const c = h`.mdc-circular-progress__determinate-circle,.mdc-circular-progress__indeterminate-circle-graphic{stroke:#6200ee;stroke:var(--mdc-theme-primary, #6200ee)}.mdc-circular-progress__determinate-track{stroke:transparent}@keyframes mdc-circular-progress-container-rotate{to{transform:rotate(360deg)}}@keyframes mdc-circular-progress-spinner-layer-rotate{12.5%{transform:rotate(135deg)}25%{transform:rotate(270deg)}37.5%{transform:rotate(405deg)}50%{transform:rotate(540deg)}62.5%{transform:rotate(675deg)}75%{transform:rotate(810deg)}87.5%{transform:rotate(945deg)}100%{transform:rotate(1080deg)}}@keyframes mdc-circular-progress-color-1-fade-in-out{from{opacity:.99}25%{opacity:.99}26%{opacity:0}89%{opacity:0}90%{opacity:.99}to{opacity:.99}}@keyframes mdc-circular-progress-color-2-fade-in-out{from{opacity:0}15%{opacity:0}25%{opacity:.99}50%{opacity:.99}51%{opacity:0}to{opacity:0}}@keyframes mdc-circular-progress-color-3-fade-in-out{from{opacity:0}40%{opacity:0}50%{opacity:.99}75%{opacity:.99}76%{opacity:0}to{opacity:0}}@keyframes mdc-circular-progress-color-4-fade-in-out{from{opacity:0}65%{opacity:0}75%{opacity:.99}90%{opacity:.99}to{opacity:0}}@keyframes mdc-circular-progress-left-spin{from{transform:rotate(265deg)}50%{transform:rotate(130deg)}to{transform:rotate(265deg)}}@keyframes mdc-circular-progress-right-spin{from{transform:rotate(-265deg)}50%{transform:rotate(-130deg)}to{transform:rotate(-265deg)}}.mdc-circular-progress{display:inline-flex;position:relative;direction:ltr;line-height:0;transition:opacity 250ms 0ms cubic-bezier(0.4, 0, 0.6, 1)}.mdc-circular-progress__determinate-container,.mdc-circular-progress__indeterminate-circle-graphic,.mdc-circular-progress__indeterminate-container,.mdc-circular-progress__spinner-layer{position:absolute;width:100%;height:100%}.mdc-circular-progress__determinate-container{transform:rotate(-90deg)}.mdc-circular-progress__indeterminate-container{font-size:0;letter-spacing:0;white-space:nowrap;opacity:0}.mdc-circular-progress__determinate-circle-graphic,.mdc-circular-progress__indeterminate-circle-graphic{fill:transparent}.mdc-circular-progress__determinate-circle{transition:stroke-dashoffset 500ms 0ms cubic-bezier(0, 0, 0.2, 1)}.mdc-circular-progress__gap-patch{position:absolute;top:0;left:47.5%;box-sizing:border-box;width:5%;height:100%;overflow:hidden}.mdc-circular-progress__gap-patch .mdc-circular-progress__indeterminate-circle-graphic{left:-900%;width:2000%;transform:rotate(180deg)}.mdc-circular-progress__circle-clipper{display:inline-flex;position:relative;width:50%;height:100%;overflow:hidden}.mdc-circular-progress__circle-clipper .mdc-circular-progress__indeterminate-circle-graphic{width:200%}.mdc-circular-progress__circle-right .mdc-circular-progress__indeterminate-circle-graphic{left:-100%}.mdc-circular-progress--indeterminate .mdc-circular-progress__determinate-container{opacity:0}.mdc-circular-progress--indeterminate .mdc-circular-progress__indeterminate-container{opacity:1}.mdc-circular-progress--indeterminate .mdc-circular-progress__indeterminate-container{animation:mdc-circular-progress-container-rotate 1568.2352941176ms linear infinite}.mdc-circular-progress--indeterminate .mdc-circular-progress__spinner-layer{animation:mdc-circular-progress-spinner-layer-rotate 5332ms cubic-bezier(0.4, 0, 0.2, 1) infinite both}.mdc-circular-progress--indeterminate .mdc-circular-progress__color-1{animation:mdc-circular-progress-spinner-layer-rotate 5332ms cubic-bezier(0.4, 0, 0.2, 1) infinite both,mdc-circular-progress-color-1-fade-in-out 5332ms cubic-bezier(0.4, 0, 0.2, 1) infinite both}.mdc-circular-progress--indeterminate .mdc-circular-progress__color-2{animation:mdc-circular-progress-spinner-layer-rotate 5332ms cubic-bezier(0.4, 0, 0.2, 1) infinite both,mdc-circular-progress-color-2-fade-in-out 5332ms cubic-bezier(0.4, 0, 0.2, 1) infinite both}.mdc-circular-progress--indeterminate .mdc-circular-progress__color-3{animation:mdc-circular-progress-spinner-layer-rotate 5332ms cubic-bezier(0.4, 0, 0.2, 1) infinite both,mdc-circular-progress-color-3-fade-in-out 5332ms cubic-bezier(0.4, 0, 0.2, 1) infinite both}.mdc-circular-progress--indeterminate .mdc-circular-progress__color-4{animation:mdc-circular-progress-spinner-layer-rotate 5332ms cubic-bezier(0.4, 0, 0.2, 1) infinite both,mdc-circular-progress-color-4-fade-in-out 5332ms cubic-bezier(0.4, 0, 0.2, 1) infinite both}.mdc-circular-progress--indeterminate .mdc-circular-progress__circle-left .mdc-circular-progress__indeterminate-circle-graphic{animation:mdc-circular-progress-left-spin 1333ms cubic-bezier(0.4, 0, 0.2, 1) infinite both}.mdc-circular-progress--indeterminate .mdc-circular-progress__circle-right .mdc-circular-progress__indeterminate-circle-graphic{animation:mdc-circular-progress-right-spin 1333ms cubic-bezier(0.4, 0, 0.2, 1) infinite both}.mdc-circular-progress--closed{opacity:0}:host{display:inline-flex}.mdc-circular-progress__determinate-track{stroke:transparent;stroke:var(--mdc-circular-progress-track-color, transparent)}`;
 let d = class extends l {};
 d.styles = [c], d = t([_("mwc-circular-progress")], d);
 const f = async t => {
-    import("./c.6eebcb7a.js");
+    import("./c.4c0eda7e.js");
     const e = document.createElement("esphome-no-port-picked-dialog");
     return e.doTryAgain = t, document.body.append(e), !0
 };
 class u extends Error {}
 
 function p(t) {
     let e = t.length;
```

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.c0a69417.js` & `esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.c0a69417.js`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.c2d1f4be.js` & `esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.3bbbdf4b.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -24,68 +24,69 @@
     j as y,
     z as w,
     A as $,
     C as S,
     D as C,
     E as R,
     F as E,
-    G as P
-} from "./index-d3dd97b9.js";
-import "./c.e4466087.js";
+    G as P,
+    H as z
+} from "./index-bfcf9cd9.js";
+import "./c.4971d925.js";
 import {
-    F as z
-} from "./c.834bbab0.js";
+    F as A
+} from "./c.1107b6f0.js";
 import {
-    o as A,
-    c as B
-} from "./c.bff582f5.js";
+    o as B,
+    c as T
+} from "./c.17838855.js";
 import {
-    s as T,
+    s as H,
     a as D,
     m as F,
-    b as H,
-    c as I
-} from "./c.e683a7a9.js";
+    b as I,
+    c as L
+} from "./c.884f2894.js";
 import {
-    g as L,
-    f as O,
-    r as N
-} from "./c.3b4072f5.js";
+    g as O,
+    f as N,
+    r as j
+} from "./c.cd26dc5d.js";
 import {
-    S as j,
-    a as M,
-    c as U,
-    s as W
-} from "./c.dde41422.js";
+    S as M,
+    a as U,
+    c as W,
+    s as q
+} from "./c.2d34b51a.js";
 import {
-    c as q
+    c as K
 } from "./c.440fff61.js";
 import {
-    s as K
+    s as Y
 } from "./c.a6e96e5a.js";
-const Y = Symbol("selection controller");
-class X {
+const X = Symbol("selection controller");
+class G {
     constructor() {
         this.selected = null, this.ordered = null, this.set = new Set
     }
 }
-class G {
+class V {
     constructor(e) {
         this.sets = {}, this.focusedSet = null, this.mouseIsDown = !1, this.updating = !1, e.addEventListener("keydown", (e => {
             this.keyDownHandler(e)
         })), e.addEventListener("mousedown", (() => {
             this.mousedownHandler()
         })), e.addEventListener("mouseup", (() => {
             this.mouseupHandler()
         }))
     }
     static getController(e) {
         const t = !("global" in e) || "global" in e && e.global ? document : e.getRootNode();
-        let c = t[Y];
-        return void 0 === c && (c = new G(t), t[Y] = c), c
+        let c = t[X];
+        return void 0 === c && (c = new V(t), t[X] = c), c
     }
     keyDownHandler(e) {
         const t = e.target;
         "checked" in t && this.has(t) && ("ArrowRight" == e.key || "ArrowDown" == e.key ? this.selectNext(t) : "ArrowLeft" != e.key && "ArrowUp" != e.key || this.selectPrevious(t))
     }
     mousedownHandler() {
         this.mouseIsDown = !0
@@ -124,15 +125,15 @@
         return !1
     }
     getOrdered(e) {
         const t = this.getSet(e.name);
         return t.ordered || (t.ordered = Array.from(t.set), t.ordered.sort(((e, t) => e.compareDocumentPosition(t) == Node.DOCUMENT_POSITION_PRECEDING ? 1 : 0))), t.ordered
     }
     getSet(e) {
-        return this.sets[e] || (this.sets[e] = new X), this.sets[e]
+        return this.sets[e] || (this.sets[e] = new G), this.sets[e]
     }
     register(e) {
         const t = e.name || e.getAttribute("name") || "",
             c = this.getSet(t);
         c.set.add(e), c.ordered = null
     }
     unregister(e) {
@@ -151,34 +152,34 @@
             for (const e of t.set) {
                 if (void 0 === e.formElementTabIndex) break;
                 e.formElementTabIndex = e.checked ? 0 : -1
             }
         this.updating = !1
     }
 }
-var V = {
+var J = {
         NATIVE_CONTROL_SELECTOR: ".mdc-radio__native-control"
     },
-    J = {
+    Q = {
         DISABLED: "mdc-radio--disabled",
         ROOT: "mdc-radio"
     },
-    Q = function(c) {
+    Z = function(c) {
         function o(e) {
             return c.call(this, t(t({}, o.defaultAdapter), e)) || this
         }
         return e(o, c), Object.defineProperty(o, "cssClasses", {
             get: function() {
-                return J
+                return Q
             },
             enumerable: !1,
             configurable: !0
         }), Object.defineProperty(o, "strings", {
             get: function() {
-                return V
+                return J
             },
             enumerable: !1,
             configurable: !0
         }), Object.defineProperty(o, "defaultAdapter", {
             get: function() {
                 return {
                     addClass: function() {},
@@ -189,17 +190,17 @@
             enumerable: !1,
             configurable: !0
         }), o.prototype.setDisabled = function(e) {
             var t = o.cssClasses.DISABLED;
             this.adapter.setNativeControlDisabled(e), e ? this.adapter.addClass(t) : this.adapter.removeClass(t)
         }, o
     }(c);
-class Z extends z {
+class ee extends A {
     constructor() {
-        super(...arguments), this._checked = !1, this.useStateLayerCustomProperties = !1, this.global = !1, this.disabled = !1, this.value = "on", this.name = "", this.reducedTouchTarget = !1, this.mdcFoundationClass = Q, this.formElementTabIndex = 0, this.focused = !1, this.shouldRenderRipple = !1, this.rippleElement = null, this.rippleHandlers = new m((() => (this.shouldRenderRipple = !0, this.ripple.then((e => {
+        super(...arguments), this._checked = !1, this.useStateLayerCustomProperties = !1, this.global = !1, this.disabled = !1, this.value = "on", this.name = "", this.reducedTouchTarget = !1, this.mdcFoundationClass = Z, this.formElementTabIndex = 0, this.focused = !1, this.shouldRenderRipple = !1, this.rippleElement = null, this.rippleHandlers = new m((() => (this.shouldRenderRipple = !0, this.ripple.then((e => {
             this.rippleElement = e
         })), this.ripple)))
     }
     get checked() {
         return this._checked
     }
     set checked(e) {
@@ -219,15 +220,15 @@
         .disabled="${this.disabled}"></mwc-ripple>` : ""
     }
     get isRippleActive() {
         var e;
         return (null === (e = this.rippleElement) || void 0 === e ? void 0 : e.isActive) || !1
     }
     connectedCallback() {
-        super.connectedCallback(), this._selectionController = G.getController(this), this._selectionController.register(this), this._selectionController.update(this)
+        super.connectedCallback(), this._selectionController = V.getController(this), this._selectionController.register(this), this._selectionController.update(this)
     }
     disconnectedCallback() {
         this._selectionController.unregister(this), this._selectionController = void 0
     }
     focus() {
         this.formElement.focus()
     }
@@ -306,65 +307,65 @@
     handleRippleFocus() {
         this.rippleHandlers.startFocus()
     }
     changeHandler() {
         this.checked = this.formElement.checked
     }
 }
-o([i(".mdc-radio")], Z.prototype, "mdcRoot", void 0), o([i("input")], Z.prototype, "formElement", void 0), o([r()], Z.prototype, "useStateLayerCustomProperties", void 0), o([a({
+o([i(".mdc-radio")], ee.prototype, "mdcRoot", void 0), o([i("input")], ee.prototype, "formElement", void 0), o([r()], ee.prototype, "useStateLayerCustomProperties", void 0), o([a({
     type: Boolean
-})], Z.prototype, "global", void 0), o([a({
+})], ee.prototype, "global", void 0), o([a({
     type: Boolean,
     reflect: !0
-})], Z.prototype, "checked", null), o([a({
+})], ee.prototype, "checked", null), o([a({
     type: Boolean
 }), d((function(e) {
     this.mdcFoundation.setDisabled(e)
-}))], Z.prototype, "disabled", void 0), o([a({
+}))], ee.prototype, "disabled", void 0), o([a({
     type: String
 }), d((function(e) {
     this._handleUpdatedValue(e)
-}))], Z.prototype, "value", void 0), o([a({
+}))], ee.prototype, "value", void 0), o([a({
     type: String
-})], Z.prototype, "name", void 0), o([a({
+})], ee.prototype, "name", void 0), o([a({
     type: Boolean
-})], Z.prototype, "reducedTouchTarget", void 0), o([a({
+})], ee.prototype, "reducedTouchTarget", void 0), o([a({
     type: Number
-})], Z.prototype, "formElementTabIndex", void 0), o([r()], Z.prototype, "focused", void 0), o([r()], Z.prototype, "shouldRenderRipple", void 0), o([n("mwc-ripple")], Z.prototype, "ripple", void 0), o([s, a({
+})], ee.prototype, "formElementTabIndex", void 0), o([r()], ee.prototype, "focused", void 0), o([r()], ee.prototype, "shouldRenderRipple", void 0), o([n("mwc-ripple")], ee.prototype, "ripple", void 0), o([s, a({
     attribute: "aria-label"
-})], Z.prototype, "ariaLabel", void 0), o([s, a({
+})], ee.prototype, "ariaLabel", void 0), o([s, a({
     attribute: "aria-labelledby"
-})], Z.prototype, "ariaLabelledBy", void 0), o([l({
+})], ee.prototype, "ariaLabelledBy", void 0), o([l({
     passive: !0
-})], Z.prototype, "handleRippleTouchStart", null);
-const ee = k`.mdc-touch-target-wrapper{display:inline}.mdc-radio{padding:calc((40px - 20px) / 2)}.mdc-radio .mdc-radio__native-control:enabled:not(:checked)+.mdc-radio__background .mdc-radio__outer-circle{border-color:rgba(0, 0, 0, 0.54)}.mdc-radio .mdc-radio__native-control:enabled:checked+.mdc-radio__background .mdc-radio__outer-circle{border-color:#018786;border-color:var(--mdc-theme-secondary, #018786)}.mdc-radio .mdc-radio__native-control:enabled+.mdc-radio__background .mdc-radio__inner-circle{border-color:#018786;border-color:var(--mdc-theme-secondary, #018786)}.mdc-radio [aria-disabled=true] .mdc-radio__native-control:not(:checked)+.mdc-radio__background .mdc-radio__outer-circle,.mdc-radio .mdc-radio__native-control:disabled:not(:checked)+.mdc-radio__background .mdc-radio__outer-circle{border-color:rgba(0, 0, 0, 0.38)}.mdc-radio [aria-disabled=true] .mdc-radio__native-control:checked+.mdc-radio__background .mdc-radio__outer-circle,.mdc-radio .mdc-radio__native-control:disabled:checked+.mdc-radio__background .mdc-radio__outer-circle{border-color:rgba(0, 0, 0, 0.38)}.mdc-radio [aria-disabled=true] .mdc-radio__native-control+.mdc-radio__background .mdc-radio__inner-circle,.mdc-radio .mdc-radio__native-control:disabled+.mdc-radio__background .mdc-radio__inner-circle{border-color:rgba(0, 0, 0, 0.38)}.mdc-radio .mdc-radio__background::before{background-color:#018786;background-color:var(--mdc-theme-secondary, #018786)}.mdc-radio .mdc-radio__background::before{top:calc(-1 * (40px - 20px) / 2);left:calc(-1 * (40px - 20px) / 2);width:40px;height:40px}.mdc-radio .mdc-radio__native-control{top:calc((40px - 40px) / 2);right:calc((40px - 40px) / 2);left:calc((40px - 40px) / 2);width:40px;height:40px}@media screen and (forced-colors: active),(-ms-high-contrast: active){.mdc-radio.mdc-radio--disabled [aria-disabled=true] .mdc-radio__native-control:not(:checked)+.mdc-radio__background .mdc-radio__outer-circle,.mdc-radio.mdc-radio--disabled .mdc-radio__native-control:disabled:not(:checked)+.mdc-radio__background .mdc-radio__outer-circle{border-color:GrayText}.mdc-radio.mdc-radio--disabled [aria-disabled=true] .mdc-radio__native-control:checked+.mdc-radio__background .mdc-radio__outer-circle,.mdc-radio.mdc-radio--disabled .mdc-radio__native-control:disabled:checked+.mdc-radio__background .mdc-radio__outer-circle{border-color:GrayText}.mdc-radio.mdc-radio--disabled [aria-disabled=true] .mdc-radio__native-control+.mdc-radio__background .mdc-radio__inner-circle,.mdc-radio.mdc-radio--disabled .mdc-radio__native-control:disabled+.mdc-radio__background .mdc-radio__inner-circle{border-color:GrayText}}.mdc-radio{display:inline-block;position:relative;flex:0 0 auto;box-sizing:content-box;width:20px;height:20px;cursor:pointer;will-change:opacity,transform,border-color,color}.mdc-radio__background{display:inline-block;position:relative;box-sizing:border-box;width:20px;height:20px}.mdc-radio__background::before{position:absolute;transform:scale(0, 0);border-radius:50%;opacity:0;pointer-events:none;content:"";transition:opacity 120ms 0ms cubic-bezier(0.4, 0, 0.6, 1),transform 120ms 0ms cubic-bezier(0.4, 0, 0.6, 1)}.mdc-radio__outer-circle{position:absolute;top:0;left:0;box-sizing:border-box;width:100%;height:100%;border-width:2px;border-style:solid;border-radius:50%;transition:border-color 120ms 0ms cubic-bezier(0.4, 0, 0.6, 1)}.mdc-radio__inner-circle{position:absolute;top:0;left:0;box-sizing:border-box;width:100%;height:100%;transform:scale(0, 0);border-width:10px;border-style:solid;border-radius:50%;transition:transform 120ms 0ms cubic-bezier(0.4, 0, 0.6, 1),border-color 120ms 0ms cubic-bezier(0.4, 0, 0.6, 1)}.mdc-radio__native-control{position:absolute;margin:0;padding:0;opacity:0;cursor:inherit;z-index:1}.mdc-radio--touch{margin-top:4px;margin-bottom:4px;margin-right:4px;margin-left:4px}.mdc-radio--touch .mdc-radio__native-control{top:calc((40px - 48px) / 2);right:calc((40px - 48px) / 2);left:calc((40px - 48px) / 2);width:48px;height:48px}.mdc-radio.mdc-ripple-upgraded--background-focused .mdc-radio__focus-ring,.mdc-radio:not(.mdc-ripple-upgraded):focus .mdc-radio__focus-ring{pointer-events:none;border:2px solid transparent;border-radius:6px;box-sizing:content-box;position:absolute;top:50%;left:50%;transform:translate(-50%, -50%);height:100%;width:100%}@media screen and (forced-colors: active){.mdc-radio.mdc-ripple-upgraded--background-focused .mdc-radio__focus-ring,.mdc-radio:not(.mdc-ripple-upgraded):focus .mdc-radio__focus-ring{border-color:CanvasText}}.mdc-radio.mdc-ripple-upgraded--background-focused .mdc-radio__focus-ring::after,.mdc-radio:not(.mdc-ripple-upgraded):focus .mdc-radio__focus-ring::after{content:"";border:2px solid transparent;border-radius:8px;display:block;position:absolute;top:50%;left:50%;transform:translate(-50%, -50%);height:calc(100% + 4px);width:calc(100% + 4px)}@media screen and (forced-colors: active){.mdc-radio.mdc-ripple-upgraded--background-focused .mdc-radio__focus-ring::after,.mdc-radio:not(.mdc-ripple-upgraded):focus .mdc-radio__focus-ring::after{border-color:CanvasText}}.mdc-radio__native-control:checked+.mdc-radio__background,.mdc-radio__native-control:disabled+.mdc-radio__background{transition:opacity 120ms 0ms cubic-bezier(0, 0, 0.2, 1),transform 120ms 0ms cubic-bezier(0, 0, 0.2, 1)}.mdc-radio__native-control:checked+.mdc-radio__background .mdc-radio__outer-circle,.mdc-radio__native-control:disabled+.mdc-radio__background .mdc-radio__outer-circle{transition:border-color 120ms 0ms cubic-bezier(0, 0, 0.2, 1)}.mdc-radio__native-control:checked+.mdc-radio__background .mdc-radio__inner-circle,.mdc-radio__native-control:disabled+.mdc-radio__background .mdc-radio__inner-circle{transition:transform 120ms 0ms cubic-bezier(0, 0, 0.2, 1),border-color 120ms 0ms cubic-bezier(0, 0, 0.2, 1)}.mdc-radio--disabled{cursor:default;pointer-events:none}.mdc-radio__native-control:checked+.mdc-radio__background .mdc-radio__inner-circle{transform:scale(0.5);transition:transform 120ms 0ms cubic-bezier(0, 0, 0.2, 1),border-color 120ms 0ms cubic-bezier(0, 0, 0.2, 1)}.mdc-radio__native-control:disabled+.mdc-radio__background,[aria-disabled=true] .mdc-radio__native-control+.mdc-radio__background{cursor:default}.mdc-radio__native-control:focus+.mdc-radio__background::before{transform:scale(1);opacity:.12;transition:opacity 120ms 0ms cubic-bezier(0, 0, 0.2, 1),transform 120ms 0ms cubic-bezier(0, 0, 0.2, 1)}:host{display:inline-block;outline:none}.mdc-radio{vertical-align:bottom}.mdc-radio .mdc-radio__native-control:enabled:not(:checked)+.mdc-radio__background .mdc-radio__outer-circle{border-color:var(--mdc-radio-unchecked-color, rgba(0, 0, 0, 0.54))}.mdc-radio [aria-disabled=true] .mdc-radio__native-control:not(:checked)+.mdc-radio__background .mdc-radio__outer-circle,.mdc-radio .mdc-radio__native-control:disabled:not(:checked)+.mdc-radio__background .mdc-radio__outer-circle{border-color:var(--mdc-radio-disabled-color, rgba(0, 0, 0, 0.38))}.mdc-radio [aria-disabled=true] .mdc-radio__native-control:checked+.mdc-radio__background .mdc-radio__outer-circle,.mdc-radio .mdc-radio__native-control:disabled:checked+.mdc-radio__background .mdc-radio__outer-circle{border-color:var(--mdc-radio-disabled-color, rgba(0, 0, 0, 0.38))}.mdc-radio [aria-disabled=true] .mdc-radio__native-control+.mdc-radio__background .mdc-radio__inner-circle,.mdc-radio .mdc-radio__native-control:disabled+.mdc-radio__background .mdc-radio__inner-circle{border-color:var(--mdc-radio-disabled-color, rgba(0, 0, 0, 0.38))}`;
-let te = class extends Z {};
-te.styles = [ee], te = o([_("mwc-radio")], te);
-var ce = {
+})], ee.prototype, "handleRippleTouchStart", null);
+const te = k`.mdc-touch-target-wrapper{display:inline}.mdc-radio{padding:calc((40px - 20px) / 2)}.mdc-radio .mdc-radio__native-control:enabled:not(:checked)+.mdc-radio__background .mdc-radio__outer-circle{border-color:rgba(0, 0, 0, 0.54)}.mdc-radio .mdc-radio__native-control:enabled:checked+.mdc-radio__background .mdc-radio__outer-circle{border-color:#018786;border-color:var(--mdc-theme-secondary, #018786)}.mdc-radio .mdc-radio__native-control:enabled+.mdc-radio__background .mdc-radio__inner-circle{border-color:#018786;border-color:var(--mdc-theme-secondary, #018786)}.mdc-radio [aria-disabled=true] .mdc-radio__native-control:not(:checked)+.mdc-radio__background .mdc-radio__outer-circle,.mdc-radio .mdc-radio__native-control:disabled:not(:checked)+.mdc-radio__background .mdc-radio__outer-circle{border-color:rgba(0, 0, 0, 0.38)}.mdc-radio [aria-disabled=true] .mdc-radio__native-control:checked+.mdc-radio__background .mdc-radio__outer-circle,.mdc-radio .mdc-radio__native-control:disabled:checked+.mdc-radio__background .mdc-radio__outer-circle{border-color:rgba(0, 0, 0, 0.38)}.mdc-radio [aria-disabled=true] .mdc-radio__native-control+.mdc-radio__background .mdc-radio__inner-circle,.mdc-radio .mdc-radio__native-control:disabled+.mdc-radio__background .mdc-radio__inner-circle{border-color:rgba(0, 0, 0, 0.38)}.mdc-radio .mdc-radio__background::before{background-color:#018786;background-color:var(--mdc-theme-secondary, #018786)}.mdc-radio .mdc-radio__background::before{top:calc(-1 * (40px - 20px) / 2);left:calc(-1 * (40px - 20px) / 2);width:40px;height:40px}.mdc-radio .mdc-radio__native-control{top:calc((40px - 40px) / 2);right:calc((40px - 40px) / 2);left:calc((40px - 40px) / 2);width:40px;height:40px}@media screen and (forced-colors: active),(-ms-high-contrast: active){.mdc-radio.mdc-radio--disabled [aria-disabled=true] .mdc-radio__native-control:not(:checked)+.mdc-radio__background .mdc-radio__outer-circle,.mdc-radio.mdc-radio--disabled .mdc-radio__native-control:disabled:not(:checked)+.mdc-radio__background .mdc-radio__outer-circle{border-color:GrayText}.mdc-radio.mdc-radio--disabled [aria-disabled=true] .mdc-radio__native-control:checked+.mdc-radio__background .mdc-radio__outer-circle,.mdc-radio.mdc-radio--disabled .mdc-radio__native-control:disabled:checked+.mdc-radio__background .mdc-radio__outer-circle{border-color:GrayText}.mdc-radio.mdc-radio--disabled [aria-disabled=true] .mdc-radio__native-control+.mdc-radio__background .mdc-radio__inner-circle,.mdc-radio.mdc-radio--disabled .mdc-radio__native-control:disabled+.mdc-radio__background .mdc-radio__inner-circle{border-color:GrayText}}.mdc-radio{display:inline-block;position:relative;flex:0 0 auto;box-sizing:content-box;width:20px;height:20px;cursor:pointer;will-change:opacity,transform,border-color,color}.mdc-radio__background{display:inline-block;position:relative;box-sizing:border-box;width:20px;height:20px}.mdc-radio__background::before{position:absolute;transform:scale(0, 0);border-radius:50%;opacity:0;pointer-events:none;content:"";transition:opacity 120ms 0ms cubic-bezier(0.4, 0, 0.6, 1),transform 120ms 0ms cubic-bezier(0.4, 0, 0.6, 1)}.mdc-radio__outer-circle{position:absolute;top:0;left:0;box-sizing:border-box;width:100%;height:100%;border-width:2px;border-style:solid;border-radius:50%;transition:border-color 120ms 0ms cubic-bezier(0.4, 0, 0.6, 1)}.mdc-radio__inner-circle{position:absolute;top:0;left:0;box-sizing:border-box;width:100%;height:100%;transform:scale(0, 0);border-width:10px;border-style:solid;border-radius:50%;transition:transform 120ms 0ms cubic-bezier(0.4, 0, 0.6, 1),border-color 120ms 0ms cubic-bezier(0.4, 0, 0.6, 1)}.mdc-radio__native-control{position:absolute;margin:0;padding:0;opacity:0;cursor:inherit;z-index:1}.mdc-radio--touch{margin-top:4px;margin-bottom:4px;margin-right:4px;margin-left:4px}.mdc-radio--touch .mdc-radio__native-control{top:calc((40px - 48px) / 2);right:calc((40px - 48px) / 2);left:calc((40px - 48px) / 2);width:48px;height:48px}.mdc-radio.mdc-ripple-upgraded--background-focused .mdc-radio__focus-ring,.mdc-radio:not(.mdc-ripple-upgraded):focus .mdc-radio__focus-ring{pointer-events:none;border:2px solid transparent;border-radius:6px;box-sizing:content-box;position:absolute;top:50%;left:50%;transform:translate(-50%, -50%);height:100%;width:100%}@media screen and (forced-colors: active){.mdc-radio.mdc-ripple-upgraded--background-focused .mdc-radio__focus-ring,.mdc-radio:not(.mdc-ripple-upgraded):focus .mdc-radio__focus-ring{border-color:CanvasText}}.mdc-radio.mdc-ripple-upgraded--background-focused .mdc-radio__focus-ring::after,.mdc-radio:not(.mdc-ripple-upgraded):focus .mdc-radio__focus-ring::after{content:"";border:2px solid transparent;border-radius:8px;display:block;position:absolute;top:50%;left:50%;transform:translate(-50%, -50%);height:calc(100% + 4px);width:calc(100% + 4px)}@media screen and (forced-colors: active){.mdc-radio.mdc-ripple-upgraded--background-focused .mdc-radio__focus-ring::after,.mdc-radio:not(.mdc-ripple-upgraded):focus .mdc-radio__focus-ring::after{border-color:CanvasText}}.mdc-radio__native-control:checked+.mdc-radio__background,.mdc-radio__native-control:disabled+.mdc-radio__background{transition:opacity 120ms 0ms cubic-bezier(0, 0, 0.2, 1),transform 120ms 0ms cubic-bezier(0, 0, 0.2, 1)}.mdc-radio__native-control:checked+.mdc-radio__background .mdc-radio__outer-circle,.mdc-radio__native-control:disabled+.mdc-radio__background .mdc-radio__outer-circle{transition:border-color 120ms 0ms cubic-bezier(0, 0, 0.2, 1)}.mdc-radio__native-control:checked+.mdc-radio__background .mdc-radio__inner-circle,.mdc-radio__native-control:disabled+.mdc-radio__background .mdc-radio__inner-circle{transition:transform 120ms 0ms cubic-bezier(0, 0, 0.2, 1),border-color 120ms 0ms cubic-bezier(0, 0, 0.2, 1)}.mdc-radio--disabled{cursor:default;pointer-events:none}.mdc-radio__native-control:checked+.mdc-radio__background .mdc-radio__inner-circle{transform:scale(0.5);transition:transform 120ms 0ms cubic-bezier(0, 0, 0.2, 1),border-color 120ms 0ms cubic-bezier(0, 0, 0.2, 1)}.mdc-radio__native-control:disabled+.mdc-radio__background,[aria-disabled=true] .mdc-radio__native-control+.mdc-radio__background{cursor:default}.mdc-radio__native-control:focus+.mdc-radio__background::before{transform:scale(1);opacity:.12;transition:opacity 120ms 0ms cubic-bezier(0, 0, 0.2, 1),transform 120ms 0ms cubic-bezier(0, 0, 0.2, 1)}:host{display:inline-block;outline:none}.mdc-radio{vertical-align:bottom}.mdc-radio .mdc-radio__native-control:enabled:not(:checked)+.mdc-radio__background .mdc-radio__outer-circle{border-color:var(--mdc-radio-unchecked-color, rgba(0, 0, 0, 0.54))}.mdc-radio [aria-disabled=true] .mdc-radio__native-control:not(:checked)+.mdc-radio__background .mdc-radio__outer-circle,.mdc-radio .mdc-radio__native-control:disabled:not(:checked)+.mdc-radio__background .mdc-radio__outer-circle{border-color:var(--mdc-radio-disabled-color, rgba(0, 0, 0, 0.38))}.mdc-radio [aria-disabled=true] .mdc-radio__native-control:checked+.mdc-radio__background .mdc-radio__outer-circle,.mdc-radio .mdc-radio__native-control:disabled:checked+.mdc-radio__background .mdc-radio__outer-circle{border-color:var(--mdc-radio-disabled-color, rgba(0, 0, 0, 0.38))}.mdc-radio [aria-disabled=true] .mdc-radio__native-control+.mdc-radio__background .mdc-radio__inner-circle,.mdc-radio .mdc-radio__native-control:disabled+.mdc-radio__background .mdc-radio__inner-circle{border-color:var(--mdc-radio-disabled-color, rgba(0, 0, 0, 0.38))}`;
+let ce = class extends ee {};
+ce.styles = [te], ce = o([_("mwc-radio")], ce);
+var oe = {
         ROOT: "mdc-form-field"
     },
-    oe = {
+    ie = {
         LABEL_SELECTOR: ".mdc-form-field > label"
     },
-    ie = function(c) {
+    re = function(c) {
         function o(e) {
             var i = c.call(this, t(t({}, o.defaultAdapter), e)) || this;
             return i.click = function() {
                 i.handleClick()
             }, i
         }
         return e(o, c), Object.defineProperty(o, "cssClasses", {
             get: function() {
-                return ce
+                return oe
             },
             enumerable: !1,
             configurable: !0
         }), Object.defineProperty(o, "strings", {
             get: function() {
-                return oe
+                return ie
             },
             enumerable: !1,
             configurable: !0
         }), Object.defineProperty(o, "defaultAdapter", {
             get: function() {
                 return {
                     activateInputRipple: function() {},
@@ -382,36 +383,36 @@
         }, o.prototype.handleClick = function() {
             var e = this;
             this.adapter.activateInputRipple(), requestAnimationFrame((function() {
                 e.adapter.deactivateInputRipple()
             }))
         }, o
     }(c);
-class re extends g {
+class ae extends g {
     constructor() {
-        super(...arguments), this.alignEnd = !1, this.spaceBetween = !1, this.nowrap = !1, this.label = "", this.mdcFoundationClass = ie
+        super(...arguments), this.alignEnd = !1, this.spaceBetween = !1, this.nowrap = !1, this.label = "", this.mdcFoundationClass = re
     }
     createAdapter() {
         return {
             registerInteractionHandler: (e, t) => {
                 this.labelEl.addEventListener(e, t)
             },
             deregisterInteractionHandler: (e, t) => {
                 this.labelEl.removeEventListener(e, t)
             },
             activateInputRipple: async () => {
                 const e = this.input;
-                if (e instanceof z) {
+                if (e instanceof A) {
                     const t = await e.ripple;
                     t && t.startPress()
                 }
             },
             deactivateInputRipple: async () => {
                 const e = this.input;
-                if (e instanceof z) {
+                if (e instanceof A) {
                     const t = await e.ripple;
                     t && t.endPress()
                 }
             }
         }
     }
     get input() {
@@ -437,28 +438,28 @@
     _labelClick() {
         const e = this.input;
         e && (e.focus(), e.click())
     }
 }
 o([a({
     type: Boolean
-})], re.prototype, "alignEnd", void 0), o([a({
+})], ae.prototype, "alignEnd", void 0), o([a({
     type: Boolean
-})], re.prototype, "spaceBetween", void 0), o([a({
+})], ae.prototype, "spaceBetween", void 0), o([a({
     type: Boolean
-})], re.prototype, "nowrap", void 0), o([a({
+})], ae.prototype, "nowrap", void 0), o([a({
     type: String
 }), d((async function(e) {
     var t;
     null === (t = this.input) || void 0 === t || t.setAttribute("aria-label", e)
-}))], re.prototype, "label", void 0), o([i(".mdc-form-field")], re.prototype, "mdcRoot", void 0), o([f("", !0, "*")], re.prototype, "slottedInputs", void 0), o([i("label")], re.prototype, "labelEl", void 0);
-const ae = k`.mdc-form-field{-moz-osx-font-smoothing:grayscale;-webkit-font-smoothing:antialiased;font-family:Roboto, sans-serif;font-family:var(--mdc-typography-body2-font-family, var(--mdc-typography-font-family, Roboto, sans-serif));font-size:0.875rem;font-size:var(--mdc-typography-body2-font-size, 0.875rem);line-height:1.25rem;line-height:var(--mdc-typography-body2-line-height, 1.25rem);font-weight:400;font-weight:var(--mdc-typography-body2-font-weight, 400);letter-spacing:0.0178571429em;letter-spacing:var(--mdc-typography-body2-letter-spacing, 0.0178571429em);text-decoration:inherit;text-decoration:var(--mdc-typography-body2-text-decoration, inherit);text-transform:inherit;text-transform:var(--mdc-typography-body2-text-transform, inherit);color:rgba(0, 0, 0, 0.87);color:var(--mdc-theme-text-primary-on-background, rgba(0, 0, 0, 0.87));display:inline-flex;align-items:center;vertical-align:middle}.mdc-form-field>label{margin-left:0;margin-right:auto;padding-left:4px;padding-right:0;order:0}[dir=rtl] .mdc-form-field>label,.mdc-form-field>label[dir=rtl]{margin-left:auto;margin-right:0}[dir=rtl] .mdc-form-field>label,.mdc-form-field>label[dir=rtl]{padding-left:0;padding-right:4px}.mdc-form-field--nowrap>label{text-overflow:ellipsis;overflow:hidden;white-space:nowrap}.mdc-form-field--align-end>label{margin-left:auto;margin-right:0;padding-left:0;padding-right:4px;order:-1}[dir=rtl] .mdc-form-field--align-end>label,.mdc-form-field--align-end>label[dir=rtl]{margin-left:0;margin-right:auto}[dir=rtl] .mdc-form-field--align-end>label,.mdc-form-field--align-end>label[dir=rtl]{padding-left:4px;padding-right:0}.mdc-form-field--space-between{justify-content:space-between}.mdc-form-field--space-between>label{margin:0}[dir=rtl] .mdc-form-field--space-between>label,.mdc-form-field--space-between>label[dir=rtl]{margin:0}:host{display:inline-flex}.mdc-form-field{width:100%}::slotted(*){-moz-osx-font-smoothing:grayscale;-webkit-font-smoothing:antialiased;font-family:Roboto, sans-serif;font-family:var(--mdc-typography-body2-font-family, var(--mdc-typography-font-family, Roboto, sans-serif));font-size:0.875rem;font-size:var(--mdc-typography-body2-font-size, 0.875rem);line-height:1.25rem;line-height:var(--mdc-typography-body2-line-height, 1.25rem);font-weight:400;font-weight:var(--mdc-typography-body2-font-weight, 400);letter-spacing:0.0178571429em;letter-spacing:var(--mdc-typography-body2-letter-spacing, 0.0178571429em);text-decoration:inherit;text-decoration:var(--mdc-typography-body2-text-decoration, inherit);text-transform:inherit;text-transform:var(--mdc-typography-body2-text-transform, inherit);color:rgba(0, 0, 0, 0.87);color:var(--mdc-theme-text-primary-on-background, rgba(0, 0, 0, 0.87))}::slotted(mwc-switch){margin-right:10px}[dir=rtl] ::slotted(mwc-switch),::slotted(mwc-switch[dir=rtl]){margin-left:10px}`;
-let de = class extends re {};
-de.styles = [ae], de = o([_("mwc-formfield")], de);
-class ne extends z {
+}))], ae.prototype, "label", void 0), o([i(".mdc-form-field")], ae.prototype, "mdcRoot", void 0), o([f("", !0, "*")], ae.prototype, "slottedInputs", void 0), o([i("label")], ae.prototype, "labelEl", void 0);
+const de = k`.mdc-form-field{-moz-osx-font-smoothing:grayscale;-webkit-font-smoothing:antialiased;font-family:Roboto, sans-serif;font-family:var(--mdc-typography-body2-font-family, var(--mdc-typography-font-family, Roboto, sans-serif));font-size:0.875rem;font-size:var(--mdc-typography-body2-font-size, 0.875rem);line-height:1.25rem;line-height:var(--mdc-typography-body2-line-height, 1.25rem);font-weight:400;font-weight:var(--mdc-typography-body2-font-weight, 400);letter-spacing:0.0178571429em;letter-spacing:var(--mdc-typography-body2-letter-spacing, 0.0178571429em);text-decoration:inherit;text-decoration:var(--mdc-typography-body2-text-decoration, inherit);text-transform:inherit;text-transform:var(--mdc-typography-body2-text-transform, inherit);color:rgba(0, 0, 0, 0.87);color:var(--mdc-theme-text-primary-on-background, rgba(0, 0, 0, 0.87));display:inline-flex;align-items:center;vertical-align:middle}.mdc-form-field>label{margin-left:0;margin-right:auto;padding-left:4px;padding-right:0;order:0}[dir=rtl] .mdc-form-field>label,.mdc-form-field>label[dir=rtl]{margin-left:auto;margin-right:0}[dir=rtl] .mdc-form-field>label,.mdc-form-field>label[dir=rtl]{padding-left:0;padding-right:4px}.mdc-form-field--nowrap>label{text-overflow:ellipsis;overflow:hidden;white-space:nowrap}.mdc-form-field--align-end>label{margin-left:auto;margin-right:0;padding-left:0;padding-right:4px;order:-1}[dir=rtl] .mdc-form-field--align-end>label,.mdc-form-field--align-end>label[dir=rtl]{margin-left:0;margin-right:auto}[dir=rtl] .mdc-form-field--align-end>label,.mdc-form-field--align-end>label[dir=rtl]{padding-left:4px;padding-right:0}.mdc-form-field--space-between{justify-content:space-between}.mdc-form-field--space-between>label{margin:0}[dir=rtl] .mdc-form-field--space-between>label,.mdc-form-field--space-between>label[dir=rtl]{margin:0}:host{display:inline-flex}.mdc-form-field{width:100%}::slotted(*){-moz-osx-font-smoothing:grayscale;-webkit-font-smoothing:antialiased;font-family:Roboto, sans-serif;font-family:var(--mdc-typography-body2-font-family, var(--mdc-typography-font-family, Roboto, sans-serif));font-size:0.875rem;font-size:var(--mdc-typography-body2-font-size, 0.875rem);line-height:1.25rem;line-height:var(--mdc-typography-body2-line-height, 1.25rem);font-weight:400;font-weight:var(--mdc-typography-body2-font-weight, 400);letter-spacing:0.0178571429em;letter-spacing:var(--mdc-typography-body2-letter-spacing, 0.0178571429em);text-decoration:inherit;text-decoration:var(--mdc-typography-body2-text-decoration, inherit);text-transform:inherit;text-transform:var(--mdc-typography-body2-text-transform, inherit);color:rgba(0, 0, 0, 0.87);color:var(--mdc-theme-text-primary-on-background, rgba(0, 0, 0, 0.87))}::slotted(mwc-switch){margin-right:10px}[dir=rtl] ::slotted(mwc-switch),::slotted(mwc-switch[dir=rtl]){margin-left:10px}`;
+let ne = class extends ae {};
+ne.styles = [de], ne = o([_("mwc-formfield")], ne);
+class se extends A {
     constructor() {
         super(...arguments), this.checked = !1, this.indeterminate = !1, this.disabled = !1, this.name = "", this.value = "on", this.reducedTouchTarget = !1, this.animationClass = "", this.shouldRenderRipple = !1, this.focused = !1, this.mdcFoundationClass = void 0, this.mdcFoundation = void 0, this.rippleElement = null, this.rippleHandlers = new m((() => (this.shouldRenderRipple = !0, this.ripple.then((e => this.rippleElement = e)), this.ripple)))
     }
     createAdapter() {
         return {}
     }
     update(e) {
@@ -574,50 +575,50 @@
         this.animationClass = ""
     }
     get isRippleActive() {
         var e;
         return (null === (e = this.rippleElement) || void 0 === e ? void 0 : e.isActive) || !1
     }
 }
-o([i(".mdc-checkbox")], ne.prototype, "mdcRoot", void 0), o([i("input")], ne.prototype, "formElement", void 0), o([a({
+o([i(".mdc-checkbox")], se.prototype, "mdcRoot", void 0), o([i("input")], se.prototype, "formElement", void 0), o([a({
     type: Boolean,
     reflect: !0
-})], ne.prototype, "checked", void 0), o([a({
+})], se.prototype, "checked", void 0), o([a({
     type: Boolean
-})], ne.prototype, "indeterminate", void 0), o([a({
+})], se.prototype, "indeterminate", void 0), o([a({
     type: Boolean,
     reflect: !0
-})], ne.prototype, "disabled", void 0), o([a({
+})], se.prototype, "disabled", void 0), o([a({
     type: String,
     reflect: !0
-})], ne.prototype, "name", void 0), o([a({
+})], se.prototype, "name", void 0), o([a({
     type: String
-})], ne.prototype, "value", void 0), o([s, a({
+})], se.prototype, "value", void 0), o([s, a({
     type: String,
     attribute: "aria-label"
-})], ne.prototype, "ariaLabel", void 0), o([s, a({
+})], se.prototype, "ariaLabel", void 0), o([s, a({
     type: String,
     attribute: "aria-labelledby"
-})], ne.prototype, "ariaLabelledBy", void 0), o([s, a({
+})], se.prototype, "ariaLabelledBy", void 0), o([s, a({
     type: String,
     attribute: "aria-describedby"
-})], ne.prototype, "ariaDescribedBy", void 0), o([a({
+})], se.prototype, "ariaDescribedBy", void 0), o([a({
     type: Boolean
-})], ne.prototype, "reducedTouchTarget", void 0), o([r()], ne.prototype, "animationClass", void 0), o([r()], ne.prototype, "shouldRenderRipple", void 0), o([r()], ne.prototype, "focused", void 0), o([n("mwc-ripple")], ne.prototype, "ripple", void 0), o([l({
+})], se.prototype, "reducedTouchTarget", void 0), o([r()], se.prototype, "animationClass", void 0), o([r()], se.prototype, "shouldRenderRipple", void 0), o([r()], se.prototype, "focused", void 0), o([n("mwc-ripple")], se.prototype, "ripple", void 0), o([l({
     passive: !0
-})], ne.prototype, "handleRippleTouchStart", null);
-const se = k`.mdc-checkbox{padding:calc((40px - 18px) / 2);padding:calc((var(--mdc-checkbox-ripple-size, 40px) - 18px) / 2);margin:calc((40px - 40px) / 2);margin:calc((var(--mdc-checkbox-touch-target-size, 40px) - 40px) / 2)}.mdc-checkbox .mdc-checkbox__ripple::before,.mdc-checkbox .mdc-checkbox__ripple::after{background-color:#000;background-color:var(--mdc-ripple-color, #000)}.mdc-checkbox:hover .mdc-checkbox__ripple::before,.mdc-checkbox.mdc-ripple-surface--hover .mdc-checkbox__ripple::before{opacity:0.04;opacity:var(--mdc-ripple-hover-opacity, 0.04)}.mdc-checkbox.mdc-ripple-upgraded--background-focused .mdc-checkbox__ripple::before,.mdc-checkbox:not(.mdc-ripple-upgraded):focus .mdc-checkbox__ripple::before{transition-duration:75ms;opacity:0.12;opacity:var(--mdc-ripple-focus-opacity, 0.12)}.mdc-checkbox:not(.mdc-ripple-upgraded) .mdc-checkbox__ripple::after{transition:opacity 150ms linear}.mdc-checkbox:not(.mdc-ripple-upgraded):active .mdc-checkbox__ripple::after{transition-duration:75ms;opacity:0.12;opacity:var(--mdc-ripple-press-opacity, 0.12)}.mdc-checkbox.mdc-ripple-upgraded{--mdc-ripple-fg-opacity:var(--mdc-ripple-press-opacity, 0.12)}.mdc-checkbox.mdc-checkbox--selected .mdc-checkbox__ripple::before,.mdc-checkbox.mdc-checkbox--selected .mdc-checkbox__ripple::after{background-color:#018786;background-color:var(--mdc-ripple-color, var(--mdc-theme-secondary, #018786))}.mdc-checkbox.mdc-checkbox--selected:hover .mdc-checkbox__ripple::before,.mdc-checkbox.mdc-checkbox--selected.mdc-ripple-surface--hover .mdc-checkbox__ripple::before{opacity:0.04;opacity:var(--mdc-ripple-hover-opacity, 0.04)}.mdc-checkbox.mdc-checkbox--selected.mdc-ripple-upgraded--background-focused .mdc-checkbox__ripple::before,.mdc-checkbox.mdc-checkbox--selected:not(.mdc-ripple-upgraded):focus .mdc-checkbox__ripple::before{transition-duration:75ms;opacity:0.12;opacity:var(--mdc-ripple-focus-opacity, 0.12)}.mdc-checkbox.mdc-checkbox--selected:not(.mdc-ripple-upgraded) .mdc-checkbox__ripple::after{transition:opacity 150ms linear}.mdc-checkbox.mdc-checkbox--selected:not(.mdc-ripple-upgraded):active .mdc-checkbox__ripple::after{transition-duration:75ms;opacity:0.12;opacity:var(--mdc-ripple-press-opacity, 0.12)}.mdc-checkbox.mdc-checkbox--selected.mdc-ripple-upgraded{--mdc-ripple-fg-opacity:var(--mdc-ripple-press-opacity, 0.12)}.mdc-checkbox.mdc-ripple-upgraded--background-focused.mdc-checkbox--selected .mdc-checkbox__ripple::before,.mdc-checkbox.mdc-ripple-upgraded--background-focused.mdc-checkbox--selected .mdc-checkbox__ripple::after{background-color:#018786;background-color:var(--mdc-ripple-color, var(--mdc-theme-secondary, #018786))}.mdc-checkbox .mdc-checkbox__background{top:calc((40px - 18px) / 2);top:calc((var(--mdc-checkbox-ripple-size, 40px) - 18px) / 2);left:calc((40px - 18px) / 2);left:calc((var(--mdc-checkbox-ripple-size, 40px) - 18px) / 2)}.mdc-checkbox .mdc-checkbox__native-control{top:calc((40px - 40px) / 2);top:calc((40px - var(--mdc-checkbox-touch-target-size, 40px)) / 2);right:calc((40px - 40px) / 2);right:calc((40px - var(--mdc-checkbox-touch-target-size, 40px)) / 2);left:calc((40px - 40px) / 2);left:calc((40px - var(--mdc-checkbox-touch-target-size, 40px)) / 2);width:40px;width:var(--mdc-checkbox-touch-target-size, 40px);height:40px;height:var(--mdc-checkbox-touch-target-size, 40px)}.mdc-checkbox .mdc-checkbox__native-control:enabled:not(:checked):not(:indeterminate):not([data-indeterminate=true])~.mdc-checkbox__background{border-color:rgba(0, 0, 0, 0.54);border-color:var(--mdc-checkbox-unchecked-color, rgba(0, 0, 0, 0.54));background-color:transparent}.mdc-checkbox .mdc-checkbox__native-control:enabled:checked~.mdc-checkbox__background,.mdc-checkbox .mdc-checkbox__native-control:enabled:indeterminate~.mdc-checkbox__background,.mdc-checkbox .mdc-checkbox__native-control[data-indeterminate=true]:enabled~.mdc-checkbox__background{border-color:#018786;border-color:var(--mdc-checkbox-checked-color, var(--mdc-theme-secondary, #018786));background-color:#018786;background-color:var(--mdc-checkbox-checked-color, var(--mdc-theme-secondary, #018786))}@keyframes mdc-checkbox-fade-in-background-8A000000FF01878600000000FF018786{0%{border-color:rgba(0, 0, 0, 0.54);border-color:var(--mdc-checkbox-unchecked-color, rgba(0, 0, 0, 0.54));background-color:transparent}50%{border-color:#018786;border-color:var(--mdc-checkbox-checked-color, var(--mdc-theme-secondary, #018786));background-color:#018786;background-color:var(--mdc-checkbox-checked-color, var(--mdc-theme-secondary, #018786))}}@keyframes mdc-checkbox-fade-out-background-8A000000FF01878600000000FF018786{0%,80%{border-color:#018786;border-color:var(--mdc-checkbox-checked-color, var(--mdc-theme-secondary, #018786));background-color:#018786;background-color:var(--mdc-checkbox-checked-color, var(--mdc-theme-secondary, #018786))}100%{border-color:rgba(0, 0, 0, 0.54);border-color:var(--mdc-checkbox-unchecked-color, rgba(0, 0, 0, 0.54));background-color:transparent}}.mdc-checkbox.mdc-checkbox--anim-unchecked-checked .mdc-checkbox__native-control:enabled~.mdc-checkbox__background,.mdc-checkbox.mdc-checkbox--anim-unchecked-indeterminate .mdc-checkbox__native-control:enabled~.mdc-checkbox__background{animation-name:mdc-checkbox-fade-in-background-8A000000FF01878600000000FF018786}.mdc-checkbox.mdc-checkbox--anim-checked-unchecked .mdc-checkbox__native-control:enabled~.mdc-checkbox__background,.mdc-checkbox.mdc-checkbox--anim-indeterminate-unchecked .mdc-checkbox__native-control:enabled~.mdc-checkbox__background{animation-name:mdc-checkbox-fade-out-background-8A000000FF01878600000000FF018786}.mdc-checkbox .mdc-checkbox__native-control[disabled]:not(:checked):not(:indeterminate):not([data-indeterminate=true])~.mdc-checkbox__background{border-color:rgba(0, 0, 0, 0.38);border-color:var(--mdc-checkbox-disabled-color, rgba(0, 0, 0, 0.38));background-color:transparent}.mdc-checkbox .mdc-checkbox__native-control[disabled]:checked~.mdc-checkbox__background,.mdc-checkbox .mdc-checkbox__native-control[disabled]:indeterminate~.mdc-checkbox__background,.mdc-checkbox .mdc-checkbox__native-control[data-indeterminate=true][disabled]~.mdc-checkbox__background{border-color:transparent;background-color:rgba(0, 0, 0, 0.38);background-color:var(--mdc-checkbox-disabled-color, rgba(0, 0, 0, 0.38))}.mdc-checkbox .mdc-checkbox__native-control:enabled~.mdc-checkbox__background .mdc-checkbox__checkmark{color:#fff;color:var(--mdc-checkbox-ink-color, #fff)}.mdc-checkbox .mdc-checkbox__native-control:enabled~.mdc-checkbox__background .mdc-checkbox__mixedmark{border-color:#fff;border-color:var(--mdc-checkbox-ink-color, #fff)}.mdc-checkbox .mdc-checkbox__native-control:disabled~.mdc-checkbox__background .mdc-checkbox__checkmark{color:#fff;color:var(--mdc-checkbox-ink-color, #fff)}.mdc-checkbox .mdc-checkbox__native-control:disabled~.mdc-checkbox__background .mdc-checkbox__mixedmark{border-color:#fff;border-color:var(--mdc-checkbox-ink-color, #fff)}.mdc-touch-target-wrapper{display:inline}@keyframes mdc-checkbox-unchecked-checked-checkmark-path{0%,50%{stroke-dashoffset:29.7833385}50%{animation-timing-function:cubic-bezier(0, 0, 0.2, 1)}100%{stroke-dashoffset:0}}@keyframes mdc-checkbox-unchecked-indeterminate-mixedmark{0%,68.2%{transform:scaleX(0)}68.2%{animation-timing-function:cubic-bezier(0, 0, 0, 1)}100%{transform:scaleX(1)}}@keyframes mdc-checkbox-checked-unchecked-checkmark-path{from{animation-timing-function:cubic-bezier(0.4, 0, 1, 1);opacity:1;stroke-dashoffset:0}to{opacity:0;stroke-dashoffset:-29.7833385}}@keyframes mdc-checkbox-checked-indeterminate-checkmark{from{animation-timing-function:cubic-bezier(0, 0, 0.2, 1);transform:rotate(0deg);opacity:1}to{transform:rotate(45deg);opacity:0}}@keyframes mdc-checkbox-indeterminate-checked-checkmark{from{animation-timing-function:cubic-bezier(0.14, 0, 0, 1);transform:rotate(45deg);opacity:0}to{transform:rotate(360deg);opacity:1}}@keyframes mdc-checkbox-checked-indeterminate-mixedmark{from{animation-timing-function:mdc-animation-deceleration-curve-timing-function;transform:rotate(-45deg);opacity:0}to{transform:rotate(0deg);opacity:1}}@keyframes mdc-checkbox-indeterminate-checked-mixedmark{from{animation-timing-function:cubic-bezier(0.14, 0, 0, 1);transform:rotate(0deg);opacity:1}to{transform:rotate(315deg);opacity:0}}@keyframes mdc-checkbox-indeterminate-unchecked-mixedmark{0%{animation-timing-function:linear;transform:scaleX(1);opacity:1}32.8%,100%{transform:scaleX(0);opacity:0}}.mdc-checkbox{display:inline-block;position:relative;flex:0 0 18px;box-sizing:content-box;width:18px;height:18px;line-height:0;white-space:nowrap;cursor:pointer;vertical-align:bottom}.mdc-checkbox.mdc-ripple-upgraded--background-focused .mdc-checkbox__focus-ring,.mdc-checkbox:not(.mdc-ripple-upgraded):focus .mdc-checkbox__focus-ring{pointer-events:none;border:2px solid transparent;border-radius:6px;box-sizing:content-box;position:absolute;top:50%;left:50%;transform:translate(-50%, -50%);height:100%;width:100%}@media screen and (forced-colors: active){.mdc-checkbox.mdc-ripple-upgraded--background-focused .mdc-checkbox__focus-ring,.mdc-checkbox:not(.mdc-ripple-upgraded):focus .mdc-checkbox__focus-ring{border-color:CanvasText}}.mdc-checkbox.mdc-ripple-upgraded--background-focused .mdc-checkbox__focus-ring::after,.mdc-checkbox:not(.mdc-ripple-upgraded):focus .mdc-checkbox__focus-ring::after{content:"";border:2px solid transparent;border-radius:8px;display:block;position:absolute;top:50%;left:50%;transform:translate(-50%, -50%);height:calc(100% + 4px);width:calc(100% + 4px)}@media screen and (forced-colors: active){.mdc-checkbox.mdc-ripple-upgraded--background-focused .mdc-checkbox__focus-ring::after,.mdc-checkbox:not(.mdc-ripple-upgraded):focus .mdc-checkbox__focus-ring::after{border-color:CanvasText}}@media all and (-ms-high-contrast: none){.mdc-checkbox .mdc-checkbox__focus-ring{display:none}}@media screen and (forced-colors: active),(-ms-high-contrast: active){.mdc-checkbox__mixedmark{margin:0 1px}}.mdc-checkbox--disabled{cursor:default;pointer-events:none}.mdc-checkbox__background{display:inline-flex;position:absolute;align-items:center;justify-content:center;box-sizing:border-box;width:18px;height:18px;border:2px solid currentColor;border-radius:2px;background-color:transparent;pointer-events:none;will-change:background-color,border-color;transition:background-color 90ms 0ms cubic-bezier(0.4, 0, 0.6, 1),border-color 90ms 0ms cubic-bezier(0.4, 0, 0.6, 1)}.mdc-checkbox__checkmark{position:absolute;top:0;right:0;bottom:0;left:0;width:100%;opacity:0;transition:opacity 180ms 0ms cubic-bezier(0.4, 0, 0.6, 1)}.mdc-checkbox--upgraded .mdc-checkbox__checkmark{opacity:1}.mdc-checkbox__checkmark-path{transition:stroke-dashoffset 180ms 0ms cubic-bezier(0.4, 0, 0.6, 1);stroke:currentColor;stroke-width:3.12px;stroke-dashoffset:29.7833385;stroke-dasharray:29.7833385}.mdc-checkbox__mixedmark{width:100%;height:0;transform:scaleX(0) rotate(0deg);border-width:1px;border-style:solid;opacity:0;transition:opacity 90ms 0ms cubic-bezier(0.4, 0, 0.6, 1),transform 90ms 0ms cubic-bezier(0.4, 0, 0.6, 1)}.mdc-checkbox--anim-unchecked-checked .mdc-checkbox__background,.mdc-checkbox--anim-unchecked-indeterminate .mdc-checkbox__background,.mdc-checkbox--anim-checked-unchecked .mdc-checkbox__background,.mdc-checkbox--anim-indeterminate-unchecked .mdc-checkbox__background{animation-duration:180ms;animation-timing-function:linear}.mdc-checkbox--anim-unchecked-checked .mdc-checkbox__checkmark-path{animation:mdc-checkbox-unchecked-checked-checkmark-path 180ms linear 0s;transition:none}.mdc-checkbox--anim-unchecked-indeterminate .mdc-checkbox__mixedmark{animation:mdc-checkbox-unchecked-indeterminate-mixedmark 90ms linear 0s;transition:none}.mdc-checkbox--anim-checked-unchecked .mdc-checkbox__checkmark-path{animation:mdc-checkbox-checked-unchecked-checkmark-path 90ms linear 0s;transition:none}.mdc-checkbox--anim-checked-indeterminate .mdc-checkbox__checkmark{animation:mdc-checkbox-checked-indeterminate-checkmark 90ms linear 0s;transition:none}.mdc-checkbox--anim-checked-indeterminate .mdc-checkbox__mixedmark{animation:mdc-checkbox-checked-indeterminate-mixedmark 90ms linear 0s;transition:none}.mdc-checkbox--anim-indeterminate-checked .mdc-checkbox__checkmark{animation:mdc-checkbox-indeterminate-checked-checkmark 500ms linear 0s;transition:none}.mdc-checkbox--anim-indeterminate-checked .mdc-checkbox__mixedmark{animation:mdc-checkbox-indeterminate-checked-mixedmark 500ms linear 0s;transition:none}.mdc-checkbox--anim-indeterminate-unchecked .mdc-checkbox__mixedmark{animation:mdc-checkbox-indeterminate-unchecked-mixedmark 300ms linear 0s;transition:none}.mdc-checkbox__native-control:checked~.mdc-checkbox__background,.mdc-checkbox__native-control:indeterminate~.mdc-checkbox__background,.mdc-checkbox__native-control[data-indeterminate=true]~.mdc-checkbox__background{transition:border-color 90ms 0ms cubic-bezier(0, 0, 0.2, 1),background-color 90ms 0ms cubic-bezier(0, 0, 0.2, 1)}.mdc-checkbox__native-control:checked~.mdc-checkbox__background .mdc-checkbox__checkmark-path,.mdc-checkbox__native-control:indeterminate~.mdc-checkbox__background .mdc-checkbox__checkmark-path,.mdc-checkbox__native-control[data-indeterminate=true]~.mdc-checkbox__background .mdc-checkbox__checkmark-path{stroke-dashoffset:0}.mdc-checkbox__native-control{position:absolute;margin:0;padding:0;opacity:0;cursor:inherit}.mdc-checkbox__native-control:disabled{cursor:default;pointer-events:none}.mdc-checkbox--touch{margin:calc((48px - 40px) / 2);margin:calc((var(--mdc-checkbox-state-layer-size, 48px) - var(--mdc-checkbox-state-layer-size, 40px)) / 2)}.mdc-checkbox--touch .mdc-checkbox__native-control{top:calc((40px - 48px) / 2);top:calc((var(--mdc-checkbox-state-layer-size, 40px) - var(--mdc-checkbox-state-layer-size, 48px)) / 2);right:calc((40px - 48px) / 2);right:calc((var(--mdc-checkbox-state-layer-size, 40px) - var(--mdc-checkbox-state-layer-size, 48px)) / 2);left:calc((40px - 48px) / 2);left:calc((var(--mdc-checkbox-state-layer-size, 40px) - var(--mdc-checkbox-state-layer-size, 48px)) / 2);width:48px;width:var(--mdc-checkbox-state-layer-size, 48px);height:48px;height:var(--mdc-checkbox-state-layer-size, 48px)}.mdc-checkbox__native-control:checked~.mdc-checkbox__background .mdc-checkbox__checkmark{transition:opacity 180ms 0ms cubic-bezier(0, 0, 0.2, 1),transform 180ms 0ms cubic-bezier(0, 0, 0.2, 1);opacity:1}.mdc-checkbox__native-control:checked~.mdc-checkbox__background .mdc-checkbox__mixedmark{transform:scaleX(1) rotate(-45deg)}.mdc-checkbox__native-control:indeterminate~.mdc-checkbox__background .mdc-checkbox__checkmark,.mdc-checkbox__native-control[data-indeterminate=true]~.mdc-checkbox__background .mdc-checkbox__checkmark{transform:rotate(45deg);opacity:0;transition:opacity 90ms 0ms cubic-bezier(0.4, 0, 0.6, 1),transform 90ms 0ms cubic-bezier(0.4, 0, 0.6, 1)}.mdc-checkbox__native-control:indeterminate~.mdc-checkbox__background .mdc-checkbox__mixedmark,.mdc-checkbox__native-control[data-indeterminate=true]~.mdc-checkbox__background .mdc-checkbox__mixedmark{transform:scaleX(1) rotate(0deg);opacity:1}.mdc-checkbox.mdc-checkbox--upgraded .mdc-checkbox__background,.mdc-checkbox.mdc-checkbox--upgraded .mdc-checkbox__checkmark,.mdc-checkbox.mdc-checkbox--upgraded .mdc-checkbox__checkmark-path,.mdc-checkbox.mdc-checkbox--upgraded .mdc-checkbox__mixedmark{transition:none}:host{outline:none;display:inline-flex;-webkit-tap-highlight-color:transparent}:host([checked]),:host([indeterminate]){--mdc-ripple-color:var(--mdc-theme-secondary, #018786)}.mdc-checkbox .mdc-checkbox__background::before{content:none}`;
-let le = class extends ne {};
-le.styles = [se], le = o([_("mwc-checkbox")], le);
-let me = class extends v {
+})], se.prototype, "handleRippleTouchStart", null);
+const le = k`.mdc-checkbox{padding:calc((40px - 18px) / 2);padding:calc((var(--mdc-checkbox-ripple-size, 40px) - 18px) / 2);margin:calc((40px - 40px) / 2);margin:calc((var(--mdc-checkbox-touch-target-size, 40px) - 40px) / 2)}.mdc-checkbox .mdc-checkbox__ripple::before,.mdc-checkbox .mdc-checkbox__ripple::after{background-color:#000;background-color:var(--mdc-ripple-color, #000)}.mdc-checkbox:hover .mdc-checkbox__ripple::before,.mdc-checkbox.mdc-ripple-surface--hover .mdc-checkbox__ripple::before{opacity:0.04;opacity:var(--mdc-ripple-hover-opacity, 0.04)}.mdc-checkbox.mdc-ripple-upgraded--background-focused .mdc-checkbox__ripple::before,.mdc-checkbox:not(.mdc-ripple-upgraded):focus .mdc-checkbox__ripple::before{transition-duration:75ms;opacity:0.12;opacity:var(--mdc-ripple-focus-opacity, 0.12)}.mdc-checkbox:not(.mdc-ripple-upgraded) .mdc-checkbox__ripple::after{transition:opacity 150ms linear}.mdc-checkbox:not(.mdc-ripple-upgraded):active .mdc-checkbox__ripple::after{transition-duration:75ms;opacity:0.12;opacity:var(--mdc-ripple-press-opacity, 0.12)}.mdc-checkbox.mdc-ripple-upgraded{--mdc-ripple-fg-opacity:var(--mdc-ripple-press-opacity, 0.12)}.mdc-checkbox.mdc-checkbox--selected .mdc-checkbox__ripple::before,.mdc-checkbox.mdc-checkbox--selected .mdc-checkbox__ripple::after{background-color:#018786;background-color:var(--mdc-ripple-color, var(--mdc-theme-secondary, #018786))}.mdc-checkbox.mdc-checkbox--selected:hover .mdc-checkbox__ripple::before,.mdc-checkbox.mdc-checkbox--selected.mdc-ripple-surface--hover .mdc-checkbox__ripple::before{opacity:0.04;opacity:var(--mdc-ripple-hover-opacity, 0.04)}.mdc-checkbox.mdc-checkbox--selected.mdc-ripple-upgraded--background-focused .mdc-checkbox__ripple::before,.mdc-checkbox.mdc-checkbox--selected:not(.mdc-ripple-upgraded):focus .mdc-checkbox__ripple::before{transition-duration:75ms;opacity:0.12;opacity:var(--mdc-ripple-focus-opacity, 0.12)}.mdc-checkbox.mdc-checkbox--selected:not(.mdc-ripple-upgraded) .mdc-checkbox__ripple::after{transition:opacity 150ms linear}.mdc-checkbox.mdc-checkbox--selected:not(.mdc-ripple-upgraded):active .mdc-checkbox__ripple::after{transition-duration:75ms;opacity:0.12;opacity:var(--mdc-ripple-press-opacity, 0.12)}.mdc-checkbox.mdc-checkbox--selected.mdc-ripple-upgraded{--mdc-ripple-fg-opacity:var(--mdc-ripple-press-opacity, 0.12)}.mdc-checkbox.mdc-ripple-upgraded--background-focused.mdc-checkbox--selected .mdc-checkbox__ripple::before,.mdc-checkbox.mdc-ripple-upgraded--background-focused.mdc-checkbox--selected .mdc-checkbox__ripple::after{background-color:#018786;background-color:var(--mdc-ripple-color, var(--mdc-theme-secondary, #018786))}.mdc-checkbox .mdc-checkbox__background{top:calc((40px - 18px) / 2);top:calc((var(--mdc-checkbox-ripple-size, 40px) - 18px) / 2);left:calc((40px - 18px) / 2);left:calc((var(--mdc-checkbox-ripple-size, 40px) - 18px) / 2)}.mdc-checkbox .mdc-checkbox__native-control{top:calc((40px - 40px) / 2);top:calc((40px - var(--mdc-checkbox-touch-target-size, 40px)) / 2);right:calc((40px - 40px) / 2);right:calc((40px - var(--mdc-checkbox-touch-target-size, 40px)) / 2);left:calc((40px - 40px) / 2);left:calc((40px - var(--mdc-checkbox-touch-target-size, 40px)) / 2);width:40px;width:var(--mdc-checkbox-touch-target-size, 40px);height:40px;height:var(--mdc-checkbox-touch-target-size, 40px)}.mdc-checkbox .mdc-checkbox__native-control:enabled:not(:checked):not(:indeterminate):not([data-indeterminate=true])~.mdc-checkbox__background{border-color:rgba(0, 0, 0, 0.54);border-color:var(--mdc-checkbox-unchecked-color, rgba(0, 0, 0, 0.54));background-color:transparent}.mdc-checkbox .mdc-checkbox__native-control:enabled:checked~.mdc-checkbox__background,.mdc-checkbox .mdc-checkbox__native-control:enabled:indeterminate~.mdc-checkbox__background,.mdc-checkbox .mdc-checkbox__native-control[data-indeterminate=true]:enabled~.mdc-checkbox__background{border-color:#018786;border-color:var(--mdc-checkbox-checked-color, var(--mdc-theme-secondary, #018786));background-color:#018786;background-color:var(--mdc-checkbox-checked-color, var(--mdc-theme-secondary, #018786))}@keyframes mdc-checkbox-fade-in-background-8A000000FF01878600000000FF018786{0%{border-color:rgba(0, 0, 0, 0.54);border-color:var(--mdc-checkbox-unchecked-color, rgba(0, 0, 0, 0.54));background-color:transparent}50%{border-color:#018786;border-color:var(--mdc-checkbox-checked-color, var(--mdc-theme-secondary, #018786));background-color:#018786;background-color:var(--mdc-checkbox-checked-color, var(--mdc-theme-secondary, #018786))}}@keyframes mdc-checkbox-fade-out-background-8A000000FF01878600000000FF018786{0%,80%{border-color:#018786;border-color:var(--mdc-checkbox-checked-color, var(--mdc-theme-secondary, #018786));background-color:#018786;background-color:var(--mdc-checkbox-checked-color, var(--mdc-theme-secondary, #018786))}100%{border-color:rgba(0, 0, 0, 0.54);border-color:var(--mdc-checkbox-unchecked-color, rgba(0, 0, 0, 0.54));background-color:transparent}}.mdc-checkbox.mdc-checkbox--anim-unchecked-checked .mdc-checkbox__native-control:enabled~.mdc-checkbox__background,.mdc-checkbox.mdc-checkbox--anim-unchecked-indeterminate .mdc-checkbox__native-control:enabled~.mdc-checkbox__background{animation-name:mdc-checkbox-fade-in-background-8A000000FF01878600000000FF018786}.mdc-checkbox.mdc-checkbox--anim-checked-unchecked .mdc-checkbox__native-control:enabled~.mdc-checkbox__background,.mdc-checkbox.mdc-checkbox--anim-indeterminate-unchecked .mdc-checkbox__native-control:enabled~.mdc-checkbox__background{animation-name:mdc-checkbox-fade-out-background-8A000000FF01878600000000FF018786}.mdc-checkbox .mdc-checkbox__native-control[disabled]:not(:checked):not(:indeterminate):not([data-indeterminate=true])~.mdc-checkbox__background{border-color:rgba(0, 0, 0, 0.38);border-color:var(--mdc-checkbox-disabled-color, rgba(0, 0, 0, 0.38));background-color:transparent}.mdc-checkbox .mdc-checkbox__native-control[disabled]:checked~.mdc-checkbox__background,.mdc-checkbox .mdc-checkbox__native-control[disabled]:indeterminate~.mdc-checkbox__background,.mdc-checkbox .mdc-checkbox__native-control[data-indeterminate=true][disabled]~.mdc-checkbox__background{border-color:transparent;background-color:rgba(0, 0, 0, 0.38);background-color:var(--mdc-checkbox-disabled-color, rgba(0, 0, 0, 0.38))}.mdc-checkbox .mdc-checkbox__native-control:enabled~.mdc-checkbox__background .mdc-checkbox__checkmark{color:#fff;color:var(--mdc-checkbox-ink-color, #fff)}.mdc-checkbox .mdc-checkbox__native-control:enabled~.mdc-checkbox__background .mdc-checkbox__mixedmark{border-color:#fff;border-color:var(--mdc-checkbox-ink-color, #fff)}.mdc-checkbox .mdc-checkbox__native-control:disabled~.mdc-checkbox__background .mdc-checkbox__checkmark{color:#fff;color:var(--mdc-checkbox-ink-color, #fff)}.mdc-checkbox .mdc-checkbox__native-control:disabled~.mdc-checkbox__background .mdc-checkbox__mixedmark{border-color:#fff;border-color:var(--mdc-checkbox-ink-color, #fff)}.mdc-touch-target-wrapper{display:inline}@keyframes mdc-checkbox-unchecked-checked-checkmark-path{0%,50%{stroke-dashoffset:29.7833385}50%{animation-timing-function:cubic-bezier(0, 0, 0.2, 1)}100%{stroke-dashoffset:0}}@keyframes mdc-checkbox-unchecked-indeterminate-mixedmark{0%,68.2%{transform:scaleX(0)}68.2%{animation-timing-function:cubic-bezier(0, 0, 0, 1)}100%{transform:scaleX(1)}}@keyframes mdc-checkbox-checked-unchecked-checkmark-path{from{animation-timing-function:cubic-bezier(0.4, 0, 1, 1);opacity:1;stroke-dashoffset:0}to{opacity:0;stroke-dashoffset:-29.7833385}}@keyframes mdc-checkbox-checked-indeterminate-checkmark{from{animation-timing-function:cubic-bezier(0, 0, 0.2, 1);transform:rotate(0deg);opacity:1}to{transform:rotate(45deg);opacity:0}}@keyframes mdc-checkbox-indeterminate-checked-checkmark{from{animation-timing-function:cubic-bezier(0.14, 0, 0, 1);transform:rotate(45deg);opacity:0}to{transform:rotate(360deg);opacity:1}}@keyframes mdc-checkbox-checked-indeterminate-mixedmark{from{animation-timing-function:mdc-animation-deceleration-curve-timing-function;transform:rotate(-45deg);opacity:0}to{transform:rotate(0deg);opacity:1}}@keyframes mdc-checkbox-indeterminate-checked-mixedmark{from{animation-timing-function:cubic-bezier(0.14, 0, 0, 1);transform:rotate(0deg);opacity:1}to{transform:rotate(315deg);opacity:0}}@keyframes mdc-checkbox-indeterminate-unchecked-mixedmark{0%{animation-timing-function:linear;transform:scaleX(1);opacity:1}32.8%,100%{transform:scaleX(0);opacity:0}}.mdc-checkbox{display:inline-block;position:relative;flex:0 0 18px;box-sizing:content-box;width:18px;height:18px;line-height:0;white-space:nowrap;cursor:pointer;vertical-align:bottom}.mdc-checkbox.mdc-ripple-upgraded--background-focused .mdc-checkbox__focus-ring,.mdc-checkbox:not(.mdc-ripple-upgraded):focus .mdc-checkbox__focus-ring{pointer-events:none;border:2px solid transparent;border-radius:6px;box-sizing:content-box;position:absolute;top:50%;left:50%;transform:translate(-50%, -50%);height:100%;width:100%}@media screen and (forced-colors: active){.mdc-checkbox.mdc-ripple-upgraded--background-focused .mdc-checkbox__focus-ring,.mdc-checkbox:not(.mdc-ripple-upgraded):focus .mdc-checkbox__focus-ring{border-color:CanvasText}}.mdc-checkbox.mdc-ripple-upgraded--background-focused .mdc-checkbox__focus-ring::after,.mdc-checkbox:not(.mdc-ripple-upgraded):focus .mdc-checkbox__focus-ring::after{content:"";border:2px solid transparent;border-radius:8px;display:block;position:absolute;top:50%;left:50%;transform:translate(-50%, -50%);height:calc(100% + 4px);width:calc(100% + 4px)}@media screen and (forced-colors: active){.mdc-checkbox.mdc-ripple-upgraded--background-focused .mdc-checkbox__focus-ring::after,.mdc-checkbox:not(.mdc-ripple-upgraded):focus .mdc-checkbox__focus-ring::after{border-color:CanvasText}}@media all and (-ms-high-contrast: none){.mdc-checkbox .mdc-checkbox__focus-ring{display:none}}@media screen and (forced-colors: active),(-ms-high-contrast: active){.mdc-checkbox__mixedmark{margin:0 1px}}.mdc-checkbox--disabled{cursor:default;pointer-events:none}.mdc-checkbox__background{display:inline-flex;position:absolute;align-items:center;justify-content:center;box-sizing:border-box;width:18px;height:18px;border:2px solid currentColor;border-radius:2px;background-color:transparent;pointer-events:none;will-change:background-color,border-color;transition:background-color 90ms 0ms cubic-bezier(0.4, 0, 0.6, 1),border-color 90ms 0ms cubic-bezier(0.4, 0, 0.6, 1)}.mdc-checkbox__checkmark{position:absolute;top:0;right:0;bottom:0;left:0;width:100%;opacity:0;transition:opacity 180ms 0ms cubic-bezier(0.4, 0, 0.6, 1)}.mdc-checkbox--upgraded .mdc-checkbox__checkmark{opacity:1}.mdc-checkbox__checkmark-path{transition:stroke-dashoffset 180ms 0ms cubic-bezier(0.4, 0, 0.6, 1);stroke:currentColor;stroke-width:3.12px;stroke-dashoffset:29.7833385;stroke-dasharray:29.7833385}.mdc-checkbox__mixedmark{width:100%;height:0;transform:scaleX(0) rotate(0deg);border-width:1px;border-style:solid;opacity:0;transition:opacity 90ms 0ms cubic-bezier(0.4, 0, 0.6, 1),transform 90ms 0ms cubic-bezier(0.4, 0, 0.6, 1)}.mdc-checkbox--anim-unchecked-checked .mdc-checkbox__background,.mdc-checkbox--anim-unchecked-indeterminate .mdc-checkbox__background,.mdc-checkbox--anim-checked-unchecked .mdc-checkbox__background,.mdc-checkbox--anim-indeterminate-unchecked .mdc-checkbox__background{animation-duration:180ms;animation-timing-function:linear}.mdc-checkbox--anim-unchecked-checked .mdc-checkbox__checkmark-path{animation:mdc-checkbox-unchecked-checked-checkmark-path 180ms linear 0s;transition:none}.mdc-checkbox--anim-unchecked-indeterminate .mdc-checkbox__mixedmark{animation:mdc-checkbox-unchecked-indeterminate-mixedmark 90ms linear 0s;transition:none}.mdc-checkbox--anim-checked-unchecked .mdc-checkbox__checkmark-path{animation:mdc-checkbox-checked-unchecked-checkmark-path 90ms linear 0s;transition:none}.mdc-checkbox--anim-checked-indeterminate .mdc-checkbox__checkmark{animation:mdc-checkbox-checked-indeterminate-checkmark 90ms linear 0s;transition:none}.mdc-checkbox--anim-checked-indeterminate .mdc-checkbox__mixedmark{animation:mdc-checkbox-checked-indeterminate-mixedmark 90ms linear 0s;transition:none}.mdc-checkbox--anim-indeterminate-checked .mdc-checkbox__checkmark{animation:mdc-checkbox-indeterminate-checked-checkmark 500ms linear 0s;transition:none}.mdc-checkbox--anim-indeterminate-checked .mdc-checkbox__mixedmark{animation:mdc-checkbox-indeterminate-checked-mixedmark 500ms linear 0s;transition:none}.mdc-checkbox--anim-indeterminate-unchecked .mdc-checkbox__mixedmark{animation:mdc-checkbox-indeterminate-unchecked-mixedmark 300ms linear 0s;transition:none}.mdc-checkbox__native-control:checked~.mdc-checkbox__background,.mdc-checkbox__native-control:indeterminate~.mdc-checkbox__background,.mdc-checkbox__native-control[data-indeterminate=true]~.mdc-checkbox__background{transition:border-color 90ms 0ms cubic-bezier(0, 0, 0.2, 1),background-color 90ms 0ms cubic-bezier(0, 0, 0.2, 1)}.mdc-checkbox__native-control:checked~.mdc-checkbox__background .mdc-checkbox__checkmark-path,.mdc-checkbox__native-control:indeterminate~.mdc-checkbox__background .mdc-checkbox__checkmark-path,.mdc-checkbox__native-control[data-indeterminate=true]~.mdc-checkbox__background .mdc-checkbox__checkmark-path{stroke-dashoffset:0}.mdc-checkbox__native-control{position:absolute;margin:0;padding:0;opacity:0;cursor:inherit}.mdc-checkbox__native-control:disabled{cursor:default;pointer-events:none}.mdc-checkbox--touch{margin:calc((48px - 40px) / 2);margin:calc((var(--mdc-checkbox-state-layer-size, 48px) - var(--mdc-checkbox-state-layer-size, 40px)) / 2)}.mdc-checkbox--touch .mdc-checkbox__native-control{top:calc((40px - 48px) / 2);top:calc((var(--mdc-checkbox-state-layer-size, 40px) - var(--mdc-checkbox-state-layer-size, 48px)) / 2);right:calc((40px - 48px) / 2);right:calc((var(--mdc-checkbox-state-layer-size, 40px) - var(--mdc-checkbox-state-layer-size, 48px)) / 2);left:calc((40px - 48px) / 2);left:calc((var(--mdc-checkbox-state-layer-size, 40px) - var(--mdc-checkbox-state-layer-size, 48px)) / 2);width:48px;width:var(--mdc-checkbox-state-layer-size, 48px);height:48px;height:var(--mdc-checkbox-state-layer-size, 48px)}.mdc-checkbox__native-control:checked~.mdc-checkbox__background .mdc-checkbox__checkmark{transition:opacity 180ms 0ms cubic-bezier(0, 0, 0.2, 1),transform 180ms 0ms cubic-bezier(0, 0, 0.2, 1);opacity:1}.mdc-checkbox__native-control:checked~.mdc-checkbox__background .mdc-checkbox__mixedmark{transform:scaleX(1) rotate(-45deg)}.mdc-checkbox__native-control:indeterminate~.mdc-checkbox__background .mdc-checkbox__checkmark,.mdc-checkbox__native-control[data-indeterminate=true]~.mdc-checkbox__background .mdc-checkbox__checkmark{transform:rotate(45deg);opacity:0;transition:opacity 90ms 0ms cubic-bezier(0.4, 0, 0.6, 1),transform 90ms 0ms cubic-bezier(0.4, 0, 0.6, 1)}.mdc-checkbox__native-control:indeterminate~.mdc-checkbox__background .mdc-checkbox__mixedmark,.mdc-checkbox__native-control[data-indeterminate=true]~.mdc-checkbox__background .mdc-checkbox__mixedmark{transform:scaleX(1) rotate(0deg);opacity:1}.mdc-checkbox.mdc-checkbox--upgraded .mdc-checkbox__background,.mdc-checkbox.mdc-checkbox--upgraded .mdc-checkbox__checkmark,.mdc-checkbox.mdc-checkbox--upgraded .mdc-checkbox__checkmark-path,.mdc-checkbox.mdc-checkbox--upgraded .mdc-checkbox__mixedmark{transition:none}:host{outline:none;display:inline-flex;-webkit-tap-highlight-color:transparent}:host([checked]),:host([indeterminate]){--mdc-ripple-color:var(--mdc-theme-secondary, #018786)}.mdc-checkbox .mdc-checkbox__background::before{content:none}`;
+let me = class extends se {};
+me.styles = [le], me = o([_("mwc-checkbox")], me);
+let he = class extends v {
     constructor() {
         super(...arguments), this._busy = !1, this._platform = "ESP32", this._board = this._platformData().defaultBoard, this._useRecommended = !0, this._hasWifiSecrets = void 0, this._data = {
-            ssid: `!secret ${j}`,
-            psk: `!secret ${M}`
-        }, this._state = T ? "basic_config" : "ask_esphome_web", this._installed = !1, this._cleanSSIDBlur = e => {
+            ssid: `!secret ${M}`,
+            psk: `!secret ${U}`
+        }, this._state = H ? "basic_config" : "ask_esphome_web", this._installed = !1, this._cleanSSIDBlur = e => {
             const t = e.target;
             t.value = t.value.trim()
         }
     }
     _platformData() {
         return D[this._platform]
     }
@@ -674,15 +675,15 @@
         return ["New device", h`
       <div>
         A device needs to be connected to a computer using a USB cable to be
         added to ESPHome. Once added, ESPHome will interact with the device
         wirelessly.
       </div>
       <div>
-        ${H?"Your browser does not support WebSerial.":"You are not browsing the dashboard over a secure connection (HTTPS)."}
+        ${I?"Your browser does not support WebSerial.":"You are not browsing the dashboard over a secure connection (HTTPS)."}
         This prevents ESPHome from being able to install this on devices
         connected to this computer.
       </div>
       <div>
         You will still be able to install ESPHome by connecting the device to
         the computer that runs the ESPHome dashboard.
       </div>
@@ -709,15 +710,15 @@
           label="Open ESPHome Web"
         ></mwc-button>
       </a>
     `, !1]
     }
     _renderBasicConfig() {
         if (void 0 === this._hasWifiSecrets) return [void 0, this._renderProgress("Initializing"), !0];
-        return [T ? "New device" : "Create configuration", h`
+        return [H ? "New device" : "Create configuration", h`
       ${this._error?h`<div class="error">${this._error}</div>`:""}
 
       <mwc-textfield label="Name" name="name" required></mwc-textfield>
 
       ${this._hasWifiSecrets?h`
             <div>
               This device will be configured to connect to the Wi-Fi network
@@ -927,15 +928,15 @@
               dialogAction="close"
               label="Skip"
             ></mwc-button>
           `}
     `
     }
     firstUpdated(e) {
-        super.firstUpdated(e), U().then((e => {
+        super.firstUpdated(e), W().then((e => {
             this._hasWifiSecrets = e
         }))
     }
     updated(e) {
         if (super.updated(e), e.has("_state") || e.has("_hasWifiSecrets")) {
             const e = this.shadowRoot.querySelector("mwc-textfield, mwc-radio, mwc-button");
             e && e.updateComplete.then((() => e.focus()))
@@ -959,15 +960,15 @@
         if (!t) return void e.focus();
         if (!c) return void this._inputSSID.focus();
         const o = e.value;
         this._data.name = o, this._hasWifiSecrets || (this._wifi = {
             ssid: this._inputSSID.value,
             password: this._inputPassword.value
         }), setTimeout((() => {
-            this._state = T && H ? "connect_webserial" : "pick_platform"
+            this._state = H && I ? "connect_webserial" : "pick_platform"
         }), 0)
     }
     _handleUseRecommendedCheckbox(e) {
         this._useRecommended = e.target.checked
     }
     _handlePickBoardSelect(e) {
         this._board = e.target.value
@@ -975,15 +976,15 @@
     async _handlePickPlatformClick(e) {
         this._supportedBoards = void 0, this._platform = e.currentTarget.platform, this._board = this._platformData().defaultBoard, this._useRecommended && null !== this._board ? await this._handlePickBoardSubmit() : (this._busy = !0, this._state = "pick_board")
     }
     async _handlePickBoardSubmit() {
         if (this._board) {
             this._data.board = this._board, this._busy = !0;
             try {
-                this._wifi && await W(this._wifi.ssid, this._wifi.password);
+                this._wifi && await q(this._wifi.ssid, this._wifi.password);
                 const e = await w(this._data);
                 this._configFilename = e.configuration, $(), this._apiKey = await S(this._configFilename), this._state = "done"
             } catch (e) {
                 this._error = e.message || e
             } finally {
                 this._busy = !1
             }
@@ -998,26 +999,26 @@
         this._busy = !0, this._error = void 0;
         let c = !1;
         try {
             let o, i;
             try {
                 o = await navigator.serial.requestPort()
             } catch (e) {
-                return console.error(e), void("NotFoundError" === e.name ? A() : this._error = e.message || String(e))
+                return console.error(e), void("NotFoundError" === e.name ? B() : this._error = e.message || String(e))
             }
-            t = B(o), this._state = "connecting_webserial";
+            t = T(o), this._state = "connecting_webserial";
             try {
                 await t.main_fn(), await t.flash_id()
             } catch (e) {
                 return console.error(e), this._state = "connect_webserial", void(this._error = "Failed to initialize. Try resetting your device or holding the BOOT button while selecting your serial port until it starts preparing the installation.")
             }
             this._state = "prepare_flash";
             const r = t.chip.CHIP_NAME;
-            if (!Object.keys(I).includes(r)) return this._state = "connect_webserial", void(this._error = `Unable to identify the connected device (${t.chip.CHIP_NAME}).`);
-            i = I[r], this._data.board = null !== (e = D[i].defaultBoard) && void 0 !== e ? e : void 0;
+            if (!Object.keys(L).includes(r)) return this._state = "connect_webserial", void(this._error = `Unable to identify the connected device (${t.chip.CHIP_NAME}).`);
+            i = L[r], this._data.board = null !== (e = D[i].defaultBoard) && void 0 !== e ? e : void 0;
             try {
                 const {
                     configuration: e
                 } = await w(this._data);
                 this._configFilename = e
             } catch (e) {
                 return console.error(e), this._state = "connect_webserial", void(this._error = "Unable to create the configuration")
@@ -1026,22 +1027,22 @@
             try {
                 await C(this._configFilename)
             } catch (e) {
                 return console.error(e), this._state = "connect_webserial", void(this._error = "Unable to compile the configuration")
             }
             this._state = "flashing";
             try {
-                const e = await L(this._configFilename);
-                await O(t, e, !0, (e => {
+                const e = await O(this._configFilename);
+                await N(t, e, !0, (e => {
                     this._writeProgress = e
                 }))
             } catch (e) {
                 return console.error(e), this._state = "connect_webserial", void(this._error = "Error installing the configuration")
             }
-            c = !1, this._installed = !0, await N(t.transport), this._state = "wait_come_online";
+            c = !1, this._installed = !0, await j(t.transport), this._state = "wait_come_online";
             try {
                 await new Promise(((e, t) => {
                     const c = R((t => {
                             t[this._configFilename] && (c(), clearTimeout(o), e(void 0))
                         })),
                         o = setTimeout((() => {
                             c(), t("Timeout")
@@ -1056,18 +1057,18 @@
         }
     }
     async _handleClose() {
         this.parentNode.removeChild(this)
     }
     async _handleCopyApiKey() {
         var e;
-        q(this._apiKey), this._inputApiKeyBanner.style.setProperty("display", "flex"), await K(3e3), null === (e = this._inputApiKeyBanner) || void 0 === e || e.style.setProperty("display", "none")
+        K(this._apiKey), this._inputApiKeyBanner.style.setProperty("display", "flex"), await Y(3e3), null === (e = this._inputApiKeyBanner) || void 0 === e || e.style.setProperty("display", "none")
     }
 };
-me.styles = [P, k`
+he.styles = [P, z, k`
       :host {
         --mdc-dialog-max-width: 390px;
       }
       .center {
         text-align: center;
       }
       mwc-circular-progress {
@@ -1108,11 +1109,11 @@
       }
       .footer-left {
         position: absolute;
         left: 0;
         bottom: 4px;
         z-index: 1;
       }
-    `], o([r()], me.prototype, "_busy", void 0), o([r()], me.prototype, "_board", void 0), o([r()], me.prototype, "_useRecommended", void 0), o([r()], me.prototype, "_hasWifiSecrets", void 0), o([r()], me.prototype, "_writeProgress", void 0), o([r()], me.prototype, "_state", void 0), o([r()], me.prototype, "_error", void 0), o([i("mwc-textfield[name=name]")], me.prototype, "_inputName", void 0), o([i("mwc-textfield[name=ssid]")], me.prototype, "_inputSSID", void 0), o([i("mwc-textfield[name=password]")], me.prototype, "_inputPassword", void 0), o([i(".api-key-banner")], me.prototype, "_inputApiKeyBanner", void 0), me = o([_("esphome-wizard-dialog")], me);
+    `], o([r()], he.prototype, "_busy", void 0), o([r()], he.prototype, "_board", void 0), o([r()], he.prototype, "_useRecommended", void 0), o([r()], he.prototype, "_hasWifiSecrets", void 0), o([r()], he.prototype, "_writeProgress", void 0), o([r()], he.prototype, "_state", void 0), o([r()], he.prototype, "_error", void 0), o([i("mwc-textfield[name=name]")], he.prototype, "_inputName", void 0), o([i("mwc-textfield[name=ssid]")], he.prototype, "_inputSSID", void 0), o([i("mwc-textfield[name=password]")], he.prototype, "_inputPassword", void 0), o([i(".api-key-banner")], he.prototype, "_inputApiKeyBanner", void 0), he = o([_("esphome-wizard-dialog")], he);
 export {
-    me as ESPHomeWizardDialog
+    he as ESPHomeWizardDialog
 };
```

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.c74d5ae3.js` & `esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.c74d5ae3.js`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.db573db5.js` & `esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.90e5e76e.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -2,21 +2,21 @@
     r as t,
     b as o,
     d as e,
     l as s,
     n as i,
     s as n,
     y as r,
-    H as a
-} from "./index-d3dd97b9.js";
-import "./c.1bc018ae.js";
+    I as a
+} from "./index-bfcf9cd9.js";
+import "./c.22fb066b.js";
 import {
     o as l
-} from "./c.45f3bfa8.js";
-import "./c.e4466087.js";
+} from "./c.d861da54.js";
+import "./c.4971d925.js";
 let c = class extends n {
     render() {
         return r`
       <esphome-process-dialog
         .heading=${`Install ${this.configuration}`}
         .type=${"run"}
         .spawnParams=${{configuration:this.configuration,port:this.target}}
```

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.e1319253.js` & `esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.6951bded.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -2,25 +2,25 @@
     r as o,
     b as t,
     d as e,
     l as i,
     n as r,
     s,
     y as a,
-    Q as n
-} from "./index-d3dd97b9.js";
-import "./c.1bc018ae.js";
+    S as n
+} from "./index-bfcf9cd9.js";
+import "./c.22fb066b.js";
 import {
     o as c
-} from "./c.9e5eaea1.js";
-import "./c.e4466087.js";
-import "./c.7d2e85dd.js";
-import "./c.bff582f5.js";
-import "./c.e683a7a9.js";
-import "./c.45f3bfa8.js";
+} from "./c.3f59652f.js";
+import "./c.4971d925.js";
+import "./c.c84471ef.js";
+import "./c.17838855.js";
+import "./c.884f2894.js";
+import "./c.d861da54.js";
 let d = class extends s {
     constructor() {
         super(...arguments), this.downloadFactoryFirmware = !0
     }
     render() {
         return a`
       <esphome-process-dialog
```

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.e4466087.js` & `esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.4971d925.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -4,21 +4,21 @@
     M as i,
     b as o,
     i as n,
     d as a,
     o as d,
     B as r,
     g as s,
-    a2 as c,
-    a3 as l,
+    a3 as c,
+    a4 as l,
     y as m,
     f as u,
     r as h,
     n as g
-} from "./index-d3dd97b9.js";
+} from "./index-bfcf9cd9.js";
 (() => {
     var t, e, i;
     const o = Symbol(),
         n = Symbol(),
         a = Symbol(),
         d = Symbol(),
         r = Symbol(),
```

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.e683a7a9.js` & `esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.884f2894.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 import {
-    T as e
-} from "./index-d3dd97b9.js";
+    U as e
+} from "./index-bfcf9cd9.js";
 const a = "serial" in navigator,
     s = window.isSecureContext,
-    P = {
+    i = {
         ESP32: {
             label: "ESP32",
             showInPickerTitle: !0,
             defaultBoard: "esp32dev"
         },
         ESP32S2: {
             label: "ESP32-S2",
@@ -31,22 +31,22 @@
         },
         RP2040: {
             label: "Raspberry Pi Pico W",
             showInPickerTitle: !1,
             defaultBoard: "rpipicow"
         }
     },
-    S = {
+    l = {
         ESP32: "ESP32",
         "ESP32-S2": "ESP32S2",
         "ESP32-S3": "ESP32S3",
         "ESP32-C3": "ESP32C3",
         ESP8266: "ESP8266"
     },
-    i = e`
-  <svg width="24" height="24" viewBox="0 0 24 24" slot="meta">
+    P = e`
+  <svg class="svg-fill-primary" width="24" height="24" viewBox="0 0 24 24" slot="meta">
     <path d="M8.59,16.58L13.17,12L8.59,7.41L10,6L16,12L10,18L8.59,16.58Z" />
   </svg>
 `;
 export {
-    P as a, s as b, S as c, i as m, a as s
+    i as a, s as b, l as c, P as m, a as s
 };
```

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.e6db31ca.js` & `esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.25394cef.js`

 * *Files 15% similar despite different names*

#### js-beautify {}

```diff
@@ -1,58 +1,44 @@
 import {
-    b as o,
-    d as t,
+    b as e,
+    d as o,
     l as s,
-    n as e,
+    n as t,
     s as i,
-    y as r,
-    H as n
-} from "./index-d3dd97b9.js";
-import "./c.1bc018ae.js";
-import {
-    o as a
-} from "./c.61332c08.js";
-import "./c.e4466087.js";
-import "./c.7d2e85dd.js";
-import "./c.e683a7a9.js";
-let l = class extends i {
+    y as a,
+    a6 as n
+} from "./index-bfcf9cd9.js";
+import "./c.22fb066b.js";
+import "./c.4971d925.js";
+let r = class extends i {
     render() {
-        return r`
+        return a`
       <esphome-process-dialog
         always-show-close
-        .heading=${`Logs ${this.configuration}`}
-        .type=${"logs"}
-        .spawnParams=${{configuration:this.configuration,port:this.target}}
+        .heading=${`Rename ${this.configuration}`}
+        .type=${"rename"}
+        .spawnParams=${{configuration:this.configuration,newName:`${this.newName}`}}
         @closed=${this._handleClose}
         @process-done=${this._handleProcessDone}
       >
-        <mwc-button
-          slot="secondaryAction"
-          dialogAction="close"
-          label="Edit"
-          @click=${this._openEdit}
-        ></mwc-button>
-        ${void 0===this._result||0===this._result?"":r`
+        ${void 0===this._result||0===this._result?"":a`
               <mwc-button
                 slot="secondaryAction"
                 dialogAction="close"
                 label="Retry"
                 @click=${this._handleRetry}
               ></mwc-button>
             `}
       </esphome-process-dialog>
     `
     }
-    _openEdit() {
-        n(this.configuration)
-    }
-    _handleProcessDone(o) {
-        this._result = o.detail
+    _handleProcessDone(e) {
+        this._result = e.detail
     }
     _handleRetry() {
-        a(this.configuration, this.target)
+        n(this.configuration, this.newName)
     }
     _handleClose() {
         this.parentNode.removeChild(this)
     }
 };
-o([t()], l.prototype, "configuration", void 0), o([t()], l.prototype, "target", void 0), o([s()], l.prototype, "_result", void 0), l = o([e("esphome-logs-dialog")], l);
+e([o()], r.prototype, "configuration", void 0), e([o()], r.prototype, "newName", void 0), e([s()], r.prototype, "_result", void 0), r = e([t("esphome-rename-process-dialog")], r);
```

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/c.f4034d2e.js` & `esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/c.f4034d2e.js`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/js/esphome/index-d3dd97b9.js` & `esphome-dashboard-20230621.0/esphome_dashboard/static/js/esphome/index-bfcf9cd9.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1377,15 +1377,15 @@
     }),
     de = se((() => ne("./devices")), 5e3),
     le = () => {
         const t = de((() => {}));
         t.refresh(), t()
     },
     ce = () => {
-        import("./c.c2d1f4be.js"), document.body.append(document.createElement("esphome-wizard-dialog"))
+        import("./c.3bbbdf4b.js"), document.body.append(document.createElement("esphome-wizard-dialog"))
     },
     pe = Tt`:host{font-family:var(--mdc-icon-font, "Material Icons");font-weight:normal;font-style:normal;font-size:var(--mdc-icon-size, 24px);line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-smoothing:antialiased;text-rendering:optimizeLegibility;-moz-osx-font-smoothing:grayscale;font-feature-settings:"liga"}`;
 let he = class extends Ht {
     render() {
         return S`<span><slot></slot></span>`
     }
 };
@@ -9045,37 +9045,37 @@
         }
     },
     _removeListeners: function() {
         this._target && (this.unlisten(this._target, "mouseenter", "show"), this.unlisten(this._target, "focus", "show"), this.unlisten(this._target, "mouseleave", "hide"), this.unlisten(this._target, "blur", "hide"), this.unlisten(this._target, "tap", "hide")), this.unlisten(this.$.tooltip, "animationend", "_onAnimationEnd"), this.unlisten(this, "mouseenter", "hide")
     }
 });
 const Yd = t => {
-        import("./c.363ea4b9.js");
+        import("./c.9fa8c472.js");
         const e = document.createElement("esphome-clean-mqtt-dialog");
         e.configuration = t, document.body.append(e)
     },
     Wd = t => {
-        import("./c.734d4b21.js");
+        import("./c.b545a09c.js");
         const e = document.createElement("esphome-clean-dialog");
         e.configuration = t, document.body.append(e)
     },
     Xd = t => {
-        import("./c.52f07dd8.js");
+        import("./c.cce2f2f7.js");
         const e = document.createElement("esphome-validate-dialog");
         e.configuration = t, document.body.append(e)
     },
     Jd = t => {
-        import("./c.9e5eaea1.js").then((function(t) {
+        import("./c.3f59652f.js").then((function(t) {
             return t.i
         }));
         const e = document.createElement("esphome-install-choose-dialog");
         e.configuration = t, document.body.append(e)
     },
     Kd = t => {
-        import("./c.61332c08.js").then((function(t) {
+        import("./c.f0358a8b.js").then((function(t) {
             return t.l
         }));
         const e = document.createElement("esphome-logs-target-dialog");
         e.configuration = t, document.body.append(e)
     },
     Zd = (t, e, i, n) => {
         n = n || {};
@@ -9084,15 +9084,15 @@
             cancelable: Boolean(n.cancelable),
             composed: void 0 === n.composed || n.composed,
             detail: i
         });
         t.dispatchEvent(o)
     },
     Qd = (t, e, i) => {
-        import("./c.78cf8c6e.js");
+        import("./c.9d543f02.js");
         const n = document.createElement("esphome-delete-device-dialog");
         n.name = t, n.configuration = e, i && n.addEventListener("deleted", i), document.body.append(n)
     },
     tl = Tt`
   esphome-card {
     height: 100%;
     display: flex;
@@ -9102,38 +9102,29 @@
     color: var(--mdc-theme-primary);
   }
   .flex {
     flex: 1;
   }
   mwc-button {
     line-height: 1em;
+    --mdc-theme-primary: var(--primary-text-color);
   }
   .card-actions {
     display: flex;
     padding: 4px;
     align-items: center;
   }
   .card-actions a {
     text-decoration: none;
   }
-  .card-actions mwc-button {
-    --mdc-theme-primary: rgba(0, 0, 0, 0.88);
-  }
-  esphome-button-menu {
-    color: rgba(0, 0, 0, 0.88);
-  }
   .card-actions mwc-icon-button {
     --mdc-icon-button-size: 32px;
   }
 `,
     el = Tt`
-  :host {
-    --mdc-dialog-content-ink-color: #212121;
-  }
-
   a {
     color: var(--mdc-theme-primary);
   }
 
   a[slot="primaryAction"],
   a[slot="secondaryAction"] {
     text-decoration: none;
@@ -9172,16 +9163,16 @@
     font: inherit;
     text-align: left;
     text-decoration: underline;
     cursor: pointer;
   }
 
   mwc-button[no-attention] {
-    --mdc-theme-primary: #444;
-    --mdc-theme-on-primary: white;
+    --mdc-theme-primary: var(--mdc-theme-primary-no-attention);
+    --mdc-theme-on-primary: var(--mdc-theme-on-primary-no-attention);
   }
 
   @media only screen and (max-width: 450px) {
     mwc-dialog {
       --mdc-dialog-min-width: 100vw !important;
       --mdc-dialog-max-width: 100vw !important;
       --mdc-dialog-max-height: 100vh !important;
@@ -9194,60 +9185,69 @@
   mwc-list.platforms {
     margin: 0 -24px;
   }
 
   mwc-list.platforms mwc-list-item {
     padding: 0 24px;
   }
+
+  mwc-button {
+    --mdc-theme-primary: var(--primary-text-color);
+  }
+`,
+    il = Tt`
+  .svg-fill-primary {
+    fill: var(--primary-text-color);
+  }
 `,
-    il = (t, e) => {
-        import("./c.6d280f04.js");
+    nl = (t, e) => {
+        import("./c.64ac3748.js");
         const i = document.createElement("esphome-rename-dialog");
         i.configuration = t, i.suggestedName = e, document.body.append(i)
     },
-    nl = t => {
-        import("./c.b9286028.js");
+    ol = t => {
+        import("./c.9f55698d.js");
         const e = document.createElement("esphome-show-api-key-dialog");
         e.configuration = t, document.body.append(e)
     },
-    ol = t => {
+    rl = t => {
         Zd(document.body, "edit-file", t)
     },
-    rl = async t => {
+    sl = async t => {
         try {
             return ie(`./edit?configuration=${t}`)
         } catch (t) {
             if (t instanceof te && 404 === t.status) return null;
             throw t
         }
-    }, sl = async (t, e) => ie(`./edit?configuration=${t}`, {
+    }, al = async (t, e) => ie(`./edit?configuration=${t}`, {
         method: "POST",
         body: e
-    }), al = (t, e = "") => {
+    }), dl = (t, e = "") => {
         const i = new Blob([t], {
                 type: "text/plain"
             }),
             n = URL.createObjectURL(i);
         ((t, e = "") => {
             const i = document.createElement("a");
             i.target = "_blank", i.href = t, i.download = e, document.body.appendChild(i), i.dispatchEvent(new MouseEvent("click")), document.body.removeChild(i)
         })(n, e), setTimeout((() => URL.revokeObjectURL(n)), 0)
     };
-var dl = "M11,15H13V17H11V15M11,7H13V13H11V7M12,2C6.47,2 2,6.5 2,12A10,10 0 0,0 12,22A10,10 0 0,0 22,12A10,10 0 0,0 12,2M12,20A8,8 0 0,1 4,12A8,8 0 0,1 12,4A8,8 0 0,1 20,12A8,8 0 0,1 12,20Z",
-    ll = "M12,2L1,21H23M12,6L19.53,19H4.47M11,10V14H13V10M11,16V18H13V16",
-    cl = "M19.36,2.72L20.78,4.14L15.06,9.85C16.13,11.39 16.28,13.24 15.38,14.44L9.06,8.12C10.26,7.22 12.11,7.37 13.65,8.44L19.36,2.72M5.93,17.57C3.92,15.56 2.69,13.16 2.35,10.92L7.23,8.83L14.67,16.27L12.58,21.15C10.34,20.81 7.94,19.58 5.93,17.57Z",
-    pl = "M20,12A8,8 0 0,1 12,20A8,8 0 0,1 4,12A8,8 0 0,1 12,4C12.76,4 13.5,4.11 14.2,4.31L15.77,2.74C14.61,2.26 13.34,2 12,2A10,10 0 0,0 2,12A10,10 0 0,0 12,22A10,10 0 0,0 22,12M7.91,10.08L6.5,11.5L11,16L21,6L19.59,4.58L11,13.17L7.91,10.08Z",
-    hl = "M11,9H13V7H11M12,20C7.59,20 4,16.41 4,12C4,7.59 7.59,4 12,4C16.41,4 20,7.59 20,12C20,16.41 16.41,20 12,20M12,2A10,10 0 0,0 2,12A10,10 0 0,0 12,22A10,10 0 0,0 22,12A10,10 0 0,0 12,2M11,17H13V11H11V17Z";
-const ul = {
-    NEW: "rgb(255, 165, 0)",
+var ll = "M11,15H13V17H11V15M11,7H13V13H11V7M12,2C6.47,2 2,6.5 2,12A10,10 0 0,0 12,22A10,10 0 0,0 22,12A10,10 0 0,0 12,2M12,20A8,8 0 0,1 4,12A8,8 0 0,1 12,4A8,8 0 0,1 20,12A8,8 0 0,1 12,20Z",
+    cl = "M12,2L1,21H23M12,6L19.53,19H4.47M11,10V14H13V10M11,16V18H13V16",
+    pl = "M19.36,2.72L20.78,4.14L15.06,9.85C16.13,11.39 16.28,13.24 15.38,14.44L9.06,8.12C10.26,7.22 12.11,7.37 13.65,8.44L19.36,2.72M5.93,17.57C3.92,15.56 2.69,13.16 2.35,10.92L7.23,8.83L14.67,16.27L12.58,21.15C10.34,20.81 7.94,19.58 5.93,17.57Z",
+    hl = "M20,12A8,8 0 0,1 12,20A8,8 0 0,1 4,12A8,8 0 0,1 12,4C12.76,4 13.5,4.11 14.2,4.31L15.77,2.74C14.61,2.26 13.34,2 12,2A10,10 0 0,0 2,12A10,10 0 0,0 12,22A10,10 0 0,0 22,12M7.91,10.08L6.5,11.5L11,16L21,6L19.59,4.58L11,13.17L7.91,10.08Z",
+    ul = "M11,9H13V7H11M12,20C7.59,20 4,16.41 4,12C4,7.59 7.59,4 12,4C16.41,4 20,7.59 20,12C20,16.41 16.41,20 12,20M12,2A10,10 0 0,0 2,12A10,10 0 0,0 12,22A10,10 0 0,0 22,12A10,10 0 0,0 12,2M11,17H13V11H11V17Z";
+const ml = {
+    NEW: "var(--status-new)",
     OFFLINE: "var(--alert-error-color)",
     "UPDATE AVAILABLE": "var(--update-available-color)",
-    ONLINE: "rgba(0,0,0,.5)"
+    ONLINE: "var(--status-connected)"
 };
-let ml = class extends Ht {
+let fl = class extends Ht {
     constructor() {
         super(...arguments), this.highlightOnAdd = !1, this._highlight = !1
     }
     async highlight() {
         this._highlight = !0, await this.updateComplete, await this.shadowRoot.querySelector("esphome-card").getAttention(), await new Promise((t => setTimeout(t, 4e3))), this._highlight = !1
     }
     render() {
@@ -9264,15 +9264,15 @@
         const e = (i = this.device).current_version !== i.deployed_version;
         var i;
         const n = this._highlight ? "NEW" : !1 === this.onlineStatus ? "OFFLINE" : e ? "UPDATE AVAILABLE" : !0 === this.onlineStatus ? "ONLINE" : void 0;
         return S`
       <esphome-card
         .status=${n}
         .noStatusBar=${"ONLINE"===n}
-        style=${Re({"--status-color":void 0===n?"":ul[n]})}
+        style=${Re({"--status-color":void 0===n?"":ml[n]})}
       >
         <div class="card-header">
           ${this.device.friendly_name||this.device.name}
         </div>
 
         ${t.length?S`<div class="card-content flex">${t}</div>`:S`<div class="flex"></div>`}
 
@@ -9342,15 +9342,15 @@
                 .path=${"M18,17H10.5L12.5,15H18M6,17V14.5L13.88,6.65C14.07,6.45 14.39,6.45 14.59,6.65L16.35,8.41C16.55,8.61 16.55,8.92 16.35,9.12L8.47,17M19,3H5C3.89,3 3,3.89 3,5V19A2,2 0 0,0 5,21H19A2,2 0 0,0 21,19V5C21,3.89 20.1,3 19,3Z"}
               ></esphome-svg-icon>
             </mwc-list-item>
             <mwc-list-item graphic="icon">
               Clean Build Files
               <esphome-svg-icon
                 slot="graphic"
-                .path=${cl}
+                .path=${pl}
               ></esphome-svg-icon>
             </mwc-list-item>
             <li divider role="separator"></li>
             <mwc-list-item class="warning" graphic="icon">
               Delete
               <esphome-svg-icon
                 class="warning"
@@ -9358,15 +9358,15 @@
                 .path=${"M19,4H15.5L14.5,3H9.5L8.5,4H5V6H19M6,19A2,2 0 0,0 8,21H16A2,2 0 0,0 18,19V7H6V19Z"}
               ></esphome-svg-icon>
             </mwc-list-item>
             ${"mqtt"in this.device.loaded_integrations?S`<mwc-list-item graphic="icon">
                   Clean MQTT
                   <esphome-svg-icon
                     slot="graphic"
-                    .path=${cl}
+                    .path=${pl}
                   ></esphome-svg-icon>
                 </mwc-list-item>`:""}
           </esphome-button-menu>
         </div>
       </esphome-card>
     `
     }
@@ -9378,84 +9378,84 @@
             case 0:
                 Xd(this.device.configuration);
                 break;
             case 1:
                 this._handleInstall();
                 break;
             case 2:
-                nl(this.device.configuration);
+                ol(this.device.configuration);
                 break;
             case 3:
                 this._handleDownloadYaml();
                 break;
             case 4:
-                il(this.device.configuration, this.device.name);
+                nl(this.device.configuration, this.device.name);
                 break;
             case 5:
                 Wd(this.device.configuration);
                 break;
             case 6:
                 Qd(this.device.name, this.device.configuration, (() => Zd(this, "deleted")));
                 break;
             case 7:
                 Yd(this.device.configuration)
         }
     }
     _handleEdit() {
-        ol(this.device.configuration)
+        rl(this.device.configuration)
     }
     _handleInstall() {
         Jd(this.device.configuration)
     }
     _handleLogs() {
         Kd(this.device.configuration)
     }
     async _handleDownloadYaml() {
-        rl(this.device.configuration).then((t => {
-            al(t, this.device.configuration)
+        sl(this.device.configuration).then((t => {
+            dl(t, this.device.configuration)
         }))
     }
 };
-ml.styles = [tl, Tt`
-      :host {
-        --update-available-color: #2e3dd4;
-      }
+fl.styles = [tl, Tt`
       .device-config-path {
         margin-bottom: 8px;
         font-size: 14px;
       }
       .inlinecode {
         box-sizing: border-box;
         padding: 0.2em 0.4em;
         margin: 0;
         font-size: 85%;
-        background-color: rgba(27, 31, 35, 0.05);
+        background-color: var(--card-background-color)
         border-radius: 3px;
         font-family: "SFMono-Regular", Consolas, "Liberation Mono", Menlo,
           Courier, monospace;
       }
       .card-actions mwc-button.update-available {
         --mdc-theme-primary: var(--update-available-color);
       }
       esphome-button-menu {
-        --mdc-theme-text-icon-on-background: rgba(0, 0, 0, 0.56);
+        --mdc-theme-text-icon-on-background: var(--primary-text-color);
       }
       .tooltip-container {
         display: inline-block;
       }
       .warning {
         color: var(--alert-error-color);
       }
-    `], r([jt()], ml.prototype, "device", void 0), r([jt()], ml.prototype, "onlineStatus", void 0), r([jt()], ml.prototype, "highlightOnAdd", void 0), r([Vt()], ml.prototype, "_highlight", void 0), ml = r([Bt("esphome-configured-device-card")], ml);
-const fl = (t, e) => {
-    import("./c.1c31574e.js");
+      .mdc-icon-button {
+        color: var(--primary-text-color);
+      }
+    `], r([jt()], fl.prototype, "device", void 0), r([jt()], fl.prototype, "onlineStatus", void 0), r([jt()], fl.prototype, "highlightOnAdd", void 0), r([Vt()], fl.prototype, "_highlight", void 0), fl = r([Bt("esphome-configured-device-card")], fl);
+const _l = (t, e) => {
+    import("./c.fadc3045.js");
     const i = document.createElement("esphome-adopt-dialog");
     i.device = t, i.addEventListener("adopted", e), document.body.append(i)
 };
-let _l = class extends Ht {
+let gl = class extends Ht {
     constructor() {
         super(...arguments), this.highlightOnAdd = !1
     }
     render() {
         return S`
       <esphome-card status="DISCOVERED">
         <div class="card-header">
@@ -9482,55 +9482,55 @@
     }
     firstUpdated(t) {
         super.firstUpdated(t), this.highlightOnAdd && setTimeout((() => {
             this.shadowRoot.querySelector("esphome-card").getAttention()
         }), 1e3)
     }
     async _handleAdopt() {
-        fl(this.device, (() => Zd(this, "adopted")))
+        _l(this.device, (() => Zd(this, "adopted")))
     }
 };
-_l.styles = [tl, Tt`
+gl.styles = [tl, Tt`
       esphome-card {
-        --status-color: #4caf50;
+        --status-color: var(--status-imported);
       }
       .inlinecode {
         box-sizing: border-box;
         padding: 0.2em 0.4em;
         margin: 0;
         font-size: 85%;
         background-color: rgba(27, 31, 35, 0.05);
         border-radius: 3px;
         font-family: "SFMono-Regular", Consolas, "Liberation Mono", Menlo,
           Courier, monospace;
       }
       .card-actions mwc-button {
         --mdc-theme-primary: #4caf50;
       }
-    `], r([jt()], _l.prototype, "device", void 0), r([jt()], _l.prototype, "highlightOnAdd", void 0), _l = r([Bt("esphome-importable-device-card")], _l);
-const gl = t => ne("./wizard", {
+    `], r([jt()], gl.prototype, "device", void 0), r([jt()], gl.prototype, "highlightOnAdd", void 0), gl = r([Bt("esphome-importable-device-card")], gl);
+const bl = t => ne("./wizard", {
         method: "post",
         body: JSON.stringify(t)
     }),
-    bl = t => ne(`./info?configuration=${t}`),
-    yl = t => ie(`./delete?configuration=${t}`, {
+    yl = t => ne(`./info?configuration=${t}`),
+    vl = t => ie(`./delete?configuration=${t}`, {
         method: "post"
     }),
-    vl = (t, e) => re("compile", {
+    xl = (t, e) => re("compile", {
         configuration: t
     }, void 0, e),
-    xl = (t, e) => re("compile", {
+    wl = (t, e) => re("compile", {
         configuration: t,
         only_generate: !0
     }, void 0, e),
-    wl = (t, e) => {
+    Cl = (t, e) => {
         let i = `./download.bin?configuration=${encodeURIComponent(t)}`;
         return e && (i += "&type=firmware-factory.bin"), i
     },
-    Cl = async t => {
+    Al = async t => {
         var e, i;
         let n;
         try {
             n = await (async t => {
                 try {
                     return ne(`./json-config?configuration=${t}`)
                 } catch (t) {
@@ -9539,36 +9539,36 @@
                 }
             })(t)
         } catch {
             return null
         }
         return (null === (i = null === (e = null == n ? void 0 : n.api) || void 0 === e ? void 0 : e.encryption) || void 0 === i ? void 0 : i.key) || null
     };
-class Al {
+class El {
     constructor() {
         this.toRefresh = [], this.compileFailed = new Set, this.running = !1
     }
     add(t) {
         this.compileFailed.has(t) || (this.toRefresh.push(t), this.running || (this.running = !0, this.run()))
     }
     async run() {
         for (; this.toRefresh.length;) {
             const t = this.toRefresh.shift();
             try {
-                await xl(t)
+                await wl(t)
             } catch (e) {
                 this.compileFailed.add(t)
             }
         }
         this.running = !1
     }
 }
-let El = class extends Ht {
+let Sl = class extends Ht {
     constructor() {
-        super(...arguments), this._highlightOnAdd = !1, this._metadataRefresher = new Al
+        super(...arguments), this._highlightOnAdd = !1, this._metadataRefresher = new El
     }
     render() {
         if (void 0 === this._devices) return S``;
         if (0 === this._devices.configured.length && 0 === this._devices.importable.length) return S`
         <div class="welcome-container">
           <h5>Welcome to ESPHome</h5>
           <p>It looks like you don't yet have any devices.</p>
@@ -9636,15 +9636,15 @@
             this._onlineStatus = t
         }))
     }
     disconnectedCallback() {
         super.disconnectedCallback(), this._devicesUnsub && this._devicesUnsub(), this._onlineStatusUnsub && this._onlineStatusUnsub()
     }
 };
-El.styles = Tt`
+Sl.styles = Tt`
     .grid {
       display: grid;
       grid-template-columns: 1fr;
       grid-template-columns: 1fr 1fr 1fr;
       grid-column-gap: 1.5rem;
       margin: 20px auto;
       width: 90%;
@@ -9680,45 +9680,42 @@
       font-weight: 400;
       margin: 1rem 0 0.65rem 0;
     }
     hr {
       margin-top: 16px;
       margin-bottom: 16px;
     }
-    mwc-button {
-      --mdc-theme-primary: #4caf50;
-    }
-  `, r([Vt()], El.prototype, "_devices", void 0), r([Vt()], El.prototype, "_onlineStatus", void 0), El = r([Bt("esphome-devices-list")], El);
-const Sl = "secrets.yaml",
-    Tl = async () => {
+  `, r([Vt()], Sl.prototype, "_devices", void 0), r([Vt()], Sl.prototype, "_onlineStatus", void 0), Sl = r([Bt("esphome-devices-list")], Sl);
+const Tl = "secrets.yaml",
+    Pl = async () => {
         try {
             return await ne("./secret_keys")
         } catch (t) {
             if (t instanceof te && 404 === t.status) return [];
             throw t
         }
-    }, Pl = async (t, e) => {
-        let i = await rl(Sl);
+    }, Ol = async (t, e) => {
+        let i = await sl(Tl);
         null === i && (i = "");
         let n = 0 === i.length ? "" : "\n" !== i.charAt(i.length - 1) ? "\n\n" : "\n";
         e && (n += `# ${e}\n`);
         for (const [e, i] of Object.entries(t)) n += `${e}: ${JSON.stringify(i)}\n`;
-        await sl(Sl, i + n)
-    }, Ol = () => {
-        import("./c.d408ba9c.js"), document.body.append(document.createElement("esphome-update-all-dialog"))
-    }, Il = t => new Promise((e => {
-        import("./c.a613b168.js").then((() => {
+        await al(Tl, i + n)
+    }, Il = () => {
+        import("./c.1fccc3bb.js"), document.body.append(document.createElement("esphome-update-all-dialog"))
+    }, Rl = t => new Promise((e => {
+        import("./c.670cd819.js").then((() => {
             const i = document.createElement("esphome-confirmation-dialog");
             document.body.append(i), i.showDialog(t, e)
         }))
-    })), Rl = window.matchMedia("(min-width: 601px)");
-let kl = class extends Ht {
+    })), kl = window.matchMedia("(min-width: 641px)");
+let Nl = class extends Ht {
     constructor() {
-        super(...arguments), this._isWide = Rl.matches, this._isWideUpdated = () => {
-            this._isWide = Rl.matches
+        super(...arguments), this._isWide = kl.matches, this._isWideUpdated = () => {
+            this._isWide = kl.matches
         }
     }
     render() {
         return this._isWide ? S`
         <mwc-button
           icon="system_update"
           label="Update All"
@@ -9736,69 +9733,77 @@
             `:""}
       ` : S`
       <esphome-button-menu
         corner="BOTTOM_START"
         @action=${this._handleOverflowAction}
       >
         <mwc-icon-button slot="trigger" icon="more_vert"></mwc-icon-button>
-        <mwc-list-item>Update All</mwc-list-item>
-        <mwc-list-item>Secrets Editor</mwc-list-item>
+        <mwc-list-item graphic="icon"
+          ><mwc-icon slot="graphic">system_update</mwc-icon>Update
+          All</mwc-list-item
+        >
+        <mwc-list-item graphic="icon"
+          ><mwc-icon slot="graphic">lock</mwc-icon>Secrets Editor</mwc-list-item
+        >
         ${this.logoutUrl?S`
               <a href=${this.logoutUrl}
                 ><mwc-list-item>Log Out</mwc-list-item></a
               >
             `:""}
         <slot></slot>
       </esphome-button-menu>
     `
     }
     connectedCallback() {
-        super.connectedCallback(), Rl.addEventListener("change", this._isWideUpdated)
+        super.connectedCallback(), kl.addEventListener("change", this._isWideUpdated)
     }
     disconnectedCallback() {
-        super.disconnectedCallback(), Rl.removeEventListener("change", this._isWideUpdated)
+        super.disconnectedCallback(), kl.removeEventListener("change", this._isWideUpdated)
     }
     async _handleUpdateAll() {
-        await Il({
+        await Rl({
             title: "Update All",
             text: "Do you want to update all devices?",
             confirmText: "Update All",
             dismissText: "Cancel"
-        }) && Ol()
+        }) && Il()
     }
     _handleEditSecrets() {
-        ol(Sl)
+        rl(Tl)
     }
     async _handleOverflowAction(t) {
         switch (t.detail.index) {
             case 0:
                 this._handleUpdateAll();
                 break;
             case 1:
                 this._handleEditSecrets()
         }
     }
 };
-kl.styles = Tt`
+Nl.styles = Tt`
     esphome-button-menu {
       z-index: 1;
     }
     mwc-button {
-      --mdc-theme-primary: black;
+      --mdc-theme-primary: var(--primary-text-color);
       margin-left: 16px;
       line-height: 1em;
     }
+    mwc-icon {
+      --mdc-theme-text-icon-on-background: var(--primary-text-color);
+    }
     a {
       text-decoration: none;
     }
   `, r([jt({
     type: String,
     attribute: "logout-url"
-})], kl.prototype, "logoutUrl", void 0), r([Vt()], kl.prototype, "_isWide", void 0), kl = r([Bt("esphome-header-menu")], kl);
-class Nl extends Ht {
+})], Nl.prototype, "logoutUrl", void 0), r([Vt()], Nl.prototype, "_isWide", void 0), Nl = r([Bt("esphome-header-menu")], Nl);
+class $l extends Ht {
     constructor() {
         super(...arguments), this.mini = !1, this.exited = !1, this.disabled = !1, this.extended = !1, this.showIconAtEnd = !1, this.reducedTouchTarget = !1, this.icon = "", this.label = "", this.shouldRenderRipple = !1, this.useStateLayerCustomProperties = !1, this.rippleHandlers = new Le((() => (this.shouldRenderRipple = !0, this.ripple)))
     }
     render() {
         const t = this.mini && !this.reducedTouchTarget,
             e = {
                 "mdc-fab--mini": this.mini,
@@ -9870,60 +9875,60 @@
     handleRippleFocus() {
         this.rippleHandlers.startFocus()
     }
     handleRippleBlur() {
         this.rippleHandlers.endFocus()
     }
 }
-Nl.shadowRootOptions = {
+$l.shadowRootOptions = {
     mode: "open",
     delegatesFocus: !0
-}, r([Wt("mwc-ripple")], Nl.prototype, "ripple", void 0), r([jt({
+}, r([Wt("mwc-ripple")], $l.prototype, "ripple", void 0), r([jt({
     type: Boolean
-})], Nl.prototype, "mini", void 0), r([jt({
+})], $l.prototype, "mini", void 0), r([jt({
     type: Boolean
-})], Nl.prototype, "exited", void 0), r([jt({
+})], $l.prototype, "exited", void 0), r([jt({
     type: Boolean
-})], Nl.prototype, "disabled", void 0), r([jt({
+})], $l.prototype, "disabled", void 0), r([jt({
     type: Boolean
-})], Nl.prototype, "extended", void 0), r([jt({
+})], $l.prototype, "extended", void 0), r([jt({
     type: Boolean
-})], Nl.prototype, "showIconAtEnd", void 0), r([jt({
+})], $l.prototype, "showIconAtEnd", void 0), r([jt({
     type: Boolean
-})], Nl.prototype, "reducedTouchTarget", void 0), r([jt()], Nl.prototype, "icon", void 0), r([jt()], Nl.prototype, "label", void 0), r([Vt()], Nl.prototype, "shouldRenderRipple", void 0), r([Vt()], Nl.prototype, "useStateLayerCustomProperties", void 0), r([Gt({
+})], $l.prototype, "reducedTouchTarget", void 0), r([jt()], $l.prototype, "icon", void 0), r([jt()], $l.prototype, "label", void 0), r([Vt()], $l.prototype, "shouldRenderRipple", void 0), r([Vt()], $l.prototype, "useStateLayerCustomProperties", void 0), r([Gt({
     passive: !0
-})], Nl.prototype, "handleRippleStartPress", null);
-const $l = Tt`:host .mdc-fab .material-icons{font-family:var(--mdc-icon-font, "Material Icons");font-weight:normal;font-style:normal;font-size:var(--mdc-icon-size, 24px);line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-smoothing:antialiased;text-rendering:optimizeLegibility;-moz-osx-font-smoothing:grayscale;font-feature-settings:"liga"}:host{outline:none;--mdc-ripple-color: currentcolor;user-select:none;-webkit-tap-highlight-color:transparent;display:inline-flex;-webkit-tap-highlight-color:transparent;display:inline-flex;outline:none;user-select:none}:host .mdc-touch-target-wrapper{display:inline}:host .mdc-elevation-overlay{position:absolute;border-radius:inherit;pointer-events:none;opacity:0;opacity:var(--mdc-elevation-overlay-opacity, 0);transition:opacity 280ms cubic-bezier(0.4, 0, 0.2, 1);background-color:#fff;background-color:var(--mdc-elevation-overlay-color, #fff)}:host .mdc-fab{position:relative;display:inline-flex;position:relative;align-items:center;justify-content:center;box-sizing:border-box;width:56px;height:56px;padding:0;border:none;fill:currentColor;text-decoration:none;cursor:pointer;user-select:none;-moz-appearance:none;-webkit-appearance:none;overflow:visible;transition:box-shadow 280ms cubic-bezier(0.4, 0, 0.2, 1),opacity 15ms linear 30ms,transform 270ms 0ms cubic-bezier(0, 0, 0.2, 1)}:host .mdc-fab .mdc-elevation-overlay{width:100%;height:100%;top:0;left:0}:host .mdc-fab::-moz-focus-inner{padding:0;border:0}:host .mdc-fab:hover{box-shadow:0px 5px 5px -3px rgba(0, 0, 0, 0.2),0px 8px 10px 1px rgba(0, 0, 0, 0.14),0px 3px 14px 2px rgba(0,0,0,.12)}:host .mdc-fab.mdc-ripple-upgraded--background-focused,:host .mdc-fab:not(.mdc-ripple-upgraded):focus{box-shadow:0px 5px 5px -3px rgba(0, 0, 0, 0.2),0px 8px 10px 1px rgba(0, 0, 0, 0.14),0px 3px 14px 2px rgba(0,0,0,.12)}:host .mdc-fab .mdc-fab__focus-ring{position:absolute}:host .mdc-fab.mdc-ripple-upgraded--background-focused .mdc-fab__focus-ring,:host .mdc-fab:not(.mdc-ripple-upgraded):focus .mdc-fab__focus-ring{pointer-events:none;border:2px solid transparent;border-radius:6px;box-sizing:content-box;position:absolute;top:50%;left:50%;transform:translate(-50%, -50%);height:calc( 100% + 4px );width:calc( 100% + 4px )}@media screen and (forced-colors: active){:host .mdc-fab.mdc-ripple-upgraded--background-focused .mdc-fab__focus-ring,:host .mdc-fab:not(.mdc-ripple-upgraded):focus .mdc-fab__focus-ring{border-color:CanvasText}}:host .mdc-fab.mdc-ripple-upgraded--background-focused .mdc-fab__focus-ring::after,:host .mdc-fab:not(.mdc-ripple-upgraded):focus .mdc-fab__focus-ring::after{content:"";border:2px solid transparent;border-radius:8px;display:block;position:absolute;top:50%;left:50%;transform:translate(-50%, -50%);height:calc(100% + 4px);width:calc(100% + 4px)}@media screen and (forced-colors: active){:host .mdc-fab.mdc-ripple-upgraded--background-focused .mdc-fab__focus-ring::after,:host .mdc-fab:not(.mdc-ripple-upgraded):focus .mdc-fab__focus-ring::after{border-color:CanvasText}}:host .mdc-fab:active,:host .mdc-fab:focus:active{box-shadow:0px 7px 8px -4px rgba(0, 0, 0, 0.2),0px 12px 17px 2px rgba(0, 0, 0, 0.14),0px 5px 22px 4px rgba(0,0,0,.12)}:host .mdc-fab:active,:host .mdc-fab:focus{outline:none}:host .mdc-fab:hover{cursor:pointer}:host .mdc-fab>svg{width:100%}:host .mdc-fab--mini{width:40px;height:40px}:host .mdc-fab--extended{-moz-osx-font-smoothing:grayscale;-webkit-font-smoothing:antialiased;font-family:Roboto, sans-serif;font-family:var(--mdc-typography-button-font-family, var(--mdc-typography-font-family, Roboto, sans-serif));font-size:0.875rem;font-size:var(--mdc-typography-button-font-size, 0.875rem);line-height:2.25rem;line-height:var(--mdc-typography-button-line-height, 2.25rem);font-weight:500;font-weight:var(--mdc-typography-button-font-weight, 500);letter-spacing:0.0892857143em;letter-spacing:var(--mdc-typography-button-letter-spacing, 0.0892857143em);text-decoration:none;text-decoration:var(--mdc-typography-button-text-decoration, none);text-transform:uppercase;text-transform:var(--mdc-typography-button-text-transform, uppercase);border-radius:24px;padding-left:20px;padding-right:20px;width:auto;max-width:100%;height:48px;line-height:normal}:host .mdc-fab--extended .mdc-fab__ripple{border-radius:24px}:host .mdc-fab--extended .mdc-fab__icon{margin-left:calc(12px - 20px);margin-right:12px}[dir=rtl] :host .mdc-fab--extended .mdc-fab__icon,:host .mdc-fab--extended .mdc-fab__icon[dir=rtl]{margin-left:12px;margin-right:calc(12px - 20px)}:host .mdc-fab--extended .mdc-fab__label+.mdc-fab__icon{margin-left:12px;margin-right:calc(12px - 20px)}[dir=rtl] :host .mdc-fab--extended .mdc-fab__label+.mdc-fab__icon,:host .mdc-fab--extended .mdc-fab__label+.mdc-fab__icon[dir=rtl]{margin-left:calc(12px - 20px);margin-right:12px}:host .mdc-fab--touch{margin-top:4px;margin-bottom:4px;margin-right:4px;margin-left:4px}:host .mdc-fab--touch .mdc-fab__touch{position:absolute;top:50%;height:48px;left:50%;width:48px;transform:translate(-50%, -50%)}:host .mdc-fab::before{position:absolute;box-sizing:border-box;width:100%;height:100%;top:0;left:0;border:1px solid transparent;border-radius:inherit;content:"";pointer-events:none}@media screen and (forced-colors: active){:host .mdc-fab::before{border-color:CanvasText}}:host .mdc-fab__label{justify-content:flex-start;text-overflow:ellipsis;white-space:nowrap;overflow-x:hidden;overflow-y:visible}:host .mdc-fab__icon{transition:transform 180ms 90ms cubic-bezier(0, 0, 0.2, 1);fill:currentColor;will-change:transform}:host .mdc-fab .mdc-fab__icon{display:inline-flex;align-items:center;justify-content:center}:host .mdc-fab--exited{transform:scale(0);opacity:0;transition:opacity 15ms linear 150ms,transform 180ms 0ms cubic-bezier(0.4, 0, 1, 1)}:host .mdc-fab--exited .mdc-fab__icon{transform:scale(0);transition:transform 135ms 0ms cubic-bezier(0.4, 0, 1, 1)}:host .mdc-fab{background-color:#018786;background-color:var(--mdc-theme-secondary, #018786);box-shadow:0px 3px 5px -1px rgba(0, 0, 0, 0.2),0px 6px 10px 0px rgba(0, 0, 0, 0.14),0px 1px 18px 0px rgba(0,0,0,.12)}:host .mdc-fab .mdc-fab__icon{width:24px;height:24px;font-size:24px}:host .mdc-fab,:host .mdc-fab:not(:disabled) .mdc-fab__icon,:host .mdc-fab:not(:disabled) .mdc-fab__label,:host .mdc-fab:disabled .mdc-fab__icon,:host .mdc-fab:disabled .mdc-fab__label{color:#fff;color:var(--mdc-theme-on-secondary, #fff)}:host .mdc-fab:not(.mdc-fab--extended){border-radius:50%}:host .mdc-fab:not(.mdc-fab--extended) .mdc-fab__ripple{border-radius:50%}:host .mdc-fab{position:relative;display:inline-flex;position:relative;align-items:center;justify-content:center;box-sizing:border-box;width:56px;height:56px;padding:0;border:none;fill:currentColor;text-decoration:none;cursor:pointer;user-select:none;-moz-appearance:none;-webkit-appearance:none;overflow:visible;transition:box-shadow 280ms cubic-bezier(0.4, 0, 0.2, 1),opacity 15ms linear 30ms,transform 270ms 0ms cubic-bezier(0, 0, 0.2, 1)}:host .mdc-fab .mdc-elevation-overlay{width:100%;height:100%;top:0;left:0}:host .mdc-fab::-moz-focus-inner{padding:0;border:0}:host .mdc-fab:hover{box-shadow:0px 5px 5px -3px rgba(0, 0, 0, 0.2),0px 8px 10px 1px rgba(0, 0, 0, 0.14),0px 3px 14px 2px rgba(0,0,0,.12)}:host .mdc-fab.mdc-ripple-upgraded--background-focused,:host .mdc-fab:not(.mdc-ripple-upgraded):focus{box-shadow:0px 5px 5px -3px rgba(0, 0, 0, 0.2),0px 8px 10px 1px rgba(0, 0, 0, 0.14),0px 3px 14px 2px rgba(0,0,0,.12)}:host .mdc-fab .mdc-fab__focus-ring{position:absolute}:host .mdc-fab.mdc-ripple-upgraded--background-focused .mdc-fab__focus-ring,:host .mdc-fab:not(.mdc-ripple-upgraded):focus .mdc-fab__focus-ring{pointer-events:none;border:2px solid transparent;border-radius:6px;box-sizing:content-box;position:absolute;top:50%;left:50%;transform:translate(-50%, -50%);height:calc( 100% + 4px );width:calc( 100% + 4px )}@media screen and (forced-colors: active){:host .mdc-fab.mdc-ripple-upgraded--background-focused .mdc-fab__focus-ring,:host .mdc-fab:not(.mdc-ripple-upgraded):focus .mdc-fab__focus-ring{border-color:CanvasText}}:host .mdc-fab.mdc-ripple-upgraded--background-focused .mdc-fab__focus-ring::after,:host .mdc-fab:not(.mdc-ripple-upgraded):focus .mdc-fab__focus-ring::after{content:"";border:2px solid transparent;border-radius:8px;display:block;position:absolute;top:50%;left:50%;transform:translate(-50%, -50%);height:calc(100% + 4px);width:calc(100% + 4px)}@media screen and (forced-colors: active){:host .mdc-fab.mdc-ripple-upgraded--background-focused .mdc-fab__focus-ring::after,:host .mdc-fab:not(.mdc-ripple-upgraded):focus .mdc-fab__focus-ring::after{border-color:CanvasText}}:host .mdc-fab:active,:host .mdc-fab:focus:active{box-shadow:0px 7px 8px -4px rgba(0, 0, 0, 0.2),0px 12px 17px 2px rgba(0, 0, 0, 0.14),0px 5px 22px 4px rgba(0,0,0,.12)}:host .mdc-fab:active,:host .mdc-fab:focus{outline:none}:host .mdc-fab:hover{cursor:pointer}:host .mdc-fab>svg{width:100%}:host .mdc-fab--mini{width:40px;height:40px}:host .mdc-fab--extended{-moz-osx-font-smoothing:grayscale;-webkit-font-smoothing:antialiased;font-family:Roboto, sans-serif;font-family:var(--mdc-typography-button-font-family, var(--mdc-typography-font-family, Roboto, sans-serif));font-size:0.875rem;font-size:var(--mdc-typography-button-font-size, 0.875rem);line-height:2.25rem;line-height:var(--mdc-typography-button-line-height, 2.25rem);font-weight:500;font-weight:var(--mdc-typography-button-font-weight, 500);letter-spacing:0.0892857143em;letter-spacing:var(--mdc-typography-button-letter-spacing, 0.0892857143em);text-decoration:none;text-decoration:var(--mdc-typography-button-text-decoration, none);text-transform:uppercase;text-transform:var(--mdc-typography-button-text-transform, uppercase);border-radius:24px;padding-left:20px;padding-right:20px;width:auto;max-width:100%;height:48px;line-height:normal}:host .mdc-fab--extended .mdc-fab__ripple{border-radius:24px}:host .mdc-fab--extended .mdc-fab__icon{margin-left:calc(12px - 20px);margin-right:12px}[dir=rtl] :host .mdc-fab--extended .mdc-fab__icon,:host .mdc-fab--extended .mdc-fab__icon[dir=rtl]{margin-left:12px;margin-right:calc(12px - 20px)}:host .mdc-fab--extended .mdc-fab__label+.mdc-fab__icon{margin-left:12px;margin-right:calc(12px - 20px)}[dir=rtl] :host .mdc-fab--extended .mdc-fab__label+.mdc-fab__icon,:host .mdc-fab--extended .mdc-fab__label+.mdc-fab__icon[dir=rtl]{margin-left:calc(12px - 20px);margin-right:12px}:host .mdc-fab--touch{margin-top:4px;margin-bottom:4px;margin-right:4px;margin-left:4px}:host .mdc-fab--touch .mdc-fab__touch{position:absolute;top:50%;height:48px;left:50%;width:48px;transform:translate(-50%, -50%)}:host .mdc-fab::before{position:absolute;box-sizing:border-box;width:100%;height:100%;top:0;left:0;border:1px solid transparent;border-radius:inherit;content:"";pointer-events:none}@media screen and (forced-colors: active){:host .mdc-fab::before{border-color:CanvasText}}:host .mdc-fab__label{justify-content:flex-start;text-overflow:ellipsis;white-space:nowrap;overflow-x:hidden;overflow-y:visible}:host .mdc-fab__icon{transition:transform 180ms 90ms cubic-bezier(0, 0, 0.2, 1);fill:currentColor;will-change:transform}:host .mdc-fab .mdc-fab__icon{display:inline-flex;align-items:center;justify-content:center}:host .mdc-fab--exited{transform:scale(0);opacity:0;transition:opacity 15ms linear 150ms,transform 180ms 0ms cubic-bezier(0.4, 0, 1, 1)}:host .mdc-fab--exited .mdc-fab__icon{transform:scale(0);transition:transform 135ms 0ms cubic-bezier(0.4, 0, 1, 1)}:host .mdc-fab .ripple{overflow:hidden}:host .mdc-fab:not(.mdc-fab--extended) .ripple{border-radius:50%}:host .mdc-fab.mdc-fab--extended .ripple{border-radius:24px}:host .mdc-fab .mdc-fab__label{z-index:0}:host .mdc-fab .mdc-fab__icon ::slotted(*){width:inherit;height:inherit;font-size:inherit}:host .mdc-fab--extended.mdc-fab--exited .mdc-fab__icon ::slotted(*){transform:scale(0);transition:transform 135ms 0ms cubic-bezier(0.4, 0, 1, 1)}:host .mdc-fab{padding-top:0px;padding-top:max(0px, var(--mdc-fab-focus-outline-width, 0px));padding-right:0px;padding-right:max(0px, var(--mdc-fab-focus-outline-width, 0px));padding-bottom:0px;padding-bottom:max(0px, var(--mdc-fab-focus-outline-width, 0px));padding-left:0px;padding-left:max(0px, var(--mdc-fab-focus-outline-width, 0px));box-shadow:0px 3px 5px -1px rgba(0, 0, 0, 0.2), 0px 6px 10px 0px rgba(0, 0, 0, 0.14), 0px 1px 18px 0px rgba(0, 0, 0, 0.12);box-shadow:var(--mdc-fab-box-shadow, 0px 3px 5px -1px rgba(0, 0, 0, 0.2), 0px 6px 10px 0px rgba(0, 0, 0, 0.14), 0px 1px 18px 0px rgba(0, 0, 0, 0.12))}:host .mdc-fab:not(:disabled).mdc-ripple-upgraded--background-focused,:host .mdc-fab:not(:disabled):not(.mdc-ripple-upgraded):focus{border-color:initial;border-color:var(--mdc-fab-focus-outline-color, initial)}:host .mdc-fab:not(:disabled).mdc-ripple-upgraded--background-focused,:host .mdc-fab:not(:disabled):not(.mdc-ripple-upgraded):focus{border-style:solid;border-width:var(--mdc-fab-focus-outline-width, 0px);padding-top:0px;padding-top:max(calc(0px - var(--mdc-fab-focus-outline-width, 0px)), calc(calc(0px - var(--mdc-fab-focus-outline-width, 0px)) * -1));padding-right:0px;padding-right:max(calc(0px - var(--mdc-fab-focus-outline-width, 0px)), calc(calc(0px - var(--mdc-fab-focus-outline-width, 0px)) * -1));padding-bottom:0px;padding-bottom:max(calc(0px - var(--mdc-fab-focus-outline-width, 0px)), calc(calc(0px - var(--mdc-fab-focus-outline-width, 0px)) * -1));padding-left:0px;padding-left:max(calc(0px - var(--mdc-fab-focus-outline-width, 0px)), calc(calc(0px - var(--mdc-fab-focus-outline-width, 0px)) * -1))}:host .mdc-fab:hover,:host .mdc-fab:focus{box-shadow:0px 5px 5px -3px rgba(0, 0, 0, 0.2), 0px 8px 10px 1px rgba(0, 0, 0, 0.14), 0px 3px 14px 2px rgba(0, 0, 0, 0.12);box-shadow:var(--mdc-fab-box-shadow, 0px 5px 5px -3px rgba(0, 0, 0, 0.2), 0px 8px 10px 1px rgba(0, 0, 0, 0.14), 0px 3px 14px 2px rgba(0, 0, 0, 0.12))}:host .mdc-fab:active{box-shadow:0px 7px 8px -4px rgba(0, 0, 0, 0.2), 0px 12px 17px 2px rgba(0, 0, 0, 0.14), 0px 5px 22px 4px rgba(0, 0, 0, 0.12);box-shadow:var(--mdc-fab-box-shadow, 0px 7px 8px -4px rgba(0, 0, 0, 0.2), 0px 12px 17px 2px rgba(0, 0, 0, 0.14), 0px 5px 22px 4px rgba(0, 0, 0, 0.12))}:host .mdc-fab .ripple{overflow:hidden}:host .mdc-fab .mdc-fab__label{z-index:0}:host .mdc-fab:not(.mdc-fab--extended) .ripple{border-radius:50%}:host .mdc-fab.mdc-fab--extended .ripple{border-radius:24px}:host .mdc-fab .mdc-fab__icon{width:24px;width:var(--mdc-icon-size, 24px);height:24px;height:var(--mdc-icon-size, 24px);font-size:24px;font-size:var(--mdc-icon-size, 24px);transition:transform 180ms 90ms cubic-bezier(0, 0, 0.2, 1);fill:currentColor;will-change:transform;display:inline-flex;align-items:center;justify-content:center}:host .mdc-fab.mdc-fab--extended{padding-top:0px;padding-top:max(0px, var(--mdc-fab-focus-outline-width, 0px));padding-right:20px;padding-right:max(var(--mdc-fab-extended-label-padding, 20px), var(--mdc-fab-focus-outline-width, 0px));padding-bottom:0px;padding-bottom:max(0px, var(--mdc-fab-focus-outline-width, 0px));padding-left:20px;padding-left:max(var(--mdc-fab-extended-label-padding, 20px), var(--mdc-fab-focus-outline-width, 0px))}:host .mdc-fab.mdc-fab--extended:not(:disabled).mdc-ripple-upgraded--background-focused,:host .mdc-fab.mdc-fab--extended:not(:disabled):not(.mdc-ripple-upgraded):focus{border-style:solid;border-width:var(--mdc-fab-focus-outline-width, 0px);padding-top:0px;padding-top:max(calc(0px - var(--mdc-fab-focus-outline-width, 0px)), calc(calc(0px - var(--mdc-fab-focus-outline-width, 0px)) * -1));padding-right:20px;padding-right:max(calc(var(--mdc-fab-extended-label-padding, 20px) - var(--mdc-fab-focus-outline-width, 0px)), calc(calc(var(--mdc-fab-extended-label-padding, 20px) - var(--mdc-fab-focus-outline-width, 0px)) * -1));padding-bottom:0px;padding-bottom:max(calc(0px - var(--mdc-fab-focus-outline-width, 0px)), calc(calc(0px - var(--mdc-fab-focus-outline-width, 0px)) * -1));padding-left:20px;padding-left:max(calc(var(--mdc-fab-extended-label-padding, 20px) - var(--mdc-fab-focus-outline-width, 0px)), calc(calc(var(--mdc-fab-extended-label-padding, 20px) - var(--mdc-fab-focus-outline-width, 0px)) * -1))}:host .mdc-fab.mdc-fab--extended.icon-end .mdc-fab__icon{margin-left:12px;margin-left:var(--mdc-fab-extended-icon-padding, 12px);margin-right:calc(12px - 20px);margin-right:calc(var(--mdc-fab-extended-icon-padding, 12px) - var(--mdc-fab-extended-label-padding, 20px))}[dir=rtl] :host .mdc-fab.mdc-fab--extended.icon-end .mdc-fab__icon,:host .mdc-fab.mdc-fab--extended.icon-end .mdc-fab__icon[dir=rtl]{margin-left:calc(12px - 20px);margin-left:calc(var(--mdc-fab-extended-icon-padding, 12px) - var(--mdc-fab-extended-label-padding, 20px));margin-right:12px;margin-right:var(--mdc-fab-extended-icon-padding, 12px)}`;
-let Ml = class extends Nl {};
-Ml.styles = [$l], Ml = r([Bt("mwc-fab")], Ml);
-let Ll = class extends Ht {
+})], $l.prototype, "handleRippleStartPress", null);
+const Ml = Tt`:host .mdc-fab .material-icons{font-family:var(--mdc-icon-font, "Material Icons");font-weight:normal;font-style:normal;font-size:var(--mdc-icon-size, 24px);line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-smoothing:antialiased;text-rendering:optimizeLegibility;-moz-osx-font-smoothing:grayscale;font-feature-settings:"liga"}:host{outline:none;--mdc-ripple-color: currentcolor;user-select:none;-webkit-tap-highlight-color:transparent;display:inline-flex;-webkit-tap-highlight-color:transparent;display:inline-flex;outline:none;user-select:none}:host .mdc-touch-target-wrapper{display:inline}:host .mdc-elevation-overlay{position:absolute;border-radius:inherit;pointer-events:none;opacity:0;opacity:var(--mdc-elevation-overlay-opacity, 0);transition:opacity 280ms cubic-bezier(0.4, 0, 0.2, 1);background-color:#fff;background-color:var(--mdc-elevation-overlay-color, #fff)}:host .mdc-fab{position:relative;display:inline-flex;position:relative;align-items:center;justify-content:center;box-sizing:border-box;width:56px;height:56px;padding:0;border:none;fill:currentColor;text-decoration:none;cursor:pointer;user-select:none;-moz-appearance:none;-webkit-appearance:none;overflow:visible;transition:box-shadow 280ms cubic-bezier(0.4, 0, 0.2, 1),opacity 15ms linear 30ms,transform 270ms 0ms cubic-bezier(0, 0, 0.2, 1)}:host .mdc-fab .mdc-elevation-overlay{width:100%;height:100%;top:0;left:0}:host .mdc-fab::-moz-focus-inner{padding:0;border:0}:host .mdc-fab:hover{box-shadow:0px 5px 5px -3px rgba(0, 0, 0, 0.2),0px 8px 10px 1px rgba(0, 0, 0, 0.14),0px 3px 14px 2px rgba(0,0,0,.12)}:host .mdc-fab.mdc-ripple-upgraded--background-focused,:host .mdc-fab:not(.mdc-ripple-upgraded):focus{box-shadow:0px 5px 5px -3px rgba(0, 0, 0, 0.2),0px 8px 10px 1px rgba(0, 0, 0, 0.14),0px 3px 14px 2px rgba(0,0,0,.12)}:host .mdc-fab .mdc-fab__focus-ring{position:absolute}:host .mdc-fab.mdc-ripple-upgraded--background-focused .mdc-fab__focus-ring,:host .mdc-fab:not(.mdc-ripple-upgraded):focus .mdc-fab__focus-ring{pointer-events:none;border:2px solid transparent;border-radius:6px;box-sizing:content-box;position:absolute;top:50%;left:50%;transform:translate(-50%, -50%);height:calc( 100% + 4px );width:calc( 100% + 4px )}@media screen and (forced-colors: active){:host .mdc-fab.mdc-ripple-upgraded--background-focused .mdc-fab__focus-ring,:host .mdc-fab:not(.mdc-ripple-upgraded):focus .mdc-fab__focus-ring{border-color:CanvasText}}:host .mdc-fab.mdc-ripple-upgraded--background-focused .mdc-fab__focus-ring::after,:host .mdc-fab:not(.mdc-ripple-upgraded):focus .mdc-fab__focus-ring::after{content:"";border:2px solid transparent;border-radius:8px;display:block;position:absolute;top:50%;left:50%;transform:translate(-50%, -50%);height:calc(100% + 4px);width:calc(100% + 4px)}@media screen and (forced-colors: active){:host .mdc-fab.mdc-ripple-upgraded--background-focused .mdc-fab__focus-ring::after,:host .mdc-fab:not(.mdc-ripple-upgraded):focus .mdc-fab__focus-ring::after{border-color:CanvasText}}:host .mdc-fab:active,:host .mdc-fab:focus:active{box-shadow:0px 7px 8px -4px rgba(0, 0, 0, 0.2),0px 12px 17px 2px rgba(0, 0, 0, 0.14),0px 5px 22px 4px rgba(0,0,0,.12)}:host .mdc-fab:active,:host .mdc-fab:focus{outline:none}:host .mdc-fab:hover{cursor:pointer}:host .mdc-fab>svg{width:100%}:host .mdc-fab--mini{width:40px;height:40px}:host .mdc-fab--extended{-moz-osx-font-smoothing:grayscale;-webkit-font-smoothing:antialiased;font-family:Roboto, sans-serif;font-family:var(--mdc-typography-button-font-family, var(--mdc-typography-font-family, Roboto, sans-serif));font-size:0.875rem;font-size:var(--mdc-typography-button-font-size, 0.875rem);line-height:2.25rem;line-height:var(--mdc-typography-button-line-height, 2.25rem);font-weight:500;font-weight:var(--mdc-typography-button-font-weight, 500);letter-spacing:0.0892857143em;letter-spacing:var(--mdc-typography-button-letter-spacing, 0.0892857143em);text-decoration:none;text-decoration:var(--mdc-typography-button-text-decoration, none);text-transform:uppercase;text-transform:var(--mdc-typography-button-text-transform, uppercase);border-radius:24px;padding-left:20px;padding-right:20px;width:auto;max-width:100%;height:48px;line-height:normal}:host .mdc-fab--extended .mdc-fab__ripple{border-radius:24px}:host .mdc-fab--extended .mdc-fab__icon{margin-left:calc(12px - 20px);margin-right:12px}[dir=rtl] :host .mdc-fab--extended .mdc-fab__icon,:host .mdc-fab--extended .mdc-fab__icon[dir=rtl]{margin-left:12px;margin-right:calc(12px - 20px)}:host .mdc-fab--extended .mdc-fab__label+.mdc-fab__icon{margin-left:12px;margin-right:calc(12px - 20px)}[dir=rtl] :host .mdc-fab--extended .mdc-fab__label+.mdc-fab__icon,:host .mdc-fab--extended .mdc-fab__label+.mdc-fab__icon[dir=rtl]{margin-left:calc(12px - 20px);margin-right:12px}:host .mdc-fab--touch{margin-top:4px;margin-bottom:4px;margin-right:4px;margin-left:4px}:host .mdc-fab--touch .mdc-fab__touch{position:absolute;top:50%;height:48px;left:50%;width:48px;transform:translate(-50%, -50%)}:host .mdc-fab::before{position:absolute;box-sizing:border-box;width:100%;height:100%;top:0;left:0;border:1px solid transparent;border-radius:inherit;content:"";pointer-events:none}@media screen and (forced-colors: active){:host .mdc-fab::before{border-color:CanvasText}}:host .mdc-fab__label{justify-content:flex-start;text-overflow:ellipsis;white-space:nowrap;overflow-x:hidden;overflow-y:visible}:host .mdc-fab__icon{transition:transform 180ms 90ms cubic-bezier(0, 0, 0.2, 1);fill:currentColor;will-change:transform}:host .mdc-fab .mdc-fab__icon{display:inline-flex;align-items:center;justify-content:center}:host .mdc-fab--exited{transform:scale(0);opacity:0;transition:opacity 15ms linear 150ms,transform 180ms 0ms cubic-bezier(0.4, 0, 1, 1)}:host .mdc-fab--exited .mdc-fab__icon{transform:scale(0);transition:transform 135ms 0ms cubic-bezier(0.4, 0, 1, 1)}:host .mdc-fab{background-color:#018786;background-color:var(--mdc-theme-secondary, #018786);box-shadow:0px 3px 5px -1px rgba(0, 0, 0, 0.2),0px 6px 10px 0px rgba(0, 0, 0, 0.14),0px 1px 18px 0px rgba(0,0,0,.12)}:host .mdc-fab .mdc-fab__icon{width:24px;height:24px;font-size:24px}:host .mdc-fab,:host .mdc-fab:not(:disabled) .mdc-fab__icon,:host .mdc-fab:not(:disabled) .mdc-fab__label,:host .mdc-fab:disabled .mdc-fab__icon,:host .mdc-fab:disabled .mdc-fab__label{color:#fff;color:var(--mdc-theme-on-secondary, #fff)}:host .mdc-fab:not(.mdc-fab--extended){border-radius:50%}:host .mdc-fab:not(.mdc-fab--extended) .mdc-fab__ripple{border-radius:50%}:host .mdc-fab{position:relative;display:inline-flex;position:relative;align-items:center;justify-content:center;box-sizing:border-box;width:56px;height:56px;padding:0;border:none;fill:currentColor;text-decoration:none;cursor:pointer;user-select:none;-moz-appearance:none;-webkit-appearance:none;overflow:visible;transition:box-shadow 280ms cubic-bezier(0.4, 0, 0.2, 1),opacity 15ms linear 30ms,transform 270ms 0ms cubic-bezier(0, 0, 0.2, 1)}:host .mdc-fab .mdc-elevation-overlay{width:100%;height:100%;top:0;left:0}:host .mdc-fab::-moz-focus-inner{padding:0;border:0}:host .mdc-fab:hover{box-shadow:0px 5px 5px -3px rgba(0, 0, 0, 0.2),0px 8px 10px 1px rgba(0, 0, 0, 0.14),0px 3px 14px 2px rgba(0,0,0,.12)}:host .mdc-fab.mdc-ripple-upgraded--background-focused,:host .mdc-fab:not(.mdc-ripple-upgraded):focus{box-shadow:0px 5px 5px -3px rgba(0, 0, 0, 0.2),0px 8px 10px 1px rgba(0, 0, 0, 0.14),0px 3px 14px 2px rgba(0,0,0,.12)}:host .mdc-fab .mdc-fab__focus-ring{position:absolute}:host .mdc-fab.mdc-ripple-upgraded--background-focused .mdc-fab__focus-ring,:host .mdc-fab:not(.mdc-ripple-upgraded):focus .mdc-fab__focus-ring{pointer-events:none;border:2px solid transparent;border-radius:6px;box-sizing:content-box;position:absolute;top:50%;left:50%;transform:translate(-50%, -50%);height:calc( 100% + 4px );width:calc( 100% + 4px )}@media screen and (forced-colors: active){:host .mdc-fab.mdc-ripple-upgraded--background-focused .mdc-fab__focus-ring,:host .mdc-fab:not(.mdc-ripple-upgraded):focus .mdc-fab__focus-ring{border-color:CanvasText}}:host .mdc-fab.mdc-ripple-upgraded--background-focused .mdc-fab__focus-ring::after,:host .mdc-fab:not(.mdc-ripple-upgraded):focus .mdc-fab__focus-ring::after{content:"";border:2px solid transparent;border-radius:8px;display:block;position:absolute;top:50%;left:50%;transform:translate(-50%, -50%);height:calc(100% + 4px);width:calc(100% + 4px)}@media screen and (forced-colors: active){:host .mdc-fab.mdc-ripple-upgraded--background-focused .mdc-fab__focus-ring::after,:host .mdc-fab:not(.mdc-ripple-upgraded):focus .mdc-fab__focus-ring::after{border-color:CanvasText}}:host .mdc-fab:active,:host .mdc-fab:focus:active{box-shadow:0px 7px 8px -4px rgba(0, 0, 0, 0.2),0px 12px 17px 2px rgba(0, 0, 0, 0.14),0px 5px 22px 4px rgba(0,0,0,.12)}:host .mdc-fab:active,:host .mdc-fab:focus{outline:none}:host .mdc-fab:hover{cursor:pointer}:host .mdc-fab>svg{width:100%}:host .mdc-fab--mini{width:40px;height:40px}:host .mdc-fab--extended{-moz-osx-font-smoothing:grayscale;-webkit-font-smoothing:antialiased;font-family:Roboto, sans-serif;font-family:var(--mdc-typography-button-font-family, var(--mdc-typography-font-family, Roboto, sans-serif));font-size:0.875rem;font-size:var(--mdc-typography-button-font-size, 0.875rem);line-height:2.25rem;line-height:var(--mdc-typography-button-line-height, 2.25rem);font-weight:500;font-weight:var(--mdc-typography-button-font-weight, 500);letter-spacing:0.0892857143em;letter-spacing:var(--mdc-typography-button-letter-spacing, 0.0892857143em);text-decoration:none;text-decoration:var(--mdc-typography-button-text-decoration, none);text-transform:uppercase;text-transform:var(--mdc-typography-button-text-transform, uppercase);border-radius:24px;padding-left:20px;padding-right:20px;width:auto;max-width:100%;height:48px;line-height:normal}:host .mdc-fab--extended .mdc-fab__ripple{border-radius:24px}:host .mdc-fab--extended .mdc-fab__icon{margin-left:calc(12px - 20px);margin-right:12px}[dir=rtl] :host .mdc-fab--extended .mdc-fab__icon,:host .mdc-fab--extended .mdc-fab__icon[dir=rtl]{margin-left:12px;margin-right:calc(12px - 20px)}:host .mdc-fab--extended .mdc-fab__label+.mdc-fab__icon{margin-left:12px;margin-right:calc(12px - 20px)}[dir=rtl] :host .mdc-fab--extended .mdc-fab__label+.mdc-fab__icon,:host .mdc-fab--extended .mdc-fab__label+.mdc-fab__icon[dir=rtl]{margin-left:calc(12px - 20px);margin-right:12px}:host .mdc-fab--touch{margin-top:4px;margin-bottom:4px;margin-right:4px;margin-left:4px}:host .mdc-fab--touch .mdc-fab__touch{position:absolute;top:50%;height:48px;left:50%;width:48px;transform:translate(-50%, -50%)}:host .mdc-fab::before{position:absolute;box-sizing:border-box;width:100%;height:100%;top:0;left:0;border:1px solid transparent;border-radius:inherit;content:"";pointer-events:none}@media screen and (forced-colors: active){:host .mdc-fab::before{border-color:CanvasText}}:host .mdc-fab__label{justify-content:flex-start;text-overflow:ellipsis;white-space:nowrap;overflow-x:hidden;overflow-y:visible}:host .mdc-fab__icon{transition:transform 180ms 90ms cubic-bezier(0, 0, 0.2, 1);fill:currentColor;will-change:transform}:host .mdc-fab .mdc-fab__icon{display:inline-flex;align-items:center;justify-content:center}:host .mdc-fab--exited{transform:scale(0);opacity:0;transition:opacity 15ms linear 150ms,transform 180ms 0ms cubic-bezier(0.4, 0, 1, 1)}:host .mdc-fab--exited .mdc-fab__icon{transform:scale(0);transition:transform 135ms 0ms cubic-bezier(0.4, 0, 1, 1)}:host .mdc-fab .ripple{overflow:hidden}:host .mdc-fab:not(.mdc-fab--extended) .ripple{border-radius:50%}:host .mdc-fab.mdc-fab--extended .ripple{border-radius:24px}:host .mdc-fab .mdc-fab__label{z-index:0}:host .mdc-fab .mdc-fab__icon ::slotted(*){width:inherit;height:inherit;font-size:inherit}:host .mdc-fab--extended.mdc-fab--exited .mdc-fab__icon ::slotted(*){transform:scale(0);transition:transform 135ms 0ms cubic-bezier(0.4, 0, 1, 1)}:host .mdc-fab{padding-top:0px;padding-top:max(0px, var(--mdc-fab-focus-outline-width, 0px));padding-right:0px;padding-right:max(0px, var(--mdc-fab-focus-outline-width, 0px));padding-bottom:0px;padding-bottom:max(0px, var(--mdc-fab-focus-outline-width, 0px));padding-left:0px;padding-left:max(0px, var(--mdc-fab-focus-outline-width, 0px));box-shadow:0px 3px 5px -1px rgba(0, 0, 0, 0.2), 0px 6px 10px 0px rgba(0, 0, 0, 0.14), 0px 1px 18px 0px rgba(0, 0, 0, 0.12);box-shadow:var(--mdc-fab-box-shadow, 0px 3px 5px -1px rgba(0, 0, 0, 0.2), 0px 6px 10px 0px rgba(0, 0, 0, 0.14), 0px 1px 18px 0px rgba(0, 0, 0, 0.12))}:host .mdc-fab:not(:disabled).mdc-ripple-upgraded--background-focused,:host .mdc-fab:not(:disabled):not(.mdc-ripple-upgraded):focus{border-color:initial;border-color:var(--mdc-fab-focus-outline-color, initial)}:host .mdc-fab:not(:disabled).mdc-ripple-upgraded--background-focused,:host .mdc-fab:not(:disabled):not(.mdc-ripple-upgraded):focus{border-style:solid;border-width:var(--mdc-fab-focus-outline-width, 0px);padding-top:0px;padding-top:max(calc(0px - var(--mdc-fab-focus-outline-width, 0px)), calc(calc(0px - var(--mdc-fab-focus-outline-width, 0px)) * -1));padding-right:0px;padding-right:max(calc(0px - var(--mdc-fab-focus-outline-width, 0px)), calc(calc(0px - var(--mdc-fab-focus-outline-width, 0px)) * -1));padding-bottom:0px;padding-bottom:max(calc(0px - var(--mdc-fab-focus-outline-width, 0px)), calc(calc(0px - var(--mdc-fab-focus-outline-width, 0px)) * -1));padding-left:0px;padding-left:max(calc(0px - var(--mdc-fab-focus-outline-width, 0px)), calc(calc(0px - var(--mdc-fab-focus-outline-width, 0px)) * -1))}:host .mdc-fab:hover,:host .mdc-fab:focus{box-shadow:0px 5px 5px -3px rgba(0, 0, 0, 0.2), 0px 8px 10px 1px rgba(0, 0, 0, 0.14), 0px 3px 14px 2px rgba(0, 0, 0, 0.12);box-shadow:var(--mdc-fab-box-shadow, 0px 5px 5px -3px rgba(0, 0, 0, 0.2), 0px 8px 10px 1px rgba(0, 0, 0, 0.14), 0px 3px 14px 2px rgba(0, 0, 0, 0.12))}:host .mdc-fab:active{box-shadow:0px 7px 8px -4px rgba(0, 0, 0, 0.2), 0px 12px 17px 2px rgba(0, 0, 0, 0.14), 0px 5px 22px 4px rgba(0, 0, 0, 0.12);box-shadow:var(--mdc-fab-box-shadow, 0px 7px 8px -4px rgba(0, 0, 0, 0.2), 0px 12px 17px 2px rgba(0, 0, 0, 0.14), 0px 5px 22px 4px rgba(0, 0, 0, 0.12))}:host .mdc-fab .ripple{overflow:hidden}:host .mdc-fab .mdc-fab__label{z-index:0}:host .mdc-fab:not(.mdc-fab--extended) .ripple{border-radius:50%}:host .mdc-fab.mdc-fab--extended .ripple{border-radius:24px}:host .mdc-fab .mdc-fab__icon{width:24px;width:var(--mdc-icon-size, 24px);height:24px;height:var(--mdc-icon-size, 24px);font-size:24px;font-size:var(--mdc-icon-size, 24px);transition:transform 180ms 90ms cubic-bezier(0, 0, 0.2, 1);fill:currentColor;will-change:transform;display:inline-flex;align-items:center;justify-content:center}:host .mdc-fab.mdc-fab--extended{padding-top:0px;padding-top:max(0px, var(--mdc-fab-focus-outline-width, 0px));padding-right:20px;padding-right:max(var(--mdc-fab-extended-label-padding, 20px), var(--mdc-fab-focus-outline-width, 0px));padding-bottom:0px;padding-bottom:max(0px, var(--mdc-fab-focus-outline-width, 0px));padding-left:20px;padding-left:max(var(--mdc-fab-extended-label-padding, 20px), var(--mdc-fab-focus-outline-width, 0px))}:host .mdc-fab.mdc-fab--extended:not(:disabled).mdc-ripple-upgraded--background-focused,:host .mdc-fab.mdc-fab--extended:not(:disabled):not(.mdc-ripple-upgraded):focus{border-style:solid;border-width:var(--mdc-fab-focus-outline-width, 0px);padding-top:0px;padding-top:max(calc(0px - var(--mdc-fab-focus-outline-width, 0px)), calc(calc(0px - var(--mdc-fab-focus-outline-width, 0px)) * -1));padding-right:20px;padding-right:max(calc(var(--mdc-fab-extended-label-padding, 20px) - var(--mdc-fab-focus-outline-width, 0px)), calc(calc(var(--mdc-fab-extended-label-padding, 20px) - var(--mdc-fab-focus-outline-width, 0px)) * -1));padding-bottom:0px;padding-bottom:max(calc(0px - var(--mdc-fab-focus-outline-width, 0px)), calc(calc(0px - var(--mdc-fab-focus-outline-width, 0px)) * -1));padding-left:20px;padding-left:max(calc(var(--mdc-fab-extended-label-padding, 20px) - var(--mdc-fab-focus-outline-width, 0px)), calc(calc(var(--mdc-fab-extended-label-padding, 20px) - var(--mdc-fab-focus-outline-width, 0px)) * -1))}:host .mdc-fab.mdc-fab--extended.icon-end .mdc-fab__icon{margin-left:12px;margin-left:var(--mdc-fab-extended-icon-padding, 12px);margin-right:calc(12px - 20px);margin-right:calc(var(--mdc-fab-extended-icon-padding, 12px) - var(--mdc-fab-extended-label-padding, 20px))}[dir=rtl] :host .mdc-fab.mdc-fab--extended.icon-end .mdc-fab__icon,:host .mdc-fab.mdc-fab--extended.icon-end .mdc-fab__icon[dir=rtl]{margin-left:calc(12px - 20px);margin-left:calc(var(--mdc-fab-extended-icon-padding, 12px) - var(--mdc-fab-extended-label-padding, 20px));margin-right:12px;margin-right:var(--mdc-fab-extended-icon-padding, 12px)}`;
+let Ll = class extends $l {};
+Ll.styles = [Ml], Ll = r([Bt("mwc-fab")], Ll);
+let Fl = class extends Ht {
     render() {
         return S`
       <mwc-fab
         extended
         icon="add"
         label="New device"
         @click=${this._handleClick}
       ></mwc-fab>
     `
     }
     _handleClick() {
         ce()
     }
 };
-Ll.styles = Tt`
+Fl.styles = Tt`
     mwc-fab {
       position: fixed;
       right: 23px;
       bottom: 23px;
       z-index: 997;
       --mdc-theme-secondary: var(--alert-success-color);
     }
-  `, Ll = r([Bt("esphome-fab")], Ll);
-let Fl = class extends Ht {
+  `, Fl = r([Bt("esphome-fab")], Fl);
+let Dl = class extends Ht {
     constructor() {
         super(...arguments), this.version = "unknown", this.docsLink = ""
     }
     render() {
         return this.editing ? S`
         <style>
           esphome-editor {
@@ -9965,19 +9970,19 @@
     }
     createRenderRoot() {
         return this
     }
     firstUpdated(t) {
         super.firstUpdated(t), document.body.addEventListener("edit-file", (t => {
             this.editing = t.detail
-        })), import("./c.5cae2e65.js").then((function(t) {
+        })), import("./c.a94304a8.js").then((function(t) {
             return t.e
         }))
     }
     _handleEditorClose() {
         this.editing = void 0
     }
 };
-r([jt()], Fl.prototype, "version", void 0), r([jt()], Fl.prototype, "docsLink", void 0), r([jt()], Fl.prototype, "logoutUrl", void 0), r([Vt()], Fl.prototype, "editing", void 0), Fl = r([Bt("esphome-main")], Fl);
+r([jt()], Dl.prototype, "version", void 0), r([jt()], Dl.prototype, "docsLink", void 0), r([jt()], Dl.prototype, "logoutUrl", void 0), r([Vt()], Dl.prototype, "editing", void 0), Dl = r([Bt("esphome-main")], Dl);
 export {
-    K as $, le as A, ve as B, Cl as C, vl as D, Be as E, yl as F, el as G, ol as H, P as I, J, hl as K, ll as L, xe as M, dl as N, pl as O, bl as P, wl as Q, Le as R, Re as S, T, ae as U, Tl as V, Pl as W, W as X, s as Y, q as Z, i as _, o as a, O as a0, it as a1, me as a2, ue as a3, al as a4, il as a5, re as a6, r as b, ct as c, jt as d, Y as e, Ie as f, fe as g, Zd as h, Yt as i, Jd as j, rl as k, Vt as l, Wt as m, Bt as n, Ue as o, Me as p, Gt as q, Tt as r, Ht as s, G as t, Fe as u, Kt as v, sl as w, ne as x, S as y, gl as z
+    s as $, le as A, ve as B, Al as C, xl as D, Be as E, vl as F, el as G, il as H, rl as I, P as J, J as K, ul as L, xe as M, cl as N, ll as O, hl as P, yl as Q, Le as R, Cl as S, Re as T, T as U, ae as V, Pl as W, Ol as X, W as Y, q as Z, i as _, o as a, K as a0, O as a1, it as a2, me as a3, ue as a4, dl as a5, nl as a6, re as a7, r as b, ct as c, jt as d, Y as e, Ie as f, fe as g, Zd as h, Yt as i, Jd as j, sl as k, Vt as l, Wt as m, Bt as n, Ue as o, Me as p, Gt as q, Tt as r, Ht as s, G as t, Fe as u, Kt as v, al as w, ne as x, S as y, bl as z
 };
```

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/a4988.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/a4988.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/absolute_humidity.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/absolute_humidity.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ac_dimmer.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ac_dimmer.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/adc.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/adc.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/adc128s102.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/adc128s102.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/addressable_light.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/addressable_light.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ade7953.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ade7953.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ads1115.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ads1115.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/aht10.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/aht10.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/airthings_ble.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/airthings_ble.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/airthings_wave_mini.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/airthings_wave_mini.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/airthings_wave_plus.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/airthings_wave_plus.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/am2320.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/am2320.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/am43.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/am43.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/analog_threshold.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/analog_threshold.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/animation.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/animation.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/anova.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/anova.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/apds9960.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/apds9960.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/api.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/api.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/as3935.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/as3935.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/as3935_i2c.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/as3935_i2c.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/as3935_spi.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/as3935_spi.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/as7341.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/as7341.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/atc_mithermometer.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/atc_mithermometer.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/atm90e32.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/atm90e32.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/b_parasite.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/b_parasite.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ballu.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ballu.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/bang_bang.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/bang_bang.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/bedjet.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/bedjet.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/bh1750.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/bh1750.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/binary.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/binary.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/binary_sensor.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/binary_sensor.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/binary_sensor_map.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/binary_sensor_map.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/bl0939.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/bl0939.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/bl0940.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/bl0940.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/bl0942.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/bl0942.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ble_client.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ble_client.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ble_presence.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ble_presence.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ble_rssi.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ble_rssi.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ble_scanner.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ble_scanner.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/bluetooth_proxy.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/bluetooth_proxy.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/bme280.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/bme280.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/bme680.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/bme680.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/bme680_bsec.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/bme680_bsec.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/bmp085.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/bmp085.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/bmp280.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/bmp280.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/bmp3xx.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/bmp3xx.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/bp1658cj.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/bp1658cj.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/bp5758d.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/bp5758d.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/button.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/button.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/canbus.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/canbus.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/cap1188.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/cap1188.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/captive_portal.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/captive_portal.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ccs811.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ccs811.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/cd74hc4067.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/cd74hc4067.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/climate.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/climate.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/climate_ir.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/climate_ir.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/climate_ir_lg.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/climate_ir_lg.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/color.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/color.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/color_temperature.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/color_temperature.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/component.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/component.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/coolix.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/coolix.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/copy.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/copy.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/cover.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/cover.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/cs5460a.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/cs5460a.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/cse7761.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/cse7761.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/cse7766.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/cse7766.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ct_clamp.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ct_clamp.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/current_based.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/current_based.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/custom.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/custom.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/custom_component.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/custom_component.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/cwww.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/cwww.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/dac7678.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/dac7678.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/daikin.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/daikin.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/daikin_brc.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/daikin_brc.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/dallas.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/dallas.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/daly_bms.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/daly_bms.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/debug.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/debug.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/deep_sleep.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/deep_sleep.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/delonghi.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/delonghi.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/demo.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/demo.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/dfplayer.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/dfplayer.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/dht.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/dht.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/dht12.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/dht12.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/display.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/display.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/display_menu.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/display_menu.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/display_menu_base.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/display_menu_base.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/dps310.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/dps310.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ds1307.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ds1307.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/dsmr.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/dsmr.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/duty_cycle.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/duty_cycle.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/e131.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/e131.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ee895.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ee895.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ektf2232.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ektf2232.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/endstop.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/endstop.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ens210.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ens210.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/esp32.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/esp32.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/esp32_ble.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/esp32_ble.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/esp32_ble_beacon.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/esp32_ble_beacon.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/esp32_ble_server.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/esp32_ble_server.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/esp32_ble_tracker.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/esp32_ble_tracker.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/esp32_camera.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/esp32_camera.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/esp32_camera_web_server.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/esp32_camera_web_server.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/esp32_can.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/esp32_can.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/esp32_dac.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/esp32_dac.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/esp32_hall.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/esp32_hall.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/esp32_improv.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/esp32_improv.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/esp32_touch.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/esp32_touch.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/esp8266.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/esp8266.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/esp8266_pwm.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/esp8266_pwm.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/esphome.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/esphome.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ethernet.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ethernet.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ethernet_info.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ethernet_info.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/exposure_notifications.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/exposure_notifications.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/external_components.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/external_components.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ezo.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ezo.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ezo_pmp.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ezo_pmp.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/factory_reset.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/factory_reset.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/fan.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/fan.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/fastled_base.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/fastled_base.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/fastled_clockless.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/fastled_clockless.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/fastled_spi.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/fastled_spi.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/feedback.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/feedback.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/fingerprint_grow.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/fingerprint_grow.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/font.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/font.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/fs3000.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/fs3000.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/fujitsu_general.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/fujitsu_general.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/globals.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/globals.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/gpio.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/gpio.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/gps.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/gps.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/graph.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/graph.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/growatt_solar.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/growatt_solar.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/haier.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/haier.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/havells_solar.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/havells_solar.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/hbridge.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/hbridge.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/hdc1080.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/hdc1080.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/heatpumpir.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/heatpumpir.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/hitachi_ac344.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/hitachi_ac344.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/hitachi_ac424.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/hitachi_ac424.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/hlw8012.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/hlw8012.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/hm3301.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/hm3301.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/hmc5883l.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/hmc5883l.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/homeassistant.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/homeassistant.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/honeywellabp.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/honeywellabp.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/hrxl_maxsonar_wr.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/hrxl_maxsonar_wr.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/hte501.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/hte501.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/http_request.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/http_request.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/htu21d.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/htu21d.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/hx711.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/hx711.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/hydreon_rgxx.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/hydreon_rgxx.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/hyt271.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/hyt271.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/i2c.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/i2c.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/i2s_audio.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/i2s_audio.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ili9xxx.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ili9xxx.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/image.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/image.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ina219.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ina219.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ina226.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ina226.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ina260.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ina260.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ina3221.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ina3221.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/inkbird_ibsth1_mini.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/inkbird_ibsth1_mini.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/inkplate6.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/inkplate6.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/integration.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/integration.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/internal_temperature.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/internal_temperature.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/interval.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/interval.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/kalman_combinator.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/kalman_combinator.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/key_collector.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/key_collector.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/kuntze.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/kuntze.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/lcd_base.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/lcd_base.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/lcd_gpio.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/lcd_gpio.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/lcd_menu.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/lcd_menu.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/lcd_pcf8574.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/lcd_pcf8574.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ld2410.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ld2410.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ledc.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ledc.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/light.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/light.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/lilygo_t5_47.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/lilygo_t5_47.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/lock.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/lock.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/logger.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/logger.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ltr390.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ltr390.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/matrix_keypad.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/matrix_keypad.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/max31855.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/max31855.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/max31856.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/max31856.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/max31865.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/max31865.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/max44009.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/max44009.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/max6675.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/max6675.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/max6956.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/max6956.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/max7219.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/max7219.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/max7219digit.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/max7219digit.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/max9611.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/max9611.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mcp23008.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mcp23008.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mcp23016.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mcp23016.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mcp23017.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mcp23017.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mcp23s08.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mcp23s08.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mcp23s17.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mcp23s17.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mcp2515.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mcp2515.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mcp3008.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mcp3008.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mcp3204.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mcp3204.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mcp4725.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mcp4725.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mcp4728.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mcp4728.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mcp47a1.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mcp47a1.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mcp9600.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mcp9600.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mcp9808.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mcp9808.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mdns.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mdns.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/media_player.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/media_player.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mhz19.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mhz19.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/microphone.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/microphone.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mics_4514.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mics_4514.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/midea.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/midea.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/midea_ac.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/midea_ac.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/midea_ir.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/midea_ir.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mitsubishi.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mitsubishi.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mlx90393.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mlx90393.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mlx90614.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mlx90614.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mmc5603.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mmc5603.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/modbus.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/modbus.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/modbus_controller.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/modbus_controller.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/monochromatic.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/monochromatic.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mopeka_ble.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mopeka_ble.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mopeka_pro_check.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mopeka_pro_check.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mopeka_std_check.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mopeka_std_check.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mpl3115a2.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mpl3115a2.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mpr121.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mpr121.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mpu6050.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mpu6050.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mpu6886.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mpu6886.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mqtt.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mqtt.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/mqtt_subscribe.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/mqtt_subscribe.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ms5611.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ms5611.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/my9231.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/my9231.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/neopixelbus.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/neopixelbus.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/network.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/network.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/nextion.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/nextion.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ntc.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ntc.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/number.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/number.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ota.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ota.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/output.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/output.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/packages.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/packages.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/page.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/page.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/partition.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/partition.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/pca6416a.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/pca6416a.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/pca9554.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/pca9554.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/pca9685.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/pca9685.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/pcd8544.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/pcd8544.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/pcf85063.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/pcf85063.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/pcf8574.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/pcf8574.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/pid.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/pid.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/pipsolar.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/pipsolar.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/pm1006.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/pm1006.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/pmsa003i.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/pmsa003i.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/pmsx003.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/pmsx003.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/pn532.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/pn532.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/pn532_i2c.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/pn532_i2c.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/pn532_spi.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/pn532_spi.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/power_supply.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/power_supply.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/preferences.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/preferences.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/prometheus.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/prometheus.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/pulse_counter.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/pulse_counter.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/pulse_meter.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/pulse_meter.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/pulse_width.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/pulse_width.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/pvvx_mithermometer.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/pvvx_mithermometer.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/pzem004t.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/pzem004t.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/pzemac.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/pzemac.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/pzemdc.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/pzemdc.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/qmc5883l.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/qmc5883l.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/qmp6988.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/qmp6988.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/qr_code.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/qr_code.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/radon_eye_ble.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/radon_eye_ble.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/radon_eye_rd200.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/radon_eye_rd200.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/rc522.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/rc522.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/rc522_i2c.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/rc522_i2c.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/rc522_spi.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/rc522_spi.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/rdm6300.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/rdm6300.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/remote_base.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/remote_base.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/remote_receiver.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/remote_receiver.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/remote_transmitter.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/remote_transmitter.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/resistance.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/resistance.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/restart.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/restart.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/rf_bridge.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/rf_bridge.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/rgb.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/rgb.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/rgbct.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/rgbct.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/rgbw.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/rgbw.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/rgbww.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/rgbww.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/rotary_encoder.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/rotary_encoder.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/rp2040.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/rp2040.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/rp2040_pwm.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/rp2040_pwm.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/rtttl.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/rtttl.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ruuvi_ble.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ruuvi_ble.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ruuvitag.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ruuvitag.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/safe_mode.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/safe_mode.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/scd30.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/scd30.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/scd4x.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/scd4x.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/script.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/script.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sdm_meter.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sdm_meter.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sdp3x.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sdp3x.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sds011.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sds011.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/selec_meter.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/selec_meter.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/select.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/select.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sen21231.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sen21231.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sen5x.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sen5x.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/senseair.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/senseair.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sensor.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sensor.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/servo.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/servo.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sgp30.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sgp30.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sgp4x.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sgp4x.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/shelly_dimmer.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/shelly_dimmer.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sht3xd.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sht3xd.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sht4x.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sht4x.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/shtcx.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/shtcx.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/shutdown.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/shutdown.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sigma_delta_output.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sigma_delta_output.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sim800l.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sim800l.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/slow_pwm.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/slow_pwm.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sm10bit_base.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sm10bit_base.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sm16716.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sm16716.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sm2135.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sm2135.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sm2235.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sm2235.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sm2335.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sm2335.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sm300d2.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sm300d2.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sml.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sml.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/smt100.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/smt100.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sn74hc165.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sn74hc165.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sn74hc595.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sn74hc595.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sntp.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sntp.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sonoff_d1.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sonoff_d1.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/speed.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/speed.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/spi.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/spi.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sprinkler.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sprinkler.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sps30.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sps30.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ssd1306_base.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ssd1306_base.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ssd1306_i2c.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ssd1306_i2c.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ssd1306_spi.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ssd1306_spi.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ssd1322_spi.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ssd1322_spi.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ssd1325_spi.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ssd1325_spi.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ssd1327_base.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ssd1327_base.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ssd1327_i2c.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ssd1327_i2c.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ssd1327_spi.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ssd1327_spi.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ssd1331_spi.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ssd1331_spi.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ssd1351_spi.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ssd1351_spi.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/st7735.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/st7735.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/st7789v.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/st7789v.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/st7920.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/st7920.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/status.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/status.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/status_led.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/status_led.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/stepper.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/stepper.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sts3x.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sts3x.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sun.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sun.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/switch.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/switch.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/sx1509.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/sx1509.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/t6615.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/t6615.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/tca9548a.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/tca9548a.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/tcl112.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/tcl112.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/tcs34725.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/tcs34725.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/tee501.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/tee501.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/teleinfo.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/teleinfo.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/template.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/template.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/text_sensor.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/text_sensor.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/thermostat.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/thermostat.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/time.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/time.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/time_based.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/time_based.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/tlc59208f.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/tlc59208f.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/tlc5947.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/tlc5947.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/tm1621.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/tm1621.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/tm1637.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/tm1637.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/tm1638.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/tm1638.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/tm1651.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/tm1651.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/tmp102.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/tmp102.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/tmp117.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/tmp117.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/tof10120.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/tof10120.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/toshiba.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/toshiba.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/total_daily_energy.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/total_daily_energy.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/touchscreen.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/touchscreen.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/tsl2561.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/tsl2561.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/tsl2591.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/tsl2591.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ttp229_bsf.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ttp229_bsf.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ttp229_lsf.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ttp229_lsf.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/tuya.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/tuya.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/tx20.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/tx20.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/uart.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/uart.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ufire_ec.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ufire_ec.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ufire_ise.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ufire_ise.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/uln2003.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/uln2003.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/ultrasonic.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/ultrasonic.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/uptime.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/uptime.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/vbus.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/vbus.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/version.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/version.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/vl53l0x.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/vl53l0x.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/voice_assistant.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/voice_assistant.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/wake_on_lan.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/wake_on_lan.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/waveshare_epaper.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/waveshare_epaper.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/web_server.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/web_server.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/whirlpool.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/whirlpool.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/whynter.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/whynter.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/wiegand.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/wiegand.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/wifi.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/wifi.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/wifi_info.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/wifi_info.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/wifi_signal.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/wifi_signal.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/wl_134.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/wl_134.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/x9c.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/x9c.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/xiaomi_ble.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/xiaomi_ble.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/xiaomi_cgd1.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/xiaomi_cgd1.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/xiaomi_cgdk2.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/xiaomi_cgdk2.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/xiaomi_cgg1.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/xiaomi_cgg1.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/xiaomi_cgpr1.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/xiaomi_cgpr1.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/xiaomi_gcls002.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/xiaomi_gcls002.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/xiaomi_hhccjcy01.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/xiaomi_hhccjcy01.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/xiaomi_hhccpot002.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/xiaomi_hhccpot002.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/xiaomi_jqjcy01ym.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/xiaomi_jqjcy01ym.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/xiaomi_lywsd02.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/xiaomi_lywsd02.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/xiaomi_lywsd03mmc.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/xiaomi_lywsd03mmc.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/xiaomi_lywsdcgq.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/xiaomi_lywsdcgq.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/xiaomi_mhoc303.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/xiaomi_mhoc303.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/xiaomi_mhoc401.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/xiaomi_mhoc401.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/xiaomi_miscale.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/xiaomi_miscale.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/xiaomi_mjyd02yla.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/xiaomi_mjyd02yla.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/xiaomi_mue4094rt.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/xiaomi_mue4094rt.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/xiaomi_rtcgq02lm.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/xiaomi_rtcgq02lm.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/xiaomi_wx08zm.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/xiaomi_wx08zm.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/xpt2046.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/xpt2046.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/yashima.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/yashima.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard/static/schema/zyaura.json` & `esphome-dashboard-20230621.0/esphome_dashboard/static/schema/zyaura.json`

 * *Files identical despite different names*

### Comparing `esphome-dashboard-20230516.0/esphome_dashboard.egg-info/SOURCES.txt` & `esphome-dashboard-20230621.0/esphome_dashboard.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,54 +20,54 @@
 esphome_dashboard/static/fonts/material-icons/LICENSE
 esphome_dashboard/static/fonts/material-icons/MaterialIcons-Regular.woff
 esphome_dashboard/static/fonts/material-icons/MaterialIcons-Regular.woff2
 esphome_dashboard/static/fonts/material-icons/README.md
 esphome_dashboard/static/fonts/material-icons/material-icons.css
 esphome_dashboard/static/images/favicon.ico
 esphome_dashboard/static/images/logo-text.svg
-esphome_dashboard/static/js/esphome/c.1bc018ae.js
-esphome_dashboard/static/js/esphome/c.1c31574e.js
+esphome_dashboard/static/js/esphome/c.1107b6f0.js
+esphome_dashboard/static/js/esphome/c.11743138.js
+esphome_dashboard/static/js/esphome/c.17838855.js
+esphome_dashboard/static/js/esphome/c.1fccc3bb.js
+esphome_dashboard/static/js/esphome/c.22fb066b.js
+esphome_dashboard/static/js/esphome/c.25394cef.js
 esphome_dashboard/static/js/esphome/c.286ad693.js
-esphome_dashboard/static/js/esphome/c.29c28c21.js
-esphome_dashboard/static/js/esphome/c.2b18cdda.js
-esphome_dashboard/static/js/esphome/c.363ea4b9.js
-esphome_dashboard/static/js/esphome/c.3b4072f5.js
+esphome_dashboard/static/js/esphome/c.2d34b51a.js
+esphome_dashboard/static/js/esphome/c.323af3d2.js
+esphome_dashboard/static/js/esphome/c.3bbbdf4b.js
+esphome_dashboard/static/js/esphome/c.3f59652f.js
+esphome_dashboard/static/js/esphome/c.40278fa0.js
 esphome_dashboard/static/js/esphome/c.417d3d2d.js
 esphome_dashboard/static/js/esphome/c.440fff61.js
-esphome_dashboard/static/js/esphome/c.45f3bfa8.js
-esphome_dashboard/static/js/esphome/c.52f07dd8.js
-esphome_dashboard/static/js/esphome/c.5cae2e65.js
+esphome_dashboard/static/js/esphome/c.4971d925.js
+esphome_dashboard/static/js/esphome/c.4c0eda7e.js
 esphome_dashboard/static/js/esphome/c.5cd5d307.js
-esphome_dashboard/static/js/esphome/c.61332c08.js
-esphome_dashboard/static/js/esphome/c.6d280f04.js
-esphome_dashboard/static/js/esphome/c.6eebcb7a.js
-esphome_dashboard/static/js/esphome/c.734d4b21.js
-esphome_dashboard/static/js/esphome/c.78cf8c6e.js
-esphome_dashboard/static/js/esphome/c.7d2e85dd.js
+esphome_dashboard/static/js/esphome/c.64ac3748.js
+esphome_dashboard/static/js/esphome/c.670cd819.js
+esphome_dashboard/static/js/esphome/c.6951bded.js
 esphome_dashboard/static/js/esphome/c.7e8b4fbe.js
-esphome_dashboard/static/js/esphome/c.834bbab0.js
-esphome_dashboard/static/js/esphome/c.98e8e8d2.js
-esphome_dashboard/static/js/esphome/c.9e5eaea1.js
-esphome_dashboard/static/js/esphome/c.a613b168.js
+esphome_dashboard/static/js/esphome/c.884f2894.js
+esphome_dashboard/static/js/esphome/c.8ab91975.js
+esphome_dashboard/static/js/esphome/c.90e5e76e.js
+esphome_dashboard/static/js/esphome/c.9d543f02.js
+esphome_dashboard/static/js/esphome/c.9f55698d.js
+esphome_dashboard/static/js/esphome/c.9fa8c472.js
 esphome_dashboard/static/js/esphome/c.a6e96e5a.js
-esphome_dashboard/static/js/esphome/c.b9286028.js
-esphome_dashboard/static/js/esphome/c.bff582f5.js
+esphome_dashboard/static/js/esphome/c.a94304a8.js
+esphome_dashboard/static/js/esphome/c.b545a09c.js
 esphome_dashboard/static/js/esphome/c.c0a69417.js
-esphome_dashboard/static/js/esphome/c.c2d1f4be.js
 esphome_dashboard/static/js/esphome/c.c74d5ae3.js
-esphome_dashboard/static/js/esphome/c.d408ba9c.js
-esphome_dashboard/static/js/esphome/c.db573db5.js
-esphome_dashboard/static/js/esphome/c.dde41422.js
-esphome_dashboard/static/js/esphome/c.e1319253.js
-esphome_dashboard/static/js/esphome/c.e4466087.js
-esphome_dashboard/static/js/esphome/c.e683a7a9.js
-esphome_dashboard/static/js/esphome/c.e6db31ca.js
-esphome_dashboard/static/js/esphome/c.ed145062.js
+esphome_dashboard/static/js/esphome/c.c84471ef.js
+esphome_dashboard/static/js/esphome/c.cce2f2f7.js
+esphome_dashboard/static/js/esphome/c.cd26dc5d.js
+esphome_dashboard/static/js/esphome/c.d861da54.js
+esphome_dashboard/static/js/esphome/c.f0358a8b.js
 esphome_dashboard/static/js/esphome/c.f4034d2e.js
-esphome_dashboard/static/js/esphome/index-d3dd97b9.js
+esphome_dashboard/static/js/esphome/c.fadc3045.js
+esphome_dashboard/static/js/esphome/index-bfcf9cd9.js
 esphome_dashboard/static/js/esphome/manifest.json
 esphome_dashboard/static/js/esphome/monaco-editor/esm/vs/editor/editor.worker.js
 esphome_dashboard/static/schema/a4988.json
 esphome_dashboard/static/schema/absolute_humidity.json
 esphome_dashboard/static/schema/ac_dimmer.json
 esphome_dashboard/static/schema/adalight.json
 esphome_dashboard/static/schema/adc.json
```

