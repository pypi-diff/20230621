# Comparing `tmp/garpix_company-2.8.3.tar.gz` & `tmp/garpix_company-2.9.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garpix_company-2.8.3.tar", last modified: Mon May 22 15:06:56 2023, max compression
+gzip compressed data, was "garpix_company-2.9.0rc1.tar", last modified: Wed Jun 21 15:56:40 2023, max compression
```

## Comparing `garpix_company-2.8.3.tar` & `garpix_company-2.9.0rc1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-22 15:06:56.139331 garpix_company-2.8.3/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       34 2023-05-22 15:06:56.000000 garpix_company-2.8.3/MANIFEST.in
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4078 2023-05-22 15:06:56.139170 garpix_company-2.8.3/PKG-INFO
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-22 15:06:56.131147 garpix_company-2.8.3/garpix_company/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2820 2023-05-22 15:06:42.000000 garpix_company-2.8.3/garpix_company/CHANGELOG.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1020 2022-10-21 09:53:17.000000 garpix_company-2.8.3/garpix_company/CONTRIBUTING.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       34 2022-10-21 09:53:17.000000 garpix_company-2.8.3/garpix_company/MANIFEST.in
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3508 2023-05-11 10:44:26.000000 garpix_company-2.8.3/garpix_company/README.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       63 2022-10-21 09:53:17.000000 garpix_company-2.8.3/garpix_company/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-22 15:06:56.134532 garpix_company-2.8.3/garpix_company/admin/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       83 2022-10-21 09:53:17.000000 garpix_company-2.8.3/garpix_company/admin/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      403 2023-05-11 10:08:25.000000 garpix_company-2.8.3/garpix_company/admin/company.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      235 2023-02-02 10:50:50.000000 garpix_company-2.8.3/garpix_company/admin/company_invite.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      137 2022-10-21 09:53:17.000000 garpix_company-2.8.3/garpix_company/apps.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      550 2022-10-21 09:53:17.000000 garpix_company-2.8.3/garpix_company/helpers.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-22 15:06:56.134926 garpix_company-2.8.3/garpix_company/managers/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-21 09:53:17.000000 garpix_company-2.8.3/garpix_company/managers/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      239 2022-10-21 09:53:17.000000 garpix_company-2.8.3/garpix_company/managers/company.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      254 2022-10-21 09:53:17.000000 garpix_company-2.8.3/garpix_company/managers/invite.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-22 15:06:56.135054 garpix_company-2.8.3/garpix_company/migrations/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-21 09:53:17.000000 garpix_company-2.8.3/garpix_company/migrations/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-22 15:06:56.135149 garpix_company-2.8.3/garpix_company/mixins/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-21 09:53:17.000000 garpix_company-2.8.3/garpix_company/mixins/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-22 15:06:56.135371 garpix_company-2.8.3/garpix_company/mixins/views/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       53 2022-10-21 09:53:17.000000 garpix_company-2.8.3/garpix_company/mixins/views/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      401 2023-02-02 07:19:24.000000 garpix_company-2.8.3/garpix_company/mixins/views/company_mixin.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-22 15:06:56.136132 garpix_company-2.8.3/garpix_company/models/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      209 2023-05-05 07:20:15.000000 garpix_company-2.8.3/garpix_company/models/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     6079 2023-05-11 09:19:51.000000 garpix_company-2.8.3/garpix_company/models/company.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4356 2023-05-04 14:33:02.000000 garpix_company-2.8.3/garpix_company/models/invite.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4133 2023-05-10 09:40:57.000000 garpix_company-2.8.3/garpix_company/models/user_company.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1943 2023-01-30 05:54:06.000000 garpix_company-2.8.3/garpix_company/models/user_role.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-22 15:06:56.136774 garpix_company-2.8.3/garpix_company/permissions/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      130 2023-02-10 15:45:53.000000 garpix_company-2.8.3/garpix_company/permissions/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1035 2023-05-04 14:33:02.000000 garpix_company-2.8.3/garpix_company/permissions/company_admin.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      706 2023-05-04 15:00:30.000000 garpix_company-2.8.3/garpix_company/permissions/company_owner.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      441 2023-02-10 15:45:53.000000 garpix_company-2.8.3/garpix_company/permissions/company_user.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      410 2023-05-11 10:44:26.000000 garpix_company-2.8.3/garpix_company/permissions/invite_receiver.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-22 15:06:56.137710 garpix_company-2.8.3/garpix_company/serializers/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      266 2023-01-30 05:54:06.000000 garpix_company-2.8.3/garpix_company/serializers/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3137 2023-05-04 14:33:02.000000 garpix_company-2.8.3/garpix_company/serializers/company.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5898 2023-05-22 15:06:07.000000 garpix_company-2.8.3/garpix_company/serializers/invite.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      277 2023-01-30 05:54:06.000000 garpix_company-2.8.3/garpix_company/serializers/role.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      235 2023-01-20 07:56:37.000000 garpix_company-2.8.3/garpix_company/serializers/user.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      926 2023-05-12 11:36:47.000000 garpix_company-2.8.3/garpix_company/serializers/user_company.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-22 15:06:56.137950 garpix_company-2.8.3/garpix_company/services/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-01-30 05:54:06.000000 garpix_company-2.8.3/garpix_company/services/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      607 2023-05-10 09:40:24.000000 garpix_company-2.8.3/garpix_company/services/role_service.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      580 2023-01-30 08:58:28.000000 garpix_company-2.8.3/garpix_company/settings.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1194 2023-05-22 15:06:42.000000 garpix_company-2.8.3/garpix_company/setup.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       68 2022-10-21 09:53:17.000000 garpix_company-2.8.3/garpix_company/tests.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      733 2023-02-10 15:45:53.000000 garpix_company-2.8.3/garpix_company/urls.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-22 15:06:56.138983 garpix_company-2.8.3/garpix_company/views/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      124 2023-01-19 14:51:26.000000 garpix_company-2.8.3/garpix_company/views/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     6000 2023-05-12 10:59:00.000000 garpix_company-2.8.3/garpix_company/views/company.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2201 2023-05-12 11:28:16.000000 garpix_company-2.8.3/garpix_company/views/invite.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3645 2023-05-12 10:46:57.000000 garpix_company-2.8.3/garpix_company/views/user_company.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-22 15:06:56.131929 garpix_company-2.8.3/garpix_company.egg-info/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4078 2023-05-22 15:06:56.000000 garpix_company-2.8.3/garpix_company.egg-info/PKG-INFO
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1721 2023-05-22 15:06:56.000000 garpix_company-2.8.3/garpix_company.egg-info/SOURCES.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-05-22 15:06:56.000000 garpix_company-2.8.3/garpix_company.egg-info/dependency_links.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-05-22 15:06:56.000000 garpix_company-2.8.3/garpix_company.egg-info/not-zip-safe
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       83 2023-05-22 15:06:56.000000 garpix_company-2.8.3/garpix_company.egg-info/requires.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       15 2023-05-22 15:06:56.000000 garpix_company-2.8.3/garpix_company.egg-info/top_level.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       38 2023-05-22 15:06:56.139375 garpix_company-2.8.3/setup.cfg
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1194 2023-05-22 15:06:56.000000 garpix_company-2.8.3/setup.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-21 15:56:40.989550 garpix_company-2.9.0rc1/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       34 2023-06-21 15:56:40.000000 garpix_company-2.9.0rc1/MANIFEST.in
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4081 2023-06-21 15:56:40.989424 garpix_company-2.9.0rc1/PKG-INFO
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-21 15:56:40.985323 garpix_company-2.9.0rc1/garpix_company/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2820 2023-05-22 15:06:42.000000 garpix_company-2.9.0rc1/garpix_company/CHANGELOG.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1020 2022-10-21 09:53:17.000000 garpix_company-2.9.0rc1/garpix_company/CONTRIBUTING.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       34 2022-10-21 09:53:17.000000 garpix_company-2.9.0rc1/garpix_company/MANIFEST.in
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3508 2023-05-11 10:44:26.000000 garpix_company-2.9.0rc1/garpix_company/README.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       63 2022-10-21 09:53:17.000000 garpix_company-2.9.0rc1/garpix_company/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-21 15:56:40.986281 garpix_company-2.9.0rc1/garpix_company/admin/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       83 2022-10-21 09:53:17.000000 garpix_company-2.9.0rc1/garpix_company/admin/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      403 2023-05-11 10:08:25.000000 garpix_company-2.9.0rc1/garpix_company/admin/company.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      235 2023-02-02 10:50:50.000000 garpix_company-2.9.0rc1/garpix_company/admin/company_invite.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      137 2022-10-21 09:53:17.000000 garpix_company-2.9.0rc1/garpix_company/apps.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      550 2022-10-21 09:53:17.000000 garpix_company-2.9.0rc1/garpix_company/helpers.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-21 15:56:40.986571 garpix_company-2.9.0rc1/garpix_company/managers/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-21 09:53:17.000000 garpix_company-2.9.0rc1/garpix_company/managers/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      239 2022-10-21 09:53:17.000000 garpix_company-2.9.0rc1/garpix_company/managers/company.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      254 2022-10-21 09:53:17.000000 garpix_company-2.9.0rc1/garpix_company/managers/invite.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-21 15:56:40.986681 garpix_company-2.9.0rc1/garpix_company/migrations/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-21 09:53:17.000000 garpix_company-2.9.0rc1/garpix_company/migrations/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-21 15:56:40.986773 garpix_company-2.9.0rc1/garpix_company/mixins/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-21 09:53:17.000000 garpix_company-2.9.0rc1/garpix_company/mixins/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-21 15:56:40.986961 garpix_company-2.9.0rc1/garpix_company/mixins/views/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       53 2022-10-21 09:53:17.000000 garpix_company-2.9.0rc1/garpix_company/mixins/views/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      401 2023-02-02 07:19:24.000000 garpix_company-2.9.0rc1/garpix_company/mixins/views/company_mixin.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-21 15:56:40.987492 garpix_company-2.9.0rc1/garpix_company/models/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      222 2023-06-21 15:54:39.000000 garpix_company-2.9.0rc1/garpix_company/models/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     6252 2023-06-21 15:49:16.000000 garpix_company-2.9.0rc1/garpix_company/models/company.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4356 2023-05-04 14:33:02.000000 garpix_company-2.9.0rc1/garpix_company/models/invite.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4539 2023-06-21 15:54:04.000000 garpix_company-2.9.0rc1/garpix_company/models/user_company.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1943 2023-01-30 05:54:06.000000 garpix_company-2.9.0rc1/garpix_company/models/user_role.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-21 15:56:40.988029 garpix_company-2.9.0rc1/garpix_company/permissions/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      130 2023-02-10 15:45:53.000000 garpix_company-2.9.0rc1/garpix_company/permissions/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1069 2023-06-21 15:51:24.000000 garpix_company-2.9.0rc1/garpix_company/permissions/company_admin.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      706 2023-05-04 15:00:30.000000 garpix_company-2.9.0rc1/garpix_company/permissions/company_owner.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      545 2023-06-21 15:50:30.000000 garpix_company-2.9.0rc1/garpix_company/permissions/company_user.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      410 2023-05-11 10:44:26.000000 garpix_company-2.9.0rc1/garpix_company/permissions/invite_receiver.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-21 15:56:40.988663 garpix_company-2.9.0rc1/garpix_company/serializers/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      266 2023-01-30 05:54:06.000000 garpix_company-2.9.0rc1/garpix_company/serializers/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3137 2023-05-04 14:33:02.000000 garpix_company-2.9.0rc1/garpix_company/serializers/company.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5898 2023-05-22 15:06:07.000000 garpix_company-2.9.0rc1/garpix_company/serializers/invite.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      277 2023-01-30 05:54:06.000000 garpix_company-2.9.0rc1/garpix_company/serializers/role.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      235 2023-01-20 07:56:37.000000 garpix_company-2.9.0rc1/garpix_company/serializers/user.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      926 2023-05-12 11:36:47.000000 garpix_company-2.9.0rc1/garpix_company/serializers/user_company.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-21 15:56:40.988859 garpix_company-2.9.0rc1/garpix_company/services/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-01-30 05:54:06.000000 garpix_company-2.9.0rc1/garpix_company/services/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      607 2023-05-10 09:40:24.000000 garpix_company-2.9.0rc1/garpix_company/services/role_service.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      580 2023-01-30 08:58:28.000000 garpix_company-2.9.0rc1/garpix_company/settings.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1198 2023-06-21 15:46:46.000000 garpix_company-2.9.0rc1/garpix_company/setup.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       68 2022-10-21 09:53:17.000000 garpix_company-2.9.0rc1/garpix_company/tests.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      733 2023-02-10 15:45:53.000000 garpix_company-2.9.0rc1/garpix_company/urls.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-21 15:56:40.989266 garpix_company-2.9.0rc1/garpix_company/views/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      124 2023-01-19 14:51:26.000000 garpix_company-2.9.0rc1/garpix_company/views/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     6000 2023-05-12 10:59:00.000000 garpix_company-2.9.0rc1/garpix_company/views/company.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2201 2023-05-12 11:28:16.000000 garpix_company-2.9.0rc1/garpix_company/views/invite.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3645 2023-05-12 10:46:57.000000 garpix_company-2.9.0rc1/garpix_company/views/user_company.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-21 15:56:40.985955 garpix_company-2.9.0rc1/garpix_company.egg-info/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4081 2023-06-21 15:56:40.000000 garpix_company-2.9.0rc1/garpix_company.egg-info/PKG-INFO
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1721 2023-06-21 15:56:40.000000 garpix_company-2.9.0rc1/garpix_company.egg-info/SOURCES.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-06-21 15:56:40.000000 garpix_company-2.9.0rc1/garpix_company.egg-info/dependency_links.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-06-21 15:56:40.000000 garpix_company-2.9.0rc1/garpix_company.egg-info/not-zip-safe
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       83 2023-06-21 15:56:40.000000 garpix_company-2.9.0rc1/garpix_company.egg-info/requires.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       15 2023-06-21 15:56:40.000000 garpix_company-2.9.0rc1/garpix_company.egg-info/top_level.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       38 2023-06-21 15:56:40.989584 garpix_company-2.9.0rc1/setup.cfg
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1198 2023-06-21 15:56:40.000000 garpix_company-2.9.0rc1/setup.py
```

### Comparing `garpix_company-2.8.3/PKG-INFO` & `garpix_company-2.9.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garpix_company
-Version: 2.8.3
+Version: 2.9.0rc1
 Home-page: https://github.com/garpixcms/garpix_company
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `garpix_company-2.8.3/garpix_company/CHANGELOG.md` & `garpix_company-2.9.0rc1/garpix_company/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `garpix_company-2.8.3/garpix_company/CONTRIBUTING.md` & `garpix_company-2.9.0rc1/garpix_company/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `garpix_company-2.8.3/garpix_company/README.md` & `garpix_company-2.9.0rc1/garpix_company/README.md`

 * *Files identical despite different names*

### Comparing `garpix_company-2.8.3/garpix_company/helpers.py` & `garpix_company-2.9.0rc1/garpix_company/helpers.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.8.3/garpix_company/models/company.py` & `garpix_company-2.9.0rc1/garpix_company/models/company.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,23 +20,23 @@
     Данные о компании.
     """
 
     COMPANY_STATUS = COMPANY_STATUS_ENUM
 
     title = models.CharField(max_length=255, verbose_name=_('Название'))
     full_title = models.CharField(max_length=255, verbose_name=_('Полное название'))
-    inn = models.CharField(max_length=15, verbose_name=_('ИНН'))
+    inn = models.CharField(max_length=15, null=True, blank=True, verbose_name=_('ИНН'))
     ogrn = models.CharField(max_length=15, null=True, blank=True, verbose_name=_('ОГРН'))
     kpp = models.CharField(max_length=50, null=True, blank=True, verbose_name=_("КПП"))
     bank_title = models.CharField(max_length=100, null=True, blank=True, verbose_name=_("Наименование банка"))
     bic = models.CharField(max_length=100, null=True, blank=True, verbose_name=_("БИК банка"))
     schet = models.CharField(max_length=50, null=True, blank=True, verbose_name=_("Номер счета"))
     korschet = models.CharField(max_length=50, null=True, blank=True, verbose_name=_("Кор. счет"))
-    ur_address = models.CharField(max_length=300, verbose_name=_("Юридический адрес"))
-    fact_address = models.CharField(max_length=300, verbose_name=_("Фактический адрес"))
+    ur_address = models.CharField(max_length=300, null=True, blank=True, verbose_name=_("Юридический адрес"))
+    fact_address = models.CharField(max_length=300, null=True, blank=True, verbose_name=_("Фактический адрес"))
     status = FSMField(default=COMPANY_STATUS.ACTIVE, choices=COMPANY_STATUS.CHOICES, verbose_name=_('Статус'))
     participants = models.ManyToManyField(User, through=settings.GARPIX_USER_COMPANY_MODEL,
                                           verbose_name=_('Участники компании'))
     created_at = models.DateTimeField(auto_now_add=True, verbose_name=_('Дата создания'))
     updated_at = models.DateTimeField(auto_now=True, verbose_name=_('Дата изменения'))
     objects = models.Manager()
     active_objects = CompanyActiveManager()
@@ -116,16 +116,18 @@
 
     @classmethod
     def invite_confirmation_link(cls, token):
         return f'{settings.SITE_URL}invite/{token}'
 
     @property
     def owner(self):
+        UserCompany = get_user_company_model()
         company_role_service = UserCompanyRoleService()
-        user_model_instance = self.user_companies.filter(role=company_role_service.get_owner_role()).first()
+        user_model_instance = UserCompany.active_objects.select_related('user').filter(
+            role=company_role_service.get_owner_role(), company=self).first()
         if user_model_instance:
             return user_model_instance.user
         return None
 
 
 def get_company_model():
     """
```

### Comparing `garpix_company-2.8.3/garpix_company/models/invite.py` & `garpix_company-2.9.0rc1/garpix_company/models/invite.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.8.3/garpix_company/models/user_company.py` & `garpix_company-2.9.0rc1/garpix_company/models/user_company.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,16 +16,16 @@
         return super().get_queryset().filter(is_blocked=False)
 
 
 class AbstractUserCompany(models.Model):
     """
     Модель участников. Связка между компанией и пользователем.
     """
-    user = models.ForeignKey(User, on_delete=models.CASCADE, related_name='user_companies', verbose_name=_('Пользователь'))
-    company = models.ForeignKey(settings.GARPIX_COMPANY_MODEL, related_name='user_companies', on_delete=models.CASCADE)
+    user = models.ForeignKey(User, on_delete=models.CASCADE, verbose_name=_('Пользователь'))
+    company = models.ForeignKey(settings.GARPIX_COMPANY_MODEL, on_delete=models.CASCADE)
     created_at = models.DateTimeField(auto_now_add=True, verbose_name=_("Дата/время создания"))
     is_blocked = models.BooleanField(default=False, verbose_name=_("Заблокирован администратором компании"))
     role = models.ForeignKey(settings.GARPIX_COMPANY_ROLE_MODEL, null=True, blank=True, on_delete=models.SET_NULL,
                              verbose_name=_('Роль в компании'))
 
     objects = Manager()
     active_objects = ActiveManager()
@@ -77,18 +77,21 @@
         if role == company_role_service.get_owner_role():
             return False, _('Нельзя сделать пользователя владельцем. Воспользуйтесь функционалом смены владельца')
         if role == company_role_service.get_admin_role() and self.is_blocked:
             return False, _('Нельзя сделать администратором заблокированного пользователя')
         self.role = role
         self.save()
         return True, None
-#
-#
-# class UserCompany(AbstractUserCompany):
-#     pass
+
+
+class UserCompany(AbstractUserCompany):
+    user = models.ForeignKey(User, on_delete=models.CASCADE, related_name='user_companies', verbose_name=_('Пользователь'))
+    company = models.ForeignKey(settings.GARPIX_COMPANY_MODEL, related_name='user_companies', on_delete=models.CASCADE)
+    role = models.ForeignKey(settings.GARPIX_COMPANY_ROLE_MODEL, null=True, blank=True, on_delete=models.SET_NULL,
+                             related_name='user_company_roles', verbose_name=_('Роль в компании'))
 
 
 def get_user_company_model():
     """
     Return the UserCompany model that is active in this project.
     """
     try:
```

### Comparing `garpix_company-2.8.3/garpix_company/models/user_role.py` & `garpix_company-2.9.0rc1/garpix_company/models/user_role.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.8.3/garpix_company/permissions/company_admin.py` & `garpix_company-2.9.0rc1/garpix_company/permissions/company_admin.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,13 +12,13 @@
     Доступ только для администратора компании
     """
 
     def has_object_permission(self, request, view, obj):
         company_role_service = UserCompanyRoleService()
 
         if isinstance(obj, Company):
-            return request.user.is_authenticated and request.user.id in obj.user_companies.filter(
-                role=company_role_service.get_admin_role()).values_list('user', flat=True)
+            return request.user.is_authenticated and request.user.id in UserCompany.active_objects.filter(
+                role=company_role_service.get_admin_role(), company=obj).values_list('user', flat=True)
         if isinstance(obj, InviteToCompany) or isinstance(obj, UserCompany):
-            return request.user.is_authenticated and obj.company.user_companies.filter(
-                role=company_role_service.get_admin_role(), user=request.user)
+            return request.user.is_authenticated and UserCompany.active_objects.filter(
+                role=company_role_service.get_admin_role(), user=request.user, company=obj)
         return False
```

### Comparing `garpix_company-2.8.3/garpix_company/permissions/company_owner.py` & `garpix_company-2.9.0rc1/garpix_company/permissions/company_owner.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.8.3/garpix_company/serializers/company.py` & `garpix_company-2.9.0rc1/garpix_company/serializers/company.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.8.3/garpix_company/serializers/invite.py` & `garpix_company-2.9.0rc1/garpix_company/serializers/invite.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.8.3/garpix_company/serializers/user_company.py` & `garpix_company-2.9.0rc1/garpix_company/serializers/user_company.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.8.3/garpix_company/services/role_service.py` & `garpix_company-2.9.0rc1/garpix_company/services/role_service.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.8.3/garpix_company/settings.py` & `garpix_company-2.9.0rc1/garpix_company/settings.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.8.3/garpix_company/setup.py` & `garpix_company-2.9.0rc1/garpix_company/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = path.join(path.abspath(path.dirname(__file__)), 'garpix_company')
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='garpix_company',
-    version='2.8.3',
+    version='2.9.0-rc1',
     description='',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/garpixcms/garpix_company',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
```

### Comparing `garpix_company-2.8.3/garpix_company/urls.py` & `garpix_company-2.9.0rc1/garpix_company/urls.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.8.3/garpix_company/views/company.py` & `garpix_company-2.9.0rc1/garpix_company/views/company.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.8.3/garpix_company/views/invite.py` & `garpix_company-2.9.0rc1/garpix_company/views/invite.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.8.3/garpix_company/views/user_company.py` & `garpix_company-2.9.0rc1/garpix_company/views/user_company.py`

 * *Files identical despite different names*

### Comparing `garpix_company-2.8.3/garpix_company.egg-info/PKG-INFO` & `garpix_company-2.9.0rc1/garpix_company.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garpix-company
-Version: 2.8.3
+Version: 2.9.0rc1
 Home-page: https://github.com/garpixcms/garpix_company
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `garpix_company-2.8.3/garpix_company.egg-info/SOURCES.txt` & `garpix_company-2.9.0rc1/garpix_company.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `garpix_company-2.8.3/setup.py` & `garpix_company-2.9.0rc1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = path.join(path.abspath(path.dirname(__file__)), 'garpix_company')
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='garpix_company',
-    version='2.8.3',
+    version='2.9.0-rc1',
     description='',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/garpixcms/garpix_company',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
```

