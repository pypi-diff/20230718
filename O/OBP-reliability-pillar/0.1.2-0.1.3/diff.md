# Comparing `tmp/OBP_reliability_pillar-0.1.2.tar.gz` & `tmp/OBP_reliability_pillar-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OBP_reliability_pillar-0.1.2.tar", last modified: Mon Jul 17 19:04:42 2023, max compression
+gzip compressed data, was "OBP_reliability_pillar-0.1.3.tar", last modified: Tue Jul 18 05:32:31 2023, max compression
```

## Comparing `OBP_reliability_pillar-0.1.2.tar` & `OBP_reliability_pillar-0.1.3.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 19:04:42.550038 OBP_reliability_pillar-0.1.2/
--rw-rw-rw-   0        0        0        0 2022-11-24 06:08:48.000000 OBP_reliability_pillar-0.1.2/LICENCE
-drwxrwxrwx   0        0        0        0 2023-07-17 19:04:41.059296 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/
--rw-rw-rw-   0        0        0     4908 2023-07-17 19:04:06.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 19:04:41.177554 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/auto_scaling/
--rw-rw-rw-   0        0        0      197 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/auto_scaling/__init__.py
--rw-rw-rw-   0        0        0     2101 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/auto_scaling/asg_elb_healthcheck_required.py
--rw-rw-rw-   0        0        0      607 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/auto_scaling/compliance.py
--rw-rw-rw-   0        0        0     2223 2023-05-31 08:41:04.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/auto_scaling/launch_config_public_ip_disabled.py
-drwxrwxrwx   0        0        0        0 2023-07-17 19:04:41.285200 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/cloudwatch/
--rw-rw-rw-   0        0        0      193 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/cloudwatch/__init__.py
--rw-rw-rw-   0        0        0     3134 2023-05-31 08:41:04.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/cloudwatch/alarm_action_check.py
--rw-rw-rw-   0        0        0      485 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/cloudwatch/compliance.py
-drwxrwxrwx   0        0        0        0 2023-07-17 19:04:41.369037 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/dynamodb/
--rw-rw-rw-   0        0        0      187 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/dynamodb/__init__.py
--rw-rw-rw-   0        0        0      667 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/dynamodb/compliance.py
--rw-rw-rw-   0        0        0     2565 2023-07-17 18:59:49.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/dynamodb/dynamodb_autoscaling_enabled.py
--rw-rw-rw-   0        0        0     2106 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/dynamodb/dynamodb_pitr_enabled.py
--rw-rw-rw-   0        0        0      557 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/dynamodb/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-17 19:04:41.480043 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/ec2/
--rw-rw-rw-   0        0        0      177 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/ec2/__init__.py
--rw-rw-rw-   0        0        0      709 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/ec2/compliance.py
--rw-rw-rw-   0        0        0     2233 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/ec2/ec2_instance_detailed_monitoring_enabled.py
--rw-rw-rw-   0        0        0     2257 2023-05-31 08:17:16.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/ec2/instance_in_vpc.py
-drwxrwxrwx   0        0        0        0 2023-07-17 19:04:41.565664 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/elastic_beanstalk/
--rw-rw-rw-   0        0        0      205 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/elastic_beanstalk/__init__.py
--rw-rw-rw-   0        0        0      508 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/elastic_beanstalk/compliance.py
--rw-rw-rw-   0        0        0     2339 2023-05-31 08:23:26.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/elastic_beanstalk/enhanced_health_reporting_enabled.py
-drwxrwxrwx   0        0        0        0 2023-07-17 19:04:41.702452 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/elastic_load_balancer/
--rw-rw-rw-   0        0        0      177 2023-01-27 09:44:59.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/elastic_load_balancer/__init__.py
--rw-rw-rw-   0        0        0      737 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/elastic_load_balancer/compliance.py
--rw-rw-rw-   0        0        0     1829 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/elastic_load_balancer/cross_zone_load_balancing_enabled.py
--rw-rw-rw-   0        0        0     1994 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/elastic_load_balancer/elb_deletion_protection.py
--rw-rw-rw-   0        0        0     1700 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/elastic_load_balancer/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-17 19:04:41.790888 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/elastic_search/
--rw-rw-rw-   0        0        0      197 2023-01-27 11:52:50.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/elastic_search/__init__.py
--rw-rw-rw-   0        0        0      432 2023-05-31 11:40:25.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/elastic_search/compliance.py
--rw-rw-rw-   0        0        0     1940 2023-05-31 08:41:04.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/elastic_search/elastic_search_in_vpc_only.py
-drwxrwxrwx   0        0        0        0 2023-07-17 19:04:41.880795 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/guard_duty/
--rw-rw-rw-   0        0        0      207 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/guard_duty/__init__.py
--rw-rw-rw-   0        0        0      430 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/guard_duty/compliance.py
--rw-rw-rw-   0        0        0     1965 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/guard_duty/guard_duty_enabled.py
-drwxrwxrwx   0        0        0        0 2023-07-17 19:04:42.052487 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/lambdafn/
--rw-rw-rw-   0        0        0      181 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/lambdafn/__init__.py
--rw-rw-rw-   0        0        0      648 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/lambdafn/compliance.py
--rw-rw-rw-   0        0        0     1932 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/lambdafn/lambda_dlq_check.py
--rw-rw-rw-   0        0        0     1737 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/lambdafn/lambda_inside_vpc.py
--rw-rw-rw-   0        0        0      844 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/lambdafn/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-17 19:04:42.239343 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/rds/
--rw-rw-rw-   0        0        0      360 2023-06-06 07:06:27.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/rds/__init__.py
--rw-rw-rw-   0        0        0     2126 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/rds/compliance.py
--rw-rw-rw-   0        0        0     1558 2023-05-31 07:38:13.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/rds/rds_automatic_minor_version_upgrade_enabled.py
--rw-rw-rw-   0        0        0     2319 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/rds/rds_backup_enabled.py
--rw-rw-rw-   0        0        0     2126 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/rds/rds_enhanced_monitoring_enabled.py
--rw-rw-rw-   0        0        0     1479 2023-05-31 07:38:13.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/rds/rds_instance_deletion_protection_enabled.py
--rw-rw-rw-   0        0        0     1375 2023-05-31 07:38:13.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/rds/rds_multi_az_support_enabled.py
-drwxrwxrwx   0        0        0        0 2023-07-17 19:04:42.355567 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/redshift/
--rw-rw-rw-   0        0        0      213 2023-05-31 08:47:40.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/redshift/__init__.py
--rw-rw-rw-   0        0        0     1738 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/redshift/compliance.py
--rw-rw-rw-   0        0        0     1383 2023-05-31 08:41:04.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/redshift/redshift_backup_enabled.py
--rw-rw-rw-   0        0        0     1710 2023-05-31 08:41:05.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/redshift/redshift_cluster_maintenancesettings_check.py
-drwxrwxrwx   0        0        0        0 2023-07-17 19:04:42.506858 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/s3/
--rw-rw-rw-   0        0        0      297 2023-06-06 07:10:52.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/s3/__init__.py
--rw-rw-rw-   0        0        0     1112 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/s3/compliance.py
--rw-rw-rw-   0        0        0     1825 2023-05-31 08:23:26.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/s3/s3_bucket_default_lock_enabled.py
--rw-rw-rw-   0        0        0     1796 2023-05-31 09:39:39.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/s3/s3_bucket_replication_enabled.py
--rw-rw-rw-   0        0        0     1716 2023-05-31 08:23:25.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/s3/s3_bucket_versioning_enabled.py
-drwxrwxrwx   0        0        0        0 2023-07-17 19:04:42.539690 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/security_hub/
--rw-rw-rw-   0        0        0     1586 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/security_hub/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 19:04:41.077247 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar.egg-info/
--rw-rw-rw-   0        0        0     1114 2023-07-17 19:04:40.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3079 2023-07-17 19:04:41.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 19:04:40.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-07-17 19:04:40.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1114 2023-07-17 19:04:42.545674 OBP_reliability_pillar-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      755 2022-12-19 13:35:30.000000 OBP_reliability_pillar-0.1.2/README.md
--rw-rw-rw-   0        0        0      498 2023-07-17 19:04:06.000000 OBP_reliability_pillar-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-17 19:04:42.552073 OBP_reliability_pillar-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-18 05:32:31.128191 OBP_reliability_pillar-0.1.3/
+-rw-rw-rw-   0        0        0        0 2022-11-24 06:08:48.000000 OBP_reliability_pillar-0.1.3/LICENCE
+drwxrwxrwx   0        0        0        0 2023-07-18 05:32:30.314808 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/
+-rw-rw-rw-   0        0        0     4908 2023-07-18 05:32:06.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 05:32:30.370562 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/auto_scaling/
+-rw-rw-rw-   0        0        0      197 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/auto_scaling/__init__.py
+-rw-rw-rw-   0        0        0     2101 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/auto_scaling/asg_elb_healthcheck_required.py
+-rw-rw-rw-   0        0        0      607 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/auto_scaling/compliance.py
+-rw-rw-rw-   0        0        0     2223 2023-05-31 08:41:04.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/auto_scaling/launch_config_public_ip_disabled.py
+drwxrwxrwx   0        0        0        0 2023-07-18 05:32:30.398447 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/cloudwatch/
+-rw-rw-rw-   0        0        0      193 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/cloudwatch/__init__.py
+-rw-rw-rw-   0        0        0     3134 2023-05-31 08:41:04.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/cloudwatch/alarm_action_check.py
+-rw-rw-rw-   0        0        0      485 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/cloudwatch/compliance.py
+drwxrwxrwx   0        0        0        0 2023-07-18 05:32:30.453193 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/dynamodb/
+-rw-rw-rw-   0        0        0      187 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/dynamodb/__init__.py
+-rw-rw-rw-   0        0        0      667 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/dynamodb/compliance.py
+-rw-rw-rw-   0        0        0     2565 2023-07-17 18:59:49.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/dynamodb/dynamodb_autoscaling_enabled.py
+-rw-rw-rw-   0        0        0     2106 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/dynamodb/dynamodb_pitr_enabled.py
+-rw-rw-rw-   0        0        0      557 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/dynamodb/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-18 05:32:30.520892 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/ec2/
+-rw-rw-rw-   0        0        0      177 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/ec2/__init__.py
+-rw-rw-rw-   0        0        0      709 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/ec2/compliance.py
+-rw-rw-rw-   0        0        0     2233 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/ec2/ec2_instance_detailed_monitoring_enabled.py
+-rw-rw-rw-   0        0        0     2257 2023-05-31 08:17:16.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/ec2/instance_in_vpc.py
+drwxrwxrwx   0        0        0        0 2023-07-18 05:32:30.552749 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/elastic_beanstalk/
+-rw-rw-rw-   0        0        0      205 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/elastic_beanstalk/__init__.py
+-rw-rw-rw-   0        0        0      508 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/elastic_beanstalk/compliance.py
+-rw-rw-rw-   0        0        0     2339 2023-05-31 08:23:26.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/elastic_beanstalk/enhanced_health_reporting_enabled.py
+drwxrwxrwx   0        0        0        0 2023-07-18 05:32:30.619477 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/elastic_load_balancer/
+-rw-rw-rw-   0        0        0      177 2023-01-27 09:44:59.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/elastic_load_balancer/__init__.py
+-rw-rw-rw-   0        0        0      737 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/elastic_load_balancer/compliance.py
+-rw-rw-rw-   0        0        0     1829 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/elastic_load_balancer/cross_zone_load_balancing_enabled.py
+-rw-rw-rw-   0        0        0     1994 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/elastic_load_balancer/elb_deletion_protection.py
+-rw-rw-rw-   0        0        0     1700 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/elastic_load_balancer/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-18 05:32:30.649321 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/elastic_search/
+-rw-rw-rw-   0        0        0      197 2023-01-27 11:52:50.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/elastic_search/__init__.py
+-rw-rw-rw-   0        0        0      432 2023-05-31 11:40:25.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/elastic_search/compliance.py
+-rw-rw-rw-   0        0        0     1940 2023-05-31 08:41:04.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/elastic_search/elastic_search_in_vpc_only.py
+drwxrwxrwx   0        0        0        0 2023-07-18 05:32:30.696113 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/guard_duty/
+-rw-rw-rw-   0        0        0      207 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/guard_duty/__init__.py
+-rw-rw-rw-   0        0        0      430 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/guard_duty/compliance.py
+-rw-rw-rw-   0        0        0     1965 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/guard_duty/guard_duty_enabled.py
+drwxrwxrwx   0        0        0        0 2023-07-18 05:32:30.785715 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/lambdafn/
+-rw-rw-rw-   0        0        0      181 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/lambdafn/__init__.py
+-rw-rw-rw-   0        0        0      648 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/lambdafn/compliance.py
+-rw-rw-rw-   0        0        0     1932 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/lambdafn/lambda_dlq_check.py
+-rw-rw-rw-   0        0        0     1737 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/lambdafn/lambda_inside_vpc.py
+-rw-rw-rw-   0        0        0      844 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/lambdafn/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-18 05:32:30.917129 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/rds/
+-rw-rw-rw-   0        0        0      360 2023-06-06 07:06:27.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/rds/__init__.py
+-rw-rw-rw-   0        0        0     2126 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/rds/compliance.py
+-rw-rw-rw-   0        0        0     1558 2023-05-31 07:38:13.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/rds/rds_automatic_minor_version_upgrade_enabled.py
+-rw-rw-rw-   0        0        0     2319 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/rds/rds_backup_enabled.py
+-rw-rw-rw-   0        0        0     2126 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/rds/rds_enhanced_monitoring_enabled.py
+-rw-rw-rw-   0        0        0     1479 2023-05-31 07:38:13.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/rds/rds_instance_deletion_protection_enabled.py
+-rw-rw-rw-   0        0        0     1375 2023-05-31 07:38:13.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/rds/rds_multi_az_support_enabled.py
+drwxrwxrwx   0        0        0        0 2023-07-18 05:32:31.037593 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/redshift/
+-rw-rw-rw-   0        0        0      213 2023-05-31 08:47:40.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/redshift/__init__.py
+-rw-rw-rw-   0        0        0     1738 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/redshift/compliance.py
+-rw-rw-rw-   0        0        0     1383 2023-05-31 08:41:04.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/redshift/redshift_backup_enabled.py
+-rw-rw-rw-   0        0        0     1710 2023-05-31 08:41:05.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/redshift/redshift_cluster_maintenancesettings_check.py
+drwxrwxrwx   0        0        0        0 2023-07-18 05:32:31.101309 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/s3/
+-rw-rw-rw-   0        0        0      297 2023-06-06 07:10:52.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/s3/__init__.py
+-rw-rw-rw-   0        0        0     1112 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/s3/compliance.py
+-rw-rw-rw-   0        0        0     1825 2023-05-31 08:23:26.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/s3/s3_bucket_default_lock_enabled.py
+-rw-rw-rw-   0        0        0     1796 2023-05-31 09:39:39.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/s3/s3_bucket_replication_enabled.py
+-rw-rw-rw-   0        0        0     1932 2023-07-18 05:30:32.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/s3/s3_bucket_versioning_enabled.py
+drwxrwxrwx   0        0        0        0 2023-07-18 05:32:31.117240 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/security_hub/
+-rw-rw-rw-   0        0        0     1586 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/security_hub/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 05:32:30.326756 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar.egg-info/
+-rw-rw-rw-   0        0        0     1114 2023-07-18 05:32:30.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3079 2023-07-18 05:32:30.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 05:32:30.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-07-18 05:32:30.000000 OBP_reliability_pillar-0.1.3/OBP_reliability_pillar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1114 2023-07-18 05:32:31.121224 OBP_reliability_pillar-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      755 2022-12-19 13:35:30.000000 OBP_reliability_pillar-0.1.3/README.md
+-rw-rw-rw-   0        0        0      498 2023-07-18 05:32:06.000000 OBP_reliability_pillar-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-18 05:32:31.129187 OBP_reliability_pillar-0.1.3/setup.cfg
```

### Comparing `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/__init__.py` & `OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from OBP_reliability_pillar.s3 import s3
 # from OBP_reliability_pillar.security_hub import security_hub
 from OBP_reliability_pillar.auto_scaling import auto_scaling
 from OBP_reliability_pillar.lambdafn import lambdafn
 from OBP_reliability_pillar.guard_duty import guard_duty
 from OBP_reliability_pillar.elastic_search import elastic_search
 
-__version__ = '0.1.2'
+__version__ = '0.1.3'
 __author__ = 'Dheeraj Banodha'
 
 import logging
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
```

### Comparing `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/auto_scaling/asg_elb_healthcheck_required.py` & `OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/auto_scaling/asg_elb_healthcheck_required.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/auto_scaling/compliance.py` & `OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/auto_scaling/compliance.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/auto_scaling/launch_config_public_ip_disabled.py` & `OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/auto_scaling/launch_config_public_ip_disabled.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/cloudwatch/alarm_action_check.py` & `OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/cloudwatch/alarm_action_check.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/dynamodb/compliance.py` & `OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/dynamodb/compliance.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/dynamodb/dynamodb_autoscaling_enabled.py` & `OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/dynamodb/dynamodb_autoscaling_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/dynamodb/dynamodb_pitr_enabled.py` & `OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/dynamodb/dynamodb_pitr_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/dynamodb/utils.py` & `OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/dynamodb/utils.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/ec2/compliance.py` & `OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/ec2/compliance.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/ec2/ec2_instance_detailed_monitoring_enabled.py` & `OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/ec2/ec2_instance_detailed_monitoring_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/ec2/instance_in_vpc.py` & `OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/ec2/instance_in_vpc.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/elastic_beanstalk/enhanced_health_reporting_enabled.py` & `OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/elastic_beanstalk/enhanced_health_reporting_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/elastic_load_balancer/compliance.py` & `OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/elastic_load_balancer/compliance.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/elastic_load_balancer/cross_zone_load_balancing_enabled.py` & `OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/elastic_load_balancer/cross_zone_load_balancing_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/elastic_load_balancer/elb_deletion_protection.py` & `OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/elastic_load_balancer/elb_deletion_protection.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/elastic_load_balancer/utils.py` & `OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/elastic_load_balancer/utils.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/elastic_search/elastic_search_in_vpc_only.py` & `OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/elastic_search/elastic_search_in_vpc_only.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/guard_duty/guard_duty_enabled.py` & `OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/guard_duty/guard_duty_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/lambdafn/compliance.py` & `OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/lambdafn/compliance.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/lambdafn/lambda_dlq_check.py` & `OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/lambdafn/lambda_dlq_check.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/lambdafn/lambda_inside_vpc.py` & `OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/lambdafn/lambda_inside_vpc.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/lambdafn/utils.py` & `OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/lambdafn/utils.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/rds/compliance.py` & `OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/rds/compliance.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/rds/rds_automatic_minor_version_upgrade_enabled.py` & `OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/rds/rds_automatic_minor_version_upgrade_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/rds/rds_backup_enabled.py` & `OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/rds/rds_backup_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/rds/rds_enhanced_monitoring_enabled.py` & `OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/rds/rds_enhanced_monitoring_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/rds/rds_instance_deletion_protection_enabled.py` & `OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/rds/rds_instance_deletion_protection_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/rds/rds_multi_az_support_enabled.py` & `OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/rds/rds_multi_az_support_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/redshift/compliance.py` & `OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/redshift/compliance.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/redshift/redshift_backup_enabled.py` & `OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/redshift/redshift_backup_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/redshift/redshift_cluster_maintenancesettings_check.py` & `OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/redshift/redshift_cluster_maintenancesettings_check.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/s3/compliance.py` & `OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/s3/compliance.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/s3/s3_bucket_default_lock_enabled.py` & `OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/s3/s3_bucket_default_lock_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/s3/s3_bucket_replication_enabled.py` & `OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/s3/s3_bucket_replication_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/s3/s3_bucket_versioning_enabled.py` & `OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/s3/s3_bucket_versioning_enabled.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import logging
 
+from botocore.exceptions import ClientError
+
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
 # checks the compliance.py for s3 bucket versioning enabled
 def s3_bucket_versioning_enabled(self, buckets):
     """
@@ -35,14 +37,18 @@
             )
             status = resp['Status']
         except KeyError:
             result = False
             failReason = "Either bucket versioning is not enabled or configuration not found"
             offenders.append(bucket_name)
             continue
+        except ClientError:
+            result = False
+            failReason = "Access denied for get_bucket_logging api"
+            offenders.append(bucket_name)
 
         if not status == 'Enabled':
             result = False
             failReason = "Either bucket versioning is not enabled or configuration not found"
             offenders.append(bucket_name)
 
     return {
```

### Comparing `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/security_hub/__init__.py` & `OBP_reliability_pillar-0.1.3/OBP_reliability_pillar/security_hub/__init__.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar.egg-info/PKG-INFO` & `OBP_reliability_pillar-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: OBP-reliability-pillar
-Version: 0.1.2
+Name: OBP_reliability_pillar
+Version: 0.1.3
 Summary: Provides AWS compliance details
 Author-email: "dheeraj.banodha" <dheerajmbanodha@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar.egg-info/SOURCES.txt` & `OBP_reliability_pillar-0.1.3/OBP_reliability_pillar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.2/PKG-INFO` & `OBP_reliability_pillar-0.1.3/OBP_reliability_pillar.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: OBP_reliability_pillar
-Version: 0.1.2
+Name: OBP-reliability-pillar
+Version: 0.1.3
 Summary: Provides AWS compliance details
 Author-email: "dheeraj.banodha" <dheerajmbanodha@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `OBP_reliability_pillar-0.1.2/README.md` & `OBP_reliability_pillar-0.1.3/README.md`

 * *Files identical despite different names*

