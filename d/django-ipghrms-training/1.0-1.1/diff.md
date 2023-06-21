# Comparing `tmp/django-ipghrms-training-1.0.tar.gz` & `tmp/django-ipghrms-training-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-ipghrms-training-1.0.tar", last modified: Mon Mar 27 15:20:26 2023, max compression
+gzip compressed data, was "django-ipghrms-training-1.1.tar", last modified: Wed Jun 21 14:35:32 2023, max compression
```

## Comparing `django-ipghrms-training-1.0.tar` & `django-ipghrms-training-1.1.tar`

### file list

```diff
@@ -1,167 +1,167 @@
-drwxrwxrwx   0        0        0        0 2023-03-27 15:20:26.448710 django-ipghrms-training-1.0/
--rw-rw-rw-   0        0        0     1068 2023-03-27 15:20:00.000000 django-ipghrms-training-1.0/LICENSE
--rw-rw-rw-   0        0        0      186 2023-03-27 14:32:07.000000 django-ipghrms-training-1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      951 2023-03-27 15:20:26.448710 django-ipghrms-training-1.0/PKG-INFO
--rw-rw-rw-   0        0        0      503 2023-03-27 14:32:12.000000 django-ipghrms-training-1.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-27 15:20:25.819326 django-ipghrms-training-1.0/django_ipghrms_training.egg-info/
--rw-rw-rw-   0        0        0      951 2023-03-27 15:20:25.000000 django-ipghrms-training-1.0/django_ipghrms_training.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8630 2023-03-27 15:20:25.000000 django-ipghrms-training-1.0/django_ipghrms_training.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-27 15:20:25.000000 django-ipghrms-training-1.0/django_ipghrms_training.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-03-27 15:20:25.000000 django-ipghrms-training-1.0/django_ipghrms_training.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      511 2023-03-27 15:20:26.450708 django-ipghrms-training-1.0/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-03-22 07:44:49.000000 django-ipghrms-training-1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-27 15:20:25.840662 django-ipghrms-training-1.0/training/
--rw-rw-rw-   0        0        0        0 2022-10-18 10:39:31.000000 django-ipghrms-training-1.0/training/__init__.py
--rw-rw-rw-   0        0        0      772 2023-03-11 06:48:13.000000 django-ipghrms-training-1.0/training/admin.py
-drwxrwxrwx   0        0        0        0 2023-03-27 15:20:25.846669 django-ipghrms-training-1.0/training/api/
-drwxrwxrwx   0        0        0        0 2023-03-27 15:20:25.860973 django-ipghrms-training-1.0/training/api/__pycache__/
--rw-rw-rw-   0        0        0      349 2022-11-07 13:19:38.000000 django-ipghrms-training-1.0/training/api/__pycache__/urls.cpython-310.pyc
--rw-rw-rw-   0        0        0      345 2022-11-05 14:51:39.000000 django-ipghrms-training-1.0/training/api/__pycache__/urls.cpython-37.pyc
--rw-rw-rw-   0        0        0     2772 2023-03-12 10:06:03.000000 django-ipghrms-training-1.0/training/api/__pycache__/views.cpython-310.pyc
--rw-rw-rw-   0        0        0     2751 2022-11-05 14:51:39.000000 django-ipghrms-training-1.0/training/api/__pycache__/views.cpython-37.pyc
--rw-rw-rw-   0        0        0      203 2022-11-04 05:28:45.000000 django-ipghrms-training-1.0/training/api/urls.py
--rw-rw-rw-   0        0        0     2473 2023-03-12 10:05:59.000000 django-ipghrms-training-1.0/training/api/views.py
--rw-rw-rw-   0        0        0      148 2022-10-18 10:39:31.000000 django-ipghrms-training-1.0/training/apps.py
--rw-rw-rw-   0        0        0    10676 2023-03-12 05:28:12.000000 django-ipghrms-training-1.0/training/forms.py
-drwxrwxrwx   0        0        0        0 2023-03-27 15:20:25.955000 django-ipghrms-training-1.0/training/migrations/
--rw-rw-rw-   0        0        0     6057 2022-10-18 10:39:31.000000 django-ipghrms-training-1.0/training/migrations/0001_initial.py
--rw-rw-rw-   0        0        0     7595 2022-11-04 05:28:45.000000 django-ipghrms-training-1.0/training/migrations/0002_hrcriteria_trainingemp_tyear_unitcriteria_and_more.py
--rw-rw-rw-   0        0        0      730 2022-11-04 05:28:45.000000 django-ipghrms-training-1.0/training/migrations/0003_rename_fundtype_ttype_delete_trainingtype_and_more.py
--rw-rw-rw-   0        0        0      467 2022-11-04 05:28:45.000000 django-ipghrms-training-1.0/training/migrations/0004_trainingplan_duration.py
--rw-rw-rw-   0        0        0     2249 2022-11-04 05:28:45.000000 django-ipghrms-training-1.0/training/migrations/0005_tcriteria_trainingcriteria_remove_unitcriteria_plan_and_more.py
--rw-rw-rw-   0        0        0      443 2022-11-04 05:28:45.000000 django-ipghrms-training-1.0/training/migrations/0006_alter_tcriteria_subject.py
--rw-rw-rw-   0        0        0      979 2022-11-04 05:28:45.000000 django-ipghrms-training-1.0/training/migrations/0007_trainingplan_is_approve_trainingplan_is_certify_and_more.py
--rw-rw-rw-   0        0        0     1402 2022-11-04 05:28:45.000000 django-ipghrms-training-1.0/training/migrations/0008_trainingsubject.py
--rw-rw-rw-   0        0        0      886 2022-11-04 05:28:45.000000 django-ipghrms-training-1.0/training/migrations/0009_remove_trainingplan_duration_and_more.py
--rw-rw-rw-   0        0        0      872 2022-11-04 05:28:45.000000 django-ipghrms-training-1.0/training/migrations/0010_trainingplan_duration_trainingplan_place_and_more.py
--rw-rw-rw-   0        0        0      442 2022-11-04 05:28:45.000000 django-ipghrms-training-1.0/training/migrations/0011_remove_trainingemp_hashed_delete_trainingsubject.py
--rw-rw-rw-   0        0        0     1386 2022-11-04 05:28:45.000000 django-ipghrms-training-1.0/training/migrations/0012_trainingemp_diploma_alter_trainingemp_department_and_more.py
--rw-rw-rw-   0        0        0      583 2022-11-04 05:28:45.000000 django-ipghrms-training-1.0/training/migrations/0013_alter_trainingcriteria_criteria.py
--rw-rw-rw-   0        0        0      404 2022-11-04 05:28:45.000000 django-ipghrms-training-1.0/training/migrations/0014_tcriteria_is_active.py
--rw-rw-rw-   0        0        0     1254 2022-12-09 17:26:57.000000 django-ipghrms-training-1.0/training/migrations/0015_auto_20221210_0226.py
--rw-rw-rw-   0        0        0      435 2022-12-09 18:16:10.000000 django-ipghrms-training-1.0/training/migrations/0016_trainingemp_is_update.py
--rw-rw-rw-   0        0        0     3780 2022-12-10 05:05:40.000000 django-ipghrms-training-1.0/training/migrations/0017_scholarshipplan_sprogress_stype.py
--rw-rw-rw-   0        0        0     1262 2022-12-10 05:35:42.000000 django-ipghrms-training-1.0/training/migrations/0018_auto_20221210_1435.py
--rw-rw-rw-   0        0        0     2568 2022-12-10 06:30:52.000000 django-ipghrms-training-1.0/training/migrations/0019_scholarshipemp_scholarshipempprogress.py
--rw-rw-rw-   0        0        0      483 2022-12-10 06:50:52.000000 django-ipghrms-training-1.0/training/migrations/0020_auto_20221210_1550.py
--rw-rw-rw-   0        0        0      398 2022-12-10 07:01:38.000000 django-ipghrms-training-1.0/training/migrations/0021_rename_start_date_scholarshipempprogress_date.py
--rw-rw-rw-   0        0        0      623 2022-12-10 07:55:09.000000 django-ipghrms-training-1.0/training/migrations/0022_alter_scholarshipemp_emp.py
--rw-rw-rw-   0        0        0      445 2022-12-10 08:37:10.000000 django-ipghrms-training-1.0/training/migrations/0023_scholarshipplan_is_update.py
--rw-rw-rw-   0        0        0      564 2022-12-10 08:42:50.000000 django-ipghrms-training-1.0/training/migrations/0024_auto_20221210_1742.py
--rw-rw-rw-   0        0        0      660 2023-02-14 03:45:18.000000 django-ipghrms-training-1.0/training/migrations/0025_trainingemp_subject.py
--rw-rw-rw-   0        0        0     1196 2023-03-11 04:12:21.000000 django-ipghrms-training-1.0/training/migrations/0026_traininggap.py
--rw-rw-rw-   0        0        0      426 2023-03-11 04:25:14.000000 django-ipghrms-training-1.0/training/migrations/0027_traininggap_is_done.py
--rw-rw-rw-   0        0        0      576 2023-03-11 04:56:44.000000 django-ipghrms-training-1.0/training/migrations/0028_traininggap_employee.py
--rw-rw-rw-   0        0        0      435 2023-03-11 05:24:46.000000 django-ipghrms-training-1.0/training/migrations/0029_traininggap_is_lock.py
--rw-rw-rw-   0        0        0     1928 2023-03-11 06:46:35.000000 django-ipghrms-training-1.0/training/migrations/0030_trainingdep_trainingplangap.py
--rw-rw-rw-   0        0        0      891 2023-03-11 17:15:26.000000 django-ipghrms-training-1.0/training/migrations/0031_auto_20230312_0215.py
--rw-rw-rw-   0        0        0      436 2023-03-12 07:17:20.000000 django-ipghrms-training-1.0/training/migrations/0032_trainingplan_is_update.py
--rw-rw-rw-   0        0        0      559 2023-03-12 07:19:34.000000 django-ipghrms-training-1.0/training/migrations/0033_auto_20230312_1619.py
--rw-rw-rw-   0        0        0        0 2022-10-18 10:39:31.000000 django-ipghrms-training-1.0/training/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-27 15:20:26.163381 django-ipghrms-training-1.0/training/migrations/__pycache__/
--rw-rw-rw-   0        0        0     2885 2022-11-07 13:19:40.000000 django-ipghrms-training-1.0/training/migrations/__pycache__/0001_initial.cpython-310.pyc
--rw-rw-rw-   0        0        0     2874 2022-10-20 01:03:56.000000 django-ipghrms-training-1.0/training/migrations/__pycache__/0001_initial.cpython-37.pyc
--rw-rw-rw-   0        0        0     2889 2022-10-18 10:39:31.000000 django-ipghrms-training-1.0/training/migrations/__pycache__/0001_initial.cpython-39.pyc
--rw-rw-rw-   0        0        0     3320 2022-11-07 13:19:40.000000 django-ipghrms-training-1.0/training/migrations/__pycache__/0002_hrcriteria_trainingemp_tyear_unitcriteria_and_more.cpython-310.pyc
--rw-rw-rw-   0        0        0     3090 2022-11-05 14:52:09.000000 django-ipghrms-training-1.0/training/migrations/__pycache__/0002_hrcriteria_trainingemp_tyear_unitcriteria_and_more.cpython-37.pyc
--rw-rw-rw-   0        0        0      916 2022-11-07 13:19:40.000000 django-ipghrms-training-1.0/training/migrations/__pycache__/0003_rename_fundtype_ttype_delete_trainingtype_and_more.cpython-310.pyc
--rw-rw-rw-   0        0        0      898 2022-11-05 14:52:09.000000 django-ipghrms-training-1.0/training/migrations/__pycache__/0003_rename_fundtype_ttype_delete_trainingtype_and_more.cpython-37.pyc
--rw-rw-rw-   0        0        0      667 2022-11-07 13:19:40.000000 django-ipghrms-training-1.0/training/migrations/__pycache__/0004_trainingplan_duration.cpython-310.pyc
--rw-rw-rw-   0        0        0      653 2022-11-05 14:52:09.000000 django-ipghrms-training-1.0/training/migrations/__pycache__/0004_trainingplan_duration.cpython-37.pyc
--rw-rw-rw-   0        0        0     1634 2022-11-07 13:19:40.000000 django-ipghrms-training-1.0/training/migrations/__pycache__/0005_tcriteria_trainingcriteria_remove_unitcriteria_plan_and_more.cpython-310.pyc
--rw-rw-rw-   0        0        0     1604 2022-11-05 14:52:09.000000 django-ipghrms-training-1.0/training/migrations/__pycache__/0005_tcriteria_trainingcriteria_remove_unitcriteria_plan_and_more.cpython-37.pyc
--rw-rw-rw-   0        0        0      650 2022-11-07 13:19:40.000000 django-ipghrms-training-1.0/training/migrations/__pycache__/0006_alter_tcriteria_subject.cpython-310.pyc
--rw-rw-rw-   0        0        0      636 2022-11-05 14:52:09.000000 django-ipghrms-training-1.0/training/migrations/__pycache__/0006_alter_tcriteria_subject.cpython-37.pyc
--rw-rw-rw-   0        0        0      793 2022-11-07 13:19:40.000000 django-ipghrms-training-1.0/training/migrations/__pycache__/0007_trainingplan_is_approve_trainingplan_is_certify_and_more.cpython-310.pyc
--rw-rw-rw-   0        0        0      773 2022-11-05 14:52:09.000000 django-ipghrms-training-1.0/training/migrations/__pycache__/0007_trainingplan_is_approve_trainingplan_is_certify_and_more.cpython-37.pyc
--rw-rw-rw-   0        0        0     1324 2022-11-07 13:19:40.000000 django-ipghrms-training-1.0/training/migrations/__pycache__/0008_trainingsubject.cpython-310.pyc
--rw-rw-rw-   0        0        0     1308 2022-11-05 14:52:09.000000 django-ipghrms-training-1.0/training/migrations/__pycache__/0008_trainingsubject.cpython-37.pyc
--rw-rw-rw-   0        0        0      701 2022-11-07 13:19:40.000000 django-ipghrms-training-1.0/training/migrations/__pycache__/0009_remove_trainingplan_duration_and_more.cpython-310.pyc
--rw-rw-rw-   0        0        0      677 2022-11-05 14:52:09.000000 django-ipghrms-training-1.0/training/migrations/__pycache__/0009_remove_trainingplan_duration_and_more.cpython-37.pyc
--rw-rw-rw-   0        0        0      850 2022-11-07 13:19:40.000000 django-ipghrms-training-1.0/training/migrations/__pycache__/0010_trainingplan_duration_trainingplan_place_and_more.cpython-310.pyc
--rw-rw-rw-   0        0        0      832 2022-11-05 14:52:09.000000 django-ipghrms-training-1.0/training/migrations/__pycache__/0010_trainingplan_duration_trainingplan_place_and_more.cpython-37.pyc
--rw-rw-rw-   0        0        0      639 2022-11-07 13:19:40.000000 django-ipghrms-training-1.0/training/migrations/__pycache__/0011_remove_trainingemp_hashed_delete_trainingsubject.cpython-310.pyc
--rw-rw-rw-   0        0        0      623 2022-11-05 14:52:09.000000 django-ipghrms-training-1.0/training/migrations/__pycache__/0011_remove_trainingemp_hashed_delete_trainingsubject.cpython-37.pyc
--rw-rw-rw-   0        0        0     1063 2022-11-07 13:19:40.000000 django-ipghrms-training-1.0/training/migrations/__pycache__/0012_trainingemp_diploma_alter_trainingemp_department_and_more.cpython-310.pyc
--rw-rw-rw-   0        0        0     1043 2022-11-05 14:52:09.000000 django-ipghrms-training-1.0/training/migrations/__pycache__/0012_trainingemp_diploma_alter_trainingemp_department_and_more.cpython-37.pyc
--rw-rw-rw-   0        0        0      798 2022-11-07 13:19:40.000000 django-ipghrms-training-1.0/training/migrations/__pycache__/0013_alter_trainingcriteria_criteria.cpython-310.pyc
--rw-rw-rw-   0        0        0      784 2022-11-05 14:52:09.000000 django-ipghrms-training-1.0/training/migrations/__pycache__/0013_alter_trainingcriteria_criteria.cpython-37.pyc
--rw-rw-rw-   0        0        0      604 2022-11-07 13:19:40.000000 django-ipghrms-training-1.0/training/migrations/__pycache__/0014_tcriteria_is_active.cpython-310.pyc
--rw-rw-rw-   0        0        0      590 2022-11-05 14:52:09.000000 django-ipghrms-training-1.0/training/migrations/__pycache__/0014_tcriteria_is_active.cpython-37.pyc
--rw-rw-rw-   0        0        0     1073 2022-12-09 17:27:01.000000 django-ipghrms-training-1.0/training/migrations/__pycache__/0015_auto_20221210_0226.cpython-310.pyc
--rw-rw-rw-   0        0        0      611 2022-12-09 18:16:15.000000 django-ipghrms-training-1.0/training/migrations/__pycache__/0016_trainingemp_is_update.cpython-310.pyc
--rw-rw-rw-   0        0        0     2431 2022-12-10 05:05:46.000000 django-ipghrms-training-1.0/training/migrations/__pycache__/0017_scholarshipplan_sprogress_stype.cpython-310.pyc
--rw-rw-rw-   0        0        0     1061 2022-12-10 05:35:48.000000 django-ipghrms-training-1.0/training/migrations/__pycache__/0018_auto_20221210_1435.cpython-310.pyc
--rw-rw-rw-   0        0        0     1777 2022-12-10 06:30:58.000000 django-ipghrms-training-1.0/training/migrations/__pycache__/0019_scholarshipemp_scholarshipempprogress.cpython-310.pyc
--rw-rw-rw-   0        0        0      569 2022-12-10 06:50:57.000000 django-ipghrms-training-1.0/training/migrations/__pycache__/0020_auto_20221210_1550.cpython-310.pyc
--rw-rw-rw-   0        0        0      589 2022-12-10 07:01:44.000000 django-ipghrms-training-1.0/training/migrations/__pycache__/0021_rename_start_date_scholarshipempprogress_date.cpython-310.pyc
--rw-rw-rw-   0        0        0      803 2022-12-10 07:55:13.000000 django-ipghrms-training-1.0/training/migrations/__pycache__/0022_alter_scholarshipemp_emp.cpython-310.pyc
--rw-rw-rw-   0        0        0      625 2022-12-10 08:37:15.000000 django-ipghrms-training-1.0/training/migrations/__pycache__/0023_scholarshipplan_is_update.cpython-310.pyc
--rw-rw-rw-   0        0        0      680 2022-12-10 08:42:57.000000 django-ipghrms-training-1.0/training/migrations/__pycache__/0024_auto_20221210_1742.cpython-310.pyc
--rw-rw-rw-   0        0        0      875 2023-02-14 03:45:25.000000 django-ipghrms-training-1.0/training/migrations/__pycache__/0025_trainingemp_subject.cpython-310.pyc
--rw-rw-rw-   0        0        0     1193 2023-03-11 04:12:27.000000 django-ipghrms-training-1.0/training/migrations/__pycache__/0026_traininggap.cpython-310.pyc
--rw-rw-rw-   0        0        0      600 2023-03-11 04:25:19.000000 django-ipghrms-training-1.0/training/migrations/__pycache__/0027_traininggap_is_done.cpython-310.pyc
--rw-rw-rw-   0        0        0      756 2023-03-11 04:56:49.000000 django-ipghrms-training-1.0/training/migrations/__pycache__/0028_traininggap_employee.cpython-310.pyc
--rw-rw-rw-   0        0        0      609 2023-03-11 05:24:51.000000 django-ipghrms-training-1.0/training/migrations/__pycache__/0029_traininggap_is_lock.cpython-310.pyc
--rw-rw-rw-   0        0        0     1367 2023-03-11 06:46:39.000000 django-ipghrms-training-1.0/training/migrations/__pycache__/0030_trainingdep_trainingplangap.cpython-310.pyc
--rw-rw-rw-   0        0        0      872 2023-03-11 17:15:33.000000 django-ipghrms-training-1.0/training/migrations/__pycache__/0031_auto_20230312_0215.cpython-310.pyc
--rw-rw-rw-   0        0        0      613 2023-03-12 07:17:32.000000 django-ipghrms-training-1.0/training/migrations/__pycache__/0032_trainingplan_is_update.cpython-310.pyc
--rw-rw-rw-   0        0        0      675 2023-03-12 07:19:47.000000 django-ipghrms-training-1.0/training/migrations/__pycache__/0033_auto_20230312_1619.cpython-310.pyc
--rw-rw-rw-   0        0        0      148 2022-11-07 13:19:40.000000 django-ipghrms-training-1.0/training/migrations/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      146 2022-10-20 01:03:56.000000 django-ipghrms-training-1.0/training/migrations/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0      154 2022-10-18 10:39:31.000000 django-ipghrms-training-1.0/training/migrations/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     9748 2023-03-12 07:19:26.000000 django-ipghrms-training-1.0/training/models.py
--rw-rw-rw-   0        0        0     1429 2022-12-14 13:29:23.000000 django-ipghrms-training-1.0/training/schor_url.py
-drwxrwxrwx   0        0        0        0 2023-03-27 15:20:25.786775 django-ipghrms-training-1.0/training/templates/
-drwxrwxrwx   0        0        0        0 2023-03-27 15:20:26.176900 django-ipghrms-training-1.0/training/templates/gap/
--rw-rw-rw-   0        0        0     6137 2023-03-12 09:39:19.000000 django-ipghrms-training-1.0/training/templates/gap/emp_gap_list.html
--rw-rw-rw-   0        0        0     1008 2023-03-11 04:55:00.000000 django-ipghrms-training-1.0/training/templates/gap/form.html
--rw-rw-rw-   0        0        0     2131 2023-03-11 04:47:10.000000 django-ipghrms-training-1.0/training/templates/gap/list.html
-drwxrwxrwx   0        0        0        0 2023-03-27 15:20:26.208676 django-ipghrms-training-1.0/training/templates/scholariship/
--rw-rw-rw-   0        0        0     5659 2023-02-08 06:35:10.000000 django-ipghrms-training-1.0/training/templates/scholariship/detail.html
--rw-rw-rw-   0        0        0     6083 2022-12-10 09:59:32.000000 django-ipghrms-training-1.0/training/templates/scholariship/emp_detail.html
--rw-rw-rw-   0        0        0     1403 2023-02-15 08:45:30.000000 django-ipghrms-training-1.0/training/templates/scholariship/form.html
--rw-rw-rw-   0        0        0     3962 2023-02-21 00:43:44.000000 django-ipghrms-training-1.0/training/templates/scholariship/list.html
--rw-rw-rw-   0        0        0     9792 2023-02-08 06:38:33.000000 django-ipghrms-training-1.0/training/templates/scholariship/raw_list.html
-drwxrwxrwx   0        0        0        0 2023-03-27 15:20:26.353512 django-ipghrms-training-1.0/training/templates/training/
--rw-rw-rw-   0        0        0     3097 2022-12-13 05:05:48.000000 django-ipghrms-training-1.0/training/templates/training/c_crit_list.html
--rw-rw-rw-   0        0        0     3225 2023-03-11 04:33:00.000000 django-ipghrms-training-1.0/training/templates/training/c_dash.html
--rw-rw-rw-   0        0        0    10413 2023-03-12 05:14:06.000000 django-ipghrms-training-1.0/training/templates/training/c_plan_detail.html
--rw-rw-rw-   0        0        0     3550 2023-03-11 14:55:49.000000 django-ipghrms-training-1.0/training/templates/training/c_plan_list.html
--rw-rw-rw-   0        0        0     7250 2023-03-12 09:59:48.000000 django-ipghrms-training-1.0/training/templates/training/c_raw_data.html
--rw-rw-rw-   0        0        0     3537 2023-02-21 00:39:33.000000 django-ipghrms-training-1.0/training/templates/training/de_dash.html
--rw-rw-rw-   0        0        0     6183 2023-03-12 09:47:03.000000 django-ipghrms-training-1.0/training/templates/training/de_plan_detail.html
--rw-rw-rw-   0        0        0     3179 2023-03-12 09:42:42.000000 django-ipghrms-training-1.0/training/templates/training/de_plan_list.html
--rw-rw-rw-   0        0        0     1746 2023-03-11 15:37:03.000000 django-ipghrms-training-1.0/training/templates/training/form.html
--rw-rw-rw-   0        0        0     1824 2023-03-11 07:29:03.000000 django-ipghrms-training-1.0/training/templates/training/form2.html
--rw-rw-rw-   0        0        0     7902 2022-11-16 15:20:29.000000 django-ipghrms-training-1.0/training/templates/training/hr_crit_list.html
--rw-rw-rw-   0        0        0     3631 2023-02-21 06:19:33.000000 django-ipghrms-training-1.0/training/templates/training/hr_dash.html
--rw-rw-rw-   0        0        0     7402 2023-03-12 07:27:15.000000 django-ipghrms-training-1.0/training/templates/training/hr_plan_detail.html
--rw-rw-rw-   0        0        0     3039 2023-03-12 05:49:58.000000 django-ipghrms-training-1.0/training/templates/training/hr_plan_list.html
--rw-rw-rw-   0        0        0     5407 2023-02-21 00:47:04.000000 django-ipghrms-training-1.0/training/templates/training/raw_data.html
--rw-rw-rw-   0        0        0     6859 2023-02-13 03:44:15.000000 django-ipghrms-training-1.0/training/templates/training/summary.html
--rw-rw-rw-   0        0        0     9222 2022-12-15 13:08:52.000000 django-ipghrms-training-1.0/training/templates/training/summary_year.html
-drwxrwxrwx   0        0        0        0 2023-03-27 15:20:26.388983 django-ipghrms-training-1.0/training/templates/training_chart/
--rw-rw-rw-   0        0        0     1212 2022-11-04 05:28:45.000000 django-ipghrms-training-1.0/training/templates/training_chart/myoption.js
--rw-rw-rw-   0        0        0     2082 2023-02-20 14:59:07.000000 django-ipghrms-training-1.0/training/templates/training_chart/train_dep.js
--rw-rw-rw-   0        0        0     1513 2023-01-23 17:57:18.000000 django-ipghrms-training-1.0/training/templates/training_chart/train_unit.js
--rw-rw-rw-   0        0        0     2087 2023-02-20 02:08:50.000000 django-ipghrms-training-1.0/training/templates/training_chart/train_year.js
--rw-rw-rw-   0        0        0       60 2022-10-18 10:39:31.000000 django-ipghrms-training-1.0/training/tests.py
--rw-rw-rw-   0        0        0     4148 2023-03-12 09:41:07.000000 django-ipghrms-training-1.0/training/urls.py
--rw-rw-rw-   0        0        0      468 2023-02-14 03:44:01.000000 django-ipghrms-training-1.0/training/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-27 15:20:26.406922 django-ipghrms-training-1.0/training/views/
--rw-rw-rw-   0        0        0       95 2022-12-10 06:41:27.000000 django-ipghrms-training-1.0/training/views/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-27 15:20:26.444672 django-ipghrms-training-1.0/training/views/__pycache__/
--rw-rw-rw-   0        0        0      226 2022-12-10 06:41:31.000000 django-ipghrms-training-1.0/training/views/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      190 2022-11-05 14:51:39.000000 django-ipghrms-training-1.0/training/views/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0     6979 2023-02-15 09:15:38.000000 django-ipghrms-training-1.0/training/views/__pycache__/m_scho.cpython-310.pyc
--rw-rw-rw-   0        0        0    10682 2023-03-12 05:34:38.000000 django-ipghrms-training-1.0/training/views/__pycache__/training_m.cpython-310.pyc
--rw-rw-rw-   0        0        0     8767 2022-11-05 14:51:39.000000 django-ipghrms-training-1.0/training/views/__pycache__/training_m.cpython-37.pyc
--rw-rw-rw-   0        0        0    13531 2023-03-12 09:54:15.000000 django-ipghrms-training-1.0/training/views/__pycache__/training_v.cpython-310.pyc
--rw-rw-rw-   0        0        0     6057 2022-11-05 14:51:39.000000 django-ipghrms-training-1.0/training/views/__pycache__/training_v.cpython-37.pyc
--rw-rw-rw-   0        0        0     3055 2023-02-21 00:44:25.000000 django-ipghrms-training-1.0/training/views/__pycache__/v_scho.cpython-310.pyc
--rw-rw-rw-   0        0        0    10124 2023-02-15 09:15:33.000000 django-ipghrms-training-1.0/training/views/m_scho.py
--rw-rw-rw-   0        0        0    15361 2023-03-12 05:34:34.000000 django-ipghrms-training-1.0/training/views/training_m.py
--rw-rw-rw-   0        0        0    17355 2023-03-12 09:54:11.000000 django-ipghrms-training-1.0/training/views/training_v.py
--rw-rw-rw-   0        0        0     3399 2023-02-21 00:44:21.000000 django-ipghrms-training-1.0/training/views/v_scho.py
--rw-rw-rw-   0        0        0       63 2022-10-18 10:39:31.000000 django-ipghrms-training-1.0/training/views.py
+drwxrwxrwx   0        0        0        0 2023-06-21 14:35:32.614211 django-ipghrms-training-1.1/
+-rw-rw-rw-   0        0        0     1068 2023-03-27 15:20:00.000000 django-ipghrms-training-1.1/LICENSE
+-rw-rw-rw-   0        0        0      186 2023-03-27 14:32:07.000000 django-ipghrms-training-1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      951 2023-06-21 14:35:32.614211 django-ipghrms-training-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      503 2023-03-27 14:32:12.000000 django-ipghrms-training-1.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-21 14:35:31.118128 django-ipghrms-training-1.1/django_ipghrms_training.egg-info/
+-rw-rw-rw-   0        0        0      951 2023-06-21 14:35:30.000000 django-ipghrms-training-1.1/django_ipghrms_training.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8630 2023-06-21 14:35:30.000000 django-ipghrms-training-1.1/django_ipghrms_training.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 14:35:30.000000 django-ipghrms-training-1.1/django_ipghrms_training.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-21 14:35:30.000000 django-ipghrms-training-1.1/django_ipghrms_training.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      511 2023-06-21 14:35:32.633906 django-ipghrms-training-1.1/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-03-22 07:44:49.000000 django-ipghrms-training-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 14:35:31.166506 django-ipghrms-training-1.1/training/
+-rw-rw-rw-   0        0        0        0 2022-10-18 10:39:31.000000 django-ipghrms-training-1.1/training/__init__.py
+-rw-rw-rw-   0        0        0      772 2023-03-11 06:48:13.000000 django-ipghrms-training-1.1/training/admin.py
+drwxrwxrwx   0        0        0        0 2023-06-21 14:35:31.177518 django-ipghrms-training-1.1/training/api/
+drwxrwxrwx   0        0        0        0 2023-06-21 14:35:31.199613 django-ipghrms-training-1.1/training/api/__pycache__/
+-rw-rw-rw-   0        0        0      349 2022-11-07 13:19:38.000000 django-ipghrms-training-1.1/training/api/__pycache__/urls.cpython-310.pyc
+-rw-rw-rw-   0        0        0      345 2022-11-05 14:51:39.000000 django-ipghrms-training-1.1/training/api/__pycache__/urls.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2772 2023-03-12 10:06:03.000000 django-ipghrms-training-1.1/training/api/__pycache__/views.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2751 2022-11-05 14:51:39.000000 django-ipghrms-training-1.1/training/api/__pycache__/views.cpython-37.pyc
+-rw-rw-rw-   0        0        0      203 2022-11-04 05:28:45.000000 django-ipghrms-training-1.1/training/api/urls.py
+-rw-rw-rw-   0        0        0     2510 2023-06-21 14:32:28.000000 django-ipghrms-training-1.1/training/api/views.py
+-rw-rw-rw-   0        0        0      148 2022-10-18 10:39:31.000000 django-ipghrms-training-1.1/training/apps.py
+-rw-rw-rw-   0        0        0    10676 2023-03-12 05:28:12.000000 django-ipghrms-training-1.1/training/forms.py
+drwxrwxrwx   0        0        0        0 2023-06-21 14:35:31.372642 django-ipghrms-training-1.1/training/migrations/
+-rw-rw-rw-   0        0        0     6057 2022-10-18 10:39:31.000000 django-ipghrms-training-1.1/training/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0     7595 2022-11-04 05:28:45.000000 django-ipghrms-training-1.1/training/migrations/0002_hrcriteria_trainingemp_tyear_unitcriteria_and_more.py
+-rw-rw-rw-   0        0        0      730 2022-11-04 05:28:45.000000 django-ipghrms-training-1.1/training/migrations/0003_rename_fundtype_ttype_delete_trainingtype_and_more.py
+-rw-rw-rw-   0        0        0      467 2022-11-04 05:28:45.000000 django-ipghrms-training-1.1/training/migrations/0004_trainingplan_duration.py
+-rw-rw-rw-   0        0        0     2249 2022-11-04 05:28:45.000000 django-ipghrms-training-1.1/training/migrations/0005_tcriteria_trainingcriteria_remove_unitcriteria_plan_and_more.py
+-rw-rw-rw-   0        0        0      443 2022-11-04 05:28:45.000000 django-ipghrms-training-1.1/training/migrations/0006_alter_tcriteria_subject.py
+-rw-rw-rw-   0        0        0      979 2022-11-04 05:28:45.000000 django-ipghrms-training-1.1/training/migrations/0007_trainingplan_is_approve_trainingplan_is_certify_and_more.py
+-rw-rw-rw-   0        0        0     1402 2022-11-04 05:28:45.000000 django-ipghrms-training-1.1/training/migrations/0008_trainingsubject.py
+-rw-rw-rw-   0        0        0      886 2022-11-04 05:28:45.000000 django-ipghrms-training-1.1/training/migrations/0009_remove_trainingplan_duration_and_more.py
+-rw-rw-rw-   0        0        0      872 2022-11-04 05:28:45.000000 django-ipghrms-training-1.1/training/migrations/0010_trainingplan_duration_trainingplan_place_and_more.py
+-rw-rw-rw-   0        0        0      442 2022-11-04 05:28:45.000000 django-ipghrms-training-1.1/training/migrations/0011_remove_trainingemp_hashed_delete_trainingsubject.py
+-rw-rw-rw-   0        0        0     1386 2022-11-04 05:28:45.000000 django-ipghrms-training-1.1/training/migrations/0012_trainingemp_diploma_alter_trainingemp_department_and_more.py
+-rw-rw-rw-   0        0        0      583 2022-11-04 05:28:45.000000 django-ipghrms-training-1.1/training/migrations/0013_alter_trainingcriteria_criteria.py
+-rw-rw-rw-   0        0        0      404 2022-11-04 05:28:45.000000 django-ipghrms-training-1.1/training/migrations/0014_tcriteria_is_active.py
+-rw-rw-rw-   0        0        0     1254 2022-12-09 17:26:57.000000 django-ipghrms-training-1.1/training/migrations/0015_auto_20221210_0226.py
+-rw-rw-rw-   0        0        0      435 2022-12-09 18:16:10.000000 django-ipghrms-training-1.1/training/migrations/0016_trainingemp_is_update.py
+-rw-rw-rw-   0        0        0     3780 2022-12-10 05:05:40.000000 django-ipghrms-training-1.1/training/migrations/0017_scholarshipplan_sprogress_stype.py
+-rw-rw-rw-   0        0        0     1262 2022-12-10 05:35:42.000000 django-ipghrms-training-1.1/training/migrations/0018_auto_20221210_1435.py
+-rw-rw-rw-   0        0        0     2568 2022-12-10 06:30:52.000000 django-ipghrms-training-1.1/training/migrations/0019_scholarshipemp_scholarshipempprogress.py
+-rw-rw-rw-   0        0        0      483 2022-12-10 06:50:52.000000 django-ipghrms-training-1.1/training/migrations/0020_auto_20221210_1550.py
+-rw-rw-rw-   0        0        0      398 2022-12-10 07:01:38.000000 django-ipghrms-training-1.1/training/migrations/0021_rename_start_date_scholarshipempprogress_date.py
+-rw-rw-rw-   0        0        0      623 2022-12-10 07:55:09.000000 django-ipghrms-training-1.1/training/migrations/0022_alter_scholarshipemp_emp.py
+-rw-rw-rw-   0        0        0      445 2022-12-10 08:37:10.000000 django-ipghrms-training-1.1/training/migrations/0023_scholarshipplan_is_update.py
+-rw-rw-rw-   0        0        0      564 2022-12-10 08:42:50.000000 django-ipghrms-training-1.1/training/migrations/0024_auto_20221210_1742.py
+-rw-rw-rw-   0        0        0      660 2023-02-14 03:45:18.000000 django-ipghrms-training-1.1/training/migrations/0025_trainingemp_subject.py
+-rw-rw-rw-   0        0        0     1196 2023-03-11 04:12:21.000000 django-ipghrms-training-1.1/training/migrations/0026_traininggap.py
+-rw-rw-rw-   0        0        0      426 2023-03-11 04:25:14.000000 django-ipghrms-training-1.1/training/migrations/0027_traininggap_is_done.py
+-rw-rw-rw-   0        0        0      576 2023-03-11 04:56:44.000000 django-ipghrms-training-1.1/training/migrations/0028_traininggap_employee.py
+-rw-rw-rw-   0        0        0      435 2023-03-11 05:24:46.000000 django-ipghrms-training-1.1/training/migrations/0029_traininggap_is_lock.py
+-rw-rw-rw-   0        0        0     1928 2023-03-11 06:46:35.000000 django-ipghrms-training-1.1/training/migrations/0030_trainingdep_trainingplangap.py
+-rw-rw-rw-   0        0        0      891 2023-03-11 17:15:26.000000 django-ipghrms-training-1.1/training/migrations/0031_auto_20230312_0215.py
+-rw-rw-rw-   0        0        0      436 2023-03-12 07:17:20.000000 django-ipghrms-training-1.1/training/migrations/0032_trainingplan_is_update.py
+-rw-rw-rw-   0        0        0      559 2023-03-12 07:19:34.000000 django-ipghrms-training-1.1/training/migrations/0033_auto_20230312_1619.py
+-rw-rw-rw-   0        0        0        0 2022-10-18 10:39:31.000000 django-ipghrms-training-1.1/training/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 14:35:31.713835 django-ipghrms-training-1.1/training/migrations/__pycache__/
+-rw-rw-rw-   0        0        0     2885 2022-11-07 13:19:40.000000 django-ipghrms-training-1.1/training/migrations/__pycache__/0001_initial.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2874 2022-10-20 01:03:56.000000 django-ipghrms-training-1.1/training/migrations/__pycache__/0001_initial.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2889 2022-10-18 10:39:31.000000 django-ipghrms-training-1.1/training/migrations/__pycache__/0001_initial.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3320 2022-11-07 13:19:40.000000 django-ipghrms-training-1.1/training/migrations/__pycache__/0002_hrcriteria_trainingemp_tyear_unitcriteria_and_more.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3090 2022-11-05 14:52:09.000000 django-ipghrms-training-1.1/training/migrations/__pycache__/0002_hrcriteria_trainingemp_tyear_unitcriteria_and_more.cpython-37.pyc
+-rw-rw-rw-   0        0        0      916 2022-11-07 13:19:40.000000 django-ipghrms-training-1.1/training/migrations/__pycache__/0003_rename_fundtype_ttype_delete_trainingtype_and_more.cpython-310.pyc
+-rw-rw-rw-   0        0        0      898 2022-11-05 14:52:09.000000 django-ipghrms-training-1.1/training/migrations/__pycache__/0003_rename_fundtype_ttype_delete_trainingtype_and_more.cpython-37.pyc
+-rw-rw-rw-   0        0        0      667 2022-11-07 13:19:40.000000 django-ipghrms-training-1.1/training/migrations/__pycache__/0004_trainingplan_duration.cpython-310.pyc
+-rw-rw-rw-   0        0        0      653 2022-11-05 14:52:09.000000 django-ipghrms-training-1.1/training/migrations/__pycache__/0004_trainingplan_duration.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1634 2022-11-07 13:19:40.000000 django-ipghrms-training-1.1/training/migrations/__pycache__/0005_tcriteria_trainingcriteria_remove_unitcriteria_plan_and_more.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1604 2022-11-05 14:52:09.000000 django-ipghrms-training-1.1/training/migrations/__pycache__/0005_tcriteria_trainingcriteria_remove_unitcriteria_plan_and_more.cpython-37.pyc
+-rw-rw-rw-   0        0        0      650 2022-11-07 13:19:40.000000 django-ipghrms-training-1.1/training/migrations/__pycache__/0006_alter_tcriteria_subject.cpython-310.pyc
+-rw-rw-rw-   0        0        0      636 2022-11-05 14:52:09.000000 django-ipghrms-training-1.1/training/migrations/__pycache__/0006_alter_tcriteria_subject.cpython-37.pyc
+-rw-rw-rw-   0        0        0      793 2022-11-07 13:19:40.000000 django-ipghrms-training-1.1/training/migrations/__pycache__/0007_trainingplan_is_approve_trainingplan_is_certify_and_more.cpython-310.pyc
+-rw-rw-rw-   0        0        0      773 2022-11-05 14:52:09.000000 django-ipghrms-training-1.1/training/migrations/__pycache__/0007_trainingplan_is_approve_trainingplan_is_certify_and_more.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1324 2022-11-07 13:19:40.000000 django-ipghrms-training-1.1/training/migrations/__pycache__/0008_trainingsubject.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1308 2022-11-05 14:52:09.000000 django-ipghrms-training-1.1/training/migrations/__pycache__/0008_trainingsubject.cpython-37.pyc
+-rw-rw-rw-   0        0        0      701 2022-11-07 13:19:40.000000 django-ipghrms-training-1.1/training/migrations/__pycache__/0009_remove_trainingplan_duration_and_more.cpython-310.pyc
+-rw-rw-rw-   0        0        0      677 2022-11-05 14:52:09.000000 django-ipghrms-training-1.1/training/migrations/__pycache__/0009_remove_trainingplan_duration_and_more.cpython-37.pyc
+-rw-rw-rw-   0        0        0      850 2022-11-07 13:19:40.000000 django-ipghrms-training-1.1/training/migrations/__pycache__/0010_trainingplan_duration_trainingplan_place_and_more.cpython-310.pyc
+-rw-rw-rw-   0        0        0      832 2022-11-05 14:52:09.000000 django-ipghrms-training-1.1/training/migrations/__pycache__/0010_trainingplan_duration_trainingplan_place_and_more.cpython-37.pyc
+-rw-rw-rw-   0        0        0      639 2022-11-07 13:19:40.000000 django-ipghrms-training-1.1/training/migrations/__pycache__/0011_remove_trainingemp_hashed_delete_trainingsubject.cpython-310.pyc
+-rw-rw-rw-   0        0        0      623 2022-11-05 14:52:09.000000 django-ipghrms-training-1.1/training/migrations/__pycache__/0011_remove_trainingemp_hashed_delete_trainingsubject.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1063 2022-11-07 13:19:40.000000 django-ipghrms-training-1.1/training/migrations/__pycache__/0012_trainingemp_diploma_alter_trainingemp_department_and_more.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1043 2022-11-05 14:52:09.000000 django-ipghrms-training-1.1/training/migrations/__pycache__/0012_trainingemp_diploma_alter_trainingemp_department_and_more.cpython-37.pyc
+-rw-rw-rw-   0        0        0      798 2022-11-07 13:19:40.000000 django-ipghrms-training-1.1/training/migrations/__pycache__/0013_alter_trainingcriteria_criteria.cpython-310.pyc
+-rw-rw-rw-   0        0        0      784 2022-11-05 14:52:09.000000 django-ipghrms-training-1.1/training/migrations/__pycache__/0013_alter_trainingcriteria_criteria.cpython-37.pyc
+-rw-rw-rw-   0        0        0      604 2022-11-07 13:19:40.000000 django-ipghrms-training-1.1/training/migrations/__pycache__/0014_tcriteria_is_active.cpython-310.pyc
+-rw-rw-rw-   0        0        0      590 2022-11-05 14:52:09.000000 django-ipghrms-training-1.1/training/migrations/__pycache__/0014_tcriteria_is_active.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1073 2022-12-09 17:27:01.000000 django-ipghrms-training-1.1/training/migrations/__pycache__/0015_auto_20221210_0226.cpython-310.pyc
+-rw-rw-rw-   0        0        0      611 2022-12-09 18:16:15.000000 django-ipghrms-training-1.1/training/migrations/__pycache__/0016_trainingemp_is_update.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2431 2022-12-10 05:05:46.000000 django-ipghrms-training-1.1/training/migrations/__pycache__/0017_scholarshipplan_sprogress_stype.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1061 2022-12-10 05:35:48.000000 django-ipghrms-training-1.1/training/migrations/__pycache__/0018_auto_20221210_1435.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1777 2022-12-10 06:30:58.000000 django-ipghrms-training-1.1/training/migrations/__pycache__/0019_scholarshipemp_scholarshipempprogress.cpython-310.pyc
+-rw-rw-rw-   0        0        0      569 2022-12-10 06:50:57.000000 django-ipghrms-training-1.1/training/migrations/__pycache__/0020_auto_20221210_1550.cpython-310.pyc
+-rw-rw-rw-   0        0        0      589 2022-12-10 07:01:44.000000 django-ipghrms-training-1.1/training/migrations/__pycache__/0021_rename_start_date_scholarshipempprogress_date.cpython-310.pyc
+-rw-rw-rw-   0        0        0      803 2022-12-10 07:55:13.000000 django-ipghrms-training-1.1/training/migrations/__pycache__/0022_alter_scholarshipemp_emp.cpython-310.pyc
+-rw-rw-rw-   0        0        0      625 2022-12-10 08:37:15.000000 django-ipghrms-training-1.1/training/migrations/__pycache__/0023_scholarshipplan_is_update.cpython-310.pyc
+-rw-rw-rw-   0        0        0      680 2022-12-10 08:42:57.000000 django-ipghrms-training-1.1/training/migrations/__pycache__/0024_auto_20221210_1742.cpython-310.pyc
+-rw-rw-rw-   0        0        0      875 2023-02-14 03:45:25.000000 django-ipghrms-training-1.1/training/migrations/__pycache__/0025_trainingemp_subject.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1193 2023-03-11 04:12:27.000000 django-ipghrms-training-1.1/training/migrations/__pycache__/0026_traininggap.cpython-310.pyc
+-rw-rw-rw-   0        0        0      600 2023-03-11 04:25:19.000000 django-ipghrms-training-1.1/training/migrations/__pycache__/0027_traininggap_is_done.cpython-310.pyc
+-rw-rw-rw-   0        0        0      756 2023-03-11 04:56:49.000000 django-ipghrms-training-1.1/training/migrations/__pycache__/0028_traininggap_employee.cpython-310.pyc
+-rw-rw-rw-   0        0        0      609 2023-03-11 05:24:51.000000 django-ipghrms-training-1.1/training/migrations/__pycache__/0029_traininggap_is_lock.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1367 2023-03-11 06:46:39.000000 django-ipghrms-training-1.1/training/migrations/__pycache__/0030_trainingdep_trainingplangap.cpython-310.pyc
+-rw-rw-rw-   0        0        0      872 2023-03-11 17:15:33.000000 django-ipghrms-training-1.1/training/migrations/__pycache__/0031_auto_20230312_0215.cpython-310.pyc
+-rw-rw-rw-   0        0        0      613 2023-03-12 07:17:32.000000 django-ipghrms-training-1.1/training/migrations/__pycache__/0032_trainingplan_is_update.cpython-310.pyc
+-rw-rw-rw-   0        0        0      675 2023-03-12 07:19:47.000000 django-ipghrms-training-1.1/training/migrations/__pycache__/0033_auto_20230312_1619.cpython-310.pyc
+-rw-rw-rw-   0        0        0      148 2022-11-07 13:19:40.000000 django-ipghrms-training-1.1/training/migrations/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      146 2022-10-20 01:03:56.000000 django-ipghrms-training-1.1/training/migrations/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0      154 2022-10-18 10:39:31.000000 django-ipghrms-training-1.1/training/migrations/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     9748 2023-03-12 07:19:26.000000 django-ipghrms-training-1.1/training/models.py
+-rw-rw-rw-   0        0        0     1429 2022-12-14 13:29:23.000000 django-ipghrms-training-1.1/training/schor_url.py
+drwxrwxrwx   0        0        0        0 2023-06-21 14:35:31.060479 django-ipghrms-training-1.1/training/templates/
+drwxrwxrwx   0        0        0        0 2023-06-21 14:35:31.769298 django-ipghrms-training-1.1/training/templates/gap/
+-rw-rw-rw-   0        0        0     6137 2023-03-12 09:39:19.000000 django-ipghrms-training-1.1/training/templates/gap/emp_gap_list.html
+-rw-rw-rw-   0        0        0     1008 2023-03-11 04:55:00.000000 django-ipghrms-training-1.1/training/templates/gap/form.html
+-rw-rw-rw-   0        0        0     2131 2023-03-11 04:47:10.000000 django-ipghrms-training-1.1/training/templates/gap/list.html
+drwxrwxrwx   0        0        0        0 2023-06-21 14:35:31.928499 django-ipghrms-training-1.1/training/templates/scholariship/
+-rw-rw-rw-   0        0        0     5659 2023-02-08 06:35:10.000000 django-ipghrms-training-1.1/training/templates/scholariship/detail.html
+-rw-rw-rw-   0        0        0     6083 2022-12-10 09:59:32.000000 django-ipghrms-training-1.1/training/templates/scholariship/emp_detail.html
+-rw-rw-rw-   0        0        0     1403 2023-02-15 08:45:30.000000 django-ipghrms-training-1.1/training/templates/scholariship/form.html
+-rw-rw-rw-   0        0        0     3962 2023-02-21 00:43:44.000000 django-ipghrms-training-1.1/training/templates/scholariship/list.html
+-rw-rw-rw-   0        0        0     9792 2023-02-08 06:38:33.000000 django-ipghrms-training-1.1/training/templates/scholariship/raw_list.html
+drwxrwxrwx   0        0        0        0 2023-06-21 14:35:32.433998 django-ipghrms-training-1.1/training/templates/training/
+-rw-rw-rw-   0        0        0     3097 2022-12-13 05:05:48.000000 django-ipghrms-training-1.1/training/templates/training/c_crit_list.html
+-rw-rw-rw-   0        0        0     3225 2023-03-11 04:33:00.000000 django-ipghrms-training-1.1/training/templates/training/c_dash.html
+-rw-rw-rw-   0        0        0    10413 2023-03-12 05:14:06.000000 django-ipghrms-training-1.1/training/templates/training/c_plan_detail.html
+-rw-rw-rw-   0        0        0     3550 2023-03-11 14:55:49.000000 django-ipghrms-training-1.1/training/templates/training/c_plan_list.html
+-rw-rw-rw-   0        0        0     7250 2023-03-12 09:59:48.000000 django-ipghrms-training-1.1/training/templates/training/c_raw_data.html
+-rw-rw-rw-   0        0        0     3537 2023-02-21 00:39:33.000000 django-ipghrms-training-1.1/training/templates/training/de_dash.html
+-rw-rw-rw-   0        0        0     6183 2023-03-12 09:47:03.000000 django-ipghrms-training-1.1/training/templates/training/de_plan_detail.html
+-rw-rw-rw-   0        0        0     3179 2023-03-12 09:42:42.000000 django-ipghrms-training-1.1/training/templates/training/de_plan_list.html
+-rw-rw-rw-   0        0        0     1746 2023-03-11 15:37:03.000000 django-ipghrms-training-1.1/training/templates/training/form.html
+-rw-rw-rw-   0        0        0     1824 2023-03-11 07:29:03.000000 django-ipghrms-training-1.1/training/templates/training/form2.html
+-rw-rw-rw-   0        0        0     7902 2022-11-16 15:20:29.000000 django-ipghrms-training-1.1/training/templates/training/hr_crit_list.html
+-rw-rw-rw-   0        0        0     3631 2023-02-21 06:19:33.000000 django-ipghrms-training-1.1/training/templates/training/hr_dash.html
+-rw-rw-rw-   0        0        0     7402 2023-03-12 07:27:15.000000 django-ipghrms-training-1.1/training/templates/training/hr_plan_detail.html
+-rw-rw-rw-   0        0        0     9107 2023-06-21 14:32:52.000000 django-ipghrms-training-1.1/training/templates/training/hr_plan_list.html
+-rw-rw-rw-   0        0        0     5407 2023-02-21 00:47:04.000000 django-ipghrms-training-1.1/training/templates/training/raw_data.html
+-rw-rw-rw-   0        0        0     6859 2023-02-13 03:44:15.000000 django-ipghrms-training-1.1/training/templates/training/summary.html
+-rw-rw-rw-   0        0        0     9222 2022-12-15 13:08:52.000000 django-ipghrms-training-1.1/training/templates/training/summary_year.html
+drwxrwxrwx   0        0        0        0 2023-06-21 14:35:32.492101 django-ipghrms-training-1.1/training/templates/training_chart/
+-rw-rw-rw-   0        0        0     1212 2022-11-04 05:28:45.000000 django-ipghrms-training-1.1/training/templates/training_chart/myoption.js
+-rw-rw-rw-   0        0        0     2082 2023-02-20 14:59:07.000000 django-ipghrms-training-1.1/training/templates/training_chart/train_dep.js
+-rw-rw-rw-   0        0        0     1513 2023-01-23 17:57:18.000000 django-ipghrms-training-1.1/training/templates/training_chart/train_unit.js
+-rw-rw-rw-   0        0        0     2087 2023-02-20 02:08:50.000000 django-ipghrms-training-1.1/training/templates/training_chart/train_year.js
+-rw-rw-rw-   0        0        0       60 2022-10-18 10:39:31.000000 django-ipghrms-training-1.1/training/tests.py
+-rw-rw-rw-   0        0        0     4148 2023-03-12 09:41:07.000000 django-ipghrms-training-1.1/training/urls.py
+-rw-rw-rw-   0        0        0      468 2023-02-14 03:44:01.000000 django-ipghrms-training-1.1/training/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-21 14:35:32.529078 django-ipghrms-training-1.1/training/views/
+-rw-rw-rw-   0        0        0       95 2022-12-10 06:41:27.000000 django-ipghrms-training-1.1/training/views/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 14:35:32.610305 django-ipghrms-training-1.1/training/views/__pycache__/
+-rw-rw-rw-   0        0        0      226 2022-12-10 06:41:31.000000 django-ipghrms-training-1.1/training/views/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      190 2022-11-05 14:51:39.000000 django-ipghrms-training-1.1/training/views/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0     6979 2023-02-15 09:15:38.000000 django-ipghrms-training-1.1/training/views/__pycache__/m_scho.cpython-310.pyc
+-rw-rw-rw-   0        0        0    10682 2023-03-12 05:34:38.000000 django-ipghrms-training-1.1/training/views/__pycache__/training_m.cpython-310.pyc
+-rw-rw-rw-   0        0        0     8767 2022-11-05 14:51:39.000000 django-ipghrms-training-1.1/training/views/__pycache__/training_m.cpython-37.pyc
+-rw-rw-rw-   0        0        0    13531 2023-03-12 09:54:15.000000 django-ipghrms-training-1.1/training/views/__pycache__/training_v.cpython-310.pyc
+-rw-rw-rw-   0        0        0     6057 2022-11-05 14:51:39.000000 django-ipghrms-training-1.1/training/views/__pycache__/training_v.cpython-37.pyc
+-rw-rw-rw-   0        0        0     3055 2023-02-21 00:44:25.000000 django-ipghrms-training-1.1/training/views/__pycache__/v_scho.cpython-310.pyc
+-rw-rw-rw-   0        0        0    10124 2023-02-15 09:15:33.000000 django-ipghrms-training-1.1/training/views/m_scho.py
+-rw-rw-rw-   0        0        0    15361 2023-03-12 05:34:34.000000 django-ipghrms-training-1.1/training/views/training_m.py
+-rw-rw-rw-   0        0        0    17756 2023-06-21 14:33:26.000000 django-ipghrms-training-1.1/training/views/training_v.py
+-rw-rw-rw-   0        0        0     3399 2023-02-21 00:44:21.000000 django-ipghrms-training-1.1/training/views/v_scho.py
+-rw-rw-rw-   0        0        0       63 2022-10-18 10:39:31.000000 django-ipghrms-training-1.1/training/views.py
```

### Comparing `django-ipghrms-training-1.0/LICENSE` & `django-ipghrms-training-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/PKG-INFO` & `django-ipghrms-training-1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ipghrms-training
-Version: 1.0
+Version: 1.1
 Summary: Django IPG HRMS APP training
 Home-page: http://ipg.tl/
 Author: Kinos
 Author-email: info@kinos.tl
 Maintainer: kinos
 Maintainer-email: info@kinos.tl
 License: MIT
```

### Comparing `django-ipghrms-training-1.0/django_ipghrms_training.egg-info/PKG-INFO` & `django-ipghrms-training-1.1/django_ipghrms_training.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ipghrms-training
-Version: 1.0
+Version: 1.1
 Summary: Django IPG HRMS APP training
 Home-page: http://ipg.tl/
 Author: Kinos
 Author-email: info@kinos.tl
 Maintainer: kinos
 Maintainer-email: info@kinos.tl
 License: MIT
```

### Comparing `django-ipghrms-training-1.0/django_ipghrms_training.egg-info/SOURCES.txt` & `django-ipghrms-training-1.1/django_ipghrms_training.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/admin.py` & `django-ipghrms-training-1.1/training/admin.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/api/__pycache__/views.cpython-310.pyc` & `django-ipghrms-training-1.1/training/api/__pycache__/views.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/api/__pycache__/views.cpython-37.pyc` & `django-ipghrms-training-1.1/training/api/__pycache__/views.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/api/views.py` & `django-ipghrms-training-1.1/training/api/views.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,49 +16,49 @@
 		group = request.user.groups.all()[0].name
 		years = TrainingPlan.objects.filter().distinct().values('year__year').all()
 		obj,label = list(),list()
 		for i in years:
 			objects = []
 			if group == 'unit':
 				_, unit = c_unit(request.user)
-				objects = TrainingPlan.objects.filter((Q(unit=unit)|Q(dep__unit=unit))).all().count()
+				objects = TrainingPlan.objects.filter((Q(unit=unit)|Q(dep__unit=unit)), is_approve=True).all().count()
 			else:
-				objects = TrainingPlan.objects.filter().all().count()
+				objects = TrainingPlan.objects.filter(is_approve=True).all().count()
 			label.append(i['year__year'])
 			# obj.append(objects)
 			obj.append(objects)
-		data = { 'legend': 'DISTRIBUISAUN FUNSIONARIO TUIR TREINAMENTO KADA TINAN', 'obj': obj,  'label':label}
+		data = { 'legend': 'DISTRIBUISAUN TREINAMENTO KADA TINAN', 'obj': obj,  'label':label}
 		return Response(data)
 
 class APITrainDep(APIView):
 	authentication_classes = [SessionAuthentication, BasicAuthentication]
 	permission_classes = [IsAuthenticated]
 	def get(self, request, format=None):
 		group = request.user.groups.all()[0].name
 		label= list()
 		obj = list()
-		legend = 'DISTRIBUISAUN FUNSIONARIO TUIR TREINAMENTO KADA EKIPA'
+		legend = 'DISTRIBUISAUN  TREINAMENTO TUIR EKIPA'
 		if group == 'unit':
 			_, unit = c_unit(request.user)
 			deps = Department.objects.filter(unit=unit).all()
 		else:
 			deps = Department.objects.filter().all()
 		for i in deps:
-			objects = TrainingDep.objects.filter(department=i).all().count()
+			objects = TrainingDep.objects.filter(plan__is_approve=True,department=i).all().count()
 			label.append(i.name)
 			obj.append(objects)
 		data = { 'legend':legend, 'label': label, 'obj': obj, }
 		return Response(data)
 
 class APITrainUnit(APIView):
 	authentication_classes = [SessionAuthentication, BasicAuthentication]
 	permission_classes = [IsAuthenticated]
 	def get(self, request, format=None):
 		group = request.user.groups.all()[0].name
 		units = Unit.objects.filter().all()
 		obj,label = [],[]
 		for i in units:
-			objects = TrainingPlan.objects.filter(unit=i).all().count()
+			objects = TrainingPlan.objects.filter(is_approve=True,unit=i).all().count()
 			label.append(i.name)
 			obj.append(objects)
 		data = { 'label': label, 'obj': obj, }
 		return Response(data)
```

### Comparing `django-ipghrms-training-1.0/training/forms.py` & `django-ipghrms-training-1.1/training/forms.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/0001_initial.py` & `django-ipghrms-training-1.1/training/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/0002_hrcriteria_trainingemp_tyear_unitcriteria_and_more.py` & `django-ipghrms-training-1.1/training/migrations/0002_hrcriteria_trainingemp_tyear_unitcriteria_and_more.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/0003_rename_fundtype_ttype_delete_trainingtype_and_more.py` & `django-ipghrms-training-1.1/training/migrations/0003_rename_fundtype_ttype_delete_trainingtype_and_more.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/0005_tcriteria_trainingcriteria_remove_unitcriteria_plan_and_more.py` & `django-ipghrms-training-1.1/training/migrations/0005_tcriteria_trainingcriteria_remove_unitcriteria_plan_and_more.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/0007_trainingplan_is_approve_trainingplan_is_certify_and_more.py` & `django-ipghrms-training-1.1/training/migrations/0007_trainingplan_is_approve_trainingplan_is_certify_and_more.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/0008_trainingsubject.py` & `django-ipghrms-training-1.1/training/migrations/0008_trainingsubject.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/0009_remove_trainingplan_duration_and_more.py` & `django-ipghrms-training-1.1/training/migrations/0009_remove_trainingplan_duration_and_more.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/0010_trainingplan_duration_trainingplan_place_and_more.py` & `django-ipghrms-training-1.1/training/migrations/0010_trainingplan_duration_trainingplan_place_and_more.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/0012_trainingemp_diploma_alter_trainingemp_department_and_more.py` & `django-ipghrms-training-1.1/training/migrations/0012_trainingemp_diploma_alter_trainingemp_department_and_more.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/0013_alter_trainingcriteria_criteria.py` & `django-ipghrms-training-1.1/training/migrations/0013_alter_trainingcriteria_criteria.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/0015_auto_20221210_0226.py` & `django-ipghrms-training-1.1/training/migrations/0015_auto_20221210_0226.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/0017_scholarshipplan_sprogress_stype.py` & `django-ipghrms-training-1.1/training/migrations/0017_scholarshipplan_sprogress_stype.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/0018_auto_20221210_1435.py` & `django-ipghrms-training-1.1/training/migrations/0018_auto_20221210_1435.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/0019_scholarshipemp_scholarshipempprogress.py` & `django-ipghrms-training-1.1/training/migrations/0019_scholarshipemp_scholarshipempprogress.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/0022_alter_scholarshipemp_emp.py` & `django-ipghrms-training-1.1/training/migrations/0022_alter_scholarshipemp_emp.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/0024_auto_20221210_1742.py` & `django-ipghrms-training-1.1/training/migrations/0024_auto_20221210_1742.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/0025_trainingemp_subject.py` & `django-ipghrms-training-1.1/training/migrations/0025_trainingemp_subject.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/0026_traininggap.py` & `django-ipghrms-training-1.1/training/migrations/0026_traininggap.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/0028_traininggap_employee.py` & `django-ipghrms-training-1.1/training/migrations/0028_traininggap_employee.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/0030_trainingdep_trainingplangap.py` & `django-ipghrms-training-1.1/training/migrations/0030_trainingdep_trainingplangap.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/0031_auto_20230312_0215.py` & `django-ipghrms-training-1.1/training/migrations/0031_auto_20230312_0215.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/0033_auto_20230312_1619.py` & `django-ipghrms-training-1.1/training/migrations/0033_auto_20230312_1619.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/__pycache__/0001_initial.cpython-310.pyc` & `django-ipghrms-training-1.1/training/migrations/__pycache__/0001_initial.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/__pycache__/0001_initial.cpython-37.pyc` & `django-ipghrms-training-1.1/training/migrations/__pycache__/0001_initial.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/__pycache__/0001_initial.cpython-39.pyc` & `django-ipghrms-training-1.1/training/migrations/__pycache__/0001_initial.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/__pycache__/0002_hrcriteria_trainingemp_tyear_unitcriteria_and_more.cpython-310.pyc` & `django-ipghrms-training-1.1/training/migrations/__pycache__/0002_hrcriteria_trainingemp_tyear_unitcriteria_and_more.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/__pycache__/0002_hrcriteria_trainingemp_tyear_unitcriteria_and_more.cpython-37.pyc` & `django-ipghrms-training-1.1/training/migrations/__pycache__/0002_hrcriteria_trainingemp_tyear_unitcriteria_and_more.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/__pycache__/0003_rename_fundtype_ttype_delete_trainingtype_and_more.cpython-310.pyc` & `django-ipghrms-training-1.1/training/migrations/__pycache__/0003_rename_fundtype_ttype_delete_trainingtype_and_more.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/__pycache__/0003_rename_fundtype_ttype_delete_trainingtype_and_more.cpython-37.pyc` & `django-ipghrms-training-1.1/training/migrations/__pycache__/0003_rename_fundtype_ttype_delete_trainingtype_and_more.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/__pycache__/0004_trainingplan_duration.cpython-310.pyc` & `django-ipghrms-training-1.1/training/migrations/__pycache__/0004_trainingplan_duration.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/__pycache__/0004_trainingplan_duration.cpython-37.pyc` & `django-ipghrms-training-1.1/training/migrations/__pycache__/0004_trainingplan_duration.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/__pycache__/0005_tcriteria_trainingcriteria_remove_unitcriteria_plan_and_more.cpython-310.pyc` & `django-ipghrms-training-1.1/training/migrations/__pycache__/0005_tcriteria_trainingcriteria_remove_unitcriteria_plan_and_more.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/__pycache__/0005_tcriteria_trainingcriteria_remove_unitcriteria_plan_and_more.cpython-37.pyc` & `django-ipghrms-training-1.1/training/migrations/__pycache__/0005_tcriteria_trainingcriteria_remove_unitcriteria_plan_and_more.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/__pycache__/0006_alter_tcriteria_subject.cpython-310.pyc` & `django-ipghrms-training-1.1/training/migrations/__pycache__/0006_alter_tcriteria_subject.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/__pycache__/0006_alter_tcriteria_subject.cpython-37.pyc` & `django-ipghrms-training-1.1/training/migrations/__pycache__/0006_alter_tcriteria_subject.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/__pycache__/0007_trainingplan_is_approve_trainingplan_is_certify_and_more.cpython-310.pyc` & `django-ipghrms-training-1.1/training/migrations/__pycache__/0007_trainingplan_is_approve_trainingplan_is_certify_and_more.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/__pycache__/0007_trainingplan_is_approve_trainingplan_is_certify_and_more.cpython-37.pyc` & `django-ipghrms-training-1.1/training/migrations/__pycache__/0007_trainingplan_is_approve_trainingplan_is_certify_and_more.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/__pycache__/0008_trainingsubject.cpython-310.pyc` & `django-ipghrms-training-1.1/training/migrations/__pycache__/0008_trainingsubject.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/__pycache__/0008_trainingsubject.cpython-37.pyc` & `django-ipghrms-training-1.1/training/migrations/__pycache__/0008_trainingsubject.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/__pycache__/0009_remove_trainingplan_duration_and_more.cpython-310.pyc` & `django-ipghrms-training-1.1/training/migrations/__pycache__/0009_remove_trainingplan_duration_and_more.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/__pycache__/0009_remove_trainingplan_duration_and_more.cpython-37.pyc` & `django-ipghrms-training-1.1/training/migrations/__pycache__/0009_remove_trainingplan_duration_and_more.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/__pycache__/0010_trainingplan_duration_trainingplan_place_and_more.cpython-310.pyc` & `django-ipghrms-training-1.1/training/migrations/__pycache__/0010_trainingplan_duration_trainingplan_place_and_more.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/__pycache__/0010_trainingplan_duration_trainingplan_place_and_more.cpython-37.pyc` & `django-ipghrms-training-1.1/training/migrations/__pycache__/0010_trainingplan_duration_trainingplan_place_and_more.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/__pycache__/0011_remove_trainingemp_hashed_delete_trainingsubject.cpython-310.pyc` & `django-ipghrms-training-1.1/training/migrations/__pycache__/0011_remove_trainingemp_hashed_delete_trainingsubject.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/__pycache__/0011_remove_trainingemp_hashed_delete_trainingsubject.cpython-37.pyc` & `django-ipghrms-training-1.1/training/migrations/__pycache__/0011_remove_trainingemp_hashed_delete_trainingsubject.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/__pycache__/0012_trainingemp_diploma_alter_trainingemp_department_and_more.cpython-310.pyc` & `django-ipghrms-training-1.1/training/migrations/__pycache__/0012_trainingemp_diploma_alter_trainingemp_department_and_more.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/__pycache__/0012_trainingemp_diploma_alter_trainingemp_department_and_more.cpython-37.pyc` & `django-ipghrms-training-1.1/training/migrations/__pycache__/0012_trainingemp_diploma_alter_trainingemp_department_and_more.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/__pycache__/0013_alter_trainingcriteria_criteria.cpython-310.pyc` & `django-ipghrms-training-1.1/training/migrations/__pycache__/0013_alter_trainingcriteria_criteria.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/__pycache__/0013_alter_trainingcriteria_criteria.cpython-37.pyc` & `django-ipghrms-training-1.1/training/migrations/__pycache__/0013_alter_trainingcriteria_criteria.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/__pycache__/0014_tcriteria_is_active.cpython-310.pyc` & `django-ipghrms-training-1.1/training/migrations/__pycache__/0014_tcriteria_is_active.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/__pycache__/0014_tcriteria_is_active.cpython-37.pyc` & `django-ipghrms-training-1.1/training/migrations/__pycache__/0014_tcriteria_is_active.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/__pycache__/0015_auto_20221210_0226.cpython-310.pyc` & `django-ipghrms-training-1.1/training/migrations/__pycache__/0015_auto_20221210_0226.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/__pycache__/0016_trainingemp_is_update.cpython-310.pyc` & `django-ipghrms-training-1.1/training/migrations/__pycache__/0016_trainingemp_is_update.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/__pycache__/0017_scholarshipplan_sprogress_stype.cpython-310.pyc` & `django-ipghrms-training-1.1/training/migrations/__pycache__/0017_scholarshipplan_sprogress_stype.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/__pycache__/0018_auto_20221210_1435.cpython-310.pyc` & `django-ipghrms-training-1.1/training/migrations/__pycache__/0018_auto_20221210_1435.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/__pycache__/0019_scholarshipemp_scholarshipempprogress.cpython-310.pyc` & `django-ipghrms-training-1.1/training/migrations/__pycache__/0019_scholarshipemp_scholarshipempprogress.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/__pycache__/0020_auto_20221210_1550.cpython-310.pyc` & `django-ipghrms-training-1.1/training/migrations/__pycache__/0020_auto_20221210_1550.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/__pycache__/0021_rename_start_date_scholarshipempprogress_date.cpython-310.pyc` & `django-ipghrms-training-1.1/training/migrations/__pycache__/0021_rename_start_date_scholarshipempprogress_date.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/__pycache__/0022_alter_scholarshipemp_emp.cpython-310.pyc` & `django-ipghrms-training-1.1/training/migrations/__pycache__/0022_alter_scholarshipemp_emp.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/__pycache__/0023_scholarshipplan_is_update.cpython-310.pyc` & `django-ipghrms-training-1.1/training/migrations/__pycache__/0023_scholarshipplan_is_update.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/__pycache__/0024_auto_20221210_1742.cpython-310.pyc` & `django-ipghrms-training-1.1/training/migrations/__pycache__/0024_auto_20221210_1742.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/__pycache__/0025_trainingemp_subject.cpython-310.pyc` & `django-ipghrms-training-1.1/training/migrations/__pycache__/0025_trainingemp_subject.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/__pycache__/0026_traininggap.cpython-310.pyc` & `django-ipghrms-training-1.1/training/migrations/__pycache__/0026_traininggap.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/__pycache__/0027_traininggap_is_done.cpython-310.pyc` & `django-ipghrms-training-1.1/training/migrations/__pycache__/0027_traininggap_is_done.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/__pycache__/0028_traininggap_employee.cpython-310.pyc` & `django-ipghrms-training-1.1/training/migrations/__pycache__/0028_traininggap_employee.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/__pycache__/0029_traininggap_is_lock.cpython-310.pyc` & `django-ipghrms-training-1.1/training/migrations/__pycache__/0029_traininggap_is_lock.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/__pycache__/0030_trainingdep_trainingplangap.cpython-310.pyc` & `django-ipghrms-training-1.1/training/migrations/__pycache__/0030_trainingdep_trainingplangap.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/__pycache__/0031_auto_20230312_0215.cpython-310.pyc` & `django-ipghrms-training-1.1/training/migrations/__pycache__/0031_auto_20230312_0215.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/__pycache__/0032_trainingplan_is_update.cpython-310.pyc` & `django-ipghrms-training-1.1/training/migrations/__pycache__/0032_trainingplan_is_update.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/migrations/__pycache__/0033_auto_20230312_1619.cpython-310.pyc` & `django-ipghrms-training-1.1/training/migrations/__pycache__/0033_auto_20230312_1619.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/models.py` & `django-ipghrms-training-1.1/training/models.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/schor_url.py` & `django-ipghrms-training-1.1/training/schor_url.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/templates/gap/emp_gap_list.html` & `django-ipghrms-training-1.1/training/templates/gap/emp_gap_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/templates/gap/form.html` & `django-ipghrms-training-1.1/training/templates/gap/form.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/templates/gap/list.html` & `django-ipghrms-training-1.1/training/templates/gap/list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/templates/scholariship/detail.html` & `django-ipghrms-training-1.1/training/templates/scholariship/detail.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/templates/scholariship/emp_detail.html` & `django-ipghrms-training-1.1/training/templates/scholariship/emp_detail.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/templates/scholariship/form.html` & `django-ipghrms-training-1.1/training/templates/scholariship/form.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/templates/scholariship/list.html` & `django-ipghrms-training-1.1/training/templates/scholariship/list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/templates/scholariship/raw_list.html` & `django-ipghrms-training-1.1/training/templates/scholariship/raw_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/templates/training/c_crit_list.html` & `django-ipghrms-training-1.1/training/templates/training/c_crit_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/templates/training/c_dash.html` & `django-ipghrms-training-1.1/training/templates/training/c_dash.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/templates/training/c_plan_detail.html` & `django-ipghrms-training-1.1/training/templates/training/c_plan_detail.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/templates/training/c_plan_list.html` & `django-ipghrms-training-1.1/training/templates/training/c_plan_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/templates/training/c_raw_data.html` & `django-ipghrms-training-1.1/training/templates/training/c_raw_data.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/templates/training/de_dash.html` & `django-ipghrms-training-1.1/training/templates/training/de_dash.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/templates/training/de_plan_detail.html` & `django-ipghrms-training-1.1/training/templates/training/de_plan_detail.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/templates/training/de_plan_list.html` & `django-ipghrms-training-1.1/training/templates/training/de_plan_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/templates/training/form.html` & `django-ipghrms-training-1.1/training/templates/training/form.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/templates/training/form2.html` & `django-ipghrms-training-1.1/training/templates/training/form2.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/templates/training/hr_crit_list.html` & `django-ipghrms-training-1.1/training/templates/training/hr_crit_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/templates/training/hr_dash.html` & `django-ipghrms-training-1.1/training/templates/training/hr_dash.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/templates/training/hr_plan_detail.html` & `django-ipghrms-training-1.1/training/templates/training/hr_plan_detail.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/templates/training/raw_data.html` & `django-ipghrms-training-1.1/training/templates/training/raw_data.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/templates/training/summary.html` & `django-ipghrms-training-1.1/training/templates/training/summary.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/templates/training/summary_year.html` & `django-ipghrms-training-1.1/training/templates/training/summary_year.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/templates/training_chart/myoption.js` & `django-ipghrms-training-1.1/training/templates/training_chart/myoption.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/templates/training_chart/train_dep.js` & `django-ipghrms-training-1.1/training/templates/training_chart/train_dep.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/templates/training_chart/train_unit.js` & `django-ipghrms-training-1.1/training/templates/training_chart/train_unit.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/templates/training_chart/train_year.js` & `django-ipghrms-training-1.1/training/templates/training_chart/train_year.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/urls.py` & `django-ipghrms-training-1.1/training/urls.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/views/__pycache__/m_scho.cpython-310.pyc` & `django-ipghrms-training-1.1/training/views/__pycache__/m_scho.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/views/__pycache__/training_m.cpython-310.pyc` & `django-ipghrms-training-1.1/training/views/__pycache__/training_m.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/views/__pycache__/training_m.cpython-37.pyc` & `django-ipghrms-training-1.1/training/views/__pycache__/training_m.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/views/__pycache__/training_v.cpython-310.pyc` & `django-ipghrms-training-1.1/training/views/__pycache__/training_v.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/views/__pycache__/training_v.cpython-37.pyc` & `django-ipghrms-training-1.1/training/views/__pycache__/training_v.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/views/__pycache__/v_scho.cpython-310.pyc` & `django-ipghrms-training-1.1/training/views/__pycache__/v_scho.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/views/m_scho.py` & `django-ipghrms-training-1.1/training/views/m_scho.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/views/training_m.py` & `django-ipghrms-training-1.1/training/views/training_m.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-training-1.0/training/views/training_v.py` & `django-ipghrms-training-1.1/training/views/training_v.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,26 +48,37 @@
 	context = {
 		'group': group, 'objects': objects,
 		'title': f'Painel Treinamento  & Bolso Estudo', 'legend': f'Painel Treinamento  & Bolso Estudo'
 	}
 	return render(request, 'training/de_dash.html', context)
 ###
 @login_required
-@allowed_users(allowed_roles=['unit'])
-def cTPlanList(request):
+@allowed_users(allowed_roles=['hr','hr_s'])
+def hrTPlanList(request):
 	group = request.user.groups.all()[0].name
-	c_emp, unit = c_unit(request.user)
-	objects = TrainingPlan.objects.filter(unit=unit).all().order_by('-year','id')
-	years = TrainingPlan.objects.filter().distinct().values('year__year').all()
+	current_date = dt.now()
+	default_month = current_date.month
+	default_year = current_date.year
+	start_date = request.GET.get('start_date')
+	end_date = request.GET.get('end_date')
+	date_range_query = {}
+	if start_date and end_date:
+		start_date = dt.strptime(start_date, "%Y-%m-%d")
+		end_date = dt.strptime(end_date, "%Y-%m-%d")
+		date_range_query['start_date__range'] = (start_date, end_date)
+	c_emp, dep = c_unit(request.user)
+	objects = TrainingPlan.objects.filter(is_send=True,  **date_range_query).all().order_by('-year','id')
 	context = {
-		'group': group, 'unit': unit, 'objects': objects,
-		'title': f'Lista Planu Treinamento', 'legend': f'Lista Planu Treinamento', 'years':years
+		'group': group, 'dep': dep, 'objects': objects,
+		'title': f'Lista Planu Treinamento', 'legend': f'Lista Planu Treinamento',
+		'start_date':start_date,
+		'end_date':end_date,
+		'page':'trainning'
 	}
-	return render(request, 'training/c_plan_list.html', context)
-
+	return render(request, 'training/hr_plan_list.html', context)
 
 		
 
 @login_required
 @allowed_users(allowed_roles=['hr','de'])
 def hrTSumaryList(request):
 	group = request.user.groups.all()[0].name
```

### Comparing `django-ipghrms-training-1.0/training/views/v_scho.py` & `django-ipghrms-training-1.1/training/views/v_scho.py`

 * *Files identical despite different names*

