# Comparing `tmp/yz-core2-1.0.56b2.tar.gz` & `tmp/yz-core2-1.0.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yz-core2-1.0.56b2.tar", last modified: Thu Jun 29 06:22:39 2023, max compression
+gzip compressed data, was "yz-core2-1.0.60.tar", last modified: Wed Jul 12 08:02:03 2023, max compression
```

## Comparing `yz-core2-1.0.56b2.tar` & `yz-core2-1.0.60.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-29 06:22:39.966537 yz-core2-1.0.56b2/
--rw-r--r--   0 zhouwei    (501) staff       (20)     1085 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/LICENSE
--rw-r--r--   0 zhouwei    (501) staff       (20)     3114 2023-06-29 06:22:39.966405 yz-core2-1.0.56b2/PKG-INFO
--rw-r--r--   0 zhouwei    (501) staff       (20)     2509 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/README.md
--rw-r--r--   0 zhouwei    (501) staff       (20)       38 2023-06-29 06:22:39.966580 yz-core2-1.0.56b2/setup.cfg
--rw-r--r--   0 zhouwei    (501) staff       (20)     1785 2023-06-29 06:21:47.000000 yz-core2-1.0.56b2/setup.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-29 06:22:39.948381 yz-core2-1.0.56b2/tests/
--rw-r--r--   0 zhouwei    (501) staff       (20)       94 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/tests/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      965 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/tests/test_setting_reload.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1822 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/tests/test_uid.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-29 06:22:39.949330 yz-core2-1.0.56b2/yz_core2.egg-info/
--rw-r--r--   0 zhouwei    (501) staff       (20)     3114 2023-06-29 06:22:39.000000 yz-core2-1.0.56b2/yz_core2.egg-info/PKG-INFO
--rw-r--r--   0 zhouwei    (501) staff       (20)     3594 2023-06-29 06:22:39.000000 yz-core2-1.0.56b2/yz_core2.egg-info/SOURCES.txt
--rw-r--r--   0 zhouwei    (501) staff       (20)        1 2023-06-29 06:22:39.000000 yz-core2-1.0.56b2/yz_core2.egg-info/dependency_links.txt
--rw-r--r--   0 zhouwei    (501) staff       (20)       48 2023-06-29 06:22:39.000000 yz-core2-1.0.56b2/yz_core2.egg-info/entry_points.txt
--rw-r--r--   0 zhouwei    (501) staff       (20)      240 2023-06-29 06:22:39.000000 yz-core2-1.0.56b2/yz_core2.egg-info/requires.txt
--rw-r--r--   0 zhouwei    (501) staff       (20)       13 2023-06-29 06:22:39.000000 yz-core2-1.0.56b2/yz_core2.egg-info/top_level.txt
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-29 06:22:39.950501 yz-core2-1.0.56b2/yzcore/
--rw-r--r--   0 zhouwei    (501) staff       (20)       90 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      440 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/__main__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-29 06:22:39.951469 yz-core2-1.0.56b2/yzcore/core/
--rw-r--r--   0 zhouwei    (501) staff       (20)       95 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/core/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      301 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/core/const.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      466 2023-06-28 05:59:58.000000 yz-core2-1.0.56b2/yzcore/core/data_hash.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     4722 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/core/datastructures.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     5244 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/core/encoders.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-29 06:22:39.952024 yz-core2-1.0.56b2/yzcore/core/management/
--rw-r--r--   0 zhouwei    (501) staff       (20)      614 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/core/management/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      122 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/core/management/base.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-29 06:22:39.952480 yz-core2-1.0.56b2/yzcore/core/management/commands/
--rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/core/management/commands/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      594 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/core/management/commands/startapp.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      783 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/core/management/commands/startproject.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     5219 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/core/management/templates.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     6334 2023-06-29 03:18:27.000000 yz-core2-1.0.56b2/yzcore/core/storage.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-29 06:22:39.953069 yz-core2-1.0.56b2/yzcore/db/
--rw-r--r--   0 zhouwei    (501) staff       (20)       92 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/db/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1413 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/db/db_session.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     7679 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/db/pymongo_crud_base.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     7165 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/db/sqlalchemy_crud_base.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1651 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/decorators.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     2525 2023-05-16 05:58:39.000000 yz-core2-1.0.56b2/yzcore/default_settings.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     2695 2023-06-21 07:48:50.000000 yz-core2-1.0.56b2/yzcore/exceptions.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-29 06:22:39.953328 yz-core2-1.0.56b2/yzcore/extensions/
--rw-r--r--   0 zhouwei    (501) staff       (20)       93 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/extensions/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-29 06:22:39.954440 yz-core2-1.0.56b2/yzcore/extensions/storage/
--rw-r--r--   0 zhouwei    (501) staff       (20)     1830 2023-06-21 08:59:49.000000 yz-core2-1.0.56b2/yzcore/extensions/storage/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-29 06:22:39.954865 yz-core2-1.0.56b2/yzcore/extensions/storage/amazon/
--rw-r--r--   0 zhouwei    (501) staff       (20)     6691 2023-06-29 03:02:25.000000 yz-core2-1.0.56b2/yzcore/extensions/storage/amazon/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      838 2023-06-21 07:48:50.000000 yz-core2-1.0.56b2/yzcore/extensions/storage/amazon/utils.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-29 06:22:39.955285 yz-core2-1.0.56b2/yzcore/extensions/storage/azure/
--rw-r--r--   0 zhouwei    (501) staff       (20)     8288 2023-06-28 09:52:19.000000 yz-core2-1.0.56b2/yzcore/extensions/storage/azure/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      465 2023-06-28 09:52:19.000000 yz-core2-1.0.56b2/yzcore/extensions/storage/azure/utils.py
--rw-r--r--   0 zhouwei    (501) staff       (20)    12248 2023-06-29 06:19:15.000000 yz-core2-1.0.56b2/yzcore/extensions/storage/base.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      724 2023-06-21 10:47:27.000000 yz-core2-1.0.56b2/yzcore/extensions/storage/const.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-29 06:22:39.955700 yz-core2-1.0.56b2/yzcore/extensions/storage/minio/
--rw-r--r--   0 zhouwei    (501) staff       (20)     9712 2023-06-29 03:06:15.000000 yz-core2-1.0.56b2/yzcore/extensions/storage/minio/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      820 2023-06-21 07:48:50.000000 yz-core2-1.0.56b2/yzcore/extensions/storage/minio/utils.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-29 06:22:39.956658 yz-core2-1.0.56b2/yzcore/extensions/storage/obs/
--rw-r--r--   0 zhouwei    (501) staff       (20)     9388 2023-06-29 06:19:15.000000 yz-core2-1.0.56b2/yzcore/extensions/storage/obs/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1109 2023-04-21 02:05:49.000000 yz-core2-1.0.56b2/yzcore/extensions/storage/obs/const.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     3101 2023-05-06 02:48:14.000000 yz-core2-1.0.56b2/yzcore/extensions/storage/obs/obs_inherit.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      678 2023-06-21 07:48:50.000000 yz-core2-1.0.56b2/yzcore/extensions/storage/obs/utils.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-29 06:22:39.957285 yz-core2-1.0.56b2/yzcore/extensions/storage/oss/
--rw-r--r--   0 zhouwei    (501) staff       (20)    11341 2023-06-29 03:03:39.000000 yz-core2-1.0.56b2/yzcore/extensions/storage/oss/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      762 2023-04-21 02:05:49.000000 yz-core2-1.0.56b2/yzcore/extensions/storage/oss/const.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      699 2023-06-21 07:48:50.000000 yz-core2-1.0.56b2/yzcore/extensions/storage/oss/utils.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1394 2023-06-29 06:19:15.000000 yz-core2-1.0.56b2/yzcore/extensions/storage/schemas.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      878 2023-06-28 07:37:13.000000 yz-core2-1.0.56b2/yzcore/extensions/storage/utils.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     2724 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/extensions/uid.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-29 06:22:39.960089 yz-core2-1.0.56b2/yzcore/logger/
--rw-r--r--   0 zhouwei    (501) staff       (20)     6943 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/logger/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)    10770 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/logger/config.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1177 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/logger/filters.py
--rw-r--r--   0 zhouwei    (501) staff       (20)    10780 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/logger/handlers.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-29 06:22:39.960393 yz-core2-1.0.56b2/yzcore/request/
--rw-r--r--   0 zhouwei    (501) staff       (20)      133 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/request/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     8293 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/request/aio_http.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-29 06:22:39.960813 yz-core2-1.0.56b2/yzcore/response/
--rw-r--r--   0 zhouwei    (501) staff       (20)      188 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/response/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     2934 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/response/response.py
--rw-r--r--   0 zhouwei    (501) staff       (20)    36606 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/response/response_code.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-29 06:22:39.961011 yz-core2-1.0.56b2/yzcore/templates/
--rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/templates/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-29 06:22:39.961763 yz-core2-1.0.56b2/yzcore/templates/app_template/
--rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/templates/app_template/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      945 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/templates/app_template/controllers.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      421 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/templates/app_template/models.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      907 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/templates/app_template/schemas.py
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/templates/app_template/tests.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1632 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/templates/app_template/views.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-29 06:22:39.962131 yz-core2-1.0.56b2/yzcore/templates/project_template/
--rw-r--r--   0 zhouwei    (501) staff       (20)     1816 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/templates/project_template/.gitignore
--rw-r--r--   0 zhouwei    (501) staff       (20)     2508 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/templates/project_template/README.md
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-29 06:22:39.962372 yz-core2-1.0.56b2/yzcore/templates/project_template/docs/
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/templates/project_template/docs/install_explain.md
--rw-r--r--   0 zhouwei    (501) staff       (20)      922 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/templates/project_template/docs/supervisor.ini
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-29 06:22:39.962511 yz-core2-1.0.56b2/yzcore/templates/project_template/migrations/
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/templates/project_template/migrations/README.md
--rw-r--r--   0 zhouwei    (501) staff       (20)      453 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/templates/project_template/requirements.txt
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-29 06:22:39.962857 yz-core2-1.0.56b2/yzcore/templates/project_template/src/
--rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/templates/project_template/src/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-29 06:22:39.962998 yz-core2-1.0.56b2/yzcore/templates/project_template/src/apps/
--rw-r--r--   0 zhouwei    (501) staff       (20)       90 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/templates/project_template/src/apps/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-29 06:22:39.963667 yz-core2-1.0.56b2/yzcore/templates/project_template/src/conf/
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/templates/project_template/src/conf/config_dev.ini
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/templates/project_template/src/conf/config_dev.yaml
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/templates/project_template/src/conf/config_production.ini
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/templates/project_template/src/conf/config_production.yaml
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/templates/project_template/src/conf/config_testing.ini
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/templates/project_template/src/conf/config_testing.yaml
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-29 06:22:39.964171 yz-core2-1.0.56b2/yzcore/templates/project_template/src/const/
--rw-r--r--   0 zhouwei    (501) staff       (20)      157 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/templates/project_template/src/const/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      409 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/templates/project_template/src/const/_job.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      418 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/templates/project_template/src/const/_task.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      843 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/templates/project_template/src/main.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      807 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/templates/project_template/src/settings.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-29 06:22:39.964474 yz-core2-1.0.56b2/yzcore/templates/project_template/src/tests/
--rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/templates/project_template/src/tests/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      840 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/templates/project_template/src/tests/test_xxx.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-29 06:22:39.964612 yz-core2-1.0.56b2/yzcore/templates/project_template/src/utils/
--rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/templates/project_template/src/utils/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-29 06:22:39.966129 yz-core2-1.0.56b2/yzcore/utils/
--rw-r--r--   0 zhouwei    (501) staff       (20)      386 2023-06-21 07:25:34.000000 yz-core2-1.0.56b2/yzcore/utils/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      231 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/utils/check_path.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1293 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/utils/check_sys.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     2229 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/utils/crypto.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     2064 2023-06-29 03:18:27.000000 yz-core2-1.0.56b2/yzcore/utils/decorator.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     9061 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/utils/encoding.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1755 2023-04-21 02:16:16.000000 yz-core2-1.0.56b2/yzcore/utils/nacos.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     2129 2023-05-09 10:16:49.000000 yz-core2-1.0.56b2/yzcore/utils/time_utils.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-12 08:02:03.009018 yz-core2-1.0.60/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1085 2023-04-21 02:16:16.000000 yz-core2-1.0.60/LICENSE
+-rw-r--r--   0 zhouwei    (501) staff       (20)     3112 2023-07-12 08:02:03.008871 yz-core2-1.0.60/PKG-INFO
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2509 2023-04-21 02:16:16.000000 yz-core2-1.0.60/README.md
+-rw-r--r--   0 zhouwei    (501) staff       (20)       38 2023-07-12 08:02:03.009055 yz-core2-1.0.60/setup.cfg
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1783 2023-07-12 07:38:28.000000 yz-core2-1.0.60/setup.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-12 08:02:02.993133 yz-core2-1.0.60/tests/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       94 2023-04-21 02:16:16.000000 yz-core2-1.0.60/tests/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      965 2023-04-21 02:16:16.000000 yz-core2-1.0.60/tests/test_setting_reload.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1822 2023-04-21 02:16:16.000000 yz-core2-1.0.60/tests/test_uid.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-12 08:02:02.993951 yz-core2-1.0.60/yz_core2.egg-info/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     3112 2023-07-12 08:02:02.000000 yz-core2-1.0.60/yz_core2.egg-info/PKG-INFO
+-rw-r--r--   0 zhouwei    (501) staff       (20)     3594 2023-07-12 08:02:02.000000 yz-core2-1.0.60/yz_core2.egg-info/SOURCES.txt
+-rw-r--r--   0 zhouwei    (501) staff       (20)        1 2023-07-12 08:02:02.000000 yz-core2-1.0.60/yz_core2.egg-info/dependency_links.txt
+-rw-r--r--   0 zhouwei    (501) staff       (20)       48 2023-07-12 08:02:02.000000 yz-core2-1.0.60/yz_core2.egg-info/entry_points.txt
+-rw-r--r--   0 zhouwei    (501) staff       (20)      240 2023-07-12 08:02:02.000000 yz-core2-1.0.60/yz_core2.egg-info/requires.txt
+-rw-r--r--   0 zhouwei    (501) staff       (20)       13 2023-07-12 08:02:02.000000 yz-core2-1.0.60/yz_core2.egg-info/top_level.txt
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-12 08:02:02.994842 yz-core2-1.0.60/yzcore/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       90 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      440 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/__main__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-12 08:02:02.996112 yz-core2-1.0.60/yzcore/core/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       95 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/core/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      301 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/core/const.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      466 2023-06-28 05:59:58.000000 yz-core2-1.0.60/yzcore/core/data_hash.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     4722 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/core/datastructures.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     5244 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/core/encoders.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-12 08:02:02.996775 yz-core2-1.0.60/yzcore/core/management/
+-rw-r--r--   0 zhouwei    (501) staff       (20)      614 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/core/management/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      122 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/core/management/base.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-12 08:02:02.997257 yz-core2-1.0.60/yzcore/core/management/commands/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/core/management/commands/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      594 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/core/management/commands/startapp.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      783 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/core/management/commands/startproject.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     5219 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/core/management/templates.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     6334 2023-07-12 07:23:44.000000 yz-core2-1.0.60/yzcore/core/storage.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-12 08:02:02.997829 yz-core2-1.0.60/yzcore/db/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       92 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/db/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1413 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/db/db_session.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     7679 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/db/pymongo_crud_base.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     7165 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/db/sqlalchemy_crud_base.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1651 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/decorators.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2525 2023-05-16 05:58:39.000000 yz-core2-1.0.60/yzcore/default_settings.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2695 2023-07-12 07:23:44.000000 yz-core2-1.0.60/yzcore/exceptions.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-12 08:02:02.998104 yz-core2-1.0.60/yzcore/extensions/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       93 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/extensions/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-12 08:02:02.998828 yz-core2-1.0.60/yzcore/extensions/storage/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1830 2023-07-12 07:23:44.000000 yz-core2-1.0.60/yzcore/extensions/storage/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-12 08:02:02.999083 yz-core2-1.0.60/yzcore/extensions/storage/amazon/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     6691 2023-07-12 07:23:44.000000 yz-core2-1.0.60/yzcore/extensions/storage/amazon/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      838 2023-07-12 07:23:44.000000 yz-core2-1.0.60/yzcore/extensions/storage/amazon/utils.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-12 08:02:02.999405 yz-core2-1.0.60/yzcore/extensions/storage/azure/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     8281 2023-07-12 07:26:10.000000 yz-core2-1.0.60/yzcore/extensions/storage/azure/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      465 2023-07-12 07:23:44.000000 yz-core2-1.0.60/yzcore/extensions/storage/azure/utils.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)    12848 2023-07-12 07:58:49.000000 yz-core2-1.0.60/yzcore/extensions/storage/base.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      724 2023-07-12 07:23:44.000000 yz-core2-1.0.60/yzcore/extensions/storage/const.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-12 08:02:02.999734 yz-core2-1.0.60/yzcore/extensions/storage/minio/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     9578 2023-07-12 07:27:42.000000 yz-core2-1.0.60/yzcore/extensions/storage/minio/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      820 2023-07-12 07:23:44.000000 yz-core2-1.0.60/yzcore/extensions/storage/minio/utils.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-12 08:02:03.000689 yz-core2-1.0.60/yzcore/extensions/storage/obs/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     9388 2023-07-12 07:30:17.000000 yz-core2-1.0.60/yzcore/extensions/storage/obs/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1109 2023-04-21 02:05:49.000000 yz-core2-1.0.60/yzcore/extensions/storage/obs/const.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     3101 2023-05-06 02:48:14.000000 yz-core2-1.0.60/yzcore/extensions/storage/obs/obs_inherit.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      678 2023-07-12 07:23:44.000000 yz-core2-1.0.60/yzcore/extensions/storage/obs/utils.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-12 08:02:03.001321 yz-core2-1.0.60/yzcore/extensions/storage/oss/
+-rw-r--r--   0 zhouwei    (501) staff       (20)    11320 2023-07-12 07:32:29.000000 yz-core2-1.0.60/yzcore/extensions/storage/oss/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      762 2023-04-21 02:05:49.000000 yz-core2-1.0.60/yzcore/extensions/storage/oss/const.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      699 2023-07-12 07:23:44.000000 yz-core2-1.0.60/yzcore/extensions/storage/oss/utils.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1551 2023-07-12 07:23:44.000000 yz-core2-1.0.60/yzcore/extensions/storage/schemas.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      878 2023-07-12 07:23:44.000000 yz-core2-1.0.60/yzcore/extensions/storage/utils.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2724 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/extensions/uid.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-12 08:02:03.001850 yz-core2-1.0.60/yzcore/logger/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     6943 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/logger/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)    10770 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/logger/config.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1177 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/logger/filters.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)    10780 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/logger/handlers.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-12 08:02:03.002156 yz-core2-1.0.60/yzcore/request/
+-rw-r--r--   0 zhouwei    (501) staff       (20)      133 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/request/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     8293 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/request/aio_http.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-12 08:02:03.002693 yz-core2-1.0.60/yzcore/response/
+-rw-r--r--   0 zhouwei    (501) staff       (20)      188 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/response/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2934 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/response/response.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)    36606 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/response/response_code.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-12 08:02:03.002902 yz-core2-1.0.60/yzcore/templates/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/templates/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-12 08:02:03.003800 yz-core2-1.0.60/yzcore/templates/app_template/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/templates/app_template/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      945 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/templates/app_template/controllers.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      421 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/templates/app_template/models.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      907 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/templates/app_template/schemas.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/templates/app_template/tests.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1632 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/templates/app_template/views.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-12 08:02:03.004414 yz-core2-1.0.60/yzcore/templates/project_template/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1816 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/templates/project_template/.gitignore
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2508 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/templates/project_template/README.md
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-12 08:02:03.004706 yz-core2-1.0.60/yzcore/templates/project_template/docs/
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/templates/project_template/docs/install_explain.md
+-rw-r--r--   0 zhouwei    (501) staff       (20)      922 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/templates/project_template/docs/supervisor.ini
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-12 08:02:03.004851 yz-core2-1.0.60/yzcore/templates/project_template/migrations/
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/templates/project_template/migrations/README.md
+-rw-r--r--   0 zhouwei    (501) staff       (20)      453 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/templates/project_template/requirements.txt
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-12 08:02:03.005500 yz-core2-1.0.60/yzcore/templates/project_template/src/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/templates/project_template/src/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-12 08:02:03.005673 yz-core2-1.0.60/yzcore/templates/project_template/src/apps/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       90 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/templates/project_template/src/apps/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-12 08:02:03.006263 yz-core2-1.0.60/yzcore/templates/project_template/src/conf/
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/templates/project_template/src/conf/config_dev.ini
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/templates/project_template/src/conf/config_dev.yaml
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/templates/project_template/src/conf/config_production.ini
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/templates/project_template/src/conf/config_production.yaml
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/templates/project_template/src/conf/config_testing.ini
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/templates/project_template/src/conf/config_testing.yaml
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-12 08:02:03.006607 yz-core2-1.0.60/yzcore/templates/project_template/src/const/
+-rw-r--r--   0 zhouwei    (501) staff       (20)      157 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/templates/project_template/src/const/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      409 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/templates/project_template/src/const/_job.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      418 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/templates/project_template/src/const/_task.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      843 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/templates/project_template/src/main.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      807 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/templates/project_template/src/settings.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-12 08:02:03.006856 yz-core2-1.0.60/yzcore/templates/project_template/src/tests/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/templates/project_template/src/tests/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      840 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/templates/project_template/src/tests/test_xxx.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-12 08:02:03.006984 yz-core2-1.0.60/yzcore/templates/project_template/src/utils/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/templates/project_template/src/utils/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-12 08:02:03.008533 yz-core2-1.0.60/yzcore/utils/
+-rw-r--r--   0 zhouwei    (501) staff       (20)      386 2023-06-21 07:25:34.000000 yz-core2-1.0.60/yzcore/utils/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      231 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/utils/check_path.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1293 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/utils/check_sys.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2229 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/utils/crypto.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2064 2023-07-12 07:23:44.000000 yz-core2-1.0.60/yzcore/utils/decorator.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     9061 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/utils/encoding.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1755 2023-04-21 02:16:16.000000 yz-core2-1.0.60/yzcore/utils/nacos.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2129 2023-05-09 10:16:49.000000 yz-core2-1.0.60/yzcore/utils/time_utils.py
```

### Comparing `yz-core2-1.0.56b2/LICENSE` & `yz-core2-1.0.60/LICENSE`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/PKG-INFO` & `yz-core2-1.0.60/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yz-core2
-Version: 1.0.56b2
+Version: 1.0.60
 Summary: An ID generator for distributed microservices
 Home-page: https://github.com/zhouwe1/yz-core.git
 Author: zhouwe1
 Author-email: zhouwei@live.it
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yz-core2-1.0.56b2/README.md` & `yz-core2-1.0.60/README.md`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/setup.py` & `yz-core2-1.0.60/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="yz-core2",  # Replace with your own username
-    version="1.0.56b2",
+    version="1.0.60",
     author="zhouwe1",
     author_email="zhouwei@live.it",
     description="An ID generator for distributed microservices",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/zhouwe1/yz-core.git",
     packages=setuptools.find_packages(),
```

### Comparing `yz-core2-1.0.56b2/tests/test_setting_reload.py` & `yz-core2-1.0.60/tests/test_setting_reload.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/tests/test_uid.py` & `yz-core2-1.0.60/tests/test_uid.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/yz_core2.egg-info/PKG-INFO` & `yz-core2-1.0.60/yz_core2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yz-core2
-Version: 1.0.56b2
+Version: 1.0.60
 Summary: An ID generator for distributed microservices
 Home-page: https://github.com/zhouwe1/yz-core.git
 Author: zhouwe1
 Author-email: zhouwei@live.it
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yz-core2-1.0.56b2/yz_core2.egg-info/SOURCES.txt` & `yz-core2-1.0.60/yz_core2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/yzcore/core/datastructures.py` & `yz-core2-1.0.60/yzcore/core/datastructures.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/yzcore/core/encoders.py` & `yz-core2-1.0.60/yzcore/core/encoders.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/yzcore/core/management/__init__.py` & `yz-core2-1.0.60/yzcore/core/management/__init__.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/yzcore/core/management/commands/startapp.py` & `yz-core2-1.0.60/yzcore/core/management/commands/startapp.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/yzcore/core/management/commands/startproject.py` & `yz-core2-1.0.60/yzcore/core/management/commands/startproject.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/yzcore/core/management/templates.py` & `yz-core2-1.0.60/yzcore/core/management/templates.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/yzcore/core/storage.py` & `yz-core2-1.0.60/yzcore/core/storage.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/yzcore/db/db_session.py` & `yz-core2-1.0.60/yzcore/db/db_session.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/yzcore/db/pymongo_crud_base.py` & `yz-core2-1.0.60/yzcore/db/pymongo_crud_base.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/yzcore/db/sqlalchemy_crud_base.py` & `yz-core2-1.0.60/yzcore/db/sqlalchemy_crud_base.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/yzcore/decorators.py` & `yz-core2-1.0.60/yzcore/decorators.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/yzcore/default_settings.py` & `yz-core2-1.0.60/yzcore/default_settings.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/yzcore/exceptions.py` & `yz-core2-1.0.60/yzcore/exceptions.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/yzcore/extensions/storage/__init__.py` & `yz-core2-1.0.60/yzcore/extensions/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/yzcore/extensions/storage/amazon/__init__.py` & `yz-core2-1.0.60/yzcore/extensions/storage/amazon/__init__.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/yzcore/extensions/storage/amazon/utils.py` & `yz-core2-1.0.60/yzcore/extensions/storage/amazon/utils.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/yzcore/extensions/storage/azure/__init__.py` & `yz-core2-1.0.60/yzcore/extensions/storage/azure/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -193,15 +193,15 @@
         blob_client.delete_blob(delete_snapshots='include')
         return True
 
     def get_policy(
             self,
             filepath: str,
             callback_url: str,
-            callback_data: dict = None,
+            callback_data: dict,
             **kwargs
     ):
         """
         授权给第三方上传
         :param filepath: 需要在前一步拼接好完整的key
         :param callback_url: 对象存储的回调地址
         :param callback_data: 需要回传的参数
```

### Comparing `yz-core2-1.0.56b2/yzcore/extensions/storage/base.py` & `yz-core2-1.0.60/yzcore/extensions/storage/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -253,14 +253,15 @@
             # assert self._cors_check(), f'{self.bucket_name}: CORS设置错误'
 
             # 生成一个带有随机字符串的内存文件
             temp_file = create_temp_file(text_length=32)
             text = temp_file.getvalue().decode()
 
             key = f'storage_check_{text}.txt'
+            logger.debug(f'file_exists: {self.file_exists(key)}')
             # 上传
             file_url = self.upload_obj(temp_file, key=key)
             logger.debug(f'upload: {file_url}')
             assert file_url, f'{self.bucket_name}: Upload Failed'
             # 加签url
             assert self._check_sign_url(key), f'{self.bucket_name}: Sign Url Error'
             # 下载
@@ -277,14 +278,24 @@
             logger.debug(f'update_file_headers: {self.get_object_meta(key)}')
 
             # 遍历文件
             objects = self.iter_objects(key)
             logger.debug(f'iter_objects: {objects}')
             assert objects, f'{self.bucket_name} iter objects Failed'
 
+            # 删除文件
+            self.delete_object(key)
+            logger.debug(f'file_exists: {self.file_exists(key)}')
+            assert not self.file_exists(key), f'{self.bucket_name} delete object Failed'
+
+            # 生成post policy
+            policy = self.get_policy(filepath='upload_policy/', callback_url='https://hub.realibox.com/api/hub/v1/test', callback_data={'a':'b'})
+            logger.debug(f'get_policy: {policy}')
+            assert isinstance(policy, dict), f'{self.bucket_name}: Get policy Failed'
+
             return True
         except AssertionError as e:
             raise StorageRequestError(e)
 
     def _cors_check(self):
         """检查存储桶的CORS配置是否设置正确"""
         allowed_methods = {'GET', 'PUT', 'POST', 'DELETE', 'HEAD'}
```

### Comparing `yz-core2-1.0.56b2/yzcore/extensions/storage/const.py` & `yz-core2-1.0.60/yzcore/extensions/storage/const.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/yzcore/extensions/storage/minio/__init__.py` & `yz-core2-1.0.60/yzcore/extensions/storage/minio/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 
 
 class MinioManager(StorageManagerBase):
 
     def __init__(self, conf: MinioConfig):
         super(MinioManager, self).__init__(conf)
         self.internal_endpoint = conf.internal_endpoint
-        # 禁用internal_endpoint, 默认为False，只有minio部署在k8s集群而windows转换机无法访问到时才需要禁用
         self.disable_internal_endpoint = conf.disable_internal_endpoint
         self.internal_minioClient = None
 
         self.__init()
 
     def __init(self, bucket_name=None):
         """初始化对象"""
```

### Comparing `yz-core2-1.0.56b2/yzcore/extensions/storage/minio/utils.py` & `yz-core2-1.0.60/yzcore/extensions/storage/minio/utils.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/yzcore/extensions/storage/obs/__init__.py` & `yz-core2-1.0.60/yzcore/extensions/storage/obs/__init__.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/yzcore/extensions/storage/obs/const.py` & `yz-core2-1.0.60/yzcore/extensions/storage/obs/const.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/yzcore/extensions/storage/obs/obs_inherit.py` & `yz-core2-1.0.60/yzcore/extensions/storage/obs/obs_inherit.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/yzcore/extensions/storage/obs/utils.py` & `yz-core2-1.0.60/yzcore/extensions/storage/obs/utils.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/yzcore/extensions/storage/oss/__init__.py` & `yz-core2-1.0.60/yzcore/extensions/storage/oss/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -220,15 +220,14 @@
 
     def get_policy(
             self,
             filepath: str,
             callback_url: str,
             callback_data: dict,
             callback_content_type: str = "application/x-www-form-urlencoded",
-            **kwargs
     ):
         """
         授权给第三方上传
 
         :param filepath:
         :param callback_url:
         :param callback_data: 需要回传的参数
```

### Comparing `yz-core2-1.0.56b2/yzcore/extensions/storage/oss/const.py` & `yz-core2-1.0.60/yzcore/extensions/storage/oss/const.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/yzcore/extensions/storage/oss/utils.py` & `yz-core2-1.0.60/yzcore/extensions/storage/oss/utils.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/yzcore/extensions/storage/schemas.py` & `yz-core2-1.0.60/yzcore/extensions/storage/schemas.py`

 * *Files 20% similar despite different names*

```diff
@@ -32,16 +32,16 @@
 
 
 class ObsConfig(BaseConfig):
     callback_directly: bool = True  # True obs直接发起回调 / False 前端发起回调
 
 
 class MinioConfig(BaseConfig):
-    internal_endpoint: str = None
-    disable_internal_endpoint: bool = False
+    internal_endpoint: str = None  # minio的内网地址
+    disable_internal_endpoint: bool = False  # 禁用internal_endpoint, 默认为False，目前只有minio部署在k8s集群而windows转换机无法访问到时才需要禁用
 
 
 class AzureConfig(BaseConfig):
     connection_string: str
     account_key: str
     account_name: str
     access_key_id: Optional[str] = None
```

### Comparing `yz-core2-1.0.56b2/yzcore/extensions/storage/utils.py` & `yz-core2-1.0.60/yzcore/extensions/storage/utils.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/yzcore/extensions/uid.py` & `yz-core2-1.0.60/yzcore/extensions/uid.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/yzcore/logger/__init__.py` & `yz-core2-1.0.60/yzcore/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/yzcore/logger/config.py` & `yz-core2-1.0.60/yzcore/logger/config.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/yzcore/logger/filters.py` & `yz-core2-1.0.60/yzcore/logger/filters.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/yzcore/logger/handlers.py` & `yz-core2-1.0.60/yzcore/logger/handlers.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/yzcore/request/aio_http.py` & `yz-core2-1.0.60/yzcore/request/aio_http.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/yzcore/response/response.py` & `yz-core2-1.0.60/yzcore/response/response.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/yzcore/response/response_code.py` & `yz-core2-1.0.60/yzcore/response/response_code.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/yzcore/templates/app_template/controllers.py` & `yz-core2-1.0.60/yzcore/templates/app_template/controllers.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/yzcore/templates/app_template/schemas.py` & `yz-core2-1.0.60/yzcore/templates/app_template/schemas.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/yzcore/templates/app_template/views.py` & `yz-core2-1.0.60/yzcore/templates/app_template/views.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/yzcore/templates/project_template/.gitignore` & `yz-core2-1.0.60/yzcore/templates/project_template/.gitignore`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/yzcore/templates/project_template/README.md` & `yz-core2-1.0.60/yzcore/templates/project_template/README.md`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/yzcore/templates/project_template/docs/supervisor.ini` & `yz-core2-1.0.60/yzcore/templates/project_template/docs/supervisor.ini`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/yzcore/templates/project_template/src/main.py` & `yz-core2-1.0.60/yzcore/templates/project_template/src/main.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/yzcore/templates/project_template/src/settings.py` & `yz-core2-1.0.60/yzcore/templates/project_template/src/settings.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/yzcore/templates/project_template/src/tests/test_xxx.py` & `yz-core2-1.0.60/yzcore/templates/project_template/src/tests/test_xxx.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/yzcore/utils/check_sys.py` & `yz-core2-1.0.60/yzcore/utils/check_sys.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/yzcore/utils/crypto.py` & `yz-core2-1.0.60/yzcore/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/yzcore/utils/decorator.py` & `yz-core2-1.0.60/yzcore/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/yzcore/utils/encoding.py` & `yz-core2-1.0.60/yzcore/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/yzcore/utils/nacos.py` & `yz-core2-1.0.60/yzcore/utils/nacos.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.56b2/yzcore/utils/time_utils.py` & `yz-core2-1.0.60/yzcore/utils/time_utils.py`

 * *Files identical despite different names*

