# Comparing `tmp/nobinobi-daily-follow-up-0.1.2.6.tar.gz` & `tmp/nobinobi-daily-follow-up-0.1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nobinobi-daily-follow-up-0.1.2.6.tar", last modified: Tue Jun 20 14:25:47 2023, max compression
+gzip compressed data, was "nobinobi-daily-follow-up-0.1.2.7.tar", last modified: Wed Jun 21 14:55:46 2023, max compression
```

## Comparing `nobinobi-daily-follow-up-0.1.2.6.tar` & `nobinobi-daily-follow-up-0.1.2.7.tar`

### file list

```diff
@@ -1,185 +1,183 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.667243 nobinobi-daily-follow-up-0.1.2.6/
--rw-rw-rw-   0        0        0      166 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/AUTHORS.rst
--rw-rw-rw-   0        0        0     3491 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     4717 2023-06-20 14:24:55.000000 nobinobi-daily-follow-up-0.1.2.6/HISTORY.rst
--rw-rw-rw-   0        0        0    31999 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/LICENSE
--rw-rw-rw-   0        0        0      508 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/MANIFEST.in
--rw-rw-rw-   0        0        0     8475 2023-06-20 14:25:47.667243 nobinobi-daily-follow-up-0.1.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     3016 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.329452 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/
--rw-rw-rw-   0        0        0      901 2023-06-20 14:24:55.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/__init__.py
--rw-rw-rw-   0        0        0     6644 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/admin.py
--rw-rw-rw-   0        0        0     2132 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/apps.py
--rw-rw-rw-   0        0        0    24928 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/forms.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.231352 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/locale/
-drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.230352 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/locale/en/
-drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.338000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/locale/en/LC_MESSAGES/
--rw-rw-rw-   0        0        0    36220 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/locale/en/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.231352 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/locale/fr/
-drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.368895 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0        0        0    17584 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/locale/fr/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    43173 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/locale/fr/LC_MESSAGES/django.po
--rw-rw-rw-   0        0        0     3840 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/menus.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.421690 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/
--rw-rw-rw-   0        0        0    21335 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0001_initial.py
--rw-rw-rw-   0        0        0    29811 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0001_initial_squashed_0011_auto_20200401_1117.py
--rw-rw-rw-   0        0        0     1251 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0002_auto_20190513_1535.py
--rw-rw-rw-   0        0        0      902 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0002_auto_20230201_1346.py
--rw-rw-rw-   0        0        0     2218 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0003_troubleshooting.py
--rw-rw-rw-   0        0        0    18214 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0004_auto_20190815_1141.py
--rw-rw-rw-   0        0        0     3355 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0005_auto_20190923_1517.py
--rw-rw-rw-   0        0        0     1288 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0006_medication_child.py
--rw-rw-rw-   0        0        0     1313 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0007_givemedication_date.py
--rw-rw-rw-   0        0        0     1966 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0008_auto_20191021_1443.py
--rw-rw-rw-   0        0        0     1357 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0009_fix_early_troubleshoting_relation.py
--rw-rw-rw-   0        0        0     1577 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0010_add_intermediary_departure_arrival_time.py
--rw-rw-rw-   0        0        0     1368 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0011_auto_20200401_1117.py
--rw-rw-rw-   0        0        0      794 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/__init__.py
--rw-rw-rw-   0        0        0    18845 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/models.py
--rw-rw-rw-   0        0        0     6365 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/serializers.py
--rw-rw-rw-   0        0        0    13848 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/signals.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.233569 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/
-drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.426243 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/css/
--rw-rw-rw-   0        0        0     2723 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/css/nobinobi_daily_follow_up.css
--rw-rw-rw-   0        0        0     1132 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/css/nobinobi_daily_follow_up.css.map
--rw-rw-rw-   0        0        0     2984 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/css/nobinobi_daily_follow_up.scss
-drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.427239 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/
--rw-rw-rw-   0        0        0        0 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/.gitignore
-drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.516753 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/
--rw-rw-rw-   0        0        0    26606 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/anger.png
--rw-rw-rw-   0        0        0    26912 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/burn.png
--rw-rw-rw-   0        0        0    25533 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/caca.png
--rw-rw-rw-   0        0        0    23167 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/confused.png
--rw-rw-rw-   0        0        0    24827 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/cool.png
--rw-rw-rw-   0        0        0    24276 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/cry.png
--rw-rw-rw-   0        0        0    30248 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/fire.png
--rw-rw-rw-   0        0        0    30457 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/grimace.png
--rw-rw-rw-   0        0        0    27131 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/love.png
--rw-rw-rw-   0        0        0    23405 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/miao.png
--rw-rw-rw-   0        0        0    38098 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/nothing.png
--rw-rw-rw-   0        0        0   191276 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/nothing.psd
--rw-rw-rw-   0        0        0    31987 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/prettiness.png
--rw-rw-rw-   0        0        0    26621 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/question.png
--rw-rw-rw-   0        0        0    23059 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/shout.png
--rw-rw-rw-   0        0        0    26669 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/slobber.png
--rw-rw-rw-   0        0        0    27523 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/smile.png
--rw-rw-rw-   0        0        0    22780 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/spook.png
--rw-rw-rw-   0        0        0    26432 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/startle.png
--rw-rw-rw-   0        0        0    31314 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/surprise.png
--rw-rw-rw-   0        0        0    24973 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/sweat.png
--rw-rw-rw-   0        0        0    24280 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/thirst.png
--rw-rw-rw-   0        0        0    27373 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/vomit.png
-drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.518767 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/js/
--rw-rw-rw-   0        0        0      805 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/js/nobinobi_daily_follow_up.js
-drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.519761 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/js/notifications/
--rw-rw-rw-   0        0        0     2602 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/js/notifications/notify.js
-drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.520762 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/js/vendor/
--rw-rw-rw-   0        0        0    38511 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/js/vendor/bootstrap-datetimepicker.min.js
-drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.235598 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/
-drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.522763 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_child/
--rw-rw-rw-   0        0        0     4633 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_child/base.html
-drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.525273 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/
-drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.532585 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/
--rw-rw-rw-   0        0        0     1196 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_choice_classroom.html
--rw-rw-rw-   0        0        0      650 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_confirm_delete.html
--rw-rw-rw-   0        0        0     1535 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_create.html
--rw-rw-rw-   0        0        0     1535 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_update.html
--rw-rw-rw-   0        0        0     1598 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/group_activity_update.html
-drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.533848 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/bootstrap_datepicker_plus/
--rw-rw-rw-   0        0        0      301 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/bootstrap_datepicker_plus/time-picker.html
-drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.555490 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/
--rw-rw-rw-   0        0        0     1542 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/dailyfollowup_update.html
--rw-rw-rw-   0        0        0     1418 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/group_choice_classroom.html
--rw-rw-rw-   0        0        0     1718 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/group_daily_follow_up_update.html
--rw-rw-rw-   0        0        0    45469 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/summary_week.html
--rw-rw-rw-   0        0        0     1407 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/summary_week_choice.html
-drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.561147 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowuptomedication/
--rw-rw-rw-   0        0        0      660 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowuptomedication/dailyfollowuptomedication_confirm_delete.html
--rw-rw-rw-   0        0        0     1565 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowuptomedication/dailyfollowuptomedication_create.html
--rw-rw-rw-   0        0        0     1567 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowuptomedication/dailyfollowuptomedication_update.html
-drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.564147 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/diaperchange/
--rw-rw-rw-   0        0        0      655 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/diaperchange/diaperchange_confirm_delete.html
--rw-rw-rw-   0        0        0     1416 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/diaperchange/diaperchange_create.html
--rw-rw-rw-   0        0        0     1416 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/diaperchange/diaperchange_update.html
-drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.571190 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/
--rw-rw-rw-   0        0        0      782 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_confirm_delete.html
--rw-rw-rw-   0        0        0     1551 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_create.html
--rw-rw-rw-   0        0        0      968 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_detail.html
--rw-rw-rw-   0        0        0     6663 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_list.html
--rw-rw-rw-   0        0        0     1551 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_update.html
-drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.238612 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/
-drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.575188 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/widgets/
--rw-rw-rw-   0        0        0       49 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/widgets/checkbox.html
--rw-rw-rw-   0        0        0      400 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/widgets/inline-img-radio-input.html
--rw-rw-rw-   0        0        0      717 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/widgets/inline-img-radio.html
--rw-rw-rw-   0        0        0      490 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/widgets/inline_img_checkbox_option.html
--rw-rw-rw-   0        0        0      717 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/widgets/inline_img_checkbox_select.html
-drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.580300 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/
--rw-rw-rw-   0        0        0      726 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/givemedication_confirm_delete.html
--rw-rw-rw-   0        0        0     1540 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/givemedication_create.html
--rw-rw-rw-   0        0        0     1664 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/givemedication_delay.html
--rw-rw-rw-   0        0        0     1542 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/givemedication_update.html
-drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.585300 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/
--rw-rw-rw-   0        0        0     2228 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/checkboxselectmultiple_image.html
--rw-rw-rw-   0        0        0     1647 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/checkboxselectmultiple_inline_image.html
--rw-rw-rw-   0        0        0     2209 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/radioselect_image.html
--rw-rw-rw-   0        0        0     1689 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/radioselect_inline_image.html
-drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.587821 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/lotiondailyfollowup/
--rw-rw-rw-   0        0        0      691 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/lotiondailyfollowup/lotiondailyfollowup_confirm_delete.html
--rw-rw-rw-   0        0        0     1536 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/lotiondailyfollowup/lotiondailyfollowup_create.html
--rw-rw-rw-   0        0        0     1549 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/lotiondailyfollowup/lotiondailyfollowup_update.html
-drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.591342 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/meals/
--rw-rw-rw-   0        0        0     2235 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/meals/mealdailyfollowup_create.html
--rw-rw-rw-   0        0        0     1535 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/meals/mealdailyfollowup_update.html
-drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.595851 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/
--rw-rw-rw-   0        0        0      660 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/medication_confirm_delete.html
--rw-rw-rw-   0        0        0     1565 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/medication_create.html
--rw-rw-rw-   0        0        0     1259 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/medication_multiday.html
--rw-rw-rw-   0        0        0     1567 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/medication_update.html
-drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.598864 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/nap/
--rw-rw-rw-   0        0        0      626 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/nap/nap_confirm_delete.html
--rw-rw-rw-   0        0        0     1533 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/nap/nap_create.html
--rw-rw-rw-   0        0        0     1533 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/nap/nap_update.html
-drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.634545 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/
--rw-rw-rw-   0        0        0    32358 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/admin_presence_week_list.html
--rw-rw-rw-   0        0        0     1196 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_choice_classroom.html
--rw-rw-rw-   0        0        0     1538 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_create.html
--rw-rw-rw-   0        0        0     1535 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_update.html
--rw-rw-rw-   0        0        0    21134 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_week_kindergarten_list.html
--rw-rw-rw-   0        0        0    10664 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_week_list.html
--rw-rw-rw-   0        0        0     1158 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence_choice.html
--rw-rw-rw-   0        0        0    52404 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence_detail_list.html
-drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.635545 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/reception/
--rw-rw-rw-   0        0        0     1539 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/reception/reception_update.html
-drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.638581 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/stroll/
--rw-rw-rw-   0        0        0     1196 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/stroll/stroll_choice_classroom.html
--rw-rw-rw-   0        0        0     1797 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/stroll/stroll_pdf.html
-drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.643099 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templatetags/
--rw-rw-rw-   0        0        0     1498 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templatetags/__init__.py
--rw-rw-rw-   0        0        0     3742 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templatetags/notifications_custom_tags.py
--rw-rw-rw-   0        0        0      978 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templatetags/replacement_classroom_tags.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.644098 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/test_utils/
--rw-rw-rw-   0        0        0      794 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/test_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.663720 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/test_utils/test_app/
--rw-rw-rw-   0        0        0      794 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/test_utils/test_app/__init__.py
--rw-rw-rw-   0        0        0      867 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/test_utils/test_app/admin.py
--rw-rw-rw-   0        0        0      889 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/test_utils/test_app/apps.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.665229 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/test_utils/test_app/migrations/
--rw-rw-rw-   0        0        0      794 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/test_utils/test_app/migrations/__init__.py
--rw-rw-rw-   0        0        0      855 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/test_utils/test_app/models.py
--rw-rw-rw-   0        0        0    25536 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/urls.py
--rw-rw-rw-   0        0        0     3866 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/utils.py
--rw-rw-rw-   0        0        0   130484 2023-06-20 14:24:55.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/views.py
--rw-rw-rw-   0        0        0     1964 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/widgets.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.336485 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up.egg-info/
--rw-rw-rw-   0        0        0     8475 2023-06-20 14:25:46.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    10027 2023-06-20 14:25:46.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 14:25:46.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-20 14:25:46.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      169 2023-06-20 14:25:46.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-06-20 14:25:46.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      195 2023-06-14 13:30:37.000000 nobinobi-daily-follow-up-0.1.2.6/requirements.txt
--rw-rw-rw-   0        0        0      125 2023-06-15 10:29:37.000000 nobinobi-daily-follow-up-0.1.2.6/requirements_dev.txt
--rw-rw-rw-   0        0        0      205 2023-06-20 14:24:55.000000 nobinobi-daily-follow-up-0.1.2.6/requirements_test.txt
--rw-rw-rw-   0        0        0      301 2023-06-20 14:25:47.668244 nobinobi-daily-follow-up-0.1.2.6/setup.cfg
--rw-rw-rw-   0        0        0     2357 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 14:55:46.307505 nobinobi-daily-follow-up-0.1.2.7/
+-rw-rw-rw-   0        0        0      166 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3491 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     4804 2023-06-21 14:55:17.000000 nobinobi-daily-follow-up-0.1.2.7/HISTORY.rst
+-rw-rw-rw-   0        0        0    31999 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/LICENSE
+-rw-rw-rw-   0        0        0      508 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     8562 2023-06-21 14:55:46.307505 nobinobi-daily-follow-up-0.1.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3016 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-21 14:55:45.927707 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/
+-rw-rw-rw-   0        0        0      901 2023-06-21 14:55:17.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/__init__.py
+-rw-rw-rw-   0        0        0     6644 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/admin.py
+-rw-rw-rw-   0        0        0     2132 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/apps.py
+-rw-rw-rw-   0        0        0    23591 2023-06-21 14:55:17.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/forms.py
+drwxrwxrwx   0        0        0        0 2023-06-21 14:55:45.776965 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/locale/
+drwxrwxrwx   0        0        0        0 2023-06-21 14:55:45.776965 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/locale/en/
+drwxrwxrwx   0        0        0        0 2023-06-21 14:55:45.934225 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/locale/en/LC_MESSAGES/
+-rw-rw-rw-   0        0        0    36220 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/locale/en/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-06-21 14:55:45.776965 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/locale/fr/
+drwxrwxrwx   0        0        0        0 2023-06-21 14:55:45.968412 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0        0        0    17584 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    43173 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/locale/fr/LC_MESSAGES/django.po
+-rw-rw-rw-   0        0        0     3840 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/menus.py
+drwxrwxrwx   0        0        0        0 2023-06-21 14:55:46.035214 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/migrations/
+-rw-rw-rw-   0        0        0    21335 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0    29811 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/migrations/0001_initial_squashed_0011_auto_20200401_1117.py
+-rw-rw-rw-   0        0        0     1251 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/migrations/0002_auto_20190513_1535.py
+-rw-rw-rw-   0        0        0      902 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/migrations/0002_auto_20230201_1346.py
+-rw-rw-rw-   0        0        0     2218 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/migrations/0003_troubleshooting.py
+-rw-rw-rw-   0        0        0    18214 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/migrations/0004_auto_20190815_1141.py
+-rw-rw-rw-   0        0        0     3355 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/migrations/0005_auto_20190923_1517.py
+-rw-rw-rw-   0        0        0     1288 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/migrations/0006_medication_child.py
+-rw-rw-rw-   0        0        0     1313 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/migrations/0007_givemedication_date.py
+-rw-rw-rw-   0        0        0     1966 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/migrations/0008_auto_20191021_1443.py
+-rw-rw-rw-   0        0        0     1357 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/migrations/0009_fix_early_troubleshoting_relation.py
+-rw-rw-rw-   0        0        0     1577 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/migrations/0010_add_intermediary_departure_arrival_time.py
+-rw-rw-rw-   0        0        0     1368 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/migrations/0011_auto_20200401_1117.py
+-rw-rw-rw-   0        0        0      794 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/migrations/__init__.py
+-rw-rw-rw-   0        0        0    18845 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/models.py
+-rw-rw-rw-   0        0        0     6365 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/serializers.py
+-rw-rw-rw-   0        0        0    13848 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/signals.py
+drwxrwxrwx   0        0        0        0 2023-06-21 14:55:45.778964 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/
+drwxrwxrwx   0        0        0        0 2023-06-21 14:55:46.048236 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/css/
+-rw-rw-rw-   0        0        0     2723 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/css/nobinobi_daily_follow_up.css
+-rw-rw-rw-   0        0        0     1132 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/css/nobinobi_daily_follow_up.css.map
+-rw-rw-rw-   0        0        0     2984 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/css/nobinobi_daily_follow_up.scss
+drwxrwxrwx   0        0        0        0 2023-06-21 14:55:46.049237 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/img/
+-rw-rw-rw-   0        0        0        0 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/img/.gitignore
+drwxrwxrwx   0        0        0        0 2023-06-21 14:55:46.163151 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/img/smiley/
+-rw-rw-rw-   0        0        0    26606 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/img/smiley/anger.png
+-rw-rw-rw-   0        0        0    26912 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/img/smiley/burn.png
+-rw-rw-rw-   0        0        0    25533 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/img/smiley/caca.png
+-rw-rw-rw-   0        0        0    23167 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/img/smiley/confused.png
+-rw-rw-rw-   0        0        0    24827 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/img/smiley/cool.png
+-rw-rw-rw-   0        0        0    24276 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/img/smiley/cry.png
+-rw-rw-rw-   0        0        0    30248 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/img/smiley/fire.png
+-rw-rw-rw-   0        0        0    30457 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/img/smiley/grimace.png
+-rw-rw-rw-   0        0        0    27131 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/img/smiley/love.png
+-rw-rw-rw-   0        0        0    23405 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/img/smiley/miao.png
+-rw-rw-rw-   0        0        0    38098 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/img/smiley/nothing.png
+-rw-rw-rw-   0        0        0   191276 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/img/smiley/nothing.psd
+-rw-rw-rw-   0        0        0    31987 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/img/smiley/prettiness.png
+-rw-rw-rw-   0        0        0    26621 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/img/smiley/question.png
+-rw-rw-rw-   0        0        0    23059 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/img/smiley/shout.png
+-rw-rw-rw-   0        0        0    26669 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/img/smiley/slobber.png
+-rw-rw-rw-   0        0        0    27523 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/img/smiley/smile.png
+-rw-rw-rw-   0        0        0    22780 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/img/smiley/spook.png
+-rw-rw-rw-   0        0        0    26432 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/img/smiley/startle.png
+-rw-rw-rw-   0        0        0    31314 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/img/smiley/surprise.png
+-rw-rw-rw-   0        0        0    24973 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/img/smiley/sweat.png
+-rw-rw-rw-   0        0        0    24280 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/img/smiley/thirst.png
+-rw-rw-rw-   0        0        0    27373 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/img/smiley/vomit.png
+drwxrwxrwx   0        0        0        0 2023-06-21 14:55:46.166662 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/js/
+-rw-rw-rw-   0        0        0      805 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/js/nobinobi_daily_follow_up.js
+drwxrwxrwx   0        0        0        0 2023-06-21 14:55:46.168663 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/js/notifications/
+-rw-rw-rw-   0        0        0     2602 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/js/notifications/notify.js
+drwxrwxrwx   0        0        0        0 2023-06-21 14:55:46.169662 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/js/vendor/
+-rw-rw-rw-   0        0        0    38511 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/js/vendor/bootstrap-datetimepicker.min.js
+drwxrwxrwx   0        0        0        0 2023-06-21 14:55:45.779969 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/
+drwxrwxrwx   0        0        0        0 2023-06-21 14:55:46.172181 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_child/
+-rw-rw-rw-   0        0        0     4860 2023-06-21 14:55:17.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_child/base.html
+drwxrwxrwx   0        0        0        0 2023-06-21 14:55:46.174290 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/
+drwxrwxrwx   0        0        0        0 2023-06-21 14:55:46.180814 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/
+-rw-rw-rw-   0        0        0     1196 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_choice_classroom.html
+-rw-rw-rw-   0        0        0      650 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_confirm_delete.html
+-rw-rw-rw-   0        0        0     1531 2023-06-21 14:55:17.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_create.html
+-rw-rw-rw-   0        0        0     1531 2023-06-21 14:55:17.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_update.html
+-rw-rw-rw-   0        0        0     1598 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/group_activity_update.html
+drwxrwxrwx   0        0        0        0 2023-06-21 14:55:46.208244 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/
+-rw-rw-rw-   0        0        0     1538 2023-06-21 14:55:17.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/dailyfollowup_update.html
+-rw-rw-rw-   0        0        0     1418 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/group_choice_classroom.html
+-rw-rw-rw-   0        0        0     1718 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/group_daily_follow_up_update.html
+-rw-rw-rw-   0        0        0    45469 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/summary_week.html
+-rw-rw-rw-   0        0        0     1407 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/summary_week_choice.html
+drwxrwxrwx   0        0        0        0 2023-06-21 14:55:46.218542 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowuptomedication/
+-rw-rw-rw-   0        0        0      660 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowuptomedication/dailyfollowuptomedication_confirm_delete.html
+-rw-rw-rw-   0        0        0     1561 2023-06-21 14:55:17.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowuptomedication/dailyfollowuptomedication_create.html
+-rw-rw-rw-   0        0        0     1563 2023-06-21 14:55:17.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowuptomedication/dailyfollowuptomedication_update.html
+drwxrwxrwx   0        0        0        0 2023-06-21 14:55:46.220541 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/diaperchange/
+-rw-rw-rw-   0        0        0      655 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/diaperchange/diaperchange_confirm_delete.html
+-rw-rw-rw-   0        0        0     1558 2023-06-21 14:55:17.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/diaperchange/diaperchange_create.html
+-rw-rw-rw-   0        0        0     1558 2023-06-21 14:55:17.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/diaperchange/diaperchange_update.html
+drwxrwxrwx   0        0        0        0 2023-06-21 14:55:46.229571 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/
+-rw-rw-rw-   0        0        0      782 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_confirm_delete.html
+-rw-rw-rw-   0        0        0     1547 2023-06-21 14:55:17.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_create.html
+-rw-rw-rw-   0        0        0      968 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_detail.html
+-rw-rw-rw-   0        0        0     6663 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_list.html
+-rw-rw-rw-   0        0        0     1547 2023-06-21 14:55:17.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_update.html
+drwxrwxrwx   0        0        0        0 2023-06-21 14:55:45.783018 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/
+drwxrwxrwx   0        0        0        0 2023-06-21 14:55:46.233089 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/widgets/
+-rw-rw-rw-   0        0        0       49 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/widgets/checkbox.html
+-rw-rw-rw-   0        0        0      400 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/widgets/inline-img-radio-input.html
+-rw-rw-rw-   0        0        0      717 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/widgets/inline-img-radio.html
+-rw-rw-rw-   0        0        0      490 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/widgets/inline_img_checkbox_option.html
+-rw-rw-rw-   0        0        0      717 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/widgets/inline_img_checkbox_select.html
+drwxrwxrwx   0        0        0        0 2023-06-21 14:55:46.239204 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/
+-rw-rw-rw-   0        0        0      726 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/givemedication_confirm_delete.html
+-rw-rw-rw-   0        0        0     1536 2023-06-21 14:55:17.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/givemedication_create.html
+-rw-rw-rw-   0        0        0     1825 2023-06-21 14:55:17.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/givemedication_delay.html
+-rw-rw-rw-   0        0        0     1538 2023-06-21 14:55:17.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/givemedication_update.html
+drwxrwxrwx   0        0        0        0 2023-06-21 14:55:46.245726 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/
+-rw-rw-rw-   0        0        0     2228 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/checkboxselectmultiple_image.html
+-rw-rw-rw-   0        0        0     1647 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/checkboxselectmultiple_inline_image.html
+-rw-rw-rw-   0        0        0     2209 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/radioselect_image.html
+-rw-rw-rw-   0        0        0     1689 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/radioselect_inline_image.html
+drwxrwxrwx   0        0        0        0 2023-06-21 14:55:46.249254 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/lotiondailyfollowup/
+-rw-rw-rw-   0        0        0      691 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/lotiondailyfollowup/lotiondailyfollowup_confirm_delete.html
+-rw-rw-rw-   0        0        0     1532 2023-06-21 14:55:17.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/lotiondailyfollowup/lotiondailyfollowup_create.html
+-rw-rw-rw-   0        0        0     1545 2023-06-21 14:55:17.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/lotiondailyfollowup/lotiondailyfollowup_update.html
+drwxrwxrwx   0        0        0        0 2023-06-21 14:55:46.251253 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/meals/
+-rw-rw-rw-   0        0        0     1531 2023-06-21 14:55:17.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/meals/mealdailyfollowup_create.html
+-rw-rw-rw-   0        0        0     1531 2023-06-21 14:55:17.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/meals/mealdailyfollowup_update.html
+drwxrwxrwx   0        0        0        0 2023-06-21 14:55:46.256780 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/
+-rw-rw-rw-   0        0        0      660 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/medication_confirm_delete.html
+-rw-rw-rw-   0        0        0     1561 2023-06-21 14:55:17.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/medication_create.html
+-rw-rw-rw-   0        0        0     1259 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/medication_multiday.html
+-rw-rw-rw-   0        0        0     1563 2023-06-21 14:55:17.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/medication_update.html
+drwxrwxrwx   0        0        0        0 2023-06-21 14:55:46.260310 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/nap/
+-rw-rw-rw-   0        0        0      626 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/nap/nap_confirm_delete.html
+-rw-rw-rw-   0        0        0     1529 2023-06-21 14:55:17.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/nap/nap_create.html
+-rw-rw-rw-   0        0        0     1529 2023-06-21 14:55:17.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/nap/nap_update.html
+drwxrwxrwx   0        0        0        0 2023-06-21 14:55:46.288264 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/
+-rw-rw-rw-   0        0        0    32358 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/admin_presence_week_list.html
+-rw-rw-rw-   0        0        0     1196 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_choice_classroom.html
+-rw-rw-rw-   0        0        0     1534 2023-06-21 14:55:17.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_create.html
+-rw-rw-rw-   0        0        0     1531 2023-06-21 14:55:17.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_update.html
+-rw-rw-rw-   0        0        0    21134 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_week_kindergarten_list.html
+-rw-rw-rw-   0        0        0    10664 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_week_list.html
+-rw-rw-rw-   0        0        0     1158 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence_choice.html
+-rw-rw-rw-   0        0        0    52138 2023-06-21 14:55:17.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence_detail_list.html
+drwxrwxrwx   0        0        0        0 2023-06-21 14:55:46.290308 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/reception/
+-rw-rw-rw-   0        0        0     1535 2023-06-21 14:55:17.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/reception/reception_update.html
+drwxrwxrwx   0        0        0        0 2023-06-21 14:55:46.292829 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/stroll/
+-rw-rw-rw-   0        0        0     1196 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/stroll/stroll_choice_classroom.html
+-rw-rw-rw-   0        0        0     1797 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/stroll/stroll_pdf.html
+drwxrwxrwx   0        0        0        0 2023-06-21 14:55:46.296839 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templatetags/
+-rw-rw-rw-   0        0        0     1498 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templatetags/__init__.py
+-rw-rw-rw-   0        0        0     3742 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templatetags/notifications_custom_tags.py
+-rw-rw-rw-   0        0        0      978 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templatetags/replacement_classroom_tags.py
+drwxrwxrwx   0        0        0        0 2023-06-21 14:55:46.297836 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/test_utils/
+-rw-rw-rw-   0        0        0      794 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/test_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 14:55:46.305504 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/test_utils/test_app/
+-rw-rw-rw-   0        0        0      794 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/test_utils/test_app/__init__.py
+-rw-rw-rw-   0        0        0      867 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/test_utils/test_app/admin.py
+-rw-rw-rw-   0        0        0      889 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/test_utils/test_app/apps.py
+drwxrwxrwx   0        0        0        0 2023-06-21 14:55:46.306506 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/test_utils/test_app/migrations/
+-rw-rw-rw-   0        0        0      794 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/test_utils/test_app/migrations/__init__.py
+-rw-rw-rw-   0        0        0      855 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/test_utils/test_app/models.py
+-rw-rw-rw-   0        0        0    25536 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/urls.py
+-rw-rw-rw-   0        0        0     3866 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/utils.py
+-rw-rw-rw-   0        0        0   130484 2023-06-20 14:24:55.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/views.py
+-rw-rw-rw-   0        0        0     1964 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/widgets.py
+drwxrwxrwx   0        0        0        0 2023-06-21 14:55:45.933225 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up.egg-info/
+-rw-rw-rw-   0        0        0     8562 2023-06-21 14:55:45.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     9924 2023-06-21 14:55:45.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 14:55:45.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-21 14:55:45.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      169 2023-06-21 14:55:45.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-06-21 14:55:45.000000 nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      205 2023-06-21 14:50:27.000000 nobinobi-daily-follow-up-0.1.2.7/requirements.txt
+-rw-rw-rw-   0        0        0      125 2023-06-15 10:29:37.000000 nobinobi-daily-follow-up-0.1.2.7/requirements_dev.txt
+-rw-rw-rw-   0        0        0      205 2023-06-20 14:24:55.000000 nobinobi-daily-follow-up-0.1.2.7/requirements_test.txt
+-rw-rw-rw-   0        0        0      301 2023-06-21 14:55:46.308504 nobinobi-daily-follow-up-0.1.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     2357 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.7/setup.py
```

### Comparing `nobinobi-daily-follow-up-0.1.2.6/CONTRIBUTING.rst` & `nobinobi-daily-follow-up-0.1.2.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/HISTORY.rst` & `nobinobi-daily-follow-up-0.1.2.7/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 .. :changelog:
 
 History
 -------
 
+0.1.2.7 (2023-06-21)
++++++++++++++++++++++++++
+
+* bd33989 - Fix date time picker
+
 0.1.2.6 (2023-06-20)
 +++++++++++++++++++++++++
 
 * 33ddd86 - fix error in create presence day table
 * Update requirements
 
 0.1.2.5 (2023-06-15)
```

### Comparing `nobinobi-daily-follow-up-0.1.2.6/LICENSE` & `nobinobi-daily-follow-up-0.1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/PKG-INFO` & `nobinobi-daily-follow-up-0.1.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobinobi-daily-follow-up
-Version: 0.1.2.6
+Version: 0.1.2.7
 Summary: Application Daily follow-up for nobinobi
 Home-page: https://github.com/prolibre-ch/nobinobi-daily-follow-up
 Author: Florian Alu
 Author-email: alu@prolibre.com
 Keywords: nobinobi-daily-follow-up
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django :: 3.1
@@ -135,14 +135,19 @@
 
 
 
 
 History
 -------
 
+0.1.2.7 (2023-06-21)
++++++++++++++++++++++++++
+
+* bd33989 - Fix date time picker
+
 0.1.2.6 (2023-06-20)
 +++++++++++++++++++++++++
 
 * 33ddd86 - fix error in create presence day table
 * Update requirements
 
 0.1.2.5 (2023-06-15)
```

### Comparing `nobinobi-daily-follow-up-0.1.2.6/README.rst` & `nobinobi-daily-follow-up-0.1.2.7/README.rst`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/__init__.py` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 #      but WITHOUT ANY WARRANTY; without even the implied warranty of
 #      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #      GNU Affero General Public License for more details.
 #
 #      You should have received a copy of the GNU Affero General Public License
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-__version__ = '0.1.2.6'
+__version__ = '0.1.2.7'
 default_app_config = 'nobinobi_daily_follow_up.apps.NobinobiDailyFollowUpConfig'
```

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/admin.py` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/admin.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/apps.py` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/apps.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/forms.py` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/forms.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 from bootstrap_datepicker_plus.widgets import TimePickerInput, DatePickerInput
 from bootstrap_modal_forms.forms import BSModalModelForm
 from bootstrap_modal_forms.mixins import CreateUpdateAjaxMixin, PopRequestMixin
 from crispy_forms.helper import FormHelper
 from crispy_forms.layout import Submit, Layout, Div, Field
 from django import forms
-from django.conf import settings
 from django.contrib import messages
 from django.contrib.auth import get_user_model
 from django.core.exceptions import ValidationError
 from django.db.models import Q
 from django.forms import ModelForm
 from django.forms.renderers import get_default_renderer
 from django.utils import timezone
@@ -34,16 +33,16 @@
 
 from nobinobi_daily_follow_up.models import Reception, MealDailyFollowUp, Nap, LotionDailyFollowUp, DiaperChange, \
     Activity, Medication, DailyFollowUp, Presence, TypeActivity, GiveMedication, DailyFollowUpToMedication, \
     EarlyTroubleshooting
 from nobinobi_daily_follow_up.utils import GroupedModelMultiChoiceField
 
 
-class FaTimePickerInput(TimePickerInput):
-    template_name = 'nobinobi_daily_follow_up/bootstrap_datepicker_plus/time-picker.html'
+# class FaTimePickerInput(TimePickerInput):
+#     template_name = 'nobinobi_daily_follow_up/bootstrap_datepicker_plus/time-picker.html'
 
 
 class InlineImgRadioInput(forms.RadioSelect):
     template_name = 'nobinobi_daily_follow_up/forms/widgets/inline-img-radio.html'
     option_template_name = 'nobinobi_daily_follow_up/forms/widgets/inline-img-radio-input.html'
 
 
@@ -94,16 +93,16 @@
     # )
 
     class Meta:
         model = Presence
         fields = ("child", "arrival_time", "departure_time")
 
         widgets = {
-            "arrival_time": FaTimePickerInput(options={"locale": "fr"}).start_of('presence days'),
-            "departure_time": FaTimePickerInput(options={"locale": "fr"}).end_of('presence days'),
+            "arrival_time": TimePickerInput(),
+            "departure_time": TimePickerInput(range_from="arrival_time"),
         }
 
     def __init__(self, *args, **kwargs):
         self.date = kwargs.pop("date", None)
         self.classroom = kwargs.pop("classroom", None)
         self.child_pk = kwargs.pop("child_pk", None)
         if self.classroom:
@@ -116,15 +115,14 @@
         super(PresenceCreateForm, self).__init__(*args, **kwargs)
         # if not preselect image before add
         if self.classroom:
             if self.child_pk is None:
                 self.fields['child'].queryset = Child.objects.filter(classroom=self.classroom,
                                                                      status=Child.STATUS.in_progress)
 
-
     def save(self, commit=True):
         if not self.request.is_ajax():
             instance = super(PresenceCreateForm, self).save(commit=False)
             instance.date = self.date
             instance.classroom = self.classroom
             try:
                 Presence.objects.get(child=instance.child, date=self.date)
@@ -139,18 +137,17 @@
         return instance
 
 
 class PresenceDepartureForm(CreateUpdateAjaxMixin, forms.ModelForm):
     class Meta:
         model = Presence
         fields = ("arrival_time", "departure_time",)
-
         widgets = {
-            "departure_time": FaTimePickerInput(options={"locale": "fr"}),
-            "arrival_time": FaTimePickerInput(options={"locale": "fr"}),
+            "arrival_time": TimePickerInput(),
+            "departure_time": TimePickerInput(range_from="arrival_time"),
         }
 
     def __init__(self, *args, **kwargs):
         self.request = kwargs.pop("request", None)
         self.date = kwargs.pop("date", None)
         self.classroom = kwargs.pop("classroom", None)
         self.child_pk = kwargs.pop("child_pk", None)
@@ -177,18 +174,17 @@
 
 class PresenceintermediateDepartureForm(CreateUpdateAjaxMixin, forms.ModelForm):
     class Meta:
         model = Presence
         fields = ("intermediate_departure_time", "intermediate_arrival_time")
 
         widgets = {
-            "intermediate_departure_time": FaTimePickerInput(options={"locale": "fr"}).start_of(
-                'presence days intermediate'),
-            "intermediate_arrival_time": FaTimePickerInput(options={"locale": "fr"}).end_of(
-                'presence days intermediate'),
+            "intermediate_arrival_time": TimePickerInput(),
+            "intermediate_departure_time": TimePickerInput(range_from="intermediate_arrival_time"),
+
         }
 
     def __init__(self, *args, **kwargs):
         self.request = kwargs.pop("request", None)
         self.date = kwargs.pop("date", None)
         self.classroom = kwargs.pop("classroom", None)
         self.child_pk = kwargs.pop("child_pk", None)
@@ -200,15 +196,15 @@
 
 
 class ReceptionForm(BSModalModelForm):
     class Meta:
         model = Reception
         fields = ["wake_up_time", "breakfast", "breakfast_time", "sleep", "sick", "fever", "condition", "comment"]
         widgets = {
-            "breakfast_time": FaTimePickerInput(options={"locale": "fr"}),
+            "breakfast_time": TimePickerInput(),
             "breakfast": InlineImgRadioInput(),
             "sleep": InlineImgRadioInput(),
             "condition": InlineImgRadioInput(),
         }
 
 
 class MealDailyFollowUpForm(BSModalModelForm):
@@ -219,17 +215,17 @@
         widgets = {
             "snack_quality": InlineImgRadioInput(),
             "snack_meals": InlineImgMealCheckboxInput(),
             "lunch_quality": InlineImgRadioInput(),
             "lunch_meals": InlineImgMealCheckboxInput(),
             "afternoon_snack_quality": InlineImgRadioInput(),
             "afternoon_snack_meals": InlineImgMealCheckboxInput(),
-            "snack_time": FaTimePickerInput(options={"locale": "fr"}),
-            "lunch_time": FaTimePickerInput(options={"locale": "fr"}),
-            "afternoon_snack_time": FaTimePickerInput(options={"locale": "fr"}),
+            "snack_time": TimePickerInput(),
+            "lunch_time": TimePickerInput(),
+            "afternoon_snack_time": TimePickerInput(),
         }
 
     def full_clean(self):
         return super(MealDailyFollowUpForm, self).full_clean()
 
     # def __init__(self, *args, **kwargs):
     #     super(MealDailyFollowUpForm, self).__init__(*args, **kwargs)
@@ -255,28 +251,25 @@
 
 
 class NapForm(BSModalModelForm):
     class Meta:
         model = Nap
         fields = ["start_time", "end_time"]
         widgets = {
-            # "start_time": TimePickerInput(options={"locale": "fr"}),
-            "start_time": FaTimePickerInput(options={"locale": "fr"}).start_of('nap time'),
-            # "end_time": FaTimePickerInput(options={"locale": "fr"}),
-            "end_time": FaTimePickerInput(options={"locale": "fr"}).end_of('nap time'),
+            "start_time": TimePickerInput(),
+            "end_time": TimePickerInput(range_from="start_time"),
         }
 
 
 class DiaperChangeForm(BSModalModelForm):
     class Meta:
         model = DiaperChange
         fields = ["hour", "feces"]
         widgets = {
-            "hour": FaTimePickerInput(
-                options={"locale": "fr"}),
+            "hour": TimePickerInput(),
             "feces": InlineImgRadioInput(),
         }
 
 
 class LotionDailyFollowUpForm(BSModalModelForm):
     class Meta:
         model = LotionDailyFollowUp
@@ -296,16 +289,16 @@
 
 
 class MedicationForm(BSModalModelForm):
     class Meta:
         model = Medication
         fields = ["from_date", "end_date", "type_medication", "comment", "attachment"]
         widgets = {
-            "from_date": DatePickerInput(options={"locale": "fr", "format": "DD/MM/YYYY"}).start_of('medic days'),
-            "end_date": DatePickerInput(options={"locale": "fr", "format": "DD/MM/YYYY"}).end_of('medic days'),
+            "from_date": DatePickerInput(),
+            "end_date": DatePickerInput(range_from="from_date"),
         }
 
     def __init__(self, *args, **kwargs):
         self.daily_follow_up = kwargs.pop("daily_follow_up", None)
         self.child = kwargs.pop("child", None)
         super(MedicationForm, self).__init__(*args, **kwargs)
 
@@ -327,16 +320,16 @@
     staff = forms.ModelChoiceField(label=_("Staff"), queryset=Staff.objects.filter(status=Staff.STATUS.active),
                                    required=False)
 
     class Meta:
         model = GiveMedication
         fields = ["staff", "give_hour", "given_hour"]
         widgets = {
-            "give_hour": FaTimePickerInput(options={"locale": "fr"}),
-            "given_hour": FaTimePickerInput(options={"locale": "fr"}),
+            "give_hour": TimePickerInput(),
+            "given_hour": TimePickerInput(),
         }
 
     def __init__(self, *args, **kwargs):
         self.date = kwargs.pop("date", None)
         super(GiveMedicationForm, self).__init__(*args, **kwargs)
 
     def save(self, commit=True):
@@ -380,18 +373,15 @@
             search_fields=['first_name__icontains'],
         ),
         required=True
     )
 
     date = forms.DateField(
         label=_("Date"),
-        widget=DatePickerInput(options={
-            "locale": "fr",
-            "format": "DD/MM/YYYY"
-        }),
+        widget=DatePickerInput(),
     )
 
     class Meta:
         fields = ("child", "date")
 
     def __init__(self, *args, **kwargs):
         super(ChoiceChildDateForm, self).__init__(*args, **kwargs)
@@ -524,23 +514,19 @@
         self.helper.label_class = "col-lg-2"
         self.helper.field_class = "col-lg-10"
 
         self.helper.add_input(Submit('submit', _("Submit")))
 
 
 class MultiDayMedicationForm(ModelForm):
-    give_hour = forms.TimeField(label=_("Give hour"), widget=TimePickerInput(options={"locale": "fr"}))
-    give_hour2 = forms.TimeField(label=_("Give hour") + " 2", widget=TimePickerInput(options={"locale": "fr"}),
-                                 required=False)
-    give_hour3 = forms.TimeField(label=_("Give hour") + " 3", widget=TimePickerInput(options={"locale": "fr"}),
-                                 required=False)
-    give_hour4 = forms.TimeField(label=_("Give hour") + " 4", widget=TimePickerInput(options={"locale": "fr"}),
-                                 required=False)
-    give_hour5 = forms.TimeField(label=_("Give hour") + " 5", widget=TimePickerInput(options={"locale": "fr"}),
-                                 required=False)
+    give_hour = forms.TimeField(label=_("Give hour"), widget=TimePickerInput())
+    give_hour2 = forms.TimeField(label=_("Give hour") + " 2", widget=TimePickerInput(), required=False)
+    give_hour3 = forms.TimeField(label=_("Give hour") + " 3", widget=TimePickerInput(), required=False)
+    give_hour4 = forms.TimeField(label=_("Give hour") + " 4", widget=TimePickerInput(), required=False)
+    give_hour5 = forms.TimeField(label=_("Give hour") + " 5", widget=TimePickerInput(), required=False)
     child = forms.ModelChoiceField(
         queryset=Child.objects.filter(status=Child.STATUS.in_progress).order_by("age_group",
                                                                                 'first_name',
                                                                                 'last_name'),
         label=_("Child"),
         widget=ModelSelect2Widget(
             model=Child,
@@ -553,16 +539,16 @@
     )
 
     class Meta:
         model = Medication
         fields = ["child", "from_date", "end_date", "type_medication", "attachment", "comment", "give_hour",
                   "give_hour2", "give_hour3", "give_hour4", "give_hour5", ]
         widgets = {
-            "from_date": DatePickerInput(options={"locale": "fr", "format": "DD/MM/YYYY"}).start_of('medic days'),
-            "end_date": DatePickerInput(options={"locale": "fr", "format": "DD/MM/YYYY"}).end_of('medic days'),
+            "from_date": DatePickerInput(),
+            "end_date": DatePickerInput(range_from="from_date"),
         }
 
     def __init__(self, *args, **kwargs):
         super(MultiDayMedicationForm, self).__init__(*args, **kwargs)
         # Redefinition de la query qui get les enfants qui sont dans le groupe
         # fournie par la page d'avant dans le url
 
@@ -574,18 +560,15 @@
 
         self.helper.add_input(Submit('submit', _("Submit")))
 
 
 class EarlyTroubleshootingForm(BSModalModelForm):
     date = forms.DateField(
         label=_("Date"),
-        widget=DatePickerInput(options={
-            "locale": "fr",
-            "format": "DD/MM/YYYY"
-        }),
+        widget=DatePickerInput(),
     )
 
     class Meta:
         model = EarlyTroubleshooting
         fields = ("child", "date", "periods")
 
     def clean_periods(self):
```

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/locale/en/LC_MESSAGES/django.po` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/locale/fr/LC_MESSAGES/django.mo` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/locale/fr/LC_MESSAGES/django.po` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/menus.py` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/menus.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0001_initial.py` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0001_initial_squashed_0011_auto_20200401_1117.py` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/migrations/0001_initial_squashed_0011_auto_20200401_1117.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0002_auto_20190513_1535.py` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/migrations/0002_auto_20190513_1535.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0002_auto_20230201_1346.py` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/migrations/0002_auto_20230201_1346.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0003_troubleshooting.py` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/migrations/0003_troubleshooting.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0004_auto_20190815_1141.py` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/migrations/0004_auto_20190815_1141.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0005_auto_20190923_1517.py` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/migrations/0005_auto_20190923_1517.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0006_medication_child.py` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/migrations/0006_medication_child.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0007_givemedication_date.py` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/migrations/0007_givemedication_date.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0008_auto_20191021_1443.py` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/migrations/0008_auto_20191021_1443.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0009_fix_early_troubleshoting_relation.py` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/migrations/0009_fix_early_troubleshoting_relation.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0010_add_intermediary_departure_arrival_time.py` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/migrations/0010_add_intermediary_departure_arrival_time.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0011_auto_20200401_1117.py` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/migrations/0011_auto_20200401_1117.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/__init__.py` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/models.py` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/models.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/serializers.py` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/serializers.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/signals.py` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/signals.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/css/nobinobi_daily_follow_up.css` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/css/nobinobi_daily_follow_up.css`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/css/nobinobi_daily_follow_up.css.map` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/css/nobinobi_daily_follow_up.css.map`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/css/nobinobi_daily_follow_up.scss` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/css/nobinobi_daily_follow_up.scss`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/anger.png` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/img/smiley/anger.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/burn.png` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/img/smiley/burn.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/caca.png` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/img/smiley/caca.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/confused.png` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/img/smiley/confused.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/cool.png` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/img/smiley/cool.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/cry.png` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/img/smiley/cry.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/fire.png` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/img/smiley/fire.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/grimace.png` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/img/smiley/grimace.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/love.png` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/img/smiley/love.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/miao.png` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/img/smiley/miao.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/nothing.png` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/img/smiley/nothing.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/nothing.psd` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/img/smiley/nothing.psd`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/prettiness.png` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/img/smiley/prettiness.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/question.png` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/img/smiley/question.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/shout.png` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/img/smiley/shout.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/slobber.png` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/img/smiley/slobber.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/smile.png` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/img/smiley/smile.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/spook.png` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/img/smiley/spook.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/startle.png` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/img/smiley/startle.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/surprise.png` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/img/smiley/surprise.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/sweat.png` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/img/smiley/sweat.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/thirst.png` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/img/smiley/thirst.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/vomit.png` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/img/smiley/vomit.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/js/nobinobi_daily_follow_up.js` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/js/nobinobi_daily_follow_up.js`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/js/notifications/notify.js` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/js/notifications/notify.js`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/js/vendor/bootstrap-datetimepicker.min.js` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/static/js/vendor/bootstrap-datetimepicker.min.js`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_child/base.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_child/base.html`

 * *Files 5% similar despite different names*

```diff
@@ -27,16 +27,17 @@
     {% endif %}
     {% include "includes/modal.html" %}
 
 {% endblock %}
 {% block extrajs %}
     {{ block.super }}
     <script type="text/javascript" src="{% static 'js/moment-with-locales.min.js' %}"></script>
-    <script type="text/javascript" src="{% static 'js/vendor/bootstrap-datetimepicker.min.js' %}"></script>
-    <script src="{% static 'js/jquery.bootstrap.modal.forms.js' %}"></script>
+    <script src="https://cdn.jsdelivr.net/npm/eonasdan-bootstrap-datetimepicker@4.17.49/build/js/bootstrap-datetimepicker.min.js"></script>
+    <script src="https://cdn.jsdelivr.net/gh/monim67/django-bootstrap-datepicker-plus@5.0.2/src/bootstrap_datepicker_plus/static/bootstrap_datepicker_plus/js/datepicker-widget.js"></script>
+    <script src="{% static 'js/jquery.bootstrap.modal.forms.min.js' %}"></script>
     <script src="{% static 'js/notifications/notify.js' %}" type="text/javascript"></script>
     <script>
         function fill_notification_lists(data) {
             var menus = document.getElementsByClassName(notify_menu_class);
             if (menus) {
                 var messages = data.all_list.map(function (item) {
                     var message = "";
```

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_choice_classroom.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_choice_classroom.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_confirm_delete.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_create.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_create.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% load widget_tweaks static i18n %}
+{{ form.media }}
 
 <form method="post" action="">
     {% csrf_token %}
-    {{ form.media }}
     <div class="modal-header">
         <h3 class="modal-title">{% trans "Create Activity" %}</h3>
         <button type="button" class="close" data-dismiss="modal" aria-label="Close">
             <span aria-hidden="true">&times;</span>
         </button>
     </div>
```

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_update.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_update.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% load widget_tweaks static i18n %}
+{{ form.media }}
 
 <form method="post" action="">
     {% csrf_token %}
-    {{ form.media }}
     <div class="modal-header">
         <h3 class="modal-title">{% trans "Update Activity" %}</h3>
         <button type="button" class="close" data-dismiss="modal" aria-label="Close">
             <span aria-hidden="true">&times;</span>
         </button>
     </div>
```

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/group_activity_update.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/group_activity_update.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/dailyfollowup_update.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/dailyfollowup_update.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% load widget_tweaks static i18n %}
+{{ form.media }}
 
 <form method="post" action="">
     {% csrf_token %}
-    {{ form.media }}
     <div class="modal-header">
         <h3 class="modal-title">{% trans "Update Daily follow-up" %}</h3>
         <button type="button" class="close" data-dismiss="modal" aria-label="Close">
             <span aria-hidden="true">&times;</span>
         </button>
     </div>
```

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/group_choice_classroom.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/group_choice_classroom.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/group_daily_follow_up_update.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/group_daily_follow_up_update.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/summary_week.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/summary_week.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/summary_week_choice.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/summary_week_choice.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowuptomedication/dailyfollowuptomedication_confirm_delete.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowuptomedication/dailyfollowuptomedication_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowuptomedication/dailyfollowuptomedication_create.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowuptomedication/dailyfollowuptomedication_create.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% load widget_tweaks static i18n %}
+{{ form.media }}
 
 <form method="post" action="" enctype="multipart/form-data">
     {% csrf_token %}
-    {{ form.media }}
     <div class="modal-header">
         <h3 class="modal-title">{% trans "Create Medication" %}</h3>
         <button type="button" class="close" data-dismiss="modal" aria-label="Close">
             <span aria-hidden="true">&times;</span>
         </button>
     </div>
```

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowuptomedication/dailyfollowuptomedication_update.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowuptomedication/dailyfollowuptomedication_update.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% load widget_tweaks static i18n %}
+{{ form.media }}
 
 <form method="post" action="" enctype="multipart/form-data">
     {% csrf_token %}
-    {{ form.media }}
     <div class="modal-header">
         <h3 class="modal-title">{% trans "Update Medication" %}</h3>
         <button type="button" class="close" data-dismiss="modal" aria-label="Close">
             <span aria-hidden="true">&times;</span>
         </button>
     </div>
```

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/diaperchange/diaperchange_confirm_delete.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/diaperchange/diaperchange_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/diaperchange/diaperchange_create.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_create.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-{% load static %}
 {% load i18n %}
 {% load widget_tweaks %}
+{{ form.media }}
+
 <form method="post" action="">
-	{% csrf_token %}
-	{{ form.media }}
+    {% csrf_token %}
     <div class="modal-header">
-        <h3 class="modal-title">{% trans "Create diaper change" %}</h3>
+        <h3 class="modal-title">{% trans "Create Presence" %}</h3>
         <button type="button" class="close" data-dismiss="modal" aria-label="Close">
             <span aria-hidden="true">&times;</span>
         </button>
     </div>
 
     <div class="modal-body">
+
         <div class="{% if form.non_field_errors %}invalid{% endif %} mb-2">
-			{% for error in form.non_field_errors %}
-				{{ error }}
-			{% endfor %}
+            {% for error in form.non_field_errors %}
+                {{ error }}
+            {% endfor %}
         </div>
 
-		{% for field in form %}
+        {% for field in form %}
             <div class="form-group">
                 <label for="{{ field.id_for_label }}">{{ field.label }}</label>
-				{% if field.field.required %}
-					{% render_field field required="required" class="form-control" placeholder=field.label %}
-				{% else %}
-					{% render_field field class="form-control" placeholder=field.label %}
-				{% endif %}
+                {% if field.field.required %}
+                    {% render_field field required="required" class="form-control" placeholder=field.label %}
+                {% else %}
+                    {% render_field field class="form-control" placeholder=field.label %}
+                {% endif %}
                 <div class="{% if field.errors %} invalid{% endif %}">
-					{% for error in field.errors %}
+                    {% for error in field.errors %}
                         <p class="help-block">{{ error }}</p>
-					{% endfor %}
+                    {% endfor %}
                 </div>
             </div>
-		{% endfor %}
+        {% endfor %}
     </div>
 
     <div class="modal-footer">
         <button type="submit" class="submit-btn btn btn-primary">{% trans "Create" %}</button>
     </div>
 </form>
-
```

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/diaperchange/diaperchange_update.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/meals/mealdailyfollowup_create.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-{% load static %}
 {% load i18n %}
 {% load widget_tweaks %}
+{{ form.media }}
+
 <form method="post" action="">
-	{% csrf_token %}
-	{{ form.media }}
+    {% csrf_token %}
     <div class="modal-header">
-        <h3 class="modal-title">{% trans "Update diaper change" %}</h3>
+        <h3 class="modal-title">{% trans "Create meals" %}</h3>
         <button type="button" class="close" data-dismiss="modal" aria-label="Close">
             <span aria-hidden="true">&times;</span>
         </button>
     </div>
 
     <div class="modal-body">
+
         <div class="{% if form.non_field_errors %}invalid{% endif %} mb-2">
-			{% for error in form.non_field_errors %}
-				{{ error }}
-			{% endfor %}
+            {% for error in form.non_field_errors %}
+                {{ error }}
+            {% endfor %}
         </div>
 
-		{% for field in form %}
+        {% for field in form %}
             <div class="form-group">
                 <label for="{{ field.id_for_label }}">{{ field.label }}</label>
-				{% if field.field.required %}
-					{% render_field field required="required" class="form-control" placeholder=field.label %}
-				{% else %}
-					{% render_field field class="form-control" placeholder=field.label %}
-				{% endif %}
+                {% if field.field.required %}
+                    {% render_field field required="required" class="form-control" placeholder=field.label %}
+                {% else %}
+                    {% render_field field class="form-control" placeholder=field.label %}
+                {% endif %}
                 <div class="{% if field.errors %} invalid{% endif %}">
-					{% for error in field.errors %}
+                    {% for error in field.errors %}
                         <p class="help-block">{{ error }}</p>
-					{% endfor %}
+                    {% endfor %}
                 </div>
             </div>
-		{% endfor %}
+        {% endfor %}
     </div>
 
     <div class="modal-footer">
-        <button type="submit" class="submit-btn btn btn-primary">{% trans "Update" %}</button>
+        <button type="submit" class="submit-btn btn btn-primary">{% trans "Create" %}</button>
     </div>
 </form>
-
```

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_confirm_delete.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_create.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_create.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {% load i18n %}
 {% load widget_tweaks %}
+{{ form.media }}
 
 <form method="post" action="">
     {% csrf_token %}
-    {{ form.media }}
     <div class="modal-header">
         <h3 class="modal-title">{% trans "Create Early troubleshooting" %}</h3>
         <button type="button" class="close" data-dismiss="modal" aria-label="Close">
             <span aria-hidden="true">&times;</span>
         </button>
     </div>
```

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_detail.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_detail.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_list.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_list.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_update.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/nap/nap_create.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 {% load i18n %}
 {% load widget_tweaks %}
+{{ form.media }}
 
 <form method="post" action="">
     {% csrf_token %}
-    {{ form.media }}
     <div class="modal-header">
-        <h3 class="modal-title">{% trans "Update Early troubleshooting" %}</h3>
+        <h3 class="modal-title">{% trans "Create Nap" %}</h3>
         <button type="button" class="close" data-dismiss="modal" aria-label="Close">
             <span aria-hidden="true">&times;</span>
         </button>
     </div>
 
     <div class="modal-body">
 
@@ -33,10 +33,10 @@
                     {% endfor %}
                 </div>
             </div>
         {% endfor %}
     </div>
 
     <div class="modal-footer">
-        <button type="submit" class="submit-btn btn btn-primary">{% trans "Update" %}</button>
+        <button type="submit" class="submit-btn btn btn-primary">{% trans "Create" %}</button>
     </div>
 </form>
```

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/widgets/inline-img-radio.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/widgets/inline-img-radio.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/widgets/inline_img_checkbox_select.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/widgets/inline_img_checkbox_select.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/givemedication_confirm_delete.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/givemedication_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/givemedication_create.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/givemedication_create.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% load widget_tweaks static i18n %}
+{{ form.media }}
 
 <form method="post" action="">
     {% csrf_token %}
-    {{ form.media }}
     <div class="modal-header">
         <h3 class="modal-title">{% trans "Create Give Medication" %}</h3>
         <button type="button" class="close" data-dismiss="modal" aria-label="Close">
             <span aria-hidden="true">&times;</span>
         </button>
     </div>
```

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/givemedication_delay.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/givemedication_delay.html`

 * *Files 11% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 {% load widget_tweaks static i18n %}
+{{ form.media }}
 
 <form method="post" action="">
-	{% csrf_token %}
-	{{ form.media }}
+    {% csrf_token %}
     <div class="modal-header">
         <h3 class="modal-title">{% trans "Delay Give Medication" %}</h3>
         <button type="button" class="close" data-dismiss="modal" aria-label="Close">
             <span aria-hidden="true">&times;</span>
         </button>
     </div>
 
     <div class="modal-body">
 
         <div class="{% if form.non_field_errors %}invalid{% endif %} mb-2">
-			{% for error in form.non_field_errors %}
-				{{ error }}
-			{% endfor %}
+            {% for error in form.non_field_errors %}
+                {{ error }}
+            {% endfor %}
         </div>
 
-		{% for field in form %}
+        {% for field in form %}
             <div class="alert alert-warning" role="alert">
                 <strong>{{ field.help_text }}</strong>
             </div>
             <div class="form-group row mx-auto">
                 <label for="{{ field.id_for_label }}" class="col-sm-2 col-form-label">{{ field.label }}</label>
                 <div class="col-sm-1 col-form-label">
-					{% if field.field.required %}
-						{% render_field field required="required" class="" placeholder=field.label %}
-					{% else %}
-						{% render_field field class="form-control" placeholder=field.label %}
-					{% endif %}
+                    {% if field.field.required %}
+                        {% render_field field required="required" class="" placeholder=field.label %}
+                    {% else %}
+                        {% render_field field class="form-control" placeholder=field.label %}
+                    {% endif %}
                     <div class="{% if field.errors %} invalid{% endif %}">
-						{% for error in field.errors %}
+                        {% for error in field.errors %}
                             <p class="help-block">{{ error }}</p>
-						{% endfor %}
+                        {% endfor %}
                     </div>
                 </div>
 
             </div>
-		{% endfor %}
+        {% endfor %}
     </div>
 
     <div class="modal-footer">
         <button type="submit" class="submit-btn btn btn-primary">{% trans "Delay" %}</button>
     </div>
 
 </form>
```

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/givemedication_update.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/givemedication_update.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% load widget_tweaks static i18n %}
+{{ form.media }}
 
 <form method="post" action="">
     {% csrf_token %}
-    {{ form.media }}
     <div class="modal-header">
         <h3 class="modal-title">{% trans "Update Give Medication" %}</h3>
         <button type="button" class="close" data-dismiss="modal" aria-label="Close">
             <span aria-hidden="true">&times;</span>
         </button>
     </div>
```

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/checkboxselectmultiple_image.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/checkboxselectmultiple_image.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/checkboxselectmultiple_inline_image.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/checkboxselectmultiple_inline_image.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/radioselect_image.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/radioselect_image.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/radioselect_inline_image.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/radioselect_inline_image.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/lotiondailyfollowup/lotiondailyfollowup_confirm_delete.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/lotiondailyfollowup/lotiondailyfollowup_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/lotiondailyfollowup/lotiondailyfollowup_create.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/lotiondailyfollowup/lotiondailyfollowup_create.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {% load i18n %}
 {% load widget_tweaks %}
+{{ form.media }}
 
 <form method="post" action="">
     {% csrf_token %}
-    {{ form.media }}
     <div class="modal-header">
         <h3 class="modal-title">{% trans "Create Lotion" %}</h3>
         <button type="button" class="close" data-dismiss="modal" aria-label="Close">
             <span aria-hidden="true">&times;</span>
         </button>
     </div>
```

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/lotiondailyfollowup/lotiondailyfollowup_update.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/lotiondailyfollowup/lotiondailyfollowup_update.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% load widget_tweaks static i18n %}
+{{ form.media }}
 
 <form method="post" action="">
     {% csrf_token %}
-    {{ form.media }}
     <div class="modal-header">
         <h3 class="modal-title">{% trans "Update lotion daily follow-up" %}</h3>
         <button type="button" class="close" data-dismiss="modal" aria-label="Close">
             <span aria-hidden="true">&times;</span>
         </button>
     </div>
```

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/meals/mealdailyfollowup_create.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/meals/mealdailyfollowup_update.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,15 @@
-{#{% load static i18n crispy_forms_tags %}#}
-{#<form method="post" action="">#}
-{#  {% csrf_token %}#}
-{#  <div class="modal-header">#}
-{#    <h3 class="modal-title">{% trans "Create meals" %}</h3>#}
-{#    <button type="button" class="close" data-dismiss="modal" aria-label="Close">#}
-{#      <span aria-hidden="true">&times;</span>#}
-{#    </button>#}
-{#  </div>#}
-{##}
-{#  <div class="modal-body">#}
-{#    {% crispy form form.helper %}#}
-{#  </div>#}
-{##}
-{#  <div class="modal-footer">#}
-{#      <input type="submit" name="submit" value="{% trans "Create" %}" class="btn btn-primary submit-btn btn btn-primary"#}
-{#             id="submit-id-submit"></div>#}
-{#</form>#}
-{##}
-
 {% load i18n %}
 {% load widget_tweaks %}
+{{ form.media }}
 
 <form method="post" action="">
     {% csrf_token %}
-    {{ form.media }}
     <div class="modal-header">
-        <h3 class="modal-title">{% trans "Create meals" %}</h3>
+        <h3 class="modal-title">{% trans "Update meals" %}</h3>
         <button type="button" class="close" data-dismiss="modal" aria-label="Close">
             <span aria-hidden="true">&times;</span>
         </button>
     </div>
 
     <div class="modal-body">
 
@@ -53,10 +33,10 @@
                     {% endfor %}
                 </div>
             </div>
         {% endfor %}
     </div>
 
     <div class="modal-footer">
-        <button type="submit" class="submit-btn btn btn-primary">{% trans "Create" %}</button>
+        <button type="submit" class="submit-btn btn btn-primary">{% trans "Update" %}</button>
     </div>
 </form>
```

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/meals/mealdailyfollowup_update.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/diaperchange/diaperchange_create.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
+{% load static %}
 {% load i18n %}
 {% load widget_tweaks %}
+{{ form.media }}
 
 <form method="post" action="">
     {% csrf_token %}
-    {{ form.media }}
     <div class="modal-header">
-        <h3 class="modal-title">{% trans "Update meals" %}</h3>
+        <h3 class="modal-title">{% trans "Create diaper change" %}</h3>
         <button type="button" class="close" data-dismiss="modal" aria-label="Close">
             <span aria-hidden="true">&times;</span>
         </button>
     </div>
 
     <div class="modal-body">
-
         <div class="{% if form.non_field_errors %}invalid{% endif %} mb-2">
             {% for error in form.non_field_errors %}
                 {{ error }}
             {% endfor %}
         </div>
 
         {% for field in form %}
@@ -33,10 +33,11 @@
                     {% endfor %}
                 </div>
             </div>
         {% endfor %}
     </div>
 
     <div class="modal-footer">
-        <button type="submit" class="submit-btn btn btn-primary">{% trans "Update" %}</button>
+        <button type="submit" class="submit-btn btn btn-primary">{% trans "Create" %}</button>
     </div>
 </form>
+
```

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/medication_confirm_delete.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/medication_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/medication_create.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/medication_create.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% load widget_tweaks static i18n %}
+{{ form.media }}
 
 <form method="post" action="" enctype="multipart/form-data">
     {% csrf_token %}
-    {{ form.media }}
     <div class="modal-header">
         <h3 class="modal-title">{% trans "Create Medication" %}</h3>
         <button type="button" class="close" data-dismiss="modal" aria-label="Close">
             <span aria-hidden="true">&times;</span>
         </button>
     </div>
```

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/medication_multiday.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/medication_multiday.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/medication_update.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/medication_update.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% load widget_tweaks static i18n %}
+{{ form.media }}
 
 <form method="post" action="" enctype="multipart/form-data">
     {% csrf_token %}
-    {{ form.media }}
     <div class="modal-header">
         <h3 class="modal-title">{% trans "Update Medication" %}</h3>
         <button type="button" class="close" data-dismiss="modal" aria-label="Close">
             <span aria-hidden="true">&times;</span>
         </button>
     </div>
```

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/nap/nap_confirm_delete.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/nap/nap_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/nap/nap_create.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_update.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-{% load i18n %}
-{% load widget_tweaks %}
+{% load widget_tweaks static i18n %}
+{{ form.media }}
 
 <form method="post" action="">
     {% csrf_token %}
-    {{ form.media }}
     <div class="modal-header">
-        <h3 class="modal-title">{% trans "Create Nap" %}</h3>
+        <h3 class="modal-title">{% trans "Update presence" %}</h3>
         <button type="button" class="close" data-dismiss="modal" aria-label="Close">
             <span aria-hidden="true">&times;</span>
         </button>
     </div>
 
     <div class="modal-body">
 
@@ -33,10 +32,11 @@
                     {% endfor %}
                 </div>
             </div>
         {% endfor %}
     </div>
 
     <div class="modal-footer">
-        <button type="submit" class="submit-btn btn btn-primary">{% trans "Create" %}</button>
+        <button type="submit" class="submit-btn btn btn-primary">{% trans "Update" %}</button>
     </div>
+
 </form>
```

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/nap/nap_update.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/nap/nap_update.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {% load i18n %}
 {% load widget_tweaks %}
+{{ form.media }}
 
 <form method="post" action="">
     {% csrf_token %}
-    {{ form.media }}
     <div class="modal-header">
         <h3 class="modal-title">{% trans "Update Nap" %}</h3>
         <button type="button" class="close" data-dismiss="modal" aria-label="Close">
             <span aria-hidden="true">&times;</span>
         </button>
     </div>
```

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/admin_presence_week_list.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/admin_presence_week_list.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_choice_classroom.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_choice_classroom.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_create.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_update.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 {% load i18n %}
 {% load widget_tweaks %}
+{{ form.media }}
 
 <form method="post" action="">
     {% csrf_token %}
-    {{ form.media }}
     <div class="modal-header">
-        <h3 class="modal-title">{% trans "Create Presence" %}</h3>
+        <h3 class="modal-title">{% trans "Update Early troubleshooting" %}</h3>
         <button type="button" class="close" data-dismiss="modal" aria-label="Close">
             <span aria-hidden="true">&times;</span>
         </button>
     </div>
 
     <div class="modal-body">
 
@@ -33,10 +33,10 @@
                     {% endfor %}
                 </div>
             </div>
         {% endfor %}
     </div>
 
     <div class="modal-footer">
-        <button type="submit" class="submit-btn btn btn-primary">{% trans "Create" %}</button>
+        <button type="submit" class="submit-btn btn btn-primary">{% trans "Update" %}</button>
     </div>
 </form>
```

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_update.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/reception/reception_update.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-{% load widget_tweaks static i18n %}
+{% load i18n %}
+{% load widget_tweaks %}
+{{ form.media }}
 
 <form method="post" action="">
     {% csrf_token %}
-    {{ form.media }}
     <div class="modal-header">
-        <h3 class="modal-title">{% trans "Update presence" %}</h3>
+        <h3 class="modal-title">{% trans "Update reception" %}</h3>
         <button type="button" class="close" data-dismiss="modal" aria-label="Close">
             <span aria-hidden="true">&times;</span>
         </button>
     </div>
 
     <div class="modal-body">
 
@@ -34,9 +35,8 @@
             </div>
         {% endfor %}
     </div>
 
     <div class="modal-footer">
         <button type="submit" class="submit-btn btn btn-primary">{% trans "Update" %}</button>
     </div>
-
 </form>
```

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_week_kindergarten_list.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_week_kindergarten_list.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_week_list.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_week_list.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence_choice.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence_choice.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence_detail_list.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence_detail_list.html`

 * *Files 1% similar despite different names*

```diff
@@ -204,18 +204,15 @@
     <!-- modal instanstiation -->
 
     {% include "includes/modal.html" %}
 {% endblock %}
 
 {% block extrajs %}
     {{ block.super }}
-    <script src="{% static 'js/moment-with-locales.min.js' %}"></script>
     <script src="{% static 'vendor/DataTables/datatables.min.js' %}"></script>
-    <script src="{% static 'js/jquery.bootstrap.modal.forms.min.js' %}"></script>
-    <script type="text/javascript" src="{% static 'js/vendor/bootstrap-datetimepicker.min.js' %}"></script>
     <script>
         function docReady(fn) {
             // see if DOM is already available
             if (document.readyState === "complete" || document.readyState === "interactive") {
                 // call on next available tick
                 setTimeout(fn, 1);
             } else {
```

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/reception/reception_update.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/diaperchange/diaperchange_update.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
+{% load static %}
 {% load i18n %}
 {% load widget_tweaks %}
+{{ form.media }}
 
 <form method="post" action="">
     {% csrf_token %}
-    {{ form.media }}
     <div class="modal-header">
-        <h3 class="modal-title">{% trans "Update reception" %}</h3>
+        <h3 class="modal-title">{% trans "Update diaper change" %}</h3>
         <button type="button" class="close" data-dismiss="modal" aria-label="Close">
             <span aria-hidden="true">&times;</span>
         </button>
     </div>
 
     <div class="modal-body">
-
         <div class="{% if form.non_field_errors %}invalid{% endif %} mb-2">
             {% for error in form.non_field_errors %}
                 {{ error }}
             {% endfor %}
         </div>
 
         {% for field in form %}
@@ -36,7 +36,8 @@
         {% endfor %}
     </div>
 
     <div class="modal-footer">
         <button type="submit" class="submit-btn btn btn-primary">{% trans "Update" %}</button>
     </div>
 </form>
+
```

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/stroll/stroll_choice_classroom.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/stroll/stroll_choice_classroom.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/stroll/stroll_pdf.html` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/stroll/stroll_pdf.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templatetags/__init__.py` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templatetags/__init__.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templatetags/notifications_custom_tags.py` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templatetags/notifications_custom_tags.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templatetags/replacement_classroom_tags.py` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/templatetags/replacement_classroom_tags.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/test_utils/__init__.py` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/test_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/test_utils/test_app/__init__.py` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/test_utils/test_app/__init__.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/test_utils/test_app/admin.py` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/test_utils/test_app/admin.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/test_utils/test_app/apps.py` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/test_utils/test_app/apps.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/test_utils/test_app/migrations/__init__.py` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/test_utils/test_app/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/test_utils/test_app/models.py` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/test_utils/test_app/models.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/urls.py` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/urls.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/utils.py` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/utils.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/views.py` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/views.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/widgets.py` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up/widgets.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up.egg-info/PKG-INFO` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobinobi-daily-follow-up
-Version: 0.1.2.6
+Version: 0.1.2.7
 Summary: Application Daily follow-up for nobinobi
 Home-page: https://github.com/prolibre-ch/nobinobi-daily-follow-up
 Author: Florian Alu
 Author-email: alu@prolibre.com
 Keywords: nobinobi-daily-follow-up
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django :: 3.1
@@ -135,14 +135,19 @@
 
 
 
 
 History
 -------
 
+0.1.2.7 (2023-06-21)
++++++++++++++++++++++++++
+
+* bd33989 - Fix date time picker
+
 0.1.2.6 (2023-06-20)
 +++++++++++++++++++++++++
 
 * 33ddd86 - fix error in create presence day table
 * Update requirements
 
 0.1.2.5 (2023-06-15)
```

### Comparing `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up.egg-info/SOURCES.txt` & `nobinobi-daily-follow-up-0.1.2.7/nobinobi_daily_follow_up.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,14 @@
 nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence_choice.html
 nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence_detail_list.html
 nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_choice_classroom.html
 nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_confirm_delete.html
 nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_create.html
 nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_update.html
 nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/group_activity_update.html
-nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/bootstrap_datepicker_plus/time-picker.html
 nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/dailyfollowup_update.html
 nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/group_choice_classroom.html
 nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/group_daily_follow_up_update.html
 nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/summary_week.html
 nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/summary_week_choice.html
 nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowuptomedication/dailyfollowuptomedication_confirm_delete.html
 nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowuptomedication/dailyfollowuptomedication_create.html
```

### Comparing `nobinobi-daily-follow-up-0.1.2.6/setup.py` & `nobinobi-daily-follow-up-0.1.2.7/setup.py`

 * *Files identical despite different names*

