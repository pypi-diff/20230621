# Comparing `tmp/snort_web_master-1.0.0.0.tar.gz` & `tmp/snort_web_master-1.0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\snort_web_master-1.0.0.0.tar", last modified: Wed Jun 21 14:29:26 2023, max compression
+gzip compressed data, was "dist\snort_web_master-1.0.0.1.tar", last modified: Wed Jun 21 16:07:24 2023, max compression
```

## Comparing `snort_web_master-1.0.0.0.tar` & `snort_web_master-1.0.0.1.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 14:29:26.363937 snort_web_master-1.0.0.0/
--rw-rw-rw-   0        0        0       54 2022-11-21 06:29:02.000000 snort_web_master-1.0.0.0/LICENSE.rst
--rw-rw-rw-   0        0        0       24 2022-11-24 17:54:23.000000 snort_web_master-1.0.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0      251 2023-06-21 14:29:26.363937 snort_web_master-1.0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      716 2022-11-21 06:20:44.000000 snort_web_master-1.0.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-21 14:29:26.270184 snort_web_master-1.0.0.0/data/
-drwxrwxrwx   0        0        0        0 2023-06-21 14:29:26.270184 snort_web_master-1.0.0.0/data/admin/
--rw-rw-rw-   0        0        0      698 2023-04-19 07:30:34.000000 snort_web_master-1.0.0.0/data/admin/0004_keyword_delete_keywords.py
-drwxrwxrwx   0        0        0        0 2023-06-21 14:29:26.270184 snort_web_master-1.0.0.0/data/admin/image/
--rw-rw-rw-   0        0        0     7972 2023-01-16 16:49:34.000000 snort_web_master-1.0.0.0/data/admin/image/images.png
--rw-rw-rw-   0        0        0   356352 2023-06-21 14:26:22.000000 snort_web_master-1.0.0.0/data/db.sqlite3
--rw-rw-rw-   0        0        0    39363 2022-10-13 12:31:39.000000 snort_web_master-1.0.0.0/data/dicts.py
--rw-rw-rw-   0        0        0      690 2023-01-23 09:10:03.000000 snort_web_master-1.0.0.0/data/dockercompose
--rw-rw-rw-   0        0        0   139272 2023-01-16 16:50:11.000000 snort_web_master-1.0.0.0/data/favicon.ico
--rw-rw-rw-   0        0        0    25803 2023-05-02 11:59:42.000000 snort_web_master-1.0.0.0/data/http.cap
--rw-rw-rw-   0        0        0      898 2023-01-23 08:40:15.000000 snort_web_master-1.0.0.0/data/migrate sqllite to postgresql
--rw-rw-rw-   0        0        0      402 2022-11-14 09:05:52.000000 snort_web_master-1.0.0.0/data/my-snort-rule.tmp
-drwxrwxrwx   0        0        0        0 2023-06-21 14:29:26.270184 snort_web_master-1.0.0.0/data/nginx/
--rw-rw-rw-   0        0        0       96 2023-01-23 09:09:18.000000 snort_web_master-1.0.0.0/data/nginx/nginx
--rw-rw-rw-   0        0        0      296 2023-01-23 09:04:00.000000 snort_web_master-1.0.0.0/data/nginx/nginx.conf
--rw-rw-rw-   0        0        0      162 2023-01-23 08:44:15.000000 snort_web_master-1.0.0.0/data/requirements.txt
--rw-rw-rw-   0        0        0      889 2023-05-02 14:51:31.000000 snort_web_master-1.0.0.0/data/snortFile
-drwxrwxrwx   0        0        0        0 2023-06-21 14:29:26.270184 snort_web_master-1.0.0.0/data/static/
-drwxrwxrwx   0        0        0        0 2023-06-21 14:29:26.223337 snort_web_master-1.0.0.0/data/static/admin/
-drwxrwxrwx   0        0        0        0 2023-06-21 14:29:26.270184 snort_web_master-1.0.0.0/data/static/admin/css/
--rw-rw-rw-   0        0        0     1172 2023-06-21 13:46:42.000000 snort_web_master-1.0.0.0/data/static/admin/css/admin-styles.css
--rw-rw-rw-   0        0        0    20344 2023-06-10 07:58:01.000000 snort_web_master-1.0.0.0/data/static/admin/css/base.css
--rw-rw-rw-   0        0        0     9730 2023-06-10 07:59:05.000000 snort_web_master-1.0.0.0/data/static/admin/css/forms.css
--rw-rw-rw-   0        0        0     2619 2023-06-10 07:58:10.000000 snort_web_master-1.0.0.0/data/static/admin/css/nav_sidebar.css
-drwxrwxrwx   0        0        0        0 2023-06-21 14:29:26.223337 snort_web_master-1.0.0.0/data/static/admin/css/vendor/
-drwxrwxrwx   0        0        0        0 2023-06-21 14:29:26.285809 snort_web_master-1.0.0.0/data/static/admin/css/vendor/select2/
--rw-rw-rw-   0        0        0     1124 2022-12-26 08:06:54.000000 snort_web_master-1.0.0.0/data/static/admin/css/vendor/select2/LICENSE-SELECT2.md
--rw-rw-rw-   0        0        0    17358 2022-12-26 08:06:54.000000 snort_web_master-1.0.0.0/data/static/admin/css/vendor/select2/select2.css
--rw-rw-rw-   0        0        0    14966 2022-12-26 08:06:54.000000 snort_web_master-1.0.0.0/data/static/admin/css/vendor/select2/select2.min.css
-drwxrwxrwx   0        0        0        0 2023-06-21 14:29:26.285809 snort_web_master-1.0.0.0/data/static/admin/image/
--rw-rw-rw-   0        0        0     7972 2023-01-16 16:49:34.000000 snort_web_master-1.0.0.0/data/static/admin/image/images.png
-drwxrwxrwx   0        0        0        0 2023-06-21 14:29:26.285809 snort_web_master-1.0.0.0/data/static/css/
--rw-rw-rw-   0        0        0     1890 2023-06-14 17:15:26.000000 snort_web_master-1.0.0.0/data/static/css/main.55b651d4.css
--rw-rw-rw-   0        0        0     3089 2023-06-14 17:15:26.000000 snort_web_master-1.0.0.0/data/static/css/main.55b651d4.css.map
--rw-rw-rw-   0        0        0   139272 2023-01-16 16:50:11.000000 snort_web_master-1.0.0.0/data/static/favico.ico
-drwxrwxrwx   0        0        0        0 2023-06-21 14:29:26.285809 snort_web_master-1.0.0.0/data/static/js/
--rw-rw-rw-   0        0        0     4591 2023-06-14 11:57:57.000000 snort_web_master-1.0.0.0/data/static/js/787.2c2ec360.chunk.js
--rw-rw-rw-   0        0        0    10592 2023-06-14 11:57:57.000000 snort_web_master-1.0.0.0/data/static/js/787.2c2ec360.chunk.js.map
--rw-rw-rw-   0        0        0   656292 2023-06-21 12:35:36.000000 snort_web_master-1.0.0.0/data/static/js/main.ad6031d4.js
--rw-rw-rw-   0        0        0     1458 2023-06-21 12:35:36.000000 snort_web_master-1.0.0.0/data/static/js/main.ad6031d4.js.LICENSE.txt
--rw-rw-rw-   0        0        0  2485433 2023-06-21 12:35:36.000000 snort_web_master-1.0.0.0/data/static/js/main.ad6031d4.js.map
-drwxrwxrwx   0        0        0        0 2023-06-21 14:29:26.238937 snort_web_master-1.0.0.0/data/templates/
-drwxrwxrwx   0        0        0        0 2023-06-21 14:29:26.301434 snort_web_master-1.0.0.0/data/templates/html/
--rw-rw-rw-   0        0        0      150 2023-06-21 12:36:15.000000 snort_web_master-1.0.0.0/data/templates/html/full_rule.html
--rw-rw-rw-   0        0        0      420 2023-01-23 09:19:00.000000 snort_web_master-1.0.0.0/data/templates/html/import.html
--rw-rw-rw-   0        0        0     3565 2023-06-14 12:05:15.000000 snort_web_master-1.0.0.0/data/templates/html/snortBuilder.html
--rw-rw-rw-   0        0        0      140 2023-06-21 14:29:26.363937 snort_web_master-1.0.0.0/setup.cfg
--rw-rw-rw-   0        0        0      862 2023-06-21 14:29:21.000000 snort_web_master-1.0.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-21 14:29:26.238937 snort_web_master-1.0.0.0/snort_web_master/
-drwxrwxrwx   0        0        0        0 2023-06-21 14:29:26.301434 snort_web_master-1.0.0.0/snort_web_master/pcaps/
--rw-rw-rw-   0        0        0        0 2022-10-31 09:04:45.000000 snort_web_master-1.0.0.0/snort_web_master/pcaps/__init__.py
--rw-rw-rw-   0        0        0     2689 2023-01-08 17:50:03.000000 snort_web_master-1.0.0.0/snort_web_master/pcaps/admin.py
--rw-rw-rw-   0        0        0      148 2022-10-31 09:04:45.000000 snort_web_master-1.0.0.0/snort_web_master/pcaps/apps.py
-drwxrwxrwx   0        0        0        0 2023-06-21 14:29:26.317061 snort_web_master-1.0.0.0/snort_web_master/pcaps/migrations/
--rw-rw-rw-   0        0        0     1385 2022-12-19 18:20:00.000000 snort_web_master-1.0.0.0/snort_web_master/pcaps/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      813 2022-12-19 18:20:00.000000 snort_web_master-1.0.0.0/snort_web_master/pcaps/migrations/0002_initial.py
--rw-rw-rw-   0        0        0      555 2022-12-19 18:24:58.000000 snort_web_master-1.0.0.0/snort_web_master/pcaps/migrations/0003_rename_rule_to_validate_pcap_rule_to_validate2_and_more.py
--rw-rw-rw-   0        0        0      603 2022-12-19 18:25:24.000000 snort_web_master-1.0.0.0/snort_web_master/pcaps/migrations/0004_rename_rule_to_validate2_pcap_rule_to_validate_and_more.py
--rw-rw-rw-   0        0        0        0 2022-12-19 18:19:43.000000 snort_web_master-1.0.0.0/snort_web_master/pcaps/migrations/__init__.py
--rw-rw-rw-   0        0        0     1060 2022-12-19 18:25:20.000000 snort_web_master-1.0.0.0/snort_web_master/pcaps/models.py
--rw-rw-rw-   0        0        0       63 2022-10-31 09:04:45.000000 snort_web_master-1.0.0.0/snort_web_master/pcaps/tests.py
--rw-rw-rw-   0        0        0       66 2022-10-31 09:04:45.000000 snort_web_master-1.0.0.0/snort_web_master/pcaps/views.py
-drwxrwxrwx   0        0        0        0 2023-06-21 14:29:26.317061 snort_web_master-1.0.0.0/snort_web_master/settings/
--rw-rw-rw-   0        0        0        0 2022-12-19 07:00:41.000000 snort_web_master-1.0.0.0/snort_web_master/settings/__init__.py
--rw-rw-rw-   0        0        0      546 2023-04-19 09:25:30.000000 snort_web_master-1.0.0.0/snort_web_master/settings/admin.py
--rw-rw-rw-   0        0        0      154 2022-12-19 07:00:41.000000 snort_web_master-1.0.0.0/snort_web_master/settings/apps.py
-drwxrwxrwx   0        0        0        0 2023-06-21 14:29:26.317061 snort_web_master-1.0.0.0/snort_web_master/settings/migrations/
--rw-rw-rw-   0        0        0     1595 2022-12-19 18:20:00.000000 snort_web_master-1.0.0.0/snort_web_master/settings/migrations/0001_initial.py
--rw-rw-rw-   0        0        0     1350 2022-12-26 06:21:16.000000 snort_web_master-1.0.0.0/snort_web_master/settings/migrations/0002_remove_keywords_type_keywords_description_and_more.py
--rw-rw-rw-   0        0        0      530 2022-12-26 06:23:11.000000 snort_web_master-1.0.0.0/snort_web_master/settings/migrations/0003_keywords_avalable.py
--rw-rw-rw-   0        0        0      698 2023-04-19 07:30:34.000000 snort_web_master-1.0.0.0/snort_web_master/settings/migrations/0004_keyword_delete_keywords.py
--rw-rw-rw-   0        0        0     1268 2023-04-19 09:28:30.000000 snort_web_master-1.0.0.0/snort_web_master/settings/migrations/0005_remove_keyword_negation_alter_keyword_description_and_more.py
--rw-rw-rw-   0        0        0        0 2022-12-19 18:19:43.000000 snort_web_master-1.0.0.0/snort_web_master/settings/migrations/__init__.py
--rw-rw-rw-   0        0        0     1476 2023-06-01 19:36:46.000000 snort_web_master-1.0.0.0/snort_web_master/settings/models.py
--rw-rw-rw-   0        0        0       63 2022-12-19 07:00:41.000000 snort_web_master-1.0.0.0/snort_web_master/settings/tests.py
--rw-rw-rw-   0        0        0       66 2022-12-19 07:00:41.000000 snort_web_master-1.0.0.0/snort_web_master/settings/views.py
-drwxrwxrwx   0        0        0        0 2023-06-21 14:29:26.332686 snort_web_master-1.0.0.0/snort_web_master/snort/
--rw-rw-rw-   0        0        0        0 2022-10-31 09:04:41.000000 snort_web_master-1.0.0.0/snort_web_master/snort/__init__.py
--rw-rw-rw-   0        0        0    32396 2023-06-21 12:54:36.000000 snort_web_master-1.0.0.0/snort_web_master/snort/admin.py
--rw-rw-rw-   0        0        0      148 2022-10-31 09:04:41.000000 snort_web_master-1.0.0.0/snort_web_master/snort/apps.py
-drwxrwxrwx   0        0        0        0 2023-06-21 14:29:26.348312 snort_web_master-1.0.0.0/snort_web_master/snort/migrations/
--rw-rw-rw-   0        0        0     1974 2022-12-19 18:20:00.000000 snort_web_master-1.0.0.0/snort_web_master/snort/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      870 2023-01-05 14:35:56.000000 snort_web_master-1.0.0.0/snort_web_master/snort/migrations/0002_snortruleviewarray.py
--rw-rw-rw-   0        0        0      610 2023-01-06 06:03:56.000000 snort_web_master-1.0.0.0/snort_web_master/snort/migrations/0003_snortruleviewarray_htmlid_and_more.py
--rw-rw-rw-   0        0        0      423 2023-01-06 13:23:29.000000 snort_web_master-1.0.0.0/snort_web_master/snort/migrations/0004_snortrule_deleted.py
--rw-rw-rw-   0        0        0      522 2023-01-08 17:24:52.000000 snort_web_master-1.0.0.0/snort_web_master/snort/migrations/0005_remove_snortrule_template_snortrule_is_template.py
--rw-rw-rw-   0        0        0      759 2023-02-21 08:33:21.000000 snort_web_master-1.0.0.0/snort_web_master/snort/migrations/0006_rename_main_ref_snortrule_document_and_more.py
--rw-rw-rw-   0        0        0      477 2023-04-19 09:28:30.000000 snort_web_master-1.0.0.0/snort_web_master/snort/migrations/0007_snortrule_tag.py
--rw-rw-rw-   0        0        0        0 2022-12-19 18:19:43.000000 snort_web_master-1.0.0.0/snort_web_master/snort/migrations/__init__.py
--rw-rw-rw-   0        0        0     2187 2023-04-19 09:28:26.000000 snort_web_master-1.0.0.0/snort_web_master/snort/models.py
--rw-rw-rw-   0        0        0    20381 2023-06-07 09:00:35.000000 snort_web_master-1.0.0.0/snort_web_master/snort/parser.py
--rw-rw-rw-   0        0        0     2271 2022-12-19 09:13:39.000000 snort_web_master-1.0.0.0/snort_web_master/snort/snort_templates.py
--rw-rw-rw-   0        0        0     4016 2023-02-21 08:27:30.000000 snort_web_master-1.0.0.0/snort_web_master/snort/tests.py
--rw-rw-rw-   0        0        0    15563 2023-06-21 14:25:19.000000 snort_web_master-1.0.0.0/snort_web_master/snort/views.py
-drwxrwxrwx   0        0        0        0 2023-06-21 14:29:26.348312 snort_web_master-1.0.0.0/snort_web_master/snort_web_master/
--rw-rw-rw-   0        0        0        0 2022-11-21 06:23:37.000000 snort_web_master-1.0.0.0/snort_web_master/snort_web_master/__init__.py
--rw-rw-rw-   0        0        0      425 2022-10-31 09:02:02.000000 snort_web_master-1.0.0.0/snort_web_master/snort_web_master/asgi.py
-drwxrwxrwx   0        0        0        0 2023-06-21 14:29:26.363937 snort_web_master-1.0.0.0/snort_web_master/snort_web_master/middleware/
--rw-rw-rw-   0        0        0        0 2023-01-09 07:35:12.000000 snort_web_master-1.0.0.0/snort_web_master/snort_web_master/middleware/__init__.py
--rw-rw-rw-   0        0        0      733 2023-05-24 09:46:45.000000 snort_web_master-1.0.0.0/snort_web_master/snort_web_master/middleware/no_cache.py
--rw-rw-rw-   0        0        0     5965 2023-06-10 07:48:30.000000 snort_web_master-1.0.0.0/snort_web_master/snort_web_master/settings.py
--rw-rw-rw-   0        0        0     2413 2023-06-21 12:48:53.000000 snort_web_master-1.0.0.0/snort_web_master/snort_web_master/urls.py
--rw-rw-rw-   0        0        0      425 2023-04-19 08:13:33.000000 snort_web_master-1.0.0.0/snort_web_master/snort_web_master/wsgi.py
-drwxrwxrwx   0        0        0        0 2023-06-21 14:29:26.363937 snort_web_master-1.0.0.0/snort_web_master/snort_web_master.egg-info/
--rw-rw-rw-   0        0        0      251 2023-06-21 14:29:26.000000 snort_web_master-1.0.0.0/snort_web_master/snort_web_master.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3656 2023-06-21 14:29:26.000000 snort_web_master-1.0.0.0/snort_web_master/snort_web_master.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 14:29:26.000000 snort_web_master-1.0.0.0/snort_web_master/snort_web_master.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      155 2023-06-21 14:29:26.000000 snort_web_master-1.0.0.0/snort_web_master/snort_web_master.egg-info/requires.txt
--rw-rw-rw-   0        0        0       38 2023-06-21 14:29:26.000000 snort_web_master-1.0.0.0/snort_web_master/snort_web_master.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-21 16:07:24.564910 snort_web_master-1.0.0.1/
+-rw-rw-rw-   0        0        0       54 2022-11-21 06:29:02.000000 snort_web_master-1.0.0.1/LICENSE.rst
+-rw-rw-rw-   0        0        0       24 2022-11-24 17:54:23.000000 snort_web_master-1.0.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      251 2023-06-21 16:07:24.564910 snort_web_master-1.0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      716 2022-11-21 06:20:44.000000 snort_web_master-1.0.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-21 16:07:24.096279 snort_web_master-1.0.0.1/data/
+drwxrwxrwx   0        0        0        0 2023-06-21 16:07:24.127624 snort_web_master-1.0.0.1/data/admin/
+-rw-rw-rw-   0        0        0      698 2023-04-19 07:30:34.000000 snort_web_master-1.0.0.1/data/admin/0004_keyword_delete_keywords.py
+drwxrwxrwx   0        0        0        0 2023-06-21 16:07:24.127624 snort_web_master-1.0.0.1/data/admin/image/
+-rw-rw-rw-   0        0        0     7972 2023-01-16 16:49:34.000000 snort_web_master-1.0.0.1/data/admin/image/images.png
+-rw-rw-rw-   0        0        0   356352 2023-06-21 14:26:22.000000 snort_web_master-1.0.0.1/data/db.sqlite3
+-rw-rw-rw-   0        0        0    39363 2022-10-13 12:31:39.000000 snort_web_master-1.0.0.1/data/dicts.py
+-rw-rw-rw-   0        0        0      690 2023-01-23 09:10:03.000000 snort_web_master-1.0.0.1/data/dockercompose
+-rw-rw-rw-   0        0        0   139272 2023-01-16 16:50:11.000000 snort_web_master-1.0.0.1/data/favicon.ico
+-rw-rw-rw-   0        0        0    25803 2023-05-02 11:59:42.000000 snort_web_master-1.0.0.1/data/http.cap
+-rw-rw-rw-   0        0        0      898 2023-01-23 08:40:15.000000 snort_web_master-1.0.0.1/data/migrate sqllite to postgresql
+-rw-rw-rw-   0        0        0      402 2022-11-14 09:05:52.000000 snort_web_master-1.0.0.1/data/my-snort-rule.tmp
+drwxrwxrwx   0        0        0        0 2023-06-21 16:07:24.127624 snort_web_master-1.0.0.1/data/nginx/
+-rw-rw-rw-   0        0        0       96 2023-01-23 09:09:18.000000 snort_web_master-1.0.0.1/data/nginx/nginx
+-rw-rw-rw-   0        0        0      296 2023-01-23 09:04:00.000000 snort_web_master-1.0.0.1/data/nginx/nginx.conf
+-rw-rw-rw-   0        0        0      162 2023-01-23 08:44:15.000000 snort_web_master-1.0.0.1/data/requirements.txt
+-rw-rw-rw-   0        0        0      889 2023-05-02 14:51:31.000000 snort_web_master-1.0.0.1/data/snortFile
+drwxrwxrwx   0        0        0        0 2023-06-21 16:07:24.127624 snort_web_master-1.0.0.1/data/static/
+drwxrwxrwx   0        0        0        0 2023-06-21 16:07:24.018051 snort_web_master-1.0.0.1/data/static/admin/
+drwxrwxrwx   0        0        0        0 2023-06-21 16:07:24.143045 snort_web_master-1.0.0.1/data/static/admin/css/
+-rw-rw-rw-   0        0        0     1172 2023-06-21 13:46:42.000000 snort_web_master-1.0.0.1/data/static/admin/css/admin-styles.css
+-rw-rw-rw-   0        0        0    20344 2023-06-10 07:58:01.000000 snort_web_master-1.0.0.1/data/static/admin/css/base.css
+-rw-rw-rw-   0        0        0     9730 2023-06-10 07:59:05.000000 snort_web_master-1.0.0.1/data/static/admin/css/forms.css
+-rw-rw-rw-   0        0        0     2619 2023-06-10 07:58:10.000000 snort_web_master-1.0.0.1/data/static/admin/css/nav_sidebar.css
+drwxrwxrwx   0        0        0        0 2023-06-21 16:07:24.018051 snort_web_master-1.0.0.1/data/static/admin/css/vendor/
+drwxrwxrwx   0        0        0        0 2023-06-21 16:07:24.143045 snort_web_master-1.0.0.1/data/static/admin/css/vendor/select2/
+-rw-rw-rw-   0        0        0     1124 2022-12-26 08:06:54.000000 snort_web_master-1.0.0.1/data/static/admin/css/vendor/select2/LICENSE-SELECT2.md
+-rw-rw-rw-   0        0        0    17358 2022-12-26 08:06:54.000000 snort_web_master-1.0.0.1/data/static/admin/css/vendor/select2/select2.css
+-rw-rw-rw-   0        0        0    14966 2022-12-26 08:06:54.000000 snort_web_master-1.0.0.1/data/static/admin/css/vendor/select2/select2.min.css
+drwxrwxrwx   0        0        0        0 2023-06-21 16:07:24.158660 snort_web_master-1.0.0.1/data/static/admin/image/
+-rw-rw-rw-   0        0        0     7972 2023-01-16 16:49:34.000000 snort_web_master-1.0.0.1/data/static/admin/image/images.png
+drwxrwxrwx   0        0        0        0 2023-06-21 16:07:24.158660 snort_web_master-1.0.0.1/data/static/css/
+-rw-rw-rw-   0        0        0     1890 2023-06-14 17:15:26.000000 snort_web_master-1.0.0.1/data/static/css/main.55b651d4.css
+-rw-rw-rw-   0        0        0     3089 2023-06-14 17:15:26.000000 snort_web_master-1.0.0.1/data/static/css/main.55b651d4.css.map
+-rw-rw-rw-   0        0        0   139272 2023-01-16 16:50:11.000000 snort_web_master-1.0.0.1/data/static/favico.ico
+drwxrwxrwx   0        0        0        0 2023-06-21 16:07:24.174285 snort_web_master-1.0.0.1/data/static/js/
+-rw-rw-rw-   0        0        0     4591 2023-06-14 11:57:57.000000 snort_web_master-1.0.0.1/data/static/js/787.2c2ec360.chunk.js
+-rw-rw-rw-   0        0        0    10592 2023-06-14 11:57:57.000000 snort_web_master-1.0.0.1/data/static/js/787.2c2ec360.chunk.js.map
+-rw-rw-rw-   0        0        0   656292 2023-06-21 12:35:36.000000 snort_web_master-1.0.0.1/data/static/js/main.ad6031d4.js
+-rw-rw-rw-   0        0        0     1458 2023-06-21 12:35:36.000000 snort_web_master-1.0.0.1/data/static/js/main.ad6031d4.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  2485433 2023-06-21 12:35:36.000000 snort_web_master-1.0.0.1/data/static/js/main.ad6031d4.js.map
+drwxrwxrwx   0        0        0        0 2023-06-21 16:07:24.018051 snort_web_master-1.0.0.1/data/templates/
+drwxrwxrwx   0        0        0        0 2023-06-21 16:07:24.189909 snort_web_master-1.0.0.1/data/templates/html/
+-rw-rw-rw-   0        0        0      150 2023-06-21 12:36:15.000000 snort_web_master-1.0.0.1/data/templates/html/full_rule.html
+-rw-rw-rw-   0        0        0      420 2023-01-23 09:19:00.000000 snort_web_master-1.0.0.1/data/templates/html/import.html
+-rw-rw-rw-   0        0        0     3565 2023-06-14 12:05:15.000000 snort_web_master-1.0.0.1/data/templates/html/snortBuilder.html
+-rw-rw-rw-   0        0        0      140 2023-06-21 16:07:24.580532 snort_web_master-1.0.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      862 2023-06-21 16:06:12.000000 snort_web_master-1.0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 16:07:24.018051 snort_web_master-1.0.0.1/snort_web_master/
+drwxrwxrwx   0        0        0        0 2023-06-21 16:07:24.236805 snort_web_master-1.0.0.1/snort_web_master/pcaps/
+-rw-rw-rw-   0        0        0        0 2022-10-31 09:04:45.000000 snort_web_master-1.0.0.1/snort_web_master/pcaps/__init__.py
+-rw-rw-rw-   0        0        0     2689 2023-01-08 17:50:03.000000 snort_web_master-1.0.0.1/snort_web_master/pcaps/admin.py
+-rw-rw-rw-   0        0        0      148 2022-10-31 09:04:45.000000 snort_web_master-1.0.0.1/snort_web_master/pcaps/apps.py
+drwxrwxrwx   0        0        0        0 2023-06-21 16:07:24.268048 snort_web_master-1.0.0.1/snort_web_master/pcaps/migrations/
+-rw-rw-rw-   0        0        0     1385 2022-12-19 18:20:00.000000 snort_web_master-1.0.0.1/snort_web_master/pcaps/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      813 2022-12-19 18:20:00.000000 snort_web_master-1.0.0.1/snort_web_master/pcaps/migrations/0002_initial.py
+-rw-rw-rw-   0        0        0      555 2022-12-19 18:24:58.000000 snort_web_master-1.0.0.1/snort_web_master/pcaps/migrations/0003_rename_rule_to_validate_pcap_rule_to_validate2_and_more.py
+-rw-rw-rw-   0        0        0      603 2022-12-19 18:25:24.000000 snort_web_master-1.0.0.1/snort_web_master/pcaps/migrations/0004_rename_rule_to_validate2_pcap_rule_to_validate_and_more.py
+-rw-rw-rw-   0        0        0        0 2022-12-19 18:19:43.000000 snort_web_master-1.0.0.1/snort_web_master/pcaps/migrations/__init__.py
+-rw-rw-rw-   0        0        0     1060 2022-12-19 18:25:20.000000 snort_web_master-1.0.0.1/snort_web_master/pcaps/models.py
+-rw-rw-rw-   0        0        0       63 2022-10-31 09:04:45.000000 snort_web_master-1.0.0.1/snort_web_master/pcaps/tests.py
+-rw-rw-rw-   0        0        0       66 2022-10-31 09:04:45.000000 snort_web_master-1.0.0.1/snort_web_master/pcaps/views.py
+drwxrwxrwx   0        0        0        0 2023-06-21 16:07:24.283657 snort_web_master-1.0.0.1/snort_web_master/settings/
+-rw-rw-rw-   0        0        0        0 2022-12-19 07:00:41.000000 snort_web_master-1.0.0.1/snort_web_master/settings/__init__.py
+-rw-rw-rw-   0        0        0      546 2023-04-19 09:25:30.000000 snort_web_master-1.0.0.1/snort_web_master/settings/admin.py
+-rw-rw-rw-   0        0        0      154 2022-12-19 07:00:41.000000 snort_web_master-1.0.0.1/snort_web_master/settings/apps.py
+drwxrwxrwx   0        0        0        0 2023-06-21 16:07:24.346171 snort_web_master-1.0.0.1/snort_web_master/settings/migrations/
+-rw-rw-rw-   0        0        0     1595 2022-12-19 18:20:00.000000 snort_web_master-1.0.0.1/snort_web_master/settings/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0     1350 2022-12-26 06:21:16.000000 snort_web_master-1.0.0.1/snort_web_master/settings/migrations/0002_remove_keywords_type_keywords_description_and_more.py
+-rw-rw-rw-   0        0        0      530 2022-12-26 06:23:11.000000 snort_web_master-1.0.0.1/snort_web_master/settings/migrations/0003_keywords_avalable.py
+-rw-rw-rw-   0        0        0      698 2023-04-19 07:30:34.000000 snort_web_master-1.0.0.1/snort_web_master/settings/migrations/0004_keyword_delete_keywords.py
+-rw-rw-rw-   0        0        0     1268 2023-04-19 09:28:30.000000 snort_web_master-1.0.0.1/snort_web_master/settings/migrations/0005_remove_keyword_negation_alter_keyword_description_and_more.py
+-rw-rw-rw-   0        0        0        0 2022-12-19 18:19:43.000000 snort_web_master-1.0.0.1/snort_web_master/settings/migrations/__init__.py
+-rw-rw-rw-   0        0        0     1476 2023-06-01 19:36:46.000000 snort_web_master-1.0.0.1/snort_web_master/settings/models.py
+-rw-rw-rw-   0        0        0       63 2022-12-19 07:00:41.000000 snort_web_master-1.0.0.1/snort_web_master/settings/tests.py
+-rw-rw-rw-   0        0        0       66 2022-12-19 07:00:41.000000 snort_web_master-1.0.0.1/snort_web_master/settings/views.py
+drwxrwxrwx   0        0        0        0 2023-06-21 16:07:24.440137 snort_web_master-1.0.0.1/snort_web_master/snort/
+-rw-rw-rw-   0        0        0        0 2022-10-31 09:04:41.000000 snort_web_master-1.0.0.1/snort_web_master/snort/__init__.py
+-rw-rw-rw-   0        0        0    32726 2023-06-21 16:04:57.000000 snort_web_master-1.0.0.1/snort_web_master/snort/admin.py
+-rw-rw-rw-   0        0        0      148 2022-10-31 09:04:41.000000 snort_web_master-1.0.0.1/snort_web_master/snort/apps.py
+drwxrwxrwx   0        0        0        0 2023-06-21 16:07:24.471247 snort_web_master-1.0.0.1/snort_web_master/snort/migrations/
+-rw-rw-rw-   0        0        0     1974 2022-12-19 18:20:00.000000 snort_web_master-1.0.0.1/snort_web_master/snort/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      870 2023-01-05 14:35:56.000000 snort_web_master-1.0.0.1/snort_web_master/snort/migrations/0002_snortruleviewarray.py
+-rw-rw-rw-   0        0        0      610 2023-01-06 06:03:56.000000 snort_web_master-1.0.0.1/snort_web_master/snort/migrations/0003_snortruleviewarray_htmlid_and_more.py
+-rw-rw-rw-   0        0        0      423 2023-01-06 13:23:29.000000 snort_web_master-1.0.0.1/snort_web_master/snort/migrations/0004_snortrule_deleted.py
+-rw-rw-rw-   0        0        0      522 2023-01-08 17:24:52.000000 snort_web_master-1.0.0.1/snort_web_master/snort/migrations/0005_remove_snortrule_template_snortrule_is_template.py
+-rw-rw-rw-   0        0        0      759 2023-02-21 08:33:21.000000 snort_web_master-1.0.0.1/snort_web_master/snort/migrations/0006_rename_main_ref_snortrule_document_and_more.py
+-rw-rw-rw-   0        0        0      477 2023-04-19 09:28:30.000000 snort_web_master-1.0.0.1/snort_web_master/snort/migrations/0007_snortrule_tag.py
+-rw-rw-rw-   0        0        0        0 2022-12-19 18:19:43.000000 snort_web_master-1.0.0.1/snort_web_master/snort/migrations/__init__.py
+-rw-rw-rw-   0        0        0     2187 2023-04-19 09:28:26.000000 snort_web_master-1.0.0.1/snort_web_master/snort/models.py
+-rw-rw-rw-   0        0        0    20381 2023-06-07 09:00:35.000000 snort_web_master-1.0.0.1/snort_web_master/snort/parser.py
+-rw-rw-rw-   0        0        0     2271 2022-12-19 09:13:39.000000 snort_web_master-1.0.0.1/snort_web_master/snort/snort_templates.py
+-rw-rw-rw-   0        0        0     4016 2023-02-21 08:27:30.000000 snort_web_master-1.0.0.1/snort_web_master/snort/tests.py
+-rw-rw-rw-   0        0        0    15754 2023-06-21 15:52:15.000000 snort_web_master-1.0.0.1/snort_web_master/snort/views.py
+drwxrwxrwx   0        0        0        0 2023-06-21 16:07:24.518255 snort_web_master-1.0.0.1/snort_web_master/snort_web_master/
+-rw-rw-rw-   0        0        0        0 2022-11-21 06:23:37.000000 snort_web_master-1.0.0.1/snort_web_master/snort_web_master/__init__.py
+-rw-rw-rw-   0        0        0      425 2022-10-31 09:02:02.000000 snort_web_master-1.0.0.1/snort_web_master/snort_web_master/asgi.py
+drwxrwxrwx   0        0        0        0 2023-06-21 16:07:24.564910 snort_web_master-1.0.0.1/snort_web_master/snort_web_master/middleware/
+-rw-rw-rw-   0        0        0        0 2023-01-09 07:35:12.000000 snort_web_master-1.0.0.1/snort_web_master/snort_web_master/middleware/__init__.py
+-rw-rw-rw-   0        0        0      733 2023-05-24 09:46:45.000000 snort_web_master-1.0.0.1/snort_web_master/snort_web_master/middleware/no_cache.py
+-rw-rw-rw-   0        0        0     5965 2023-06-10 07:48:30.000000 snort_web_master-1.0.0.1/snort_web_master/snort_web_master/settings.py
+-rw-rw-rw-   0        0        0     2413 2023-06-21 12:48:53.000000 snort_web_master-1.0.0.1/snort_web_master/snort_web_master/urls.py
+-rw-rw-rw-   0        0        0      425 2023-04-19 08:13:33.000000 snort_web_master-1.0.0.1/snort_web_master/snort_web_master/wsgi.py
+drwxrwxrwx   0        0        0        0 2023-06-21 16:07:24.564910 snort_web_master-1.0.0.1/snort_web_master/snort_web_master.egg-info/
+-rw-rw-rw-   0        0        0      251 2023-06-21 16:07:23.000000 snort_web_master-1.0.0.1/snort_web_master/snort_web_master.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3656 2023-06-21 16:07:23.000000 snort_web_master-1.0.0.1/snort_web_master/snort_web_master.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 16:07:23.000000 snort_web_master-1.0.0.1/snort_web_master/snort_web_master.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      155 2023-06-21 16:07:23.000000 snort_web_master-1.0.0.1/snort_web_master/snort_web_master.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       38 2023-06-21 16:07:23.000000 snort_web_master-1.0.0.1/snort_web_master/snort_web_master.egg-info/top_level.txt
```

### Comparing `snort_web_master-1.0.0.0/README.md` & `snort_web_master-1.0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/data/admin/0004_keyword_delete_keywords.py` & `snort_web_master-1.0.0.1/data/admin/0004_keyword_delete_keywords.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/data/admin/image/images.png` & `snort_web_master-1.0.0.1/data/admin/image/images.png`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/data/db.sqlite3` & `snort_web_master-1.0.0.1/data/db.sqlite3`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/data/dicts.py` & `snort_web_master-1.0.0.1/data/dicts.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/data/dockercompose` & `snort_web_master-1.0.0.1/data/dockercompose`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/data/favicon.ico` & `snort_web_master-1.0.0.1/data/favicon.ico`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/data/http.cap` & `snort_web_master-1.0.0.1/data/http.cap`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/data/migrate sqllite to postgresql` & `snort_web_master-1.0.0.1/data/migrate sqllite to postgresql`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/data/snortFile` & `snort_web_master-1.0.0.1/data/snortFile`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/data/static/admin/css/admin-styles.css` & `snort_web_master-1.0.0.1/data/static/admin/css/admin-styles.css`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/data/static/admin/css/base.css` & `snort_web_master-1.0.0.1/data/static/admin/css/base.css`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/data/static/admin/css/forms.css` & `snort_web_master-1.0.0.1/data/static/admin/css/forms.css`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/data/static/admin/css/nav_sidebar.css` & `snort_web_master-1.0.0.1/data/static/admin/css/nav_sidebar.css`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/data/static/admin/css/vendor/select2/LICENSE-SELECT2.md` & `snort_web_master-1.0.0.1/data/static/admin/css/vendor/select2/LICENSE-SELECT2.md`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/data/static/admin/css/vendor/select2/select2.css` & `snort_web_master-1.0.0.1/data/static/admin/css/vendor/select2/select2.css`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/data/static/admin/css/vendor/select2/select2.min.css` & `snort_web_master-1.0.0.1/data/static/admin/css/vendor/select2/select2.min.css`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/data/static/admin/image/images.png` & `snort_web_master-1.0.0.1/data/static/admin/image/images.png`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/data/static/css/main.55b651d4.css` & `snort_web_master-1.0.0.1/data/static/css/main.55b651d4.css`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/data/static/css/main.55b651d4.css.map` & `snort_web_master-1.0.0.1/data/static/css/main.55b651d4.css.map`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/data/static/favico.ico` & `snort_web_master-1.0.0.1/data/static/favico.ico`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/data/static/js/787.2c2ec360.chunk.js` & `snort_web_master-1.0.0.1/data/static/js/787.2c2ec360.chunk.js`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/data/static/js/787.2c2ec360.chunk.js.map` & `snort_web_master-1.0.0.1/data/static/js/787.2c2ec360.chunk.js.map`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/data/static/js/main.ad6031d4.js` & `snort_web_master-1.0.0.1/data/static/js/main.ad6031d4.js`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/data/static/js/main.ad6031d4.js.LICENSE.txt` & `snort_web_master-1.0.0.1/data/static/js/main.ad6031d4.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/data/static/js/main.ad6031d4.js.map` & `snort_web_master-1.0.0.1/data/static/js/main.ad6031d4.js.map`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/data/templates/html/snortBuilder.html` & `snort_web_master-1.0.0.1/data/templates/html/snortBuilder.html`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/setup.py` & `snort_web_master-1.0.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 from setuptools import setup, find_packages
 
 
 setup(
     name='snort_web_master',
-    version='1.0.0.0',
+    version='1.0.0.1',
     license='MoCorp',
     readme="README.md",
     author="meir dahan",
     author_email='1dahanmeir1@gmail.com',
     packages=find_packages('snort_web_master'),
     package_dir={'': 'snort_web_master'},
     url='https://github.com/mosheovadi1/snort-web-master',
```

### Comparing `snort_web_master-1.0.0.0/snort_web_master/pcaps/admin.py` & `snort_web_master-1.0.0.1/snort_web_master/pcaps/admin.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/snort_web_master/pcaps/migrations/0001_initial.py` & `snort_web_master-1.0.0.1/snort_web_master/pcaps/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/snort_web_master/pcaps/migrations/0002_initial.py` & `snort_web_master-1.0.0.1/snort_web_master/pcaps/migrations/0002_initial.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/snort_web_master/pcaps/migrations/0003_rename_rule_to_validate_pcap_rule_to_validate2_and_more.py` & `snort_web_master-1.0.0.1/snort_web_master/pcaps/migrations/0003_rename_rule_to_validate_pcap_rule_to_validate2_and_more.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/snort_web_master/pcaps/migrations/0004_rename_rule_to_validate2_pcap_rule_to_validate_and_more.py` & `snort_web_master-1.0.0.1/snort_web_master/pcaps/migrations/0004_rename_rule_to_validate2_pcap_rule_to_validate_and_more.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/snort_web_master/pcaps/models.py` & `snort_web_master-1.0.0.1/snort_web_master/pcaps/models.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/snort_web_master/settings/admin.py` & `snort_web_master-1.0.0.1/snort_web_master/settings/admin.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/snort_web_master/settings/migrations/0001_initial.py` & `snort_web_master-1.0.0.1/snort_web_master/settings/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/snort_web_master/settings/migrations/0002_remove_keywords_type_keywords_description_and_more.py` & `snort_web_master-1.0.0.1/snort_web_master/settings/migrations/0002_remove_keywords_type_keywords_description_and_more.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/snort_web_master/settings/migrations/0003_keywords_avalable.py` & `snort_web_master-1.0.0.1/snort_web_master/settings/migrations/0003_keywords_avalable.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/snort_web_master/settings/migrations/0004_keyword_delete_keywords.py` & `snort_web_master-1.0.0.1/snort_web_master/settings/migrations/0004_keyword_delete_keywords.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/snort_web_master/settings/migrations/0005_remove_keyword_negation_alter_keyword_description_and_more.py` & `snort_web_master-1.0.0.1/snort_web_master/settings/migrations/0005_remove_keyword_negation_alter_keyword_description_and_more.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/snort_web_master/settings/models.py` & `snort_web_master-1.0.0.1/snort_web_master/settings/models.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/snort_web_master/snort/admin.py` & `snort_web_master-1.0.0.1/snort_web_master/snort/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import copy
 import os
 import csv
 import time
 from io import StringIO
 from django.contrib import messages
 import re
+import json
 
 from django.core.exceptions import ValidationError
 from import_export.admin import ImportExportModelAdmin
 from django import forms
 
 import pcaps.models
 from .models import SnortRule, SnortRuleViewArray, save_rule_to_s3, delete_rule_from_s3
 from .snort_templates import types_list
 from .parser import Parser
 from django.utils.encoding import smart_str
 from django.http.response import HttpResponse, HttpResponseRedirect
 from django.utils.html import mark_safe
 from django.db import transaction
 import suricataparser
-from snort.views import build_keyword_dict
+from snort.views import build_keyword_dict, build_rule_parse
 # Register your models here.
 from django.contrib import admin
 from django_object_actions import DjangoObjectActions
 import subprocess
 from settings.models import Setting, keyword, attackGroup
 from django.shortcuts import render
 from pcaps.admin import verify_legal_pcap
@@ -82,15 +83,14 @@
         if not dict(types_list).get(self.cleaned_data.get("type")):
             raise forms.ValidationError("cant find type, did you forgot it? or forgot to add type to db", code=404)
         return self.cleaned_data.get("type")
 
     def clean_content(self):
         try:
             parser = Parser(self.data["content"])
-            parser = Parser(self.data["content"])
             parser.parse_header()
             options = parser.parse_options()
             for option in options:
                 try:
                     if options[option][1] != [""] and options[option][0] != "tag":
                         break
                 except:
@@ -284,32 +284,36 @@
             content = re.sub(regex, subst, content, 0, re.MULTILINE)
             if "user" not in self.changed_data:
                 self.changed_data.append("user")
         except Exception as e:
             self.add_error("user", e)
         try:
             self.clean_content()
+            if not self.current_user.is_superuser:
+                res = build_rule_parse("/build_rule_parse/", self.data["content"])
+                if json.loads(res.content).get("unparsed_data"):
+                    raise Exception("unparsed data exists, non admin cannot add unparsed data!")
         except Exception as e:
             if not self.errors:
-                raise ValidationError(e)
+                self.add_error(None, e)
 
 
         self.instance.deleted = False
         if not self.instance.pk and not self.errors:
             self.instance.save()
             # set sid in content for the new rule
-            if "sid:-;" in content:
-                self.cleaned_data["content"] = content.replace("sid:-;", f"sid:{self.instance.pk};")
+            if "sid:None;" in content:
+                self.cleaned_data["content"] = content.replace("sid:None;", f"sid:{self.instance.pk};")
                 if "content" not in self.changed_data:
                     self.changed_data.append("content")
         else:
             self.cleaned_data["content"] = content
+        self.instance.content = self.cleaned_data["content"]
         if not self.errors:
             SnortRuleViewArray.objects.filter(snortId=self.instance.id).delete()
-        if not self.errors:
             cache.set(self.instance.id, content)
         else:
             cache.set(self.instance.id, content)
             return
         if self.cleaned_data.get("active"):
             save_rule_to_s3(self.instance.id, self.instance.content)
             pass
@@ -576,20 +580,20 @@
     def get_actions(self, request):
         actions = super().get_actions(request)
         if 'delete_selected' in actions:
             del actions['delete_selected']
         return actions
 
     def snort_builder(self, obj):
-        set_rule = cache.get(obj.id)
-        if not set_rule:
-            set_rule = SnortRuleViewArray.objects.filter(snortId=obj.id)
-            cache.set(obj.id, set_rule)
-        else:
-            cache.set(obj.id, [])
+        # set_rule = cache.get(obj.id)
+        # if not set_rule:
+        #     set_rule = SnortRuleViewArray.objects.filter(snortId=obj.id)
+        #     cache.set(obj.id, set_rule)
+        # else:
+        #     cache.set(obj.id, [])
         context = {}
         # todo handle caching of rule
         # context["build_items"] = set_rule
         # context["actions"] = keyword.objects.filter(stage="action", available="True")
         # context["protocols"] = keyword.objects.filter(stage="protocol", available="True")
 
         tmp_context = copy.deepcopy(self.request.session.get("cloned_rule", {}))
```

### Comparing `snort_web_master-1.0.0.0/snort_web_master/snort/migrations/0001_initial.py` & `snort_web_master-1.0.0.1/snort_web_master/snort/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/snort_web_master/snort/migrations/0002_snortruleviewarray.py` & `snort_web_master-1.0.0.1/snort_web_master/snort/migrations/0002_snortruleviewarray.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/snort_web_master/snort/migrations/0003_snortruleviewarray_htmlid_and_more.py` & `snort_web_master-1.0.0.1/snort_web_master/snort/migrations/0003_snortruleviewarray_htmlid_and_more.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/snort_web_master/snort/migrations/0005_remove_snortrule_template_snortrule_is_template.py` & `snort_web_master-1.0.0.1/snort_web_master/snort/migrations/0005_remove_snortrule_template_snortrule_is_template.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/snort_web_master/snort/migrations/0006_rename_main_ref_snortrule_document_and_more.py` & `snort_web_master-1.0.0.1/snort_web_master/snort/migrations/0006_rename_main_ref_snortrule_document_and_more.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/snort_web_master/snort/models.py` & `snort_web_master-1.0.0.1/snort_web_master/snort/models.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/snort_web_master/snort/parser.py` & `snort_web_master-1.0.0.1/snort_web_master/snort/parser.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/snort_web_master/snort/snort_templates.py` & `snort_web_master-1.0.0.1/snort_web_master/snort/snort_templates.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/snort_web_master/snort/tests.py` & `snort_web_master-1.0.0.1/snort_web_master/snort/tests.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/snort_web_master/snort/views.py` & `snort_web_master-1.0.0.1/snort_web_master/snort/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import os
 from django.views.decorators.csrf import csrf_exempt
 from django.conf import settings
 from .parser import Parser, SerializeRule
 from settings.models import keyword
 from settings.models import Setting
 from django.core.serializers import serialize
+from django.core.cache import cache
 # Create your views here.
 
 def get_rule_keys(request, rule_id=None):
     rule_keywordss = SnortRuleViewArray.objects.filter(**{"snortId": rule_id})
     results = {"data": []}
     for rule_key in rule_keywordss:
         results["data"].append({"htmlId": rule_key.htmlId, "value": rule_key.value, "typeOfItem": rule_key.typeOfItem,
@@ -22,15 +23,20 @@
     return JsonResponse(results)
 
 
 def get_rule(request, rule_id=None, cloned=None):
     if (request.session.get("instance")):
         r_value = HttpResponse(json.loads(request.session.pop("instance"))[0]["fields"]["content"])
         return r_value
-    full_rule = SnortRule.objects.get(**{"id": rule_id}).content
+    else:
+        full_rule = cache.get(rule_id) or ""
+        if full_rule:
+            cache.delete(rule_id)
+    if not full_rule and rule_id:
+        full_rule = SnortRule.objects.get(**{"id": rule_id}).content
     return HttpResponse(full_rule)
 
 @csrf_exempt
 def build_rule_keyword_to_rule(request, full_rule=""):
     if not full_rule and request.method == "POST":
         try:
             full_rule = json.loads(request.body.decode()).get("fule_rule")
```

### Comparing `snort_web_master-1.0.0.0/snort_web_master/snort_web_master/middleware/no_cache.py` & `snort_web_master-1.0.0.1/snort_web_master/snort_web_master/middleware/no_cache.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/snort_web_master/snort_web_master/settings.py` & `snort_web_master-1.0.0.1/snort_web_master/snort_web_master/settings.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/snort_web_master/snort_web_master/urls.py` & `snort_web_master-1.0.0.1/snort_web_master/snort_web_master/urls.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-1.0.0.0/snort_web_master/snort_web_master.egg-info/SOURCES.txt` & `snort_web_master-1.0.0.1/snort_web_master/snort_web_master.egg-info/SOURCES.txt`

 * *Files identical despite different names*

