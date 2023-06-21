# Comparing `tmp/mkdocs-kpn-1.5.2.tar.gz` & `tmp/mkdocs-kpn-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-kpn-1.5.2.tar", last modified: Wed Jan 11 15:13:00 2023, max compression
+gzip compressed data, was "mkdocs-kpn-1.6.0.tar", last modified: Wed Jun 21 07:43:54 2023, max compression
```

## Comparing `mkdocs-kpn-1.5.2.tar` & `mkdocs-kpn-1.6.0.tar`

### file list

```diff
@@ -1,95 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 15:13:00.815641 mkdocs-kpn-1.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-01-11 15:13:00.811641 mkdocs-kpn-1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 15:13:00.799641 mkdocs-kpn-1.5.2/kpn_theme/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/404.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12330 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 15:13:00.799641 mkdocs-kpn-1.5.2/kpn_theme/css/
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/css/atom-dark-one.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    80046 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/css/bundle.css
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/css/colors.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 15:13:00.803641 mkdocs-kpn-1.5.2/kpn_theme/css/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    78940 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/css/fonts/kpn-metric-bold.eot
--rw-r--r--   0 runner    (1001) docker     (123)   390677 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/css/fonts/kpn-metric-bold.svg
--rw-r--r--   0 runner    (1001) docker     (123)    78720 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/css/fonts/kpn-metric-bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    33196 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/css/fonts/kpn-metric-bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)    78860 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/css/fonts/kpn-metric-light.eot
--rw-r--r--   0 runner    (1001) docker     (123)   390945 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/css/fonts/kpn-metric-light.svg
--rw-r--r--   0 runner    (1001) docker     (123)    78620 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/css/fonts/kpn-metric-light.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    32964 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/css/fonts/kpn-metric-light.woff
--rw-r--r--   0 runner    (1001) docker     (123)    78376 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/css/fonts/kpn-metric-normal.eot
--rw-r--r--   0 runner    (1001) docker     (123)   389277 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/css/fonts/kpn-metric-normal.svg
--rw-r--r--   0 runner    (1001) docker     (123)    78144 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/css/fonts/kpn-metric-normal.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    32500 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/css/fonts/kpn-metric-normal.woff
--rw-r--r--   0 runner    (1001) docker     (123)    78664 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/css/fonts/kpn-metric-semi-bold.eot
--rw-r--r--   0 runner    (1001) docker     (123)   392846 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/css/fonts/kpn-metric-semi-bold.svg
--rw-r--r--   0 runner    (1001) docker     (123)    78412 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/css/fonts/kpn-metric-semi-bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    33068 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/css/fonts/kpn-metric-semi-bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)    86848 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/css/fonts/kpn-service-icons.eot
--rw-r--r--   0 runner    (1001) docker     (123)   338715 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/css/fonts/kpn-service-icons.svg
--rw-r--r--   0 runner    (1001) docker     (123)    86644 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/css/fonts/kpn-service-icons.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    86720 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/css/fonts/kpn-service-icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)    53476 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/css/fonts/kpn-ui-icons.eot
--rw-r--r--   0 runner    (1001) docker     (123)   208830 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/css/fonts/kpn-ui-icons.svg
--rw-r--r--   0 runner    (1001) docker     (123)    53292 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/css/fonts/kpn-ui-icons.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    53368 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/css/fonts/kpn-ui-icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/css/ir-black.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     8920 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/css/theme.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 15:13:00.811641 mkdocs-kpn-1.5.2/kpn_theme/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    78940 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/fonts/kpn-metric-bold.eot
--rw-r--r--   0 runner    (1001) docker     (123)   390677 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/fonts/kpn-metric-bold.svg
--rw-r--r--   0 runner    (1001) docker     (123)    78720 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/fonts/kpn-metric-bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    33196 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/fonts/kpn-metric-bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)    78860 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/fonts/kpn-metric-light.eot
--rw-r--r--   0 runner    (1001) docker     (123)   390945 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/fonts/kpn-metric-light.svg
--rw-r--r--   0 runner    (1001) docker     (123)    78620 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/fonts/kpn-metric-light.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    32964 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/fonts/kpn-metric-light.woff
--rw-r--r--   0 runner    (1001) docker     (123)    78376 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/fonts/kpn-metric-normal.eot
--rw-r--r--   0 runner    (1001) docker     (123)   389277 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/fonts/kpn-metric-normal.svg
--rw-r--r--   0 runner    (1001) docker     (123)    78144 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/fonts/kpn-metric-normal.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    32500 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/fonts/kpn-metric-normal.woff
--rw-r--r--   0 runner    (1001) docker     (123)    78664 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/fonts/kpn-metric-semi-bold.eot
--rw-r--r--   0 runner    (1001) docker     (123)   392846 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/fonts/kpn-metric-semi-bold.svg
--rw-r--r--   0 runner    (1001) docker     (123)    78412 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/fonts/kpn-metric-semi-bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    33068 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/fonts/kpn-metric-semi-bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)    86848 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/fonts/kpn-service-icons.eot
--rw-r--r--   0 runner    (1001) docker     (123)   338715 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/fonts/kpn-service-icons.svg
--rw-r--r--   0 runner    (1001) docker     (123)    86644 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/fonts/kpn-service-icons.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    86720 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/fonts/kpn-service-icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)    53476 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/fonts/kpn-ui-icons.eot
--rw-r--r--   0 runner    (1001) docker     (123)   208830 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/fonts/kpn-ui-icons.svg
--rw-r--r--   0 runner    (1001) docker     (123)    53292 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/fonts/kpn-ui-icons.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    53368 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/fonts/kpn-ui-icons.woff
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 15:13:00.811641 mkdocs-kpn-1.5.2/kpn_theme/img/
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/img/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/img/git-icon-black.png
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/img/git.svg
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/img/logo-bitbucket.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/img/logo-gitea.svg
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/img/logo-github.svg
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/img/logo-gitlab.svg
--rw-r--r--   0 runner    (1001) docker     (123)    34659 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/img/logo-kpn.png
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/img/logo-kpn.svg
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/img/ui-bulb.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 15:13:00.811641 mkdocs-kpn-1.5.2/kpn_theme/js/
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/js/detail.js
--rw-r--r--   0 runner    (1001) docker     (123)   120762 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/js/highlight.min.js
--rw-r--r--   0 runner    (1001) docker     (123)  1100357 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/js/mermaid.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/js/theme.js
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/main.html
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/mkdocs_theme.yml
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/nav.html
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/kpn_theme/search.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 15:13:00.811641 mkdocs-kpn-1.5.2/mkdocs_kpn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-01-11 15:13:00.000000 mkdocs-kpn-1.5.2/mkdocs_kpn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-01-11 15:13:00.000000 mkdocs-kpn-1.5.2/mkdocs_kpn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 15:13:00.000000 mkdocs-kpn-1.5.2/mkdocs_kpn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-01-11 15:13:00.000000 mkdocs-kpn-1.5.2/mkdocs_kpn.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 15:12:59.000000 mkdocs-kpn-1.5.2/mkdocs_kpn.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-01-11 15:13:00.000000 mkdocs-kpn-1.5.2/mkdocs_kpn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-11 15:13:00.000000 mkdocs-kpn-1.5.2/mkdocs_kpn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-11 15:13:00.815641 mkdocs-kpn-1.5.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1273 2023-01-11 15:12:48.000000 mkdocs-kpn-1.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:43:54.211860 mkdocs-kpn-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-21 07:43:54.211860 mkdocs-kpn-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:43:54.187860 mkdocs-kpn-1.6.0/kpn_theme/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/404.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12525 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:43:54.187860 mkdocs-kpn-1.6.0/kpn_theme/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/css/atom-dark-one.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    80046 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/css/bundle.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/css/colors.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:43:54.195860 mkdocs-kpn-1.6.0/kpn_theme/css/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    78940 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/css/fonts/kpn-metric-bold.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   390677 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/css/fonts/kpn-metric-bold.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    78720 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/css/fonts/kpn-metric-bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    33196 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/css/fonts/kpn-metric-bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    78860 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/css/fonts/kpn-metric-light.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   390945 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/css/fonts/kpn-metric-light.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    78620 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/css/fonts/kpn-metric-light.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    32964 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/css/fonts/kpn-metric-light.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    78376 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/css/fonts/kpn-metric-normal.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   389277 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/css/fonts/kpn-metric-normal.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    78144 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/css/fonts/kpn-metric-normal.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    32500 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/css/fonts/kpn-metric-normal.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    78664 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/css/fonts/kpn-metric-semi-bold.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   392846 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/css/fonts/kpn-metric-semi-bold.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    78412 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/css/fonts/kpn-metric-semi-bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    33068 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/css/fonts/kpn-metric-semi-bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    86848 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/css/fonts/kpn-service-icons.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   338715 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/css/fonts/kpn-service-icons.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    86644 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/css/fonts/kpn-service-icons.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    86720 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/css/fonts/kpn-service-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    53476 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/css/fonts/kpn-ui-icons.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   208830 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/css/fonts/kpn-ui-icons.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    53292 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/css/fonts/kpn-ui-icons.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    53368 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/css/fonts/kpn-ui-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/css/ir-black.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     8920 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/css/theme.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:43:54.203860 mkdocs-kpn-1.6.0/kpn_theme/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    78940 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/fonts/kpn-metric-bold.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   390677 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/fonts/kpn-metric-bold.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    78720 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/fonts/kpn-metric-bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    33196 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/fonts/kpn-metric-bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    78860 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/fonts/kpn-metric-light.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   390945 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/fonts/kpn-metric-light.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    78620 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/fonts/kpn-metric-light.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    32964 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/fonts/kpn-metric-light.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    78376 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/fonts/kpn-metric-normal.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   389277 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/fonts/kpn-metric-normal.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    78144 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/fonts/kpn-metric-normal.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    32500 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/fonts/kpn-metric-normal.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    78664 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/fonts/kpn-metric-semi-bold.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   392846 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/fonts/kpn-metric-semi-bold.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    78412 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/fonts/kpn-metric-semi-bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    33068 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/fonts/kpn-metric-semi-bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    86848 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/fonts/kpn-service-icons.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   338715 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/fonts/kpn-service-icons.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    86644 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/fonts/kpn-service-icons.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    86720 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/fonts/kpn-service-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    53476 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/fonts/kpn-ui-icons.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   208830 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/fonts/kpn-ui-icons.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    53292 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/fonts/kpn-ui-icons.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    53368 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/fonts/kpn-ui-icons.woff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:43:54.207860 mkdocs-kpn-1.6.0/kpn_theme/img/
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/img/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/img/git-icon-black.png
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/img/git.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/img/logo-bitbucket.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/img/logo-gitea.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/img/logo-github.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/img/logo-gitlab.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    34659 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/img/logo-kpn.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/img/logo-kpn.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/img/ui-bulb.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:43:54.211860 mkdocs-kpn-1.6.0/kpn_theme/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/js/detail.js
+-rw-r--r--   0 runner    (1001) docker     (123)   125913 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/js/highlight.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:43:54.211860 mkdocs-kpn-1.6.0/kpn_theme/js/languages/
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/js/languages/asciidoc.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/js/languages/groovy.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/js/languages/nix.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1100357 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/js/mermaid.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/js/theme.js
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/main.html
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/mkdocs_theme.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/nav.html
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/kpn_theme/search.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:43:54.211860 mkdocs-kpn-1.6.0/mkdocs_kpn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-21 07:43:54.000000 mkdocs-kpn-1.6.0/mkdocs_kpn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-06-21 07:43:54.000000 mkdocs-kpn-1.6.0/mkdocs_kpn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 07:43:54.000000 mkdocs-kpn-1.6.0/mkdocs_kpn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-21 07:43:54.000000 mkdocs-kpn-1.6.0/mkdocs_kpn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 07:43:52.000000 mkdocs-kpn-1.6.0/mkdocs_kpn.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-21 07:43:54.000000 mkdocs-kpn-1.6.0/mkdocs_kpn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-21 07:43:54.000000 mkdocs-kpn-1.6.0/mkdocs_kpn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 07:43:54.211860 mkdocs-kpn-1.6.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1273 2023-06-21 07:43:37.000000 mkdocs-kpn-1.6.0/setup.py
```

### Comparing `mkdocs-kpn-1.5.2/LICENSE` & `mkdocs-kpn-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/PKG-INFO` & `mkdocs-kpn-1.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-kpn
-Version: 1.5.2
+Version: 1.6.0
 Summary: A KPN-styles theme for MkDocs
 Home-page: https://github.com/kpn/mkdocs-kpn-theme
 Author: Santiago Fraire Willemoës
 Author-email: de-ddci@kpn.com
 License: MIT
 Keywords: mkdocs,documentation,theme
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mkdocs-kpn-1.5.2/README.md` & `mkdocs-kpn-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/base.html` & `mkdocs-kpn-1.6.0/kpn_theme/base.html`

 * *Files 3% similar despite different names*

```diff
@@ -299,14 +299,18 @@
 
   <!--
     To include static assets from our theme, just add
     {{ base_url }} beforehand which will be the relative path to
     the root of the documentation.
   -->
   <script src="{{ "js/highlight.min.js"|url }}"></script>
+  <script src="{{ "js/languages/groovy.min.js"|url }}"></script>
+  <script src="{{ "js/languages/asciidoc.min.js"|url }}"></script>
+  <script src="{{ "js/languages/nix.min.js"|url }}"></script>
+
   <script>
     hljs.highlightAll();
   </script>
   <script async src="{{ "js/detail.js"|url }}"></script>
   <!--
     extra_javascript contains paths to JavaScript files in the
     users documentation directory or a list of JavaScript files
```

#### html2text {}

```diff
@@ -70,11 +70,14 @@
 %} {% if config.copyright %}
 {{ config.copyright }}
 {% endif %} {% if page.next_page %} Next_Page_→ {% else %} Next Page → {% endif
 %}
 {% endif %}
 
 ighlight.min.js"|url }}">
+anguages/groovy.min.js"|url }}">
+anguages/asciidoc.min.js"|url }}">
+anguages/nix.min.js"|url }}">
 
 etail.js"|url }}">
  {% for path in config.extra_javascript %}
  {% endfor %}
```

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/css/atom-dark-one.min.css` & `mkdocs-kpn-1.6.0/kpn_theme/css/atom-dark-one.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/css/bundle.css` & `mkdocs-kpn-1.6.0/kpn_theme/css/bundle.css`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/css/colors.css` & `mkdocs-kpn-1.6.0/kpn_theme/css/colors.css`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/css/fonts/kpn-metric-bold.eot` & `mkdocs-kpn-1.6.0/kpn_theme/css/fonts/kpn-metric-bold.eot`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/css/fonts/kpn-metric-bold.svg` & `mkdocs-kpn-1.6.0/kpn_theme/css/fonts/kpn-metric-bold.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/css/fonts/kpn-metric-bold.ttf` & `mkdocs-kpn-1.6.0/kpn_theme/css/fonts/kpn-metric-bold.ttf`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/css/fonts/kpn-metric-bold.woff` & `mkdocs-kpn-1.6.0/kpn_theme/css/fonts/kpn-metric-bold.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/css/fonts/kpn-metric-light.eot` & `mkdocs-kpn-1.6.0/kpn_theme/css/fonts/kpn-metric-light.eot`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/css/fonts/kpn-metric-light.svg` & `mkdocs-kpn-1.6.0/kpn_theme/css/fonts/kpn-metric-light.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/css/fonts/kpn-metric-light.ttf` & `mkdocs-kpn-1.6.0/kpn_theme/css/fonts/kpn-metric-light.ttf`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/css/fonts/kpn-metric-light.woff` & `mkdocs-kpn-1.6.0/kpn_theme/css/fonts/kpn-metric-light.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/css/fonts/kpn-metric-normal.eot` & `mkdocs-kpn-1.6.0/kpn_theme/css/fonts/kpn-metric-normal.eot`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/css/fonts/kpn-metric-normal.svg` & `mkdocs-kpn-1.6.0/kpn_theme/css/fonts/kpn-metric-normal.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/css/fonts/kpn-metric-normal.ttf` & `mkdocs-kpn-1.6.0/kpn_theme/css/fonts/kpn-metric-normal.ttf`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/css/fonts/kpn-metric-normal.woff` & `mkdocs-kpn-1.6.0/kpn_theme/css/fonts/kpn-metric-normal.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/css/fonts/kpn-metric-semi-bold.eot` & `mkdocs-kpn-1.6.0/kpn_theme/css/fonts/kpn-metric-semi-bold.eot`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/css/fonts/kpn-metric-semi-bold.svg` & `mkdocs-kpn-1.6.0/kpn_theme/css/fonts/kpn-metric-semi-bold.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/css/fonts/kpn-metric-semi-bold.ttf` & `mkdocs-kpn-1.6.0/kpn_theme/css/fonts/kpn-metric-semi-bold.ttf`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/css/fonts/kpn-metric-semi-bold.woff` & `mkdocs-kpn-1.6.0/kpn_theme/css/fonts/kpn-metric-semi-bold.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/css/fonts/kpn-service-icons.eot` & `mkdocs-kpn-1.6.0/kpn_theme/css/fonts/kpn-service-icons.eot`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/css/fonts/kpn-service-icons.svg` & `mkdocs-kpn-1.6.0/kpn_theme/css/fonts/kpn-service-icons.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/css/fonts/kpn-service-icons.ttf` & `mkdocs-kpn-1.6.0/kpn_theme/css/fonts/kpn-service-icons.ttf`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/css/fonts/kpn-service-icons.woff` & `mkdocs-kpn-1.6.0/kpn_theme/css/fonts/kpn-service-icons.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/css/fonts/kpn-ui-icons.eot` & `mkdocs-kpn-1.6.0/kpn_theme/css/fonts/kpn-ui-icons.eot`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/css/fonts/kpn-ui-icons.svg` & `mkdocs-kpn-1.6.0/kpn_theme/css/fonts/kpn-ui-icons.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/css/fonts/kpn-ui-icons.ttf` & `mkdocs-kpn-1.6.0/kpn_theme/css/fonts/kpn-ui-icons.ttf`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/css/fonts/kpn-ui-icons.woff` & `mkdocs-kpn-1.6.0/kpn_theme/css/fonts/kpn-ui-icons.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/css/ir-black.min.css` & `mkdocs-kpn-1.6.0/kpn_theme/css/ir-black.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/css/theme.css` & `mkdocs-kpn-1.6.0/kpn_theme/css/theme.css`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/fonts/kpn-metric-bold.eot` & `mkdocs-kpn-1.6.0/kpn_theme/fonts/kpn-metric-bold.eot`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/fonts/kpn-metric-bold.svg` & `mkdocs-kpn-1.6.0/kpn_theme/fonts/kpn-metric-bold.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/fonts/kpn-metric-bold.ttf` & `mkdocs-kpn-1.6.0/kpn_theme/fonts/kpn-metric-bold.ttf`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/fonts/kpn-metric-bold.woff` & `mkdocs-kpn-1.6.0/kpn_theme/fonts/kpn-metric-bold.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/fonts/kpn-metric-light.eot` & `mkdocs-kpn-1.6.0/kpn_theme/fonts/kpn-metric-light.eot`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/fonts/kpn-metric-light.svg` & `mkdocs-kpn-1.6.0/kpn_theme/fonts/kpn-metric-light.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/fonts/kpn-metric-light.ttf` & `mkdocs-kpn-1.6.0/kpn_theme/fonts/kpn-metric-light.ttf`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/fonts/kpn-metric-light.woff` & `mkdocs-kpn-1.6.0/kpn_theme/fonts/kpn-metric-light.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/fonts/kpn-metric-normal.eot` & `mkdocs-kpn-1.6.0/kpn_theme/fonts/kpn-metric-normal.eot`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/fonts/kpn-metric-normal.svg` & `mkdocs-kpn-1.6.0/kpn_theme/fonts/kpn-metric-normal.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/fonts/kpn-metric-normal.ttf` & `mkdocs-kpn-1.6.0/kpn_theme/fonts/kpn-metric-normal.ttf`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/fonts/kpn-metric-normal.woff` & `mkdocs-kpn-1.6.0/kpn_theme/fonts/kpn-metric-normal.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/fonts/kpn-metric-semi-bold.eot` & `mkdocs-kpn-1.6.0/kpn_theme/fonts/kpn-metric-semi-bold.eot`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/fonts/kpn-metric-semi-bold.svg` & `mkdocs-kpn-1.6.0/kpn_theme/fonts/kpn-metric-semi-bold.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/fonts/kpn-metric-semi-bold.ttf` & `mkdocs-kpn-1.6.0/kpn_theme/fonts/kpn-metric-semi-bold.ttf`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/fonts/kpn-metric-semi-bold.woff` & `mkdocs-kpn-1.6.0/kpn_theme/fonts/kpn-metric-semi-bold.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/fonts/kpn-service-icons.eot` & `mkdocs-kpn-1.6.0/kpn_theme/fonts/kpn-service-icons.eot`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/fonts/kpn-service-icons.svg` & `mkdocs-kpn-1.6.0/kpn_theme/fonts/kpn-service-icons.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/fonts/kpn-service-icons.ttf` & `mkdocs-kpn-1.6.0/kpn_theme/fonts/kpn-service-icons.ttf`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/fonts/kpn-service-icons.woff` & `mkdocs-kpn-1.6.0/kpn_theme/fonts/kpn-service-icons.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/fonts/kpn-ui-icons.eot` & `mkdocs-kpn-1.6.0/kpn_theme/fonts/kpn-ui-icons.eot`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/fonts/kpn-ui-icons.svg` & `mkdocs-kpn-1.6.0/kpn_theme/fonts/kpn-ui-icons.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/fonts/kpn-ui-icons.ttf` & `mkdocs-kpn-1.6.0/kpn_theme/fonts/kpn-ui-icons.ttf`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/fonts/kpn-ui-icons.woff` & `mkdocs-kpn-1.6.0/kpn_theme/fonts/kpn-ui-icons.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/img/favicon.ico` & `mkdocs-kpn-1.6.0/kpn_theme/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/img/git-icon-black.png` & `mkdocs-kpn-1.6.0/kpn_theme/img/git-icon-black.png`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/img/git.svg` & `mkdocs-kpn-1.6.0/kpn_theme/img/git.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/img/logo-gitea.svg` & `mkdocs-kpn-1.6.0/kpn_theme/img/logo-gitea.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/img/logo-github.svg` & `mkdocs-kpn-1.6.0/kpn_theme/img/logo-github.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/img/logo-gitlab.svg` & `mkdocs-kpn-1.6.0/kpn_theme/img/logo-gitlab.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/img/logo-kpn.png` & `mkdocs-kpn-1.6.0/kpn_theme/img/logo-kpn.png`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/img/logo-kpn.svg` & `mkdocs-kpn-1.6.0/kpn_theme/img/logo-kpn.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/img/ui-bulb.svg` & `mkdocs-kpn-1.6.0/kpn_theme/img/ui-bulb.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/js/detail.js` & `mkdocs-kpn-1.6.0/kpn_theme/js/detail.js`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/js/highlight.min.js` & `mkdocs-kpn-1.6.0/kpn_theme/js/highlight.min.js`

 * *Files 23% similar despite different names*

#### js-beautify {}

```diff
@@ -1,103 +1,101 @@
 /*!
-  Highlight.js v11.7.0 (git: 82688fad18)
-  (c) 2006-2022 undefined and other contributors
+  Highlight.js v11.8.0 (git: 65687a907b)
+  (c) 2006-2023 undefined and other contributors
   License: BSD-3-Clause
  */
 var hljs = function() {
     "use strict";
-    var e = {
-        exports: {}
-    };
 
-    function n(e) {
-        return e instanceof Map ? e.clear = e.delete = e.set = () => {
+    function e(n) {
+        return n instanceof Map ? n.clear = n.delete = n.set = () => {
             throw Error("map is read-only")
-        } : e instanceof Set && (e.add = e.clear = e.delete = () => {
+        } : n instanceof Set && (n.add = n.clear = n.delete = () => {
             throw Error("set is read-only")
-        }), Object.freeze(e), Object.getOwnPropertyNames(e).forEach((t => {
-            var a = e[t];
-            "object" != typeof a || Object.isFrozen(a) || n(a)
-        })), e
+        }), Object.freeze(n), Object.getOwnPropertyNames(n).forEach((t => {
+            const a = n[t],
+                i = typeof a;
+            "object" !== i && "function" !== i || Object.isFrozen(a) || e(a)
+        })), n
     }
-    e.exports = n, e.exports.default = n;
-    class t {
+    class n {
         constructor(e) {
             void 0 === e.data && (e.data = {}), this.data = e.data, this.isMatchIgnored = !1
         }
         ignoreMatch() {
             this.isMatchIgnored = !0
         }
     }
 
-    function a(e) {
+    function t(e) {
         return e.replace(/&/g, "&amp;").replace(/</g, "&lt;").replace(/>/g, "&gt;").replace(/"/g, "&quot;").replace(/'/g, "&#x27;")
     }
 
-    function i(e, ...n) {
+    function a(e, ...n) {
         const t = Object.create(null);
         for (const n in e) t[n] = e[n];
         return n.forEach((e => {
             for (const n in e) t[n] = e[n]
         })), t
     }
-    const r = e => !!e.scope || e.sublanguage && e.language;
-    class s {
+    const i = e => !!e.scope;
+    class r {
         constructor(e, n) {
             this.buffer = "", this.classPrefix = n.classPrefix, e.walk(this)
         }
         addText(e) {
-            this.buffer += a(e)
+            this.buffer += t(e)
         }
         openNode(e) {
-            if (!r(e)) return;
-            let n = "";
-            n = e.sublanguage ? "language-" + e.language : ((e, {
+            if (!i(e)) return;
+            const n = ((e, {
                 prefix: n
             }) => {
+                if (e.startsWith("language:")) return e.replace("language:", "language-");
                 if (e.includes(".")) {
                     const t = e.split(".");
                     return [`${n}${t.shift()}`, ...t.map(((e, n) => `${e}${"_".repeat(n+1)}`))].join(" ")
                 }
                 return `${n}${e}`
             })(e.scope, {
                 prefix: this.classPrefix
-            }), this.span(n)
+            });
+            this.span(n)
         }
         closeNode(e) {
-            r(e) && (this.buffer += "</span>")
+            i(e) && (this.buffer += "</span>")
         }
         value() {
             return this.buffer
         }
         span(e) {
             this.buffer += `<span class="${e}">`
         }
     }
-    const o = (e = {}) => {
+    const s = (e = {}) => {
         const n = {
             children: []
         };
         return Object.assign(n, e), n
     };
-    class l {
+    class o {
         constructor() {
-            this.rootNode = o(), this.stack = [this.rootNode]
+            this.rootNode = s(), this.stack = [this.rootNode]
         }
         get top() {
             return this.stack[this.stack.length - 1]
         }
         get root() {
             return this.rootNode
         }
         add(e) {
             this.top.children.push(e)
         }
         openNode(e) {
-            const n = o({
+            const n = s({
                 scope: e
             });
             this.add(n), this.stack.push(n)
         }
         closeNode() {
             if (this.stack.length > 1) return this.stack.pop()
         }
@@ -112,372 +110,376 @@
         }
         static _walk(e, n) {
             return "string" == typeof n ? e.addText(n) : n.children && (e.openNode(n),
                 n.children.forEach((n => this._walk(e, n))), e.closeNode(n)), e
         }
         static _collapse(e) {
             "string" != typeof e && e.children && (e.children.every((e => "string" == typeof e)) ? e.children = [e.children.join("")] : e.children.forEach((e => {
-                l._collapse(e)
+                o._collapse(e)
             })))
         }
     }
-    class c extends l {
+    class l extends o {
         constructor(e) {
             super(), this.options = e
         }
-        addKeyword(e, n) {
-            "" !== e && (this.openNode(n), this.addText(e), this.closeNode())
-        }
         addText(e) {
             "" !== e && this.add(e)
         }
-        addSublanguage(e, n) {
+        startScope(e) {
+            this.openNode(e)
+        }
+        endScope() {
+            this.closeNode()
+        }
+        __addSublanguage(e, n) {
             const t = e.root;
-            t.sublanguage = !0, t.language = n, this.add(t)
+            n && (t.scope = "language:" + n), this.add(t)
         }
         toHTML() {
-            return new s(this, this.options).value()
+            return new r(this, this.options).value()
         }
         finalize() {
-            return !0
+            return this.closeAllNodes(), !0
         }
     }
 
-    function d(e) {
+    function c(e) {
         return e ? "string" == typeof e ? e : e.source : null
     }
 
+    function d(e) {
+        return b("(?=", e, ")")
+    }
+
     function g(e) {
-        return m("(?=", e, ")")
+        return b("(?:", e, ")*")
     }
 
     function u(e) {
-        return m("(?:", e, ")*")
+        return b("(?:", e, ")?")
     }
 
-    function b(e) {
-        return m("(?:", e, ")?")
+    function b(...e) {
+        return e.map((e => c(e))).join("")
     }
 
     function m(...e) {
-        return e.map((e => d(e))).join("")
-    }
-
-    function p(...e) {
         const n = (e => {
             const n = e[e.length - 1];
             return "object" == typeof n && n.constructor === Object ? (e.splice(e.length - 1, 1), n) : {}
         })(e);
-        return "(" + (n.capture ? "" : "?:") + e.map((e => d(e))).join("|") + ")"
+        return "(" + (n.capture ? "" : "?:") + e.map((e => c(e))).join("|") + ")"
     }
 
-    function _(e) {
+    function p(e) {
         return RegExp(e.toString() + "|").exec("").length - 1
     }
-    const h = /\[(?:[^\\\]]|\\.)*\]|\(\??|\\([1-9][0-9]*)|\\./;
+    const _ = /\[(?:[^\\\]]|\\.)*\]|\(\??|\\([1-9][0-9]*)|\\./;
 
-    function f(e, {
+    function h(e, {
         joinWith: n
     }) {
         let t = 0;
         return e.map((e => {
             t += 1;
             const n = t;
-            let a = d(e),
+            let a = c(e),
                 i = "";
             for (; a.length > 0;) {
-                const e = h.exec(a);
+                const e = _.exec(a);
                 if (!e) {
                     i += a;
                     break
                 }
                 i += a.substring(0, e.index),
                     a = a.substring(e.index + e[0].length), "\\" === e[0][0] && e[1] ? i += "\\" + (Number(e[1]) + n) : (i += e[0],
                         "(" === e[0] && t++)
             }
             return i
         })).map((e => `(${e})`)).join(n)
     }
-    const E = "[a-zA-Z]\\w*",
-        y = "[a-zA-Z_]\\w*",
-        w = "\\b\\d+(\\.\\d+)?",
+    const f = "[a-zA-Z]\\w*",
+        E = "[a-zA-Z_]\\w*",
+        y = "\\b\\d+(\\.\\d+)?",
         N = "(-?)(\\b0[xX][a-fA-F0-9]+|(\\b\\d+(\\.\\d*)?|\\.\\d+)([eE][-+]?\\d+)?)",
-        v = "\\b(0b[01]+)",
-        O = {
+        w = "\\b(0b[01]+)",
+        v = {
             begin: "\\\\[\\s\\S]",
             relevance: 0
         },
-        k = {
+        O = {
             scope: "string",
             begin: "'",
             end: "'",
             illegal: "\\n",
-            contains: [O]
+            contains: [v]
         },
-        x = {
+        k = {
             scope: "string",
             begin: '"',
             end: '"',
             illegal: "\\n",
-            contains: [O]
+            contains: [v]
         },
-        M = (e, n, t = {}) => {
-            const a = i({
+        x = (e, n, t = {}) => {
+            const i = a({
                 scope: "comment",
                 begin: e,
                 end: n,
                 contains: []
             }, t);
-            a.contains.push({
+            i.contains.push({
                 scope: "doctag",
                 begin: "[ ]*(?=(TODO|FIXME|NOTE|BUG|OPTIMIZE|HACK|XXX):)",
                 end: /(TODO|FIXME|NOTE|BUG|OPTIMIZE|HACK|XXX):/,
                 excludeBegin: !0,
                 relevance: 0
             });
-            const r = p("I", "a", "is", "so", "us", "to", "at", "if", "in", "it", "on", /[A-Za-z]+['](d|ve|re|ll|t|s|n)/, /[A-Za-z]+[-][a-z]+/, /[A-Za-z][a-z]{2,}/);
-            return a.contains.push({
-                begin: m(/[ ]+/, "(", r, /[.]?[:]?([.][ ]|[ ])/, "){3}")
-            }), a
-        },
-        S = M("//", "$"),
-        A = M("/\\*", "\\*/"),
-        C = M("#", "$");
-    var T = Object.freeze({
+            const r = m("I", "a", "is", "so", "us", "to", "at", "if", "in", "it", "on", /[A-Za-z]+['](d|ve|re|ll|t|s|n)/, /[A-Za-z]+[-][a-z]+/, /[A-Za-z][a-z]{2,}/);
+            return i.contains.push({
+                begin: b(/[ ]+/, "(", r, /[.]?[:]?([.][ ]|[ ])/, "){3}")
+            }), i
+        },
+        M = x("//", "$"),
+        S = x("/\\*", "\\*/"),
+        A = x("#", "$");
+    var C = Object.freeze({
         __proto__: null,
         MATCH_NOTHING_RE: /\b\B/,
-        IDENT_RE: E,
-        UNDERSCORE_IDENT_RE: y,
-        NUMBER_RE: w,
+        IDENT_RE: f,
+        UNDERSCORE_IDENT_RE: E,
+        NUMBER_RE: y,
         C_NUMBER_RE: N,
-        BINARY_NUMBER_RE: v,
+        BINARY_NUMBER_RE: w,
         RE_STARTERS_RE: "!|!=|!==|%|%=|&|&&|&=|\\*|\\*=|\\+|\\+=|,|-|-=|/=|/|:|;|<<|<<=|<=|<|===|==|=|>>>=|>>=|>=|>>>|>>|>|\\?|\\[|\\{|\\(|\\^|\\^=|\\||\\|=|\\|\\||~",
         SHEBANG: (e = {}) => {
             const n = /^#![ ]*\//;
-            return e.binary && (e.begin = m(n, /.*\b/, e.binary, /\b.*/)), i({
+            return e.binary && (e.begin = b(n, /.*\b/, e.binary, /\b.*/)), a({
                 scope: "meta",
                 begin: n,
                 end: /$/,
                 relevance: 0,
                 "on:begin": (e, n) => {
                     0 !== e.index && n.ignoreMatch()
                 }
             }, e)
         },
-        BACKSLASH_ESCAPE: O,
-        APOS_STRING_MODE: k,
-        QUOTE_STRING_MODE: x,
+        BACKSLASH_ESCAPE: v,
+        APOS_STRING_MODE: O,
+        QUOTE_STRING_MODE: k,
         PHRASAL_WORDS_MODE: {
             begin: /\b(a|an|the|are|I'm|isn't|don't|doesn't|won't|but|just|should|pretty|simply|enough|gonna|going|wtf|so|such|will|you|your|they|like|more)\b/
         },
-        COMMENT: M,
-        C_LINE_COMMENT_MODE: S,
-        C_BLOCK_COMMENT_MODE: A,
-        HASH_COMMENT_MODE: C,
+        COMMENT: x,
+        C_LINE_COMMENT_MODE: M,
+        C_BLOCK_COMMENT_MODE: S,
+        HASH_COMMENT_MODE: A,
         NUMBER_MODE: {
             scope: "number",
-            begin: w,
+            begin: y,
             relevance: 0
         },
         C_NUMBER_MODE: {
             scope: "number",
             begin: N,
             relevance: 0
         },
         BINARY_NUMBER_MODE: {
             scope: "number",
-            begin: v,
+            begin: w,
             relevance: 0
         },
         REGEXP_MODE: {
             begin: /(?=\/[^/\n]*\/)/,
             contains: [{
                 scope: "regexp",
                 begin: /\//,
                 end: /\/[gimuy]*/,
                 illegal: /\n/,
-                contains: [O, {
+                contains: [v, {
                     begin: /\[/,
                     end: /\]/,
                     relevance: 0,
-                    contains: [O]
+                    contains: [v]
                 }]
             }]
         },
         TITLE_MODE: {
             scope: "title",
-            begin: E,
+            begin: f,
             relevance: 0
         },
         UNDERSCORE_TITLE_MODE: {
             scope: "title",
-            begin: y,
+            begin: E,
             relevance: 0
         },
         METHOD_GUARD: {
-            begin: "\\.\\s*[a-zA-Z_]\\w*",
+            begin: "\\.\\s*" + E,
             relevance: 0
         },
         END_SAME_AS_BEGIN: e => Object.assign(e, {
             "on:begin": (e, n) => {
                 n.data._beginMatch = e[1]
             },
             "on:end": (e, n) => {
                 n.data._beginMatch !== e[1] && n.ignoreMatch()
             }
         })
     });
 
-    function R(e, n) {
+    function T(e, n) {
         "." === e.input[e.index - 1] && n.ignoreMatch()
     }
 
-    function D(e, n) {
+    function R(e, n) {
         void 0 !== e.className && (e.scope = e.className, delete e.className)
     }
 
-    function I(e, n) {
+    function D(e, n) {
         n && e.beginKeywords && (e.begin = "\\b(" + e.beginKeywords.split(" ").join("|") + ")(?!\\.)(?=\\b|\\s)",
-            e.__beforeBegin = R, e.keywords = e.keywords || e.beginKeywords, delete e.beginKeywords,
+            e.__beforeBegin = T, e.keywords = e.keywords || e.beginKeywords, delete e.beginKeywords,
             void 0 === e.relevance && (e.relevance = 0))
     }
 
-    function L(e, n) {
-        Array.isArray(e.illegal) && (e.illegal = p(...e.illegal))
+    function I(e, n) {
+        Array.isArray(e.illegal) && (e.illegal = m(...e.illegal))
     }
 
-    function B(e, n) {
+    function L(e, n) {
         if (e.match) {
             if (e.begin || e.end) throw Error("begin & end are not supported with match");
             e.begin = e.match, delete e.match
         }
     }
 
-    function $(e, n) {
+    function B(e, n) {
         void 0 === e.relevance && (e.relevance = 1)
     }
-    const z = (e, n) => {
+    const $ = (e, n) => {
             if (!e.beforeMatch) return;
             if (e.starts) throw Error("beforeMatch cannot be used with starts");
             const t = Object.assign({}, e);
             Object.keys(e).forEach((n => {
                 delete e[n]
-            })), e.keywords = t.keywords, e.begin = m(t.beforeMatch, g(t.begin)), e.starts = {
+            })), e.keywords = t.keywords, e.begin = b(t.beforeMatch, d(t.begin)), e.starts = {
                 relevance: 0,
                 contains: [Object.assign(t, {
                     endsParent: !0
                 })]
             }, e.relevance = 0, delete t.beforeMatch
         },
-        F = ["of", "and", "for", "in", "not", "or", "if", "then", "parent", "list", "value"];
+        z = ["of", "and", "for", "in", "not", "or", "if", "then", "parent", "list", "value"],
+        F = "keyword";
 
-    function U(e, n, t = "keyword") {
+    function U(e, n, t = F) {
         const a = Object.create(null);
         return "string" == typeof e ? i(t, e.split(" ")) : Array.isArray(e) ? i(t, e) : Object.keys(e).forEach((t => {
             Object.assign(a, U(e[t], n, t))
         })), a;
 
         function i(e, t) {
             n && (t = t.map((e => e.toLowerCase()))), t.forEach((n => {
                 const t = n.split("|");
                 a[t[0]] = [e, j(t[0], t[1])]
             }))
         }
     }
 
     function j(e, n) {
-        return n ? Number(n) : (e => F.includes(e.toLowerCase()))(e) ? 0 : 1
+        return n ? Number(n) : (e => z.includes(e.toLowerCase()))(e) ? 0 : 1
     }
     const P = {},
         K = e => {
             console.error(e)
         },
-        H = (e, ...n) => {
+        q = (e, ...n) => {
             console.log("WARN: " + e, ...n)
         },
-        q = (e, n) => {
+        H = (e, n) => {
             P[`${e}/${n}`] || (console.log(`Deprecated as of ${e}. ${n}`), P[`${e}/${n}`] = !0)
         },
-        Z = Error();
+        G = Error();
 
-    function G(e, n, {
+    function Z(e, n, {
         key: t
     }) {
         let a = 0;
         const i = e[t],
             r = {},
             s = {};
-        for (let e = 1; e <= n.length; e++) s[e + a] = i[e], r[e + a] = !0, a += _(n[e - 1]);
+        for (let e = 1; e <= n.length; e++) s[e + a] = i[e], r[e + a] = !0, a += p(n[e - 1]);
         e[t] = s, e[t]._emit = r, e[t]._multi = !0
     }
 
     function W(e) {
         (e => {
             e.scope && "object" == typeof e.scope && null !== e.scope && (e.beginScope = e.scope,
                 delete e.scope)
         })(e), "string" == typeof e.beginScope && (e.beginScope = {
             _wrap: e.beginScope
         }), "string" == typeof e.endScope && (e.endScope = {
             _wrap: e.endScope
         }), (e => {
             if (Array.isArray(e.begin)) {
                 if (e.skip || e.excludeBegin || e.returnBegin) throw K("skip, excludeBegin, returnBegin not compatible with beginScope: {}"),
-                    Z;
+                    G;
                 if ("object" != typeof e.beginScope || null === e.beginScope) throw K("beginScope must be object"),
-                    Z;
-                G(e, e.begin, {
+                    G;
+                Z(e, e.begin, {
                     key: "beginScope"
-                }), e.begin = f(e.begin, {
+                }), e.begin = h(e.begin, {
                     joinWith: ""
                 })
             }
         })(e), (e => {
             if (Array.isArray(e.end)) {
                 if (e.skip || e.excludeEnd || e.returnEnd) throw K("skip, excludeEnd, returnEnd not compatible with endScope: {}"),
-                    Z;
+                    G;
                 if ("object" != typeof e.endScope || null === e.endScope) throw K("endScope must be object"),
-                    Z;
-                G(e, e.end, {
+                    G;
+                Z(e, e.end, {
                     key: "endScope"
-                }), e.end = f(e.end, {
+                }), e.end = h(e.end, {
                     joinWith: ""
                 })
             }
         })(e)
     }
 
     function Q(e) {
         function n(n, t) {
-            return RegExp(d(n), "m" + (e.case_insensitive ? "i" : "") + (e.unicodeRegex ? "u" : "") + (t ? "g" : ""))
+            return RegExp(c(n), "m" + (e.case_insensitive ? "i" : "") + (e.unicodeRegex ? "u" : "") + (t ? "g" : ""))
         }
         class t {
             constructor() {
                 this.matchIndexes = {}, this.regexes = [], this.matchAt = 1, this.position = 0
             }
             addRule(e, n) {
                 n.position = this.position++, this.matchIndexes[this.matchAt] = n, this.regexes.push([n, e]),
-                    this.matchAt += _(e) + 1
+                    this.matchAt += p(e) + 1
             }
             compile() {
                 0 === this.regexes.length && (this.exec = () => null);
                 const e = this.regexes.map((e => e[1]));
-                this.matcherRe = n(f(e, {
+                this.matcherRe = n(h(e, {
                     joinWith: "|"
                 }), !0), this.lastIndex = 0
             }
             exec(e) {
                 this.matcherRe.lastIndex = this.lastIndex;
                 const n = this.matcherRe.exec(e);
                 if (!n) return null;
                 const t = n.findIndex(((e, n) => n > 0 && void 0 !== e)),
                     a = this.matchIndexes[t];
                 return n.splice(0, t), Object.assign(n, a)
             }
         }
-        class a {
+        class i {
             constructor() {
                 this.rules = [], this.multiRegexes = [],
                     this.count = 0, this.lastIndex = 0, this.regexIndex = 0
             }
             getMatcher(e) {
                 if (this.multiRegexes[e]) return this.multiRegexes[e];
                 const n = new t;
@@ -505,37 +507,37 @@
                     }
                 return t && (this.regexIndex += t.position + 1,
                     this.regexIndex === this.count && this.considerAll()), t
             }
         }
         if (e.compilerExtensions || (e.compilerExtensions = []),
             e.contains && e.contains.includes("self")) throw Error("ERR: contains `self` is not supported at the top-level of a language.  See documentation.");
-        return e.classNameAliases = i(e.classNameAliases || {}),
+        return e.classNameAliases = a(e.classNameAliases || {}),
             function t(r, s) {
                 const o = r;
                 if (r.isCompiled) return o;
-                [D, B, W, z].forEach((e => e(r, s))), e.compilerExtensions.forEach((e => e(r, s))),
-                    r.__beforeBegin = null, [I, L, $].forEach((e => e(r, s))), r.isCompiled = !0;
+                [R, L, W, $].forEach((e => e(r, s))), e.compilerExtensions.forEach((e => e(r, s))),
+                    r.__beforeBegin = null, [D, I, B].forEach((e => e(r, s))), r.isCompiled = !0;
                 let l = null;
                 return "object" == typeof r.keywords && r.keywords.$pattern && (r.keywords = Object.assign({}, r.keywords),
                         l = r.keywords.$pattern,
                         delete r.keywords.$pattern), l = l || /\w+/, r.keywords && (r.keywords = U(r.keywords, e.case_insensitive)),
                     o.keywordPatternRe = n(l, !0),
                     s && (r.begin || (r.begin = /\B|\b/), o.beginRe = n(o.begin), r.end || r.endsWithParent || (r.end = /\B|\b/),
                         r.end && (o.endRe = n(o.end)),
-                        o.terminatorEnd = d(o.end) || "", r.endsWithParent && s.terminatorEnd && (o.terminatorEnd += (r.end ? "|" : "") + s.terminatorEnd)),
+                        o.terminatorEnd = c(o.end) || "", r.endsWithParent && s.terminatorEnd && (o.terminatorEnd += (r.end ? "|" : "") + s.terminatorEnd)),
                     r.illegal && (o.illegalRe = n(r.illegal)),
-                    r.contains || (r.contains = []), r.contains = [].concat(...r.contains.map((e => (e => (e.variants && !e.cachedVariants && (e.cachedVariants = e.variants.map((n => i(e, {
+                    r.contains || (r.contains = []), r.contains = [].concat(...r.contains.map((e => (e => (e.variants && !e.cachedVariants && (e.cachedVariants = e.variants.map((n => a(e, {
                         variants: null
-                    }, n)))), e.cachedVariants ? e.cachedVariants : X(e) ? i(e, {
-                        starts: e.starts ? i(e.starts) : null
-                    }) : Object.isFrozen(e) ? i(e) : e))("self" === e ? r : e)))), r.contains.forEach((e => {
+                    }, n)))), e.cachedVariants ? e.cachedVariants : X(e) ? a(e, {
+                        starts: e.starts ? a(e.starts) : null
+                    }) : Object.isFrozen(e) ? a(e) : e))("self" === e ? r : e)))), r.contains.forEach((e => {
                         t(e, o)
                     })), r.starts && t(r.starts, s), o.matcher = (e => {
-                        const n = new a;
+                        const n = new i;
                         return e.contains.forEach((e => n.addRule(e.begin, {
                             rule: e,
                             type: "begin"
                         }))), e.terminatorEnd && n.addRule(e.terminatorEnd, {
                             type: "end"
                         }), e.illegal && n.addRule(e.illegal, {
                             type: "illegal"
@@ -548,422 +550,436 @@
         return !!e && (e.endsWithParent || X(e.starts))
     }
     class V extends Error {
         constructor(e, n) {
             super(e), this.name = "HTMLInjectionError", this.html = n
         }
     }
-    const J = a,
-        Y = i,
-        ee = Symbol("nomatch");
-    var ne = (n => {
-        const a = Object.create(null),
-            i = Object.create(null),
-            r = [];
-        let s = !0;
-        const o = "Could not find the language '{}', did you forget to load/include a language module?",
-            l = {
-                disableAutodetect: !0,
-                name: "Plain text",
-                contains: []
+    const J = t,
+        Y = a,
+        ee = Symbol("nomatch"),
+        ne = t => {
+            const a = Object.create(null),
+                i = Object.create(null),
+                r = [];
+            let s = !0;
+            const o = "Could not find the language '{}', did you forget to load/include a language module?",
+                c = {
+                    disableAutodetect: !0,
+                    name: "Plain text",
+                    contains: []
+                };
+            let p = {
+                ignoreUnescapedHTML: !1,
+                throwUnescapedHTML: !1,
+                noHighlightRe: /^(no-?highlight)$/i,
+                languageDetectRe: /\blang(?:uage)?-([\w-]+)\b/i,
+                classPrefix: "hljs-",
+                cssSelector: "pre code",
+                languages: null,
+                __emitter: l
             };
-        let d = {
-            ignoreUnescapedHTML: !1,
-            throwUnescapedHTML: !1,
-            noHighlightRe: /^(no-?highlight)$/i,
-            languageDetectRe: /\blang(?:uage)?-([\w-]+)\b/i,
-            classPrefix: "hljs-",
-            cssSelector: "pre code",
-            languages: null,
-            __emitter: c
-        };
-
-        function _(e) {
-            return d.noHighlightRe.test(e)
-        }
 
-        function h(e, n, t) {
-            let a = "",
-                i = "";
-            "object" == typeof n ? (a = e,
-                t = n.ignoreIllegals, i = n.language) : (q("10.7.0", "highlight(lang, code, ...args) has been deprecated."),
-                q("10.7.0", "Please use highlight(code, options) instead.\nhttps://github.com/highlightjs/highlight.js/issues/2277"),
-                i = e, a = n), void 0 === t && (t = !0);
-            const r = {
-                code: a,
-                language: i
-            };
-            x("before:highlight", r);
-            const s = r.result ? r.result : f(r.language, r.code, t);
-            return s.code = r.code, x("after:highlight", s), s
-        }
+            function _(e) {
+                return p.noHighlightRe.test(e)
+            }
 
-        function f(e, n, i, r) {
-            const l = Object.create(null);
+            function h(e, n, t) {
+                let a = "",
+                    i = "";
+                "object" == typeof n ? (a = e,
+                    t = n.ignoreIllegals, i = n.language) : (H("10.7.0", "highlight(lang, code, ...args) has been deprecated."),
+                    H("10.7.0", "Please use highlight(code, options) instead.\nhttps://github.com/highlightjs/highlight.js/issues/2277"),
+                    i = e, a = n), void 0 === t && (t = !0);
+                const r = {
+                    code: a,
+                    language: i
+                };
+                x("before:highlight", r);
+                const s = r.result ? r.result : f(r.language, r.code, t);
+                return s.code = r.code, x("after:highlight", s), s
+            }
+
+            function f(e, t, i, r) {
+                const l = Object.create(null);
+
+                function c() {
+                    if (!x.keywords) return void S.addText(A);
+                    let e = 0;
+                    x.keywordPatternRe.lastIndex = 0;
+                    let n = x.keywordPatternRe.exec(A),
+                        t = "";
+                    for (; n;) {
+                        t += A.substring(e, n.index);
+                        const i = w.case_insensitive ? n[0].toLowerCase() : n[0],
+                            r = (a = i, x.keywords[a]);
+                        if (r) {
+                            const [e, a] = r
+                            ;
+                            if (S.addText(t), t = "", l[i] = (l[i] || 0) + 1, l[i] <= 7 && (C += a), e.startsWith("_")) t += n[0];
+                            else {
+                                const t = w.classNameAliases[e] || e;
+                                g(n[0], t)
+                            }
+                        } else t += n[0];
+                        e = x.keywordPatternRe.lastIndex, n = x.keywordPatternRe.exec(A)
+                    }
+                    var a;
+                    t += A.substring(e), S.addText(t)
+                }
 
-            function c() {
-                if (!k.keywords) return void M.addText(S);
-                let e = 0;
-                k.keywordPatternRe.lastIndex = 0;
-                let n = k.keywordPatternRe.exec(S),
-                    t = "";
-                for (; n;) {
-                    t += S.substring(e, n.index);
-                    const i = w.case_insensitive ? n[0].toLowerCase() : n[0],
-                        r = (a = i, k.keywords[a]);
-                    if (r) {
-                        const [e, a] = r
-                        ;
-                        if (M.addText(t), t = "", l[i] = (l[i] || 0) + 1, l[i] <= 7 && (A += a), e.startsWith("_")) t += n[0];
-                        else {
-                            const t = w.classNameAliases[e] || e;
-                            M.addKeyword(n[0], t)
-                        }
-                    } else t += n[0];
-                    e = k.keywordPatternRe.lastIndex, n = k.keywordPatternRe.exec(S)
+                function d() {
+                    null != x.subLanguage ? (() => {
+                        if ("" === A) return;
+                        let e = null;
+                        if ("string" == typeof x.subLanguage) {
+                            if (!a[x.subLanguage]) return void S.addText(A);
+                            e = f(x.subLanguage, A, !0, M[x.subLanguage]), M[x.subLanguage] = e._top
+                        } else e = E(A, x.subLanguage.length ? x.subLanguage : null);
+                        x.relevance > 0 && (C += e.relevance), S.__addSublanguage(e._emitter, e.language)
+                    })() : c(), A = ""
                 }
-                var a;
-                t += S.substring(e), M.addText(t)
-            }
 
-            function g() {
-                null != k.subLanguage ? (() => {
-                    if ("" === S) return;
-                    let e = null;
-                    if ("string" == typeof k.subLanguage) {
-                        if (!a[k.subLanguage]) return void M.addText(S);
-                        e = f(k.subLanguage, S, !0, x[k.subLanguage]), x[k.subLanguage] = e._top
-                    } else e = E(S, k.subLanguage.length ? k.subLanguage : null);
-                    k.relevance > 0 && (A += e.relevance), M.addSublanguage(e._emitter, e.language)
-                })() : c(), S = ""
-            }
-
-            function u(e, n) {
-                let t = 1;
-                const a = n.length - 1;
-                for (; t <= a;) {
-                    if (!e._emit[t]) {
-                        t++;
-                        continue
-                    }
-                    const a = w.classNameAliases[e[t]] || e[t],
-                        i = n[t];
-                    a ? M.addKeyword(i, a) : (S = i, c(), S = ""), t++
+                function g(e, n) {
+                    "" !== e && (S.startScope(n), S.addText(e), S.endScope())
                 }
-            }
 
-            function b(e, n) {
-                return e.scope && "string" == typeof e.scope && M.openNode(w.classNameAliases[e.scope] || e.scope),
-                    e.beginScope && (e.beginScope._wrap ? (M.addKeyword(S, w.classNameAliases[e.beginScope._wrap] || e.beginScope._wrap),
-                        S = "") : e.beginScope._multi && (u(e.beginScope, n), S = "")), k = Object.create(e, {
-                        parent: {
-                            value: k
+                function u(e, n) {
+                    let t = 1;
+                    const a = n.length - 1;
+                    for (; t <= a;) {
+                        if (!e._emit[t]) {
+                            t++;
+                            continue
                         }
-                    }), k
-            }
-
-            function m(e, n, a) {
-                let i = ((e, n) => {
-                    const t = e && e.exec(n);
-                    return t && 0 === t.index
-                })(e.endRe, a);
-                if (i) {
-                    if (e["on:end"]) {
-                        const a = new t(e);
-                        e["on:end"](n, a), a.isMatchIgnored && (i = !1)
-                    }
-                    if (i) {
-                        for (; e.endsParent && e.parent;) e = e.parent;
-                        return e
+                        const a = w.classNameAliases[e[t]] || e[t],
+                            i = n[t];
+                        a ? g(i, a) : (A = i, c(), A = ""), t++
                     }
                 }
-                if (e.endsWithParent) return m(e.parent, n, a)
-            }
 
-            function p(e) {
-                return 0 === k.matcher.regexIndex ? (S += e[0], 1) : (R = !0, 0)
-            }
+                function b(e, n) {
+                    return e.scope && "string" == typeof e.scope && S.openNode(w.classNameAliases[e.scope] || e.scope),
+                        e.beginScope && (e.beginScope._wrap ? (g(A, w.classNameAliases[e.beginScope._wrap] || e.beginScope._wrap),
+                            A = "") : e.beginScope._multi && (u(e.beginScope, n), A = "")), x = Object.create(e, {
+                            parent: {
+                                value: x
+                            }
+                        }), x
+                }
 
-            function _(e) {
-                const t = e[0],
-                    a = n.substring(e.index),
-                    i = m(k, e, a);
-                if (!i) return ee;
-                const r = k;
-                k.endScope && k.endScope._wrap ? (g(),
-                    M.addKeyword(t, k.endScope._wrap)) : k.endScope && k.endScope._multi ? (g(),
-                    u(k.endScope, e)) : r.skip ? S += t : (r.returnEnd || r.excludeEnd || (S += t),
-                    g(), r.excludeEnd && (S = t));
-                do {
-                    k.scope && M.closeNode(), k.skip || k.subLanguage || (A += k.relevance), k = k.parent
-                } while (k !== i.parent);
-                return i.starts && b(i.starts, e), r.returnEnd ? 0 : t.length
-            }
-            let h = {};
-
-            function y(a, r) {
-                const o = r && r[0];
-                if (S += a, null == o) return g(), 0;
-                if ("begin" === h.type && "end" === r.type && h.index === r.index && "" === o) {
-                    if (S += n.slice(r.index, r.index + 1), !s) {
-                        const n = Error(`0 width match regex (${e})`);
-                        throw n.languageName = e, n.badRule = h.rule, n
+                function m(e, t, a) {
+                    let i = ((e, n) => {
+                        const t = e && e.exec(n);
+                        return t && 0 === t.index
+                    })(e.endRe, a);
+                    if (i) {
+                        if (e["on:end"]) {
+                            const a = new n(e);
+                            e["on:end"](t, a), a.isMatchIgnored && (i = !1)
+                        }
+                        if (i) {
+                            for (; e.endsParent && e.parent;) e = e.parent;
+                            return e
+                        }
                     }
-                    return 1
+                    if (e.endsWithParent) return m(e.parent, t, a)
                 }
-                if (h = r, "begin" === r.type) return (e => {
-                    const n = e[0],
-                        a = e.rule,
-                        i = new t(a),
-                        r = [a.__beforeBegin, a["on:begin"]];
-                    for (const t of r)
-                        if (t && (t(e, i), i.isMatchIgnored)) return p(n);
-                    return a.skip ? S += n : (a.excludeBegin && (S += n),
-                        g(), a.returnBegin || a.excludeBegin || (S = n)), b(a, e), a.returnBegin ? 0 : n.length
-                })(r);
-                if ("illegal" === r.type && !i) {
-                    const e = Error('Illegal lexeme "' + o + '" for mode "' + (k.scope || "<unnamed>") + '"');
-                    throw e.mode = k, e
-                }
-                if ("end" === r.type) {
-                    const e = _(r);
-                    if (e !== ee) return e
-                }
-                if ("illegal" === r.type && "" === o) return 1;
-                if (T > 1e5 && T > 3 * r.index) throw Error("potential infinite loop, way more iterations than matches");
-                return S += o, o.length
-            }
-            const w = v(e);
-            if (!w) throw K(o.replace("{}", e)), Error('Unknown language: "' + e + '"');
-            const N = Q(w);
-            let O = "",
-                k = r || N;
-            const x = {},
-                M = new d.__emitter(d);
-            (() => {
-                const e = [];
-                for (let n = k; n !== w; n = n.parent) n.scope && e.unshift(n.scope);
-                e.forEach((e => M.openNode(e)))
-            })();
-            let S = "",
-                A = 0,
-                C = 0,
-                T = 0,
-                R = !1;
-            try {
-                for (k.matcher.considerAll();;) {
-                    T++, R ? R = !1 : k.matcher.considerAll(), k.matcher.lastIndex = C;
-                    const e = k.matcher.exec(n);
-                    if (!e) break;
-                    const t = y(n.substring(C, e.index), e);
-                    C = e.index + t
+
+                function _(e) {
+                    return 0 === x.matcher.regexIndex ? (A += e[0], 1) : (D = !0, 0)
                 }
-                return y(n.substring(C)), M.closeAllNodes(), M.finalize(), O = M.toHTML(), {
-                    language: e,
-                    value: O,
-                    relevance: A,
-                    illegal: !1,
-                    _emitter: M,
-                    _top: k
+
+                function h(e) {
+                    const n = e[0],
+                        a = t.substring(e.index),
+                        i = m(x, e, a);
+                    if (!i) return ee;
+                    const r = x;
+                    x.endScope && x.endScope._wrap ? (d(),
+                        g(n, x.endScope._wrap)) : x.endScope && x.endScope._multi ? (d(),
+                        u(x.endScope, e)) : r.skip ? A += n : (r.returnEnd || r.excludeEnd || (A += n),
+                        d(), r.excludeEnd && (A = n));
+                    do {
+                        x.scope && S.closeNode(), x.skip || x.subLanguage || (C += x.relevance), x = x.parent
+                    } while (x !== i.parent);
+                    return i.starts && b(i.starts, e), r.returnEnd ? 0 : n.length
                 }
-            } catch (t) {
-                if (t.message && t.message.includes("Illegal")) return {
-                    language: e,
-                    value: J(n),
-                    illegal: !0,
-                    relevance: 0,
-                    _illegalBy: {
-                        message: t.message,
-                        index: C,
-                        context: n.slice(C - 100, C + 100),
-                        mode: t.mode,
-                        resultSoFar: O
-                    },
-                    _emitter: M
-                };
-                if (s) return {
-                    language: e,
-                    value: J(n),
-                    illegal: !1,
-                    relevance: 0,
-                    errorRaised: t,
-                    _emitter: M,
-                    _top: k
-                };
-                throw t
-            }
-        }
+                let y = {};
 
-        function E(e, n) {
-            n = n || d.languages || Object.keys(a);
-            const t = (e => {
-                    const n = {
-                        value: J(e),
+                function N(a, r) {
+                    const o = r && r[0];
+                    if (A += a, null == o) return d(), 0;
+                    if ("begin" === y.type && "end" === r.type && y.index === r.index && "" === o) {
+                        if (A += t.slice(r.index, r.index + 1), !s) {
+                            const n = Error(`0 width match regex (${e})`);
+                            throw n.languageName = e, n.badRule = y.rule, n
+                        }
+                        return 1
+                    }
+                    if (y = r, "begin" === r.type) return (e => {
+                        const t = e[0],
+                            a = e.rule,
+                            i = new n(a),
+                            r = [a.__beforeBegin, a["on:begin"]];
+                        for (const n of r)
+                            if (n && (n(e, i), i.isMatchIgnored)) return _(t);
+                        return a.skip ? A += t : (a.excludeBegin && (A += t),
+                            d(), a.returnBegin || a.excludeBegin || (A = t)), b(a, e), a.returnBegin ? 0 : t.length
+                    })(r);
+                    if ("illegal" === r.type && !i) {
+                        const e = Error('Illegal lexeme "' + o + '" for mode "' + (x.scope || "<unnamed>") + '"');
+                        throw e.mode = x, e
+                    }
+                    if ("end" === r.type) {
+                        const e = h(r);
+                        if (e !== ee) return e
+                    }
+                    if ("illegal" === r.type && "" === o) return 1;
+                    if (R > 1e5 && R > 3 * r.index) throw Error("potential infinite loop, way more iterations than matches");
+                    return A += o, o.length
+                }
+                const w = v(e);
+                if (!w) throw K(o.replace("{}", e)), Error('Unknown language: "' + e + '"');
+                const O = Q(w);
+                let k = "",
+                    x = r || O;
+                const M = {},
+                    S = new p.__emitter(p);
+                (() => {
+                    const e = [];
+                    for (let n = x; n !== w; n = n.parent) n.scope && e.unshift(n.scope);
+                    e.forEach((e => S.openNode(e)))
+                })();
+                let A = "",
+                    C = 0,
+                    T = 0,
+                    R = 0,
+                    D = !1;
+                try {
+                    if (w.__emitTokens) w.__emitTokens(t, S);
+                    else {
+                        for (x.matcher.considerAll();;) {
+                            R++, D ? D = !1 : x.matcher.considerAll(), x.matcher.lastIndex = T;
+                            const e = x.matcher.exec(t);
+                            if (!e) break;
+                            const n = N(t.substring(T, e.index), e);
+                            T = e.index + n
+                        }
+                        N(t.substring(T))
+                    }
+                    return S.finalize(), k = S.toHTML(), {
+                        language: e,
+                        value: k,
+                        relevance: C,
                         illegal: !1,
+                        _emitter: S,
+                        _top: x
+                    }
+                } catch (n) {
+                    if (n.message && n.message.includes("Illegal")) return {
+                        language: e,
+                        value: J(t),
+                        illegal: !0,
                         relevance: 0,
-                        _top: l,
-                        _emitter: new d.__emitter(d)
+                        _illegalBy: {
+                            message: n.message,
+                            index: T,
+                            context: t.slice(T - 100, T + 100),
+                            mode: n.mode,
+                            resultSoFar: k
+                        },
+                        _emitter: S
                     };
-                    return n._emitter.addText(e), n
-                })(e),
-                i = n.filter(v).filter(k).map((n => f(n, e, !1)));
-            i.unshift(t);
-            const r = i.sort(((e, n) => {
-                    if (e.relevance !== n.relevance) return n.relevance - e.relevance;
-                    if (e.language && n.language) {
-                        if (v(e.language).supersetOf === n.language) return 1;
-                        if (v(n.language).supersetOf === e.language) return -1
-                    }
-                    return 0
-                })),
-                [s, o] = r,
-                c = s;
-            return c.secondBest = o, c
-        }
-
-        function y(e) {
-            let n = null;
-            const t = (e => {
-                let n = e.className + " ";
-                n += e.parentNode ? e.parentNode.className : "";
-                const t = d.languageDetectRe.exec(n);
-                if (t) {
-                    const n = v(t[1]);
-                    return n || (H(o.replace("{}", t[1])),
-                        H("Falling back to no-highlight mode for this block.", e)), n ? t[1] : "no-highlight"
+                    if (s) return {
+                        language: e,
+                        value: J(t),
+                        illegal: !1,
+                        relevance: 0,
+                        errorRaised: n,
+                        _emitter: S,
+                        _top: x
+                    };
+                    throw n
                 }
-                return n.split(/\s+/).find((e => _(e) || v(e)))
-            })(e);
-            if (_(t)) return;
-            if (x("before:highlightElement", {
-                    el: e,
-                    language: t
-                }), e.children.length > 0 && (d.ignoreUnescapedHTML || (console.warn("One of your code blocks includes unescaped HTML. This is a potentially serious security risk."),
-                    console.warn("https://github.com/highlightjs/highlight.js/wiki/security"),
-                    console.warn("The element with unescaped HTML:"),
-                    console.warn(e)), d.throwUnescapedHTML)) throw new V("One of your code blocks includes unescaped HTML.", e.innerHTML);
-            n = e;
-            const a = n.textContent,
-                r = t ? h(a, {
-                    language: t,
-                    ignoreIllegals: !0
-                }) : E(a);
-            e.innerHTML = r.value, ((e, n, t) => {
-                const a = n && i[n] || t;
-                e.classList.add("hljs"), e.classList.add("language-" + a)
-            })(e, t, r.language), e.result = {
-                language: r.language,
-                re: r.relevance,
-                relevance: r.relevance
-            }, r.secondBest && (e.secondBest = {
-                language: r.secondBest.language,
-                relevance: r.secondBest.relevance
-            }), x("after:highlightElement", {
-                el: e,
-                result: r,
-                text: a
-            })
-        }
-        let w = !1;
-
-        function N() {
-            "loading" !== document.readyState ? document.querySelectorAll(d.cssSelector).forEach(y) : w = !0
-        }
+            }
 
-        function v(e) {
-            return e = (e || "").toLowerCase(), a[e] || a[i[e]]
-        }
+            function E(e, n) {
+                n = n || p.languages || Object.keys(a);
+                const t = (e => {
+                        const n = {
+                            value: J(e),
+                            illegal: !1,
+                            relevance: 0,
+                            _top: c,
+                            _emitter: new p.__emitter(p)
+                        };
+                        return n._emitter.addText(e), n
+                    })(e),
+                    i = n.filter(v).filter(k).map((n => f(n, e, !1)));
+                i.unshift(t);
+                const r = i.sort(((e, n) => {
+                        if (e.relevance !== n.relevance) return n.relevance - e.relevance;
+                        if (e.language && n.language) {
+                            if (v(e.language).supersetOf === n.language) return 1;
+                            if (v(n.language).supersetOf === e.language) return -1
+                        }
+                        return 0
+                    })),
+                    [s, o] = r,
+                    l = s;
+                return l.secondBest = o, l
+            }
+
+            function y(e) {
+                let n = null;
+                const t = (e => {
+                    let n = e.className + " ";
+                    n += e.parentNode ? e.parentNode.className : "";
+                    const t = p.languageDetectRe.exec(n);
+                    if (t) {
+                        const n = v(t[1]);
+                        return n || (q(o.replace("{}", t[1])),
+                            q("Falling back to no-highlight mode for this block.", e)), n ? t[1] : "no-highlight"
+                    }
+                    return n.split(/\s+/).find((e => _(e) || v(e)))
+                })(e);
+                if (_(t)) return;
+                if (x("before:highlightElement", {
+                        el: e,
+                        language: t
+                    }), e.children.length > 0 && (p.ignoreUnescapedHTML || (console.warn("One of your code blocks includes unescaped HTML. This is a potentially serious security risk."),
+                        console.warn("https://github.com/highlightjs/highlight.js/wiki/security"),
+                        console.warn("The element with unescaped HTML:"),
+                        console.warn(e)), p.throwUnescapedHTML)) throw new V("One of your code blocks includes unescaped HTML.", e.innerHTML);
+                n = e;
+                const a = n.textContent,
+                    r = t ? h(a, {
+                        language: t,
+                        ignoreIllegals: !0
+                    }) : E(a);
+                e.innerHTML = r.value, ((e, n, t) => {
+                    const a = n && i[n] || t;
+                    e.classList.add("hljs"), e.classList.add("language-" + a)
+                })(e, t, r.language), e.result = {
+                    language: r.language,
+                    re: r.relevance,
+                    relevance: r.relevance
+                }, r.secondBest && (e.secondBest = {
+                    language: r.secondBest.language,
+                    relevance: r.secondBest.relevance
+                }), x("after:highlightElement", {
+                    el: e,
+                    result: r,
+                    text: a
+                })
+            }
+            let N = !1;
 
-        function O(e, {
-            languageName: n
-        }) {
-            "string" == typeof e && (e = [e]), e.forEach((e => {
-                i[e.toLowerCase()] = n
-            }))
-        }
+            function w() {
+                "loading" !== document.readyState ? document.querySelectorAll(p.cssSelector).forEach(y) : N = !0
+            }
 
-        function k(e) {
-            const n = v(e);
-            return n && !n.disableAutodetect
-        }
+            function v(e) {
+                return e = (e || "").toLowerCase(), a[e] || a[i[e]]
+            }
 
-        function x(e, n) {
-            const t = e;
-            r.forEach((e => {
-                e[t] && e[t](n)
-            }))
-        }
-        "undefined" != typeof window && window.addEventListener && window.addEventListener("DOMContentLoaded", (() => {
-            w && N()
-        }), !1), Object.assign(n, {
-            highlight: h,
-            highlightAuto: E,
-            highlightAll: N,
-            highlightElement: y,
-            highlightBlock: e => (q("10.7.0", "highlightBlock will be removed entirely in v12.0"),
-                q("10.7.0", "Please use highlightElement now."), y(e)),
-            configure: e => {
-                d = Y(d, e)
-            },
-            initHighlighting: () => {
-                N(), q("10.6.0", "initHighlighting() deprecated.  Use highlightAll() now.")
-            },
-            initHighlightingOnLoad: () => {
-                N(), q("10.6.0", "initHighlightingOnLoad() deprecated.  Use highlightAll() now.")
-            },
-            registerLanguage: (e, t) => {
-                let i = null;
-                try {
-                    i = t(n)
-                } catch (n) {
-                    if (K("Language definition for '{}' could not be registered.".replace("{}", e)),
-                        !s) throw n;
-                    K(n), i = l
-                }
-                i.name || (i.name = e), a[e] = i, i.rawDefinition = t.bind(null, n), i.aliases && O(i.aliases, {
-                    languageName: e
-                })
-            },
-            unregisterLanguage: e => {
-                delete a[e];
-                for (const n of Object.keys(i)) i[n] === e && delete i[n]
-            },
-            listLanguages: () => Object.keys(a),
-            getLanguage: v,
-            registerAliases: O,
-            autoDetection: k,
-            inherit: Y,
-            addPlugin: e => {
-                (e => {
-                    e["before:highlightBlock"] && !e["before:highlightElement"] && (e["before:highlightElement"] = n => {
-                        e["before:highlightBlock"](Object.assign({
-                            block: n.el
-                        }, n))
-                    }), e["after:highlightBlock"] && !e["after:highlightElement"] && (e["after:highlightElement"] = n => {
-                        e["after:highlightBlock"](Object.assign({
-                            block: n.el
-                        }, n))
+            function O(e, {
+                languageName: n
+            }) {
+                "string" == typeof e && (e = [e]), e.forEach((e => {
+                    i[e.toLowerCase()] = n
+                }))
+            }
+
+            function k(e) {
+                const n = v(e);
+                return n && !n.disableAutodetect
+            }
+
+            function x(e, n) {
+                const t = e;
+                r.forEach((e => {
+                    e[t] && e[t](n)
+                }))
+            }
+            "undefined" != typeof window && window.addEventListener && window.addEventListener("DOMContentLoaded", (() => {
+                N && w()
+            }), !1), Object.assign(t, {
+                highlight: h,
+                highlightAuto: E,
+                highlightAll: w,
+                highlightElement: y,
+                highlightBlock: e => (H("10.7.0", "highlightBlock will be removed entirely in v12.0"),
+                    H("10.7.0", "Please use highlightElement now."), y(e)),
+                configure: e => {
+                    p = Y(p, e)
+                },
+                initHighlighting: () => {
+                    w(), H("10.6.0", "initHighlighting() deprecated.  Use highlightAll() now.")
+                },
+                initHighlightingOnLoad: () => {
+                    w(), H("10.6.0", "initHighlightingOnLoad() deprecated.  Use highlightAll() now.")
+                },
+                registerLanguage: (e, n) => {
+                    let i = null;
+                    try {
+                        i = n(t)
+                    } catch (n) {
+                        if (K("Language definition for '{}' could not be registered.".replace("{}", e)),
+                            !s) throw n;
+                        K(n), i = c
+                    }
+                    i.name || (i.name = e), a[e] = i, i.rawDefinition = n.bind(null, t), i.aliases && O(i.aliases, {
+                        languageName: e
                     })
-                })(e), r.push(e)
-            }
-        }), n.debugMode = () => {
-            s = !1
-        }, n.safeMode = () => {
-            s = !0
-        }, n.versionString = "11.7.0", n.regex = {
-            concat: m,
-            lookahead: g,
-            either: p,
-            optional: b,
-            anyNumberOfTimes: u
-        };
-        for (const n in T) "object" == typeof T[n] && e.exports(T[n]);
-        return Object.assign(n, T), n
-    })({});
-    const te = e => ({
+                },
+                unregisterLanguage: e => {
+                    delete a[e];
+                    for (const n of Object.keys(i)) i[n] === e && delete i[n]
+                },
+                listLanguages: () => Object.keys(a),
+                getLanguage: v,
+                registerAliases: O,
+                autoDetection: k,
+                inherit: Y,
+                addPlugin: e => {
+                    (e => {
+                        e["before:highlightBlock"] && !e["before:highlightElement"] && (e["before:highlightElement"] = n => {
+                            e["before:highlightBlock"](Object.assign({
+                                block: n.el
+                            }, n))
+                        }), e["after:highlightBlock"] && !e["after:highlightElement"] && (e["after:highlightElement"] = n => {
+                            e["after:highlightBlock"](Object.assign({
+                                block: n.el
+                            }, n))
+                        })
+                    })(e), r.push(e)
+                },
+                removePlugin: e => {
+                    const n = r.indexOf(e); - 1 !== n && r.splice(n, 1)
+                }
+            }), t.debugMode = () => {
+                s = !1
+            }, t.safeMode = () => {
+                s = !0
+            }, t.versionString = "11.8.0", t.regex = {
+                concat: b,
+                lookahead: d,
+                either: m,
+                optional: u,
+                anyNumberOfTimes: g
+            };
+            for (const n in C) "object" == typeof C[n] && e(C[n]);
+            return Object.assign(t, C), t
+        },
+        te = ne({});
+    te.newInstance = () => ne({});
+    var ae = te;
+    const ie = e => ({
             IMPORTANT: {
                 scope: "meta",
                 begin: "!important"
             },
             BLOCK_COMMENT: e.C_BLOCK_COMMENT_MODE,
             HEXCOLOR: {
                 scope: "number",
@@ -986,61 +1002,62 @@
                 relevance: 0
             },
             CSS_VARIABLE: {
                 className: "attr",
                 begin: /--[A-Za-z][A-Za-z0-9_-]*/
             }
         }),
-        ae = ["a", "abbr", "address", "article", "aside", "audio", "b", "blockquote", "body", "button", "canvas", "caption", "cite", "code", "dd", "del", "details", "dfn", "div", "dl", "dt", "em", "fieldset", "figcaption", "figure", "footer", "form", "h1", "h2", "h3", "h4", "h5", "h6", "header", "hgroup", "html", "i", "iframe", "img", "input", "ins", "kbd", "label", "legend", "li", "main", "mark", "menu", "nav", "object", "ol", "p", "q", "quote", "samp", "section", "span", "strong", "summary", "sup", "table", "tbody", "td", "textarea", "tfoot", "th", "thead", "time", "tr", "ul", "var", "video"],
-        ie = ["any-hover", "any-pointer", "aspect-ratio", "color", "color-gamut", "color-index", "device-aspect-ratio", "device-height", "device-width", "display-mode", "forced-colors", "grid", "height", "hover", "inverted-colors", "monochrome", "orientation", "overflow-block", "overflow-inline", "pointer", "prefers-color-scheme", "prefers-contrast", "prefers-reduced-motion", "prefers-reduced-transparency", "resolution", "scan", "scripting", "update", "width", "min-width", "max-width", "min-height", "max-height"],
-        re = ["active", "any-link", "blank", "checked", "current", "default", "defined", "dir", "disabled", "drop", "empty", "enabled", "first", "first-child", "first-of-type", "fullscreen", "future", "focus", "focus-visible", "focus-within", "has", "host", "host-context", "hover", "indeterminate", "in-range", "invalid", "is", "lang", "last-child", "last-of-type", "left", "link", "local-link", "not", "nth-child", "nth-col", "nth-last-child", "nth-last-col", "nth-last-of-type", "nth-of-type", "only-child", "only-of-type", "optional", "out-of-range", "past", "placeholder-shown", "read-only", "read-write", "required", "right", "root", "scope", "target", "target-within", "user-invalid", "valid", "visited", "where"],
-        se = ["after", "backdrop", "before", "cue", "cue-region", "first-letter", "first-line", "grammar-error", "marker", "part", "placeholder", "selection", "slotted", "spelling-error"],
-        oe = ["align-content", "align-items", "align-self", "all", "animation", "animation-delay", "animation-direction", "animation-duration", "animation-fill-mode", "animation-iteration-count", "animation-name", "animation-play-state", "animation-timing-function", "backface-visibility", "background", "background-attachment", "background-blend-mode", "background-clip", "background-color", "background-image", "background-origin", "background-position", "background-repeat", "background-size", "block-size", "border", "border-block", "border-block-color", "border-block-end", "border-block-end-color", "border-block-end-style", "border-block-end-width", "border-block-start", "border-block-start-color", "border-block-start-style", "border-block-start-width", "border-block-style", "border-block-width", "border-bottom", "border-bottom-color", "border-bottom-left-radius", "border-bottom-right-radius", "border-bottom-style", "border-bottom-width", "border-collapse", "border-color", "border-image", "border-image-outset", "border-image-repeat", "border-image-slice", "border-image-source", "border-image-width", "border-inline", "border-inline-color", "border-inline-end", "border-inline-end-color", "border-inline-end-style", "border-inline-end-width", "border-inline-start", "border-inline-start-color", "border-inline-start-style", "border-inline-start-width", "border-inline-style", "border-inline-width", "border-left", "border-left-color", "border-left-style", "border-left-width", "border-radius", "border-right", "border-right-color", "border-right-style", "border-right-width", "border-spacing", "border-style", "border-top", "border-top-color", "border-top-left-radius", "border-top-right-radius", "border-top-style", "border-top-width", "border-width", "bottom", "box-decoration-break", "box-shadow", "box-sizing", "break-after", "break-before", "break-inside", "caption-side", "caret-color", "clear", "clip", "clip-path", "clip-rule", "color", "column-count", "column-fill", "column-gap", "column-rule", "column-rule-color", "column-rule-style", "column-rule-width", "column-span", "column-width", "columns", "contain", "content", "content-visibility", "counter-increment", "counter-reset", "cue", "cue-after", "cue-before", "cursor", "direction", "display", "empty-cells", "filter", "flex", "flex-basis", "flex-direction", "flex-flow", "flex-grow", "flex-shrink", "flex-wrap", "float", "flow", "font", "font-display", "font-family", "font-feature-settings", "font-kerning", "font-language-override", "font-size", "font-size-adjust", "font-smoothing", "font-stretch", "font-style", "font-synthesis", "font-variant", "font-variant-caps", "font-variant-east-asian", "font-variant-ligatures", "font-variant-numeric", "font-variant-position", "font-variation-settings", "font-weight", "gap", "glyph-orientation-vertical", "grid", "grid-area", "grid-auto-columns", "grid-auto-flow", "grid-auto-rows", "grid-column", "grid-column-end", "grid-column-start", "grid-gap", "grid-row", "grid-row-end", "grid-row-start", "grid-template", "grid-template-areas", "grid-template-columns", "grid-template-rows", "hanging-punctuation", "height", "hyphens", "icon", "image-orientation", "image-rendering", "image-resolution", "ime-mode", "inline-size", "isolation", "justify-content", "left", "letter-spacing", "line-break", "line-height", "list-style", "list-style-image", "list-style-position", "list-style-type", "margin", "margin-block", "margin-block-end", "margin-block-start", "margin-bottom", "margin-inline", "margin-inline-end", "margin-inline-start", "margin-left", "margin-right", "margin-top", "marks", "mask", "mask-border", "mask-border-mode", "mask-border-outset", "mask-border-repeat", "mask-border-slice", "mask-border-source", "mask-border-width", "mask-clip", "mask-composite", "mask-image", "mask-mode", "mask-origin", "mask-position", "mask-repeat", "mask-size", "mask-type", "max-block-size", "max-height", "max-inline-size", "max-width", "min-block-size", "min-height", "min-inline-size", "min-width", "mix-blend-mode", "nav-down", "nav-index", "nav-left", "nav-right", "nav-up", "none", "normal", "object-fit", "object-position", "opacity", "order", "orphans", "outline", "outline-color", "outline-offset", "outline-style", "outline-width", "overflow", "overflow-wrap", "overflow-x", "overflow-y", "padding", "padding-block", "padding-block-end", "padding-block-start", "padding-bottom", "padding-inline", "padding-inline-end", "padding-inline-start", "padding-left", "padding-right", "padding-top", "page-break-after", "page-break-before", "page-break-inside", "pause", "pause-after", "pause-before", "perspective", "perspective-origin", "pointer-events", "position", "quotes", "resize", "rest", "rest-after", "rest-before", "right", "row-gap", "scroll-margin", "scroll-margin-block", "scroll-margin-block-end", "scroll-margin-block-start", "scroll-margin-bottom", "scroll-margin-inline", "scroll-margin-inline-end", "scroll-margin-inline-start", "scroll-margin-left", "scroll-margin-right", "scroll-margin-top", "scroll-padding", "scroll-padding-block", "scroll-padding-block-end", "scroll-padding-block-start", "scroll-padding-bottom", "scroll-padding-inline", "scroll-padding-inline-end", "scroll-padding-inline-start", "scroll-padding-left", "scroll-padding-right", "scroll-padding-top", "scroll-snap-align", "scroll-snap-stop", "scroll-snap-type", "scrollbar-color", "scrollbar-gutter", "scrollbar-width", "shape-image-threshold", "shape-margin", "shape-outside", "speak", "speak-as", "src", "tab-size", "table-layout", "text-align", "text-align-all", "text-align-last", "text-combine-upright", "text-decoration", "text-decoration-color", "text-decoration-line", "text-decoration-style", "text-emphasis", "text-emphasis-color", "text-emphasis-position", "text-emphasis-style", "text-indent", "text-justify", "text-orientation", "text-overflow", "text-rendering", "text-shadow", "text-transform", "text-underline-position", "top", "transform", "transform-box", "transform-origin", "transform-style", "transition", "transition-delay", "transition-duration", "transition-property", "transition-timing-function", "unicode-bidi", "vertical-align", "visibility", "voice-balance", "voice-duration", "voice-family", "voice-pitch", "voice-range", "voice-rate", "voice-stress", "voice-volume", "white-space", "widows", "width", "will-change", "word-break", "word-spacing", "word-wrap", "writing-mode", "z-index"].reverse(),
-        le = re.concat(se);
-    var ce = "\\.([0-9](_*[0-9])*)",
-        de = "[0-9a-fA-F](_*[0-9a-fA-F])*",
-        ge = {
+        re = ["a", "abbr", "address", "article", "aside", "audio", "b", "blockquote", "body", "button", "canvas", "caption", "cite", "code", "dd", "del", "details", "dfn", "div", "dl", "dt", "em", "fieldset", "figcaption", "figure", "footer", "form", "h1", "h2", "h3", "h4", "h5", "h6", "header", "hgroup", "html", "i", "iframe", "img", "input", "ins", "kbd", "label", "legend", "li", "main", "mark", "menu", "nav", "object", "ol", "p", "q", "quote", "samp", "section", "span", "strong", "summary", "sup", "table", "tbody", "td", "textarea", "tfoot", "th", "thead", "time", "tr", "ul", "var", "video"],
+        se = ["any-hover", "any-pointer", "aspect-ratio", "color", "color-gamut", "color-index", "device-aspect-ratio", "device-height", "device-width", "display-mode", "forced-colors", "grid", "height", "hover", "inverted-colors", "monochrome", "orientation", "overflow-block", "overflow-inline", "pointer", "prefers-color-scheme", "prefers-contrast", "prefers-reduced-motion", "prefers-reduced-transparency", "resolution", "scan", "scripting", "update", "width", "min-width", "max-width", "min-height", "max-height"],
+        oe = ["active", "any-link", "blank", "checked", "current", "default", "defined", "dir", "disabled", "drop", "empty", "enabled", "first", "first-child", "first-of-type", "fullscreen", "future", "focus", "focus-visible", "focus-within", "has", "host", "host-context", "hover", "indeterminate", "in-range", "invalid", "is", "lang", "last-child", "last-of-type", "left", "link", "local-link", "not", "nth-child", "nth-col", "nth-last-child", "nth-last-col", "nth-last-of-type", "nth-of-type", "only-child", "only-of-type", "optional", "out-of-range", "past", "placeholder-shown", "read-only", "read-write", "required", "right", "root", "scope", "target", "target-within", "user-invalid", "valid", "visited", "where"],
+        le = ["after", "backdrop", "before", "cue", "cue-region", "first-letter", "first-line", "grammar-error", "marker", "part", "placeholder", "selection", "slotted", "spelling-error"],
+        ce = ["align-content", "align-items", "align-self", "all", "animation", "animation-delay", "animation-direction", "animation-duration", "animation-fill-mode", "animation-iteration-count", "animation-name", "animation-play-state", "animation-timing-function", "backface-visibility", "background", "background-attachment", "background-blend-mode", "background-clip", "background-color", "background-image", "background-origin", "background-position", "background-repeat", "background-size", "block-size", "border", "border-block", "border-block-color", "border-block-end", "border-block-end-color", "border-block-end-style", "border-block-end-width", "border-block-start", "border-block-start-color", "border-block-start-style", "border-block-start-width", "border-block-style", "border-block-width", "border-bottom", "border-bottom-color", "border-bottom-left-radius", "border-bottom-right-radius", "border-bottom-style", "border-bottom-width", "border-collapse", "border-color", "border-image", "border-image-outset", "border-image-repeat", "border-image-slice", "border-image-source", "border-image-width", "border-inline", "border-inline-color", "border-inline-end", "border-inline-end-color", "border-inline-end-style", "border-inline-end-width", "border-inline-start", "border-inline-start-color", "border-inline-start-style", "border-inline-start-width", "border-inline-style", "border-inline-width", "border-left", "border-left-color", "border-left-style", "border-left-width", "border-radius", "border-right", "border-right-color", "border-right-style", "border-right-width", "border-spacing", "border-style", "border-top", "border-top-color", "border-top-left-radius", "border-top-right-radius", "border-top-style", "border-top-width", "border-width", "bottom", "box-decoration-break", "box-shadow", "box-sizing", "break-after", "break-before", "break-inside", "caption-side", "caret-color", "clear", "clip", "clip-path", "clip-rule", "color", "column-count", "column-fill", "column-gap", "column-rule", "column-rule-color", "column-rule-style", "column-rule-width", "column-span", "column-width", "columns", "contain", "content", "content-visibility", "counter-increment", "counter-reset", "cue", "cue-after", "cue-before", "cursor", "direction", "display", "empty-cells", "filter", "flex", "flex-basis", "flex-direction", "flex-flow", "flex-grow", "flex-shrink", "flex-wrap", "float", "flow", "font", "font-display", "font-family", "font-feature-settings", "font-kerning", "font-language-override", "font-size", "font-size-adjust", "font-smoothing", "font-stretch", "font-style", "font-synthesis", "font-variant", "font-variant-caps", "font-variant-east-asian", "font-variant-ligatures", "font-variant-numeric", "font-variant-position", "font-variation-settings", "font-weight", "gap", "glyph-orientation-vertical", "grid", "grid-area", "grid-auto-columns", "grid-auto-flow", "grid-auto-rows", "grid-column", "grid-column-end", "grid-column-start", "grid-gap", "grid-row", "grid-row-end", "grid-row-start", "grid-template", "grid-template-areas", "grid-template-columns", "grid-template-rows", "hanging-punctuation", "height", "hyphens", "icon", "image-orientation", "image-rendering", "image-resolution", "ime-mode", "inline-size", "isolation", "justify-content", "left", "letter-spacing", "line-break", "line-height", "list-style", "list-style-image", "list-style-position", "list-style-type", "margin", "margin-block", "margin-block-end", "margin-block-start", "margin-bottom", "margin-inline", "margin-inline-end", "margin-inline-start", "margin-left", "margin-right", "margin-top", "marks", "mask", "mask-border", "mask-border-mode", "mask-border-outset", "mask-border-repeat", "mask-border-slice", "mask-border-source", "mask-border-width", "mask-clip", "mask-composite", "mask-image", "mask-mode", "mask-origin", "mask-position", "mask-repeat", "mask-size", "mask-type", "max-block-size", "max-height", "max-inline-size", "max-width", "min-block-size", "min-height", "min-inline-size", "min-width", "mix-blend-mode", "nav-down", "nav-index", "nav-left", "nav-right", "nav-up", "none", "normal", "object-fit", "object-position", "opacity", "order", "orphans", "outline", "outline-color", "outline-offset", "outline-style", "outline-width", "overflow", "overflow-wrap", "overflow-x", "overflow-y", "padding", "padding-block", "padding-block-end", "padding-block-start", "padding-bottom", "padding-inline", "padding-inline-end", "padding-inline-start", "padding-left", "padding-right", "padding-top", "page-break-after", "page-break-before", "page-break-inside", "pause", "pause-after", "pause-before", "perspective", "perspective-origin", "pointer-events", "position", "quotes", "resize", "rest", "rest-after", "rest-before", "right", "row-gap", "scroll-margin", "scroll-margin-block", "scroll-margin-block-end", "scroll-margin-block-start", "scroll-margin-bottom", "scroll-margin-inline", "scroll-margin-inline-end", "scroll-margin-inline-start", "scroll-margin-left", "scroll-margin-right", "scroll-margin-top", "scroll-padding", "scroll-padding-block", "scroll-padding-block-end", "scroll-padding-block-start", "scroll-padding-bottom", "scroll-padding-inline", "scroll-padding-inline-end", "scroll-padding-inline-start", "scroll-padding-left", "scroll-padding-right", "scroll-padding-top", "scroll-snap-align", "scroll-snap-stop", "scroll-snap-type", "scrollbar-color", "scrollbar-gutter", "scrollbar-width", "shape-image-threshold", "shape-margin", "shape-outside", "speak", "speak-as", "src", "tab-size", "table-layout", "text-align", "text-align-all", "text-align-last", "text-combine-upright", "text-decoration", "text-decoration-color", "text-decoration-line", "text-decoration-style", "text-emphasis", "text-emphasis-color", "text-emphasis-position", "text-emphasis-style", "text-indent", "text-justify", "text-orientation", "text-overflow", "text-rendering", "text-shadow", "text-transform", "text-underline-position", "top", "transform", "transform-box", "transform-origin", "transform-style", "transition", "transition-delay", "transition-duration", "transition-property", "transition-timing-function", "unicode-bidi", "vertical-align", "visibility", "voice-balance", "voice-duration", "voice-family", "voice-pitch", "voice-range", "voice-rate", "voice-stress", "voice-volume", "white-space", "widows", "width", "will-change", "word-break", "word-spacing", "word-wrap", "writing-mode", "z-index"].reverse(),
+        de = oe.concat(le);
+    var ge = "[0-9](_*[0-9])*",
+        ue = `\\.(${ge})`,
+        be = "[0-9a-fA-F](_*[0-9a-fA-F])*",
+        me = {
             className: "number",
             variants: [{
-                begin: `(\\b([0-9](_*[0-9])*)((${ce})|\\.)?|(${ce}))[eE][+-]?([0-9](_*[0-9])*)[fFdD]?\\b`
+                begin: `(\\b(${ge})((${ue})|\\.)?|(${ue}))[eE][+-]?(${ge})[fFdD]?\\b`
             }, {
-                begin: `\\b([0-9](_*[0-9])*)((${ce})[fFdD]?\\b|\\.([fFdD]\\b)?)`
+                begin: `\\b(${ge})((${ue})[fFdD]?\\b|\\.([fFdD]\\b)?)`
             }, {
-                begin: `(${ce})[fFdD]?\\b`
+                begin: `(${ue})[fFdD]?\\b`
             }, {
-                begin: "\\b([0-9](_*[0-9])*)[fFdD]\\b"
+                begin: `\\b(${ge})[fFdD]\\b`
             }, {
-                begin: `\\b0[xX]((${de})\\.?|(${de})?\\.(${de}))[pP][+-]?([0-9](_*[0-9])*)[fFdD]?\\b`
+                begin: `\\b0[xX]((${be})\\.?|(${be})?\\.(${be}))[pP][+-]?(${ge})[fFdD]?\\b`
             }, {
                 begin: "\\b(0|[1-9](_*[0-9])*)[lL]?\\b"
             }, {
-                begin: `\\b0[xX](${de})[lL]?\\b`
+                begin: `\\b0[xX](${be})[lL]?\\b`
             }, {
                 begin: "\\b0(_*[0-7])*[lL]?\\b"
             }, {
                 begin: "\\b0[bB][01](_*[01])*[lL]?\\b"
             }],
             relevance: 0
         };
 
-    function ue(e, n, t) {
-        return -1 === t ? "" : e.replace(n, (a => ue(e, n, t - 1)))
+    function pe(e, n, t) {
+        return -1 === t ? "" : e.replace(n, (a => pe(e, n, t - 1)))
     }
-    const be = "[A-Za-z$_][0-9A-Za-z$_]*",
-        me = ["as", "in", "of", "if", "for", "while", "finally", "var", "new", "function", "do", "return", "void", "else", "break", "catch", "instanceof", "with", "throw", "case", "default", "try", "switch", "continue", "typeof", "delete", "let", "yield", "const", "class", "debugger", "async", "await", "static", "import", "from", "export", "extends"],
-        pe = ["true", "false", "null", "undefined", "NaN", "Infinity"],
-        _e = ["Object", "Function", "Boolean", "Symbol", "Math", "Date", "Number", "BigInt", "String", "RegExp", "Array", "Float32Array", "Float64Array", "Int8Array", "Uint8Array", "Uint8ClampedArray", "Int16Array", "Int32Array", "Uint16Array", "Uint32Array", "BigInt64Array", "BigUint64Array", "Set", "Map", "WeakSet", "WeakMap", "ArrayBuffer", "SharedArrayBuffer", "Atomics", "DataView", "JSON", "Promise", "Generator", "GeneratorFunction", "AsyncFunction", "Reflect", "Proxy", "Intl", "WebAssembly"],
-        he = ["Error", "EvalError", "InternalError", "RangeError", "ReferenceError", "SyntaxError", "TypeError", "URIError"],
-        fe = ["setInterval", "setTimeout", "clearInterval", "clearTimeout", "require", "exports", "eval", "isFinite", "isNaN", "parseFloat", "parseInt", "decodeURI", "decodeURIComponent", "encodeURI", "encodeURIComponent", "escape", "unescape"],
-        Ee = ["arguments", "this", "super", "console", "window", "document", "localStorage", "module", "global"],
-        ye = [].concat(fe, _e, he);
+    const _e = "[A-Za-z$_][0-9A-Za-z$_]*",
+        he = ["as", "in", "of", "if", "for", "while", "finally", "var", "new", "function", "do", "return", "void", "else", "break", "catch", "instanceof", "with", "throw", "case", "default", "try", "switch", "continue", "typeof", "delete", "let", "yield", "const", "class", "debugger", "async", "await", "static", "import", "from", "export", "extends"],
+        fe = ["true", "false", "null", "undefined", "NaN", "Infinity"],
+        Ee = ["Object", "Function", "Boolean", "Symbol", "Math", "Date", "Number", "BigInt", "String", "RegExp", "Array", "Float32Array", "Float64Array", "Int8Array", "Uint8Array", "Uint8ClampedArray", "Int16Array", "Int32Array", "Uint16Array", "Uint32Array", "BigInt64Array", "BigUint64Array", "Set", "Map", "WeakSet", "WeakMap", "ArrayBuffer", "SharedArrayBuffer", "Atomics", "DataView", "JSON", "Promise", "Generator", "GeneratorFunction", "AsyncFunction", "Reflect", "Proxy", "Intl", "WebAssembly"],
+        ye = ["Error", "EvalError", "InternalError", "RangeError", "ReferenceError", "SyntaxError", "TypeError", "URIError"],
+        Ne = ["setInterval", "setTimeout", "clearInterval", "clearTimeout", "require", "exports", "eval", "isFinite", "isNaN", "parseFloat", "parseInt", "decodeURI", "decodeURIComponent", "encodeURI", "encodeURIComponent", "escape", "unescape"],
+        we = ["arguments", "this", "super", "console", "window", "document", "localStorage", "sessionStorage", "module", "global"],
+        ve = [].concat(Ne, Ee, ye);
 
-    function we(e) {
+    function Oe(e) {
         const n = e.regex,
-            t = be,
+            t = _e,
             a = {
                 begin: /<[A-Za-z0-9\\._:-]+/,
                 end: /\/[A-Za-z0-9\\._:-]+>|\/>/,
                 isTrulyOpeningTag: (e, n) => {
                     const t = e[0].length + e.index,
                         a = e.input[t];
                     if ("<" === a || "," === a) return void n.ignoreMatch();
@@ -1054,75 +1071,86 @@
                         after: t
                     }) || n.ignoreMatch());
                     const r = e.input.substring(t);
                     ((i = r.match(/^\s*=/)) || (i = r.match(/^\s+extends\s+/)) && 0 === i.index) && n.ignoreMatch()
                 }
             },
             i = {
-                $pattern: be,
-                keyword: me,
-                literal: pe,
-                built_in: ye,
-                "variable.language": Ee
+                $pattern: _e,
+                keyword: he,
+                literal: fe,
+                built_in: ve,
+                "variable.language": we
             },
-            r = "\\.([0-9](_?[0-9])*)",
-            s = "0|[1-9](_?[0-9])*|0[0-7]*[89][0-9]*",
-            o = {
+            r = "[0-9](_?[0-9])*",
+            s = `\\.(${r})`,
+            o = "0|[1-9](_?[0-9])*|0[0-7]*[89][0-9]*",
+            l = {
                 className: "number",
                 variants: [{
-                    begin: `(\\b(${s})((${r})|\\.)?|(${r}))[eE][+-]?([0-9](_?[0-9])*)\\b`
+                    begin: `(\\b(${o})((${s})|\\.)?|(${s}))[eE][+-]?(${r})\\b`
                 }, {
-                    begin: `\\b(${s})\\b((${r})\\b|\\.)?|(${r})\\b`
+                    begin: `\\b(${o})\\b((${s})\\b|\\.)?|(${s})\\b`
                 }, {
                     begin: "\\b(0|[1-9](_?[0-9])*)n\\b"
                 }, {
                     begin: "\\b0[xX][0-9a-fA-F](_?[0-9a-fA-F])*n?\\b"
                 }, {
                     begin: "\\b0[bB][0-1](_?[0-1])*n?\\b"
                 }, {
                     begin: "\\b0[oO][0-7](_?[0-7])*n?\\b"
                 }, {
                     begin: "\\b0[0-7]+n?\\b"
                 }],
                 relevance: 0
             },
-            l = {
+            c = {
                 className: "subst",
                 begin: "\\$\\{",
                 end: "\\}",
                 keywords: i,
                 contains: []
             },
-            c = {
+            d = {
                 begin: "html`",
                 end: "",
                 starts: {
                     end: "`",
                     returnEnd: !1,
-                    contains: [e.BACKSLASH_ESCAPE, l],
+                    contains: [e.BACKSLASH_ESCAPE, c],
                     subLanguage: "xml"
                 }
             },
-            d = {
+            g = {
                 begin: "css`",
                 end: "",
                 starts: {
                     end: "`",
                     returnEnd: !1,
-                    contains: [e.BACKSLASH_ESCAPE, l],
+                    contains: [e.BACKSLASH_ESCAPE, c],
                     subLanguage: "css"
                 }
             },
-            g = {
+            u = {
+                begin: "gql`",
+                end: "",
+                starts: {
+                    end: "`",
+                    returnEnd: !1,
+                    contains: [e.BACKSLASH_ESCAPE, c],
+                    subLanguage: "graphql"
+                }
+            },
+            b = {
                 className: "string",
                 begin: "`",
                 end: "`",
-                contains: [e.BACKSLASH_ESCAPE, l]
+                contains: [e.BACKSLASH_ESCAPE, c]
             },
-            u = {
+            m = {
                 className: "comment",
                 variants: [e.COMMENT(/\/\*\*(?!\/)/, "\\*/", {
                     relevance: 0,
                     contains: [{
                         begin: "(?=@[A-Za-z]+)",
                         relevance: 0,
                         contains: [{
@@ -1143,40 +1171,40 @@
                         }, {
                             begin: /(?=[^\n])\s/,
                             relevance: 0
                         }]
                     }]
                 }), e.C_BLOCK_COMMENT_MODE, e.C_LINE_COMMENT_MODE]
             },
-            b = [e.APOS_STRING_MODE, e.QUOTE_STRING_MODE, c, d, g, {
+            p = [e.APOS_STRING_MODE, e.QUOTE_STRING_MODE, d, g, u, b, {
                 match: /\$\d+/
-            }, o];
-        l.contains = b.concat({
+            }, l];
+        c.contains = p.concat({
             begin: /\{/,
             end: /\}/,
             keywords: i,
-            contains: ["self"].concat(b)
+            contains: ["self"].concat(p)
         });
-        const m = [].concat(u, l.contains),
-            p = m.concat([{
+        const _ = [].concat(m, c.contains),
+            h = _.concat([{
                 begin: /\(/,
                 end: /\)/,
                 keywords: i,
-                contains: ["self"].concat(m)
+                contains: ["self"].concat(_)
             }]),
-            _ = {
+            f = {
                 className: "params",
                 begin: /\(/,
                 end: /\)/,
                 excludeBegin: !0,
                 excludeEnd: !0,
                 keywords: i,
-                contains: p
+                contains: h
             },
-            h = {
+            E = {
                 variants: [{
                     match: [/class/, /\s+/, t, /\s+/, /extends/, /\s+/, n.concat(t, "(", n.concat(/\./, t), ")*")],
                     scope: {
                         1: "keyword",
                         3: "title.class",
                         5: "keyword",
                         7: "title.class.inherited"
@@ -1185,101 +1213,101 @@
                     match: [/class/, /\s+/, t],
                     scope: {
                         1: "keyword",
                         3: "title.class"
                     }
                 }]
             },
-            f = {
+            y = {
                 relevance: 0,
                 match: n.either(/\bJSON/, /\b[A-Z][a-z]+([A-Z][a-z]*|\d)*/, /\b[A-Z]{2,}([A-Z][a-z]+|\d)+([A-Z][a-z]*)*/, /\b[A-Z]{2,}[a-z]+([A-Z][a-z]+|\d)*([A-Z][a-z]*)*/),
                 className: "title.class",
                 keywords: {
-                    _: [..._e, ...he]
+                    _: [...Ee, ...ye]
                 }
             },
-            E = {
+            N = {
                 variants: [{
                     match: [/function/, /\s+/, t, /(?=\s*\()/]
                 }, {
                     match: [/function/, /\s*(?=\()/]
                 }],
                 className: {
                     1: "keyword",
                     3: "title.function"
                 },
                 label: "func.def",
-                contains: [_],
+                contains: [f],
                 illegal: /%/
             },
-            y = {
-                match: n.concat(/\b/, (w = [...fe, "super", "import"], n.concat("(?!", w.join("|"), ")")), t, n.lookahead(/\(/)),
+            w = {
+                match: n.concat(/\b/, (v = [...Ne, "super", "import"], n.concat("(?!", v.join("|"), ")")), t, n.lookahead(/\(/)),
                 className: "title.function",
                 relevance: 0
             };
-        var w;
-        const N = {
+        var v;
+        const O = {
                 begin: n.concat(/\./, n.lookahead(n.concat(t, /(?![0-9A-Za-z$_(])/))),
                 end: t,
                 excludeBegin: !0,
                 keywords: "prototype",
                 className: "property",
                 relevance: 0
             },
-            v = {
+            k = {
                 match: [/get|set/, /\s+/, t, /(?=\()/],
                 className: {
                     1: "keyword",
                     3: "title.function"
                 },
                 contains: [{
                     begin: /\(\)/
-                }, _]
+                }, f]
             },
-            O = "(\\([^()]*(\\([^()]*(\\([^()]*\\)[^()]*)*\\)[^()]*)*\\)|" + e.UNDERSCORE_IDENT_RE + ")\\s*=>",
-            k = {
-                match: [/const|var|let/, /\s+/, t, /\s*/, /=\s*/, /(async\s*)?/, n.lookahead(O)],
+            x = "(\\([^()]*(\\([^()]*(\\([^()]*\\)[^()]*)*\\)[^()]*)*\\)|" + e.UNDERSCORE_IDENT_RE + ")\\s*=>",
+            M = {
+                match: [/const|var|let/, /\s+/, t, /\s*/, /=\s*/, /(async\s*)?/, n.lookahead(x)],
                 keywords: "async",
                 className: {
                     1: "keyword",
                     3: "title.function"
                 },
-                contains: [_]
+                contains: [f]
             };
         return {
-            name: "Javascript",
+            name: "JavaScript",
             aliases: ["js", "jsx", "mjs", "cjs"],
             keywords: i,
             exports: {
-                PARAMS_CONTAINS: p,
-                CLASS_REFERENCE: f
+                PARAMS_CONTAINS: h,
+                CLASS_REFERENCE: y
             },
             illegal: /#(?![$_A-z])/,
             contains: [e.SHEBANG({
                 label: "shebang",
                 binary: "node",
                 relevance: 5
             }), {
                 label: "use_strict",
                 className: "meta",
                 relevance: 10,
                 begin: /^\s*['"]use (strict|asm)['"]/
-            }, e.APOS_STRING_MODE, e.QUOTE_STRING_MODE, c, d, g, u, {
+            }, e.APOS_STRING_MODE, e.QUOTE_STRING_MODE, d, g, u, b, m, {
                 match: /\$\d+/
-            }, o, f, {
+            }, l, y, {
                 className: "attr",
                 begin: t + n.lookahead(":"),
                 relevance: 0
-            }, k, {
+            }, M, {
                 begin: "(" + e.RE_STARTERS_RE + "|\\b(case|return|throw)\\b)\\s*",
                 keywords: "return throw case",
                 relevance: 0,
-                contains: [u, e.REGEXP_MODE, {
+                contains: [m, e.REGEXP_MODE, {
                     className: "function",
-                    begin: O,
+                    begin: x,
                     returnBegin: !0,
                     end: "\\s*=>",
                     contains: [{
                         className: "params",
                         variants: [{
                             begin: e.UNDERSCORE_IDENT_RE,
                             relevance: 0
@@ -1289,15 +1317,15 @@
                             skip: !0
                         }, {
                             begin: /\(/,
                             end: /\)/,
                             excludeBegin: !0,
                             excludeEnd: !0,
                             keywords: i,
-                            contains: p
+                            contains: h
                         }]
                     }]
                 }, {
                     begin: /,/,
                     relevance: 0
                 }, {
                     match: /\s+/,
@@ -1317,64 +1345,64 @@
                     contains: [{
                         begin: a.begin,
                         end: a.end,
                         skip: !0,
                         contains: ["self"]
                     }]
                 }]
-            }, E, {
+            }, N, {
                 beginKeywords: "while if switch catch for"
             }, {
                 begin: "\\b(?!function)" + e.UNDERSCORE_IDENT_RE + "\\([^()]*(\\([^()]*(\\([^()]*\\)[^()]*)*\\)[^()]*)*\\)\\s*\\{",
                 returnBegin: !0,
                 label: "func.def",
-                contains: [_, e.inherit(e.TITLE_MODE, {
+                contains: [f, e.inherit(e.TITLE_MODE, {
                     begin: t,
                     className: "title.function"
                 })]
             }, {
                 match: /\.\.\./,
                 relevance: 0
-            }, N, {
+            }, O, {
                 match: "\\$" + t,
                 relevance: 0
             }, {
                 match: [/\bconstructor(?=\s*\()/],
                 className: {
                     1: "title.function"
                 },
-                contains: [_]
-            }, y, {
+                contains: [f]
+            }, w, {
                 relevance: 0,
                 match: /\b[A-Z][A-Z_0-9]+\b/,
                 className: "variable.constant"
-            }, h, v, {
+            }, E, k, {
                 match: /\$[(.]/
             }]
         }
     }
-    const Ne = e => m(/\b/, e, /\w$/.test(e) ? /\b/ : /\B/),
-        ve = ["Protocol", "Type"].map(Ne),
-        Oe = ["init", "self"].map(Ne),
-        ke = ["Any", "Self"],
-        xe = ["actor", "any", "associatedtype", "async", "await", /as\?/, /as!/, "as", "break", "case", "catch", "class", "continue", "convenience", "default", "defer", "deinit", "didSet", "distributed", "do", "dynamic", "else", "enum", "extension", "fallthrough", /fileprivate\(set\)/, "fileprivate", "final", "for", "func", "get", "guard", "if", "import", "indirect", "infix", /init\?/, /init!/, "inout", /internal\(set\)/, "internal", "in", "is", "isolated", "nonisolated", "lazy", "let", "mutating", "nonmutating", /open\(set\)/, "open", "operator", "optional", "override", "postfix", "precedencegroup", "prefix", /private\(set\)/, "private", "protocol", /public\(set\)/, "public", "repeat", "required", "rethrows", "return", "set", "some", "static", "struct", "subscript", "super", "switch", "throws", "throw", /try\?/, /try!/, "try", "typealias", /unowned\(safe\)/, /unowned\(unsafe\)/, "unowned", "var", "weak", "where", "while", "willSet"],
-        Me = ["false", "nil", "true"],
-        Se = ["assignment", "associativity", "higherThan", "left", "lowerThan", "none", "right"],
-        Ae = ["#colorLiteral", "#column", "#dsohandle", "#else", "#elseif", "#endif", "#error", "#file", "#fileID", "#fileLiteral", "#filePath", "#function", "#if", "#imageLiteral", "#keyPath", "#line", "#selector", "#sourceLocation", "#warn_unqualified_access", "#warning"],
-        Ce = ["abs", "all", "any", "assert", "assertionFailure", "debugPrint", "dump", "fatalError", "getVaList", "isKnownUniquelyReferenced", "max", "min", "numericCast", "pointwiseMax", "pointwiseMin", "precondition", "preconditionFailure", "print", "readLine", "repeatElement", "sequence", "stride", "swap", "swift_unboxFromSwiftValueWithType", "transcode", "type", "unsafeBitCast", "unsafeDowncast", "withExtendedLifetime", "withUnsafeMutablePointer", "withUnsafePointer", "withVaList", "withoutActuallyEscaping", "zip"],
-        Te = p(/[/=\-+!*%<>&|^~?]/, /[\u00A1-\u00A7]/, /[\u00A9\u00AB]/, /[\u00AC\u00AE]/, /[\u00B0\u00B1]/, /[\u00B6\u00BB\u00BF\u00D7\u00F7]/, /[\u2016-\u2017]/, /[\u2020-\u2027]/, /[\u2030-\u203E]/, /[\u2041-\u2053]/, /[\u2055-\u205E]/, /[\u2190-\u23FF]/, /[\u2500-\u2775]/, /[\u2794-\u2BFF]/, /[\u2E00-\u2E7F]/, /[\u3001-\u3003]/, /[\u3008-\u3020]/, /[\u3030]/),
-        Re = p(Te, /[\u0300-\u036F]/, /[\u1DC0-\u1DFF]/, /[\u20D0-\u20FF]/, /[\uFE00-\uFE0F]/, /[\uFE20-\uFE2F]/),
-        De = m(Te, Re, "*"),
-        Ie = p(/[a-zA-Z_]/, /[\u00A8\u00AA\u00AD\u00AF\u00B2-\u00B5\u00B7-\u00BA]/, /[\u00BC-\u00BE\u00C0-\u00D6\u00D8-\u00F6\u00F8-\u00FF]/, /[\u0100-\u02FF\u0370-\u167F\u1681-\u180D\u180F-\u1DBF]/, /[\u1E00-\u1FFF]/, /[\u200B-\u200D\u202A-\u202E\u203F-\u2040\u2054\u2060-\u206F]/, /[\u2070-\u20CF\u2100-\u218F\u2460-\u24FF\u2776-\u2793]/, /[\u2C00-\u2DFF\u2E80-\u2FFF]/, /[\u3004-\u3007\u3021-\u302F\u3031-\u303F\u3040-\uD7FF]/, /[\uF900-\uFD3D\uFD40-\uFDCF\uFDF0-\uFE1F\uFE30-\uFE44]/, /[\uFE47-\uFEFE\uFF00-\uFFFD]/),
-        Le = p(Ie, /\d/, /[\u0300-\u036F\u1DC0-\u1DFF\u20D0-\u20FF\uFE20-\uFE2F]/),
-        Be = m(Ie, Le, "*"),
-        $e = m(/[A-Z]/, Le, "*"),
-        ze = ["autoclosure", m(/convention\(/, p("swift", "block", "c"), /\)/), "discardableResult", "dynamicCallable", "dynamicMemberLookup", "escaping", "frozen", "GKInspectable", "IBAction", "IBDesignable", "IBInspectable", "IBOutlet", "IBSegueAction", "inlinable", "main", "nonobjc", "NSApplicationMain", "NSCopying", "NSManaged", m(/objc\(/, Be, /\)/), "objc", "objcMembers", "propertyWrapper", "requires_stored_property_inits", "resultBuilder", "testable", "UIApplicationMain", "unknown", "usableFromInline"],
-        Fe = ["iOS", "iOSApplicationExtension", "macOS", "macOSApplicationExtension", "macCatalyst", "macCatalystApplicationExtension", "watchOS", "watchOSApplicationExtension", "tvOS", "tvOSApplicationExtension", "swift"];
-    var Ue = Object.freeze({
+    const ke = e => b(/\b/, e, /\w$/.test(e) ? /\b/ : /\B/),
+        xe = ["Protocol", "Type"].map(ke),
+        Me = ["init", "self"].map(ke),
+        Se = ["Any", "Self"],
+        Ae = ["actor", "any", "associatedtype", "async", "await", /as\?/, /as!/, "as", "break", "case", "catch", "class", "continue", "convenience", "default", "defer", "deinit", "didSet", "distributed", "do", "dynamic", "else", "enum", "extension", "fallthrough", /fileprivate\(set\)/, "fileprivate", "final", "for", "func", "get", "guard", "if", "import", "indirect", "infix", /init\?/, /init!/, "inout", /internal\(set\)/, "internal", "in", "is", "isolated", "nonisolated", "lazy", "let", "mutating", "nonmutating", /open\(set\)/, "open", "operator", "optional", "override", "postfix", "precedencegroup", "prefix", /private\(set\)/, "private", "protocol", /public\(set\)/, "public", "repeat", "required", "rethrows", "return", "set", "some", "static", "struct", "subscript", "super", "switch", "throws", "throw", /try\?/, /try!/, "try", "typealias", /unowned\(safe\)/, /unowned\(unsafe\)/, "unowned", "var", "weak", "where", "while", "willSet"],
+        Ce = ["false", "nil", "true"],
+        Te = ["assignment", "associativity", "higherThan", "left", "lowerThan", "none", "right"],
+        Re = ["#colorLiteral", "#column", "#dsohandle", "#else", "#elseif", "#endif", "#error", "#file", "#fileID", "#fileLiteral", "#filePath", "#function", "#if", "#imageLiteral", "#keyPath", "#line", "#selector", "#sourceLocation", "#warn_unqualified_access", "#warning"],
+        De = ["abs", "all", "any", "assert", "assertionFailure", "debugPrint", "dump", "fatalError", "getVaList", "isKnownUniquelyReferenced", "max", "min", "numericCast", "pointwiseMax", "pointwiseMin", "precondition", "preconditionFailure", "print", "readLine", "repeatElement", "sequence", "stride", "swap", "swift_unboxFromSwiftValueWithType", "transcode", "type", "unsafeBitCast", "unsafeDowncast", "withExtendedLifetime", "withUnsafeMutablePointer", "withUnsafePointer", "withVaList", "withoutActuallyEscaping", "zip"],
+        Ie = m(/[/=\-+!*%<>&|^~?]/, /[\u00A1-\u00A7]/, /[\u00A9\u00AB]/, /[\u00AC\u00AE]/, /[\u00B0\u00B1]/, /[\u00B6\u00BB\u00BF\u00D7\u00F7]/, /[\u2016-\u2017]/, /[\u2020-\u2027]/, /[\u2030-\u203E]/, /[\u2041-\u2053]/, /[\u2055-\u205E]/, /[\u2190-\u23FF]/, /[\u2500-\u2775]/, /[\u2794-\u2BFF]/, /[\u2E00-\u2E7F]/, /[\u3001-\u3003]/, /[\u3008-\u3020]/, /[\u3030]/),
+        Le = m(Ie, /[\u0300-\u036F]/, /[\u1DC0-\u1DFF]/, /[\u20D0-\u20FF]/, /[\uFE00-\uFE0F]/, /[\uFE20-\uFE2F]/),
+        Be = b(Ie, Le, "*"),
+        $e = m(/[a-zA-Z_]/, /[\u00A8\u00AA\u00AD\u00AF\u00B2-\u00B5\u00B7-\u00BA]/, /[\u00BC-\u00BE\u00C0-\u00D6\u00D8-\u00F6\u00F8-\u00FF]/, /[\u0100-\u02FF\u0370-\u167F\u1681-\u180D\u180F-\u1DBF]/, /[\u1E00-\u1FFF]/, /[\u200B-\u200D\u202A-\u202E\u203F-\u2040\u2054\u2060-\u206F]/, /[\u2070-\u20CF\u2100-\u218F\u2460-\u24FF\u2776-\u2793]/, /[\u2C00-\u2DFF\u2E80-\u2FFF]/, /[\u3004-\u3007\u3021-\u302F\u3031-\u303F\u3040-\uD7FF]/, /[\uF900-\uFD3D\uFD40-\uFDCF\uFDF0-\uFE1F\uFE30-\uFE44]/, /[\uFE47-\uFEFE\uFF00-\uFFFD]/),
+        ze = m($e, /\d/, /[\u0300-\u036F\u1DC0-\u1DFF\u20D0-\u20FF\uFE20-\uFE2F]/),
+        Fe = b($e, ze, "*"),
+        Ue = b(/[A-Z]/, ze, "*"),
+        je = ["autoclosure", b(/convention\(/, m("swift", "block", "c"), /\)/), "discardableResult", "dynamicCallable", "dynamicMemberLookup", "escaping", "frozen", "GKInspectable", "IBAction", "IBDesignable", "IBInspectable", "IBOutlet", "IBSegueAction", "inlinable", "main", "nonobjc", "NSApplicationMain", "NSCopying", "NSManaged", b(/objc\(/, Fe, /\)/), "objc", "objcMembers", "propertyWrapper", "requires_stored_property_inits", "resultBuilder", "testable", "UIApplicationMain", "unknown", "usableFromInline"],
+        Pe = ["iOS", "iOSApplicationExtension", "macOS", "macOSApplicationExtension", "macCatalyst", "macCatalystApplicationExtension", "watchOS", "watchOSApplicationExtension", "tvOS", "tvOSApplicationExtension", "swift"];
+    var Ke = Object.freeze({
         __proto__: null,
         grmr_bash: e => {
             const n = e.regex,
                 t = {},
                 a = {
                     begin: /\$\{/,
                     end: /\}/,
@@ -1434,15 +1462,15 @@
                     relevance: 0
                 };
             return {
                 name: "Bash",
                 aliases: ["sh"],
                 keywords: {
                     $pattern: /\b[a-z][a-z0-9._-]+\b/,
-                    keyword: ["if", "then", "else", "elif", "fi", "for", "while", "in", "do", "done", "case", "esac", "function"],
+                    keyword: ["if", "then", "else", "elif", "fi", "for", "while", "until", "in", "do", "done", "case", "esac", "function", "select"],
                     literal: ["true", "false"],
                     built_in: ["break", "cd", "continue", "eval", "exec", "exit", "export", "getopts", "hash", "pwd", "readonly", "return", "shift", "test", "times", "trap", "umask", "unset", "alias", "bind", "builtin", "caller", "command", "declare", "echo", "enable", "help", "let", "local", "logout", "mapfile", "printf", "read", "readarray", "source", "type", "typeset", "ulimit", "unalias", "set", "shopt", "autoload", "bg", "bindkey", "bye", "cap", "chdir", "clone", "comparguments", "compcall", "compctl", "compdescribe", "compfiles", "compgroups", "compquote", "comptags", "comptry", "compvalues", "dirs", "disable", "disown", "echotc", "echoti", "emulate", "fc", "fg", "float", "functions", "getcap", "getln", "history", "integer", "jobs", "kill", "limit", "log", "noglob", "popd", "print", "pushd", "pushln", "rehash", "sched", "setcap", "setopt", "stat", "suspend", "ttyctl", "unfunction", "unhash", "unlimit", "unsetopt", "vared", "wait", "whence", "where", "which", "zcompile", "zformat", "zftp", "zle", "zmodload", "zparseopts", "zprof", "zpty", "zregexparse", "zsocket", "zstyle", "ztcp", "chcon", "chgrp", "chown", "chmod", "cp", "dd", "df", "dir", "dircolors", "ln", "ls", "mkdir", "mkfifo", "mknod", "mktemp", "mv", "realpath", "rm", "rmdir", "shred", "sync", "touch", "truncate", "vdir", "b2sum", "base32", "base64", "cat", "cksum", "comm", "csplit", "cut", "expand", "fmt", "fold", "head", "join", "md5sum", "nl", "numfmt", "od", "paste", "ptx", "pr", "sha1sum", "sha224sum", "sha256sum", "sha384sum", "sha512sum", "shuf", "sort", "split", "sum", "tac", "tail", "tr", "tsort", "unexpand", "uniq", "wc", "arch", "basename", "chroot", "date", "dirname", "du", "echo", "env", "expr", "factor", "groups", "hostid", "id", "link", "logname", "nice", "nohup", "nproc", "pathchk", "pinky", "printenv", "printf", "pwd", "readlink", "runcon", "seq", "sleep", "stat", "stdbuf", "stty", "tee", "test", "timeout", "tty", "uname", "unlink", "uptime", "users", "who", "whoami", "yes"]
                 },
                 contains: [l, e.SHEBANG(), c, o, e.HASH_COMMENT_MODE, r, {
                     match: /(\/[a-z._-]+)+/
                 }, s, {
                     className: "",
@@ -1457,25 +1485,26 @@
         grmr_c: e => {
             const n = e.regex,
                 t = e.COMMENT("//", "$", {
                     contains: [{
                         begin: /\\\n/
                     }]
                 }),
-                a = "[a-zA-Z_]\\w*::",
-                i = "(decltype\\(auto\\)|" + n.optional(a) + "[a-zA-Z_]\\w*" + n.optional("<[^<>]+>") + ")",
-                r = {
+                a = "decltype\\(auto\\)",
+                i = "[a-zA-Z_]\\w*::",
+                r = "(" + a + "|" + n.optional(i) + "[a-zA-Z_]\\w*" + n.optional("<[^<>]+>") + ")",
+                s = {
                     className: "type",
                     variants: [{
                         begin: "\\b[a-z\\d_]*_t\\b"
                     }, {
                         match: /\batomic_[a-z]{3,6}\b/
                     }]
                 },
-                s = {
+                o = {
                     className: "string",
                     variants: [{
                         begin: '(u8?|U|L)?"',
                         end: '"',
                         illegal: "\\n",
                         contains: [e.BACKSLASH_ESCAPE]
                     }, {
@@ -1483,150 +1512,151 @@
                         end: "'",
                         illegal: "."
                     }, e.END_SAME_AS_BEGIN({
                         begin: /(?:u8?|U|L)?R"([^()\\ ]{0,16})\(/,
                         end: /\)([^()\\ ]{0,16})"/
                     })]
                 },
-                o = {
+                l = {
                     className: "number",
                     variants: [{
                         begin: "\\b(0b[01']+)"
                     }, {
                         begin: "(-?)\\b([\\d']+(\\.[\\d']*)?|\\.[\\d']+)((ll|LL|l|L)(u|U)?|(u|U)(ll|LL|l|L)?|f|F|b|B)"
                     }, {
                         begin: "(-?)(\\b0[xX][a-fA-F0-9']+|(\\b[\\d']+(\\.[\\d']*)?|\\.[\\d']+)([eE][-+]?[\\d']+)?)"
                     }],
                     relevance: 0
                 },
-                l = {
+                c = {
                     className: "meta",
                     begin: /#\s*[a-z]+\b/,
                     end: /$/,
                     keywords: {
                         keyword: "if else elif endif define undef warning error line pragma _Pragma ifdef ifndef include"
                     },
                     contains: [{
                         begin: /\\\n/,
                         relevance: 0
-                    }, e.inherit(s, {
+                    }, e.inherit(o, {
                         className: "string"
                     }), {
                         className: "string",
                         begin: /<.*?>/
                     }, t, e.C_BLOCK_COMMENT_MODE]
                 },
-                c = {
+                d = {
                     className: "title",
-                    begin: n.optional(a) + e.IDENT_RE,
+                    begin: n.optional(i) + e.IDENT_RE,
                     relevance: 0
                 },
-                d = n.optional(a) + e.IDENT_RE + "\\s*\\(",
-                g = {
+                g = n.optional(i) + e.IDENT_RE + "\\s*\\(",
+                u = {
                     keyword: ["asm", "auto", "break", "case", "continue", "default", "do", "else", "enum", "extern", "for", "fortran", "goto", "if", "inline", "register", "restrict", "return", "sizeof", "struct", "switch", "typedef", "union", "volatile", "while", "_Alignas", "_Alignof", "_Atomic", "_Generic", "_Noreturn", "_Static_assert", "_Thread_local", "alignas", "alignof", "noreturn", "static_assert", "thread_local", "_Pragma"],
                     type: ["float", "double", "signed", "unsigned", "int", "short", "long", "char", "void", "_Bool", "_Complex", "_Imaginary", "_Decimal32", "_Decimal64", "_Decimal128", "const", "static", "complex", "bool", "imaginary"],
                     literal: "true false NULL",
                     built_in: "std string wstring cin cout cerr clog stdin stdout stderr stringstream istringstream ostringstream auto_ptr deque list queue stack vector map set pair bitset multiset multimap unordered_set unordered_map unordered_multiset unordered_multimap priority_queue make_pair array shared_ptr abort terminate abs acos asin atan2 atan calloc ceil cosh cos exit exp fabs floor fmod fprintf fputs free frexp fscanf future isalnum isalpha iscntrl isdigit isgraph islower isprint ispunct isspace isupper isxdigit tolower toupper labs ldexp log10 log malloc realloc memchr memcmp memcpy memset modf pow printf putchar puts scanf sinh sin snprintf sprintf sqrt sscanf strcat strchr strcmp strcpy strcspn strlen strncat strncmp strncpy strpbrk strrchr strspn strstr tanh tan vfprintf vprintf vsprintf endl initializer_list unique_ptr"
                 },
-                u = [l, r, t, e.C_BLOCK_COMMENT_MODE, o, s],
-                b = {
+                b = [c, s, t, e.C_BLOCK_COMMENT_MODE, l, o],
+                m = {
                     variants: [{
                         begin: /=/,
                         end: /;/
                     }, {
                         begin: /\(/,
                         end: /\)/
                     }, {
                         beginKeywords: "new throw return else",
                         end: /;/
                     }],
-                    keywords: g,
-                    contains: u.concat([{
+                    keywords: u,
+                    contains: b.concat([{
                         begin: /\(/,
                         end: /\)/,
-                        keywords: g,
-                        contains: u.concat(["self"]),
+                        keywords: u,
+                        contains: b.concat(["self"]),
                         relevance: 0
                     }]),
                     relevance: 0
                 },
-                m = {
-                    begin: "(" + i + "[\\*&\\s]+)+" + d,
+                p = {
+                    begin: "(" + r + "[\\*&\\s]+)+" + g,
                     returnBegin: !0,
                     end: /[{;=]/,
                     excludeEnd: !0,
-                    keywords: g,
+                    keywords: u,
                     illegal: /[^\w\s\*&:<>.]/,
                     contains: [{
-                        begin: "decltype\\(auto\\)",
-                        keywords: g,
+                        begin: a,
+                        keywords: u,
                         relevance: 0
                     }, {
-                        begin: d,
+                        begin: g,
                         returnBegin: !0,
-                        contains: [e.inherit(c, {
+                        contains: [e.inherit(d, {
                             className: "title.function"
                         })],
                         relevance: 0
                     }, {
                         relevance: 0,
                         match: /,/
                     }, {
                         className: "params",
                         begin: /\(/,
                         end: /\)/,
-                        keywords: g,
+                        keywords: u,
                         relevance: 0,
-                        contains: [t, e.C_BLOCK_COMMENT_MODE, s, o, r, {
+                        contains: [t, e.C_BLOCK_COMMENT_MODE, o, l, s, {
                             begin: /\(/,
                             end: /\)/,
-                            keywords: g,
+                            keywords: u,
                             relevance: 0,
-                            contains: ["self", t, e.C_BLOCK_COMMENT_MODE, s, o, r]
+                            contains: ["self", t, e.C_BLOCK_COMMENT_MODE, o, l, s]
                         }]
-                    }, r, t, e.C_BLOCK_COMMENT_MODE, l]
+                    }, s, t, e.C_BLOCK_COMMENT_MODE, c]
                 };
             return {
                 name: "C",
                 aliases: ["h"],
-                keywords: g,
+                keywords: u,
                 disableAutodetect: !0,
                 illegal: "</",
-                contains: [].concat(b, m, u, [l, {
+                contains: [].concat(m, p, b, [c, {
                     begin: e.IDENT_RE + "::",
-                    keywords: g
+                    keywords: u
                 }, {
                     className: "class",
                     beginKeywords: "enum class struct union",
                     end: /[{;:<>=]/,
                     contains: [{
                         beginKeywords: "final class struct"
                     }, e.TITLE_MODE]
                 }]),
                 exports: {
-                    preprocessor: l,
-                    strings: s,
-                    keywords: g
+                    preprocessor: c,
+                    strings: o,
+                    keywords: u
                 }
             }
         },
         grmr_cpp: e => {
             const n = e.regex,
                 t = e.COMMENT("//", "$", {
                     contains: [{
                         begin: /\\\n/
                     }]
                 }),
-                a = "[a-zA-Z_]\\w*::",
-                i = "(?!struct)(decltype\\(auto\\)|" + n.optional(a) + "[a-zA-Z_]\\w*" + n.optional("<[^<>]+>") + ")",
-                r = {
+                a = "decltype\\(auto\\)",
+                i = "[a-zA-Z_]\\w*::",
+                r = "(?!struct)(" + a + "|" + n.optional(i) + "[a-zA-Z_]\\w*" + n.optional("<[^<>]+>") + ")",
+                s = {
                     className: "type",
                     begin: "\\b[a-z\\d_]*_t\\b"
                 },
-                s = {
+                o = {
                     className: "string",
                     variants: [{
                         begin: '(u8?|U|L)?"',
                         end: '"',
                         illegal: "\\n",
                         contains: [e.BACKSLASH_ESCAPE]
                     }, {
@@ -1634,143 +1664,143 @@
                         end: "'",
                         illegal: "."
                     }, e.END_SAME_AS_BEGIN({
                         begin: /(?:u8?|U|L)?R"([^()\\ ]{0,16})\(/,
                         end: /\)([^()\\ ]{0,16})"/
                     })]
                 },
-                o = {
+                l = {
                     className: "number",
                     variants: [{
                         begin: "\\b(0b[01']+)"
                     }, {
                         begin: "(-?)\\b([\\d']+(\\.[\\d']*)?|\\.[\\d']+)((ll|LL|l|L)(u|U)?|(u|U)(ll|LL|l|L)?|f|F|b|B)"
                     }, {
                         begin: "(-?)(\\b0[xX][a-fA-F0-9']+|(\\b[\\d']+(\\.[\\d']*)?|\\.[\\d']+)([eE][-+]?[\\d']+)?)"
                     }],
                     relevance: 0
                 },
-                l = {
+                c = {
                     className: "meta",
                     begin: /#\s*[a-z]+\b/,
                     end: /$/,
                     keywords: {
                         keyword: "if else elif endif define undef warning error line pragma _Pragma ifdef ifndef include"
                     },
                     contains: [{
                         begin: /\\\n/,
                         relevance: 0
-                    }, e.inherit(s, {
+                    }, e.inherit(o, {
                         className: "string"
                     }), {
                         className: "string",
                         begin: /<.*?>/
                     }, t, e.C_BLOCK_COMMENT_MODE]
                 },
-                c = {
+                d = {
                     className: "title",
-                    begin: n.optional(a) + e.IDENT_RE,
+                    begin: n.optional(i) + e.IDENT_RE,
                     relevance: 0
                 },
-                d = n.optional(a) + e.IDENT_RE + "\\s*\\(",
-                g = {
+                g = n.optional(i) + e.IDENT_RE + "\\s*\\(",
+                u = {
                     type: ["bool", "char", "char16_t", "char32_t", "char8_t", "double", "float", "int", "long", "short", "void", "wchar_t", "unsigned", "signed", "const", "static"],
                     keyword: ["alignas", "alignof", "and", "and_eq", "asm", "atomic_cancel", "atomic_commit", "atomic_noexcept", "auto", "bitand", "bitor", "break", "case", "catch", "class", "co_await", "co_return", "co_yield", "compl", "concept", "const_cast|10", "consteval", "constexpr", "constinit", "continue", "decltype", "default", "delete", "do", "dynamic_cast|10", "else", "enum", "explicit", "export", "extern", "false", "final", "for", "friend", "goto", "if", "import", "inline", "module", "mutable", "namespace", "new", "noexcept", "not", "not_eq", "nullptr", "operator", "or", "or_eq", "override", "private", "protected", "public", "reflexpr", "register", "reinterpret_cast|10", "requires", "return", "sizeof", "static_assert", "static_cast|10", "struct", "switch", "synchronized", "template", "this", "thread_local", "throw", "transaction_safe", "transaction_safe_dynamic", "true", "try", "typedef", "typeid", "typename", "union", "using", "virtual", "volatile", "while", "xor", "xor_eq"],
                     literal: ["NULL", "false", "nullopt", "nullptr", "true"],
                     built_in: ["_Pragma"],
                     _type_hints: ["any", "auto_ptr", "barrier", "binary_semaphore", "bitset", "complex", "condition_variable", "condition_variable_any", "counting_semaphore", "deque", "false_type", "future", "imaginary", "initializer_list", "istringstream", "jthread", "latch", "lock_guard", "multimap", "multiset", "mutex", "optional", "ostringstream", "packaged_task", "pair", "promise", "priority_queue", "queue", "recursive_mutex", "recursive_timed_mutex", "scoped_lock", "set", "shared_future", "shared_lock", "shared_mutex", "shared_timed_mutex", "shared_ptr", "stack", "string_view", "stringstream", "timed_mutex", "thread", "true_type", "tuple", "unique_lock", "unique_ptr", "unordered_map", "unordered_multimap", "unordered_multiset", "unordered_set", "variant", "vector", "weak_ptr", "wstring", "wstring_view"]
                 },
-                u = {
+                b = {
                     className: "function.dispatch",
                     relevance: 0,
                     keywords: {
                         _hint: ["abort", "abs", "acos", "apply", "as_const", "asin", "atan", "atan2", "calloc", "ceil", "cerr", "cin", "clog", "cos", "cosh", "cout", "declval", "endl", "exchange", "exit", "exp", "fabs", "floor", "fmod", "forward", "fprintf", "fputs", "free", "frexp", "fscanf", "future", "invoke", "isalnum", "isalpha", "iscntrl", "isdigit", "isgraph", "islower", "isprint", "ispunct", "isspace", "isupper", "isxdigit", "labs", "launder", "ldexp", "log", "log10", "make_pair", "make_shared", "make_shared_for_overwrite", "make_tuple", "make_unique", "malloc", "memchr", "memcmp", "memcpy", "memset", "modf", "move", "pow", "printf", "putchar", "puts", "realloc", "scanf", "sin", "sinh", "snprintf", "sprintf", "sqrt", "sscanf", "std", "stderr", "stdin", "stdout", "strcat", "strchr", "strcmp", "strcpy", "strcspn", "strlen", "strncat", "strncmp", "strncpy", "strpbrk", "strrchr", "strspn", "strstr", "swap", "tan", "tanh", "terminate", "to_underlying", "tolower", "toupper", "vfprintf", "visit", "vprintf", "vsprintf"]
                     },
                     begin: n.concat(/\b/, /(?!decltype)/, /(?!if)/, /(?!for)/, /(?!switch)/, /(?!while)/, e.IDENT_RE, n.lookahead(/(<[^<>]+>|)\s*\(/))
                 },
-                b = [u, l, r, t, e.C_BLOCK_COMMENT_MODE, o, s],
-                m = {
+                m = [b, c, s, t, e.C_BLOCK_COMMENT_MODE, l, o],
+                p = {
                     variants: [{
                         begin: /=/,
                         end: /;/
                     }, {
                         begin: /\(/,
                         end: /\)/
                     }, {
                         beginKeywords: "new throw return else",
                         end: /;/
                     }],
-                    keywords: g,
-                    contains: b.concat([{
+                    keywords: u,
+                    contains: m.concat([{
                         begin: /\(/,
                         end: /\)/,
-                        keywords: g,
-                        contains: b.concat(["self"]),
+                        keywords: u,
+                        contains: m.concat(["self"]),
                         relevance: 0
                     }]),
                     relevance: 0
                 },
-                p = {
+                _ = {
                     className: "function",
-                    begin: "(" + i + "[\\*&\\s]+)+" + d,
+                    begin: "(" + r + "[\\*&\\s]+)+" + g,
                     returnBegin: !0,
                     end: /[{;=]/,
                     excludeEnd: !0,
-                    keywords: g,
+                    keywords: u,
                     illegal: /[^\w\s\*&:<>.]/,
                     contains: [{
-                        begin: "decltype\\(auto\\)",
-                        keywords: g,
+                        begin: a,
+                        keywords: u,
                         relevance: 0
                     }, {
-                        begin: d,
+                        begin: g,
                         returnBegin: !0,
-                        contains: [c],
+                        contains: [d],
                         relevance: 0
                     }, {
                         begin: /::/,
                         relevance: 0
                     }, {
                         begin: /:/,
                         endsWithParent: !0,
-                        contains: [s, o]
+                        contains: [o, l]
                     }, {
                         relevance: 0,
                         match: /,/
                     }, {
                         className: "params",
                         begin: /\(/,
                         end: /\)/,
-                        keywords: g,
+                        keywords: u,
                         relevance: 0,
-                        contains: [t, e.C_BLOCK_COMMENT_MODE, s, o, r, {
+                        contains: [t, e.C_BLOCK_COMMENT_MODE, o, l, s, {
                             begin: /\(/,
                             end: /\)/,
-                            keywords: g,
+                            keywords: u,
                             relevance: 0,
-                            contains: ["self", t, e.C_BLOCK_COMMENT_MODE, s, o, r]
+                            contains: ["self", t, e.C_BLOCK_COMMENT_MODE, o, l, s]
                         }]
-                    }, r, t, e.C_BLOCK_COMMENT_MODE, l]
+                    }, s, t, e.C_BLOCK_COMMENT_MODE, c]
                 };
             return {
                 name: "C++",
                 aliases: ["cc", "c++", "h++", "hpp", "hh", "hxx", "cxx"],
-                keywords: g,
+                keywords: u,
                 illegal: "</",
                 classNameAliases: {
                     "function.dispatch": "built_in"
                 },
-                contains: [].concat(m, p, u, b, [l, {
+                contains: [].concat(p, _, b, m, [c, {
                     begin: "\\b(deque|list|queue|priority_queue|pair|stack|vector|map|set|bitset|multiset|multimap|unordered_map|unordered_set|unordered_multiset|unordered_multimap|array|tuple|optional|variant|function)\\s*<(?!<)",
                     end: ">",
-                    keywords: g,
-                    contains: ["self", r]
+                    keywords: u,
+                    contains: ["self", s]
                 }, {
                     begin: e.IDENT_RE + "::",
-                    keywords: g
+                    keywords: u
                 }, {
                     match: [/\b(?:enum(?:\s+(?:class|struct))?|class|struct|union)/, /\s+/, /\w+/],
                     className: {
                         1: "keyword",
                         3: "title.class"
                     }
                 }])
@@ -1956,15 +1986,15 @@
                         contains: [g, a, e.C_BLOCK_COMMENT_MODE]
                     }, e.C_LINE_COMMENT_MODE, e.C_BLOCK_COMMENT_MODE]
                 }, m]
             }
         },
         grmr_css: e => {
             const n = e.regex,
-                t = te(e),
+                t = ie(e),
                 a = [e.APOS_STRING_MODE, e.QUOTE_STRING_MODE];
             return {
                 name: "CSS",
                 case_insensitive: !0,
                 illegal: /[=|'\$]/,
                 keywords: {
                     keyframePosition: "from to"
@@ -1981,21 +2011,21 @@
                 }, {
                     className: "selector-class",
                     begin: "\\.[a-zA-Z-][a-zA-Z0-9_-]*",
                     relevance: 0
                 }, t.ATTRIBUTE_SELECTOR_MODE, {
                     className: "selector-pseudo",
                     variants: [{
-                        begin: ":(" + re.join("|") + ")"
+                        begin: ":(" + oe.join("|") + ")"
                     }, {
-                        begin: ":(:)?(" + se.join("|") + ")"
+                        begin: ":(:)?(" + le.join("|") + ")"
                     }]
                 }, t.CSS_VARIABLE, {
                     className: "attribute",
-                    begin: "\\b(" + oe.join("|") + ")\\b"
+                    begin: "\\b(" + ce.join("|") + ")\\b"
                 }, {
                     begin: /:/,
                     end: /[;}{]/,
                     contains: [t.BLOCK_COMMENT, t.HEXCOLOR, t.IMPORTANT, t.CSS_NUMBER_MODE, ...a, {
                         begin: /(url|data-uri)\(/,
                         end: /\)/,
                         relevance: 0,
@@ -2021,24 +2051,24 @@
                         begin: /\s/,
                         endsWithParent: !0,
                         excludeEnd: !0,
                         relevance: 0,
                         keywords: {
                             $pattern: /[a-z-]+/,
                             keyword: "and or not only",
-                            attribute: ie.join(" ")
+                            attribute: se.join(" ")
                         },
                         contains: [{
                             begin: /[a-z-]+(?=:)/,
                             className: "attribute"
                         }, ...a, t.CSS_NUMBER_MODE]
                     }]
                 }, {
                     className: "selector-tag",
-                    begin: "\\b(" + ae.join("|") + ")\\b"
+                    begin: "\\b(" + re.join("|") + ")\\b"
                 }]
             }
         },
         grmr_diff: e => {
             const n = e.regex;
             return {
                 name: "Diff",
@@ -2224,15 +2254,15 @@
                     }
                 }]
             }
         },
         grmr_java: e => {
             const n = e.regex,
                 t = "[\xc0-\u02b8a-zA-Z_$][\xc0-\u02b8a-zA-Z_$0-9]*",
-                a = t + ue("(?:<" + t + "~~~(?:\\s*,\\s*" + t + "~~~)*>)?", /~~~/g, 2),
+                a = t + pe("(?:<" + t + "~~~(?:\\s*,\\s*" + t + "~~~)*>)?", /~~~/g, 2),
                 i = {
                     keyword: ["synchronized", "abstract", "private", "var", "static", "if", "const ", "for", "while", "strictfp", "finally", "protected", "import", "native", "final", "void", "enum", "else", "break", "transient", "catch", "instanceof", "volatile", "case", "assert", "package", "default", "public", "try", "switch", "continue", "throws", "protected", "public", "private", "module", "requires", "exports", "do", "sealed", "yield", "permits"],
                     literal: ["false", "true", "null"],
                     type: ["char", "boolean", "long", "float", "int", "byte", "short", "double"],
                     built_in: ["super", "this"]
                 },
                 r = {
@@ -2310,20 +2340,20 @@
                     keywords: i,
                     contains: [{
                         className: "params",
                         begin: /\(/,
                         end: /\)/,
                         keywords: i,
                         relevance: 0,
-                        contains: [r, e.APOS_STRING_MODE, e.QUOTE_STRING_MODE, ge, e.C_BLOCK_COMMENT_MODE]
+                        contains: [r, e.APOS_STRING_MODE, e.QUOTE_STRING_MODE, me, e.C_BLOCK_COMMENT_MODE]
                     }, e.C_LINE_COMMENT_MODE, e.C_BLOCK_COMMENT_MODE]
-                }, ge, r]
+                }, me, r]
             }
         },
-        grmr_javascript: we,
+        grmr_javascript: Oe,
         grmr_json: e => {
             const n = ["true", "false", "null"],
                 t = {
                     scope: "literal",
                     beginKeywords: n.join(" ")
                 };
             return {
@@ -2393,15 +2423,15 @@
                         begin: /\(/,
                         end: /\)/,
                         contains: [e.inherit(r, {
                             className: "string"
                         }), "self"]
                     }]
                 },
-                l = ge,
+                l = me,
                 c = e.COMMENT("/\\*", "\\*/", {
                     contains: [e.C_BLOCK_COMMENT_MODE]
                 }),
                 d = {
                     variants: [{
                         className: "type",
                         begin: e.UNDERSCORE_IDENT_RE
@@ -2495,163 +2525,164 @@
                     begin: "^#!/usr/bin/env",
                     end: "$",
                     illegal: "\n"
                 }, l]
             }
         },
         grmr_less: e => {
-            const n = te(e),
-                t = le,
-                a = "([\\w-]+|@\\{[\\w-]+\\})",
-                i = [],
+            const n = ie(e),
+                t = de,
+                a = "[\\w-]+",
+                i = "(" + a + "|@\\{" + a + "\\})",
                 r = [],
-                s = e => ({
+                s = [],
+                o = e => ({
                     className: "string",
                     begin: "~?" + e + ".*?" + e
                 }),
-                o = (e, n, t) => ({
+                l = (e, n, t) => ({
                     className: e,
                     begin: n,
                     relevance: t
                 }),
-                l = {
+                c = {
                     $pattern: /[a-z-]+/,
                     keyword: "and or not only",
-                    attribute: ie.join(" ")
+                    attribute: se.join(" ")
                 },
-                c = {
+                d = {
                     begin: "\\(",
                     end: "\\)",
-                    contains: r,
-                    keywords: l,
+                    contains: s,
+                    keywords: c,
                     relevance: 0
                 };
-            r.push(e.C_LINE_COMMENT_MODE, e.C_BLOCK_COMMENT_MODE, s("'"), s('"'), n.CSS_NUMBER_MODE, {
+            s.push(e.C_LINE_COMMENT_MODE, e.C_BLOCK_COMMENT_MODE, o("'"), o('"'), n.CSS_NUMBER_MODE, {
                 begin: "(url|data-uri)\\(",
                 starts: {
                     className: "string",
                     end: "[\\)\\n]",
                     excludeEnd: !0
                 }
-            }, n.HEXCOLOR, c, o("variable", "@@?[\\w-]+", 10), o("variable", "@\\{[\\w-]+\\}"), o("built_in", "~?`[^`]*?`"), {
+            }, n.HEXCOLOR, d, l("variable", "@@?" + a, 10), l("variable", "@\\{" + a + "\\}"), l("built_in", "~?`[^`]*?`"), {
                 className: "attribute",
-                begin: "[\\w-]+\\s*:",
+                begin: a + "\\s*:",
                 end: ":",
                 returnBegin: !0,
                 excludeEnd: !0
             }, n.IMPORTANT, {
                 beginKeywords: "and not"
             }, n.FUNCTION_DISPATCH);
-            const d = r.concat({
+            const g = s.concat({
                     begin: /\{/,
                     end: /\}/,
-                    contains: i
+                    contains: r
                 }),
-                g = {
+                u = {
                     beginKeywords: "when",
                     endsWithParent: !0,
                     contains: [{
                         beginKeywords: "and not"
-                    }].concat(r)
+                    }].concat(s)
                 },
-                u = {
-                    begin: a + "\\s*:",
+                b = {
+                    begin: i + "\\s*:",
                     returnBegin: !0,
                     end: /[;}]/,
                     relevance: 0,
                     contains: [{
                         begin: /-(webkit|moz|ms|o)-/
                     }, n.CSS_VARIABLE, {
                         className: "attribute",
-                        begin: "\\b(" + oe.join("|") + ")\\b",
+                        begin: "\\b(" + ce.join("|") + ")\\b",
                         end: /(?=:)/,
                         starts: {
                             endsWithParent: !0,
                             illegal: "[<=$]",
                             relevance: 0,
-                            contains: r
+                            contains: s
                         }
                     }]
                 },
-                b = {
+                m = {
                     className: "keyword",
                     begin: "@(import|media|charset|font-face|(-[a-z]+-)?keyframes|supports|document|namespace|page|viewport|host)\\b",
                     starts: {
                         end: "[;{}]",
-                        keywords: l,
+                        keywords: c,
                         returnEnd: !0,
-                        contains: r,
+                        contains: s,
                         relevance: 0
                     }
                 },
-                m = {
+                p = {
                     className: "variable",
                     variants: [{
-                        begin: "@[\\w-]+\\s*:",
+                        begin: "@" + a + "\\s*:",
                         relevance: 15
                     }, {
-                        begin: "@[\\w-]+"
+                        begin: "@" + a
                     }],
                     starts: {
                         end: "[;}]",
                         returnEnd: !0,
-                        contains: d
+                        contains: g
                     }
                 },
-                p = {
+                _ = {
                     variants: [{
                         begin: "[\\.#:&\\[>]",
                         end: "[;{}]"
                     }, {
-                        begin: a,
+                        begin: i,
                         end: /\{/
                     }],
                     returnBegin: !0,
                     returnEnd: !0,
                     illegal: "[<='$\"]",
                     relevance: 0,
-                    contains: [e.C_LINE_COMMENT_MODE, e.C_BLOCK_COMMENT_MODE, g, o("keyword", "all\\b"), o("variable", "@\\{[\\w-]+\\}"), {
-                        begin: "\\b(" + ae.join("|") + ")\\b",
+                    contains: [e.C_LINE_COMMENT_MODE, e.C_BLOCK_COMMENT_MODE, u, l("keyword", "all\\b"), l("variable", "@\\{" + a + "\\}"), {
+                        begin: "\\b(" + re.join("|") + ")\\b",
                         className: "selector-tag"
-                    }, n.CSS_NUMBER_MODE, o("selector-tag", a, 0), o("selector-id", "#" + a), o("selector-class", "\\." + a, 0), o("selector-tag", "&", 0), n.ATTRIBUTE_SELECTOR_MODE, {
+                    }, n.CSS_NUMBER_MODE, l("selector-tag", i, 0), l("selector-id", "#" + i), l("selector-class", "\\." + i, 0), l("selector-tag", "&", 0), n.ATTRIBUTE_SELECTOR_MODE, {
                         className: "selector-pseudo",
-                        begin: ":(" + re.join("|") + ")"
+                        begin: ":(" + oe.join("|") + ")"
                     }, {
                         className: "selector-pseudo",
-                        begin: ":(:)?(" + se.join("|") + ")"
+                        begin: ":(:)?(" + le.join("|") + ")"
                     }, {
                         begin: /\(/,
                         end: /\)/,
                         relevance: 0,
-                        contains: d
+                        contains: g
                     }, {
                         begin: "!important"
                     }, n.FUNCTION_DISPATCH]
                 },
-                _ = {
-                    begin: `[\\w-]+:(:)?(${t.join("|")})`,
+                h = {
+                    begin: a + ":(:)?" + `(${t.join("|")})`,
                     returnBegin: !0,
-                    contains: [p]
+                    contains: [_]
                 };
-            return i.push(e.C_LINE_COMMENT_MODE, e.C_BLOCK_COMMENT_MODE, b, m, _, u, p, g, n.FUNCTION_DISPATCH), {
+            return r.push(e.C_LINE_COMMENT_MODE, e.C_BLOCK_COMMENT_MODE, m, p, h, b, _, u, n.FUNCTION_DISPATCH), {
                 name: "Less",
                 case_insensitive: !0,
                 illegal: "[=>'/<($\"]",
-                contains: i
+                contains: r
             }
         },
         grmr_lua: e => {
             const n = "\\[=*\\[",
                 t = "\\]=*\\]",
                 a = {
                     begin: n,
                     end: t,
                     contains: ["self"]
                 },
-                i = [e.COMMENT("--(?!\\[=*\\[)", "$"), e.COMMENT("--\\[=*\\[", t, {
+                i = [e.COMMENT("--(?!" + n + ")", "$"), e.COMMENT("--" + n, t, {
                     contains: [a],
                     relevance: 10
                 })];
             return {
                 name: "Lua",
                 keywords: {
                     $pattern: e.UNDERSCORE_IDENT_RE,
@@ -3262,18 +3293,27 @@
                 }),
                 l = "[ \t\n]",
                 c = {
                     scope: "string",
                     variants: [e.inherit(e.QUOTE_STRING_MODE, {
                         illegal: null,
                         contains: e.QUOTE_STRING_MODE.contains.concat(s)
-                    }), o, e.END_SAME_AS_BEGIN({
-                        begin: /<<<[ \t]*(\w+)\n/,
+                    }), o, {
+                        begin: /<<<[ \t]*(?:(\w+)|"(\w+)")\n/,
                         end: /[ \t]*(\w+)\b/,
-                        contains: e.QUOTE_STRING_MODE.contains.concat(s)
+                        contains: e.QUOTE_STRING_MODE.contains.concat(s),
+                        "on:begin": (e, n) => {
+                            n.data._beginMatch = e[1] || e[2]
+                        },
+                        "on:end": (e, n) => {
+                            n.data._beginMatch !== e[1] && n.ignoreMatch()
+                        }
+                    }, e.END_SAME_AS_BEGIN({
+                        begin: /<<<[ \t]*'(\w+)'\n/,
+                        end: /[ \t]*(\w+)\b/
                     })]
                 },
                 d = {
                     scope: "number",
                     variants: [{
                         begin: "\\b0[bB][01]+(?:_[01]+)*\\b"
                     }, {
@@ -3346,24 +3386,24 @@
                 y = {
                     relevance: 0,
                     begin: /\(/,
                     end: /\)/,
                     keywords: m,
                     contains: [E, r, f, e.C_BLOCK_COMMENT_MODE, c, d, _]
                 },
-                w = {
+                N = {
                     relevance: 0,
                     match: [/\b/, n.concat("(?!fn\\b|function\\b|", p(u).join("\\b|"), "|", p(b).join("\\b|"), "\\b)"), a, n.concat(l, "*"), n.lookahead(/(?=\()/)],
                     scope: {
                         3: "title.function.invoke"
                     },
                     contains: [y]
                 };
-            y.contains.push(w);
-            const N = [E, f, e.C_BLOCK_COMMENT_MODE, c, d, _];
+            y.contains.push(N);
+            const w = [E, f, e.C_BLOCK_COMMENT_MODE, c, d, _];
             return {
                 case_insensitive: !1,
                 keywords: m,
                 contains: [{
                     begin: n.concat(/#\[\s*/, i),
                     beginScope: "meta",
                     end: /]/,
@@ -3375,16 +3415,16 @@
                     contains: [{
                         begin: /\[/,
                         end: /]/,
                         keywords: {
                             literal: g,
                             keyword: ["new", "array"]
                         },
-                        contains: ["self", ...N]
-                    }, ...N, {
+                        contains: ["self", ...w]
+                    }, ...w, {
                         scope: "meta",
                         match: i
                     }]
                 }, e.HASH_COMMENT_MODE, e.COMMENT("//", "$"), e.COMMENT("/\\*", "\\*/", {
                     contains: [{
                         scope: "doctag",
                         match: "@[A-Za-z]+"
@@ -3413,15 +3453,15 @@
                         relevance: .1
                     }, {
                         begin: /\?>/
                     }]
                 }, {
                     scope: "variable.language",
                     match: /\$this\b/
-                }, r, w, f, {
+                }, r, N, f, {
                     match: [/const/, /\s/, a],
                     scope: {
                         1: "keyword",
                         3: "variable.constant"
                     }
                 }, _, {
                     scope: "function",
@@ -3637,15 +3677,15 @@
                     }]
                 };
             return s.contains = [l, u, r], {
                 name: "Python",
                 aliases: ["py", "gyp", "ipython"],
                 unicodeRegex: !0,
                 keywords: i,
-                illegal: /(<\/|->|\?)|=>/,
+                illegal: /(<\/|\?)|=>/,
                 contains: [r, u, {
                     begin: /\bself\b/
                 }, {
                     beginKeywords: "if",
                     relevance: 0
                 }, l, b, e.HASH_COMMENT_MODE, {
                     match: [/\bdef/, /\s+/, t],
@@ -4147,17 +4187,17 @@
                 }, {
                     className: "punctuation",
                     begin: "->"
                 }, t]
             }
         },
         grmr_scss: e => {
-            const n = te(e),
-                t = se,
-                a = re,
+            const n = ie(e),
+                t = le,
+                a = oe,
                 i = "@[a-z-]+",
                 r = {
                     className: "variable",
                     begin: "(\\$[a-zA-Z-][a-zA-Z0-9_-]*)\\b",
                     relevance: 0
                 };
             return {
@@ -4170,29 +4210,29 @@
                     relevance: 0
                 }, {
                     className: "selector-class",
                     begin: "\\.[A-Za-z0-9_-]+",
                     relevance: 0
                 }, n.ATTRIBUTE_SELECTOR_MODE, {
                     className: "selector-tag",
-                    begin: "\\b(" + ae.join("|") + ")\\b",
+                    begin: "\\b(" + re.join("|") + ")\\b",
                     relevance: 0
                 }, {
                     className: "selector-pseudo",
                     begin: ":(" + a.join("|") + ")"
                 }, {
                     className: "selector-pseudo",
                     begin: ":(:)?(" + t.join("|") + ")"
                 }, r, {
                     begin: /\(/,
                     end: /\)/,
                     contains: [n.CSS_NUMBER_MODE]
                 }, n.CSS_VARIABLE, {
                     className: "attribute",
-                    begin: "\\b(" + oe.join("|") + ")\\b"
+                    begin: "\\b(" + ce.join("|") + ")\\b"
                 }, {
                     begin: "\\b(whitespace|wait|w-resize|visible|vertical-text|vertical-ideographic|uppercase|upper-roman|upper-alpha|underline|transparent|top|thin|thick|text|text-top|text-bottom|tb-rl|table-header-group|table-footer-group|sw-resize|super|strict|static|square|solid|small-caps|separate|se-resize|scroll|s-resize|rtl|row-resize|ridge|right|repeat|repeat-y|repeat-x|relative|progress|pointer|overline|outside|outset|oblique|nowrap|not-allowed|normal|none|nw-resize|no-repeat|no-drop|newspaper|ne-resize|n-resize|move|middle|medium|ltr|lr-tb|lowercase|lower-roman|lower-alpha|loose|list-item|line|line-through|line-edge|lighter|left|keep-all|justify|italic|inter-word|inter-ideograph|inside|inset|inline|inline-block|inherit|inactive|ideograph-space|ideograph-parenthesis|ideograph-numeric|ideograph-alpha|horizontal|hidden|help|hand|groove|fixed|ellipsis|e-resize|double|dotted|distribute|distribute-space|distribute-letter|distribute-all-lines|disc|disabled|default|decimal|dashed|crosshair|collapse|col-resize|circle|char|center|capitalize|break-word|break-all|bottom|both|bolder|bold|block|bidi-override|below|baseline|auto|always|all-scroll|absolute|table|table-cell)\\b"
                 }, {
                     begin: /:/,
                     end: /[;}{]/,
                     relevance: 0,
                     contains: [n.BLOCK_COMMENT, r, n.HEXCOLOR, n.CSS_NUMBER_MODE, e.QUOTE_STRING_MODE, e.APOS_STRING_MODE, n.IMPORTANT, n.FUNCTION_DISPATCH]
@@ -4205,15 +4245,15 @@
                 }, {
                     begin: "@",
                     end: "[{;]",
                     returnBegin: !0,
                     keywords: {
                         $pattern: /[a-z-]+/,
                         keyword: "and or not only",
-                        attribute: ie.join(" ")
+                        attribute: se.join(" ")
                     },
                     contains: [{
                         begin: i,
                         className: "keyword"
                     }, {
                         begin: /[a-z-]+(?=:)/,
                         className: "attribute"
@@ -4278,15 +4318,15 @@
                         type: i
                     }
                 }, {
                     className: "type",
                     begin: n.either("double precision", "large object", "with timezone", "without timezone")
                 }, c, {
                     className: "variable",
-                    begin: /@[a-z0-9]+/
+                    begin: /@[a-z0-9][a-z0-9_]*/
                 }, {
                     className: "string",
                     variants: [{
                         begin: /'/,
                         end: /'/,
                         contains: [{
                             begin: /''/
@@ -4311,301 +4351,303 @@
                     relevance: 0
                 },
                 t = e.COMMENT("/\\*", "\\*/", {
                     contains: ["self"]
                 }),
                 a = [e.C_LINE_COMMENT_MODE, t],
                 i = {
-                    match: [/\./, p(...ve, ...Oe)],
+                    match: [/\./, m(...xe, ...Me)],
                     className: {
                         2: "keyword"
                     }
                 },
                 r = {
-                    match: m(/\./, p(...xe)),
+                    match: b(/\./, m(...Ae)),
                     relevance: 0
                 },
-                s = xe.filter((e => "string" == typeof e)).concat(["_|0"]),
+                s = Ae.filter((e => "string" == typeof e)).concat(["_|0"]),
                 o = {
                     variants: [{
                         className: "keyword",
-                        match: p(...xe.filter((e => "string" != typeof e)).concat(ke).map(Ne), ...Oe)
+                        match: m(...Ae.filter((e => "string" != typeof e)).concat(Se).map(ke), ...Me)
                     }]
                 },
                 l = {
-                    $pattern: p(/\b\w+/, /#\w+/),
-                    keyword: s.concat(Ae),
-                    literal: Me
+                    $pattern: m(/\b\w+/, /#\w+/),
+                    keyword: s.concat(Re),
+                    literal: Ce
                 },
                 c = [i, r, o],
-                d = [{
-                    match: m(/\./, p(...Ce)),
+                g = [{
+                    match: b(/\./, m(...De)),
                     relevance: 0
                 }, {
                     className: "built_in",
-                    match: m(/\b/, p(...Ce), /(?=\()/)
+                    match: b(/\b/, m(...De), /(?=\()/)
                 }],
                 u = {
                     match: /->/,
                     relevance: 0
                 },
-                b = [u, {
+                p = [u, {
                     className: "operator",
                     relevance: 0,
                     variants: [{
-                        match: De
+                        match: Be
                     }, {
-                        match: `\\.(\\.|${Re})+`
+                        match: `\\.(\\.|${Le})+`
                     }]
                 }],
-                _ = "([0-9a-fA-F]_*)+",
-                h = {
+                _ = "([0-9]_*)+",
+                h = "([0-9a-fA-F]_*)+",
+                f = {
                     className: "number",
                     relevance: 0,
                     variants: [{
-                        match: "\\b(([0-9]_*)+)(\\.(([0-9]_*)+))?([eE][+-]?(([0-9]_*)+))?\\b"
+                        match: `\\b(${_})(\\.(${_}))?([eE][+-]?(${_}))?\\b`
                     }, {
-                        match: `\\b0x(${_})(\\.(${_}))?([pP][+-]?(([0-9]_*)+))?\\b`
+                        match: `\\b0x(${h})(\\.(${h}))?([pP][+-]?(${_}))?\\b`
                     }, {
                         match: /\b0o([0-7]_*)+\b/
                     }, {
                         match: /\b0b([01]_*)+\b/
                     }]
                 },
-                f = (e = "") => ({
+                E = (e = "") => ({
                     className: "subst",
                     variants: [{
-                        match: m(/\\/, e, /[0\\tnr"']/)
+                        match: b(/\\/, e, /[0\\tnr"']/)
                     }, {
-                        match: m(/\\/, e, /u\{[0-9a-fA-F]{1,8}\}/)
+                        match: b(/\\/, e, /u\{[0-9a-fA-F]{1,8}\}/)
                     }]
                 }),
-                E = (e = "") => ({
+                y = (e = "") => ({
                     className: "subst",
-                    match: m(/\\/, e, /[\t ]*(?:[\r\n]|\r\n)/)
+                    match: b(/\\/, e, /[\t ]*(?:[\r\n]|\r\n)/)
                 }),
-                y = (e = "") => ({
+                N = (e = "") => ({
                     className: "subst",
                     label: "interpol",
-                    begin: m(/\\/, e, /\(/),
+                    begin: b(/\\/, e, /\(/),
                     end: /\)/
                 }),
                 w = (e = "") => ({
-                    begin: m(e, /"""/),
-                    end: m(/"""/, e),
-                    contains: [f(e), E(e), y(e)]
+                    begin: b(e, /"""/),
+                    end: b(/"""/, e),
+                    contains: [E(e), y(e), N(e)]
                 }),
-                N = (e = "") => ({
-                    begin: m(e, /"/),
-                    end: m(/"/, e),
-                    contains: [f(e), y(e)]
+                v = (e = "") => ({
+                    begin: b(e, /"/),
+                    end: b(/"/, e),
+                    contains: [E(e), N(e)]
                 }),
-                v = {
+                O = {
                     className: "string",
-                    variants: [w(), w("#"), w("##"), w("###"), N(), N("#"), N("##"), N("###")]
+                    variants: [w(), w("#"), w("##"), w("###"), v(), v("#"), v("##"), v("###")]
                 },
-                O = {
-                    match: m(/`/, Be, /`/)
+                k = {
+                    match: b(/`/, Fe, /`/)
                 },
-                k = [O, {
+                x = [k, {
                     className: "variable",
                     match: /\$\d+/
                 }, {
                     className: "variable",
-                    match: `\\$${Le}+`
+                    match: `\\$${ze}+`
                 }],
-                x = [{
+                M = [{
                     match: /(@|#(un)?)available/,
                     className: "keyword",
                     starts: {
                         contains: [{
                             begin: /\(/,
                             end: /\)/,
-                            keywords: Fe,
-                            contains: [...b, h, v]
+                            keywords: Pe,
+                            contains: [...p, f, O]
                         }]
                     }
                 }, {
                     className: "keyword",
-                    match: m(/@/, p(...ze))
+                    match: b(/@/, m(...je))
                 }, {
                     className: "meta",
-                    match: m(/@/, Be)
+                    match: b(/@/, Fe)
                 }],
-                M = {
-                    match: g(/\b[A-Z]/),
+                S = {
+                    match: d(/\b[A-Z]/),
                     relevance: 0,
                     contains: [{
                         className: "type",
-                        match: m(/(AV|CA|CF|CG|CI|CL|CM|CN|CT|MK|MP|MTK|MTL|NS|SCN|SK|UI|WK|XC)/, Le, "+")
+                        match: b(/(AV|CA|CF|CG|CI|CL|CM|CN|CT|MK|MP|MTK|MTL|NS|SCN|SK|UI|WK|XC)/, ze, "+")
                     }, {
                         className: "type",
-                        match: $e,
+                        match: Ue,
                         relevance: 0
                     }, {
                         match: /[?!]+/,
                         relevance: 0
                     }, {
                         match: /\.\.\./,
                         relevance: 0
                     }, {
-                        match: m(/\s+&\s+/, g($e)),
+                        match: b(/\s+&\s+/, d(Ue)),
                         relevance: 0
                     }]
                 },
-                S = {
+                A = {
                     begin: /</,
                     end: />/,
                     keywords: l,
-                    contains: [...a, ...c, ...x, u, M]
+                    contains: [...a, ...c, ...M, u, S]
                 };
-            M.contains.push(S);
-            const A = {
+            S.contains.push(A);
+            const C = {
                     begin: /\(/,
                     end: /\)/,
                     relevance: 0,
                     keywords: l,
                     contains: ["self", {
-                        match: m(Be, /\s*:/),
+                        match: b(Fe, /\s*:/),
                         keywords: "_|0",
                         relevance: 0
-                    }, ...a, ...c, ...d, ...b, h, v, ...k, ...x, M]
+                    }, ...a, ...c, ...g, ...p, f, O, ...x, ...M, S]
                 },
-                C = {
+                T = {
                     begin: /</,
                     end: />/,
-                    contains: [...a, M]
+                    contains: [...a, S]
                 },
-                T = {
+                R = {
                     begin: /\(/,
                     end: /\)/,
                     keywords: l,
                     contains: [{
-                        begin: p(g(m(Be, /\s*:/)), g(m(Be, /\s+/, Be, /\s*:/))),
+                        begin: m(d(b(Fe, /\s*:/)), d(b(Fe, /\s+/, Fe, /\s*:/))),
                         end: /:/,
                         relevance: 0,
                         contains: [{
                             className: "keyword",
                             match: /\b_\b/
                         }, {
                             className: "params",
-                            match: Be
+                            match: Fe
                         }]
-                    }, ...a, ...c, ...b, h, v, ...x, M, A],
+                    }, ...a, ...c, ...p, f, O, ...M, S, C],
                     endsParent: !0,
                     illegal: /["']/
                 },
-                R = {
-                    match: [/func/, /\s+/, p(O.match, Be, De)],
+                D = {
+                    match: [/func/, /\s+/, m(k.match, Fe, Be)],
                     className: {
                         1: "keyword",
                         3: "title.function"
                     },
-                    contains: [C, T, n],
+                    contains: [T, R, n],
                     illegal: [/\[/, /%/]
                 },
-                D = {
+                I = {
                     match: [/\b(?:subscript|init[?!]?)/, /\s*(?=[<(])/],
                     className: {
                         1: "keyword"
                     },
-                    contains: [C, T, n],
+                    contains: [T, R, n],
                     illegal: /\[|%/
                 },
-                I = {
-                    match: [/operator/, /\s+/, De],
+                L = {
+                    match: [/operator/, /\s+/, Be],
                     className: {
                         1: "keyword",
                         3: "title"
                     }
                 },
-                L = {
-                    begin: [/precedencegroup/, /\s+/, $e],
+                B = {
+                    begin: [/precedencegroup/, /\s+/, Ue],
                     className: {
                         1: "keyword",
                         3: "title"
                     },
-                    contains: [M],
-                    keywords: [...Se, ...Me],
+                    contains: [S],
+                    keywords: [...Te, ...Ce],
                     end: /}/
                 };
-            for (const e of v.variants) {
+            for (const e of O.variants) {
                 const n = e.contains.find((e => "interpol" === e.label));
                 n.keywords = l;
-                const t = [...c, ...d, ...b, h, v, ...k];
+                const t = [...c, ...g, ...p, f, O, ...x];
                 n.contains = [...t, {
                     begin: /\(/,
                     end: /\)/,
                     contains: ["self", ...t]
                 }]
             }
             return {
                 name: "Swift",
                 keywords: l,
-                contains: [...a, R, D, {
+                contains: [...a, D, I, {
                     beginKeywords: "struct protocol class extension enum actor",
                     end: "\\{",
                     excludeEnd: !0,
                     keywords: l,
                     contains: [e.inherit(e.TITLE_MODE, {
                         className: "title.class",
                         begin: /[A-Za-z$_][\u00C0-\u02B80-9A-Za-z$_]*/
                     }), ...c]
-                }, I, L, {
+                }, L, B, {
                     beginKeywords: "import",
                     end: /$/,
                     contains: [...a],
                     relevance: 0
-                }, ...c, ...d, ...b, h, v, ...k, ...x, M, A]
+                }, ...c, ...g, ...p, f, O, ...x, ...M, S, C]
             }
         },
         grmr_typescript: e => {
-            const n = we(e),
-                t = ["any", "void", "number", "boolean", "string", "object", "never", "symbol", "bigint", "unknown"],
-                a = {
+            const n = Oe(e),
+                t = _e,
+                a = ["any", "void", "number", "boolean", "string", "object", "never", "symbol", "bigint", "unknown"],
+                i = {
                     beginKeywords: "namespace",
                     end: /\{/,
                     excludeEnd: !0,
                     contains: [n.exports.CLASS_REFERENCE]
                 },
-                i = {
+                r = {
                     beginKeywords: "interface",
                     end: /\{/,
                     excludeEnd: !0,
                     keywords: {
                         keyword: "interface extends",
-                        built_in: t
+                        built_in: a
                     },
                     contains: [n.exports.CLASS_REFERENCE]
                 },
-                r = {
-                    $pattern: be,
-                    keyword: me.concat(["type", "namespace", "interface", "public", "private", "protected", "implements", "declare", "abstract", "readonly", "enum", "override"]),
-                    literal: pe,
-                    built_in: ye.concat(t),
-                    "variable.language": Ee
-                },
                 s = {
+                    $pattern: _e,
+                    keyword: he.concat(["type", "namespace", "interface", "public", "private", "protected", "implements", "declare", "abstract", "readonly", "enum", "override"]),
+                    literal: fe,
+                    built_in: ve.concat(a),
+                    "variable.language": we
+                },
+                o = {
                     className: "meta",
-                    begin: "@[A-Za-z$_][0-9A-Za-z$_]*"
+                    begin: "@" + t
                 },
-                o = (e, n, t) => {
+                l = (e, n, t) => {
                     const a = e.contains.findIndex((e => e.label === n));
                     if (-1 === a) throw Error("can not find mode to replace");
                     e.contains.splice(a, 1, t)
                 };
-            return Object.assign(n.keywords, r),
-                n.exports.PARAMS_CONTAINS.push(s), n.contains = n.contains.concat([s, a, i]),
-                o(n, "shebang", e.SHEBANG()), o(n, "use_strict", {
+            return Object.assign(n.keywords, s),
+                n.exports.PARAMS_CONTAINS.push(o), n.contains = n.contains.concat([o, i, r]),
+                l(n, "shebang", e.SHEBANG()), l(n, "use_strict", {
                     className: "meta",
                     relevance: 10,
                     begin: /^\s*['"]use strict['"]/
                 }), n.contains.find((e => "func.def" === e.label)).relevance = 0, Object.assign(n, {
                     name: "TypeScript",
-                    aliases: ["ts", "tsx"]
+                    aliases: ["ts", "tsx", "mts", "cts"]
                 }), n
         },
         grmr_vbnet: e => {
             const n = e.regex,
                 t = /\d{1,2}\/\d{1,2}\/\d{4}/,
                 a = /\d{4}-\d{1,2}-\d{1,2}/,
                 i = /(\d|1[012])(:\d+){0,2} *(AM|PM)/,
@@ -4851,15 +4893,15 @@
                 name: "YAML",
                 case_insensitive: !0,
                 aliases: ["yml"],
                 contains: l
             }
         }
     });
-    const je = ne;
-    for (const e of Object.keys(Ue)) {
+    const qe = ae;
+    for (const e of Object.keys(Ke)) {
         const n = e.replace("grmr_", "").replace("_", "-");
-        je.registerLanguage(n, Ue[e])
+        qe.registerLanguage(n, Ke[e])
     }
-    return je
+    return qe
 }();
 "object" == typeof exports && "undefined" != typeof module && (module.exports = hljs);
```

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/js/mermaid.min.js` & `mkdocs-kpn-1.6.0/kpn_theme/js/mermaid.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/js/theme.js` & `mkdocs-kpn-1.6.0/kpn_theme/js/theme.js`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/nav.html` & `mkdocs-kpn-1.6.0/kpn_theme/nav.html`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/kpn_theme/search.html` & `mkdocs-kpn-1.6.0/kpn_theme/search.html`

 * *Files identical despite different names*

### Comparing `mkdocs-kpn-1.5.2/mkdocs_kpn.egg-info/PKG-INFO` & `mkdocs-kpn-1.6.0/mkdocs_kpn.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-kpn
-Version: 1.5.2
+Version: 1.6.0
 Summary: A KPN-styles theme for MkDocs
 Home-page: https://github.com/kpn/mkdocs-kpn-theme
 Author: Santiago Fraire Willemoës
 Author-email: de-ddci@kpn.com
 License: MIT
 Keywords: mkdocs,documentation,theme
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mkdocs-kpn-1.5.2/mkdocs_kpn.egg-info/SOURCES.txt` & `mkdocs-kpn-1.6.0/mkdocs_kpn.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,17 @@
 kpn_theme/img/logo-kpn.png
 kpn_theme/img/logo-kpn.svg
 kpn_theme/img/ui-bulb.svg
 kpn_theme/js/detail.js
 kpn_theme/js/highlight.min.js
 kpn_theme/js/mermaid.min.js
 kpn_theme/js/theme.js
+kpn_theme/js/languages/asciidoc.min.js
+kpn_theme/js/languages/groovy.min.js
+kpn_theme/js/languages/nix.min.js
 mkdocs_kpn.egg-info/PKG-INFO
 mkdocs_kpn.egg-info/SOURCES.txt
 mkdocs_kpn.egg-info/dependency_links.txt
 mkdocs_kpn.egg-info/entry_points.txt
 mkdocs_kpn.egg-info/not-zip-safe
 mkdocs_kpn.egg-info/requires.txt
 mkdocs_kpn.egg-info/top_level.txt
```

### Comparing `mkdocs-kpn-1.5.2/setup.py` & `mkdocs-kpn-1.6.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "1.5.2"
+VERSION = "1.6.0"
 
 
 def get_long_description():
     """
     Return the README.
     """
     with open("README.md", encoding="utf8") as f:
```

