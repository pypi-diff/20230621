# Comparing `tmp/aa_memberaudit-2.9.0.tar.gz` & `tmp/aa_memberaudit-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa_memberaudit-2.9.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aa_memberaudit-2.9.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aa_memberaudit-2.9.0.tar` & `aa_memberaudit-2.9.1.tar`

### file list

```diff
@@ -1,236 +1,241 @@
--rw-r--r--   0        0        0     1070 2020-12-07 16:50:18.594218 aa_memberaudit-2.9.0/LICENSE
--rw-r--r--   0        0        0     5782 2023-05-08 12:02:59.444605 aa_memberaudit-2.9.0/README.md
--rw-r--r--   0        0        0      240 2023-06-16 11:16:00.600980 aa_memberaudit-2.9.0/memberaudit/__init__.py
--rw-r--r--   0        0        0    24242 2023-06-16 10:42:01.351559 aa_memberaudit-2.9.0/memberaudit/admin.py
--rw-r--r--   0        0        0     4486 2023-03-22 16:51:39.502903 aa_memberaudit-2.9.0/memberaudit/app_settings.py
--rw-r--r--   0        0        0      317 2023-03-22 16:51:39.502903 aa_memberaudit-2.9.0/memberaudit/apps.py
--rw-r--r--   0        0        0     1223 2021-05-04 15:11:43.693169 aa_memberaudit-2.9.0/memberaudit/auth_hooks.py
--rw-r--r--   0        0        0     1242 2023-03-22 20:38:17.650401 aa_memberaudit-2.9.0/memberaudit/checks.py
--rw-r--r--   0        0        0     1354 2023-03-22 22:31:11.057446 aa_memberaudit-2.9.0/memberaudit/constants.py
--rw-r--r--   0        0        0        0 2023-06-16 11:41:55.994440 aa_memberaudit-2.9.0/memberaudit/core/__init__.py
--rw-r--r--   0        0        0    11702 2023-06-16 09:54:37.516799 aa_memberaudit-2.9.0/memberaudit/core/data_exporters.py
--rw-r--r--   0        0        0    19286 2023-06-16 09:54:37.516799 aa_memberaudit-2.9.0/memberaudit/core/eft_parser.py
--rw-r--r--   0        0        0     5439 2023-05-08 11:52:50.148096 aa_memberaudit-2.9.0/memberaudit/core/fittings.py
--rw-r--r--   0        0        0     2219 2022-09-03 21:36:22.049912 aa_memberaudit-2.9.0/memberaudit/core/skill_plans.py
--rw-r--r--   0        0        0     5362 2023-06-16 09:54:37.516799 aa_memberaudit-2.9.0/memberaudit/core/skills.py
--rw-r--r--   0        0        0     3159 2023-06-16 09:54:37.516799 aa_memberaudit-2.9.0/memberaudit/core/xml_converter.py
--rw-r--r--   0        0        0     2346 2023-06-16 09:54:37.520799 aa_memberaudit-2.9.0/memberaudit/decorators.py
--rw-r--r--   0        0        0     3691 2023-06-16 09:54:37.520799 aa_memberaudit-2.9.0/memberaudit/forms.py
--rw-r--r--   0        0        0     2331 2023-06-16 09:54:37.520799 aa_memberaudit-2.9.0/memberaudit/helpers.py
--rw-r--r--   0        0        0      384 2023-04-25 19:10:30.704306 aa_memberaudit-2.9.0/memberaudit/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    43105 2023-06-15 19:47:27.818479 aa_memberaudit-2.9.0/memberaudit/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    43046 2023-06-15 19:47:27.818479 aa_memberaudit-2.9.0/memberaudit/locale/django.pot
--rw-r--r--   0        0        0    43093 2023-06-15 19:47:27.822479 aa_memberaudit-2.9.0/memberaudit/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      380 2023-04-19 20:05:21.889406 aa_memberaudit-2.9.0/memberaudit/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    43093 2023-06-15 19:47:27.822479 aa_memberaudit-2.9.0/memberaudit/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      450 2023-04-25 19:10:30.708306 aa_memberaudit-2.9.0/memberaudit/locale/fr_FR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    43171 2023-06-15 19:47:27.822479 aa_memberaudit-2.9.0/memberaudit/locale/fr_FR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      438 2023-04-25 19:10:30.712306 aa_memberaudit-2.9.0/memberaudit/locale/it_IT/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    43159 2023-06-15 19:47:27.822479 aa_memberaudit-2.9.0/memberaudit/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      379 2023-04-25 19:10:30.712306 aa_memberaudit-2.9.0/memberaudit/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    43100 2023-06-15 19:47:27.822479 aa_memberaudit-2.9.0/memberaudit/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      391 2023-04-25 19:10:30.716307 aa_memberaudit-2.9.0/memberaudit/locale/ko_KR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    43112 2023-06-15 19:47:27.822479 aa_memberaudit-2.9.0/memberaudit/locale/ko_KR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    26859 2023-04-25 19:10:30.716307 aa_memberaudit-2.9.0/memberaudit/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    54952 2023-06-15 19:47:27.822479 aa_memberaudit-2.9.0/memberaudit/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      609 2023-04-25 19:10:30.716307 aa_memberaudit-2.9.0/memberaudit/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    43330 2023-06-15 19:47:27.826479 aa_memberaudit-2.9.0/memberaudit/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      373 2023-04-19 20:05:21.917406 aa_memberaudit-2.9.0/memberaudit/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    43086 2023-06-15 19:47:27.826479 aa_memberaudit-2.9.0/memberaudit/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      102 2020-11-24 21:31:34.925680 aa_memberaudit-2.9.0/memberaudit/management/commands/__init__.py
--rw-r--r--   0        0        0     1441 2023-06-16 09:54:37.520799 aa_memberaudit-2.9.0/memberaudit/management/commands/memberaudit_data_export.py
--rw-r--r--   0        0        0     1374 2023-06-16 09:54:37.520799 aa_memberaudit-2.9.0/memberaudit/management/commands/memberaudit_load_eve.py
--rw-r--r--   0        0        0     3859 2023-06-16 09:54:37.520799 aa_memberaudit-2.9.0/memberaudit/management/commands/memberaudit_reset_characters.py
--rw-r--r--   0        0        0      740 2023-06-16 09:54:37.524799 aa_memberaudit-2.9.0/memberaudit/management/commands/memberaudit_stats.py
--rw-r--r--   0        0        0     1941 2023-06-16 09:54:37.524799 aa_memberaudit-2.9.0/memberaudit/management/commands/memberaudit_update_characters.py
--rw-r--r--   0        0        0        0 2023-06-16 11:41:55.994440 aa_memberaudit-2.9.0/memberaudit/managers/__init__.py
--rw-r--r--   0        0        0    13021 2023-06-16 09:54:37.524799 aa_memberaudit-2.9.0/memberaudit/managers/character.py
--rw-r--r--   0        0        0    21508 2023-06-16 09:54:37.524799 aa_memberaudit-2.9.0/memberaudit/managers/general.py
--rw-r--r--   0        0        0    49552 2023-06-16 09:54:37.528799 aa_memberaudit-2.9.0/memberaudit/managers/sections.py
--rw-r--r--   0        0        0    65995 2023-02-24 17:11:11.385592 aa_memberaudit-2.9.0/memberaudit/migrations/0001_initial_new.py
--rw-r--r--   0        0        0     3444 2023-02-24 17:11:11.385592 aa_memberaudit-2.9.0/memberaudit/migrations/0002_add_mining_ledger.py
--rw-r--r--   0        0        0     1478 2023-02-24 17:11:11.385592 aa_memberaudit-2.9.0/memberaudit/migrations/0003_add_notify_permission.py
--rw-r--r--   0        0        0      513 2023-02-24 17:11:11.385592 aa_memberaudit-2.9.0/memberaudit/migrations/0004_character_is_disabled.py
--rw-r--r--   0        0        0     3819 2023-03-22 20:57:15.506894 aa_memberaudit-2.9.0/memberaudit/migrations/0005_add_fw_stats.py
--rw-r--r--   0        0        0     5969 2023-04-16 16:03:49.361835 aa_memberaudit-2.9.0/memberaudit/migrations/0006_add_localizations.py
--rw-r--r--   0        0        0     2129 2023-04-19 20:05:21.917406 aa_memberaudit-2.9.0/memberaudit/migrations/0007_add_localization_2.py
--rw-r--r--   0        0        0     2727 2023-06-15 13:23:00.558207 aa_memberaudit-2.9.0/memberaudit/migrations/0008_improve_skill_sets.py
--rw-r--r--   0        0        0     3274 2023-06-15 21:43:52.147759 aa_memberaudit-2.9.0/memberaudit/migrations/0009_add_planetary_industry.py
--rw-r--r--   0        0        0        0 2023-06-16 11:41:55.998440 aa_memberaudit-2.9.0/memberaudit/migrations/__init__.py
--rw-r--r--   0        0        0     1054 2023-06-15 19:47:27.826479 aa_memberaudit-2.9.0/memberaudit/models/__init__.py
--rw-r--r--   0        0        0    55242 2023-06-15 19:47:27.830479 aa_memberaudit-2.9.0/memberaudit/models/character.py
--rw-r--r--   0        0        0      108 2021-01-17 22:43:01.025805 aa_memberaudit-2.9.0/memberaudit/models/constants.py
--rw-r--r--   0        0        0    16994 2023-06-16 10:42:01.351559 aa_memberaudit-2.9.0/memberaudit/models/general.py
--rw-r--r--   0        0        0    40984 2023-06-15 21:43:52.147759 aa_memberaudit-2.9.0/memberaudit/models/sections.py
--rw-r--r--   0        0        0      256 2023-06-16 09:54:37.528799 aa_memberaudit-2.9.0/memberaudit/providers.py
--rw-r--r--   0        0        0      509 2022-03-05 14:47:06.220060 aa_memberaudit-2.9.0/memberaudit/signals.py
--rw-r--r--   0        0        0      191 2023-02-24 14:11:29.027672 aa_memberaudit-2.9.0/memberaudit/static/memberaudit/css/admin.css
--rw-r--r--   0        0        0      174 2022-02-09 21:55:36.823364 aa_memberaudit-2.9.0/memberaudit/static/memberaudit/css/character_finder.css
--rw-r--r--   0        0        0     5736 2023-06-15 20:13:14.507685 aa_memberaudit-2.9.0/memberaudit/static/memberaudit/css/character_viewer.css
--rw-r--r--   0        0        0     2540 2021-01-29 15:59:17.153310 aa_memberaudit-2.9.0/memberaudit/static/memberaudit/css/character_viewer.min.css
--rw-r--r--   0        0        0       94 2022-11-27 20:20:23.212674 aa_memberaudit-2.9.0/memberaudit/static/memberaudit/css/data_export.css
--rw-r--r--   0        0        0     1538 2021-05-04 21:32:43.714694 aa_memberaudit-2.9.0/memberaudit/static/memberaudit/css/global.css
--rw-r--r--   0        0        0      646 2021-01-29 15:59:17.153310 aa_memberaudit-2.9.0/memberaudit/static/memberaudit/css/global.min.css
--rw-r--r--   0        0        0     4331 2020-11-03 21:09:40.510944 aa_memberaudit-2.9.0/memberaudit/static/memberaudit/css/launcher.css
--rw-r--r--   0        0        0     2765 2021-01-29 15:59:17.153310 aa_memberaudit-2.9.0/memberaudit/static/memberaudit/css/launcher.min.css
--rw-r--r--   0        0        0     1363 2021-02-16 17:03:36.468870 aa_memberaudit-2.9.0/memberaudit/static/memberaudit/css/memberaudit.css
--rw-r--r--   0        0        0      617 2021-02-16 17:03:36.468870 aa_memberaudit-2.9.0/memberaudit/static/memberaudit/css/memberaudit.min.css
--rw-r--r--   0        0        0      611 2021-02-17 10:40:00.762093 aa_memberaudit-2.9.0/memberaudit/static/memberaudit/css/reports.css
--rw-r--r--   0        0        0    43262 2020-10-26 16:42:17.713201 aa_memberaudit-2.9.0/memberaudit/static/memberaudit/images/Spinner-1s-64px-dark.gif
--rw-r--r--   0        0        0    43381 2020-10-26 16:42:17.713201 aa_memberaudit-2.9.0/memberaudit/static/memberaudit/images/Spinner-1s-64px-light.gif
--rw-r--r--   0        0        0     1862 2021-02-23 10:36:55.530247 aa_memberaudit-2.9.0/memberaudit/static/memberaudit/images/charisma.png
--rw-r--r--   0        0        0      694 2020-11-03 21:09:40.510944 aa_memberaudit-2.9.0/memberaudit/static/memberaudit/images/eve-prism.png
--rw-r--r--   0        0        0      220 2020-11-03 21:09:40.510944 aa_memberaudit-2.9.0/memberaudit/static/memberaudit/images/evelogo.png
--rw-r--r--   0        0        0      595 2020-11-03 21:09:40.510944 aa_memberaudit-2.9.0/memberaudit/static/memberaudit/images/evesearch.png
--rw-r--r--   0        0        0     1966 2021-02-23 10:36:55.530247 aa_memberaudit-2.9.0/memberaudit/static/memberaudit/images/intelligence.png
--rw-r--r--   0        0        0     1809 2021-02-23 10:36:55.530247 aa_memberaudit-2.9.0/memberaudit/static/memberaudit/images/memory.png
--rw-r--r--   0        0        0     1803 2021-02-23 10:36:55.530247 aa_memberaudit-2.9.0/memberaudit/static/memberaudit/images/perception.png
--rw-r--r--   0        0        0     1782 2021-02-23 10:36:55.530247 aa_memberaudit-2.9.0/memberaudit/static/memberaudit/images/willpower.png
--rw-r--r--   0        0        0      259 2020-10-22 17:18:29.995572 aa_memberaudit-2.9.0/memberaudit/static/memberaudit/images/zkillboard.png
--rw-r--r--   0        0        0     5573 2020-10-22 17:18:29.995572 aa_memberaudit-2.9.0/memberaudit/static/memberaudit/vendor/datatables/plugins/dataTables.rowGroup.min.js
--rw-r--r--   0        0        0     3908 2022-04-01 19:33:31.239451 aa_memberaudit-2.9.0/memberaudit/static/memberaudit/vendor/datatables/plugins/datetime.js
--rw-r--r--   0        0        0     2529 2022-04-01 19:48:30.310949 aa_memberaudit-2.9.0/memberaudit/static/memberaudit/vendor/datatables/plugins/filterDropDown.min.js
--rw-r--r--   0        0        0      384 2020-10-22 17:18:29.995572 aa_memberaudit-2.9.0/memberaudit/static/memberaudit/vendor/datatables/plugins/rowGroup.bootstrap.min.css
--rw-r--r--   0        0        0      384 2020-10-22 17:18:29.995572 aa_memberaudit-2.9.0/memberaudit/static/memberaudit/vendor/datatables/plugins/rowGroup.dataTables.min.css
--rw-r--r--   0        0        0    69950 2020-10-28 14:46:25.711812 aa_memberaudit-2.9.0/memberaudit/static/memberaudit/vendor/moment/moment.min.js
--rw-r--r--   0        0        0   881821 2023-02-16 19:01:05.384001 aa_memberaudit-2.9.0/memberaudit/swagger.json
--rw-r--r--   0        0        0    40181 2023-06-16 09:54:37.528799 aa_memberaudit-2.9.0/memberaudit/tasks.py
--rw-r--r--   0        0        0      687 2023-04-16 16:03:49.365835 aa_memberaudit-2.9.0/memberaudit/templates/admin/memberaudit/character/confirm_character_deletion.html
--rw-r--r--   0        0        0      488 2022-09-02 18:40:08.749489 aa_memberaudit-2.9.0/memberaudit/templates/admin/memberaudit/skillset/change_list.html
--rw-r--r--   0        0        0      848 2023-04-16 16:03:49.365835 aa_memberaudit-2.9.0/memberaudit/templates/admin/memberaudit/skillset/import_skills.html
--rw-r--r--   0        0        0      367 2020-12-07 00:53:01.652277 aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/base.html
--rw-r--r--   0        0        0     4801 2023-04-25 19:10:30.720306 aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/character_finder.html
--rw-r--r--   0        0        0    29413 2023-06-16 09:54:37.528799 aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/character_viewer.html
--rw-r--r--   0        0        0     2932 2023-04-25 19:10:30.720306 aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/data_export.html
--rw-r--r--   0        0        0     8515 2023-04-16 16:03:49.365835 aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/launcher.html
--rw-r--r--   0        0        0     1238 2021-01-29 15:52:00.995855 aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/modals/character_viewer/asset_container.html
--rw-r--r--   0        0        0     4307 2022-04-01 19:33:31.243451 aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/modals/character_viewer/asset_container_content.html
--rw-r--r--   0        0        0     1713 2021-02-18 07:41:27.336226 aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/modals/character_viewer/character_skill_set_details.html
--rw-r--r--   0        0        0     1246 2020-11-01 21:48:51.676098 aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/modals/character_viewer/contract.html
--rw-r--r--   0        0        0     8075 2023-04-16 16:03:49.365835 aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/modals/character_viewer/contract_content.html
--rw-r--r--   0        0        0      658 2023-04-16 16:03:49.365835 aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/modals/character_viewer/contract_items.html
--rw-r--r--   0        0        0     1375 2022-02-09 21:55:36.827364 aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/modals/character_viewer/mail.html
--rw-r--r--   0        0        0      382 2023-04-16 16:03:49.369835 aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/modals/character_viewer/mail_content.html
--rw-r--r--   0        0        0     3880 2022-04-01 19:33:31.243451 aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/modals/character_viewer/skill_set_content.html
--rw-r--r--   0        0        0     9005 2023-06-15 11:31:30.596583 aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/character_viewer/overview.html
--rw-r--r--   0        0        0     1451 2023-04-16 16:03:49.369835 aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/character_viewer/sidebar.html
--rw-r--r--   0        0        0      637 2023-06-15 19:47:27.834479 aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/character_viewer/sidebar_character.html
--rw-r--r--   0        0        0     1256 2023-06-15 19:47:27.834479 aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/assets.html
--rw-r--r--   0        0        0      560 2023-06-15 19:47:27.834479 aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes.html
--rw-r--r--   0        0        0     2604 2021-02-23 15:40:36.322996 aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes_content.html
--rw-r--r--   0        0        0      314 2023-06-15 19:47:27.834479 aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_bio.html
--rw-r--r--   0        0        0      848 2023-06-15 19:47:27.834479 aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contacts.html
--rw-r--r--   0        0        0      960 2023-06-15 19:47:27.834479 aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contracts.html
--rw-r--r--   0        0        0      582 2023-06-15 19:47:27.834479 aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history.html
--rw-r--r--   0        0        0      894 2020-12-14 23:31:49.226782 aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html
--rw-r--r--   0        0        0      549 2023-06-15 19:47:27.834479 aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats.html
--rw-r--r--   0        0        0     2786 2023-04-16 16:03:49.373835 aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats_content.html
--rw-r--r--   0        0        0      563 2023-06-15 19:47:27.834479 aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/implants.html
--rw-r--r--   0        0        0      721 2023-06-15 19:47:27.838479 aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/jump_clones.html
--rw-r--r--   0        0        0      148 2020-11-09 19:29:14.885373 aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/last_updated.html
--rw-r--r--   0        0        0      611 2023-06-15 19:47:27.838479 aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/loyalty.html
--rw-r--r--   0        0        0     2878 2023-06-15 19:47:27.838479 aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mails.html
--rw-r--r--   0        0        0      779 2023-06-15 19:47:27.838479 aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mining_ledger.html
--rw-r--r--   0        0        0      885 2023-06-16 09:54:37.528799 aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/planets.html
--rw-r--r--   0        0        0      669 2023-06-15 19:47:27.838479 aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_queue.html
--rw-r--r--   0        0        0      882 2023-06-15 19:47:27.838479 aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_sets.html
--rw-r--r--   0        0        0      592 2023-06-15 19:47:27.838479 aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skills.html
--rw-r--r--   0        0        0      907 2023-06-15 19:47:27.838479 aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_journal.html
--rw-r--r--   0        0        0      916 2023-06-15 19:47:27.838479 aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_transactions.html
--rw-r--r--   0        0        0     3941 2023-06-15 19:47:27.838479 aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs_navigation.html
--rw-r--r--   0        0        0     2674 2022-01-23 15:08:18.156059 aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/menu.html
--rw-r--r--   0        0        0      292 2023-04-16 16:03:49.373835 aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/reports/tabs/_compliance_color_code.html
--rw-r--r--   0        0        0      684 2023-04-16 16:03:49.373835 aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/reports/tabs/corporation_compliance.html
--rw-r--r--   0        0        0      760 2023-04-16 16:03:49.377835 aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/reports/tabs/skill_sets.html
--rw-r--r--   0        0        0      775 2023-04-16 16:03:49.377835 aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/reports/tabs/user_compliance.html
--rw-r--r--   0        0        0      691 2021-02-16 15:13:05.236586 aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/reports/tabs_navigation.html
--rw-r--r--   0        0        0      709 2023-04-16 16:03:49.377835 aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/solar_system.html
--rw-r--r--   0        0        0     9420 2022-04-01 19:56:47.910687 aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/reports.html
--rw-r--r--   0        0        0        0 2023-06-16 11:41:56.026440 aa_memberaudit-2.9.0/memberaudit/templatetags/__init__.py
--rw-r--r--   0        0        0      330 2021-01-05 22:10:38.500385 aa_memberaudit-2.9.0/memberaudit/templatetags/memberaudit.py
--rw-r--r--   0        0        0        0 2023-06-16 11:41:56.026440 aa_memberaudit-2.9.0/memberaudit/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-06-16 11:41:56.026440 aa_memberaudit-2.9.0/memberaudit/tests/core/__init__.py
--rw-r--r--   0        0        0     6350 2023-06-16 09:54:37.532799 aa_memberaudit-2.9.0/memberaudit/tests/core/test_core_xml_converter.py
--rw-r--r--   0        0        0    12727 2023-06-16 09:54:37.532799 aa_memberaudit-2.9.0/memberaudit/tests/core/test_data_exporters.py
--rw-r--r--   0        0        0    22366 2023-06-16 09:54:37.532799 aa_memberaudit-2.9.0/memberaudit/tests/core/test_eft_parser.py
--rw-r--r--   0        0        0     6371 2023-06-16 09:54:37.536799 aa_memberaudit-2.9.0/memberaudit/tests/core/test_fittings.py
--rw-r--r--   0        0        0     4082 2022-09-03 21:36:22.049912 aa_memberaudit-2.9.0/memberaudit/tests/core/test_skill_plans.py
--rw-r--r--   0        0        0     2458 2023-06-16 09:54:37.536799 aa_memberaudit-2.9.0/memberaudit/tests/core/test_skills.py
--rw-r--r--   0        0        0        0 2023-06-16 11:41:56.030440 aa_memberaudit-2.9.0/memberaudit/tests/managers/__init__.py
--rw-r--r--   0        0        0    18357 2023-02-24 14:11:29.027672 aa_memberaudit-2.9.0/memberaudit/tests/managers/test_character.py
--rw-r--r--   0        0        0    41576 2023-04-20 18:56:43.507645 aa_memberaudit-2.9.0/memberaudit/tests/managers/test_general.py
--rw-r--r--   0        0        0     5209 2023-06-16 09:54:37.536799 aa_memberaudit-2.9.0/memberaudit/tests/managers/test_sections.py
--rw-r--r--   0        0        0        0 2023-06-16 11:41:56.030440 aa_memberaudit-2.9.0/memberaudit/tests/models/__init__.py
--rw-r--r--   0        0        0    36071 2023-06-16 09:54:37.536799 aa_memberaudit-2.9.0/memberaudit/tests/models/test_character_1.py
--rw-r--r--   0        0        0    35844 2023-06-16 09:54:37.536799 aa_memberaudit-2.9.0/memberaudit/tests/models/test_character_2.py
--rw-r--r--   0        0        0    40708 2023-06-16 09:54:37.540799 aa_memberaudit-2.9.0/memberaudit/tests/models/test_character_3.py
--rw-r--r--   0        0        0    28285 2023-06-15 19:47:27.842479 aa_memberaudit-2.9.0/memberaudit/tests/models/test_character_4.py
--rw-r--r--   0        0        0     4440 2023-06-15 19:47:27.842479 aa_memberaudit-2.9.0/memberaudit/tests/models/test_character_5.py
--rw-r--r--   0        0        0    11795 2023-06-16 10:42:01.351559 aa_memberaudit-2.9.0/memberaudit/tests/models/test_general.py
--rw-r--r--   0        0        0     2963 2023-04-19 17:34:14.731735 aa_memberaudit-2.9.0/memberaudit/tests/models/test_sections.py
--rw-r--r--   0        0        0     1058 2023-06-16 09:54:37.540799 aa_memberaudit-2.9.0/memberaudit/tests/models/utils.py
--rw-r--r--   0        0        0    15428 2023-06-15 13:23:00.558207 aa_memberaudit-2.9.0/memberaudit/tests/test_admin.py
--rw-r--r--   0        0        0     1807 2023-02-24 17:52:57.675286 aa_memberaudit-2.9.0/memberaudit/tests/test_auth_hooks.py
--rw-r--r--   0        0        0     1314 2023-03-22 16:51:39.514903 aa_memberaudit-2.9.0/memberaudit/tests/test_checks.py
--rw-r--r--   0        0        0     3487 2023-06-16 09:54:37.540799 aa_memberaudit-2.9.0/memberaudit/tests/test_commands.py
--rw-r--r--   0        0        0     4083 2023-06-16 09:54:37.540799 aa_memberaudit-2.9.0/memberaudit/tests/test_decorators.py
--rw-r--r--   0        0        0      900 2023-06-16 09:54:37.540799 aa_memberaudit-2.9.0/memberaudit/tests/test_factories.py
--rw-r--r--   0        0        0     3516 2022-09-03 16:21:19.096009 aa_memberaudit-2.9.0/memberaudit/tests/test_forms.py
--rw-r--r--   0        0        0     3824 2023-06-16 09:54:37.544799 aa_memberaudit-2.9.0/memberaudit/tests/test_helpers.py
--rw-r--r--   0        0        0    12534 2023-04-19 17:34:14.735735 aa_memberaudit-2.9.0/memberaudit/tests/test_integration.py
--rw-r--r--   0        0        0     1215 2022-03-05 14:47:06.220060 aa_memberaudit-2.9.0/memberaudit/tests/test_signals.py
--rw-r--r--   0        0        0    36906 2023-04-20 17:47:44.088801 aa_memberaudit-2.9.0/memberaudit/tests/test_tasks.py
--rw-r--r--   0        0        0      968 2023-06-16 09:54:37.544799 aa_memberaudit-2.9.0/memberaudit/tests/test_templatetags.py
--rw-r--r--   0        0        0      267 2020-10-22 17:18:30.011572 aa_memberaudit-2.9.0/memberaudit/tests/testdata/__init__.py
--rw-r--r--   0        0        0     4359 2023-06-15 19:47:27.842479 aa_memberaudit-2.9.0/memberaudit/tests/testdata/create_eveuniverse.py
--rw-r--r--   0        0        0     4350 2022-02-10 22:57:31.960297 aa_memberaudit-2.9.0/memberaudit/tests/testdata/entities.json
--rw-r--r--   0        0        0     4857 2023-06-15 19:47:27.842479 aa_memberaudit-2.9.0/memberaudit/tests/testdata/esi_client_stub.py
--rw-r--r--   0        0        0    41017 2023-06-15 19:47:27.842479 aa_memberaudit-2.9.0/memberaudit/tests/testdata/esi_testdata.json
--rw-r--r--   0        0        0  1225856 2023-06-15 19:47:27.862479 aa_memberaudit-2.9.0/memberaudit/tests/testdata/eveuniverse.json
--rw-r--r--   0        0        0    13498 2023-06-16 10:42:01.351559 aa_memberaudit-2.9.0/memberaudit/tests/testdata/factories.py
--rw-r--r--   0        0        0      799 2022-04-01 19:33:31.251451 aa_memberaudit-2.9.0/memberaudit/tests/testdata/fittings/fitting_archon.txt
--rw-r--r--   0        0        0      889 2022-04-01 19:33:31.251451 aa_memberaudit-2.9.0/memberaudit/tests/testdata/fittings/fitting_archon_max.txt
--rw-r--r--   0        0        0      231 2022-04-01 19:33:31.251451 aa_memberaudit-2.9.0/memberaudit/tests/testdata/fittings/fitting_empty.txt
--rw-r--r--   0        0        0      503 2022-04-01 19:33:31.251451 aa_memberaudit-2.9.0/memberaudit/tests/testdata/fittings/fitting_eve_celestis_no_high_slots.txt
--rw-r--r--   0        0        0      193 2022-04-01 19:33:31.251451 aa_memberaudit-2.9.0/memberaudit/tests/testdata/fittings/fitting_eve_tristan_3.txt
--rw-r--r--   0        0        0      377 2022-04-01 19:33:31.251451 aa_memberaudit-2.9.0/memberaudit/tests/testdata/fittings/fitting_eve_tristian.txt
--rw-r--r--   0        0        0      293 2022-04-01 19:33:31.251451 aa_memberaudit-2.9.0/memberaudit/tests/testdata/fittings/fitting_eve_tristian_2.txt
--rw-r--r--   0        0        0       96 2022-04-01 19:33:31.251451 aa_memberaudit-2.9.0/memberaudit/tests/testdata/fittings/fitting_eve_tristian_empty.txt
--rw-r--r--   0        0        0      583 2022-04-01 19:33:31.251451 aa_memberaudit-2.9.0/memberaudit/tests/testdata/fittings/fitting_svipul.txt
--rw-r--r--   0        0        0      432 2022-04-01 19:33:31.251451 aa_memberaudit-2.9.0/memberaudit/tests/testdata/fittings/fitting_svipul_2.txt
--rw-r--r--   0        0        0      700 2022-04-01 19:33:31.251451 aa_memberaudit-2.9.0/memberaudit/tests/testdata/fittings/fitting_tengu.txt
--rw-r--r--   0        0        0      459 2022-04-01 19:33:31.251451 aa_memberaudit-2.9.0/memberaudit/tests/testdata/fittings/fitting_tristan.txt
--rw-r--r--   0        0        0      332 2022-04-01 19:33:31.251451 aa_memberaudit-2.9.0/memberaudit/tests/testdata/fittings/fitting_tristan_missing_rigs.txt
--rw-r--r--   0        0        0      410 2022-04-01 19:33:31.251451 aa_memberaudit-2.9.0/memberaudit/tests/testdata/fittings/fitting_tristan_no_title.txt
--rw-r--r--   0        0        0      460 2022-04-01 19:33:31.251451 aa_memberaudit-2.9.0/memberaudit/tests/testdata/fittings/fitting_tristan_unknown_types.txt
--rw-r--r--   0        0        0      455 2023-05-08 11:52:50.156096 aa_memberaudit-2.9.0/memberaudit/tests/testdata/fittings/fitting_unknown_ship_type.txt
--rw-r--r--   0        0        0     4272 2023-06-16 09:54:37.544799 aa_memberaudit-2.9.0/memberaudit/tests/testdata/generate_character.py
--rw-r--r--   0        0        0     3859 2022-01-20 23:34:01.558036 aa_memberaudit-2.9.0/memberaudit/tests/testdata/generate_doctrines.py
--rw-r--r--   0        0        0     3671 2022-08-07 14:41:41.990259 aa_memberaudit-2.9.0/memberaudit/tests/testdata/load_entities.py
--rw-r--r--   0        0        0      412 2020-10-22 17:18:30.015572 aa_memberaudit-2.9.0/memberaudit/tests/testdata/load_eveuniverse.py
--rw-r--r--   0        0        0     1188 2022-02-10 21:29:55.833941 aa_memberaudit-2.9.0/memberaudit/tests/testdata/load_locations.py
--rw-r--r--   0        0        0     1097 2022-04-01 19:33:31.251451 aa_memberaudit-2.9.0/memberaudit/tests/testdata/pilot_esi_error_handling.py
--rw-r--r--   0        0        0      825 2022-04-01 19:33:31.259451 aa_memberaudit-2.9.0/memberaudit/tests/testdata/profiler_toolbox.py
--rw-r--r--   0        0        0     3950 2023-06-15 13:23:00.558207 aa_memberaudit-2.9.0/memberaudit/tests/utils.py
--rw-r--r--   0        0        0        0 2023-06-16 11:41:56.046440 aa_memberaudit-2.9.0/memberaudit/tests/views/__init__.py
--rw-r--r--   0        0        0     9299 2023-06-15 13:23:00.562207 aa_memberaudit-2.9.0/memberaudit/tests/views/test_admin.py
--rw-r--r--   0        0        0     7089 2023-06-16 09:54:37.544799 aa_memberaudit-2.9.0/memberaudit/tests/views/test_character_finder.py
--rw-r--r--   0        0        0    32680 2023-03-22 21:45:48.968406 aa_memberaudit-2.9.0/memberaudit/tests/views/test_character_viewer_1.py
--rw-r--r--   0        0        0    24561 2023-06-15 19:47:27.866479 aa_memberaudit-2.9.0/memberaudit/tests/views/test_character_viewer_2.py
--rw-r--r--   0        0        0    14594 2023-06-16 09:54:37.544799 aa_memberaudit-2.9.0/memberaudit/tests/views/test_characters.py
--rw-r--r--   0        0        0     4101 2023-06-16 09:54:37.544799 aa_memberaudit-2.9.0/memberaudit/tests/views/test_data_export.py
--rw-r--r--   0        0        0    16249 2023-06-16 09:54:37.544799 aa_memberaudit-2.9.0/memberaudit/tests/views/test_reports.py
--rw-r--r--   0        0        0     3051 2022-10-21 18:07:26.108963 aa_memberaudit-2.9.0/memberaudit/tools/drop_tables.sql
--rw-r--r--   0        0        0      329 2020-12-16 22:00:54.319925 aa_memberaudit-2.9.0/memberaudit/tools/total_size.sql
--rw-r--r--   0        0        0     7203 2023-06-16 09:54:37.544799 aa_memberaudit-2.9.0/memberaudit/urls.py
--rw-r--r--   0        0        0        0 2023-06-16 11:41:56.050440 aa_memberaudit-2.9.0/memberaudit/views/__init__.py
--rw-r--r--   0        0        0     1508 2023-06-16 09:54:37.548799 aa_memberaudit-2.9.0/memberaudit/views/_common.py
--rw-r--r--   0        0        0     3490 2023-06-15 13:23:00.562207 aa_memberaudit-2.9.0/memberaudit/views/admin.py
--rw-r--r--   0        0        0    12549 2023-06-16 09:54:37.548799 aa_memberaudit-2.9.0/memberaudit/views/character_finder.py
--rw-r--r--   0        0        0    24254 2023-06-15 21:43:52.151759 aa_memberaudit-2.9.0/memberaudit/views/character_viewer_1.py
--rw-r--r--   0        0        0    24494 2023-06-16 09:54:37.548799 aa_memberaudit-2.9.0/memberaudit/views/character_viewer_2.py
--rw-r--r--   0        0        0     8010 2023-06-16 09:54:37.548799 aa_memberaudit-2.9.0/memberaudit/views/characters.py
--rw-r--r--   0        0        0     2196 2023-06-16 09:54:37.548799 aa_memberaudit-2.9.0/memberaudit/views/data_export.py
--rw-r--r--   0        0        0    13130 2023-06-16 09:54:37.548799 aa_memberaudit-2.9.0/memberaudit/views/reports.py
--rw-r--r--   0        0        0     2207 2023-06-15 19:47:27.866479 aa_memberaudit-2.9.0/pyproject.toml
--rw-r--r--   0        0        0     7367 1970-01-01 00:00:00.000000 aa_memberaudit-2.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2020-12-07 16:50:18.594218 aa_memberaudit-2.9.1/LICENSE
+-rw-r--r--   0        0        0     5782 2023-05-08 12:02:59.444605 aa_memberaudit-2.9.1/README.md
+-rw-r--r--   0        0        0      240 2023-06-20 12:20:45.235100 aa_memberaudit-2.9.1/memberaudit/__init__.py
+-rw-r--r--   0        0        0    24333 2023-06-20 12:20:45.235100 aa_memberaudit-2.9.1/memberaudit/admin.py
+-rw-r--r--   0        0        0     4548 2023-06-18 14:40:14.289539 aa_memberaudit-2.9.1/memberaudit/app_settings.py
+-rw-r--r--   0        0        0      407 2023-06-18 19:47:02.522598 aa_memberaudit-2.9.1/memberaudit/apps.py
+-rw-r--r--   0        0        0     1251 2023-06-18 19:47:02.522598 aa_memberaudit-2.9.1/memberaudit/auth_hooks.py
+-rw-r--r--   0        0        0     1271 2023-06-18 14:40:14.289539 aa_memberaudit-2.9.1/memberaudit/checks.py
+-rw-r--r--   0        0        0     1704 2023-06-18 14:40:14.293539 aa_memberaudit-2.9.1/memberaudit/constants.py
+-rw-r--r--   0        0        0        0 2023-06-21 11:55:38.002082 aa_memberaudit-2.9.1/memberaudit/core/__init__.py
+-rw-r--r--   0        0        0    11526 2023-06-19 16:16:36.734579 aa_memberaudit-2.9.1/memberaudit/core/data_exporters.py
+-rw-r--r--   0        0        0    19456 2023-06-18 16:38:29.684085 aa_memberaudit-2.9.1/memberaudit/core/eft_parser.py
+-rw-r--r--   0        0        0     5563 2023-06-20 12:20:45.235100 aa_memberaudit-2.9.1/memberaudit/core/fittings.py
+-rw-r--r--   0        0        0     2244 2023-06-18 14:40:14.293539 aa_memberaudit-2.9.1/memberaudit/core/skill_plans.py
+-rw-r--r--   0        0        0     5362 2023-06-20 12:20:45.235100 aa_memberaudit-2.9.1/memberaudit/core/skills.py
+-rw-r--r--   0        0        0     3159 2023-06-16 09:54:37.516799 aa_memberaudit-2.9.1/memberaudit/core/xml_converter.py
+-rw-r--r--   0        0        0     2430 2023-06-18 14:40:14.293539 aa_memberaudit-2.9.1/memberaudit/decorators.py
+-rw-r--r--   0        0        0     3740 2023-06-18 14:40:14.293539 aa_memberaudit-2.9.1/memberaudit/forms.py
+-rw-r--r--   0        0        0     1820 2023-06-18 19:20:57.381084 aa_memberaudit-2.9.1/memberaudit/helpers.py
+-rw-r--r--   0        0        0      384 2023-04-25 19:10:30.704306 aa_memberaudit-2.9.1/memberaudit/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    43105 2023-06-15 19:47:27.818479 aa_memberaudit-2.9.1/memberaudit/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    43046 2023-06-15 19:47:27.818479 aa_memberaudit-2.9.1/memberaudit/locale/django.pot
+-rw-r--r--   0        0        0    43093 2023-06-15 19:47:27.822479 aa_memberaudit-2.9.1/memberaudit/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      380 2023-04-19 20:05:21.889406 aa_memberaudit-2.9.1/memberaudit/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    43093 2023-06-15 19:47:27.822479 aa_memberaudit-2.9.1/memberaudit/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      450 2023-04-25 19:10:30.708306 aa_memberaudit-2.9.1/memberaudit/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    43171 2023-06-15 19:47:27.822479 aa_memberaudit-2.9.1/memberaudit/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      438 2023-04-25 19:10:30.712306 aa_memberaudit-2.9.1/memberaudit/locale/it_IT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    43159 2023-06-15 19:47:27.822479 aa_memberaudit-2.9.1/memberaudit/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      379 2023-04-25 19:10:30.712306 aa_memberaudit-2.9.1/memberaudit/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    43100 2023-06-15 19:47:27.822479 aa_memberaudit-2.9.1/memberaudit/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      391 2023-04-25 19:10:30.716307 aa_memberaudit-2.9.1/memberaudit/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    43112 2023-06-15 19:47:27.822479 aa_memberaudit-2.9.1/memberaudit/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    26859 2023-04-25 19:10:30.716307 aa_memberaudit-2.9.1/memberaudit/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    54952 2023-06-15 19:47:27.822479 aa_memberaudit-2.9.1/memberaudit/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      609 2023-04-25 19:10:30.716307 aa_memberaudit-2.9.1/memberaudit/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    43330 2023-06-15 19:47:27.826479 aa_memberaudit-2.9.1/memberaudit/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      373 2023-04-19 20:05:21.917406 aa_memberaudit-2.9.1/memberaudit/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    43086 2023-06-15 19:47:27.826479 aa_memberaudit-2.9.1/memberaudit/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      102 2020-11-24 21:31:34.925680 aa_memberaudit-2.9.1/memberaudit/management/commands/__init__.py
+-rw-r--r--   0        0        0     1443 2023-06-18 19:47:02.526598 aa_memberaudit-2.9.1/memberaudit/management/commands/memberaudit_data_export.py
+-rw-r--r--   0        0        0     1374 2023-06-16 09:54:37.520799 aa_memberaudit-2.9.1/memberaudit/management/commands/memberaudit_load_eve.py
+-rw-r--r--   0        0        0     3859 2023-06-16 09:54:37.520799 aa_memberaudit-2.9.1/memberaudit/management/commands/memberaudit_reset_characters.py
+-rw-r--r--   0        0        0      740 2023-06-16 09:54:37.524799 aa_memberaudit-2.9.1/memberaudit/management/commands/memberaudit_stats.py
+-rw-r--r--   0        0        0     1941 2023-06-16 09:54:37.524799 aa_memberaudit-2.9.1/memberaudit/management/commands/memberaudit_update_characters.py
+-rw-r--r--   0        0        0        0 2023-06-21 11:55:38.006082 aa_memberaudit-2.9.1/memberaudit/managers/__init__.py
+-rw-r--r--   0        0        0    13017 2023-06-18 16:38:29.684085 aa_memberaudit-2.9.1/memberaudit/managers/character.py
+-rw-r--r--   0        0        0    26850 2023-06-20 12:20:45.239100 aa_memberaudit-2.9.1/memberaudit/managers/character_sections_1.py
+-rw-r--r--   0        0        0    29910 2023-06-20 12:20:45.239100 aa_memberaudit-2.9.1/memberaudit/managers/character_sections_2.py
+-rw-r--r--   0        0        0    25043 2023-06-19 16:16:36.738579 aa_memberaudit-2.9.1/memberaudit/managers/character_sections_3.py
+-rw-r--r--   0        0        0    24472 2023-06-18 16:38:29.684085 aa_memberaudit-2.9.1/memberaudit/managers/general.py
+-rw-r--r--   0        0        0    65995 2023-02-24 17:11:11.385592 aa_memberaudit-2.9.1/memberaudit/migrations/0001_initial_new.py
+-rw-r--r--   0        0        0     3444 2023-02-24 17:11:11.385592 aa_memberaudit-2.9.1/memberaudit/migrations/0002_add_mining_ledger.py
+-rw-r--r--   0        0        0     1478 2023-02-24 17:11:11.385592 aa_memberaudit-2.9.1/memberaudit/migrations/0003_add_notify_permission.py
+-rw-r--r--   0        0        0      513 2023-02-24 17:11:11.385592 aa_memberaudit-2.9.1/memberaudit/migrations/0004_character_is_disabled.py
+-rw-r--r--   0        0        0     3819 2023-03-22 20:57:15.506894 aa_memberaudit-2.9.1/memberaudit/migrations/0005_add_fw_stats.py
+-rw-r--r--   0        0        0     5969 2023-04-16 16:03:49.361835 aa_memberaudit-2.9.1/memberaudit/migrations/0006_add_localizations.py
+-rw-r--r--   0        0        0     2129 2023-04-19 20:05:21.917406 aa_memberaudit-2.9.1/memberaudit/migrations/0007_add_localization_2.py
+-rw-r--r--   0        0        0     2727 2023-06-15 13:23:00.558207 aa_memberaudit-2.9.1/memberaudit/migrations/0008_improve_skill_sets.py
+-rw-r--r--   0        0        0     3274 2023-06-15 21:43:52.147759 aa_memberaudit-2.9.1/memberaudit/migrations/0009_add_planetary_industry.py
+-rw-r--r--   0        0        0        0 2023-06-21 11:55:38.006082 aa_memberaudit-2.9.1/memberaudit/migrations/__init__.py
+-rw-r--r--   0        0        0     1117 2023-06-18 15:15:28.267801 aa_memberaudit-2.9.1/memberaudit/models/__init__.py
+-rw-r--r--   0        0        0    15243 2023-06-18 16:38:29.688085 aa_memberaudit-2.9.1/memberaudit/models/character_sections_1.py
+-rw-r--r--   0        0        0    13506 2023-06-18 15:15:28.267801 aa_memberaudit-2.9.1/memberaudit/models/character_sections_2.py
+-rw-r--r--   0        0        0    13923 2023-06-18 15:15:28.271801 aa_memberaudit-2.9.1/memberaudit/models/character_sections_3.py
+-rw-r--r--   0        0        0    26983 2023-06-20 12:20:45.247100 aa_memberaudit-2.9.1/memberaudit/models/characters.py
+-rw-r--r--   0        0        0      108 2021-01-17 22:43:01.025805 aa_memberaudit-2.9.1/memberaudit/models/constants.py
+-rw-r--r--   0        0        0    17213 2023-06-18 16:38:29.688085 aa_memberaudit-2.9.1/memberaudit/models/general.py
+-rw-r--r--   0        0        0      299 2023-06-18 14:40:14.297539 aa_memberaudit-2.9.1/memberaudit/providers.py
+-rw-r--r--   0        0        0      542 2023-06-18 14:40:14.297539 aa_memberaudit-2.9.1/memberaudit/signals.py
+-rw-r--r--   0        0        0      191 2023-02-24 14:11:29.027672 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/css/admin.css
+-rw-r--r--   0        0        0      174 2022-02-09 21:55:36.823364 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/css/character_finder.css
+-rw-r--r--   0        0        0     5736 2023-06-15 20:13:14.507685 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/css/character_viewer.css
+-rw-r--r--   0        0        0     2540 2021-01-29 15:59:17.153310 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/css/character_viewer.min.css
+-rw-r--r--   0        0        0       94 2022-11-27 20:20:23.212674 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/css/data_export.css
+-rw-r--r--   0        0        0     1538 2021-05-04 21:32:43.714694 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/css/global.css
+-rw-r--r--   0        0        0      646 2021-01-29 15:59:17.153310 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/css/global.min.css
+-rw-r--r--   0        0        0     4331 2020-11-03 21:09:40.510944 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/css/launcher.css
+-rw-r--r--   0        0        0     2765 2021-01-29 15:59:17.153310 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/css/launcher.min.css
+-rw-r--r--   0        0        0     1363 2021-02-16 17:03:36.468870 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/css/memberaudit.css
+-rw-r--r--   0        0        0      617 2021-02-16 17:03:36.468870 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/css/memberaudit.min.css
+-rw-r--r--   0        0        0      611 2021-02-17 10:40:00.762093 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/css/reports.css
+-rw-r--r--   0        0        0    43262 2020-10-26 16:42:17.713201 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/images/Spinner-1s-64px-dark.gif
+-rw-r--r--   0        0        0    43381 2020-10-26 16:42:17.713201 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/images/Spinner-1s-64px-light.gif
+-rw-r--r--   0        0        0     1862 2021-02-23 10:36:55.530247 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/images/charisma.png
+-rw-r--r--   0        0        0      694 2020-11-03 21:09:40.510944 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/images/eve-prism.png
+-rw-r--r--   0        0        0      220 2020-11-03 21:09:40.510944 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/images/evelogo.png
+-rw-r--r--   0        0        0      595 2020-11-03 21:09:40.510944 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/images/evesearch.png
+-rw-r--r--   0        0        0     1966 2021-02-23 10:36:55.530247 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/images/intelligence.png
+-rw-r--r--   0        0        0     1809 2021-02-23 10:36:55.530247 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/images/memory.png
+-rw-r--r--   0        0        0     1803 2021-02-23 10:36:55.530247 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/images/perception.png
+-rw-r--r--   0        0        0     1782 2021-02-23 10:36:55.530247 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/images/willpower.png
+-rw-r--r--   0        0        0      259 2020-10-22 17:18:29.995572 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/images/zkillboard.png
+-rw-r--r--   0        0        0     5573 2020-10-22 17:18:29.995572 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/vendor/datatables/plugins/dataTables.rowGroup.min.js
+-rw-r--r--   0        0        0     3908 2022-04-01 19:33:31.239451 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/vendor/datatables/plugins/datetime.js
+-rw-r--r--   0        0        0     2529 2022-04-01 19:48:30.310949 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/vendor/datatables/plugins/filterDropDown.min.js
+-rw-r--r--   0        0        0      384 2020-10-22 17:18:29.995572 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/vendor/datatables/plugins/rowGroup.bootstrap.min.css
+-rw-r--r--   0        0        0      384 2020-10-22 17:18:29.995572 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/vendor/datatables/plugins/rowGroup.dataTables.min.css
+-rw-r--r--   0        0        0    69950 2020-10-28 14:46:25.711812 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/vendor/moment/moment.min.js
+-rw-r--r--   0        0        0   881821 2023-02-16 19:01:05.384001 aa_memberaudit-2.9.1/memberaudit/swagger.json
+-rw-r--r--   0        0        0    40513 2023-06-20 12:20:45.247100 aa_memberaudit-2.9.1/memberaudit/tasks.py
+-rw-r--r--   0        0        0      687 2023-04-16 16:03:49.365835 aa_memberaudit-2.9.1/memberaudit/templates/admin/memberaudit/character/confirm_character_deletion.html
+-rw-r--r--   0        0        0      488 2022-09-02 18:40:08.749489 aa_memberaudit-2.9.1/memberaudit/templates/admin/memberaudit/skillset/change_list.html
+-rw-r--r--   0        0        0      848 2023-04-16 16:03:49.365835 aa_memberaudit-2.9.1/memberaudit/templates/admin/memberaudit/skillset/import_skills.html
+-rw-r--r--   0        0        0      367 2020-12-07 00:53:01.652277 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/base.html
+-rw-r--r--   0        0        0     4801 2023-04-25 19:10:30.720306 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/character_finder.html
+-rw-r--r--   0        0        0    29413 2023-06-16 09:54:37.528799 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/character_viewer.html
+-rw-r--r--   0        0        0     2932 2023-04-25 19:10:30.720306 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/data_export.html
+-rw-r--r--   0        0        0     8515 2023-04-16 16:03:49.365835 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/launcher.html
+-rw-r--r--   0        0        0     1238 2021-01-29 15:52:00.995855 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/modals/character_viewer/asset_container.html
+-rw-r--r--   0        0        0     4307 2022-04-01 19:33:31.243451 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/modals/character_viewer/asset_container_content.html
+-rw-r--r--   0        0        0     1713 2021-02-18 07:41:27.336226 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/modals/character_viewer/character_skill_set_details.html
+-rw-r--r--   0        0        0     1246 2020-11-01 21:48:51.676098 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/modals/character_viewer/contract.html
+-rw-r--r--   0        0        0     8075 2023-04-16 16:03:49.365835 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/modals/character_viewer/contract_content.html
+-rw-r--r--   0        0        0      658 2023-04-16 16:03:49.365835 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/modals/character_viewer/contract_items.html
+-rw-r--r--   0        0        0     1375 2022-02-09 21:55:36.827364 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/modals/character_viewer/mail.html
+-rw-r--r--   0        0        0      382 2023-04-16 16:03:49.369835 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/modals/character_viewer/mail_content.html
+-rw-r--r--   0        0        0     3880 2022-04-01 19:33:31.243451 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/modals/character_viewer/skill_set_content.html
+-rw-r--r--   0        0        0     9005 2023-06-15 11:31:30.596583 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/overview.html
+-rw-r--r--   0        0        0     1451 2023-04-16 16:03:49.369835 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/sidebar.html
+-rw-r--r--   0        0        0      637 2023-06-15 19:47:27.834479 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/sidebar_character.html
+-rw-r--r--   0        0        0     1256 2023-06-15 19:47:27.834479 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/assets.html
+-rw-r--r--   0        0        0      560 2023-06-15 19:47:27.834479 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes.html
+-rw-r--r--   0        0        0     2604 2021-02-23 15:40:36.322996 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes_content.html
+-rw-r--r--   0        0        0      314 2023-06-15 19:47:27.834479 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_bio.html
+-rw-r--r--   0        0        0      848 2023-06-15 19:47:27.834479 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contacts.html
+-rw-r--r--   0        0        0      960 2023-06-15 19:47:27.834479 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contracts.html
+-rw-r--r--   0        0        0      582 2023-06-15 19:47:27.834479 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history.html
+-rw-r--r--   0        0        0      894 2020-12-14 23:31:49.226782 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html
+-rw-r--r--   0        0        0      549 2023-06-15 19:47:27.834479 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats.html
+-rw-r--r--   0        0        0     2786 2023-04-16 16:03:49.373835 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats_content.html
+-rw-r--r--   0        0        0      563 2023-06-15 19:47:27.834479 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/implants.html
+-rw-r--r--   0        0        0      721 2023-06-15 19:47:27.838479 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/jump_clones.html
+-rw-r--r--   0        0        0      148 2020-11-09 19:29:14.885373 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/last_updated.html
+-rw-r--r--   0        0        0      611 2023-06-15 19:47:27.838479 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/loyalty.html
+-rw-r--r--   0        0        0     2878 2023-06-15 19:47:27.838479 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mails.html
+-rw-r--r--   0        0        0      779 2023-06-15 19:47:27.838479 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mining_ledger.html
+-rw-r--r--   0        0        0      885 2023-06-16 09:54:37.528799 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/planets.html
+-rw-r--r--   0        0        0      669 2023-06-15 19:47:27.838479 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_queue.html
+-rw-r--r--   0        0        0      882 2023-06-15 19:47:27.838479 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_sets.html
+-rw-r--r--   0        0        0      592 2023-06-15 19:47:27.838479 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skills.html
+-rw-r--r--   0        0        0      907 2023-06-15 19:47:27.838479 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_journal.html
+-rw-r--r--   0        0        0      916 2023-06-15 19:47:27.838479 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_transactions.html
+-rw-r--r--   0        0        0     3941 2023-06-15 19:47:27.838479 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs_navigation.html
+-rw-r--r--   0        0        0     2674 2022-01-23 15:08:18.156059 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/menu.html
+-rw-r--r--   0        0        0      292 2023-04-16 16:03:49.373835 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/reports/tabs/_compliance_color_code.html
+-rw-r--r--   0        0        0      684 2023-04-16 16:03:49.373835 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/reports/tabs/corporation_compliance.html
+-rw-r--r--   0        0        0      760 2023-04-16 16:03:49.377835 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/reports/tabs/skill_sets.html
+-rw-r--r--   0        0        0      775 2023-04-16 16:03:49.377835 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/reports/tabs/user_compliance.html
+-rw-r--r--   0        0        0      691 2021-02-16 15:13:05.236586 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/reports/tabs_navigation.html
+-rw-r--r--   0        0        0      709 2023-04-16 16:03:49.377835 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/solar_system.html
+-rw-r--r--   0        0        0     9420 2022-04-01 19:56:47.910687 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/reports.html
+-rw-r--r--   0        0        0        0 2023-06-21 11:55:38.018082 aa_memberaudit-2.9.1/memberaudit/templatetags/__init__.py
+-rw-r--r--   0        0        0      355 2023-06-18 16:38:29.688085 aa_memberaudit-2.9.1/memberaudit/templatetags/memberaudit.py
+-rw-r--r--   0        0        0        0 2023-06-21 11:55:38.018082 aa_memberaudit-2.9.1/memberaudit/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-21 11:55:38.018082 aa_memberaudit-2.9.1/memberaudit/tests/core/__init__.py
+-rw-r--r--   0        0        0     6350 2023-06-16 09:54:37.532799 aa_memberaudit-2.9.1/memberaudit/tests/core/test_core_xml_converter.py
+-rw-r--r--   0        0        0    12725 2023-06-18 19:47:02.526598 aa_memberaudit-2.9.1/memberaudit/tests/core/test_data_exporters.py
+-rw-r--r--   0        0        0    22366 2023-06-16 09:54:37.532799 aa_memberaudit-2.9.1/memberaudit/tests/core/test_eft_parser.py
+-rw-r--r--   0        0        0     6371 2023-06-16 09:54:37.536799 aa_memberaudit-2.9.1/memberaudit/tests/core/test_fittings.py
+-rw-r--r--   0        0        0     4082 2022-09-03 21:36:22.049912 aa_memberaudit-2.9.1/memberaudit/tests/core/test_skill_plans.py
+-rw-r--r--   0        0        0     2458 2023-06-16 09:54:37.536799 aa_memberaudit-2.9.1/memberaudit/tests/core/test_skills.py
+-rw-r--r--   0        0        0        0 2023-06-21 11:55:38.018082 aa_memberaudit-2.9.1/memberaudit/tests/managers/__init__.py
+-rw-r--r--   0        0        0    18357 2023-02-24 14:11:29.027672 aa_memberaudit-2.9.1/memberaudit/tests/managers/test_character.py
+-rw-r--r--   0        0        0    30687 2023-06-20 12:20:45.247100 aa_memberaudit-2.9.1/memberaudit/tests/managers/test_character_sections_1.py
+-rw-r--r--   0        0        0    37493 2023-06-19 14:17:29.534236 aa_memberaudit-2.9.1/memberaudit/tests/managers/test_character_sections_2.py
+-rw-r--r--   0        0        0    24751 2023-06-19 16:16:36.742579 aa_memberaudit-2.9.1/memberaudit/tests/managers/test_character_sections_3.py
+-rw-r--r--   0        0        0    46675 2023-06-17 19:32:02.157925 aa_memberaudit-2.9.1/memberaudit/tests/managers/test_general.py
+-rw-r--r--   0        0        0        0 2023-06-21 11:55:38.018082 aa_memberaudit-2.9.1/memberaudit/tests/models/__init__.py
+-rw-r--r--   0        0        0     2963 2023-06-18 15:15:28.271801 aa_memberaudit-2.9.1/memberaudit/tests/models/test_character_sections.py
+-rw-r--r--   0        0        0    36073 2023-06-18 15:15:28.271801 aa_memberaudit-2.9.1/memberaudit/tests/models/test_characters_1.py
+-rw-r--r--   0        0        0    23158 2023-06-20 12:20:45.247100 aa_memberaudit-2.9.1/memberaudit/tests/models/test_characters_2.py
+-rw-r--r--   0        0        0    10969 2023-06-16 19:39:55.468632 aa_memberaudit-2.9.1/memberaudit/tests/models/test_general.py
+-rw-r--r--   0        0        0    15428 2023-06-15 13:23:00.558207 aa_memberaudit-2.9.1/memberaudit/tests/test_admin.py
+-rw-r--r--   0        0        0     1807 2023-02-24 17:52:57.675286 aa_memberaudit-2.9.1/memberaudit/tests/test_auth_hooks.py
+-rw-r--r--   0        0        0     1314 2023-03-22 16:51:39.514903 aa_memberaudit-2.9.1/memberaudit/tests/test_checks.py
+-rw-r--r--   0        0        0     3487 2023-06-16 09:54:37.540799 aa_memberaudit-2.9.1/memberaudit/tests/test_commands.py
+-rw-r--r--   0        0        0     4119 2023-06-17 19:32:02.161924 aa_memberaudit-2.9.1/memberaudit/tests/test_decorators.py
+-rw-r--r--   0        0        0      900 2023-06-16 09:54:37.540799 aa_memberaudit-2.9.1/memberaudit/tests/test_factories.py
+-rw-r--r--   0        0        0     3516 2022-09-03 16:21:19.096009 aa_memberaudit-2.9.1/memberaudit/tests/test_forms.py
+-rw-r--r--   0        0        0     1476 2023-06-18 19:20:57.381084 aa_memberaudit-2.9.1/memberaudit/tests/test_helpers.py
+-rw-r--r--   0        0        0    15643 2023-06-18 13:31:57.369928 aa_memberaudit-2.9.1/memberaudit/tests/test_integration.py
+-rw-r--r--   0        0        0     1215 2022-03-05 14:47:06.220060 aa_memberaudit-2.9.1/memberaudit/tests/test_signals.py
+-rw-r--r--   0        0        0    38340 2023-06-19 16:16:36.742579 aa_memberaudit-2.9.1/memberaudit/tests/test_tasks.py
+-rw-r--r--   0        0        0      968 2023-06-16 09:54:37.544799 aa_memberaudit-2.9.1/memberaudit/tests/test_templatetags.py
+-rw-r--r--   0        0        0     3822 2023-06-16 19:39:55.468632 aa_memberaudit-2.9.1/memberaudit/tests/test_utils.py
+-rw-r--r--   0        0        0      267 2020-10-22 17:18:30.011572 aa_memberaudit-2.9.1/memberaudit/tests/testdata/__init__.py
+-rw-r--r--   0        0        0     4432 2023-06-18 16:38:29.692085 aa_memberaudit-2.9.1/memberaudit/tests/testdata/create_eveuniverse.py
+-rw-r--r--   0        0        0     4350 2022-02-10 22:57:31.960297 aa_memberaudit-2.9.1/memberaudit/tests/testdata/entities.json
+-rw-r--r--   0        0        0     5298 2023-06-19 21:45:47.103045 aa_memberaudit-2.9.1/memberaudit/tests/testdata/esi_client_stub.py
+-rw-r--r--   0        0        0    41017 2023-06-15 19:47:27.842479 aa_memberaudit-2.9.1/memberaudit/tests/testdata/esi_testdata.json
+-rw-r--r--   0        0        0  1225856 2023-06-15 19:47:27.862479 aa_memberaudit-2.9.1/memberaudit/tests/testdata/eveuniverse.json
+-rw-r--r--   0        0        0    13508 2023-06-18 16:38:29.692085 aa_memberaudit-2.9.1/memberaudit/tests/testdata/factories.py
+-rw-r--r--   0        0        0      799 2022-04-01 19:33:31.251451 aa_memberaudit-2.9.1/memberaudit/tests/testdata/fittings/fitting_archon.txt
+-rw-r--r--   0        0        0      889 2022-04-01 19:33:31.251451 aa_memberaudit-2.9.1/memberaudit/tests/testdata/fittings/fitting_archon_max.txt
+-rw-r--r--   0        0        0      231 2022-04-01 19:33:31.251451 aa_memberaudit-2.9.1/memberaudit/tests/testdata/fittings/fitting_empty.txt
+-rw-r--r--   0        0        0      503 2022-04-01 19:33:31.251451 aa_memberaudit-2.9.1/memberaudit/tests/testdata/fittings/fitting_eve_celestis_no_high_slots.txt
+-rw-r--r--   0        0        0      193 2022-04-01 19:33:31.251451 aa_memberaudit-2.9.1/memberaudit/tests/testdata/fittings/fitting_eve_tristan_3.txt
+-rw-r--r--   0        0        0      377 2022-04-01 19:33:31.251451 aa_memberaudit-2.9.1/memberaudit/tests/testdata/fittings/fitting_eve_tristian.txt
+-rw-r--r--   0        0        0      293 2022-04-01 19:33:31.251451 aa_memberaudit-2.9.1/memberaudit/tests/testdata/fittings/fitting_eve_tristian_2.txt
+-rw-r--r--   0        0        0       96 2022-04-01 19:33:31.251451 aa_memberaudit-2.9.1/memberaudit/tests/testdata/fittings/fitting_eve_tristian_empty.txt
+-rw-r--r--   0        0        0      583 2022-04-01 19:33:31.251451 aa_memberaudit-2.9.1/memberaudit/tests/testdata/fittings/fitting_svipul.txt
+-rw-r--r--   0        0        0      432 2022-04-01 19:33:31.251451 aa_memberaudit-2.9.1/memberaudit/tests/testdata/fittings/fitting_svipul_2.txt
+-rw-r--r--   0        0        0      700 2022-04-01 19:33:31.251451 aa_memberaudit-2.9.1/memberaudit/tests/testdata/fittings/fitting_tengu.txt
+-rw-r--r--   0        0        0      459 2022-04-01 19:33:31.251451 aa_memberaudit-2.9.1/memberaudit/tests/testdata/fittings/fitting_tristan.txt
+-rw-r--r--   0        0        0      332 2022-04-01 19:33:31.251451 aa_memberaudit-2.9.1/memberaudit/tests/testdata/fittings/fitting_tristan_missing_rigs.txt
+-rw-r--r--   0        0        0      410 2022-04-01 19:33:31.251451 aa_memberaudit-2.9.1/memberaudit/tests/testdata/fittings/fitting_tristan_no_title.txt
+-rw-r--r--   0        0        0      460 2022-04-01 19:33:31.251451 aa_memberaudit-2.9.1/memberaudit/tests/testdata/fittings/fitting_tristan_unknown_types.txt
+-rw-r--r--   0        0        0      455 2023-05-08 11:52:50.156096 aa_memberaudit-2.9.1/memberaudit/tests/testdata/fittings/fitting_unknown_ship_type.txt
+-rw-r--r--   0        0        0     4268 2023-06-18 16:38:29.692085 aa_memberaudit-2.9.1/memberaudit/tests/testdata/generate_character.py
+-rw-r--r--   0        0        0     3859 2022-01-20 23:34:01.558036 aa_memberaudit-2.9.1/memberaudit/tests/testdata/generate_doctrines.py
+-rw-r--r--   0        0        0     3680 2023-06-18 16:38:29.692085 aa_memberaudit-2.9.1/memberaudit/tests/testdata/load_entities.py
+-rw-r--r--   0        0        0      478 2023-06-18 16:38:29.692085 aa_memberaudit-2.9.1/memberaudit/tests/testdata/load_eveuniverse.py
+-rw-r--r--   0        0        0     1188 2022-02-10 21:29:55.833941 aa_memberaudit-2.9.1/memberaudit/tests/testdata/load_locations.py
+-rw-r--r--   0        0        0     1097 2022-04-01 19:33:31.251451 aa_memberaudit-2.9.1/memberaudit/tests/testdata/pilot_esi_error_handling.py
+-rw-r--r--   0        0        0      838 2023-06-18 16:38:29.696085 aa_memberaudit-2.9.1/memberaudit/tests/testdata/profiler_toolbox.py
+-rw-r--r--   0        0        0     5744 2023-06-20 12:20:45.251100 aa_memberaudit-2.9.1/memberaudit/tests/utils.py
+-rw-r--r--   0        0        0        0 2023-06-21 11:55:38.022082 aa_memberaudit-2.9.1/memberaudit/tests/views/__init__.py
+-rw-r--r--   0        0        0     9299 2023-06-15 13:23:00.562207 aa_memberaudit-2.9.1/memberaudit/tests/views/test_admin.py
+-rw-r--r--   0        0        0     7089 2023-06-16 09:54:37.544799 aa_memberaudit-2.9.1/memberaudit/tests/views/test_character_finder.py
+-rw-r--r--   0        0        0    32680 2023-03-22 21:45:48.968406 aa_memberaudit-2.9.1/memberaudit/tests/views/test_character_viewer_1.py
+-rw-r--r--   0        0        0    24561 2023-06-15 19:47:27.866479 aa_memberaudit-2.9.1/memberaudit/tests/views/test_character_viewer_2.py
+-rw-r--r--   0        0        0    14594 2023-06-16 09:54:37.544799 aa_memberaudit-2.9.1/memberaudit/tests/views/test_characters.py
+-rw-r--r--   0        0        0     4101 2023-06-16 09:54:37.544799 aa_memberaudit-2.9.1/memberaudit/tests/views/test_data_export.py
+-rw-r--r--   0        0        0    16249 2023-06-16 09:54:37.544799 aa_memberaudit-2.9.1/memberaudit/tests/views/test_reports.py
+-rw-r--r--   0        0        0      710 2023-06-16 19:39:55.468632 aa_memberaudit-2.9.1/memberaudit/tools/clear_celery_once_locks.py
+-rw-r--r--   0        0        0     3051 2022-10-21 18:07:26.108963 aa_memberaudit-2.9.1/memberaudit/tools/drop_tables.sql
+-rw-r--r--   0        0        0      329 2020-12-16 22:00:54.319925 aa_memberaudit-2.9.1/memberaudit/tools/total_size.sql
+-rw-r--r--   0        0        0     7242 2023-06-18 14:40:14.297539 aa_memberaudit-2.9.1/memberaudit/urls.py
+-rw-r--r--   0        0        0     2367 2023-06-18 16:38:29.696085 aa_memberaudit-2.9.1/memberaudit/utils.py
+-rw-r--r--   0        0        0        0 2023-06-21 11:55:38.022082 aa_memberaudit-2.9.1/memberaudit/views/__init__.py
+-rw-r--r--   0        0        0     1539 2023-06-18 14:40:14.297539 aa_memberaudit-2.9.1/memberaudit/views/_common.py
+-rw-r--r--   0        0        0     3510 2023-06-18 14:40:14.297539 aa_memberaudit-2.9.1/memberaudit/views/admin.py
+-rw-r--r--   0        0        0    12637 2023-06-18 16:38:29.696085 aa_memberaudit-2.9.1/memberaudit/views/character_finder.py
+-rw-r--r--   0        0        0    24043 2023-06-18 19:20:57.385084 aa_memberaudit-2.9.1/memberaudit/views/character_viewer_1.py
+-rw-r--r--   0        0        0    24241 2023-06-20 12:20:45.251100 aa_memberaudit-2.9.1/memberaudit/views/character_viewer_2.py
+-rw-r--r--   0        0        0     8029 2023-06-18 16:38:29.700085 aa_memberaudit-2.9.1/memberaudit/views/characters.py
+-rw-r--r--   0        0        0     2222 2023-06-18 14:40:14.301539 aa_memberaudit-2.9.1/memberaudit/views/data_export.py
+-rw-r--r--   0        0        0    13139 2023-06-20 12:20:45.251100 aa_memberaudit-2.9.1/memberaudit/views/reports.py
+-rw-r--r--   0        0        0     2278 2023-06-19 21:45:47.107045 aa_memberaudit-2.9.1/pyproject.toml
+-rw-r--r--   0        0        0     7367 1970-01-01 00:00:00.000000 aa_memberaudit-2.9.1/PKG-INFO
```

### Comparing `aa_memberaudit-2.9.0/LICENSE` & `aa_memberaudit-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/README.md` & `aa_memberaudit-2.9.1/README.md`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/admin.py` & `aa_memberaudit-2.9.1/memberaudit/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Define admin site for Member Audit."""
+
 from typing import List, Optional
 
 from django import forms
 from django.contrib import admin
 from django.contrib.auth.models import Group
 from django.core.exceptions import ValidationError
 from django.db.models import Max, Prefetch
@@ -139,18 +141,18 @@
 
     def lookups(self, request, model_admin):
         qs = model_admin.get_queryset(request)
         counts = []
         for status in Character.UpdateStatus:
             counts.append((status, qs.filter(update_status=status.value).count()))
         result = tuple(
-            [
+            (
                 (status.value, status.label.title() + f" ({count:,})")
                 for status, count in counts
-            ]
+            )
         )
         return result
 
     def queryset(self, request, queryset):
         for value in Character.UpdateStatus.values:
             if self.value() == value:
                 return queryset.filter(update_status=value)
@@ -337,15 +339,15 @@
         return obj.created_at
 
     @admin.display(ordering="last_update_at", description=_("last update"))
     def _last_update_at(self, obj: Character):
         return obj.last_update_at
 
     def _missing_sections(self, obj):
-        existing = {x.section for x in obj.update_status_set.all()}
+        existing = {status.section for status in obj.update_status_set.all()}
         all_sections = set(Character.UpdateSection.values)
         missing = all_sections.difference(existing)
         if missing:
             return sorted(
                 [Character.UpdateSection.display_name(obj) for obj in missing]
             )
         return None
@@ -539,15 +541,17 @@
                 "skill_sets",
                 queryset=SkillSet.objects.order_by("name"),
                 to_attr="skill_sets_ordered",
             )
         )
 
     def _skill_sets(self, obj):
-        return format_html("<br>".join([x.name for x in obj.skill_sets_ordered]))
+        return format_html(
+            "<br>".join([skill_set.name for skill_set in obj.skill_sets_ordered])
+        )
 
     def save_model(self, request, obj, form, change):
         obj.last_modified_by = request.user
         obj.last_modified_at = now()
         super().save_model(request, obj, form, change)
```

### Comparing `aa_memberaudit-2.9.0/memberaudit/app_settings.py` & `aa_memberaudit-2.9.1/memberaudit/app_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+"""Definition and parsing of Member Audit's settings."""
+
 from django.utils.translation import gettext_lazy as _
 
-from app_utils.django import clean_setting
+from app_utils.app_settings import clean_setting
 
-from memberaudit.helpers import get_unidecoded_slug
+from memberaudit.utils import get_unidecoded_slug
 
 MEMBERAUDIT_APP_NAME = clean_setting(
     "MEMBERAUDIT_APP_NAME", _("Member Audit"), required_type=str
 )
 """Name of this app as shown in the Auth sidebar and page titles."""
 
 MEMBERAUDIT_BASE_URL = get_unidecoded_slug(MEMBERAUDIT_APP_NAME)
```

### Comparing `aa_memberaudit-2.9.0/memberaudit/auth_hooks.py` & `aa_memberaudit-2.9.1/memberaudit/auth_hooks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
+"""Define hooks for Alliance Auth like the sidebar menu entry."""
+
 from allianceauth import hooks
 from allianceauth.services.hooks import MenuItemHook, UrlHook
 
 from . import urls
 from .app_settings import MEMBERAUDIT_APP_NAME, MEMBERAUDIT_BASE_URL
 from .models import Character
 
 
 class MemberauditMenuItem(MenuItemHook):
     """This class ensures only authorized users will see the menu entry"""
 
     def __init__(self):
-        # setup menu entry for sidebar
         MenuItemHook.__init__(
             self,
             MEMBERAUDIT_APP_NAME,
             "far fa-address-card fa-fw fa-fw",
             "memberaudit:index",
             navactive=["memberaudit:"],
         )
```

### Comparing `aa_memberaudit-2.9.0/memberaudit/checks.py` & `aa_memberaudit-2.9.1/memberaudit/checks.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Django system checks."""
+
 from django.core.checks import Critical, Tags, register
 
 
 @register(Tags.database)
 def upgrade_from_1_x_check(app_configs, **kwargs):
     """Ensure users are upgrading to 2.0 first, when coming from 1.x"""
     from packaging.version import Version
```

### Comparing `aa_memberaudit-2.9.0/memberaudit/core/data_exporters.py` & `aa_memberaudit-2.9.1/memberaudit/core/data_exporters.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from pathlib import Path
 from typing import List
 
 from pytz import utc
 
 from django.conf import settings
 from django.db import models
-from django.utils.functional import classproperty
 from django.utils.timezone import now
 
 from allianceauth.services.hooks import get_extension_logger
 from app_utils.logging import LoggerAddTag
 from app_utils.views import yesno_str
 
 from memberaudit import __title__
@@ -78,31 +77,30 @@
 
 
 def _gather_export_files(destination_folder: str) -> dict:
     if not destination_folder:
         destination_path = default_destination()
     else:
         destination_path = Path(destination_folder)
-    files = [file for file in destination_path.glob(f"{_app_name()}_*.zip")]
-    export_files = dict()
+    files = list(destination_path.glob(f"{_app_name()}_*.zip"))
+    export_files = {}
     if files:
         for file in files:
             parts = file.with_suffix("").name.split("_")
             export_files[parts[1]] = file
     return export_files
 
 
 def _compile_topics(export_files):
     topics = []
-    for topic in DataExporter.topics:
+    for topic in DataExporter.topics():
         export_file = export_files[topic] if topic in export_files.keys() else None
         if export_file:
             timestamp = export_file.stat().st_mtime
             last_updated_at = dt.datetime.fromtimestamp(timestamp, tz=utc)
-            MEMBERAUDIT_DATA_EXPORT_MIN_UPDATE_AGE
             update_allowed = settings.DEBUG or (
                 now() - last_updated_at
             ).total_seconds() > (MEMBERAUDIT_DATA_EXPORT_MIN_UPDATE_AGE * 60)
         else:
             last_updated_at = None
             update_allowed = True
         exporter = DataExporter.create_exporter(topic)
@@ -150,15 +148,15 @@
 
     @abstractmethod
     def get_queryset(self) -> models.QuerySet:
         """Return queryset to fetch the data for this exporter."""
         raise NotImplementedError()
 
     @abstractmethod
-    def format_obj(self, obj: models.Model) -> dict:
+    def format_obj(self, obj) -> dict:
         """Format object into row for output."""
         raise NotImplementedError()
 
     def has_data(self) -> bool:
         return self.queryset.exists()
 
     def count(self) -> bool:
@@ -181,32 +179,32 @@
             writer.writeheader()
             chunk_size = 1000
             for obj in self.queryset.iterator(chunk_size=chunk_size):
                 row = self.format_obj(obj)
                 writer.writerow(row)
         return output_file
 
-    @classproperty
+    @classmethod
     def _exporters(cls) -> list:
         """Supported exporter classes."""
         return [ContractExporter, ContractItemExporter, WalletJournalExporter]
 
-    @classproperty
+    @classmethod
     def topics(cls) -> list:
         """Available export topics."""
-        return sorted([exporter.topic for exporter in cls._exporters])
+        return sorted([exporter.topic for exporter in cls._exporters()])
 
     @classmethod
     def create_exporter(cls, topic: str) -> "DataExporter":
         """Create an exporter for the requested topic.
 
         Raises:
         - ValueError for invalid topics
         """
-        for exporter in cls._exporters:
+        for exporter in cls._exporters():
             if topic == exporter.topic:
                 return exporter()
         raise ValueError(f"Invalid topic: {topic}")
 
 
 class ContractExporter(DataExporter):
     topic = "contract"
@@ -220,15 +218,15 @@
             "end_location",
             "issuer_corporation",
             "issuer",
             "start_location",
             "character",
         ).order_by("date_issued")
 
-    def format_obj(self, obj: models.Model) -> dict:
+    def format_obj(self, obj) -> dict:
         return {
             "owner character": obj.character.eve_character.character_name,
             "owner corporation": obj.character.eve_character.corporation_name,
             "contract pk": obj.pk,
             "contract id": obj.contract_id,
             "contract_type": obj.get_contract_type_display(),
             "status": obj.get_status_display(),
@@ -260,15 +258,15 @@
     )
 
     def get_queryset(self) -> models.QuerySet:
         return CharacterContractItem.objects.select_related(
             "contract", "eve_type"
         ).order_by("contract", "record_id")
 
-    def format_obj(self, obj: models.Model) -> dict:
+    def format_obj(self, obj) -> dict:
         return {
             "contract pk": obj.contract.pk,
             "record id": obj.record_id,
             "type": obj.eve_type.name,
             "quantity": obj.quantity,
             "is included": yesno_str(obj.is_included),
             "is singleton": yesno_str(obj.is_blueprint),
@@ -284,17 +282,17 @@
     description = "List of wallet journal entries."
 
     def get_queryset(self) -> models.QuerySet:
         return CharacterWalletJournalEntry.objects.select_related(
             "first_party", "second_party", "character"
         ).order_by("date")
 
-    def format_obj(self, obj: models.Model) -> dict:
+    def format_obj(self, obj) -> dict:
         if not obj:
-            return dict()
+            return {}
         return {
             "date": obj.date.strftime("%Y-%m-%d %H:%M:%S"),
             "owner character": obj.character.eve_character.character_name,
             "owner corporation": obj.character.eve_character.corporation_name,
             "entry id": obj.entry_id,
             "ref type": obj.ref_type.replace("_", " ").title(),
             "first party": _name_or_default(obj.first_party),
```

### Comparing `aa_memberaudit-2.9.0/memberaudit/core/eft_parser.py` & `aa_memberaudit-2.9.1/memberaudit/core/eft_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Parser for fitting in EFT Format"""
+
 from dataclasses import dataclass, field
 from enum import Enum, auto
 from typing import Any, Dict, Iterable, List, Optional, Set, Tuple
 
 from bravado.exception import HTTPNotFound
 
 from eveuniverse.models import EveEntity, EveType
@@ -111,15 +112,15 @@
                 "EFT parser: failed to identify types: %s",
                 type_names_str(missing_type_names_2),
             )
         return eve_types, missing_type_names_2
 
     @staticmethod
     def _fetch_types_from_esi(entity_ids) -> Dict[str, EveType]:
-        eve_types = dict()
+        eve_types = {}
         for entity_id in entity_ids:
             try:
                 obj, _ = EveType.objects.get_or_create_esi(
                     id=entity_id, enabled_sections=[EveType.Section.DOGMAS]
                 )
             except HTTPNotFound:
                 pass
@@ -164,14 +165,15 @@
     item_type: Optional[str] = None
     charge_type: Optional[str] = None
     quantity: Optional[int] = None
     is_offline: bool = False
     slot_type: _EftSlotType = _EftSlotType.NONE
 
     def type_names(self) -> Set[str]:
+        """Return types used in the item."""
         types = set()
         if self.item_type:
             types.add(self.item_type)
         if self.charge_type:
             types.add(self.charge_type)
         return types
 
@@ -213,21 +215,23 @@
 @dataclass
 class _EftTextSection:
     """Text section of an EFT fitting used for parsing."""
 
     items: List[_EftTextItem] = field(default_factory=list)
 
     def type_names(self) -> Set[str]:
+        """Return types used in the section."""
         types = set()
         for item in self.items:
             types |= item.type_names()
         return types
 
     @classmethod
-    def create_from_lines(cls, lines):
+    def create_from_lines(cls, lines: Iterable[str]) -> "_EftTextSection":
+        """Create new object from lines."""
         items = [_EftTextItem.create_from_line(line) for line in lines]
         return cls(items=items)
 
 
 @dataclass
 class _EftItem:
     """Item of an EFT fitting used for parsing."""
@@ -265,56 +269,66 @@
         if self.is_empty:
             return False
         return self._item_category_id() == EveCategoryId.FIGHTER
 
     def is_high_slot(self) -> bool:
         if self.slot_type is _EftSlotType.HIGH_SLOT:
             return True
-        elif self.is_empty:
+
+        if self.is_empty:
             return False
+
         effect_ids = {
             obj.eve_dogma_effect_id for obj in self.item_type.dogma_effects.all()
         }
         return EveDogmaEffectId.HI_POWER in effect_ids
 
     def is_med_slot(self) -> bool:
         if self.slot_type is _EftSlotType.MEDIUM_SLOT:
             return True
-        elif self.is_empty:
+
+        if self.is_empty:
             return False
+
         effect_ids = {
             obj.eve_dogma_effect_id for obj in self.item_type.dogma_effects.all()
         }
         return EveDogmaEffectId.MED_POWER in effect_ids
 
     def is_low_slot(self) -> bool:
         if self.slot_type is _EftSlotType.LOW_SLOT:
             return True
-        elif self.is_empty:
+
+        if self.is_empty:
             return False
+
         effect_ids = {
             obj.eve_dogma_effect_id for obj in self.item_type.dogma_effects.all()
         }
         return EveDogmaEffectId.LO_POWER in effect_ids
 
     def is_rig_slot(self) -> bool:
         if self.slot_type is _EftSlotType.RIG_SLOT:
             return True
-        elif self.is_empty:
+
+        if self.is_empty:
             return False
+
         effect_ids = {
             obj.eve_dogma_effect_id for obj in self.item_type.dogma_effects.all()
         }
         return EveDogmaEffectId.RIG_SLOT in effect_ids
 
     def is_subsystem(self) -> bool:
         if self.slot_type is _EftSlotType.SUBSYSTEM_SLOT:
             return True
-        elif self.is_empty:
+
+        if self.is_empty:
             return False
+
         effect_ids = {
             obj.eve_dogma_effect_id for obj in self.item_type.dogma_effects.all()
         }
         return EveDogmaEffectId.SUB_SYSTEM in effect_ids
 
     def _item_category_id(self) -> Optional[int]:
         if self.is_empty:
@@ -366,39 +380,39 @@
             }
 
     items: List[_EftItem] = field(default_factory=list)
     category: Category = Category.UNKNOWN
 
     @property
     def is_slots(self) -> bool:
-        return any([item.is_slot for item in self.items])
+        return any((item.is_slot for item in self.items))
 
     def guess_category(self) -> Optional["_EftSection.Category"]:
         """Try to guess the category of this section based on it's items.
         Returns ``None`` if the guess fails.
         """
         if self.is_slots:
-            if any([item.is_booster() for item in self.items]):
+            if any((item.is_booster() for item in self.items)):
                 return self.Category.BOOSTERS
-            if any([item.is_cyber_implant() for item in self.items]):
+            if any((item.is_cyber_implant() for item in self.items)):
                 return self.Category.IMPLANTS
-            if any([item.is_low_slot() for item in self.items]):
+            if any((item.is_low_slot() for item in self.items)):
                 return self.Category.LOW_SLOTS
-            if any([item.is_med_slot() for item in self.items]):
+            if any((item.is_med_slot() for item in self.items)):
                 return self.Category.MEDIUM_SLOTS
-            if any([item.is_high_slot() for item in self.items]):
+            if any((item.is_high_slot() for item in self.items)):
                 return self.Category.HIGH_SLOTS
-            if any([item.is_rig_slot() for item in self.items]):
+            if any((item.is_rig_slot() for item in self.items)):
                 return self.Category.RIG_SLOTS
-            if any([item.is_subsystem() for item in self.items]):
+            if any((item.is_subsystem() for item in self.items)):
                 return self.Category.SUBSYSTEM_SLOTS
         else:
-            if any([item.is_drone() for item in self.items]):
+            if any((item.is_drone() for item in self.items)):
                 return self.Category.DRONES_BAY
-            if any([item.is_fighter() for item in self.items]):
+            if any((item.is_fighter() for item in self.items)):
                 return self.Category.FIGHTER_BAY
         return None
 
     def to_modules(self) -> List[Module]:
         """Convert eft items into fitting modules.
 
         Types from modules that can not be resolved will result in an empty slot.
```

### Comparing `aa_memberaudit-2.9.0/memberaudit/core/fittings.py` & `aa_memberaudit-2.9.1/memberaudit/core/fittings.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,30 @@
-"""Eve Online Fittings"""
+"""Eve Online fittings."""
+
 from dataclasses import dataclass, field
 from typing import List, Optional, Set, Tuple, Union
 
 from eveuniverse.models import EveType
 
 from .skills import Skill, compress_skills, required_skills_from_eve_types
 
 
 @dataclass(frozen=True)
 class _BaseFittingItem:
     def eve_types(self) -> Set[EveType]:
+        """Return types used in this fitting."""
         raise NotImplementedError()
 
     @property
     def is_empty(self) -> bool:
+        """Return True if fitting empty, else False."""
         raise NotImplementedError()
 
     def to_eft(self) -> str:
+        """Convert to EFT string format."""
         raise NotImplementedError()
 
     def __init__(self) -> None:
         raise RuntimeError("No instantiation from abstract base class")
 
 
 @dataclass(frozen=True)
@@ -117,16 +121,16 @@
             + self.drone_bay
             + self.fighter_bay
             + self.implants
             + self.boosters
             + self.cargo_bay
         )
         types = {self.ship_type}
-        for obj in [x for x in objs if x]:
-            types |= {eve_type for eve_type in obj.eve_types()}
+        for obj in [o for o in objs if o]:
+            types |= obj.eve_types()
         return types
 
     def required_skills(self) -> List[Skill]:
         """Skills required to fly this fitting."""
 
         eve_types = self.eve_types()
         skills = required_skills_from_eve_types(eve_types)
```

### Comparing `aa_memberaudit-2.9.0/memberaudit/core/skill_plans.py` & `aa_memberaudit-2.9.1/memberaudit/core/skill_plans.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Eve Online Skill plans."""
+"""Eve Online skill plans."""
 
 from dataclasses import dataclass
 from typing import List, Tuple
 
 from eveuniverse.models import EveType
 
 from .skills import Skill, compress_skills
@@ -14,14 +14,16 @@
 
 class NoSkillsIdentified(SkillPlanError):
     """Did not identify any skills."""
 
 
 @dataclass
 class SkillPlan:
+    """A skill plan."""
+
     name: str
     skills: List[Skill]
 
     @classmethod
     def create_from_plain_text(
         cls, name: str, text: str
     ) -> Tuple["SkillPlan", List[str]]:
```

### Comparing `aa_memberaudit-2.9.0/memberaudit/core/skills.py` & `aa_memberaudit-2.9.1/memberaudit/core/skills.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     """
     skills_raw = _identify_skills_from_eve_types(eve_types)
     skill_types = _gather_skill_types(skills_raw)
     skills = [
         Skill(eve_type=skill_types[type_id], level=level)
         for type_id, level in skills_raw
     ]
-    return sorted(skills, key=lambda x: x.eve_type.name)
+    return sorted(skills, key=lambda o: o.eve_type.name)
 
 
 def _identify_skills_from_eve_types(
     eve_types: Iterable[EveType],
 ) -> List[Tuple[int, int]]:
     eve_types = _reload_eve_types_without_dogmas(eve_types)
     all_attributes_map = _fetch_attributes_for_eve_types(eve_types)
```

### Comparing `aa_memberaudit-2.9.0/memberaudit/core/xml_converter.py` & `aa_memberaudit-2.9.1/memberaudit/core/xml_converter.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/decorators.py` & `aa_memberaudit-2.9.1/memberaudit/decorators.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Decorators for Member Audit."""
+
 from functools import wraps
 
 from django.http import HttpResponseForbidden, HttpResponseNotFound
 
 from allianceauth.services.hooks import get_extension_logger
 from app_utils.logging import LoggerAddTag
 
@@ -46,30 +48,30 @@
 
         return _wrapped_view
 
     return decorator
 
 
 def fetch_token_for_character(scopes=None):
-    """returns valid token for character.
-    Needs to be attached on a Character method !!
+    """Fetch and add valid token for a character.
+    Needs to be attached on a character section manager method !!
 
     Args:
-    -scopes: Optionally provide the required scopes.
-    Otherwise will use all scopes defined for this character.
+        -scopes: Optionally provide the required scopes.
+            Otherwise will use all scopes defined for this character.
     """
 
     def decorator(func):
         @wraps(func)
-        def _wrapped_view(character, *args, **kwargs):
+        def _wrapped_view(self, character, *args, **kwargs):
             token = character.fetch_token(scopes)
             logger.debug(
                 "%s: Using token %s for `%s`",
                 token.character_name,
                 token.pk,
                 func.__name__,
             )
-            return func(character, token, *args, **kwargs)
+            return func(self, character, token, *args, **kwargs)
 
         return _wrapped_view
 
     return decorator
```

### Comparing `aa_memberaudit-2.9.0/memberaudit/forms.py` & `aa_memberaudit-2.9.1/memberaudit/forms.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Member Audit forms."""
+
 from django import forms
 from django.core.exceptions import ValidationError
 
 from memberaudit.core.eft_parser import EftParserError
 from memberaudit.core.fittings import Fitting
 from memberaudit.core.skill_plans import SkillPlan, SkillPlanError
 from memberaudit.models import SkillSet, SkillSetGroup
@@ -43,15 +45,16 @@
         except EftParserError:
             raise ValidationError(
                 {
                     "fitting_text": (
                         "This fitting does not appear to be a valid EFT format."
                     )
                 }
-            )
+            ) from None
+
         data["_fitting"] = fitting
         data["_errors"] = errors
         skill_set_name = data.get("skill_set_name") or fitting.name
         if (
             not data["can_overwrite"]
             and SkillSet.objects.filter(name=skill_set_name).exists()
         ):
@@ -94,15 +97,16 @@
         try:
             skill_plan, errors = SkillPlan.create_from_plain_text(
                 name=data["skill_set_name"], text=data["skill_plan_text"]
             )
         except SkillPlanError:
             raise ValidationError(
                 {"skill_plan_text": "This does not appear to be a valid skill plan."}
-            )
+            ) from None
+
         data["_skill_plan"] = skill_plan
         data["_errors"] = errors
         if (
             not data["can_overwrite"]
             and SkillSet.objects.filter(name=data["skill_set_name"]).exists()
         ):
             raise ValidationError(
```

### Comparing `aa_memberaudit-2.9.0/memberaudit/helpers.py` & `aa_memberaudit-2.9.1/memberaudit/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Generic helpers."""
+
 from typing import Optional
 
 import unidecode
 
 from django.contrib.auth.models import User
 from django.db import models
 from django.utils.text import slugify
@@ -11,22 +13,22 @@
 
 from memberaudit import __title__
 
 logger = LoggerAddTag(get_extension_logger(__name__), __title__)
 
 
 def get_or_create_esi_or_none(
-    prop_name: str, dct: dict, Model: type
+    prop_name: str, dct: dict, model_class: type
 ) -> Optional[models.Model]:
     """Gets or creates a new eveuniverse object from a dictionary entry.
 
     return the object on success or None
     """
     if dct.get(prop_name):
-        obj, _ = Model.objects.get_or_create_esi(id=dct.get(prop_name))  # type: ignore
+        obj, _ = model_class.objects.get_or_create_esi(id=dct.get(prop_name))  # type: ignore
     else:
         obj = None
 
     return obj
 
 
 def get_or_create_or_none(
```

### Comparing `aa_memberaudit-2.9.0/memberaudit/locale/de/LC_MESSAGES/django.po` & `aa_memberaudit-2.9.1/memberaudit/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/locale/django.pot` & `aa_memberaudit-2.9.1/memberaudit/locale/django.pot`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/locale/en/LC_MESSAGES/django.po` & `aa_memberaudit-2.9.1/memberaudit/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/locale/es/LC_MESSAGES/django.po` & `aa_memberaudit-2.9.1/memberaudit/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/locale/fr_FR/LC_MESSAGES/django.po` & `aa_memberaudit-2.9.1/memberaudit/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/locale/it_IT/LC_MESSAGES/django.po` & `aa_memberaudit-2.9.1/memberaudit/locale/it_IT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/locale/ja/LC_MESSAGES/django.po` & `aa_memberaudit-2.9.1/memberaudit/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/locale/ko_KR/LC_MESSAGES/django.po` & `aa_memberaudit-2.9.1/memberaudit/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/locale/ru/LC_MESSAGES/django.mo` & `aa_memberaudit-2.9.1/memberaudit/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/locale/ru/LC_MESSAGES/django.po` & `aa_memberaudit-2.9.1/memberaudit/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/locale/uk/LC_MESSAGES/django.mo` & `aa_memberaudit-2.9.1/memberaudit/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/locale/uk/LC_MESSAGES/django.po` & `aa_memberaudit-2.9.1/memberaudit/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/locale/zh_Hans/LC_MESSAGES/django.po` & `aa_memberaudit-2.9.1/memberaudit/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/management/commands/memberaudit_data_export.py` & `aa_memberaudit-2.9.1/memberaudit/management/commands/memberaudit_data_export.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 class Command(BaseCommand):
     help = "Export data into a CSV file."
 
     def add_arguments(self, parser):
         parser.add_argument(
             "topic",
-            choices=sorted(DataExporter.topics),
+            choices=sorted(DataExporter.topics()),
             help="Section for exporting data from",
         )
         parser.add_argument(
             "--destination",
             default=str(Path.cwd().resolve()),
             help="Directory the output file will be written to",
         )
```

### Comparing `aa_memberaudit-2.9.0/memberaudit/management/commands/memberaudit_load_eve.py` & `aa_memberaudit-2.9.1/memberaudit/management/commands/memberaudit_load_eve.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/management/commands/memberaudit_reset_characters.py` & `aa_memberaudit-2.9.1/memberaudit/management/commands/memberaudit_reset_characters.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/management/commands/memberaudit_stats.py` & `aa_memberaudit-2.9.1/memberaudit/management/commands/memberaudit_stats.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/management/commands/memberaudit_update_characters.py` & `aa_memberaudit-2.9.1/memberaudit/management/commands/memberaudit_update_characters.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/managers/character.py` & `aa_memberaudit-2.9.1/memberaudit/managers/character.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,15 +198,15 @@
         duration_expression = ExpressionWrapper(
             F("finished_at") - F("started_at"),
             output_field=models.fields.DurationField(),
         )
         qs_base = qs_base.filter(root_task_id__in=root_task_ids.values()).annotate(
             duration=duration_expression
         )
-        update_stats = dict()
+        update_stats = {}
         if self.count() > 0:
             # per ring
             for ring in range(1, 4):
                 sections = Character.sections_in_ring(ring)
 
                 # calc totals
                 qs = qs_base.filter(section__in=sections)
```

### Comparing `aa_memberaudit-2.9.0/memberaudit/managers/general.py` & `aa_memberaudit-2.9.1/memberaudit/managers/general.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import datetime as dt
-from typing import Iterable, List, Optional, Tuple
+from typing import Iterable, List, Optional, Set, Tuple
 
 from bravado.exception import HTTPForbidden, HTTPUnauthorized
 from celery_once import AlreadyQueued
 
 from django.contrib.auth.models import Group, User
 from django.db import models, transaction
 from django.db.models import Q
@@ -15,23 +15,26 @@
 from allianceauth.services.hooks import get_extension_logger
 from app_utils.esi import fetch_esi_status
 from app_utils.logging import LoggerAddTag
 
 from memberaudit import __title__
 from memberaudit.app_settings import (
     MEMBERAUDIT_BULK_METHODS_BATCH_SIZE,
+    MEMBERAUDIT_DEVELOPER_MODE,
     MEMBERAUDIT_LOCATION_STALE_HOURS,
     MEMBERAUDIT_TASKS_LOW_PRIORITY,
 )
 from memberaudit.constants import DATETIME_FORMAT, EveCategoryId, EveTypeId
 from memberaudit.core.fittings import Fitting
 from memberaudit.core.skill_plans import SkillPlan
 from memberaudit.core.skills import Skill
-from memberaudit.helpers import filter_groups_available_to_user
+from memberaudit.decorators import fetch_token_for_character
+from memberaudit.helpers import store_debug_data_to_disk
 from memberaudit.providers import esi
+from memberaudit.utils import filter_groups_available_to_user
 
 logger = LoggerAddTag(get_extension_logger(__name__), __title__)
 
 
 class ComplianceGroupDesignationManager(models.Manager):
     def groups(self) -> models.QuerySet:
         """Groups which are compliance groups."""
@@ -182,35 +185,39 @@
             eve_type, _ = EveType.objects.get_or_create_esi(
                 id=EveTypeId.ASSET_SAFETY_WRAP
             )
             return self.update_or_create(
                 id=id,
                 defaults={"name": "ASSET SAFETY", "eve_type": eve_type},
             )
-        elif self.model.is_solar_system_id(id):
+
+        if self.model.is_solar_system_id(id):
             eve_solar_system, _ = EveSolarSystem.objects.get_or_create_esi(id=id)
             eve_type, _ = EveType.objects.get_or_create_esi(id=EveTypeId.SOLAR_SYSTEM)
             return self.update_or_create(
                 id=id,
                 defaults={
                     "name": eve_solar_system.name,
                     "eve_solar_system": eve_solar_system,
                     "eve_type": eve_type,
                 },
             )
-        elif self.model.is_station_id(id):
+
+        if self.model.is_station_id(id):
             logger.info("%s: Fetching station from ESI", id)
             station = esi.client.Universe.get_universe_stations_station_id(
                 station_id=id
             ).results()
             return self._station_update_or_create_dict(id=id, station=station)
-        elif self.model.is_structure_id(id):
+
+        if self.model.is_structure_id(id):
             if update_async:
                 return self._structure_update_or_create_esi_async(id=id, token=token)
             return self.structure_update_or_create_esi(id=id, token=token)
+
         logger.warning(
             "%s: Creating empty location for ID not matching any known pattern:", id
         )
         return self.get_or_create(id=id)
 
     def _station_update_or_create_dict(
         self, id: int, station: dict
@@ -258,23 +265,23 @@
         """Update or creates structure from ESI"""
         fetch_esi_status().raise_for_status()
         try:
             structure = esi.client.Universe.get_universe_structures_structure_id(
                 structure_id=id, token=token.valid_access_token()
             ).results()
         except (HTTPUnauthorized, HTTPForbidden) as http_error:
-            logger.warn(
+            logger.warning(
                 "%s: No access to structure #%s: %s",
                 token.character_name,
                 id,
                 http_error,
             )
             return self.get_or_create(id=id)
-        else:
-            return self._structure_update_or_create_dict(id=id, structure=structure)
+
+        return self._structure_update_or_create_dict(id=id, structure=structure)
 
     def _structure_update_or_create_dict(
         self, id: int, structure: dict
     ) -> Tuple[models.Model, bool]:
         """creates a new Location object from a structure dict"""
         if solar_system_id := structure.get("solar_system_id"):
             eve_solar_system, _ = EveSolarSystem.objects.get_or_create_esi(
@@ -299,14 +306,39 @@
                 "name": structure.get("name", ""),
                 "eve_solar_system": eve_solar_system,
                 "eve_type": eve_type,
                 "owner": owner,
             },
         )
 
+    def create_missing_esi(self, location_ids: Iterable, token: Token) -> Set[int]:
+        """Create missing locations from ESI based on given location IDs.
+        And return all existing location IDs.
+
+        Will do nothing when no IDs provided.
+        """
+        if not location_ids:
+            return set()
+
+        incoming_ids = set(location_ids)
+        existing_ids = set(self.values_list("id", flat=True))
+        missing_ids = incoming_ids.difference(existing_ids)
+        if missing_ids:
+            logger.info(
+                "%s: Loading %s missing locations from ESI", self, len(missing_ids)
+            )
+            for location_id in missing_ids:
+                try:
+                    self.get_or_create_esi_async(id=location_id, token=token)
+                except ValueError:
+                    pass
+                else:
+                    existing_ids.add(location_id)
+        return existing_ids
+
 
 class MailEntityManager(models.Manager):
     def get_or_create_esi(
         self, id: int, category: Optional[str] = None
     ) -> Tuple[models.Model, bool]:
         return self._get_or_create_esi(id=id, category=category, update_async=False)
 
@@ -354,38 +386,39 @@
             eve_entity, _ = EveEntity.objects.get_or_create_esi(id=id)
             if eve_entity:
                 return self.update_or_create_from_eve_entity(eve_entity)
             return self.update_or_create(
                 id=id,
                 defaults={"category": self.model.Category.MAILING_LIST},
             )
-        else:
-            if category == self.model.Category.MAILING_LIST:
-                return self.update_or_create(
-                    id=id,
-                    defaults={"category": self.model.Category.MAILING_LIST},
-                )
-            return self.update_or_create_from_eve_entity_id(id=id)
+
+        if category == self.model.Category.MAILING_LIST:
+            return self.update_or_create(
+                id=id,
+                defaults={"category": self.model.Category.MAILING_LIST},
+            )
+
+        return self.update_or_create_from_eve_entity_id(id=id)
 
     def update_or_create_esi_async(
         self, id: int, category: Optional[str] = None
     ) -> Tuple[models.Model, bool]:
         """Same as update_or_create_esi, but will create and return an empty object and delegate the ID resolution to a task (if needed),
         which will automatically retry on many common error conditions
         """
         id = int(id)
         try:
             obj = self.get(id=id)
+        except self.model.DoesNotExist:
+            pass
+        else:
             if obj.category == self.model.Category.MAILING_LIST:
                 return obj, False
-            else:
-                category = obj.category
 
-        except self.model.DoesNotExist:
-            pass
+            category = obj.category
 
         if category and category in self.model.Category.eve_entity_compatible():
             return self.update_or_create_esi(id=id, category=category)
         return self._update_or_create_esi_async(id=id)
 
     def _update_or_create_esi_async(self, id: int) -> Tuple[models.Model, bool]:
         from ..tasks import update_mail_entity_esi as task_update_mail_entity_esi
@@ -446,20 +479,68 @@
 
             self.bulk_update(
                 valid_objs.values(),
                 ["name"],
                 batch_size=MEMBERAUDIT_BULK_METHODS_BATCH_SIZE,
             )
 
+    @fetch_token_for_character("esi-mail.read_mail.v1")
+    def update_or_create_mailing_lists_esi(self, character, token: Token, force_update):
+        """Update or create wallet balance for a character from ESI.
+
+        Note: Obsolete mailing lists must not be removed,
+        since they might still be referenced by older mails.
+        """
+
+        logger.info("%s: Fetching mailing lists from ESI", character)
+        mailing_lists_raw = esi.client.Mail.get_characters_character_id_mail_lists(
+            character_id=character.eve_character.character_id,
+            token=token.valid_access_token(),
+        ).results()
+        if mailing_lists_raw:
+            mailing_lists = {
+                obj["mailing_list_id"]: obj
+                for obj in mailing_lists_raw
+                if "mailing_list_id" in obj
+            }
+        else:
+            mailing_lists = {}
+
+        if MEMBERAUDIT_DEVELOPER_MODE:
+            store_debug_data_to_disk(character, mailing_lists, "mailing_lists")
+
+        # TODO: replace with bulk methods to optimize
+
+        incoming_ids = set(mailing_lists.keys())
+        # existing_ids = set(character.mailing_lists.values_list("list_id", flat=True))
+        if not incoming_ids:
+            logger.info("%s: No new mailing lists", character)
+            return
+
+        section = character.UpdateSection.MAILS
+        if force_update or character.has_section_changed(
+            section=section, content=mailing_lists, hash_num=2
+        ):
+            new_mailing_lists = self._update_or_create_mailing_list_objs(
+                character=character, mailing_lists=mailing_lists
+            )
+            character.mailing_lists.set(new_mailing_lists, clear=True)
+            character.update_section_content_hash(
+                section=section, content=mailing_lists, hash_num=2
+            )
+
+        else:
+            logger.info("%s: Mailing lists have not changed", character)
+
     # @transaction.atomic()
-    def update_for_character(self, character, mailing_lists):
+    def _update_or_create_mailing_list_objs(self, character, mailing_lists):
         logger.info(
             "%s: Updating %s mailing lists", character, set(mailing_lists.keys())
         )
-        new_mailing_lists = list()
+        new_mailing_lists = []
         for list_id, mailing_list in mailing_lists.items():
             mailing_list_obj, _ = self.model.objects.update_or_create(
                 id=list_id,
                 defaults={
                     "category": self.model.Category.MAILING_LIST,
                     "name": mailing_list.get("name"),
                 },
@@ -549,15 +630,15 @@
 
         def _add_skill_set(groups_map, skill_set, group=None):
             group_id = group.id if group else 0
             if group_id not in groups_map.keys():
                 groups_map[group_id] = {"group": group, "skill_sets": []}
             groups_map[group_id]["skill_sets"].append(skill_set)
 
-        groups_map = dict()
+        groups_map = {}
         for skill_set in (
             self.select_related("ship_type").prefetch_related("groups").all()
         ):
             if skill_set.groups.exists():
                 for group in skill_set.groups.all():
                     _add_skill_set(groups_map, skill_set, group)
             else:
```

### Comparing `aa_memberaudit-2.9.0/memberaudit/migrations/0001_initial_new.py` & `aa_memberaudit-2.9.1/memberaudit/migrations/0001_initial_new.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/migrations/0002_add_mining_ledger.py` & `aa_memberaudit-2.9.1/memberaudit/migrations/0002_add_mining_ledger.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/migrations/0003_add_notify_permission.py` & `aa_memberaudit-2.9.1/memberaudit/migrations/0003_add_notify_permission.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/migrations/0004_character_is_disabled.py` & `aa_memberaudit-2.9.1/memberaudit/migrations/0004_character_is_disabled.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/migrations/0005_add_fw_stats.py` & `aa_memberaudit-2.9.1/memberaudit/migrations/0005_add_fw_stats.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/migrations/0006_add_localizations.py` & `aa_memberaudit-2.9.1/memberaudit/migrations/0006_add_localizations.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/migrations/0007_add_localization_2.py` & `aa_memberaudit-2.9.1/memberaudit/migrations/0007_add_localization_2.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/migrations/0008_improve_skill_sets.py` & `aa_memberaudit-2.9.1/memberaudit/migrations/0008_improve_skill_sets.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/migrations/0009_add_planetary_industry.py` & `aa_memberaudit-2.9.1/memberaudit/migrations/0009_add_planetary_industry.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/models/__init__.py` & `aa_memberaudit-2.9.1/memberaudit/models/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,43 +1,49 @@
-from .character import Character, CharacterUpdateStatus  # noqa: F401
-from .general import (  # noqa: F401
-    ComplianceGroupDesignation,
-    EveShipType,
-    EveSkillType,
-    General,
-    Location,
-    MailEntity,
-    SkillSet,
-    SkillSetGroup,
-    SkillSetSkill,
-)
-from .sections import (  # noqa: F401
+# flake8: noqa
+
+from .character_sections_1 import (
     CharacterAsset,
     CharacterAttributes,
     CharacterContact,
     CharacterContactLabel,
     CharacterContract,
     CharacterContractBid,
     CharacterContractItem,
+)
+from .character_sections_2 import (
     CharacterCorporationHistory,
     CharacterDetails,
     CharacterFwStats,
     CharacterImplant,
     CharacterJumpClone,
     CharacterJumpCloneImplant,
     CharacterLocation,
     CharacterLoyaltyEntry,
     CharacterMail,
     CharacterMailLabel,
     CharacterMailUnreadCount,
+)
+from .character_sections_3 import (
     CharacterMiningLedgerEntry,
     CharacterOnlineStatus,
     CharacterPlanet,
     CharacterShip,
     CharacterSkill,
     CharacterSkillpoints,
     CharacterSkillqueueEntry,
     CharacterSkillSetCheck,
     CharacterWalletBalance,
     CharacterWalletJournalEntry,
     CharacterWalletTransaction,
 )
+from .characters import Character, CharacterUpdateStatus
+from .general import (
+    ComplianceGroupDesignation,
+    EveShipType,
+    EveSkillType,
+    General,
+    Location,
+    MailEntity,
+    SkillSet,
+    SkillSetGroup,
+    SkillSetSkill,
+)
```

### Comparing `aa_memberaudit-2.9.0/memberaudit/models/general.py` & `aa_memberaudit-2.9.1/memberaudit/models/general.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Top level models
 """
+from typing import Set
 
 from django.contrib.auth.models import Group, Permission, User
 from django.core.exceptions import ValidationError
 from django.core.validators import MaxValueValidator, MinValueValidator
 from django.db import models
 from django.utils.timezone import now
 from django.utils.translation import gettext_lazy as _
@@ -60,32 +61,36 @@
         """return basic permission needed to use this app"""
         return Permission.objects.select_related("content_type").get(
             content_type__app_label=cls._meta.app_label, codename="basic_access"
         )
 
     @classmethod
     def users_with_basic_access(cls) -> models.QuerySet:
+        """Return users which have at least basic access to Member Audit."""
         return users_with_permission(cls.basic_permission())
 
     @classmethod
     def accessible_users(cls, user: User) -> models.QuerySet:
         """Users that the given user can access."""
         if user.has_perm("memberaudit.view_everything"):
             return cls.users_with_basic_access()
-        elif (
+
+        if (
             user.has_perm("memberaudit.view_same_alliance")
             and user.profile.main_character.alliance_id
         ):
             return cls.users_with_basic_access().filter(
                 profile__main_character__alliance_id=user.profile.main_character.alliance_id
             )
-        elif user.has_perm("memberaudit.view_same_corporation"):
+
+        if user.has_perm("memberaudit.view_same_corporation"):
             return cls.users_with_basic_access().filter(
                 profile__main_character__corporation_id=user.profile.main_character.corporation_id
             )
+
         return User.objects.filter(pk=user.pk)
 
     @classmethod
     def compliant_users(cls) -> models.QuerySet:
         """Users which are fully compliant."""
         return cls.users_with_basic_access().exclude(
             character_ownerships__character__memberaudit_character__isnull=True
@@ -438,15 +443,15 @@
         return bool(self.required_level)
 
     @property
     def required_skill_str(self) -> str:  # TODO: Add test
         return self._skill_str(self.required_level) if self.required_level else ""
 
     @property
-    def recommened_skill_str(self) -> str:  # TODO: Add test
+    def recommended_skill_str(self) -> str:  # TODO: Add test
         return self._skill_str(self.recommended_level) if self.recommended_level else ""
 
     @property
     def maximum_level(self) -> int:  # TODO: Add test
         """Maximum level of this skill."""
         levels = [1]
         if self.recommended_level:
@@ -465,22 +470,25 @@
         return f"{self.eve_type.name} {level_str}"
 
 
 class MailEntity(models.Model):
     """A sender or recipient in a mail"""
 
     class Category(models.TextChoices):
+        """A category of a mail entity."""
+
         ALLIANCE = "AL", _("Alliance")
         CHARACTER = "CH", _("Character")
         CORPORATION = "CO", _("Corporation")
         MAILING_LIST = "ML", _("Mailing List")
         UNKNOWN = "UN", _("Unknown")
 
         @classmethod
-        def eve_entity_compatible(cls) -> set:
+        def eve_entity_compatible(cls) -> Set["MailEntity.Category"]:
+            """Return categories, which are compatible with EveEntity."""
             return {cls.ALLIANCE, cls.CHARACTER, cls.CORPORATION}
 
     id = models.PositiveIntegerField(primary_key=True)
     category = models.CharField(
         max_length=2, choices=Category.choices, db_index=True
     )  # mandatory
     name = models.CharField(max_length=255, db_index=True)  # optional
@@ -517,15 +525,14 @@
         super().save(*args, **kwargs)
 
     def external_url(self) -> str:
         """returns URL for to show details of this entity on external website"""
         if self.category == self.Category.ALLIANCE and self.name:
             return dotlan.alliance_url(self.name)
 
-        elif self.category == self.Category.CHARACTER:
+        if self.category == self.Category.CHARACTER:
             return evewho.character_url(self.id)
 
-        elif self.category == self.Category.CORPORATION and self.name:
+        if self.category == self.Category.CORPORATION and self.name:
             return dotlan.corporation_url(self.name)
 
-        else:
-            return ""
+        return ""
```

### Comparing `aa_memberaudit-2.9.0/memberaudit/static/memberaudit/css/character_viewer.css` & `aa_memberaudit-2.9.1/memberaudit/static/memberaudit/css/character_viewer.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/static/memberaudit/css/character_viewer.min.css` & `aa_memberaudit-2.9.1/memberaudit/static/memberaudit/css/character_viewer.min.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/static/memberaudit/css/global.css` & `aa_memberaudit-2.9.1/memberaudit/static/memberaudit/css/global.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/static/memberaudit/css/global.min.css` & `aa_memberaudit-2.9.1/memberaudit/static/memberaudit/css/global.min.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/static/memberaudit/css/launcher.css` & `aa_memberaudit-2.9.1/memberaudit/static/memberaudit/css/launcher.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/static/memberaudit/css/launcher.min.css` & `aa_memberaudit-2.9.1/memberaudit/static/memberaudit/css/launcher.min.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/static/memberaudit/css/memberaudit.css` & `aa_memberaudit-2.9.1/memberaudit/static/memberaudit/css/memberaudit.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/static/memberaudit/css/memberaudit.min.css` & `aa_memberaudit-2.9.1/memberaudit/static/memberaudit/css/memberaudit.min.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/static/memberaudit/css/reports.css` & `aa_memberaudit-2.9.1/memberaudit/static/memberaudit/css/reports.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/static/memberaudit/images/Spinner-1s-64px-dark.gif` & `aa_memberaudit-2.9.1/memberaudit/static/memberaudit/images/Spinner-1s-64px-dark.gif`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/static/memberaudit/images/Spinner-1s-64px-light.gif` & `aa_memberaudit-2.9.1/memberaudit/static/memberaudit/images/Spinner-1s-64px-light.gif`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/static/memberaudit/images/charisma.png` & `aa_memberaudit-2.9.1/memberaudit/static/memberaudit/images/charisma.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/static/memberaudit/images/eve-prism.png` & `aa_memberaudit-2.9.1/memberaudit/static/memberaudit/images/eve-prism.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/static/memberaudit/images/evesearch.png` & `aa_memberaudit-2.9.1/memberaudit/static/memberaudit/images/evesearch.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/static/memberaudit/images/intelligence.png` & `aa_memberaudit-2.9.1/memberaudit/static/memberaudit/images/intelligence.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/static/memberaudit/images/memory.png` & `aa_memberaudit-2.9.1/memberaudit/static/memberaudit/images/memory.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/static/memberaudit/images/perception.png` & `aa_memberaudit-2.9.1/memberaudit/static/memberaudit/images/perception.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/static/memberaudit/images/willpower.png` & `aa_memberaudit-2.9.1/memberaudit/static/memberaudit/images/willpower.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/static/memberaudit/vendor/datatables/plugins/dataTables.rowGroup.min.js` & `aa_memberaudit-2.9.1/memberaudit/static/memberaudit/vendor/datatables/plugins/dataTables.rowGroup.min.js`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/static/memberaudit/vendor/datatables/plugins/datetime.js` & `aa_memberaudit-2.9.1/memberaudit/static/memberaudit/vendor/datatables/plugins/datetime.js`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/static/memberaudit/vendor/datatables/plugins/filterDropDown.min.js` & `aa_memberaudit-2.9.1/memberaudit/static/memberaudit/vendor/datatables/plugins/filterDropDown.min.js`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/static/memberaudit/vendor/moment/moment.min.js` & `aa_memberaudit-2.9.1/memberaudit/static/memberaudit/vendor/moment/moment.min.js`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/swagger.json` & `aa_memberaudit-2.9.1/memberaudit/swagger.json`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/tasks.py` & `aa_memberaudit-2.9.1/memberaudit/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Celery tasks for Member Audit."""
+
 import inspect
 import random
 from typing import Optional
 
 from celery import chain, shared_task
 
 from django.contrib.auth.models import Group, User
@@ -18,15 +20,15 @@
     EsiDailyDowntime,
     EsiErrorLimitExceeded,
     EsiOffline,
     fetch_esi_status,
 )
 from app_utils.logging import LoggerAddTag
 
-from memberaudit import __title__, helpers
+from memberaudit import __title__, utils
 from memberaudit.app_settings import (
     MEMBERAUDIT_BULK_METHODS_BATCH_SIZE,
     MEMBERAUDIT_LOG_UPDATE_STATS,
     MEMBERAUDIT_TASKS_LOW_PRIORITY,
     MEMBERAUDIT_TASKS_MAX_ASSETS_PER_PASS,
     MEMBERAUDIT_TASKS_NORMAL_PRIORITY,
     MEMBERAUDIT_TASKS_OBJECT_CACHE_TIMEOUT,
@@ -260,15 +262,20 @@
 
 # Update sections
 
 
 @shared_task(
     **{
         **TASK_DEFAULTS_BIND_ONCE,
-        **{"once": {"keys": ["character_pk", "section", "force_update"]}},
+        **{
+            "once": {
+                "keys": ["character_pk", "section", "force_update"],
+                "graceful": True,
+            }
+        },
     }
 )
 def update_character_section(
     self,
     character_pk: int,
     section: str,
     force_update: bool = False,
@@ -355,15 +362,15 @@
 
 # Special tasks for updating assets
 
 
 @shared_task(
     **{
         **TASK_DEFAULTS_BIND_ONCE,
-        **{"once": {"keys": ["character_pk", "force_update"]}},
+        **{"once": {"keys": ["character_pk", "force_update"], "graceful": True}},
     }
 )
 def update_character_assets(
     self,
     character_pk: int,
     force_update: bool = False,
     root_task_id: Optional[str] = None,
@@ -446,16 +453,16 @@
     )
     if asset_list is None:
         _log_character_update_success(character, Character.UpdateSection.ASSETS)
         return
 
     logger.info("%s: Creating parent assets - pass %s", character, cycle)
 
-    assets_flat = {int(x["item_id"]): x for x in asset_list}
-    new_assets = list()
+    assets_flat = {int(item["item_id"]): item for item in asset_list}
+    new_assets = []
     priority = _get_task_priority(self) or MEMBERAUDIT_TASKS_LOW_PRIORITY
     with transaction.atomic():
         if cycle == 1:
             character.assets.all().delete()
 
         location_ids = set(Location.objects.values_list("id", flat=True))
         parent_asset_ids = {
@@ -529,18 +536,18 @@
     """
     character = Character.objects.get_cached(
         pk=character_pk, timeout=MEMBERAUDIT_TASKS_OBJECT_CACHE_TIMEOUT
     )
     logger.info("%s: Creating child assets - pass %s", character, cycle)
 
     # for debug
-    # character._store_list_to_disk(asset_list, f"child_asset_list_{cycle}")
+    # store_list_to_disk(character, asset_list, f"child_asset_list_{cycle}")
 
-    new_assets = list()
-    assets_flat = {int(x["item_id"]): x for x in asset_list}
+    new_assets = []
+    assets_flat = {int(item["item_id"]): item for item in asset_list}
     priority = _get_task_priority(self) or MEMBERAUDIT_TASKS_LOW_PRIORITY
     with transaction.atomic():
         parent_asset_ids = set(character.assets.values_list("item_id", flat=True))
         child_asset_ids = {
             item_id
             for item_id, item in assets_flat.items()
             if item.get("location_id") and item["location_id"] in parent_asset_ids
@@ -597,15 +604,15 @@
 
 # Special tasks for updating mail section
 
 
 @shared_task(
     **{
         **TASK_DEFAULTS_BIND_ONCE,
-        **{"once": {"keys": ["character_pk", "force_update"]}},
+        **{"once": {"keys": ["character_pk", "force_update"], "graceful": True}},
     }
 )
 def update_character_mails(
     self,
     character_pk: int,
     force_update: bool = False,
     root_task_id: Optional[str] = None,
@@ -729,15 +736,15 @@
 
 # special tasks for updating contacts
 
 
 @shared_task(
     **{
         **TASK_DEFAULTS_BIND_ONCE,
-        **{"once": {"keys": ["character_pk", "force_update"]}},
+        **{"once": {"keys": ["character_pk", "force_update"], "graceful": True}},
     }
 )
 def update_character_contacts(
     self,
     character_pk: int,
     force_update: bool = False,
     root_task_id: Optional[str] = None,
@@ -803,15 +810,15 @@
 
 # special tasks for updating contracts
 
 
 @shared_task(
     **{
         **TASK_DEFAULTS_BIND_ONCE,
-        **{"once": {"keys": ["character_pk", "force_update"]}},
+        **{"once": {"keys": ["character_pk", "force_update"], "graceful": True}},
     }
 )
 def update_character_contracts(
     self,
     character_pk: int,
     force_update: bool = False,
     root_task_id: Optional[str] = None,
@@ -935,15 +942,20 @@
     contract = CharacterContract.objects.get(pk=contract_pk)
     character.update_contract_bids(contract)
 
 
 # special tasks for updating wallet
 
 
-@shared_task(**{**TASK_DEFAULTS_BIND_ONCE, **{"once": {"keys": ["character_pk"]}}})
+@shared_task(
+    **{
+        **TASK_DEFAULTS_BIND_ONCE,
+        **{"once": {"keys": ["character_pk"], "graceful": True}},
+    }
+)
 def update_character_wallet_journal(
     self,
     character_pk: int,
     root_task_id: Optional[str] = None,
     parent_task_id: Optional[str] = None,
 ) -> None:
     """Main task for updating wallet journal of a character"""
@@ -992,15 +1004,18 @@
         return
     EveMarketPrice.objects.update_from_esi(
         minutes_until_stale=MEMBERAUDIT_UPDATE_STALE_RING_2
     )
 
 
 @shared_task(
-    **{**TASK_DEFAULTS_BIND_ONCE, **{"once": {"keys": ["id"]}, "max_retries": None}}
+    **{
+        **TASK_DEFAULTS_BIND_ONCE,
+        **{"once": {"keys": ["id"], "graceful": True}, "max_retries": None},
+    }
 )
 def update_structure_esi(self, id: int, token_pk: int):
     """Updates a structure object from ESI
     and retries later if the ESI error limit has already been reached
     """
     try:
         token = Token.objects.get(pk=token_pk)
@@ -1026,15 +1041,18 @@
             id,
             ex.retry_in,
         )
         raise self.retry(countdown=ex.retry_in) from ex
 
 
 @shared_task(
-    **{**TASK_DEFAULTS_ONCE, **{"once": {"keys": ["id"]}, "max_retries": None}}
+    **{
+        **TASK_DEFAULTS_ONCE,
+        **{"once": {"keys": ["id"], "graceful": True}, "max_retries": None},
+    }
 )
 def update_mail_entity_esi(id: int, category: Optional[str] = None):
     """Updates a mail entity object from ESI
     and retries later if the ESI error limit has already been reached
     """
     MailEntity.objects.update_or_create_esi(id=id, category=category)
 
@@ -1079,15 +1097,15 @@
 
 @shared_task(**TASK_DEFAULTS_BIND)
 def export_data(self, user_pk: Optional[int] = None) -> None:
     """Export data to files."""
     priority = _get_task_priority(self) or MEMBERAUDIT_TASKS_LOW_PRIORITY
     tasks = [
         _export_data_for_topic.si(topic).set(priority=priority)
-        for topic in data_exporters.DataExporter.topics
+        for topic in data_exporters.DataExporter.topics()
     ]
     if user_pk:
         tasks.append(_export_data_inform_user.si(user_pk))
     chain(tasks).delay()
 
 
 @shared_task(**TASK_DEFAULTS_BIND)
@@ -1116,16 +1134,16 @@
         message = f"Data export has been completed for topic {topic}."
     else:
         title = f"{__title__}: Full data export completed"
         message = (
             "Data export for all topics has been completed. "
             "It covers the following:\n"
         )
-        for topic in data_exporters.DataExporter.topics:
-            message += f"- {topic}\n"
+        for obj in data_exporters.DataExporter.topics():
+            message += f"- {obj}\n"
     notify(user=user, title=title, message=message, level="INFO")
 
 
 @shared_task(**TASK_DEFAULTS_BIND_ONCE)
 def update_compliance_groups_for_all(self):
     """Update compliance groups for all users."""
     if ComplianceGroupDesignation.objects.exists():
@@ -1150,8 +1168,8 @@
     General.add_compliant_users_to_group(group)
 
 
 @shared_task(**TASK_DEFAULTS)
 def clear_users_from_group(group_pk: int):
     """Clear all users from given group."""
     group = Group.objects.get(pk=group_pk)
-    helpers.clear_users_from_group(group)
+    utils.clear_users_from_group(group)
```

### Comparing `aa_memberaudit-2.9.0/memberaudit/templates/admin/memberaudit/character/confirm_character_deletion.html` & `aa_memberaudit-2.9.1/memberaudit/templates/admin/memberaudit/character/confirm_character_deletion.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/templates/admin/memberaudit/skillset/import_skills.html` & `aa_memberaudit-2.9.1/memberaudit/templates/admin/memberaudit/skillset/import_skills.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/character_finder.html` & `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/character_finder.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/character_viewer.html` & `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/character_viewer.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/data_export.html` & `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/data_export.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/launcher.html` & `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/launcher.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/modals/character_viewer/asset_container.html` & `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/modals/character_viewer/asset_container.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/modals/character_viewer/asset_container_content.html` & `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/modals/character_viewer/asset_container_content.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/modals/character_viewer/character_skill_set_details.html` & `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/modals/character_viewer/character_skill_set_details.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/modals/character_viewer/contract.html` & `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/modals/character_viewer/contract.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/modals/character_viewer/contract_content.html` & `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/modals/character_viewer/contract_content.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/modals/character_viewer/contract_items.html` & `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/modals/character_viewer/contract_items.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/modals/character_viewer/mail.html` & `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/modals/character_viewer/mail.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/modals/character_viewer/skill_set_content.html` & `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/modals/character_viewer/skill_set_content.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/character_viewer/overview.html` & `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/overview.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/character_viewer/sidebar.html` & `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/sidebar.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/character_viewer/sidebar_character.html` & `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/sidebar_character.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/assets.html` & `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/assets.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes.html` & `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes_content.html` & `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes_content.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contacts.html` & `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contacts.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contracts.html` & `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contracts.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history.html` & `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html` & `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats.html` & `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats_content.html` & `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats_content.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/implants.html` & `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/implants.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/jump_clones.html` & `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/jump_clones.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/loyalty.html` & `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/loyalty.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mails.html` & `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mails.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mining_ledger.html` & `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mining_ledger.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/planets.html` & `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/planets.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_queue.html` & `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_queue.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_sets.html` & `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_sets.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skills.html` & `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skills.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_journal.html` & `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_journal.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_transactions.html` & `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_transactions.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs_navigation.html` & `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs_navigation.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/menu.html` & `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/menu.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/reports/tabs/corporation_compliance.html` & `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/reports/tabs/corporation_compliance.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/reports/tabs/skill_sets.html` & `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/reports/tabs/skill_sets.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/reports/tabs/user_compliance.html` & `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/reports/tabs/user_compliance.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/reports/tabs_navigation.html` & `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/reports/tabs_navigation.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/partials/solar_system.html` & `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/solar_system.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/templates/memberaudit/reports.html` & `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/reports.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/tests/core/test_core_xml_converter.py` & `aa_memberaudit-2.9.1/memberaudit/tests/core/test_core_xml_converter.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/tests/core/test_data_exporters.py` & `aa_memberaudit-2.9.1/memberaudit/tests/core/test_data_exporters.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
             with ZipFile(zip_file, "r") as myzip:
                 namelist = myzip.namelist()
             self.assertIn(source_file.name, namelist)
 
 
 class NotTopicExporter(DataExporter):
     def format_obj(self, *args, **kwargs):
-        return dict()
+        return {}
 
     def get_queryset(self, *args, **kwargs):
         return None
 
 
 class InvalidTopicExporter(NotTopicExporter):
     topic = "invalid_topic"
@@ -150,15 +150,15 @@
 
     def test_should_not_create_exporters(self):
         with self.assertRaises(ValueError):
             DataExporter.create_exporter("not-implemented")
 
     def test_should_return_topics(self):
         self.assertListEqual(
-            DataExporter.topics, ["contract", "contract-item", "wallet-journal"]
+            DataExporter.topics(), ["contract", "contract-item", "wallet-journal"]
         )
 
     def test_can_not_init_exporter_without_topic(self):
         with self.assertRaises(ValueError):
             NotTopicExporter()
 
     def test_can_not_init_exporter_with_invalid_topic(self):
```

### Comparing `aa_memberaudit-2.9.0/memberaudit/tests/core/test_eft_parser.py` & `aa_memberaudit-2.9.1/memberaudit/tests/core/test_eft_parser.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/tests/core/test_fittings.py` & `aa_memberaudit-2.9.1/memberaudit/tests/core/test_fittings.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/tests/core/test_skill_plans.py` & `aa_memberaudit-2.9.1/memberaudit/tests/core/test_skill_plans.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/tests/core/test_skills.py` & `aa_memberaudit-2.9.1/memberaudit/tests/core/test_skills.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/tests/managers/test_character.py` & `aa_memberaudit-2.9.1/memberaudit/tests/managers/test_character.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/tests/managers/test_general.py` & `aa_memberaudit-2.9.1/memberaudit/tests/managers/test_general.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from bravado.exception import HTTPForbidden, HTTPNotFound, HTTPUnauthorized
 from celery_once import AlreadyQueued
 
 from django.core.cache import cache
 from django.test import override_settings
 from django.utils.timezone import now
+from esi.models import Token
 from eveuniverse.models import EveEntity, EveSolarSystem, EveType
 
 from allianceauth.eveonline.models import EveCorporationInfo
 from allianceauth.notifications.models import Notification
 from app_utils.esi import EsiStatus, fetch_esi_status
 from app_utils.esi_testing import BravadoOperationStub, BravadoResponseStub
 from app_utils.testing import (
@@ -34,14 +35,15 @@
     create_skill,
     create_skill_plan,
     create_skill_set_group,
 )
 from ..testdata.load_entities import load_entities
 from ..testdata.load_eveuniverse import load_eveuniverse
 from ..utils import (
+    CharacterUpdateTestDataMixin,
     NoSocketsTestCaseFixtures,
     add_auth_character_to_user,
     add_memberaudit_character_to_user,
     create_memberaudit_character,
 )
 
 MANAGERS_PATH = "memberaudit.managers.general"
@@ -166,15 +168,15 @@
         # when
         ComplianceGroupDesignation.objects.update_user(user)
         # then
         self.assertNotIn(compliance_group_1, user.groups.all())
         self.assertNotIn(compliance_group_2, user.groups.all())
         self.assertIn(other_group, user.groups.all())
 
-    def test_user_with_one_registered_and_one_unregistered_characater_is_not_compliant(
+    def test_user_with_one_registered_and_one_unregistered_character_is_not_compliant(
         self, mock_notify
     ):
         # given
         compliance_group = create_compliance_group()
         user, _ = create_user_from_evecharacter(
             1001, permissions=["memberaudit.basic_access"]
         )
@@ -893,14 +895,63 @@
         self.assertEqual(obj.id, 2004)
         self.assertEqual(obj.name, "ASSET SAFETY")
         self.assertIsNone(obj.eve_solar_system)
         self.assertIsNone(obj.owner)
         self.assertEqual(obj.eve_type, EveType.objects.get(id=60))
 
 
+@patch(MANAGERS_PATH + ".esi")
+@patch(MANAGERS_PATH + ".LocationManager.get_or_create_esi_async")
+class TestLocationManagerPreload(NoSocketsTestCase):
+    @classmethod
+    def setUpClass(cls) -> None:
+        super().setUpClass()
+        load_eveuniverse()
+        load_entities()
+        cls.token = MagicMock(spec=Token)
+
+    def test_can_preload_missing_locations(
+        self, mock_get_or_create_esi_async, mock_esi
+    ):
+        # given
+        mock_esi.client = esi_client_stub
+        Location.objects.update_or_create_esi(id=60003760, token=self.token)
+        # when
+        result = Location.objects.create_missing_esi([60003760, 30002537], self.token)
+        # then
+        self.assertEqual(mock_get_or_create_esi_async.call_count, 1)
+        _, kwargs = mock_get_or_create_esi_async.call_args
+        self.assertEqual(kwargs["id"], 30002537)
+        self.assertSetEqual(result, {60003760, 30002537})
+
+    def test_can_do_nothing_when_all_locations_found(
+        self, mock_get_or_create_esi_async, mock_esi
+    ):
+        # given
+        mock_esi.client = esi_client_stub
+        Location.objects.update_or_create_esi(id=60003760, token=self.token)
+        Location.objects.update_or_create_esi(id=30002537, token=self.token)
+        # when
+        result = Location.objects.create_missing_esi([60003760, 30002537], self.token)
+        # then
+        self.assertEqual(mock_get_or_create_esi_async.call_count, 0)
+        self.assertSetEqual(result, {60003760, 30002537})
+
+    def test_can_do_nothing_when_no_ids_provided(
+        self, mock_get_or_create_esi_async, mock_esi
+    ):
+        # given
+        mock_esi.client = esi_client_stub
+        # when
+        result = Location.objects.create_missing_esi([], self.token)
+        # then
+        self.assertEqual(mock_get_or_create_esi_async.call_count, 0)
+        self.assertSetEqual(result, set())
+
+
 class TestLocationManagerAsync(NoSocketsTestCaseFixtures):
     @classmethod
     def setUpClass(cls) -> None:
         super().setUpClass()
         load_eveuniverse()
         load_entities()
         cls.jita = EveSolarSystem.objects.get(id=30000142)
@@ -958,14 +1009,103 @@
         self.assertTrue(created)
         self.assertEqual(obj.id, 1000000000001)
         self.assertIsNone(obj.eve_solar_system)
         self.assertIsNone(obj.eve_type)
         self.assertTrue(mock_task_update_structure_esi.apply_async.called)
 
 
+@patch(MANAGERS_PATH + ".esi")
+class TestCharacterMailingLists(CharacterUpdateTestDataMixin, NoSocketsTestCase):
+    def test_update_mailing_lists_1(self, mock_esi):
+        """can create new mailing lists from scratch"""
+        mock_esi.client = esi_client_stub
+
+        self.character_1001.update_mailing_lists()
+
+        self.assertSetEqual(
+            set(MailEntity.objects.values_list("id", flat=True)), {9001, 9002}
+        )
+        self.assertSetEqual(
+            set(self.character_1001.mailing_lists.values_list("id", flat=True)),
+            {9001, 9002},
+        )
+
+        obj = MailEntity.objects.get(id=9001)
+        self.assertEqual(obj.name, "Dummy 1")
+
+        obj = MailEntity.objects.get(id=9002)
+        self.assertEqual(obj.name, "Dummy 2")
+
+    def test_update_mailing_lists_2(self, mock_esi):
+        """does not remove obsolete mailing lists"""
+        mock_esi.client = esi_client_stub
+        MailEntity.objects.create(
+            id=5, category=MailEntity.Category.MAILING_LIST, name="Obsolete"
+        )
+
+        self.character_1001.update_mailing_lists()
+
+        self.assertSetEqual(
+            set(MailEntity.objects.values_list("id", flat=True)), {9001, 9002, 5}
+        )
+        self.assertSetEqual(
+            set(self.character_1001.mailing_lists.values_list("id", flat=True)),
+            {9001, 9002},
+        )
+
+    def test_update_mailing_lists_3(self, mock_esi):
+        """updates existing mailing lists"""
+        mock_esi.client = esi_client_stub
+        MailEntity.objects.create(
+            id=9001, category=MailEntity.Category.MAILING_LIST, name="Update me"
+        )
+
+        self.character_1001.update_mailing_lists()
+
+        self.assertSetEqual(
+            set(MailEntity.objects.values_list("id", flat=True)), {9001, 9002}
+        )
+        self.assertSetEqual(
+            set(self.character_1001.mailing_lists.values_list("id", flat=True)),
+            {9001, 9002},
+        )
+        obj = MailEntity.objects.get(id=9001)
+        self.assertEqual(obj.name, "Dummy 1")
+
+    def test_update_mailing_lists_4(self, mock_esi):
+        """when data from ESI has not changed, then skip update"""
+        mock_esi.client = esi_client_stub
+
+        self.character_1001.update_mailing_lists()
+        obj = MailEntity.objects.get(id=9001)
+        obj.name = "Extravaganza"
+        obj.save()
+        self.character_1001.mailing_lists.clear()
+
+        self.character_1001.update_mailing_lists()
+        obj = MailEntity.objects.get(id=9001)
+        self.assertEqual(obj.name, "Extravaganza")
+        self.assertSetEqual(
+            set(self.character_1001.mailing_lists.values_list("id", flat=True)), set()
+        )
+
+    def test_update_mailing_lists_5(self, mock_esi):
+        """when data from ESI has not changed and update is forced, then do update"""
+        mock_esi.client = esi_client_stub
+
+        self.character_1001.update_mailing_lists()
+        obj = MailEntity.objects.get(id=9001)
+        obj.name = "Extravaganza"
+        obj.save()
+
+        self.character_1001.update_mailing_lists(force_update=True)
+        obj = MailEntity.objects.get(id=9001)
+        self.assertEqual(obj.name, "Dummy 1")
+
+
 class TestSkillSetManager(NoSocketsTestCase):
     @classmethod
     def setUpClass(cls) -> None:
         super().setUpClass()
         load_eveuniverse()
         load_entities()
         cls.fitting = create_fitting(name="My fitting")
```

### Comparing `aa_memberaudit-2.9.0/memberaudit/tests/models/test_character_1.py` & `aa_memberaudit-2.9.1/memberaudit/tests/models/test_characters_1.py`

 * *Files 0% similar despite different names*

```diff
@@ -376,15 +376,15 @@
     def test_should_raise_exception_with_scope_not_found_for_orphans(self):
         # given
         character = create_character(EveCharacter.objects.get(character_id=1121))
         # when
         with self.assertRaises(TokenError):
             character.fetch_token()
 
-    @patch(MODELS_PATH + ".character.notify_throttled")
+    @patch(MODELS_PATH + ".characters.notify_throttled")
     def test_should_raise_exception_and_notify_user_if_scope_not_found(
         self, mock_notify_throttled
     ):
         # given
         character = create_memberaudit_character(1001)
         # when
         with self.assertRaises(TokenError):
@@ -932,15 +932,15 @@
         )
 
     def test_is_updating_2(self):
         """When section does not exist, then return False"""
         self.assertTrue(self.character_1001.is_section_updating(section=self.section))
 
 
-@patch(MODELS_PATH + ".character.MEMBERAUDIT_UPDATE_STALE_RING_3", 640)
+@patch(MODELS_PATH + ".characters.MEMBERAUDIT_UPDATE_STALE_RING_3", 640)
 class TestCharacterIsUpdateSectionStale(NoSocketsTestCase):
     @classmethod
     def setUpClass(cls) -> None:
         super().setUpClass()
         load_entities()
         cls.section = Character.UpdateSection.ASSETS
```

### Comparing `aa_memberaudit-2.9.0/memberaudit/tests/models/test_character_2.py` & `aa_memberaudit-2.9.1/memberaudit/tests/managers/test_character_sections_2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,536 +1,127 @@
 import datetime as dt
 from unittest.mock import patch
 
-from pytz import utc
-
-from django.test import override_settings
+from django.test import TestCase, override_settings
 from django.utils.dateparse import parse_datetime
 from django.utils.timezone import now
-from eveuniverse.models import EveEntity, EveType
 
+from app_utils.esi_testing import EsiClientStub, EsiEndpoint, build_http_error
 from app_utils.testing import NoSocketsTestCase
 
 from memberaudit.core.xml_converter import eve_xml_to_html
-
-from ...models import (
-    CharacterContact,
-    CharacterContactLabel,
-    CharacterContract,
-    CharacterContractBid,
+from memberaudit.models import (
+    CharacterCorporationHistory,
     CharacterDetails,
+    CharacterFwStats,
+    CharacterJumpClone,
+    CharacterLocation,
+    CharacterLoyaltyEntry,
+    CharacterMail,
+    CharacterMailLabel,
+    MailEntity,
 )
-from ..testdata.esi_client_stub import esi_client_stub
-from ..utils import create_memberaudit_character
-from .utils import CharacterUpdateTestDataMixin
-
-MODELS_PATH = "memberaudit.models"
-MANAGERS_PATH = "memberaudit.managers"
-TASKS_PATH = "memberaudit.tasks"
-
-
-@override_settings(CELERY_ALWAYS_EAGER=True, CELERY_EAGER_PROPAGATES_EXCEPTIONS=True)
-@patch(MODELS_PATH + ".character.esi")
-class TestCharacterUpdateContacts(CharacterUpdateTestDataMixin, NoSocketsTestCase):
-    def test_update_contact_labels_1(self, mock_esi):
-        """can create new contact labels from scratch"""
-        mock_esi.client = esi_client_stub
-
-        self.character_1001.update_contact_labels()
-        self.assertEqual(self.character_1001.contact_labels.count(), 2)
-
-        label = self.character_1001.contact_labels.get(label_id=1)
-        self.assertEqual(label.name, "friend")
-
-        label = self.character_1001.contact_labels.get(label_id=2)
-        self.assertEqual(label.name, "pirate")
-
-    def test_update_contact_labels_2(self, mock_esi):
-        """can remove obsolete labels"""
-        mock_esi.client = esi_client_stub
-        CharacterContactLabel.objects.create(
-            character=self.character_1001, label_id=99, name="Obsolete"
-        )
-
-        self.character_1001.update_contact_labels()
-        self.assertEqual(
-            {x.label_id for x in self.character_1001.contact_labels.all()}, {1, 2}
-        )
-
-    def test_update_contact_labels_3(self, mock_esi):
-        """can update existing labels"""
-        mock_esi.client = esi_client_stub
-        CharacterContactLabel.objects.create(
-            character=self.character_1001, label_id=1, name="Obsolete"
-        )
-
-        self.character_1001.update_contact_labels()
-        self.assertEqual(
-            {x.label_id for x in self.character_1001.contact_labels.all()}, {1, 2}
-        )
-
-        label = self.character_1001.contact_labels.get(label_id=1)
-        self.assertEqual(label.name, "friend")
-
-    def test_update_contact_labels_4(self, mock_esi):
-        """when data from ESI has not changed, then skip update"""
-        mock_esi.client = esi_client_stub
-
-        self.character_1001.update_contact_labels()
-        label = self.character_1001.contact_labels.get(label_id=1)
-        label.name = "foe"
-        label.save()
-
-        self.character_1001.update_contact_labels()
-
-        self.assertEqual(self.character_1001.contact_labels.count(), 2)
-        label = self.character_1001.contact_labels.get(label_id=1)
-        self.assertEqual(label.name, "foe")
-
-    def test_update_contact_labels_5(self, mock_esi):
-        """when data from ESI has not changed and update is forced, then do update"""
-        mock_esi.client = esi_client_stub
-
-        self.character_1001.update_contact_labels()
-        label = self.character_1001.contact_labels.get(label_id=1)
-        label.name = "foe"
-        label.save()
-
-        self.character_1001.update_contact_labels(force_update=True)
-
-        self.assertEqual(self.character_1001.contact_labels.count(), 2)
-        label = self.character_1001.contact_labels.get(label_id=1)
-        self.assertEqual(label.name, "friend")
-
-    def test_update_contacts_1(self, mock_esi):
-        """can create contacts"""
-        mock_esi.client = esi_client_stub
-        CharacterContactLabel.objects.create(
-            character=self.character_1001, label_id=1, name="friend"
-        )
-        CharacterContactLabel.objects.create(
-            character=self.character_1001, label_id=2, name="pirate"
-        )
-
-        self.character_1001.update_contacts()
-
-        self.assertEqual(self.character_1001.contacts.count(), 2)
-
-        obj = self.character_1001.contacts.get(eve_entity_id=1101)
-        self.assertEqual(obj.eve_entity.category, EveEntity.CATEGORY_CHARACTER)
-        self.assertFalse(obj.is_blocked)
-        self.assertTrue(obj.is_watched)
-        self.assertEqual(obj.standing, -10)
-        self.assertEqual({x.label_id for x in obj.labels.all()}, {2})
-
-        obj = self.character_1001.contacts.get(eve_entity_id=2002)
-        self.assertEqual(obj.eve_entity.category, EveEntity.CATEGORY_CORPORATION)
-        self.assertFalse(obj.is_blocked)
-        self.assertFalse(obj.is_watched)
-        self.assertEqual(obj.standing, 5)
-        self.assertEqual(obj.labels.count(), 0)
-
-    def test_update_contacts_2(self, mock_esi):
-        """can remove obsolete contacts"""
-        mock_esi.client = esi_client_stub
-        CharacterContactLabel.objects.create(
-            character=self.character_1001, label_id=1, name="friend"
-        )
-        CharacterContactLabel.objects.create(
-            character=self.character_1001, label_id=2, name="pirate"
-        )
-        CharacterContact.objects.create(
-            character=self.character_1001,
-            eve_entity=EveEntity.objects.get(id=3101),
-            standing=-5,
-        )
-
-        self.character_1001.update_contacts()
 
-        self.assertEqual(
-            {x.eve_entity_id for x in self.character_1001.contacts.all()}, {1101, 2002}
-        )
-
-    def test_update_contacts_3(self, mock_esi):
-        """can update existing contacts"""
-        mock_esi.client = esi_client_stub
-        CharacterContactLabel.objects.create(
-            character=self.character_1001, label_id=2, name="pirate"
-        )
-        my_label = CharacterContactLabel.objects.create(
-            character=self.character_1001, label_id=1, name="Dummy"
-        )
-        my_contact = CharacterContact.objects.create(
-            character=self.character_1001,
-            eve_entity=EveEntity.objects.get(id=1101),
-            is_blocked=True,
-            is_watched=False,
-            standing=-5,
-        )
-        my_contact.labels.add(my_label)
-
-        self.character_1001.update_contacts()
-
-        obj = self.character_1001.contacts.get(eve_entity_id=1101)
-        self.assertEqual(obj.eve_entity.category, EveEntity.CATEGORY_CHARACTER)
-        self.assertFalse(obj.is_blocked)
-        self.assertTrue(obj.is_watched)
-        self.assertEqual(obj.standing, -10)
-        self.assertEqual({x.label_id for x in obj.labels.all()}, {2})
-
-    def test_update_contacts_4(self, mock_esi):
-        """when ESI data has not changed, then skip update"""
-        mock_esi.client = esi_client_stub
-        CharacterContactLabel.objects.create(
-            character=self.character_1001, label_id=1, name="friend"
-        )
-        CharacterContactLabel.objects.create(
-            character=self.character_1001, label_id=2, name="pirate"
-        )
-
-        self.character_1001.update_contacts()
-        obj = self.character_1001.contacts.get(eve_entity_id=1101)
-        obj.is_watched = False
-        obj.save()
+from ..testdata.esi_client_stub import esi_client_stub, esi_stub
+from ..testdata.factories import (
+    create_character_mail_label,
+    create_mail_entity_from_eve_entity,
+    create_mailing_list,
+)
+from ..testdata.load_entities import load_entities
+from ..testdata.load_eveuniverse import load_eveuniverse
+from ..utils import CharacterUpdateTestDataMixin, create_memberaudit_character
 
-        self.character_1001.update_contacts()
+MODULE_PATH = "memberaudit.managers.character_sections_2"
 
-        obj = self.character_1001.contacts.get(eve_entity_id=1101)
-        self.assertFalse(obj.is_watched)
 
-    def test_update_contacts_5(self, mock_esi):
-        """when ESI data has not changed and update is forced, then update"""
+@patch(MODULE_PATH + ".esi")
+class TestCharacterCorporationHistoryManager(
+    CharacterUpdateTestDataMixin, NoSocketsTestCase
+):
+    def test_can_create_from_scratch(self, mock_esi):
+        # given
         mock_esi.client = esi_client_stub
-        CharacterContactLabel.objects.create(
-            character=self.character_1001, label_id=1, name="friend"
-        )
-        CharacterContactLabel.objects.create(
-            character=self.character_1001, label_id=2, name="pirate"
-        )
-
-        self.character_1001.update_contacts()
-        obj = self.character_1001.contacts.get(eve_entity_id=1101)
-        obj.is_watched = False
-        obj.save()
-
-        self.character_1001.update_contacts(force_update=True)
+        # when
+        CharacterCorporationHistory.objects.update_or_create_esi(self.character_1001)
+        # then
+        self.assertEqual(self.character_1001.corporation_history.count(), 2)
 
-        obj = self.character_1001.contacts.get(eve_entity_id=1101)
-        self.assertTrue(obj.is_watched)
+        obj = self.character_1001.corporation_history.get(record_id=500)
+        self.assertEqual(obj.corporation, self.corporation_2001)
+        self.assertTrue(obj.is_deleted)
+        self.assertEqual(obj.start_date, parse_datetime("2016-06-26T20:00:00Z"))
 
+        obj = self.character_1001.corporation_history.get(record_id=501)
+        self.assertEqual(obj.corporation, self.corporation_2002)
+        self.assertFalse(obj.is_deleted)
+        self.assertEqual(obj.start_date, parse_datetime("2016-07-26T20:00:00Z"))
 
-@override_settings(CELERY_ALWAYS_EAGER=True, CELERY_EAGER_PROPAGATES_EXCEPTIONS=True)
-@patch(MODELS_PATH + ".character.esi")
-class TestCharacterUpdateContracts(CharacterUpdateTestDataMixin, NoSocketsTestCase):
-    @patch(MODELS_PATH + ".character.MEMBERAUDIT_DATA_RETENTION_LIMIT", None)
-    def test_update_contracts_1(self, mock_esi):
-        """can create new courier contract"""
+    def test_can_update_existing_history(self, mock_esi):
+        # given
         mock_esi.client = esi_client_stub
-
-        self.character_1001.update_contract_headers()
-        self.assertSetEqual(
-            set(self.character_1001.contracts.values_list("contract_id", flat=True)),
-            {100000001, 100000002, 100000003},
+        self.character_1001.corporation_history.create(
+            record_id=500, corporation=self.corporation_2002, start_date=now()
         )
+        # when
+        CharacterCorporationHistory.objects.update_or_create_esi(self.character_1001)
+        # then
+        self.assertEqual(self.character_1001.corporation_history.count(), 2)
 
-        obj = self.character_1001.contracts.get(contract_id=100000001)
-        self.assertEqual(obj.contract_type, CharacterContract.TYPE_COURIER)
-        self.assertEqual(obj.acceptor, EveEntity.objects.get(id=1101))
-        self.assertEqual(obj.assignee, EveEntity.objects.get(id=2101))
-        self.assertEqual(obj.availability, CharacterContract.AVAILABILITY_PERSONAL)
-        self.assertIsNone(obj.buyout)
-        self.assertEqual(float(obj.collateral), 550000000.0)
-        self.assertEqual(obj.date_accepted, parse_datetime("2019-10-06T13:15:21Z"))
-        self.assertEqual(obj.date_completed, parse_datetime("2019-10-07T13:15:21Z"))
-        self.assertEqual(obj.date_expired, parse_datetime("2019-10-09T13:15:21Z"))
-        self.assertEqual(obj.date_issued, parse_datetime("2019-10-02T13:15:21Z"))
-        self.assertEqual(obj.days_to_complete, 3)
-        self.assertEqual(obj.end_location, self.structure_1)
-        self.assertFalse(obj.for_corporation)
-        self.assertEqual(obj.issuer_corporation, EveEntity.objects.get(id=2001))
-        self.assertEqual(obj.issuer, EveEntity.objects.get(id=1001))
-        self.assertEqual(float(obj.price), 0.0)
-        self.assertEqual(float(obj.reward), 500000000.0)
-        self.assertEqual(obj.start_location, self.jita_44)
-        self.assertEqual(obj.status, CharacterContract.STATUS_IN_PROGRESS)
-        self.assertEqual(obj.title, "Test 1")
-        self.assertEqual(obj.volume, 486000.0)
-
-    @patch(MODELS_PATH + ".character.MEMBERAUDIT_DATA_RETENTION_LIMIT", None)
-    def test_update_contracts_2(self, mock_esi):
-        """can create new item exchange contract"""
-        mock_esi.client = esi_client_stub
-
-        self.character_1001.update_contract_headers()
-        obj = self.character_1001.contracts.get(contract_id=100000002)
-        self.assertEqual(obj.contract_type, CharacterContract.TYPE_ITEM_EXCHANGE)
-        self.assertEqual(float(obj.price), 270000000.0)
-        self.assertEqual(obj.volume, 486000.0)
-        self.assertEqual(obj.status, CharacterContract.STATUS_FINISHED)
-
-        self.character_1001.update_contract_items(contract=obj)
-
-        self.assertEqual(obj.items.count(), 2)
-
-        item = obj.items.get(record_id=1)
-        self.assertTrue(item.is_included)
-        self.assertFalse(item.is_singleton)
-        self.assertEqual(item.quantity, 3)
-        self.assertEqual(item.eve_type, EveType.objects.get(id=19540))
-
-        item = obj.items.get(record_id=2)
-        self.assertTrue(item.is_included)
-        self.assertFalse(item.is_singleton)
-        self.assertEqual(item.quantity, 5)
-        self.assertEqual(item.raw_quantity, -1)
-        self.assertEqual(item.eve_type, EveType.objects.get(id=19551))
-
-    @patch(MODELS_PATH + ".character.MEMBERAUDIT_DATA_RETENTION_LIMIT", None)
-    def test_update_contracts_3(self, mock_esi):
-        """can create new auction contract"""
-        mock_esi.client = esi_client_stub
-
-        self.character_1001.update_contract_headers()
-        obj = self.character_1001.contracts.get(contract_id=100000003)
-        self.assertEqual(obj.contract_type, CharacterContract.TYPE_AUCTION)
-        self.assertEqual(float(obj.buyout), 200_000_000.0)
-        self.assertEqual(float(obj.price), 20_000_000.0)
-        self.assertEqual(obj.volume, 400.0)
-        self.assertEqual(obj.status, CharacterContract.STATUS_OUTSTANDING)
-
-        self.character_1001.update_contract_items(contract=obj)
-
-        self.assertEqual(obj.items.count(), 1)
-        item = obj.items.get(record_id=1)
-        self.assertTrue(item.is_included)
-        self.assertFalse(item.is_singleton)
-        self.assertEqual(item.quantity, 3)
-        self.assertEqual(item.eve_type, EveType.objects.get(id=19540))
-
-        self.character_1001.update_contract_bids(contract=obj)
-
-        self.assertEqual(obj.bids.count(), 1)
-        bid = obj.bids.get(bid_id=1)
-        self.assertEqual(float(bid.amount), 1_000_000.23)
-        self.assertEqual(bid.date_bid, parse_datetime("2017-01-01T10:10:10Z"))
-        self.assertEqual(bid.bidder, EveEntity.objects.get(id=1101))
-
-    @patch(MODELS_PATH + ".character.MEMBERAUDIT_DATA_RETENTION_LIMIT", None)
-    def test_update_contracts_4(self, mock_esi):
-        """old contracts must be kept"""
-        mock_esi.client = esi_client_stub
-
-        CharacterContract.objects.create(
-            character=self.character_1001,
-            contract_id=190000001,
-            availability=CharacterContract.AVAILABILITY_PERSONAL,
-            contract_type=CharacterContract.TYPE_COURIER,
-            assignee=EveEntity.objects.get(id=1002),
-            date_issued=now() - dt.timedelta(days=60),
-            date_expired=now() - dt.timedelta(days=30),
-            for_corporation=False,
-            issuer=EveEntity.objects.get(id=1001),
-            issuer_corporation=EveEntity.objects.get(id=2001),
-            status=CharacterContract.STATUS_IN_PROGRESS,
-            start_location=self.jita_44,
-            end_location=self.structure_1,
-            title="Old contract",
-        )
-
-        self.character_1001.update_contract_headers()
-        self.assertEqual(self.character_1001.contracts.count(), 4)
-
-    @patch(MODELS_PATH + ".character.MEMBERAUDIT_DATA_RETENTION_LIMIT", None)
-    def test_update_contracts_5(self, mock_esi):
-        """Existing contracts are updated"""
-        mock_esi.client = esi_client_stub
+        obj = self.character_1001.corporation_history.get(record_id=500)
+        self.assertEqual(obj.corporation, self.corporation_2001)
+        self.assertTrue(obj.is_deleted)
+        self.assertEqual(obj.start_date, parse_datetime("2016-06-26T20:00:00Z"))
 
-        CharacterContract.objects.create(
-            character=self.character_1001,
-            contract_id=100000001,
-            availability=CharacterContract.AVAILABILITY_PERSONAL,
-            contract_type=CharacterContract.TYPE_COURIER,
-            assignee=EveEntity.objects.get(id=2101),
-            date_issued=parse_datetime("2019-10-02T13:15:21Z"),
-            date_expired=parse_datetime("2019-10-09T13:15:21Z"),
-            for_corporation=False,
-            issuer=EveEntity.objects.get(id=1001),
-            issuer_corporation=EveEntity.objects.get(id=2001),
-            status=CharacterContract.STATUS_OUTSTANDING,
-            start_location=self.jita_44,
-            end_location=self.structure_1,
-            title="Test 1",
-            collateral=550000000,
-            reward=500000000,
-            volume=486000,
-            days_to_complete=3,
-        )
-
-        self.character_1001.update_contract_headers()
-
-        obj = self.character_1001.contracts.get(contract_id=100000001)
-        self.assertEqual(obj.contract_type, CharacterContract.TYPE_COURIER)
-        self.assertEqual(obj.acceptor, EveEntity.objects.get(id=1101))
-        self.assertEqual(obj.assignee, EveEntity.objects.get(id=2101))
-        self.assertEqual(obj.availability, CharacterContract.AVAILABILITY_PERSONAL)
-        self.assertIsNone(obj.buyout)
-        self.assertEqual(float(obj.collateral), 550000000.0)
-        self.assertEqual(obj.date_accepted, parse_datetime("2019-10-06T13:15:21Z"))
-        self.assertEqual(obj.date_completed, parse_datetime("2019-10-07T13:15:21Z"))
-        self.assertEqual(obj.date_expired, parse_datetime("2019-10-09T13:15:21Z"))
-        self.assertEqual(obj.date_issued, parse_datetime("2019-10-02T13:15:21Z"))
-        self.assertEqual(obj.days_to_complete, 3)
-        self.assertEqual(obj.end_location, self.structure_1)
-        self.assertFalse(obj.for_corporation)
-        self.assertEqual(obj.issuer_corporation, EveEntity.objects.get(id=2001))
-        self.assertEqual(obj.issuer, EveEntity.objects.get(id=1001))
-        self.assertEqual(float(obj.reward), 500000000.0)
-        self.assertEqual(obj.start_location, self.jita_44)
-        self.assertEqual(obj.status, CharacterContract.STATUS_IN_PROGRESS)
-        self.assertEqual(obj.title, "Test 1")
-        self.assertEqual(obj.volume, 486000.0)
-
-    @patch(MODELS_PATH + ".character.MEMBERAUDIT_DATA_RETENTION_LIMIT", None)
-    def test_update_contracts_6(self, mock_esi):
-        """can add new bids to auction contract"""
+    def test_should_skip_update_when_data_on_ESI_has_not_changed(self, mock_esi):
+        # given
         mock_esi.client = esi_client_stub
-        contract = CharacterContract.objects.create(
-            character=self.character_1001,
-            contract_id=100000003,
-            availability=CharacterContract.AVAILABILITY_PERSONAL,
-            contract_type=CharacterContract.TYPE_AUCTION,
-            assignee=EveEntity.objects.get(id=2101),
-            date_issued=parse_datetime("2019-10-02T13:15:21Z"),
-            date_expired=parse_datetime("2019-10-09T13:15:21Z"),
-            for_corporation=False,
-            issuer=EveEntity.objects.get(id=1001),
-            issuer_corporation=EveEntity.objects.get(id=2001),
-            status=CharacterContract.STATUS_OUTSTANDING,
-            start_location=self.jita_44,
-            end_location=self.jita_44,
-            buyout=200_000_000,
-            price=20_000_000,
-            volume=400,
-        )
-        CharacterContractBid.objects.create(
-            contract=contract,
-            bid_id=2,
-            amount=21_000_000,
-            bidder=EveEntity.objects.get(id=1003),
-            date_bid=now(),
-        )
-
-        self.character_1001.update_contract_headers()
-        obj = self.character_1001.contracts.get(contract_id=100000003)
-        self.character_1001.update_contract_bids(contract=obj)
-
-        self.assertEqual(obj.bids.count(), 2)
-
-        bid = obj.bids.get(bid_id=1)
-        self.assertEqual(float(bid.amount), 1_000_000.23)
-        self.assertEqual(bid.date_bid, parse_datetime("2017-01-01T10:10:10Z"))
-        self.assertEqual(bid.bidder, EveEntity.objects.get(id=1101))
-
-        bid = obj.bids.get(bid_id=2)
-        self.assertEqual(float(bid.amount), 21_000_000)
-
-    @patch(MODELS_PATH + ".character.MEMBERAUDIT_DATA_RETENTION_LIMIT", None)
-    def test_update_contracts_7(self, mock_esi):
-        """when contract list from ESI has not changed, then skip update"""
-        mock_esi.client = esi_client_stub
-
-        self.character_1001.update_contract_headers()
-        obj = self.character_1001.contracts.get(contract_id=100000001)
-        obj.status = CharacterContract.STATUS_FINISHED
+        self.character_1001.update_corporation_history()
+        obj = self.character_1001.corporation_history.get(record_id=500)
+        obj.corporation = self.corporation_2002
         obj.save()
+        # when
+        CharacterCorporationHistory.objects.update_or_create_esi(self.character_1001)
+        # then
+        obj = self.character_1001.corporation_history.get(record_id=500)
+        self.assertEqual(obj.corporation, self.corporation_2002)
 
-        self.character_1001.update_contract_headers()
-
-        obj = self.character_1001.contracts.get(contract_id=100000001)
-        self.assertEqual(obj.status, CharacterContract.STATUS_FINISHED)
-
-    @patch(MODELS_PATH + ".character.MEMBERAUDIT_DATA_RETENTION_LIMIT", None)
-    def test_update_contracts_8(self, mock_esi):
-        """
-        when contract list from ESI has not changed and update is forced, then update
-        """
+    def test_should_update_always_when_forced(self, mock_esi):
+        # given
         mock_esi.client = esi_client_stub
-
-        self.character_1001.update_contract_headers()
-        obj = self.character_1001.contracts.get(contract_id=100000001)
-        obj.status = CharacterContract.STATUS_FINISHED
+        self.character_1001.update_corporation_history()
+        obj = self.character_1001.corporation_history.get(record_id=500)
+        obj.corporation = self.corporation_2002
         obj.save()
-
-        self.character_1001.update_contract_headers(force_update=True)
-
-        obj = self.character_1001.contracts.get(contract_id=100000001)
-        self.assertEqual(obj.status, CharacterContract.STATUS_IN_PROGRESS)
-
-    @patch(MODELS_PATH + ".character.MEMBERAUDIT_DATA_RETENTION_LIMIT", 10)
-    def test_update_contracts_9(self, mock_esi):
-        """when retention limit is set, then only create contracts younger than limit"""
-        mock_esi.client = esi_client_stub
-
-        with patch(MODELS_PATH + ".character.now") as mock_now:
-            mock_now.return_value = dt.datetime(2019, 10, 21, 1, 15, tzinfo=utc)
-            self.character_1001.update_contract_headers()
-
-        self.assertSetEqual(
-            set(self.character_1001.contracts.values_list("contract_id", flat=True)),
-            {100000002, 100000003},
+        # when
+        CharacterCorporationHistory.objects.update_or_create_esi(
+            self.character_1001, force_update=True
         )
+        # then
+        obj = self.character_1001.corporation_history.get(record_id=500)
+        self.assertEqual(obj.corporation, self.corporation_2001)
 
-    @patch(MODELS_PATH + ".character.MEMBERAUDIT_DATA_RETENTION_LIMIT", 15)
-    def test_update_contracts_10(self, mock_esi):
-        """when retention limit is set,
-        then remove existing contracts older than limit
-        """
+    def test_should_handle_empty_response(self, mock_esi):
+        # given
         mock_esi.client = esi_client_stub
-        CharacterContract.objects.create(
-            character=self.character_1001,
-            contract_id=100000004,
-            availability=CharacterContract.AVAILABILITY_PERSONAL,
-            contract_type=CharacterContract.TYPE_COURIER,
-            assignee=EveEntity.objects.get(id=2101),
-            date_issued=parse_datetime("2019-09-02T13:15:21Z"),
-            date_expired=parse_datetime("2019-09-09T13:15:21Z"),
-            for_corporation=False,
-            issuer=EveEntity.objects.get(id=1001),
-            issuer_corporation=EveEntity.objects.get(id=2001),
-            status=CharacterContract.STATUS_OUTSTANDING,
-            start_location=self.jita_44,
-            end_location=self.structure_1,
-            title="This contract is too old",
-            collateral=550000000,
-            reward=500000000,
-            volume=486000,
-            days_to_complete=3,
-        )
-
-        with patch(MODELS_PATH + ".character.now") as mock_now:
-            mock_now.return_value = dt.datetime(2019, 10, 21, 1, 15, tzinfo=utc)
-            self.character_1001.update_contract_headers()
-
-        self.assertSetEqual(
-            set(self.character_1001.contracts.values_list("contract_id", flat=True)),
-            {100000001, 100000002, 100000003},
-        )
+        # when
+        CharacterCorporationHistory.objects.update_or_create_esi(self.character_1002)
+        # then
+        self.assertEqual(self.character_1001.corporation_history.count(), 0)
 
 
-@patch(MANAGERS_PATH + ".sections.eve_xml_to_html")
-@patch(MODELS_PATH + ".character.esi")
-class TestCharacterUpdateCharacterDetails(
-    CharacterUpdateTestDataMixin, NoSocketsTestCase
-):
+@patch(MODULE_PATH + ".eve_xml_to_html")
+@patch(MODULE_PATH + ".esi")
+class TestCharacterDetailManager(CharacterUpdateTestDataMixin, NoSocketsTestCase):
     def test_can_create_from_scratch(self, mock_esi, mock_eve_xml_to_html):
         # given
         mock_esi.client = esi_client_stub
         mock_eve_xml_to_html.side_effect = lambda x: eve_xml_to_html(x)
         # when
-        self.character_1001.update_character_details()
+        CharacterDetails.objects.update_or_create_esi(self.character_1001)
         # then
         self.assertEqual(self.character_1001.details.eve_ancestry.id, 11)
         self.assertEqual(
             self.character_1001.details.birthday, parse_datetime("2015-03-24T11:37:00Z")
         )
         self.assertEqual(self.character_1001.details.eve_bloodline_id, 1)
         self.assertEqual(self.character_1001.details.corporation, self.corporation_2001)
@@ -668,87 +259,166 @@
     #     self.assertEqual(self.character_1001.details.eve_race.id, 1)
     #     self.assertEqual(
     #         self.character_1001.details.title, "All round pretty awesome guy"
     #     )
     #     self.assertTrue(mock_eve_xml_to_html.called)
 
 
-@patch(MODELS_PATH + ".character.esi")
-class TestCharacterUpdateCorporationHistory(
-    CharacterUpdateTestDataMixin, NoSocketsTestCase
-):
-    def test_create(self, mock_esi):
-        """can create corporation history from scratch"""
-        mock_esi.client = esi_client_stub
-        self.character_1001.update_corporation_history()
-        self.assertEqual(self.character_1001.corporation_history.count(), 2)
-
-        obj = self.character_1001.corporation_history.get(record_id=500)
-        self.assertEqual(obj.corporation, self.corporation_2001)
-        self.assertTrue(obj.is_deleted)
-        self.assertEqual(obj.start_date, parse_datetime("2016-06-26T20:00:00Z"))
+@patch(MODULE_PATH + ".esi")
+class TestCharacterFwStatsManager(NoSocketsTestCase):
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+        load_eveuniverse()
+        load_entities()
+        cls.character_1001 = create_memberaudit_character(1001)
+        cls.endpoints = [
+            EsiEndpoint(
+                "Faction_Warfare",
+                "get_characters_character_id_fw_stats",
+                "character_id",
+                needs_token=True,
+                data={
+                    "1001": {
+                        "current_rank": 3,
+                        "enlisted_on": dt.datetime(
+                            2023, 3, 21, 15, 0, tzinfo=dt.timezone.utc
+                        ),
+                        "faction_id": 500001,
+                        "highest_rank": 4,
+                        "kills": {
+                            "last_week": 893,
+                            "total": 684350,
+                            "yesterday": 136,
+                        },
+                        "victory_points": {
+                            "last_week": 102640,
+                            "total": 52658260,
+                            "yesterday": 15980,
+                        },
+                    }
+                },
+            ),
+        ]
+        cls.esi_client_stub = EsiClientStub.create_from_endpoints(cls.endpoints)
 
-        obj = self.character_1001.corporation_history.get(record_id=501)
-        self.assertEqual(obj.corporation, self.corporation_2002)
-        self.assertFalse(obj.is_deleted)
-        self.assertEqual(obj.start_date, parse_datetime("2016-07-26T20:00:00Z"))
-
-    def test_update_1(self, mock_esi):
-        """can update existing corporation history"""
-        mock_esi.client = esi_client_stub
-        self.character_1001.corporation_history.create(
-            record_id=500, corporation=self.corporation_2002, start_date=now()
+    def test_should_add_new_entry_from_scratch(self, mock_esi):
+        # given
+        mock_esi.client = self.esi_client_stub
+        # when
+        with patch(MODULE_PATH + ".data_retention_cutoff", lambda: None):
+            CharacterFwStats.objects.update_or_create_esi(self.character_1001)
+        # then
+        obj: CharacterFwStats = self.character_1001.fw_stats
+        self.assertEqual(obj.current_rank, 3)
+        self.assertEqual(
+            obj.enlisted_on,
+            dt.datetime(2023, 3, 21, 15, 0, tzinfo=dt.timezone.utc),
         )
+        self.assertEqual(obj.faction_id, 500001)
+        self.assertEqual(obj.highest_rank, 4)
+        self.assertEqual(obj.kills_last_week, 893)
+        self.assertEqual(obj.kills_total, 684350)
+        self.assertEqual(obj.kills_yesterday, 136)
+        self.assertEqual(obj.victory_points_last_week, 102640)
+        self.assertEqual(obj.victory_points_total, 52658260)
+        self.assertEqual(obj.victory_points_yesterday, 15980)
 
-        self.character_1001.update_corporation_history()
-        self.assertEqual(self.character_1001.corporation_history.count(), 2)
-
-        obj = self.character_1001.corporation_history.get(record_id=500)
-        self.assertEqual(obj.corporation, self.corporation_2001)
-        self.assertTrue(obj.is_deleted)
-        self.assertEqual(obj.start_date, parse_datetime("2016-06-26T20:00:00Z"))
-
-    def test_update_2(self, mock_esi):
-        """when data from ESI has not changed, then skip update"""
-        mock_esi.client = esi_client_stub
-
-        self.character_1001.update_corporation_history()
-        obj = self.character_1001.corporation_history.get(record_id=500)
-        obj.corporation = self.corporation_2002
-        obj.save()
-
-        self.character_1001.update_corporation_history()
-        obj = self.character_1001.corporation_history.get(record_id=500)
-        self.assertEqual(obj.corporation, self.corporation_2002)
-
-    def test_update_3(self, mock_esi):
-        """when data from ESI has not changed and update is forced, then do update"""
-        mock_esi.client = esi_client_stub
-
-        self.character_1001.update_corporation_history()
-        obj = self.character_1001.corporation_history.get(record_id=500)
-        obj.corporation = self.corporation_2002
-        obj.save()
-
-        self.character_1001.update_corporation_history(force_update=True)
-
-        obj = self.character_1001.corporation_history.get(record_id=500)
-        self.assertEqual(obj.corporation, self.corporation_2001)
+    def test_should_update_existing_entries(self, mock_esi):
+        # given
+        mock_esi.client = self.esi_client_stub
+        CharacterFwStats.objects.create(
+            character=self.character_1001,
+            kills_last_week=0,
+            kills_total=0,
+            kills_yesterday=0,
+            victory_points_last_week=0,
+            victory_points_total=0,
+            victory_points_yesterday=0,
+        )
+        # when
+        with patch(MODULE_PATH + ".data_retention_cutoff", lambda: None):
+            CharacterFwStats.objects.update_or_create_esi(self.character_1001)
+        # then
+        self.character_1001.refresh_from_db()
+        obj: CharacterFwStats = self.character_1001.fw_stats
+        self.assertEqual(obj.current_rank, 3)
+        self.assertEqual(
+            obj.enlisted_on,
+            dt.datetime(2023, 3, 21, 15, 0, tzinfo=dt.timezone.utc),
+        )
+        self.assertEqual(obj.faction_id, 500001)
+        self.assertEqual(obj.highest_rank, 4)
+        self.assertEqual(obj.kills_last_week, 893)
+        self.assertEqual(obj.kills_total, 684350)
+        self.assertEqual(obj.kills_yesterday, 136)
+        self.assertEqual(obj.victory_points_last_week, 102640)
+        self.assertEqual(obj.victory_points_total, 52658260)
+        self.assertEqual(obj.victory_points_yesterday, 15980)
 
-    def test_should_handle_empty_response(self, mock_esi):
+    def test_should_add_new_entry_from_scratch_for_unlisted(self, mock_esi):
         # given
-        mock_esi.client = esi_client_stub
+        endpoints = [
+            EsiEndpoint(
+                "Faction_Warfare",
+                "get_characters_character_id_fw_stats",
+                "character_id",
+                needs_token=True,
+                data={
+                    "1001": {
+                        "kills": {
+                            "last_week": 0,
+                            "total": 684350,
+                            "yesterday": 0,
+                        },
+                        "victory_points": {
+                            "last_week": 0,
+                            "total": 52658260,
+                            "yesterday": 0,
+                        },
+                    }
+                },
+            ),
+        ]
+        mock_esi.client = EsiClientStub.create_from_endpoints(endpoints)
         # when
-        self.character_1002.update_corporation_history()
+        with patch(MODULE_PATH + ".data_retention_cutoff", lambda: None):
+            CharacterFwStats.objects.update_or_create_esi(self.character_1001)
         # then
-        self.assertEqual(self.character_1001.corporation_history.count(), 0)
+        obj: CharacterFwStats = self.character_1001.fw_stats
+        self.assertIsNone(obj.current_rank)
+        self.assertIsNone(obj.enlisted_on)
+        self.assertIsNone(obj.faction)
+        self.assertIsNone(obj.highest_rank)
+        self.assertEqual(obj.kills_last_week, 0)
+        self.assertEqual(obj.kills_total, 684350)
+        self.assertEqual(obj.kills_yesterday, 0)
+        self.assertEqual(obj.victory_points_last_week, 0)
+        self.assertEqual(obj.victory_points_total, 52658260)
+        self.assertEqual(obj.victory_points_yesterday, 0)
+
+    # FIXME: Test stopped working after moving it over
+    # @patch(MODULE_PATH + ".CharacterFwStats.objects.update_for_character")
+    # def test_should_not_update_when_not_changed(
+    #     self, mock_update_for_character, mock_esi
+    # ):
+    #     # given
+    #     mock_esi.client = self.esi_client_stub
+    #     # when
+    #     with patch(
+    #         MODULE_PATH + ".Character.has_section_changed"
+    #     ) as mock_has_section_changed:
+    #         mock_has_section_changed.return_value = False
+    #         CharacterFwStats.objects.update_or_create_esi(self.character_1001)
+    #     # then
+    #     self.assertFalse(mock_update_for_character.called)
 
 
-@patch(MODELS_PATH + ".character.esi")
-class TestCharacterUpdateImplants(CharacterUpdateTestDataMixin, NoSocketsTestCase):
+@patch(MODULE_PATH + ".esi")
+class TestCharacterImplantManager(CharacterUpdateTestDataMixin, NoSocketsTestCase):
     def test_update_implants_1(self, mock_esi):
         """can create implants from scratch"""
         mock_esi.client = esi_client_stub
 
         self.character_1001.update_implants()
         self.assertEqual(self.character_1001.implants.count(), 3)
         self.assertSetEqual(
@@ -783,61 +453,464 @@
         self.character_1001.implants.get(eve_type_id=19540).delete()
 
         self.character_1001.update_implants(force_update=True)
         self.assertTrue(self.character_1001.implants.filter(eve_type_id=19540).exists())
 
 
 @override_settings(CELERY_ALWAYS_EAGER=True, CELERY_EAGER_PROPAGATES_EXCEPTIONS=True)
-@patch(MODELS_PATH + ".character.esi")
-class TestCharacterUpdateJumpClones(CharacterUpdateTestDataMixin, NoSocketsTestCase):
-    def test_update_jump_clones_1(self, mock_esi):
-        """can update jump clones with implants"""
+@patch(MODULE_PATH + ".esi")
+class TestCharacterJumpClonesManager(CharacterUpdateTestDataMixin, NoSocketsTestCase):
+    def test_can_update_with_implants(self, mock_esi):
+        # given
         mock_esi.client = esi_client_stub
-
-        self.character_1001.update_jump_clones()
+        # when
+        CharacterJumpClone.objects.update_or_create_esi(self.character_1001)
+        # then
         self.assertEqual(self.character_1001.jump_clones.count(), 1)
-
         obj = self.character_1001.jump_clones.get(jump_clone_id=12345)
         self.assertEqual(obj.location, self.jita_44)
         self.assertEqual(
             {x for x in obj.implants.values_list("eve_type", flat=True)},
             {19540, 19551, 19553},
         )
 
-    def test_update_jump_clones_2(self, mock_esi):
-        """can update jump clones without implants"""
+    def test_can_update_without_implants(self, mock_esi):
+        # given
         mock_esi.client = esi_client_stub
-
-        self.character_1002.update_jump_clones()
+        # when
+        CharacterJumpClone.objects.update_or_create_esi(self.character_1002)
+        # then
         self.assertEqual(self.character_1002.jump_clones.count(), 1)
-
         obj = self.character_1002.jump_clones.get(jump_clone_id=12345)
         self.assertEqual(obj.location, self.jita_44)
         self.assertEqual(obj.implants.count(), 0)
 
-    def test_skip_update_1(self, mock_esi):
-        """when ESI data has not changed, then skip update"""
+    def test_skip_update_when_no_new_data(self, mock_esi):
+        # given
         mock_esi.client = esi_client_stub
-
-        self.character_1001.update_jump_clones()
+        CharacterJumpClone.objects.update_or_create_esi(self.character_1001)
         obj = self.character_1001.jump_clones.get(jump_clone_id=12345)
         obj.location = self.structure_1
         obj.save()
-
-        self.character_1001.update_jump_clones()
-
+        # when
+        CharacterJumpClone.objects.update_or_create_esi(self.character_1001)
+        # then
         obj = self.character_1001.jump_clones.get(jump_clone_id=12345)
         self.assertEqual(obj.location, self.structure_1)
 
-    def test_skip_update_2(self, mock_esi):
-        """when ESI data has not changed and update is forced, then do update"""
+    def test_update_always_when_forced(self, mock_esi):
+        # given
         mock_esi.client = esi_client_stub
-
-        self.character_1001.update_jump_clones()
+        CharacterJumpClone.objects.update_or_create_esi(self.character_1001)
         obj = self.character_1001.jump_clones.get(jump_clone_id=12345)
         obj.location = self.structure_1
         obj.save()
-
-        self.character_1001.update_jump_clones(force_update=True)
-
+        # when
+        CharacterJumpClone.objects.update_or_create_esi(
+            self.character_1001, force_update=True
+        )
+        # then
         obj = self.character_1001.jump_clones.get(jump_clone_id=12345)
         self.assertEqual(obj.location, self.jita_44)
+
+
+@override_settings(CELERY_ALWAYS_EAGER=True, CELERY_EAGER_PROPAGATES_EXCEPTIONS=True)
+@patch(MODULE_PATH + ".esi")
+class TestCharacterLocationManager(CharacterUpdateTestDataMixin, NoSocketsTestCase):
+    def test_update_location_1(self, mock_esi):
+        # given
+        mock_esi.client = esi_client_stub
+        # when
+        CharacterLocation.objects.update_or_create_esi(self.character_1001)
+        # then
+        self.assertEqual(self.character_1001.location.eve_solar_system, self.jita)
+        self.assertEqual(self.character_1001.location.location, self.jita_44)
+
+    def test_update_location_2(self, mock_esi):
+        # given
+        mock_esi.client = esi_client_stub
+        # when
+        CharacterLocation.objects.update_or_create_esi(self.character_1002)
+        # then
+        self.assertEqual(self.character_1002.location.eve_solar_system, self.amamake)
+        self.assertEqual(self.character_1002.location.location, self.structure_1)
+
+    # TODO: Add tests for no change and forced update
+
+
+@patch(MODULE_PATH + ".esi")
+class TestCharacterLoyaltyManager(CharacterUpdateTestDataMixin, NoSocketsTestCase):
+    def test_can_create_from_scratch(self, mock_esi):
+        # given
+        mock_esi.client = esi_client_stub
+        # when
+        CharacterLoyaltyEntry.objects.update_or_create_esi(self.character_1001)
+        # then
+        self.assertEqual(self.character_1001.loyalty_entries.count(), 1)
+        obj = self.character_1001.loyalty_entries.get(corporation_id=2002)
+        self.assertEqual(obj.loyalty_points, 100)
+
+    def test_can_update_existing_entries(self, mock_esi):
+        # given
+        mock_esi.client = esi_client_stub
+        self.character_1001.loyalty_entries.create(
+            corporation=self.corporation_2001, loyalty_points=200
+        )
+        # when
+        CharacterLoyaltyEntry.objects.update_or_create_esi(self.character_1001)
+        # then
+        self.assertEqual(self.character_1001.loyalty_entries.count(), 1)
+        obj = self.character_1001.loyalty_entries.get(corporation=self.corporation_2002)
+        self.assertEqual(obj.loyalty_points, 100)
+
+    def test_should_skip_update_when_no_change(self, mock_esi):
+        # given
+        mock_esi.client = esi_client_stub
+        CharacterLoyaltyEntry.objects.update_or_create_esi(self.character_1001)
+        obj = self.character_1001.loyalty_entries.get(corporation=self.corporation_2002)
+        obj.loyalty_points = 200
+        obj.save()
+        # when
+        CharacterLoyaltyEntry.objects.update_or_create_esi(self.character_1001)
+        # then
+        obj = self.character_1001.loyalty_entries.get(corporation=self.corporation_2002)
+        self.assertEqual(obj.loyalty_points, 200)
+
+    def test_should_always_update_when_forced(self, mock_esi):
+        # given
+        mock_esi.client = esi_client_stub
+        CharacterLoyaltyEntry.objects.update_or_create_esi(self.character_1001)
+        obj = self.character_1001.loyalty_entries.get(corporation=self.corporation_2002)
+        obj.loyalty_points = 200
+        obj.save()
+        # when
+        CharacterLoyaltyEntry.objects.update_or_create_esi(
+            self.character_1001, force_update=True
+        )
+        # then
+        obj = self.character_1001.loyalty_entries.get(corporation=self.corporation_2002)
+        self.assertEqual(obj.loyalty_points, 100)
+
+    def test_should_thread_http_500_as_empty_loyalty_list(self, mock_esi):
+        # given
+        exception = build_http_error(
+            500, '{"error":"Unhandled internal error encountered!"}'
+        )
+        mock_esi.client.Loyalty.get_characters_character_id_loyalty_points.side_effect = (
+            exception
+        )
+        self.character_1001.loyalty_entries.create(
+            corporation=self.corporation_2001, loyalty_points=100
+        )
+        # when
+        CharacterLoyaltyEntry.objects.update_or_create_esi(self.character_1001)
+        # then
+        self.assertEqual(self.character_1001.loyalty_entries.count(), 1)
+        obj = self.character_1001.loyalty_entries.get(corporation=self.corporation_2001)
+        self.assertEqual(obj.loyalty_points, 100)
+
+
+@override_settings(CELERY_ALWAYS_EAGER=True, CELERY_EAGER_PROPAGATES_EXCEPTIONS=True)
+@patch(MODULE_PATH + ".esi")
+class TestCharacterMailManager(CharacterUpdateTestDataMixin, NoSocketsTestCase):
+    @patch(MODULE_PATH + ".data_retention_cutoff", lambda: None)
+    def test_can_create_new_mail_from_scratch(self, mock_esi):
+        # given
+        mock_esi.client = esi_client_stub
+        create_mail_entity_from_eve_entity(1002)
+        create_mailing_list(id=9001)
+        create_character_mail_label(character=self.character_1001, label_id=3)
+        # when
+        self.character_1001.update_mail_headers()
+        # then
+        self.assertSetEqual(
+            set(self.character_1001.mails.values_list("mail_id", flat=True)),
+            {1, 2, 3},
+        )
+        obj = self.character_1001.mails.get(mail_id=1)
+        self.assertEqual(obj.sender.id, 1002)
+        self.assertTrue(obj.is_read)
+        self.assertEqual(obj.subject, "Mail 1")
+        self.assertEqual(obj.timestamp, parse_datetime("2015-09-05T16:07:00Z"))
+        self.assertFalse(obj.body)
+        self.assertTrue(obj.recipients.filter(id=1001).exists())
+        self.assertTrue(obj.recipients.filter(id=9001).exists())
+        self.assertSetEqual(set(obj.labels.values_list("label_id", flat=True)), {3})
+
+        obj = self.character_1001.mails.get(mail_id=2)
+        self.assertEqual(obj.sender_id, 9001)
+        self.assertFalse(obj.is_read)
+        self.assertEqual(obj.subject, "Mail 2")
+        self.assertEqual(obj.timestamp, parse_datetime("2015-09-10T18:07:00Z"))
+        self.assertFalse(obj.body)
+        self.assertSetEqual(set(obj.labels.values_list("label_id", flat=True)), {3})
+
+        obj = self.character_1001.mails.get(mail_id=3)
+        self.assertEqual(obj.sender_id, 1002)
+        self.assertTrue(obj.recipients.filter(id=9003).exists())
+        self.assertEqual(obj.timestamp, parse_datetime("2015-09-20T12:07:00Z"))
+
+    @patch(MODULE_PATH + ".data_retention_cutoff", lambda: None)
+    def test_should_skip_update_when_no_change(self, mock_esi):
+        # given
+        mock_esi.client = esi_client_stub
+        create_mail_entity_from_eve_entity(1002)
+        create_mailing_list(id=9001)
+        create_character_mail_label(character=self.character_1001, label_id=3)
+        self.character_1001.update_mail_headers()
+        obj = self.character_1001.mails.get(mail_id=1)
+        obj.is_read = False
+        obj.save()
+        # when
+        self.character_1001.update_mail_headers()
+        # then
+        obj = self.character_1001.mails.get(mail_id=1)
+        self.assertFalse(obj.is_read)
+
+    @patch(MODULE_PATH + ".data_retention_cutoff", lambda: None)
+    def test_should_always_update_when_forced(self, mock_esi):
+        # given
+        mock_esi.client = esi_client_stub
+        create_mail_entity_from_eve_entity(1002)
+        create_mailing_list(id=9001)
+        create_character_mail_label(character=self.character_1001, label_id=3)
+        self.character_1001.update_mail_headers()
+        obj = self.character_1001.mails.get(mail_id=1)
+        obj.is_read = False
+        obj.save()
+        # when
+        self.character_1001.update_mail_headers(force_update=True)
+        # then
+        obj = self.character_1001.mails.get(mail_id=1)
+        self.assertTrue(obj.is_read)
+
+    @patch(
+        MODULE_PATH + ".data_retention_cutoff",
+        lambda: dt.datetime(2015, 9, 20, 20, 5, tzinfo=dt.timezone.utc)
+        - dt.timedelta(days=15),
+    )
+    def test_update_mail_headers_6(self, mock_esi):
+        """when data retention limit is set, then only fetch mails within that limit"""
+        mock_esi.client = esi_client_stub
+        create_mail_entity_from_eve_entity(1002)
+        create_mailing_list(id=9001)
+        create_character_mail_label(character=self.character_1001, label_id=3)
+
+        self.character_1001.update_mail_headers()
+
+        self.assertSetEqual(
+            set(self.character_1001.mails.values_list("mail_id", flat=True)),
+            {2, 3},
+        )
+
+    @patch(
+        MODULE_PATH + ".data_retention_cutoff",
+        lambda: dt.datetime(2015, 9, 20, 20, 5, tzinfo=dt.timezone.utc)
+        - dt.timedelta(days=15),
+    )
+    def test_update_mail_headers_7(self, mock_esi):
+        """when data retention limit is set, then remove old data beyond that limit"""
+        mock_esi.client = esi_client_stub
+        sender, _ = MailEntity.objects.update_or_create_from_eve_entity_id(id=1002)
+        CharacterMail.objects.create(
+            character=self.character_1001,
+            mail_id=99,
+            sender=sender,
+            subject="Mail Old",
+            timestamp=parse_datetime("2015-09-02T14:02:00Z"),
+            is_read=False,
+        )
+
+        create_mail_entity_from_eve_entity(1002)
+        create_mailing_list(id=9001)
+        create_character_mail_label(character=self.character_1001, label_id=3)
+
+        self.character_1001.update_mail_headers()
+
+        self.assertSetEqual(
+            set(self.character_1001.mails.values_list("mail_id", flat=True)),
+            {2, 3},
+        )
+
+    def test_should_update_existing_mail_body(self, mock_esi):
+        # given
+        mock_esi.client = esi_client_stub
+        sender = create_mail_entity_from_eve_entity(1002)
+        mail = CharacterMail.objects.create(
+            character=self.character_1001,
+            mail_id=1,
+            sender=sender,
+            subject="Mail 1",
+            body="Update me",
+            is_read=False,
+            timestamp=parse_datetime("2015-09-30T16:07:00Z"),
+        )
+        recipient_1001 = create_mail_entity_from_eve_entity(1001)
+        recipient_9001 = create_mailing_list(
+            id=9001, category=MailEntity.Category.MAILING_LIST, name="Dummy 2"
+        )
+        mail.recipients.add(recipient_1001, recipient_9001)
+        # when
+        self.character_1001.update_mail_body(mail)
+        # then
+        obj = self.character_1001.mails.get(mail_id=1)
+        self.assertEqual(obj.body, "blah blah blah 😓")
+
+    @patch(MODULE_PATH + ".eve_xml_to_html")
+    def test_should_update_mail_body_from_scratch(self, mock_eve_xml_to_html, mock_esi):
+        # given
+        mock_esi.client = esi_client_stub
+        mock_eve_xml_to_html.side_effect = lambda x: eve_xml_to_html(x)
+        sender = create_mail_entity_from_eve_entity(1002)
+        mail = CharacterMail.objects.create(
+            character=self.character_1001,
+            mail_id=2,
+            sender=sender,
+            subject="Mail 1",
+            is_read=False,
+            timestamp=parse_datetime("2015-09-30T16:07:00Z"),
+        )
+        recipient_1 = create_mail_entity_from_eve_entity(1001)
+        mail.recipients.add(recipient_1)
+        # when
+        self.character_1001.update_mail_body(mail)
+        # then
+        obj = self.character_1001.mails.get(mail_id=2)
+        self.assertTrue(obj.body)
+        self.assertTrue(mock_eve_xml_to_html.called)
+
+    def test_should_delete_mail_header_when_fetching_body_returns_404(self, mock_esi):
+        # given
+        mock_esi.client.Mail.get_characters_character_id_mail_mail_id.side_effect = (
+            build_http_error(404, "Test")
+        )
+        sender = create_mail_entity_from_eve_entity(1002)
+        mail = CharacterMail.objects.create(
+            character=self.character_1001,
+            mail_id=1,
+            sender=sender,
+            subject="Mail 1",
+            is_read=False,
+            timestamp=parse_datetime("2015-09-30T16:07:00Z"),
+        )
+        recipient_1001 = create_mail_entity_from_eve_entity(1001)
+        recipient_9001 = create_mailing_list(
+            id=9001, category=MailEntity.Category.MAILING_LIST, name="Dummy 2"
+        )
+        mail.recipients.add(recipient_1001, recipient_9001)
+        # when
+        self.character_1001.update_mail_body(mail)
+        # then
+        self.assertFalse(self.character_1001.mails.filter(mail_id=1).exists())
+
+    @patch("memberaudit.models.MailEntity.objects.get_or_create_esi_async")
+    def test_can_preload_mail_senders(self, mock_get_or_create_esi_async, mock_esi):
+        # given
+        create_mailing_list(id=9001)
+        headers = {1: {"from": 9001, "mail_id": 1}, 2: {"from": 9002, "mail_id": 2}}
+        # when
+        CharacterMail.objects._preload_mail_senders(headers)
+        # then
+        self.assertTrue(mock_get_or_create_esi_async.called)
+        mail_entity_ids = {
+            o[1]["id"] for o in mock_get_or_create_esi_async.call_args_list
+        }
+        self.assertSetEqual(mail_entity_ids, {9002})
+
+
+@patch(MODULE_PATH + ".esi", esi_stub)
+class TestCharacterMailLabelManager(CharacterUpdateTestDataMixin, TestCase):
+    def test_normal(self):
+        label_1 = CharacterMailLabel.objects.create(
+            character=self.character_1001, label_id=1, name="Alpha"
+        )
+        label_2 = CharacterMailLabel.objects.create(
+            character=self.character_1001, label_id=2, name="Bravo"
+        )
+        labels = CharacterMailLabel.objects.get_all_labels()
+        self.assertDictEqual(
+            labels, {label_1.label_id: label_1, label_2.label_id: label_2}
+        )
+
+    def test_empty(self):
+        labels = CharacterMailLabel.objects.get_all_labels()
+        self.assertDictEqual(labels, {})
+
+    def test_update_mail_labels_1(self):
+        """can create from scratch"""
+        self.character_1001.update_mail_labels()
+
+        self.assertEqual(self.character_1001.unread_mail_count.total, 5)
+        self.assertSetEqual(
+            set(self.character_1001.mail_labels.values_list("label_id", flat=True)),
+            {3, 17},
+        )
+
+        obj = self.character_1001.mail_labels.get(label_id=3)
+        self.assertEqual(obj.name, "PINK")
+        self.assertEqual(obj.unread_count, 4)
+        self.assertEqual(obj.color, "#660066")
+
+        obj = self.character_1001.mail_labels.get(label_id=17)
+        self.assertEqual(obj.name, "WHITE")
+        self.assertEqual(obj.unread_count, 1)
+        self.assertEqual(obj.color, "#ffffff")
+
+    def test_update_mail_labels_2(self):
+        """will remove obsolete labels"""
+        CharacterMailLabel.objects.create(
+            character=self.character_1001, label_id=666, name="Obsolete"
+        )
+
+        self.character_1001.update_mail_labels()
+
+        self.assertSetEqual(
+            set(self.character_1001.mail_labels.values_list("label_id", flat=True)),
+            {3, 17},
+        )
+
+    def test_update_mail_labels_3(self):
+        """will update existing labels"""
+        CharacterMailLabel.objects.create(
+            character=self.character_1001,
+            label_id=3,
+            name="Update me",
+            unread_count=0,
+            color=0,
+        )
+
+        self.character_1001.update_mail_labels()
+
+        self.assertSetEqual(
+            set(self.character_1001.mail_labels.values_list("label_id", flat=True)),
+            {3, 17},
+        )
+
+        obj = self.character_1001.mail_labels.get(label_id=3)
+        self.assertEqual(obj.name, "PINK")
+        self.assertEqual(obj.unread_count, 4)
+        self.assertEqual(obj.color, "#660066")
+
+    def test_update_mail_labels_4(self):
+        """when data from ESI has not changed, then skip update"""
+        self.character_1001.update_mail_labels()
+        obj = self.character_1001.mail_labels.get(label_id=3)
+        obj.name = "MAGENTA"
+        obj.save()
+
+        self.character_1001.update_mail_labels()
+
+        obj = self.character_1001.mail_labels.get(label_id=3)
+        self.assertEqual(obj.name, "MAGENTA")
+
+    def test_update_mail_labels_5(self):
+        """when data from ESI has not changed and update is forced, then do update"""
+
+        self.character_1001.update_mail_labels()
+        obj = self.character_1001.mail_labels.get(label_id=3)
+        obj.name = "MAGENTA"
+        obj.save()
+
+        self.character_1001.update_mail_labels(force_update=True)
+
+        obj = self.character_1001.mail_labels.get(label_id=3)
+        self.assertEqual(obj.name, "PINK")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aa_memberaudit-2.9.0/memberaudit/tests/models/test_character_3.py` & `aa_memberaudit-2.9.1/memberaudit/tests/managers/test_character_sections_3.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,604 +1,204 @@
 import datetime as dt
 from unittest.mock import patch
 
-from bravado.exception import HTTPNotFound
-from pytz import utc
-
-from django.test import TestCase, override_settings
+from django.test import override_settings
 from django.utils.dateparse import parse_datetime
 from django.utils.timezone import now
-from eveuniverse.models import EveEntity, EveType
+from eveuniverse.models import EveEntity, EvePlanet, EveSolarSystem, EveType
 
-from app_utils.esi import EsiStatus
-from app_utils.esi_testing import BravadoResponseStub, build_http_error
+from app_utils.esi_testing import (
+    BravadoOperationStub,
+    EsiClientStub,
+    EsiEndpoint,
+    build_http_error,
+)
 from app_utils.testing import NoSocketsTestCase
 
-from memberaudit.core.xml_converter import eve_xml_to_html
-
-from ...models import (
+from memberaudit.models import (
     Character,
-    CharacterMail,
-    CharacterMailLabel,
+    CharacterOnlineStatus,
+    CharacterPlanet,
     CharacterShip,
     CharacterSkill,
+    CharacterSkillqueueEntry,
+    CharacterWalletBalance,
     CharacterWalletJournalEntry,
+    CharacterWalletTransaction,
     Location,
-    MailEntity,
 )
-from ..testdata.esi_client_stub import esi_client_stub
-from .utils import CharacterUpdateTestDataMixin
-
-MODELS_PATH = "memberaudit.models"
-MANAGERS_PATH = "memberaudit.managers"
-TASKS_PATH = "memberaudit.tasks"
-
-
-@override_settings(CELERY_ALWAYS_EAGER=True, CELERY_EAGER_PROPAGATES_EXCEPTIONS=True)
-@patch(MODELS_PATH + ".character.esi")
-class TestCharacterUpdateMails(CharacterUpdateTestDataMixin, TestCase):
-    def test_update_mailing_lists_1(self, mock_esi):
-        """can create new mailing lists from scratch"""
-        mock_esi.client = esi_client_stub
-
-        self.character_1001.update_mailing_lists()
-
-        self.assertSetEqual(
-            set(MailEntity.objects.values_list("id", flat=True)), {9001, 9002}
-        )
-        self.assertSetEqual(
-            set(self.character_1001.mailing_lists.values_list("id", flat=True)),
-            {9001, 9002},
-        )
-
-        obj = MailEntity.objects.get(id=9001)
-        self.assertEqual(obj.name, "Dummy 1")
-
-        obj = MailEntity.objects.get(id=9002)
-        self.assertEqual(obj.name, "Dummy 2")
-
-    def test_update_mailing_lists_2(self, mock_esi):
-        """does not remove obsolete mailing lists"""
-        mock_esi.client = esi_client_stub
-        MailEntity.objects.create(
-            id=5, category=MailEntity.Category.MAILING_LIST, name="Obsolete"
-        )
-
-        self.character_1001.update_mailing_lists()
-
-        self.assertSetEqual(
-            set(MailEntity.objects.values_list("id", flat=True)), {9001, 9002, 5}
-        )
-        self.assertSetEqual(
-            set(self.character_1001.mailing_lists.values_list("id", flat=True)),
-            {9001, 9002},
-        )
-
-    def test_update_mailing_lists_3(self, mock_esi):
-        """updates existing mailing lists"""
-        mock_esi.client = esi_client_stub
-        MailEntity.objects.create(
-            id=9001, category=MailEntity.Category.MAILING_LIST, name="Update me"
-        )
-
-        self.character_1001.update_mailing_lists()
-
-        self.assertSetEqual(
-            set(MailEntity.objects.values_list("id", flat=True)), {9001, 9002}
-        )
-        self.assertSetEqual(
-            set(self.character_1001.mailing_lists.values_list("id", flat=True)),
-            {9001, 9002},
-        )
-        obj = MailEntity.objects.get(id=9001)
-        self.assertEqual(obj.name, "Dummy 1")
-
-    def test_update_mailing_lists_4(self, mock_esi):
-        """when data from ESI has not changed, then skip update"""
-        mock_esi.client = esi_client_stub
-
-        self.character_1001.update_mailing_lists()
-        obj = MailEntity.objects.get(id=9001)
-        obj.name = "Extravaganza"
-        obj.save()
-        self.character_1001.mailing_lists.clear()
-
-        self.character_1001.update_mailing_lists()
-        obj = MailEntity.objects.get(id=9001)
-        self.assertEqual(obj.name, "Extravaganza")
-        self.assertSetEqual(
-            set(self.character_1001.mailing_lists.values_list("id", flat=True)), set()
-        )
-
-    def test_update_mailing_lists_5(self, mock_esi):
-        """when data from ESI has not changed and update is forced, then do update"""
-        mock_esi.client = esi_client_stub
-
-        self.character_1001.update_mailing_lists()
-        obj = MailEntity.objects.get(id=9001)
-        obj.name = "Extravaganza"
-        obj.save()
-
-        self.character_1001.update_mailing_lists(force_update=True)
-        obj = MailEntity.objects.get(id=9001)
-        self.assertEqual(obj.name, "Dummy 1")
-
-    def test_update_mail_labels_1(self, mock_esi):
-        """can create from scratch"""
-        mock_esi.client = esi_client_stub
-
-        self.character_1001.update_mail_labels()
-
-        self.assertEqual(self.character_1001.unread_mail_count.total, 5)
-        self.assertSetEqual(
-            set(self.character_1001.mail_labels.values_list("label_id", flat=True)),
-            {3, 17},
-        )
-
-        obj = self.character_1001.mail_labels.get(label_id=3)
-        self.assertEqual(obj.name, "PINK")
-        self.assertEqual(obj.unread_count, 4)
-        self.assertEqual(obj.color, "#660066")
-
-        obj = self.character_1001.mail_labels.get(label_id=17)
-        self.assertEqual(obj.name, "WHITE")
-        self.assertEqual(obj.unread_count, 1)
-        self.assertEqual(obj.color, "#ffffff")
-
-    def test_update_mail_labels_2(self, mock_esi):
-        """will remove obsolete labels"""
-        mock_esi.client = esi_client_stub
-        CharacterMailLabel.objects.create(
-            character=self.character_1001, label_id=666, name="Obsolete"
-        )
-
-        self.character_1001.update_mail_labels()
-
-        self.assertSetEqual(
-            set(self.character_1001.mail_labels.values_list("label_id", flat=True)),
-            {3, 17},
-        )
-
-    def test_update_mail_labels_3(self, mock_esi):
-        """will update existing labels"""
-        mock_esi.client = esi_client_stub
-        CharacterMailLabel.objects.create(
-            character=self.character_1001,
-            label_id=3,
-            name="Update me",
-            unread_count=0,
-            color=0,
-        )
 
-        self.character_1001.update_mail_labels()
-
-        self.assertSetEqual(
-            set(self.character_1001.mail_labels.values_list("label_id", flat=True)),
-            {3, 17},
-        )
-
-        obj = self.character_1001.mail_labels.get(label_id=3)
-        self.assertEqual(obj.name, "PINK")
-        self.assertEqual(obj.unread_count, 4)
-        self.assertEqual(obj.color, "#660066")
-
-    def test_update_mail_labels_4(self, mock_esi):
-        """when data from ESI has not changed, then skip update"""
-        mock_esi.client = esi_client_stub
-
-        self.character_1001.update_mail_labels()
-        obj = self.character_1001.mail_labels.get(label_id=3)
-        obj.name = "MAGENTA"
-        obj.save()
-
-        self.character_1001.update_mail_labels()
-
-        obj = self.character_1001.mail_labels.get(label_id=3)
-        self.assertEqual(obj.name, "MAGENTA")
-
-    def test_update_mail_labels_5(self, mock_esi):
-        """when data from ESI has not changed and update is forced, then do update"""
-        mock_esi.client = esi_client_stub
-
-        self.character_1001.update_mail_labels()
-        obj = self.character_1001.mail_labels.get(label_id=3)
-        obj.name = "MAGENTA"
-        obj.save()
-
-        self.character_1001.update_mail_labels(force_update=True)
-
-        obj = self.character_1001.mail_labels.get(label_id=3)
-        self.assertEqual(obj.name, "PINK")
-
-    @staticmethod
-    def stub_eve_entity_get_or_create_esi(id, *args, **kwargs):
-        """will return EveEntity if it exists else None, False"""
-        try:
-            obj = EveEntity.objects.get(id=id)
-            return obj, True
-        except EveEntity.DoesNotExist:
-            return None, False
-
-    @patch(MODELS_PATH + ".character.MEMBERAUDIT_DATA_RETENTION_LIMIT", None)
-    @patch(MANAGERS_PATH + ".general.fetch_esi_status")
-    @patch(MANAGERS_PATH + ".sections.EveEntity.objects.get_or_create_esi")
-    def test_update_mail_headers_1(
-        self, mock_eve_entity, mock_fetch_esi_status, mock_esi
-    ):
-        """can create new mail from scratch"""
-        mock_esi.client = esi_client_stub
-        mock_eve_entity.side_effect = self.stub_eve_entity_get_or_create_esi
-        mock_fetch_esi_status.return_value = EsiStatus(True, 99, 60)
-
-        self.character_1001.update_mailing_lists()
-        self.character_1001.update_mail_labels()
-        self.character_1001.update_mail_headers()
-        self.assertSetEqual(
-            set(self.character_1001.mails.values_list("mail_id", flat=True)),
-            {1, 2, 3},
-        )
-
-        obj = self.character_1001.mails.get(mail_id=1)
-        self.assertEqual(obj.sender.id, 1002)
-        self.assertTrue(obj.is_read)
-        self.assertEqual(obj.subject, "Mail 1")
-        self.assertEqual(obj.timestamp, parse_datetime("2015-09-05T16:07:00Z"))
-        self.assertFalse(obj.body)
-        self.assertTrue(obj.recipients.filter(id=1001).exists())
-        self.assertTrue(obj.recipients.filter(id=9001).exists())
-        self.assertSetEqual(set(obj.labels.values_list("label_id", flat=True)), {3})
-
-        obj = self.character_1001.mails.get(mail_id=2)
-        self.assertEqual(obj.sender_id, 9001)
-        self.assertFalse(obj.is_read)
-        self.assertEqual(obj.subject, "Mail 2")
-        self.assertEqual(obj.timestamp, parse_datetime("2015-09-10T18:07:00Z"))
-        self.assertFalse(obj.body)
-        self.assertSetEqual(set(obj.labels.values_list("label_id", flat=True)), {3})
-
-        obj = self.character_1001.mails.get(mail_id=3)
-        self.assertEqual(obj.sender_id, 1002)
-        self.assertTrue(obj.recipients.filter(id=9003).exists())
-        self.assertEqual(obj.timestamp, parse_datetime("2015-09-20T12:07:00Z"))
-
-    @patch(MODELS_PATH + ".character.MEMBERAUDIT_DATA_RETENTION_LIMIT", None)
-    @patch(MANAGERS_PATH + ".general.fetch_esi_status")
-    @patch(MANAGERS_PATH + ".sections.EveEntity.objects.get_or_create_esi")
-    def test_update_mail_headers_2(
-        self, mock_eve_entity, mock_fetch_esi_status, mock_esi
-    ):
-        """can update existing mail"""
-        mock_esi.client = esi_client_stub
-        mock_eve_entity.side_effect = self.stub_eve_entity_get_or_create_esi
-        mock_fetch_esi_status.return_value = EsiStatus(True, 99, 60)
-        sender, _ = MailEntity.objects.update_or_create_from_eve_entity_id(id=1002)
-        mail = CharacterMail.objects.create(
-            character=self.character_1001,
-            mail_id=1,
-            sender=sender,
-            subject="Mail 1",
-            timestamp=parse_datetime("2015-09-05T16:07:00Z"),
-            is_read=False,  # to be updated
-        )
-        recipient_1, _ = MailEntity.objects.update_or_create_from_eve_entity_id(id=1001)
-        recipient_2 = MailEntity.objects.create(
-            id=9001, category=MailEntity.Category.MAILING_LIST, name="Dummy 2"
-        )
-        mail.recipients.set([recipient_1, recipient_2])
-
-        self.character_1001.update_mailing_lists()
-        self.character_1001.update_mail_labels()
-        label = self.character_1001.mail_labels.get(label_id=17)
-        mail.labels.add(label)  # to be updated
-
-        self.character_1001.update_mail_headers()
-        self.assertSetEqual(
-            set(self.character_1001.mails.values_list("mail_id", flat=True)),
-            {1, 2, 3},
-        )
-
-        obj = self.character_1001.mails.get(mail_id=1)
-        self.assertEqual(obj.sender_id, 1002)
-        self.assertTrue(obj.is_read)
-        self.assertEqual(obj.subject, "Mail 1")
-        self.assertEqual(obj.timestamp, parse_datetime("2015-09-05T16:07:00Z"))
-        self.assertFalse(obj.body)
-        self.assertTrue(obj.recipients.filter(id=1001).exists())
-        self.assertTrue(obj.recipients.filter(id=9001).exists())
-        self.assertSetEqual(set(obj.labels.values_list("label_id", flat=True)), {3})
-
-    @patch(MODELS_PATH + ".character.MEMBERAUDIT_DATA_RETENTION_LIMIT", None)
-    @patch(MANAGERS_PATH + ".general.fetch_esi_status")
-    @patch(MANAGERS_PATH + ".sections.EveEntity.objects.get_or_create_esi")
-    def test_update_mail_headers_3(
-        self, mock_eve_entity, mock_fetch_esi_status, mock_esi
-    ):
-        """when ESI data is unchanged, then skip update"""
-        mock_esi.client = esi_client_stub
-        mock_eve_entity.side_effect = self.stub_eve_entity_get_or_create_esi
-        mock_fetch_esi_status.return_value = EsiStatus(True, 99, 60)
-
-        self.character_1001.update_mailing_lists()
-        self.character_1001.update_mail_labels()
-        self.character_1001.update_mail_headers()
-        obj = self.character_1001.mails.get(mail_id=1)
-        obj.is_read = False
-        obj.save()
-
-        self.character_1001.update_mail_headers()
-
-        obj = self.character_1001.mails.get(mail_id=1)
-        self.assertFalse(obj.is_read)
-
-    @patch(MODELS_PATH + ".character.MEMBERAUDIT_DATA_RETENTION_LIMIT", None)
-    @patch(MANAGERS_PATH + ".general.fetch_esi_status")
-    @patch(MANAGERS_PATH + ".sections.EveEntity.objects.get_or_create_esi")
-    def test_update_mail_headers_4(
-        self, mock_eve_entity, mock_fetch_esi_status, mock_esi
-    ):
-        """when ESI data is unchanged and update forced, then do update"""
-        mock_esi.client = esi_client_stub
-        mock_eve_entity.side_effect = self.stub_eve_entity_get_or_create_esi
-        mock_fetch_esi_status.return_value = EsiStatus(True, 99, 60)
-
-        self.character_1001.update_mailing_lists()
-        self.character_1001.update_mail_labels()
-        self.character_1001.update_mail_headers()
-        obj = self.character_1001.mails.get(mail_id=1)
-        obj.is_read = False
-        obj.save()
-
-        self.character_1001.update_mail_headers(force_update=True)
-
-        obj = self.character_1001.mails.get(mail_id=1)
-        self.assertTrue(obj.is_read)
-
-    @patch(MODELS_PATH + ".character.MEMBERAUDIT_DATA_RETENTION_LIMIT", 15)
-    @patch(MANAGERS_PATH + ".general.fetch_esi_status")
-    @patch(MANAGERS_PATH + ".sections.EveEntity.objects.get_or_create_esi")
-    def test_update_mail_headers_6(
-        self, mock_eve_entity, mock_fetch_esi_status, mock_esi
-    ):
-        """when data retention limit is set, then only fetch mails within that limit"""
-        mock_esi.client = esi_client_stub
-        mock_eve_entity.side_effect = self.stub_eve_entity_get_or_create_esi
-        mock_fetch_esi_status.return_value = EsiStatus(True, 99, 60)
-
-        with patch(MODELS_PATH + ".character.now") as mock_now:
-            mock_now.return_value = dt.datetime(2015, 9, 20, 20, 5, tzinfo=utc)
-            self.character_1001.update_mailing_lists()
-            self.character_1001.update_mail_labels()
-            self.character_1001.update_mail_headers()
-
-        self.assertSetEqual(
-            set(self.character_1001.mails.values_list("mail_id", flat=True)),
-            {2, 3},
-        )
-
-    @patch(MODELS_PATH + ".character.MEMBERAUDIT_DATA_RETENTION_LIMIT", 15)
-    @patch(MANAGERS_PATH + ".general.fetch_esi_status")
-    @patch(MANAGERS_PATH + ".sections.EveEntity.objects.get_or_create_esi")
-    def test_update_mail_headers_7(
-        self, mock_eve_entity, mock_fetch_esi_status, mock_esi
-    ):
-        """when data retention limit is set, then remove old data beyond that limit"""
-        mock_esi.client = esi_client_stub
-        mock_eve_entity.side_effect = self.stub_eve_entity_get_or_create_esi
-        mock_fetch_esi_status.return_value = EsiStatus(True, 99, 60)
-        sender, _ = MailEntity.objects.update_or_create_from_eve_entity_id(id=1002)
-        CharacterMail.objects.create(
-            character=self.character_1001,
-            mail_id=99,
-            sender=sender,
-            subject="Mail Old",
-            timestamp=parse_datetime("2015-09-02T14:02:00Z"),
-            is_read=False,
-        )
-
-        with patch(MODELS_PATH + ".character.now") as mock_now:
-            mock_now.return_value = dt.datetime(2015, 9, 20, 20, 5, tzinfo=utc)
-            self.character_1001.update_mailing_lists()
-            self.character_1001.update_mail_labels()
-            self.character_1001.update_mail_headers()
-
-        self.assertSetEqual(
-            set(self.character_1001.mails.values_list("mail_id", flat=True)),
-            {2, 3},
-        )
+from ..testdata.esi_client_stub import esi_client_stub
+from ..testdata.factories import (
+    create_character_mining_ledger_entry,
+    create_character_planet,
+)
+from ..testdata.load_entities import load_entities
+from ..testdata.load_eveuniverse import load_eveuniverse
+from ..utils import CharacterUpdateTestDataMixin, create_memberaudit_character
+
+MODULE_PATH = "memberaudit.managers.character_sections_3"
+
+
+@patch(MODULE_PATH + ".esi")
+class TestCharacterMiningLedgerManager(NoSocketsTestCase):
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+        load_eveuniverse()
+        load_entities()
+        cls.character_1001 = create_memberaudit_character(1001)
+        cls.endpoints = [
+            EsiEndpoint(
+                "Industry",
+                "get_characters_character_id_mining",
+                "character_id",
+                needs_token=True,
+                data={
+                    "1001": [
+                        {
+                            "date": "2017-09-19",
+                            "quantity": 7004,
+                            "solar_system_id": 30002537,
+                            "type_id": 17471,
+                        },
+                        {
+                            "date": "2017-09-18",
+                            "quantity": 5199,
+                            "solar_system_id": 30002537,
+                            "type_id": 17471,
+                        },
+                    ]
+                },
+            ),
+        ]
+        cls.esi_client_stub = EsiClientStub.create_from_endpoints(cls.endpoints)
 
-    def test_should_update_existing_mail_body(self, mock_esi):
+    def test_should_add_new_entry_from_scratch(self, mock_esi):
         # given
-        mock_esi.client = esi_client_stub
-        sender, _ = MailEntity.objects.update_or_create_from_eve_entity_id(id=1002)
-        mail = CharacterMail.objects.create(
-            character=self.character_1001,
-            mail_id=1,
-            sender=sender,
-            subject="Mail 1",
-            body="Update me",
-            is_read=False,
-            timestamp=parse_datetime("2015-09-30T16:07:00Z"),
-        )
-        recipient_1001, _ = MailEntity.objects.update_or_create_from_eve_entity_id(
-            id=1001
-        )
-        recipient_9001 = MailEntity.objects.create(
-            id=9001, category=MailEntity.Category.MAILING_LIST, name="Dummy 2"
-        )
-        mail.recipients.add(recipient_1001, recipient_9001)
+        mock_esi.client = self.esi_client_stub
         # when
-        self.character_1001.update_mail_body(mail)
+        self.character_1001.update_mining_ledger()
         # then
-        obj = self.character_1001.mails.get(mail_id=1)
-        self.assertEqual(obj.body, "blah blah blah 😓")
-
-    @patch(MODELS_PATH + ".character.eve_xml_to_html")
-    def test_should_update_mail_body_from_scratch(self, mock_eve_xml_to_html, mock_esi):
-        # given
-        mock_esi.client = esi_client_stub
-        mock_eve_xml_to_html.side_effect = lambda x: eve_xml_to_html(x)
-        sender, _ = MailEntity.objects.update_or_create_from_eve_entity_id(id=1002)
-        mail = CharacterMail.objects.create(
-            character=self.character_1001,
-            mail_id=2,
-            sender=sender,
-            subject="Mail 1",
-            is_read=False,
-            timestamp=parse_datetime("2015-09-30T16:07:00Z"),
+        self.assertEqual(self.character_1001.mining_ledger.count(), 2)
+        obj = self.character_1001.mining_ledger.first()
+        self.assertEqual(obj.date, dt.date(2017, 9, 19))
+        self.assertEqual(obj.eve_type, EveType.objects.get(name="Dense Veldspar"))
+        self.assertEqual(
+            obj.eve_solar_system, EveSolarSystem.objects.get(name="Amamake")
         )
-        recipient_1, _ = MailEntity.objects.update_or_create_from_eve_entity_id(id=1001)
-        mail.recipients.add(recipient_1)
-        # when
-        self.character_1001.update_mail_body(mail)
-        # then
-        obj = self.character_1001.mails.get(mail_id=2)
-        self.assertTrue(obj.body)
-        self.assertTrue(mock_eve_xml_to_html.called)
+        self.assertEqual(obj.quantity, 7004)
 
-    def test_should_delete_mail_header_when_fetching_body_returns_404(self, mock_esi):
+    def test_should_update_existing_entries(self, mock_esi):
         # given
-        mock_esi.client.Mail.get_characters_character_id_mail_mail_id.side_effect = (
-            HTTPNotFound(response=BravadoResponseStub(404, "Test"))
-        )
-        sender, _ = MailEntity.objects.update_or_create_from_eve_entity_id(id=1002)
-        mail = CharacterMail.objects.create(
+        mock_esi.client = self.esi_client_stub
+        create_character_mining_ledger_entry(
             character=self.character_1001,
-            mail_id=1,
-            sender=sender,
-            subject="Mail 1",
-            is_read=False,
-            timestamp=parse_datetime("2015-09-30T16:07:00Z"),
-        )
-        recipient_1001, _ = MailEntity.objects.update_or_create_from_eve_entity_id(
-            id=1001
+            date=dt.date(2017, 9, 19),
+            eve_solar_system=EveSolarSystem.objects.get(name="Amamake"),
+            eve_type=EveType.objects.get(name="Dense Veldspar"),
+            quantity=5,
         )
-        recipient_9001 = MailEntity.objects.create(
-            id=9001, category=MailEntity.Category.MAILING_LIST, name="Dummy 2"
-        )
-        mail.recipients.add(recipient_1001, recipient_9001)
         # when
-        self.character_1001.update_mail_body(mail)
+        self.character_1001.update_mining_ledger()
         # then
-        self.assertFalse(self.character_1001.mails.filter(mail_id=1).exists())
-
-
-@patch(MODELS_PATH + ".character.esi")
-class TestCharacterUpdateLoyalty(CharacterUpdateTestDataMixin, NoSocketsTestCase):
-    def test_create(self, mock_esi):
-        """can create from scratch"""
-        mock_esi.client = esi_client_stub
-
-        self.character_1001.update_loyalty()
-        self.assertEqual(self.character_1001.loyalty_entries.count(), 1)
-
-        obj = self.character_1001.loyalty_entries.get(corporation_id=2002)
-        self.assertEqual(obj.loyalty_points, 100)
-
-    def test_update(self, mock_esi):
-        """can update existing loyalty"""
-        mock_esi.client = esi_client_stub
-        self.character_1001.loyalty_entries.create(
-            corporation=self.corporation_2001, loyalty_points=200
+        self.assertEqual(self.character_1001.mining_ledger.count(), 2)
+        obj = self.character_1001.mining_ledger.get(
+            date=dt.date(2017, 9, 19),
+            eve_solar_system=EveSolarSystem.objects.get(name="Amamake"),
+            eve_type=EveType.objects.get(name="Dense Veldspar"),
         )
+        self.assertEqual(obj.quantity, 7004)
 
-        self.character_1001.update_loyalty()
-        self.assertEqual(self.character_1001.loyalty_entries.count(), 1)
-
-        obj = self.character_1001.loyalty_entries.get(corporation=self.corporation_2002)
-        self.assertEqual(obj.loyalty_points, 100)
-
-    def test_skip_update_1(self, mock_esi):
-        """when data from ESI has not changed, then skip update"""
-        mock_esi.client = esi_client_stub
-
-        self.character_1001.update_loyalty()
-        obj = self.character_1001.loyalty_entries.get(corporation=self.corporation_2002)
-        obj.loyalty_points = 200
-        obj.save()
-        self.character_1001.update_loyalty()
 
-        obj = self.character_1001.loyalty_entries.get(corporation=self.corporation_2002)
-        self.assertEqual(obj.loyalty_points, 200)
-
-    def test_skip_update_2(self, mock_esi):
-        """when data from ESI has not changed and update is forced, then do update"""
-        mock_esi.client = esi_client_stub
-
-        self.character_1001.update_loyalty()
-        obj = self.character_1001.loyalty_entries.get(corporation=self.corporation_2002)
-        obj.loyalty_points = 200
-        obj.save()
-
-        self.character_1001.update_loyalty(force_update=True)
-
-        obj = self.character_1001.loyalty_entries.get(corporation=self.corporation_2002)
-        self.assertEqual(obj.loyalty_points, 100)
-
-    def test_should_thread_http_500_as_empty_loyalty_list(self, mock_esi):
+@patch(MODULE_PATH + ".esi")
+class TestCharacterOnlineStatusManager(CharacterUpdateTestDataMixin, NoSocketsTestCase):
+    def test_update_online_status(self, mock_esi):
         # given
-        exception = build_http_error(
-            500, '{"error":"Unhandled internal error encountered!"}'
-        )
-        mock_esi.client.Loyalty.get_characters_character_id_loyalty_points.side_effect = (
-            exception
-        )
-        self.character_1001.loyalty_entries.create(
-            corporation=self.corporation_2001, loyalty_points=100
-        )
+        mock_esi.client = esi_client_stub
         # when
-        self.character_1001.update_loyalty()
+        CharacterOnlineStatus.objects.update_or_create_esi(self.character_1001)
         # then
-        self.assertEqual(self.character_1001.loyalty_entries.count(), 1)
-        obj = self.character_1001.loyalty_entries.get(corporation=self.corporation_2001)
-        self.assertEqual(obj.loyalty_points, 100)
-
-
-@override_settings(CELERY_ALWAYS_EAGER=True, CELERY_EAGER_PROPAGATES_EXCEPTIONS=True)
-@patch(MODELS_PATH + ".character.esi")
-class TestCharacterUpdateLocation(CharacterUpdateTestDataMixin, NoSocketsTestCase):
-    def test_update_location_1(self, mock_esi):
-        mock_esi.client = esi_client_stub
-
-        self.character_1001.update_location()
-        self.assertEqual(self.character_1001.location.eve_solar_system, self.jita)
-        self.assertEqual(self.character_1001.location.location, self.jita_44)
-
-    def test_update_location_2(self, mock_esi):
-        mock_esi.client = esi_client_stub
-
-        self.character_1002.update_location()
-        self.assertEqual(self.character_1002.location.eve_solar_system, self.amamake)
-        self.assertEqual(self.character_1002.location.location, self.structure_1)
-
-
-@override_settings(CELERY_ALWAYS_EAGER=True, CELERY_EAGER_PROPAGATES_EXCEPTIONS=True)
-@patch(MODELS_PATH + ".character.esi")
-class TestCharacterUpdateOnlineStatus(CharacterUpdateTestDataMixin, NoSocketsTestCase):
-    def test_update_online_status(self, mock_esi):
-        mock_esi.client = esi_client_stub
-
-        self.character_1001.update_online_status()
         self.assertEqual(
             self.character_1001.online_status.last_login,
             parse_datetime("2017-01-02T03:04:05Z"),
         )
         self.assertEqual(
             self.character_1001.online_status.last_logout,
             parse_datetime("2017-01-02T04:05:06Z"),
         )
         self.assertEqual(self.character_1001.online_status.logins, 9001)
 
 
-@patch(MODELS_PATH + ".character.esi")
-class TestCharacterUpdateShip(CharacterUpdateTestDataMixin, NoSocketsTestCase):
+@patch(MODULE_PATH + ".esi")
+class TestCharacterPlanetManager(NoSocketsTestCase):
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+        load_eveuniverse()
+        load_entities()
+        cls.character_1001 = create_memberaudit_character(1001)
+        cls.endpoints = [
+            EsiEndpoint(
+                "Planetary_Interaction",
+                "get_characters_character_id_planets",
+                "character_id",
+                needs_token=True,
+                data={
+                    "1001": [
+                        {
+                            "last_update": "2016-11-28T16:42:51Z",
+                            "num_pins": 1,
+                            "owner_id": 1001,
+                            "planet_id": 40161463,
+                            "planet_type": "barren",
+                            "solar_system_id": 30002537,
+                            "upgrade_level": 0,
+                        }
+                    ]
+                },
+            ),
+        ]
+        cls.esi_client_stub = EsiClientStub.create_from_endpoints(cls.endpoints)
+
+    def test_should_add_new_planet(self, mock_esi):
+        # given
+        mock_esi.client = self.esi_client_stub
+        # when
+        self.character_1001.update_planets()
+        # then
+        self.assertEqual(self.character_1001.planets.count(), 1)
+        obj: CharacterPlanet = self.character_1001.planets.first()
+        self.assertIsInstance(obj.last_update_at, dt.datetime)
+        self.assertEqual(obj.eve_planet, EvePlanet.objects.get(id=40161463))
+        self.assertEqual(obj.num_pins, 1)
+        self.assertEqual(obj.upgrade_level, 0)
+
+    def test_should_update_existing_entries(self, mock_esi):
+        # given
+        mock_esi.client = self.esi_client_stub
+        create_character_planet(character=self.character_1001)
+        # when
+        self.character_1001.update_planets()
+        # then
+        self.assertEqual(self.character_1001.planets.count(), 1)
+        obj: CharacterPlanet = self.character_1001.planets.first()
+        self.assertIsInstance(obj.last_update_at, dt.datetime)
+        self.assertEqual(obj.eve_planet, EvePlanet.objects.get(id=40161463))
+        self.assertEqual(obj.num_pins, 1)
+        self.assertEqual(obj.upgrade_level, 0)
+
+
+@patch(MODULE_PATH + ".esi")
+class TestCharacterShipManager(CharacterUpdateTestDataMixin, NoSocketsTestCase):
     def test_should_update_all_fields(self, mock_esi):
         # given
         mock_esi.client = esi_client_stub
         # when
-        self.character_1001.update_ship()
+        CharacterShip.objects.update_or_create_esi(self.character_1001)
         # then
         self.assertEqual(self.character_1001.ship.eve_type_id, 603)
         self.assertEqual(self.character_1001.ship.name, "Shooter Boy")
 
     def test_should_ignore_error_500(self, mock_esi):
         # given
         error_500 = build_http_error(
@@ -607,121 +207,136 @@
         mock_esi.client.Location.get_characters_character_id_ship.side_effect = (
             error_500
         )
         CharacterShip.objects.create(
             character=self.character_1001, eve_type_id=603, name="Shooter Boy"
         )
         # when
-        self.character_1001.update_ship()
+        CharacterShip.objects.update_or_create_esi(self.character_1001)
         # then
         self.character_1001.refresh_from_db()
         self.assertEqual(self.character_1001.ship.eve_type_id, 603)
         self.assertEqual(self.character_1001.ship.name, "Shooter Boy")
 
+    def test_should_remove_ship_when_esi_returns_empty_response(self, mock_esi):
+        # given
+        mock_esi.client.Location.get_characters_character_id_ship.return_value = (
+            BravadoOperationStub(data={})
+        )
+        CharacterShip.objects.create(
+            character=self.character_1001, eve_type_id=603, name="Shooter Boy"
+        )
+        # when
+        CharacterShip.objects.update_or_create_esi(self.character_1001)
+        # then
+        self.assertFalse(
+            CharacterShip.objects.filter(character=self.character_1001).exists()
+        )
 
-@patch(MODELS_PATH + ".character.esi")
-class TestCharacterUpdateSkills(CharacterUpdateTestDataMixin, NoSocketsTestCase):
-    def test_update_skills_1(self, mock_esi):
-        """can create new skills"""
-        mock_esi.client = esi_client_stub
 
-        self.character_1001.update_skills()
+@patch(MODULE_PATH + ".esi")
+class TestCharacterSkillManager(CharacterUpdateTestDataMixin, NoSocketsTestCase):
+    def test_can_create_new_skills(self, mock_esi):
+        # given
+        mock_esi.client = esi_client_stub
+        # when
+        CharacterSkill.objects.update_or_create_esi(character=self.character_1001)
+        # then
         self.assertEqual(self.character_1001.skillpoints.total, 30_000)
         self.assertEqual(self.character_1001.skillpoints.unallocated, 1_000)
-
         self.assertSetEqual(
             set(self.character_1001.skills.values_list("eve_type_id", flat=True)),
             {24311, 24312},
         )
-
         skill = self.character_1001.skills.get(eve_type_id=24311)
         self.assertEqual(skill.active_skill_level, 3)
         self.assertEqual(skill.skillpoints_in_skill, 20_000)
         self.assertEqual(skill.trained_skill_level, 4)
 
         skill = self.character_1001.skills.get(eve_type_id=24312)
         self.assertEqual(skill.active_skill_level, 1)
         self.assertEqual(skill.skillpoints_in_skill, 10_000)
         self.assertEqual(skill.trained_skill_level, 1)
 
-    def test_update_skills_2(self, mock_esi):
-        """can update existing skills"""
+    def test_caen_update_existing_skills(self, mock_esi):
+        # given
         mock_esi.client = esi_client_stub
-
         CharacterSkill.objects.create(
             character=self.character_1001,
             eve_type=EveType.objects.get(id=24311),
             active_skill_level=1,
             skillpoints_in_skill=1,
             trained_skill_level=1,
         )
-
-        self.character_1001.update_skills()
-
+        # when
+        CharacterSkill.objects.update_or_create_esi(character=self.character_1001)
+        # then
         self.assertEqual(self.character_1001.skills.count(), 2)
         skill = self.character_1001.skills.get(eve_type_id=24311)
         self.assertEqual(skill.active_skill_level, 3)
         self.assertEqual(skill.skillpoints_in_skill, 20_000)
         self.assertEqual(skill.trained_skill_level, 4)
 
-    def test_update_skills_3(self, mock_esi):
-        """can delete obsolete skills"""
+    def test_can_delete_obsolete_skills(self, mock_esi):
+        # given
         mock_esi.client = esi_client_stub
-
         CharacterSkill.objects.create(
             character=self.character_1001,
             eve_type=EveType.objects.get(id=20185),
             active_skill_level=1,
             skillpoints_in_skill=1,
             trained_skill_level=1,
         )
-
-        self.character_1001.update_skills()
-
+        # when
+        CharacterSkill.objects.update_or_create_esi(character=self.character_1001)
+        # then
         self.assertSetEqual(
             set(self.character_1001.skills.values_list("eve_type_id", flat=True)),
             {24311, 24312},
         )
 
     def test_update_skills_4(self, mock_esi):
         """when ESI info has not changed, then do not update local data"""
+        # given
         mock_esi.client = esi_client_stub
-
         self.character_1001.reset_update_section(Character.UpdateSection.SKILLS)
         self.character_1001.update_skills()
         skill = self.character_1001.skills.get(eve_type_id=24311)
         skill.active_skill_level = 4
         skill.save()
-        self.character_1001.update_skills()
+        # when
+        CharacterSkill.objects.update_or_create_esi(character=self.character_1001)
+        # then
         skill.refresh_from_db()
         self.assertEqual(skill.active_skill_level, 4)
 
     def test_update_skills_5(self, mock_esi):
         """when ESI info has not changed and update forced, then update local data"""
+        # given
         mock_esi.client = esi_client_stub
-
         self.character_1001.reset_update_section(Character.UpdateSection.SKILLS)
-        self.character_1001.update_skills()
+        # when
+        CharacterSkill.objects.update_or_create_esi(character=self.character_1001)
+        # then
         skill = self.character_1001.skills.get(eve_type_id=24311)
         skill.active_skill_level = 4
         skill.save()
-
         self.character_1001.update_skills(force_update=True)
-
         skill = self.character_1001.skills.get(eve_type_id=24311)
         self.assertEqual(skill.active_skill_level, 3)
 
 
-@patch(MODELS_PATH + ".character.esi")
-class TestCharacterUpdateSkillQueue(CharacterUpdateTestDataMixin, NoSocketsTestCase):
-    def test_create(self, mock_esi):
-        """can create skill queue from scratch"""
+@patch(MODULE_PATH + ".esi")
+class TestCharacterSkillQueueManager(CharacterUpdateTestDataMixin, NoSocketsTestCase):
+    def test_can_create_from_scratch(self, mock_esi):
+        # given
         mock_esi.client = esi_client_stub
-
-        self.character_1001.update_skill_queue()
+        # when
+        CharacterSkillqueueEntry.objects.update_or_create_esi(self.character_1001)
+        # then
         self.assertEqual(self.character_1001.skillqueue.count(), 3)
 
         entry = self.character_1001.skillqueue.get(queue_position=0)
         self.assertEqual(entry.eve_type, EveType.objects.get(id=24311))
         self.assertEqual(entry.finish_date, parse_datetime("2016-06-29T10:47:00Z"))
         self.assertEqual(entry.finished_level, 3)
         self.assertEqual(entry.start_date, parse_datetime("2016-06-29T10:46:00Z"))
@@ -735,71 +350,83 @@
         self.assertEqual(entry.start_date, parse_datetime("2016-06-29T10:47:00Z"))
         self.assertEqual(entry.training_start_sp, 50)
 
         entry = self.character_1001.skillqueue.get(queue_position=2)
         self.assertEqual(entry.eve_type, EveType.objects.get(id=24312))
         self.assertEqual(entry.finished_level, 5)
 
-    def test_update_1(self, mock_esi):
-        """can update existing skill queue"""
+    def test_can_update_existing_queue(self, mock_esi):
+        # given
         mock_esi.client = esi_client_stub
         self.character_1001.skillqueue.create(
             queue_position=0,
             eve_type=EveType.objects.get(id=24311),
             finish_date=now() + dt.timedelta(days=1),
             finished_level=4,
             start_date=now() - dt.timedelta(days=1),
         )
-
-        self.character_1001.update_skill_queue()
+        # when
+        CharacterSkillqueueEntry.objects.update_or_create_esi(self.character_1001)
+        # then
         self.assertEqual(self.character_1001.skillqueue.count(), 3)
 
         entry = self.character_1001.skillqueue.get(queue_position=0)
         self.assertEqual(entry.eve_type, EveType.objects.get(id=24311))
         self.assertEqual(entry.finish_date, parse_datetime("2016-06-29T10:47:00Z"))
         self.assertEqual(entry.finished_level, 3)
         self.assertEqual(entry.start_date, parse_datetime("2016-06-29T10:46:00Z"))
 
-    def test_skip_update_1(self, mock_esi):
-        """when ESI data has not changed, then skip update"""
+    def test_should_skip_update_when_no_change(self, mock_esi):
+        # given
         mock_esi.client = esi_client_stub
-
-        self.character_1001.update_skill_queue()
+        CharacterSkillqueueEntry.objects.update_or_create_esi(self.character_1001)
         entry = self.character_1001.skillqueue.get(queue_position=0)
         entry.finished_level = 4
         entry.save()
-
-        self.character_1001.update_skill_queue()
+        # when
+        CharacterSkillqueueEntry.objects.update_or_create_esi(self.character_1001)
+        # then
         entry = self.character_1001.skillqueue.get(queue_position=0)
         self.assertEqual(entry.finished_level, 4)
 
-    def test_skip_update_2(self, mock_esi):
-        """when ESI data has not changed and update is forced, then do update"""
+    def test_should_always_update_when_forced(self, mock_esi):
+        # given
         mock_esi.client = esi_client_stub
-
-        self.character_1001.update_skill_queue()
+        CharacterSkillqueueEntry.objects.update_or_create_esi(self.character_1001)
         entry = self.character_1001.skillqueue.get(queue_position=0)
         entry.finished_level = 4
         entry.save()
-
-        self.character_1001.update_skill_queue(force_update=True)
+        # when
+        CharacterSkillqueueEntry.objects.update_or_create_esi(
+            self.character_1001, force_update=True
+        )
+        # then
         entry = self.character_1001.skillqueue.get(queue_position=0)
         self.assertEqual(entry.finished_level, 3)
 
 
-@override_settings(CELERY_ALWAYS_EAGER=True, CELERY_EAGER_PROPAGATES_EXCEPTIONS=True)
-@patch(MODELS_PATH + ".character.esi")
-class TestCharacterUpdateWalletJournal(CharacterUpdateTestDataMixin, NoSocketsTestCase):
+@patch(MODULE_PATH + ".esi")
+class TestCharacterWalletBalanceManager(
+    CharacterUpdateTestDataMixin, NoSocketsTestCase
+):
     def test_update_wallet_balance(self, mock_esi):
+        # given
         mock_esi.client = esi_client_stub
-
-        self.character_1001.update_wallet_balance()
+        # when
+        CharacterWalletBalance.objects.update_or_create_esi(self.character_1001)
+        # then
         self.assertEqual(self.character_1001.wallet_balance.total, 123456789)
 
-    @patch(MODELS_PATH + ".character.MEMBERAUDIT_DATA_RETENTION_LIMIT", None)
+
+@override_settings(CELERY_ALWAYS_EAGER=True, CELERY_EAGER_PROPAGATES_EXCEPTIONS=True)
+@patch(MODULE_PATH + ".esi")
+class TestCharacterWalletJournalManager(
+    CharacterUpdateTestDataMixin, NoSocketsTestCase
+):
+    @patch(MODULE_PATH + ".data_retention_cutoff", lambda: None)
     def test_update_wallet_journal_1(self, mock_esi):
         """can create wallet journal entry from scratch"""
         mock_esi.client = esi_client_stub
 
         self.character_1001.update_wallet_journal()
 
         self.assertSetEqual(
@@ -819,15 +446,15 @@
         self.assertEqual(obj.second_party.id, 2002)
 
         obj = self.character_1001.wallet_journal.get(entry_id=91)
         self.assertEqual(
             obj.ref_type, "agent_mission_time_bonus_reward_corporation_tax"
         )
 
-    @patch(MODELS_PATH + ".character.MEMBERAUDIT_DATA_RETENTION_LIMIT", None)
+    @patch(MODULE_PATH + ".data_retention_cutoff", lambda: None)
     def test_update_wallet_journal_2(self, mock_esi):
         """can add entry to existing wallet journal"""
         mock_esi.client = esi_client_stub
         CharacterWalletJournalEntry.objects.create(
             character=self.character_1001,
             entry_id=1,
             amount=1_000_000,
@@ -853,15 +480,15 @@
         self.assertEqual(obj.context_id_type, obj.CONTEXT_ID_TYPE_CONTRACT_ID)
         self.assertEqual(obj.date, parse_datetime("2018-02-23T14:31:32Z"))
         self.assertEqual(obj.description, "Contract Deposit")
         self.assertEqual(obj.first_party.id, 2001)
         self.assertEqual(obj.ref_type, "contract_deposit")
         self.assertEqual(obj.second_party.id, 2002)
 
-    @patch(MODELS_PATH + ".character.MEMBERAUDIT_DATA_RETENTION_LIMIT", None)
+    @patch(MODULE_PATH + ".data_retention_cutoff", lambda: None)
     def test_update_wallet_journal_3(self, mock_esi):
         """does not update existing entries"""
         mock_esi.client = esi_client_stub
         CharacterWalletJournalEntry.objects.create(
             character=self.character_1001,
             entry_id=89,
             amount=1_000_000,
@@ -885,64 +512,68 @@
         self.assertEqual(
             obj.context_id_type, CharacterWalletJournalEntry.CONTEXT_ID_TYPE_UNDEFINED
         )
         self.assertEqual(obj.description, "dummy")
         self.assertEqual(obj.first_party.id, 1001)
         self.assertEqual(obj.second_party.id, 1002)
 
-    @patch(MODELS_PATH + ".character.MEMBERAUDIT_DATA_RETENTION_LIMIT", 10)
     def test_update_wallet_journal_4(self, mock_esi):
         """When new wallet entry is older than retention limit, then do not store it"""
         mock_esi.client = esi_client_stub
 
-        with patch(MODELS_PATH + ".character.now") as mock_now:
-            mock_now.return_value = dt.datetime(2018, 3, 11, 20, 5, tzinfo=utc)
+        with patch(
+            MODULE_PATH + ".data_retention_cutoff",
+            lambda: dt.datetime(2018, 3, 11, 20, 5, tzinfo=dt.timezone.utc)
+            - dt.timedelta(days=10),
+        ):
             self.character_1001.update_wallet_journal()
 
         self.assertSetEqual(
             set(self.character_1001.wallet_journal.values_list("entry_id", flat=True)),
             {91},
         )
 
-    @patch(MODELS_PATH + ".character.MEMBERAUDIT_DATA_RETENTION_LIMIT", 20)
     def test_update_wallet_journal_5(self, mock_esi):
         """When wallet existing entry is older than retention limit, then delete it"""
         mock_esi.client = esi_client_stub
         CharacterWalletJournalEntry.objects.create(
             character=self.character_1001,
             entry_id=55,
             amount=1_000_000,
             balance=10_000_000,
             context_id_type=CharacterWalletJournalEntry.CONTEXT_ID_TYPE_UNDEFINED,
-            date=dt.datetime(2018, 2, 11, 20, 5, tzinfo=utc),
+            date=dt.datetime(2018, 2, 11, 20, 5, tzinfo=dt.timezone.utc),
             description="dummy",
             first_party=EveEntity.objects.get(id=1001),
             second_party=EveEntity.objects.get(id=1002),
         )
 
-        with patch(MODELS_PATH + ".character.now") as mock_now:
-            mock_now.return_value = dt.datetime(2018, 3, 11, 20, 5, tzinfo=utc)
+        with patch(
+            MODULE_PATH + ".data_retention_cutoff",
+            lambda: dt.datetime(2018, 3, 11, 20, 5, tzinfo=dt.timezone.utc)
+            - dt.timedelta(days=20),
+        ):
             self.character_1001.update_wallet_journal()
 
         self.assertSetEqual(
             set(self.character_1001.wallet_journal.values_list("entry_id", flat=True)),
             {89, 91},
         )
 
 
-@patch(MODELS_PATH + ".character.esi")
-class TestCharacterUpdateWalletTransaction(
+@patch(MODULE_PATH + ".esi")
+class TestCharacterWalletTransactionManager(
     CharacterUpdateTestDataMixin, NoSocketsTestCase
 ):
     def test_should_add_wallet_transactions_from_scratch(self, mock_esi):
         # given
         mock_esi.client = esi_client_stub
         # when
-        with patch(MODELS_PATH + ".character.MEMBERAUDIT_DATA_RETENTION_LIMIT", None):
-            self.character_1001.update_wallet_transactions()
+        with patch(MODULE_PATH + ".data_retention_cutoff", lambda: None):
+            CharacterWalletTransaction.objects.update_or_create_esi(self.character_1001)
         # then
         self.assertSetEqual(
             set(
                 self.character_1001.wallet_transactions.values_list(
                     "transaction_id", flat=True
                 )
             ),
@@ -972,34 +603,20 @@
             context_id_type=CharacterWalletJournalEntry.CONTEXT_ID_TYPE_UNDEFINED,
             date=parse_datetime("2016-10-24T09:00:00Z"),
             description="dummy",
             first_party=EveEntity.objects.get(id=1001),
             second_party=EveEntity.objects.get(id=1003),
         )
         # when
-        with patch(MODELS_PATH + ".character.MEMBERAUDIT_DATA_RETENTION_LIMIT", None):
-            self.character_1001.update_wallet_transactions()
+        with patch(MODULE_PATH + ".data_retention_cutoff", lambda: None):
+            CharacterWalletTransaction.objects.update_or_create_esi(self.character_1001)
         # then
         self.assertSetEqual(
             set(
                 self.character_1001.wallet_transactions.values_list(
                     "transaction_id", flat=True
                 )
             ),
             {42},
         )
         obj = self.character_1001.wallet_transactions.get(transaction_id=42)
         self.assertEqual(obj.journal_ref, journal_entry)
-
-
-# class TestCharacterMailingList(CharacterUpdateTestDataMixin, NoSocketsTestCase):
-#     def test_name_plus_1(self):
-#         """when mailing list has name then return it's name"""
-#         mailing_list = CharacterMailingList(
-#             self.character_1001, list_id=99, name="Avengers Talk"
-#         )
-#         self.assertEqual(mailing_list.name_plus, "Avengers Talk")
-
-#     def test_name_plus_2(self):
-#         """when mailing list has no name then return a generic name"""
-#         mailing_list = CharacterMailingList(self.character_1001, list_id=99)
-#         self.assertEqual(mailing_list.name_plus, "Mailing list #99")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `aa_memberaudit-2.9.0/memberaudit/tests/models/test_character_4.py` & `aa_memberaudit-2.9.1/memberaudit/tests/models/test_characters_2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,25 @@
-import datetime as dt
-from unittest.mock import patch
+from unittest.mock import MagicMock, patch
 
 from django.test import TestCase
-from django.utils.dateparse import parse_datetime
-from eveuniverse.models import EveSolarSystem, EveType
 
 from allianceauth.eveonline.models import EveCharacter
 from allianceauth.tests.auth_utils import AuthUtils
-from app_utils.esi_testing import EsiClientStub, EsiEndpoint
-from app_utils.testing import NoSocketsTestCase, create_user_from_evecharacter
+from app_utils.esi_testing import build_http_error
+from app_utils.testing import create_user_from_evecharacter
 
-from memberaudit.models import CharacterAttributes, CharacterFwStats
-
-from ..testdata.esi_client_stub import esi_client_stub
-from ..testdata.factories import create_character, create_character_mining_ledger_entry
+from ..testdata.factories import create_character
 from ..testdata.load_entities import load_entities
-from ..testdata.load_eveuniverse import load_eveuniverse
 from ..utils import (
     add_memberaudit_character_to_user,
     create_memberaudit_character,
     create_user_from_evecharacter_with_access,
 )
-from .utils import CharacterUpdateTestDataMixin
 
-MODELS_PATH = "memberaudit.models"
-MANAGERS_PATH = "memberaudit.managers"
-TASKS_PATH = "memberaudit.tasks"
+MODULE_PATH = "memberaudit.models.characters"
 
 
 class TestCharacterUserHasAccess(TestCase):
     @classmethod
     def setUpClass(cls) -> None:
         super().setUpClass()
         load_entities()
@@ -456,284 +446,159 @@
         user_3 = AuthUtils.add_permission_to_user_by_name(
             "memberaudit.view_same_alliance", user_3
         )
         # when/then
         self.assertFalse(character_1001.user_has_scope(user_3))
 
 
-@patch(MODELS_PATH + ".character.esi")
-class TestCharacterUpdateAttributes(CharacterUpdateTestDataMixin, NoSocketsTestCase):
-    def test_create(self, mock_esi):
-        """can load attributes from test data"""
-        mock_esi.client = esi_client_stub
-
-        self.character_1001.update_attributes()
-        self.assertEqual(
-            self.character_1001.attributes.accrued_remap_cooldown_date,
-            parse_datetime("2016-10-24T09:00:00Z"),
-        )
-
-        self.assertEqual(
-            self.character_1001.attributes.last_remap_date,
-            parse_datetime("2016-10-24T09:00:00Z"),
-        )
-
-        self.assertEqual(self.character_1001.attributes.charisma, 16)
-        self.assertEqual(self.character_1001.attributes.intelligence, 17)
-        self.assertEqual(self.character_1001.attributes.memory, 18)
-        self.assertEqual(self.character_1001.attributes.perception, 19)
-        self.assertEqual(self.character_1001.attributes.willpower, 20)
-
-    def test_update(self, mock_esi):
-        """can create attributes from scratch"""
-        mock_esi.client = esi_client_stub
-
-        CharacterAttributes.objects.create(
-            character=self.character_1001,
-            accrued_remap_cooldown_date="2020-10-24T09:00:00Z",
-            last_remap_date="2020-10-24T09:00:00Z",
-            bonus_remaps=4,
-            charisma=102,
-            intelligence=103,
-            memory=104,
-            perception=105,
-            willpower=106,
-        )
-
-        self.character_1001.update_attributes()
-        self.character_1001.attributes.refresh_from_db()
-
-        self.assertEqual(
-            self.character_1001.attributes.accrued_remap_cooldown_date,
-            parse_datetime("2016-10-24T09:00:00Z"),
-        )
-
-        self.assertEqual(
-            self.character_1001.attributes.last_remap_date,
-            parse_datetime("2016-10-24T09:00:00Z"),
-        )
-
-        self.assertEqual(self.character_1001.attributes.charisma, 16)
-        self.assertEqual(self.character_1001.attributes.intelligence, 17)
-        self.assertEqual(self.character_1001.attributes.memory, 18)
-        self.assertEqual(self.character_1001.attributes.perception, 19)
-        self.assertEqual(self.character_1001.attributes.willpower, 20)
-
-
-@patch(MODELS_PATH + ".character.esi")
-class TestCharacterUpdateMiningLedger(NoSocketsTestCase):
+@patch(MODULE_PATH + ".Character.update_section_content_hash")
+@patch(MODULE_PATH + ".Character.has_section_changed")
+class TestCharacterUpdateDataIfChangedOrForced(TestCase):
     @classmethod
-    def setUpClass(cls):
+    def setUpClass(cls) -> None:
         super().setUpClass()
-        load_eveuniverse()
         load_entities()
-        cls.character_1001 = create_memberaudit_character(1001)
-        cls.endpoints = [
-            EsiEndpoint(
-                "Industry",
-                "get_characters_character_id_mining",
-                "character_id",
-                needs_token=True,
-                data={
-                    "1001": [
-                        {
-                            "date": "2017-09-19",
-                            "quantity": 7004,
-                            "solar_system_id": 30002537,
-                            "type_id": 17471,
-                        },
-                        {
-                            "date": "2017-09-18",
-                            "quantity": 5199,
-                            "solar_system_id": 30002537,
-                            "type_id": 17471,
-                        },
-                    ]
-                },
-            ),
-        ]
-        cls.esi_client_stub = EsiClientStub.create_from_endpoints(cls.endpoints)
 
-    def test_should_add_new_entry_from_scratch(self, mock_esi):
+    @staticmethod
+    def _fetch_func_template(character):
+        return ["alpha"]
+
+    @staticmethod
+    def _store_func_template(character, data):
+        pass
+
+    def test_should_store_data_when_changed(
+        self, mock_has_section_changed, mock_update_section_content_hash
+    ):
         # given
-        mock_esi.client = self.esi_client_stub
+        character = create_memberaudit_character(1001)
+        fetch_func_mock = MagicMock(side_effect=self._fetch_func_template)
+        store_func_mock = MagicMock(side_effect=self._store_func_template)
+        mock_has_section_changed.return_value = True
         # when
-        with patch(MODELS_PATH + ".character.MEMBERAUDIT_DATA_RETENTION_LIMIT", None):
-            self.character_1001.update_mining_ledger()
-        # then
-        self.assertEqual(self.character_1001.mining_ledger.count(), 2)
-        obj = self.character_1001.mining_ledger.first()
-        self.assertEqual(obj.date, dt.date(2017, 9, 19))
-        self.assertEqual(obj.eve_type, EveType.objects.get(name="Dense Veldspar"))
-        self.assertEqual(
-            obj.eve_solar_system, EveSolarSystem.objects.get(name="Amamake")
-        )
-        self.assertEqual(obj.quantity, 7004)
-
-    def test_should_update_existing_entries(self, mock_esi):
-        # given
-        mock_esi.client = self.esi_client_stub
-        create_character_mining_ledger_entry(
-            character=self.character_1001,
-            date=dt.date(2017, 9, 19),
-            eve_solar_system=EveSolarSystem.objects.get(name="Amamake"),
-            eve_type=EveType.objects.get(name="Dense Veldspar"),
-            quantity=5,
+        result, changed = character.update_data_if_changed_or_forced(
+            section=character.UpdateSection.LOCATION,
+            fetch_func=fetch_func_mock,
+            store_func=store_func_mock,
+            force_update=False,
         )
-        # when
-        with patch(MODELS_PATH + ".character.MEMBERAUDIT_DATA_RETENTION_LIMIT", None):
-            self.character_1001.update_mining_ledger()
         # then
-        self.assertEqual(self.character_1001.mining_ledger.count(), 2)
-        obj = self.character_1001.mining_ledger.get(
-            date=dt.date(2017, 9, 19),
-            eve_solar_system=EveSolarSystem.objects.get(name="Amamake"),
-            eve_type=EveType.objects.get(name="Dense Veldspar"),
-        )
-        self.assertEqual(obj.quantity, 7004)
+        self.assertTrue(fetch_func_mock.called)
+        self.assertTrue(store_func_mock.called)
+        args, _ = store_func_mock.call_args
+        self.assertEqual(args[1], ["alpha"])
+        self.assertTrue(mock_update_section_content_hash.called)
+        _, kwargs = mock_update_section_content_hash.call_args
+        self.assertEqual(kwargs["content"], ["alpha"])
+        self.assertListEqual(result, ["alpha"])
+        self.assertTrue(changed)
 
-
-@patch(MODELS_PATH + ".character.esi")
-class TestCharacterUpdateFwStats(NoSocketsTestCase):
-    @classmethod
-    def setUpClass(cls):
-        super().setUpClass()
-        load_eveuniverse()
-        load_entities()
-        cls.character_1001 = create_memberaudit_character(1001)
-        cls.endpoints = [
-            EsiEndpoint(
-                "Faction_Warfare",
-                "get_characters_character_id_fw_stats",
-                "character_id",
-                needs_token=True,
-                data={
-                    "1001": {
-                        "current_rank": 3,
-                        "enlisted_on": dt.datetime(
-                            2023, 3, 21, 15, 0, tzinfo=dt.timezone.utc
-                        ),
-                        "faction_id": 500001,
-                        "highest_rank": 4,
-                        "kills": {
-                            "last_week": 893,
-                            "total": 684350,
-                            "yesterday": 136,
-                        },
-                        "victory_points": {
-                            "last_week": 102640,
-                            "total": 52658260,
-                            "yesterday": 15980,
-                        },
-                    }
-                },
-            ),
-        ]
-        cls.esi_client_stub = EsiClientStub.create_from_endpoints(cls.endpoints)
-
-    def test_should_add_new_entry_from_scratch(self, mock_esi):
+    def test_should_not_store_data_when_not_changed(
+        self, mock_has_section_changed, mock_update_section_content_hash
+    ):
         # given
-        mock_esi.client = self.esi_client_stub
+        character = create_memberaudit_character(1001)
+        fetch_func_mock = MagicMock(side_effect=self._fetch_func_template)
+        store_func_mock = MagicMock(side_effect=self._store_func_template)
+        mock_has_section_changed.return_value = False
         # when
-        with patch(MODELS_PATH + ".character.MEMBERAUDIT_DATA_RETENTION_LIMIT", None):
-            self.character_1001.update_fw_stats()
+        result, changed = character.update_data_if_changed_or_forced(
+            section=character.UpdateSection.LOCATION,
+            fetch_func=fetch_func_mock,
+            store_func=store_func_mock,
+            force_update=False,
+        )
         # then
-        obj: CharacterFwStats = self.character_1001.fw_stats
-        self.assertEqual(obj.current_rank, 3)
-        self.assertEqual(
-            obj.enlisted_on, dt.datetime(2023, 3, 21, 15, 0, tzinfo=dt.timezone.utc)
-        )
-        self.assertEqual(obj.faction_id, 500001)
-        self.assertEqual(obj.highest_rank, 4)
-        self.assertEqual(obj.kills_last_week, 893)
-        self.assertEqual(obj.kills_total, 684350)
-        self.assertEqual(obj.kills_yesterday, 136)
-        self.assertEqual(obj.victory_points_last_week, 102640)
-        self.assertEqual(obj.victory_points_total, 52658260)
-        self.assertEqual(obj.victory_points_yesterday, 15980)
-
-    def test_should_update_existing_entries(self, mock_esi):
-        # given
-        mock_esi.client = self.esi_client_stub
-        CharacterFwStats.objects.create(
-            character=self.character_1001,
-            kills_last_week=0,
-            kills_total=0,
-            kills_yesterday=0,
-            victory_points_last_week=0,
-            victory_points_total=0,
-            victory_points_yesterday=0,
+        self.assertTrue(fetch_func_mock.called)
+        self.assertFalse(store_func_mock.called)
+        self.assertFalse(mock_update_section_content_hash.called)
+        self.assertIsNone(result)
+        self.assertFalse(changed)
+
+    def test_should_always_store_data_when_forced(
+        self, mock_has_section_changed, mock_update_section_content_hash
+    ):
+        # given
+        character = create_memberaudit_character(1001)
+        fetch_func_mock = MagicMock(side_effect=self._fetch_func_template)
+        store_func_mock = MagicMock(side_effect=self._store_func_template)
+        mock_has_section_changed.return_value = False
+        # when
+        result, changed = character.update_data_if_changed_or_forced(
+            section=character.UpdateSection.LOCATION,
+            fetch_func=fetch_func_mock,
+            store_func=store_func_mock,
+            force_update=True,
         )
+        # then
+        self.assertTrue(fetch_func_mock.called)
+        self.assertTrue(store_func_mock.called)
+        self.assertTrue(mock_update_section_content_hash.called)
+        self.assertListEqual(result, ["alpha"])
+        self.assertTrue(changed)
+
+    def test_should_not_store_anything_when_esi_returns_http_500_and_return_none(
+        self, mock_has_section_changed, mock_update_section_content_hash
+    ):
+        # given
+        character = create_memberaudit_character(1001)
+        fetch_func_mock = MagicMock(side_effect=build_http_error(500, "Test exception"))
+        store_func_mock = MagicMock(side_effect=self._store_func_template)
+        mock_has_section_changed.side_effect = RuntimeError("Should not be called")
         # when
-        with patch(MODELS_PATH + ".character.MEMBERAUDIT_DATA_RETENTION_LIMIT", None):
-            self.character_1001.update_fw_stats()
+        result, changed = character.update_data_if_changed_or_forced(
+            section=character.UpdateSection.LOCATION,
+            fetch_func=fetch_func_mock,
+            store_func=store_func_mock,
+            force_update=False,
+        )
         # then
-        self.character_1001.refresh_from_db()
-        obj: CharacterFwStats = self.character_1001.fw_stats
-        self.assertEqual(obj.current_rank, 3)
-        self.assertEqual(
-            obj.enlisted_on, dt.datetime(2023, 3, 21, 15, 0, tzinfo=dt.timezone.utc)
-        )
-        self.assertEqual(obj.faction_id, 500001)
-        self.assertEqual(obj.highest_rank, 4)
-        self.assertEqual(obj.kills_last_week, 893)
-        self.assertEqual(obj.kills_total, 684350)
-        self.assertEqual(obj.kills_yesterday, 136)
-        self.assertEqual(obj.victory_points_last_week, 102640)
-        self.assertEqual(obj.victory_points_total, 52658260)
-        self.assertEqual(obj.victory_points_yesterday, 15980)
-
-    def test_should_add_new_entry_from_scratch_for_unlisted(self, mock_esi):
-        # given
-        endpoints = [
-            EsiEndpoint(
-                "Faction_Warfare",
-                "get_characters_character_id_fw_stats",
-                "character_id",
-                needs_token=True,
-                data={
-                    "1001": {
-                        "kills": {
-                            "last_week": 0,
-                            "total": 684350,
-                            "yesterday": 0,
-                        },
-                        "victory_points": {
-                            "last_week": 0,
-                            "total": 52658260,
-                            "yesterday": 0,
-                        },
-                    }
-                },
-            ),
-        ]
-        mock_esi.client = EsiClientStub.create_from_endpoints(endpoints)
+        self.assertTrue(fetch_func_mock.called)
+        self.assertFalse(store_func_mock.called)
+        self.assertFalse(mock_update_section_content_hash.called)
+        self.assertIsNone(result)
+        self.assertIsNone(changed)
+
+    def test_should_store_data_when_changed_and_use_hash_num(
+        self, mock_has_section_changed, mock_update_section_content_hash
+    ):
+        # given
+        character = create_memberaudit_character(1001)
+        fetch_func_mock = MagicMock(side_effect=self._fetch_func_template)
+        store_func_mock = MagicMock(side_effect=self._store_func_template)
+        mock_has_section_changed.return_value = True
         # when
-        with patch(MODELS_PATH + ".character.MEMBERAUDIT_DATA_RETENTION_LIMIT", None):
-            self.character_1001.update_fw_stats()
+        character.update_data_if_changed_or_forced(
+            section=character.UpdateSection.LOCATION,
+            fetch_func=fetch_func_mock,
+            store_func=store_func_mock,
+            force_update=False,
+            hash_num=2,
+        )
         # then
-        obj: CharacterFwStats = self.character_1001.fw_stats
-        self.assertIsNone(obj.current_rank)
-        self.assertIsNone(obj.enlisted_on)
-        self.assertIsNone(obj.faction)
-        self.assertIsNone(obj.highest_rank)
-        self.assertEqual(obj.kills_last_week, 0)
-        self.assertEqual(obj.kills_total, 684350)
-        self.assertEqual(obj.kills_yesterday, 0)
-        self.assertEqual(obj.victory_points_last_week, 0)
-        self.assertEqual(obj.victory_points_total, 52658260)
-        self.assertEqual(obj.victory_points_yesterday, 0)
-
-    @patch(MODELS_PATH + ".CharacterFwStats.objects.update_for_character")
-    def test_should_not_update_when_not_changed(
-        self, mock_update_for_character, mock_esi
+        self.assertTrue(fetch_func_mock.called)
+        self.assertTrue(store_func_mock.called)
+        args, _ = store_func_mock.call_args
+        self.assertEqual(args[1], ["alpha"])
+        _, kwargs = mock_has_section_changed.call_args
+        self.assertEqual(kwargs["hash_num"], 2)
+        _, kwargs = mock_update_section_content_hash.call_args
+        self.assertEqual(kwargs["hash_num"], 2)
+
+    def test_should_skip_storing_data_when_no_store_func_provided(
+        self, mock_has_section_changed, mock_update_section_content_hash
     ):
         # given
-        mock_esi.client = self.esi_client_stub
+        character = create_memberaudit_character(1001)
+        fetch_func_mock = MagicMock(side_effect=self._fetch_func_template)
+        mock_has_section_changed.return_value = True
         # when
-        with patch(
-            MODELS_PATH + ".Character.has_section_changed"
-        ) as mock_has_section_changed:
-            mock_has_section_changed.return_value = False
-            self.character_1001.update_fw_stats()
+        result, changed = character.update_data_if_changed_or_forced(
+            section=character.UpdateSection.LOCATION,
+            fetch_func=fetch_func_mock,
+            store_func=None,
+        )
         # then
-        self.assertFalse(mock_update_for_character.called)
+        self.assertTrue(fetch_func_mock.called)
+        self.assertTrue(mock_update_section_content_hash.called)
+        self.assertListEqual(result, ["alpha"])
+        self.assertTrue(changed)
```

### Comparing `aa_memberaudit-2.9.0/memberaudit/tests/models/test_general.py` & `aa_memberaudit-2.9.1/memberaudit/tests/models/test_general.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,20 @@
-import datetime as dt
-from unittest.mock import patch
-
 from django.contrib.auth.models import User
 from django.core.exceptions import ValidationError
-from django.test import TestCase
 from eveuniverse.models import EveSolarSystem, EveType
 
 from allianceauth.tests.auth_utils import AuthUtils
 from app_utils.testing import (
     NoSocketsTestCase,
     create_authgroup,
     create_user_from_evecharacter,
     queryset_pks,
 )
 
 from memberaudit.models import General, Location, MailEntity, SkillSetSkill
-from memberaudit.models.character import data_retention_cutoff
 
 from ..testdata.factories import (
     create_compliance_group_designation,
     create_skill_set,
     create_skill_set_skill,
 )
 from ..testdata.load_entities import load_entities
@@ -213,28 +208,14 @@
         result = General.accessible_users(user=self.user_1001)
         # then
         self.assertSetEqual(
             queryset_pks(result), {self.user_1001.pk, self.user_1002.pk}
         )
 
 
-class TestDataRetentionCutoff(TestCase):
-    @patch(MODELS_PATH + ".character.MEMBERAUDIT_DATA_RETENTION_LIMIT", 10)
-    def test_limit_is_set(self):
-        with patch(MODELS_PATH + ".character.now") as mock_now:
-            mock_now.return_value = dt.datetime(2020, 12, 19, 16, 15)
-            self.assertEqual(data_retention_cutoff(), dt.datetime(2020, 12, 9, 16, 0))
-
-    @patch(MODELS_PATH + ".character.MEMBERAUDIT_DATA_RETENTION_LIMIT", None)
-    def test_limit_not_set(self):
-        with patch(MODELS_PATH + ".character.now") as mock_now:
-            mock_now.return_value = dt.datetime(2020, 12, 19, 16, 15)
-            self.assertIsNone(data_retention_cutoff())
-
-
 class TestLocation(NoSocketsTestCase):
     @classmethod
     def setUpClass(cls) -> None:
         super().setUpClass()
         load_eveuniverse()
         load_entities()
         load_locations()
```

### Comparing `aa_memberaudit-2.9.0/memberaudit/tests/models/test_sections.py` & `aa_memberaudit-2.9.1/memberaudit/tests/models/test_character_sections.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/tests/test_admin.py` & `aa_memberaudit-2.9.1/memberaudit/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/tests/test_auth_hooks.py` & `aa_memberaudit-2.9.1/memberaudit/tests/test_auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/tests/test_checks.py` & `aa_memberaudit-2.9.1/memberaudit/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/tests/test_commands.py` & `aa_memberaudit-2.9.1/memberaudit/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/tests/test_decorators.py` & `aa_memberaudit-2.9.1/memberaudit/tests/test_decorators.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,28 +92,28 @@
         load_entities()
 
     def setUp(self) -> None:
         self.character = create_memberaudit_character(1001)
 
     def test_defaults(self):
         @fetch_token_for_character()
-        def dummy(character, token):
+        def dummy(self, character, token):
             self.assertIsInstance(token, Token)
             self.assertSetEqual(scope_names_set(token), set(Character.get_esi_scopes()))
 
-        dummy(self.character)
+        dummy(self, self.character)
 
     def test_specified_scope(self):
         @fetch_token_for_character("esi-mail.read_mail.v1")
-        def dummy(character, token):
+        def dummy(self, character, token):
             self.assertIsInstance(token, Token)
             self.assertIn("esi-mail.read_mail.v1", scope_names_set(token))
 
-        dummy(self.character)
+        dummy(self, self.character)
 
     def test_exceptions_if_not_found(self):
         @fetch_token_for_character("invalid_scope")
-        def dummy(character, token):
+        def dummy(self, character, token):
             pass
 
         with self.assertRaises(TokenError):
-            dummy(self.character)
+            dummy(self, self.character)
```

### Comparing `aa_memberaudit-2.9.0/memberaudit/tests/test_factories.py` & `aa_memberaudit-2.9.1/memberaudit/tests/test_factories.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/tests/test_forms.py` & `aa_memberaudit-2.9.1/memberaudit/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/tests/test_helpers.py` & `aa_memberaudit-2.9.1/memberaudit/tests/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from allianceauth.eveonline.models import EveCorporationInfo
 from app_utils.testing import (
     create_authgroup,
     create_state,
     create_user_from_evecharacter,
 )
 
-from memberaudit.helpers import (
+from memberaudit.utils import (
     clear_users_from_group,
     filter_groups_available_to_user,
     get_unidecoded_slug,
 )
 
 from .testdata.load_entities import load_entities
```

### Comparing `aa_memberaudit-2.9.0/memberaudit/tests/test_integration.py` & `aa_memberaudit-2.9.1/memberaudit/tests/test_integration.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 import datetime as dt
 from unittest.mock import MagicMock, patch
 
 from django.test import TestCase, override_settings
 from django.urls import reverse
+from django.utils.dateparse import parse_datetime
 from django.utils.timezone import now
 from django_webtest import WebTest
 from eveuniverse.models import EveEntity, EveType
 
 from allianceauth.tests.auth_utils import AuthUtils
 from app_utils.esi import EsiStatus, fetch_esi_status
+from app_utils.testing import NoSocketsTestCase
 
 from memberaudit import tasks
 from memberaudit.models import (
     Character,
     CharacterAsset,
     CharacterContract,
     CharacterContractItem,
     CharacterMail,
     CharacterMailLabel,
     Location,
     MailEntity,
 )
 
-from .testdata.esi_client_stub import esi_client_stub
+from .testdata.esi_client_stub import esi_client_stub, esi_stub
 from .testdata.load_entities import load_entities
 from .testdata.load_eveuniverse import load_eveuniverse
 from .testdata.load_locations import load_locations
 from .utils import (
+    CharacterUpdateTestDataMixin,
     add_auth_character_to_user,
     add_memberaudit_character_to_user,
-    clear_celery_once_locks,
     create_memberaudit_character,
     create_user_from_evecharacter_with_access,
 )
 
 MANAGERS_PATH = "memberaudit.managers"
 MODELS_PATH = "memberaudit.models"
 TASKS_PATH = "memberaudit.tasks"
@@ -45,15 +47,14 @@
 
     @classmethod
     def setUpClass(cls):
         super().setUpClass()
         load_eveuniverse()
         load_entities()
         load_locations()
-        clear_celery_once_locks()
 
     def setUp(self) -> None:
         self.user, _ = create_user_from_evecharacter_with_access(1002)
 
     def test_open_character_viewer(self):
         """
         given user has character registered
@@ -71,24 +72,26 @@
         # user clicks on character link
         character_viewer = launcher.click(
             href=reverse("memberaudit:character_viewer", args=[character.pk]),
             index=0,  # follow the first matching link
         )
         self.assertEqual(character_viewer.status_code, 200)
 
-    @patch(MODELS_PATH + ".character.esi")
+    @patch(MANAGERS_PATH + ".character_sections_1.esi", esi_stub)
+    @patch(MANAGERS_PATH + ".character_sections_2.esi", esi_stub)
+    @patch(MANAGERS_PATH + ".character_sections_3.esi", esi_stub)
+    @patch(MANAGERS_PATH + ".general.esi", esi_stub)
     @override_settings(
         CELERY_ALWAYS_EAGER=True, CELERY_EAGER_PROPAGATES_EXCEPTIONS=True
     )
-    def test_add_character(self, mock_esi):
+    def test_add_character(self):
         """
         when clicking on "register"
         then user can add a new character
         """
-        mock_esi.client = esi_client_stub
         # user as another auth character
         character_ownership_1001 = add_auth_character_to_user(self.user, 1001)
 
         # login & open launcher page
         self.app.set_user(self.user)
         launcher = self.app.get(reverse("memberaudit:launcher"))
         self.assertEqual(launcher.status_code, 200)
@@ -325,32 +328,97 @@
         self.assertIn(body_text, mail_details.text)
 
 
 @patch(
     TASKS_PATH + ".Character.objects.get_cached",
     lambda pk, timeout: Character.objects.get(pk=pk),
 )
-@patch(TASKS_PATH + ".fetch_esi_status", MagicMock(spec=fetch_esi_status))
+@patch(TASKS_PATH + ".fetch_esi_status", lambda: EsiStatus(True, 99, 60))
 @patch(MANAGERS_PATH + ".general.fetch_esi_status", lambda: EsiStatus(True, 99, 60))
 @patch(TASKS_PATH + ".MEMBERAUDIT_LOG_UPDATE_STATS", False)
-@patch(MODELS_PATH + ".character.MEMBERAUDIT_DATA_RETENTION_LIMIT", None)
-@patch(MODELS_PATH + ".character.esi")
+@patch(MANAGERS_PATH + ".character_sections_1.data_retention_cutoff", lambda: None)
+@patch(MANAGERS_PATH + ".character_sections_2.data_retention_cutoff", lambda: None)
+@patch(MANAGERS_PATH + ".character_sections_3.data_retention_cutoff", lambda: None)
+@patch(MANAGERS_PATH + ".character_sections_1.esi", esi_stub)
+@patch(MANAGERS_PATH + ".character_sections_2.esi", esi_stub)
+@patch(MANAGERS_PATH + ".character_sections_3.esi", esi_stub)
+@patch(MANAGERS_PATH + ".general.esi", esi_stub)
 @override_settings(CELERY_ALWAYS_EAGER=True, CELERY_EAGER_PROPAGATES_EXCEPTIONS=True)
 class TestTasksE2E(TestCase):
     fixtures = ["disable_analytics.json"]
 
     @classmethod
     def setUpClass(cls) -> None:
         super().setUpClass()
         load_eveuniverse()
         load_entities()
         load_locations()
-        clear_celery_once_locks()
 
-    def test_should_update_all_characters(self, mock_esi):
+    def test_should_update_all_characters(self):
         # given
-        mock_esi.client = esi_client_stub
         character_1001 = create_memberaudit_character(1001)
         # when
         tasks.update_all_characters()
         # then
         self.assertTrue(character_1001.is_update_status_ok())
+
+
+@patch(MANAGERS_PATH + ".character_sections_2.esi")
+@patch(MANAGERS_PATH + ".general.esi")
+class TestCharacterMailUpdate(CharacterUpdateTestDataMixin, NoSocketsTestCase):
+    @staticmethod
+    def stub_eve_entity_get_or_create_esi(id, *args, **kwargs):
+        """will return EveEntity if it exists else None, False"""
+        try:
+            obj = EveEntity.objects.get(id=id)
+            return obj, True
+        except EveEntity.DoesNotExist:
+            return None, False
+
+    @patch(MANAGERS_PATH + ".character_sections_2.data_retention_cutoff", lambda: None)
+    @patch(MANAGERS_PATH + ".character_sections_2.EveEntity.objects.get_or_create_esi")
+    def test_update_mail_headers_2(
+        self,
+        mock_eve_entity,
+        mock_esi_character,
+        mock_esi_sections,
+    ):
+        """can update existing mail"""
+        mock_esi_character.client = esi_client_stub
+        mock_esi_sections.client = esi_client_stub
+        mock_eve_entity.side_effect = self.stub_eve_entity_get_or_create_esi
+        sender, _ = MailEntity.objects.update_or_create_from_eve_entity_id(id=1002)
+        mail = CharacterMail.objects.create(
+            character=self.character_1001,
+            mail_id=1,
+            sender=sender,
+            subject="Mail 1",
+            timestamp=parse_datetime("2015-09-05T16:07:00Z"),
+            is_read=False,  # to be updated
+        )
+        recipient_1, _ = MailEntity.objects.update_or_create_from_eve_entity_id(id=1001)
+        recipient_2 = MailEntity.objects.create(
+            id=9001, category=MailEntity.Category.MAILING_LIST, name="Dummy 2"
+        )
+        mail.recipients.set([recipient_1, recipient_2])
+
+        self.character_1001.update_mailing_lists()
+        self.character_1001.update_mail_labels()
+
+        label = self.character_1001.mail_labels.get(label_id=17)
+        mail.labels.add(label)  # to be updated
+
+        self.character_1001.update_mail_headers()
+        self.assertSetEqual(
+            set(self.character_1001.mails.values_list("mail_id", flat=True)),
+            {1, 2, 3},
+        )
+
+        obj = self.character_1001.mails.get(mail_id=1)
+        self.assertEqual(obj.sender_id, 1002)
+        self.assertTrue(obj.is_read)
+        self.assertEqual(obj.subject, "Mail 1")
+        self.assertEqual(obj.timestamp, parse_datetime("2015-09-05T16:07:00Z"))
+        self.assertFalse(obj.body)
+        self.assertTrue(obj.recipients.filter(id=1001).exists())
+        self.assertTrue(obj.recipients.filter(id=9001).exists())
+        self.assertSetEqual(set(obj.labels.values_list("label_id", flat=True)), {3})
```

### Comparing `aa_memberaudit-2.9.0/memberaudit/tests/test_signals.py` & `aa_memberaudit-2.9.1/memberaudit/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/tests/test_tasks.py` & `aa_memberaudit-2.9.1/memberaudit/tests/test_tasks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import datetime as dt
-from unittest import skip
+from unittest import skipIf
 from unittest.mock import MagicMock, patch
 
 from celery.exceptions import Retry as CeleryRetry
 
 from django.test import override_settings
 from django.utils.timezone import now
 from esi.models import Token
@@ -30,20 +30,20 @@
 from memberaudit.models import (
     Character,
     CharacterAsset,
     CharacterUpdateStatus,
     Location,
 )
 
-from .testdata.esi_client_stub import esi_client_error_stub, esi_client_stub
+from .testdata.esi_client_stub import esi_client_stub, esi_error_stub, esi_stub
 from .testdata.factories import create_character, create_compliance_group_designation
 from .testdata.load_entities import load_entities
 from .testdata.load_eveuniverse import load_eveuniverse
 from .testdata.load_locations import load_locations
-from .utils import clear_celery_once_locks, create_memberaudit_character
+from .utils import TOX_IS_RUNNING, create_memberaudit_character
 
 MODELS_PATH = "memberaudit.models"
 MANAGERS_PATH = "memberaudit.managers"
 TASKS_PATH = "memberaudit.tasks"
 
 
 class TestCaseTasks(NoSocketsTestCase):
@@ -90,15 +90,15 @@
     def test_update_market_prices(self, mock_update_from_esi):
         tasks.update_market_prices()
         self.assertTrue(mock_update_from_esi.called)
 
 
 @override_settings(CELERY_ALWAYS_EAGER=True)  # need to ignore exceptions
 @patch(TASKS_PATH + ".fetch_esi_status", MagicMock(spec=fetch_esi_status))
-@patch(MODELS_PATH + ".character.esi")
+@patch(MANAGERS_PATH + ".character_sections_1.esi")
 class TestUpdateCharacterAssets(TestCaseTasks):
     @classmethod
     def setUpClass(cls) -> None:
         super().setUpClass()
         load_eveuniverse()
         load_entities()
         load_locations()
@@ -284,64 +284,67 @@
         )
         self.assertTrue(status.is_success)
         self.assertFalse(status.last_error_message)
 
     def test_update_assets_6(self, mock_esi):
         """when update failed then report the error"""
         # given
-        exception = build_http_error(500, "Test exception")
+        exception = build_http_error(502, "Test exception")
         mock_esi.client.Assets.get_characters_character_id_assets.side_effect = (
             exception
         )
         # when
         with self.assertRaises(OSError):
             tasks.update_character_assets(self.character_1001.pk)
         # then
         status = self.character_1001.update_status_set.get(
             section=Character.UpdateSection.ASSETS
         )
         self.assertFalse(status.is_success)
         self.assertEqual(
-            status.last_error_message, "HTTPInternalServerError: 500 Test exception"
+            status.last_error_message, "HTTPBadGateway: 502 Test exception"
         )
 
     def test_update_assets_7(self, mock_esi):
         """when preload objects failed then report the error"""
         mock_esi.client = esi_client_stub
 
-        with patch(MODELS_PATH + ".character.Location", spec=True) as m:
-            exception = build_http_error(500, "Test exception")
-            m.objects.get_or_create_esi_async.side_effect = exception
+        with patch(
+            MANAGERS_PATH + ".general.LocationManager.get_or_create_esi_async",
+            spec=True,
+        ) as m:
+            exception = build_http_error(502, "Test exception")
+            m.side_effect = exception
             with self.assertRaises(OSError):
                 tasks.update_character_assets(self.character_1001.pk)
 
         status = self.character_1001.update_status_set.get(
             section=Character.UpdateSection.ASSETS
         )
         self.assertFalse(status.is_success)
         self.assertEqual(
-            status.last_error_message, "HTTPInternalServerError: 500 Test exception"
+            status.last_error_message, "HTTPBadGateway: 502 Test exception"
         )
 
     def test_update_assets_8(self, mock_esi):
         """when building the asset tree failed then report the error"""
         mock_esi.client = esi_client_stub
 
-        with patch(MODELS_PATH + ".character.logger") as m:
-            exception = build_http_error(500, "Test exception")
+        with patch(MANAGERS_PATH + ".character_sections_1.logger") as m:
+            exception = build_http_error(502, "Test exception")
             m.info.side_effect = exception
             with self.assertRaises(OSError):
                 tasks.update_character_assets(self.character_1001.pk)
 
         status = self.character_1001.update_status_set.get(
             section=Character.UpdateSection.ASSETS
         )
         self.assertFalse(status.is_success)
         self.assertEqual(
-            status.last_error_message, "HTTPInternalServerError: 500 Test exception"
+            status.last_error_message, "HTTPBadGateway: 502 Test exception"
         )
 
     def test_update_assets_9(self, mock_esi):
         """when info from ESI has not change, then don't re-create asset tree"""
         mock_esi.client = esi_client_stub
 
         self.character_1001.reset_update_section(Character.UpdateSection.ASSETS)
@@ -378,160 +381,164 @@
         )
         self.assertTrue(status.is_success)
 
 
 @override_settings(CELERY_ALWAYS_EAGER=True, CELERY_EAGER_PROPAGATES_EXCEPTIONS=True)
 @patch(TASKS_PATH + ".fetch_esi_status", MagicMock(spec=fetch_esi_status))
 @patch(MANAGERS_PATH + ".general.fetch_esi_status", lambda: EsiStatus(True, 99, 60))
-@patch(MODELS_PATH + ".character.esi")
-class TestUpdateCharacterMails(TestCaseTasks):
+@patch(MANAGERS_PATH + ".character_sections_1.esi")
+class TestUpdateCharacterContacts(TestCaseTasks):
     @classmethod
     def setUpClass(cls) -> None:
         super().setUpClass()
         load_eveuniverse()
         load_entities()
         cls.character_1001 = create_memberaudit_character(1001)
         cls.token = (
             cls.character_1001.eve_character.character_ownership.user.token_set.first()
         )
 
     def test_update_ok(self, mock_esi):
         """when update succeeded then report update success"""
         mock_esi.client = esi_client_stub
 
-        tasks.update_character_mails(self.character_1001.pk)
+        tasks.update_character_contacts(self.character_1001.pk)
 
         status = self.character_1001.update_status_set.get(
-            section=Character.UpdateSection.MAILS
+            section=Character.UpdateSection.CONTACTS
         )
         self.assertTrue(status.is_success)
         self.assertFalse(status.last_error_message)
 
     def test_detect_error(self, mock_esi):
         """when update failed then report the error"""
-        exception = build_http_error(500, "Test exception")
-        mock_esi.client.Mail.get_characters_character_id_mail_lists.side_effect = (
+        exception = build_http_error(502, "Test exception")
+        mock_esi.client.Contacts.get_characters_character_id_contacts_labels.side_effect = (
             exception
         )
 
         try:
-            tasks.update_character_mails(self.character_1001.pk)
+            tasks.update_character_contacts(self.character_1001.pk)
         except Exception:
             status = self.character_1001.update_status_set.get(
-                section=Character.UpdateSection.MAILS
+                section=Character.UpdateSection.CONTACTS
             )
             self.assertFalse(status.is_success)
             self.assertEqual(
-                status.last_error_message, "HTTPInternalServerError: 500 Test exception"
+                status.last_error_message, "HTTPBadGateway: 502 Test exception"
             )
         else:
             self.assertTrue(False)  # Hack to ensure the test fails when it gets here
 
 
 @override_settings(CELERY_ALWAYS_EAGER=True, CELERY_EAGER_PROPAGATES_EXCEPTIONS=True)
 @patch(TASKS_PATH + ".fetch_esi_status", MagicMock(spec=fetch_esi_status))
 @patch(MANAGERS_PATH + ".general.fetch_esi_status", lambda: EsiStatus(True, 99, 60))
-@patch(MODELS_PATH + ".character.esi")
-class TestUpdateCharacterContacts(TestCaseTasks):
+@patch(MANAGERS_PATH + ".character_sections_1.esi")
+class TestUpdateCharacterContracts(TestCaseTasks):
     @classmethod
     def setUpClass(cls) -> None:
         super().setUpClass()
         load_eveuniverse()
         load_entities()
+        load_locations()
         cls.character_1001 = create_memberaudit_character(1001)
         cls.token = (
             cls.character_1001.eve_character.character_ownership.user.token_set.first()
         )
 
     def test_update_ok(self, mock_esi):
         """when update succeeded then report update success"""
         mock_esi.client = esi_client_stub
 
-        tasks.update_character_contacts(self.character_1001.pk)
+        tasks.update_character_contracts(self.character_1001.pk)
 
         status = self.character_1001.update_status_set.get(
-            section=Character.UpdateSection.CONTACTS
+            section=Character.UpdateSection.CONTRACTS
         )
         self.assertTrue(status.is_success)
         self.assertFalse(status.last_error_message)
 
     def test_detect_error(self, mock_esi):
         """when update failed then report the error"""
-        exception = build_http_error(500, "Test exception")
-        mock_esi.client.Contacts.get_characters_character_id_contacts_labels.side_effect = (
+        exception = build_http_error(502, "Test exception")
+        mock_esi.client.Contracts.get_characters_character_id_contracts.side_effect = (
             exception
         )
 
         try:
-            tasks.update_character_contacts(self.character_1001.pk)
+            tasks.update_character_contracts(self.character_1001.pk)
         except Exception:
             status = self.character_1001.update_status_set.get(
-                section=Character.UpdateSection.CONTACTS
+                section=Character.UpdateSection.CONTRACTS
             )
             self.assertFalse(status.is_success)
             self.assertEqual(
-                status.last_error_message, "HTTPInternalServerError: 500 Test exception"
+                status.last_error_message, "HTTPBadGateway: 502 Test exception"
             )
         else:
             self.assertTrue(False)  # Hack to ensure the test fails when it gets here
 
 
 @override_settings(CELERY_ALWAYS_EAGER=True, CELERY_EAGER_PROPAGATES_EXCEPTIONS=True)
 @patch(TASKS_PATH + ".fetch_esi_status", MagicMock(spec=fetch_esi_status))
 @patch(MANAGERS_PATH + ".general.fetch_esi_status", lambda: EsiStatus(True, 99, 60))
-@patch(MODELS_PATH + ".character.esi")
-class TestUpdateCharacterContracts(TestCaseTasks):
+@patch(MANAGERS_PATH + ".character_sections_2.esi")
+@patch(MANAGERS_PATH + ".general.esi")
+class TestUpdateCharacterMails(TestCaseTasks):
     @classmethod
     def setUpClass(cls) -> None:
         super().setUpClass()
         load_eveuniverse()
         load_entities()
-        load_locations()
         cls.character_1001 = create_memberaudit_character(1001)
         cls.token = (
             cls.character_1001.eve_character.character_ownership.user.token_set.first()
         )
 
-    def test_update_ok(self, mock_esi):
+    def test_update_ok(self, mock_esi_character, mock_esi_sections):
         """when update succeeded then report update success"""
-        mock_esi.client = esi_client_stub
+        mock_esi_character.client = esi_client_stub
+        mock_esi_sections.client = esi_client_stub
 
-        tasks.update_character_contracts(self.character_1001.pk)
+        tasks.update_character_mails(self.character_1001.pk)
 
         status = self.character_1001.update_status_set.get(
-            section=Character.UpdateSection.CONTRACTS
+            section=Character.UpdateSection.MAILS
         )
         self.assertTrue(status.is_success)
         self.assertFalse(status.last_error_message)
 
-    def test_detect_error(self, mock_esi):
+    def test_detect_error(self, mock_esi_character, mock_esi_sections):
         """when update failed then report the error"""
-        exception = build_http_error(500, "Test exception")
-        mock_esi.client.Contracts.get_characters_character_id_contracts.side_effect = (
+        exception = build_http_error(502, "Test exception")
+        mock_esi_character.client.Mail.get_characters_character_id_mail_lists.side_effect = (
+            exception
+        )
+        mock_esi_sections.client.Mail.get_characters_character_id_mail_lists.side_effect = (
             exception
         )
-
         try:
-            tasks.update_character_contracts(self.character_1001.pk)
+            tasks.update_character_mails(self.character_1001.pk)
         except Exception:
             status = self.character_1001.update_status_set.get(
-                section=Character.UpdateSection.CONTRACTS
+                section=Character.UpdateSection.MAILS
             )
             self.assertFalse(status.is_success)
             self.assertEqual(
-                status.last_error_message, "HTTPInternalServerError: 500 Test exception"
+                status.last_error_message, "HTTPBadGateway: 502 Test exception"
             )
         else:
             self.assertTrue(False)  # Hack to ensure the test fails when it gets here
 
 
 @override_settings(CELERY_ALWAYS_EAGER=True, CELERY_EAGER_PROPAGATES_EXCEPTIONS=True)
 @patch(TASKS_PATH + ".fetch_esi_status", MagicMock(spec=fetch_esi_status))
 @patch(MANAGERS_PATH + ".general.fetch_esi_status", lambda: EsiStatus(True, 99, 60))
-@patch(MODELS_PATH + ".character.esi")
+@patch(MANAGERS_PATH + ".character_sections_3.esi")
 class TestUpdateCharacterWalletJournal(TestCaseTasks):
     @classmethod
     def setUpClass(cls) -> None:
         super().setUpClass()
         load_eveuniverse()
         load_entities()
         cls.character_1001 = create_memberaudit_character(1001)
@@ -549,163 +556,182 @@
             section=Character.UpdateSection.WALLET_JOURNAL
         )
         self.assertTrue(status.is_success)
         self.assertFalse(status.last_error_message)
 
     def test_detect_error(self, mock_esi):
         """when update failed then report the error"""
-        exception = build_http_error(500, "Test exception")
+        exception = build_http_error(502, "Test exception")
         mock_esi.client.Wallet.get_characters_character_id_wallet_journal.side_effect = (
             exception
         )
 
         try:
             tasks.update_character_wallet_journal(self.character_1001.pk)
         except Exception:
             status = self.character_1001.update_status_set.get(
                 section=Character.UpdateSection.WALLET_JOURNAL
             )
             self.assertFalse(status.is_success)
             self.assertEqual(
-                status.last_error_message, "HTTPInternalServerError: 500 Test exception"
+                status.last_error_message, "HTTPBadGateway: 502 Test exception"
             )
         else:
             self.assertTrue(False)  # Hack to ensure the test fails when it gets here
 
 
-@patch(MODELS_PATH + ".character.MEMBERAUDIT_DATA_RETENTION_LIMIT", None)
-@patch(TASKS_PATH + ".fetch_esi_status", MagicMock(spec=fetch_esi_status))
+@patch(TASKS_PATH + ".fetch_esi_status", lambda: EsiStatus(True, 99, 60))
 @patch(MANAGERS_PATH + ".general.fetch_esi_status", lambda: EsiStatus(True, 99, 60))
-@patch(MODELS_PATH + ".character.esi")
+@patch(MANAGERS_PATH + ".character_sections_1.data_retention_cutoff", lambda: None)
+@patch(MANAGERS_PATH + ".character_sections_2.data_retention_cutoff", lambda: None)
+@patch(MANAGERS_PATH + ".character_sections_3.data_retention_cutoff", lambda: None)
+@patch(MANAGERS_PATH + ".character_sections_1.esi", esi_stub)
+@patch(MANAGERS_PATH + ".character_sections_2.esi", esi_stub)
+@patch(MANAGERS_PATH + ".character_sections_3.esi", esi_stub)
+@patch(MANAGERS_PATH + ".general.esi", esi_stub)
 @override_settings(CELERY_ALWAYS_EAGER=True, CELERY_EAGER_PROPAGATES_EXCEPTIONS=True)
-class TestUpdateCharacter(TestCaseTasks):
+class TestCharacterUpdateFull(TestCaseTasks):
     @classmethod
     def setUpClass(cls) -> None:
         super().setUpClass()
         load_eveuniverse()
         load_entities()
         load_locations()
 
     def setUp(self) -> None:
         self.character_1001 = create_memberaudit_character(1001)
-        clear_celery_once_locks()
 
-    @skip  # temporary disabled because it does not work in tox
-    def test_should_update_normally(self, mock_esi):
+    @skipIf(TOX_IS_RUNNING, "does not work with tox")
+    def test_should_update_normally(self):
         """can update from scratch"""
-        mock_esi.client = esi_client_stub
-
+        # when
         result = tasks.update_character(self.character_1001.pk)
+        # then
         self.assertTrue(result)
         self.assertTrue(self.character_1001.is_update_status_ok())
 
-    def test_should_report_errors_during_updates(self, mock_esi):
-        mock_esi.client = esi_client_error_stub
-
-        with self.assertRaises(OSError):  # raised when trying to fetch attributes
-            tasks.update_character(self.character_1001.pk)
-
-        self.assertFalse(self.character_1001.is_update_status_ok())
-
-        status = self.character_1001.update_status_set.get(
-            character=self.character_1001,
-            section=Character.UpdateSection.ATTRIBUTES,
-        )
-        self.assertFalse(status.is_success)
-        self.assertEqual(
-            status.last_error_message, "HTTPInternalServerError: 500 Test exception"
-        )
-        self.assertTrue(status.finished_at)
-
     @patch(TASKS_PATH + ".Character.update_loyalty", spec=True)
-    def test_should_update_stale_sections_only_1(self, update_loyalty, mock_esi):
-        """normal section"""
-        mock_esi.client = esi_client_stub
+    def test_should_update_normal_section_only_when_stale(self, update_loyalty):
+        # given
         CharacterUpdateStatus.objects.create(
             character=self.character_1001,
             section=Character.UpdateSection.LOYALTY,
             is_success=True,
             started_at=now() - dt.timedelta(seconds=30),
             finished_at=now(),
         )
-
+        # when
         tasks.update_character(self.character_1001.pk)
-
+        # then
         self.assertFalse(update_loyalty.called)
 
     @patch(TASKS_PATH + ".update_character_mails", spec=True)
-    def test_should_update_stale_sections_only_2(
-        self, mock_update_character_mails, mock_esi
+    def test_should_update_special_section_only_when_stale(
+        self, mock_update_character_mails
     ):
-        """special section"""
-        mock_esi.client = esi_client_stub
+        # given
         CharacterUpdateStatus.objects.create(
             character=self.character_1001,
             section=Character.UpdateSection.MAILS,
             is_success=True,
             started_at=now() - dt.timedelta(seconds=30),
             finished_at=now(),
         )
-
+        # when
         tasks.update_character(self.character_1001.pk)
-
+        # then
         self.assertFalse(mock_update_character_mails.apply_async.called)
 
-    @patch(TASKS_PATH + ".Character.update_skills", spec=True)
-    def test_should_update_stale_sections_only_3(self, mock_update_skills, mock_esi):
+    def test_should_update_stale_sections_only_3(self):
         """When generic section has recently been updated and force_update is called
         then update again
         """
-        mock_esi.client = esi_client_stub
-        CharacterUpdateStatus.objects.create(
+        # given
+        section: CharacterUpdateStatus = CharacterUpdateStatus.objects.create(
             character=self.character_1001,
-            section=Character.UpdateSection.SKILLS,
+            section=Character.UpdateSection.SKILLS.value,
             is_success=True,
             started_at=now() - dt.timedelta(seconds=30),
             finished_at=now(),
         )
-
+        last_finished = section.finished_at
+        # when
         tasks.update_character(self.character_1001.pk, force_update=True)
+        # then
+        section.refresh_from_db()
+        self.assertGreater(section.finished_at, last_finished)
 
-        self.assertTrue(mock_update_skills.called)
-
-    def test_no_update_required(self, mock_esi):
-        """Do not update anything when not required"""
-        mock_esi.client = esi_client_stub
+    def test_should_do_nothing_when_not_required(self):
+        # given
         for section in Character.UpdateSection.values:
             CharacterUpdateStatus.objects.create(
                 character=self.character_1001,
                 section=section,
                 is_success=True,
                 started_at=now() - dt.timedelta(seconds=30),
                 finished_at=now(),
             )
-
+        # when
         result = tasks.update_character(self.character_1001.pk)
+        # then
         self.assertFalse(result)
 
-    def test_update_forced(self, mock_esi):
-        """Can do forced update"""
-        mock_esi.client = esi_client_stub
-
+    def test_can_do_forced_update(self):
+        # when
         result = tasks.update_character(self.character_1001.pk, force_update=True)
+        # then
         self.assertTrue(result)
         self.assertTrue(self.character_1001.is_update_status_ok())
 
-    def test_skip_update_for_orphans(self, mock_esi):
+    def test_skip_update_for_orphans(self):
         # given
-        mock_esi.client = esi_client_stub
         character = create_character(EveCharacter.objects.get(character_id=1121))
         # when
         result = tasks.update_character(character.pk)
         # then
         self.assertFalse(result)
         self.assertIsNone(character.is_update_status_ok())
 
 
+@patch(TASKS_PATH + ".fetch_esi_status", lambda: EsiStatus(True, 99, 60))
+@patch(MANAGERS_PATH + ".general.fetch_esi_status", lambda: EsiStatus(True, 99, 60))
+@patch(MANAGERS_PATH + ".character_sections_1.data_retention_cutoff", lambda: None)
+@patch(MANAGERS_PATH + ".character_sections_2.data_retention_cutoff", lambda: None)
+@patch(MANAGERS_PATH + ".character_sections_3.data_retention_cutoff", lambda: None)
+@patch(MANAGERS_PATH + ".character_sections_1.esi", esi_error_stub)
+@patch(MANAGERS_PATH + ".character_sections_2.esi", esi_error_stub)
+@patch(MANAGERS_PATH + ".character_sections_3.esi", esi_error_stub)
+@patch(MANAGERS_PATH + ".general.esi", esi_error_stub)
+@override_settings(CELERY_ALWAYS_EAGER=True, CELERY_EAGER_PROPAGATES_EXCEPTIONS=True)
+class TestCharacterUpdateErrorReporting(TestCaseTasks):
+    @classmethod
+    def setUpClass(cls) -> None:
+        super().setUpClass()
+        load_eveuniverse()
+        load_entities()
+        load_locations()
+
+    def setUp(self) -> None:
+        self.character_1001 = create_memberaudit_character(1001)
+
+    def test_should_report_errors_during_updates(self):
+        # when
+        with self.assertRaises(OSError):  # raised when trying to fetch attributes
+            tasks.update_character(self.character_1001.pk)
+        # then
+        self.assertFalse(self.character_1001.is_update_status_ok())
+        status = self.character_1001.update_status_set.filter(
+            character=self.character_1001, is_success=False
+        ).first()
+        self.assertEqual(
+            status.last_error_message, "HTTPBadGateway: 502 Test exception"
+        )
+        self.assertTrue(status.finished_at)
+
+
 @patch(TASKS_PATH + ".fetch_esi_status", MagicMock(spec=fetch_esi_status))
 @patch(MANAGERS_PATH + ".general.fetch_esi_status", lambda: EsiStatus(True, 99, 60))
 @patch(TASKS_PATH + ".Location.objects.structure_update_or_create_esi", spec=True)
 class TestUpdateStructureEsi(TestCaseTasks):
     @classmethod
     def setUpClass(cls) -> None:
         super().setUpClass()
@@ -781,15 +807,15 @@
     def setUpClass(cls) -> None:
         super().setUpClass()
         load_entities()
 
     def setUp(self) -> None:
         self.character_1001 = create_memberaudit_character(1001)
 
-    @patch(MODELS_PATH + ".character.Character.update_skill_sets")
+    @patch(MODELS_PATH + ".characters.Character.update_skill_sets")
     def test_normal(self, mock_update_skill_sets):
         tasks.update_characters_skill_checks()
         self.assertTrue(mock_update_skill_sets.called)
 
 
 @override_settings(CELERY_ALWAYS_EAGER=True, CELERY_EAGER_PROPAGATES_EXCEPTIONS=True)
 class TestDeleteCharacter(TestCaseTasks):
```

### Comparing `aa_memberaudit-2.9.0/memberaudit/tests/test_templatetags.py` & `aa_memberaudit-2.9.1/memberaudit/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/tests/testdata/create_eveuniverse.py` & `aa_memberaudit-2.9.1/memberaudit/tests/testdata/create_eveuniverse.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Create testdata for eveuniverse models by fetching them from ESI."""
+
 from django.test import TestCase
 from eveuniverse.models import EveUniverseEntityModel
 from eveuniverse.tools.testdata import ModelSpec, create_testdata
 
 from memberaudit.constants import EveCategoryId
 
 from . import eveuniverse_test_data_filename
```

### Comparing `aa_memberaudit-2.9.0/memberaudit/tests/testdata/entities.json` & `aa_memberaudit-2.9.1/memberaudit/tests/testdata/entities.json`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/tests/testdata/esi_client_stub.py` & `aa_memberaudit-2.9.1/memberaudit/tests/testdata/esi_client_stub.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,22 @@
+"""Stubs for replacing the ESI client from the django-esi library."""
+
 import inspect
 import json
 import os
+from typing import NamedTuple
 
 from app_utils.esi_testing import EsiClientStub, EsiEndpoint
 
-_currentdir = os.path.dirname(os.path.abspath(inspect.getfile(inspect.currentframe())))
+_current_dir = os.path.dirname(os.path.abspath(inspect.getfile(inspect.currentframe())))
 _FILENAME_ESI_TESTDATA = "esi_testdata.json"
 
 
 def load_test_data():
-    with open(f"{_currentdir}/{_FILENAME_ESI_TESTDATA}", "r", encoding="utf-8") as f:
+    with open(f"{_current_dir}/{_FILENAME_ESI_TESTDATA}", "r", encoding="utf-8") as f:
         return json.load(f)
 
 
 _endpoints = [
     EsiEndpoint(
         "Assets",
         "get_characters_character_id_assets",
@@ -185,10 +188,27 @@
         "get_characters_character_id_attributes",
         "character_id",
         needs_token=True,
     ),
 ]
 
 esi_client_stub = EsiClientStub(load_test_data(), endpoints=_endpoints)
+
 esi_client_error_stub = EsiClientStub(
-    load_test_data(), endpoints=_endpoints, http_error=True
+    load_test_data(), endpoints=_endpoints, http_error=502
 )
+
+
+class EsiStub(NamedTuple):
+    """This helper allows patching the esi object from a provider directly
+    and without required to define mock.
+
+    Example:
+
+    ``@patch(MANAGERS_PATH + ".general.esi", esi_stub)``
+    """
+
+    client: EsiClientStub
+
+
+esi_stub = EsiStub(esi_client_stub)
+esi_error_stub = EsiStub(esi_client_error_stub)
```

### Comparing `aa_memberaudit-2.9.0/memberaudit/tests/testdata/esi_testdata.json` & `aa_memberaudit-2.9.1/memberaudit/tests/testdata/esi_testdata.json`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/tests/testdata/eveuniverse.json` & `aa_memberaudit-2.9.1/memberaudit/tests/testdata/eveuniverse.json`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/tests/testdata/factories.py` & `aa_memberaudit-2.9.1/memberaudit/tests/testdata/factories.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
     This factory is designed to work with both the old and new variant of Character
     introduced in version 2.
     """
     try:
         character_ownership = user.profile.main_character.character_ownership
     except AttributeError:
-        raise ValueError("User needs to have a main character.")
+        raise ValueError("User needs to have a main character.") from None
     if hasattr(Character, "eve_character"):
         params = {"eve_character": character_ownership.character}
     else:
         params = {"character_ownership": character_ownership}
     params.update(kwargs)
     return Character.objects.create(**params)
 
@@ -240,16 +240,16 @@
     params.update(kwargs)
     return Fitting(**params)
 
 
 def create_fitting_text(file_name: str) -> str:
     testdata_folder = Path(__file__).parent / "fittings"
     fitting_file = testdata_folder / file_name
-    with fitting_file.open("r") as fp:
-        return fp.read()
+    with fitting_file.open("r") as file:
+        return file.read()
 
 
 def create_skill(**kwargs) -> Skill:
     params = {}
     if "eve_type" not in kwargs:
         params["eve_type"] = (
             EveType.objects.filter(
@@ -396,12 +396,12 @@
 
 def next_number(key=None) -> int:
     if key is None:
         key = "_general"
     try:
         return next_number._counter[key].__next__()
     except AttributeError:
-        next_number._counter = dict()
+        next_number._counter = {}
     except KeyError:
         pass
     next_number._counter[key] = count(start=1)
     return next_number._counter[key].__next__()
```

### Comparing `aa_memberaudit-2.9.0/memberaudit/tests/testdata/fittings/fitting_archon.txt` & `aa_memberaudit-2.9.1/memberaudit/tests/testdata/fittings/fitting_archon.txt`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/tests/testdata/fittings/fitting_archon_max.txt` & `aa_memberaudit-2.9.1/memberaudit/tests/testdata/fittings/fitting_archon_max.txt`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/tests/testdata/fittings/fitting_svipul.txt` & `aa_memberaudit-2.9.1/memberaudit/tests/testdata/fittings/fitting_svipul.txt`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/tests/testdata/fittings/fitting_tengu.txt` & `aa_memberaudit-2.9.1/memberaudit/tests/testdata/fittings/fitting_tengu.txt`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/tests/testdata/generate_character.py` & `aa_memberaudit-2.9.1/memberaudit/tests/testdata/generate_character.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
     print(f"Creating wallet journal with {WALLET_JOURNAL_ENTRIES} entries...")
     first_party, _ = EveEntity.objects.get_or_create_esi(id=eve_character.character_id)
     some_characters = list(
         EveEntity.objects.filter(category=EveEntity.CATEGORY_CHARACTER).order_by("?")[
             :20
         ]
     )
-    objs = list()
+    objs = []
     balance = 10_000_000_000_000
     date = now() - dt.timedelta(days=5_000)
     for entry_id in range(1, WALLET_JOURNAL_ENTRIES):
         amount = random.randint(1_000_000, 100_000_000)
         balance -= amount
         second_party = random.choice(some_characters)
         date += dt.timedelta(minutes=random.randint(1, 15))
```

### Comparing `aa_memberaudit-2.9.0/memberaudit/tests/testdata/generate_doctrines.py` & `aa_memberaudit-2.9.1/memberaudit/tests/testdata/generate_doctrines.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/tests/testdata/load_entities.py` & `aa_memberaudit-2.9.1/memberaudit/tests/testdata/load_entities.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,15 +90,15 @@
             category=entity_info.get("category"),
         )
 
     for EveModel in [EveConstellation, EveFaction, EveRegion, EveSolarSystem, EveType]:
         _generate_eve_entities_from_eve_universe(EveModel)
 
 
-def _generate_eve_entities_from_eve_universe(EveModel):
-    category = EveModel.eve_entity_category()
-    for obj in EveModel.objects.all():
+def _generate_eve_entities_from_eve_universe(model_class):
+    category = model_class.eve_entity_category()
+    for obj in model_class.objects.all():
         EveEntity.objects.create(
             id=obj.id,
             name=obj.name,
             category=category,
         )
```

### Comparing `aa_memberaudit-2.9.0/memberaudit/tests/testdata/load_locations.py` & `aa_memberaudit-2.9.1/memberaudit/tests/testdata/load_locations.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/tests/testdata/pilot_esi_error_handling.py` & `aa_memberaudit-2.9.1/memberaudit/tests/testdata/pilot_esi_error_handling.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/tests/testdata/profiler_toolbox.py` & `aa_memberaudit-2.9.1/memberaudit/tests/testdata/profiler_toolbox.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # flake8: noqa
 """
-This is a standalone scripts that generates a test character
+This is a standalone scripts for profiling code sections of Member Audit.
 """
 
 import inspect
 import os
 import sys
 
 currentdir = os.path.dirname(os.path.abspath(inspect.getfile(inspect.currentframe())))
```

### Comparing `aa_memberaudit-2.9.0/memberaudit/tests/utils.py` & `aa_memberaudit-2.9.1/memberaudit/tests/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,90 @@
+"""Shared utils for tests."""
+
 import json
+import os
 from typing import Tuple
 
 from django.contrib.auth.models import User
 from django.http import JsonResponse
 from django.test import RequestFactory, TestCase
 from esi.models import Token
 from eveuniverse.models import EveEntity, EveSolarSystem, EveType
 
 from allianceauth.authentication.models import CharacterOwnership
 from allianceauth.eveonline.models import EveCharacter
 from allianceauth.tests.auth_utils import AuthUtils
-from allianceauth.utils.cache import get_redis_client
 from app_utils.testing import NoSocketsTestCase, add_character_to_user, response_text
 
 from memberaudit.models import Character, Location
 
 from .testdata.load_entities import load_entities
 from .testdata.load_eveuniverse import load_eveuniverse
 from .testdata.load_locations import load_locations
 
 
+class CharacterUpdateTestDataMixin:
+    """Mixin for TestCase class defining a complete character and setting up fixtures."""
+
+    @classmethod
+    def setUpClass(cls) -> None:
+        super().setUpClass()
+        load_eveuniverse()
+        load_entities()
+        load_locations()
+        cls.character_1001 = create_memberaudit_character(1001)
+        cls.character_1002 = create_memberaudit_character(1002)
+        cls.corporation_2001 = EveEntity.objects.get(id=2001)
+        cls.corporation_2002 = EveEntity.objects.get(id=2002)
+        cls.token = cls.character_1001.user.token_set.first()
+        cls.jita = EveSolarSystem.objects.get(id=30000142)
+        cls.jita_44 = Location.objects.get(id=60003760)
+        cls.amamake = EveSolarSystem.objects.get(id=30002537)
+        cls.structure_1 = Location.objects.get(id=1000000000001)
+
+
+class TestCharacterUpdateBase(TestCase):
+    """TestCase variant defining a complete character and setting up fixtures."""
+
+    @classmethod
+    def setUpClass(cls) -> None:
+        super().setUpClass()
+        load_eveuniverse()
+        load_entities()
+        load_locations()
+        cls.character_1001 = create_memberaudit_character(1001)
+        cls.character_1002 = create_memberaudit_character(1002)
+        cls.corporation_2001 = EveEntity.objects.get(id=2001)
+        cls.corporation_2002 = EveEntity.objects.get(id=2002)
+        cls.token = (
+            cls.character_1001.eve_character.character_ownership.user.token_set.first()
+        )
+        cls.jita = EveSolarSystem.objects.get(id=30000142)
+        cls.jita_44 = Location.objects.get(id=60003760)
+        cls.amamake = EveSolarSystem.objects.get(id=30002537)
+        cls.structure_1 = Location.objects.get(id=1000000000001)
+
+
 def create_user_from_evecharacter_with_access(
     character_id: int,
 ) -> Tuple[User, CharacterOwnership]:
+    """Create user with access from an existing eve character and use it as main."""
     auth_character = EveCharacter.objects.get(character_id=character_id)
     user = AuthUtils.create_user(auth_character.character_name)
     user = AuthUtils.add_permission_to_user_by_name("memberaudit.basic_access", user)
     character_ownership = add_character_to_user(
         user, auth_character, is_main=True, scopes=Character.get_esi_scopes()
     )
     return user, character_ownership
 
 
 def create_memberaudit_character(character_id: int) -> Character:
+    """Create a memberaudit character from an existing auth character
+    incl. user and making it the main.
+    """
     _, character_ownership = create_user_from_evecharacter_with_access(character_id)
     return Character.objects.create(eve_character=character_ownership.character)
 
 
 def add_auth_character_to_user(
     user: User, character_id: int, scopes=None
 ) -> CharacterOwnership:
@@ -83,23 +131,19 @@
     """Convert JSON response into Python object."""
     data = json.loads(response_text(response))
     return data[data_key]
 
 
 def json_response_to_dict_2(response: JsonResponse, key="id", data_key="data") -> dict:
     """Convert JSON response into dict by given key."""
-    return {x[key]: x for x in json_response_to_python_2(response, data_key)}
-
-
-def clear_celery_once_locks():
-    """Clear all celery once locks (if any exist)."""
-    r = get_redis_client()
-    if keys := r.keys(":?:qo_memberaudit.*"):
-        r.delete(*keys)
+    return {o[key]: o for o in json_response_to_python_2(response, data_key)}
 
 
 class TestCaseWithFixtures(TestCase):
     fixtures = ["disable_analytics.json"]
 
 
 class NoSocketsTestCaseFixtures(NoSocketsTestCase):
     fixtures = ["disable_analytics.json"]
+
+
+TOX_IS_RUNNING = os.getenv("TOX_IS_RUNNING") == "1"
```

### Comparing `aa_memberaudit-2.9.0/memberaudit/tests/views/test_admin.py` & `aa_memberaudit-2.9.1/memberaudit/tests/views/test_admin.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/tests/views/test_character_finder.py` & `aa_memberaudit-2.9.1/memberaudit/tests/views/test_character_finder.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/tests/views/test_character_viewer_1.py` & `aa_memberaudit-2.9.1/memberaudit/tests/views/test_character_viewer_1.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/tests/views/test_character_viewer_2.py` & `aa_memberaudit-2.9.1/memberaudit/tests/views/test_character_viewer_2.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/tests/views/test_characters.py` & `aa_memberaudit-2.9.1/memberaudit/tests/views/test_characters.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/tests/views/test_data_export.py` & `aa_memberaudit-2.9.1/memberaudit/tests/views/test_data_export.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/tests/views/test_reports.py` & `aa_memberaudit-2.9.1/memberaudit/tests/views/test_reports.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/tools/drop_tables.sql` & `aa_memberaudit-2.9.1/memberaudit/tools/drop_tables.sql`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.0/memberaudit/urls.py` & `aa_memberaudit-2.9.1/memberaudit/urls.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Define routes for Member Audit."""
+
 from django.urls import path
 
 from memberaudit.views import (
     admin,
     character_finder,
     character_viewer_1,
     character_viewer_2,
```

### Comparing `aa_memberaudit-2.9.0/memberaudit/views/_common.py` & `aa_memberaudit-2.9.1/memberaudit/views/_common.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Shared view components."""
+
 from django.utils.html import format_html
 from django.utils.translation import gettext_lazy
 from eveuniverse.core import dotlan
 from eveuniverse.models import EveSolarSystem
 
 from app_utils.views import link_html
```

### Comparing `aa_memberaudit-2.9.0/memberaudit/views/admin.py` & `aa_memberaudit-2.9.1/memberaudit/views/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Admin views."""
+
 from django.contrib import messages
 from django.contrib.admin.views.decorators import staff_member_required
 from django.contrib.auth.decorators import login_required
 from django.shortcuts import redirect, render
 from django.utils.html import format_html
 from django.utils.translation import gettext_lazy as _
```

### Comparing `aa_memberaudit-2.9.0/memberaudit/views/character_finder.py` & `aa_memberaudit-2.9.1/memberaudit/views/character_finder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Character finder views."""
+
 from dj_datatables_view.base_datatable_view import BaseDatatableView
 
 from django.contrib.auth.decorators import login_required, permission_required
 from django.contrib.auth.mixins import LoginRequiredMixin, PermissionRequiredMixin
 from django.core.exceptions import ObjectDoesNotExist
 from django.db.models import Case, F, Q, Value, When
 from django.http import HttpResponse, JsonResponse
@@ -40,14 +42,16 @@
         add_common_context(request, context),
     )
 
 
 class CharacterFinderListJson(
     PermissionRequiredMixin, LoginRequiredMixin, BaseDatatableView
 ):
+    """Server based datatable view for character finder."""
+
     model = EveCharacter
     permission_required = "memberaudit.finder_access"
     columns = [
         "character",
         "character_organization",
         "main_character",
         "main_organization",
@@ -276,15 +280,15 @@
         return None
 
 
 @login_required
 @permission_required("memberaudit.finder_access")
 def character_finder_list_fdd_data(request) -> JsonResponse:
     """Provide lists for drop down fields."""
-    result = dict()
+    result = {}
     qs = CharacterFinderListJson.initial_queryset(request)
     columns = request.GET.get("columns")
     if columns:
         for column in columns.split(","):
             if column == "alliance_name":
                 options = qs.exclude(alliance_id__isnull=True).values_list(
                     "alliance_name", flat=True
```

### Comparing `aa_memberaudit-2.9.0/memberaudit/views/character_viewer_1.py` & `aa_memberaudit-2.9.1/memberaudit/views/character_viewer_1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Character viewer views (1/2)."""
+
 from typing import Optional, Tuple
 
 from django.contrib.auth.decorators import login_required, permission_required
 from django.core.exceptions import ObjectDoesNotExist
 from django.db import models
 from django.db.models import Count, F, Max, Q, Sum
 from django.http import HttpResponse, HttpResponseNotFound, JsonResponse
@@ -25,17 +27,17 @@
 
 from memberaudit import __title__
 from memberaudit.constants import (
     DEFAULT_ICON_SIZE,
     MAIL_LABEL_ID_ALL_MAILS,
     MY_DATETIME_FORMAT,
     EveCategoryId,
-    EveDogmaAttributeId,
 )
 from memberaudit.decorators import fetch_character_if_allowed
+from memberaudit.helpers import implant_slot_num
 from memberaudit.models import (
     Character,
     CharacterAsset,
     CharacterContract,
     CharacterFwStats,
     Location,
 )
@@ -130,18 +132,18 @@
     # mail labels
     mail_labels = list(
         character.mail_labels.values(
             "label_id", "name", unread_count_2=F("unread_count")
         )
     )
     total_unread_count = sum(
-        [obj["unread_count_2"] for obj in mail_labels if obj["unread_count_2"]]
+        (obj["unread_count_2"] for obj in mail_labels if obj["unread_count_2"])
     )
     total_unread_count += sum(
-        [obj["unread_count"] for obj in mailing_lists if obj["unread_count"]]
+        (obj["unread_count"] for obj in mailing_lists if obj["unread_count"])
     )
     mail_labels.append(
         {
             "label_id": MAIL_LABEL_ID_ALL_MAILS,
             "name": "All Mails",
             "unread_count_2": total_unread_count,
         }
@@ -243,15 +245,15 @@
 
 @login_required
 @permission_required("memberaudit.basic_access")
 @fetch_character_if_allowed()
 def character_assets_data(
     request, character_pk: int, character: Character
 ) -> JsonResponse:
-    data = list()
+    data = []
     asset_qs = (
         character.assets.annotate_pricing()
         .select_related(
             "eve_type",
             "eve_type__eve_group",
             "eve_type__eve_group__eve_category",
             "location__eve_solar_system",
@@ -367,15 +369,15 @@
 
 @login_required
 @permission_required("memberaudit.basic_access")
 @fetch_character_if_allowed()
 def character_asset_container_data(
     request, character_pk: int, character: Character, parent_asset_pk: int
 ) -> JsonResponse:
-    data = list()
+    data = []
     try:
         parent_asset = character.assets.get(pk=parent_asset_pk)
     except CharacterAsset.DoesNotExist:
         error_msg = (
             f"Asset with pk {parent_asset_pk} not found for character {character}"
         )
         logger.warning(error_msg)
@@ -428,15 +430,15 @@
 
 @login_required
 @permission_required("memberaudit.basic_access")
 @fetch_character_if_allowed()
 def character_contacts_data(
     request, character_pk: int, character: Character
 ) -> JsonResponse:
-    data = list()
+    data = []
     for contact in character.contacts.select_related("eve_entity").all():
         is_watched = contact.is_watched is True
         is_blocked = contact.is_blocked is True
         name = contact.eve_entity.name
         is_npc = contact.eve_entity.is_npc
         if is_npc:
             name_plus = format_html("{} {}", name, bootstrap_label_html("NPC", "info"))
@@ -466,15 +468,15 @@
 
 @login_required
 @permission_required("memberaudit.basic_access")
 @fetch_character_if_allowed()
 def character_contracts_data(
     request, character_pk: int, character: Character
 ) -> JsonResponse:
-    data = list()
+    data = []
     for contract in character.contracts.select_related("issuer", "assignee").all():
         if now() < contract.date_expired:
             time_left = timeuntil(contract.date_expired, now())
         else:
             time_left = "expired"
 
         ajax_contract_detail = reverse(
@@ -585,15 +587,15 @@
 def _character_contract_items_data(
     request,
     character_pk: int,
     character: Character,
     contract_pk: int,
     is_included: bool,
 ) -> JsonResponse:
-    data = list()
+    data = []
     try:
         contract = character.contracts.prefetch_related("items").get(pk=contract_pk)
     except CharacterAsset.DoesNotExist:
         error_msg = (
             f"Contract with pk {contract_pk} not found for character {character}"
         )
         logger.warning(error_msg)
@@ -630,15 +632,15 @@
 
 @login_required
 @permission_required("memberaudit.basic_access")
 @fetch_character_if_allowed()
 def character_corporation_history(
     request, character_pk: int, character: Character
 ) -> HttpResponse:
-    corporation_history = list()
+    corporation_history = []
     try:
         corporation_history_qs = character.corporation_history.select_related(
             "corporation"
         ).order_by("start_date")
     except ObjectDoesNotExist:
         pass
 
@@ -694,32 +696,25 @@
 
 @login_required
 @permission_required("memberaudit.basic_access")
 @fetch_character_if_allowed()
 def character_implants_data(
     request, character_pk: int, character: Character
 ) -> JsonResponse:
-    data = list()
+    data = []
     for implant in character.implants.select_related("eve_type").prefetch_related(
         "eve_type__dogma_attributes"
     ):
         implant_html = bootstrap_icon_plus_name_html(
             implant.eve_type.icon_url(
                 DEFAULT_ICON_SIZE, variant=EveType.IconVariant.REGULAR
             ),
             implant.eve_type.name,
         )
-        dogma_attributes = {
-            obj.eve_dogma_attribute_id: obj.value
-            for obj in implant.eve_type.dogma_attributes.all()
-        }
-        try:
-            slot_num = int(dogma_attributes[EveDogmaAttributeId.IMPLANT_SLOT])
-        except KeyError:
-            slot_num = 0
+        slot_num = implant_slot_num(implant.eve_type)
         data.append(
             {
                 "id": implant.pk,
                 "implant": {"display": implant_html, "sort": slot_num},
             }
         )
 
@@ -728,15 +723,15 @@
 
 @login_required
 @permission_required("memberaudit.basic_access")
 @fetch_character_if_allowed()
 def character_loyalty_data(
     request, character_pk: int, character: Character
 ) -> JsonResponse:
-    data = list()
+    data = []
     for entry in character.loyalty_entries.select_related("corporation"):
         corporation_html = bootstrap_icon_plus_name_html(
             entry.corporation.icon_url(DEFAULT_ICON_SIZE), entry.corporation.name
         )
         data.append(
             {
                 "id": entry.pk,
```

### Comparing `aa_memberaudit-2.9.0/memberaudit/views/character_viewer_2.py` & `aa_memberaudit-2.9.1/memberaudit/views/character_viewer_2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Character viewer views (2/2)."""
+
 import datetime as dt
 from typing import Optional
 
 import humanize
 from humanize import naturaltime
 
 from django.contrib.auth.decorators import login_required, permission_required
@@ -30,17 +32,17 @@
 from memberaudit.constants import (
     DATETIME_FORMAT,
     DEFAULT_ICON_SIZE,
     MAIL_LABEL_ID_ALL_MAILS,
     MAP_ARABIC_TO_ROMAN_NUMBERS,
     MY_DATETIME_FORMAT,
     SKILL_SET_DEFAULT_ICON_TYPE_ID,
-    EveDogmaAttributeId,
 )
 from memberaudit.decorators import fetch_character_if_allowed
+from memberaudit.helpers import implant_slot_num
 from memberaudit.models import (
     Character,
     CharacterMail,
     CharacterPlanet,
     SkillSet,
     SkillSetSkill,
 )
@@ -60,15 +62,15 @@
 
 @login_required
 @permission_required("memberaudit.basic_access")
 @fetch_character_if_allowed()
 def character_jump_clones_data(
     request, character_pk: int, character: Character
 ) -> HttpResponse:
-    data = list()
+    data = []
     try:
         for jump_clone in (
             character.jump_clones.select_related(
                 "location",
                 "location__eve_solar_system",
                 "location__eve_solar_system__eve_constellation__eve_region",
             )
@@ -81,39 +83,32 @@
                     eve_solar_system, show_region=False
                 )
                 region = eve_solar_system.eve_constellation.eve_region.name
             else:
                 solar_system = "-"
                 region = "-"
 
-            implants_data = list()
+            implants_data = []
             for implant in jump_clone.implants.all():
-                dogma_attributes = {
-                    obj.eve_dogma_attribute_id: obj.value
-                    for obj in implant.eve_type.dogma_attributes.all()
-                }
-                try:
-                    slot_num = int(dogma_attributes[EveDogmaAttributeId.IMPLANT_SLOT])
-                except KeyError:
-                    slot_num = 0
+                slot_num = implant_slot_num(implant.eve_type)
                 implants_data.append(
                     {
                         "name": implant.eve_type.name,
                         "icon_url": implant.eve_type.icon_url(
                             DEFAULT_ICON_SIZE, variant=EveType.IconVariant.REGULAR
                         ),
                         "slot_num": slot_num,
                     }
                 )
             if implants_data:
                 implants = "<br>".join(
                     bootstrap_icon_plus_name_html(
-                        x["icon_url"], no_wrap_html(x["name"]), size=24
+                        implant["icon_url"], no_wrap_html(implant["name"]), size=24
                     )
-                    for x in sorted(implants_data, key=lambda k: k["slot_num"])
+                    for implant in sorted(implants_data, key=lambda k: k["slot_num"])
                 )
             else:
                 implants = "(none)"
 
             data.append(
                 {
                     "id": jump_clone.pk,
@@ -126,15 +121,15 @@
     except ObjectDoesNotExist:
         pass
 
     return JsonResponse({"data": data})
 
 
 def _character_mail_headers_data(request, character, mail_headers_qs) -> JsonResponse:
-    mails_data = list()
+    mails_data = []
     try:
         for mail in mail_headers_qs.select_related("sender").prefetch_related(
             "recipients"
         ):
             mail_ajax_url = reverse(
                 "memberaudit:character_mail", args=[character.pk, mail.pk]
             )
@@ -263,15 +258,15 @@
 
 @login_required
 @permission_required("memberaudit.basic_access")
 @fetch_character_if_allowed()
 def character_planets_data(
     request, character_pk: int, character: Character
 ) -> JsonResponse:
-    data = list()
+    data = []
     my_now = now()
     for planet in character.planets.select_related(
         "eve_planet",
         "eve_planet__eve_type",
         "eve_planet__eve_solar_system",
         "eve_planet__eve_solar_system__eve_constellation__eve_region",
     ):
@@ -312,15 +307,15 @@
 
 @login_required
 @permission_required("memberaudit.basic_access")
 @fetch_character_if_allowed()
 def character_skillqueue_data(
     request, character_pk: int, character: Character
 ) -> JsonResponse:
-    data = list()
+    data = []
     try:
         for row in character.skillqueue.select_related("eve_type").filter(
             character_id=character_pk
         ):
             level_roman = MAP_ARABIC_TO_ROMAN_NUMBERS[row.finished_level]
             skill_str = f"{row.eve_type.name}&nbsp;{level_roman}"
             if row.is_active:
@@ -499,15 +494,15 @@
         skill_set_id=skill_set_pk
     )
     skill_set_skills = {obj.eve_type_id: obj for obj in skill_set_skills_qs}
     character_skills_qs = character.skills.select_related("eve_type").filter(
         eve_type_id__in=skill_set_skills.keys()
     )
     character_skills = {obj.eve_type_id: obj for obj in character_skills_qs}
-    out_data = list()
+    out_data = []
     url = (
         skill_set.ship_type.icon_url(ICON_SIZE_64, variant=EveType.IconVariant.REGULAR)
         if skill_set.ship_type
         else eveimageserver.type_icon_url(
             SKILL_SET_DEFAULT_ICON_TYPE_ID, size=ICON_SIZE_64
         )
     )
@@ -600,15 +595,15 @@
 
 @login_required
 @permission_required("memberaudit.basic_access")
 @fetch_character_if_allowed()
 def character_skills_data(
     request, character_pk: int, character: Character
 ) -> JsonResponse:
-    skills_data = list()
+    skills_data = []
     try:
         for skill in character.skills.select_related("eve_type", "eve_type__eve_group"):
             level_str = MAP_ARABIC_TO_ROMAN_NUMBERS[skill.active_skill_level]
             skill_name = format_html(
                 '<span title="{}">{} {}</span>',
                 skill.eve_type.description,
                 skill.eve_type.name,
@@ -631,15 +626,15 @@
 
 @login_required
 @permission_required("memberaudit.basic_access")
 @fetch_character_if_allowed()
 def character_wallet_journal_data(
     request, character_pk: int, character: Character
 ) -> JsonResponse:
-    wallet_data = list()
+    wallet_data = []
     try:
         for row in character.wallet_journal.select_related(
             "first_party", "second_party"
         ).all():
             first_party = row.first_party.name if row.first_party else "-"
             second_party = row.second_party.name if row.second_party else "-"
             wallet_data.append(
@@ -662,15 +657,15 @@
 
 @login_required
 @permission_required("memberaudit.basic_access")
 @fetch_character_if_allowed()
 def character_wallet_transactions_data(
     request, character_pk: int, character: Character
 ) -> JsonResponse:
-    wallet_data = list()
+    wallet_data = []
     try:
         for row in character.wallet_transactions.select_related(
             "client", "eve_type", "location"
         ).all():
             buy_or_sell = gettext_lazy("Buy") if row.is_buy else gettext_lazy("Sell")
             wallet_data.append(
                 {
```

### Comparing `aa_memberaudit-2.9.0/memberaudit/views/characters.py` & `aa_memberaudit-2.9.1/memberaudit/views/characters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Character views."""
+
 from django.contrib import messages
 from django.contrib.auth.decorators import login_required, permission_required
 from django.contrib.auth.models import Permission
 from django.db import transaction
 from django.http import HttpResponse, HttpResponseForbidden, HttpResponseNotFound
 from django.shortcuts import get_object_or_404, redirect, render
 from django.utils.html import format_html
@@ -42,16 +44,16 @@
             "memberaudit_character__skillpoints",
             "memberaudit_character__unread_mail_count",
             "memberaudit_character__wallet_balance",
         )
         .order_by("character_name")
     )
     has_auth_characters = owned_chars_query.exists()
-    auth_characters = list()
-    unregistered_chars = list()
+    auth_characters = []
+    unregistered_chars = []
     for eve_character in owned_chars_query:
         try:
             character = eve_character.memberaudit_character
         except AttributeError:
             unregistered_chars.append(eve_character.character_name)
         else:
             auth_characters.append(
@@ -78,25 +80,24 @@
         "auth_characters": auth_characters,
         "has_auth_characters": has_auth_characters,
         "unregistered_chars": unregistered_chars,
         "has_registered_characters": len(auth_characters) > 0,
         "main_character_id": main_character_id,
     }
 
-    """
-    if has_auth_characters:
-        messages.warning(
-            request,
-            format_html(
-                "Please register all your characters. "
-                "You currently have <strong>{}</strong> unregistered characters.",
-                unregistered_chars,
-            ),
-        )
-    """
+    # if has_auth_characters:
+    #     messages.warning(
+    #         request,
+    #         format_html(
+    #             "Please register all your characters. "
+    #             "You currently have <strong>{}</strong> unregistered characters.",
+    #             unregistered_chars,
+    #         ),
+    #     )
+
     return render(
         request, "memberaudit/launcher.html", add_common_context(request, context)
     )
 
 
 @login_required
 @permission_required("memberaudit.basic_access")
```

### Comparing `aa_memberaudit-2.9.0/memberaudit/views/data_export.py` & `aa_memberaudit-2.9.1/memberaudit/views/data_export.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Data export views."""
+
 from django.contrib import messages
 from django.contrib.auth.decorators import login_required, permission_required
 from django.http import FileResponse, Http404
 from django.shortcuts import redirect, render
 from django.utils.translation import gettext_lazy as _
 
 from allianceauth.services.hooks import get_extension_logger
```

### Comparing `aa_memberaudit-2.9.0/memberaudit/views/reports.py` & `aa_memberaudit-2.9.1/memberaudit/views/reports.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Report views."""
+
 from collections import defaultdict
 
 from django.contrib.auth.decorators import login_required, permission_required
 from django.core.exceptions import ObjectDoesNotExist
 from django.db.models import Count, Exists, OuterRef, Q
 from django.http import HttpResponse, JsonResponse
 from django.shortcuts import render
@@ -55,15 +57,15 @@
                 "character_ownerships",
                 filter=Q(character_ownerships__character__memberaudit_character=None),
                 distinct=True,
             )
         )
         .select_related("profile__main_character", "profile__state")
     )
-    user_data = list()
+    user_data = []
     for user in users_and_character_counts:
         if user.profile.main_character:
             main_character = user.profile.main_character
             if user == request.user or request.user.has_perm(
                 "memberaudit.characters_access"
             ):
                 try:
@@ -159,15 +161,15 @@
                 filter=Q(
                     userprofile__user__character_ownerships__character__memberaudit_character__isnull=True
                 ),
                 distinct=True,
             )
         )
     )
-    data = list()
+    data = []
     for corporation in corporations:
         organization_name = "{}{}".format(
             corporation["corporation_name"],
             f" [{corporation['alliance_ticker']}]"
             if corporation["alliance_ticker"]
             else "",
         )
@@ -253,15 +255,15 @@
                 )
                 if obj.ship_type
                 else eveimageserver.type_icon_url(
                     SKILL_SET_DEFAULT_ICON_TYPE_ID, size=DEFAULT_ICON_SIZE
                 ),
                 obj.name,
             )
-            for obj in sorted(skill_sets, key=lambda x: x.name.lower())
+            for obj in sorted(skill_sets, key=lambda o: o.name.lower())
         ]
         has_required_html = (
             "<br>".join(has_required)
             if has_required
             else '<i class="fas fa-times boolean-icon-false"></i>'
         )
         state_name = character.user.profile.state.name if character.user else ""
@@ -305,15 +307,15 @@
     for skill_set_check in skill_set_checks_qs:
         character_skill_checks[skill_set_check.skill_set.pk].append(skill_set_check)
 
     data = []
     groups_map = SkillSet.objects.compile_groups_map()
     for group_map in groups_map.values():
         group = group_map["group"]
-        characters_map = dict()
+        characters_map = {}
         for skill_set in group_map["skill_sets"]:
             for skill_check in character_skill_checks[skill_set.pk]:
                 character = skill_check.character
                 if character.pk not in characters_map:
                     characters_map[character.pk] = {
                         "character": character,
                         "character_name": character,
```

### Comparing `aa_memberaudit-2.9.0/pyproject.toml` & `aa_memberaudit-2.9.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
 ]
 dependencies = [
-    "allianceauth-app-utils>=1.18.0",
+    "allianceauth-app-utils>=1.18.1",
     "allianceauth>=3",
     "bleach",
     "dj-datatables-view",
     "django-eveuniverse>=1.2",
     "humanize",
     "unidecode",
 ]
@@ -66,16 +66,17 @@
     "LOCALFOLDER"
 ]
 known_allianceauth = ["allianceauth", "app_utils"]
 known_django = ["django", "django_webtest", "esi", "eveuniverse"]
 
 [tool.pylint.'MASTER']
 ignore-patterns = ["test_.*.py,__init__.py", "generate_.*.py"]
+ignore-paths = ["^.*//migrations//.*$"]
 
 [tool.pylint.'BASIC']
 good-names = ["i", "j", "k", "x", "f", "ex"]
 
 [tool.pylint.'FORMAT']
-max-line-length = 100
+max-line-length = 120
 
 [tool.pylint.'MESSAGES CONTROL']
-disable = ["R", "C"]
+disable = ["E0213", "E1101", "C0209", "C"]  # , "C"
```

### Comparing `aa_memberaudit-2.9.0/PKG-INFO` & `aa_memberaudit-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-memberaudit
-Version: 2.9.0
+Version: 2.9.1
 Summary: "An Alliance Auth app that provides full access to Eve characters
 Keywords: allianceauth,eveonline,memberaudit
 Author-email: Erik Kalkoken <kalkoken87@gmail.com>, Peter Pfeufer <develop@ppfeufer.de>, Rebecca Murphy <rebecca@rcmurphy.me>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Dist: allianceauth-app-utils>=1.18.0
+Requires-Dist: allianceauth-app-utils>=1.18.1
 Requires-Dist: allianceauth>=3
 Requires-Dist: bleach
 Requires-Dist: dj-datatables-view
 Requires-Dist: django-eveuniverse>=1.2
 Requires-Dist: humanize
 Requires-Dist: unidecode
 Project-URL: Changelog, https://gitlab.com/ErikKalkoken/aa-memberaudit/-/blob/master/CHANGELOG.md
```

