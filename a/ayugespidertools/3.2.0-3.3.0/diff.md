# Comparing `tmp/ayugespidertools-3.2.0.tar.gz` & `tmp/ayugespidertools-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ayugespidertools-3.2.0.tar", max compression
+gzip compressed data, was "ayugespidertools-3.3.0.tar", max compression
```

## Comparing `ayugespidertools-3.2.0.tar` & `ayugespidertools-3.3.0.tar`

### file list

```diff
@@ -1,84 +1,83 @@
--rw-r--r--   0        0        0     1091 2023-01-29 07:51:47.000000 ayugespidertools-3.2.0/LICENSE
--rw-r--r--   0        0        0    14157 2023-06-07 06:26:34.000000 ayugespidertools-3.2.0/README.md
--rw-r--r--   0        0        0      482 2023-04-26 03:31:14.000000 ayugespidertools-3.2.0/ayugespidertools/__init__.py
--rw-r--r--   0        0        0        0 2023-04-18 02:21:23.000000 ayugespidertools-3.2.0/ayugespidertools/commands/__init__.py
--rw-r--r--   0        0        0      250 2023-02-23 07:01:46.000000 ayugespidertools-3.2.0/ayugespidertools/commands/crawl.py
--rw-r--r--   0        0        0      346 2023-02-10 19:57:28.000000 ayugespidertools-3.2.0/ayugespidertools/commands/genspider.py
--rw-r--r--   0        0        0     3880 2023-05-12 03:27:33.000000 ayugespidertools-3.2.0/ayugespidertools/commands/startproject.py
--rw-r--r--   0        0        0      524 2023-04-18 02:24:43.000000 ayugespidertools-3.2.0/ayugespidertools/commands/version.py
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.2.0/ayugespidertools/common/__init__.py
--rw-r--r--   0        0        0     3696 2023-06-07 02:13:50.000000 ayugespidertools-3.2.0/ayugespidertools/common/encryption.py
--rw-r--r--   0        0        0     6610 2023-06-07 02:13:56.000000 ayugespidertools-3.2.0/ayugespidertools/common/expend.py
--rw-r--r--   0        0        0     5269 2023-06-06 08:28:35.000000 ayugespidertools-3.2.0/ayugespidertools/common/mongodbpipe.py
--rw-r--r--   0        0        0    16994 2023-06-07 07:22:39.000000 ayugespidertools-3.2.0/ayugespidertools/common/multiplexing.py
--rw-r--r--   0        0        0    13306 2023-06-07 01:56:44.000000 ayugespidertools-3.2.0/ayugespidertools/common/mysqlerrhandle.py
--rw-r--r--   0        0        0    32707 2023-06-07 06:20:10.000000 ayugespidertools-3.2.0/ayugespidertools/common/params.py
--rw-r--r--   0        0        0     6000 2023-06-06 07:14:58.000000 ayugespidertools-3.2.0/ayugespidertools/common/spiderconf.py
--rw-r--r--   0        0        0     3718 2023-06-07 02:14:02.000000 ayugespidertools-3.2.0/ayugespidertools/common/sqlformat.py
--rw-r--r--   0        0        0     3158 2023-06-07 07:53:47.000000 ayugespidertools-3.2.0/ayugespidertools/common/typevars.py
--rw-r--r--   0        0        0    11402 2023-06-07 02:14:12.000000 ayugespidertools-3.2.0/ayugespidertools/common/utils.py
--rw-r--r--   0        0        0     3685 2023-06-07 02:14:19.000000 ayugespidertools-3.2.0/ayugespidertools/common/yidungap.py
--rw-r--r--   0        0        0      388 2023-06-07 02:14:26.000000 ayugespidertools-3.2.0/ayugespidertools/config.py
--rw-r--r--   0        0        0     9982 2023-06-07 02:14:34.000000 ayugespidertools-3.2.0/ayugespidertools/formatdata.py
--rw-r--r--   0        0        0     7673 2023-06-07 02:14:39.000000 ayugespidertools-3.2.0/ayugespidertools/imgoperation.py
--rw-r--r--   0        0        0     5065 2023-05-25 07:32:25.000000 ayugespidertools-3.2.0/ayugespidertools/items.py
--rw-r--r--   0        0        0      752 2023-06-07 06:21:31.000000 ayugespidertools-3.2.0/ayugespidertools/middlewares.py
--rw-r--r--   0        0        0     8542 2023-06-07 02:14:45.000000 ayugespidertools-3.2.0/ayugespidertools/mongoclient.py
--rw-r--r--   0        0        0     1132 2023-06-07 02:14:51.000000 ayugespidertools-3.2.0/ayugespidertools/mysqlclient.py
--rw-r--r--   0        0        0     5423 2023-06-07 02:14:57.000000 ayugespidertools-3.2.0/ayugespidertools/oss.py
--rw-r--r--   0        0        0     1015 2023-06-06 07:39:29.000000 ayugespidertools-3.2.0/ayugespidertools/pipelines.py
--rw-r--r--   0        0        0      209 2023-04-26 03:31:04.000000 ayugespidertools-3.2.0/ayugespidertools/request.py
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/__init__.py
--rw-r--r--   0        0        0      209 2023-04-26 03:31:29.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/http/__init__.py
--rw-r--r--   0        0        0     1350 2023-04-25 02:58:04.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/http/request/__init__.py
--rw-r--r--   0        0        0     1093 2023-04-27 08:03:48.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/http/request/form.py
--rw-r--r--   0        0        0     1049 2023-06-07 06:21:05.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/middlewares/__init__.py
--rw-r--r--   0        0        0     1734 2023-06-07 02:13:19.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/middlewares/headers/ua.py
--rw-r--r--   0        0        0      232 2023-06-07 06:21:21.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/middlewares/netlib/__init__.py
--rw-r--r--   0        0        0    10500 2023-06-07 06:02:16.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/middlewares/netlib/aiohttplib.py
--rw-r--r--   0        0        0      408 2023-04-24 02:20:24.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/middlewares/proxy/__init__.py
--rw-r--r--   0        0        0     3779 2023-06-07 02:15:17.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/middlewares/proxy/dynamic.py
--rw-r--r--   0        0        0     2429 2023-06-07 02:15:24.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/middlewares/proxy/exclusive.py
--rw-r--r--   0        0        0    11201 2023-04-25 02:59:35.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/middlewares/proxy/private.py
--rw-r--r--   0        0        0     1042 2023-05-26 07:14:18.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/__init__.py
--rw-r--r--   0        0        0      820 2023-02-10 19:57:28.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/download/file.py
--rw-r--r--   0        0        0      793 2023-02-10 19:57:28.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/download/image.py
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/mongo/__init__.py
--rw-r--r--   0        0        0     1569 2023-06-07 02:15:30.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/mongo/asynced.py
--rw-r--r--   0        0        0     2161 2023-06-06 09:22:26.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/mongo/fantasy.py
--rw-r--r--   0        0        0     1302 2023-06-06 08:33:11.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/mongo/twisted.py
--rw-r--r--   0        0        0      148 2023-05-26 02:23:50.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/msgproducer/__init__.py
--rw-r--r--   0        0        0     3132 2023-06-06 08:44:33.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/msgproducer/kafkapub.py
--rw-r--r--   0        0        0     1726 2023-06-07 07:28:59.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/msgproducer/mqpub.py
--rw-r--r--   0        0        0    11521 2023-06-06 08:20:22.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/mysql/__init__.py
--rw-r--r--   0        0        0     4109 2023-06-06 08:42:02.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/mysql/asynced.py
--rw-r--r--   0        0        0      338 2023-04-11 08:02:51.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/mysql/fantasy.py
--rw-r--r--   0        0        0     1754 2023-04-25 03:01:24.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/mysql/stats.py
--rw-r--r--   0        0        0     2734 2023-06-06 08:35:52.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/mysql/turbo.py
--rw-r--r--   0        0        0     3854 2023-06-06 08:41:13.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/mysql/twisted.py
--rw-r--r--   0        0        0     7938 2023-06-06 07:14:49.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/spiders/__init__.py
--rw-r--r--   0        0        0      442 2023-04-12 09:55:11.000000 ayugespidertools-3.2.0/ayugespidertools/scraper/spiders/crawl.py
--rw-r--r--   0        0        0      182 2023-04-25 03:15:03.000000 ayugespidertools-3.2.0/ayugespidertools/spiders.py
--rw-r--r--   0        0        0       36 2023-02-10 19:57:28.000000 ayugespidertools-3.2.0/ayugespidertools/templates/project/README.md
--rw-r--r--   0        0        0      820 2023-06-07 01:45:35.000000 ayugespidertools-3.2.0/ayugespidertools/templates/project/module/VIT/.conf
--rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-3.2.0/ayugespidertools/templates/project/module/__init__.py
--rw-r--r--   0        0        0      817 2023-04-25 08:43:59.000000 ayugespidertools-3.2.0/ayugespidertools/templates/project/module/items.py.tmpl
--rw-r--r--   0        0        0     3765 2023-02-10 19:57:28.000000 ayugespidertools-3.2.0/ayugespidertools/templates/project/module/middlewares.py.tmpl
--rw-r--r--   0        0        0      381 2023-01-29 07:51:47.000000 ayugespidertools-3.2.0/ayugespidertools/templates/project/module/pipelines.py.tmpl
--rw-r--r--   0        0        0       77 2023-02-10 19:57:28.000000 ayugespidertools-3.2.0/ayugespidertools/templates/project/module/run.py.tmpl
--rw-r--r--   0        0        0      164 2023-04-17 13:23:51.000000 ayugespidertools-3.2.0/ayugespidertools/templates/project/module/run.sh.tmpl
--rw-r--r--   0        0        0     1337 2023-05-17 09:02:33.000000 ayugespidertools-3.2.0/ayugespidertools/templates/project/module/settings.py.tmpl
--rw-r--r--   0        0        0      165 2023-01-29 07:51:47.000000 ayugespidertools-3.2.0/ayugespidertools/templates/project/module/spiders/__init__.py
--rw-r--r--   0        0        0       67 2023-02-10 19:57:28.000000 ayugespidertools-3.2.0/ayugespidertools/templates/project/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.2.0/ayugespidertools/templates/project/requirements.txt
--rw-r--r--   0        0        0      284 2023-02-03 06:47:49.000000 ayugespidertools-3.2.0/ayugespidertools/templates/project/scrapy.cfg
--rw-r--r--   0        0        0     1650 2023-04-25 06:08:11.000000 ayugespidertools-3.2.0/ayugespidertools/templates/spiders/async.tmpl
--rw-r--r--   0        0        0     5992 2023-06-07 07:57:01.000000 ayugespidertools-3.2.0/ayugespidertools/templates/spiders/basic.tmpl
--rw-r--r--   0        0        0     1685 2023-06-06 08:24:33.000000 ayugespidertools-3.2.0/ayugespidertools/templates/spiders/crawl.tmpl
--rw-r--r--   0        0        0      567 2023-02-03 02:54:45.000000 ayugespidertools-3.2.0/ayugespidertools/templates/spiders/csvfeed.tmpl
--rw-r--r--   0        0        0      559 2023-02-03 02:54:59.000000 ayugespidertools-3.2.0/ayugespidertools/templates/spiders/xmlfeed.tmpl
--rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-3.2.0/ayugespidertools/utils/__init__.py
--rw-r--r--   0        0        0     5943 2023-05-18 08:39:18.000000 ayugespidertools-3.2.0/ayugespidertools/utils/cmdline.py
--rw-r--r--   0        0        0     6924 2023-04-25 03:04:11.000000 ayugespidertools-3.2.0/ayugespidertools/verificationcode.py
--rw-r--r--   0        0        0     3073 2023-06-07 01:35:09.000000 ayugespidertools-3.2.0/pyproject.toml
--rw-r--r--   0        0        0    15887 1970-01-01 00:00:00.000000 ayugespidertools-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-01-29 07:51:47.000000 ayugespidertools-3.3.0/LICENSE
+-rw-r--r--   0        0        0    14144 2023-06-21 05:41:38.000000 ayugespidertools-3.3.0/README.md
+-rw-r--r--   0        0        0      433 2023-06-20 01:16:24.000000 ayugespidertools-3.3.0/ayugespidertools/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-18 02:21:23.000000 ayugespidertools-3.3.0/ayugespidertools/commands/__init__.py
+-rw-r--r--   0        0        0      250 2023-02-23 07:01:46.000000 ayugespidertools-3.3.0/ayugespidertools/commands/crawl.py
+-rw-r--r--   0        0        0      346 2023-02-10 19:57:28.000000 ayugespidertools-3.3.0/ayugespidertools/commands/genspider.py
+-rw-r--r--   0        0        0     3880 2023-05-12 03:27:33.000000 ayugespidertools-3.3.0/ayugespidertools/commands/startproject.py
+-rw-r--r--   0        0        0      524 2023-04-18 02:24:43.000000 ayugespidertools-3.3.0/ayugespidertools/commands/version.py
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.3.0/ayugespidertools/common/__init__.py
+-rw-r--r--   0        0        0     3696 2023-06-07 02:13:50.000000 ayugespidertools-3.3.0/ayugespidertools/common/encryption.py
+-rw-r--r--   0        0        0     6610 2023-06-07 02:13:56.000000 ayugespidertools-3.3.0/ayugespidertools/common/expend.py
+-rw-r--r--   0        0        0     5265 2023-06-09 09:17:13.000000 ayugespidertools-3.3.0/ayugespidertools/common/mongodbpipe.py
+-rw-r--r--   0        0        0    16918 2023-06-20 02:40:39.000000 ayugespidertools-3.3.0/ayugespidertools/common/multiplexing.py
+-rw-r--r--   0        0        0    13306 2023-06-07 01:56:44.000000 ayugespidertools-3.3.0/ayugespidertools/common/mysqlerrhandle.py
+-rw-r--r--   0        0        0    32649 2023-06-20 01:18:52.000000 ayugespidertools-3.3.0/ayugespidertools/common/params.py
+-rw-r--r--   0        0        0     6000 2023-06-06 07:14:58.000000 ayugespidertools-3.3.0/ayugespidertools/common/spiderconf.py
+-rw-r--r--   0        0        0     3718 2023-06-07 02:14:02.000000 ayugespidertools-3.3.0/ayugespidertools/common/sqlformat.py
+-rw-r--r--   0        0        0     3158 2023-06-07 07:53:47.000000 ayugespidertools-3.3.0/ayugespidertools/common/typevars.py
+-rw-r--r--   0        0        0    10672 2023-06-20 02:00:17.000000 ayugespidertools-3.3.0/ayugespidertools/common/utils.py
+-rw-r--r--   0        0        0     3685 2023-06-07 02:14:19.000000 ayugespidertools-3.3.0/ayugespidertools/common/yidungap.py
+-rw-r--r--   0        0        0      388 2023-06-07 02:14:26.000000 ayugespidertools-3.3.0/ayugespidertools/config.py
+-rw-r--r--   0        0        0     9982 2023-06-07 02:14:34.000000 ayugespidertools-3.3.0/ayugespidertools/formatdata.py
+-rw-r--r--   0        0        0     7673 2023-06-07 02:14:39.000000 ayugespidertools-3.3.0/ayugespidertools/imgoperation.py
+-rw-r--r--   0        0        0     4714 2023-06-21 02:16:27.000000 ayugespidertools-3.3.0/ayugespidertools/items.py
+-rw-r--r--   0        0        0      752 2023-06-07 06:21:31.000000 ayugespidertools-3.3.0/ayugespidertools/middlewares.py
+-rw-r--r--   0        0        0     8542 2023-06-07 02:14:45.000000 ayugespidertools-3.3.0/ayugespidertools/mongoclient.py
+-rw-r--r--   0        0        0     1132 2023-06-07 02:14:51.000000 ayugespidertools-3.3.0/ayugespidertools/mysqlclient.py
+-rw-r--r--   0        0        0     5448 2023-06-09 09:27:15.000000 ayugespidertools-3.3.0/ayugespidertools/oss.py
+-rw-r--r--   0        0        0     1129 2023-06-21 02:34:36.000000 ayugespidertools-3.3.0/ayugespidertools/pipelines.py
+-rw-r--r--   0        0        0      209 2023-04-26 03:31:04.000000 ayugespidertools-3.3.0/ayugespidertools/request.py
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/__init__.py
+-rw-r--r--   0        0        0      209 2023-04-26 03:31:29.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/http/__init__.py
+-rw-r--r--   0        0        0     1350 2023-04-25 02:58:04.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/http/request/__init__.py
+-rw-r--r--   0        0        0     1093 2023-04-27 08:03:48.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/http/request/form.py
+-rw-r--r--   0        0        0      900 2023-06-19 02:30:56.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/middlewares/__init__.py
+-rw-r--r--   0        0        0     1734 2023-06-07 02:13:19.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/middlewares/headers/ua.py
+-rw-r--r--   0        0        0      232 2023-06-07 06:21:21.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/middlewares/netlib/__init__.py
+-rw-r--r--   0        0        0    10562 2023-06-19 03:16:03.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/middlewares/netlib/aiohttplib.py
+-rw-r--r--   0        0        0      408 2023-04-24 02:20:24.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/middlewares/proxy/__init__.py
+-rw-r--r--   0        0        0     3779 2023-06-07 02:15:17.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/middlewares/proxy/dynamic.py
+-rw-r--r--   0        0        0     2429 2023-06-07 02:15:24.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/middlewares/proxy/exclusive.py
+-rw-r--r--   0        0        0     1154 2023-06-21 02:33:49.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-19 02:39:39.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/download/__init__.py
+-rw-r--r--   0        0        0     2453 2023-06-21 06:16:08.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/download/file.py
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/mongo/__init__.py
+-rw-r--r--   0        0        0     1495 2023-06-19 09:43:52.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/mongo/asynced.py
+-rw-r--r--   0        0        0     2046 2023-06-19 09:44:14.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/mongo/fantasy.py
+-rw-r--r--   0        0        0     1183 2023-06-19 09:44:52.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/mongo/twisted.py
+-rw-r--r--   0        0        0      148 2023-05-26 02:23:50.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/msgproducer/__init__.py
+-rw-r--r--   0        0        0     3180 2023-06-07 09:54:44.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/msgproducer/kafkapub.py
+-rw-r--r--   0        0        0     1779 2023-06-07 09:52:37.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/msgproducer/mqpub.py
+-rw-r--r--   0        0        0    11430 2023-06-20 02:32:25.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/mysql/__init__.py
+-rw-r--r--   0        0        0     3851 2023-06-19 09:45:42.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/mysql/asynced.py
+-rw-r--r--   0        0        0      338 2023-04-11 08:02:51.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/mysql/fantasy.py
+-rw-r--r--   0        0        0     1754 2023-06-16 03:09:25.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/mysql/stats.py
+-rw-r--r--   0        0        0     2734 2023-06-06 08:35:52.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/mysql/turbo.py
+-rw-r--r--   0        0        0     3608 2023-06-19 09:45:59.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/mysql/twisted.py
+-rw-r--r--   0        0        0     7944 2023-06-21 08:29:00.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/spiders/__init__.py
+-rw-r--r--   0        0        0      442 2023-04-12 09:55:11.000000 ayugespidertools-3.3.0/ayugespidertools/scraper/spiders/crawl.py
+-rw-r--r--   0        0        0      182 2023-04-25 03:15:03.000000 ayugespidertools-3.3.0/ayugespidertools/spiders.py
+-rw-r--r--   0        0        0       36 2023-02-10 19:57:28.000000 ayugespidertools-3.3.0/ayugespidertools/templates/project/README.md
+-rw-r--r--   0        0        0      820 2023-06-07 01:45:35.000000 ayugespidertools-3.3.0/ayugespidertools/templates/project/module/VIT/.conf
+-rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-3.3.0/ayugespidertools/templates/project/module/__init__.py
+-rw-r--r--   0        0        0      817 2023-04-25 08:43:59.000000 ayugespidertools-3.3.0/ayugespidertools/templates/project/module/items.py.tmpl
+-rw-r--r--   0        0        0     3765 2023-02-10 19:57:28.000000 ayugespidertools-3.3.0/ayugespidertools/templates/project/module/middlewares.py.tmpl
+-rw-r--r--   0        0        0      381 2023-01-29 07:51:47.000000 ayugespidertools-3.3.0/ayugespidertools/templates/project/module/pipelines.py.tmpl
+-rw-r--r--   0        0        0       77 2023-02-10 19:57:28.000000 ayugespidertools-3.3.0/ayugespidertools/templates/project/module/run.py.tmpl
+-rw-r--r--   0        0        0      164 2023-04-17 13:23:51.000000 ayugespidertools-3.3.0/ayugespidertools/templates/project/module/run.sh.tmpl
+-rw-r--r--   0        0        0     1337 2023-05-17 09:02:33.000000 ayugespidertools-3.3.0/ayugespidertools/templates/project/module/settings.py.tmpl
+-rw-r--r--   0        0        0      165 2023-01-29 07:51:47.000000 ayugespidertools-3.3.0/ayugespidertools/templates/project/module/spiders/__init__.py
+-rw-r--r--   0        0        0       67 2023-02-10 19:57:28.000000 ayugespidertools-3.3.0/ayugespidertools/templates/project/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.3.0/ayugespidertools/templates/project/requirements.txt
+-rw-r--r--   0        0        0      284 2023-02-03 06:47:49.000000 ayugespidertools-3.3.0/ayugespidertools/templates/project/scrapy.cfg
+-rw-r--r--   0        0        0     1650 2023-04-25 06:08:11.000000 ayugespidertools-3.3.0/ayugespidertools/templates/spiders/async.tmpl
+-rw-r--r--   0        0        0     5168 2023-06-21 08:26:39.000000 ayugespidertools-3.3.0/ayugespidertools/templates/spiders/basic.tmpl
+-rw-r--r--   0        0        0     1673 2023-06-20 01:20:48.000000 ayugespidertools-3.3.0/ayugespidertools/templates/spiders/crawl.tmpl
+-rw-r--r--   0        0        0      567 2023-02-03 02:54:45.000000 ayugespidertools-3.3.0/ayugespidertools/templates/spiders/csvfeed.tmpl
+-rw-r--r--   0        0        0      559 2023-02-03 02:54:59.000000 ayugespidertools-3.3.0/ayugespidertools/templates/spiders/xmlfeed.tmpl
+-rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-3.3.0/ayugespidertools/utils/__init__.py
+-rw-r--r--   0        0        0     5943 2023-05-18 08:39:18.000000 ayugespidertools-3.3.0/ayugespidertools/utils/cmdline.py
+-rw-r--r--   0        0        0     6924 2023-04-25 03:04:11.000000 ayugespidertools-3.3.0/ayugespidertools/verificationcode.py
+-rw-r--r--   0        0        0     3074 2023-06-21 07:30:30.000000 ayugespidertools-3.3.0/pyproject.toml
+-rw-r--r--   0        0        0    15883 1970-01-01 00:00:00.000000 ayugespidertools-3.3.0/PKG-INFO
```

### Comparing `ayugespidertools-3.2.0/LICENSE` & `ayugespidertools-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.2.0/README.md` & `ayugespidertools-3.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # AyugeSpiderTools 工具说明
 
 > 一句话介绍：用于扩展 `Scrapy` 功能来解放双手，还内置一些爬虫开发中的通用方法。
 
 ## 前言
 
-在使用 `Python` `Scrapy` 库开发爬虫时，免不了会重复的修改和编写 `settings.py`，`middlewares.py`，`pipelines.py`，`item.py` 和一些通用方法或脚本，但其实各个项目中的这些文件内容大致相同，那为何不把他们统一整理在一起呢。虽说可以使用 `scrapy` 的模板功能，但还是无法适配所有的开发场景。
+在使用 `Python` `Scrapy` 库开发爬虫时，免不了会重复的修改和编写 `settings.py`，`item.py`，`middlewares.py`，`pipelines.py` 和一些通用方法或脚本，但其实各个项目中的这些文件内容大致相同，那为何不把他们统一整理在一起呢。虽说可以使用 `scrapy` 的模板功能，但还是无法适配所有的开发场景。
 
 刚开始我也只是想把它用来适配 `Mysql` 存储的场景，可以自动创建相关数据库，数据表，字段注释，自动添加新添加的字段，和自动修复常见（字段编码，`Data too long`，存储字段不存在等等）的存储问题。后来不断优化和添加各种场景，使得爬虫开发在通用场景下几乎只用在意 `spider` 脚本的解析规则和 `VIT` 下的 `.conf` 配置即可，脱离无意义的重复操作。
 
 至于此库做了哪些功能，只要你熟悉 `python` 语法和 `scrapy` 库，再结合 [DemoSpider](https://github.com/shengchenyang/DemoSpider) 中的应用示例，你可以很快上手。具体的内容和注意事项也可以在 [AyugeSpiderTools readthedocs 文档](https://ayugespidertools.readthedocs.io/en/latest/) 中查看。
 
 ## 1. 前提条件
 
@@ -47,16 +47,14 @@
 使用方法示例 `GIF` 如下：
 
 ![ayugespidertools.gif](https://raw.githubusercontent.com/shengchenyang/AyugeSpiderTools/main/examples/ayugespidertools-use.gif)
 
 对以上 `GIF` 中的步骤进行解释：
 
 ```shell
-# 注：ayugespidertools 的 cli 已剔除，现只能使用 ayuge。
-
 # 查看库版本
 ayuge version
 
 # 创建项目
 ayuge startproject <project_name>
 
 # 进入项目根目录
@@ -105,15 +103,16 @@
 
 # 本库中给出支持 Item Loaders 特性的示例(文档地址：https://ayugespidertools.readthedocs.io/en/latest/topics/loaders.html)
 +15).demo_item_loader: 本库中使用 Item Loaders 的示例
 -16).demo_item_loader_two: 展示本库使用 itemLoader 特性的示例，此示例已删除，可查看上个 demo_item_loader 中的示例，目前已经可以很方便的使用 Item Loaders 功能了
 
 +17).demo_mongo_async: asyncio 版本存储 mongoDB 的 pipelines 示例
 +18).demo_mq: 数据存入 rabbitmq 的模板示例
-+19).demo_kafka: 数据存入 rabbitmq 的模板示例
++19).demo_kafka: 数据存入 kafka 的模板示例
++20).demo_file: 下载图片等文件到本地的模板示例
 ```
 
 注：具体内容及时效性请以 [DemoSpider](https://github.com/shengchenyang/DemoSpider) 项目中描述为准。
 
 ### 2.2. 开发场景
 
 > 这里不再一一列举所有功能，大概介绍下包含的大致功能。
```

### Comparing `ayugespidertools-3.2.0/ayugespidertools/commands/startproject.py` & `ayugespidertools-3.3.0/ayugespidertools/commands/startproject.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.2.0/ayugespidertools/commands/version.py` & `ayugespidertools-3.3.0/ayugespidertools/commands/version.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.2.0/ayugespidertools/common/encryption.py` & `ayugespidertools-3.3.0/ayugespidertools/common/encryption.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.2.0/ayugespidertools/common/expend.py` & `ayugespidertools-3.3.0/ayugespidertools/common/expend.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.2.0/ayugespidertools/common/mongodbpipe.py` & `ayugespidertools-3.3.0/ayugespidertools/common/mongodbpipe.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             item_dict: item ItemAdapter 或者 dict 格式数据，可像字典一样操作
 
         Returns:
             None
         """
         insert_data = ReuseOperation.get_items_except_keys(
             dict_conf=item_dict,
-            key_list=["_table", "_item_mode", "_mongo_update_rule"],
+            keys=["_table", "_item_mode", "_mongo_update_rule"],
         )
         judge_item = next(iter(insert_data.values()))
         # 是 namedtuple 类型
         if ReuseOperation.is_namedtuple_instance(judge_item):
             insert_data = {v: insert_data[v].key_value for v in insert_data.keys()}
         # 是普通的 dict 格式，则直接为 insert_data
         return insert_data
```

### Comparing `ayugespidertools-3.2.0/ayugespidertools/common/multiplexing.py` & `ayugespidertools-3.3.0/ayugespidertools/common/multiplexing.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,20 +4,21 @@
 import os
 import random
 from typing import Any, List, Union
 
 import cv2
 import numpy as np
 import pymysql
+from itemadapter import ItemAdapter
 from scrapy.settings import Settings
 from twisted.internet.defer import Deferred
 
 from ayugespidertools.common.typevars import MysqlConf
 from ayugespidertools.config import logger
-from ayugespidertools.items import MongoDataItem, MysqlDataItem, ScrapyItem
+from ayugespidertools.items import AyuItem, ScrapyItem
 
 __all__ = [
     "ReuseOperation",
 ]
 
 
 class ReuseOperation:
@@ -137,28 +138,26 @@
             "topic": config_parser.get("kafka", "topic", fallback=None),
             "key": config_parser.get("kafka", "key", fallback=None),
         }
         return inner_settings
 
     @staticmethod
     def item_to_dict(
-        item: Union[MysqlDataItem, MongoDataItem, ScrapyItem, dict]
-    ) -> dict:
+        item: Union[AyuItem, ScrapyItem, dict]
+    ) -> Union[ItemAdapter, dict]:
         """
         将 item 转换为 dict 类型
         将 spider 中的 yield 的 item 转换为 dict 类型，方便后续处理
         Args:
             item: spider 中的 yield 的 item
 
         Returns:
             1). dict 类型的 item
         """
-        if isinstance(item, (MongoDataItem, MysqlDataItem)):
-            return item.asdict()
-        return dict(item)
+        return item.asdict() if isinstance(item, AyuItem) else ItemAdapter(item)
 
     @staticmethod
     def is_namedtuple_instance(x: Any) -> bool:
         """
         判断 x 是否为 namedtuple 类型
         Args:
             x: 需要判断的参数
@@ -172,15 +171,15 @@
     def get_files_from_path(path: str) -> list:
         """
         获取 path 文件夹下的所有文件，而且输出以 path 为根目录的相对路径
         Args:
             path: 需要判断的文件夹路径
 
         Returns:
-            file_list: path 文件夹下的文件列表
+            1). path 文件夹下的文件列表
         """
         return [f.path for f in os.scandir(path) if f.is_file()]
 
     @staticmethod
     def get_bytes_by_file(file_path: str) -> bytes:
         """
         获取媒体文件的 bytes 内容
@@ -268,44 +267,44 @@
 
         return all(key in dict_conf for key in key_list)
 
     @classmethod
     def get_items_by_keys(
         cls,
         dict_conf: dict,
-        key_list: List[str],
+        keys: List[str],
     ) -> dict:
         """
-        获取 dict_conf 中的含有 key_list 的 key 的字段
+        获取 dict_conf 中的含有 keys 的 key 的字段
         Args:
             dict_conf: 需要处理的参数
-            key_list: 需要取的 key 值列表
+            keys: 需要取的 key 值列表
 
         Returns:
             1). 取值后的 dict，或不满足请求的 False 值
         """
         # 参数先要满足最小限定，然后再取出限定的参数值；否则返回空字典
         return (
-            {k: dict_conf[k] for k in key_list}
-            if cls.is_dict_meet_min_limit(dict_conf=dict_conf, key_list=key_list)
+            {k: dict_conf[k] for k in keys}
+            if cls.is_dict_meet_min_limit(dict_conf=dict_conf, key_list=keys)
             else {}
         )
 
     @classmethod
-    def get_items_except_keys(cls, dict_conf, key_list: List[str]) -> dict:
+    def get_items_except_keys(cls, dict_conf, keys: List[str]) -> dict:
         """
-        获取 dict_conf 中的不含有 key_list 的 key 的字段
+        获取 dict_conf 中的不含有 keys 的 key 的字段
         Args:
             dict_conf: 需要处理的参数
-            key_list: 需要排除的 key 值列表
+            keys: 需要排除的 key 值列表
 
         Returns:
-            1). dict_conf 排除 key_list 中的键值后的值
+            1). dict_conf 排除 keys 中的键值后的值
         """
-        return {k: dict_conf[k] for k in dict_conf if k not in key_list}
+        return {k: dict_conf[k] for k in dict_conf if k not in keys}
 
     @classmethod
     def create_database(cls, mysql_conf: MysqlConf) -> None:
         """
         创建数据库
         由于这是在连接数据库，报数据库不存在错误时的场景，则需要新建(不指定数据库)连接创建好所需数据库即可
         Args:
@@ -384,15 +383,15 @@
             settings: scrapy 的 settings 信息
 
         Returns:
             consul_conf_dict_min: 满足要求的最少要求的 consul 配置
         """
         consul_conf_dict = settings.get("CONSUL_CONFIG", {})
         return cls.get_items_by_keys(
-            dict_conf=consul_conf_dict, key_list=["token", "url", "format"]
+            dict_conf=consul_conf_dict, keys=["token", "url", "format"]
         )
 
     @classmethod
     def judge_str_is_json(cls, judge_str: str) -> bool:
         """
         判断字符串是否为 json 格式
         Args:
```

### Comparing `ayugespidertools-3.2.0/ayugespidertools/common/mysqlerrhandle.py` & `ayugespidertools-3.3.0/ayugespidertools/common/mysqlerrhandle.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.2.0/ayugespidertools/common/params.py` & `ayugespidertools-3.3.0/ayugespidertools/common/params.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import List, TypeVar
 
 # 用于 type hint，不要删除
 import pymongo
 import pymysql
 from itemadapter import ItemAdapter
 
-from ayugespidertools.items import MongoDataItem, MysqlDataItem, ScrapyClassicItem
+from ayugespidertools.items import AyuItem, ScrapyClassicItem
 
 __all__ = [
     "Param",
 ]
 
 
 class Param:
@@ -27,17 +27,15 @@
     Str_Lstr = TypeVar("Str_Lstr", str, List[str])
     PymongoDataBase = TypeVar("PymongoDataBase", bound="pymongo.database.Database")
     PymysqlConnect = TypeVar("PymysqlConnect", bound="pymysql.connections.Connection")
     PymysqlCursor = TypeVar("PymysqlCursor", bound="pymysql.cursors.Cursor")
     PymysqlDictCursor = TypeVar("PymysqlDictCursor", bound="pymysql.cursors.DictCursor")
     ItemAdapterType = TypeVar("ItemAdapterType", bound="ItemAdapter")
     # 此框架中 Item 的类型种类
-    ScrapyItems = TypeVar(
-        "ScrapyItems", MysqlDataItem, MongoDataItem, ScrapyClassicItem
-    )
+    ScrapyItems = TypeVar("ScrapyItems", AyuItem, ScrapyClassicItem)
 
     # 基本的请求头
     base_headers = {
         "Connection": "close",
         "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/93.0.4577.82 Safari/537.36",
     }
```

### Comparing `ayugespidertools-3.2.0/ayugespidertools/common/spiderconf.py` & `ayugespidertools-3.3.0/ayugespidertools/common/spiderconf.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.2.0/ayugespidertools/common/sqlformat.py` & `ayugespidertools-3.3.0/ayugespidertools/common/sqlformat.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.2.0/ayugespidertools/common/typevars.py` & `ayugespidertools-3.3.0/ayugespidertools/common/typevars.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.2.0/ayugespidertools/common/utils.py` & `ayugespidertools-3.3.0/ayugespidertools/common/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from typing import Any, List, Literal, Optional, Union
 from urllib.parse import urlparse
 
 import hcl2
 import pandas
 import requests
 import yaml
-from itemadapter import ItemAdapter
 
 from ayugespidertools.common.encryption import EncryptOperation
 from ayugespidertools.common.multiplexing import ReuseOperation
 from ayugespidertools.common.params import Param
 from ayugespidertools.common.typevars import MysqlConf
 from ayugespidertools.config import logger
 from ayugespidertools.formatdata import DataHandle
@@ -240,32 +239,14 @@
         collate = charset_collate_map.get(mysql_conf.charset)
         assert (
             collate is not None
         ), f"数据库配置出现未知 charset：{mysql_conf.charset}，若抛错请查看或手动创建所需数据表！"
         return collate
 
     @staticmethod
-    def convert_items_to_dict(item) -> ItemAdapter:
-        """
-        数据容器对象的包装器，提供了一个通用接口以统一的方式处理不同类型的对象，而不管它们的底层实现如何。
-        目前支持的类型有：
-            1. scrapy.item.Item
-            2. dict
-            3. dataclass 基础类
-            4. attrs 基础类
-            5. pydantic 基础类
-        Args:
-            item: 需要转换的项目，请查看支持类型
-
-        Returns:
-            1). 转换的 ItemAdapter 结果，可以通过  obj["params"] 或 obj.get("params") 来取值
-        """
-        return ItemAdapter(item)
-
-    @staticmethod
     def first_not_none(data_lst: List[Any]) -> Any:
         """
         获取列表中第一个不为 None 的值
         Args:
             data_lst: 数据列表
 
         Returns:
```

### Comparing `ayugespidertools-3.2.0/ayugespidertools/common/yidungap.py` & `ayugespidertools-3.3.0/ayugespidertools/common/yidungap.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.2.0/ayugespidertools/formatdata.py` & `ayugespidertools-3.3.0/ayugespidertools/formatdata.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.2.0/ayugespidertools/imgoperation.py` & `ayugespidertools-3.3.0/ayugespidertools/imgoperation.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.2.0/ayugespidertools/middlewares.py` & `ayugespidertools-3.3.0/ayugespidertools/middlewares.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.2.0/ayugespidertools/mongoclient.py` & `ayugespidertools-3.3.0/ayugespidertools/mongoclient.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.2.0/ayugespidertools/mysqlclient.py` & `ayugespidertools-3.3.0/ayugespidertools/mysqlclient.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.2.0/ayugespidertools/oss.py` & `ayugespidertools-3.3.0/ayugespidertools/oss.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,17 @@
                 put_bytes_or_url,
             )
         except Exception:
             return False, ""
         return True, input_file_name
 
     def enumer_file_by_pre(
-        self, prefix: str, count_by_type: Union[Param.Str_Lstr, Param.NoneType] = None
+        self,
+        prefix: str,
+        count_by_type: Union[Param.Str_Lstr, Param.NoneType, list] = None,
     ) -> list:
         """
         列举 prefix 文件夹下的所有的 count_by_type 类型的文件元素
         Args:
             prefix: 文件夹目录
             count_by_type: 统计的依据，计数文件夹中的此类型的元素
                 参数示例如下:
```

### Comparing `ayugespidertools-3.2.0/ayugespidertools/pipelines.py` & `ayugespidertools-3.3.0/ayugespidertools/pipelines.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from ayugespidertools.scraper.pipelines.download.file import FilesDownloadPipeline
 from ayugespidertools.scraper.pipelines.mongo.asynced import AsyncMongoPipeline
 from ayugespidertools.scraper.pipelines.mongo.fantasy import AyuFtyMongoPipeline
 from ayugespidertools.scraper.pipelines.mongo.twisted import AyuTwistedMongoPipeline
 from ayugespidertools.scraper.pipelines.msgproducer.kafkapub import AyuKafkaPipeline
 from ayugespidertools.scraper.pipelines.msgproducer.mqpub import AyuMQPipeline
 from ayugespidertools.scraper.pipelines.mysql.asynced import AsyncMysqlPipeline
 from ayugespidertools.scraper.pipelines.mysql.fantasy import AyuFtyMysqlPipeline
@@ -14,8 +15,9 @@
     "AyuTwistedMysqlPipeline",
     "AsyncMongoPipeline",
     "AsyncMysqlPipeline",
     "AyuFtyMongoPipeline",
     "AyuTwistedMongoPipeline",
     "AyuMQPipeline",
     "AyuKafkaPipeline",
+    "FilesDownloadPipeline",
 ]
```

### Comparing `ayugespidertools-3.2.0/ayugespidertools/scraper/http/request/__init__.py` & `ayugespidertools-3.3.0/ayugespidertools/scraper/http/request/__init__.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.2.0/ayugespidertools/scraper/http/request/form.py` & `ayugespidertools-3.3.0/ayugespidertools/scraper/http/request/form.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.2.0/ayugespidertools/scraper/middlewares/__init__.py` & `ayugespidertools-3.3.0/ayugespidertools/scraper/middlewares/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,20 +10,16 @@
 from ayugespidertools.scraper.middlewares.proxy.dynamic import (
     AbuDynamicProxyDownloaderMiddleware,
     DynamicProxyDownloaderMiddleware,
 )
 from ayugespidertools.scraper.middlewares.proxy.exclusive import (
     ExclusiveProxyDownloaderMiddleware,
 )
-from ayugespidertools.scraper.middlewares.proxy.private import (
-    PrivateProxyDownloaderMiddleware,
-)
 
 __all__ = [
     "RandomRequestUaMiddleware",
     "AiohttpAsyncDownloaderMiddleware",
     "AiohttpDownloaderMiddleware",
     "DynamicProxyDownloaderMiddleware",
     "AbuDynamicProxyDownloaderMiddleware",
     "ExclusiveProxyDownloaderMiddleware",
-    "PrivateProxyDownloaderMiddleware",
 ]
```

### Comparing `ayugespidertools-3.2.0/ayugespidertools/scraper/middlewares/headers/ua.py` & `ayugespidertools-3.3.0/ayugespidertools/scraper/middlewares/headers/ua.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.2.0/ayugespidertools/scraper/middlewares/netlib/aiohttplib.py` & `ayugespidertools-3.3.0/ayugespidertools/scraper/middlewares/netlib/aiohttplib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import asyncio
 from typing import Optional, Union
 
 import aiohttp
 import scrapy
 from aiohttp.connector import BaseConnector
+from itemadapter import ItemAdapter
 from scrapy.http import HtmlResponse
 from scrapy.utils.python import global_object_name
 
 from ayugespidertools.common.multiplexing import ReuseOperation
 from ayugespidertools.common.params import Param
 from ayugespidertools.common.typevars import AiohttpConf, AiohttpRequestArgs
 from ayugespidertools.common.utils import ToolsForAyu
@@ -37,37 +38,38 @@
         重试请求
         Args:
             request: scrapy request
             reason: reason
             spider: scrapy spider
 
         Returns:
-            retryreq: 重试的 request 对象
+            retry_req: 重试的 request 对象
         """
         retries = request.meta.get("retry_times", 0) + 1
         stats = spider.crawler.stats
         if retries <= self.retry_times:
-            logger.debug(f"Retrying {request} (failed {retries} times): {reason}")
-            retryreq = request.copy()
-            retryreq.meta["retry_times"] = retries
-            retryreq.dont_filter = True
-            # 优先级逐级降低，以防堆积
-            retryreq.priority = request.priority + self.priority_adjust
-
-            if isinstance(reason, Exception):
-                reason = global_object_name(reason.__class__)
-
-            stats.inc_value("retry/count")
-            stats.inc_value(f"retry/reason_count/{reason}")
-            return retryreq
-        else:
-            stats.inc_value("retry/max_reached")
-            logger.error(
-                f"Gave up retrying {request} (failed {retries} times): {reason}"
-            )
+            return self._retry_with_limit(request, retries, reason, stats)
+
+        stats.inc_value("retry/max_reached")
+        logger.error(f"Gave up retrying {request} (failed {retries} times): {reason}")
+
+    def _retry_with_limit(self, request, retries, reason, stats):
+        logger.debug(f"Retrying {request} (failed {retries} times): {reason}")
+        retry_req = request.copy()
+        retry_req.meta["retry_times"] = retries
+        retry_req.dont_filter = True
+        # 优先级逐级降低，以防堆积
+        retry_req.priority = request.priority + self.priority_adjust
+
+        if isinstance(reason, Exception):
+            reason = global_object_name(reason.__class__)
+
+        stats.inc_value("retry/count")
+        stats.inc_value(f"retry/reason_count/{reason}")
+        return retry_req
 
     def _get_args(self, key: str):
         """
         根据优先级依次获取不为 None 的请求参数
         """
         data_lst = [
             self.aiohttp_args.get(key),
@@ -216,15 +218,15 @@
         # 请求超时设置
         _timeout_obj = None
         if _timeout := self.aiohttp_args.get("timeout"):
             aiohttp_req_args.timeout = _timeout
         elif self.timeout is not None:
             _timeout_obj = aiohttp.ClientTimeout(total=self.timeout)
 
-        aio_request_args = ToolsForAyu.convert_items_to_dict(item=aiohttp_req_args)
+        aio_request_args = ItemAdapter(aiohttp_req_args)
         status_code, html_content = await self._request_by_aiohttp(
             timeout=_timeout_obj,
             aio_request_args=aio_request_args,
             connector=_connector,
         )
 
         # 请求间隔设置
```

### Comparing `ayugespidertools-3.2.0/ayugespidertools/scraper/middlewares/proxy/dynamic.py` & `ayugespidertools-3.3.0/ayugespidertools/scraper/middlewares/proxy/dynamic.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.2.0/ayugespidertools/scraper/middlewares/proxy/exclusive.py` & `ayugespidertools-3.3.0/ayugespidertools/scraper/middlewares/proxy/exclusive.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/__init__.py` & `ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Define your item pipelines here
 #
 # Don"t forget to add your pipeline to the ITEM_PIPELINES setting
 # See: https://docs.scrapy.org/en/latest/topics/item-pipeline.html
+from ayugespidertools.scraper.pipelines.download.file import FilesDownloadPipeline
 from ayugespidertools.scraper.pipelines.mongo.fantasy import AyuFtyMongoPipeline
 from ayugespidertools.scraper.pipelines.mongo.twisted import AyuTwistedMongoPipeline
 from ayugespidertools.scraper.pipelines.msgproducer.mqpub import AyuMQPipeline
 from ayugespidertools.scraper.pipelines.mysql import AyuMysqlPipeline
 from ayugespidertools.scraper.pipelines.mysql.asynced import AsyncMysqlPipeline
 from ayugespidertools.scraper.pipelines.mysql.fantasy import AyuFtyMysqlPipeline
 from ayugespidertools.scraper.pipelines.mysql.turbo import AyuTurboMysqlPipeline
@@ -16,8 +17,9 @@
     "AyuFtyMysqlPipeline",
     "AyuTurboMysqlPipeline",
     "AyuTwistedMysqlPipeline",
     "AsyncMysqlPipeline",
     "AyuFtyMongoPipeline",
     "AyuTwistedMongoPipeline",
     "AyuMQPipeline",
+    "FilesDownloadPipeline",
 ]
```

### Comparing `ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/mongo/asynced.py` & `ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/mongo/asynced.py`

 * *Files 18% similar despite different names*

```diff
@@ -30,15 +30,14 @@
         self.db = self.client[spider.mongodb_conf.database]
 
     async def close_spider(self, spider):
         self.client.close()
 
     async def process_item(self, item, spider):
         item_dict = ReuseOperation.item_to_dict(item)
-        if item_dict["_item_mode"] == "MongoDB":
-            await asyncio.shield(
-                AsyncioAsynchronous().process_item_template(
-                    item_dict=item_dict,
-                    db=self.db,
-                )
+        await asyncio.shield(
+            AsyncioAsynchronous().process_item_template(
+                item_dict=item_dict,
+                db=self.db,
             )
+        )
         return item
```

### Comparing `ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/mongo/fantasy.py` & `ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/mongo/fantasy.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,15 +49,13 @@
             item: scrapy item
             spider: scrapy spider
 
         Returns:
             item: scrapy item
         """
         item_dict = ReuseOperation.item_to_dict(item)
-        # 先查看存储场景是否匹配
-        if item_dict["_item_mode"] == "MongoDB":
-            mongodb_pipe(
-                Synchronize(),
-                item_dict=item_dict,
-                db=self.db,
-            )
+        mongodb_pipe(
+            Synchronize(),
+            item_dict=item_dict,
+            db=self.db,
+        )
         return item
```

### Comparing `ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/mongo/twisted.py` & `ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/mongo/twisted.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,15 +26,13 @@
         out = defer.Deferred()
         reactor.callInThread(self.db_insert, item, out)
         yield out
         defer.returnValue(item)
 
     def db_insert(self, item, out):
         item_dict = ReuseOperation.item_to_dict(item)
-        # 先查看存储场景是否匹配
-        if item_dict["_item_mode"] == "MongoDB":
-            mongodb_pipe(
-                TwistedAsynchronous(),
-                item_dict=item_dict,
-                db=self.db,
-            )
-            reactor.callFromThread(out.callback, item_dict)
+        mongodb_pipe(
+            TwistedAsynchronous(),
+            item_dict=item_dict,
+            db=self.db,
+        )
+        reactor.callFromThread(out.callback, item_dict)
```

### Comparing `ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/msgproducer/kafkapub.py` & `ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/msgproducer/kafkapub.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,14 +81,17 @@
 
     def close_producer(self):
         if self.producer:
             self.producer.close()
 
 
 class AyuKafkaPipeline:
+    def __init__(self):
+        self.kp = None
+
     def open_spider(self, spider):
         # 如果有多个 kafka 服务地址，用逗号分隔，会在此处拆分为列表
         _bts = spider.kafka_conf.bootstrap_servers
         bts_lst = _bts.split(",")
         self.kp = KafkaProducerClient(bootstrap_servers=bts_lst)
 
     def process_item(self, item, spider):
```

### Comparing `ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/msgproducer/mqpub.py` & `ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/msgproducer/mqpub.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 
 
 class AyuMQPipeline:
     """
     消息队列发布场景的 scrapy pipeline 扩展 - pika mq
     """
 
+    def __init__(self):
+        self.channel = None
+
     def _dict_to_bytes(self, item: dict) -> bytes:
         item_json_str = json.dumps(item)
         return bytes(item_json_str, encoding="utf-8")
 
     def open_spider(self, spider):
         assert hasattr(
             spider, "rabbitmq_conf"
```

### Comparing `ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/mysql/__init__.py` & `ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/mysql/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         Returns:
             1). 整合后的 item
         """
         new_item = {}
         notes_dic = {}
 
         insert_data = ReuseOperation.get_items_except_keys(
-            dict_conf=item_dict, key_list=["_item_mode", "_table"]
+            dict_conf=item_dict, keys=["_item_mode", "_mongo_update_rule", "_table"]
         )
         judge_item = next(iter(insert_data.values()))
         # 是 namedtuple 类型
         if ReuseOperation.is_namedtuple_instance(judge_item):
             for key, value in insert_data.items():
                 new_item[key] = value.key_value
                 notes_dic[key] = value.notes
@@ -98,20 +98,18 @@
                 new_item[key] = value
                 notes_dic[key] = ""
 
         return AlterItem(new_item=new_item, notes_dic=notes_dic)
 
     def process_item(self, item, spider):
         item_dict = ReuseOperation.item_to_dict(item)
-        # 先查看存储场景是否匹配
-        if item_dict["_item_mode"] == "Mysql":
-            self.insert_item(
-                alter_item=self.get_new_item(item_dict),
-                table=item_dict["_table"],
-            )
+        self.insert_item(
+            alter_item=self.get_new_item(item_dict),
+            table=item_dict["_table"],
+        )
         return item
 
     def insert_item(self, alter_item: AlterItem, table: str):
         """
         通用插入数据，将 item 数据存入 Mysql 中，item 中的 key 需要跟 Mysql 数据中的字段名称一致
         Args:
             alter_item: 经过转变后的 item
```

### Comparing `ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/mysql/asynced.py` & `ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/mysql/asynced.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,26 +37,23 @@
             db=self.mysql_conf.database,
             charset=self.mysql_conf.charset,
             cursorclass=aiomysql.DictCursor,
         )
 
     async def process_item(self, item, spider):
         item_dict = ReuseOperation.item_to_dict(item)
-        if item_dict["_item_mode"] == "Mysql":
-            async with self.db.cursor() as cursor:
-                async with self.lock:
-                    alter_item = super(AsyncNormalMysqlPipeline, self).get_new_item(
-                        item_dict
-                    )
-                    new_item = alter_item.new_item
-                    sql = self._get_sql_by_item(
-                        table=item_dict["_table"], item=new_item
-                    )
-                    await cursor.execute(sql, tuple(new_item.values()) * 2)
-                    await self.db.commit()
+        async with self.db.cursor() as cursor:
+            async with self.lock:
+                alter_item = super(AsyncNormalMysqlPipeline, self).get_new_item(
+                    item_dict
+                )
+                new_item = alter_item.new_item
+                sql = self._get_sql_by_item(table=item_dict["_table"], item=new_item)
+                await cursor.execute(sql, tuple(new_item.values()) * 2)
+                await self.db.commit()
         return item
 
     async def _close_spider(self):
         pass
 
     def close_spider(self, spider):
         self.db.close()
@@ -90,26 +87,23 @@
             maxsize=10,
             # 连接池最小连接数
             minsize=1,
         )
 
     async def process_item(self, item, spider):
         item_dict = ReuseOperation.item_to_dict(item)
-        if item_dict["_item_mode"] == "Mysql":
-            async with self.pool.acquire() as conn:
-                async with conn.cursor() as cursor:
-                    alter_item = super(AsyncMysqlPipeline, self).get_new_item(item_dict)
-                    new_item = alter_item.new_item
-                    sql = self._get_sql_by_item(
-                        table=item_dict["_table"],
-                        item=new_item,
-                    )
-                    await asyncio.shield(
-                        cursor.execute(sql, tuple(new_item.values()) * 2)
-                    )
+        async with self.pool.acquire() as conn:
+            async with conn.cursor() as cursor:
+                alter_item = super(AsyncMysqlPipeline, self).get_new_item(item_dict)
+                new_item = alter_item.new_item
+                sql = self._get_sql_by_item(
+                    table=item_dict["_table"],
+                    item=new_item,
+                )
+                await asyncio.shield(cursor.execute(sql, tuple(new_item.values()) * 2))
         return item
 
     async def _close_spider(self):
         self.pool.close()
         await self.pool.wait_closed()
 
     def close_spider(self, spider):
```

### Comparing `ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/mysql/stats.py` & `ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/mysql/stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 class AyuStatisticsMysqlPipeline(AyuMysqlPipeline):
     """
     Mysql 存储且记录脚本运行状态的简单示例
     """
 
-    # TODO: 此方法暂用于测试
+    # Note: 此方法暂用于测试
     def __init__(self, env):
         self.env = env
         self.slog = None
         self.conn = None
         self.cursor = None
         self.collate = None
         self.mysql_conf = None
```

### Comparing `ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/mysql/turbo.py` & `ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/mysql/turbo.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.2.0/ayugespidertools/scraper/pipelines/mysql/twisted.py` & `ayugespidertools-3.3.0/ayugespidertools/scraper/pipelines/mysql/twisted.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,18 +52,16 @@
         pass
 
     def db_create_err(self, failure):
         self.slog.error(f"创建数据表失败: {failure}")
 
     def process_item(self, item, spider):
         item_dict = ReuseOperation.item_to_dict(item)
-        # 先查看存储场景是否匹配
-        if item_dict["_item_mode"] == "Mysql":
-            query = self.dbpool.runInteraction(self.db_insert, item_dict)
-            query.addErrback(self.handle_error, item)
+        query = self.dbpool.runInteraction(self.db_insert, item_dict)
+        query.addErrback(self.handle_error, item)
         return item
 
     def db_insert(self, cursor, item):
         alter_item = super(AyuTwistedMysqlPipeline, self).get_new_item(item)
         table = item["_table"]
 
         if not (new_item := alter_item.new_item):
@@ -93,9 +91,8 @@
 
         return item
 
     def handle_error(self, failure, item):
         self.slog.error(f"插入数据失败:{failure}, item: {item}")
 
     def close_spider(self, spider):
-        # 这里新建数据库链接，是为了正常继承父类的脚本运行统计的方法（需要 self 的 mysql 连接对象存在）
         super(AyuTwistedMysqlPipeline, self).close_spider(spider)
```

### Comparing `ayugespidertools-3.2.0/ayugespidertools/scraper/spiders/__init__.py` & `ayugespidertools-3.3.0/ayugespidertools/scraper/spiders/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,50 +167,50 @@
         spider.slog.debug(f"settings_type 配置: {cls.settings_type}")
 
         _consul_conf = ReuseOperation.get_consul_conf(settings=crawler.settings)
         # 以下将 .conf 中或 consul 中对应的配置信息，赋值给 spider 对象，方便后续使用
         if mysql_conf := get_spider_conf(
             MysqlConfCreator().create_product(crawler.settings, _consul_conf)
         ):
-            spider.slog.info("项目中配置了 mysql_conf 信息")
+            spider.slog.debug("项目中配置了 mysql_conf 信息")
             spider.mysql_conf = mysql_conf
             if cls.mysql_engine_enabled:
                 mysql_url = (
                     f"mysql+pymysql://{mysql_conf.user}"
                     f":{mysql_conf.password}@{mysql_conf.host}"
                     f":{mysql_conf.port}/{mysql_conf.database}"
                     f"?charset={mysql_conf.charset}"
                 )
                 spider.mysql_engine = MySqlEngineClass(engine_url=mysql_url).engine
 
         if mongodb_conf := get_spider_conf(
             MongoDBConfCreator().create_product(crawler.settings, _consul_conf)
         ):
-            spider.slog.info("项目中配置了 mongodb_conf 信息")
+            spider.slog.debug("项目中配置了 mongodb_conf 信息")
             spider.mongodb_conf = mongodb_conf
 
         if rabbitmq_conf := get_spider_conf(
             MQConfCreator().create_product(crawler.settings, _consul_conf)
         ):
-            spider.slog.info("项目中配置了 rabbitmq_conf 信息")
+            spider.slog.debug("项目中配置了 rabbitmq_conf 信息")
             spider.rabbitmq_conf = rabbitmq_conf
 
         if kafka_conf := get_spider_conf(
             KafkaConfCreator().create_product(crawler.settings, _consul_conf)
         ):
-            spider.slog.info("项目中配置了 kafka_conf 信息")
+            spider.slog.debug("项目中配置了 kafka_conf 信息")
             spider.kafka_conf = kafka_conf
 
         # 动态代理
         if dynamicproxy_conf := get_spider_conf(
             DynamicProxyCreator().create_product(crawler.settings, _consul_conf)
         ):
-            spider.slog.info("项目中配置了 dynamicproxy_conf 信息")
+            spider.slog.debug("项目中配置了 dynamicproxy_conf 信息")
             spider.dynamicproxy_conf = dynamicproxy_conf
 
         # 独享代理
         if exclusiveproxy_conf := get_spider_conf(
             ExclusiveProxyCreator().create_product(crawler.settings, _consul_conf)
         ):
-            spider.slog.info("项目中配置了 exclusiveproxy_conf 信息")
+            spider.slog.debug("项目中配置了 exclusiveproxy_conf 信息")
             spider.exclusiveproxy_conf = exclusiveproxy_conf
         return spider
```

### Comparing `ayugespidertools-3.2.0/ayugespidertools/templates/project/module/VIT/.conf` & `ayugespidertools-3.3.0/ayugespidertools/templates/project/module/VIT/.conf`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.2.0/ayugespidertools/templates/project/module/items.py.tmpl` & `ayugespidertools-3.3.0/ayugespidertools/templates/project/module/items.py.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.2.0/ayugespidertools/templates/project/module/middlewares.py.tmpl` & `ayugespidertools-3.3.0/ayugespidertools/templates/project/module/middlewares.py.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.2.0/ayugespidertools/templates/project/module/settings.py.tmpl` & `ayugespidertools-3.3.0/ayugespidertools/templates/project/module/settings.py.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.2.0/ayugespidertools/templates/spiders/async.tmpl` & `ayugespidertools-3.3.0/ayugespidertools/templates/spiders/async.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.2.0/ayugespidertools/templates/spiders/basic.tmpl` & `ayugespidertools-3.3.0/ayugespidertools/templates/spiders/basic.tmpl`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pandas
 from scrapy.http import Request
 from $project_name.settings import logger
 from scrapy.http.response.text import TextResponse
 from $project_name.items import TableEnum
 from ayugespidertools.spiders import AyuSpider
 from ayugespidertools.common.utils import ToolsForAyu
-from ayugespidertools.items import DataItem, MysqlDataItem, MongoDataItem
+from ayugespidertools.items import AyuItem, DataItem
 
 """
 ####################################################################################################
 # collection_website: $domain - 采集的目标站点介绍
 # collection_content: 采集内容介绍
 # create_time: xxxx-xx-xx
 # explain:
@@ -18,39 +18,24 @@
 """
 
 
 class $classname(AyuSpider):
     name = "$name"
     allowed_domains = ["$domain"]
     start_urls = ["http://$domain/"]
-
-    # 数据库表的枚举信息
     custom_table_enum = TableEnum
-    # 初始化配置的类型
-    settings_type = "debug"
     custom_settings = {
-        # scrapy 日志等级配置
-        "LOG_LEVEL": "DEBUG",
-        # 是否开启记录项目相关运行统计信息。不配置默认为 False
-        "RECORD_LOG_TO_MYSQL": False,
-        # 以 loguru 来管理日志，本库会在 settings 中生成规则示例，可自行修改。也可不配置
-        "LOGURU_CONFIG": logger,
         "ITEM_PIPELINES": {
-            # 激活此项则数据会存储至 Mysql
             "ayugespidertools.pipelines.AyuFtyMysqlPipeline": 300,
-            # 激活此项则数据会存储至 MongoDB
             "ayugespidertools.pipelines.AyuFtyMongoPipeline": 301,
         },
         "DOWNLOADER_MIDDLEWARES": {
-            # 随机请求头
             "ayugespidertools.middlewares.RandomRequestUaMiddleware": 400,
         },
     }
-
-    # 打开 mysql 引擎开关，用于数据入库前更新逻辑判断
     mysql_engine_enabled = True
 
     def start_requests(self):
         """
         get 请求首页，获取项目列表数据
         """
         yield Request(
@@ -62,18 +47,17 @@
             cb_kwargs={
                 "curr_site": "csdn",
             },
             dont_filter=True
         )
 
     def parse_first(self, response: TextResponse, curr_site: str):
-        # 日志使用: scrapy 的 self.logger 或本库的 self.slog 或直接使用全局的 logger handle 也行（根据场景自行选择）
         self.slog.info(f"当前采集的站点为: {curr_site}")
 
-        # 你可以自定义解析规则，使用 lxml 还是 response.css response.xpath 等等都可以。
+        # 你可以自定义解析规则，使用 lxml 还是 response.css response.xpath 等都可以。
         data_list = ToolsForAyu.extract_with_json(json_data=response.json(), query="data")
         for curr_data in data_list:
             article_detail_url = ToolsForAyu.extract_with_json(
                 json_data=curr_data,
                 query="articleDetailUrl")
 
             article_title = ToolsForAyu.extract_with_json(
@@ -88,49 +72,43 @@
                 json_data=curr_data,
                 query="favorCount")
 
             nick_name = ToolsForAyu.extract_with_json(
                 json_data=curr_data,
                 query="nickName")
 
-            ArticleInfoMysqlItem = MysqlDataItem(
+            ArticleInfoItem = AyuItem(
                 article_detail_url=DataItem(article_detail_url, "文章详情链接"),
                 article_title=DataItem(article_title, "文章标题"),
                 comment_count=DataItem(comment_count, "文章评论数量"),
                 favor_count=DataItem(favor_count, "文章赞成数量"),
                 nick_name=DataItem(nick_name, "文章作者昵称"),
                 _table=TableEnum.article_list_table.value["value"],
+                # 可选参数：这里表示 MongoDB 存储场景以 article_detail_url 为去重规则，若存在则更新，不存在则新增
+                _mongo_update_rule={"article_detail_url": article_detail_url},
             )
-            self.slog.info(f"ArticleInfoMysqlItem: {ArticleInfoMysqlItem}")
+            self.slog.info(f"ArticleInfoItem: {ArticleInfoItem}")
 
-            # 数据入库逻辑，你可以使用 mysql_engine 来去重或自定义规则
+            # 注意：同时存储至 mysql 和 mongodb 时，不建议使用以下去重方法，会互相影响。
+            # 此时更适合：
+            #    1.mysql 添加唯一索引去重（本库会根据 on duplicate key update 更新），
+            #      mongoDB 场景下设置 _mongo_update_rule 参数即可；
+            #    2.或者添加爬取时间字段并每次新增的场景，即不去重，请根据使用场景自行选择。
+            # 这里只是为了介绍使用 mysql_engine 来对 mysql 去重的方法。
             try:
                 save_table = TableEnum.article_list_table.value["value"]
                 sql = f'''select `id` from `{save_table}` where `article_detail_url` = "{article_detail_url}" limit 1'''
                 df = pandas.read_sql(sql, self.mysql_engine)
 
                 # 如果为空，说明此数据不存在于数据库，则新增
                 if df.empty:
-                    yield ArticleInfoMysqlItem
+                    yield ArticleInfoItem
 
                 # 如果已存在，1). 若需要更新，请自定义更新数据结构和更新逻辑；2). 若不用更新，则跳过即可。
                 else:
                     self.slog.debug(f"标题为 ”{article_title}“ 的数据已存在")
 
             except Exception as e:
                 if any(["1146" in str(e), "1054" in str(e), "doesn't exist" in str(e)]):
-                    yield ArticleInfoMysqlItem
+                    yield ArticleInfoItem
                 else:
                     self.slog.error(f"请查看数据库链接或网络是否通畅！Error: {e}")
-
-            # 这是 MongoDB 存储场景的示例
-            ArticleInfoMongoItem = MongoDataItem(
-                article_detail_url=article_detail_url,
-                article_title=article_title,
-                comment_count=comment_count,
-                favor_count=favor_count,
-                nick_name=nick_name,
-                _table=TableEnum.article_list_table.value["value"],
-                # 这里表示以 article_detail_url 为去重规则，若存在则更新，不存在则新增
-                _mongo_update_rule={"article_detail_url": article_detail_url},
-            )
-            yield ArticleInfoMongoItem
```

### Comparing `ayugespidertools-3.2.0/ayugespidertools/templates/spiders/crawl.tmpl` & `ayugespidertools-3.3.0/ayugespidertools/templates/spiders/crawl.tmpl`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import scrapy
 from scrapy.spiders import Rule
 from $project_name.settings import logger
 from scrapy.linkextractors import LinkExtractor
-from ayugespidertools.items import MysqlDataItem
+from ayugespidertools.items import AyuItem
 from $project_name.common.DataEnum import TableEnum
 from ayugespidertools.spiders import AyuCrawlSpider
 
 
 class $classname(AyuCrawlSpider):
     name = "$name"
     allowed_domains = ["$domain"]
@@ -36,12 +36,12 @@
 
     def parse_item(self, response):
         # 获取图书名称 - （获取的是详情页中的图书名称）
         book_name_list = response.xpath('//div[@class="book-name"]//text()').extract()
         book_name = "".join(book_name_list).strip()
         self.slog.debug(f"book_name: {book_name}")
 
-        NovelInfoItem = MysqlDataItem(
+        NovelInfoItem = AyuItem(
             book_name=book_name,
             _table=TableEnum.article_list_table.value["value"],
         )
         yield NovelInfoItem
```

### Comparing `ayugespidertools-3.2.0/ayugespidertools/templates/spiders/csvfeed.tmpl` & `ayugespidertools-3.3.0/ayugespidertools/templates/spiders/csvfeed.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.2.0/ayugespidertools/templates/spiders/xmlfeed.tmpl` & `ayugespidertools-3.3.0/ayugespidertools/templates/spiders/xmlfeed.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.2.0/ayugespidertools/utils/cmdline.py` & `ayugespidertools-3.3.0/ayugespidertools/utils/cmdline.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.2.0/ayugespidertools/verificationcode.py` & `ayugespidertools-3.3.0/ayugespidertools/verificationcode.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.2.0/pyproject.toml` & `ayugespidertools-3.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AyugeSpiderTools"
-version = "3.2.0"
+version = "3.3.0"
 description = "scrapy 扩展库：用于扩展 Scrapy 功能来解放双手，还内置一些爬虫开发中的通用方法。"
 authors = ["ayuge <ayugesheng@gmail.com>"]
 maintainers = ["ayuge <ayugesheng@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ayugespidertools"}]
 repository = "https://github.com/shengchenyang/AyugeSpiderTools"
 documentation = "https://ayugespidertools.readthedocs.io/en/latest/"
@@ -12,16 +12,16 @@
 homepage = "https://www.ayuge.top/mkdocs-material/"
 include = ["pyproject.toml"]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 opencv-python = "^4.6.0.66"
 PyMySQL = "^1.0.2"
-loguru = "^0.6.0"
-numpy = "1.24.2"
+loguru = "~0.7.0"
+numpy = "~1.24.3"
 requests = "^2.28.1"
 Pillow = "^9.2.0"
 Scrapy = "2.9.0"
 pandas = "^1.5.0"
 WorkWeixinRobot = "^1.0.1"
 retrying = "^1.3.3"
 SQLAlchemy = "^1.4.41"
```

### Comparing `ayugespidertools-3.2.0/PKG-INFO` & `ayugespidertools-3.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ayugespidertools
-Version: 3.2.0
+Version: 3.3.0
 Summary: scrapy 扩展库：用于扩展 Scrapy 功能来解放双手，还内置一些爬虫开发中的通用方法。
 Home-page: https://www.ayuge.top/mkdocs-material/
 Keywords: crawler,scraping,twisted,aiohttp,asyncio,scrapy,aiomysql,mmh3
 Author: ayuge
 Author-email: ayugesheng@gmail.com
 Maintainer: ayuge
 Maintainer-email: ayugesheng@gmail.com
@@ -21,18 +21,18 @@
 Requires-Dist: WorkWeixinRobot (>=1.0.1,<2.0.0)
 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
 Requires-Dist: aiomysql (>=0.1.1,<0.2.0)
 Requires-Dist: attrs (>=22.2.0,<23.0.0)
 Requires-Dist: html2text (>=2020.1.16,<2021.0.0)
 Requires-Dist: itemadapter (>=0.7.0,<0.8.0)
 Requires-Dist: kafka-python (==2.0.2)
-Requires-Dist: loguru (>=0.6.0,<0.7.0)
+Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: mmh3 (>=3.0.0,<4.0.0)
 Requires-Dist: motor (==2.5.1)
-Requires-Dist: numpy (==1.24.2)
+Requires-Dist: numpy (>=1.24.3,<1.25.0)
 Requires-Dist: opencv-python (>=4.6.0.66,<5.0.0.0)
 Requires-Dist: oss2 (>=2.16.0,<3.0.0)
 Requires-Dist: pandas (>=1.5.0,<2.0.0)
 Requires-Dist: pika (>=1.3.2,<1.4.0)
 Requires-Dist: pycryptodome (>=3.15.0,<4.0.0)
 Requires-Dist: pymongo (>=3.12.3,<4.0.0)
 Requires-Dist: python-hcl2 (>=4.3.0,<5.0.0)
@@ -56,15 +56,15 @@
 
 # AyugeSpiderTools 工具说明
 
 > 一句话介绍：用于扩展 `Scrapy` 功能来解放双手，还内置一些爬虫开发中的通用方法。
 
 ## 前言
 
-在使用 `Python` `Scrapy` 库开发爬虫时，免不了会重复的修改和编写 `settings.py`，`middlewares.py`，`pipelines.py`，`item.py` 和一些通用方法或脚本，但其实各个项目中的这些文件内容大致相同，那为何不把他们统一整理在一起呢。虽说可以使用 `scrapy` 的模板功能，但还是无法适配所有的开发场景。
+在使用 `Python` `Scrapy` 库开发爬虫时，免不了会重复的修改和编写 `settings.py`，`item.py`，`middlewares.py`，`pipelines.py` 和一些通用方法或脚本，但其实各个项目中的这些文件内容大致相同，那为何不把他们统一整理在一起呢。虽说可以使用 `scrapy` 的模板功能，但还是无法适配所有的开发场景。
 
 刚开始我也只是想把它用来适配 `Mysql` 存储的场景，可以自动创建相关数据库，数据表，字段注释，自动添加新添加的字段，和自动修复常见（字段编码，`Data too long`，存储字段不存在等等）的存储问题。后来不断优化和添加各种场景，使得爬虫开发在通用场景下几乎只用在意 `spider` 脚本的解析规则和 `VIT` 下的 `.conf` 配置即可，脱离无意义的重复操作。
 
 至于此库做了哪些功能，只要你熟悉 `python` 语法和 `scrapy` 库，再结合 [DemoSpider](https://github.com/shengchenyang/DemoSpider) 中的应用示例，你可以很快上手。具体的内容和注意事项也可以在 [AyugeSpiderTools readthedocs 文档](https://ayugespidertools.readthedocs.io/en/latest/) 中查看。
 
 ## 1. 前提条件
 
@@ -93,16 +93,14 @@
 使用方法示例 `GIF` 如下：
 
 ![ayugespidertools.gif](https://raw.githubusercontent.com/shengchenyang/AyugeSpiderTools/main/examples/ayugespidertools-use.gif)
 
 对以上 `GIF` 中的步骤进行解释：
 
 ```shell
-# 注：ayugespidertools 的 cli 已剔除，现只能使用 ayuge。
-
 # 查看库版本
 ayuge version
 
 # 创建项目
 ayuge startproject <project_name>
 
 # 进入项目根目录
@@ -151,15 +149,16 @@
 
 # 本库中给出支持 Item Loaders 特性的示例(文档地址：https://ayugespidertools.readthedocs.io/en/latest/topics/loaders.html)
 +15).demo_item_loader: 本库中使用 Item Loaders 的示例
 -16).demo_item_loader_two: 展示本库使用 itemLoader 特性的示例，此示例已删除，可查看上个 demo_item_loader 中的示例，目前已经可以很方便的使用 Item Loaders 功能了
 
 +17).demo_mongo_async: asyncio 版本存储 mongoDB 的 pipelines 示例
 +18).demo_mq: 数据存入 rabbitmq 的模板示例
-+19).demo_kafka: 数据存入 rabbitmq 的模板示例
++19).demo_kafka: 数据存入 kafka 的模板示例
++20).demo_file: 下载图片等文件到本地的模板示例
 ```
 
 注：具体内容及时效性请以 [DemoSpider](https://github.com/shengchenyang/DemoSpider) 项目中描述为准。
 
 ### 2.2. 开发场景
 
 > 这里不再一一列举所有功能，大概介绍下包含的大致功能。
```

