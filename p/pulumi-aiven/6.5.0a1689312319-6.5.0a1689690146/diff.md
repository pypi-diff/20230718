# Comparing `tmp/pulumi_aiven-6.5.0a1689312319.tar.gz` & `tmp/pulumi_aiven-6.5.0a1689690146.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_aiven-6.5.0a1689312319.tar", last modified: Fri Jul 14 05:34:18 2023, max compression
+gzip compressed data, was "pulumi_aiven-6.5.0a1689690146.tar", last modified: Tue Jul 18 14:27:57 2023, max compression
```

## Comparing `pulumi_aiven-6.5.0a1689312319.tar` & `pulumi_aiven-6.5.0a1689690146.tar`

### file list

```diff
@@ -1,146 +1,148 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:34:18.073686 pulumi_aiven-6.5.0a1689312319/
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-14 05:34:18.073686 pulumi_aiven-6.5.0a1689312319/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:34:18.069686 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/
--rw-r--r--   0 runner    (1001) docker     (123)    15267 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   605185 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    18710 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/account.py
--rw-r--r--   0 runner    (1001) docker     (123)    36913 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/account_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/account_team.py
--rw-r--r--   0 runner    (1001) docker     (123)    17027 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/account_team_member.py
--rw-r--r--   0 runner    (1001) docker     (123)    12601 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/account_team_project.py
--rw-r--r--   0 runner    (1001) docker     (123)    15297 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/aws_privatelink.py
--rw-r--r--   0 runner    (1001) docker     (123)    18483 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/aws_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    18159 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/azure_privatelink.py
--rw-r--r--   0 runner    (1001) docker     (123)    15298 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/azure_privatelink_connection_approval.py
--rw-r--r--   0 runner    (1001) docker     (123)    24958 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/azure_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    29700 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/billing_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    75264 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/cassandra.py
--rw-r--r--   0 runner    (1001) docker     (123)    19426 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/cassandra_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    74927 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (123)    17227 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/clickhouse_database.py
--rw-r--r--   0 runner    (1001) docker     (123)    26558 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/clickhouse_grant.py
--rw-r--r--   0 runner    (1001) docker     (123)    13649 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/clickhouse_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    16426 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/clickhouse_user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:34:18.069686 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    26197 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/connection_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    74949 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/flink.py
--rw-r--r--   0 runner    (1001) docker     (123)    17471 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/flink_application.py
--rw-r--r--   0 runner    (1001) docker     (123)    22264 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/flink_application_deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)    31939 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/flink_application_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15247 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/gcp_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    12740 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_account_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_account_team.py
--rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_account_team_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_account_team_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_aws_privatelink.py
--rw-r--r--   0 runner    (1001) docker     (123)     8738 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_aws_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     7967 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_azure_privatelink.py
--rw-r--r--   0 runner    (1001) docker     (123)    10992 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_azure_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9876 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_billing_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    22288 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_cassanda.py
--rw-r--r--   0 runner    (1001) docker     (123)    21956 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_cassandra.py
--rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_cassandra_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    22032 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_clickhouse_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_clickhouse_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     9261 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_connection_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    21712 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_flink.py
--rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_flink_application.py
--rw-r--r--   0 runner    (1001) docker     (123)    11198 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_flink_application_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_gcp_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    21816 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_grafana.py
--rw-r--r--   0 runner    (1001) docker     (123)    21893 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_influx_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_influxdb_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_influxdb_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    22711 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)     8784 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_kafka_acl.py
--rw-r--r--   0 runner    (1001) docker     (123)    22188 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_kafka_connect.py
--rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_kafka_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    22457 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_kafka_mirror_maker.py
--rw-r--r--   0 runner    (1001) docker     (123)     8372 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_kafka_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_kafka_schema_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_kafka_schema_registry_acl.py
--rw-r--r--   0 runner    (1001) docker     (123)     8642 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_kafka_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     8102 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_kafka_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    22135 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_m3_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)    21648 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_m3_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_m3db_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    13043 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_mirror_maker_replication_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    21724 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_my_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     6911 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_mysql_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     8731 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_mysql_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    22025 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_open_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_open_search_acl_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8788 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_open_search_acl_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_opensearch_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_organizational_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)    21537 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_pg.py
--rw-r--r--   0 runner    (1001) docker     (123)     8070 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_pg_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_pg_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    11717 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_project_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_project_vpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    21691 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_redis.py
--rw-r--r--   0 runner    (1001) docker     (123)    10043 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_redis_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_service_component.py
--rw-r--r--   0 runner    (1001) docker     (123)    18127 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_service_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    15549 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_service_integration_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     9330 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_transit_gateway_vpc_attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)    76518 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/grafana.py
--rw-r--r--   0 runner    (1001) docker     (123)    74979 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/influx_db.py
--rw-r--r--   0 runner    (1001) docker     (123)    16389 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/influxdb_database.py
--rw-r--r--   0 runner    (1001) docker     (123)    19380 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/influxdb_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    80341 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)    19320 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/kafka_acl.py
--rw-r--r--   0 runner    (1001) docker     (123)    77911 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/kafka_connect.py
--rw-r--r--   0 runner    (1001) docker     (123)    24756 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/kafka_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    78467 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/kafka_mirror_maker.py
--rw-r--r--   0 runner    (1001) docker     (123)    22353 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/kafka_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    14423 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/kafka_schema_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    19053 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/kafka_schema_registry_acl.py
--rw-r--r--   0 runner    (1001) docker     (123)    24119 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/kafka_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)    18906 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/kafka_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    77311 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/m3_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)    76197 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/m3_db.py
--rw-r--r--   0 runner    (1001) docker     (123)    16718 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/m3db_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    37020 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/mirror_maker_replication_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    76820 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/my_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)    17313 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/mysql_database.py
--rw-r--r--   0 runner    (1001) docker     (123)    21561 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/mysql_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    75940 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/open_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    18457 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/open_search_acl_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    22685 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/open_search_acl_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    16994 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/opensearch_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/organization.py
--rw-r--r--   0 runner    (1001) docker     (123)    10927 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/organizational_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)   908748 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    73358 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/pg.py
--rw-r--r--   0 runner    (1001) docker     (123)    22840 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/pg_database.py
--rw-r--r--   0 runner    (1001) docker     (123)    21818 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/pg_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    37913 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    13742 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/project_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/project_vpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    76316 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)    30212 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/redis_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    53125 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/service_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    52318 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/service_integration_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    14185 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/static_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)    23726 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven/transit_gateway_vpc_attachment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:34:18.069686 pulumi_aiven-6.5.0a1689312319/pulumi_aiven.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-14 05:34:18.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-07-14 05:34:18.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 05:34:18.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 05:34:18.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-14 05:34:18.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-14 05:34:18.000000 pulumi_aiven-6.5.0a1689312319/pulumi_aiven.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 05:34:18.073686 pulumi_aiven-6.5.0a1689312319/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-14 05:34:17.000000 pulumi_aiven-6.5.0a1689312319/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:27:57.919870 pulumi_aiven-6.5.0a1689690146/
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-18 14:27:57.919870 pulumi_aiven-6.5.0a1689690146/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:27:57.919870 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/
+-rw-r--r--   0 runner    (1001) docker     (123)    15512 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   618269 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18710 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36913 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/account_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/account_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17027 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/account_team_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12601 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/account_team_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15297 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/aws_privatelink.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18483 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/aws_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18159 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/azure_privatelink.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15298 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/azure_privatelink_connection_approval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24958 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/azure_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34308 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/billing_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75264 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/cassandra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19426 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/cassandra_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74927 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17227 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/clickhouse_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26558 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/clickhouse_grant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13649 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/clickhouse_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16426 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/clickhouse_user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:27:57.919870 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26197 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/connection_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74949 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/flink.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17471 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/flink_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22264 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/flink_application_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31939 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/flink_application_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15247 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/gcp_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12740 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_account_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_account_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_account_team_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_account_team_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_aws_privatelink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8738 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_aws_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7967 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_azure_privatelink.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10992 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_azure_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10510 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_billing_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22288 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_cassanda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21956 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_cassandra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_cassandra_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22032 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_clickhouse_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_clickhouse_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9261 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_connection_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21712 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_flink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_flink_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11198 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_flink_application_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_gcp_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21816 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_grafana.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21893 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_influx_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_influxdb_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_influxdb_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22711 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8784 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_kafka_acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22188 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_kafka_connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_kafka_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22457 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_kafka_mirror_maker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8372 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_kafka_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_kafka_schema_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_kafka_schema_registry_acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8642 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_kafka_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8102 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_kafka_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22135 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_m3_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21648 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_m3_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_m3db_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13043 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_mirror_maker_replication_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21724 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_my_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6911 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_mysql_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8731 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_mysql_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22025 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_open_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_open_search_acl_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8788 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_open_search_acl_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_opensearch_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_organization_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_organizational_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21537 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_pg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8070 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_pg_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_pg_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12344 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_project_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_project_vpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21691 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10043 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_redis_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_service_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18127 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_service_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15549 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_service_integration_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9330 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_transit_gateway_vpc_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76518 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/grafana.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74979 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/influx_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16389 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/influxdb_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19380 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/influxdb_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80341 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19320 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/kafka_acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77911 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/kafka_connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24756 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/kafka_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78467 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/kafka_mirror_maker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22353 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/kafka_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14423 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/kafka_schema_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19053 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/kafka_schema_registry_acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24119 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/kafka_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18906 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/kafka_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77311 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/m3_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76197 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/m3_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16718 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/m3db_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37020 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/mirror_maker_replication_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76820 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/my_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17313 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/mysql_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21561 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/mysql_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75940 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/open_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18457 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/open_search_acl_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22685 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/open_search_acl_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16994 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/opensearch_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14643 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/organization_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10927 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/organizational_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)   929584 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73358 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/pg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22840 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/pg_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21818 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/pg_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42472 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13742 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/project_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/project_vpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    76316 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30212 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/redis_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53125 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/service_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52318 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/service_integration_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14185 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/static_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23726 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/transit_gateway_vpc_attachment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:27:57.919870 pulumi_aiven-6.5.0a1689690146/pulumi_aiven.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 14:27:57.919870 pulumi_aiven-6.5.0a1689690146/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/setup.py
```

### Comparing `pulumi_aiven-6.5.0a1689312319/PKG-INFO` & `pulumi_aiven-6.5.0a1689690146/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_aiven
-Version: 6.5.0a1689312319
+Version: 6.5.0a1689690146
 Summary: A Pulumi package for creating and managing Aiven cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-aiven
 Keywords: pulumi aiven
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_aiven-6.5.0a1689312319/README.md` & `pulumi_aiven-6.5.0a1689690146/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/__init__.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,15 @@
 from .get_mysql_database import *
 from .get_mysql_user import *
 from .get_open_search import *
 from .get_open_search_acl_config import *
 from .get_open_search_acl_rule import *
 from .get_opensearch_user import *
 from .get_organization import *
+from .get_organization_user import *
 from .get_organizational_unit import *
 from .get_pg import *
 from .get_pg_database import *
 from .get_pg_user import *
 from .get_project import *
 from .get_project_user import *
 from .get_project_vpc import *
@@ -111,14 +112,15 @@
 from .mysql_database import *
 from .mysql_user import *
 from .open_search import *
 from .open_search_acl_config import *
 from .open_search_acl_rule import *
 from .opensearch_user import *
 from .organization import *
+from .organization_user import *
 from .organizational_unit import *
 from .pg import *
 from .pg_database import *
 from .pg_user import *
 from .project import *
 from .project_user import *
 from .project_vpc import *
@@ -540,14 +542,22 @@
   "fqn": "pulumi_aiven",
   "classes": {
    "aiven:index/organization:Organization": "Organization"
   }
  },
  {
   "pkg": "aiven",
+  "mod": "index/organizationUser",
+  "fqn": "pulumi_aiven",
+  "classes": {
+   "aiven:index/organizationUser:OrganizationUser": "OrganizationUser"
+  }
+ },
+ {
+  "pkg": "aiven",
   "mod": "index/organizationalUnit",
   "fqn": "pulumi_aiven",
   "classes": {
    "aiven:index/organizationalUnit:OrganizationalUnit": "OrganizationalUnit"
   }
  },
  {
```

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/_inputs.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/_inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,17 @@
     'CassandraCassandraUserConfigPublicAccessArgs',
     'CassandraComponentArgs',
     'CassandraServiceIntegrationArgs',
     'CassandraTagArgs',
     'ClickhouseClickhouseArgs',
     'ClickhouseClickhouseUserConfigArgs',
     'ClickhouseClickhouseUserConfigIpFilterObjectArgs',
+    'ClickhouseClickhouseUserConfigPrivateAccessArgs',
+    'ClickhouseClickhouseUserConfigPrivatelinkAccessArgs',
+    'ClickhouseClickhouseUserConfigPublicAccessArgs',
     'ClickhouseComponentArgs',
     'ClickhouseGrantPrivilegeGrantArgs',
     'ClickhouseGrantRoleGrantArgs',
     'ClickhouseServiceIntegrationArgs',
     'ClickhouseTagArgs',
     'FlinkApplicationVersionSinkArgs',
     'FlinkApplicationVersionSourceArgs',
@@ -829,39 +832,55 @@
 @pulumi.input_type
 class ClickhouseClickhouseUserConfigArgs:
     def __init__(__self__, *,
                  additional_backup_regions: Optional[pulumi.Input[str]] = None,
                  ip_filter_objects: Optional[pulumi.Input[Sequence[pulumi.Input['ClickhouseClickhouseUserConfigIpFilterObjectArgs']]]] = None,
                  ip_filter_strings: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  ip_filters: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 private_access: Optional[pulumi.Input['ClickhouseClickhouseUserConfigPrivateAccessArgs']] = None,
+                 privatelink_access: Optional[pulumi.Input['ClickhouseClickhouseUserConfigPrivatelinkAccessArgs']] = None,
                  project_to_fork_from: Optional[pulumi.Input[str]] = None,
-                 service_to_fork_from: Optional[pulumi.Input[str]] = None):
+                 public_access: Optional[pulumi.Input['ClickhouseClickhouseUserConfigPublicAccessArgs']] = None,
+                 service_to_fork_from: Optional[pulumi.Input[str]] = None,
+                 static_ips: Optional[pulumi.Input[bool]] = None):
         """
         :param pulumi.Input[str] additional_backup_regions: Additional Cloud Regions for Backup Replication.
         :param pulumi.Input[Sequence[pulumi.Input['ClickhouseClickhouseUserConfigIpFilterObjectArgs']]] ip_filter_objects: Allow incoming connections from CIDR address block, e.g. '10.20.0.0/16'.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] ip_filter_strings: Allow incoming connections from CIDR address block, e.g. '10.20.0.0/16'.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] ip_filters: Allow incoming connections from CIDR address block, e.g. '10.20.0.0/16'.
+        :param pulumi.Input['ClickhouseClickhouseUserConfigPrivateAccessArgs'] private_access: Allow access to selected service ports from private networks.
+        :param pulumi.Input['ClickhouseClickhouseUserConfigPrivatelinkAccessArgs'] privatelink_access: Allow access to selected service components through Privatelink.
         :param pulumi.Input[str] project_to_fork_from: Name of another project to fork a service from. This has effect only when a new service is being created.
+        :param pulumi.Input['ClickhouseClickhouseUserConfigPublicAccessArgs'] public_access: Allow access to selected service ports from the public Internet.
         :param pulumi.Input[str] service_to_fork_from: Name of another service to fork from. This has effect only when a new service is being created.
+        :param pulumi.Input[bool] static_ips: Use static public IP addresses.
         """
         if additional_backup_regions is not None:
             pulumi.set(__self__, "additional_backup_regions", additional_backup_regions)
         if ip_filter_objects is not None:
             pulumi.set(__self__, "ip_filter_objects", ip_filter_objects)
         if ip_filter_strings is not None:
             pulumi.set(__self__, "ip_filter_strings", ip_filter_strings)
         if ip_filters is not None:
             warnings.warn("""This will be removed in v5.0.0 and replaced with ip_filter_string instead.""", DeprecationWarning)
             pulumi.log.warn("""ip_filters is deprecated: This will be removed in v5.0.0 and replaced with ip_filter_string instead.""")
         if ip_filters is not None:
             pulumi.set(__self__, "ip_filters", ip_filters)
+        if private_access is not None:
+            pulumi.set(__self__, "private_access", private_access)
+        if privatelink_access is not None:
+            pulumi.set(__self__, "privatelink_access", privatelink_access)
         if project_to_fork_from is not None:
             pulumi.set(__self__, "project_to_fork_from", project_to_fork_from)
+        if public_access is not None:
+            pulumi.set(__self__, "public_access", public_access)
         if service_to_fork_from is not None:
             pulumi.set(__self__, "service_to_fork_from", service_to_fork_from)
+        if static_ips is not None:
+            pulumi.set(__self__, "static_ips", static_ips)
 
     @property
     @pulumi.getter(name="additionalBackupRegions")
     def additional_backup_regions(self) -> Optional[pulumi.Input[str]]:
         """
         Additional Cloud Regions for Backup Replication.
         """
@@ -907,37 +926,85 @@
         return pulumi.get(self, "ip_filters")
 
     @ip_filters.setter
     def ip_filters(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "ip_filters", value)
 
     @property
+    @pulumi.getter(name="privateAccess")
+    def private_access(self) -> Optional[pulumi.Input['ClickhouseClickhouseUserConfigPrivateAccessArgs']]:
+        """
+        Allow access to selected service ports from private networks.
+        """
+        return pulumi.get(self, "private_access")
+
+    @private_access.setter
+    def private_access(self, value: Optional[pulumi.Input['ClickhouseClickhouseUserConfigPrivateAccessArgs']]):
+        pulumi.set(self, "private_access", value)
+
+    @property
+    @pulumi.getter(name="privatelinkAccess")
+    def privatelink_access(self) -> Optional[pulumi.Input['ClickhouseClickhouseUserConfigPrivatelinkAccessArgs']]:
+        """
+        Allow access to selected service components through Privatelink.
+        """
+        return pulumi.get(self, "privatelink_access")
+
+    @privatelink_access.setter
+    def privatelink_access(self, value: Optional[pulumi.Input['ClickhouseClickhouseUserConfigPrivatelinkAccessArgs']]):
+        pulumi.set(self, "privatelink_access", value)
+
+    @property
     @pulumi.getter(name="projectToForkFrom")
     def project_to_fork_from(self) -> Optional[pulumi.Input[str]]:
         """
         Name of another project to fork a service from. This has effect only when a new service is being created.
         """
         return pulumi.get(self, "project_to_fork_from")
 
     @project_to_fork_from.setter
     def project_to_fork_from(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "project_to_fork_from", value)
 
     @property
+    @pulumi.getter(name="publicAccess")
+    def public_access(self) -> Optional[pulumi.Input['ClickhouseClickhouseUserConfigPublicAccessArgs']]:
+        """
+        Allow access to selected service ports from the public Internet.
+        """
+        return pulumi.get(self, "public_access")
+
+    @public_access.setter
+    def public_access(self, value: Optional[pulumi.Input['ClickhouseClickhouseUserConfigPublicAccessArgs']]):
+        pulumi.set(self, "public_access", value)
+
+    @property
     @pulumi.getter(name="serviceToForkFrom")
     def service_to_fork_from(self) -> Optional[pulumi.Input[str]]:
         """
         Name of another service to fork from. This has effect only when a new service is being created.
         """
         return pulumi.get(self, "service_to_fork_from")
 
     @service_to_fork_from.setter
     def service_to_fork_from(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "service_to_fork_from", value)
 
+    @property
+    @pulumi.getter(name="staticIps")
+    def static_ips(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Use static public IP addresses.
+        """
+        return pulumi.get(self, "static_ips")
+
+    @static_ips.setter
+    def static_ips(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "static_ips", value)
+
 
 @pulumi.input_type
 class ClickhouseClickhouseUserConfigIpFilterObjectArgs:
     def __init__(__self__, *,
                  network: pulumi.Input[str],
                  description: Optional[pulumi.Input[str]] = None):
         pulumi.set(__self__, "network", network)
@@ -960,14 +1027,155 @@
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
 
 @pulumi.input_type
+class ClickhouseClickhouseUserConfigPrivateAccessArgs:
+    def __init__(__self__, *,
+                 clickhouse: Optional[pulumi.Input[bool]] = None,
+                 clickhouse_https: Optional[pulumi.Input[bool]] = None,
+                 prometheus: Optional[pulumi.Input[bool]] = None):
+        """
+        :param pulumi.Input[bool] clickhouse: Clickhouse server provided values
+        """
+        if clickhouse is not None:
+            pulumi.set(__self__, "clickhouse", clickhouse)
+        if clickhouse_https is not None:
+            pulumi.set(__self__, "clickhouse_https", clickhouse_https)
+        if prometheus is not None:
+            pulumi.set(__self__, "prometheus", prometheus)
+
+    @property
+    @pulumi.getter
+    def clickhouse(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Clickhouse server provided values
+        """
+        return pulumi.get(self, "clickhouse")
+
+    @clickhouse.setter
+    def clickhouse(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "clickhouse", value)
+
+    @property
+    @pulumi.getter(name="clickhouseHttps")
+    def clickhouse_https(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "clickhouse_https")
+
+    @clickhouse_https.setter
+    def clickhouse_https(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "clickhouse_https", value)
+
+    @property
+    @pulumi.getter
+    def prometheus(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "prometheus")
+
+    @prometheus.setter
+    def prometheus(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "prometheus", value)
+
+
+@pulumi.input_type
+class ClickhouseClickhouseUserConfigPrivatelinkAccessArgs:
+    def __init__(__self__, *,
+                 clickhouse: Optional[pulumi.Input[bool]] = None,
+                 clickhouse_https: Optional[pulumi.Input[bool]] = None,
+                 prometheus: Optional[pulumi.Input[bool]] = None):
+        """
+        :param pulumi.Input[bool] clickhouse: Clickhouse server provided values
+        """
+        if clickhouse is not None:
+            pulumi.set(__self__, "clickhouse", clickhouse)
+        if clickhouse_https is not None:
+            pulumi.set(__self__, "clickhouse_https", clickhouse_https)
+        if prometheus is not None:
+            pulumi.set(__self__, "prometheus", prometheus)
+
+    @property
+    @pulumi.getter
+    def clickhouse(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Clickhouse server provided values
+        """
+        return pulumi.get(self, "clickhouse")
+
+    @clickhouse.setter
+    def clickhouse(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "clickhouse", value)
+
+    @property
+    @pulumi.getter(name="clickhouseHttps")
+    def clickhouse_https(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "clickhouse_https")
+
+    @clickhouse_https.setter
+    def clickhouse_https(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "clickhouse_https", value)
+
+    @property
+    @pulumi.getter
+    def prometheus(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "prometheus")
+
+    @prometheus.setter
+    def prometheus(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "prometheus", value)
+
+
+@pulumi.input_type
+class ClickhouseClickhouseUserConfigPublicAccessArgs:
+    def __init__(__self__, *,
+                 clickhouse: Optional[pulumi.Input[bool]] = None,
+                 clickhouse_https: Optional[pulumi.Input[bool]] = None,
+                 prometheus: Optional[pulumi.Input[bool]] = None):
+        """
+        :param pulumi.Input[bool] clickhouse: Clickhouse server provided values
+        """
+        if clickhouse is not None:
+            pulumi.set(__self__, "clickhouse", clickhouse)
+        if clickhouse_https is not None:
+            pulumi.set(__self__, "clickhouse_https", clickhouse_https)
+        if prometheus is not None:
+            pulumi.set(__self__, "prometheus", prometheus)
+
+    @property
+    @pulumi.getter
+    def clickhouse(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Clickhouse server provided values
+        """
+        return pulumi.get(self, "clickhouse")
+
+    @clickhouse.setter
+    def clickhouse(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "clickhouse", value)
+
+    @property
+    @pulumi.getter(name="clickhouseHttps")
+    def clickhouse_https(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "clickhouse_https")
+
+    @clickhouse_https.setter
+    def clickhouse_https(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "clickhouse_https", value)
+
+    @property
+    @pulumi.getter
+    def prometheus(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "prometheus")
+
+    @prometheus.setter
+    def prometheus(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "prometheus", value)
+
+
+@pulumi.input_type
 class ClickhouseComponentArgs:
     def __init__(__self__, *,
                  component: Optional[pulumi.Input[str]] = None,
                  host: Optional[pulumi.Input[str]] = None,
                  kafka_authentication_method: Optional[pulumi.Input[str]] = None,
                  port: Optional[pulumi.Input[int]] = None,
                  route: Optional[pulumi.Input[str]] = None,
@@ -3361,25 +3569,28 @@
 class InfluxDbInfluxdbUserConfigInfluxdbArgs:
     def __init__(__self__, *,
                  log_queries_after: Optional[pulumi.Input[int]] = None,
                  max_connection_limit: Optional[pulumi.Input[int]] = None,
                  max_row_limit: Optional[pulumi.Input[int]] = None,
                  max_select_buckets: Optional[pulumi.Input[int]] = None,
                  max_select_point: Optional[pulumi.Input[int]] = None,
+                 query_log_enabled: Optional[pulumi.Input[bool]] = None,
                  query_timeout: Optional[pulumi.Input[int]] = None):
         if log_queries_after is not None:
             pulumi.set(__self__, "log_queries_after", log_queries_after)
         if max_connection_limit is not None:
             pulumi.set(__self__, "max_connection_limit", max_connection_limit)
         if max_row_limit is not None:
             pulumi.set(__self__, "max_row_limit", max_row_limit)
         if max_select_buckets is not None:
             pulumi.set(__self__, "max_select_buckets", max_select_buckets)
         if max_select_point is not None:
             pulumi.set(__self__, "max_select_point", max_select_point)
+        if query_log_enabled is not None:
+            pulumi.set(__self__, "query_log_enabled", query_log_enabled)
         if query_timeout is not None:
             pulumi.set(__self__, "query_timeout", query_timeout)
 
     @property
     @pulumi.getter(name="logQueriesAfter")
     def log_queries_after(self) -> Optional[pulumi.Input[int]]:
         return pulumi.get(self, "log_queries_after")
@@ -3421,14 +3632,23 @@
         return pulumi.get(self, "max_select_point")
 
     @max_select_point.setter
     def max_select_point(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "max_select_point", value)
 
     @property
+    @pulumi.getter(name="queryLogEnabled")
+    def query_log_enabled(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "query_log_enabled")
+
+    @query_log_enabled.setter
+    def query_log_enabled(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "query_log_enabled", value)
+
+    @property
     @pulumi.getter(name="queryTimeout")
     def query_timeout(self) -> Optional[pulumi.Input[int]]:
         return pulumi.get(self, "query_timeout")
 
     @query_timeout.setter
     def query_timeout(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "query_timeout", value)
@@ -9823,28 +10043,28 @@
 @pulumi.input_type
 class OpenSearchOpensearchUserConfigPrivateAccessArgs:
     def __init__(__self__, *,
                  opensearch: Optional[pulumi.Input[bool]] = None,
                  opensearch_dashboards: Optional[pulumi.Input[bool]] = None,
                  prometheus: Optional[pulumi.Input[bool]] = None):
         """
-        :param pulumi.Input[bool] opensearch: Opensearch server provided values
+        :param pulumi.Input[bool] opensearch: OpenSearch server provided values
         """
         if opensearch is not None:
             pulumi.set(__self__, "opensearch", opensearch)
         if opensearch_dashboards is not None:
             pulumi.set(__self__, "opensearch_dashboards", opensearch_dashboards)
         if prometheus is not None:
             pulumi.set(__self__, "prometheus", prometheus)
 
     @property
     @pulumi.getter
     def opensearch(self) -> Optional[pulumi.Input[bool]]:
         """
-        Opensearch server provided values
+        OpenSearch server provided values
         """
         return pulumi.get(self, "opensearch")
 
     @opensearch.setter
     def opensearch(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "opensearch", value)
 
@@ -9870,28 +10090,28 @@
 @pulumi.input_type
 class OpenSearchOpensearchUserConfigPrivatelinkAccessArgs:
     def __init__(__self__, *,
                  opensearch: Optional[pulumi.Input[bool]] = None,
                  opensearch_dashboards: Optional[pulumi.Input[bool]] = None,
                  prometheus: Optional[pulumi.Input[bool]] = None):
         """
-        :param pulumi.Input[bool] opensearch: Opensearch server provided values
+        :param pulumi.Input[bool] opensearch: OpenSearch server provided values
         """
         if opensearch is not None:
             pulumi.set(__self__, "opensearch", opensearch)
         if opensearch_dashboards is not None:
             pulumi.set(__self__, "opensearch_dashboards", opensearch_dashboards)
         if prometheus is not None:
             pulumi.set(__self__, "prometheus", prometheus)
 
     @property
     @pulumi.getter
     def opensearch(self) -> Optional[pulumi.Input[bool]]:
         """
-        Opensearch server provided values
+        OpenSearch server provided values
         """
         return pulumi.get(self, "opensearch")
 
     @opensearch.setter
     def opensearch(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "opensearch", value)
 
@@ -9917,28 +10137,28 @@
 @pulumi.input_type
 class OpenSearchOpensearchUserConfigPublicAccessArgs:
     def __init__(__self__, *,
                  opensearch: Optional[pulumi.Input[bool]] = None,
                  opensearch_dashboards: Optional[pulumi.Input[bool]] = None,
                  prometheus: Optional[pulumi.Input[bool]] = None):
         """
-        :param pulumi.Input[bool] opensearch: Opensearch server provided values
+        :param pulumi.Input[bool] opensearch: OpenSearch server provided values
         """
         if opensearch is not None:
             pulumi.set(__self__, "opensearch", opensearch)
         if opensearch_dashboards is not None:
             pulumi.set(__self__, "opensearch_dashboards", opensearch_dashboards)
         if prometheus is not None:
             pulumi.set(__self__, "prometheus", prometheus)
 
     @property
     @pulumi.getter
     def opensearch(self) -> Optional[pulumi.Input[bool]]:
         """
-        Opensearch server provided values
+        OpenSearch server provided values
         """
         return pulumi.get(self, "opensearch")
 
     @opensearch.setter
     def opensearch(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "opensearch", value)
 
@@ -12643,21 +12863,45 @@
 
 @pulumi.input_type
 class ServiceIntegrationClickhouseKafkaUserConfigTableArgs:
     def __init__(__self__, *,
                  data_format: pulumi.Input[str],
                  group_name: pulumi.Input[str],
                  name: pulumi.Input[str],
+                 auto_offset_reset: Optional[pulumi.Input[str]] = None,
                  columns: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceIntegrationClickhouseKafkaUserConfigTableColumnArgs']]]] = None,
+                 date_time_input_format: Optional[pulumi.Input[str]] = None,
+                 handle_error_mode: Optional[pulumi.Input[str]] = None,
+                 max_block_size: Optional[pulumi.Input[int]] = None,
+                 max_rows_per_message: Optional[pulumi.Input[int]] = None,
+                 num_consumers: Optional[pulumi.Input[int]] = None,
+                 poll_max_batch_size: Optional[pulumi.Input[int]] = None,
+                 skip_broken_messages: Optional[pulumi.Input[int]] = None,
                  topics: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceIntegrationClickhouseKafkaUserConfigTableTopicArgs']]]] = None):
         pulumi.set(__self__, "data_format", data_format)
         pulumi.set(__self__, "group_name", group_name)
         pulumi.set(__self__, "name", name)
+        if auto_offset_reset is not None:
+            pulumi.set(__self__, "auto_offset_reset", auto_offset_reset)
         if columns is not None:
             pulumi.set(__self__, "columns", columns)
+        if date_time_input_format is not None:
+            pulumi.set(__self__, "date_time_input_format", date_time_input_format)
+        if handle_error_mode is not None:
+            pulumi.set(__self__, "handle_error_mode", handle_error_mode)
+        if max_block_size is not None:
+            pulumi.set(__self__, "max_block_size", max_block_size)
+        if max_rows_per_message is not None:
+            pulumi.set(__self__, "max_rows_per_message", max_rows_per_message)
+        if num_consumers is not None:
+            pulumi.set(__self__, "num_consumers", num_consumers)
+        if poll_max_batch_size is not None:
+            pulumi.set(__self__, "poll_max_batch_size", poll_max_batch_size)
+        if skip_broken_messages is not None:
+            pulumi.set(__self__, "skip_broken_messages", skip_broken_messages)
         if topics is not None:
             pulumi.set(__self__, "topics", topics)
 
     @property
     @pulumi.getter(name="dataFormat")
     def data_format(self) -> pulumi.Input[str]:
         return pulumi.get(self, "data_format")
@@ -12681,23 +12925,95 @@
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: pulumi.Input[str]):
         pulumi.set(self, "name", value)
 
     @property
+    @pulumi.getter(name="autoOffsetReset")
+    def auto_offset_reset(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "auto_offset_reset")
+
+    @auto_offset_reset.setter
+    def auto_offset_reset(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "auto_offset_reset", value)
+
+    @property
     @pulumi.getter
     def columns(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ServiceIntegrationClickhouseKafkaUserConfigTableColumnArgs']]]]:
         return pulumi.get(self, "columns")
 
     @columns.setter
     def columns(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceIntegrationClickhouseKafkaUserConfigTableColumnArgs']]]]):
         pulumi.set(self, "columns", value)
 
     @property
+    @pulumi.getter(name="dateTimeInputFormat")
+    def date_time_input_format(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "date_time_input_format")
+
+    @date_time_input_format.setter
+    def date_time_input_format(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "date_time_input_format", value)
+
+    @property
+    @pulumi.getter(name="handleErrorMode")
+    def handle_error_mode(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "handle_error_mode")
+
+    @handle_error_mode.setter
+    def handle_error_mode(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "handle_error_mode", value)
+
+    @property
+    @pulumi.getter(name="maxBlockSize")
+    def max_block_size(self) -> Optional[pulumi.Input[int]]:
+        return pulumi.get(self, "max_block_size")
+
+    @max_block_size.setter
+    def max_block_size(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "max_block_size", value)
+
+    @property
+    @pulumi.getter(name="maxRowsPerMessage")
+    def max_rows_per_message(self) -> Optional[pulumi.Input[int]]:
+        return pulumi.get(self, "max_rows_per_message")
+
+    @max_rows_per_message.setter
+    def max_rows_per_message(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "max_rows_per_message", value)
+
+    @property
+    @pulumi.getter(name="numConsumers")
+    def num_consumers(self) -> Optional[pulumi.Input[int]]:
+        return pulumi.get(self, "num_consumers")
+
+    @num_consumers.setter
+    def num_consumers(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "num_consumers", value)
+
+    @property
+    @pulumi.getter(name="pollMaxBatchSize")
+    def poll_max_batch_size(self) -> Optional[pulumi.Input[int]]:
+        return pulumi.get(self, "poll_max_batch_size")
+
+    @poll_max_batch_size.setter
+    def poll_max_batch_size(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "poll_max_batch_size", value)
+
+    @property
+    @pulumi.getter(name="skipBrokenMessages")
+    def skip_broken_messages(self) -> Optional[pulumi.Input[int]]:
+        return pulumi.get(self, "skip_broken_messages")
+
+    @skip_broken_messages.setter
+    def skip_broken_messages(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "skip_broken_messages", value)
+
+    @property
     @pulumi.getter
     def topics(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ServiceIntegrationClickhouseKafkaUserConfigTableTopicArgs']]]]:
         return pulumi.get(self, "topics")
 
     @topics.setter
     def topics(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceIntegrationClickhouseKafkaUserConfigTableTopicArgs']]]]):
         pulumi.set(self, "topics", value)
@@ -12816,15 +13132,15 @@
         :param pulumi.Input[Sequence[pulumi.Input['ServiceIntegrationDatadogUserConfigDatadogTagArgs']]] datadog_tags: Custom tags provided by user.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] exclude_consumer_groups: List of custom metrics.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] exclude_topics: List of topics to exclude.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] include_consumer_groups: List of custom metrics.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] include_topics: List of topics to include.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] kafka_custom_metrics: List of custom metrics.
         :param pulumi.Input[int] max_jmx_metrics: Maximum number of JMX metrics to send.
-        :param pulumi.Input['ServiceIntegrationDatadogUserConfigOpensearchArgs'] opensearch: Datadog Opensearch Options.
+        :param pulumi.Input['ServiceIntegrationDatadogUserConfigOpensearchArgs'] opensearch: Datadog OpenSearch Options.
         :param pulumi.Input['ServiceIntegrationDatadogUserConfigRedisArgs'] redis: Datadog Redis Options.
         """
         if datadog_dbm_enabled is not None:
             pulumi.set(__self__, "datadog_dbm_enabled", datadog_dbm_enabled)
         if datadog_tags is not None:
             pulumi.set(__self__, "datadog_tags", datadog_tags)
         if exclude_consumer_groups is not None:
@@ -12940,15 +13256,15 @@
     def max_jmx_metrics(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "max_jmx_metrics", value)
 
     @property
     @pulumi.getter
     def opensearch(self) -> Optional[pulumi.Input['ServiceIntegrationDatadogUserConfigOpensearchArgs']]:
         """
-        Datadog Opensearch Options.
+        Datadog OpenSearch Options.
         """
         return pulumi.get(self, "opensearch")
 
     @opensearch.setter
     def opensearch(self, value: Optional[pulumi.Input['ServiceIntegrationDatadogUserConfigOpensearchArgs']]):
         pulumi.set(self, "opensearch", value)
```

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/_utilities.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/account.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/account.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/account_authentication.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/account_authentication.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/account_team.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/account_team.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/account_team_member.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/account_team_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/account_team_project.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/account_team_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/aws_privatelink.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/aws_privatelink.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/aws_vpc_peering_connection.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/aws_vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/azure_privatelink.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/azure_privatelink.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/azure_privatelink_connection_approval.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/azure_privatelink_connection_approval.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/azure_vpc_peering_connection.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/azure_vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/billing_group.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/billing_group.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,14 +21,15 @@
                  billing_extra_text: Optional[pulumi.Input[str]] = None,
                  card_id: Optional[pulumi.Input[str]] = None,
                  city: Optional[pulumi.Input[str]] = None,
                  company: Optional[pulumi.Input[str]] = None,
                  copy_from_billing_group: Optional[pulumi.Input[str]] = None,
                  country_code: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
+                 parent_id: Optional[pulumi.Input[str]] = None,
                  state: Optional[pulumi.Input[str]] = None,
                  vat_id: Optional[pulumi.Input[str]] = None,
                  zip_code: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a BillingGroup resource.
         :param pulumi.Input[str] account_id: Account id
         :param pulumi.Input[Sequence[pulumi.Input[str]]] address_lines: Address lines
@@ -37,19 +38,23 @@
         :param pulumi.Input[str] billing_extra_text: Billing extra text
         :param pulumi.Input[str] card_id: Credit card id
         :param pulumi.Input[str] city: City
         :param pulumi.Input[str] company: Company name
         :param pulumi.Input[str] copy_from_billing_group: ID of the billing group to copy from
         :param pulumi.Input[str] country_code: Country code
         :param pulumi.Input[str] name: Billing Group name
+        :param pulumi.Input[str] parent_id: An optional property to link a billing group to an already existing organization or account by using its ID. To set up proper dependencies please refer to this variable as a reference.
         :param pulumi.Input[str] state: State
         :param pulumi.Input[str] vat_id: VAT id
         :param pulumi.Input[str] zip_code: Zip Code
         """
         if account_id is not None:
+            warnings.warn("""Use parent_id instead. This field will be removed in the next major release.""", DeprecationWarning)
+            pulumi.log.warn("""account_id is deprecated: Use parent_id instead. This field will be removed in the next major release.""")
+        if account_id is not None:
             pulumi.set(__self__, "account_id", account_id)
         if address_lines is not None:
             pulumi.set(__self__, "address_lines", address_lines)
         if billing_currency is not None:
             pulumi.set(__self__, "billing_currency", billing_currency)
         if billing_emails is not None:
             pulumi.set(__self__, "billing_emails", billing_emails)
@@ -63,27 +68,32 @@
             pulumi.set(__self__, "company", company)
         if copy_from_billing_group is not None:
             pulumi.set(__self__, "copy_from_billing_group", copy_from_billing_group)
         if country_code is not None:
             pulumi.set(__self__, "country_code", country_code)
         if name is not None:
             pulumi.set(__self__, "name", name)
+        if parent_id is not None:
+            pulumi.set(__self__, "parent_id", parent_id)
         if state is not None:
             pulumi.set(__self__, "state", state)
         if vat_id is not None:
             pulumi.set(__self__, "vat_id", vat_id)
         if zip_code is not None:
             pulumi.set(__self__, "zip_code", zip_code)
 
     @property
     @pulumi.getter(name="accountId")
     def account_id(self) -> Optional[pulumi.Input[str]]:
         """
         Account id
         """
+        warnings.warn("""Use parent_id instead. This field will be removed in the next major release.""", DeprecationWarning)
+        pulumi.log.warn("""account_id is deprecated: Use parent_id instead. This field will be removed in the next major release.""")
+
         return pulumi.get(self, "account_id")
 
     @account_id.setter
     def account_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "account_id", value)
 
     @property
@@ -203,14 +213,26 @@
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
+    @pulumi.getter(name="parentId")
+    def parent_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        An optional property to link a billing group to an already existing organization or account by using its ID. To set up proper dependencies please refer to this variable as a reference.
+        """
+        return pulumi.get(self, "parent_id")
+
+    @parent_id.setter
+    def parent_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "parent_id", value)
+
+    @property
     @pulumi.getter
     def state(self) -> Optional[pulumi.Input[str]]:
         """
         State
         """
         return pulumi.get(self, "state")
 
@@ -253,14 +275,15 @@
                  billing_extra_text: Optional[pulumi.Input[str]] = None,
                  card_id: Optional[pulumi.Input[str]] = None,
                  city: Optional[pulumi.Input[str]] = None,
                  company: Optional[pulumi.Input[str]] = None,
                  copy_from_billing_group: Optional[pulumi.Input[str]] = None,
                  country_code: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
+                 parent_id: Optional[pulumi.Input[str]] = None,
                  state: Optional[pulumi.Input[str]] = None,
                  vat_id: Optional[pulumi.Input[str]] = None,
                  zip_code: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering BillingGroup resources.
         :param pulumi.Input[str] account_id: Account id
         :param pulumi.Input[Sequence[pulumi.Input[str]]] address_lines: Address lines
@@ -269,19 +292,23 @@
         :param pulumi.Input[str] billing_extra_text: Billing extra text
         :param pulumi.Input[str] card_id: Credit card id
         :param pulumi.Input[str] city: City
         :param pulumi.Input[str] company: Company name
         :param pulumi.Input[str] copy_from_billing_group: ID of the billing group to copy from
         :param pulumi.Input[str] country_code: Country code
         :param pulumi.Input[str] name: Billing Group name
+        :param pulumi.Input[str] parent_id: An optional property to link a billing group to an already existing organization or account by using its ID. To set up proper dependencies please refer to this variable as a reference.
         :param pulumi.Input[str] state: State
         :param pulumi.Input[str] vat_id: VAT id
         :param pulumi.Input[str] zip_code: Zip Code
         """
         if account_id is not None:
+            warnings.warn("""Use parent_id instead. This field will be removed in the next major release.""", DeprecationWarning)
+            pulumi.log.warn("""account_id is deprecated: Use parent_id instead. This field will be removed in the next major release.""")
+        if account_id is not None:
             pulumi.set(__self__, "account_id", account_id)
         if address_lines is not None:
             pulumi.set(__self__, "address_lines", address_lines)
         if billing_currency is not None:
             pulumi.set(__self__, "billing_currency", billing_currency)
         if billing_emails is not None:
             pulumi.set(__self__, "billing_emails", billing_emails)
@@ -295,27 +322,32 @@
             pulumi.set(__self__, "company", company)
         if copy_from_billing_group is not None:
             pulumi.set(__self__, "copy_from_billing_group", copy_from_billing_group)
         if country_code is not None:
             pulumi.set(__self__, "country_code", country_code)
         if name is not None:
             pulumi.set(__self__, "name", name)
+        if parent_id is not None:
+            pulumi.set(__self__, "parent_id", parent_id)
         if state is not None:
             pulumi.set(__self__, "state", state)
         if vat_id is not None:
             pulumi.set(__self__, "vat_id", vat_id)
         if zip_code is not None:
             pulumi.set(__self__, "zip_code", zip_code)
 
     @property
     @pulumi.getter(name="accountId")
     def account_id(self) -> Optional[pulumi.Input[str]]:
         """
         Account id
         """
+        warnings.warn("""Use parent_id instead. This field will be removed in the next major release.""", DeprecationWarning)
+        pulumi.log.warn("""account_id is deprecated: Use parent_id instead. This field will be removed in the next major release.""")
+
         return pulumi.get(self, "account_id")
 
     @account_id.setter
     def account_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "account_id", value)
 
     @property
@@ -435,14 +467,26 @@
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
+    @pulumi.getter(name="parentId")
+    def parent_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        An optional property to link a billing group to an already existing organization or account by using its ID. To set up proper dependencies please refer to this variable as a reference.
+        """
+        return pulumi.get(self, "parent_id")
+
+    @parent_id.setter
+    def parent_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "parent_id", value)
+
+    @property
     @pulumi.getter
     def state(self) -> Optional[pulumi.Input[str]]:
         """
         State
         """
         return pulumi.get(self, "state")
 
@@ -487,14 +531,15 @@
                  billing_extra_text: Optional[pulumi.Input[str]] = None,
                  card_id: Optional[pulumi.Input[str]] = None,
                  city: Optional[pulumi.Input[str]] = None,
                  company: Optional[pulumi.Input[str]] = None,
                  copy_from_billing_group: Optional[pulumi.Input[str]] = None,
                  country_code: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
+                 parent_id: Optional[pulumi.Input[str]] = None,
                  state: Optional[pulumi.Input[str]] = None,
                  vat_id: Optional[pulumi.Input[str]] = None,
                  zip_code: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         The Billing Group resource allows the creation and management of Aiven Billing Groups and association with the Projects.
 
@@ -527,14 +572,15 @@
         :param pulumi.Input[str] billing_extra_text: Billing extra text
         :param pulumi.Input[str] card_id: Credit card id
         :param pulumi.Input[str] city: City
         :param pulumi.Input[str] company: Company name
         :param pulumi.Input[str] copy_from_billing_group: ID of the billing group to copy from
         :param pulumi.Input[str] country_code: Country code
         :param pulumi.Input[str] name: Billing Group name
+        :param pulumi.Input[str] parent_id: An optional property to link a billing group to an already existing organization or account by using its ID. To set up proper dependencies please refer to this variable as a reference.
         :param pulumi.Input[str] state: State
         :param pulumi.Input[str] vat_id: VAT id
         :param pulumi.Input[str] zip_code: Zip Code
         """
         ...
     @overload
     def __init__(__self__,
@@ -586,37 +632,42 @@
                  billing_extra_text: Optional[pulumi.Input[str]] = None,
                  card_id: Optional[pulumi.Input[str]] = None,
                  city: Optional[pulumi.Input[str]] = None,
                  company: Optional[pulumi.Input[str]] = None,
                  copy_from_billing_group: Optional[pulumi.Input[str]] = None,
                  country_code: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
+                 parent_id: Optional[pulumi.Input[str]] = None,
                  state: Optional[pulumi.Input[str]] = None,
                  vat_id: Optional[pulumi.Input[str]] = None,
                  zip_code: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = BillingGroupArgs.__new__(BillingGroupArgs)
 
+            if account_id is not None and not opts.urn:
+                warnings.warn("""Use parent_id instead. This field will be removed in the next major release.""", DeprecationWarning)
+                pulumi.log.warn("""account_id is deprecated: Use parent_id instead. This field will be removed in the next major release.""")
             __props__.__dict__["account_id"] = account_id
             __props__.__dict__["address_lines"] = address_lines
             __props__.__dict__["billing_currency"] = billing_currency
             __props__.__dict__["billing_emails"] = billing_emails
             __props__.__dict__["billing_extra_text"] = billing_extra_text
             __props__.__dict__["card_id"] = card_id
             __props__.__dict__["city"] = city
             __props__.__dict__["company"] = company
             __props__.__dict__["copy_from_billing_group"] = copy_from_billing_group
             __props__.__dict__["country_code"] = country_code
             __props__.__dict__["name"] = name
+            __props__.__dict__["parent_id"] = parent_id
             __props__.__dict__["state"] = state
             __props__.__dict__["vat_id"] = vat_id
             __props__.__dict__["zip_code"] = zip_code
         super(BillingGroup, __self__).__init__(
             'aiven:index/billingGroup:BillingGroup',
             resource_name,
             __props__,
@@ -633,14 +684,15 @@
             billing_extra_text: Optional[pulumi.Input[str]] = None,
             card_id: Optional[pulumi.Input[str]] = None,
             city: Optional[pulumi.Input[str]] = None,
             company: Optional[pulumi.Input[str]] = None,
             copy_from_billing_group: Optional[pulumi.Input[str]] = None,
             country_code: Optional[pulumi.Input[str]] = None,
             name: Optional[pulumi.Input[str]] = None,
+            parent_id: Optional[pulumi.Input[str]] = None,
             state: Optional[pulumi.Input[str]] = None,
             vat_id: Optional[pulumi.Input[str]] = None,
             zip_code: Optional[pulumi.Input[str]] = None) -> 'BillingGroup':
         """
         Get an existing BillingGroup resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
@@ -654,14 +706,15 @@
         :param pulumi.Input[str] billing_extra_text: Billing extra text
         :param pulumi.Input[str] card_id: Credit card id
         :param pulumi.Input[str] city: City
         :param pulumi.Input[str] company: Company name
         :param pulumi.Input[str] copy_from_billing_group: ID of the billing group to copy from
         :param pulumi.Input[str] country_code: Country code
         :param pulumi.Input[str] name: Billing Group name
+        :param pulumi.Input[str] parent_id: An optional property to link a billing group to an already existing organization or account by using its ID. To set up proper dependencies please refer to this variable as a reference.
         :param pulumi.Input[str] state: State
         :param pulumi.Input[str] vat_id: VAT id
         :param pulumi.Input[str] zip_code: Zip Code
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _BillingGroupState.__new__(_BillingGroupState)
@@ -673,25 +726,29 @@
         __props__.__dict__["billing_extra_text"] = billing_extra_text
         __props__.__dict__["card_id"] = card_id
         __props__.__dict__["city"] = city
         __props__.__dict__["company"] = company
         __props__.__dict__["copy_from_billing_group"] = copy_from_billing_group
         __props__.__dict__["country_code"] = country_code
         __props__.__dict__["name"] = name
+        __props__.__dict__["parent_id"] = parent_id
         __props__.__dict__["state"] = state
         __props__.__dict__["vat_id"] = vat_id
         __props__.__dict__["zip_code"] = zip_code
         return BillingGroup(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="accountId")
     def account_id(self) -> pulumi.Output[Optional[str]]:
         """
         Account id
         """
+        warnings.warn("""Use parent_id instead. This field will be removed in the next major release.""", DeprecationWarning)
+        pulumi.log.warn("""account_id is deprecated: Use parent_id instead. This field will be removed in the next major release.""")
+
         return pulumi.get(self, "account_id")
 
     @property
     @pulumi.getter(name="addressLines")
     def address_lines(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
         Address lines
@@ -767,14 +824,22 @@
     def name(self) -> pulumi.Output[str]:
         """
         Billing Group name
         """
         return pulumi.get(self, "name")
 
     @property
+    @pulumi.getter(name="parentId")
+    def parent_id(self) -> pulumi.Output[Optional[str]]:
+        """
+        An optional property to link a billing group to an already existing organization or account by using its ID. To set up proper dependencies please refer to this variable as a reference.
+        """
+        return pulumi.get(self, "parent_id")
+
+    @property
     @pulumi.getter
     def state(self) -> pulumi.Output[Optional[str]]:
         """
         State
         """
         return pulumi.get(self, "state")
```

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/cassandra.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/cassandra.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/cassandra_user.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/cassandra_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/clickhouse.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/clickhouse.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/clickhouse_database.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/clickhouse_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/clickhouse_grant.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/clickhouse_grant.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/clickhouse_role.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/clickhouse_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/clickhouse_user.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/clickhouse_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/config/vars.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/connection_pool.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/connection_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/flink.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/flink.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/flink_application.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/flink_application.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/flink_application_deployment.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/flink_application_deployment.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/flink_application_version.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/flink_application_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/gcp_vpc_peering_connection.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/gcp_vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_account.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_account_authentication.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_account_authentication.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_account_team.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_account_team.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_account_team_member.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_account_team_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_account_team_project.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_account_team_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_aws_privatelink.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_aws_privatelink.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_aws_vpc_peering_connection.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_aws_vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_azure_privatelink.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_azure_privatelink.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_azure_vpc_peering_connection.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_azure_vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_billing_group.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_billing_group.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ]
 
 @pulumi.output_type
 class GetBillingGroupResult:
     """
     A collection of values returned by getBillingGroup.
     """
-    def __init__(__self__, account_id=None, address_lines=None, billing_currency=None, billing_emails=None, billing_extra_text=None, billing_group_id=None, card_id=None, city=None, company=None, copy_from_billing_group=None, country_code=None, id=None, name=None, state=None, vat_id=None, zip_code=None):
+    def __init__(__self__, account_id=None, address_lines=None, billing_currency=None, billing_emails=None, billing_extra_text=None, billing_group_id=None, card_id=None, city=None, company=None, copy_from_billing_group=None, country_code=None, id=None, name=None, parent_id=None, state=None, vat_id=None, zip_code=None):
         if account_id and not isinstance(account_id, str):
             raise TypeError("Expected argument 'account_id' to be a str")
         pulumi.set(__self__, "account_id", account_id)
         if address_lines and not isinstance(address_lines, list):
             raise TypeError("Expected argument 'address_lines' to be a list")
         pulumi.set(__self__, "address_lines", address_lines)
         if billing_currency and not isinstance(billing_currency, str):
@@ -57,14 +57,17 @@
         pulumi.set(__self__, "country_code", country_code)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
         if name and not isinstance(name, str):
             raise TypeError("Expected argument 'name' to be a str")
         pulumi.set(__self__, "name", name)
+        if parent_id and not isinstance(parent_id, str):
+            raise TypeError("Expected argument 'parent_id' to be a str")
+        pulumi.set(__self__, "parent_id", parent_id)
         if state and not isinstance(state, str):
             raise TypeError("Expected argument 'state' to be a str")
         pulumi.set(__self__, "state", state)
         if vat_id and not isinstance(vat_id, str):
             raise TypeError("Expected argument 'vat_id' to be a str")
         pulumi.set(__self__, "vat_id", vat_id)
         if zip_code and not isinstance(zip_code, str):
@@ -172,14 +175,22 @@
     def name(self) -> str:
         """
         Billing Group name
         """
         return pulumi.get(self, "name")
 
     @property
+    @pulumi.getter(name="parentId")
+    def parent_id(self) -> str:
+        """
+        An optional property to link a billing group to an already existing organization or account by using its ID. To set up proper dependencies please refer to this variable as a reference.
+        """
+        return pulumi.get(self, "parent_id")
+
+    @property
     @pulumi.getter
     def state(self) -> str:
         """
         State
         """
         return pulumi.get(self, "state")
 
@@ -215,14 +226,15 @@
             card_id=self.card_id,
             city=self.city,
             company=self.company,
             copy_from_billing_group=self.copy_from_billing_group,
             country_code=self.country_code,
             id=self.id,
             name=self.name,
+            parent_id=self.parent_id,
             state=self.state,
             vat_id=self.vat_id,
             zip_code=self.zip_code)
 
 
 def get_billing_group(billing_group_id: Optional[str] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetBillingGroupResult:
@@ -247,14 +259,15 @@
         card_id=pulumi.get(__ret__, 'card_id'),
         city=pulumi.get(__ret__, 'city'),
         company=pulumi.get(__ret__, 'company'),
         copy_from_billing_group=pulumi.get(__ret__, 'copy_from_billing_group'),
         country_code=pulumi.get(__ret__, 'country_code'),
         id=pulumi.get(__ret__, 'id'),
         name=pulumi.get(__ret__, 'name'),
+        parent_id=pulumi.get(__ret__, 'parent_id'),
         state=pulumi.get(__ret__, 'state'),
         vat_id=pulumi.get(__ret__, 'vat_id'),
         zip_code=pulumi.get(__ret__, 'zip_code'))
 
 
 @_utilities.lift_output_func(get_billing_group)
 def get_billing_group_output(billing_group_id: Optional[pulumi.Input[str]] = None,
```

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_cassanda.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_cassanda.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_cassandra.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_cassandra.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_cassandra_user.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_cassandra_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_clickhouse.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_clickhouse.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_clickhouse_database.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_clickhouse_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_clickhouse_user.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_clickhouse_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_connection_pool.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_connection_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_flink.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_flink.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_flink_application.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_flink_application.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_flink_application_version.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_flink_application_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_gcp_vpc_peering_connection.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_gcp_vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_grafana.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_grafana.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_influx_db.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_influx_db.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_influxdb_database.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_influxdb_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_influxdb_user.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_influxdb_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_kafka.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_kafka.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_kafka_acl.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_kafka_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_kafka_connect.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_kafka_connect.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_kafka_connector.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_kafka_connector.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_kafka_mirror_maker.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_kafka_mirror_maker.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_kafka_schema.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_kafka_schema.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_kafka_schema_configuration.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_kafka_schema_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_kafka_schema_registry_acl.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_kafka_schema_registry_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_kafka_topic.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_kafka_topic.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_kafka_user.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_kafka_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_m3_aggregator.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_m3_aggregator.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_m3_db.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_m3_db.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_m3db_user.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_m3db_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_mirror_maker_replication_flow.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_mirror_maker_replication_flow.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_my_sql.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_my_sql.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_mysql_database.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_mysql_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_mysql_user.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_mysql_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_open_search.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_open_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,23 +196,23 @@
         """
         return pulumi.get(self, "maintenance_window_time")
 
     @property
     @pulumi.getter(name="opensearchUserConfigs")
     def opensearch_user_configs(self) -> Sequence['outputs.GetOpenSearchOpensearchUserConfigResult']:
         """
-        Opensearch user configurable settings
+        OpenSearch user configurable settings
         """
         return pulumi.get(self, "opensearch_user_configs")
 
     @property
     @pulumi.getter
     def opensearches(self) -> Sequence['outputs.GetOpenSearchOpensearchResult']:
         """
-        Opensearch server provided values
+        OpenSearch server provided values
         """
         return pulumi.get(self, "opensearches")
 
     @property
     @pulumi.getter
     def plan(self) -> str:
         """
@@ -369,15 +369,15 @@
             termination_protection=self.termination_protection)
 
 
 def get_open_search(project: Optional[str] = None,
                     service_name: Optional[str] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetOpenSearchResult:
     """
-    The Opensearch data source provides information about the existing Aiven Opensearch service.
+    The OpenSearch data source provides information about the existing Aiven OpenSearch service.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
@@ -427,15 +427,15 @@
 
 
 @_utilities.lift_output_func(get_open_search)
 def get_open_search_output(project: Optional[pulumi.Input[str]] = None,
                            service_name: Optional[pulumi.Input[str]] = None,
                            opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetOpenSearchResult]:
     """
-    The Opensearch data source provides information about the existing Aiven Opensearch service.
+    The OpenSearch data source provides information about the existing Aiven OpenSearch service.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
```

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_open_search_acl_config.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_open_search_acl_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,15 @@
             raise TypeError("Expected argument 'service_name' to be a str")
         pulumi.set(__self__, "service_name", service_name)
 
     @property
     @pulumi.getter
     def enabled(self) -> bool:
         """
-        Enable Opensearch ACLs. When disabled authenticated service users have unrestricted access. The default value is `true`.
+        Enable OpenSearch ACLs. When disabled authenticated service users have unrestricted access. The default value is `true`.
         """
         return pulumi.get(self, "enabled")
 
     @property
     @pulumi.getter(name="extendedAcl")
     def extended_acl(self) -> bool:
         """
@@ -92,15 +92,15 @@
             service_name=self.service_name)
 
 
 def get_open_search_acl_config(project: Optional[str] = None,
                                service_name: Optional[str] = None,
                                opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetOpenSearchAclConfigResult:
     """
-    The Opensearch ACL Config data source provides information about an existing Aiven Opensearch ACL Config.
+    The OpenSearch ACL Config data source provides information about an existing Aiven OpenSearch ACL Config.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
@@ -127,15 +127,15 @@
 
 
 @_utilities.lift_output_func(get_open_search_acl_config)
 def get_open_search_acl_config_output(project: Optional[pulumi.Input[str]] = None,
                                       service_name: Optional[pulumi.Input[str]] = None,
                                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetOpenSearchAclConfigResult]:
     """
-    The Opensearch ACL Config data source provides information about an existing Aiven Opensearch ACL Config.
+    The OpenSearch ACL Config data source provides information about an existing Aiven OpenSearch ACL Config.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
```

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_open_search_acl_rule.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_open_search_acl_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
 def get_open_search_acl_rule(index: Optional[str] = None,
                              permission: Optional[str] = None,
                              project: Optional[str] = None,
                              service_name: Optional[str] = None,
                              username: Optional[str] = None,
                              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetOpenSearchAclRuleResult:
     """
-    The Opensearch ACL Rule data source provides information about an existing Aiven Opensearch ACL Rule.
+    The OpenSearch ACL Rule data source provides information about an existing Aiven OpenSearch ACL Rule.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
@@ -154,15 +154,15 @@
 def get_open_search_acl_rule_output(index: Optional[pulumi.Input[str]] = None,
                                     permission: Optional[pulumi.Input[str]] = None,
                                     project: Optional[pulumi.Input[str]] = None,
                                     service_name: Optional[pulumi.Input[str]] = None,
                                     username: Optional[pulumi.Input[str]] = None,
                                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetOpenSearchAclRuleResult]:
     """
-    The Opensearch ACL Rule data source provides information about an existing Aiven Opensearch ACL Rule.
+    The OpenSearch ACL Rule data source provides information about an existing Aiven OpenSearch ACL Rule.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
```

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_opensearch_user.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_opensearch_user.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def password(self) -> str:
         """
-        The password of the Opensearch User.
+        The password of the OpenSearch User.
         """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def project(self) -> str:
         """
@@ -81,15 +81,15 @@
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def username(self) -> str:
         """
-        The actual name of the Opensearch User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
+        The actual name of the OpenSearch User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         """
         return pulumi.get(self, "username")
 
 
 class AwaitableGetOpensearchUserResult(GetOpensearchUserResult):
     # pylint: disable=using-constant-test
     def __await__(self):
@@ -105,15 +105,15 @@
 
 
 def get_opensearch_user(project: Optional[str] = None,
                         service_name: Optional[str] = None,
                         username: Optional[str] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetOpensearchUserResult:
     """
-    The Opensearch User data source provides information about the existing Aiven Cassandra User.
+    The OpenSearch User data source provides information about the existing Aiven OpenSearch User.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
@@ -121,15 +121,15 @@
         service_name="my-service",
         username="user1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
-    :param str username: The actual name of the Opensearch User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
+    :param str username: The actual name of the OpenSearch User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     """
     __args__ = dict()
     __args__['project'] = project
     __args__['serviceName'] = service_name
     __args__['username'] = username
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('aiven:index/getOpensearchUser:getOpensearchUser', __args__, opts=opts, typ=GetOpensearchUserResult).value
@@ -145,15 +145,15 @@
 
 @_utilities.lift_output_func(get_opensearch_user)
 def get_opensearch_user_output(project: Optional[pulumi.Input[str]] = None,
                                service_name: Optional[pulumi.Input[str]] = None,
                                username: Optional[pulumi.Input[str]] = None,
                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetOpensearchUserResult]:
     """
-    The Opensearch User data source provides information about the existing Aiven Cassandra User.
+    The OpenSearch User data source provides information about the existing Aiven OpenSearch User.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
@@ -161,10 +161,10 @@
         service_name="my-service",
         username="user1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
-    :param str username: The actual name of the Opensearch User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
+    :param str username: The actual name of the OpenSearch User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     """
     ...
```

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_organization.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_organization.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_organizational_unit.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_organizational_unit.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_pg.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_pg.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_pg_database.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_pg_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_pg_user.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_pg_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_project.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_project.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ]
 
 @pulumi.output_type
 class GetProjectResult:
     """
     A collection of values returned by getProject.
     """
-    def __init__(__self__, account_id=None, add_account_owners_admin_access=None, available_credits=None, billing_group=None, ca_cert=None, copy_from_project=None, default_cloud=None, estimated_balance=None, id=None, payment_method=None, project=None, tags=None, technical_emails=None, use_source_project_billing_group=None):
+    def __init__(__self__, account_id=None, add_account_owners_admin_access=None, available_credits=None, billing_group=None, ca_cert=None, copy_from_project=None, default_cloud=None, estimated_balance=None, id=None, parent_id=None, payment_method=None, project=None, tags=None, technical_emails=None, use_source_project_billing_group=None):
         if account_id and not isinstance(account_id, str):
             raise TypeError("Expected argument 'account_id' to be a str")
         pulumi.set(__self__, "account_id", account_id)
         if add_account_owners_admin_access and not isinstance(add_account_owners_admin_access, bool):
             raise TypeError("Expected argument 'add_account_owners_admin_access' to be a bool")
         pulumi.set(__self__, "add_account_owners_admin_access", add_account_owners_admin_access)
         if available_credits and not isinstance(available_credits, str):
@@ -46,14 +46,17 @@
         pulumi.set(__self__, "default_cloud", default_cloud)
         if estimated_balance and not isinstance(estimated_balance, str):
             raise TypeError("Expected argument 'estimated_balance' to be a str")
         pulumi.set(__self__, "estimated_balance", estimated_balance)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
+        if parent_id and not isinstance(parent_id, str):
+            raise TypeError("Expected argument 'parent_id' to be a str")
+        pulumi.set(__self__, "parent_id", parent_id)
         if payment_method and not isinstance(payment_method, str):
             raise TypeError("Expected argument 'payment_method' to be a str")
         pulumi.set(__self__, "payment_method", payment_method)
         if project and not isinstance(project, str):
             raise TypeError("Expected argument 'project' to be a str")
         pulumi.set(__self__, "project", project)
         if tags and not isinstance(tags, list):
@@ -66,23 +69,23 @@
             raise TypeError("Expected argument 'use_source_project_billing_group' to be a bool")
         pulumi.set(__self__, "use_source_project_billing_group", use_source_project_billing_group)
 
     @property
     @pulumi.getter(name="accountId")
     def account_id(self) -> str:
         """
-        An optional property to link a project to already an existing account by using account ID. To set up proper dependencies please refer to this variable as a reference.
+        An optional property to link a project to an already existing account by using account ID. To set up proper dependencies please refer to this variable as a reference.
         """
         return pulumi.get(self, "account_id")
 
     @property
     @pulumi.getter(name="addAccountOwnersAdminAccess")
     def add_account_owners_admin_access(self) -> bool:
         """
-        If account_id is set, grant account owner team admin access to the new project. The default value is `true`.
+        If parent_id is set, grant account owner team admin access to the new project. The default value is `true`.
         """
         return pulumi.get(self, "add_account_owners_admin_access")
 
     @property
     @pulumi.getter(name="availableCredits")
     def available_credits(self) -> str:
         """
@@ -135,14 +138,22 @@
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
+    @pulumi.getter(name="parentId")
+    def parent_id(self) -> str:
+        """
+        An optional property to link a project to an already existing organization or account by using its ID. To set up proper dependencies please refer to this variable as a reference.
+        """
+        return pulumi.get(self, "parent_id")
+
+    @property
     @pulumi.getter(name="paymentMethod")
     def payment_method(self) -> str:
         """
         The method of invoicing used for payments for this project, e.g. `card`.
         """
         return pulumi.get(self, "payment_method")
 
@@ -190,14 +201,15 @@
             available_credits=self.available_credits,
             billing_group=self.billing_group,
             ca_cert=self.ca_cert,
             copy_from_project=self.copy_from_project,
             default_cloud=self.default_cloud,
             estimated_balance=self.estimated_balance,
             id=self.id,
+            parent_id=self.parent_id,
             payment_method=self.payment_method,
             project=self.project,
             tags=self.tags,
             technical_emails=self.technical_emails,
             use_source_project_billing_group=self.use_source_project_billing_group)
 
 
@@ -229,14 +241,15 @@
         available_credits=pulumi.get(__ret__, 'available_credits'),
         billing_group=pulumi.get(__ret__, 'billing_group'),
         ca_cert=pulumi.get(__ret__, 'ca_cert'),
         copy_from_project=pulumi.get(__ret__, 'copy_from_project'),
         default_cloud=pulumi.get(__ret__, 'default_cloud'),
         estimated_balance=pulumi.get(__ret__, 'estimated_balance'),
         id=pulumi.get(__ret__, 'id'),
+        parent_id=pulumi.get(__ret__, 'parent_id'),
         payment_method=pulumi.get(__ret__, 'payment_method'),
         project=pulumi.get(__ret__, 'project'),
         tags=pulumi.get(__ret__, 'tags'),
         technical_emails=pulumi.get(__ret__, 'technical_emails'),
         use_source_project_billing_group=pulumi.get(__ret__, 'use_source_project_billing_group'))
```

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_project_user.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_project_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_project_vpc.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_project_vpc.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_redis.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_redis.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_redis_user.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_redis_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_service_component.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_service_component.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_service_integration.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_service_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_service_integration_endpoint.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_service_integration_endpoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,15 @@
         """
         return pulumi.get(self, "external_kafka_user_configs")
 
     @property
     @pulumi.getter(name="externalOpensearchLogsUserConfigs")
     def external_opensearch_logs_user_configs(self) -> Sequence['outputs.GetServiceIntegrationEndpointExternalOpensearchLogsUserConfigResult']:
         """
-        ExternalOpensearchLogs user configurable settings
+        ExternalOpenSearchLogs user configurable settings
         """
         return pulumi.get(self, "external_opensearch_logs_user_configs")
 
     @property
     @pulumi.getter(name="externalSchemaRegistryUserConfigs")
     def external_schema_registry_user_configs(self) -> Sequence['outputs.GetServiceIntegrationEndpointExternalSchemaRegistryUserConfigResult']:
         """
```

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/get_transit_gateway_vpc_attachment.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_transit_gateway_vpc_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/grafana.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/grafana.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/influx_db.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/influx_db.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/influxdb_database.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/influxdb_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/influxdb_user.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/influxdb_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/kafka.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/kafka.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/kafka_acl.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/kafka_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/kafka_connect.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/kafka_connect.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/kafka_connector.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/kafka_connector.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/kafka_mirror_maker.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/kafka_mirror_maker.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/kafka_schema.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/kafka_schema.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/kafka_schema_configuration.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/kafka_schema_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/kafka_schema_registry_acl.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/kafka_schema_registry_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/kafka_topic.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/kafka_topic.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/kafka_user.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/kafka_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/m3_aggregator.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/m3_aggregator.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/m3_db.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/m3_db.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/m3db_user.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/m3db_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/mirror_maker_replication_flow.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/mirror_maker_replication_flow.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/my_sql.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/my_sql.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/mysql_database.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/mysql_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/mysql_user.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/mysql_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/open_search.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/open_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         :param pulumi.Input[str] project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
         :param pulumi.Input[str] additional_disk_space: Additional disk space. Possible values depend on the service type, the cloud provider and the project. Therefore, reducing will result in the service rebalancing.
         :param pulumi.Input[str] cloud_name: Defines where the cloud provider and region where the service is hosted in. This can be changed freely after service is created. Changing the value will trigger a potentially lengthy migration process for the service. Format is cloud provider name (`aws`, `azure`, `do` `google`, `upcloud`, etc.), dash, and the cloud provider specific region name. These are documented on each Cloud provider's own support articles, like [here for Google](https://cloud.google.com/compute/docs/regions-zones/) and [here for AWS](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Concepts.RegionsAndAvailabilityZones.html).
         :param pulumi.Input[str] disk_space: Service disk space. Possible values depend on the service type, the cloud provider and the project. Therefore, reducing will result in the service rebalancing.
         :param pulumi.Input[str] maintenance_window_dow: Day of week when maintenance operations should be performed. One monday, tuesday, wednesday, etc.
         :param pulumi.Input[str] maintenance_window_time: Time of day when maintenance operations should be performed. UTC time in HH:mm:ss format.
-        :param pulumi.Input['OpenSearchOpensearchUserConfigArgs'] opensearch_user_config: Opensearch user configurable settings
+        :param pulumi.Input['OpenSearchOpensearchUserConfigArgs'] opensearch_user_config: OpenSearch user configurable settings
         :param pulumi.Input[str] plan: Defines what kind of computing resources are allocated for the service. It can be changed after creation, though there are some restrictions when going to a smaller plan such as the new plan must have sufficient amount of disk space to store all current data and switching to a plan with fewer nodes might not be supported. The basic plan names are `hobbyist`, `startup-x`, `business-x` and `premium-x` where `x` is (roughly) the amount of memory on each node (also other attributes like number of CPUs and amount of disk space varies but naming is based on memory). The available options can be seem from the [Aiven pricing page](https://aiven.io/pricing).
         :param pulumi.Input[str] project_vpc_id: Specifies the VPC the service should run in. If the value is not set the service is not run inside a VPC. When set, the value should be given as a reference to set up dependencies correctly and the VPC must be in the same cloud and region as the service itself. Project can be freely moved to and from VPC after creation but doing so triggers migration to new servers so the operation can take significant amount of time to complete if the service has a lot of data.
         :param pulumi.Input[Sequence[pulumi.Input['OpenSearchServiceIntegrationArgs']]] service_integrations: Service integrations to specify when creating a service. Not applied after initial service creation
         :param pulumi.Input[Sequence[pulumi.Input[str]]] static_ips: Static IPs that are going to be associated with this service. Please assign a value using the 'toset' function. Once a static ip resource is in the 'assigned' state it cannot be unbound from the node again
         :param pulumi.Input[Sequence[pulumi.Input['OpenSearchTagArgs']]] tags: Tags are key-value pairs that allow you to categorize services.
         :param pulumi.Input[bool] termination_protection: Prevents the service from being deleted. It is recommended to set this to `true` for all production services to prevent unintentional service deletion. This does not shield against deleting databases or topics but for services with backups much of the content can at least be restored from backup in case accidental deletion is done.
         """
@@ -164,15 +164,15 @@
     def maintenance_window_time(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "maintenance_window_time", value)
 
     @property
     @pulumi.getter(name="opensearchUserConfig")
     def opensearch_user_config(self) -> Optional[pulumi.Input['OpenSearchOpensearchUserConfigArgs']]:
         """
-        Opensearch user configurable settings
+        OpenSearch user configurable settings
         """
         return pulumi.get(self, "opensearch_user_config")
 
     @opensearch_user_config.setter
     def opensearch_user_config(self, value: Optional[pulumi.Input['OpenSearchOpensearchUserConfigArgs']]):
         pulumi.set(self, "opensearch_user_config", value)
 
@@ -287,16 +287,16 @@
         :param pulumi.Input[str] disk_space: Service disk space. Possible values depend on the service type, the cloud provider and the project. Therefore, reducing will result in the service rebalancing.
         :param pulumi.Input[str] disk_space_cap: The maximum disk space of the service, possible values depend on the service type, the cloud provider and the project.
         :param pulumi.Input[str] disk_space_default: The default disk space of the service, possible values depend on the service type, the cloud provider and the project. Its also the minimum value for `disk_space`
         :param pulumi.Input[str] disk_space_step: The default disk space step of the service, possible values depend on the service type, the cloud provider and the project. `disk_space` needs to increment from `disk_space_default` by increments of this size.
         :param pulumi.Input[str] disk_space_used: Disk space that service is currently using
         :param pulumi.Input[str] maintenance_window_dow: Day of week when maintenance operations should be performed. One monday, tuesday, wednesday, etc.
         :param pulumi.Input[str] maintenance_window_time: Time of day when maintenance operations should be performed. UTC time in HH:mm:ss format.
-        :param pulumi.Input['OpenSearchOpensearchUserConfigArgs'] opensearch_user_config: Opensearch user configurable settings
-        :param pulumi.Input[Sequence[pulumi.Input['OpenSearchOpensearchArgs']]] opensearches: Opensearch server provided values
+        :param pulumi.Input['OpenSearchOpensearchUserConfigArgs'] opensearch_user_config: OpenSearch user configurable settings
+        :param pulumi.Input[Sequence[pulumi.Input['OpenSearchOpensearchArgs']]] opensearches: OpenSearch server provided values
         :param pulumi.Input[str] plan: Defines what kind of computing resources are allocated for the service. It can be changed after creation, though there are some restrictions when going to a smaller plan such as the new plan must have sufficient amount of disk space to store all current data and switching to a plan with fewer nodes might not be supported. The basic plan names are `hobbyist`, `startup-x`, `business-x` and `premium-x` where `x` is (roughly) the amount of memory on each node (also other attributes like number of CPUs and amount of disk space varies but naming is based on memory). The available options can be seem from the [Aiven pricing page](https://aiven.io/pricing).
         :param pulumi.Input[str] project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] project_vpc_id: Specifies the VPC the service should run in. If the value is not set the service is not run inside a VPC. When set, the value should be given as a reference to set up dependencies correctly and the VPC must be in the same cloud and region as the service itself. Project can be freely moved to and from VPC after creation but doing so triggers migration to new servers so the operation can take significant amount of time to complete if the service has a lot of data.
         :param pulumi.Input[str] service_host: The hostname of the service.
         :param pulumi.Input[Sequence[pulumi.Input['OpenSearchServiceIntegrationArgs']]] service_integrations: Service integrations to specify when creating a service. Not applied after initial service creation
         :param pulumi.Input[str] service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
         :param pulumi.Input[str] service_password: Password used for connecting to the service, if applicable
@@ -490,27 +490,27 @@
     def maintenance_window_time(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "maintenance_window_time", value)
 
     @property
     @pulumi.getter(name="opensearchUserConfig")
     def opensearch_user_config(self) -> Optional[pulumi.Input['OpenSearchOpensearchUserConfigArgs']]:
         """
-        Opensearch user configurable settings
+        OpenSearch user configurable settings
         """
         return pulumi.get(self, "opensearch_user_config")
 
     @opensearch_user_config.setter
     def opensearch_user_config(self, value: Optional[pulumi.Input['OpenSearchOpensearchUserConfigArgs']]):
         pulumi.set(self, "opensearch_user_config", value)
 
     @property
     @pulumi.getter
     def opensearches(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['OpenSearchOpensearchArgs']]]]:
         """
-        Opensearch server provided values
+        OpenSearch server provided values
         """
         return pulumi.get(self, "opensearches")
 
     @opensearches.setter
     def opensearches(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['OpenSearchOpensearchArgs']]]]):
         pulumi.set(self, "opensearches", value)
 
@@ -712,15 +712,15 @@
                  service_integrations: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['OpenSearchServiceIntegrationArgs']]]]] = None,
                  service_name: Optional[pulumi.Input[str]] = None,
                  static_ips: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['OpenSearchTagArgs']]]]] = None,
                  termination_protection: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
-        The Opensearch resource allows the creation and management of Aiven Opensearch services.
+        The OpenSearch resource allows the creation and management of Aiven OpenSearch services.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_aiven as aiven
 
@@ -753,15 +753,15 @@
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] additional_disk_space: Additional disk space. Possible values depend on the service type, the cloud provider and the project. Therefore, reducing will result in the service rebalancing.
         :param pulumi.Input[str] cloud_name: Defines where the cloud provider and region where the service is hosted in. This can be changed freely after service is created. Changing the value will trigger a potentially lengthy migration process for the service. Format is cloud provider name (`aws`, `azure`, `do` `google`, `upcloud`, etc.), dash, and the cloud provider specific region name. These are documented on each Cloud provider's own support articles, like [here for Google](https://cloud.google.com/compute/docs/regions-zones/) and [here for AWS](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Concepts.RegionsAndAvailabilityZones.html).
         :param pulumi.Input[str] disk_space: Service disk space. Possible values depend on the service type, the cloud provider and the project. Therefore, reducing will result in the service rebalancing.
         :param pulumi.Input[str] maintenance_window_dow: Day of week when maintenance operations should be performed. One monday, tuesday, wednesday, etc.
         :param pulumi.Input[str] maintenance_window_time: Time of day when maintenance operations should be performed. UTC time in HH:mm:ss format.
-        :param pulumi.Input[pulumi.InputType['OpenSearchOpensearchUserConfigArgs']] opensearch_user_config: Opensearch user configurable settings
+        :param pulumi.Input[pulumi.InputType['OpenSearchOpensearchUserConfigArgs']] opensearch_user_config: OpenSearch user configurable settings
         :param pulumi.Input[str] plan: Defines what kind of computing resources are allocated for the service. It can be changed after creation, though there are some restrictions when going to a smaller plan such as the new plan must have sufficient amount of disk space to store all current data and switching to a plan with fewer nodes might not be supported. The basic plan names are `hobbyist`, `startup-x`, `business-x` and `premium-x` where `x` is (roughly) the amount of memory on each node (also other attributes like number of CPUs and amount of disk space varies but naming is based on memory). The available options can be seem from the [Aiven pricing page](https://aiven.io/pricing).
         :param pulumi.Input[str] project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] project_vpc_id: Specifies the VPC the service should run in. If the value is not set the service is not run inside a VPC. When set, the value should be given as a reference to set up dependencies correctly and the VPC must be in the same cloud and region as the service itself. Project can be freely moved to and from VPC after creation but doing so triggers migration to new servers so the operation can take significant amount of time to complete if the service has a lot of data.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['OpenSearchServiceIntegrationArgs']]]] service_integrations: Service integrations to specify when creating a service. Not applied after initial service creation
         :param pulumi.Input[str] service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] static_ips: Static IPs that are going to be associated with this service. Please assign a value using the 'toset' function. Once a static ip resource is in the 'assigned' state it cannot be unbound from the node again
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['OpenSearchTagArgs']]]] tags: Tags are key-value pairs that allow you to categorize services.
@@ -770,15 +770,15 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: OpenSearchArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        The Opensearch resource allows the creation and management of Aiven Opensearch services.
+        The OpenSearch resource allows the creation and management of Aiven OpenSearch services.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_aiven as aiven
 
@@ -932,16 +932,16 @@
         :param pulumi.Input[str] disk_space: Service disk space. Possible values depend on the service type, the cloud provider and the project. Therefore, reducing will result in the service rebalancing.
         :param pulumi.Input[str] disk_space_cap: The maximum disk space of the service, possible values depend on the service type, the cloud provider and the project.
         :param pulumi.Input[str] disk_space_default: The default disk space of the service, possible values depend on the service type, the cloud provider and the project. Its also the minimum value for `disk_space`
         :param pulumi.Input[str] disk_space_step: The default disk space step of the service, possible values depend on the service type, the cloud provider and the project. `disk_space` needs to increment from `disk_space_default` by increments of this size.
         :param pulumi.Input[str] disk_space_used: Disk space that service is currently using
         :param pulumi.Input[str] maintenance_window_dow: Day of week when maintenance operations should be performed. One monday, tuesday, wednesday, etc.
         :param pulumi.Input[str] maintenance_window_time: Time of day when maintenance operations should be performed. UTC time in HH:mm:ss format.
-        :param pulumi.Input[pulumi.InputType['OpenSearchOpensearchUserConfigArgs']] opensearch_user_config: Opensearch user configurable settings
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['OpenSearchOpensearchArgs']]]] opensearches: Opensearch server provided values
+        :param pulumi.Input[pulumi.InputType['OpenSearchOpensearchUserConfigArgs']] opensearch_user_config: OpenSearch user configurable settings
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['OpenSearchOpensearchArgs']]]] opensearches: OpenSearch server provided values
         :param pulumi.Input[str] plan: Defines what kind of computing resources are allocated for the service. It can be changed after creation, though there are some restrictions when going to a smaller plan such as the new plan must have sufficient amount of disk space to store all current data and switching to a plan with fewer nodes might not be supported. The basic plan names are `hobbyist`, `startup-x`, `business-x` and `premium-x` where `x` is (roughly) the amount of memory on each node (also other attributes like number of CPUs and amount of disk space varies but naming is based on memory). The available options can be seem from the [Aiven pricing page](https://aiven.io/pricing).
         :param pulumi.Input[str] project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] project_vpc_id: Specifies the VPC the service should run in. If the value is not set the service is not run inside a VPC. When set, the value should be given as a reference to set up dependencies correctly and the VPC must be in the same cloud and region as the service itself. Project can be freely moved to and from VPC after creation but doing so triggers migration to new servers so the operation can take significant amount of time to complete if the service has a lot of data.
         :param pulumi.Input[str] service_host: The hostname of the service.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['OpenSearchServiceIntegrationArgs']]]] service_integrations: Service integrations to specify when creating a service. Not applied after initial service creation
         :param pulumi.Input[str] service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
         :param pulumi.Input[str] service_password: Password used for connecting to the service, if applicable
@@ -1070,23 +1070,23 @@
         """
         return pulumi.get(self, "maintenance_window_time")
 
     @property
     @pulumi.getter(name="opensearchUserConfig")
     def opensearch_user_config(self) -> pulumi.Output[Optional['outputs.OpenSearchOpensearchUserConfig']]:
         """
-        Opensearch user configurable settings
+        OpenSearch user configurable settings
         """
         return pulumi.get(self, "opensearch_user_config")
 
     @property
     @pulumi.getter
     def opensearches(self) -> pulumi.Output[Sequence['outputs.OpenSearchOpensearch']]:
         """
-        Opensearch server provided values
+        OpenSearch server provided values
         """
         return pulumi.get(self, "opensearches")
 
     @property
     @pulumi.getter
     def plan(self) -> pulumi.Output[Optional[str]]:
         """
```

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/open_search_acl_config.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/open_search_acl_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
                  service_name: pulumi.Input[str],
                  enabled: Optional[pulumi.Input[bool]] = None,
                  extended_acl: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a OpenSearchAclConfig resource.
         :param pulumi.Input[str] project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
-        :param pulumi.Input[bool] enabled: Enable Opensearch ACLs. When disabled authenticated service users have unrestricted access. The default value is `true`.
+        :param pulumi.Input[bool] enabled: Enable OpenSearch ACLs. When disabled authenticated service users have unrestricted access. The default value is `true`.
         :param pulumi.Input[bool] extended_acl: Index rules can be applied in a limited fashion to the _mget, _msearch and _bulk APIs (and only those) by enabling the ExtendedAcl option for the service. When it is enabled, users can use these APIs as long as all operations only target indexes they have been granted access to. The default value is `true`.
         """
         pulumi.set(__self__, "project", project)
         pulumi.set(__self__, "service_name", service_name)
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
         if extended_acl is not None:
@@ -56,15 +56,15 @@
     def service_name(self, value: pulumi.Input[str]):
         pulumi.set(self, "service_name", value)
 
     @property
     @pulumi.getter
     def enabled(self) -> Optional[pulumi.Input[bool]]:
         """
-        Enable Opensearch ACLs. When disabled authenticated service users have unrestricted access. The default value is `true`.
+        Enable OpenSearch ACLs. When disabled authenticated service users have unrestricted access. The default value is `true`.
         """
         return pulumi.get(self, "enabled")
 
     @enabled.setter
     def enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enabled", value)
 
@@ -86,15 +86,15 @@
     def __init__(__self__, *,
                  enabled: Optional[pulumi.Input[bool]] = None,
                  extended_acl: Optional[pulumi.Input[bool]] = None,
                  project: Optional[pulumi.Input[str]] = None,
                  service_name: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering OpenSearchAclConfig resources.
-        :param pulumi.Input[bool] enabled: Enable Opensearch ACLs. When disabled authenticated service users have unrestricted access. The default value is `true`.
+        :param pulumi.Input[bool] enabled: Enable OpenSearch ACLs. When disabled authenticated service users have unrestricted access. The default value is `true`.
         :param pulumi.Input[bool] extended_acl: Index rules can be applied in a limited fashion to the _mget, _msearch and _bulk APIs (and only those) by enabling the ExtendedAcl option for the service. When it is enabled, users can use these APIs as long as all operations only target indexes they have been granted access to. The default value is `true`.
         :param pulumi.Input[str] project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         """
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
         if extended_acl is not None:
@@ -104,15 +104,15 @@
         if service_name is not None:
             pulumi.set(__self__, "service_name", service_name)
 
     @property
     @pulumi.getter
     def enabled(self) -> Optional[pulumi.Input[bool]]:
         """
-        Enable Opensearch ACLs. When disabled authenticated service users have unrestricted access. The default value is `true`.
+        Enable OpenSearch ACLs. When disabled authenticated service users have unrestricted access. The default value is `true`.
         """
         return pulumi.get(self, "enabled")
 
     @enabled.setter
     def enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enabled", value)
 
@@ -160,15 +160,15 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  enabled: Optional[pulumi.Input[bool]] = None,
                  extended_acl: Optional[pulumi.Input[bool]] = None,
                  project: Optional[pulumi.Input[str]] = None,
                  service_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        The Opensearch resource allows the creation and management of Aiven Opensearch services.
+        The OpenSearch resource allows the creation and management of Aiven OpenSearch services.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_aiven as aiven
 
@@ -195,27 +195,27 @@
 
         ```sh
          $ pulumi import aiven:index/openSearchAclConfig:OpenSearchAclConfig foo project/service_name
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[bool] enabled: Enable Opensearch ACLs. When disabled authenticated service users have unrestricted access. The default value is `true`.
+        :param pulumi.Input[bool] enabled: Enable OpenSearch ACLs. When disabled authenticated service users have unrestricted access. The default value is `true`.
         :param pulumi.Input[bool] extended_acl: Index rules can be applied in a limited fashion to the _mget, _msearch and _bulk APIs (and only those) by enabling the ExtendedAcl option for the service. When it is enabled, users can use these APIs as long as all operations only target indexes they have been granted access to. The default value is `true`.
         :param pulumi.Input[str] project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: OpenSearchAclConfigArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        The Opensearch resource allows the creation and management of Aiven Opensearch services.
+        The OpenSearch resource allows the creation and management of Aiven OpenSearch services.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_aiven as aiven
 
@@ -297,15 +297,15 @@
         """
         Get an existing OpenSearchAclConfig resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[bool] enabled: Enable Opensearch ACLs. When disabled authenticated service users have unrestricted access. The default value is `true`.
+        :param pulumi.Input[bool] enabled: Enable OpenSearch ACLs. When disabled authenticated service users have unrestricted access. The default value is `true`.
         :param pulumi.Input[bool] extended_acl: Index rules can be applied in a limited fashion to the _mget, _msearch and _bulk APIs (and only those) by enabling the ExtendedAcl option for the service. When it is enabled, users can use these APIs as long as all operations only target indexes they have been granted access to. The default value is `true`.
         :param pulumi.Input[str] project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _OpenSearchAclConfigState.__new__(_OpenSearchAclConfigState)
@@ -316,15 +316,15 @@
         __props__.__dict__["service_name"] = service_name
         return OpenSearchAclConfig(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def enabled(self) -> pulumi.Output[Optional[bool]]:
         """
-        Enable Opensearch ACLs. When disabled authenticated service users have unrestricted access. The default value is `true`.
+        Enable OpenSearch ACLs. When disabled authenticated service users have unrestricted access. The default value is `true`.
         """
         return pulumi.get(self, "enabled")
 
     @property
     @pulumi.getter(name="extendedAcl")
     def extended_acl(self) -> pulumi.Output[Optional[bool]]:
         """
```

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/open_search_acl_rule.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/open_search_acl_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,15 +190,15 @@
                  index: Optional[pulumi.Input[str]] = None,
                  permission: Optional[pulumi.Input[str]] = None,
                  project: Optional[pulumi.Input[str]] = None,
                  service_name: Optional[pulumi.Input[str]] = None,
                  username: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        The Opensearch ACL Rule resource models a single ACL Rule for an Aiven Opensearch service.
+        The OpenSearch ACL Rule resource models a single ACL Rule for an Aiven OpenSearch service.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_aiven as aiven
 
@@ -272,15 +272,15 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: OpenSearchAclRuleArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        The Opensearch ACL Rule resource models a single ACL Rule for an Aiven Opensearch service.
+        The OpenSearch ACL Rule resource models a single ACL Rule for an Aiven OpenSearch service.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_aiven as aiven
```

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/opensearch_user.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/opensearch_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,16 @@
                  service_name: pulumi.Input[str],
                  username: pulumi.Input[str],
                  password: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a OpensearchUser resource.
         :param pulumi.Input[str] project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
-        :param pulumi.Input[str] username: The actual name of the Opensearch User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
-        :param pulumi.Input[str] password: The password of the Opensearch User.
+        :param pulumi.Input[str] username: The actual name of the OpenSearch User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
+        :param pulumi.Input[str] password: The password of the OpenSearch User.
         """
         pulumi.set(__self__, "project", project)
         pulumi.set(__self__, "service_name", service_name)
         pulumi.set(__self__, "username", username)
         if password is not None:
             pulumi.set(__self__, "password", password)
 
@@ -55,27 +55,27 @@
     def service_name(self, value: pulumi.Input[str]):
         pulumi.set(self, "service_name", value)
 
     @property
     @pulumi.getter
     def username(self) -> pulumi.Input[str]:
         """
-        The actual name of the Opensearch User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
+        The actual name of the OpenSearch User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         """
         return pulumi.get(self, "username")
 
     @username.setter
     def username(self, value: pulumi.Input[str]):
         pulumi.set(self, "username", value)
 
     @property
     @pulumi.getter
     def password(self) -> Optional[pulumi.Input[str]]:
         """
-        The password of the Opensearch User.
+        The password of the OpenSearch User.
         """
         return pulumi.get(self, "password")
 
     @password.setter
     def password(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "password", value)
 
@@ -86,19 +86,19 @@
                  password: Optional[pulumi.Input[str]] = None,
                  project: Optional[pulumi.Input[str]] = None,
                  service_name: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering OpensearchUser resources.
-        :param pulumi.Input[str] password: The password of the Opensearch User.
+        :param pulumi.Input[str] password: The password of the OpenSearch User.
         :param pulumi.Input[str] project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] type: Type of the user account. Tells whether the user is the primary account or a regular account.
-        :param pulumi.Input[str] username: The actual name of the Opensearch User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
+        :param pulumi.Input[str] username: The actual name of the OpenSearch User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         """
         if password is not None:
             pulumi.set(__self__, "password", password)
         if project is not None:
             pulumi.set(__self__, "project", project)
         if service_name is not None:
             pulumi.set(__self__, "service_name", service_name)
@@ -107,15 +107,15 @@
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def password(self) -> Optional[pulumi.Input[str]]:
         """
-        The password of the Opensearch User.
+        The password of the OpenSearch User.
         """
         return pulumi.get(self, "password")
 
     @password.setter
     def password(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "password", value)
 
@@ -155,15 +155,15 @@
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter
     def username(self) -> Optional[pulumi.Input[str]]:
         """
-        The actual name of the Opensearch User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
+        The actual name of the OpenSearch User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         """
         return pulumi.get(self, "username")
 
     @username.setter
     def username(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "username", value)
 
@@ -175,15 +175,15 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  password: Optional[pulumi.Input[str]] = None,
                  project: Optional[pulumi.Input[str]] = None,
                  service_name: Optional[pulumi.Input[str]] = None,
                  username: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        The Opensearch User resource allows the creation and management of Aiven Opensearch Users.
+        The OpenSearch User resource allows the creation and management of Aiven OpenSearch Users.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_aiven as aiven
 
@@ -198,27 +198,27 @@
 
         ```sh
          $ pulumi import aiven:index/opensearchUser:OpensearchUser foo project/service_name/username
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] password: The password of the Opensearch User.
+        :param pulumi.Input[str] password: The password of the OpenSearch User.
         :param pulumi.Input[str] project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
-        :param pulumi.Input[str] username: The actual name of the Opensearch User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
+        :param pulumi.Input[str] username: The actual name of the OpenSearch User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: OpensearchUserArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        The Opensearch User resource allows the creation and management of Aiven Opensearch Users.
+        The OpenSearch User resource allows the creation and management of Aiven OpenSearch Users.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_aiven as aiven
 
@@ -294,19 +294,19 @@
         """
         Get an existing OpensearchUser resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] password: The password of the Opensearch User.
+        :param pulumi.Input[str] password: The password of the OpenSearch User.
         :param pulumi.Input[str] project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] type: Type of the user account. Tells whether the user is the primary account or a regular account.
-        :param pulumi.Input[str] username: The actual name of the Opensearch User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
+        :param pulumi.Input[str] username: The actual name of the OpenSearch User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _OpensearchUserState.__new__(_OpensearchUserState)
 
         __props__.__dict__["password"] = password
         __props__.__dict__["project"] = project
@@ -315,15 +315,15 @@
         __props__.__dict__["username"] = username
         return OpensearchUser(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def password(self) -> pulumi.Output[str]:
         """
-        The password of the Opensearch User.
+        The password of the OpenSearch User.
         """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def project(self) -> pulumi.Output[str]:
         """
@@ -347,11 +347,11 @@
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def username(self) -> pulumi.Output[str]:
         """
-        The actual name of the Opensearch User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
+        The actual name of the OpenSearch User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         """
         return pulumi.get(self, "username")
```

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/organization.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/organization.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/organizational_unit.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/organizational_unit.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/outputs.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,17 @@
     'CassandraCassandraUserConfigPublicAccess',
     'CassandraComponent',
     'CassandraServiceIntegration',
     'CassandraTag',
     'ClickhouseClickhouse',
     'ClickhouseClickhouseUserConfig',
     'ClickhouseClickhouseUserConfigIpFilterObject',
+    'ClickhouseClickhouseUserConfigPrivateAccess',
+    'ClickhouseClickhouseUserConfigPrivatelinkAccess',
+    'ClickhouseClickhouseUserConfigPublicAccess',
     'ClickhouseComponent',
     'ClickhouseGrantPrivilegeGrant',
     'ClickhouseGrantRoleGrant',
     'ClickhouseServiceIntegration',
     'ClickhouseTag',
     'FlinkApplicationVersionSink',
     'FlinkApplicationVersionSource',
@@ -225,14 +228,17 @@
     'GetCassandraCassandraUserConfigPublicAccessResult',
     'GetCassandraComponentResult',
     'GetCassandraServiceIntegrationResult',
     'GetCassandraTagResult',
     'GetClickhouseClickhouseResult',
     'GetClickhouseClickhouseUserConfigResult',
     'GetClickhouseClickhouseUserConfigIpFilterObjectResult',
+    'GetClickhouseClickhouseUserConfigPrivateAccessResult',
+    'GetClickhouseClickhouseUserConfigPrivatelinkAccessResult',
+    'GetClickhouseClickhouseUserConfigPublicAccessResult',
     'GetClickhouseComponentResult',
     'GetClickhouseServiceIntegrationResult',
     'GetClickhouseTagResult',
     'GetFlinkApplicationVersionSinkResult',
     'GetFlinkApplicationVersionSourceResult',
     'GetFlinkComponentResult',
     'GetFlinkFlinkResult',
@@ -1003,18 +1009,26 @@
             suggest = "additional_backup_regions"
         elif key == "ipFilterObjects":
             suggest = "ip_filter_objects"
         elif key == "ipFilterStrings":
             suggest = "ip_filter_strings"
         elif key == "ipFilters":
             suggest = "ip_filters"
+        elif key == "privateAccess":
+            suggest = "private_access"
+        elif key == "privatelinkAccess":
+            suggest = "privatelink_access"
         elif key == "projectToForkFrom":
             suggest = "project_to_fork_from"
+        elif key == "publicAccess":
+            suggest = "public_access"
         elif key == "serviceToForkFrom":
             suggest = "service_to_fork_from"
+        elif key == "staticIps":
+            suggest = "static_ips"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in ClickhouseClickhouseUserConfig. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
         ClickhouseClickhouseUserConfig.__key_warning(key)
         return super().__getitem__(key)
@@ -1024,36 +1038,52 @@
         return super().get(key, default)
 
     def __init__(__self__, *,
                  additional_backup_regions: Optional[str] = None,
                  ip_filter_objects: Optional[Sequence['outputs.ClickhouseClickhouseUserConfigIpFilterObject']] = None,
                  ip_filter_strings: Optional[Sequence[str]] = None,
                  ip_filters: Optional[Sequence[str]] = None,
+                 private_access: Optional['outputs.ClickhouseClickhouseUserConfigPrivateAccess'] = None,
+                 privatelink_access: Optional['outputs.ClickhouseClickhouseUserConfigPrivatelinkAccess'] = None,
                  project_to_fork_from: Optional[str] = None,
-                 service_to_fork_from: Optional[str] = None):
+                 public_access: Optional['outputs.ClickhouseClickhouseUserConfigPublicAccess'] = None,
+                 service_to_fork_from: Optional[str] = None,
+                 static_ips: Optional[bool] = None):
         """
         :param str additional_backup_regions: Additional Cloud Regions for Backup Replication.
         :param Sequence['ClickhouseClickhouseUserConfigIpFilterObjectArgs'] ip_filter_objects: Allow incoming connections from CIDR address block, e.g. '10.20.0.0/16'.
         :param Sequence[str] ip_filter_strings: Allow incoming connections from CIDR address block, e.g. '10.20.0.0/16'.
         :param Sequence[str] ip_filters: Allow incoming connections from CIDR address block, e.g. '10.20.0.0/16'.
+        :param 'ClickhouseClickhouseUserConfigPrivateAccessArgs' private_access: Allow access to selected service ports from private networks.
+        :param 'ClickhouseClickhouseUserConfigPrivatelinkAccessArgs' privatelink_access: Allow access to selected service components through Privatelink.
         :param str project_to_fork_from: Name of another project to fork a service from. This has effect only when a new service is being created.
+        :param 'ClickhouseClickhouseUserConfigPublicAccessArgs' public_access: Allow access to selected service ports from the public Internet.
         :param str service_to_fork_from: Name of another service to fork from. This has effect only when a new service is being created.
+        :param bool static_ips: Use static public IP addresses.
         """
         if additional_backup_regions is not None:
             pulumi.set(__self__, "additional_backup_regions", additional_backup_regions)
         if ip_filter_objects is not None:
             pulumi.set(__self__, "ip_filter_objects", ip_filter_objects)
         if ip_filter_strings is not None:
             pulumi.set(__self__, "ip_filter_strings", ip_filter_strings)
         if ip_filters is not None:
             pulumi.set(__self__, "ip_filters", ip_filters)
+        if private_access is not None:
+            pulumi.set(__self__, "private_access", private_access)
+        if privatelink_access is not None:
+            pulumi.set(__self__, "privatelink_access", privatelink_access)
         if project_to_fork_from is not None:
             pulumi.set(__self__, "project_to_fork_from", project_to_fork_from)
+        if public_access is not None:
+            pulumi.set(__self__, "public_access", public_access)
         if service_to_fork_from is not None:
             pulumi.set(__self__, "service_to_fork_from", service_to_fork_from)
+        if static_ips is not None:
+            pulumi.set(__self__, "static_ips", static_ips)
 
     @property
     @pulumi.getter(name="additionalBackupRegions")
     def additional_backup_regions(self) -> Optional[str]:
         """
         Additional Cloud Regions for Backup Replication.
         """
@@ -1083,29 +1113,61 @@
         """
         warnings.warn("""This will be removed in v5.0.0 and replaced with ip_filter_string instead.""", DeprecationWarning)
         pulumi.log.warn("""ip_filters is deprecated: This will be removed in v5.0.0 and replaced with ip_filter_string instead.""")
 
         return pulumi.get(self, "ip_filters")
 
     @property
+    @pulumi.getter(name="privateAccess")
+    def private_access(self) -> Optional['outputs.ClickhouseClickhouseUserConfigPrivateAccess']:
+        """
+        Allow access to selected service ports from private networks.
+        """
+        return pulumi.get(self, "private_access")
+
+    @property
+    @pulumi.getter(name="privatelinkAccess")
+    def privatelink_access(self) -> Optional['outputs.ClickhouseClickhouseUserConfigPrivatelinkAccess']:
+        """
+        Allow access to selected service components through Privatelink.
+        """
+        return pulumi.get(self, "privatelink_access")
+
+    @property
     @pulumi.getter(name="projectToForkFrom")
     def project_to_fork_from(self) -> Optional[str]:
         """
         Name of another project to fork a service from. This has effect only when a new service is being created.
         """
         return pulumi.get(self, "project_to_fork_from")
 
     @property
+    @pulumi.getter(name="publicAccess")
+    def public_access(self) -> Optional['outputs.ClickhouseClickhouseUserConfigPublicAccess']:
+        """
+        Allow access to selected service ports from the public Internet.
+        """
+        return pulumi.get(self, "public_access")
+
+    @property
     @pulumi.getter(name="serviceToForkFrom")
     def service_to_fork_from(self) -> Optional[str]:
         """
         Name of another service to fork from. This has effect only when a new service is being created.
         """
         return pulumi.get(self, "service_to_fork_from")
 
+    @property
+    @pulumi.getter(name="staticIps")
+    def static_ips(self) -> Optional[bool]:
+        """
+        Use static public IP addresses.
+        """
+        return pulumi.get(self, "static_ips")
+
 
 @pulumi.output_type
 class ClickhouseClickhouseUserConfigIpFilterObject(dict):
     def __init__(__self__, *,
                  network: str,
                  description: Optional[str] = None):
         pulumi.set(__self__, "network", network)
@@ -1120,14 +1182,170 @@
     @property
     @pulumi.getter
     def description(self) -> Optional[str]:
         return pulumi.get(self, "description")
 
 
 @pulumi.output_type
+class ClickhouseClickhouseUserConfigPrivateAccess(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "clickhouseHttps":
+            suggest = "clickhouse_https"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ClickhouseClickhouseUserConfigPrivateAccess. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ClickhouseClickhouseUserConfigPrivateAccess.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ClickhouseClickhouseUserConfigPrivateAccess.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 clickhouse: Optional[bool] = None,
+                 clickhouse_https: Optional[bool] = None,
+                 prometheus: Optional[bool] = None):
+        """
+        :param bool clickhouse: Clickhouse server provided values
+        """
+        if clickhouse is not None:
+            pulumi.set(__self__, "clickhouse", clickhouse)
+        if clickhouse_https is not None:
+            pulumi.set(__self__, "clickhouse_https", clickhouse_https)
+        if prometheus is not None:
+            pulumi.set(__self__, "prometheus", prometheus)
+
+    @property
+    @pulumi.getter
+    def clickhouse(self) -> Optional[bool]:
+        """
+        Clickhouse server provided values
+        """
+        return pulumi.get(self, "clickhouse")
+
+    @property
+    @pulumi.getter(name="clickhouseHttps")
+    def clickhouse_https(self) -> Optional[bool]:
+        return pulumi.get(self, "clickhouse_https")
+
+    @property
+    @pulumi.getter
+    def prometheus(self) -> Optional[bool]:
+        return pulumi.get(self, "prometheus")
+
+
+@pulumi.output_type
+class ClickhouseClickhouseUserConfigPrivatelinkAccess(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "clickhouseHttps":
+            suggest = "clickhouse_https"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ClickhouseClickhouseUserConfigPrivatelinkAccess. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ClickhouseClickhouseUserConfigPrivatelinkAccess.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ClickhouseClickhouseUserConfigPrivatelinkAccess.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 clickhouse: Optional[bool] = None,
+                 clickhouse_https: Optional[bool] = None,
+                 prometheus: Optional[bool] = None):
+        """
+        :param bool clickhouse: Clickhouse server provided values
+        """
+        if clickhouse is not None:
+            pulumi.set(__self__, "clickhouse", clickhouse)
+        if clickhouse_https is not None:
+            pulumi.set(__self__, "clickhouse_https", clickhouse_https)
+        if prometheus is not None:
+            pulumi.set(__self__, "prometheus", prometheus)
+
+    @property
+    @pulumi.getter
+    def clickhouse(self) -> Optional[bool]:
+        """
+        Clickhouse server provided values
+        """
+        return pulumi.get(self, "clickhouse")
+
+    @property
+    @pulumi.getter(name="clickhouseHttps")
+    def clickhouse_https(self) -> Optional[bool]:
+        return pulumi.get(self, "clickhouse_https")
+
+    @property
+    @pulumi.getter
+    def prometheus(self) -> Optional[bool]:
+        return pulumi.get(self, "prometheus")
+
+
+@pulumi.output_type
+class ClickhouseClickhouseUserConfigPublicAccess(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "clickhouseHttps":
+            suggest = "clickhouse_https"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ClickhouseClickhouseUserConfigPublicAccess. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ClickhouseClickhouseUserConfigPublicAccess.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ClickhouseClickhouseUserConfigPublicAccess.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 clickhouse: Optional[bool] = None,
+                 clickhouse_https: Optional[bool] = None,
+                 prometheus: Optional[bool] = None):
+        """
+        :param bool clickhouse: Clickhouse server provided values
+        """
+        if clickhouse is not None:
+            pulumi.set(__self__, "clickhouse", clickhouse)
+        if clickhouse_https is not None:
+            pulumi.set(__self__, "clickhouse_https", clickhouse_https)
+        if prometheus is not None:
+            pulumi.set(__self__, "prometheus", prometheus)
+
+    @property
+    @pulumi.getter
+    def clickhouse(self) -> Optional[bool]:
+        """
+        Clickhouse server provided values
+        """
+        return pulumi.get(self, "clickhouse")
+
+    @property
+    @pulumi.getter(name="clickhouseHttps")
+    def clickhouse_https(self) -> Optional[bool]:
+        return pulumi.get(self, "clickhouse_https")
+
+    @property
+    @pulumi.getter
+    def prometheus(self) -> Optional[bool]:
+        return pulumi.get(self, "prometheus")
+
+
+@pulumi.output_type
 class ClickhouseComponent(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "kafkaAuthenticationMethod":
             suggest = "kafka_authentication_method"
 
@@ -3416,14 +3634,16 @@
             suggest = "max_connection_limit"
         elif key == "maxRowLimit":
             suggest = "max_row_limit"
         elif key == "maxSelectBuckets":
             suggest = "max_select_buckets"
         elif key == "maxSelectPoint":
             suggest = "max_select_point"
+        elif key == "queryLogEnabled":
+            suggest = "query_log_enabled"
         elif key == "queryTimeout":
             suggest = "query_timeout"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in InfluxDbInfluxdbUserConfigInfluxdb. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
@@ -3436,25 +3656,28 @@
 
     def __init__(__self__, *,
                  log_queries_after: Optional[int] = None,
                  max_connection_limit: Optional[int] = None,
                  max_row_limit: Optional[int] = None,
                  max_select_buckets: Optional[int] = None,
                  max_select_point: Optional[int] = None,
+                 query_log_enabled: Optional[bool] = None,
                  query_timeout: Optional[int] = None):
         if log_queries_after is not None:
             pulumi.set(__self__, "log_queries_after", log_queries_after)
         if max_connection_limit is not None:
             pulumi.set(__self__, "max_connection_limit", max_connection_limit)
         if max_row_limit is not None:
             pulumi.set(__self__, "max_row_limit", max_row_limit)
         if max_select_buckets is not None:
             pulumi.set(__self__, "max_select_buckets", max_select_buckets)
         if max_select_point is not None:
             pulumi.set(__self__, "max_select_point", max_select_point)
+        if query_log_enabled is not None:
+            pulumi.set(__self__, "query_log_enabled", query_log_enabled)
         if query_timeout is not None:
             pulumi.set(__self__, "query_timeout", query_timeout)
 
     @property
     @pulumi.getter(name="logQueriesAfter")
     def log_queries_after(self) -> Optional[int]:
         return pulumi.get(self, "log_queries_after")
@@ -3476,14 +3699,19 @@
 
     @property
     @pulumi.getter(name="maxSelectPoint")
     def max_select_point(self) -> Optional[int]:
         return pulumi.get(self, "max_select_point")
 
     @property
+    @pulumi.getter(name="queryLogEnabled")
+    def query_log_enabled(self) -> Optional[bool]:
+        return pulumi.get(self, "query_log_enabled")
+
+    @property
     @pulumi.getter(name="queryTimeout")
     def query_timeout(self) -> Optional[int]:
         return pulumi.get(self, "query_timeout")
 
 
 @pulumi.output_type
 class InfluxDbInfluxdbUserConfigIpFilterObject(dict):
@@ -9368,28 +9596,28 @@
         return super().get(key, default)
 
     def __init__(__self__, *,
                  opensearch: Optional[bool] = None,
                  opensearch_dashboards: Optional[bool] = None,
                  prometheus: Optional[bool] = None):
         """
-        :param bool opensearch: Opensearch server provided values
+        :param bool opensearch: OpenSearch server provided values
         """
         if opensearch is not None:
             pulumi.set(__self__, "opensearch", opensearch)
         if opensearch_dashboards is not None:
             pulumi.set(__self__, "opensearch_dashboards", opensearch_dashboards)
         if prometheus is not None:
             pulumi.set(__self__, "prometheus", prometheus)
 
     @property
     @pulumi.getter
     def opensearch(self) -> Optional[bool]:
         """
-        Opensearch server provided values
+        OpenSearch server provided values
         """
         return pulumi.get(self, "opensearch")
 
     @property
     @pulumi.getter(name="opensearchDashboards")
     def opensearch_dashboards(self) -> Optional[bool]:
         return pulumi.get(self, "opensearch_dashboards")
@@ -9420,28 +9648,28 @@
         return super().get(key, default)
 
     def __init__(__self__, *,
                  opensearch: Optional[bool] = None,
                  opensearch_dashboards: Optional[bool] = None,
                  prometheus: Optional[bool] = None):
         """
-        :param bool opensearch: Opensearch server provided values
+        :param bool opensearch: OpenSearch server provided values
         """
         if opensearch is not None:
             pulumi.set(__self__, "opensearch", opensearch)
         if opensearch_dashboards is not None:
             pulumi.set(__self__, "opensearch_dashboards", opensearch_dashboards)
         if prometheus is not None:
             pulumi.set(__self__, "prometheus", prometheus)
 
     @property
     @pulumi.getter
     def opensearch(self) -> Optional[bool]:
         """
-        Opensearch server provided values
+        OpenSearch server provided values
         """
         return pulumi.get(self, "opensearch")
 
     @property
     @pulumi.getter(name="opensearchDashboards")
     def opensearch_dashboards(self) -> Optional[bool]:
         return pulumi.get(self, "opensearch_dashboards")
@@ -9472,28 +9700,28 @@
         return super().get(key, default)
 
     def __init__(__self__, *,
                  opensearch: Optional[bool] = None,
                  opensearch_dashboards: Optional[bool] = None,
                  prometheus: Optional[bool] = None):
         """
-        :param bool opensearch: Opensearch server provided values
+        :param bool opensearch: OpenSearch server provided values
         """
         if opensearch is not None:
             pulumi.set(__self__, "opensearch", opensearch)
         if opensearch_dashboards is not None:
             pulumi.set(__self__, "opensearch_dashboards", opensearch_dashboards)
         if prometheus is not None:
             pulumi.set(__self__, "prometheus", prometheus)
 
     @property
     @pulumi.getter
     def opensearch(self) -> Optional[bool]:
         """
-        Opensearch server provided values
+        OpenSearch server provided values
         """
         return pulumi.get(self, "opensearch")
 
     @property
     @pulumi.getter(name="opensearchDashboards")
     def opensearch_dashboards(self) -> Optional[bool]:
         return pulumi.get(self, "opensearch_dashboards")
@@ -11876,14 +12104,30 @@
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "dataFormat":
             suggest = "data_format"
         elif key == "groupName":
             suggest = "group_name"
+        elif key == "autoOffsetReset":
+            suggest = "auto_offset_reset"
+        elif key == "dateTimeInputFormat":
+            suggest = "date_time_input_format"
+        elif key == "handleErrorMode":
+            suggest = "handle_error_mode"
+        elif key == "maxBlockSize":
+            suggest = "max_block_size"
+        elif key == "maxRowsPerMessage":
+            suggest = "max_rows_per_message"
+        elif key == "numConsumers":
+            suggest = "num_consumers"
+        elif key == "pollMaxBatchSize":
+            suggest = "poll_max_batch_size"
+        elif key == "skipBrokenMessages":
+            suggest = "skip_broken_messages"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in ServiceIntegrationClickhouseKafkaUserConfigTable. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
         ServiceIntegrationClickhouseKafkaUserConfigTable.__key_warning(key)
         return super().__getitem__(key)
@@ -11892,21 +12136,45 @@
         ServiceIntegrationClickhouseKafkaUserConfigTable.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  data_format: str,
                  group_name: str,
                  name: str,
+                 auto_offset_reset: Optional[str] = None,
                  columns: Optional[Sequence['outputs.ServiceIntegrationClickhouseKafkaUserConfigTableColumn']] = None,
+                 date_time_input_format: Optional[str] = None,
+                 handle_error_mode: Optional[str] = None,
+                 max_block_size: Optional[int] = None,
+                 max_rows_per_message: Optional[int] = None,
+                 num_consumers: Optional[int] = None,
+                 poll_max_batch_size: Optional[int] = None,
+                 skip_broken_messages: Optional[int] = None,
                  topics: Optional[Sequence['outputs.ServiceIntegrationClickhouseKafkaUserConfigTableTopic']] = None):
         pulumi.set(__self__, "data_format", data_format)
         pulumi.set(__self__, "group_name", group_name)
         pulumi.set(__self__, "name", name)
+        if auto_offset_reset is not None:
+            pulumi.set(__self__, "auto_offset_reset", auto_offset_reset)
         if columns is not None:
             pulumi.set(__self__, "columns", columns)
+        if date_time_input_format is not None:
+            pulumi.set(__self__, "date_time_input_format", date_time_input_format)
+        if handle_error_mode is not None:
+            pulumi.set(__self__, "handle_error_mode", handle_error_mode)
+        if max_block_size is not None:
+            pulumi.set(__self__, "max_block_size", max_block_size)
+        if max_rows_per_message is not None:
+            pulumi.set(__self__, "max_rows_per_message", max_rows_per_message)
+        if num_consumers is not None:
+            pulumi.set(__self__, "num_consumers", num_consumers)
+        if poll_max_batch_size is not None:
+            pulumi.set(__self__, "poll_max_batch_size", poll_max_batch_size)
+        if skip_broken_messages is not None:
+            pulumi.set(__self__, "skip_broken_messages", skip_broken_messages)
         if topics is not None:
             pulumi.set(__self__, "topics", topics)
 
     @property
     @pulumi.getter(name="dataFormat")
     def data_format(self) -> str:
         return pulumi.get(self, "data_format")
@@ -11918,19 +12186,59 @@
 
     @property
     @pulumi.getter
     def name(self) -> str:
         return pulumi.get(self, "name")
 
     @property
+    @pulumi.getter(name="autoOffsetReset")
+    def auto_offset_reset(self) -> Optional[str]:
+        return pulumi.get(self, "auto_offset_reset")
+
+    @property
     @pulumi.getter
     def columns(self) -> Optional[Sequence['outputs.ServiceIntegrationClickhouseKafkaUserConfigTableColumn']]:
         return pulumi.get(self, "columns")
 
     @property
+    @pulumi.getter(name="dateTimeInputFormat")
+    def date_time_input_format(self) -> Optional[str]:
+        return pulumi.get(self, "date_time_input_format")
+
+    @property
+    @pulumi.getter(name="handleErrorMode")
+    def handle_error_mode(self) -> Optional[str]:
+        return pulumi.get(self, "handle_error_mode")
+
+    @property
+    @pulumi.getter(name="maxBlockSize")
+    def max_block_size(self) -> Optional[int]:
+        return pulumi.get(self, "max_block_size")
+
+    @property
+    @pulumi.getter(name="maxRowsPerMessage")
+    def max_rows_per_message(self) -> Optional[int]:
+        return pulumi.get(self, "max_rows_per_message")
+
+    @property
+    @pulumi.getter(name="numConsumers")
+    def num_consumers(self) -> Optional[int]:
+        return pulumi.get(self, "num_consumers")
+
+    @property
+    @pulumi.getter(name="pollMaxBatchSize")
+    def poll_max_batch_size(self) -> Optional[int]:
+        return pulumi.get(self, "poll_max_batch_size")
+
+    @property
+    @pulumi.getter(name="skipBrokenMessages")
+    def skip_broken_messages(self) -> Optional[int]:
+        return pulumi.get(self, "skip_broken_messages")
+
+    @property
     @pulumi.getter
     def topics(self) -> Optional[Sequence['outputs.ServiceIntegrationClickhouseKafkaUserConfigTableTopic']]:
         return pulumi.get(self, "topics")
 
 
 @pulumi.output_type
 class ServiceIntegrationClickhouseKafkaUserConfigTableColumn(dict):
@@ -12052,15 +12360,15 @@
         :param Sequence['ServiceIntegrationDatadogUserConfigDatadogTagArgs'] datadog_tags: Custom tags provided by user.
         :param Sequence[str] exclude_consumer_groups: List of custom metrics.
         :param Sequence[str] exclude_topics: List of topics to exclude.
         :param Sequence[str] include_consumer_groups: List of custom metrics.
         :param Sequence[str] include_topics: List of topics to include.
         :param Sequence[str] kafka_custom_metrics: List of custom metrics.
         :param int max_jmx_metrics: Maximum number of JMX metrics to send.
-        :param 'ServiceIntegrationDatadogUserConfigOpensearchArgs' opensearch: Datadog Opensearch Options.
+        :param 'ServiceIntegrationDatadogUserConfigOpensearchArgs' opensearch: Datadog OpenSearch Options.
         :param 'ServiceIntegrationDatadogUserConfigRedisArgs' redis: Datadog Redis Options.
         """
         if datadog_dbm_enabled is not None:
             pulumi.set(__self__, "datadog_dbm_enabled", datadog_dbm_enabled)
         if datadog_tags is not None:
             pulumi.set(__self__, "datadog_tags", datadog_tags)
         if exclude_consumer_groups is not None:
@@ -12144,15 +12452,15 @@
         """
         return pulumi.get(self, "max_jmx_metrics")
 
     @property
     @pulumi.getter
     def opensearch(self) -> Optional['outputs.ServiceIntegrationDatadogUserConfigOpensearch']:
         """
-        Datadog Opensearch Options.
+        Datadog OpenSearch Options.
         """
         return pulumi.get(self, "opensearch")
 
     @property
     @pulumi.getter
     def redis(self) -> Optional['outputs.ServiceIntegrationDatadogUserConfigRedis']:
         """
@@ -14535,28 +14843,43 @@
 @pulumi.output_type
 class GetClickhouseClickhouseUserConfigResult(dict):
     def __init__(__self__, *,
                  additional_backup_regions: Optional[str] = None,
                  ip_filter_objects: Optional[Sequence['outputs.GetClickhouseClickhouseUserConfigIpFilterObjectResult']] = None,
                  ip_filter_strings: Optional[Sequence[str]] = None,
                  ip_filters: Optional[Sequence[str]] = None,
+                 private_access: Optional['outputs.GetClickhouseClickhouseUserConfigPrivateAccessResult'] = None,
+                 privatelink_access: Optional['outputs.GetClickhouseClickhouseUserConfigPrivatelinkAccessResult'] = None,
                  project_to_fork_from: Optional[str] = None,
-                 service_to_fork_from: Optional[str] = None):
+                 public_access: Optional['outputs.GetClickhouseClickhouseUserConfigPublicAccessResult'] = None,
+                 service_to_fork_from: Optional[str] = None,
+                 static_ips: Optional[bool] = None):
+        """
+        :param bool static_ips: Static IPs that are going to be associated with this service. Please assign a value using the 'toset' function. Once a static ip resource is in the 'assigned' state it cannot be unbound from the node again
+        """
         if additional_backup_regions is not None:
             pulumi.set(__self__, "additional_backup_regions", additional_backup_regions)
         if ip_filter_objects is not None:
             pulumi.set(__self__, "ip_filter_objects", ip_filter_objects)
         if ip_filter_strings is not None:
             pulumi.set(__self__, "ip_filter_strings", ip_filter_strings)
         if ip_filters is not None:
             pulumi.set(__self__, "ip_filters", ip_filters)
+        if private_access is not None:
+            pulumi.set(__self__, "private_access", private_access)
+        if privatelink_access is not None:
+            pulumi.set(__self__, "privatelink_access", privatelink_access)
         if project_to_fork_from is not None:
             pulumi.set(__self__, "project_to_fork_from", project_to_fork_from)
+        if public_access is not None:
+            pulumi.set(__self__, "public_access", public_access)
         if service_to_fork_from is not None:
             pulumi.set(__self__, "service_to_fork_from", service_to_fork_from)
+        if static_ips is not None:
+            pulumi.set(__self__, "static_ips", static_ips)
 
     @property
     @pulumi.getter(name="additionalBackupRegions")
     def additional_backup_regions(self) -> Optional[str]:
         return pulumi.get(self, "additional_backup_regions")
 
     @property
@@ -14574,23 +14897,46 @@
     def ip_filters(self) -> Optional[Sequence[str]]:
         warnings.warn("""This will be removed in v5.0.0 and replaced with ip_filter_string instead.""", DeprecationWarning)
         pulumi.log.warn("""ip_filters is deprecated: This will be removed in v5.0.0 and replaced with ip_filter_string instead.""")
 
         return pulumi.get(self, "ip_filters")
 
     @property
+    @pulumi.getter(name="privateAccess")
+    def private_access(self) -> Optional['outputs.GetClickhouseClickhouseUserConfigPrivateAccessResult']:
+        return pulumi.get(self, "private_access")
+
+    @property
+    @pulumi.getter(name="privatelinkAccess")
+    def privatelink_access(self) -> Optional['outputs.GetClickhouseClickhouseUserConfigPrivatelinkAccessResult']:
+        return pulumi.get(self, "privatelink_access")
+
+    @property
     @pulumi.getter(name="projectToForkFrom")
     def project_to_fork_from(self) -> Optional[str]:
         return pulumi.get(self, "project_to_fork_from")
 
     @property
+    @pulumi.getter(name="publicAccess")
+    def public_access(self) -> Optional['outputs.GetClickhouseClickhouseUserConfigPublicAccessResult']:
+        return pulumi.get(self, "public_access")
+
+    @property
     @pulumi.getter(name="serviceToForkFrom")
     def service_to_fork_from(self) -> Optional[str]:
         return pulumi.get(self, "service_to_fork_from")
 
+    @property
+    @pulumi.getter(name="staticIps")
+    def static_ips(self) -> Optional[bool]:
+        """
+        Static IPs that are going to be associated with this service. Please assign a value using the 'toset' function. Once a static ip resource is in the 'assigned' state it cannot be unbound from the node again
+        """
+        return pulumi.get(self, "static_ips")
+
 
 @pulumi.output_type
 class GetClickhouseClickhouseUserConfigIpFilterObjectResult(dict):
     def __init__(__self__, *,
                  network: str,
                  description: Optional[str] = None):
         pulumi.set(__self__, "network", network)
@@ -14605,14 +14951,119 @@
     @property
     @pulumi.getter
     def description(self) -> Optional[str]:
         return pulumi.get(self, "description")
 
 
 @pulumi.output_type
+class GetClickhouseClickhouseUserConfigPrivateAccessResult(dict):
+    def __init__(__self__, *,
+                 clickhouse: Optional[bool] = None,
+                 clickhouse_https: Optional[bool] = None,
+                 prometheus: Optional[bool] = None):
+        """
+        :param bool clickhouse: Clickhouse server provided values
+        """
+        if clickhouse is not None:
+            pulumi.set(__self__, "clickhouse", clickhouse)
+        if clickhouse_https is not None:
+            pulumi.set(__self__, "clickhouse_https", clickhouse_https)
+        if prometheus is not None:
+            pulumi.set(__self__, "prometheus", prometheus)
+
+    @property
+    @pulumi.getter
+    def clickhouse(self) -> Optional[bool]:
+        """
+        Clickhouse server provided values
+        """
+        return pulumi.get(self, "clickhouse")
+
+    @property
+    @pulumi.getter(name="clickhouseHttps")
+    def clickhouse_https(self) -> Optional[bool]:
+        return pulumi.get(self, "clickhouse_https")
+
+    @property
+    @pulumi.getter
+    def prometheus(self) -> Optional[bool]:
+        return pulumi.get(self, "prometheus")
+
+
+@pulumi.output_type
+class GetClickhouseClickhouseUserConfigPrivatelinkAccessResult(dict):
+    def __init__(__self__, *,
+                 clickhouse: Optional[bool] = None,
+                 clickhouse_https: Optional[bool] = None,
+                 prometheus: Optional[bool] = None):
+        """
+        :param bool clickhouse: Clickhouse server provided values
+        """
+        if clickhouse is not None:
+            pulumi.set(__self__, "clickhouse", clickhouse)
+        if clickhouse_https is not None:
+            pulumi.set(__self__, "clickhouse_https", clickhouse_https)
+        if prometheus is not None:
+            pulumi.set(__self__, "prometheus", prometheus)
+
+    @property
+    @pulumi.getter
+    def clickhouse(self) -> Optional[bool]:
+        """
+        Clickhouse server provided values
+        """
+        return pulumi.get(self, "clickhouse")
+
+    @property
+    @pulumi.getter(name="clickhouseHttps")
+    def clickhouse_https(self) -> Optional[bool]:
+        return pulumi.get(self, "clickhouse_https")
+
+    @property
+    @pulumi.getter
+    def prometheus(self) -> Optional[bool]:
+        return pulumi.get(self, "prometheus")
+
+
+@pulumi.output_type
+class GetClickhouseClickhouseUserConfigPublicAccessResult(dict):
+    def __init__(__self__, *,
+                 clickhouse: Optional[bool] = None,
+                 clickhouse_https: Optional[bool] = None,
+                 prometheus: Optional[bool] = None):
+        """
+        :param bool clickhouse: Clickhouse server provided values
+        """
+        if clickhouse is not None:
+            pulumi.set(__self__, "clickhouse", clickhouse)
+        if clickhouse_https is not None:
+            pulumi.set(__self__, "clickhouse_https", clickhouse_https)
+        if prometheus is not None:
+            pulumi.set(__self__, "prometheus", prometheus)
+
+    @property
+    @pulumi.getter
+    def clickhouse(self) -> Optional[bool]:
+        """
+        Clickhouse server provided values
+        """
+        return pulumi.get(self, "clickhouse")
+
+    @property
+    @pulumi.getter(name="clickhouseHttps")
+    def clickhouse_https(self) -> Optional[bool]:
+        return pulumi.get(self, "clickhouse_https")
+
+    @property
+    @pulumi.getter
+    def prometheus(self) -> Optional[bool]:
+        return pulumi.get(self, "prometheus")
+
+
+@pulumi.output_type
 class GetClickhouseComponentResult(dict):
     def __init__(__self__, *,
                  component: str,
                  host: str,
                  kafka_authentication_method: str,
                  port: int,
                  route: str,
@@ -16082,25 +16533,28 @@
 class GetInfluxDbInfluxdbUserConfigInfluxdbResult(dict):
     def __init__(__self__, *,
                  log_queries_after: Optional[int] = None,
                  max_connection_limit: Optional[int] = None,
                  max_row_limit: Optional[int] = None,
                  max_select_buckets: Optional[int] = None,
                  max_select_point: Optional[int] = None,
+                 query_log_enabled: Optional[bool] = None,
                  query_timeout: Optional[int] = None):
         if log_queries_after is not None:
             pulumi.set(__self__, "log_queries_after", log_queries_after)
         if max_connection_limit is not None:
             pulumi.set(__self__, "max_connection_limit", max_connection_limit)
         if max_row_limit is not None:
             pulumi.set(__self__, "max_row_limit", max_row_limit)
         if max_select_buckets is not None:
             pulumi.set(__self__, "max_select_buckets", max_select_buckets)
         if max_select_point is not None:
             pulumi.set(__self__, "max_select_point", max_select_point)
+        if query_log_enabled is not None:
+            pulumi.set(__self__, "query_log_enabled", query_log_enabled)
         if query_timeout is not None:
             pulumi.set(__self__, "query_timeout", query_timeout)
 
     @property
     @pulumi.getter(name="logQueriesAfter")
     def log_queries_after(self) -> Optional[int]:
         return pulumi.get(self, "log_queries_after")
@@ -16122,14 +16576,19 @@
 
     @property
     @pulumi.getter(name="maxSelectPoint")
     def max_select_point(self) -> Optional[int]:
         return pulumi.get(self, "max_select_point")
 
     @property
+    @pulumi.getter(name="queryLogEnabled")
+    def query_log_enabled(self) -> Optional[bool]:
+        return pulumi.get(self, "query_log_enabled")
+
+    @property
     @pulumi.getter(name="queryTimeout")
     def query_timeout(self) -> Optional[int]:
         return pulumi.get(self, "query_timeout")
 
 
 @pulumi.output_type
 class GetInfluxDbInfluxdbUserConfigIpFilterObjectResult(dict):
@@ -19818,15 +20277,15 @@
                  project_to_fork_from: Optional[str] = None,
                  public_access: Optional['outputs.GetOpenSearchOpensearchUserConfigPublicAccessResult'] = None,
                  recovery_basebackup_name: Optional[str] = None,
                  saml: Optional['outputs.GetOpenSearchOpensearchUserConfigSamlResult'] = None,
                  service_to_fork_from: Optional[str] = None,
                  static_ips: Optional[bool] = None):
         """
-        :param 'GetOpenSearchOpensearchUserConfigOpensearchArgs' opensearch: Opensearch server provided values
+        :param 'GetOpenSearchOpensearchUserConfigOpensearchArgs' opensearch: OpenSearch server provided values
         :param bool static_ips: Static IPs that are going to be associated with this service. Please assign a value using the 'toset' function. Once a static ip resource is in the 'assigned' state it cannot be unbound from the node again
         """
         if additional_backup_regions is not None:
             pulumi.set(__self__, "additional_backup_regions", additional_backup_regions)
         if custom_domain is not None:
             pulumi.set(__self__, "custom_domain", custom_domain)
         if disable_replication_factor_adjustment is not None:
@@ -19927,15 +20386,15 @@
 
         return pulumi.get(self, "max_index_count")
 
     @property
     @pulumi.getter
     def opensearch(self) -> Optional['outputs.GetOpenSearchOpensearchUserConfigOpensearchResult']:
         """
-        Opensearch server provided values
+        OpenSearch server provided values
         """
         return pulumi.get(self, "opensearch")
 
     @property
     @pulumi.getter(name="opensearchDashboards")
     def opensearch_dashboards(self) -> Optional['outputs.GetOpenSearchOpensearchUserConfigOpensearchDashboardsResult']:
         return pulumi.get(self, "opensearch_dashboards")
@@ -20350,28 +20809,28 @@
 @pulumi.output_type
 class GetOpenSearchOpensearchUserConfigPrivateAccessResult(dict):
     def __init__(__self__, *,
                  opensearch: Optional[bool] = None,
                  opensearch_dashboards: Optional[bool] = None,
                  prometheus: Optional[bool] = None):
         """
-        :param bool opensearch: Opensearch server provided values
+        :param bool opensearch: OpenSearch server provided values
         """
         if opensearch is not None:
             pulumi.set(__self__, "opensearch", opensearch)
         if opensearch_dashboards is not None:
             pulumi.set(__self__, "opensearch_dashboards", opensearch_dashboards)
         if prometheus is not None:
             pulumi.set(__self__, "prometheus", prometheus)
 
     @property
     @pulumi.getter
     def opensearch(self) -> Optional[bool]:
         """
-        Opensearch server provided values
+        OpenSearch server provided values
         """
         return pulumi.get(self, "opensearch")
 
     @property
     @pulumi.getter(name="opensearchDashboards")
     def opensearch_dashboards(self) -> Optional[bool]:
         return pulumi.get(self, "opensearch_dashboards")
@@ -20385,28 +20844,28 @@
 @pulumi.output_type
 class GetOpenSearchOpensearchUserConfigPrivatelinkAccessResult(dict):
     def __init__(__self__, *,
                  opensearch: Optional[bool] = None,
                  opensearch_dashboards: Optional[bool] = None,
                  prometheus: Optional[bool] = None):
         """
-        :param bool opensearch: Opensearch server provided values
+        :param bool opensearch: OpenSearch server provided values
         """
         if opensearch is not None:
             pulumi.set(__self__, "opensearch", opensearch)
         if opensearch_dashboards is not None:
             pulumi.set(__self__, "opensearch_dashboards", opensearch_dashboards)
         if prometheus is not None:
             pulumi.set(__self__, "prometheus", prometheus)
 
     @property
     @pulumi.getter
     def opensearch(self) -> Optional[bool]:
         """
-        Opensearch server provided values
+        OpenSearch server provided values
         """
         return pulumi.get(self, "opensearch")
 
     @property
     @pulumi.getter(name="opensearchDashboards")
     def opensearch_dashboards(self) -> Optional[bool]:
         return pulumi.get(self, "opensearch_dashboards")
@@ -20420,28 +20879,28 @@
 @pulumi.output_type
 class GetOpenSearchOpensearchUserConfigPublicAccessResult(dict):
     def __init__(__self__, *,
                  opensearch: Optional[bool] = None,
                  opensearch_dashboards: Optional[bool] = None,
                  prometheus: Optional[bool] = None):
         """
-        :param bool opensearch: Opensearch server provided values
+        :param bool opensearch: OpenSearch server provided values
         """
         if opensearch is not None:
             pulumi.set(__self__, "opensearch", opensearch)
         if opensearch_dashboards is not None:
             pulumi.set(__self__, "opensearch_dashboards", opensearch_dashboards)
         if prometheus is not None:
             pulumi.set(__self__, "prometheus", prometheus)
 
     @property
     @pulumi.getter
     def opensearch(self) -> Optional[bool]:
         """
-        Opensearch server provided values
+        OpenSearch server provided values
         """
         return pulumi.get(self, "opensearch")
 
     @property
     @pulumi.getter(name="opensearchDashboards")
     def opensearch_dashboards(self) -> Optional[bool]:
         return pulumi.get(self, "opensearch_dashboards")
@@ -22153,21 +22612,45 @@
 
 @pulumi.output_type
 class GetServiceIntegrationClickhouseKafkaUserConfigTableResult(dict):
     def __init__(__self__, *,
                  data_format: str,
                  group_name: str,
                  name: str,
+                 auto_offset_reset: Optional[str] = None,
                  columns: Optional[Sequence['outputs.GetServiceIntegrationClickhouseKafkaUserConfigTableColumnResult']] = None,
+                 date_time_input_format: Optional[str] = None,
+                 handle_error_mode: Optional[str] = None,
+                 max_block_size: Optional[int] = None,
+                 max_rows_per_message: Optional[int] = None,
+                 num_consumers: Optional[int] = None,
+                 poll_max_batch_size: Optional[int] = None,
+                 skip_broken_messages: Optional[int] = None,
                  topics: Optional[Sequence['outputs.GetServiceIntegrationClickhouseKafkaUserConfigTableTopicResult']] = None):
         pulumi.set(__self__, "data_format", data_format)
         pulumi.set(__self__, "group_name", group_name)
         pulumi.set(__self__, "name", name)
+        if auto_offset_reset is not None:
+            pulumi.set(__self__, "auto_offset_reset", auto_offset_reset)
         if columns is not None:
             pulumi.set(__self__, "columns", columns)
+        if date_time_input_format is not None:
+            pulumi.set(__self__, "date_time_input_format", date_time_input_format)
+        if handle_error_mode is not None:
+            pulumi.set(__self__, "handle_error_mode", handle_error_mode)
+        if max_block_size is not None:
+            pulumi.set(__self__, "max_block_size", max_block_size)
+        if max_rows_per_message is not None:
+            pulumi.set(__self__, "max_rows_per_message", max_rows_per_message)
+        if num_consumers is not None:
+            pulumi.set(__self__, "num_consumers", num_consumers)
+        if poll_max_batch_size is not None:
+            pulumi.set(__self__, "poll_max_batch_size", poll_max_batch_size)
+        if skip_broken_messages is not None:
+            pulumi.set(__self__, "skip_broken_messages", skip_broken_messages)
         if topics is not None:
             pulumi.set(__self__, "topics", topics)
 
     @property
     @pulumi.getter(name="dataFormat")
     def data_format(self) -> str:
         return pulumi.get(self, "data_format")
@@ -22179,19 +22662,59 @@
 
     @property
     @pulumi.getter
     def name(self) -> str:
         return pulumi.get(self, "name")
 
     @property
+    @pulumi.getter(name="autoOffsetReset")
+    def auto_offset_reset(self) -> Optional[str]:
+        return pulumi.get(self, "auto_offset_reset")
+
+    @property
     @pulumi.getter
     def columns(self) -> Optional[Sequence['outputs.GetServiceIntegrationClickhouseKafkaUserConfigTableColumnResult']]:
         return pulumi.get(self, "columns")
 
     @property
+    @pulumi.getter(name="dateTimeInputFormat")
+    def date_time_input_format(self) -> Optional[str]:
+        return pulumi.get(self, "date_time_input_format")
+
+    @property
+    @pulumi.getter(name="handleErrorMode")
+    def handle_error_mode(self) -> Optional[str]:
+        return pulumi.get(self, "handle_error_mode")
+
+    @property
+    @pulumi.getter(name="maxBlockSize")
+    def max_block_size(self) -> Optional[int]:
+        return pulumi.get(self, "max_block_size")
+
+    @property
+    @pulumi.getter(name="maxRowsPerMessage")
+    def max_rows_per_message(self) -> Optional[int]:
+        return pulumi.get(self, "max_rows_per_message")
+
+    @property
+    @pulumi.getter(name="numConsumers")
+    def num_consumers(self) -> Optional[int]:
+        return pulumi.get(self, "num_consumers")
+
+    @property
+    @pulumi.getter(name="pollMaxBatchSize")
+    def poll_max_batch_size(self) -> Optional[int]:
+        return pulumi.get(self, "poll_max_batch_size")
+
+    @property
+    @pulumi.getter(name="skipBrokenMessages")
+    def skip_broken_messages(self) -> Optional[int]:
+        return pulumi.get(self, "skip_broken_messages")
+
+    @property
     @pulumi.getter
     def topics(self) -> Optional[Sequence['outputs.GetServiceIntegrationClickhouseKafkaUserConfigTableTopicResult']]:
         return pulumi.get(self, "topics")
 
 
 @pulumi.output_type
 class GetServiceIntegrationClickhouseKafkaUserConfigTableColumnResult(dict):
```

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/pg.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/pg.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/pg_database.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/pg_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/pg_user.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/pg_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/project.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/project.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,40 +18,47 @@
     def __init__(__self__, *,
                  project: pulumi.Input[str],
                  account_id: Optional[pulumi.Input[str]] = None,
                  add_account_owners_admin_access: Optional[pulumi.Input[bool]] = None,
                  billing_group: Optional[pulumi.Input[str]] = None,
                  copy_from_project: Optional[pulumi.Input[str]] = None,
                  default_cloud: Optional[pulumi.Input[str]] = None,
+                 parent_id: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectTagArgs']]]] = None,
                  technical_emails: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  use_source_project_billing_group: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a Project resource.
         :param pulumi.Input[str] project: Defines the name of the project. Name must be globally unique (between all Aiven customers) and cannot be changed later without destroying and re-creating the project, including all sub-resources.
-        :param pulumi.Input[str] account_id: An optional property to link a project to already an existing account by using account ID. To set up proper dependencies please refer to this variable as a reference.
-        :param pulumi.Input[bool] add_account_owners_admin_access: If account_id is set, grant account owner team admin access to the new project. The default value is `true`.
+        :param pulumi.Input[str] account_id: An optional property to link a project to an already existing account by using account ID. To set up proper dependencies please refer to this variable as a reference.
+        :param pulumi.Input[bool] add_account_owners_admin_access: If parent_id is set, grant account owner team admin access to the new project. The default value is `true`.
         :param pulumi.Input[str] billing_group: The id of the billing group that is linked to this project. To set up proper dependencies please refer to this variable as a reference.
         :param pulumi.Input[str] copy_from_project: is the name of another project used to copy billing information and some other project attributes like technical contacts from. This is mostly relevant when an existing project has billing type set to invoice and that needs to be copied over to a new project. (Setting billing is otherwise not allowed over the API.) This only has effect when the project is created. To set up proper dependencies please refer to this variable as a reference.
         :param pulumi.Input[str] default_cloud: Defines the default cloud provider and region where services are hosted. This can be changed freely after the project is created. This will not affect existing services.
+        :param pulumi.Input[str] parent_id: An optional property to link a project to an already existing organization or account by using its ID. To set up proper dependencies please refer to this variable as a reference.
         :param pulumi.Input[Sequence[pulumi.Input['ProjectTagArgs']]] tags: Tags are key-value pairs that allow you to categorize projects.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] technical_emails: Defines the email addresses that will receive alerts about upcoming maintenance updates or warnings about service instability. It is  good practice to keep this up-to-date to be aware of any potential issues with your project.
         :param pulumi.Input[bool] use_source_project_billing_group: Use the same billing group that is used in source project.
         """
         pulumi.set(__self__, "project", project)
         if account_id is not None:
+            warnings.warn("""Use parent_id instead. This field will be removed in the next major release.""", DeprecationWarning)
+            pulumi.log.warn("""account_id is deprecated: Use parent_id instead. This field will be removed in the next major release.""")
+        if account_id is not None:
             pulumi.set(__self__, "account_id", account_id)
         if add_account_owners_admin_access is not None:
             pulumi.set(__self__, "add_account_owners_admin_access", add_account_owners_admin_access)
         if billing_group is not None:
             pulumi.set(__self__, "billing_group", billing_group)
         if copy_from_project is not None:
             pulumi.set(__self__, "copy_from_project", copy_from_project)
         if default_cloud is not None:
             pulumi.set(__self__, "default_cloud", default_cloud)
+        if parent_id is not None:
+            pulumi.set(__self__, "parent_id", parent_id)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if technical_emails is not None:
             pulumi.set(__self__, "technical_emails", technical_emails)
         if use_source_project_billing_group is not None:
             pulumi.set(__self__, "use_source_project_billing_group", use_source_project_billing_group)
 
@@ -67,27 +74,30 @@
     def project(self, value: pulumi.Input[str]):
         pulumi.set(self, "project", value)
 
     @property
     @pulumi.getter(name="accountId")
     def account_id(self) -> Optional[pulumi.Input[str]]:
         """
-        An optional property to link a project to already an existing account by using account ID. To set up proper dependencies please refer to this variable as a reference.
+        An optional property to link a project to an already existing account by using account ID. To set up proper dependencies please refer to this variable as a reference.
         """
+        warnings.warn("""Use parent_id instead. This field will be removed in the next major release.""", DeprecationWarning)
+        pulumi.log.warn("""account_id is deprecated: Use parent_id instead. This field will be removed in the next major release.""")
+
         return pulumi.get(self, "account_id")
 
     @account_id.setter
     def account_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "account_id", value)
 
     @property
     @pulumi.getter(name="addAccountOwnersAdminAccess")
     def add_account_owners_admin_access(self) -> Optional[pulumi.Input[bool]]:
         """
-        If account_id is set, grant account owner team admin access to the new project. The default value is `true`.
+        If parent_id is set, grant account owner team admin access to the new project. The default value is `true`.
         """
         return pulumi.get(self, "add_account_owners_admin_access")
 
     @add_account_owners_admin_access.setter
     def add_account_owners_admin_access(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "add_account_owners_admin_access", value)
 
@@ -124,14 +134,26 @@
         return pulumi.get(self, "default_cloud")
 
     @default_cloud.setter
     def default_cloud(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "default_cloud", value)
 
     @property
+    @pulumi.getter(name="parentId")
+    def parent_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        An optional property to link a project to an already existing organization or account by using its ID. To set up proper dependencies please refer to this variable as a reference.
+        """
+        return pulumi.get(self, "parent_id")
+
+    @parent_id.setter
+    def parent_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "parent_id", value)
+
+    @property
     @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ProjectTagArgs']]]]:
         """
         Tags are key-value pairs that allow you to categorize projects.
         """
         return pulumi.get(self, "tags")
 
@@ -171,36 +193,41 @@
                  add_account_owners_admin_access: Optional[pulumi.Input[bool]] = None,
                  available_credits: Optional[pulumi.Input[str]] = None,
                  billing_group: Optional[pulumi.Input[str]] = None,
                  ca_cert: Optional[pulumi.Input[str]] = None,
                  copy_from_project: Optional[pulumi.Input[str]] = None,
                  default_cloud: Optional[pulumi.Input[str]] = None,
                  estimated_balance: Optional[pulumi.Input[str]] = None,
+                 parent_id: Optional[pulumi.Input[str]] = None,
                  payment_method: Optional[pulumi.Input[str]] = None,
                  project: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectTagArgs']]]] = None,
                  technical_emails: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  use_source_project_billing_group: Optional[pulumi.Input[bool]] = None):
         """
         Input properties used for looking up and filtering Project resources.
-        :param pulumi.Input[str] account_id: An optional property to link a project to already an existing account by using account ID. To set up proper dependencies please refer to this variable as a reference.
-        :param pulumi.Input[bool] add_account_owners_admin_access: If account_id is set, grant account owner team admin access to the new project. The default value is `true`.
+        :param pulumi.Input[str] account_id: An optional property to link a project to an already existing account by using account ID. To set up proper dependencies please refer to this variable as a reference.
+        :param pulumi.Input[bool] add_account_owners_admin_access: If parent_id is set, grant account owner team admin access to the new project. The default value is `true`.
         :param pulumi.Input[str] available_credits: The amount of platform credits available to the project. This could be your free trial or other promotional credits.
         :param pulumi.Input[str] billing_group: The id of the billing group that is linked to this project. To set up proper dependencies please refer to this variable as a reference.
         :param pulumi.Input[str] ca_cert: The CA certificate of the project. This is required for configuring clients that connect to certain services like Kafka.
         :param pulumi.Input[str] copy_from_project: is the name of another project used to copy billing information and some other project attributes like technical contacts from. This is mostly relevant when an existing project has billing type set to invoice and that needs to be copied over to a new project. (Setting billing is otherwise not allowed over the API.) This only has effect when the project is created. To set up proper dependencies please refer to this variable as a reference.
         :param pulumi.Input[str] default_cloud: Defines the default cloud provider and region where services are hosted. This can be changed freely after the project is created. This will not affect existing services.
         :param pulumi.Input[str] estimated_balance: The current accumulated bill for this project in the current billing period.
+        :param pulumi.Input[str] parent_id: An optional property to link a project to an already existing organization or account by using its ID. To set up proper dependencies please refer to this variable as a reference.
         :param pulumi.Input[str] payment_method: The method of invoicing used for payments for this project, e.g. `card`.
         :param pulumi.Input[str] project: Defines the name of the project. Name must be globally unique (between all Aiven customers) and cannot be changed later without destroying and re-creating the project, including all sub-resources.
         :param pulumi.Input[Sequence[pulumi.Input['ProjectTagArgs']]] tags: Tags are key-value pairs that allow you to categorize projects.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] technical_emails: Defines the email addresses that will receive alerts about upcoming maintenance updates or warnings about service instability. It is  good practice to keep this up-to-date to be aware of any potential issues with your project.
         :param pulumi.Input[bool] use_source_project_billing_group: Use the same billing group that is used in source project.
         """
         if account_id is not None:
+            warnings.warn("""Use parent_id instead. This field will be removed in the next major release.""", DeprecationWarning)
+            pulumi.log.warn("""account_id is deprecated: Use parent_id instead. This field will be removed in the next major release.""")
+        if account_id is not None:
             pulumi.set(__self__, "account_id", account_id)
         if add_account_owners_admin_access is not None:
             pulumi.set(__self__, "add_account_owners_admin_access", add_account_owners_admin_access)
         if available_credits is not None:
             pulumi.set(__self__, "available_credits", available_credits)
         if billing_group is not None:
             pulumi.set(__self__, "billing_group", billing_group)
@@ -208,14 +235,16 @@
             pulumi.set(__self__, "ca_cert", ca_cert)
         if copy_from_project is not None:
             pulumi.set(__self__, "copy_from_project", copy_from_project)
         if default_cloud is not None:
             pulumi.set(__self__, "default_cloud", default_cloud)
         if estimated_balance is not None:
             pulumi.set(__self__, "estimated_balance", estimated_balance)
+        if parent_id is not None:
+            pulumi.set(__self__, "parent_id", parent_id)
         if payment_method is not None:
             pulumi.set(__self__, "payment_method", payment_method)
         if project is not None:
             pulumi.set(__self__, "project", project)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if technical_emails is not None:
@@ -223,27 +252,30 @@
         if use_source_project_billing_group is not None:
             pulumi.set(__self__, "use_source_project_billing_group", use_source_project_billing_group)
 
     @property
     @pulumi.getter(name="accountId")
     def account_id(self) -> Optional[pulumi.Input[str]]:
         """
-        An optional property to link a project to already an existing account by using account ID. To set up proper dependencies please refer to this variable as a reference.
+        An optional property to link a project to an already existing account by using account ID. To set up proper dependencies please refer to this variable as a reference.
         """
+        warnings.warn("""Use parent_id instead. This field will be removed in the next major release.""", DeprecationWarning)
+        pulumi.log.warn("""account_id is deprecated: Use parent_id instead. This field will be removed in the next major release.""")
+
         return pulumi.get(self, "account_id")
 
     @account_id.setter
     def account_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "account_id", value)
 
     @property
     @pulumi.getter(name="addAccountOwnersAdminAccess")
     def add_account_owners_admin_access(self) -> Optional[pulumi.Input[bool]]:
         """
-        If account_id is set, grant account owner team admin access to the new project. The default value is `true`.
+        If parent_id is set, grant account owner team admin access to the new project. The default value is `true`.
         """
         return pulumi.get(self, "add_account_owners_admin_access")
 
     @add_account_owners_admin_access.setter
     def add_account_owners_admin_access(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "add_account_owners_admin_access", value)
 
@@ -316,14 +348,26 @@
         return pulumi.get(self, "estimated_balance")
 
     @estimated_balance.setter
     def estimated_balance(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "estimated_balance", value)
 
     @property
+    @pulumi.getter(name="parentId")
+    def parent_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        An optional property to link a project to an already existing organization or account by using its ID. To set up proper dependencies please refer to this variable as a reference.
+        """
+        return pulumi.get(self, "parent_id")
+
+    @parent_id.setter
+    def parent_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "parent_id", value)
+
+    @property
     @pulumi.getter(name="paymentMethod")
     def payment_method(self) -> Optional[pulumi.Input[str]]:
         """
         The method of invoicing used for payments for this project, e.g. `card`.
         """
         return pulumi.get(self, "payment_method")
 
@@ -386,14 +430,15 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  account_id: Optional[pulumi.Input[str]] = None,
                  add_account_owners_admin_access: Optional[pulumi.Input[bool]] = None,
                  billing_group: Optional[pulumi.Input[str]] = None,
                  copy_from_project: Optional[pulumi.Input[str]] = None,
                  default_cloud: Optional[pulumi.Input[str]] = None,
+                 parent_id: Optional[pulumi.Input[str]] = None,
                  project: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectTagArgs']]]]] = None,
                  technical_emails: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  use_source_project_billing_group: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
         The Project resource allows the creation and management of Aiven Projects.
@@ -402,19 +447,20 @@
 
         ```sh
          $ pulumi import aiven:index/project:Project myproject project
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] account_id: An optional property to link a project to already an existing account by using account ID. To set up proper dependencies please refer to this variable as a reference.
-        :param pulumi.Input[bool] add_account_owners_admin_access: If account_id is set, grant account owner team admin access to the new project. The default value is `true`.
+        :param pulumi.Input[str] account_id: An optional property to link a project to an already existing account by using account ID. To set up proper dependencies please refer to this variable as a reference.
+        :param pulumi.Input[bool] add_account_owners_admin_access: If parent_id is set, grant account owner team admin access to the new project. The default value is `true`.
         :param pulumi.Input[str] billing_group: The id of the billing group that is linked to this project. To set up proper dependencies please refer to this variable as a reference.
         :param pulumi.Input[str] copy_from_project: is the name of another project used to copy billing information and some other project attributes like technical contacts from. This is mostly relevant when an existing project has billing type set to invoice and that needs to be copied over to a new project. (Setting billing is otherwise not allowed over the API.) This only has effect when the project is created. To set up proper dependencies please refer to this variable as a reference.
         :param pulumi.Input[str] default_cloud: Defines the default cloud provider and region where services are hosted. This can be changed freely after the project is created. This will not affect existing services.
+        :param pulumi.Input[str] parent_id: An optional property to link a project to an already existing organization or account by using its ID. To set up proper dependencies please refer to this variable as a reference.
         :param pulumi.Input[str] project: Defines the name of the project. Name must be globally unique (between all Aiven customers) and cannot be changed later without destroying and re-creating the project, including all sub-resources.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectTagArgs']]]] tags: Tags are key-value pairs that allow you to categorize projects.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] technical_emails: Defines the email addresses that will receive alerts about upcoming maintenance updates or warnings about service instability. It is  good practice to keep this up-to-date to be aware of any potential issues with your project.
         :param pulumi.Input[bool] use_source_project_billing_group: Use the same billing group that is used in source project.
         """
         ...
     @overload
@@ -447,32 +493,37 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  account_id: Optional[pulumi.Input[str]] = None,
                  add_account_owners_admin_access: Optional[pulumi.Input[bool]] = None,
                  billing_group: Optional[pulumi.Input[str]] = None,
                  copy_from_project: Optional[pulumi.Input[str]] = None,
                  default_cloud: Optional[pulumi.Input[str]] = None,
+                 parent_id: Optional[pulumi.Input[str]] = None,
                  project: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectTagArgs']]]]] = None,
                  technical_emails: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  use_source_project_billing_group: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ProjectArgs.__new__(ProjectArgs)
 
+            if account_id is not None and not opts.urn:
+                warnings.warn("""Use parent_id instead. This field will be removed in the next major release.""", DeprecationWarning)
+                pulumi.log.warn("""account_id is deprecated: Use parent_id instead. This field will be removed in the next major release.""")
             __props__.__dict__["account_id"] = account_id
             __props__.__dict__["add_account_owners_admin_access"] = add_account_owners_admin_access
             __props__.__dict__["billing_group"] = billing_group
             __props__.__dict__["copy_from_project"] = copy_from_project
             __props__.__dict__["default_cloud"] = default_cloud
+            __props__.__dict__["parent_id"] = parent_id
             if project is None and not opts.urn:
                 raise TypeError("Missing required property 'project'")
             __props__.__dict__["project"] = project
             __props__.__dict__["tags"] = tags
             __props__.__dict__["technical_emails"] = technical_emails
             __props__.__dict__["use_source_project_billing_group"] = use_source_project_billing_group
             __props__.__dict__["available_credits"] = None
@@ -495,34 +546,36 @@
             add_account_owners_admin_access: Optional[pulumi.Input[bool]] = None,
             available_credits: Optional[pulumi.Input[str]] = None,
             billing_group: Optional[pulumi.Input[str]] = None,
             ca_cert: Optional[pulumi.Input[str]] = None,
             copy_from_project: Optional[pulumi.Input[str]] = None,
             default_cloud: Optional[pulumi.Input[str]] = None,
             estimated_balance: Optional[pulumi.Input[str]] = None,
+            parent_id: Optional[pulumi.Input[str]] = None,
             payment_method: Optional[pulumi.Input[str]] = None,
             project: Optional[pulumi.Input[str]] = None,
             tags: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectTagArgs']]]]] = None,
             technical_emails: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             use_source_project_billing_group: Optional[pulumi.Input[bool]] = None) -> 'Project':
         """
         Get an existing Project resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] account_id: An optional property to link a project to already an existing account by using account ID. To set up proper dependencies please refer to this variable as a reference.
-        :param pulumi.Input[bool] add_account_owners_admin_access: If account_id is set, grant account owner team admin access to the new project. The default value is `true`.
+        :param pulumi.Input[str] account_id: An optional property to link a project to an already existing account by using account ID. To set up proper dependencies please refer to this variable as a reference.
+        :param pulumi.Input[bool] add_account_owners_admin_access: If parent_id is set, grant account owner team admin access to the new project. The default value is `true`.
         :param pulumi.Input[str] available_credits: The amount of platform credits available to the project. This could be your free trial or other promotional credits.
         :param pulumi.Input[str] billing_group: The id of the billing group that is linked to this project. To set up proper dependencies please refer to this variable as a reference.
         :param pulumi.Input[str] ca_cert: The CA certificate of the project. This is required for configuring clients that connect to certain services like Kafka.
         :param pulumi.Input[str] copy_from_project: is the name of another project used to copy billing information and some other project attributes like technical contacts from. This is mostly relevant when an existing project has billing type set to invoice and that needs to be copied over to a new project. (Setting billing is otherwise not allowed over the API.) This only has effect when the project is created. To set up proper dependencies please refer to this variable as a reference.
         :param pulumi.Input[str] default_cloud: Defines the default cloud provider and region where services are hosted. This can be changed freely after the project is created. This will not affect existing services.
         :param pulumi.Input[str] estimated_balance: The current accumulated bill for this project in the current billing period.
+        :param pulumi.Input[str] parent_id: An optional property to link a project to an already existing organization or account by using its ID. To set up proper dependencies please refer to this variable as a reference.
         :param pulumi.Input[str] payment_method: The method of invoicing used for payments for this project, e.g. `card`.
         :param pulumi.Input[str] project: Defines the name of the project. Name must be globally unique (between all Aiven customers) and cannot be changed later without destroying and re-creating the project, including all sub-resources.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectTagArgs']]]] tags: Tags are key-value pairs that allow you to categorize projects.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] technical_emails: Defines the email addresses that will receive alerts about upcoming maintenance updates or warnings about service instability. It is  good practice to keep this up-to-date to be aware of any potential issues with your project.
         :param pulumi.Input[bool] use_source_project_billing_group: Use the same billing group that is used in source project.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
@@ -533,34 +586,38 @@
         __props__.__dict__["add_account_owners_admin_access"] = add_account_owners_admin_access
         __props__.__dict__["available_credits"] = available_credits
         __props__.__dict__["billing_group"] = billing_group
         __props__.__dict__["ca_cert"] = ca_cert
         __props__.__dict__["copy_from_project"] = copy_from_project
         __props__.__dict__["default_cloud"] = default_cloud
         __props__.__dict__["estimated_balance"] = estimated_balance
+        __props__.__dict__["parent_id"] = parent_id
         __props__.__dict__["payment_method"] = payment_method
         __props__.__dict__["project"] = project
         __props__.__dict__["tags"] = tags
         __props__.__dict__["technical_emails"] = technical_emails
         __props__.__dict__["use_source_project_billing_group"] = use_source_project_billing_group
         return Project(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="accountId")
     def account_id(self) -> pulumi.Output[Optional[str]]:
         """
-        An optional property to link a project to already an existing account by using account ID. To set up proper dependencies please refer to this variable as a reference.
+        An optional property to link a project to an already existing account by using account ID. To set up proper dependencies please refer to this variable as a reference.
         """
+        warnings.warn("""Use parent_id instead. This field will be removed in the next major release.""", DeprecationWarning)
+        pulumi.log.warn("""account_id is deprecated: Use parent_id instead. This field will be removed in the next major release.""")
+
         return pulumi.get(self, "account_id")
 
     @property
     @pulumi.getter(name="addAccountOwnersAdminAccess")
     def add_account_owners_admin_access(self) -> pulumi.Output[Optional[bool]]:
         """
-        If account_id is set, grant account owner team admin access to the new project. The default value is `true`.
+        If parent_id is set, grant account owner team admin access to the new project. The default value is `true`.
         """
         return pulumi.get(self, "add_account_owners_admin_access")
 
     @property
     @pulumi.getter(name="availableCredits")
     def available_credits(self) -> pulumi.Output[str]:
         """
@@ -605,14 +662,22 @@
     def estimated_balance(self) -> pulumi.Output[str]:
         """
         The current accumulated bill for this project in the current billing period.
         """
         return pulumi.get(self, "estimated_balance")
 
     @property
+    @pulumi.getter(name="parentId")
+    def parent_id(self) -> pulumi.Output[Optional[str]]:
+        """
+        An optional property to link a project to an already existing organization or account by using its ID. To set up proper dependencies please refer to this variable as a reference.
+        """
+        return pulumi.get(self, "parent_id")
+
+    @property
     @pulumi.getter(name="paymentMethod")
     def payment_method(self) -> pulumi.Output[str]:
         """
         The method of invoicing used for payments for this project, e.g. `card`.
         """
         return pulumi.get(self, "payment_method")
```

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/project_user.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/project_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/project_vpc.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/project_vpc.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/provider.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/redis.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/redis.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/redis_user.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/redis_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/service_integration.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/service_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/service_integration_endpoint.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/service_integration_endpoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         :param pulumi.Input[str] project: Project the service integration endpoint belongs to
         :param pulumi.Input['ServiceIntegrationEndpointDatadogUserConfigArgs'] datadog_user_config: Datadog user configurable settings
         :param pulumi.Input['ServiceIntegrationEndpointExternalAwsCloudwatchLogsUserConfigArgs'] external_aws_cloudwatch_logs_user_config: ExternalAwsCloudwatchLogs user configurable settings
         :param pulumi.Input['ServiceIntegrationEndpointExternalAwsCloudwatchMetricsUserConfigArgs'] external_aws_cloudwatch_metrics_user_config: ExternalAwsCloudwatchMetrics user configurable settings
         :param pulumi.Input['ServiceIntegrationEndpointExternalElasticsearchLogsUserConfigArgs'] external_elasticsearch_logs_user_config: ExternalElasticsearchLogs user configurable settings
         :param pulumi.Input['ServiceIntegrationEndpointExternalGoogleCloudLoggingUserConfigArgs'] external_google_cloud_logging_user_config: ExternalGoogleCloudLogging user configurable settings
         :param pulumi.Input['ServiceIntegrationEndpointExternalKafkaUserConfigArgs'] external_kafka_user_config: ExternalKafka user configurable settings
-        :param pulumi.Input['ServiceIntegrationEndpointExternalOpensearchLogsUserConfigArgs'] external_opensearch_logs_user_config: ExternalOpensearchLogs user configurable settings
+        :param pulumi.Input['ServiceIntegrationEndpointExternalOpensearchLogsUserConfigArgs'] external_opensearch_logs_user_config: ExternalOpenSearchLogs user configurable settings
         :param pulumi.Input['ServiceIntegrationEndpointExternalSchemaRegistryUserConfigArgs'] external_schema_registry_user_config: ExternalSchemaRegistry user configurable settings
         :param pulumi.Input['ServiceIntegrationEndpointJolokiaUserConfigArgs'] jolokia_user_config: Jolokia user configurable settings
         :param pulumi.Input['ServiceIntegrationEndpointPrometheusUserConfigArgs'] prometheus_user_config: Prometheus user configurable settings
         :param pulumi.Input['ServiceIntegrationEndpointRsyslogUserConfigArgs'] rsyslog_user_config: Rsyslog user configurable settings
         """
         pulumi.set(__self__, "endpoint_name", endpoint_name)
         pulumi.set(__self__, "endpoint_type", endpoint_type)
@@ -181,15 +181,15 @@
     def external_kafka_user_config(self, value: Optional[pulumi.Input['ServiceIntegrationEndpointExternalKafkaUserConfigArgs']]):
         pulumi.set(self, "external_kafka_user_config", value)
 
     @property
     @pulumi.getter(name="externalOpensearchLogsUserConfig")
     def external_opensearch_logs_user_config(self) -> Optional[pulumi.Input['ServiceIntegrationEndpointExternalOpensearchLogsUserConfigArgs']]:
         """
-        ExternalOpensearchLogs user configurable settings
+        ExternalOpenSearchLogs user configurable settings
         """
         return pulumi.get(self, "external_opensearch_logs_user_config")
 
     @external_opensearch_logs_user_config.setter
     def external_opensearch_logs_user_config(self, value: Optional[pulumi.Input['ServiceIntegrationEndpointExternalOpensearchLogsUserConfigArgs']]):
         pulumi.set(self, "external_opensearch_logs_user_config", value)
 
@@ -267,15 +267,15 @@
         :param pulumi.Input[str] endpoint_name: Name of the service integration endpoint
         :param pulumi.Input[str] endpoint_type: Type of the service integration endpoint. Possible values: `datadog`, `prometheus`, `rsyslog`, `external_elasticsearch_logs`, `external_opensearch_logs`, `external_aws_cloudwatch_logs`, `external_google_cloud_logging`, `external_kafka`, `jolokia`, `external_schema_registry`, `external_aws_cloudwatch_metrics`
         :param pulumi.Input['ServiceIntegrationEndpointExternalAwsCloudwatchLogsUserConfigArgs'] external_aws_cloudwatch_logs_user_config: ExternalAwsCloudwatchLogs user configurable settings
         :param pulumi.Input['ServiceIntegrationEndpointExternalAwsCloudwatchMetricsUserConfigArgs'] external_aws_cloudwatch_metrics_user_config: ExternalAwsCloudwatchMetrics user configurable settings
         :param pulumi.Input['ServiceIntegrationEndpointExternalElasticsearchLogsUserConfigArgs'] external_elasticsearch_logs_user_config: ExternalElasticsearchLogs user configurable settings
         :param pulumi.Input['ServiceIntegrationEndpointExternalGoogleCloudLoggingUserConfigArgs'] external_google_cloud_logging_user_config: ExternalGoogleCloudLogging user configurable settings
         :param pulumi.Input['ServiceIntegrationEndpointExternalKafkaUserConfigArgs'] external_kafka_user_config: ExternalKafka user configurable settings
-        :param pulumi.Input['ServiceIntegrationEndpointExternalOpensearchLogsUserConfigArgs'] external_opensearch_logs_user_config: ExternalOpensearchLogs user configurable settings
+        :param pulumi.Input['ServiceIntegrationEndpointExternalOpensearchLogsUserConfigArgs'] external_opensearch_logs_user_config: ExternalOpenSearchLogs user configurable settings
         :param pulumi.Input['ServiceIntegrationEndpointExternalSchemaRegistryUserConfigArgs'] external_schema_registry_user_config: ExternalSchemaRegistry user configurable settings
         :param pulumi.Input['ServiceIntegrationEndpointJolokiaUserConfigArgs'] jolokia_user_config: Jolokia user configurable settings
         :param pulumi.Input[str] project: Project the service integration endpoint belongs to
         :param pulumi.Input['ServiceIntegrationEndpointPrometheusUserConfigArgs'] prometheus_user_config: Prometheus user configurable settings
         :param pulumi.Input['ServiceIntegrationEndpointRsyslogUserConfigArgs'] rsyslog_user_config: Rsyslog user configurable settings
         """
         if datadog_user_config is not None:
@@ -417,15 +417,15 @@
     def external_kafka_user_config(self, value: Optional[pulumi.Input['ServiceIntegrationEndpointExternalKafkaUserConfigArgs']]):
         pulumi.set(self, "external_kafka_user_config", value)
 
     @property
     @pulumi.getter(name="externalOpensearchLogsUserConfig")
     def external_opensearch_logs_user_config(self) -> Optional[pulumi.Input['ServiceIntegrationEndpointExternalOpensearchLogsUserConfigArgs']]:
         """
-        ExternalOpensearchLogs user configurable settings
+        ExternalOpenSearchLogs user configurable settings
         """
         return pulumi.get(self, "external_opensearch_logs_user_config")
 
     @external_opensearch_logs_user_config.setter
     def external_opensearch_logs_user_config(self, value: Optional[pulumi.Input['ServiceIntegrationEndpointExternalOpensearchLogsUserConfigArgs']]):
         pulumi.set(self, "external_opensearch_logs_user_config", value)
 
@@ -519,15 +519,15 @@
         :param pulumi.Input[str] endpoint_name: Name of the service integration endpoint
         :param pulumi.Input[str] endpoint_type: Type of the service integration endpoint. Possible values: `datadog`, `prometheus`, `rsyslog`, `external_elasticsearch_logs`, `external_opensearch_logs`, `external_aws_cloudwatch_logs`, `external_google_cloud_logging`, `external_kafka`, `jolokia`, `external_schema_registry`, `external_aws_cloudwatch_metrics`
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalAwsCloudwatchLogsUserConfigArgs']] external_aws_cloudwatch_logs_user_config: ExternalAwsCloudwatchLogs user configurable settings
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalAwsCloudwatchMetricsUserConfigArgs']] external_aws_cloudwatch_metrics_user_config: ExternalAwsCloudwatchMetrics user configurable settings
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalElasticsearchLogsUserConfigArgs']] external_elasticsearch_logs_user_config: ExternalElasticsearchLogs user configurable settings
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalGoogleCloudLoggingUserConfigArgs']] external_google_cloud_logging_user_config: ExternalGoogleCloudLogging user configurable settings
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalKafkaUserConfigArgs']] external_kafka_user_config: ExternalKafka user configurable settings
-        :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalOpensearchLogsUserConfigArgs']] external_opensearch_logs_user_config: ExternalOpensearchLogs user configurable settings
+        :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalOpensearchLogsUserConfigArgs']] external_opensearch_logs_user_config: ExternalOpenSearchLogs user configurable settings
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalSchemaRegistryUserConfigArgs']] external_schema_registry_user_config: ExternalSchemaRegistry user configurable settings
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointJolokiaUserConfigArgs']] jolokia_user_config: Jolokia user configurable settings
         :param pulumi.Input[str] project: Project the service integration endpoint belongs to
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointPrometheusUserConfigArgs']] prometheus_user_config: Prometheus user configurable settings
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointRsyslogUserConfigArgs']] rsyslog_user_config: Rsyslog user configurable settings
         """
         ...
@@ -635,15 +635,15 @@
         :param pulumi.Input[str] endpoint_name: Name of the service integration endpoint
         :param pulumi.Input[str] endpoint_type: Type of the service integration endpoint. Possible values: `datadog`, `prometheus`, `rsyslog`, `external_elasticsearch_logs`, `external_opensearch_logs`, `external_aws_cloudwatch_logs`, `external_google_cloud_logging`, `external_kafka`, `jolokia`, `external_schema_registry`, `external_aws_cloudwatch_metrics`
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalAwsCloudwatchLogsUserConfigArgs']] external_aws_cloudwatch_logs_user_config: ExternalAwsCloudwatchLogs user configurable settings
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalAwsCloudwatchMetricsUserConfigArgs']] external_aws_cloudwatch_metrics_user_config: ExternalAwsCloudwatchMetrics user configurable settings
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalElasticsearchLogsUserConfigArgs']] external_elasticsearch_logs_user_config: ExternalElasticsearchLogs user configurable settings
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalGoogleCloudLoggingUserConfigArgs']] external_google_cloud_logging_user_config: ExternalGoogleCloudLogging user configurable settings
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalKafkaUserConfigArgs']] external_kafka_user_config: ExternalKafka user configurable settings
-        :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalOpensearchLogsUserConfigArgs']] external_opensearch_logs_user_config: ExternalOpensearchLogs user configurable settings
+        :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalOpensearchLogsUserConfigArgs']] external_opensearch_logs_user_config: ExternalOpenSearchLogs user configurable settings
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalSchemaRegistryUserConfigArgs']] external_schema_registry_user_config: ExternalSchemaRegistry user configurable settings
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointJolokiaUserConfigArgs']] jolokia_user_config: Jolokia user configurable settings
         :param pulumi.Input[str] project: Project the service integration endpoint belongs to
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointPrometheusUserConfigArgs']] prometheus_user_config: Prometheus user configurable settings
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointRsyslogUserConfigArgs']] rsyslog_user_config: Rsyslog user configurable settings
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
@@ -739,15 +739,15 @@
         """
         return pulumi.get(self, "external_kafka_user_config")
 
     @property
     @pulumi.getter(name="externalOpensearchLogsUserConfig")
     def external_opensearch_logs_user_config(self) -> pulumi.Output[Optional['outputs.ServiceIntegrationEndpointExternalOpensearchLogsUserConfig']]:
         """
-        ExternalOpensearchLogs user configurable settings
+        ExternalOpenSearchLogs user configurable settings
         """
         return pulumi.get(self, "external_opensearch_logs_user_config")
 
     @property
     @pulumi.getter(name="externalSchemaRegistryUserConfig")
     def external_schema_registry_user_config(self) -> pulumi.Output[Optional['outputs.ServiceIntegrationEndpointExternalSchemaRegistryUserConfig']]:
         """
```

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/static_ip.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/static_ip.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven/transit_gateway_vpc_attachment.py` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/transit_gateway_vpc_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven.egg-info/PKG-INFO` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-aiven
-Version: 6.5.0a1689312319
+Version: 6.5.0a1689690146
 Summary: A Pulumi package for creating and managing Aiven cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-aiven
 Keywords: pulumi aiven
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_aiven-6.5.0a1689312319/pulumi_aiven.egg-info/SOURCES.txt` & `pulumi_aiven-6.5.0a1689690146/pulumi_aiven.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,15 @@
 pulumi_aiven/get_mysql_database.py
 pulumi_aiven/get_mysql_user.py
 pulumi_aiven/get_open_search.py
 pulumi_aiven/get_open_search_acl_config.py
 pulumi_aiven/get_open_search_acl_rule.py
 pulumi_aiven/get_opensearch_user.py
 pulumi_aiven/get_organization.py
+pulumi_aiven/get_organization_user.py
 pulumi_aiven/get_organizational_unit.py
 pulumi_aiven/get_pg.py
 pulumi_aiven/get_pg_database.py
 pulumi_aiven/get_pg_user.py
 pulumi_aiven/get_project.py
 pulumi_aiven/get_project_user.py
 pulumi_aiven/get_project_vpc.py
@@ -109,14 +110,15 @@
 pulumi_aiven/mysql_database.py
 pulumi_aiven/mysql_user.py
 pulumi_aiven/open_search.py
 pulumi_aiven/open_search_acl_config.py
 pulumi_aiven/open_search_acl_rule.py
 pulumi_aiven/opensearch_user.py
 pulumi_aiven/organization.py
+pulumi_aiven/organization_user.py
 pulumi_aiven/organizational_unit.py
 pulumi_aiven/outputs.py
 pulumi_aiven/pg.py
 pulumi_aiven/pg_database.py
 pulumi_aiven/pg_user.py
 pulumi_aiven/project.py
 pulumi_aiven/project_user.py
```

### Comparing `pulumi_aiven-6.5.0a1689312319/setup.py` & `pulumi_aiven-6.5.0a1689690146/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "6.5.0a1689312319"
-PLUGIN_VERSION = "6.5.0-alpha.1689312319+402bcef1"
+VERSION = "6.5.0a1689690146"
+PLUGIN_VERSION = "6.5.0-alpha.1689690146+f57acb18"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'aiven', PLUGIN_VERSION])
         except OSError as error:
```

