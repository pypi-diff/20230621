# Comparing `tmp/django-ipghrms-users-1.0.tar.gz` & `tmp/django-ipghrms-users-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-ipghrms-users-1.0.tar", last modified: Mon Mar 27 15:23:30 2023, max compression
+gzip compressed data, was "django-ipghrms-users-1.1.tar", last modified: Wed Jun 21 01:29:45 2023, max compression
```

## Comparing `django-ipghrms-users-1.0.tar` & `django-ipghrms-users-1.1.tar`

### file list

```diff
@@ -1,49 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-03-27 15:23:30.237744 django-ipghrms-users-1.0/
--rw-rw-rw-   0        0        0     1065 2023-03-27 15:21:57.000000 django-ipghrms-users-1.0/LICENSE
--rw-rw-rw-   0        0        0      105 2023-03-27 14:32:55.000000 django-ipghrms-users-1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      924 2023-03-27 15:23:30.237744 django-ipghrms-users-1.0/PKG-INFO
--rw-rw-rw-   0        0        0      482 2023-03-27 14:33:01.000000 django-ipghrms-users-1.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-27 15:23:30.160680 django-ipghrms-users-1.0/django_ipghrms_users.egg-info/
--rw-rw-rw-   0        0        0      924 2023-03-27 15:23:30.000000 django-ipghrms-users-1.0/django_ipghrms_users.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1276 2023-03-27 15:23:30.000000 django-ipghrms-users-1.0/django_ipghrms_users.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-27 15:23:30.000000 django-ipghrms-users-1.0/django_ipghrms_users.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-03-27 15:23:30.000000 django-ipghrms-users-1.0/django_ipghrms_users.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      505 2023-03-27 15:23:30.240529 django-ipghrms-users-1.0/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-03-22 07:44:49.000000 django-ipghrms-users-1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-27 15:23:30.185140 django-ipghrms-users-1.0/users/
--rw-rw-rw-   0        0        0        0 2022-10-18 10:39:31.000000 django-ipghrms-users-1.0/users/__init__.py
--rw-rw-rw-   0        0        0      344 2023-01-18 00:19:37.000000 django-ipghrms-users-1.0/users/account_urls.py
--rw-rw-rw-   0        0        0       63 2022-10-18 10:39:31.000000 django-ipghrms-users-1.0/users/admin.py
--rw-rw-rw-   0        0        0      142 2022-10-18 10:39:31.000000 django-ipghrms-users-1.0/users/apps.py
--rw-rw-rw-   0        0        0      663 2023-03-07 10:27:46.000000 django-ipghrms-users-1.0/users/context_processors.py
--rw-rw-rw-   0        0        0     1370 2022-10-18 10:39:31.000000 django-ipghrms-users-1.0/users/forms.py
--rw-rw-rw-   0        0        0       57 2022-10-18 10:39:31.000000 django-ipghrms-users-1.0/users/models.py
--rw-rw-rw-   0        0        0      139 2023-01-18 00:18:15.000000 django-ipghrms-users-1.0/users/profile_urls.py
-drwxrwxrwx   0        0        0        0 2023-03-27 15:23:30.128775 django-ipghrms-users-1.0/users/templates/
-drwxrwxrwx   0        0        0        0 2023-03-27 15:23:30.201847 django-ipghrms-users-1.0/users/templates/auth/
--rw-rw-rw-   0        0        0     1336 2023-02-21 06:04:32.000000 django-ipghrms-users-1.0/users/templates/auth/account.html
--rw-rw-rw-   0        0        0     1101 2022-10-18 10:39:31.000000 django-ipghrms-users-1.0/users/templates/auth/change_password.html
--rw-rw-rw-   0        0        0      506 2022-10-18 10:39:31.000000 django-ipghrms-users-1.0/users/templates/auth/change_password_done.html
--rw-rw-rw-   0        0        0     1023 2022-10-18 10:39:31.000000 django-ipghrms-users-1.0/users/templates/auth/password_reset.html
--rw-rw-rw-   0        0        0      594 2022-10-18 10:39:31.000000 django-ipghrms-users-1.0/users/templates/auth/password_reset_complete.html
--rw-rw-rw-   0        0        0      747 2022-10-18 10:39:31.000000 django-ipghrms-users-1.0/users/templates/auth/password_reset_confirm.html
--rw-rw-rw-   0        0        0      780 2022-10-18 10:39:31.000000 django-ipghrms-users-1.0/users/templates/auth/password_reset_done.html
-drwxrwxrwx   0        0        0        0 2023-03-27 15:23:30.213601 django-ipghrms-users-1.0/users/templates/profile/
--rw-rw-rw-   0        0        0     2588 2023-02-10 02:57:39.000000 django-ipghrms-users-1.0/users/templates/profile/profile.html
--rw-rw-rw-   0        0        0     2168 2023-03-15 14:43:16.000000 django-ipghrms-users-1.0/users/templates/profile/profile_bottom.html
--rw-rw-rw-   0        0        0     4357 2023-03-15 14:39:29.000000 django-ipghrms-users-1.0/users/templates/profile/profile_left.html
--rw-rw-rw-   0        0        0     2209 2023-03-15 14:51:46.000000 django-ipghrms-users-1.0/users/templates/profile/profile_right.html
--rw-rw-rw-   0        0        0       60 2022-10-18 10:39:31.000000 django-ipghrms-users-1.0/users/tests.py
--rw-rw-rw-   0        0        0        0 2023-01-18 00:19:34.000000 django-ipghrms-users-1.0/users/urls.py
-drwxrwxrwx   0        0        0        0 2023-03-27 15:23:30.219035 django-ipghrms-users-1.0/users/views/
--rw-rw-rw-   0        0        0       22 2022-11-30 04:35:46.000000 django-ipghrms-users-1.0/users/views/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-27 15:23:30.235707 django-ipghrms-users-1.0/users/views/__pycache__/
--rw-rw-rw-   0        0        0      162 2022-11-30 07:30:55.000000 django-ipghrms-users-1.0/users/views/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      138 2022-10-20 01:02:07.000000 django-ipghrms-users-1.0/users/views/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0      167 2022-10-18 10:39:31.000000 django-ipghrms-users-1.0/users/views/__pycache__/__init__.cpython-38.pyc
--rw-rw-rw-   0        0        0      146 2022-10-18 10:39:31.000000 django-ipghrms-users-1.0/users/views/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     3798 2023-03-15 14:41:25.000000 django-ipghrms-users-1.0/users/views/__pycache__/profile.cpython-310.pyc
--rw-rw-rw-   0        0        0     3580 2022-10-18 10:39:31.000000 django-ipghrms-users-1.0/users/views/__pycache__/profile.cpython-38.pyc
--rw-rw-rw-   0        0        0     3549 2022-10-18 10:39:31.000000 django-ipghrms-users-1.0/users/views/__pycache__/profile.cpython-39.pyc
--rw-rw-rw-   0        0        0     4014 2023-03-15 14:41:22.000000 django-ipghrms-users-1.0/users/views/profile.py
--rw-rw-rw-   0        0        0       63 2022-10-18 10:39:31.000000 django-ipghrms-users-1.0/users/views.py
+drwxrwxrwx   0        0        0        0 2023-06-21 01:29:45.708897 django-ipghrms-users-1.1/
+-rw-rw-rw-   0        0        0     1065 2023-03-27 15:21:57.000000 django-ipghrms-users-1.1/LICENSE
+-rw-rw-rw-   0        0        0      105 2023-03-27 14:32:55.000000 django-ipghrms-users-1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      924 2023-06-21 01:29:45.710393 django-ipghrms-users-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      482 2023-03-27 14:33:01.000000 django-ipghrms-users-1.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-21 01:29:45.438985 django-ipghrms-users-1.1/django_ipghrms_users.egg-info/
+-rw-rw-rw-   0        0        0      924 2023-06-21 01:29:45.000000 django-ipghrms-users-1.1/django_ipghrms_users.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1465 2023-06-21 01:29:45.000000 django-ipghrms-users-1.1/django_ipghrms_users.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 01:29:45.000000 django-ipghrms-users-1.1/django_ipghrms_users.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-21 01:29:45.000000 django-ipghrms-users-1.1/django_ipghrms_users.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      505 2023-06-21 01:29:45.717963 django-ipghrms-users-1.1/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-03-22 07:44:49.000000 django-ipghrms-users-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 01:29:45.470608 django-ipghrms-users-1.1/users/
+-rw-rw-rw-   0        0        0        0 2022-10-18 10:39:31.000000 django-ipghrms-users-1.1/users/__init__.py
+-rw-rw-rw-   0        0        0      344 2023-01-18 00:19:37.000000 django-ipghrms-users-1.1/users/account_urls.py
+-rw-rw-rw-   0        0        0       63 2022-10-18 10:39:31.000000 django-ipghrms-users-1.1/users/admin.py
+-rw-rw-rw-   0        0        0      142 2022-10-18 10:39:31.000000 django-ipghrms-users-1.1/users/apps.py
+-rw-rw-rw-   0        0        0      663 2023-03-07 10:27:46.000000 django-ipghrms-users-1.1/users/context_processors.py
+-rw-rw-rw-   0        0        0     1370 2022-10-18 10:39:31.000000 django-ipghrms-users-1.1/users/forms.py
+-rw-rw-rw-   0        0        0       57 2022-10-18 10:39:31.000000 django-ipghrms-users-1.1/users/models.py
+-rw-rw-rw-   0        0        0     1055 2023-06-20 15:09:44.000000 django-ipghrms-users-1.1/users/profile_urls.py
+drwxrwxrwx   0        0        0        0 2023-06-21 01:29:45.395241 django-ipghrms-users-1.1/users/templates/
+drwxrwxrwx   0        0        0        0 2023-06-21 01:29:45.585755 django-ipghrms-users-1.1/users/templates/auth/
+-rw-rw-rw-   0        0        0     1336 2023-02-21 06:04:32.000000 django-ipghrms-users-1.1/users/templates/auth/account.html
+-rw-rw-rw-   0        0        0     1101 2022-10-18 10:39:31.000000 django-ipghrms-users-1.1/users/templates/auth/change_password.html
+-rw-rw-rw-   0        0        0      506 2022-10-18 10:39:31.000000 django-ipghrms-users-1.1/users/templates/auth/change_password_done.html
+-rw-rw-rw-   0        0        0     1023 2022-10-18 10:39:31.000000 django-ipghrms-users-1.1/users/templates/auth/password_reset.html
+-rw-rw-rw-   0        0        0      594 2022-10-18 10:39:31.000000 django-ipghrms-users-1.1/users/templates/auth/password_reset_complete.html
+-rw-rw-rw-   0        0        0      747 2022-10-18 10:39:31.000000 django-ipghrms-users-1.1/users/templates/auth/password_reset_confirm.html
+-rw-rw-rw-   0        0        0      780 2022-10-18 10:39:31.000000 django-ipghrms-users-1.1/users/templates/auth/password_reset_done.html
+drwxrwxrwx   0        0        0        0 2023-06-21 01:29:45.667621 django-ipghrms-users-1.1/users/templates/profile/
+-rw-rw-rw-   0        0        0     1474 2023-06-20 15:06:31.000000 django-ipghrms-users-1.1/users/templates/profile/form.html
+-rw-rw-rw-   0        0        0     1122 2023-06-20 14:45:17.000000 django-ipghrms-users-1.1/users/templates/profile/form2.html
+-rw-rw-rw-   0        0        0     6215 2023-06-20 14:50:41.000000 django-ipghrms-users-1.1/users/templates/profile/form3.html
+-rw-rw-rw-   0        0        0     2969 2023-06-20 14:59:25.000000 django-ipghrms-users-1.1/users/templates/profile/form_address.html
+-rw-rw-rw-   0        0        0     2999 2023-06-20 14:56:11.000000 django-ipghrms-users-1.1/users/templates/profile/form_location.html
+-rw-rw-rw-   0        0        0     2588 2023-02-10 02:57:39.000000 django-ipghrms-users-1.1/users/templates/profile/profile.html
+-rw-rw-rw-   0        0        0     2168 2023-03-15 14:43:16.000000 django-ipghrms-users-1.1/users/templates/profile/profile_bottom.html
+-rw-rw-rw-   0        0        0     5620 2023-06-20 15:09:24.000000 django-ipghrms-users-1.1/users/templates/profile/profile_left.html
+-rw-rw-rw-   0        0        0     2209 2023-03-15 14:51:46.000000 django-ipghrms-users-1.1/users/templates/profile/profile_right.html
+-rw-rw-rw-   0        0        0       60 2022-10-18 10:39:31.000000 django-ipghrms-users-1.1/users/tests.py
+-rw-rw-rw-   0        0        0        0 2023-01-18 00:19:34.000000 django-ipghrms-users-1.1/users/urls.py
+drwxrwxrwx   0        0        0        0 2023-06-21 01:29:45.674493 django-ipghrms-users-1.1/users/views/
+-rw-rw-rw-   0        0        0       22 2022-11-30 04:35:46.000000 django-ipghrms-users-1.1/users/views/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 01:29:45.707884 django-ipghrms-users-1.1/users/views/__pycache__/
+-rw-rw-rw-   0        0        0      162 2022-11-30 07:30:55.000000 django-ipghrms-users-1.1/users/views/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      138 2022-10-20 01:02:07.000000 django-ipghrms-users-1.1/users/views/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0      167 2022-10-18 10:39:31.000000 django-ipghrms-users-1.1/users/views/__pycache__/__init__.cpython-38.pyc
+-rw-rw-rw-   0        0        0      146 2022-10-18 10:39:31.000000 django-ipghrms-users-1.1/users/views/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3798 2023-03-15 14:41:25.000000 django-ipghrms-users-1.1/users/views/__pycache__/profile.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3580 2022-10-18 10:39:31.000000 django-ipghrms-users-1.1/users/views/__pycache__/profile.cpython-38.pyc
+-rw-rw-rw-   0        0        0     3549 2022-10-18 10:39:31.000000 django-ipghrms-users-1.1/users/views/__pycache__/profile.cpython-39.pyc
+-rw-rw-rw-   0        0        0     9247 2023-06-20 15:08:29.000000 django-ipghrms-users-1.1/users/views/profile.py
+-rw-rw-rw-   0        0        0       63 2022-10-18 10:39:31.000000 django-ipghrms-users-1.1/users/views.py
```

### Comparing `django-ipghrms-users-1.0/LICENSE` & `django-ipghrms-users-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-ipghrms-users-1.0/PKG-INFO` & `django-ipghrms-users-1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ipghrms-users
-Version: 1.0
+Version: 1.1
 Summary: Django IPG HRMS APP users
 Home-page: http://ipg.tl/
 Author: Kinos
 Author-email: info@kinos.tl
 Maintainer: kinos
 Maintainer-email: info@kinos.tl
 License: MIT
```

### Comparing `django-ipghrms-users-1.0/django_ipghrms_users.egg-info/PKG-INFO` & `django-ipghrms-users-1.1/django_ipghrms_users.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ipghrms-users
-Version: 1.0
+Version: 1.1
 Summary: Django IPG HRMS APP users
 Home-page: http://ipg.tl/
 Author: Kinos
 Author-email: info@kinos.tl
 Maintainer: kinos
 Maintainer-email: info@kinos.tl
 License: MIT
```

### Comparing `django-ipghrms-users-1.0/django_ipghrms_users.egg-info/SOURCES.txt` & `django-ipghrms-users-1.1/django_ipghrms_users.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -21,14 +21,19 @@
 users/templates/auth/account.html
 users/templates/auth/change_password.html
 users/templates/auth/change_password_done.html
 users/templates/auth/password_reset.html
 users/templates/auth/password_reset_complete.html
 users/templates/auth/password_reset_confirm.html
 users/templates/auth/password_reset_done.html
+users/templates/profile/form.html
+users/templates/profile/form2.html
+users/templates/profile/form3.html
+users/templates/profile/form_address.html
+users/templates/profile/form_location.html
 users/templates/profile/profile.html
 users/templates/profile/profile_bottom.html
 users/templates/profile/profile_left.html
 users/templates/profile/profile_right.html
 users/views/__init__.py
 users/views/profile.py
 users/views/__pycache__/__init__.cpython-310.pyc
```

### Comparing `django-ipghrms-users-1.0/users/context_processors.py` & `django-ipghrms-users-1.1/users/context_processors.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-users-1.0/users/forms.py` & `django-ipghrms-users-1.1/users/forms.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-users-1.0/users/templates/auth/account.html` & `django-ipghrms-users-1.1/users/templates/auth/account.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-users-1.0/users/templates/auth/change_password.html` & `django-ipghrms-users-1.1/users/templates/auth/change_password.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-users-1.0/users/templates/auth/password_reset.html` & `django-ipghrms-users-1.1/users/templates/auth/password_reset.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-users-1.0/users/templates/auth/password_reset_complete.html` & `django-ipghrms-users-1.1/users/templates/auth/password_reset_complete.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-users-1.0/users/templates/auth/password_reset_confirm.html` & `django-ipghrms-users-1.1/users/templates/auth/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-users-1.0/users/templates/auth/password_reset_done.html` & `django-ipghrms-users-1.1/users/templates/auth/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-users-1.0/users/templates/profile/profile.html` & `django-ipghrms-users-1.1/users/templates/profile/profile.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-users-1.0/users/templates/profile/profile_bottom.html` & `django-ipghrms-users-1.1/users/templates/profile/profile_bottom.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-users-1.0/users/templates/profile/profile_right.html` & `django-ipghrms-users-1.1/users/templates/profile/profile_right.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-users-1.0/users/views/__pycache__/profile.cpython-310.pyc` & `django-ipghrms-users-1.1/users/views/__pycache__/profile.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-users-1.0/users/views/__pycache__/profile.cpython-38.pyc` & `django-ipghrms-users-1.1/users/views/__pycache__/profile.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-users-1.0/users/views/__pycache__/profile.cpython-39.pyc` & `django-ipghrms-users-1.1/users/views/__pycache__/profile.cpython-39.pyc`

 * *Files identical despite different names*

