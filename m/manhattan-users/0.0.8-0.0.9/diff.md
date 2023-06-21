# Comparing `tmp/manhattan_users-0.0.8.tar.gz` & `tmp/manhattan_users-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/manhattan_users-0.0.8.tar", last modified: Tue Sep  3 21:09:40 2019, max compression
+gzip compressed data, was "dist/manhattan_users-0.0.9.tar", last modified: Sat Sep  7 22:32:04 2019, max compression
```

## Comparing `manhattan_users-0.0.8.tar` & `manhattan_users-0.0.9.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-09-03 21:09:40.000000 manhattan_users-0.0.8/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1101 2019-08-09 00:43:18.000000 manhattan_users-0.0.8/LICENSE
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      123 2019-08-12 03:26:52.000000 manhattan_users-0.0.8/MANIFEST.in
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1143 2019-09-03 21:09:40.000000 manhattan_users-0.0.8/PKG-INFO
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      202 2019-08-09 00:44:27.000000 manhattan_users-0.0.8/README.md
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-09-03 21:09:40.000000 manhattan_users-0.0.8/manhattan_users/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-09-03 21:09:40.000000 manhattan_users-0.0.8/manhattan_users/manhattan/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)       56 2019-08-09 00:52:25.000000 manhattan_users-0.0.8/manhattan_users/manhattan/__init__.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-09-03 21:09:40.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)        0 2019-08-09 00:52:40.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/__init__.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-09-03 21:09:40.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/models/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)       50 2019-08-09 12:19:07.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/models/__init__.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     7518 2019-08-09 15:45:00.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/models/user_sessions.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    10440 2019-08-11 13:26:02.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/models/users.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     3418 2019-09-03 21:07:45.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/settings.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-09-03 21:09:40.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/templates/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-09-03 21:09:40.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/templates/manhattan/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-09-03 21:09:40.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/templates/manhattan/users/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      489 2019-08-11 00:03:35.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/templates/manhattan/users/accept_invite.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)        0 2019-08-11 00:13:36.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/templates/manhattan/users/add.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)       60 2019-08-11 12:34:47.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/templates/manhattan/users/change_log.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)       35 2019-08-11 12:43:00.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/templates/manhattan/users/dashboard.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)       54 2019-08-11 12:52:57.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/templates/manhattan/users/delete.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-09-03 21:09:40.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/templates/manhattan/users/emails/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      742 2019-08-11 23:12:10.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/templates/manhattan/users/emails/email_changed.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      488 2019-08-11 01:11:53.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/templates/manhattan/users/emails/invite.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      840 2019-08-10 23:07:25.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/templates/manhattan/users/emails/new_device.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      654 2019-08-12 02:12:02.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/templates/manhattan/users/emails/recovery_code_used.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      698 2019-08-11 17:42:32.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/templates/manhattan/users/emails/reset_password.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-09-03 21:09:40.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/templates/manhattan/users/includes/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1129 2019-08-11 23:09:59.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/templates/manhattan/users/includes/password_rules.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      832 2019-08-11 00:01:58.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/templates/manhattan/users/includes/password_rules_minimal.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      351 2019-08-11 12:58:43.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/templates/manhattan/users/list.html
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-09-03 21:09:40.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/templates/manhattan/users/mfa/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      865 2019-08-12 02:18:57.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/templates/manhattan/users/mfa/auth.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      659 2019-08-12 01:26:56.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/templates/manhattan/users/mfa/disable.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1104 2019-08-12 01:44:56.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/templates/manhattan/users/mfa/enable.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2187 2019-08-12 01:26:50.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/templates/manhattan/users/mfa/recovery_codes.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      352 2019-08-11 16:49:05.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/templates/manhattan/users/request_new_invite.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      491 2019-08-11 17:39:29.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/templates/manhattan/users/reset_password.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2993 2019-08-11 22:32:11.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/templates/manhattan/users/security.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      485 2019-08-11 22:51:27.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/templates/manhattan/users/set_new_password.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      597 2019-08-10 13:21:05.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/templates/manhattan/users/sign_in.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      917 2019-08-11 23:06:03.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/templates/manhattan/users/update.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      497 2019-08-11 23:12:26.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/templates/manhattan/users/update_my_profile.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     3371 2019-08-12 00:21:20.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/templates/manhattan/users/view.html
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      376 2019-08-10 22:31:25.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/utils.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-09-03 21:09:40.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/views/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      488 2019-08-12 00:29:06.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/views/__init__.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     4926 2019-08-11 13:39:22.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/views/accept_invite.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2813 2019-08-13 00:41:20.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/views/add.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      177 2019-08-11 12:45:04.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/views/change_log.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      705 2019-08-11 12:45:10.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/views/dashboard.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      146 2019-08-11 12:53:22.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/views/delete.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      867 2019-08-11 13:04:14.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/views/list.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-09-03 21:09:40.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/views/mfa/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      175 2019-08-12 02:47:48.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/views/mfa/__init__.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     6996 2019-09-03 10:52:42.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/views/mfa/auth.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     3016 2019-09-03 10:52:42.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/views/mfa/disable.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      975 2019-09-03 10:52:41.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/views/mfa/download_recovery_codes.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     4091 2019-09-03 10:52:40.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/views/mfa/enable.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1920 2019-09-03 10:52:40.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/views/mfa/recovery_codes.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1370 2019-09-03 10:52:39.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/views/mfa/regenerate_recovery_codes.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      947 2019-08-11 13:26:33.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/views/remove_lock.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     4618 2019-08-11 17:34:15.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/views/request_new_invite.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1861 2019-08-11 17:18:30.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/views/resend_invite.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     4702 2019-08-11 22:54:43.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/views/reset_password.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2193 2019-08-11 22:23:12.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/views/revoke_session.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     3433 2019-09-03 10:52:59.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/views/security.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     5150 2019-08-11 22:55:25.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/views/set_new_password.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     6940 2019-08-13 00:46:31.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/views/sign_in.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      924 2019-08-10 12:49:13.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/views/sign_out.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1836 2019-08-11 23:36:11.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/views/update.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     4305 2019-09-03 10:53:03.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/views/update_my_profile.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1455 2019-08-12 00:20:50.000000 manhattan_users-0.0.8/manhattan_users/manhattan/users/views/view.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-09-03 21:09:40.000000 manhattan_users-0.0.8/manhattan_users/manhattan_users.egg-info/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1143 2019-09-03 21:09:40.000000 manhattan_users-0.0.8/manhattan_users/manhattan_users.egg-info/PKG-INFO
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4036 2019-09-03 21:09:40.000000 manhattan_users-0.0.8/manhattan_users/manhattan_users.egg-info/SOURCES.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2019-09-03 21:09:40.000000 manhattan_users-0.0.8/manhattan_users/manhattan_users.egg-info/dependency_links.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)       10 2019-09-03 21:09:40.000000 manhattan_users-0.0.8/manhattan_users/manhattan_users.egg-info/namespace_packages.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)      216 2019-09-03 21:09:40.000000 manhattan_users-0.0.8/manhattan_users/manhattan_users.egg-info/requires.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)       10 2019-09-03 21:09:40.000000 manhattan_users-0.0.8/manhattan_users/manhattan_users.egg-info/top_level.txt
--rw-rw-r--   0 anthony   (1000) anthony   (1000)       79 2019-09-03 21:09:40.000000 manhattan_users-0.0.8/setup.cfg
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     4681 2019-09-03 21:08:17.000000 manhattan_users-0.0.8/setup.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-09-07 22:32:04.000000 manhattan_users-0.0.9/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1101 2019-08-09 00:43:18.000000 manhattan_users-0.0.9/LICENSE
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      123 2019-08-12 03:26:52.000000 manhattan_users-0.0.9/MANIFEST.in
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1143 2019-09-07 22:32:04.000000 manhattan_users-0.0.9/PKG-INFO
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      202 2019-08-09 00:44:27.000000 manhattan_users-0.0.9/README.md
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-09-07 22:32:04.000000 manhattan_users-0.0.9/manhattan_users/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-09-07 22:32:04.000000 manhattan_users-0.0.9/manhattan_users/manhattan/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)       56 2019-08-09 00:52:25.000000 manhattan_users-0.0.9/manhattan_users/manhattan/__init__.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-09-07 22:32:04.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)        0 2019-08-09 00:52:40.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/__init__.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-09-07 22:32:04.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/models/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)       50 2019-08-09 12:19:07.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/models/__init__.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     7518 2019-08-09 15:45:00.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/models/user_sessions.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)    10440 2019-08-11 13:26:02.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/models/users.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     3418 2019-09-03 21:07:45.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/settings.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-09-07 22:32:04.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/templates/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-09-07 22:32:04.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/templates/manhattan/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-09-07 22:32:04.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/templates/manhattan/users/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      489 2019-08-11 00:03:35.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/templates/manhattan/users/accept_invite.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      736 2019-09-07 22:31:10.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/templates/manhattan/users/add.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)       60 2019-08-11 12:34:47.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/templates/manhattan/users/change_log.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)       35 2019-08-11 12:43:00.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/templates/manhattan/users/dashboard.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)       54 2019-08-11 12:52:57.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/templates/manhattan/users/delete.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-09-07 22:32:04.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/templates/manhattan/users/emails/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      742 2019-08-11 23:12:10.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/templates/manhattan/users/emails/email_changed.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      488 2019-08-11 01:11:53.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/templates/manhattan/users/emails/invite.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      840 2019-08-10 23:07:25.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/templates/manhattan/users/emails/new_device.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      654 2019-08-12 02:12:02.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/templates/manhattan/users/emails/recovery_code_used.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      698 2019-08-11 17:42:32.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/templates/manhattan/users/emails/reset_password.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-09-07 22:32:04.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/templates/manhattan/users/includes/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1129 2019-08-11 23:09:59.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/templates/manhattan/users/includes/password_rules.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      832 2019-08-11 00:01:58.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/templates/manhattan/users/includes/password_rules_minimal.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      351 2019-08-11 12:58:43.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/templates/manhattan/users/list.html
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-09-07 22:32:04.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/templates/manhattan/users/mfa/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      865 2019-08-12 02:18:57.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/templates/manhattan/users/mfa/auth.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      659 2019-08-12 01:26:56.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/templates/manhattan/users/mfa/disable.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1104 2019-08-12 01:44:56.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/templates/manhattan/users/mfa/enable.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2187 2019-08-12 01:26:50.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/templates/manhattan/users/mfa/recovery_codes.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      352 2019-08-11 16:49:05.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/templates/manhattan/users/request_new_invite.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      491 2019-08-11 17:39:29.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/templates/manhattan/users/reset_password.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2993 2019-08-11 22:32:11.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/templates/manhattan/users/security.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      485 2019-08-11 22:51:27.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/templates/manhattan/users/set_new_password.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      597 2019-08-10 13:21:05.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/templates/manhattan/users/sign_in.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      917 2019-08-11 23:06:03.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/templates/manhattan/users/update.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      497 2019-08-11 23:12:26.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/templates/manhattan/users/update_my_profile.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     3371 2019-08-12 00:21:20.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/templates/manhattan/users/view.html
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      376 2019-08-10 22:31:25.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/utils.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-09-07 22:32:04.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/views/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      488 2019-08-12 00:29:06.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/views/__init__.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     4926 2019-08-11 13:39:22.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/views/accept_invite.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2813 2019-08-13 00:41:20.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/views/add.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      177 2019-08-11 12:45:04.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/views/change_log.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      705 2019-08-11 12:45:10.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/views/dashboard.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      146 2019-08-11 12:53:22.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/views/delete.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      867 2019-08-11 13:04:14.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/views/list.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-09-07 22:32:04.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/views/mfa/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      175 2019-08-12 02:47:48.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/views/mfa/__init__.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     6996 2019-09-03 10:52:42.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/views/mfa/auth.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     3016 2019-09-03 10:52:42.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/views/mfa/disable.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      975 2019-09-03 10:52:41.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/views/mfa/download_recovery_codes.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     4091 2019-09-03 10:52:40.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/views/mfa/enable.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1920 2019-09-03 10:52:40.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/views/mfa/recovery_codes.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1370 2019-09-03 10:52:39.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/views/mfa/regenerate_recovery_codes.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      947 2019-08-11 13:26:33.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/views/remove_lock.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     4618 2019-08-11 17:34:15.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/views/request_new_invite.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1861 2019-08-11 17:18:30.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/views/resend_invite.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     4702 2019-08-11 22:54:43.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/views/reset_password.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2193 2019-08-11 22:23:12.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/views/revoke_session.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     3433 2019-09-03 10:52:59.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/views/security.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     5150 2019-08-11 22:55:25.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/views/set_new_password.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     6940 2019-08-13 00:46:31.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/views/sign_in.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      924 2019-08-10 12:49:13.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/views/sign_out.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1836 2019-08-11 23:36:11.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/views/update.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     4305 2019-09-03 10:53:03.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/views/update_my_profile.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1455 2019-08-12 00:20:50.000000 manhattan_users-0.0.9/manhattan_users/manhattan/users/views/view.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2019-09-07 22:32:04.000000 manhattan_users-0.0.9/manhattan_users/manhattan_users.egg-info/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1143 2019-09-07 22:32:04.000000 manhattan_users-0.0.9/manhattan_users/manhattan_users.egg-info/PKG-INFO
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4036 2019-09-07 22:32:04.000000 manhattan_users-0.0.9/manhattan_users/manhattan_users.egg-info/SOURCES.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2019-09-07 22:32:04.000000 manhattan_users-0.0.9/manhattan_users/manhattan_users.egg-info/dependency_links.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       10 2019-09-07 22:32:04.000000 manhattan_users-0.0.9/manhattan_users/manhattan_users.egg-info/namespace_packages.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      216 2019-09-07 22:32:04.000000 manhattan_users-0.0.9/manhattan_users/manhattan_users.egg-info/requires.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       10 2019-09-07 22:32:04.000000 manhattan_users-0.0.9/manhattan_users/manhattan_users.egg-info/top_level.txt
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)       79 2019-09-07 22:32:04.000000 manhattan_users-0.0.9/setup.cfg
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     4681 2019-09-07 22:31:19.000000 manhattan_users-0.0.9/setup.py
```

### Comparing `manhattan_users-0.0.8/LICENSE` & `manhattan_users-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `manhattan_users-0.0.8/PKG-INFO` & `manhattan_users-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manhattan_users
-Version: 0.0.8
+Version: 0.0.9
 Summary: Chains and factories for building user access / control functionality into a manhattan manage application.
 Home-page: https://git.getme.co.uk/manhattan/manhattan_users
 Author: Anthony Blackshaw
 Author-email: ant@getme.co.uk
 Maintainer: The Getme development team
 Maintainer-email: devs@getme.co.uk
 License: MIT
```

### Comparing `manhattan_users-0.0.8/manhattan_users/manhattan/users/models/user_sessions.py` & `manhattan_users-0.0.9/manhattan_users/manhattan/users/models/user_sessions.py`

 * *Files identical despite different names*

### Comparing `manhattan_users-0.0.8/manhattan_users/manhattan/users/models/users.py` & `manhattan_users-0.0.9/manhattan_users/manhattan/users/models/users.py`

 * *Files identical despite different names*

### Comparing `manhattan_users-0.0.8/manhattan_users/manhattan/users/settings.py` & `manhattan_users-0.0.9/manhattan_users/manhattan/users/settings.py`

 * *Files identical despite different names*

### Comparing `manhattan_users-0.0.8/manhattan_users/manhattan/users/templates/manhattan/users/emails/email_changed.html` & `manhattan_users-0.0.9/manhattan_users/manhattan/users/templates/manhattan/users/emails/email_changed.html`

 * *Files identical despite different names*

### Comparing `manhattan_users-0.0.8/manhattan_users/manhattan/users/templates/manhattan/users/emails/new_device.html` & `manhattan_users-0.0.9/manhattan_users/manhattan/users/templates/manhattan/users/emails/new_device.html`

 * *Files identical despite different names*

### Comparing `manhattan_users-0.0.8/manhattan_users/manhattan/users/templates/manhattan/users/emails/recovery_code_used.html` & `manhattan_users-0.0.9/manhattan_users/manhattan/users/templates/manhattan/users/emails/recovery_code_used.html`

 * *Files identical despite different names*

### Comparing `manhattan_users-0.0.8/manhattan_users/manhattan/users/templates/manhattan/users/emails/reset_password.html` & `manhattan_users-0.0.9/manhattan_users/manhattan/users/templates/manhattan/users/emails/reset_password.html`

 * *Files identical despite different names*

### Comparing `manhattan_users-0.0.8/manhattan_users/manhattan/users/templates/manhattan/users/includes/password_rules.html` & `manhattan_users-0.0.9/manhattan_users/manhattan/users/templates/manhattan/users/includes/password_rules.html`

 * *Files identical despite different names*

### Comparing `manhattan_users-0.0.8/manhattan_users/manhattan/users/templates/manhattan/users/includes/password_rules_minimal.html` & `manhattan_users-0.0.9/manhattan_users/manhattan/users/templates/manhattan/users/includes/password_rules_minimal.html`

 * *Files identical despite different names*

### Comparing `manhattan_users-0.0.8/manhattan_users/manhattan/users/templates/manhattan/users/mfa/auth.html` & `manhattan_users-0.0.9/manhattan_users/manhattan/users/templates/manhattan/users/mfa/auth.html`

 * *Files identical despite different names*

### Comparing `manhattan_users-0.0.8/manhattan_users/manhattan/users/templates/manhattan/users/mfa/disable.html` & `manhattan_users-0.0.9/manhattan_users/manhattan/users/templates/manhattan/users/mfa/disable.html`

 * *Files identical despite different names*

### Comparing `manhattan_users-0.0.8/manhattan_users/manhattan/users/templates/manhattan/users/mfa/enable.html` & `manhattan_users-0.0.9/manhattan_users/manhattan/users/templates/manhattan/users/mfa/enable.html`

 * *Files identical despite different names*

### Comparing `manhattan_users-0.0.8/manhattan_users/manhattan/users/templates/manhattan/users/mfa/recovery_codes.html` & `manhattan_users-0.0.9/manhattan_users/manhattan/users/templates/manhattan/users/mfa/recovery_codes.html`

 * *Files identical despite different names*

### Comparing `manhattan_users-0.0.8/manhattan_users/manhattan/users/templates/manhattan/users/security.html` & `manhattan_users-0.0.9/manhattan_users/manhattan/users/templates/manhattan/users/security.html`

 * *Files identical despite different names*

### Comparing `manhattan_users-0.0.8/manhattan_users/manhattan/users/templates/manhattan/users/sign_in.html` & `manhattan_users-0.0.9/manhattan_users/manhattan/users/templates/manhattan/users/sign_in.html`

 * *Files identical despite different names*

### Comparing `manhattan_users-0.0.8/manhattan_users/manhattan/users/templates/manhattan/users/update.html` & `manhattan_users-0.0.9/manhattan_users/manhattan/users/templates/manhattan/users/update.html`

 * *Files identical despite different names*

### Comparing `manhattan_users-0.0.8/manhattan_users/manhattan/users/templates/manhattan/users/view.html` & `manhattan_users-0.0.9/manhattan_users/manhattan/users/templates/manhattan/users/view.html`

 * *Files identical despite different names*

### Comparing `manhattan_users-0.0.8/manhattan_users/manhattan/users/views/accept_invite.py` & `manhattan_users-0.0.9/manhattan_users/manhattan/users/views/accept_invite.py`

 * *Files identical despite different names*

### Comparing `manhattan_users-0.0.8/manhattan_users/manhattan/users/views/add.py` & `manhattan_users-0.0.9/manhattan_users/manhattan/users/views/add.py`

 * *Files identical despite different names*

### Comparing `manhattan_users-0.0.8/manhattan_users/manhattan/users/views/dashboard.py` & `manhattan_users-0.0.9/manhattan_users/manhattan/users/views/dashboard.py`

 * *Files identical despite different names*

### Comparing `manhattan_users-0.0.8/manhattan_users/manhattan/users/views/list.py` & `manhattan_users-0.0.9/manhattan_users/manhattan/users/views/list.py`

 * *Files identical despite different names*

### Comparing `manhattan_users-0.0.8/manhattan_users/manhattan/users/views/mfa/auth.py` & `manhattan_users-0.0.9/manhattan_users/manhattan/users/views/mfa/auth.py`

 * *Files identical despite different names*

### Comparing `manhattan_users-0.0.8/manhattan_users/manhattan/users/views/mfa/disable.py` & `manhattan_users-0.0.9/manhattan_users/manhattan/users/views/mfa/disable.py`

 * *Files identical despite different names*

### Comparing `manhattan_users-0.0.8/manhattan_users/manhattan/users/views/mfa/download_recovery_codes.py` & `manhattan_users-0.0.9/manhattan_users/manhattan/users/views/mfa/download_recovery_codes.py`

 * *Files identical despite different names*

### Comparing `manhattan_users-0.0.8/manhattan_users/manhattan/users/views/mfa/enable.py` & `manhattan_users-0.0.9/manhattan_users/manhattan/users/views/mfa/enable.py`

 * *Files identical despite different names*

### Comparing `manhattan_users-0.0.8/manhattan_users/manhattan/users/views/mfa/recovery_codes.py` & `manhattan_users-0.0.9/manhattan_users/manhattan/users/views/mfa/recovery_codes.py`

 * *Files identical despite different names*

### Comparing `manhattan_users-0.0.8/manhattan_users/manhattan/users/views/mfa/regenerate_recovery_codes.py` & `manhattan_users-0.0.9/manhattan_users/manhattan/users/views/mfa/regenerate_recovery_codes.py`

 * *Files identical despite different names*

### Comparing `manhattan_users-0.0.8/manhattan_users/manhattan/users/views/remove_lock.py` & `manhattan_users-0.0.9/manhattan_users/manhattan/users/views/remove_lock.py`

 * *Files identical despite different names*

### Comparing `manhattan_users-0.0.8/manhattan_users/manhattan/users/views/request_new_invite.py` & `manhattan_users-0.0.9/manhattan_users/manhattan/users/views/request_new_invite.py`

 * *Files identical despite different names*

### Comparing `manhattan_users-0.0.8/manhattan_users/manhattan/users/views/resend_invite.py` & `manhattan_users-0.0.9/manhattan_users/manhattan/users/views/resend_invite.py`

 * *Files identical despite different names*

### Comparing `manhattan_users-0.0.8/manhattan_users/manhattan/users/views/reset_password.py` & `manhattan_users-0.0.9/manhattan_users/manhattan/users/views/reset_password.py`

 * *Files identical despite different names*

### Comparing `manhattan_users-0.0.8/manhattan_users/manhattan/users/views/revoke_session.py` & `manhattan_users-0.0.9/manhattan_users/manhattan/users/views/revoke_session.py`

 * *Files identical despite different names*

### Comparing `manhattan_users-0.0.8/manhattan_users/manhattan/users/views/security.py` & `manhattan_users-0.0.9/manhattan_users/manhattan/users/views/security.py`

 * *Files identical despite different names*

### Comparing `manhattan_users-0.0.8/manhattan_users/manhattan/users/views/set_new_password.py` & `manhattan_users-0.0.9/manhattan_users/manhattan/users/views/set_new_password.py`

 * *Files identical despite different names*

### Comparing `manhattan_users-0.0.8/manhattan_users/manhattan/users/views/sign_in.py` & `manhattan_users-0.0.9/manhattan_users/manhattan/users/views/sign_in.py`

 * *Files identical despite different names*

### Comparing `manhattan_users-0.0.8/manhattan_users/manhattan/users/views/sign_out.py` & `manhattan_users-0.0.9/manhattan_users/manhattan/users/views/sign_out.py`

 * *Files identical despite different names*

### Comparing `manhattan_users-0.0.8/manhattan_users/manhattan/users/views/update.py` & `manhattan_users-0.0.9/manhattan_users/manhattan/users/views/update.py`

 * *Files identical despite different names*

### Comparing `manhattan_users-0.0.8/manhattan_users/manhattan/users/views/update_my_profile.py` & `manhattan_users-0.0.9/manhattan_users/manhattan/users/views/update_my_profile.py`

 * *Files identical despite different names*

### Comparing `manhattan_users-0.0.8/manhattan_users/manhattan/users/views/view.py` & `manhattan_users-0.0.9/manhattan_users/manhattan/users/views/view.py`

 * *Files identical despite different names*

### Comparing `manhattan_users-0.0.8/manhattan_users/manhattan_users.egg-info/PKG-INFO` & `manhattan_users-0.0.9/manhattan_users/manhattan_users.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manhattan-users
-Version: 0.0.8
+Version: 0.0.9
 Summary: Chains and factories for building user access / control functionality into a manhattan manage application.
 Home-page: https://git.getme.co.uk/manhattan/manhattan_users
 Author: Anthony Blackshaw
 Author-email: ant@getme.co.uk
 Maintainer: The Getme development team
 Maintainer-email: devs@getme.co.uk
 License: MIT
```

### Comparing `manhattan_users-0.0.8/manhattan_users/manhattan_users.egg-info/SOURCES.txt` & `manhattan_users-0.0.9/manhattan_users/manhattan_users.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `manhattan_users-0.0.8/setup.py` & `manhattan_users-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 setup(
     name='manhattan_users',
     namespace_packages=['manhattan'],
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.0.8',
+    version='0.0.9',
 
     description=(
         'Chains and factories for building user access / control '
         'functionality into a manhattan manage application.'
     ),
     long_description=long_description,
     long_description_content_type='text/markdown',
```

