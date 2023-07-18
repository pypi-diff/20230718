# Comparing `tmp/bcedit_madeby_train-0.0.5.tar.gz` & `tmp/bcedit_madeby_train-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcedit_madeby_train-0.0.5.tar", last modified: Tue Jul 18 12:58:44 2023, max compression
+gzip compressed data, was "bcedit_madeby_train-0.0.6.tar", last modified: Tue Jul 18 13:01:40 2023, max compression
```

## Comparing `bcedit_madeby_train-0.0.5.tar` & `bcedit_madeby_train-0.0.6.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 12:58:44.008165 bcedit_madeby_train-0.0.5/
--rw-rw-rw-   0        0        0      479 2023-07-18 12:58:44.008165 bcedit_madeby_train-0.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-18 12:58:43.695767 bcedit_madeby_train-0.0.5/bcedit_madeby_train/
--rw-rw-rw-   0        0        0      281 2023-07-16 12:52:11.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/__init__.py
--rw-rw-rw-   0        0        0     8301 2023-07-16 12:52:11.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/__main__.py
--rw-rw-rw-   0        0        0    10151 2023-07-16 12:52:10.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/adb_handler.py
--rw-rw-rw-   0        0        0    13745 2023-07-16 12:52:10.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/config_manager.py
--rw-rw-rw-   0        0        0     1501 2023-07-16 12:52:10.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/csv_handler.py
-drwxrwxrwx   0        0        0        0 2023-07-18 12:58:43.758246 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/
--rw-rw-rw-   0        0        0       67 2023-07-16 12:52:14.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 12:58:43.789487 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/basic/
--rw-rw-rw-   0        0        0      122 2023-07-16 12:52:21.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/basic/__init__.py
--rw-rw-rw-   0        0        0     8690 2023-07-16 12:52:20.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/basic/basic_items.py
--rw-rw-rw-   0        0        0     1490 2023-07-16 12:52:20.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/basic/catfruit.py
--rw-rw-rw-   0        0        0     1931 2023-07-16 12:52:20.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/basic/catseyes.py
--rw-rw-rw-   0        0        0     1647 2023-07-16 12:52:20.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/basic/ototo_base_mats.py
--rw-rw-rw-   0        0        0     3984 2023-07-16 12:52:20.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/basic/talent_orbs.py
--rw-rw-rw-   0        0        0    16533 2023-07-16 12:52:20.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/basic/talent_orbs_new.py
-drwxrwxrwx   0        0        0        0 2023-07-18 12:58:43.836347 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/cats/
--rw-rw-rw-   0        0        0      179 2023-07-16 12:52:19.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/cats/__init__.py
--rw-rw-rw-   0        0        0     8978 2023-07-16 12:52:19.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/cats/cat_helper.py
--rw-rw-rw-   0        0        0    11121 2023-07-16 12:52:19.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/cats/cat_id_selector.py
--rw-rw-rw-   0        0        0     3249 2023-07-16 12:52:19.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/cats/chara_drop.py
--rw-rw-rw-   0        0        0     1068 2023-07-16 12:52:19.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/cats/clear_cat_guide.py
--rw-rw-rw-   0        0        0     3145 2023-07-18 11:00:13.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/cats/evolve_cats.py
--rw-rw-rw-   0        0        0     1555 2023-07-16 12:52:19.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/cats/get_remove_cats.py
--rw-rw-rw-   0        0        0     7936 2023-07-16 12:52:19.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/cats/talents.py
--rw-rw-rw-   0        0        0     1661 2023-07-18 11:44:06.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/cats/upgrade_blue.py
--rw-rw-rw-   0        0        0     6658 2023-07-18 12:33:12.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/cats/upgrade_cats.py
-drwxrwxrwx   0        0        0        0 2023-07-18 12:58:43.867589 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/gamototo/
--rw-rw-rw-   0        0        0       66 2023-07-16 12:52:19.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/gamototo/__init__.py
--rw-rw-rw-   0        0        0      309 2023-07-16 12:52:18.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/gamototo/fix_gamatoto.py
--rw-rw-rw-   0        0        0     2794 2023-07-16 12:52:18.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/gamototo/gamatoto_xp.py
--rw-rw-rw-   0        0        0     3393 2023-07-16 12:52:18.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/gamototo/helpers.py
--rw-rw-rw-   0        0        0     4137 2023-07-16 12:52:18.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/gamototo/ototo_cat_cannon.py
-drwxrwxrwx   0        0        0        0 2023-07-18 12:58:43.930068 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/levels/
--rw-rw-rw-   0        0        0      313 2023-07-16 12:52:17.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/levels/__init__.py
--rw-rw-rw-   0        0        0     1035 2023-07-16 12:52:16.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/levels/aku.py
--rw-rw-rw-   0        0        0      491 2023-07-16 12:52:16.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/levels/allow_filibuster_clearing.py
--rw-rw-rw-   0        0        0      790 2023-07-16 12:52:16.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/levels/behemoth_culling.py
--rw-rw-rw-   0        0        0      646 2023-07-16 12:52:16.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/levels/clear_tutorial.py
--rw-rw-rw-   0        0        0     1121 2023-07-16 12:52:16.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/levels/enigma_stages.py
--rw-rw-rw-   0        0        0     6307 2023-07-16 12:52:17.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/levels/event_stages.py
--rw-rw-rw-   0        0        0     1873 2023-07-16 12:52:17.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/levels/gauntlet.py
--rw-rw-rw-   0        0        0     1027 2023-07-16 12:52:17.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/levels/itf_timed_scores.py
--rw-rw-rw-   0        0        0     1469 2023-07-16 12:52:17.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/levels/legend_quest.py
--rw-rw-rw-   0        0        0     4408 2023-07-16 12:52:17.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/levels/main_story.py
--rw-rw-rw-   0        0        0     2323 2023-07-16 12:52:17.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/levels/outbreaks.py
--rw-rw-rw-   0        0        0     3031 2023-07-16 12:52:17.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/levels/story_level_id_selector.py
--rw-rw-rw-   0        0        0     1175 2023-07-16 12:52:17.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/levels/towers.py
--rw-rw-rw-   0        0        0     8458 2023-07-16 12:52:17.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/levels/treasures.py
--rw-rw-rw-   0        0        0     1043 2023-07-16 12:52:17.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/levels/uncanny.py
--rw-rw-rw-   0        0        0      784 2023-07-16 12:52:17.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/levels/unlock_aku_realm.py
-drwxrwxrwx   0        0        0        0 2023-07-18 12:58:43.976932 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/other/
--rw-rw-rw-   0        0        0      276 2023-07-16 12:52:15.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/other/__init__.py
--rw-rw-rw-   0        0        0     3878 2023-07-16 12:52:14.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/other/cat_shrine.py
--rw-rw-rw-   0        0        0     1093 2023-07-16 12:52:14.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/other/claim_user_rank_rewards.py
--rw-rw-rw-   0        0        0     1054 2023-07-16 12:52:15.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/other/create_new_account.py
--rw-rw-rw-   0        0        0     2187 2023-07-16 12:52:15.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/other/fix_elsewhere.py
--rw-rw-rw-   0        0        0      659 2023-07-16 12:52:15.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/other/fix_time_issues.py
--rw-rw-rw-   0        0        0     3825 2023-07-17 08:14:21.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/other/get_gold_pass.py
--rw-rw-rw-   0        0        0     6773 2023-07-18 11:00:49.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/other/meow_medals.py
--rw-rw-rw-   0        0        0     4354 2023-07-16 12:52:15.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/other/missions.py
--rw-rw-rw-   0        0        0      975 2023-07-16 12:52:15.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/other/play_time.py
--rw-rw-rw-   0        0        0     4568 2023-07-16 12:52:15.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/other/scheme_item.py
--rw-rw-rw-   0        0        0     1612 2023-07-16 12:52:15.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/other/trade_progress.py
--rw-rw-rw-   0        0        0      914 2023-07-18 11:01:47.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/other/unlock_enemy_guide.py
--rw-rw-rw-   0        0        0      326 2023-07-16 12:52:15.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/other/unlock_equip_menu.py
-drwxrwxrwx   0        0        0        0 2023-07-18 12:58:44.008165 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/save_management/
--rw-rw-rw-   0        0        0       56 2023-07-16 12:52:14.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/save_management/__init__.py
--rw-rw-rw-   0        0        0     1273 2023-07-16 12:52:14.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/save_management/convert.py
--rw-rw-rw-   0        0        0     2578 2023-07-16 12:52:14.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/save_management/load.py
--rw-rw-rw-   0        0        0      644 2023-07-16 12:52:14.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/save_management/other.py
--rw-rw-rw-   0        0        0     2049 2023-07-16 12:52:14.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/save_management/save.py
--rw-rw-rw-   0        0        0     1862 2023-07-16 12:52:14.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/save_management/server_upload.py
--rw-rw-rw-   0        0        0    12118 2023-07-16 12:52:10.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/feature_handler.py
--rw-rw-rw-   0        0        0     4822 2023-07-16 12:52:10.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/game_data_getter.py
--rw-rw-rw-   0        0        0    22858 2023-07-18 12:48:49.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/helper.py
--rw-rw-rw-   0        0        0     7075 2023-07-16 12:52:10.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/item.py
--rw-rw-rw-   0        0        0     3505 2023-07-16 12:52:11.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/locale_handler.py
--rw-rw-rw-   0        0        0     1269 2023-07-16 12:52:11.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/managed_item.py
--rw-rw-rw-   0        0        0    66964 2023-07-16 12:52:11.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/parse_save.py
--rw-rw-rw-   0        0        0     1301 2023-07-16 12:52:11.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/patcher.py
--rw-rw-rw-   0        0        0     2415 2023-07-16 12:52:11.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/root_handler.py
--rw-rw-rw-   0        0        0    53791 2023-07-16 12:52:11.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/serialise_save.py
--rw-rw-rw-   0        0        0    24970 2023-07-16 12:52:11.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/server_handler.py
--rw-rw-rw-   0        0        0     3717 2023-07-16 12:52:11.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/tracker.py
--rw-rw-rw-   0        0        0     3496 2023-07-18 12:57:46.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/updater.py
--rw-rw-rw-   0        0        0     8297 2023-07-16 12:52:11.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train/user_input_handler.py
-drwxrwxrwx   0        0        0        0 2023-07-18 12:58:43.758246 bcedit_madeby_train-0.0.5/bcedit_madeby_train.egg-info/
--rw-rw-rw-   0        0        0      479 2023-07-18 12:58:43.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3853 2023-07-18 12:58:43.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 12:58:43.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-18 12:58:43.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       50 2023-07-18 12:58:43.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-18 12:58:43.000000 bcedit_madeby_train-0.0.5/bcedit_madeby_train.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 12:58:44.008165 bcedit_madeby_train-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      811 2023-07-18 12:58:02.000000 bcedit_madeby_train-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 13:01:40.113111 bcedit_madeby_train-0.0.6/
+-rw-rw-rw-   0        0        0      479 2023-07-18 13:01:40.113111 bcedit_madeby_train-0.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-18 13:01:39.800716 bcedit_madeby_train-0.0.6/bcedit_madeby_train/
+-rw-rw-rw-   0        0        0      281 2023-07-16 12:52:11.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/__init__.py
+-rw-rw-rw-   0        0        0     8301 2023-07-16 12:52:11.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/__main__.py
+-rw-rw-rw-   0        0        0    10151 2023-07-16 12:52:10.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/adb_handler.py
+-rw-rw-rw-   0        0        0    13745 2023-07-16 12:52:10.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/config_manager.py
+-rw-rw-rw-   0        0        0     1501 2023-07-16 12:52:10.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/csv_handler.py
+drwxrwxrwx   0        0        0        0 2023-07-18 13:01:39.863190 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/
+-rw-rw-rw-   0        0        0       67 2023-07-16 12:52:14.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 13:01:39.894430 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/basic/
+-rw-rw-rw-   0        0        0      122 2023-07-16 12:52:21.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/basic/__init__.py
+-rw-rw-rw-   0        0        0     8690 2023-07-16 12:52:20.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/basic/basic_items.py
+-rw-rw-rw-   0        0        0     1490 2023-07-16 12:52:20.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/basic/catfruit.py
+-rw-rw-rw-   0        0        0     1931 2023-07-16 12:52:20.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/basic/catseyes.py
+-rw-rw-rw-   0        0        0     1647 2023-07-16 12:52:20.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/basic/ototo_base_mats.py
+-rw-rw-rw-   0        0        0     3984 2023-07-16 12:52:20.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/basic/talent_orbs.py
+-rw-rw-rw-   0        0        0    16533 2023-07-16 12:52:20.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/basic/talent_orbs_new.py
+drwxrwxrwx   0        0        0        0 2023-07-18 13:01:39.925670 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/cats/
+-rw-rw-rw-   0        0        0      179 2023-07-16 12:52:19.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/cats/__init__.py
+-rw-rw-rw-   0        0        0     8978 2023-07-16 12:52:19.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/cats/cat_helper.py
+-rw-rw-rw-   0        0        0    11121 2023-07-16 12:52:19.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/cats/cat_id_selector.py
+-rw-rw-rw-   0        0        0     3249 2023-07-16 12:52:19.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/cats/chara_drop.py
+-rw-rw-rw-   0        0        0     1068 2023-07-16 12:52:19.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/cats/clear_cat_guide.py
+-rw-rw-rw-   0        0        0     3145 2023-07-18 11:00:13.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/cats/evolve_cats.py
+-rw-rw-rw-   0        0        0     1555 2023-07-16 12:52:19.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/cats/get_remove_cats.py
+-rw-rw-rw-   0        0        0     7936 2023-07-16 12:52:19.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/cats/talents.py
+-rw-rw-rw-   0        0        0     1661 2023-07-18 11:44:06.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/cats/upgrade_blue.py
+-rw-rw-rw-   0        0        0     6658 2023-07-18 12:33:12.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/cats/upgrade_cats.py
+drwxrwxrwx   0        0        0        0 2023-07-18 13:01:39.956910 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/gamototo/
+-rw-rw-rw-   0        0        0       66 2023-07-16 12:52:19.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/gamototo/__init__.py
+-rw-rw-rw-   0        0        0      309 2023-07-16 12:52:18.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/gamototo/fix_gamatoto.py
+-rw-rw-rw-   0        0        0     2794 2023-07-16 12:52:18.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/gamototo/gamatoto_xp.py
+-rw-rw-rw-   0        0        0     3393 2023-07-16 12:52:18.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/gamototo/helpers.py
+-rw-rw-rw-   0        0        0     4137 2023-07-16 12:52:18.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/gamototo/ototo_cat_cannon.py
+drwxrwxrwx   0        0        0        0 2023-07-18 13:01:40.019389 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/levels/
+-rw-rw-rw-   0        0        0      313 2023-07-16 12:52:17.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/levels/__init__.py
+-rw-rw-rw-   0        0        0     1035 2023-07-16 12:52:16.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/levels/aku.py
+-rw-rw-rw-   0        0        0      491 2023-07-16 12:52:16.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/levels/allow_filibuster_clearing.py
+-rw-rw-rw-   0        0        0      790 2023-07-16 12:52:16.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/levels/behemoth_culling.py
+-rw-rw-rw-   0        0        0      646 2023-07-16 12:52:16.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/levels/clear_tutorial.py
+-rw-rw-rw-   0        0        0     1121 2023-07-16 12:52:16.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/levels/enigma_stages.py
+-rw-rw-rw-   0        0        0     6307 2023-07-16 12:52:17.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/levels/event_stages.py
+-rw-rw-rw-   0        0        0     1873 2023-07-16 12:52:17.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/levels/gauntlet.py
+-rw-rw-rw-   0        0        0     1027 2023-07-16 12:52:17.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/levels/itf_timed_scores.py
+-rw-rw-rw-   0        0        0     1469 2023-07-16 12:52:17.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/levels/legend_quest.py
+-rw-rw-rw-   0        0        0     4408 2023-07-16 12:52:17.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/levels/main_story.py
+-rw-rw-rw-   0        0        0     2323 2023-07-16 12:52:17.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/levels/outbreaks.py
+-rw-rw-rw-   0        0        0     3031 2023-07-16 12:52:17.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/levels/story_level_id_selector.py
+-rw-rw-rw-   0        0        0     1175 2023-07-16 12:52:17.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/levels/towers.py
+-rw-rw-rw-   0        0        0     8458 2023-07-16 12:52:17.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/levels/treasures.py
+-rw-rw-rw-   0        0        0     1043 2023-07-16 12:52:17.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/levels/uncanny.py
+-rw-rw-rw-   0        0        0      784 2023-07-16 12:52:17.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/levels/unlock_aku_realm.py
+drwxrwxrwx   0        0        0        0 2023-07-18 13:01:40.066249 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/other/
+-rw-rw-rw-   0        0        0      276 2023-07-16 12:52:15.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/other/__init__.py
+-rw-rw-rw-   0        0        0     3878 2023-07-16 12:52:14.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/other/cat_shrine.py
+-rw-rw-rw-   0        0        0     1093 2023-07-16 12:52:14.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/other/claim_user_rank_rewards.py
+-rw-rw-rw-   0        0        0     1054 2023-07-16 12:52:15.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/other/create_new_account.py
+-rw-rw-rw-   0        0        0     2187 2023-07-16 12:52:15.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/other/fix_elsewhere.py
+-rw-rw-rw-   0        0        0      659 2023-07-16 12:52:15.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/other/fix_time_issues.py
+-rw-rw-rw-   0        0        0     3825 2023-07-17 08:14:21.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/other/get_gold_pass.py
+-rw-rw-rw-   0        0        0     6773 2023-07-18 11:00:49.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/other/meow_medals.py
+-rw-rw-rw-   0        0        0     4354 2023-07-16 12:52:15.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/other/missions.py
+-rw-rw-rw-   0        0        0      975 2023-07-16 12:52:15.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/other/play_time.py
+-rw-rw-rw-   0        0        0     4568 2023-07-16 12:52:15.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/other/scheme_item.py
+-rw-rw-rw-   0        0        0     1612 2023-07-16 12:52:15.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/other/trade_progress.py
+-rw-rw-rw-   0        0        0      914 2023-07-18 11:01:47.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/other/unlock_enemy_guide.py
+-rw-rw-rw-   0        0        0      326 2023-07-16 12:52:15.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/other/unlock_equip_menu.py
+drwxrwxrwx   0        0        0        0 2023-07-18 13:01:40.097491 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/save_management/
+-rw-rw-rw-   0        0        0       56 2023-07-16 12:52:14.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/save_management/__init__.py
+-rw-rw-rw-   0        0        0     1273 2023-07-16 12:52:14.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/save_management/convert.py
+-rw-rw-rw-   0        0        0     2578 2023-07-16 12:52:14.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/save_management/load.py
+-rw-rw-rw-   0        0        0      644 2023-07-16 12:52:14.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/save_management/other.py
+-rw-rw-rw-   0        0        0     2049 2023-07-16 12:52:14.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/save_management/save.py
+-rw-rw-rw-   0        0        0     1862 2023-07-16 12:52:14.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/save_management/server_upload.py
+-rw-rw-rw-   0        0        0    12118 2023-07-16 12:52:10.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/feature_handler.py
+-rw-rw-rw-   0        0        0     4822 2023-07-16 12:52:10.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/game_data_getter.py
+-rw-rw-rw-   0        0        0    22858 2023-07-18 12:48:49.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/helper.py
+-rw-rw-rw-   0        0        0     7075 2023-07-16 12:52:10.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/item.py
+-rw-rw-rw-   0        0        0     3505 2023-07-16 12:52:11.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/locale_handler.py
+-rw-rw-rw-   0        0        0     1269 2023-07-16 12:52:11.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/managed_item.py
+-rw-rw-rw-   0        0        0    66964 2023-07-16 12:52:11.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/parse_save.py
+-rw-rw-rw-   0        0        0     1301 2023-07-16 12:52:11.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/patcher.py
+-rw-rw-rw-   0        0        0     2415 2023-07-16 12:52:11.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/root_handler.py
+-rw-rw-rw-   0        0        0    53791 2023-07-16 12:52:11.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/serialise_save.py
+-rw-rw-rw-   0        0        0    24970 2023-07-16 12:52:11.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/server_handler.py
+-rw-rw-rw-   0        0        0     3717 2023-07-16 12:52:11.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/tracker.py
+-rw-rw-rw-   0        0        0     3496 2023-07-18 12:57:46.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/updater.py
+-rw-rw-rw-   0        0        0     8297 2023-07-16 12:52:11.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train/user_input_handler.py
+drwxrwxrwx   0        0        0        0 2023-07-18 13:01:39.863190 bcedit_madeby_train-0.0.6/bcedit_madeby_train.egg-info/
+-rw-rw-rw-   0        0        0      479 2023-07-18 13:01:39.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3853 2023-07-18 13:01:39.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 13:01:39.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-18 13:01:39.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       50 2023-07-18 13:01:39.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-18 13:01:39.000000 bcedit_madeby_train-0.0.6/bcedit_madeby_train.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 13:01:40.113111 bcedit_madeby_train-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      811 2023-07-18 13:01:27.000000 bcedit_madeby_train-0.0.6/setup.py
```

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/__main__.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/__main__.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/adb_handler.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/adb_handler.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/config_manager.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/config_manager.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/csv_handler.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/csv_handler.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/basic/basic_items.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/basic/basic_items.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/basic/catfruit.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/basic/catfruit.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/basic/catseyes.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/basic/catseyes.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/basic/ototo_base_mats.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/basic/ototo_base_mats.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/basic/talent_orbs.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/basic/talent_orbs.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/basic/talent_orbs_new.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/basic/talent_orbs_new.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/cats/cat_helper.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/cats/cat_helper.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/cats/cat_id_selector.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/cats/cat_id_selector.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/cats/chara_drop.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/cats/chara_drop.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/cats/clear_cat_guide.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/cats/clear_cat_guide.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/cats/evolve_cats.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/cats/evolve_cats.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/cats/get_remove_cats.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/cats/get_remove_cats.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/cats/talents.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/cats/talents.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/cats/upgrade_blue.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/cats/upgrade_blue.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/cats/upgrade_cats.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/cats/upgrade_cats.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/gamototo/gamatoto_xp.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/gamototo/gamatoto_xp.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/gamototo/helpers.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/gamototo/helpers.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/gamototo/ototo_cat_cannon.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/gamototo/ototo_cat_cannon.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/levels/aku.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/levels/aku.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/levels/behemoth_culling.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/levels/behemoth_culling.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/levels/clear_tutorial.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/levels/clear_tutorial.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/levels/enigma_stages.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/levels/enigma_stages.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/levels/event_stages.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/levels/event_stages.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/levels/gauntlet.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/levels/gauntlet.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/levels/itf_timed_scores.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/levels/itf_timed_scores.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/levels/legend_quest.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/levels/legend_quest.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/levels/main_story.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/levels/main_story.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/levels/outbreaks.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/levels/outbreaks.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/levels/story_level_id_selector.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/levels/story_level_id_selector.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/levels/towers.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/levels/towers.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/levels/treasures.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/levels/treasures.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/levels/uncanny.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/levels/uncanny.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/levels/unlock_aku_realm.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/levels/unlock_aku_realm.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/other/cat_shrine.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/other/cat_shrine.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/other/claim_user_rank_rewards.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/other/claim_user_rank_rewards.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/other/create_new_account.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/other/create_new_account.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/other/fix_elsewhere.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/other/fix_elsewhere.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/other/fix_time_issues.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/other/fix_time_issues.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/other/get_gold_pass.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/other/get_gold_pass.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/other/meow_medals.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/other/meow_medals.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/other/missions.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/other/missions.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/other/play_time.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/other/play_time.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/other/scheme_item.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/other/scheme_item.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/other/trade_progress.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/other/trade_progress.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/other/unlock_enemy_guide.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/other/unlock_enemy_guide.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/save_management/convert.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/save_management/convert.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/save_management/load.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/save_management/load.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/save_management/other.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/save_management/other.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/save_management/save.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/save_management/save.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/edits/save_management/server_upload.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/edits/save_management/server_upload.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/feature_handler.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/feature_handler.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/game_data_getter.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/game_data_getter.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/helper.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/helper.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/item.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/item.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/locale_handler.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/locale_handler.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/managed_item.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/managed_item.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/parse_save.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/parse_save.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/patcher.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/patcher.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/root_handler.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/root_handler.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/serialise_save.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/serialise_save.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/server_handler.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/server_handler.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/tracker.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/tracker.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/updater.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/updater.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train/user_input_handler.py` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train/user_input_handler.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/bcedit_madeby_train.egg-info/SOURCES.txt` & `bcedit_madeby_train-0.0.6/bcedit_madeby_train.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.5/setup.py` & `bcedit_madeby_train-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='bcedit_madeby_train',
-    version='0.0.5',
+    version='0.0.6',
     description='This is a project developed by Serem for development purposes',
     author='serem',
     author_email='gangh9230@gmail.com',
     url='https://github.com/hayul0629/wdex',
     install_requires=[
         "colored==1.4.4",
         "tk",
```

