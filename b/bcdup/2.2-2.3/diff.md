# Comparing `tmp/bcdup-2.2.tar.gz` & `tmp/bcdup-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcdup-2.2.tar", last modified: Mon Jun 19 03:13:15 2023, max compression
+gzip compressed data, was "bcdup-2.3.tar", last modified: Wed Jun 21 03:11:29 2023, max compression
```

## Comparing `bcdup-2.2.tar` & `bcdup-2.3.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 03:13:16.332366 bcdup-2.2/
--rw-rw-rw-   0        0        0      199 2023-06-19 03:13:16.330555 bcdup-2.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-19 03:13:16.332943 bcdup-2.2/setup.cfg
--rw-rw-rw-   0        0        0      769 2023-06-19 03:13:07.000000 bcdup-2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 03:13:15.420918 bcdup-2.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-19 03:13:15.687573 bcdup-2.2/src/bc_acc_dup/
--rw-rw-rw-   0        0        0        1 2023-06-19 03:03:00.000000 bcdup-2.2/src/bc_acc_dup/__init__.py
--rw-rw-rw-   0        0        0     2701 2023-06-19 03:10:19.000000 bcdup-2.2/src/bc_acc_dup/__main__.py
--rw-rw-rw-   0        0        0    10151 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/adb_handler.py
--rw-rw-rw-   0        0        0    15039 2023-05-20 14:53:44.000000 bcdup-2.2/src/bc_acc_dup/config_manager.py
--rw-rw-rw-   0        0        0     1501 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/csv_handler.py
-drwxrwxrwx   0        0        0        0 2023-06-19 03:13:15.698438 bcdup-2.2/src/bc_acc_dup/edits/
--rw-rw-rw-   0        0        0       67 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/edits/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 03:13:15.765545 bcdup-2.2/src/bc_acc_dup/edits/basic/
--rw-rw-rw-   0        0        0      122 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/edits/basic/__init__.py
--rw-rw-rw-   0        0        0     8734 2023-05-26 02:04:50.000000 bcdup-2.2/src/bc_acc_dup/edits/basic/basic_items.py
--rw-rw-rw-   0        0        0     1490 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/edits/basic/catfruit.py
--rw-rw-rw-   0        0        0     1931 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/edits/basic/catseyes.py
--rw-rw-rw-   0        0        0     1647 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/edits/basic/ototo_base_mats.py
--rw-rw-rw-   0        0        0     3984 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/edits/basic/talent_orbs.py
--rw-rw-rw-   0        0        0    16573 2023-05-16 02:09:48.000000 bcdup-2.2/src/bc_acc_dup/edits/basic/talent_orbs_new.py
-drwxrwxrwx   0        0        0        0 2023-06-19 03:13:15.858447 bcdup-2.2/src/bc_acc_dup/edits/cats/
--rw-rw-rw-   0        0        0      179 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/edits/cats/__init__.py
--rw-rw-rw-   0        0        0     8978 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/edits/cats/cat_helper.py
--rw-rw-rw-   0        0        0    11121 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/edits/cats/cat_id_selector.py
--rw-rw-rw-   0        0        0     3249 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/edits/cats/chara_drop.py
--rw-rw-rw-   0        0        0     1068 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/edits/cats/clear_cat_guide.py
--rw-rw-rw-   0        0        0     2844 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/edits/cats/evolve_cats.py
--rw-rw-rw-   0        0        0     1260 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/edits/cats/get_remove_cats.py
--rw-rw-rw-   0        0        0     7936 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/edits/cats/talents.py
--rw-rw-rw-   0        0        0     1900 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/edits/cats/upgrade_blue.py
--rw-rw-rw-   0        0        0     3507 2023-03-28 04:18:30.000000 bcdup-2.2/src/bc_acc_dup/edits/cats/upgrade_cats.py
-drwxrwxrwx   0        0        0        0 2023-06-19 03:13:15.903769 bcdup-2.2/src/bc_acc_dup/edits/gamototo/
--rw-rw-rw-   0        0        0       66 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/edits/gamototo/__init__.py
--rw-rw-rw-   0        0        0      309 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/edits/gamototo/fix_gamatoto.py
--rw-rw-rw-   0        0        0     2659 2023-05-26 07:00:35.000000 bcdup-2.2/src/bc_acc_dup/edits/gamototo/gamatoto_xp.py
--rw-rw-rw-   0        0        0     3418 2023-05-31 04:36:47.000000 bcdup-2.2/src/bc_acc_dup/edits/gamototo/helpers.py
--rw-rw-rw-   0        0        0     4137 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/edits/gamototo/ototo_cat_cannon.py
-drwxrwxrwx   0        0        0        0 2023-06-19 03:13:16.064615 bcdup-2.2/src/bc_acc_dup/edits/levels/
--rw-rw-rw-   0        0        0      313 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/edits/levels/__init__.py
--rw-rw-rw-   0        0        0     1024 2023-03-28 13:41:31.000000 bcdup-2.2/src/bc_acc_dup/edits/levels/aku.py
--rw-rw-rw-   0        0        0      491 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/edits/levels/allow_filibuster_clearing.py
--rw-rw-rw-   0        0        0      790 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/edits/levels/behemoth_culling.py
--rw-rw-rw-   0        0        0      646 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/edits/levels/clear_tutorial.py
--rw-rw-rw-   0        0        0     1121 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/edits/levels/enigma_stages.py
--rw-rw-rw-   0        0        0     5924 2023-03-28 13:39:14.000000 bcdup-2.2/src/bc_acc_dup/edits/levels/event_stages.py
--rw-rw-rw-   0        0        0     1873 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/edits/levels/gauntlet.py
--rw-rw-rw-   0        0        0     1027 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/edits/levels/itf_timed_scores.py
--rw-rw-rw-   0        0        0     1469 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/edits/levels/legend_quest.py
--rw-rw-rw-   0        0        0     4382 2023-03-31 01:13:58.000000 bcdup-2.2/src/bc_acc_dup/edits/levels/main_story.py
--rw-rw-rw-   0        0        0     2100 2023-03-28 04:55:05.000000 bcdup-2.2/src/bc_acc_dup/edits/levels/outbreaks.py
--rw-rw-rw-   0        0        0     2824 2023-03-31 07:47:07.000000 bcdup-2.2/src/bc_acc_dup/edits/levels/story_level_id_selector.py
--rw-rw-rw-   0        0        0     1175 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/edits/levels/towers.py
--rw-rw-rw-   0        0        0     8909 2023-03-31 02:09:48.000000 bcdup-2.2/src/bc_acc_dup/edits/levels/treasures.py
--rw-rw-rw-   0        0        0      868 2023-03-28 13:37:22.000000 bcdup-2.2/src/bc_acc_dup/edits/levels/uncanny.py
--rw-rw-rw-   0        0        0      784 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/edits/levels/unlock_aku_realm.py
-drwxrwxrwx   0        0        0        0 2023-06-19 03:13:16.218742 bcdup-2.2/src/bc_acc_dup/edits/other/
--rw-rw-rw-   0        0        0      276 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/edits/other/__init__.py
--rw-rw-rw-   0        0        0     3878 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/edits/other/cat_shrine.py
--rw-rw-rw-   0        0        0     1093 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/edits/other/claim_user_rank_rewards.py
--rw-rw-rw-   0        0        0     1054 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/edits/other/create_new_account.py
--rw-rw-rw-   0        0        0     2171 2023-03-28 13:43:08.000000 bcdup-2.2/src/bc_acc_dup/edits/other/fix_elsewhere.py
--rw-rw-rw-   0        0        0      659 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/edits/other/fix_time_issues.py
--rw-rw-rw-   0        0        0     3186 2023-03-28 13:44:07.000000 bcdup-2.2/src/bc_acc_dup/edits/other/get_gold_pass.py
--rw-rw-rw-   0        0        0     7138 2023-06-11 23:05:06.000000 bcdup-2.2/src/bc_acc_dup/edits/other/meow_medals.py
--rw-rw-rw-   0        0        0     4354 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/edits/other/missions.py
--rw-rw-rw-   0        0        0      975 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/edits/other/play_time.py
--rw-rw-rw-   0        0        0     4568 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/edits/other/scheme_item.py
--rw-rw-rw-   0        0        0     1612 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/edits/other/trade_progress.py
--rw-rw-rw-   0        0        0      914 2023-03-28 13:45:19.000000 bcdup-2.2/src/bc_acc_dup/edits/other/unlock_enemy_guide.py
--rw-rw-rw-   0        0        0      326 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/edits/other/unlock_equip_menu.py
-drwxrwxrwx   0        0        0        0 2023-06-19 03:13:16.276248 bcdup-2.2/src/bc_acc_dup/edits/save_management/
--rw-rw-rw-   0        0        0       56 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/edits/save_management/__init__.py
--rw-rw-rw-   0        0        0      841 2023-05-20 14:27:18.000000 bcdup-2.2/src/bc_acc_dup/edits/save_management/convert.py
--rw-rw-rw-   0        0        0     2575 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/edits/save_management/load.py
--rw-rw-rw-   0        0        0      657 2023-04-12 00:58:57.000000 bcdup-2.2/src/bc_acc_dup/edits/save_management/other.py
--rw-rw-rw-   0        0        0     2048 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/edits/save_management/save.py
--rw-rw-rw-   0        0        0     1904 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/edits/save_management/server_upload.py
--rw-rw-rw-   0        0        0    12640 2023-05-26 02:00:11.000000 bcdup-2.2/src/bc_acc_dup/feature_handler.py
--rw-rw-rw-   0        0        0     4822 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/game_data_getter.py
--rw-rw-rw-   0        0        0    22984 2023-03-28 04:13:46.000000 bcdup-2.2/src/bc_acc_dup/helper.py
--rw-rw-rw-   0        0        0     7075 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/item.py
--rw-rw-rw-   0        0        0     3635 2023-05-07 09:06:08.000000 bcdup-2.2/src/bc_acc_dup/locale_handler.py
--rw-rw-rw-   0        0        0     1269 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/managed_item.py
--rw-rw-rw-   0        0        0    66642 2023-06-16 04:46:07.000000 bcdup-2.2/src/bc_acc_dup/parse_save.py
--rw-rw-rw-   0        0        0     1301 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/patcher.py
--rw-rw-rw-   0        0        0        0 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/py.typed
--rw-rw-rw-   0        0        0     2415 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/root_handler.py
--rw-rw-rw-   0        0        0    53791 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/serialise_save.py
--rw-rw-rw-   0        0        0    24704 2023-06-19 00:21:50.000000 bcdup-2.2/src/bc_acc_dup/server_handler.py
--rw-rw-rw-   0        0        0     3717 2023-03-22 09:57:23.000000 bcdup-2.2/src/bc_acc_dup/tracker.py
--rw-rw-rw-   0        0        0     3486 2023-03-25 14:14:04.000000 bcdup-2.2/src/bc_acc_dup/updater.py
--rw-rw-rw-   0        0        0     8175 2023-03-31 01:12:30.000000 bcdup-2.2/src/bc_acc_dup/user_input_handler.py
-drwxrwxrwx   0        0        0        0 2023-06-19 03:13:16.317503 bcdup-2.2/src/bcdup.egg-info/
--rw-rw-rw-   0        0        0      199 2023-06-19 03:13:15.000000 bcdup-2.2/src/bcdup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3390 2023-06-19 03:13:15.000000 bcdup-2.2/src/bcdup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 03:13:15.000000 bcdup-2.2/src/bcdup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      101 2023-06-19 03:13:15.000000 bcdup-2.2/src/bcdup.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-19 03:13:15.000000 bcdup-2.2/src/bcdup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-21 03:11:29.203878 bcdup-2.3/
+-rw-rw-rw-   0        0        0      199 2023-06-21 03:11:29.196136 bcdup-2.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-21 03:11:29.204493 bcdup-2.3/setup.cfg
+-rw-rw-rw-   0        0        0      769 2023-06-21 03:11:11.000000 bcdup-2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:11:26.140590 bcdup-2.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-21 03:11:26.753847 bcdup-2.3/src/bc_acc_dup/
+-rw-rw-rw-   0        0        0        1 2023-06-19 03:03:00.000000 bcdup-2.3/src/bc_acc_dup/__init__.py
+-rw-rw-rw-   0        0        0     2931 2023-06-21 03:11:01.000000 bcdup-2.3/src/bc_acc_dup/__main__.py
+-rw-rw-rw-   0        0        0    10151 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/adb_handler.py
+-rw-rw-rw-   0        0        0    15039 2023-05-20 14:53:44.000000 bcdup-2.3/src/bc_acc_dup/config_manager.py
+-rw-rw-rw-   0        0        0     1501 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/csv_handler.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:11:26.772875 bcdup-2.3/src/bc_acc_dup/edits/
+-rw-rw-rw-   0        0        0       67 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/edits/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:11:26.976395 bcdup-2.3/src/bc_acc_dup/edits/basic/
+-rw-rw-rw-   0        0        0      122 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/edits/basic/__init__.py
+-rw-rw-rw-   0        0        0     8734 2023-05-26 02:04:50.000000 bcdup-2.3/src/bc_acc_dup/edits/basic/basic_items.py
+-rw-rw-rw-   0        0        0     1490 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/edits/basic/catfruit.py
+-rw-rw-rw-   0        0        0     1931 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/edits/basic/catseyes.py
+-rw-rw-rw-   0        0        0     1647 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/edits/basic/ototo_base_mats.py
+-rw-rw-rw-   0        0        0     3984 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/edits/basic/talent_orbs.py
+-rw-rw-rw-   0        0        0    16573 2023-05-16 02:09:48.000000 bcdup-2.3/src/bc_acc_dup/edits/basic/talent_orbs_new.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:11:27.224420 bcdup-2.3/src/bc_acc_dup/edits/cats/
+-rw-rw-rw-   0        0        0      179 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/edits/cats/__init__.py
+-rw-rw-rw-   0        0        0     8978 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/edits/cats/cat_helper.py
+-rw-rw-rw-   0        0        0    11121 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/edits/cats/cat_id_selector.py
+-rw-rw-rw-   0        0        0     3249 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/edits/cats/chara_drop.py
+-rw-rw-rw-   0        0        0     1068 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/edits/cats/clear_cat_guide.py
+-rw-rw-rw-   0        0        0     2844 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/edits/cats/evolve_cats.py
+-rw-rw-rw-   0        0        0     1260 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/edits/cats/get_remove_cats.py
+-rw-rw-rw-   0        0        0     7936 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/edits/cats/talents.py
+-rw-rw-rw-   0        0        0     1900 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/edits/cats/upgrade_blue.py
+-rw-rw-rw-   0        0        0     3507 2023-03-28 04:18:30.000000 bcdup-2.3/src/bc_acc_dup/edits/cats/upgrade_cats.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:11:27.556238 bcdup-2.3/src/bc_acc_dup/edits/gamototo/
+-rw-rw-rw-   0        0        0       66 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/edits/gamototo/__init__.py
+-rw-rw-rw-   0        0        0      309 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/edits/gamototo/fix_gamatoto.py
+-rw-rw-rw-   0        0        0     2659 2023-05-26 07:00:35.000000 bcdup-2.3/src/bc_acc_dup/edits/gamototo/gamatoto_xp.py
+-rw-rw-rw-   0        0        0     3418 2023-05-31 04:36:47.000000 bcdup-2.3/src/bc_acc_dup/edits/gamototo/helpers.py
+-rw-rw-rw-   0        0        0     4137 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/edits/gamototo/ototo_cat_cannon.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:11:28.077199 bcdup-2.3/src/bc_acc_dup/edits/levels/
+-rw-rw-rw-   0        0        0      313 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/edits/levels/__init__.py
+-rw-rw-rw-   0        0        0     1024 2023-03-28 13:41:31.000000 bcdup-2.3/src/bc_acc_dup/edits/levels/aku.py
+-rw-rw-rw-   0        0        0      491 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/edits/levels/allow_filibuster_clearing.py
+-rw-rw-rw-   0        0        0      790 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/edits/levels/behemoth_culling.py
+-rw-rw-rw-   0        0        0      646 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/edits/levels/clear_tutorial.py
+-rw-rw-rw-   0        0        0     1121 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/edits/levels/enigma_stages.py
+-rw-rw-rw-   0        0        0     5924 2023-03-28 13:39:14.000000 bcdup-2.3/src/bc_acc_dup/edits/levels/event_stages.py
+-rw-rw-rw-   0        0        0     1873 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/edits/levels/gauntlet.py
+-rw-rw-rw-   0        0        0     1027 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/edits/levels/itf_timed_scores.py
+-rw-rw-rw-   0        0        0     1469 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/edits/levels/legend_quest.py
+-rw-rw-rw-   0        0        0     4382 2023-03-31 01:13:58.000000 bcdup-2.3/src/bc_acc_dup/edits/levels/main_story.py
+-rw-rw-rw-   0        0        0     2100 2023-03-28 04:55:05.000000 bcdup-2.3/src/bc_acc_dup/edits/levels/outbreaks.py
+-rw-rw-rw-   0        0        0     2824 2023-03-31 07:47:07.000000 bcdup-2.3/src/bc_acc_dup/edits/levels/story_level_id_selector.py
+-rw-rw-rw-   0        0        0     1175 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/edits/levels/towers.py
+-rw-rw-rw-   0        0        0     8909 2023-03-31 02:09:48.000000 bcdup-2.3/src/bc_acc_dup/edits/levels/treasures.py
+-rw-rw-rw-   0        0        0      868 2023-03-28 13:37:22.000000 bcdup-2.3/src/bc_acc_dup/edits/levels/uncanny.py
+-rw-rw-rw-   0        0        0      784 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/edits/levels/unlock_aku_realm.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:11:28.675825 bcdup-2.3/src/bc_acc_dup/edits/other/
+-rw-rw-rw-   0        0        0      276 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/edits/other/__init__.py
+-rw-rw-rw-   0        0        0     3878 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/edits/other/cat_shrine.py
+-rw-rw-rw-   0        0        0     1093 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/edits/other/claim_user_rank_rewards.py
+-rw-rw-rw-   0        0        0     1054 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/edits/other/create_new_account.py
+-rw-rw-rw-   0        0        0     2171 2023-03-28 13:43:08.000000 bcdup-2.3/src/bc_acc_dup/edits/other/fix_elsewhere.py
+-rw-rw-rw-   0        0        0      659 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/edits/other/fix_time_issues.py
+-rw-rw-rw-   0        0        0     3186 2023-03-28 13:44:07.000000 bcdup-2.3/src/bc_acc_dup/edits/other/get_gold_pass.py
+-rw-rw-rw-   0        0        0     7138 2023-06-11 23:05:06.000000 bcdup-2.3/src/bc_acc_dup/edits/other/meow_medals.py
+-rw-rw-rw-   0        0        0     4354 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/edits/other/missions.py
+-rw-rw-rw-   0        0        0      975 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/edits/other/play_time.py
+-rw-rw-rw-   0        0        0     4568 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/edits/other/scheme_item.py
+-rw-rw-rw-   0        0        0     1612 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/edits/other/trade_progress.py
+-rw-rw-rw-   0        0        0      914 2023-03-28 13:45:19.000000 bcdup-2.3/src/bc_acc_dup/edits/other/unlock_enemy_guide.py
+-rw-rw-rw-   0        0        0      326 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/edits/other/unlock_equip_menu.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:11:28.919019 bcdup-2.3/src/bc_acc_dup/edits/save_management/
+-rw-rw-rw-   0        0        0       56 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/edits/save_management/__init__.py
+-rw-rw-rw-   0        0        0      841 2023-05-20 14:27:18.000000 bcdup-2.3/src/bc_acc_dup/edits/save_management/convert.py
+-rw-rw-rw-   0        0        0     2575 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/edits/save_management/load.py
+-rw-rw-rw-   0        0        0      657 2023-04-12 00:58:57.000000 bcdup-2.3/src/bc_acc_dup/edits/save_management/other.py
+-rw-rw-rw-   0        0        0     2048 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/edits/save_management/save.py
+-rw-rw-rw-   0        0        0     1904 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/edits/save_management/server_upload.py
+-rw-rw-rw-   0        0        0    12640 2023-05-26 02:00:11.000000 bcdup-2.3/src/bc_acc_dup/feature_handler.py
+-rw-rw-rw-   0        0        0     4822 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/game_data_getter.py
+-rw-rw-rw-   0        0        0    22984 2023-03-28 04:13:46.000000 bcdup-2.3/src/bc_acc_dup/helper.py
+-rw-rw-rw-   0        0        0     7075 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/item.py
+-rw-rw-rw-   0        0        0     3635 2023-05-07 09:06:08.000000 bcdup-2.3/src/bc_acc_dup/locale_handler.py
+-rw-rw-rw-   0        0        0     1269 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/managed_item.py
+-rw-rw-rw-   0        0        0    66642 2023-06-16 04:46:07.000000 bcdup-2.3/src/bc_acc_dup/parse_save.py
+-rw-rw-rw-   0        0        0     1301 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/patcher.py
+-rw-rw-rw-   0        0        0        0 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/py.typed
+-rw-rw-rw-   0        0        0     2415 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/root_handler.py
+-rw-rw-rw-   0        0        0    53791 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/serialise_save.py
+-rw-rw-rw-   0        0        0    24704 2023-06-19 00:21:50.000000 bcdup-2.3/src/bc_acc_dup/server_handler.py
+-rw-rw-rw-   0        0        0     3717 2023-03-22 09:57:23.000000 bcdup-2.3/src/bc_acc_dup/tracker.py
+-rw-rw-rw-   0        0        0     3486 2023-03-25 14:14:04.000000 bcdup-2.3/src/bc_acc_dup/updater.py
+-rw-rw-rw-   0        0        0     8175 2023-03-31 01:12:30.000000 bcdup-2.3/src/bc_acc_dup/user_input_handler.py
+drwxrwxrwx   0        0        0        0 2023-06-21 03:11:29.184024 bcdup-2.3/src/bcdup.egg-info/
+-rw-rw-rw-   0        0        0      199 2023-06-21 03:11:25.000000 bcdup-2.3/src/bcdup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3390 2023-06-21 03:11:25.000000 bcdup-2.3/src/bcdup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 03:11:25.000000 bcdup-2.3/src/bcdup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      101 2023-06-21 03:11:25.000000 bcdup-2.3/src/bcdup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-21 03:11:25.000000 bcdup-2.3/src/bcdup.egg-info/top_level.txt
```

### Comparing `bcdup-2.2/setup.py` & `bcdup-2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 import setuptools
 setup(
     name="bcdup",
-    version='2.2',
+    version='2.3',
     author="CintagramABP",
     description="BCSFE_Python personal api",
     long_description="BCSFE_Python personal api",
     url="",
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.9",
```

### Comparing `bcdup-2.2/src/bc_acc_dup/__main__.py` & `bcdup-2.3/src/bc_acc_dup/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,22 +18,25 @@
         BCSFE_Python.helper.set_save_path(path)
         game_version = helper.str_to_gv(game_version)
         save_data = BCSFE_Python.server_handler.download_save(country_code, transfer_code, confirmation_code, game_version)
         save_data = patcher.patch_save_data(save_data, country_code)
         global save_stats
         save_stats = parse_save.start_parse(save_data, country_code)
         number = int(input("복제할 갯수를 입력하세요 (숫자): "))
+        if_gacha_change = int(input("레어뽑기 시드(배열)를 변경할까요? (y/n): "))
         print("복제중... 프로그램을 닫지 마세요")
         list = []
         i = 0
         for i in range(number):
             try:
                 print("복제중...{}/{}".format(i, number))
                 i += 1
                 random_inquiry_code = random.randint(100000, 9999999)
+                if if_gacha_change == "y":
+                    save_stats["rare_gacha_seed"]["Value"] = random.randint(1, 1215752190)
                 save_stats["inquiry_code"] = random_inquiry_code
                 edits.other.create_new_account.create_new_account(save_stats)
                 edits.save_management.save.save_save(save_stats)
                 save_data = BCSFE_Python.serialise_save.start_serialize(save_stats)
                 
                 save_data = BCSFE_Python.helper.write_save_data(
                     save_data, save_stats["version"], helper.get_save_path(), False
```

### Comparing `bcdup-2.2/src/bc_acc_dup/adb_handler.py` & `bcdup-2.3/src/bc_acc_dup/adb_handler.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/config_manager.py` & `bcdup-2.3/src/bc_acc_dup/config_manager.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/csv_handler.py` & `bcdup-2.3/src/bc_acc_dup/csv_handler.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/edits/basic/basic_items.py` & `bcdup-2.3/src/bc_acc_dup/edits/basic/basic_items.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/edits/basic/catfruit.py` & `bcdup-2.3/src/bc_acc_dup/edits/basic/catfruit.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/edits/basic/catseyes.py` & `bcdup-2.3/src/bc_acc_dup/edits/basic/catseyes.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/edits/basic/ototo_base_mats.py` & `bcdup-2.3/src/bc_acc_dup/edits/basic/ototo_base_mats.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/edits/basic/talent_orbs.py` & `bcdup-2.3/src/bc_acc_dup/edits/basic/talent_orbs.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/edits/basic/talent_orbs_new.py` & `bcdup-2.3/src/bc_acc_dup/edits/basic/talent_orbs_new.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/edits/cats/cat_helper.py` & `bcdup-2.3/src/bc_acc_dup/edits/cats/cat_helper.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/edits/cats/cat_id_selector.py` & `bcdup-2.3/src/bc_acc_dup/edits/cats/cat_id_selector.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/edits/cats/chara_drop.py` & `bcdup-2.3/src/bc_acc_dup/edits/cats/chara_drop.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/edits/cats/clear_cat_guide.py` & `bcdup-2.3/src/bc_acc_dup/edits/cats/clear_cat_guide.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/edits/cats/evolve_cats.py` & `bcdup-2.3/src/bc_acc_dup/edits/cats/evolve_cats.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/edits/cats/get_remove_cats.py` & `bcdup-2.3/src/bc_acc_dup/edits/cats/get_remove_cats.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/edits/cats/talents.py` & `bcdup-2.3/src/bc_acc_dup/edits/cats/talents.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/edits/cats/upgrade_blue.py` & `bcdup-2.3/src/bc_acc_dup/edits/cats/upgrade_blue.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/edits/cats/upgrade_cats.py` & `bcdup-2.3/src/bc_acc_dup/edits/cats/upgrade_cats.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/edits/gamototo/gamatoto_xp.py` & `bcdup-2.3/src/bc_acc_dup/edits/gamototo/gamatoto_xp.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/edits/gamototo/helpers.py` & `bcdup-2.3/src/bc_acc_dup/edits/gamototo/helpers.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/edits/gamototo/ototo_cat_cannon.py` & `bcdup-2.3/src/bc_acc_dup/edits/gamototo/ototo_cat_cannon.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/edits/levels/aku.py` & `bcdup-2.3/src/bc_acc_dup/edits/levels/aku.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/edits/levels/behemoth_culling.py` & `bcdup-2.3/src/bc_acc_dup/edits/levels/behemoth_culling.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/edits/levels/clear_tutorial.py` & `bcdup-2.3/src/bc_acc_dup/edits/levels/clear_tutorial.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/edits/levels/enigma_stages.py` & `bcdup-2.3/src/bc_acc_dup/edits/levels/enigma_stages.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/edits/levels/event_stages.py` & `bcdup-2.3/src/bc_acc_dup/edits/levels/event_stages.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/edits/levels/gauntlet.py` & `bcdup-2.3/src/bc_acc_dup/edits/levels/gauntlet.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/edits/levels/itf_timed_scores.py` & `bcdup-2.3/src/bc_acc_dup/edits/levels/itf_timed_scores.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/edits/levels/legend_quest.py` & `bcdup-2.3/src/bc_acc_dup/edits/levels/legend_quest.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/edits/levels/main_story.py` & `bcdup-2.3/src/bc_acc_dup/edits/levels/main_story.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/edits/levels/outbreaks.py` & `bcdup-2.3/src/bc_acc_dup/edits/levels/outbreaks.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/edits/levels/story_level_id_selector.py` & `bcdup-2.3/src/bc_acc_dup/edits/levels/story_level_id_selector.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/edits/levels/towers.py` & `bcdup-2.3/src/bc_acc_dup/edits/levels/towers.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/edits/levels/treasures.py` & `bcdup-2.3/src/bc_acc_dup/edits/levels/treasures.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/edits/levels/uncanny.py` & `bcdup-2.3/src/bc_acc_dup/edits/levels/uncanny.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/edits/levels/unlock_aku_realm.py` & `bcdup-2.3/src/bc_acc_dup/edits/levels/unlock_aku_realm.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/edits/other/cat_shrine.py` & `bcdup-2.3/src/bc_acc_dup/edits/other/cat_shrine.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/edits/other/claim_user_rank_rewards.py` & `bcdup-2.3/src/bc_acc_dup/edits/other/claim_user_rank_rewards.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/edits/other/create_new_account.py` & `bcdup-2.3/src/bc_acc_dup/edits/other/create_new_account.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/edits/other/fix_elsewhere.py` & `bcdup-2.3/src/bc_acc_dup/edits/other/fix_elsewhere.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/edits/other/fix_time_issues.py` & `bcdup-2.3/src/bc_acc_dup/edits/other/fix_time_issues.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/edits/other/get_gold_pass.py` & `bcdup-2.3/src/bc_acc_dup/edits/other/get_gold_pass.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/edits/other/meow_medals.py` & `bcdup-2.3/src/bc_acc_dup/edits/other/meow_medals.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/edits/other/missions.py` & `bcdup-2.3/src/bc_acc_dup/edits/other/missions.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/edits/other/play_time.py` & `bcdup-2.3/src/bc_acc_dup/edits/other/play_time.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/edits/other/scheme_item.py` & `bcdup-2.3/src/bc_acc_dup/edits/other/scheme_item.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/edits/other/trade_progress.py` & `bcdup-2.3/src/bc_acc_dup/edits/other/trade_progress.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/edits/other/unlock_enemy_guide.py` & `bcdup-2.3/src/bc_acc_dup/edits/other/unlock_enemy_guide.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/edits/save_management/convert.py` & `bcdup-2.3/src/bc_acc_dup/edits/save_management/convert.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/edits/save_management/load.py` & `bcdup-2.3/src/bc_acc_dup/edits/save_management/load.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/edits/save_management/other.py` & `bcdup-2.3/src/bc_acc_dup/edits/save_management/other.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/edits/save_management/save.py` & `bcdup-2.3/src/bc_acc_dup/edits/save_management/save.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/edits/save_management/server_upload.py` & `bcdup-2.3/src/bc_acc_dup/edits/save_management/server_upload.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/feature_handler.py` & `bcdup-2.3/src/bc_acc_dup/feature_handler.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/game_data_getter.py` & `bcdup-2.3/src/bc_acc_dup/game_data_getter.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/helper.py` & `bcdup-2.3/src/bc_acc_dup/helper.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/item.py` & `bcdup-2.3/src/bc_acc_dup/item.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/locale_handler.py` & `bcdup-2.3/src/bc_acc_dup/locale_handler.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/managed_item.py` & `bcdup-2.3/src/bc_acc_dup/managed_item.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/parse_save.py` & `bcdup-2.3/src/bc_acc_dup/parse_save.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/patcher.py` & `bcdup-2.3/src/bc_acc_dup/patcher.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/root_handler.py` & `bcdup-2.3/src/bc_acc_dup/root_handler.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/serialise_save.py` & `bcdup-2.3/src/bc_acc_dup/serialise_save.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/server_handler.py` & `bcdup-2.3/src/bc_acc_dup/server_handler.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/tracker.py` & `bcdup-2.3/src/bc_acc_dup/tracker.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/updater.py` & `bcdup-2.3/src/bc_acc_dup/updater.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bc_acc_dup/user_input_handler.py` & `bcdup-2.3/src/bc_acc_dup/user_input_handler.py`

 * *Files identical despite different names*

### Comparing `bcdup-2.2/src/bcdup.egg-info/SOURCES.txt` & `bcdup-2.3/src/bcdup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

