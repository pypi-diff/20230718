# Comparing `tmp/OBP_security_pillar-0.1.1.tar.gz` & `tmp/OBP_security_pillar-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OBP_security_pillar-0.1.1.tar", last modified: Fri Jun  2 06:59:18 2023, max compression
+gzip compressed data, was "OBP_security_pillar-0.1.2.tar", last modified: Tue Jul 18 05:06:53 2023, max compression
```

## Comparing `OBP_security_pillar-0.1.1.tar` & `OBP_security_pillar-0.1.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 06:59:18.008991 OBP_security_pillar-0.1.1/
-drwxrwxrwx   0        0        0        0 2023-06-02 06:59:17.488467 OBP_security_pillar-0.1.1/OBP_security_pillar/
--rw-rw-rw-   0        0        0     3955 2023-06-02 06:52:59.000000 OBP_security_pillar-0.1.1/OBP_security_pillar/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 06:59:17.524480 OBP_security_pillar-0.1.1/OBP_security_pillar/auto_scaling/
--rw-rw-rw-   0        0        0      475 2023-05-25 10:12:07.000000 OBP_security_pillar-0.1.1/OBP_security_pillar/auto_scaling/__init__.py
--rw-rw-rw-   0        0        0     2189 2023-01-27 08:23:40.000000 OBP_security_pillar-0.1.1/OBP_security_pillar/auto_scaling/launch_config_public_ip_disabled.py
-drwxrwxrwx   0        0        0        0 2023-06-02 06:59:17.569989 OBP_security_pillar-0.1.1/OBP_security_pillar/cloudtrail/
--rw-rw-rw-   0        0        0      724 2023-05-25 10:12:07.000000 OBP_security_pillar-0.1.1/OBP_security_pillar/cloudtrail/__init__.py
--rw-rw-rw-   0        0        0     2509 2023-01-27 08:24:11.000000 OBP_security_pillar-0.1.1/OBP_security_pillar/cloudtrail/cloudtrail_cloudwatch_logs_enabled.py
--rw-rw-rw-   0        0        0     3124 2023-05-25 10:12:07.000000 OBP_security_pillar-0.1.1/OBP_security_pillar/cloudtrail/driver.py
--rw-rw-rw-   0        0        0     1251 2023-01-27 07:29:08.000000 OBP_security_pillar-0.1.1/OBP_security_pillar/compliance.py
-drwxrwxrwx   0        0        0        0 2023-06-02 06:59:17.607991 OBP_security_pillar-0.1.1/OBP_security_pillar/dynamodb/
--rw-rw-rw-   0        0        0      493 2023-05-25 10:12:07.000000 OBP_security_pillar-0.1.1/OBP_security_pillar/dynamodb/__init__.py
--rw-rw-rw-   0        0        0     2863 2023-01-27 08:24:38.000000 OBP_security_pillar-0.1.1/OBP_security_pillar/dynamodb/dynamodb_table_encrypted_kms.py
-drwxrwxrwx   0        0        0        0 2023-06-02 06:59:17.795000 OBP_security_pillar-0.1.1/OBP_security_pillar/ec2/
--rw-rw-rw-   0        0        0     2214 2023-05-25 10:01:21.000000 OBP_security_pillar-0.1.1/OBP_security_pillar/ec2/Incoming_ssh_disabled.py
--rw-rw-rw-   0        0        0     2852 2023-05-25 10:19:42.000000 OBP_security_pillar-0.1.1/OBP_security_pillar/ec2/__init__.py
--rw-rw-rw-   0        0        0     3275 2023-05-25 10:01:21.000000 OBP_security_pillar-0.1.1/OBP_security_pillar/ec2/ebs_snapshot_public_restorable_check.py
--rw-rw-rw-   0        0        0     1519 2023-05-25 10:01:21.000000 OBP_security_pillar-0.1.1/OBP_security_pillar/ec2/ec2_ebs_encryption_by_default.py
--rw-rw-rw-   0        0        0     2105 2023-01-27 07:29:08.000000 OBP_security_pillar-0.1.1/OBP_security_pillar/ec2/ec2_encrypted_volume.py
--rw-rw-rw-   0        0        0     1540 2023-05-25 10:01:21.000000 OBP_security_pillar-0.1.1/OBP_security_pillar/ec2/ec2_imdsv2_check.py
--rw-rw-rw-   0        0        0     3047 2023-05-25 10:01:21.000000 OBP_security_pillar-0.1.1/OBP_security_pillar/ec2/ec2_instance_managed_by_ssm.py
--rw-rw-rw-   0        0        0     1431 2023-05-25 10:01:21.000000 OBP_security_pillar-0.1.1/OBP_security_pillar/ec2/ec2_instance_multiple_eni_check.py
--rw-rw-rw-   0        0        0     1519 2023-05-25 10:01:21.000000 OBP_security_pillar-0.1.1/OBP_security_pillar/ec2/ec2_instance_profile_attached.py
--rw-rw-rw-   0        0        0     2088 2023-05-25 10:01:21.000000 OBP_security_pillar-0.1.1/OBP_security_pillar/ec2/ec2_volume_inuse_check.py
--rw-rw-rw-   0        0        0     2223 2023-01-27 08:28:22.000000 OBP_security_pillar-0.1.1/OBP_security_pillar/ec2/instance_in_vpc.py
--rw-rw-rw-   0        0        0     2348 2023-05-25 10:01:21.000000 OBP_security_pillar-0.1.1/OBP_security_pillar/ec2/vpc_flow_logs_enabled.py
--rw-rw-rw-   0        0        0     2793 2023-01-27 08:43:11.000000 OBP_security_pillar-0.1.1/OBP_security_pillar/elb_logging_enabled.py
--rw-rw-rw-   0        0        0     2268 2023-01-27 08:43:27.000000 OBP_security_pillar-0.1.1/OBP_security_pillar/elb_tls_https_listeners_only.py
--rw-rw-rw-   0        0        0     1969 2023-01-27 08:44:03.000000 OBP_security_pillar-0.1.1/OBP_security_pillar/guard_duty_enabled.py
--rw-rw-rw-   0        0        0     2387 2023-01-27 08:44:27.000000 OBP_security_pillar-0.1.1/OBP_security_pillar/lambda_inside_vpc.py
-drwxrwxrwx   0        0        0        0 2023-06-02 06:59:17.883989 OBP_security_pillar-0.1.1/OBP_security_pillar/rds/
--rw-rw-rw-   0        0        0     2835 2023-05-25 09:38:15.000000 OBP_security_pillar-0.1.1/OBP_security_pillar/rds/__init__.py
--rw-rw-rw-   0        0        0     1554 2023-05-25 09:12:47.000000 OBP_security_pillar-0.1.1/OBP_security_pillar/rds/rds_automatic_minor_version_upgrade_enabled.py
--rw-rw-rw-   0        0        0     1379 2023-05-25 09:12:47.000000 OBP_security_pillar-0.1.1/OBP_security_pillar/rds/rds_instance_public_access_check.py
--rw-rw-rw-   0        0        0     1392 2023-05-25 09:23:36.000000 OBP_security_pillar-0.1.1/OBP_security_pillar/rds/rds_snapshot_encrypted.py
--rw-rw-rw-   0        0        0     1901 2023-05-25 09:23:36.000000 OBP_security_pillar-0.1.1/OBP_security_pillar/rds/rds_snapshots_public_prohibited.py
--rw-rw-rw-   0        0        0     1401 2023-05-25 09:14:26.000000 OBP_security_pillar-0.1.1/OBP_security_pillar/rds/rds_storage_encrypted.py
-drwxrwxrwx   0        0        0        0 2023-06-02 06:59:18.003988 OBP_security_pillar-0.1.1/OBP_security_pillar/s3/
--rw-rw-rw-   0        0        0     1706 2023-05-25 10:12:07.000000 OBP_security_pillar-0.1.1/OBP_security_pillar/s3/__init__.py
--rw-rw-rw-   0        0        0     1451 2023-05-25 09:33:44.000000 OBP_security_pillar-0.1.1/OBP_security_pillar/s3/s3_bucket_logging_enabled.py
--rw-rw-rw-   0        0        0     2145 2023-05-25 09:33:44.000000 OBP_security_pillar-0.1.1/OBP_security_pillar/s3/s3_bucket_public_read_prohibited.py
--rw-rw-rw-   0        0        0     2147 2023-05-25 09:33:44.000000 OBP_security_pillar-0.1.1/OBP_security_pillar/s3/s3_bucket_public_write_prohibited.py
--rw-rw-rw-   0        0        0     1391 2023-05-25 09:38:15.000000 OBP_security_pillar-0.1.1/OBP_security_pillar/s3/s3_bucket_server_side_encryption_enabled.py
--rw-rw-rw-   0        0        0     2260 2023-05-25 09:33:44.000000 OBP_security_pillar-0.1.1/OBP_security_pillar/s3/s3_bucket_ssl_requests_only.py
--rw-rw-rw-   0        0        0     1713 2023-05-25 09:33:44.000000 OBP_security_pillar-0.1.1/OBP_security_pillar/s3/s3_bucket_versioning_enabled.py
--rw-rw-rw-   0        0        0     1817 2023-05-25 09:33:44.000000 OBP_security_pillar-0.1.1/OBP_security_pillar/s3/s3_default_encryption_kms.py
--rw-rw-rw-   0        0        0     1761 2023-01-04 11:06:48.000000 OBP_security_pillar-0.1.1/OBP_security_pillar/security_hub_enabled.py
-drwxrwxrwx   0        0        0        0 2023-06-02 06:59:17.499492 OBP_security_pillar-0.1.1/OBP_security_pillar.egg-info/
--rw-rw-rw-   0        0        0      797 2023-06-02 06:59:17.000000 OBP_security_pillar-0.1.1/OBP_security_pillar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2223 2023-06-02 06:59:17.000000 OBP_security_pillar-0.1.1/OBP_security_pillar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 06:59:17.000000 OBP_security_pillar-0.1.1/OBP_security_pillar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-06-02 06:59:17.000000 OBP_security_pillar-0.1.1/OBP_security_pillar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      797 2023-06-02 06:59:18.006988 OBP_security_pillar-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      464 2022-12-19 07:07:51.000000 OBP_security_pillar-0.1.1/README.md
--rw-rw-rw-   0        0        0      495 2023-06-02 06:52:59.000000 OBP_security_pillar-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-02 06:59:18.008991 OBP_security_pillar-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-18 05:06:53.018776 OBP_security_pillar-0.1.2/
+drwxrwxrwx   0        0        0        0 2023-07-18 05:06:52.802776 OBP_security_pillar-0.1.2/OBP_security_pillar/
+-rw-rw-rw-   0        0        0     3955 2023-07-18 05:06:22.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 05:06:52.825774 OBP_security_pillar-0.1.2/OBP_security_pillar/auto_scaling/
+-rw-rw-rw-   0        0        0      475 2023-05-25 10:12:07.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/auto_scaling/__init__.py
+-rw-rw-rw-   0        0        0     2189 2023-01-27 08:23:40.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/auto_scaling/launch_config_public_ip_disabled.py
+drwxrwxrwx   0        0        0        0 2023-07-18 05:06:52.840774 OBP_security_pillar-0.1.2/OBP_security_pillar/cloudtrail/
+-rw-rw-rw-   0        0        0      724 2023-05-25 10:12:07.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/cloudtrail/__init__.py
+-rw-rw-rw-   0        0        0     2509 2023-01-27 08:24:11.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/cloudtrail/cloudtrail_cloudwatch_logs_enabled.py
+-rw-rw-rw-   0        0        0     3124 2023-05-25 10:12:07.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/cloudtrail/driver.py
+-rw-rw-rw-   0        0        0     1251 2023-01-27 07:29:08.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/compliance.py
+drwxrwxrwx   0        0        0        0 2023-07-18 05:06:52.855775 OBP_security_pillar-0.1.2/OBP_security_pillar/dynamodb/
+-rw-rw-rw-   0        0        0      493 2023-05-25 10:12:07.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/dynamodb/__init__.py
+-rw-rw-rw-   0        0        0     2863 2023-01-27 08:24:38.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/dynamodb/dynamodb_table_encrypted_kms.py
+drwxrwxrwx   0        0        0        0 2023-07-18 05:06:52.936776 OBP_security_pillar-0.1.2/OBP_security_pillar/ec2/
+-rw-rw-rw-   0        0        0     2214 2023-05-25 10:01:21.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/ec2/Incoming_ssh_disabled.py
+-rw-rw-rw-   0        0        0     2852 2023-05-25 10:19:42.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/ec2/__init__.py
+-rw-rw-rw-   0        0        0     3275 2023-05-25 10:01:21.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/ec2/ebs_snapshot_public_restorable_check.py
+-rw-rw-rw-   0        0        0     1519 2023-05-25 10:01:21.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/ec2/ec2_ebs_encryption_by_default.py
+-rw-rw-rw-   0        0        0     2105 2023-01-27 07:29:08.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/ec2/ec2_encrypted_volume.py
+-rw-rw-rw-   0        0        0     1540 2023-05-25 10:01:21.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/ec2/ec2_imdsv2_check.py
+-rw-rw-rw-   0        0        0     3047 2023-05-25 10:01:21.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/ec2/ec2_instance_managed_by_ssm.py
+-rw-rw-rw-   0        0        0     1431 2023-05-25 10:01:21.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/ec2/ec2_instance_multiple_eni_check.py
+-rw-rw-rw-   0        0        0     1519 2023-05-25 10:01:21.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/ec2/ec2_instance_profile_attached.py
+-rw-rw-rw-   0        0        0     2088 2023-05-25 10:01:21.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/ec2/ec2_volume_inuse_check.py
+-rw-rw-rw-   0        0        0     2223 2023-01-27 08:28:22.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/ec2/instance_in_vpc.py
+-rw-rw-rw-   0        0        0     2348 2023-05-25 10:01:21.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/ec2/vpc_flow_logs_enabled.py
+-rw-rw-rw-   0        0        0     2793 2023-01-27 08:43:11.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/elb_logging_enabled.py
+-rw-rw-rw-   0        0        0     2268 2023-01-27 08:43:27.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/elb_tls_https_listeners_only.py
+-rw-rw-rw-   0        0        0     1969 2023-01-27 08:44:03.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/guard_duty_enabled.py
+-rw-rw-rw-   0        0        0     2387 2023-01-27 08:44:27.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/lambda_inside_vpc.py
+drwxrwxrwx   0        0        0        0 2023-07-18 05:06:52.968775 OBP_security_pillar-0.1.2/OBP_security_pillar/rds/
+-rw-rw-rw-   0        0        0     2835 2023-05-25 09:38:15.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/rds/__init__.py
+-rw-rw-rw-   0        0        0     1554 2023-05-25 09:12:47.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/rds/rds_automatic_minor_version_upgrade_enabled.py
+-rw-rw-rw-   0        0        0     1379 2023-05-25 09:12:47.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/rds/rds_instance_public_access_check.py
+-rw-rw-rw-   0        0        0     1392 2023-05-25 09:23:36.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/rds/rds_snapshot_encrypted.py
+-rw-rw-rw-   0        0        0     1901 2023-05-25 09:23:36.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/rds/rds_snapshots_public_prohibited.py
+-rw-rw-rw-   0        0        0     1401 2023-05-25 09:14:26.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/rds/rds_storage_encrypted.py
+drwxrwxrwx   0        0        0        0 2023-07-18 05:06:53.011778 OBP_security_pillar-0.1.2/OBP_security_pillar/s3/
+-rw-rw-rw-   0        0        0     1706 2023-05-25 10:12:07.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/s3/__init__.py
+-rw-rw-rw-   0        0        0     1645 2023-07-18 05:06:22.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/s3/s3_bucket_logging_enabled.py
+-rw-rw-rw-   0        0        0     2145 2023-05-25 09:33:44.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/s3/s3_bucket_public_read_prohibited.py
+-rw-rw-rw-   0        0        0     2147 2023-05-25 09:33:44.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/s3/s3_bucket_public_write_prohibited.py
+-rw-rw-rw-   0        0        0     1391 2023-05-25 09:38:15.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/s3/s3_bucket_server_side_encryption_enabled.py
+-rw-rw-rw-   0        0        0     2260 2023-05-25 09:33:44.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/s3/s3_bucket_ssl_requests_only.py
+-rw-rw-rw-   0        0        0     1954 2023-07-18 05:06:22.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/s3/s3_bucket_versioning_enabled.py
+-rw-rw-rw-   0        0        0     1817 2023-05-25 09:33:44.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/s3/s3_default_encryption_kms.py
+-rw-rw-rw-   0        0        0     1761 2023-01-04 11:06:48.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/security_hub_enabled.py
+drwxrwxrwx   0        0        0        0 2023-07-18 05:06:52.812791 OBP_security_pillar-0.1.2/OBP_security_pillar.egg-info/
+-rw-rw-rw-   0        0        0      797 2023-07-18 05:06:52.000000 OBP_security_pillar-0.1.2/OBP_security_pillar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2223 2023-07-18 05:06:52.000000 OBP_security_pillar-0.1.2/OBP_security_pillar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 05:06:52.000000 OBP_security_pillar-0.1.2/OBP_security_pillar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-07-18 05:06:52.000000 OBP_security_pillar-0.1.2/OBP_security_pillar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      797 2023-07-18 05:06:53.015780 OBP_security_pillar-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2022-12-19 07:07:51.000000 OBP_security_pillar-0.1.2/README.md
+-rw-rw-rw-   0        0        0      495 2023-07-18 05:06:22.000000 OBP_security_pillar-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-18 05:06:53.018776 OBP_security_pillar-0.1.2/setup.cfg
```

### Comparing `OBP_security_pillar-0.1.1/OBP_security_pillar/__init__.py` & `OBP_security_pillar-0.1.2/OBP_security_pillar/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
 __author__ = 'Dheeraj Banodha'
-__version__ = '0.1.1'
+__version__ = '0.1.2'
 
 
 class aws_client:
     def __init__(self, **kwargs):
         """
         @param str aws_access_key_id: AWS Access Key ID
         @param str aws_secret_access_key: AWS Secret Access Key
```

### Comparing `OBP_security_pillar-0.1.1/OBP_security_pillar/auto_scaling/launch_config_public_ip_disabled.py` & `OBP_security_pillar-0.1.2/OBP_security_pillar/auto_scaling/launch_config_public_ip_disabled.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.1/OBP_security_pillar/cloudtrail/__init__.py` & `OBP_security_pillar-0.1.2/OBP_security_pillar/cloudtrail/__init__.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.1/OBP_security_pillar/cloudtrail/cloudtrail_cloudwatch_logs_enabled.py` & `OBP_security_pillar-0.1.2/OBP_security_pillar/cloudtrail/cloudtrail_cloudwatch_logs_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.1/OBP_security_pillar/cloudtrail/driver.py` & `OBP_security_pillar-0.1.2/OBP_security_pillar/cloudtrail/driver.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.1/OBP_security_pillar/compliance.py` & `OBP_security_pillar-0.1.2/OBP_security_pillar/compliance.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.1/OBP_security_pillar/dynamodb/dynamodb_table_encrypted_kms.py` & `OBP_security_pillar-0.1.2/OBP_security_pillar/dynamodb/dynamodb_table_encrypted_kms.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.1/OBP_security_pillar/ec2/Incoming_ssh_disabled.py` & `OBP_security_pillar-0.1.2/OBP_security_pillar/ec2/Incoming_ssh_disabled.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.1/OBP_security_pillar/ec2/__init__.py` & `OBP_security_pillar-0.1.2/OBP_security_pillar/ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.1/OBP_security_pillar/ec2/ebs_snapshot_public_restorable_check.py` & `OBP_security_pillar-0.1.2/OBP_security_pillar/ec2/ebs_snapshot_public_restorable_check.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.1/OBP_security_pillar/ec2/ec2_ebs_encryption_by_default.py` & `OBP_security_pillar-0.1.2/OBP_security_pillar/ec2/ec2_ebs_encryption_by_default.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.1/OBP_security_pillar/ec2/ec2_encrypted_volume.py` & `OBP_security_pillar-0.1.2/OBP_security_pillar/ec2/ec2_encrypted_volume.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.1/OBP_security_pillar/ec2/ec2_imdsv2_check.py` & `OBP_security_pillar-0.1.2/OBP_security_pillar/ec2/ec2_imdsv2_check.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.1/OBP_security_pillar/ec2/ec2_instance_managed_by_ssm.py` & `OBP_security_pillar-0.1.2/OBP_security_pillar/ec2/ec2_instance_managed_by_ssm.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.1/OBP_security_pillar/ec2/ec2_instance_multiple_eni_check.py` & `OBP_security_pillar-0.1.2/OBP_security_pillar/ec2/ec2_instance_multiple_eni_check.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.1/OBP_security_pillar/ec2/ec2_instance_profile_attached.py` & `OBP_security_pillar-0.1.2/OBP_security_pillar/ec2/ec2_instance_profile_attached.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.1/OBP_security_pillar/ec2/ec2_volume_inuse_check.py` & `OBP_security_pillar-0.1.2/OBP_security_pillar/ec2/ec2_volume_inuse_check.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.1/OBP_security_pillar/ec2/instance_in_vpc.py` & `OBP_security_pillar-0.1.2/OBP_security_pillar/ec2/instance_in_vpc.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.1/OBP_security_pillar/ec2/vpc_flow_logs_enabled.py` & `OBP_security_pillar-0.1.2/OBP_security_pillar/ec2/vpc_flow_logs_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.1/OBP_security_pillar/elb_logging_enabled.py` & `OBP_security_pillar-0.1.2/OBP_security_pillar/elb_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.1/OBP_security_pillar/elb_tls_https_listeners_only.py` & `OBP_security_pillar-0.1.2/OBP_security_pillar/elb_tls_https_listeners_only.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.1/OBP_security_pillar/guard_duty_enabled.py` & `OBP_security_pillar-0.1.2/OBP_security_pillar/guard_duty_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.1/OBP_security_pillar/lambda_inside_vpc.py` & `OBP_security_pillar-0.1.2/OBP_security_pillar/lambda_inside_vpc.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.1/OBP_security_pillar/rds/__init__.py` & `OBP_security_pillar-0.1.2/OBP_security_pillar/rds/__init__.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.1/OBP_security_pillar/rds/rds_automatic_minor_version_upgrade_enabled.py` & `OBP_security_pillar-0.1.2/OBP_security_pillar/rds/rds_automatic_minor_version_upgrade_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.1/OBP_security_pillar/rds/rds_instance_public_access_check.py` & `OBP_security_pillar-0.1.2/OBP_security_pillar/rds/rds_instance_public_access_check.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.1/OBP_security_pillar/rds/rds_snapshot_encrypted.py` & `OBP_security_pillar-0.1.2/OBP_security_pillar/rds/rds_snapshot_encrypted.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.1/OBP_security_pillar/rds/rds_snapshots_public_prohibited.py` & `OBP_security_pillar-0.1.2/OBP_security_pillar/rds/rds_snapshots_public_prohibited.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.1/OBP_security_pillar/rds/rds_storage_encrypted.py` & `OBP_security_pillar-0.1.2/OBP_security_pillar/rds/rds_storage_encrypted.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.1/OBP_security_pillar/s3/__init__.py` & `OBP_security_pillar-0.1.2/OBP_security_pillar/s3/__init__.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.1/OBP_security_pillar/s3/s3_bucket_logging_enabled.py` & `OBP_security_pillar-0.1.2/OBP_security_pillar/s3/s3_bucket_logging_enabled.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import logging
 
+from botocore.exceptions import ClientError
+
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
 # checks the compliance.py for s3 bucket versioning enabled
 def s3_bucket_logging_enabled(self, buckets):
     """
@@ -35,15 +37,18 @@
             )
             if resp['LoggingEnabled'] is None:
                 raise KeyError
         except KeyError:
             result = False
             failReason = "Bucket logging is not enabled"
             offenders.append(bucket_name)
-            continue
+        except ClientError:
+            result = False
+            failReason = "Access denied for get_bucket_logging api"
+            offenders.append(bucket_name)
 
     return {
         'Result': result,
         'failReason': failReason,
         'resource_type': resource_type,
         'Offenders': offenders,
         'Compliance_type': compliance_type,
```

### Comparing `OBP_security_pillar-0.1.1/OBP_security_pillar/s3/s3_bucket_public_read_prohibited.py` & `OBP_security_pillar-0.1.2/OBP_security_pillar/s3/s3_bucket_public_read_prohibited.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.1/OBP_security_pillar/s3/s3_bucket_public_write_prohibited.py` & `OBP_security_pillar-0.1.2/OBP_security_pillar/s3/s3_bucket_public_write_prohibited.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.1/OBP_security_pillar/s3/s3_bucket_server_side_encryption_enabled.py` & `OBP_security_pillar-0.1.2/OBP_security_pillar/s3/s3_bucket_server_side_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.1/OBP_security_pillar/s3/s3_bucket_ssl_requests_only.py` & `OBP_security_pillar-0.1.2/OBP_security_pillar/s3/s3_bucket_ssl_requests_only.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.1/OBP_security_pillar/s3/s3_bucket_versioning_enabled.py` & `OBP_security_pillar-0.1.2/OBP_security_pillar/s3/s3_bucket_versioning_enabled.py`

 * *Files 10% similar despite different names*

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
@@ -35,14 +37,19 @@
             )
             status = resp['Status']
         except KeyError:
             result = False
             failReason = "Either bucket versioning is not enabled or configuration not found"
             offenders.append(bucket_name)
             continue
+        except ClientError:
+            result = False
+            failReason = "Access denied for get_bucket_versioning api"
+            offenders.append(bucket_name)
+            continue
 
         if not status == 'Enabled':
             result = False
             failReason = "Either bucket versioning is not enabled or configuration not found"
             offenders.append(bucket_name)
 
     return {
```

### Comparing `OBP_security_pillar-0.1.1/OBP_security_pillar/s3/s3_default_encryption_kms.py` & `OBP_security_pillar-0.1.2/OBP_security_pillar/s3/s3_default_encryption_kms.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.1/OBP_security_pillar/security_hub_enabled.py` & `OBP_security_pillar-0.1.2/OBP_security_pillar/security_hub_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.1/OBP_security_pillar.egg-info/PKG-INFO` & `OBP_security_pillar-0.1.2/OBP_security_pillar.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OBP-security-pillar
-Version: 0.1.1
+Version: 0.1.2
 Summary: Provides AWS compliance details
 Author-email: "dheeraj.banodha" <dheerajmbanodha@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `OBP_security_pillar-0.1.1/OBP_security_pillar.egg-info/SOURCES.txt` & `OBP_security_pillar-0.1.2/OBP_security_pillar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.1/PKG-INFO` & `OBP_security_pillar-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OBP_security_pillar
-Version: 0.1.1
+Version: 0.1.2
 Summary: Provides AWS compliance details
 Author-email: "dheeraj.banodha" <dheerajmbanodha@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

