# Comparing `tmp/yz-core2-1.0.61b1.tar.gz` & `tmp/yz-core2-1.0.61b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yz-core2-1.0.61b1.tar", last modified: Tue Jul 18 06:34:22 2023, max compression
+gzip compressed data, was "yz-core2-1.0.61b2.tar", last modified: Tue Jul 18 07:03:45 2023, max compression
```

## Comparing `yz-core2-1.0.61b1.tar` & `yz-core2-1.0.61b2.tar`

### file list

```diff
@@ -1,136 +1,141 @@
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 06:34:22.674689 yz-core2-1.0.61b1/
--rw-r--r--   0 zhouwei    (501) staff       (20)     1085 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/LICENSE
--rw-r--r--   0 zhouwei    (501) staff       (20)     3114 2023-07-18 06:34:22.674532 yz-core2-1.0.61b1/PKG-INFO
--rw-r--r--   0 zhouwei    (501) staff       (20)     2509 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/README.md
--rw-r--r--   0 zhouwei    (501) staff       (20)       38 2023-07-18 06:34:22.674733 yz-core2-1.0.61b1/setup.cfg
--rw-r--r--   0 zhouwei    (501) staff       (20)     1785 2023-07-18 06:33:52.000000 yz-core2-1.0.61b1/setup.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 06:34:22.656301 yz-core2-1.0.61b1/tests/
--rw-r--r--   0 zhouwei    (501) staff       (20)       94 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/tests/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      965 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/tests/test_setting_reload.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1822 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/tests/test_uid.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 06:34:22.657465 yz-core2-1.0.61b1/yz_core2.egg-info/
--rw-r--r--   0 zhouwei    (501) staff       (20)     3114 2023-07-18 06:34:22.000000 yz-core2-1.0.61b1/yz_core2.egg-info/PKG-INFO
--rw-r--r--   0 zhouwei    (501) staff       (20)     3759 2023-07-18 06:34:22.000000 yz-core2-1.0.61b1/yz_core2.egg-info/SOURCES.txt
--rw-r--r--   0 zhouwei    (501) staff       (20)        1 2023-07-18 06:34:22.000000 yz-core2-1.0.61b1/yz_core2.egg-info/dependency_links.txt
--rw-r--r--   0 zhouwei    (501) staff       (20)       48 2023-07-18 06:34:22.000000 yz-core2-1.0.61b1/yz_core2.egg-info/entry_points.txt
--rw-r--r--   0 zhouwei    (501) staff       (20)      240 2023-07-18 06:34:22.000000 yz-core2-1.0.61b1/yz_core2.egg-info/requires.txt
--rw-r--r--   0 zhouwei    (501) staff       (20)       13 2023-07-18 06:34:22.000000 yz-core2-1.0.61b1/yz_core2.egg-info/top_level.txt
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 06:34:22.658647 yz-core2-1.0.61b1/yzcore/
--rw-r--r--   0 zhouwei    (501) staff       (20)       90 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      440 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/__main__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 06:34:22.659944 yz-core2-1.0.61b1/yzcore/core/
--rw-r--r--   0 zhouwei    (501) staff       (20)       95 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/core/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      301 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/core/const.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      466 2023-06-28 05:59:58.000000 yz-core2-1.0.61b1/yzcore/core/data_hash.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     4722 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/core/datastructures.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     5244 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/core/encoders.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 06:34:22.660517 yz-core2-1.0.61b1/yzcore/core/management/
--rw-r--r--   0 zhouwei    (501) staff       (20)      614 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/core/management/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      122 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/core/management/base.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 06:34:22.660927 yz-core2-1.0.61b1/yzcore/core/management/commands/
--rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/core/management/commands/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      594 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/core/management/commands/startapp.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      783 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/core/management/commands/startproject.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     5219 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/core/management/templates.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     6334 2023-07-12 07:23:44.000000 yz-core2-1.0.61b1/yzcore/core/storage.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 06:34:22.661937 yz-core2-1.0.61b1/yzcore/db/
--rw-r--r--   0 zhouwei    (501) staff       (20)      876 2023-07-18 06:23:44.000000 yz-core2-1.0.61b1/yzcore/db/CustomQuery.py
--rw-r--r--   0 zhouwei    (501) staff       (20)       92 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/db/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1203 2023-07-18 06:23:44.000000 yz-core2-1.0.61b1/yzcore/db/db_session.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     7679 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/db/pymongo_crud_base.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     7165 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/db/sqlalchemy_crud_base.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1651 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/decorators.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     2525 2023-05-16 05:58:39.000000 yz-core2-1.0.61b1/yzcore/default_settings.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     2695 2023-07-12 07:23:44.000000 yz-core2-1.0.61b1/yzcore/exceptions.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 06:34:22.662195 yz-core2-1.0.61b1/yzcore/extensions/
--rw-r--r--   0 zhouwei    (501) staff       (20)       93 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/extensions/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 06:34:22.663224 yz-core2-1.0.61b1/yzcore/extensions/storage/
--rw-r--r--   0 zhouwei    (501) staff       (20)     1830 2023-07-12 07:23:44.000000 yz-core2-1.0.61b1/yzcore/extensions/storage/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 06:34:22.663604 yz-core2-1.0.61b1/yzcore/extensions/storage/amazon/
--rw-r--r--   0 zhouwei    (501) staff       (20)     6691 2023-07-12 07:23:44.000000 yz-core2-1.0.61b1/yzcore/extensions/storage/amazon/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      838 2023-07-12 07:23:44.000000 yz-core2-1.0.61b1/yzcore/extensions/storage/amazon/utils.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 06:34:22.663973 yz-core2-1.0.61b1/yzcore/extensions/storage/azure/
--rw-r--r--   0 zhouwei    (501) staff       (20)     8281 2023-07-12 07:26:10.000000 yz-core2-1.0.61b1/yzcore/extensions/storage/azure/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      465 2023-07-12 07:23:44.000000 yz-core2-1.0.61b1/yzcore/extensions/storage/azure/utils.py
--rw-r--r--   0 zhouwei    (501) staff       (20)    12849 2023-07-18 06:29:36.000000 yz-core2-1.0.61b1/yzcore/extensions/storage/base.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      724 2023-07-12 07:23:44.000000 yz-core2-1.0.61b1/yzcore/extensions/storage/const.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 06:34:22.664362 yz-core2-1.0.61b1/yzcore/extensions/storage/minio/
--rw-r--r--   0 zhouwei    (501) staff       (20)     9578 2023-07-12 07:27:42.000000 yz-core2-1.0.61b1/yzcore/extensions/storage/minio/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      820 2023-07-12 07:23:44.000000 yz-core2-1.0.61b1/yzcore/extensions/storage/minio/utils.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 06:34:22.665442 yz-core2-1.0.61b1/yzcore/extensions/storage/obs/
--rw-r--r--   0 zhouwei    (501) staff       (20)     9388 2023-07-12 07:30:17.000000 yz-core2-1.0.61b1/yzcore/extensions/storage/obs/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1109 2023-04-21 02:05:49.000000 yz-core2-1.0.61b1/yzcore/extensions/storage/obs/const.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     3101 2023-05-06 02:48:14.000000 yz-core2-1.0.61b1/yzcore/extensions/storage/obs/obs_inherit.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      678 2023-07-12 07:23:44.000000 yz-core2-1.0.61b1/yzcore/extensions/storage/obs/utils.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 06:34:22.666133 yz-core2-1.0.61b1/yzcore/extensions/storage/oss/
--rw-r--r--   0 zhouwei    (501) staff       (20)    11320 2023-07-12 07:32:29.000000 yz-core2-1.0.61b1/yzcore/extensions/storage/oss/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      762 2023-04-21 02:05:49.000000 yz-core2-1.0.61b1/yzcore/extensions/storage/oss/const.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      699 2023-07-12 07:23:44.000000 yz-core2-1.0.61b1/yzcore/extensions/storage/oss/utils.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1551 2023-07-12 07:23:44.000000 yz-core2-1.0.61b1/yzcore/extensions/storage/schemas.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      878 2023-07-12 07:23:44.000000 yz-core2-1.0.61b1/yzcore/extensions/storage/utils.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     2724 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/extensions/uid.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 06:34:22.666807 yz-core2-1.0.61b1/yzcore/logger/
--rw-r--r--   0 zhouwei    (501) staff       (20)     6943 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/logger/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)    10770 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/logger/config.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1177 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/logger/filters.py
--rw-r--r--   0 zhouwei    (501) staff       (20)    10780 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/logger/handlers.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 06:34:22.667094 yz-core2-1.0.61b1/yzcore/request/
--rw-r--r--   0 zhouwei    (501) staff       (20)      133 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/request/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     8293 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/request/aio_http.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 06:34:22.667570 yz-core2-1.0.61b1/yzcore/response/
--rw-r--r--   0 zhouwei    (501) staff       (20)      188 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/response/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     2934 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/response/response.py
--rw-r--r--   0 zhouwei    (501) staff       (20)    36606 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/response/response_code.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 06:34:22.667806 yz-core2-1.0.61b1/yzcore/templates/
--rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/templates/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 06:34:22.668663 yz-core2-1.0.61b1/yzcore/templates/app_template/
--rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/templates/app_template/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      945 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/templates/app_template/controllers.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      421 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/templates/app_template/models.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      907 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/templates/app_template/schemas.py
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/templates/app_template/tests.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1632 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/templates/app_template/views.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 06:34:22.669076 yz-core2-1.0.61b1/yzcore/templates/project_template/
--rw-r--r--   0 zhouwei    (501) staff       (20)     1816 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/templates/project_template/.gitignore
--rw-r--r--   0 zhouwei    (501) staff       (20)     2508 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/templates/project_template/README.md
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 06:34:22.669466 yz-core2-1.0.61b1/yzcore/templates/project_template/docs/
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/templates/project_template/docs/install_explain.md
--rw-r--r--   0 zhouwei    (501) staff       (20)      922 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/templates/project_template/docs/supervisor.ini
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 06:34:22.669625 yz-core2-1.0.61b1/yzcore/templates/project_template/migrations/
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/templates/project_template/migrations/README.md
--rw-r--r--   0 zhouwei    (501) staff       (20)      453 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/templates/project_template/requirements.txt
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 06:34:22.670019 yz-core2-1.0.61b1/yzcore/templates/project_template/src/
--rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/templates/project_template/src/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 06:34:22.670175 yz-core2-1.0.61b1/yzcore/templates/project_template/src/apps/
--rw-r--r--   0 zhouwei    (501) staff       (20)       90 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/templates/project_template/src/apps/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 06:34:22.670830 yz-core2-1.0.61b1/yzcore/templates/project_template/src/conf/
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/templates/project_template/src/conf/config_dev.ini
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/templates/project_template/src/conf/config_dev.yaml
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/templates/project_template/src/conf/config_production.ini
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/templates/project_template/src/conf/config_production.yaml
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/templates/project_template/src/conf/config_testing.ini
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/templates/project_template/src/conf/config_testing.yaml
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 06:34:22.671207 yz-core2-1.0.61b1/yzcore/templates/project_template/src/const/
--rw-r--r--   0 zhouwei    (501) staff       (20)      157 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/templates/project_template/src/const/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      409 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/templates/project_template/src/const/_job.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      418 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/templates/project_template/src/const/_task.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      843 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/templates/project_template/src/main.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      807 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/templates/project_template/src/settings.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 06:34:22.671500 yz-core2-1.0.61b1/yzcore/templates/project_template/src/tests/
--rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/templates/project_template/src/tests/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      840 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/templates/project_template/src/tests/test_xxx.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 06:34:22.671639 yz-core2-1.0.61b1/yzcore/templates/project_template/src/utils/
--rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/templates/project_template/src/utils/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 06:34:22.673575 yz-core2-1.0.61b1/yzcore/utils/
--rw-r--r--   0 zhouwei    (501) staff       (20)      386 2023-06-21 07:25:34.000000 yz-core2-1.0.61b1/yzcore/utils/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      231 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/utils/check_path.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1293 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/utils/check_sys.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     2229 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/utils/crypto.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     2064 2023-07-12 07:23:44.000000 yz-core2-1.0.61b1/yzcore/utils/decorator.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     9061 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/utils/encoding.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 06:34:22.674217 yz-core2-1.0.61b1/yzcore/utils/fastapi_context/
--rw-r--r--   0 zhouwei    (501) staff       (20)      337 2023-07-18 06:23:44.000000 yz-core2-1.0.61b1/yzcore/utils/fastapi_context/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1981 2022-08-12 10:46:46.000000 yz-core2-1.0.61b1/yzcore/utils/fastapi_context/context_middleware.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1439 2022-08-12 10:46:46.000000 yz-core2-1.0.61b1/yzcore/utils/fastapi_context/fastapi_context.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1755 2023-04-21 02:16:16.000000 yz-core2-1.0.61b1/yzcore/utils/nacos.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     2129 2023-05-09 10:16:49.000000 yz-core2-1.0.61b1/yzcore/utils/time_utils.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 07:03:45.431989 yz-core2-1.0.61b2/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1085 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/LICENSE
+-rw-r--r--   0 zhouwei    (501) staff       (20)     3114 2023-07-18 07:03:45.431841 yz-core2-1.0.61b2/PKG-INFO
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2509 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/README.md
+-rw-r--r--   0 zhouwei    (501) staff       (20)       38 2023-07-18 07:03:45.432034 yz-core2-1.0.61b2/setup.cfg
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1785 2023-07-18 07:01:27.000000 yz-core2-1.0.61b2/setup.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 07:03:45.412701 yz-core2-1.0.61b2/tests/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       94 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/tests/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      965 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/tests/test_setting_reload.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1822 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/tests/test_uid.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 07:03:45.413551 yz-core2-1.0.61b2/yz_core2.egg-info/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     3114 2023-07-18 07:03:45.000000 yz-core2-1.0.61b2/yz_core2.egg-info/PKG-INFO
+-rw-r--r--   0 zhouwei    (501) staff       (20)     3900 2023-07-18 07:03:45.000000 yz-core2-1.0.61b2/yz_core2.egg-info/SOURCES.txt
+-rw-r--r--   0 zhouwei    (501) staff       (20)        1 2023-07-18 07:03:45.000000 yz-core2-1.0.61b2/yz_core2.egg-info/dependency_links.txt
+-rw-r--r--   0 zhouwei    (501) staff       (20)       48 2023-07-18 07:03:45.000000 yz-core2-1.0.61b2/yz_core2.egg-info/entry_points.txt
+-rw-r--r--   0 zhouwei    (501) staff       (20)      240 2023-07-18 07:03:45.000000 yz-core2-1.0.61b2/yz_core2.egg-info/requires.txt
+-rw-r--r--   0 zhouwei    (501) staff       (20)       13 2023-07-18 07:03:45.000000 yz-core2-1.0.61b2/yz_core2.egg-info/top_level.txt
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 07:03:45.414660 yz-core2-1.0.61b2/yzcore/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       90 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      440 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/__main__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 07:03:45.416174 yz-core2-1.0.61b2/yzcore/core/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       95 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/core/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      301 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/core/const.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      466 2023-06-28 05:59:58.000000 yz-core2-1.0.61b2/yzcore/core/data_hash.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     4722 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/core/datastructures.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     5244 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/core/encoders.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 07:03:45.416930 yz-core2-1.0.61b2/yzcore/core/management/
+-rw-r--r--   0 zhouwei    (501) staff       (20)      614 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/core/management/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      122 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/core/management/base.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 07:03:45.417497 yz-core2-1.0.61b2/yzcore/core/management/commands/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/core/management/commands/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      594 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/core/management/commands/startapp.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      783 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/core/management/commands/startproject.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     5219 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/core/management/templates.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     6334 2023-07-12 07:23:44.000000 yz-core2-1.0.61b2/yzcore/core/storage.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 07:03:45.418551 yz-core2-1.0.61b2/yzcore/db/
+-rw-r--r--   0 zhouwei    (501) staff       (20)      876 2023-07-18 06:23:44.000000 yz-core2-1.0.61b2/yzcore/db/CustomQuery.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)       92 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/db/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1132 2023-07-18 07:02:47.000000 yz-core2-1.0.61b2/yzcore/db/db_session.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     7679 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/db/pymongo_crud_base.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     7165 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/db/sqlalchemy_crud_base.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1651 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/decorators.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2525 2023-05-16 05:58:39.000000 yz-core2-1.0.61b2/yzcore/default_settings.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2695 2023-07-12 07:23:44.000000 yz-core2-1.0.61b2/yzcore/exceptions.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 07:03:45.418907 yz-core2-1.0.61b2/yzcore/extensions/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       93 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/extensions/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 07:03:45.420132 yz-core2-1.0.61b2/yzcore/extensions/storage/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1830 2023-07-12 07:23:44.000000 yz-core2-1.0.61b2/yzcore/extensions/storage/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 07:03:45.420443 yz-core2-1.0.61b2/yzcore/extensions/storage/amazon/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     6691 2023-07-12 07:23:44.000000 yz-core2-1.0.61b2/yzcore/extensions/storage/amazon/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      838 2023-07-12 07:23:44.000000 yz-core2-1.0.61b2/yzcore/extensions/storage/amazon/utils.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 07:03:45.420904 yz-core2-1.0.61b2/yzcore/extensions/storage/azure/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     8281 2023-07-12 07:26:10.000000 yz-core2-1.0.61b2/yzcore/extensions/storage/azure/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      465 2023-07-12 07:23:44.000000 yz-core2-1.0.61b2/yzcore/extensions/storage/azure/utils.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)    12849 2023-07-18 06:29:36.000000 yz-core2-1.0.61b2/yzcore/extensions/storage/base.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      724 2023-07-12 07:23:44.000000 yz-core2-1.0.61b2/yzcore/extensions/storage/const.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 07:03:45.421310 yz-core2-1.0.61b2/yzcore/extensions/storage/minio/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     9578 2023-07-12 07:27:42.000000 yz-core2-1.0.61b2/yzcore/extensions/storage/minio/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      820 2023-07-12 07:23:44.000000 yz-core2-1.0.61b2/yzcore/extensions/storage/minio/utils.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 07:03:45.422472 yz-core2-1.0.61b2/yzcore/extensions/storage/obs/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     9388 2023-07-12 07:30:17.000000 yz-core2-1.0.61b2/yzcore/extensions/storage/obs/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1109 2023-04-21 02:05:49.000000 yz-core2-1.0.61b2/yzcore/extensions/storage/obs/const.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     3101 2023-05-06 02:48:14.000000 yz-core2-1.0.61b2/yzcore/extensions/storage/obs/obs_inherit.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      678 2023-07-12 07:23:44.000000 yz-core2-1.0.61b2/yzcore/extensions/storage/obs/utils.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 07:03:45.422996 yz-core2-1.0.61b2/yzcore/extensions/storage/oss/
+-rw-r--r--   0 zhouwei    (501) staff       (20)    11320 2023-07-12 07:32:29.000000 yz-core2-1.0.61b2/yzcore/extensions/storage/oss/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      762 2023-04-21 02:05:49.000000 yz-core2-1.0.61b2/yzcore/extensions/storage/oss/const.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      699 2023-07-12 07:23:44.000000 yz-core2-1.0.61b2/yzcore/extensions/storage/oss/utils.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1551 2023-07-12 07:23:44.000000 yz-core2-1.0.61b2/yzcore/extensions/storage/schemas.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      878 2023-07-12 07:23:44.000000 yz-core2-1.0.61b2/yzcore/extensions/storage/utils.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2724 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/extensions/uid.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 07:03:45.423652 yz-core2-1.0.61b2/yzcore/logger/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     6943 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/logger/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)    10770 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/logger/config.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1177 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/logger/filters.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)    10780 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/logger/handlers.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 07:03:45.423968 yz-core2-1.0.61b2/yzcore/request/
+-rw-r--r--   0 zhouwei    (501) staff       (20)      133 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/request/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     8293 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/request/aio_http.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 07:03:45.424466 yz-core2-1.0.61b2/yzcore/response/
+-rw-r--r--   0 zhouwei    (501) staff       (20)      188 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/response/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2934 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/response/response.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)    36606 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/response/response_code.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 07:03:45.424775 yz-core2-1.0.61b2/yzcore/templates/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/templates/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 07:03:45.425608 yz-core2-1.0.61b2/yzcore/templates/app_template/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/templates/app_template/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      945 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/templates/app_template/controllers.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      421 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/templates/app_template/models.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      907 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/templates/app_template/schemas.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/templates/app_template/tests.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1632 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/templates/app_template/views.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 07:03:45.426181 yz-core2-1.0.61b2/yzcore/templates/project_template/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1816 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/templates/project_template/.gitignore
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2508 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/templates/project_template/README.md
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 07:03:45.426444 yz-core2-1.0.61b2/yzcore/templates/project_template/docs/
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/templates/project_template/docs/install_explain.md
+-rw-r--r--   0 zhouwei    (501) staff       (20)      922 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/templates/project_template/docs/supervisor.ini
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 07:03:45.426661 yz-core2-1.0.61b2/yzcore/templates/project_template/migrations/
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/templates/project_template/migrations/README.md
+-rw-r--r--   0 zhouwei    (501) staff       (20)      453 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/templates/project_template/requirements.txt
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 07:03:45.427188 yz-core2-1.0.61b2/yzcore/templates/project_template/src/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/templates/project_template/src/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 07:03:45.427323 yz-core2-1.0.61b2/yzcore/templates/project_template/src/apps/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       90 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/templates/project_template/src/apps/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 07:03:45.427931 yz-core2-1.0.61b2/yzcore/templates/project_template/src/conf/
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/templates/project_template/src/conf/config_dev.ini
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/templates/project_template/src/conf/config_dev.yaml
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/templates/project_template/src/conf/config_production.ini
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/templates/project_template/src/conf/config_production.yaml
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/templates/project_template/src/conf/config_testing.ini
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/templates/project_template/src/conf/config_testing.yaml
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 07:03:45.428374 yz-core2-1.0.61b2/yzcore/templates/project_template/src/const/
+-rw-r--r--   0 zhouwei    (501) staff       (20)      157 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/templates/project_template/src/const/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      409 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/templates/project_template/src/const/_job.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      418 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/templates/project_template/src/const/_task.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      843 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/templates/project_template/src/main.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      807 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/templates/project_template/src/settings.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 07:03:45.428688 yz-core2-1.0.61b2/yzcore/templates/project_template/src/tests/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/templates/project_template/src/tests/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      840 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/templates/project_template/src/tests/test_xxx.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 07:03:45.428875 yz-core2-1.0.61b2/yzcore/templates/project_template/src/utils/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/templates/project_template/src/utils/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 07:03:45.430258 yz-core2-1.0.61b2/yzcore/utils/
+-rw-r--r--   0 zhouwei    (501) staff       (20)      386 2023-06-21 07:25:34.000000 yz-core2-1.0.61b2/yzcore/utils/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      231 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/utils/check_path.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1293 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/utils/check_sys.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2229 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/utils/crypto.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 07:03:45.431047 yz-core2-1.0.61b2/yzcore/utils/custom_log/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       49 2022-08-19 02:08:29.000000 yz-core2-1.0.61b2/yzcore/utils/custom_log/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      490 2023-07-18 06:50:17.000000 yz-core2-1.0.61b2/yzcore/utils/custom_log/filter.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      738 2023-07-18 07:03:26.000000 yz-core2-1.0.61b2/yzcore/utils/custom_log/formatter.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      736 2023-07-18 06:54:40.000000 yz-core2-1.0.61b2/yzcore/utils/custom_log/logger.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2064 2023-07-12 07:23:44.000000 yz-core2-1.0.61b2/yzcore/utils/decorator.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     9061 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/utils/encoding.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-07-18 07:03:45.431542 yz-core2-1.0.61b2/yzcore/utils/fastapi_context/
+-rw-r--r--   0 zhouwei    (501) staff       (20)      337 2023-07-18 06:23:44.000000 yz-core2-1.0.61b2/yzcore/utils/fastapi_context/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1981 2022-08-12 10:46:46.000000 yz-core2-1.0.61b2/yzcore/utils/fastapi_context/context_middleware.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1439 2022-08-12 10:46:46.000000 yz-core2-1.0.61b2/yzcore/utils/fastapi_context/fastapi_context.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1755 2023-04-21 02:16:16.000000 yz-core2-1.0.61b2/yzcore/utils/nacos.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2129 2023-05-09 10:16:49.000000 yz-core2-1.0.61b2/yzcore/utils/time_utils.py
```

### Comparing `yz-core2-1.0.61b1/LICENSE` & `yz-core2-1.0.61b2/LICENSE`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/PKG-INFO` & `yz-core2-1.0.61b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yz-core2
-Version: 1.0.61b1
+Version: 1.0.61b2
 Summary: An ID generator for distributed microservices
 Home-page: https://github.com/zhouwe1/yz-core.git
 Author: zhouwe1
 Author-email: zhouwei@live.it
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yz-core2-1.0.61b1/README.md` & `yz-core2-1.0.61b2/README.md`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/setup.py` & `yz-core2-1.0.61b2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="yz-core2",  # Replace with your own username
-    version="1.0.61b1",
+    version="1.0.61b2",
     author="zhouwe1",
     author_email="zhouwei@live.it",
     description="An ID generator for distributed microservices",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/zhouwe1/yz-core.git",
     packages=setuptools.find_packages(),
```

### Comparing `yz-core2-1.0.61b1/tests/test_setting_reload.py` & `yz-core2-1.0.61b2/tests/test_setting_reload.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/tests/test_uid.py` & `yz-core2-1.0.61b2/tests/test_uid.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yz_core2.egg-info/PKG-INFO` & `yz-core2-1.0.61b2/yz_core2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yz-core2
-Version: 1.0.61b1
+Version: 1.0.61b2
 Summary: An ID generator for distributed microservices
 Home-page: https://github.com/zhouwe1/yz-core.git
 Author: zhouwe1
 Author-email: zhouwei@live.it
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yz-core2-1.0.61b1/yz_core2.egg-info/SOURCES.txt` & `yz-core2-1.0.61b2/yz_core2.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -94,10 +94,14 @@
 yzcore/utils/check_path.py
 yzcore/utils/check_sys.py
 yzcore/utils/crypto.py
 yzcore/utils/decorator.py
 yzcore/utils/encoding.py
 yzcore/utils/nacos.py
 yzcore/utils/time_utils.py
+yzcore/utils/custom_log/__init__.py
+yzcore/utils/custom_log/filter.py
+yzcore/utils/custom_log/formatter.py
+yzcore/utils/custom_log/logger.py
 yzcore/utils/fastapi_context/__init__.py
 yzcore/utils/fastapi_context/context_middleware.py
 yzcore/utils/fastapi_context/fastapi_context.py
```

### Comparing `yz-core2-1.0.61b1/yzcore/core/datastructures.py` & `yz-core2-1.0.61b2/yzcore/core/datastructures.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/core/encoders.py` & `yz-core2-1.0.61b2/yzcore/core/encoders.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/core/management/__init__.py` & `yz-core2-1.0.61b2/yzcore/core/management/__init__.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/core/management/commands/startapp.py` & `yz-core2-1.0.61b2/yzcore/core/management/commands/startapp.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/core/management/commands/startproject.py` & `yz-core2-1.0.61b2/yzcore/core/management/commands/startproject.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/core/management/templates.py` & `yz-core2-1.0.61b2/yzcore/core/management/templates.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/core/storage.py` & `yz-core2-1.0.61b2/yzcore/core/storage.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/db/CustomQuery.py` & `yz-core2-1.0.61b2/yzcore/db/CustomQuery.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/db/db_session.py` & `yz-core2-1.0.61b2/yzcore/db/db_session.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,26 +14,22 @@
 from yzcore.db.CustomQuery import Query
 from yzcore.default_settings import default_setting as settings
 
 
 def get_db_engine(uri=settings.DB_URI):
     if uri is None:
         raise EnvironmentError('需要配置"DB_URI"变量！')
+    connect_args = {}
     _typ = urlparse(uri).scheme
     if _typ.startswith('sqlite'):
-        return create_engine(
-            settings.DB_URI,
-            connect_args={"check_same_thread": False}
-            # 只有SQLite才需要，其他数据库不需要。SQLite 只允许一个线程与其通信
-        )
+        # 只有SQLite才需要，其他数据库不需要。SQLite 只允许一个线程与其通信
+        connect_args['check_same_thread'] = False
     else:
-        return create_engine(
-            settings.DB_URI,
-            connect_args={"connect_timeout": 5}
-        )
+        connect_args['connect_timeout'] = 5
+    return create_engine(uri, connect_args=connect_args)
 
 
 engine = get_db_engine()
 SessionLocal = sessionmaker(autocommit=False, autoflush=False, bind=engine, query_cls=Query)
 
 Base = declarative_base()
```

### Comparing `yz-core2-1.0.61b1/yzcore/db/pymongo_crud_base.py` & `yz-core2-1.0.61b2/yzcore/db/pymongo_crud_base.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/db/sqlalchemy_crud_base.py` & `yz-core2-1.0.61b2/yzcore/db/sqlalchemy_crud_base.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/decorators.py` & `yz-core2-1.0.61b2/yzcore/decorators.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/default_settings.py` & `yz-core2-1.0.61b2/yzcore/default_settings.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/exceptions.py` & `yz-core2-1.0.61b2/yzcore/exceptions.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/extensions/storage/__init__.py` & `yz-core2-1.0.61b2/yzcore/extensions/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/extensions/storage/amazon/__init__.py` & `yz-core2-1.0.61b2/yzcore/extensions/storage/amazon/__init__.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/extensions/storage/amazon/utils.py` & `yz-core2-1.0.61b2/yzcore/extensions/storage/amazon/utils.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/extensions/storage/azure/__init__.py` & `yz-core2-1.0.61b2/yzcore/extensions/storage/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/extensions/storage/base.py` & `yz-core2-1.0.61b2/yzcore/extensions/storage/base.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/extensions/storage/const.py` & `yz-core2-1.0.61b2/yzcore/extensions/storage/const.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/extensions/storage/minio/__init__.py` & `yz-core2-1.0.61b2/yzcore/extensions/storage/minio/__init__.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/extensions/storage/minio/utils.py` & `yz-core2-1.0.61b2/yzcore/extensions/storage/minio/utils.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/extensions/storage/obs/__init__.py` & `yz-core2-1.0.61b2/yzcore/extensions/storage/obs/__init__.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/extensions/storage/obs/const.py` & `yz-core2-1.0.61b2/yzcore/extensions/storage/obs/const.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/extensions/storage/obs/obs_inherit.py` & `yz-core2-1.0.61b2/yzcore/extensions/storage/obs/obs_inherit.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/extensions/storage/obs/utils.py` & `yz-core2-1.0.61b2/yzcore/extensions/storage/obs/utils.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/extensions/storage/oss/__init__.py` & `yz-core2-1.0.61b2/yzcore/extensions/storage/oss/__init__.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/extensions/storage/oss/const.py` & `yz-core2-1.0.61b2/yzcore/extensions/storage/oss/const.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/extensions/storage/oss/utils.py` & `yz-core2-1.0.61b2/yzcore/extensions/storage/oss/utils.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/extensions/storage/schemas.py` & `yz-core2-1.0.61b2/yzcore/extensions/storage/schemas.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/extensions/storage/utils.py` & `yz-core2-1.0.61b2/yzcore/extensions/storage/utils.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/extensions/uid.py` & `yz-core2-1.0.61b2/yzcore/extensions/uid.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/logger/__init__.py` & `yz-core2-1.0.61b2/yzcore/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/logger/config.py` & `yz-core2-1.0.61b2/yzcore/logger/config.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/logger/filters.py` & `yz-core2-1.0.61b2/yzcore/logger/filters.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/logger/handlers.py` & `yz-core2-1.0.61b2/yzcore/logger/handlers.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/request/aio_http.py` & `yz-core2-1.0.61b2/yzcore/request/aio_http.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/response/response.py` & `yz-core2-1.0.61b2/yzcore/response/response.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/response/response_code.py` & `yz-core2-1.0.61b2/yzcore/response/response_code.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/templates/app_template/controllers.py` & `yz-core2-1.0.61b2/yzcore/templates/app_template/controllers.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/templates/app_template/schemas.py` & `yz-core2-1.0.61b2/yzcore/templates/app_template/schemas.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/templates/app_template/views.py` & `yz-core2-1.0.61b2/yzcore/templates/app_template/views.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/templates/project_template/.gitignore` & `yz-core2-1.0.61b2/yzcore/templates/project_template/.gitignore`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/templates/project_template/README.md` & `yz-core2-1.0.61b2/yzcore/templates/project_template/README.md`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/templates/project_template/docs/supervisor.ini` & `yz-core2-1.0.61b2/yzcore/templates/project_template/docs/supervisor.ini`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/templates/project_template/src/main.py` & `yz-core2-1.0.61b2/yzcore/templates/project_template/src/main.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/templates/project_template/src/settings.py` & `yz-core2-1.0.61b2/yzcore/templates/project_template/src/settings.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/templates/project_template/src/tests/test_xxx.py` & `yz-core2-1.0.61b2/yzcore/templates/project_template/src/tests/test_xxx.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/utils/check_sys.py` & `yz-core2-1.0.61b2/yzcore/utils/check_sys.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/utils/crypto.py` & `yz-core2-1.0.61b2/yzcore/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/utils/decorator.py` & `yz-core2-1.0.61b2/yzcore/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/utils/encoding.py` & `yz-core2-1.0.61b2/yzcore/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/utils/fastapi_context/context_middleware.py` & `yz-core2-1.0.61b2/yzcore/utils/fastapi_context/context_middleware.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/utils/fastapi_context/fastapi_context.py` & `yz-core2-1.0.61b2/yzcore/utils/fastapi_context/fastapi_context.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/utils/nacos.py` & `yz-core2-1.0.61b2/yzcore/utils/nacos.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.61b1/yzcore/utils/time_utils.py` & `yz-core2-1.0.61b2/yzcore/utils/time_utils.py`

 * *Files identical despite different names*

