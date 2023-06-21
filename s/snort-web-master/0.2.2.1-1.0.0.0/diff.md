# Comparing `tmp/snort_web_master-0.2.2.1.tar.gz` & `tmp/snort_web_master-1.0.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\snort_web_master-0.2.2.1.tar", last modified: Wed May 10 06:37:53 2023, max compression
+gzip compressed data, was "dist\snort_web_master-1.0.0.0.tar", last modified: Wed Jun 21 14:29:26 2023, max compression
```

## Comparing `snort_web_master-0.2.2.1.tar` & `snort_web_master-1.0.0.0.tar`

### file list

```diff
@@ -1,90 +1,114 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 06:37:53.011461 snort_web_master-0.2.2.1/
--rw-rw-rw-   0        0        0       54 2022-11-21 06:29:02.000000 snort_web_master-0.2.2.1/LICENSE.rst
--rw-rw-rw-   0        0        0       24 2022-11-24 17:54:23.000000 snort_web_master-0.2.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0      251 2023-05-10 06:37:53.011461 snort_web_master-0.2.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      716 2022-11-21 06:20:44.000000 snort_web_master-0.2.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 06:37:52.454203 snort_web_master-0.2.2.1/data/
-drwxrwxrwx   0        0        0        0 2023-05-10 06:37:52.470030 snort_web_master-0.2.2.1/data/admin/
--rw-rw-rw-   0        0        0      698 2023-04-19 07:30:34.000000 snort_web_master-0.2.2.1/data/admin/0004_keyword_delete_keywords.py
-drwxrwxrwx   0        0        0        0 2023-05-10 06:37:52.485548 snort_web_master-0.2.2.1/data/admin/image/
--rw-rw-rw-   0        0        0     7972 2023-01-16 16:49:34.000000 snort_web_master-0.2.2.1/data/admin/image/images.png
--rw-rw-rw-   0        0        0   241664 2023-01-07 17:05:37.000000 snort_web_master-0.2.2.1/data/db.sqlite3
--rw-rw-rw-   0        0        0    39363 2022-10-13 12:31:39.000000 snort_web_master-0.2.2.1/data/dicts.py
--rw-rw-rw-   0        0        0      690 2023-01-23 09:10:03.000000 snort_web_master-0.2.2.1/data/dockercompose
--rw-rw-rw-   0        0        0   139272 2023-01-16 16:50:11.000000 snort_web_master-0.2.2.1/data/favicon.ico
--rw-rw-rw-   0        0        0    25803 2023-05-02 11:59:42.000000 snort_web_master-0.2.2.1/data/http.cap
--rw-rw-rw-   0        0        0      898 2023-01-23 08:40:15.000000 snort_web_master-0.2.2.1/data/migrate sqllite to postgresql
--rw-rw-rw-   0        0        0      402 2022-11-14 09:05:52.000000 snort_web_master-0.2.2.1/data/my-snort-rule.tmp
-drwxrwxrwx   0        0        0        0 2023-05-10 06:37:52.485548 snort_web_master-0.2.2.1/data/nginx/
--rw-rw-rw-   0        0        0       96 2023-01-23 09:09:18.000000 snort_web_master-0.2.2.1/data/nginx/nginx
--rw-rw-rw-   0        0        0      296 2023-01-23 09:04:00.000000 snort_web_master-0.2.2.1/data/nginx/nginx.conf
--rw-rw-rw-   0        0        0      162 2023-01-23 08:44:15.000000 snort_web_master-0.2.2.1/data/requirements.txt
--rw-rw-rw-   0        0        0      889 2023-05-02 14:51:31.000000 snort_web_master-0.2.2.1/data/snortFile
-drwxrwxrwx   0        0        0        0 2023-05-10 06:37:52.321570 snort_web_master-0.2.2.1/data/templates/
-drwxrwxrwx   0        0        0        0 2023-05-10 06:37:52.516693 snort_web_master-0.2.2.1/data/templates/html/
--rw-rw-rw-   0        0        0     4866 2023-05-10 05:18:00.000000 snort_web_master-0.2.2.1/data/templates/html/full_rule.html
--rw-rw-rw-   0        0        0      420 2023-01-23 09:19:00.000000 snort_web_master-0.2.2.1/data/templates/html/import.html
--rw-rw-rw-   0        0        0    27092 2023-05-10 05:24:02.000000 snort_web_master-0.2.2.1/data/templates/html/snortBuilder.html
--rw-rw-rw-   0        0        0      140 2023-05-10 06:37:53.011461 snort_web_master-0.2.2.1/setup.cfg
--rw-rw-rw-   0        0        0      862 2023-05-10 06:33:18.000000 snort_web_master-0.2.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 06:37:52.321570 snort_web_master-0.2.2.1/snort_web_master/
-drwxrwxrwx   0        0        0        0 2023-05-10 06:37:52.563545 snort_web_master-0.2.2.1/snort_web_master/pcaps/
--rw-rw-rw-   0        0        0        0 2022-10-31 09:04:45.000000 snort_web_master-0.2.2.1/snort_web_master/pcaps/__init__.py
--rw-rw-rw-   0        0        0     2689 2023-01-08 17:50:03.000000 snort_web_master-0.2.2.1/snort_web_master/pcaps/admin.py
--rw-rw-rw-   0        0        0      148 2022-10-31 09:04:45.000000 snort_web_master-0.2.2.1/snort_web_master/pcaps/apps.py
-drwxrwxrwx   0        0        0        0 2023-05-10 06:37:52.610432 snort_web_master-0.2.2.1/snort_web_master/pcaps/migrations/
--rw-rw-rw-   0        0        0     1385 2022-12-19 18:20:00.000000 snort_web_master-0.2.2.1/snort_web_master/pcaps/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      813 2022-12-19 18:20:00.000000 snort_web_master-0.2.2.1/snort_web_master/pcaps/migrations/0002_initial.py
--rw-rw-rw-   0        0        0      555 2022-12-19 18:24:58.000000 snort_web_master-0.2.2.1/snort_web_master/pcaps/migrations/0003_rename_rule_to_validate_pcap_rule_to_validate2_and_more.py
--rw-rw-rw-   0        0        0      603 2022-12-19 18:25:24.000000 snort_web_master-0.2.2.1/snort_web_master/pcaps/migrations/0004_rename_rule_to_validate2_pcap_rule_to_validate_and_more.py
--rw-rw-rw-   0        0        0        0 2022-12-19 18:19:43.000000 snort_web_master-0.2.2.1/snort_web_master/pcaps/migrations/__init__.py
--rw-rw-rw-   0        0        0     1060 2022-12-19 18:25:20.000000 snort_web_master-0.2.2.1/snort_web_master/pcaps/models.py
--rw-rw-rw-   0        0        0       63 2022-10-31 09:04:45.000000 snort_web_master-0.2.2.1/snort_web_master/pcaps/tests.py
--rw-rw-rw-   0        0        0       66 2022-10-31 09:04:45.000000 snort_web_master-0.2.2.1/snort_web_master/pcaps/views.py
-drwxrwxrwx   0        0        0        0 2023-05-10 06:37:52.641933 snort_web_master-0.2.2.1/snort_web_master/settings/
--rw-rw-rw-   0        0        0        0 2022-12-19 07:00:41.000000 snort_web_master-0.2.2.1/snort_web_master/settings/__init__.py
--rw-rw-rw-   0        0        0      546 2023-04-19 09:25:30.000000 snort_web_master-0.2.2.1/snort_web_master/settings/admin.py
--rw-rw-rw-   0        0        0      154 2022-12-19 07:00:41.000000 snort_web_master-0.2.2.1/snort_web_master/settings/apps.py
-drwxrwxrwx   0        0        0        0 2023-05-10 06:37:52.704383 snort_web_master-0.2.2.1/snort_web_master/settings/migrations/
--rw-rw-rw-   0        0        0     1595 2022-12-19 18:20:00.000000 snort_web_master-0.2.2.1/snort_web_master/settings/migrations/0001_initial.py
--rw-rw-rw-   0        0        0     1350 2022-12-26 06:21:16.000000 snort_web_master-0.2.2.1/snort_web_master/settings/migrations/0002_remove_keywords_type_keywords_description_and_more.py
--rw-rw-rw-   0        0        0      530 2022-12-26 06:23:11.000000 snort_web_master-0.2.2.1/snort_web_master/settings/migrations/0003_keywords_avalable.py
--rw-rw-rw-   0        0        0      698 2023-04-19 07:30:34.000000 snort_web_master-0.2.2.1/snort_web_master/settings/migrations/0004_keyword_delete_keywords.py
--rw-rw-rw-   0        0        0     1268 2023-04-19 09:28:30.000000 snort_web_master-0.2.2.1/snort_web_master/settings/migrations/0005_remove_keyword_negation_alter_keyword_description_and_more.py
--rw-rw-rw-   0        0        0        0 2022-12-19 18:19:43.000000 snort_web_master-0.2.2.1/snort_web_master/settings/migrations/__init__.py
--rw-rw-rw-   0        0        0     1444 2023-04-19 07:32:10.000000 snort_web_master-0.2.2.1/snort_web_master/settings/models.py
--rw-rw-rw-   0        0        0       63 2022-12-19 07:00:41.000000 snort_web_master-0.2.2.1/snort_web_master/settings/tests.py
--rw-rw-rw-   0        0        0       66 2022-12-19 07:00:41.000000 snort_web_master-0.2.2.1/snort_web_master/settings/views.py
-drwxrwxrwx   0        0        0        0 2023-05-10 06:37:52.774916 snort_web_master-0.2.2.1/snort_web_master/snort/
--rw-rw-rw-   0        0        0        0 2022-10-31 09:04:41.000000 snort_web_master-0.2.2.1/snort_web_master/snort/__init__.py
--rw-rw-rw-   0        0        0    31989 2023-05-02 16:50:50.000000 snort_web_master-0.2.2.1/snort_web_master/snort/admin.py
--rw-rw-rw-   0        0        0      148 2022-10-31 09:04:41.000000 snort_web_master-0.2.2.1/snort_web_master/snort/apps.py
-drwxrwxrwx   0        0        0        0 2023-05-10 06:37:52.871046 snort_web_master-0.2.2.1/snort_web_master/snort/migrations/
--rw-rw-rw-   0        0        0     1974 2022-12-19 18:20:00.000000 snort_web_master-0.2.2.1/snort_web_master/snort/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      870 2023-01-05 14:35:56.000000 snort_web_master-0.2.2.1/snort_web_master/snort/migrations/0002_snortruleviewarray.py
--rw-rw-rw-   0        0        0      610 2023-01-06 06:03:56.000000 snort_web_master-0.2.2.1/snort_web_master/snort/migrations/0003_snortruleviewarray_htmlid_and_more.py
--rw-rw-rw-   0        0        0      423 2023-01-06 13:23:29.000000 snort_web_master-0.2.2.1/snort_web_master/snort/migrations/0004_snortrule_deleted.py
--rw-rw-rw-   0        0        0      522 2023-01-08 17:24:52.000000 snort_web_master-0.2.2.1/snort_web_master/snort/migrations/0005_remove_snortrule_template_snortrule_is_template.py
--rw-rw-rw-   0        0        0      759 2023-02-21 08:33:21.000000 snort_web_master-0.2.2.1/snort_web_master/snort/migrations/0006_rename_main_ref_snortrule_document_and_more.py
--rw-rw-rw-   0        0        0      477 2023-04-19 09:28:30.000000 snort_web_master-0.2.2.1/snort_web_master/snort/migrations/0007_snortrule_tag.py
--rw-rw-rw-   0        0        0        0 2022-12-19 18:19:43.000000 snort_web_master-0.2.2.1/snort_web_master/snort/migrations/__init__.py
--rw-rw-rw-   0        0        0     2187 2023-04-19 09:28:26.000000 snort_web_master-0.2.2.1/snort_web_master/snort/models.py
--rw-rw-rw-   0        0        0    19362 2023-01-12 18:25:18.000000 snort_web_master-0.2.2.1/snort_web_master/snort/parser.py
--rw-rw-rw-   0        0        0     2271 2022-12-19 09:13:39.000000 snort_web_master-0.2.2.1/snort_web_master/snort/snort_templates.py
--rw-rw-rw-   0        0        0     4016 2023-02-21 08:27:30.000000 snort_web_master-0.2.2.1/snort_web_master/snort/tests.py
--rw-rw-rw-   0        0        0     5996 2023-05-10 05:29:35.000000 snort_web_master-0.2.2.1/snort_web_master/snort/views.py
-drwxrwxrwx   0        0        0        0 2023-05-10 06:37:52.980213 snort_web_master-0.2.2.1/snort_web_master/snort_web_master/
--rw-rw-rw-   0        0        0        0 2022-11-21 06:23:37.000000 snort_web_master-0.2.2.1/snort_web_master/snort_web_master/__init__.py
--rw-rw-rw-   0        0        0      425 2022-10-31 09:02:02.000000 snort_web_master-0.2.2.1/snort_web_master/snort_web_master/asgi.py
-drwxrwxrwx   0        0        0        0 2023-05-10 06:37:53.011461 snort_web_master-0.2.2.1/snort_web_master/snort_web_master/middleware/
--rw-rw-rw-   0        0        0        0 2023-01-09 07:35:12.000000 snort_web_master-0.2.2.1/snort_web_master/snort_web_master/middleware/__init__.py
--rw-rw-rw-   0        0        0      537 2023-01-09 14:10:56.000000 snort_web_master-0.2.2.1/snort_web_master/snort_web_master/middleware/no_cache.py
--rw-rw-rw-   0        0        0     5515 2023-05-02 07:51:40.000000 snort_web_master-0.2.2.1/snort_web_master/snort_web_master/settings.py
--rw-rw-rw-   0        0        0     1959 2023-04-19 08:14:20.000000 snort_web_master-0.2.2.1/snort_web_master/snort_web_master/urls.py
--rw-rw-rw-   0        0        0      425 2023-04-19 08:13:33.000000 snort_web_master-0.2.2.1/snort_web_master/snort_web_master/wsgi.py
-drwxrwxrwx   0        0        0        0 2023-05-10 06:37:53.011461 snort_web_master-0.2.2.1/snort_web_master/snort_web_master.egg-info/
--rw-rw-rw-   0        0        0      251 2023-05-10 06:37:52.000000 snort_web_master-0.2.2.1/snort_web_master/snort_web_master.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3038 2023-05-10 06:37:52.000000 snort_web_master-0.2.2.1/snort_web_master/snort_web_master.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 06:37:52.000000 snort_web_master-0.2.2.1/snort_web_master/snort_web_master.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      155 2023-05-10 06:37:52.000000 snort_web_master-0.2.2.1/snort_web_master/snort_web_master.egg-info/requires.txt
--rw-rw-rw-   0        0        0       38 2023-05-10 06:37:52.000000 snort_web_master-0.2.2.1/snort_web_master/snort_web_master.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-21 14:29:26.363937 snort_web_master-1.0.0.0/
+-rw-rw-rw-   0        0        0       54 2022-11-21 06:29:02.000000 snort_web_master-1.0.0.0/LICENSE.rst
+-rw-rw-rw-   0        0        0       24 2022-11-24 17:54:23.000000 snort_web_master-1.0.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      251 2023-06-21 14:29:26.363937 snort_web_master-1.0.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      716 2022-11-21 06:20:44.000000 snort_web_master-1.0.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-21 14:29:26.270184 snort_web_master-1.0.0.0/data/
+drwxrwxrwx   0        0        0        0 2023-06-21 14:29:26.270184 snort_web_master-1.0.0.0/data/admin/
+-rw-rw-rw-   0        0        0      698 2023-04-19 07:30:34.000000 snort_web_master-1.0.0.0/data/admin/0004_keyword_delete_keywords.py
+drwxrwxrwx   0        0        0        0 2023-06-21 14:29:26.270184 snort_web_master-1.0.0.0/data/admin/image/
+-rw-rw-rw-   0        0        0     7972 2023-01-16 16:49:34.000000 snort_web_master-1.0.0.0/data/admin/image/images.png
+-rw-rw-rw-   0        0        0   356352 2023-06-21 14:26:22.000000 snort_web_master-1.0.0.0/data/db.sqlite3
+-rw-rw-rw-   0        0        0    39363 2022-10-13 12:31:39.000000 snort_web_master-1.0.0.0/data/dicts.py
+-rw-rw-rw-   0        0        0      690 2023-01-23 09:10:03.000000 snort_web_master-1.0.0.0/data/dockercompose
+-rw-rw-rw-   0        0        0   139272 2023-01-16 16:50:11.000000 snort_web_master-1.0.0.0/data/favicon.ico
+-rw-rw-rw-   0        0        0    25803 2023-05-02 11:59:42.000000 snort_web_master-1.0.0.0/data/http.cap
+-rw-rw-rw-   0        0        0      898 2023-01-23 08:40:15.000000 snort_web_master-1.0.0.0/data/migrate sqllite to postgresql
+-rw-rw-rw-   0        0        0      402 2022-11-14 09:05:52.000000 snort_web_master-1.0.0.0/data/my-snort-rule.tmp
+drwxrwxrwx   0        0        0        0 2023-06-21 14:29:26.270184 snort_web_master-1.0.0.0/data/nginx/
+-rw-rw-rw-   0        0        0       96 2023-01-23 09:09:18.000000 snort_web_master-1.0.0.0/data/nginx/nginx
+-rw-rw-rw-   0        0        0      296 2023-01-23 09:04:00.000000 snort_web_master-1.0.0.0/data/nginx/nginx.conf
+-rw-rw-rw-   0        0        0      162 2023-01-23 08:44:15.000000 snort_web_master-1.0.0.0/data/requirements.txt
+-rw-rw-rw-   0        0        0      889 2023-05-02 14:51:31.000000 snort_web_master-1.0.0.0/data/snortFile
+drwxrwxrwx   0        0        0        0 2023-06-21 14:29:26.270184 snort_web_master-1.0.0.0/data/static/
+drwxrwxrwx   0        0        0        0 2023-06-21 14:29:26.223337 snort_web_master-1.0.0.0/data/static/admin/
+drwxrwxrwx   0        0        0        0 2023-06-21 14:29:26.270184 snort_web_master-1.0.0.0/data/static/admin/css/
+-rw-rw-rw-   0        0        0     1172 2023-06-21 13:46:42.000000 snort_web_master-1.0.0.0/data/static/admin/css/admin-styles.css
+-rw-rw-rw-   0        0        0    20344 2023-06-10 07:58:01.000000 snort_web_master-1.0.0.0/data/static/admin/css/base.css
+-rw-rw-rw-   0        0        0     9730 2023-06-10 07:59:05.000000 snort_web_master-1.0.0.0/data/static/admin/css/forms.css
+-rw-rw-rw-   0        0        0     2619 2023-06-10 07:58:10.000000 snort_web_master-1.0.0.0/data/static/admin/css/nav_sidebar.css
+drwxrwxrwx   0        0        0        0 2023-06-21 14:29:26.223337 snort_web_master-1.0.0.0/data/static/admin/css/vendor/
+drwxrwxrwx   0        0        0        0 2023-06-21 14:29:26.285809 snort_web_master-1.0.0.0/data/static/admin/css/vendor/select2/
+-rw-rw-rw-   0        0        0     1124 2022-12-26 08:06:54.000000 snort_web_master-1.0.0.0/data/static/admin/css/vendor/select2/LICENSE-SELECT2.md
+-rw-rw-rw-   0        0        0    17358 2022-12-26 08:06:54.000000 snort_web_master-1.0.0.0/data/static/admin/css/vendor/select2/select2.css
+-rw-rw-rw-   0        0        0    14966 2022-12-26 08:06:54.000000 snort_web_master-1.0.0.0/data/static/admin/css/vendor/select2/select2.min.css
+drwxrwxrwx   0        0        0        0 2023-06-21 14:29:26.285809 snort_web_master-1.0.0.0/data/static/admin/image/
+-rw-rw-rw-   0        0        0     7972 2023-01-16 16:49:34.000000 snort_web_master-1.0.0.0/data/static/admin/image/images.png
+drwxrwxrwx   0        0        0        0 2023-06-21 14:29:26.285809 snort_web_master-1.0.0.0/data/static/css/
+-rw-rw-rw-   0        0        0     1890 2023-06-14 17:15:26.000000 snort_web_master-1.0.0.0/data/static/css/main.55b651d4.css
+-rw-rw-rw-   0        0        0     3089 2023-06-14 17:15:26.000000 snort_web_master-1.0.0.0/data/static/css/main.55b651d4.css.map
+-rw-rw-rw-   0        0        0   139272 2023-01-16 16:50:11.000000 snort_web_master-1.0.0.0/data/static/favico.ico
+drwxrwxrwx   0        0        0        0 2023-06-21 14:29:26.285809 snort_web_master-1.0.0.0/data/static/js/
+-rw-rw-rw-   0        0        0     4591 2023-06-14 11:57:57.000000 snort_web_master-1.0.0.0/data/static/js/787.2c2ec360.chunk.js
+-rw-rw-rw-   0        0        0    10592 2023-06-14 11:57:57.000000 snort_web_master-1.0.0.0/data/static/js/787.2c2ec360.chunk.js.map
+-rw-rw-rw-   0        0        0   656292 2023-06-21 12:35:36.000000 snort_web_master-1.0.0.0/data/static/js/main.ad6031d4.js
+-rw-rw-rw-   0        0        0     1458 2023-06-21 12:35:36.000000 snort_web_master-1.0.0.0/data/static/js/main.ad6031d4.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  2485433 2023-06-21 12:35:36.000000 snort_web_master-1.0.0.0/data/static/js/main.ad6031d4.js.map
+drwxrwxrwx   0        0        0        0 2023-06-21 14:29:26.238937 snort_web_master-1.0.0.0/data/templates/
+drwxrwxrwx   0        0        0        0 2023-06-21 14:29:26.301434 snort_web_master-1.0.0.0/data/templates/html/
+-rw-rw-rw-   0        0        0      150 2023-06-21 12:36:15.000000 snort_web_master-1.0.0.0/data/templates/html/full_rule.html
+-rw-rw-rw-   0        0        0      420 2023-01-23 09:19:00.000000 snort_web_master-1.0.0.0/data/templates/html/import.html
+-rw-rw-rw-   0        0        0     3565 2023-06-14 12:05:15.000000 snort_web_master-1.0.0.0/data/templates/html/snortBuilder.html
+-rw-rw-rw-   0        0        0      140 2023-06-21 14:29:26.363937 snort_web_master-1.0.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      862 2023-06-21 14:29:21.000000 snort_web_master-1.0.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 14:29:26.238937 snort_web_master-1.0.0.0/snort_web_master/
+drwxrwxrwx   0        0        0        0 2023-06-21 14:29:26.301434 snort_web_master-1.0.0.0/snort_web_master/pcaps/
+-rw-rw-rw-   0        0        0        0 2022-10-31 09:04:45.000000 snort_web_master-1.0.0.0/snort_web_master/pcaps/__init__.py
+-rw-rw-rw-   0        0        0     2689 2023-01-08 17:50:03.000000 snort_web_master-1.0.0.0/snort_web_master/pcaps/admin.py
+-rw-rw-rw-   0        0        0      148 2022-10-31 09:04:45.000000 snort_web_master-1.0.0.0/snort_web_master/pcaps/apps.py
+drwxrwxrwx   0        0        0        0 2023-06-21 14:29:26.317061 snort_web_master-1.0.0.0/snort_web_master/pcaps/migrations/
+-rw-rw-rw-   0        0        0     1385 2022-12-19 18:20:00.000000 snort_web_master-1.0.0.0/snort_web_master/pcaps/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      813 2022-12-19 18:20:00.000000 snort_web_master-1.0.0.0/snort_web_master/pcaps/migrations/0002_initial.py
+-rw-rw-rw-   0        0        0      555 2022-12-19 18:24:58.000000 snort_web_master-1.0.0.0/snort_web_master/pcaps/migrations/0003_rename_rule_to_validate_pcap_rule_to_validate2_and_more.py
+-rw-rw-rw-   0        0        0      603 2022-12-19 18:25:24.000000 snort_web_master-1.0.0.0/snort_web_master/pcaps/migrations/0004_rename_rule_to_validate2_pcap_rule_to_validate_and_more.py
+-rw-rw-rw-   0        0        0        0 2022-12-19 18:19:43.000000 snort_web_master-1.0.0.0/snort_web_master/pcaps/migrations/__init__.py
+-rw-rw-rw-   0        0        0     1060 2022-12-19 18:25:20.000000 snort_web_master-1.0.0.0/snort_web_master/pcaps/models.py
+-rw-rw-rw-   0        0        0       63 2022-10-31 09:04:45.000000 snort_web_master-1.0.0.0/snort_web_master/pcaps/tests.py
+-rw-rw-rw-   0        0        0       66 2022-10-31 09:04:45.000000 snort_web_master-1.0.0.0/snort_web_master/pcaps/views.py
+drwxrwxrwx   0        0        0        0 2023-06-21 14:29:26.317061 snort_web_master-1.0.0.0/snort_web_master/settings/
+-rw-rw-rw-   0        0        0        0 2022-12-19 07:00:41.000000 snort_web_master-1.0.0.0/snort_web_master/settings/__init__.py
+-rw-rw-rw-   0        0        0      546 2023-04-19 09:25:30.000000 snort_web_master-1.0.0.0/snort_web_master/settings/admin.py
+-rw-rw-rw-   0        0        0      154 2022-12-19 07:00:41.000000 snort_web_master-1.0.0.0/snort_web_master/settings/apps.py
+drwxrwxrwx   0        0        0        0 2023-06-21 14:29:26.317061 snort_web_master-1.0.0.0/snort_web_master/settings/migrations/
+-rw-rw-rw-   0        0        0     1595 2022-12-19 18:20:00.000000 snort_web_master-1.0.0.0/snort_web_master/settings/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0     1350 2022-12-26 06:21:16.000000 snort_web_master-1.0.0.0/snort_web_master/settings/migrations/0002_remove_keywords_type_keywords_description_and_more.py
+-rw-rw-rw-   0        0        0      530 2022-12-26 06:23:11.000000 snort_web_master-1.0.0.0/snort_web_master/settings/migrations/0003_keywords_avalable.py
+-rw-rw-rw-   0        0        0      698 2023-04-19 07:30:34.000000 snort_web_master-1.0.0.0/snort_web_master/settings/migrations/0004_keyword_delete_keywords.py
+-rw-rw-rw-   0        0        0     1268 2023-04-19 09:28:30.000000 snort_web_master-1.0.0.0/snort_web_master/settings/migrations/0005_remove_keyword_negation_alter_keyword_description_and_more.py
+-rw-rw-rw-   0        0        0        0 2022-12-19 18:19:43.000000 snort_web_master-1.0.0.0/snort_web_master/settings/migrations/__init__.py
+-rw-rw-rw-   0        0        0     1476 2023-06-01 19:36:46.000000 snort_web_master-1.0.0.0/snort_web_master/settings/models.py
+-rw-rw-rw-   0        0        0       63 2022-12-19 07:00:41.000000 snort_web_master-1.0.0.0/snort_web_master/settings/tests.py
+-rw-rw-rw-   0        0        0       66 2022-12-19 07:00:41.000000 snort_web_master-1.0.0.0/snort_web_master/settings/views.py
+drwxrwxrwx   0        0        0        0 2023-06-21 14:29:26.332686 snort_web_master-1.0.0.0/snort_web_master/snort/
+-rw-rw-rw-   0        0        0        0 2022-10-31 09:04:41.000000 snort_web_master-1.0.0.0/snort_web_master/snort/__init__.py
+-rw-rw-rw-   0        0        0    32396 2023-06-21 12:54:36.000000 snort_web_master-1.0.0.0/snort_web_master/snort/admin.py
+-rw-rw-rw-   0        0        0      148 2022-10-31 09:04:41.000000 snort_web_master-1.0.0.0/snort_web_master/snort/apps.py
+drwxrwxrwx   0        0        0        0 2023-06-21 14:29:26.348312 snort_web_master-1.0.0.0/snort_web_master/snort/migrations/
+-rw-rw-rw-   0        0        0     1974 2022-12-19 18:20:00.000000 snort_web_master-1.0.0.0/snort_web_master/snort/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      870 2023-01-05 14:35:56.000000 snort_web_master-1.0.0.0/snort_web_master/snort/migrations/0002_snortruleviewarray.py
+-rw-rw-rw-   0        0        0      610 2023-01-06 06:03:56.000000 snort_web_master-1.0.0.0/snort_web_master/snort/migrations/0003_snortruleviewarray_htmlid_and_more.py
+-rw-rw-rw-   0        0        0      423 2023-01-06 13:23:29.000000 snort_web_master-1.0.0.0/snort_web_master/snort/migrations/0004_snortrule_deleted.py
+-rw-rw-rw-   0        0        0      522 2023-01-08 17:24:52.000000 snort_web_master-1.0.0.0/snort_web_master/snort/migrations/0005_remove_snortrule_template_snortrule_is_template.py
+-rw-rw-rw-   0        0        0      759 2023-02-21 08:33:21.000000 snort_web_master-1.0.0.0/snort_web_master/snort/migrations/0006_rename_main_ref_snortrule_document_and_more.py
+-rw-rw-rw-   0        0        0      477 2023-04-19 09:28:30.000000 snort_web_master-1.0.0.0/snort_web_master/snort/migrations/0007_snortrule_tag.py
+-rw-rw-rw-   0        0        0        0 2022-12-19 18:19:43.000000 snort_web_master-1.0.0.0/snort_web_master/snort/migrations/__init__.py
+-rw-rw-rw-   0        0        0     2187 2023-04-19 09:28:26.000000 snort_web_master-1.0.0.0/snort_web_master/snort/models.py
+-rw-rw-rw-   0        0        0    20381 2023-06-07 09:00:35.000000 snort_web_master-1.0.0.0/snort_web_master/snort/parser.py
+-rw-rw-rw-   0        0        0     2271 2022-12-19 09:13:39.000000 snort_web_master-1.0.0.0/snort_web_master/snort/snort_templates.py
+-rw-rw-rw-   0        0        0     4016 2023-02-21 08:27:30.000000 snort_web_master-1.0.0.0/snort_web_master/snort/tests.py
+-rw-rw-rw-   0        0        0    15563 2023-06-21 14:25:19.000000 snort_web_master-1.0.0.0/snort_web_master/snort/views.py
+drwxrwxrwx   0        0        0        0 2023-06-21 14:29:26.348312 snort_web_master-1.0.0.0/snort_web_master/snort_web_master/
+-rw-rw-rw-   0        0        0        0 2022-11-21 06:23:37.000000 snort_web_master-1.0.0.0/snort_web_master/snort_web_master/__init__.py
+-rw-rw-rw-   0        0        0      425 2022-10-31 09:02:02.000000 snort_web_master-1.0.0.0/snort_web_master/snort_web_master/asgi.py
+drwxrwxrwx   0        0        0        0 2023-06-21 14:29:26.363937 snort_web_master-1.0.0.0/snort_web_master/snort_web_master/middleware/
+-rw-rw-rw-   0        0        0        0 2023-01-09 07:35:12.000000 snort_web_master-1.0.0.0/snort_web_master/snort_web_master/middleware/__init__.py
+-rw-rw-rw-   0        0        0      733 2023-05-24 09:46:45.000000 snort_web_master-1.0.0.0/snort_web_master/snort_web_master/middleware/no_cache.py
+-rw-rw-rw-   0        0        0     5965 2023-06-10 07:48:30.000000 snort_web_master-1.0.0.0/snort_web_master/snort_web_master/settings.py
+-rw-rw-rw-   0        0        0     2413 2023-06-21 12:48:53.000000 snort_web_master-1.0.0.0/snort_web_master/snort_web_master/urls.py
+-rw-rw-rw-   0        0        0      425 2023-04-19 08:13:33.000000 snort_web_master-1.0.0.0/snort_web_master/snort_web_master/wsgi.py
+drwxrwxrwx   0        0        0        0 2023-06-21 14:29:26.363937 snort_web_master-1.0.0.0/snort_web_master/snort_web_master.egg-info/
+-rw-rw-rw-   0        0        0      251 2023-06-21 14:29:26.000000 snort_web_master-1.0.0.0/snort_web_master/snort_web_master.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3656 2023-06-21 14:29:26.000000 snort_web_master-1.0.0.0/snort_web_master/snort_web_master.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 14:29:26.000000 snort_web_master-1.0.0.0/snort_web_master/snort_web_master.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      155 2023-06-21 14:29:26.000000 snort_web_master-1.0.0.0/snort_web_master/snort_web_master.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       38 2023-06-21 14:29:26.000000 snort_web_master-1.0.0.0/snort_web_master/snort_web_master.egg-info/top_level.txt
```

### Comparing `snort_web_master-0.2.2.1/README.md` & `snort_web_master-1.0.0.0/README.md`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.1/data/admin/0004_keyword_delete_keywords.py` & `snort_web_master-1.0.0.0/data/admin/0004_keyword_delete_keywords.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.1/data/admin/image/images.png` & `snort_web_master-1.0.0.0/data/admin/image/images.png`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.1/data/dicts.py` & `snort_web_master-1.0.0.0/data/dicts.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.1/data/dockercompose` & `snort_web_master-1.0.0.0/data/dockercompose`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.1/data/favicon.ico` & `snort_web_master-1.0.0.0/data/favicon.ico`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.1/data/http.cap` & `snort_web_master-1.0.0.0/data/http.cap`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.1/data/migrate sqllite to postgresql` & `snort_web_master-1.0.0.0/data/migrate sqllite to postgresql`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.1/data/snortFile` & `snort_web_master-1.0.0.0/data/snortFile`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.1/setup.py` & `snort_web_master-1.0.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 from setuptools import setup, find_packages
 
 
 setup(
     name='snort_web_master',
-    version='0.2.2.1',
+    version='1.0.0.0',
     license='MoCorp',
     readme="README.md",
     author="meir dahan",
     author_email='1dahanmeir1@gmail.com',
     packages=find_packages('snort_web_master'),
     package_dir={'': 'snort_web_master'},
     url='https://github.com/mosheovadi1/snort-web-master',
```

### Comparing `snort_web_master-0.2.2.1/snort_web_master/pcaps/admin.py` & `snort_web_master-1.0.0.0/snort_web_master/pcaps/admin.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.1/snort_web_master/pcaps/migrations/0001_initial.py` & `snort_web_master-1.0.0.0/snort_web_master/pcaps/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.1/snort_web_master/pcaps/migrations/0002_initial.py` & `snort_web_master-1.0.0.0/snort_web_master/pcaps/migrations/0002_initial.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.1/snort_web_master/pcaps/migrations/0003_rename_rule_to_validate_pcap_rule_to_validate2_and_more.py` & `snort_web_master-1.0.0.0/snort_web_master/pcaps/migrations/0003_rename_rule_to_validate_pcap_rule_to_validate2_and_more.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.1/snort_web_master/pcaps/migrations/0004_rename_rule_to_validate2_pcap_rule_to_validate_and_more.py` & `snort_web_master-1.0.0.0/snort_web_master/pcaps/migrations/0004_rename_rule_to_validate2_pcap_rule_to_validate_and_more.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.1/snort_web_master/pcaps/models.py` & `snort_web_master-1.0.0.0/snort_web_master/pcaps/models.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.1/snort_web_master/settings/admin.py` & `snort_web_master-1.0.0.0/snort_web_master/settings/admin.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.1/snort_web_master/settings/migrations/0001_initial.py` & `snort_web_master-1.0.0.0/snort_web_master/settings/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.1/snort_web_master/settings/migrations/0002_remove_keywords_type_keywords_description_and_more.py` & `snort_web_master-1.0.0.0/snort_web_master/settings/migrations/0002_remove_keywords_type_keywords_description_and_more.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.1/snort_web_master/settings/migrations/0003_keywords_avalable.py` & `snort_web_master-1.0.0.0/snort_web_master/settings/migrations/0003_keywords_avalable.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.1/snort_web_master/settings/migrations/0004_keyword_delete_keywords.py` & `snort_web_master-1.0.0.0/snort_web_master/settings/migrations/0004_keyword_delete_keywords.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.1/snort_web_master/settings/migrations/0005_remove_keyword_negation_alter_keyword_description_and_more.py` & `snort_web_master-1.0.0.0/snort_web_master/settings/migrations/0005_remove_keyword_negation_alter_keyword_description_and_more.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.1/snort_web_master/settings/models.py` & `snort_web_master-1.0.0.0/snort_web_master/settings/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,9 +28,10 @@
     name = models.CharField(max_length=200, help_text="keyword name")
     stage = models.CharField(null=True, blank=True, max_length=100, help_text="where will the keyword element will appeare in snort builder")
     description = models.CharField(null=True, blank=True, max_length=100, help_text="just a description")
     options = models.CharField(null=True, blank=True, max_length=100,
                                 help_text="what type of field is it, does it has sub fields")
     available = models.BooleanField(default=False,
                                 help_text="is it available in snort builder")
+    objects = models.Manager()
     def __unicode__(self):
         return self.name
```

### Comparing `snort_web_master-0.2.2.1/snort_web_master/snort/admin.py` & `snort_web_master-1.0.0.0/snort_web_master/snort/admin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import copy
 import os
 import csv
 import time
 from io import StringIO
 from django.contrib import messages
 import re
+
+from django.core.exceptions import ValidationError
 from import_export.admin import ImportExportModelAdmin
 from django import forms
 
 import pcaps.models
 from .models import SnortRule, SnortRuleViewArray, save_rule_to_s3, delete_rule_from_s3
 from .snort_templates import types_list
 from .parser import Parser
@@ -26,15 +28,15 @@
 from django.shortcuts import render
 from pcaps.admin import verify_legal_pcap
 from advanced_filters.admin import AdminAdvancedFiltersMixin
 from django.core.files.storage import default_storage
 from django.core.files.base import ContentFile
 from django.conf import settings
 from datetime import datetime
-
+from django.core.serializers import serialize
 
 class StoreAdminForm(forms.ModelForm):
     ## add an extra field:
     upfile = forms.FileField()
 
     class Meta:
         model = SnortRule
@@ -55,15 +57,15 @@
 
 BASE_FIELDS = [
     "id", "active", "is_template", "deleted", "admin_locked", 'name', "document", "treatment", "description",
     "extra", "user"]
 FILTER_FIELDS = ("active", "is_template", "deleted", "admin_locked")
 ADVANCE_FILTER_FIELDS = tuple(i for i in BASE_FIELDS + ["content", ("pcap_sanity_check__name", "pcap_sanity_check_name"), ("pcap_legal_check__name", "pcap_legal_check_name"),("group_name", "group_name")])
 FIELDS = [
-    "id", "content", "active", "is_template", "deleted", "admin_locked", "tag",'name', "document", "treatment", "snort_builder", "description",
+    "id", "snort_builder", "active", "is_template", "deleted", "admin_locked",'name', "document", "treatment",  "description",
     "extra", "user", 'pcap_sanity_check', "pcap_legal_check"]
 SEARCH_FIELDS = tuple(i for i in BASE_FIELDS + ["content", "pcap_sanity_check__name", "pcap_legal_check__name", "group__name"])
 BASE_BUILDER_KEY = ("action", "protocol", "srcipallow", "srcip", "srcportallow", "srcport", "direction", "dstipallow",
                     "dstportallow", "dstport")
 
 INPUT_TYPE = ("srcip" , "srcport", "dstip", "dstport")
 from django.core.cache import cache
@@ -80,24 +82,25 @@
         if not dict(types_list).get(self.cleaned_data.get("type")):
             raise forms.ValidationError("cant find type, did you forgot it? or forgot to add type to db", code=404)
         return self.cleaned_data.get("type")
 
     def clean_content(self):
         try:
             parser = Parser(self.data["content"])
+            parser = Parser(self.data["content"])
             parser.parse_header()
             options = parser.parse_options()
             for option in options:
                 try:
-                    if keyword.objects.get(name=options[option][0]):
+                    if options[option][1] != [""] and options[option][0] != "tag":
                         break
                 except:
                     pass
             else:
-                raise Exception("no content; please add at least one keyword")
+                raise forms.ValidationError("no content; please add at least one keyword, tag does not count as one.")
             if os.name != "nt":
                 cur_rule = SnortRule()
                 cur_rule.content = self.data.get("content")
                 cur_rule.location = self.data.get("location")
                 cur_rule.group = self.instance.group
                 cur_rule.id = self.data.get("id")
                 cur_rule.treatment = self.data.get("treatment")
@@ -243,18 +246,39 @@
             if not self.current_user.is_staff and not self.current_user.is_superuser:
                 raise forms.ValidationError(
                     f"rule is admin locked, please contact admin", code=403)
         return self.cleaned_data["active"]
 
     @transaction.atomic
     def clean(self):
+        current_data = {}
+        for info, info_path in {"group": "group.name", "name": "name", "sigid": "id", "treatment": "treatment", "description":"description", "document":"document"}.items():
+            main = info_path.split(".")[0]
+            current_data[info] = self.cleaned_data.get(main, self.data.get(main, getattr(self.instance, main)))
+            for keypath in info_path.split(".")[1:]:
+                if current_data[info]:
+                    current_data[info] = getattr(current_data[info], keypath)
+                else:
+                    current_data[info] = ""
+
         if self.cleaned_data.get("content"):
             content = self.cleaned_data.get("content")
+            content = content[:-1] + f'msg:"{current_data["group"]}" "{current_data["name"]}"; sid:{current_data["sigid"]}; ' \
+                                     f'metadata: employee "{self.clean_user()}", group "{current_data["group"]}", ' \
+                                     f'name "{current_data["name"]}",treatment "{current_data["treatment"]}", keywords "None", ' \
+                                     f'date "{datetime.now().strftime("%d-%m-%Y %H:%M:%S")}", document "{current_data["document"]}",' \
+                                     f'description "{current_data["description"]}";)'
+
         elif self.data.get("content"):
             content = self.data.get("content")
+            content = content[:-1] + f'msg:"{current_data["group"]}" "{current_data["name"]}"; sid:{current_data["sigid"]}; ' \
+                                     f'metadata: employee "{self.clean_user()}", group "{current_data["group"]}", ' \
+                                     f'name "{current_data["name"]}",treatment "{current_data["treatment"]}", keywords "None", ' \
+                                     f'date "{datetime.now().strftime("%d-%m-%Y %H:%M:%S")}", document "{current_data["document"]}",' \
+                                     f'description "{current_data["description"]}";)'
         else:
             content = self.instance.content
         try:
             self.cleaned_data["user"] = self.instance.user = self.clean_user()
             regex = r"employee '\w+',"
             subst = rf"employee '{self.cleaned_data['user']}',"
             content = re.sub(regex, subst, content, 0, re.MULTILINE)
@@ -262,67 +286,33 @@
                 self.changed_data.append("user")
         except Exception as e:
             self.add_error("user", e)
         try:
             self.clean_content()
         except Exception as e:
             if not self.errors:
-                self.add_error("content", e)
+                raise ValidationError(e)
+
 
-        rule_keys = []
         self.instance.deleted = False
         if not self.instance.pk and not self.errors:
             self.instance.save()
             # set sid in content for the new rule
             if "sid:-;" in content:
                 self.cleaned_data["content"] = content.replace("sid:-;", f"sid:{self.instance.pk};")
                 if "content" not in self.changed_data:
                     self.changed_data.append("content")
         else:
             self.cleaned_data["content"] = content
         if not self.errors:
             SnortRuleViewArray.objects.filter(snortId=self.instance.id).delete()
-        for key, value in self.data.items():
-            if key in FIELDS + ['csrfmiddlewaretoken', "_save"]:
-                continue
-            item_type = "select"
-            location_x = 0
-            location_y = 0
-            if "keyword_selection" in key:
-                location_x = 0
-                try:
-                    index = key.index("-")
-                except:
-                    index = len(key)
-                location_y = int(key[len("keyword_selection"):index])
-            elif "keyword" in key:
-                try:
-                    index = key.index("-", key.index("-") + 1)
-                except:
-                    index = len(key)
-                if key[key.index("-") + 1:index] == "not":
-                    location_x = 0
-                    location_y = 0
-                else:
-                    location_x = int(key[key.index("-") + 1:index])
-                    location_y = int(key[len("keyword"):key.index("-")])
-            if "-data" in key or key in INPUT_TYPE:
-                item_type = "input"
-            rule_keys.append(SnortRuleViewArray(snortId=self.instance,
-                               typeOfItem=item_type,
-                               locationX=location_x,
-                               locationY=location_y,
-                               value=value,
-                               htmlId=key))
         if not self.errors:
-            cache.set(self.instance.id, rule_keys)
-            for key in rule_keys:
-                key.save()
+            cache.set(self.instance.id, content)
         else:
-            cache.set(self.instance.id, rule_keys)
+            cache.set(self.instance.id, content)
             return
         if self.cleaned_data.get("active"):
             save_rule_to_s3(self.instance.id, self.instance.content)
             pass
             # todo: save to s3
         else:
             delete_rule_from_s3(self.instance.id)
@@ -545,20 +535,15 @@
             messages.error(request, "cannot clone more than 1 rule at a time")
             return
         if len(queryset) == 0:
             messages.error(request, "need exactly 1 rule to clone")
             return
         for rule in queryset:
             self.request = request
-            self.request.session["cloned_rule"] = {"cloned_rule": True,
-                           "rule_conetnt": rule.content.replace('"', "'"),
-                           "rule_description": rule.description,
-                           "rule_name": rule.name,
-                           "rule_treatment": rule.treatment,
-                           "rule_document": rule.document}
+            request.session["instance"] = serialize('json', [rule])
         request.path = "/admin/snort/snortrule/add/"
         request.path_info = "/admin/snort/snortrule/add/"
         request.method = "GET"
         return self.changeform_view(request, object_id=None)
 
     @admin.action(description='export selected snort to csv')
     def make_published(self, request, queryset):
@@ -598,17 +583,18 @@
         set_rule = cache.get(obj.id)
         if not set_rule:
             set_rule = SnortRuleViewArray.objects.filter(snortId=obj.id)
             cache.set(obj.id, set_rule)
         else:
             cache.set(obj.id, [])
         context = {}
-        context["build_items"] = set_rule
-        context["actions"] = keyword.objects.filter(stage="action", available="True")
-        context["protocols"] = keyword.objects.filter(stage="protocol", available="True")
+        # todo handle caching of rule
+        # context["build_items"] = set_rule
+        # context["actions"] = keyword.objects.filter(stage="action", available="True")
+        # context["protocols"] = keyword.objects.filter(stage="protocol", available="True")
 
         tmp_context = copy.deepcopy(self.request.session.get("cloned_rule", {}))
         self.request.session["cloned_rule"] = {}
         tmp_context.update(context)
 
 
         snort_buider_section = render(self.request, "html/snortBuilder.html", tmp_context).content.decode("utf-8")
@@ -631,22 +617,25 @@
             a = Setting.objects.get_or_create(**{"name": "MIN_SANITY_MATCH_ALLOWED"}, defaults={"value": 0})
             a = Setting.objects.get_or_create(**{"name": "MAX_LEGAL_MATCH_ALLOWED"}, defaults={"value": 0})
             a = Setting.objects.get_or_create(**{"name": "MIN_LEGAL_MATCH_ALLOWED"}, defaults={"value": 0})
         return form
 
     @transaction.atomic
     def clone_rule(self, request, obj: SnortRule):
+        # todo: clone rule does not work from main page
+        # todo: clone rule does not work from rule page
+        request.session["instance"] = serialize('json', [obj])
         return HttpResponseRedirect(f"/snort/snortrule/add/")
 
     clone_rule.label = "clone_rule"  # optional
 
     def get_readonly_fields(self, request, obj=None):
         if obj and (obj.is_template or obj.admin_locked):
             read_only_fields = (
-            "id", "active", "user", "admin_locked", "snort_builder", "deleted", "rule_validation_section",)
+            "id", "snort_builder", "active", "user", "admin_locked", "deleted", "rule_validation_section",)
         else:
-            read_only_fields = ("id", "user", "admin_locked", "snort_builder", "deleted", "rule_validation_section")
+            read_only_fields = ("id", "snort_builder", "user", "admin_locked", "deleted", "rule_validation_section")
 
         return read_only_fields
 
     # readonly_fields = ("id", "user", "admin_locked", "full_rule", "snort_builder", "deleted")
     clone_rule.short_description = "clone rule to a new rule"  # optional
```

### Comparing `snort_web_master-0.2.2.1/snort_web_master/snort/migrations/0001_initial.py` & `snort_web_master-1.0.0.0/snort_web_master/snort/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.1/snort_web_master/snort/migrations/0002_snortruleviewarray.py` & `snort_web_master-1.0.0.0/snort_web_master/snort/migrations/0002_snortruleviewarray.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.1/snort_web_master/snort/migrations/0003_snortruleviewarray_htmlid_and_more.py` & `snort_web_master-1.0.0.0/snort_web_master/snort/migrations/0003_snortruleviewarray_htmlid_and_more.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.1/snort_web_master/snort/migrations/0005_remove_snortrule_template_snortrule_is_template.py` & `snort_web_master-1.0.0.0/snort_web_master/snort/migrations/0005_remove_snortrule_template_snortrule_is_template.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.1/snort_web_master/snort/migrations/0006_rename_main_ref_snortrule_document_and_more.py` & `snort_web_master-1.0.0.0/snort_web_master/snort/migrations/0006_rename_main_ref_snortrule_document_and_more.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.1/snort_web_master/snort/models.py` & `snort_web_master-1.0.0.0/snort_web_master/snort/models.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.1/snort_web_master/snort/parser.py` & `snort_web_master-1.0.0.0/snort_web_master/snort/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,39 @@
         if action in actions:
             return action
         else:
             msg = "Invalid action specified %s" % action
             raise ValueError(msg)
 
     @staticmethod
+    def services(service: str) -> str:
+        services = {
+            "ftp",
+            "http",
+            "imap",
+            "pop3",
+            "sip",
+            "smtp",
+            "ssh",
+            "dce_http_server",
+            "dce_http_proxy",
+            "dnp3",
+            "netflow",
+            "http2",
+            "telnet",
+            "rpc",
+            "modbus"
+        }
+
+        if service.lower() in services:
+            return service
+        else:
+            msg = "Unsupported Service %s " % service
+            raise ValueError(msg)
+    @staticmethod
     def proto(proto: str) -> str:
         protos = {
             "tcp",
             "udp",
             "icmp",
             "ip"
         }
@@ -355,59 +380,64 @@
             header = header.split()
         else:
             raise ValueError("Header is missing, or unparsable")
         # get rid of empty list elements
         header = list(filter(None, header))
         header_dict = collections.OrderedDict()
         size = len(header)
-        if not size == 7 and not size == 1:
+        if not size == 7 and not size == 1 and not size == 2:
             msg = "Snort rule header is malformed %s" % header
             raise ValueError(msg)
 
         for item in header:
-                if "action" not in header_dict:
-                    action = self.actions(item)
-                    header_dict["action"] = action
-                    continue
+            if "action" not in header_dict:
+                action = self.actions(item)
+                header_dict["action"] = action
+                continue
 
-                if "proto" not in header_dict:
+            if "proto" not in header_dict:
+                try:
+                    proto = self.proto(item)
+                    header_dict["proto"] = proto
+                    continue
+                except Exception as perror:
                     try:
-                        proto = self.proto(item)
-                        header_dict["proto"] = proto
+                        service = self.services(item)
+                        header_dict["service"] = service
                         continue
                     except Exception as perror:
                         raise ValueError(perror)
 
-                if "source" not in header_dict:
-                    try:
-                        src_ip = self.ip(item)
-                        header_dict["source"] = src_ip
-                        continue
-                    except Exception as serror:
-                        raise ValueError(serror)
-
-                if "src_port" not in header_dict:
-                    src_port = self.port(item)
-                    header_dict["src_port"] = src_port
+            if "source" not in header_dict:
+                try:
+                    src_ip = self.ip(item)
+                    header_dict["source"] = src_ip
                     continue
+                except Exception as serror:
+                    raise ValueError(serror)
 
-                if "arrow" not in header_dict:
-                    dst = self.destination(item)
-                    header_dict["arrow"] = dst
-                    continue
+            if "src_port" not in header_dict:
+                src_port = self.port(item)
+                header_dict["src_port"] = src_port
+                continue
 
-                if "destination" not in header_dict:
-                    dst_ip = self.ip(item)
-                    header_dict["destination"] = dst_ip
-                    continue
+            if "arrow" not in header_dict:
+                dst = self.destination(item)
+                header_dict["arrow"] = dst
+                continue
 
-                if "dst_port" not in header_dict:
-                    dst_port = self.port(item)
-                    header_dict["dst_port"] = dst_port
-                    continue
+            if "destination" not in header_dict:
+                dst_ip = self.ip(item)
+                header_dict["destination"] = dst_ip
+                continue
+
+            if "dst_port" not in header_dict:
+                dst_port = self.port(item)
+                header_dict["dst_port"] = dst_port
+                continue
 
         return header_dict
 
     def parse_options(self, rule=None):
         if rule:
             self.rule = rule
         opts = self.get_options()
@@ -551,15 +581,19 @@
             return item
 
         if isinstance(item, tuple):
             _bool, item = item
             if isinstance(item, list):
                 return self.__list_serializer(_bool, item)
             else:
-                return item
+                if _bool:
+                    serialised = "{}".format(item)
+                if not _bool:
+                    serialised = "!{}".format(item)
+                return serialised
 
     def serialize_header(self, header: Dict = None) -> str:
         serialised = str()
         if not header:
             header = self.rule['header']
         for key, value in header.items():
             item = self.serialize_header_item(value)
@@ -575,20 +609,22 @@
             if value:
                 option_value = "{}:{}".format(key, ",".join(value))
             else:
                 option_value = "{}".format(key)
             options_list.append(option_value)
 
         _options = '; '.join(str(e) for e in options_list)
-        serialized_options = '({})'.format(_options)
+        serialized_options = '({};)'.format(_options)
         return serialized_options
 
     def serialize_rule(self):
         return "{} {}".format(self.serialize_header(), self.serialize_options()).lstrip()
 
 
 if __name__ == '__main__':
     try:
-        rule = Parser("alert tcp 192.168.0.1 any -> $HOME_NET 21 (msg:”FTP connection attempt”; sid:1000002; rev:1;)")
+        # rule = Parser("alert tcp 192.168.0.1 any -> $HOME_NET 21 (msg:”FTP connection attempt”; sid:1000002; rev:1;)")
+        # print(rule.rule + " is OK")
+        rule = Parser("alert http (msg:”FTP connection attempt”; sid:1000002; rev:1;)")
         print(rule.rule + " is OK")
     except Exception as e:
         print(e)
```

### Comparing `snort_web_master-0.2.2.1/snort_web_master/snort/snort_templates.py` & `snort_web_master-1.0.0.0/snort_web_master/snort/snort_templates.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.1/snort_web_master/snort/tests.py` & `snort_web_master-1.0.0.0/snort_web_master/snort/tests.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.1/snort_web_master/snort_web_master/middleware/no_cache.py` & `snort_web_master-1.0.0.0/snort_web_master/snort_web_master/middleware/no_cache.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,14 +6,15 @@
         # One-time configuration and initialization.
 
     def __call__(self, request):
         # Code to be executed for each request before
         # the view (and later middleware) are called.
 
         response = self.get_response(request)
-
-
+        response.headers["Access-Control-Allow-Origin"] = "*"
+        response.headers["Access-Control-Allow-Headers"] = "*"
+        response.headers["Access-Control-Expose-Headers"] = "csrftoken"
         # Code to be executed for each request/response after
         # the view is called.
 
         return response
```

### Comparing `snort_web_master-0.2.2.1/snort_web_master/snort_web_master/settings.py` & `snort_web_master-1.0.0.0/snort_web_master/snort_web_master/settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 For the full list of settings and their values, see
 https://docs.djangoproject.com/en/4.1/ref/settings/
 """
 import os
 from pathlib import Path
 import mimetypes
 
+import corsheaders.middleware
+
 mimetypes.add_type("text/javascript", ".js", True)
 # Build paths inside the project like this: BASE_DIR / 'subdir'.
 BASE_DIR = Path(__file__).resolve().parent.parent
 
 
 # Quick-start development settings - unsuitable for production
 # See https://docs.djangoproject.com/en/4.1/howto/deployment/checklist/
@@ -24,24 +26,32 @@
 # SECURITY WARNING: keep the secret key used in production secret!
 SECRET_KEY = os.environ.get("SECRET_KEY", 'django-insecure-6imn8m6=okyge)ghoygg&rz3zzei45f5!5%#*mmy1e*ekj*cq5')
 
 # SECURITY WARNING: don't run with debug turned on in production!
 DEBUG = int(os.environ.get("DEBUG", default=1))
 
 ALLOWED_HOSTS = os.environ.get("DJANGO_ALLOWED_HOSTS", "").split("") if os.environ.get("DJANGO_ALLOWED_HOSTS", "") else ["*"]
-
+CORS_ALLOWED_ORIGINS = ["http://127.0.0.1:3000",
+                        "http://localhost:3000",]
+CORS_ALLOWED_HEADERS = ["x-CSRF-TOKEN"]
+# CORS_ALLOWED_ORIGIN_REGEXES = [".*"]
+CSRF_TRUSTED_ORIGINS = ["http://*127.0.0.1:3000",
+                        "http://*localhost:3000",]
+CORS_ORIGINS_ALLOW_ALL = True
+CORS_ALLOW_ALL_ORIGINS = True
 CACHES = {
     'default': {
         'BACKEND': 'django.core.cache.backends.locmem.LocMemCache',
         'LOCATION': 'unique-snowflake',
     }
 }
 # Application definition
 
 INSTALLED_APPS = [
+#     "corsheaders",
     'django.contrib.admin',
     'django.contrib.auth',
     'django.contrib.contenttypes',
     'django.contrib.sessions',
     'django.contrib.messages',
     'django.contrib.staticfiles',
     "snort_web_master",
@@ -53,20 +63,22 @@
     'import_export'
 
 ]
 IMPORT_EXPORT_USE_TRANSACTIONS = True
 MIDDLEWARE = [
     'django.middleware.security.SecurityMiddleware',
     'django.contrib.sessions.middleware.SessionMiddleware',
+#     "corsheaders.middleware.CorsMiddleware",
     'django.middleware.common.CommonMiddleware',
     'django.middleware.csrf.CsrfViewMiddleware',
     'django.contrib.auth.middleware.AuthenticationMiddleware',
     'django.contrib.messages.middleware.MessageMiddleware',
     'django.middleware.clickjacking.XFrameOptionsMiddleware',
     "snort_web_master.middleware.no_cache.NoCacheControl",
+
 ]
 
 ROOT_URLCONF = 'snort_web_master.urls'
 
 TEMPLATES = [
     {
         'BACKEND': 'django.template.backends.django.DjangoTemplates',
```

### Comparing `snort_web_master-0.2.2.1/snort_web_master/snort_web_master/urls.py` & `snort_web_master-1.0.0.0/snort_web_master/snort_web_master/urls.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,25 +12,34 @@
 Including another URLconf
     1. Import the include() function: from django.urls import include, path
     2. Add a URL to urlpatterns:  path('blog/', include('blog.urls'))
 """
 from django.contrib import admin
 from django.urls import path, include
 from django.shortcuts import redirect
-from snort.views import get_rule, get_rule_keys, build_rule_keyword_to_rule, build_rule_rule_to_keywords, favico,get_current_user_name
+from snort.views import get_rule, get_rule_keys, get,\
+    build_rule_parse,build_rule_serialize, \
+    build_rule_keyword_to_rule, build_rule_rule_to_keywords, \
+    favico,get_current_user_name
 from django.conf import settings
 from django.conf.urls.static import static
 import django.contrib.auth.admin
 django.contrib.auth.admin.UserAdmin.readonly_fields= ("last_login", 'date_joined')
 admin.site.site_header = 'snort web master'
 app_name = "snort_web_master"
 urlpatterns = [
     path("favicon.ico", favico),
     path("get_rule_update/<int:rule_id>/", get_rule, name="get_rule_update"),
+    path("get_rule_update/<str:cloned>/", get_rule, name="get_rule_update"),
+    path("get_rule_update//", get_rule, name="get_rule_update"),
     path("get_rule_keywords/<int:rule_id>/", get_rule_keys,name="get_rule_keywords"),
     path('advanced_filters/', include("advanced_filters.urls"), name="advance_filter"),
     path("build_rule/keyword_to_rule", build_rule_keyword_to_rule,name="build_rule"),
     path("build_rule/rule_to_keywords", build_rule_rule_to_keywords,name="build_keyword"),
+    path("build_rule_parse/", build_rule_parse, name="build_rule_parse"),
+    path("build_rule_serialize/", build_rule_serialize, name="build_rule_serialize"),
     path("current_user_name", get_current_user_name, name="get_current_user_name"),
+    path("get/<str:stage>/", get, name="get"),
+    path("get/", get, name="get"),
     path('admin/', admin.site.urls, name="admin_main"),
     path('',  admin.site.urls, name="admin_main"),
 ]+ static("static/", document_root=settings.STATIC_ROOT) + static("/", document_root=settings.BASE_DIR)
```

