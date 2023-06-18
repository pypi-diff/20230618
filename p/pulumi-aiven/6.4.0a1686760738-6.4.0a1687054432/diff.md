# Comparing `tmp/pulumi_aiven-6.4.0a1686760738.tar.gz` & `tmp/pulumi_aiven-6.4.0a1687054432.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_aiven-6.4.0a1686760738.tar", last modified: Wed Jun 14 16:43:47 2023, max compression
+gzip compressed data, was "pulumi_aiven-6.4.0a1687054432.tar", last modified: Sun Jun 18 02:20:12 2023, max compression
```

## Comparing `pulumi_aiven-6.4.0a1686760738.tar` & `pulumi_aiven-6.4.0a1687054432.tar`

### file list

```diff
@@ -1,145 +1,145 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:43:47.440717 pulumi_aiven-6.4.0a1686760738/
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-14 16:43:47.440717 pulumi_aiven-6.4.0a1686760738/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:43:47.436717 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/
--rw-r--r--   0 runner    (1001) docker     (123)    15008 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   596968 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    16167 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/account.py
--rw-r--r--   0 runner    (1001) docker     (123)    36913 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/account_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/account_team.py
--rw-r--r--   0 runner    (1001) docker     (123)    17027 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/account_team_member.py
--rw-r--r--   0 runner    (1001) docker     (123)    12601 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/account_team_project.py
--rw-r--r--   0 runner    (1001) docker     (123)    15297 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/aws_privatelink.py
--rw-r--r--   0 runner    (1001) docker     (123)    18483 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/aws_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    18159 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/azure_privatelink.py
--rw-r--r--   0 runner    (1001) docker     (123)    15298 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/azure_privatelink_connection_approval.py
--rw-r--r--   0 runner    (1001) docker     (123)    24958 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/azure_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    29700 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/billing_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    74463 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/cassandra.py
--rw-r--r--   0 runner    (1001) docker     (123)    19426 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/cassandra_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    74126 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (123)    17227 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/clickhouse_database.py
--rw-r--r--   0 runner    (1001) docker     (123)    26558 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/clickhouse_grant.py
--rw-r--r--   0 runner    (1001) docker     (123)    13649 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/clickhouse_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    16426 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/clickhouse_user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:43:47.440717 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    26197 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/connection_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    74148 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/flink.py
--rw-r--r--   0 runner    (1001) docker     (123)    17471 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/flink_application.py
--rw-r--r--   0 runner    (1001) docker     (123)    30205 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/flink_application_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15247 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/gcp_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    12455 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_account_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_account_team.py
--rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_account_team_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_account_team_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_aws_privatelink.py
--rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_aws_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     7847 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_azure_privatelink.py
--rw-r--r--   0 runner    (1001) docker     (123)    10842 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_azure_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9636 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_billing_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    21868 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_cassanda.py
--rw-r--r--   0 runner    (1001) docker     (123)    21536 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_cassandra.py
--rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_cassandra_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    21612 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_clickhouse_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     7467 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_clickhouse_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     9126 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_connection_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    21292 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_flink.py
--rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_flink_application.py
--rw-r--r--   0 runner    (1001) docker     (123)    11003 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_flink_application_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_gcp_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    21396 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_grafana.py
--rw-r--r--   0 runner    (1001) docker     (123)    21473 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_influx_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_influxdb_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_influxdb_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    22261 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_kafka_acl.py
--rw-r--r--   0 runner    (1001) docker     (123)    21768 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_kafka_connect.py
--rw-r--r--   0 runner    (1001) docker     (123)    10310 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_kafka_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    22037 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_kafka_mirror_maker.py
--rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_kafka_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_kafka_schema_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_kafka_schema_registry_acl.py
--rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_kafka_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7982 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_kafka_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    21715 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_m3_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)    21228 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_m3_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_m3db_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_mirror_maker_replication_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    21304 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_my_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     6836 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_mysql_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_mysql_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    21605 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_open_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_open_search_acl_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8698 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_open_search_acl_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_opensearch_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_organizational_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)    21117 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_pg.py
--rw-r--r--   0 runner    (1001) docker     (123)     7965 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_pg_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_pg_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_project_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_project_vpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    21271 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_redis_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_service_component.py
--rw-r--r--   0 runner    (1001) docker     (123)    17872 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_service_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    15309 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_service_integration_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_transit_gateway_vpc_attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)    75717 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/grafana.py
--rw-r--r--   0 runner    (1001) docker     (123)    74178 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/influx_db.py
--rw-r--r--   0 runner    (1001) docker     (123)    16389 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/influxdb_database.py
--rw-r--r--   0 runner    (1001) docker     (123)    19380 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/influxdb_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    79009 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)    19320 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/kafka_acl.py
--rw-r--r--   0 runner    (1001) docker     (123)    77110 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/kafka_connect.py
--rw-r--r--   0 runner    (1001) docker     (123)    24756 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/kafka_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    77666 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/kafka_mirror_maker.py
--rw-r--r--   0 runner    (1001) docker     (123)    22353 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/kafka_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    14423 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/kafka_schema_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    19053 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/kafka_schema_registry_acl.py
--rw-r--r--   0 runner    (1001) docker     (123)    24119 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/kafka_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)    18906 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/kafka_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    76510 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/m3_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)    75396 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/m3_db.py
--rw-r--r--   0 runner    (1001) docker     (123)    16718 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/m3db_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    37020 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/mirror_maker_replication_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    76019 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/my_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)    17313 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/mysql_database.py
--rw-r--r--   0 runner    (1001) docker     (123)    21561 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/mysql_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    75139 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/open_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    18457 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/open_search_acl_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    22685 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/open_search_acl_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    16994 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/opensearch_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/organization.py
--rw-r--r--   0 runner    (1001) docker     (123)    10927 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/organizational_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)   892923 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    72557 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/pg.py
--rw-r--r--   0 runner    (1001) docker     (123)    22840 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/pg_database.py
--rw-r--r--   0 runner    (1001) docker     (123)    21818 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/pg_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    37913 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    13742 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/project_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/project_vpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    75515 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)    30212 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/redis_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    53125 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/service_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    52318 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/service_integration_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    14185 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/static_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)    22970 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/transit_gateway_vpc_attachment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:43:47.440717 pulumi_aiven-6.4.0a1686760738/pulumi_aiven.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-14 16:43:47.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-06-14 16:43:47.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 16:43:47.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 16:43:47.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-14 16:43:47.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-14 16:43:47.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 16:43:47.440717 pulumi_aiven-6.4.0a1686760738/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:20:12.848695 pulumi_aiven-6.4.0a1687054432/
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-18 02:20:12.848695 pulumi_aiven-6.4.0a1687054432/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:20:12.848695 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/
+-rw-r--r--   0 runner    (1001) docker     (123)    15008 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   596968 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16167 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36913 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/account_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/account_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17027 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/account_team_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12601 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/account_team_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15297 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/aws_privatelink.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18483 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/aws_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18159 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/azure_privatelink.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15298 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/azure_privatelink_connection_approval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24958 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/azure_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29700 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/billing_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74463 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/cassandra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19426 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/cassandra_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74126 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17227 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/clickhouse_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26558 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/clickhouse_grant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13649 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/clickhouse_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16426 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/clickhouse_user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:20:12.848695 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26197 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/connection_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74148 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/flink.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17471 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/flink_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30205 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/flink_application_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15247 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/gcp_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12455 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_account_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_account_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_account_team_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_account_team_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_aws_privatelink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_aws_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7847 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_azure_privatelink.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10842 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_azure_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9636 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_billing_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21868 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_cassanda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21536 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_cassandra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_cassandra_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21612 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_clickhouse_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7467 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_clickhouse_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9126 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_connection_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21292 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_flink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_flink_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11003 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_flink_application_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_gcp_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21396 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_grafana.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21473 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_influx_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_influxdb_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_influxdb_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22261 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_kafka_acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21768 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_kafka_connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10310 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_kafka_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22037 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_kafka_mirror_maker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_kafka_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_kafka_schema_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_kafka_schema_registry_acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_kafka_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7982 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_kafka_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21715 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_m3_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21228 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_m3_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_m3db_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_mirror_maker_replication_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21304 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_my_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6836 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_mysql_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_mysql_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21605 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_open_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_open_search_acl_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8698 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_open_search_acl_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_opensearch_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_organizational_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21117 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_pg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7965 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_pg_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_pg_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_project_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_project_vpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21271 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_redis_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_service_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17872 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_service_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15309 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_service_integration_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_transit_gateway_vpc_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75717 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/grafana.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74178 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/influx_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16389 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/influxdb_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19380 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/influxdb_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79009 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19320 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/kafka_acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77110 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/kafka_connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24756 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/kafka_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77666 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/kafka_mirror_maker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22353 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/kafka_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14423 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/kafka_schema_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19053 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/kafka_schema_registry_acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24119 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/kafka_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18906 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/kafka_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76510 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/m3_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75396 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/m3_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16718 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/m3db_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37020 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/mirror_maker_replication_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76019 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/my_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17313 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/mysql_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21561 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/mysql_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75139 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/open_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18457 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/open_search_acl_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22685 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/open_search_acl_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16994 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/opensearch_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10927 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/organizational_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)   892923 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72557 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/pg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22840 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/pg_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21818 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/pg_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37913 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13742 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/project_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/project_vpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    75515 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30212 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/redis_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53125 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/service_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52318 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/service_integration_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14185 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/static_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22970 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven/transit_gateway_vpc_attachment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:20:12.848695 pulumi_aiven-6.4.0a1687054432/pulumi_aiven.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/pulumi_aiven.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 02:20:12.848695 pulumi_aiven-6.4.0a1687054432/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-18 02:20:12.000000 pulumi_aiven-6.4.0a1687054432/setup.py
```

### Comparing `pulumi_aiven-6.4.0a1686760738/PKG-INFO` & `pulumi_aiven-6.4.0a1687054432/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_aiven
-Version: 6.4.0a1686760738
+Version: 6.4.0a1687054432
 Summary: A Pulumi package for creating and managing Aiven cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-aiven
 Keywords: pulumi aiven
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_aiven-6.4.0a1686760738/README.md` & `pulumi_aiven-6.4.0a1687054432/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/__init__.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/_inputs.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/_utilities.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/account.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/account.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/account_authentication.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/account_authentication.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/account_team.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/account_team.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/account_team_member.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/account_team_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/account_team_project.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/account_team_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/aws_privatelink.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/aws_privatelink.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/aws_vpc_peering_connection.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/aws_vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/azure_privatelink.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/azure_privatelink.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/azure_privatelink_connection_approval.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/azure_privatelink_connection_approval.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/azure_vpc_peering_connection.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/azure_vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/billing_group.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/billing_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/cassandra.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/cassandra.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/cassandra_user.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/cassandra_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/clickhouse.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/clickhouse.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/clickhouse_database.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/clickhouse_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/clickhouse_grant.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/clickhouse_grant.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/clickhouse_role.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/clickhouse_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/clickhouse_user.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/clickhouse_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/config/vars.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/connection_pool.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/connection_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/flink.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/flink.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/flink_application.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/flink_application.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/flink_application_version.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/flink_application_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/gcp_vpc_peering_connection.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/gcp_vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_account.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_account_authentication.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_account_authentication.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_account_team.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_account_team.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_account_team_member.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_account_team_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_account_team_project.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_account_team_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_aws_privatelink.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_aws_privatelink.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_aws_vpc_peering_connection.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_aws_vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_azure_privatelink.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_azure_privatelink.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_azure_vpc_peering_connection.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_azure_vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_billing_group.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_billing_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_cassanda.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_cassanda.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_cassandra.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_cassandra.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_cassandra_user.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_cassandra_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_clickhouse.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_clickhouse.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_clickhouse_database.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_clickhouse_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_clickhouse_user.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_clickhouse_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_connection_pool.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_connection_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_flink.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_flink.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_flink_application.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_flink_application.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_flink_application_version.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_flink_application_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_gcp_vpc_peering_connection.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_gcp_vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_grafana.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_grafana.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_influx_db.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_influx_db.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_influxdb_database.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_influxdb_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_influxdb_user.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_influxdb_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_kafka.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_kafka.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_kafka_acl.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_kafka_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_kafka_connect.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_kafka_connect.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_kafka_connector.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_kafka_connector.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_kafka_mirror_maker.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_kafka_mirror_maker.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_kafka_schema.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_kafka_schema.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_kafka_schema_configuration.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_kafka_schema_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_kafka_schema_registry_acl.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_kafka_schema_registry_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_kafka_topic.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_kafka_topic.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_kafka_user.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_kafka_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_m3_aggregator.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_m3_aggregator.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_m3_db.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_m3_db.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_m3db_user.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_m3db_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_mirror_maker_replication_flow.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_mirror_maker_replication_flow.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_my_sql.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_my_sql.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_mysql_database.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_mysql_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_mysql_user.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_mysql_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_open_search.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_open_search.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_open_search_acl_config.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_open_search_acl_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_open_search_acl_rule.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_open_search_acl_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_opensearch_user.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_opensearch_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_organization.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_organization.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_organizational_unit.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_organizational_unit.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_pg.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_pg.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_pg_database.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_pg_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_pg_user.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_pg_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_project.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_project_user.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_project_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_project_vpc.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_project_vpc.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_redis.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_redis.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_redis_user.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_redis_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_service_component.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_service_component.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_service_integration.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_service_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_service_integration_endpoint.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_service_integration_endpoint.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_transit_gateway_vpc_attachment.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/get_transit_gateway_vpc_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/grafana.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/grafana.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/influx_db.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/influx_db.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/influxdb_database.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/influxdb_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/influxdb_user.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/influxdb_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/kafka.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/kafka.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/kafka_acl.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/kafka_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/kafka_connect.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/kafka_connect.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/kafka_connector.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/kafka_connector.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/kafka_mirror_maker.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/kafka_mirror_maker.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/kafka_schema.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/kafka_schema.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/kafka_schema_configuration.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/kafka_schema_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/kafka_schema_registry_acl.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/kafka_schema_registry_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/kafka_topic.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/kafka_topic.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/kafka_user.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/kafka_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/m3_aggregator.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/m3_aggregator.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/m3_db.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/m3_db.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/m3db_user.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/m3db_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/mirror_maker_replication_flow.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/mirror_maker_replication_flow.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/my_sql.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/my_sql.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/mysql_database.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/mysql_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/mysql_user.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/mysql_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/open_search.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/open_search.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/open_search_acl_config.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/open_search_acl_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/open_search_acl_rule.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/open_search_acl_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/opensearch_user.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/opensearch_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/organization.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/organization.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/organizational_unit.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/organizational_unit.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/outputs.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/pg.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/pg.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/pg_database.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/pg_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/pg_user.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/pg_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/project.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/project.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/project_user.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/project_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/project_vpc.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/project_vpc.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/provider.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/redis.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/redis.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/redis_user.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/redis_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/service_integration.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/service_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/service_integration_endpoint.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/service_integration_endpoint.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/static_ip.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/static_ip.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/transit_gateway_vpc_attachment.py` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven/transit_gateway_vpc_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven.egg-info/PKG-INFO` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-aiven
-Version: 6.4.0a1686760738
+Version: 6.4.0a1687054432
 Summary: A Pulumi package for creating and managing Aiven cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-aiven
 Keywords: pulumi aiven
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_aiven-6.4.0a1686760738/pulumi_aiven.egg-info/SOURCES.txt` & `pulumi_aiven-6.4.0a1687054432/pulumi_aiven.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686760738/setup.py` & `pulumi_aiven-6.4.0a1687054432/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "6.4.0a1686760738"
-PLUGIN_VERSION = "6.4.0-alpha.1686760738+a70dcde0"
+VERSION = "6.4.0a1687054432"
+PLUGIN_VERSION = "6.4.0-alpha.1687054432+6d506b3c"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'aiven', PLUGIN_VERSION])
         except OSError as error:
```

