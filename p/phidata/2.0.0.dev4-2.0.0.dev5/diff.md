# Comparing `tmp/phidata-2.0.0.dev4.tar.gz` & `tmp/phidata-2.0.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phidata-2.0.0.dev4.tar", last modified: Wed Jul 12 13:31:03 2023, max compression
+gzip compressed data, was "phidata-2.0.0.dev5.tar", last modified: Tue Jul 18 13:46:12 2023, max compression
```

## Comparing `phidata-2.0.0.dev4.tar` & `phidata-2.0.0.dev5.tar`

### file list

```diff
@@ -1,738 +1,751 @@
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.770704 phidata-2.0.0.dev4/
--rw-r--r--   0 zu         (501) staff       (20)    16759 2022-11-08 02:12:00.000000 phidata-2.0.0.dev4/LICENSE
--rw-r--r--   0 zu         (501) staff       (20)     3126 2023-07-12 13:31:03.770557 phidata-2.0.0.dev4/PKG-INFO
--rw-r--r--   0 zu         (501) staff       (20)     2742 2023-06-21 12:59:34.000000 phidata-2.0.0.dev4/README.md
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.648776 phidata-2.0.0.dev4/phi/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.650007 phidata-2.0.0.dev4/phi/api/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/api/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1684 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/api/client.py
--rw-r--r--   0 zu         (501) staff       (20)      843 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/api/helpers.py
--rw-r--r--   0 zu         (501) staff       (20)      794 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/api/routes.py
--rw-r--r--   0 zu         (501) staff       (20)     4464 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/api/user.py
--rw-r--r--   0 zu         (501) staff       (20)     7188 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/api/workspace.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.650307 phidata-2.0.0.dev4/phi/aws/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1310 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/api_client.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.650880 phidata-2.0.0.dev4/phi/aws/app/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/app/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    26919 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/app/base.py
--rw-r--r--   0 zu         (501) staff       (20)      171 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/app/context.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.651241 phidata-2.0.0.dev4/phi/aws/app/fastapi/
--rw-r--r--   0 zu         (501) staff       (20)       84 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/app/fastapi/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      766 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/app/fastapi/fastapi.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.651581 phidata-2.0.0.dev4/phi/aws/app/jupyter/
--rw-r--r--   0 zu         (501) staff       (20)       84 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/app/jupyter/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     2862 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/app/jupyter/jupyter.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.651889 phidata-2.0.0.dev4/phi/aws/app/qdrant/
--rw-r--r--   0 zu         (501) staff       (20)       81 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/app/qdrant/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      649 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/app/qdrant/qdrant.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.652164 phidata-2.0.0.dev4/phi/aws/app/streamlit/
--rw-r--r--   0 zu         (501) staff       (20)       90 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/app/streamlit/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      735 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/app/streamlit/streamlit.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.654912 phidata-2.0.0.dev4/phi/aws/resource/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/resource/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.655244 phidata-2.0.0.dev4/phi/aws/resource/acm/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/resource/acm/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    10489 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/resource/acm/certificate.py
--rw-r--r--   0 zu         (501) staff       (20)     8725 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/resource/base.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.655511 phidata-2.0.0.dev4/phi/aws/resource/cloudformation/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/resource/cloudformation/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    10247 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/resource/cloudformation/stack.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.656326 phidata-2.0.0.dev4/phi/aws/resource/ec2/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/resource/ec2/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    21177 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/resource/ec2/security_group.py
--rw-r--r--   0 zu         (501) staff       (20)     2427 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/resource/ec2/subnet.py
--rw-r--r--   0 zu         (501) staff       (20)    11791 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/resource/ec2/volume.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.657310 phidata-2.0.0.dev4/phi/aws/resource/ecs/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/resource/ecs/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     6316 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/resource/ecs/cluster.py
--rw-r--r--   0 zu         (501) staff       (20)    11368 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/resource/ecs/container.py
--rw-r--r--   0 zu         (501) staff       (20)    19592 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/resource/ecs/service.py
--rw-r--r--   0 zu         (501) staff       (20)    21760 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/resource/ecs/task_definition.py
--rw-r--r--   0 zu         (501) staff       (20)     3385 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/resource/ecs/volume.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.658413 phidata-2.0.0.dev4/phi/aws/resource/eks/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/resource/eks/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     7252 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/resource/eks/addon.py
--rw-r--r--   0 zu         (501) staff       (20)    29689 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/resource/eks/cluster.py
--rw-r--r--   0 zu         (501) staff       (20)    13244 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/resource/eks/fargate_profile.py
--rw-r--r--   0 zu         (501) staff       (20)    24791 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/resource/eks/kubeconfig.py
--rw-r--r--   0 zu         (501) staff       (20)    23405 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/resource/eks/node_group.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.658954 phidata-2.0.0.dev4/phi/aws/resource/elasticache/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/resource/elasticache/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    15451 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/resource/elasticache/cluster.py
--rw-r--r--   0 zu         (501) staff       (20)     5922 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/resource/elasticache/subnet_group.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.659535 phidata-2.0.0.dev4/phi/aws/resource/elb/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/resource/elb/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    10268 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/resource/elb/listener.py
--rw-r--r--   0 zu         (501) staff       (20)     7618 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/resource/elb/load_balancer.py
--rw-r--r--   0 zu         (501) staff       (20)     9507 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/resource/elb/target_group.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.659771 phidata-2.0.0.dev4/phi/aws/resource/emr/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/resource/emr/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    12578 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/resource/emr/cluster.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.660002 phidata-2.0.0.dev4/phi/aws/resource/glue/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/resource/glue/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    12558 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/resource/glue/crawler.py
--rw-r--r--   0 zu         (501) staff       (20)    23734 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/resource/group.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.660354 phidata-2.0.0.dev4/phi/aws/resource/iam/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/resource/iam/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     7481 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/resource/iam/policy.py
--rw-r--r--   0 zu         (501) staff       (20)     9714 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/resource/iam/role.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.660989 phidata-2.0.0.dev4/phi/aws/resource/rds/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/resource/rds/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    35097 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/resource/rds/db_cluster.py
--rw-r--r--   0 zu         (501) staff       (20)    34346 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/resource/rds/db_instance.py
--rw-r--r--   0 zu         (501) staff       (20)     7611 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/resource/rds/db_subnet_group.py
--rw-r--r--   0 zu         (501) staff       (20)      290 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/resource/reference.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.661219 phidata-2.0.0.dev4/phi/aws/resource/s3/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/resource/s3/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     6400 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/resource/s3/bucket.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.661598 phidata-2.0.0.dev4/phi/aws/resource/secret/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/resource/secret/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    11028 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/resource/secret/manager.py
--rw-r--r--   0 zu         (501) staff       (20)      999 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/resource/secret/reader.py
--rw-r--r--   0 zu         (501) staff       (20)     3475 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/aws/resource/types.py
--rw-r--r--   0 zu         (501) staff       (20)     5696 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/base.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.662892 phidata-2.0.0.dev4/phi/cli/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/cli/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     3667 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/cli/auth_server.py
--rw-r--r--   0 zu         (501) staff       (20)    13385 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/cli/config.py
--rw-r--r--   0 zu         (501) staff       (20)     3316 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/cli/console.py
--rw-r--r--   0 zu         (501) staff       (20)      833 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/cli/credentials.py
--rw-r--r--   0 zu         (501) staff       (20)    20599 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/cli/entrypoint.py
--rw-r--r--   0 zu         (501) staff       (20)    15893 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/cli/operator.py
--rw-r--r--   0 zu         (501) staff       (20)     2045 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/cli/settings.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.663261 phidata-2.0.0.dev4/phi/cli/ws/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/cli/ws/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    27120 2023-07-12 13:27:33.000000 phidata-2.0.0.dev4/phi/cli/ws/ws_cli.py
--rw-r--r--   0 zu         (501) staff       (20)      696 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/constants.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.663514 phidata-2.0.0.dev4/phi/docker/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/docker/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1150 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/docker/api_client.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.664016 phidata-2.0.0.dev4/phi/docker/app/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/docker/app/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    14659 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/docker/app/base.py
--rw-r--r--   0 zu         (501) staff       (20)       87 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/docker/app/context.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.664324 phidata-2.0.0.dev4/phi/docker/app/django/
--rw-r--r--   0 zu         (501) staff       (20)       84 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/docker/app/django/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      917 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/docker/app/django/django.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.664688 phidata-2.0.0.dev4/phi/docker/app/fastapi/
--rw-r--r--   0 zu         (501) staff       (20)       87 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/docker/app/fastapi/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      932 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/docker/app/fastapi/fastapi.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.665193 phidata-2.0.0.dev4/phi/docker/app/jupyter/
--rw-r--r--   0 zu         (501) staff       (20)       87 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/docker/app/jupyter/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     3275 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/docker/app/jupyter/jupyter.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.668359 phidata-2.0.0.dev4/phi/docker/app/postgres/
--rw-r--r--   0 zu         (501) staff       (20)      148 2023-07-11 23:42:39.000000 phidata-2.0.0.dev4/phi/docker/app/postgres/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      232 2023-07-11 23:42:39.000000 phidata-2.0.0.dev4/phi/docker/app/postgres/pgvector.py
--rw-r--r--   0 zu         (501) staff       (20)     4740 2023-07-11 23:42:39.000000 phidata-2.0.0.dev4/phi/docker/app/postgres/postgres.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.668988 phidata-2.0.0.dev4/phi/docker/app/qdrant/
--rw-r--r--   0 zu         (501) staff       (20)       84 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/docker/app/qdrant/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      731 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/docker/app/qdrant/qdrant.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.669530 phidata-2.0.0.dev4/phi/docker/app/streamlit/
--rw-r--r--   0 zu         (501) staff       (20)       93 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/docker/app/streamlit/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      901 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/docker/app/streamlit/streamlit.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.673543 phidata-2.0.0.dev4/phi/docker/resource/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/docker/resource/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     4871 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/docker/resource/base.py
--rw-r--r--   0 zu         (501) staff       (20)    15125 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/docker/resource/container.py
--rw-r--r--   0 zu         (501) staff       (20)    21704 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/docker/resource/group.py
--rw-r--r--   0 zu         (501) staff       (20)    14791 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/docker/resource/image.py
--rw-r--r--   0 zu         (501) staff       (20)     5126 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/docker/resource/network.py
--rw-r--r--   0 zu         (501) staff       (20)     1130 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/docker/resource/types.py
--rw-r--r--   0 zu         (501) staff       (20)     4785 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/docker/resource/volume.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.673869 phidata-2.0.0.dev4/phi/document/
--rw-r--r--   0 zu         (501) staff       (20)       39 2023-07-11 23:42:39.000000 phidata-2.0.0.dev4/phi/document/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      314 2023-07-11 23:42:39.000000 phidata-2.0.0.dev4/phi/document/base.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.674346 phidata-2.0.0.dev4/phi/document/reader/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-11 23:42:39.000000 phidata-2.0.0.dev4/phi/document/reader/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     2763 2023-07-11 23:42:39.000000 phidata-2.0.0.dev4/phi/document/reader/base.py
--rw-r--r--   0 zu         (501) staff       (20)     1664 2023-07-11 23:42:39.000000 phidata-2.0.0.dev4/phi/document/reader/pdf.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.674667 phidata-2.0.0.dev4/phi/document/table/
--rw-r--r--   0 zu         (501) staff       (20)       71 2023-07-12 10:43:33.000000 phidata-2.0.0.dev4/phi/document/table/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1346 2023-07-12 13:30:43.000000 phidata-2.0.0.dev4/phi/document/table/base.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.674906 phidata-2.0.0.dev4/phi/infra/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/infra/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.675615 phidata-2.0.0.dev4/phi/infra/app/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/infra/app/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    13633 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/infra/app/base.py
--rw-r--r--   0 zu         (501) staff       (20)      522 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/infra/app/context.py
--rw-r--r--   0 zu         (501) staff       (20)     1253 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/infra/app/db_app.py
--rw-r--r--   0 zu         (501) staff       (20)      126 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/infra/enums.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.676114 phidata-2.0.0.dev4/phi/infra/resource/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/infra/resource/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     6896 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/infra/resource/base.py
--rw-r--r--   0 zu         (501) staff       (20)     1679 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/infra/resource/group.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.676295 phidata-2.0.0.dev4/phi/k8s/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/k8s/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.676439 phidata-2.0.0.dev4/phi/llm/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/llm/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.676856 phidata-2.0.0.dev4/phi/llm/conversation/
--rw-r--r--   0 zu         (501) staff       (20)       49 2023-07-11 23:42:39.000000 phidata-2.0.0.dev4/phi/llm/conversation/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-12 08:45:16.000000 phidata-2.0.0.dev4/phi/llm/conversation/db.py
--rw-r--r--   0 zu         (501) staff       (20)      151 2023-07-11 23:42:39.000000 phidata-2.0.0.dev4/phi/llm/conversation/schemas.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.677612 phidata-2.0.0.dev4/phi/schemas/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/schemas/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      208 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/schemas/response.py
--rw-r--r--   0 zu         (501) staff       (20)     1484 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/schemas/user.py
--rw-r--r--   0 zu         (501) staff       (20)      677 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/schemas/workspace.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.677901 phidata-2.0.0.dev4/phi/table/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-12 08:48:17.000000 phidata-2.0.0.dev4/phi/table/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.678147 phidata-2.0.0.dev4/phi/table/sql/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-12 08:48:27.000000 phidata-2.0.0.dev4/phi/table/sql/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      403 2023-07-12 08:49:04.000000 phidata-2.0.0.dev4/phi/table/sql/base.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.680924 phidata-2.0.0.dev4/phi/utils/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/utils/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      747 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/utils/common.py
--rw-r--r--   0 zu         (501) staff       (20)     1342 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/utils/defaults.py
--rw-r--r--   0 zu         (501) staff       (20)      120 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/utils/dttm.py
--rw-r--r--   0 zu         (501) staff       (20)     1020 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/utils/filesystem.py
--rw-r--r--   0 zu         (501) staff       (20)     1640 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/utils/git.py
--rw-r--r--   0 zu         (501) staff       (20)      889 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/utils/json_io.py
--rw-r--r--   0 zu         (501) staff       (20)      665 2023-07-12 13:19:56.000000 phidata-2.0.0.dev4/phi/utils/load_env.py
--rw-r--r--   0 zu         (501) staff       (20)     1009 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/utils/log.py
--rw-r--r--   0 zu         (501) staff       (20)     1010 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/utils/pickle.py
--rw-r--r--   0 zu         (501) staff       (20)      724 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/utils/py_io.py
--rw-r--r--   0 zu         (501) staff       (20)      589 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/utils/pyproject.py
--rw-r--r--   0 zu         (501) staff       (20)      962 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/utils/resource_filter.py
--rw-r--r--   0 zu         (501) staff       (20)      829 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/utils/yaml_io.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.681091 phidata-2.0.0.dev4/phi/vectordb/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-11 23:42:39.000000 phidata-2.0.0.dev4/phi/vectordb/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.681221 phidata-2.0.0.dev4/phi/vectordb/pgvector/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-11 23:42:39.000000 phidata-2.0.0.dev4/phi/vectordb/pgvector/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.682184 phidata-2.0.0.dev4/phi/workspace/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/workspace/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     9927 2023-07-12 13:25:30.000000 phidata-2.0.0.dev4/phi/workspace/config.py
--rw-r--r--   0 zu         (501) staff       (20)      321 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/workspace/enums.py
--rw-r--r--   0 zu         (501) staff       (20)     1914 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/workspace/helpers.py
--rw-r--r--   0 zu         (501) staff       (20)    20826 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/workspace/operator.py
--rw-r--r--   0 zu         (501) staff       (20)     9063 2023-07-11 15:02:10.000000 phidata-2.0.0.dev4/phi/workspace/settings.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.682678 phidata-2.0.0.dev4/phidata/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-02-28 02:08:34.000000 phidata-2.0.0.dev4/phidata/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.683969 phidata-2.0.0.dev4/phidata/airflow/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev4/phidata/airflow/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      140 2022-10-01 00:05:40.000000 phidata-2.0.0.dev4/phidata/airflow/airflow_installed.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.684391 phidata-2.0.0.dev4/phidata/airflow/operators/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev4/phidata/airflow/operators/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      584 2022-04-18 19:05:50.000000 phidata-2.0.0.dev4/phidata/airflow/operators/empty.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.686962 phidata-2.0.0.dev4/phidata/app/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-10-28 00:34:05.000000 phidata-2.0.0.dev4/phidata/app/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.689776 phidata-2.0.0.dev4/phidata/app/airflow/
--rw-r--r--   0 zu         (501) staff       (20)      385 2022-11-02 02:52:41.000000 phidata-2.0.0.dev4/phidata/app/airflow/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)   100927 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/app/airflow/airflow_base.py
--rw-r--r--   0 zu         (501) staff       (20)    30469 2023-06-15 14:48:05.000000 phidata-2.0.0.dev4/phidata/app/airflow/airflow_flower.py
--rw-r--r--   0 zu         (501) staff       (20)    30508 2023-06-15 14:48:05.000000 phidata-2.0.0.dev4/phidata/app/airflow/airflow_manager.py
--rw-r--r--   0 zu         (501) staff       (20)    30505 2023-06-15 14:48:05.000000 phidata-2.0.0.dev4/phidata/app/airflow/airflow_scheduler.py
--rw-r--r--   0 zu         (501) staff       (20)    30515 2023-06-15 14:48:05.000000 phidata-2.0.0.dev4/phidata/app/airflow/airflow_webserver.py
--rw-r--r--   0 zu         (501) staff       (20)    30710 2023-06-15 14:48:05.000000 phidata-2.0.0.dev4/phidata/app/airflow/airflow_worker.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.690326 phidata-2.0.0.dev4/phidata/app/alertmanager/
--rw-r--r--   0 zu         (501) staff       (20)      134 2023-03-11 17:22:33.000000 phidata-2.0.0.dev4/phidata/app/alertmanager/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    47889 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/app/alertmanager/alertmanager.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.691377 phidata-2.0.0.dev4/phidata/app/amundsen/
--rw-r--r--   0 zu         (501) staff       (20)      398 2023-03-11 17:40:59.000000 phidata-2.0.0.dev4/phidata/app/amundsen/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    48031 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/app/amundsen/frontend.py
--rw-r--r--   0 zu         (501) staff       (20)    48032 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/app/amundsen/metadata.py
--rw-r--r--   0 zu         (501) staff       (20)    47944 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/app/amundsen/search.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.691842 phidata-2.0.0.dev4/phidata/app/assistant/
--rw-r--r--   0 zu         (501) staff       (20)      139 2023-01-15 00:33:10.000000 phidata-2.0.0.dev4/phidata/app/assistant/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    49912 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/app/assistant/assistant.py
--rw-r--r--   0 zu         (501) staff       (20)    30166 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/app/aws_app.py
--rw-r--r--   0 zu         (501) staff       (20)    17164 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/app/base_app.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.692335 phidata-2.0.0.dev4/phidata/app/cadvisor/
--rw-r--r--   0 zu         (501) staff       (20)      118 2023-03-11 17:22:33.000000 phidata-2.0.0.dev4/phidata/app/cadvisor/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    49678 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/app/cadvisor/cadvisor.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.693237 phidata-2.0.0.dev4/phidata/app/databox/
--rw-r--r--   0 zu         (501) staff       (20)      157 2023-01-15 00:32:07.000000 phidata-2.0.0.dev4/phidata/app/databox/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    86151 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/app/databox/databox.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.694338 phidata-2.0.0.dev4/phidata/app/db/
--rw-r--r--   0 zu         (501) staff       (20)       52 2022-03-29 16:28:05.000000 phidata-2.0.0.dev4/phidata/app/db/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     3187 2023-01-05 15:43:33.000000 phidata-2.0.0.dev4/phidata/app/db/base_db.py
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-04 16:30:27.000000 phidata-2.0.0.dev4/phidata/app/db/db_app.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.695120 phidata-2.0.0.dev4/phidata/app/django/
--rw-r--r--   0 zu         (501) staff       (20)      105 2023-05-18 09:49:43.000000 phidata-2.0.0.dev4/phidata/app/django/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    27483 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/app/django/django_app.py
--rw-r--r--   0 zu         (501) staff       (20)    30070 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/app/django/django_backup.py
--rw-r--r--   0 zu         (501) staff       (20)    17172 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/app/docker_app.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.695825 phidata-2.0.0.dev4/phidata/app/elastic/
--rw-r--r--   0 zu         (501) staff       (20)       71 2022-02-28 02:08:34.000000 phidata-2.0.0.dev4/phidata/app/elastic/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     3723 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/app/elastic/elastic_app.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.696258 phidata-2.0.0.dev4/phidata/app/elasticsearch/
--rw-r--r--   0 zu         (501) staff       (20)      138 2023-03-11 17:22:33.000000 phidata-2.0.0.dev4/phidata/app/elasticsearch/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    48675 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/app/elasticsearch/elasticsearch.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.696993 phidata-2.0.0.dev4/phidata/app/fastapi/
--rw-r--r--   0 zu         (501) staff       (20)      175 2023-06-15 14:48:05.000000 phidata-2.0.0.dev4/phidata/app/fastapi/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    20266 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/app/fastapi/fastapi_server.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.697619 phidata-2.0.0.dev4/phidata/app/grafana/
--rw-r--r--   0 zu         (501) staff       (20)      114 2023-03-11 17:22:33.000000 phidata-2.0.0.dev4/phidata/app/grafana/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    49781 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/app/grafana/grafana.py
--rw-r--r--   0 zu         (501) staff       (20)      822 2023-06-15 14:48:05.000000 phidata-2.0.0.dev4/phidata/app/group.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.698806 phidata-2.0.0.dev4/phidata/app/jupyter/
--rw-r--r--   0 zu         (501) staff       (20)      273 2023-06-15 14:48:05.000000 phidata-2.0.0.dev4/phidata/app/jupyter/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    27093 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/app/jupyter/jupyter.py
--rw-r--r--   0 zu         (501) staff       (20)    46942 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/app/jupyter/jupyter_hub.py
--rw-r--r--   0 zu         (501) staff       (20)    93432 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/app/jupyter/jupyter_lab.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.699620 phidata-2.0.0.dev4/phidata/app/k8s/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-05-24 02:25:43.000000 phidata-2.0.0.dev4/phidata/app/k8s/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     3930 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/app/k8s/app.py
--rw-r--r--   0 zu         (501) staff       (20)     1766 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/app/k8s/dir.py
--rw-r--r--   0 zu         (501) staff       (20)     6550 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/app/k8s/url.py
--rw-r--r--   0 zu         (501) staff       (20)    37830 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/app/k8s_app.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.700037 phidata-2.0.0.dev4/phidata/app/mysql/
--rw-r--r--   0 zu         (501) staff       (20)      151 2023-05-03 15:21:14.000000 phidata-2.0.0.dev4/phidata/app/mysql/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    49110 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/app/mysql/mysql_db.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.700429 phidata-2.0.0.dev4/phidata/app/neo4j/
--rw-r--r--   0 zu         (501) staff       (20)      106 2023-03-11 17:22:33.000000 phidata-2.0.0.dev4/phidata/app/neo4j/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    47856 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/app/neo4j/neo4j.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.700849 phidata-2.0.0.dev4/phidata/app/nodeexporter/
--rw-r--r--   0 zu         (501) staff       (20)      134 2023-03-11 17:22:33.000000 phidata-2.0.0.dev4/phidata/app/nodeexporter/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    47898 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/app/nodeexporter/nodeexporter.py
--rw-r--r--   0 zu         (501) staff       (20)    38495 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/app/phidata_app.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.701404 phidata-2.0.0.dev4/phidata/app/postgres/
--rw-r--r--   0 zu         (501) staff       (20)      166 2023-01-15 00:33:00.000000 phidata-2.0.0.dev4/phidata/app/postgres/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    53156 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/app/postgres/postgres_db.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.701893 phidata-2.0.0.dev4/phidata/app/prometheus/
--rw-r--r--   0 zu         (501) staff       (20)      126 2023-03-11 17:22:33.000000 phidata-2.0.0.dev4/phidata/app/prometheus/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    49051 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/app/prometheus/prometheus.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.702370 phidata-2.0.0.dev4/phidata/app/qdrant/
--rw-r--r--   0 zu         (501) staff       (20)      110 2023-06-15 14:48:05.000000 phidata-2.0.0.dev4/phidata/app/qdrant/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    12372 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/app/qdrant/qdrant.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.703035 phidata-2.0.0.dev4/phidata/app/redis/
--rw-r--r--   0 zu         (501) staff       (20)      144 2023-01-15 00:32:35.000000 phidata-2.0.0.dev4/phidata/app/redis/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    49058 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/app/redis/redis.py
--rw-r--r--   0 zu         (501) staff       (20)    53296 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/app/redis/stack.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.704265 phidata-2.0.0.dev4/phidata/app/server/
--rw-r--r--   0 zu         (501) staff       (20)      207 2023-05-18 09:49:43.000000 phidata-2.0.0.dev4/phidata/app/server/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    18424 2023-06-15 14:48:05.000000 phidata-2.0.0.dev4/phidata/app/server/api_server.py
--rw-r--r--   0 zu         (501) staff       (20)    58714 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/app/server/server_base.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.705629 phidata-2.0.0.dev4/phidata/app/spark/
--rw-r--r--   0 zu         (501) staff       (20)      193 2023-02-07 16:41:27.000000 phidata-2.0.0.dev4/phidata/app/spark/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    49424 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/app/spark/spark_base.py
--rw-r--r--   0 zu         (501) staff       (20)    17222 2023-06-15 14:48:05.000000 phidata-2.0.0.dev4/phidata/app/spark/spark_driver.py
--rw-r--r--   0 zu         (501) staff       (20)    17332 2023-06-15 14:48:05.000000 phidata-2.0.0.dev4/phidata/app/spark/spark_worker.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.706175 phidata-2.0.0.dev4/phidata/app/streamlit/
--rw-r--r--   0 zu         (501) staff       (20)      174 2023-06-15 14:48:05.000000 phidata-2.0.0.dev4/phidata/app/streamlit/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    20207 2023-06-20 14:11:22.000000 phidata-2.0.0.dev4/phidata/app/streamlit/streamlit_app.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.709392 phidata-2.0.0.dev4/phidata/app/superset/
--rw-r--r--   0 zu         (501) staff       (20)      411 2022-11-02 02:52:41.000000 phidata-2.0.0.dev4/phidata/app/superset/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    71570 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/app/superset/superset_base.py
--rw-r--r--   0 zu         (501) staff       (20)    22925 2023-06-15 14:48:05.000000 phidata-2.0.0.dev4/phidata/app/superset/superset_init.py
--rw-r--r--   0 zu         (501) staff       (20)    22910 2023-06-15 14:48:05.000000 phidata-2.0.0.dev4/phidata/app/superset/superset_webserver.py
--rw-r--r--   0 zu         (501) staff       (20)    22910 2023-06-15 14:48:05.000000 phidata-2.0.0.dev4/phidata/app/superset/superset_worker.py
--rw-r--r--   0 zu         (501) staff       (20)    22917 2023-06-15 14:48:05.000000 phidata-2.0.0.dev4/phidata/app/superset/superset_worker_beat.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.710585 phidata-2.0.0.dev4/phidata/app/traefik/
--rw-r--r--   0 zu         (501) staff       (20)      173 2023-01-15 00:32:52.000000 phidata-2.0.0.dev4/phidata/app/traefik/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)   115905 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/app/traefik/crds.py
--rw-r--r--   0 zu         (501) staff       (20)    48190 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/app/traefik/ingress_route.py
--rw-r--r--   0 zu         (501) staff       (20)    44972 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/app/traefik/router.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.710894 phidata-2.0.0.dev4/phidata/asset/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/asset/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.711233 phidata-2.0.0.dev4/phidata/asset/aws/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/asset/aws/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     3210 2023-06-15 14:48:05.000000 phidata-2.0.0.dev4/phidata/asset/aws/aws_asset.py
--rw-r--r--   0 zu         (501) staff       (20)    24787 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/asset/data_asset.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.712172 phidata-2.0.0.dev4/phidata/asset/local/
--rw-r--r--   0 zu         (501) staff       (20)       71 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/asset/local/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    14564 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/asset/local/file.py
--rw-r--r--   0 zu         (501) staff       (20)      574 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/asset/local/local_asset.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.713919 phidata-2.0.0.dev4/phidata/aws/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/aws/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1835 2023-03-13 15:21:09.000000 phidata-2.0.0.dev4/phidata/aws/api_client.py
--rw-r--r--   0 zu         (501) staff       (20)      487 2023-06-15 14:48:05.000000 phidata-2.0.0.dev4/phidata/aws/args.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.714331 phidata-2.0.0.dev4/phidata/aws/athena/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/aws/athena/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     8186 2023-03-13 15:21:09.000000 phidata-2.0.0.dev4/phidata/aws/athena/query.py
--rw-r--r--   0 zu         (501) staff       (20)     3168 2023-06-15 14:48:05.000000 phidata-2.0.0.dev4/phidata/aws/config.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.714575 phidata-2.0.0.dev4/phidata/aws/create/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/aws/create/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.714912 phidata-2.0.0.dev4/phidata/aws/create/iam/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/aws/create/iam/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     3233 2023-03-13 15:21:09.000000 phidata-2.0.0.dev4/phidata/aws/create/iam/eks_admin_role.py
--rw-r--r--   0 zu         (501) staff       (20)     2472 2023-03-13 15:21:09.000000 phidata-2.0.0.dev4/phidata/aws/create/iam/role.py
--rw-r--r--   0 zu         (501) staff       (20)    23058 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/aws/driver.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.715338 phidata-2.0.0.dev4/phidata/aws/enums/
--rw-r--r--   0 zu         (501) staff       (20)       62 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/aws/enums/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1083 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/aws/enums/manager_status.py
--rw-r--r--   0 zu         (501) staff       (20)      304 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/aws/exceptions.py
--rw-r--r--   0 zu         (501) staff       (20)     8588 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/aws/manager.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.716101 phidata-2.0.0.dev4/phidata/aws/resource/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/aws/resource/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.716326 phidata-2.0.0.dev4/phidata/aws/resource/acm/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/aws/resource/acm/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    10630 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/aws/resource/acm/certificate.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.716545 phidata-2.0.0.dev4/phidata/aws/resource/athena/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/aws/resource/athena/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     8005 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/aws/resource/athena/query.py
--rw-r--r--   0 zu         (501) staff       (20)     9127 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/aws/resource/base.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.716764 phidata-2.0.0.dev4/phidata/aws/resource/cloudformation/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/aws/resource/cloudformation/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    10882 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/aws/resource/cloudformation/stack.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.717353 phidata-2.0.0.dev4/phidata/aws/resource/ec2/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/aws/resource/ec2/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    21341 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/aws/resource/ec2/security_group.py
--rw-r--r--   0 zu         (501) staff       (20)     2563 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/aws/resource/ec2/subnet.py
--rw-r--r--   0 zu         (501) staff       (20)    11801 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/aws/resource/ec2/volume.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.718617 phidata-2.0.0.dev4/phidata/aws/resource/ecs/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/aws/resource/ecs/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     6140 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/aws/resource/ecs/cluster.py
--rw-r--r--   0 zu         (501) staff       (20)    26253 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/aws/resource/ecs/container.py
--rw-r--r--   0 zu         (501) staff       (20)    19630 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/aws/resource/ecs/service.py
--rw-r--r--   0 zu         (501) staff       (20)    22397 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/aws/resource/ecs/task_definition.py
--rw-r--r--   0 zu         (501) staff       (20)     3614 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/aws/resource/ecs/volume.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.719869 phidata-2.0.0.dev4/phidata/aws/resource/eks/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/aws/resource/eks/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     7390 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/aws/resource/eks/addon.py
--rw-r--r--   0 zu         (501) staff       (20)    30104 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/aws/resource/eks/cluster.py
--rw-r--r--   0 zu         (501) staff       (20)    13731 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/aws/resource/eks/fargate_profile.py
--rw-r--r--   0 zu         (501) staff       (20)    23785 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/aws/resource/eks/kubeconfig.py
--rw-r--r--   0 zu         (501) staff       (20)    23742 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/aws/resource/eks/node_group.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.720316 phidata-2.0.0.dev4/phidata/aws/resource/elasticache/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/aws/resource/elasticache/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    15823 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/aws/resource/elasticache/cluster.py
--rw-r--r--   0 zu         (501) staff       (20)     6305 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/aws/resource/elasticache/subnet_group.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.720965 phidata-2.0.0.dev4/phidata/aws/resource/elb/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-04-07 15:40:41.000000 phidata-2.0.0.dev4/phidata/aws/resource/elb/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    10727 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/aws/resource/elb/listener.py
--rw-r--r--   0 zu         (501) staff       (20)     7994 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/aws/resource/elb/load_balancer.py
--rw-r--r--   0 zu         (501) staff       (20)     9834 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/aws/resource/elb/target_group.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.721224 phidata-2.0.0.dev4/phidata/aws/resource/emr/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/aws/resource/emr/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    12806 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/aws/resource/emr/cluster.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.721571 phidata-2.0.0.dev4/phidata/aws/resource/glue/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/aws/resource/glue/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    12850 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/aws/resource/glue/crawler.py
--rw-r--r--   0 zu         (501) staff       (20)     3418 2023-06-20 14:11:22.000000 phidata-2.0.0.dev4/phidata/aws/resource/group.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.722263 phidata-2.0.0.dev4/phidata/aws/resource/iam/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/aws/resource/iam/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     9958 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/aws/resource/iam/group.py
--rw-r--r--   0 zu         (501) staff       (20)     7653 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/aws/resource/iam/policy.py
--rw-r--r--   0 zu         (501) staff       (20)     9828 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/aws/resource/iam/role.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.722936 phidata-2.0.0.dev4/phidata/aws/resource/rds/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/aws/resource/rds/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    36056 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/aws/resource/rds/db_cluster.py
--rw-r--r--   0 zu         (501) staff       (20)    35380 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/aws/resource/rds/db_instance.py
--rw-r--r--   0 zu         (501) staff       (20)     7990 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/aws/resource/rds/db_subnet_group.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.723177 phidata-2.0.0.dev4/phidata/aws/resource/s3/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/aws/resource/s3/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     6472 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/aws/resource/s3/bucket.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.723567 phidata-2.0.0.dev4/phidata/aws/resource/secret/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/aws/resource/secret/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    11398 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/aws/resource/secret/manager.py
--rw-r--r--   0 zu         (501) staff       (20)     1007 2023-06-20 14:11:22.000000 phidata-2.0.0.dev4/phidata/aws/resource/secret/reader.py
--rw-r--r--   0 zu         (501) staff       (20)     3604 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/aws/resource/types.py
--rw-r--r--   0 zu         (501) staff       (20)     9688 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/aws/resource/utils.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.724379 phidata-2.0.0.dev4/phidata/aws/s3/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/aws/s3/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    21797 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/aws/s3/csv_dataset.py
--rw-r--r--   0 zu         (501) staff       (20)    24100 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/aws/s3/dataset.py
--rw-r--r--   0 zu         (501) staff       (20)    14394 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/aws/s3/dataset_base.py
--rw-r--r--   0 zu         (501) staff       (20)     7409 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/aws/s3/object.py
--rw-r--r--   0 zu         (501) staff       (20)    22470 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/aws/worker.py
--rw-r--r--   0 zu         (501) staff       (20)     1305 2023-06-15 14:48:05.000000 phidata-2.0.0.dev4/phidata/base.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.724937 phidata-2.0.0.dev4/phidata/checks/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/checks/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     2790 2023-01-31 22:57:08.000000 phidata-2.0.0.dev4/phidata/checks/check.py
--rw-r--r--   0 zu         (501) staff       (20)      754 2023-02-03 21:54:28.000000 phidata-2.0.0.dev4/phidata/checks/not_empty.py
--rw-r--r--   0 zu         (501) staff       (20)     1178 2023-01-04 19:03:10.000000 phidata-2.0.0.dev4/phidata/constants.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.725634 phidata-2.0.0.dev4/phidata/decorators/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-02-28 02:08:34.000000 phidata-2.0.0.dev4/phidata/decorators/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      582 2022-02-28 02:08:34.000000 phidata-2.0.0.dev4/phidata/decorators/timer.py
--rw-r--r--   0 zu         (501) staff       (20)     1110 2023-03-13 15:21:10.000000 phidata-2.0.0.dev4/phidata/decorators/validate_env.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.727260 phidata-2.0.0.dev4/phidata/docker/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/docker/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1728 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/docker/api_client.py
--rw-r--r--   0 zu         (501) staff       (20)     1645 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/docker/args.py
--rw-r--r--   0 zu         (501) staff       (20)     4482 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/docker/config.py
--rw-r--r--   0 zu         (501) staff       (20)     1166 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/docker/enums.py
--rw-r--r--   0 zu         (501) staff       (20)      322 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/docker/exceptions.py
--rw-r--r--   0 zu         (501) staff       (20)     8899 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/docker/manager.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.728643 phidata-2.0.0.dev4/phidata/docker/resource/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/docker/resource/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     3804 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/docker/resource/base.py
--rw-r--r--   0 zu         (501) staff       (20)    16440 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/docker/resource/container.py
--rw-r--r--   0 zu         (501) staff       (20)      932 2023-06-20 14:11:22.000000 phidata-2.0.0.dev4/phidata/docker/resource/group.py
--rw-r--r--   0 zu         (501) staff       (20)    14773 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/docker/resource/image.py
--rw-r--r--   0 zu         (501) staff       (20)     5226 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/docker/resource/network.py
--rw-r--r--   0 zu         (501) staff       (20)     1165 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/docker/resource/types.py
--rw-r--r--   0 zu         (501) staff       (20)    10737 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/docker/resource/utils.py
--rw-r--r--   0 zu         (501) staff       (20)     4961 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/docker/resource/volume.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.728869 phidata-2.0.0.dev4/phidata/docker/utils/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/docker/utils/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     3584 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/docker/utils/container.py
--rw-r--r--   0 zu         (501) staff       (20)    24179 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/docker/worker.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.729844 phidata-2.0.0.dev4/phidata/exceptions/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-22 20:24:07.000000 phidata-2.0.0.dev4/phidata/exceptions/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)       47 2022-05-24 18:09:11.000000 phidata-2.0.0.dev4/phidata/exceptions/app.py
--rw-r--r--   0 zu         (501) staff       (20)       39 2022-04-22 20:24:07.000000 phidata-2.0.0.dev4/phidata/exceptions/task.py
--rw-r--r--   0 zu         (501) staff       (20)       43 2022-04-25 21:05:27.000000 phidata-2.0.0.dev4/phidata/exceptions/workflow.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.731031 phidata-2.0.0.dev4/phidata/infra/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-02-28 02:08:34.000000 phidata-2.0.0.dev4/phidata/infra/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      341 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/infra/api_client.py
--rw-r--r--   0 zu         (501) staff       (20)     2466 2023-01-25 22:40:46.000000 phidata-2.0.0.dev4/phidata/infra/args.py
--rw-r--r--   0 zu         (501) staff       (20)    15390 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/infra/config.py
--rw-r--r--   0 zu         (501) staff       (20)    12048 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/infra/resource.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.734844 phidata-2.0.0.dev4/phidata/k8s/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/k8s/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     5059 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/k8s/api_client.py
--rw-r--r--   0 zu         (501) staff       (20)     1986 2023-06-15 14:48:05.000000 phidata-2.0.0.dev4/phidata/k8s/args.py
--rw-r--r--   0 zu         (501) staff       (20)     7871 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/k8s/config.py
--rw-r--r--   0 zu         (501) staff       (20)      143 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/k8s/constants.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.735841 phidata-2.0.0.dev4/phidata/k8s/create/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/k8s/create/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.736112 phidata-2.0.0.dev4/phidata/k8s/create/apiextensions_k8s_io/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/k8s/create/apiextensions_k8s_io/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.736595 phidata-2.0.0.dev4/phidata/k8s/create/apiextensions_k8s_io/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/k8s/create/apiextensions_k8s_io/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     3418 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py
--rw-r--r--   0 zu         (501) staff       (20)     2430 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.736869 phidata-2.0.0.dev4/phidata/k8s/create/apps/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/k8s/create/apps/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.737124 phidata-2.0.0.dev4/phidata/k8s/create/apps/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/k8s/create/apps/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     5429 2023-01-24 16:40:47.000000 phidata-2.0.0.dev4/phidata/k8s/create/apps/v1/deployment.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.737685 phidata-2.0.0.dev4/phidata/k8s/create/common/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/k8s/create/common/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      357 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/k8s/create/common/labels.py
--rw-r--r--   0 zu         (501) staff       (20)     1553 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/k8s/create/common/port.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.737877 phidata-2.0.0.dev4/phidata/k8s/create/core/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/k8s/create/core/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.740130 phidata-2.0.0.dev4/phidata/k8s/create/core/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/k8s/create/core/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1395 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/k8s/create/core/v1/config_map.py
--rw-r--r--   0 zu         (501) staff       (20)     5490 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/k8s/create/core/v1/container.py
--rw-r--r--   0 zu         (501) staff       (20)     1515 2023-03-13 15:21:10.000000 phidata-2.0.0.dev4/phidata/k8s/create/core/v1/namespace.py
--rw-r--r--   0 zu         (501) staff       (20)     6695 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/k8s/create/core/v1/persistent_volume.py
--rw-r--r--   0 zu         (501) staff       (20)     2005 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/k8s/create/core/v1/persistent_volume_claim.py
--rw-r--r--   0 zu         (501) staff       (20)     1555 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/k8s/create/core/v1/secret.py
--rw-r--r--   0 zu         (501) staff       (20)     4200 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/k8s/create/core/v1/service.py
--rw-r--r--   0 zu         (501) staff       (20)     2030 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/k8s/create/core/v1/service_account.py
--rw-r--r--   0 zu         (501) staff       (20)     4516 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/k8s/create/core/v1/volume.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.740406 phidata-2.0.0.dev4/phidata/k8s/create/crb/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/k8s/create/crb/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     2115 2023-03-13 15:21:10.000000 phidata-2.0.0.dev4/phidata/k8s/create/crb/eks_admin_crb.py
--rw-r--r--   0 zu         (501) staff       (20)    19062 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/k8s/create/group.py
--rw-r--r--   0 zu         (501) staff       (20)     5795 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/k8s/create/kubeconfig.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.740623 phidata-2.0.0.dev4/phidata/k8s/create/networking_k8s_io/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-31 01:52:27.000000 phidata-2.0.0.dev4/phidata/k8s/create/networking_k8s_io/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.740828 phidata-2.0.0.dev4/phidata/k8s/create/networking_k8s_io/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-31 01:52:37.000000 phidata-2.0.0.dev4/phidata/k8s/create/networking_k8s_io/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     2069 2023-01-31 02:29:01.000000 phidata-2.0.0.dev4/phidata/k8s/create/networking_k8s_io/v1/ingress.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.741113 phidata-2.0.0.dev4/phidata/k8s/create/rbac_authorization_k8s_io/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/k8s/create/rbac_authorization_k8s_io/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.741565 phidata-2.0.0.dev4/phidata/k8s/create/rbac_authorization_k8s_io/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/k8s/create/rbac_authorization_k8s_io/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1754 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py
--rw-r--r--   0 zu         (501) staff       (20)     1503 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.741740 phidata-2.0.0.dev4/phidata/k8s/create/storage_k8s_io/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/k8s/create/storage_k8s_io/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.741953 phidata-2.0.0.dev4/phidata/k8s/create/storage_k8s_io/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/k8s/create/storage_k8s_io/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     3882 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/k8s/create/storage_k8s_io/v1/storage_class.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.744016 phidata-2.0.0.dev4/phidata/k8s/enums/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/k8s/enums/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      226 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/k8s/enums/api_group.py
--rw-r--r--   0 zu         (501) staff       (20)      542 2023-01-31 02:03:51.000000 phidata-2.0.0.dev4/phidata/k8s/enums/api_version.py
--rw-r--r--   0 zu         (501) staff       (20)      162 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/k8s/enums/image_pull_policy.py
--rw-r--r--   0 zu         (501) staff       (20)      762 2023-01-31 02:04:08.000000 phidata-2.0.0.dev4/phidata/k8s/enums/kind.py
--rw-r--r--   0 zu         (501) staff       (20)     1085 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/k8s/enums/manager_status.py
--rw-r--r--   0 zu         (501) staff       (20)      127 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/k8s/enums/protocol.py
--rw-r--r--   0 zu         (501) staff       (20)      753 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/k8s/enums/pv.py
--rw-r--r--   0 zu         (501) staff       (20)      153 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/k8s/enums/restart_policy.py
--rw-r--r--   0 zu         (501) staff       (20)      171 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/k8s/enums/service_type.py
--rw-r--r--   0 zu         (501) staff       (20)      143 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/k8s/enums/storage_class.py
--rw-r--r--   0 zu         (501) staff       (20)      377 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/k8s/enums/volume_type.py
--rw-r--r--   0 zu         (501) staff       (20)      419 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/k8s/exceptions.py
--rw-r--r--   0 zu         (501) staff       (20)     8596 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/k8s/manager.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.745071 phidata-2.0.0.dev4/phidata/k8s/resource/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/k8s/resource/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.745207 phidata-2.0.0.dev4/phidata/k8s/resource/apiextensions_k8s_io/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/k8s/resource/apiextensions_k8s_io/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.745580 phidata-2.0.0.dev4/phidata/k8s/resource/apiextensions_k8s_io/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/k8s/resource/apiextensions_k8s_io/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     8592 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py
--rw-r--r--   0 zu         (501) staff       (20)    15390 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.745831 phidata-2.0.0.dev4/phidata/k8s/resource/apps/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/k8s/resource/apps/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.746306 phidata-2.0.0.dev4/phidata/k8s/resource/apps/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/k8s/resource/apps/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    10211 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/k8s/resource/apps/v1/deployment.py
--rw-r--r--   0 zu         (501) staff       (20)     1958 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/k8s/resource/apps/v1/deployment_strategy.py
--rw-r--r--   0 zu         (501) staff       (20)     8969 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/k8s/resource/base.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.746467 phidata-2.0.0.dev4/phidata/k8s/resource/core/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/k8s/resource/core/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.750577 phidata-2.0.0.dev4/phidata/k8s/resource/core/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/k8s/resource/core/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     6602 2023-03-13 15:21:10.000000 phidata-2.0.0.dev4/phidata/k8s/resource/core/v1/config_map.py
--rw-r--r--   0 zu         (501) staff       (20)    18530 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/k8s/resource/core/v1/container.py
--rw-r--r--   0 zu         (501) staff       (20)      822 2023-03-13 15:21:10.000000 phidata-2.0.0.dev4/phidata/k8s/resource/core/v1/local_object_reference.py
--rw-r--r--   0 zu         (501) staff       (20)     6635 2023-03-13 15:21:10.000000 phidata-2.0.0.dev4/phidata/k8s/resource/core/v1/namespace.py
--rw-r--r--   0 zu         (501) staff       (20)     3863 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/k8s/resource/core/v1/node_selector.py
--rw-r--r--   0 zu         (501) staff       (20)     1614 2023-03-13 15:21:10.000000 phidata-2.0.0.dev4/phidata/k8s/resource/core/v1/object_reference.py
--rw-r--r--   0 zu         (501) staff       (20)    12419 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/k8s/resource/core/v1/persistent_volume.py
--rw-r--r--   0 zu         (501) staff       (20)     8107 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/k8s/resource/core/v1/persistent_volume_claim.py
--rw-r--r--   0 zu         (501) staff       (20)     2693 2023-03-13 15:21:10.000000 phidata-2.0.0.dev4/phidata/k8s/resource/core/v1/pod.py
--rw-r--r--   0 zu         (501) staff       (20)     7468 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/k8s/resource/core/v1/pod_spec.py
--rw-r--r--   0 zu         (501) staff       (20)      901 2023-03-13 15:21:10.000000 phidata-2.0.0.dev4/phidata/k8s/resource/core/v1/pod_template_spec.py
--rw-r--r--   0 zu         (501) staff       (20)     1244 2023-03-13 15:21:10.000000 phidata-2.0.0.dev4/phidata/k8s/resource/core/v1/resource_requirements.py
--rw-r--r--   0 zu         (501) staff       (20)     6196 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/k8s/resource/core/v1/secret.py
--rw-r--r--   0 zu         (501) staff       (20)    18982 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/k8s/resource/core/v1/service.py
--rw-r--r--   0 zu         (501) staff       (20)     8657 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/k8s/resource/core/v1/service_account.py
--rw-r--r--   0 zu         (501) staff       (20)     2313 2023-03-13 15:21:10.000000 phidata-2.0.0.dev4/phidata/k8s/resource/core/v1/toleration.py
--rw-r--r--   0 zu         (501) staff       (20)     4086 2023-03-13 15:21:10.000000 phidata-2.0.0.dev4/phidata/k8s/resource/core/v1/topology_spread_constraints.py
--rw-r--r--   0 zu         (501) staff       (20)     4788 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/k8s/resource/core/v1/volume.py
--rw-r--r--   0 zu         (501) staff       (20)      890 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/k8s/resource/core/v1/volume_node_affinity.py
--rw-r--r--   0 zu         (501) staff       (20)    13397 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/k8s/resource/core/v1/volume_source.py
--rw-r--r--   0 zu         (501) staff       (20)    12690 2023-06-20 14:11:22.000000 phidata-2.0.0.dev4/phidata/k8s/resource/group.py
--rw-r--r--   0 zu         (501) staff       (20)     4475 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/k8s/resource/kubeconfig.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.750843 phidata-2.0.0.dev4/phidata/k8s/resource/meta/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/k8s/resource/meta/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.751305 phidata-2.0.0.dev4/phidata/k8s/resource/meta/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/k8s/resource/meta/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1058 2023-04-09 17:01:38.000000 phidata-2.0.0.dev4/phidata/k8s/resource/meta/v1/label_selector.py
--rw-r--r--   0 zu         (501) staff       (20)     2739 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/k8s/resource/meta/v1/object_meta.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.751540 phidata-2.0.0.dev4/phidata/k8s/resource/networking_k8s_io/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-31 01:30:16.000000 phidata-2.0.0.dev4/phidata/k8s/resource/networking_k8s_io/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.751812 phidata-2.0.0.dev4/phidata/k8s/resource/networking_k8s_io/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-31 01:30:42.000000 phidata-2.0.0.dev4/phidata/k8s/resource/networking_k8s_io/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    10026 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/k8s/resource/networking_k8s_io/v1/ingress.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.752006 phidata-2.0.0.dev4/phidata/k8s/resource/rbac_authorization_k8s_io/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/k8s/resource/rbac_authorization_k8s_io/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.752358 phidata-2.0.0.dev4/phidata/k8s/resource/rbac_authorization_k8s_io/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/k8s/resource/rbac_authorization_k8s_io/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     8969 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py
--rw-r--r--   0 zu         (501) staff       (20)     6675 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.752506 phidata-2.0.0.dev4/phidata/k8s/resource/storage_k8s_io/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/k8s/resource/storage_k8s_io/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.752709 phidata-2.0.0.dev4/phidata/k8s/resource/storage_k8s_io/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/k8s/resource/storage_k8s_io/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     7198 2023-03-13 15:21:10.000000 phidata-2.0.0.dev4/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py
--rw-r--r--   0 zu         (501) staff       (20)     3415 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/k8s/resource/types.py
--rw-r--r--   0 zu         (501) staff       (20)    10127 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/k8s/resource/utils.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.753113 phidata-2.0.0.dev4/phidata/k8s/utils/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/k8s/utils/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1864 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/k8s/utils/pod.py
--rw-r--r--   0 zu         (501) staff       (20)    43059 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/k8s/worker.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.753264 phidata-2.0.0.dev4/phidata/llm/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-04-09 17:01:38.000000 phidata-2.0.0.dev4/phidata/llm/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.754475 phidata-2.0.0.dev4/phidata/llm/duckdb/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-04-09 17:01:38.000000 phidata-2.0.0.dev4/phidata/llm/duckdb/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     4403 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/llm/duckdb/agent.py
--rw-r--r--   0 zu         (501) staff       (20)     3896 2023-04-09 17:01:38.000000 phidata-2.0.0.dev4/phidata/llm/duckdb/chain.py
--rw-r--r--   0 zu         (501) staff       (20)      920 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/llm/duckdb/connection.py
--rw-r--r--   0 zu         (501) staff       (20)     1194 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/llm/duckdb/loader.py
--rw-r--r--   0 zu         (501) staff       (20)     2177 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/llm/duckdb/query.py
--rw-r--r--   0 zu         (501) staff       (20)     1063 2023-04-09 17:01:38.000000 phidata-2.0.0.dev4/phidata/llm/duckdb/tool.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.755202 phidata-2.0.0.dev4/phidata/product/
--rw-r--r--   0 zu         (501) staff       (20)       70 2022-03-13 21:20:10.000000 phidata-2.0.0.dev4/phidata/product/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    29505 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/product/data_product.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.755499 phidata-2.0.0.dev4/phidata/resource/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-06-15 14:48:05.000000 phidata-2.0.0.dev4/phidata/resource/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      445 2023-06-15 14:48:05.000000 phidata-2.0.0.dev4/phidata/resource/reference.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.755746 phidata-2.0.0.dev4/phidata/table/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/table/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.756454 phidata-2.0.0.dev4/phidata/table/local/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/table/local/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     4616 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/table/local/csv.py
--rw-r--r--   0 zu         (501) staff       (20)    23516 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/table/local/local_table.py
--rw-r--r--   0 zu         (501) staff       (20)     4624 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/table/local/parquet.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.757143 phidata-2.0.0.dev4/phidata/table/s3/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/table/s3/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     4673 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/table/s3/csv.py
--rw-r--r--   0 zu         (501) staff       (20)     4668 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/table/s3/parquet.py
--rw-r--r--   0 zu         (501) staff       (20)    23064 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/table/s3/s3_table.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.757742 phidata-2.0.0.dev4/phidata/table/sql/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/table/sql/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1752 2023-04-07 15:40:41.000000 phidata-2.0.0.dev4/phidata/table/sql/postgres.py
--rw-r--r--   0 zu         (501) staff       (20)    35497 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/table/sql/sql_table.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.759209 phidata-2.0.0.dev4/phidata/task/
--rw-r--r--   0 zu         (501) staff       (20)       79 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/task/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.759452 phidata-2.0.0.dev4/phidata/task/aws/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev4/phidata/task/aws/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.759870 phidata-2.0.0.dev4/phidata/task/aws/athena/
--rw-r--r--   0 zu         (501) staff       (20)       81 2022-04-18 19:05:50.000000 phidata-2.0.0.dev4/phidata/task/aws/athena/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     2210 2023-03-13 15:21:10.000000 phidata-2.0.0.dev4/phidata/task/aws/athena/run_query.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.760241 phidata-2.0.0.dev4/phidata/task/aws/emr/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev4/phidata/task/aws/emr/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1637 2023-03-13 15:21:10.000000 phidata-2.0.0.dev4/phidata/task/aws/emr/create_cluster.py
--rw-r--r--   0 zu         (501) staff       (20)     1637 2023-03-13 15:21:10.000000 phidata-2.0.0.dev4/phidata/task/aws/emr/delete_cluster.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.760643 phidata-2.0.0.dev4/phidata/task/aws/glue/
--rw-r--r--   0 zu         (501) staff       (20)      100 2022-04-18 19:05:50.000000 phidata-2.0.0.dev4/phidata/task/aws/glue/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     2038 2023-03-13 15:21:10.000000 phidata-2.0.0.dev4/phidata/task/aws/glue/start_crawler.py
--rw-r--r--   0 zu         (501) staff       (20)     1381 2022-04-18 19:05:50.000000 phidata-2.0.0.dev4/phidata/task/decorator.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.760818 phidata-2.0.0.dev4/phidata/task/dev/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev4/phidata/task/dev/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.760910 phidata-2.0.0.dev4/phidata/task/download/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev4/phidata/task/download/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.761206 phidata-2.0.0.dev4/phidata/task/download/s3/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev4/phidata/task/download/s3/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     2114 2023-03-13 15:21:10.000000 phidata-2.0.0.dev4/phidata/task/download/s3/to_file.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.762193 phidata-2.0.0.dev4/phidata/task/download/url/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev4/phidata/task/download/url/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     4775 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/task/download/url/to_file.py
--rw-r--r--   0 zu         (501) staff       (20)     3681 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/task/download/url/to_s3.py
--rw-r--r--   0 zu         (501) staff       (20)     8180 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/task/download/url/to_sql.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.762362 phidata-2.0.0.dev4/phidata/task/plot/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev4/phidata/task/plot/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.762564 phidata-2.0.0.dev4/phidata/task/plot/sql/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev4/phidata/task/plot/sql/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     2541 2023-03-13 15:21:10.000000 phidata-2.0.0.dev4/phidata/task/plot/sql/query.py
--rw-r--r--   0 zu         (501) staff       (20)    12300 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/task/python_task.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.762782 phidata-2.0.0.dev4/phidata/task/run/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev4/phidata/task/run/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.762993 phidata-2.0.0.dev4/phidata/task/run/sql/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev4/phidata/task/run/sql/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     4126 2023-04-09 17:01:38.000000 phidata-2.0.0.dev4/phidata/task/run/sql/query.py
--rw-r--r--   0 zu         (501) staff       (20)     7636 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/task/task.py
--rw-r--r--   0 zu         (501) staff       (20)     1041 2022-04-25 21:05:27.000000 phidata-2.0.0.dev4/phidata/task/task_relatives.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.763245 phidata-2.0.0.dev4/phidata/task/upload/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev4/phidata/task/upload/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.763669 phidata-2.0.0.dev4/phidata/task/upload/file/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev4/phidata/task/upload/file/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     2039 2023-03-13 15:21:10.000000 phidata-2.0.0.dev4/phidata/task/upload/file/to_s3.py
--rw-r--r--   0 zu         (501) staff       (20)     4721 2023-03-13 15:21:10.000000 phidata-2.0.0.dev4/phidata/task/upload/file/to_sql.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.764730 phidata-2.0.0.dev4/phidata/types/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-02-28 02:08:34.000000 phidata-2.0.0.dev4/phidata/types/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1023 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/types/airflow.py
--rw-r--r--   0 zu         (501) staff       (20)     2063 2023-06-15 14:48:05.000000 phidata-2.0.0.dev4/phidata/types/context.py
--rw-r--r--   0 zu         (501) staff       (20)      705 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/types/phidata_runtime.py
--rw-r--r--   0 zu         (501) staff       (20)      101 2022-04-22 20:24:07.000000 phidata-2.0.0.dev4/phidata/types/run_status.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.768113 phidata-2.0.0.dev4/phidata/utils/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-02-28 02:08:34.000000 phidata-2.0.0.dev4/phidata/utils/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     4779 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/utils/cli_console.py
--rw-r--r--   0 zu         (501) staff       (20)     2044 2023-01-31 02:10:08.000000 phidata-2.0.0.dev4/phidata/utils/common.py
--rw-r--r--   0 zu         (501) staff       (20)     1037 2022-11-28 16:47:00.000000 phidata-2.0.0.dev4/phidata/utils/compare.py
--rw-r--r--   0 zu         (501) staff       (20)     2146 2023-03-13 15:21:10.000000 phidata-2.0.0.dev4/phidata/utils/context.py
--rw-r--r--   0 zu         (501) staff       (20)     1113 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/utils/dttm.py
--rw-r--r--   0 zu         (501) staff       (20)      786 2022-06-12 23:07:23.000000 phidata-2.0.0.dev4/phidata/utils/enums.py
--rw-r--r--   0 zu         (501) staff       (20)     1595 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/utils/env_file.py
--rw-r--r--   0 zu         (501) staff       (20)     1430 2022-07-31 02:48:39.000000 phidata-2.0.0.dev4/phidata/utils/env_var.py
--rw-r--r--   0 zu         (501) staff       (20)      661 2022-02-28 02:08:34.000000 phidata-2.0.0.dev4/phidata/utils/filesystem.py
--rw-r--r--   0 zu         (501) staff       (20)      742 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/utils/get_python_objects_from_module.py
--rw-r--r--   0 zu         (501) staff       (20)      893 2023-06-15 14:48:05.000000 phidata-2.0.0.dev4/phidata/utils/json_io.py
--rw-r--r--   0 zu         (501) staff       (20)     1257 2023-06-15 14:48:05.000000 phidata-2.0.0.dev4/phidata/utils/k8s.py
--rw-r--r--   0 zu         (501) staff       (20)     1459 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/utils/log.py
--rw-r--r--   0 zu         (501) staff       (20)      707 2023-01-14 19:22:32.000000 phidata-2.0.0.dev4/phidata/utils/print_table.py
--rw-r--r--   0 zu         (501) staff       (20)      994 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/utils/workspace_path.py
--rw-r--r--   0 zu         (501) staff       (20)      833 2023-06-15 14:48:05.000000 phidata-2.0.0.dev4/phidata/utils/yaml_io.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.769189 phidata-2.0.0.dev4/phidata/workflow/
--rw-r--r--   0 zu         (501) staff       (20)      109 2022-04-15 05:02:36.000000 phidata-2.0.0.dev4/phidata/workflow/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1855 2022-04-18 19:05:50.000000 phidata-2.0.0.dev4/phidata/workflow/decorator.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.769505 phidata-2.0.0.dev4/phidata/workflow/dev/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-02-28 02:08:34.000000 phidata-2.0.0.dev4/phidata/workflow/dev/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    42342 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/workflow/workflow.py
--rw-r--r--   0 zu         (501) staff       (20)     1105 2022-04-25 21:05:27.000000 phidata-2.0.0.dev4/phidata/workflow/workflow_relatives.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.769986 phidata-2.0.0.dev4/phidata/workspace/
--rw-r--r--   0 zu         (501) staff       (20)      110 2023-06-15 14:48:05.000000 phidata-2.0.0.dev4/phidata/workspace/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    11316 2023-07-07 23:39:27.000000 phidata-2.0.0.dev4/phidata/workspace/config.py
--rw-r--r--   0 zu         (501) staff       (20)     8781 2023-07-06 09:54:23.000000 phidata-2.0.0.dev4/phidata/workspace/settings.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.683719 phidata-2.0.0.dev4/phidata.egg-info/
--rw-r--r--   0 zu         (501) staff       (20)     3126 2023-07-12 13:31:03.000000 phidata-2.0.0.dev4/phidata.egg-info/PKG-INFO
--rw-r--r--   0 zu         (501) staff       (20)    18439 2023-07-12 13:31:03.000000 phidata-2.0.0.dev4/phidata.egg-info/SOURCES.txt
--rw-r--r--   0 zu         (501) staff       (20)        1 2023-07-12 13:31:03.000000 phidata-2.0.0.dev4/phidata.egg-info/dependency_links.txt
--rw-r--r--   0 zu         (501) staff       (20)       51 2023-07-12 13:31:03.000000 phidata-2.0.0.dev4/phidata.egg-info/entry_points.txt
--rw-r--r--   0 zu         (501) staff       (20)      179 2023-07-12 13:31:03.000000 phidata-2.0.0.dev4/phidata.egg-info/requires.txt
--rw-r--r--   0 zu         (501) staff       (20)       12 2023-07-12 13:31:03.000000 phidata-2.0.0.dev4/phidata.egg-info/top_level.txt
--rw-r--r--   0 zu         (501) staff       (20)     1629 2023-07-12 13:30:05.000000 phidata-2.0.0.dev4/pyproject.toml
--rw-r--r--   0 zu         (501) staff       (20)       38 2023-07-12 13:31:03.770744 phidata-2.0.0.dev4/setup.cfg
--rw-r--r--   0 zu         (501) staff       (20)       98 2022-04-14 17:46:27.000000 phidata-2.0.0.dev4/setup.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-12 13:31:03.770244 phidata-2.0.0.dev4/tests/
--rw-r--r--   0 zu         (501) staff       (20)       40 2022-11-02 01:40:20.000000 phidata-2.0.0.dev4/tests/test_placeholder.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.911659 phidata-2.0.0.dev5/
+-rw-r--r--   0 zu         (501) staff       (20)    16759 2022-11-08 02:12:00.000000 phidata-2.0.0.dev5/LICENSE
+-rw-r--r--   0 zu         (501) staff       (20)     3126 2023-07-18 13:46:12.911483 phidata-2.0.0.dev5/PKG-INFO
+-rw-r--r--   0 zu         (501) staff       (20)     2742 2023-06-21 12:59:34.000000 phidata-2.0.0.dev5/README.md
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.825127 phidata-2.0.0.dev5/phi/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.826077 phidata-2.0.0.dev5/phi/api/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/api/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1684 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/api/client.py
+-rw-r--r--   0 zu         (501) staff       (20)      843 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/api/helpers.py
+-rw-r--r--   0 zu         (501) staff       (20)      794 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/api/routes.py
+-rw-r--r--   0 zu         (501) staff       (20)     4464 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/api/user.py
+-rw-r--r--   0 zu         (501) staff       (20)     7188 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/api/workspace.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.826288 phidata-2.0.0.dev5/phi/aws/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1310 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/api_client.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.826714 phidata-2.0.0.dev5/phi/aws/app/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/app/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    26919 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/app/base.py
+-rw-r--r--   0 zu         (501) staff       (20)      171 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/app/context.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.826951 phidata-2.0.0.dev5/phi/aws/app/fastapi/
+-rw-r--r--   0 zu         (501) staff       (20)       84 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/app/fastapi/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      766 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/app/fastapi/fastapi.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.827237 phidata-2.0.0.dev5/phi/aws/app/jupyter/
+-rw-r--r--   0 zu         (501) staff       (20)       84 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/app/jupyter/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     2862 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/app/jupyter/jupyter.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.827515 phidata-2.0.0.dev5/phi/aws/app/qdrant/
+-rw-r--r--   0 zu         (501) staff       (20)       81 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/app/qdrant/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      649 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/app/qdrant/qdrant.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.827995 phidata-2.0.0.dev5/phi/aws/app/streamlit/
+-rw-r--r--   0 zu         (501) staff       (20)       90 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/app/streamlit/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      735 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/app/streamlit/streamlit.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.828877 phidata-2.0.0.dev5/phi/aws/resource/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/resource/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.829152 phidata-2.0.0.dev5/phi/aws/resource/acm/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/resource/acm/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    10489 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/resource/acm/certificate.py
+-rw-r--r--   0 zu         (501) staff       (20)     8725 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/resource/base.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.829512 phidata-2.0.0.dev5/phi/aws/resource/cloudformation/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/resource/cloudformation/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    10247 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/resource/cloudformation/stack.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.830084 phidata-2.0.0.dev5/phi/aws/resource/ec2/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/resource/ec2/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    21177 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/resource/ec2/security_group.py
+-rw-r--r--   0 zu         (501) staff       (20)     2427 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/resource/ec2/subnet.py
+-rw-r--r--   0 zu         (501) staff       (20)    11791 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/resource/ec2/volume.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.830803 phidata-2.0.0.dev5/phi/aws/resource/ecs/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/resource/ecs/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     6316 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/resource/ecs/cluster.py
+-rw-r--r--   0 zu         (501) staff       (20)    11368 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/resource/ecs/container.py
+-rw-r--r--   0 zu         (501) staff       (20)    19592 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/resource/ecs/service.py
+-rw-r--r--   0 zu         (501) staff       (20)    21760 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/resource/ecs/task_definition.py
+-rw-r--r--   0 zu         (501) staff       (20)     3385 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/resource/ecs/volume.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.831528 phidata-2.0.0.dev5/phi/aws/resource/eks/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/resource/eks/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     7252 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/resource/eks/addon.py
+-rw-r--r--   0 zu         (501) staff       (20)    29689 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/resource/eks/cluster.py
+-rw-r--r--   0 zu         (501) staff       (20)    13244 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/resource/eks/fargate_profile.py
+-rw-r--r--   0 zu         (501) staff       (20)    24791 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/resource/eks/kubeconfig.py
+-rw-r--r--   0 zu         (501) staff       (20)    23405 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/resource/eks/node_group.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.831928 phidata-2.0.0.dev5/phi/aws/resource/elasticache/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/resource/elasticache/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    15451 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/resource/elasticache/cluster.py
+-rw-r--r--   0 zu         (501) staff       (20)     5922 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/resource/elasticache/subnet_group.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.832486 phidata-2.0.0.dev5/phi/aws/resource/elb/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/resource/elb/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    10268 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/resource/elb/listener.py
+-rw-r--r--   0 zu         (501) staff       (20)     7618 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/resource/elb/load_balancer.py
+-rw-r--r--   0 zu         (501) staff       (20)     9507 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/resource/elb/target_group.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.832755 phidata-2.0.0.dev5/phi/aws/resource/emr/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/resource/emr/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    12578 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/resource/emr/cluster.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.834247 phidata-2.0.0.dev5/phi/aws/resource/glue/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/resource/glue/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    12558 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/resource/glue/crawler.py
+-rw-r--r--   0 zu         (501) staff       (20)    23734 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/resource/group.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.834799 phidata-2.0.0.dev5/phi/aws/resource/iam/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/resource/iam/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     7481 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/resource/iam/policy.py
+-rw-r--r--   0 zu         (501) staff       (20)     9714 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/resource/iam/role.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.835579 phidata-2.0.0.dev5/phi/aws/resource/rds/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/resource/rds/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    35097 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/resource/rds/db_cluster.py
+-rw-r--r--   0 zu         (501) staff       (20)    34346 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/resource/rds/db_instance.py
+-rw-r--r--   0 zu         (501) staff       (20)     7611 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/resource/rds/db_subnet_group.py
+-rw-r--r--   0 zu         (501) staff       (20)      290 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/resource/reference.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.835803 phidata-2.0.0.dev5/phi/aws/resource/s3/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/resource/s3/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     6400 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/resource/s3/bucket.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.836129 phidata-2.0.0.dev5/phi/aws/resource/secret/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/resource/secret/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    11028 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/resource/secret/manager.py
+-rw-r--r--   0 zu         (501) staff       (20)      999 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/resource/secret/reader.py
+-rw-r--r--   0 zu         (501) staff       (20)     3475 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/aws/resource/types.py
+-rw-r--r--   0 zu         (501) staff       (20)     5037 2023-07-18 13:44:43.000000 phidata-2.0.0.dev5/phi/base.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.837058 phidata-2.0.0.dev5/phi/cli/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/cli/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     3667 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/cli/auth_server.py
+-rw-r--r--   0 zu         (501) staff       (20)    13385 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/cli/config.py
+-rw-r--r--   0 zu         (501) staff       (20)     3316 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/cli/console.py
+-rw-r--r--   0 zu         (501) staff       (20)      833 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/cli/credentials.py
+-rw-r--r--   0 zu         (501) staff       (20)    20599 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/cli/entrypoint.py
+-rw-r--r--   0 zu         (501) staff       (20)    15893 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/cli/operator.py
+-rw-r--r--   0 zu         (501) staff       (20)     2045 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/cli/settings.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.837606 phidata-2.0.0.dev5/phi/cli/ws/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/cli/ws/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    27120 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/cli/ws/ws_cli.py
+-rw-r--r--   0 zu         (501) staff       (20)      696 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/constants.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.838065 phidata-2.0.0.dev5/phi/docker/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/docker/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1150 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/docker/api_client.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.838495 phidata-2.0.0.dev5/phi/docker/app/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/docker/app/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    14659 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/docker/app/base.py
+-rw-r--r--   0 zu         (501) staff       (20)       87 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/docker/app/context.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.838785 phidata-2.0.0.dev5/phi/docker/app/django/
+-rw-r--r--   0 zu         (501) staff       (20)       84 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/docker/app/django/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      917 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/docker/app/django/django.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.839263 phidata-2.0.0.dev5/phi/docker/app/fastapi/
+-rw-r--r--   0 zu         (501) staff       (20)       87 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/docker/app/fastapi/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      932 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/docker/app/fastapi/fastapi.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.839531 phidata-2.0.0.dev5/phi/docker/app/jupyter/
+-rw-r--r--   0 zu         (501) staff       (20)       87 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/docker/app/jupyter/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     3275 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/docker/app/jupyter/jupyter.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.839913 phidata-2.0.0.dev5/phi/docker/app/postgres/
+-rw-r--r--   0 zu         (501) staff       (20)      148 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/docker/app/postgres/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      232 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/docker/app/postgres/pgvector.py
+-rw-r--r--   0 zu         (501) staff       (20)     4740 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/docker/app/postgres/postgres.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.840162 phidata-2.0.0.dev5/phi/docker/app/qdrant/
+-rw-r--r--   0 zu         (501) staff       (20)       84 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/docker/app/qdrant/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      731 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/docker/app/qdrant/qdrant.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.840406 phidata-2.0.0.dev5/phi/docker/app/streamlit/
+-rw-r--r--   0 zu         (501) staff       (20)       93 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/docker/app/streamlit/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      901 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/docker/app/streamlit/streamlit.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.841424 phidata-2.0.0.dev5/phi/docker/resource/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/docker/resource/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     4871 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/docker/resource/base.py
+-rw-r--r--   0 zu         (501) staff       (20)    15125 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/docker/resource/container.py
+-rw-r--r--   0 zu         (501) staff       (20)    21704 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/docker/resource/group.py
+-rw-r--r--   0 zu         (501) staff       (20)    14791 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/docker/resource/image.py
+-rw-r--r--   0 zu         (501) staff       (20)     5126 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/docker/resource/network.py
+-rw-r--r--   0 zu         (501) staff       (20)     1130 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/docker/resource/types.py
+-rw-r--r--   0 zu         (501) staff       (20)     4785 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/docker/resource/volume.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.841730 phidata-2.0.0.dev5/phi/document/
+-rw-r--r--   0 zu         (501) staff       (20)       39 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/document/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      809 2023-07-18 13:44:43.000000 phidata-2.0.0.dev5/phi/document/base.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.842079 phidata-2.0.0.dev5/phi/document/reader/
+-rw-r--r--   0 zu         (501) staff       (20)       44 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/document/reader/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     2149 2023-07-18 13:44:43.000000 phidata-2.0.0.dev5/phi/document/reader/base.py
+-rw-r--r--   0 zu         (501) staff       (20)     2074 2023-07-18 13:44:43.000000 phidata-2.0.0.dev5/phi/document/reader/pdf.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.842403 phidata-2.0.0.dev5/phi/embedder/
+-rw-r--r--   0 zu         (501) staff       (20)       39 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/embedder/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      466 2023-07-18 13:44:43.000000 phidata-2.0.0.dev5/phi/embedder/base.py
+-rw-r--r--   0 zu         (501) staff       (20)      976 2023-07-18 13:44:43.000000 phidata-2.0.0.dev5/phi/embedder/openai.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.842652 phidata-2.0.0.dev5/phi/infra/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/infra/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.843108 phidata-2.0.0.dev5/phi/infra/app/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/infra/app/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    13633 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/infra/app/base.py
+-rw-r--r--   0 zu         (501) staff       (20)      522 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/infra/app/context.py
+-rw-r--r--   0 zu         (501) staff       (20)     1253 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/infra/app/db_app.py
+-rw-r--r--   0 zu         (501) staff       (20)      126 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/infra/enums.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.843444 phidata-2.0.0.dev5/phi/infra/resource/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/infra/resource/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     6896 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/infra/resource/base.py
+-rw-r--r--   0 zu         (501) staff       (20)     1679 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/infra/resource/group.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.843554 phidata-2.0.0.dev5/phi/k8s/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/k8s/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.843889 phidata-2.0.0.dev5/phi/llm/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/llm/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      362 2023-07-18 13:44:43.000000 phidata-2.0.0.dev5/phi/llm/base.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.844254 phidata-2.0.0.dev5/phi/llm/conversation/
+-rw-r--r--   0 zu         (501) staff       (20)      108 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/llm/conversation/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    10111 2023-07-18 13:44:43.000000 phidata-2.0.0.dev5/phi/llm/conversation/conversation.py
+-rw-r--r--   0 zu         (501) staff       (20)      833 2023-07-18 13:44:43.000000 phidata-2.0.0.dev5/phi/llm/conversation/schemas.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.845025 phidata-2.0.0.dev5/phi/llm/conversation/storage/
+-rw-r--r--   0 zu         (501) staff       (20)       66 2023-07-16 11:59:13.000000 phidata-2.0.0.dev5/phi/llm/conversation/storage/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      899 2023-07-18 10:39:15.000000 phidata-2.0.0.dev5/phi/llm/conversation/storage/base.py
+-rw-r--r--   0 zu         (501) staff       (20)     5845 2023-07-18 12:22:33.000000 phidata-2.0.0.dev5/phi/llm/conversation/storage/postgres.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.845607 phidata-2.0.0.dev5/phi/llm/knowledge/
+-rw-r--r--   0 zu         (501) staff       (20)       49 2023-07-18 13:44:43.000000 phidata-2.0.0.dev5/phi/llm/knowledge/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      646 2023-07-18 13:44:43.000000 phidata-2.0.0.dev5/phi/llm/knowledge/base.py
+-rw-r--r--   0 zu         (501) staff       (20)     2515 2023-07-18 13:44:43.000000 phidata-2.0.0.dev5/phi/llm/knowledge/pdf.py
+-rw-r--r--   0 zu         (501) staff       (20)     1169 2023-07-18 13:44:43.000000 phidata-2.0.0.dev5/phi/llm/openai.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.846085 phidata-2.0.0.dev5/phi/schemas/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/schemas/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      208 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/schemas/response.py
+-rw-r--r--   0 zu         (501) staff       (20)     1484 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/schemas/user.py
+-rw-r--r--   0 zu         (501) staff       (20)      677 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/schemas/workspace.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.846209 phidata-2.0.0.dev5/phi/table/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/table/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.846562 phidata-2.0.0.dev5/phi/table/sql/
+-rw-r--r--   0 zu         (501) staff       (20)       41 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/table/sql/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      403 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/table/sql/base.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.848239 phidata-2.0.0.dev5/phi/utils/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/utils/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      747 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/utils/common.py
+-rw-r--r--   0 zu         (501) staff       (20)     1342 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/utils/defaults.py
+-rw-r--r--   0 zu         (501) staff       (20)      120 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/utils/dttm.py
+-rw-r--r--   0 zu         (501) staff       (20)     1020 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/utils/filesystem.py
+-rw-r--r--   0 zu         (501) staff       (20)     1640 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/utils/git.py
+-rw-r--r--   0 zu         (501) staff       (20)      889 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/utils/json_io.py
+-rw-r--r--   0 zu         (501) staff       (20)      665 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/utils/load_env.py
+-rw-r--r--   0 zu         (501) staff       (20)     1009 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/utils/log.py
+-rw-r--r--   0 zu         (501) staff       (20)     1010 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/utils/pickle.py
+-rw-r--r--   0 zu         (501) staff       (20)      724 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/utils/py_io.py
+-rw-r--r--   0 zu         (501) staff       (20)      589 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/utils/pyproject.py
+-rw-r--r--   0 zu         (501) staff       (20)      962 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/utils/resource_filter.py
+-rw-r--r--   0 zu         (501) staff       (20)      829 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/utils/yaml_io.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.848453 phidata-2.0.0.dev5/phi/vectordb/
+-rw-r--r--   0 zu         (501) staff       (20)       39 2023-07-18 13:44:43.000000 phidata-2.0.0.dev5/phi/vectordb/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      700 2023-07-18 13:44:43.000000 phidata-2.0.0.dev5/phi/vectordb/base.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.848674 phidata-2.0.0.dev5/phi/vectordb/pgvector/
+-rw-r--r--   0 zu         (501) staff       (20)       52 2023-07-18 13:44:43.000000 phidata-2.0.0.dev5/phi/vectordb/pgvector/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     5557 2023-07-18 13:44:43.000000 phidata-2.0.0.dev5/phi/vectordb/pgvector/pgvector.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.849330 phidata-2.0.0.dev5/phi/workspace/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/workspace/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     9927 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/workspace/config.py
+-rw-r--r--   0 zu         (501) staff       (20)      321 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/workspace/enums.py
+-rw-r--r--   0 zu         (501) staff       (20)     1914 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/workspace/helpers.py
+-rw-r--r--   0 zu         (501) staff       (20)    20826 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/workspace/operator.py
+-rw-r--r--   0 zu         (501) staff       (20)     9063 2023-07-18 13:43:48.000000 phidata-2.0.0.dev5/phi/workspace/settings.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.849669 phidata-2.0.0.dev5/phidata/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-02-28 02:08:34.000000 phidata-2.0.0.dev5/phidata/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.850738 phidata-2.0.0.dev5/phidata/airflow/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev5/phidata/airflow/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      140 2022-10-01 00:05:40.000000 phidata-2.0.0.dev5/phidata/airflow/airflow_installed.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.850974 phidata-2.0.0.dev5/phidata/airflow/operators/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev5/phidata/airflow/operators/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      584 2022-04-18 19:05:50.000000 phidata-2.0.0.dev5/phidata/airflow/operators/empty.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.852203 phidata-2.0.0.dev5/phidata/app/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-10-28 00:34:05.000000 phidata-2.0.0.dev5/phidata/app/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.853449 phidata-2.0.0.dev5/phidata/app/airflow/
+-rw-r--r--   0 zu         (501) staff       (20)      385 2022-11-02 02:52:41.000000 phidata-2.0.0.dev5/phidata/app/airflow/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)   100927 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/app/airflow/airflow_base.py
+-rw-r--r--   0 zu         (501) staff       (20)    30469 2023-06-15 14:48:05.000000 phidata-2.0.0.dev5/phidata/app/airflow/airflow_flower.py
+-rw-r--r--   0 zu         (501) staff       (20)    30508 2023-06-15 14:48:05.000000 phidata-2.0.0.dev5/phidata/app/airflow/airflow_manager.py
+-rw-r--r--   0 zu         (501) staff       (20)    30505 2023-06-15 14:48:05.000000 phidata-2.0.0.dev5/phidata/app/airflow/airflow_scheduler.py
+-rw-r--r--   0 zu         (501) staff       (20)    30515 2023-06-15 14:48:05.000000 phidata-2.0.0.dev5/phidata/app/airflow/airflow_webserver.py
+-rw-r--r--   0 zu         (501) staff       (20)    30710 2023-06-15 14:48:05.000000 phidata-2.0.0.dev5/phidata/app/airflow/airflow_worker.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.853791 phidata-2.0.0.dev5/phidata/app/alertmanager/
+-rw-r--r--   0 zu         (501) staff       (20)      134 2023-03-11 17:22:33.000000 phidata-2.0.0.dev5/phidata/app/alertmanager/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    47889 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/app/alertmanager/alertmanager.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.854565 phidata-2.0.0.dev5/phidata/app/amundsen/
+-rw-r--r--   0 zu         (501) staff       (20)      398 2023-03-11 17:40:59.000000 phidata-2.0.0.dev5/phidata/app/amundsen/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    48031 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/app/amundsen/frontend.py
+-rw-r--r--   0 zu         (501) staff       (20)    48032 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/app/amundsen/metadata.py
+-rw-r--r--   0 zu         (501) staff       (20)    47944 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/app/amundsen/search.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.854833 phidata-2.0.0.dev5/phidata/app/assistant/
+-rw-r--r--   0 zu         (501) staff       (20)      139 2023-01-15 00:33:10.000000 phidata-2.0.0.dev5/phidata/app/assistant/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    49912 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/app/assistant/assistant.py
+-rw-r--r--   0 zu         (501) staff       (20)    30166 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/app/aws_app.py
+-rw-r--r--   0 zu         (501) staff       (20)    17164 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/app/base_app.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.855096 phidata-2.0.0.dev5/phidata/app/cadvisor/
+-rw-r--r--   0 zu         (501) staff       (20)      118 2023-03-11 17:22:33.000000 phidata-2.0.0.dev5/phidata/app/cadvisor/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    49678 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/app/cadvisor/cadvisor.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.855353 phidata-2.0.0.dev5/phidata/app/databox/
+-rw-r--r--   0 zu         (501) staff       (20)      157 2023-01-15 00:32:07.000000 phidata-2.0.0.dev5/phidata/app/databox/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    86151 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/app/databox/databox.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.855773 phidata-2.0.0.dev5/phidata/app/db/
+-rw-r--r--   0 zu         (501) staff       (20)       52 2022-03-29 16:28:05.000000 phidata-2.0.0.dev5/phidata/app/db/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     3187 2023-01-05 15:43:33.000000 phidata-2.0.0.dev5/phidata/app/db/base_db.py
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-04 16:30:27.000000 phidata-2.0.0.dev5/phidata/app/db/db_app.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.856130 phidata-2.0.0.dev5/phidata/app/django/
+-rw-r--r--   0 zu         (501) staff       (20)      105 2023-05-18 09:49:43.000000 phidata-2.0.0.dev5/phidata/app/django/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    27483 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/app/django/django_app.py
+-rw-r--r--   0 zu         (501) staff       (20)    30070 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/app/django/django_backup.py
+-rw-r--r--   0 zu         (501) staff       (20)    17172 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/app/docker_app.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.856408 phidata-2.0.0.dev5/phidata/app/elastic/
+-rw-r--r--   0 zu         (501) staff       (20)       71 2022-02-28 02:08:34.000000 phidata-2.0.0.dev5/phidata/app/elastic/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     3723 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/app/elastic/elastic_app.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.856655 phidata-2.0.0.dev5/phidata/app/elasticsearch/
+-rw-r--r--   0 zu         (501) staff       (20)      138 2023-03-11 17:22:33.000000 phidata-2.0.0.dev5/phidata/app/elasticsearch/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    48675 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/app/elasticsearch/elasticsearch.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.856946 phidata-2.0.0.dev5/phidata/app/fastapi/
+-rw-r--r--   0 zu         (501) staff       (20)      175 2023-06-15 14:48:05.000000 phidata-2.0.0.dev5/phidata/app/fastapi/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    20266 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/app/fastapi/fastapi_server.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.857196 phidata-2.0.0.dev5/phidata/app/grafana/
+-rw-r--r--   0 zu         (501) staff       (20)      114 2023-03-11 17:22:33.000000 phidata-2.0.0.dev5/phidata/app/grafana/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    49781 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/app/grafana/grafana.py
+-rw-r--r--   0 zu         (501) staff       (20)      822 2023-06-15 14:48:05.000000 phidata-2.0.0.dev5/phidata/app/group.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.857759 phidata-2.0.0.dev5/phidata/app/jupyter/
+-rw-r--r--   0 zu         (501) staff       (20)      273 2023-06-15 14:48:05.000000 phidata-2.0.0.dev5/phidata/app/jupyter/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    27093 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/app/jupyter/jupyter.py
+-rw-r--r--   0 zu         (501) staff       (20)    46942 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/app/jupyter/jupyter_hub.py
+-rw-r--r--   0 zu         (501) staff       (20)    93432 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/app/jupyter/jupyter_lab.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.858272 phidata-2.0.0.dev5/phidata/app/k8s/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-05-24 02:25:43.000000 phidata-2.0.0.dev5/phidata/app/k8s/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     3930 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/app/k8s/app.py
+-rw-r--r--   0 zu         (501) staff       (20)     1766 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/app/k8s/dir.py
+-rw-r--r--   0 zu         (501) staff       (20)     6550 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/app/k8s/url.py
+-rw-r--r--   0 zu         (501) staff       (20)    37830 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/app/k8s_app.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.858512 phidata-2.0.0.dev5/phidata/app/mysql/
+-rw-r--r--   0 zu         (501) staff       (20)      151 2023-05-03 15:21:14.000000 phidata-2.0.0.dev5/phidata/app/mysql/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    49110 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/app/mysql/mysql_db.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.858795 phidata-2.0.0.dev5/phidata/app/neo4j/
+-rw-r--r--   0 zu         (501) staff       (20)      106 2023-03-11 17:22:33.000000 phidata-2.0.0.dev5/phidata/app/neo4j/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    47856 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/app/neo4j/neo4j.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.859043 phidata-2.0.0.dev5/phidata/app/nodeexporter/
+-rw-r--r--   0 zu         (501) staff       (20)      134 2023-03-11 17:22:33.000000 phidata-2.0.0.dev5/phidata/app/nodeexporter/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    47898 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/app/nodeexporter/nodeexporter.py
+-rw-r--r--   0 zu         (501) staff       (20)    38495 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/app/phidata_app.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.859326 phidata-2.0.0.dev5/phidata/app/postgres/
+-rw-r--r--   0 zu         (501) staff       (20)      166 2023-01-15 00:33:00.000000 phidata-2.0.0.dev5/phidata/app/postgres/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    53156 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/app/postgres/postgres_db.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.859617 phidata-2.0.0.dev5/phidata/app/prometheus/
+-rw-r--r--   0 zu         (501) staff       (20)      126 2023-03-11 17:22:33.000000 phidata-2.0.0.dev5/phidata/app/prometheus/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    49051 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/app/prometheus/prometheus.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.859953 phidata-2.0.0.dev5/phidata/app/qdrant/
+-rw-r--r--   0 zu         (501) staff       (20)      110 2023-06-15 14:48:05.000000 phidata-2.0.0.dev5/phidata/app/qdrant/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    12372 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/app/qdrant/qdrant.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.860699 phidata-2.0.0.dev5/phidata/app/redis/
+-rw-r--r--   0 zu         (501) staff       (20)      144 2023-01-15 00:32:35.000000 phidata-2.0.0.dev5/phidata/app/redis/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    49058 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/app/redis/redis.py
+-rw-r--r--   0 zu         (501) staff       (20)    53296 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/app/redis/stack.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.861216 phidata-2.0.0.dev5/phidata/app/server/
+-rw-r--r--   0 zu         (501) staff       (20)      207 2023-05-18 09:49:43.000000 phidata-2.0.0.dev5/phidata/app/server/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    18424 2023-06-15 14:48:05.000000 phidata-2.0.0.dev5/phidata/app/server/api_server.py
+-rw-r--r--   0 zu         (501) staff       (20)    58714 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/app/server/server_base.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.862108 phidata-2.0.0.dev5/phidata/app/spark/
+-rw-r--r--   0 zu         (501) staff       (20)      193 2023-02-07 16:41:27.000000 phidata-2.0.0.dev5/phidata/app/spark/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    49424 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/app/spark/spark_base.py
+-rw-r--r--   0 zu         (501) staff       (20)    17222 2023-06-15 14:48:05.000000 phidata-2.0.0.dev5/phidata/app/spark/spark_driver.py
+-rw-r--r--   0 zu         (501) staff       (20)    17332 2023-06-15 14:48:05.000000 phidata-2.0.0.dev5/phidata/app/spark/spark_worker.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.862401 phidata-2.0.0.dev5/phidata/app/streamlit/
+-rw-r--r--   0 zu         (501) staff       (20)      174 2023-06-15 14:48:05.000000 phidata-2.0.0.dev5/phidata/app/streamlit/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    20207 2023-06-20 14:11:22.000000 phidata-2.0.0.dev5/phidata/app/streamlit/streamlit_app.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.866142 phidata-2.0.0.dev5/phidata/app/superset/
+-rw-r--r--   0 zu         (501) staff       (20)      411 2022-11-02 02:52:41.000000 phidata-2.0.0.dev5/phidata/app/superset/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    71570 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/app/superset/superset_base.py
+-rw-r--r--   0 zu         (501) staff       (20)    22925 2023-06-15 14:48:05.000000 phidata-2.0.0.dev5/phidata/app/superset/superset_init.py
+-rw-r--r--   0 zu         (501) staff       (20)    22910 2023-06-15 14:48:05.000000 phidata-2.0.0.dev5/phidata/app/superset/superset_webserver.py
+-rw-r--r--   0 zu         (501) staff       (20)    22910 2023-06-15 14:48:05.000000 phidata-2.0.0.dev5/phidata/app/superset/superset_worker.py
+-rw-r--r--   0 zu         (501) staff       (20)    22917 2023-06-15 14:48:05.000000 phidata-2.0.0.dev5/phidata/app/superset/superset_worker_beat.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.866905 phidata-2.0.0.dev5/phidata/app/traefik/
+-rw-r--r--   0 zu         (501) staff       (20)      173 2023-01-15 00:32:52.000000 phidata-2.0.0.dev5/phidata/app/traefik/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)   115905 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/app/traefik/crds.py
+-rw-r--r--   0 zu         (501) staff       (20)    48190 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/app/traefik/ingress_route.py
+-rw-r--r--   0 zu         (501) staff       (20)    44972 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/app/traefik/router.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.867147 phidata-2.0.0.dev5/phidata/asset/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/asset/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.867384 phidata-2.0.0.dev5/phidata/asset/aws/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/asset/aws/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     3210 2023-06-15 14:48:05.000000 phidata-2.0.0.dev5/phidata/asset/aws/aws_asset.py
+-rw-r--r--   0 zu         (501) staff       (20)    24787 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/asset/data_asset.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.867718 phidata-2.0.0.dev5/phidata/asset/local/
+-rw-r--r--   0 zu         (501) staff       (20)       71 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/asset/local/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    14564 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/asset/local/file.py
+-rw-r--r--   0 zu         (501) staff       (20)      574 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/asset/local/local_asset.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.868739 phidata-2.0.0.dev5/phidata/aws/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/aws/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1835 2023-03-13 15:21:09.000000 phidata-2.0.0.dev5/phidata/aws/api_client.py
+-rw-r--r--   0 zu         (501) staff       (20)      487 2023-06-15 14:48:05.000000 phidata-2.0.0.dev5/phidata/aws/args.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.869030 phidata-2.0.0.dev5/phidata/aws/athena/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/aws/athena/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     8186 2023-03-13 15:21:09.000000 phidata-2.0.0.dev5/phidata/aws/athena/query.py
+-rw-r--r--   0 zu         (501) staff       (20)     3168 2023-06-15 14:48:05.000000 phidata-2.0.0.dev5/phidata/aws/config.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.869177 phidata-2.0.0.dev5/phidata/aws/create/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/aws/create/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.869551 phidata-2.0.0.dev5/phidata/aws/create/iam/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/aws/create/iam/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     3233 2023-03-13 15:21:09.000000 phidata-2.0.0.dev5/phidata/aws/create/iam/eks_admin_role.py
+-rw-r--r--   0 zu         (501) staff       (20)     2472 2023-03-13 15:21:09.000000 phidata-2.0.0.dev5/phidata/aws/create/iam/role.py
+-rw-r--r--   0 zu         (501) staff       (20)    23058 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/aws/driver.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.869831 phidata-2.0.0.dev5/phidata/aws/enums/
+-rw-r--r--   0 zu         (501) staff       (20)       62 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/aws/enums/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1083 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/aws/enums/manager_status.py
+-rw-r--r--   0 zu         (501) staff       (20)      304 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/aws/exceptions.py
+-rw-r--r--   0 zu         (501) staff       (20)     8588 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/aws/manager.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.870503 phidata-2.0.0.dev5/phidata/aws/resource/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/aws/resource/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.870731 phidata-2.0.0.dev5/phidata/aws/resource/acm/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/aws/resource/acm/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    10630 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/aws/resource/acm/certificate.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.870958 phidata-2.0.0.dev5/phidata/aws/resource/athena/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/aws/resource/athena/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     8005 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/aws/resource/athena/query.py
+-rw-r--r--   0 zu         (501) staff       (20)     9127 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/aws/resource/base.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.871175 phidata-2.0.0.dev5/phidata/aws/resource/cloudformation/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/aws/resource/cloudformation/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    10882 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/aws/resource/cloudformation/stack.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.871672 phidata-2.0.0.dev5/phidata/aws/resource/ec2/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/aws/resource/ec2/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    21341 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/aws/resource/ec2/security_group.py
+-rw-r--r--   0 zu         (501) staff       (20)     2563 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/aws/resource/ec2/subnet.py
+-rw-r--r--   0 zu         (501) staff       (20)    11801 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/aws/resource/ec2/volume.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.872354 phidata-2.0.0.dev5/phidata/aws/resource/ecs/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/aws/resource/ecs/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     6140 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/aws/resource/ecs/cluster.py
+-rw-r--r--   0 zu         (501) staff       (20)    26253 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/aws/resource/ecs/container.py
+-rw-r--r--   0 zu         (501) staff       (20)    19630 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/aws/resource/ecs/service.py
+-rw-r--r--   0 zu         (501) staff       (20)    22397 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/aws/resource/ecs/task_definition.py
+-rw-r--r--   0 zu         (501) staff       (20)     3614 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/aws/resource/ecs/volume.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.873086 phidata-2.0.0.dev5/phidata/aws/resource/eks/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/aws/resource/eks/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     7390 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/aws/resource/eks/addon.py
+-rw-r--r--   0 zu         (501) staff       (20)    30104 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/aws/resource/eks/cluster.py
+-rw-r--r--   0 zu         (501) staff       (20)    13731 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/aws/resource/eks/fargate_profile.py
+-rw-r--r--   0 zu         (501) staff       (20)    23785 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/aws/resource/eks/kubeconfig.py
+-rw-r--r--   0 zu         (501) staff       (20)    23742 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/aws/resource/eks/node_group.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.873557 phidata-2.0.0.dev5/phidata/aws/resource/elasticache/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/aws/resource/elasticache/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    15823 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/aws/resource/elasticache/cluster.py
+-rw-r--r--   0 zu         (501) staff       (20)     6305 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/aws/resource/elasticache/subnet_group.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.874170 phidata-2.0.0.dev5/phidata/aws/resource/elb/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-04-07 15:40:41.000000 phidata-2.0.0.dev5/phidata/aws/resource/elb/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    10727 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/aws/resource/elb/listener.py
+-rw-r--r--   0 zu         (501) staff       (20)     7994 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/aws/resource/elb/load_balancer.py
+-rw-r--r--   0 zu         (501) staff       (20)     9834 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/aws/resource/elb/target_group.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.874458 phidata-2.0.0.dev5/phidata/aws/resource/emr/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/aws/resource/emr/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    12806 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/aws/resource/emr/cluster.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.874730 phidata-2.0.0.dev5/phidata/aws/resource/glue/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/aws/resource/glue/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    12850 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/aws/resource/glue/crawler.py
+-rw-r--r--   0 zu         (501) staff       (20)     3418 2023-06-20 14:11:22.000000 phidata-2.0.0.dev5/phidata/aws/resource/group.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.875692 phidata-2.0.0.dev5/phidata/aws/resource/iam/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/aws/resource/iam/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     9958 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/aws/resource/iam/group.py
+-rw-r--r--   0 zu         (501) staff       (20)     7653 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/aws/resource/iam/policy.py
+-rw-r--r--   0 zu         (501) staff       (20)     9828 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/aws/resource/iam/role.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.876221 phidata-2.0.0.dev5/phidata/aws/resource/rds/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/aws/resource/rds/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    36056 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/aws/resource/rds/db_cluster.py
+-rw-r--r--   0 zu         (501) staff       (20)    35380 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/aws/resource/rds/db_instance.py
+-rw-r--r--   0 zu         (501) staff       (20)     7990 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/aws/resource/rds/db_subnet_group.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.876440 phidata-2.0.0.dev5/phidata/aws/resource/s3/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/aws/resource/s3/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     6472 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/aws/resource/s3/bucket.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.876786 phidata-2.0.0.dev5/phidata/aws/resource/secret/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/aws/resource/secret/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    11398 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/aws/resource/secret/manager.py
+-rw-r--r--   0 zu         (501) staff       (20)     1007 2023-06-20 14:11:22.000000 phidata-2.0.0.dev5/phidata/aws/resource/secret/reader.py
+-rw-r--r--   0 zu         (501) staff       (20)     3604 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/aws/resource/types.py
+-rw-r--r--   0 zu         (501) staff       (20)     9688 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/aws/resource/utils.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.877495 phidata-2.0.0.dev5/phidata/aws/s3/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/aws/s3/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    21797 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/aws/s3/csv_dataset.py
+-rw-r--r--   0 zu         (501) staff       (20)    24100 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/aws/s3/dataset.py
+-rw-r--r--   0 zu         (501) staff       (20)    14394 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/aws/s3/dataset_base.py
+-rw-r--r--   0 zu         (501) staff       (20)     7409 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/aws/s3/object.py
+-rw-r--r--   0 zu         (501) staff       (20)    22470 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/aws/worker.py
+-rw-r--r--   0 zu         (501) staff       (20)     1305 2023-06-15 14:48:05.000000 phidata-2.0.0.dev5/phidata/base.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.877857 phidata-2.0.0.dev5/phidata/checks/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/checks/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     2790 2023-01-31 22:57:08.000000 phidata-2.0.0.dev5/phidata/checks/check.py
+-rw-r--r--   0 zu         (501) staff       (20)      754 2023-02-03 21:54:28.000000 phidata-2.0.0.dev5/phidata/checks/not_empty.py
+-rw-r--r--   0 zu         (501) staff       (20)     1178 2023-01-04 19:03:10.000000 phidata-2.0.0.dev5/phidata/constants.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.878234 phidata-2.0.0.dev5/phidata/decorators/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-02-28 02:08:34.000000 phidata-2.0.0.dev5/phidata/decorators/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      582 2022-02-28 02:08:34.000000 phidata-2.0.0.dev5/phidata/decorators/timer.py
+-rw-r--r--   0 zu         (501) staff       (20)     1110 2023-03-13 15:21:10.000000 phidata-2.0.0.dev5/phidata/decorators/validate_env.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.879151 phidata-2.0.0.dev5/phidata/docker/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/docker/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1728 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/docker/api_client.py
+-rw-r--r--   0 zu         (501) staff       (20)     1645 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/docker/args.py
+-rw-r--r--   0 zu         (501) staff       (20)     4482 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/docker/config.py
+-rw-r--r--   0 zu         (501) staff       (20)     1166 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/docker/enums.py
+-rw-r--r--   0 zu         (501) staff       (20)      322 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/docker/exceptions.py
+-rw-r--r--   0 zu         (501) staff       (20)     8899 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/docker/manager.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.880803 phidata-2.0.0.dev5/phidata/docker/resource/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/docker/resource/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     3804 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/docker/resource/base.py
+-rw-r--r--   0 zu         (501) staff       (20)    16440 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/docker/resource/container.py
+-rw-r--r--   0 zu         (501) staff       (20)      932 2023-06-20 14:11:22.000000 phidata-2.0.0.dev5/phidata/docker/resource/group.py
+-rw-r--r--   0 zu         (501) staff       (20)    14773 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/docker/resource/image.py
+-rw-r--r--   0 zu         (501) staff       (20)     5226 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/docker/resource/network.py
+-rw-r--r--   0 zu         (501) staff       (20)     1165 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/docker/resource/types.py
+-rw-r--r--   0 zu         (501) staff       (20)    10737 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/docker/resource/utils.py
+-rw-r--r--   0 zu         (501) staff       (20)     4961 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/docker/resource/volume.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.881036 phidata-2.0.0.dev5/phidata/docker/utils/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/docker/utils/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     3584 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/docker/utils/container.py
+-rw-r--r--   0 zu         (501) staff       (20)    24179 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/docker/worker.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.881485 phidata-2.0.0.dev5/phidata/exceptions/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-22 20:24:07.000000 phidata-2.0.0.dev5/phidata/exceptions/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)       47 2022-05-24 18:09:11.000000 phidata-2.0.0.dev5/phidata/exceptions/app.py
+-rw-r--r--   0 zu         (501) staff       (20)       39 2022-04-22 20:24:07.000000 phidata-2.0.0.dev5/phidata/exceptions/task.py
+-rw-r--r--   0 zu         (501) staff       (20)       43 2022-04-25 21:05:27.000000 phidata-2.0.0.dev5/phidata/exceptions/workflow.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.882087 phidata-2.0.0.dev5/phidata/infra/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-02-28 02:08:34.000000 phidata-2.0.0.dev5/phidata/infra/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      341 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/infra/api_client.py
+-rw-r--r--   0 zu         (501) staff       (20)     2466 2023-01-25 22:40:46.000000 phidata-2.0.0.dev5/phidata/infra/args.py
+-rw-r--r--   0 zu         (501) staff       (20)    15390 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/infra/config.py
+-rw-r--r--   0 zu         (501) staff       (20)    12048 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/infra/resource.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.883382 phidata-2.0.0.dev5/phidata/k8s/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/k8s/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     5059 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/k8s/api_client.py
+-rw-r--r--   0 zu         (501) staff       (20)     1986 2023-06-15 14:48:05.000000 phidata-2.0.0.dev5/phidata/k8s/args.py
+-rw-r--r--   0 zu         (501) staff       (20)     7871 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/k8s/config.py
+-rw-r--r--   0 zu         (501) staff       (20)      143 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/k8s/constants.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.883853 phidata-2.0.0.dev5/phidata/k8s/create/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/k8s/create/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.883992 phidata-2.0.0.dev5/phidata/k8s/create/apiextensions_k8s_io/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/k8s/create/apiextensions_k8s_io/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.884352 phidata-2.0.0.dev5/phidata/k8s/create/apiextensions_k8s_io/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/k8s/create/apiextensions_k8s_io/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     3418 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py
+-rw-r--r--   0 zu         (501) staff       (20)     2430 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.884499 phidata-2.0.0.dev5/phidata/k8s/create/apps/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/k8s/create/apps/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.884794 phidata-2.0.0.dev5/phidata/k8s/create/apps/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/k8s/create/apps/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     5429 2023-01-24 16:40:47.000000 phidata-2.0.0.dev5/phidata/k8s/create/apps/v1/deployment.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.885152 phidata-2.0.0.dev5/phidata/k8s/create/common/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/k8s/create/common/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      357 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/k8s/create/common/labels.py
+-rw-r--r--   0 zu         (501) staff       (20)     1553 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/k8s/create/common/port.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.885365 phidata-2.0.0.dev5/phidata/k8s/create/core/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/k8s/create/core/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.886947 phidata-2.0.0.dev5/phidata/k8s/create/core/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/k8s/create/core/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1395 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/k8s/create/core/v1/config_map.py
+-rw-r--r--   0 zu         (501) staff       (20)     5490 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/k8s/create/core/v1/container.py
+-rw-r--r--   0 zu         (501) staff       (20)     1515 2023-03-13 15:21:10.000000 phidata-2.0.0.dev5/phidata/k8s/create/core/v1/namespace.py
+-rw-r--r--   0 zu         (501) staff       (20)     6695 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/k8s/create/core/v1/persistent_volume.py
+-rw-r--r--   0 zu         (501) staff       (20)     2005 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/k8s/create/core/v1/persistent_volume_claim.py
+-rw-r--r--   0 zu         (501) staff       (20)     1555 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/k8s/create/core/v1/secret.py
+-rw-r--r--   0 zu         (501) staff       (20)     4200 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/k8s/create/core/v1/service.py
+-rw-r--r--   0 zu         (501) staff       (20)     2030 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/k8s/create/core/v1/service_account.py
+-rw-r--r--   0 zu         (501) staff       (20)     4516 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/k8s/create/core/v1/volume.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.887309 phidata-2.0.0.dev5/phidata/k8s/create/crb/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/k8s/create/crb/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     2115 2023-03-13 15:21:10.000000 phidata-2.0.0.dev5/phidata/k8s/create/crb/eks_admin_crb.py
+-rw-r--r--   0 zu         (501) staff       (20)    19062 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/k8s/create/group.py
+-rw-r--r--   0 zu         (501) staff       (20)     5795 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/k8s/create/kubeconfig.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.887461 phidata-2.0.0.dev5/phidata/k8s/create/networking_k8s_io/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-31 01:52:27.000000 phidata-2.0.0.dev5/phidata/k8s/create/networking_k8s_io/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.887757 phidata-2.0.0.dev5/phidata/k8s/create/networking_k8s_io/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-31 01:52:37.000000 phidata-2.0.0.dev5/phidata/k8s/create/networking_k8s_io/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     2069 2023-01-31 02:29:01.000000 phidata-2.0.0.dev5/phidata/k8s/create/networking_k8s_io/v1/ingress.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.888269 phidata-2.0.0.dev5/phidata/k8s/create/rbac_authorization_k8s_io/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/k8s/create/rbac_authorization_k8s_io/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.888617 phidata-2.0.0.dev5/phidata/k8s/create/rbac_authorization_k8s_io/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/k8s/create/rbac_authorization_k8s_io/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1754 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py
+-rw-r--r--   0 zu         (501) staff       (20)     1503 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.888772 phidata-2.0.0.dev5/phidata/k8s/create/storage_k8s_io/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/k8s/create/storage_k8s_io/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.889052 phidata-2.0.0.dev5/phidata/k8s/create/storage_k8s_io/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/k8s/create/storage_k8s_io/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     3882 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/k8s/create/storage_k8s_io/v1/storage_class.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.890778 phidata-2.0.0.dev5/phidata/k8s/enums/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/k8s/enums/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      226 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/k8s/enums/api_group.py
+-rw-r--r--   0 zu         (501) staff       (20)      542 2023-01-31 02:03:51.000000 phidata-2.0.0.dev5/phidata/k8s/enums/api_version.py
+-rw-r--r--   0 zu         (501) staff       (20)      162 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/k8s/enums/image_pull_policy.py
+-rw-r--r--   0 zu         (501) staff       (20)      762 2023-01-31 02:04:08.000000 phidata-2.0.0.dev5/phidata/k8s/enums/kind.py
+-rw-r--r--   0 zu         (501) staff       (20)     1085 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/k8s/enums/manager_status.py
+-rw-r--r--   0 zu         (501) staff       (20)      127 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/k8s/enums/protocol.py
+-rw-r--r--   0 zu         (501) staff       (20)      753 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/k8s/enums/pv.py
+-rw-r--r--   0 zu         (501) staff       (20)      153 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/k8s/enums/restart_policy.py
+-rw-r--r--   0 zu         (501) staff       (20)      171 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/k8s/enums/service_type.py
+-rw-r--r--   0 zu         (501) staff       (20)      143 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/k8s/enums/storage_class.py
+-rw-r--r--   0 zu         (501) staff       (20)      377 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/k8s/enums/volume_type.py
+-rw-r--r--   0 zu         (501) staff       (20)      419 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/k8s/exceptions.py
+-rw-r--r--   0 zu         (501) staff       (20)     8596 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/k8s/manager.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.891528 phidata-2.0.0.dev5/phidata/k8s/resource/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/k8s/resource/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.891654 phidata-2.0.0.dev5/phidata/k8s/resource/apiextensions_k8s_io/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/k8s/resource/apiextensions_k8s_io/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.892024 phidata-2.0.0.dev5/phidata/k8s/resource/apiextensions_k8s_io/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/k8s/resource/apiextensions_k8s_io/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     8592 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py
+-rw-r--r--   0 zu         (501) staff       (20)    15390 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.892381 phidata-2.0.0.dev5/phidata/k8s/resource/apps/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/k8s/resource/apps/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.892866 phidata-2.0.0.dev5/phidata/k8s/resource/apps/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/k8s/resource/apps/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    10211 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/k8s/resource/apps/v1/deployment.py
+-rw-r--r--   0 zu         (501) staff       (20)     1958 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/k8s/resource/apps/v1/deployment_strategy.py
+-rw-r--r--   0 zu         (501) staff       (20)     8969 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/k8s/resource/base.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.893019 phidata-2.0.0.dev5/phidata/k8s/resource/core/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/k8s/resource/core/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.895818 phidata-2.0.0.dev5/phidata/k8s/resource/core/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/k8s/resource/core/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     6602 2023-03-13 15:21:10.000000 phidata-2.0.0.dev5/phidata/k8s/resource/core/v1/config_map.py
+-rw-r--r--   0 zu         (501) staff       (20)    18530 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/k8s/resource/core/v1/container.py
+-rw-r--r--   0 zu         (501) staff       (20)      822 2023-03-13 15:21:10.000000 phidata-2.0.0.dev5/phidata/k8s/resource/core/v1/local_object_reference.py
+-rw-r--r--   0 zu         (501) staff       (20)     6635 2023-03-13 15:21:10.000000 phidata-2.0.0.dev5/phidata/k8s/resource/core/v1/namespace.py
+-rw-r--r--   0 zu         (501) staff       (20)     3863 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/k8s/resource/core/v1/node_selector.py
+-rw-r--r--   0 zu         (501) staff       (20)     1614 2023-03-13 15:21:10.000000 phidata-2.0.0.dev5/phidata/k8s/resource/core/v1/object_reference.py
+-rw-r--r--   0 zu         (501) staff       (20)    12419 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/k8s/resource/core/v1/persistent_volume.py
+-rw-r--r--   0 zu         (501) staff       (20)     8107 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/k8s/resource/core/v1/persistent_volume_claim.py
+-rw-r--r--   0 zu         (501) staff       (20)     2693 2023-03-13 15:21:10.000000 phidata-2.0.0.dev5/phidata/k8s/resource/core/v1/pod.py
+-rw-r--r--   0 zu         (501) staff       (20)     7468 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/k8s/resource/core/v1/pod_spec.py
+-rw-r--r--   0 zu         (501) staff       (20)      901 2023-03-13 15:21:10.000000 phidata-2.0.0.dev5/phidata/k8s/resource/core/v1/pod_template_spec.py
+-rw-r--r--   0 zu         (501) staff       (20)     1244 2023-03-13 15:21:10.000000 phidata-2.0.0.dev5/phidata/k8s/resource/core/v1/resource_requirements.py
+-rw-r--r--   0 zu         (501) staff       (20)     6196 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/k8s/resource/core/v1/secret.py
+-rw-r--r--   0 zu         (501) staff       (20)    18982 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/k8s/resource/core/v1/service.py
+-rw-r--r--   0 zu         (501) staff       (20)     8657 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/k8s/resource/core/v1/service_account.py
+-rw-r--r--   0 zu         (501) staff       (20)     2313 2023-03-13 15:21:10.000000 phidata-2.0.0.dev5/phidata/k8s/resource/core/v1/toleration.py
+-rw-r--r--   0 zu         (501) staff       (20)     4086 2023-03-13 15:21:10.000000 phidata-2.0.0.dev5/phidata/k8s/resource/core/v1/topology_spread_constraints.py
+-rw-r--r--   0 zu         (501) staff       (20)     4788 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/k8s/resource/core/v1/volume.py
+-rw-r--r--   0 zu         (501) staff       (20)      890 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/k8s/resource/core/v1/volume_node_affinity.py
+-rw-r--r--   0 zu         (501) staff       (20)    13397 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/k8s/resource/core/v1/volume_source.py
+-rw-r--r--   0 zu         (501) staff       (20)    12690 2023-06-20 14:11:22.000000 phidata-2.0.0.dev5/phidata/k8s/resource/group.py
+-rw-r--r--   0 zu         (501) staff       (20)     4475 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/k8s/resource/kubeconfig.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.895944 phidata-2.0.0.dev5/phidata/k8s/resource/meta/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/k8s/resource/meta/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.896280 phidata-2.0.0.dev5/phidata/k8s/resource/meta/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/k8s/resource/meta/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1058 2023-04-09 17:01:38.000000 phidata-2.0.0.dev5/phidata/k8s/resource/meta/v1/label_selector.py
+-rw-r--r--   0 zu         (501) staff       (20)     2739 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/k8s/resource/meta/v1/object_meta.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.896448 phidata-2.0.0.dev5/phidata/k8s/resource/networking_k8s_io/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-31 01:30:16.000000 phidata-2.0.0.dev5/phidata/k8s/resource/networking_k8s_io/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.896679 phidata-2.0.0.dev5/phidata/k8s/resource/networking_k8s_io/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-31 01:30:42.000000 phidata-2.0.0.dev5/phidata/k8s/resource/networking_k8s_io/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    10026 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/k8s/resource/networking_k8s_io/v1/ingress.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.896821 phidata-2.0.0.dev5/phidata/k8s/resource/rbac_authorization_k8s_io/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/k8s/resource/rbac_authorization_k8s_io/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.897142 phidata-2.0.0.dev5/phidata/k8s/resource/rbac_authorization_k8s_io/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/k8s/resource/rbac_authorization_k8s_io/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     8969 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py
+-rw-r--r--   0 zu         (501) staff       (20)     6675 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.897324 phidata-2.0.0.dev5/phidata/k8s/resource/storage_k8s_io/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/k8s/resource/storage_k8s_io/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.897601 phidata-2.0.0.dev5/phidata/k8s/resource/storage_k8s_io/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/k8s/resource/storage_k8s_io/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     7198 2023-03-13 15:21:10.000000 phidata-2.0.0.dev5/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py
+-rw-r--r--   0 zu         (501) staff       (20)     3415 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/k8s/resource/types.py
+-rw-r--r--   0 zu         (501) staff       (20)    10127 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/k8s/resource/utils.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.897897 phidata-2.0.0.dev5/phidata/k8s/utils/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/k8s/utils/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1864 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/k8s/utils/pod.py
+-rw-r--r--   0 zu         (501) staff       (20)    43059 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/k8s/worker.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.898034 phidata-2.0.0.dev5/phidata/llm/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-04-09 17:01:38.000000 phidata-2.0.0.dev5/phidata/llm/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.899173 phidata-2.0.0.dev5/phidata/llm/duckdb/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-04-09 17:01:38.000000 phidata-2.0.0.dev5/phidata/llm/duckdb/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     4403 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/llm/duckdb/agent.py
+-rw-r--r--   0 zu         (501) staff       (20)     3896 2023-04-09 17:01:38.000000 phidata-2.0.0.dev5/phidata/llm/duckdb/chain.py
+-rw-r--r--   0 zu         (501) staff       (20)      920 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/llm/duckdb/connection.py
+-rw-r--r--   0 zu         (501) staff       (20)     1194 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/llm/duckdb/loader.py
+-rw-r--r--   0 zu         (501) staff       (20)     2177 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/llm/duckdb/query.py
+-rw-r--r--   0 zu         (501) staff       (20)     1063 2023-04-09 17:01:38.000000 phidata-2.0.0.dev5/phidata/llm/duckdb/tool.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.899476 phidata-2.0.0.dev5/phidata/product/
+-rw-r--r--   0 zu         (501) staff       (20)       70 2022-03-13 21:20:10.000000 phidata-2.0.0.dev5/phidata/product/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    29505 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/product/data_product.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.899805 phidata-2.0.0.dev5/phidata/resource/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-06-15 14:48:05.000000 phidata-2.0.0.dev5/phidata/resource/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      445 2023-06-15 14:48:05.000000 phidata-2.0.0.dev5/phidata/resource/reference.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.899958 phidata-2.0.0.dev5/phidata/table/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/table/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.900547 phidata-2.0.0.dev5/phidata/table/local/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/table/local/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     4616 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/table/local/csv.py
+-rw-r--r--   0 zu         (501) staff       (20)    23516 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/table/local/local_table.py
+-rw-r--r--   0 zu         (501) staff       (20)     4624 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/table/local/parquet.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.901164 phidata-2.0.0.dev5/phidata/table/s3/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/table/s3/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     4673 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/table/s3/csv.py
+-rw-r--r--   0 zu         (501) staff       (20)     4668 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/table/s3/parquet.py
+-rw-r--r--   0 zu         (501) staff       (20)    23064 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/table/s3/s3_table.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.901589 phidata-2.0.0.dev5/phidata/table/sql/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/table/sql/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1752 2023-04-07 15:40:41.000000 phidata-2.0.0.dev5/phidata/table/sql/postgres.py
+-rw-r--r--   0 zu         (501) staff       (20)    35497 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/table/sql/sql_table.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.902400 phidata-2.0.0.dev5/phidata/task/
+-rw-r--r--   0 zu         (501) staff       (20)       79 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/task/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.902802 phidata-2.0.0.dev5/phidata/task/aws/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev5/phidata/task/aws/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.903321 phidata-2.0.0.dev5/phidata/task/aws/athena/
+-rw-r--r--   0 zu         (501) staff       (20)       81 2022-04-18 19:05:50.000000 phidata-2.0.0.dev5/phidata/task/aws/athena/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     2210 2023-03-13 15:21:10.000000 phidata-2.0.0.dev5/phidata/task/aws/athena/run_query.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.903808 phidata-2.0.0.dev5/phidata/task/aws/emr/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev5/phidata/task/aws/emr/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1637 2023-03-13 15:21:10.000000 phidata-2.0.0.dev5/phidata/task/aws/emr/create_cluster.py
+-rw-r--r--   0 zu         (501) staff       (20)     1637 2023-03-13 15:21:10.000000 phidata-2.0.0.dev5/phidata/task/aws/emr/delete_cluster.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.904212 phidata-2.0.0.dev5/phidata/task/aws/glue/
+-rw-r--r--   0 zu         (501) staff       (20)      100 2022-04-18 19:05:50.000000 phidata-2.0.0.dev5/phidata/task/aws/glue/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     2038 2023-03-13 15:21:10.000000 phidata-2.0.0.dev5/phidata/task/aws/glue/start_crawler.py
+-rw-r--r--   0 zu         (501) staff       (20)     1381 2022-04-18 19:05:50.000000 phidata-2.0.0.dev5/phidata/task/decorator.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.904480 phidata-2.0.0.dev5/phidata/task/dev/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev5/phidata/task/dev/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.904838 phidata-2.0.0.dev5/phidata/task/download/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev5/phidata/task/download/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.905048 phidata-2.0.0.dev5/phidata/task/download/s3/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev5/phidata/task/download/s3/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     2114 2023-03-13 15:21:10.000000 phidata-2.0.0.dev5/phidata/task/download/s3/to_file.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.905532 phidata-2.0.0.dev5/phidata/task/download/url/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev5/phidata/task/download/url/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     4775 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/task/download/url/to_file.py
+-rw-r--r--   0 zu         (501) staff       (20)     3681 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/task/download/url/to_s3.py
+-rw-r--r--   0 zu         (501) staff       (20)     8180 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/task/download/url/to_sql.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.905691 phidata-2.0.0.dev5/phidata/task/plot/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev5/phidata/task/plot/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.905934 phidata-2.0.0.dev5/phidata/task/plot/sql/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev5/phidata/task/plot/sql/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     2541 2023-03-13 15:21:10.000000 phidata-2.0.0.dev5/phidata/task/plot/sql/query.py
+-rw-r--r--   0 zu         (501) staff       (20)    12300 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/task/python_task.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.906063 phidata-2.0.0.dev5/phidata/task/run/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev5/phidata/task/run/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.906235 phidata-2.0.0.dev5/phidata/task/run/sql/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev5/phidata/task/run/sql/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     4126 2023-04-09 17:01:38.000000 phidata-2.0.0.dev5/phidata/task/run/sql/query.py
+-rw-r--r--   0 zu         (501) staff       (20)     7636 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/task/task.py
+-rw-r--r--   0 zu         (501) staff       (20)     1041 2022-04-25 21:05:27.000000 phidata-2.0.0.dev5/phidata/task/task_relatives.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.906350 phidata-2.0.0.dev5/phidata/task/upload/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev5/phidata/task/upload/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.906666 phidata-2.0.0.dev5/phidata/task/upload/file/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev5/phidata/task/upload/file/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     2039 2023-03-13 15:21:10.000000 phidata-2.0.0.dev5/phidata/task/upload/file/to_s3.py
+-rw-r--r--   0 zu         (501) staff       (20)     4721 2023-03-13 15:21:10.000000 phidata-2.0.0.dev5/phidata/task/upload/file/to_sql.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.907331 phidata-2.0.0.dev5/phidata/types/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-02-28 02:08:34.000000 phidata-2.0.0.dev5/phidata/types/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1023 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/types/airflow.py
+-rw-r--r--   0 zu         (501) staff       (20)     2063 2023-06-15 14:48:05.000000 phidata-2.0.0.dev5/phidata/types/context.py
+-rw-r--r--   0 zu         (501) staff       (20)      705 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/types/phidata_runtime.py
+-rw-r--r--   0 zu         (501) staff       (20)      101 2022-04-22 20:24:07.000000 phidata-2.0.0.dev5/phidata/types/run_status.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.910025 phidata-2.0.0.dev5/phidata/utils/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-02-28 02:08:34.000000 phidata-2.0.0.dev5/phidata/utils/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     4779 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/utils/cli_console.py
+-rw-r--r--   0 zu         (501) staff       (20)     2044 2023-01-31 02:10:08.000000 phidata-2.0.0.dev5/phidata/utils/common.py
+-rw-r--r--   0 zu         (501) staff       (20)     1037 2022-11-28 16:47:00.000000 phidata-2.0.0.dev5/phidata/utils/compare.py
+-rw-r--r--   0 zu         (501) staff       (20)     2146 2023-03-13 15:21:10.000000 phidata-2.0.0.dev5/phidata/utils/context.py
+-rw-r--r--   0 zu         (501) staff       (20)     1113 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/utils/dttm.py
+-rw-r--r--   0 zu         (501) staff       (20)      786 2022-06-12 23:07:23.000000 phidata-2.0.0.dev5/phidata/utils/enums.py
+-rw-r--r--   0 zu         (501) staff       (20)     1595 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/utils/env_file.py
+-rw-r--r--   0 zu         (501) staff       (20)     1430 2022-07-31 02:48:39.000000 phidata-2.0.0.dev5/phidata/utils/env_var.py
+-rw-r--r--   0 zu         (501) staff       (20)      661 2022-02-28 02:08:34.000000 phidata-2.0.0.dev5/phidata/utils/filesystem.py
+-rw-r--r--   0 zu         (501) staff       (20)      742 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/utils/get_python_objects_from_module.py
+-rw-r--r--   0 zu         (501) staff       (20)      893 2023-06-15 14:48:05.000000 phidata-2.0.0.dev5/phidata/utils/json_io.py
+-rw-r--r--   0 zu         (501) staff       (20)     1257 2023-06-15 14:48:05.000000 phidata-2.0.0.dev5/phidata/utils/k8s.py
+-rw-r--r--   0 zu         (501) staff       (20)     1459 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/utils/log.py
+-rw-r--r--   0 zu         (501) staff       (20)      707 2023-01-14 19:22:32.000000 phidata-2.0.0.dev5/phidata/utils/print_table.py
+-rw-r--r--   0 zu         (501) staff       (20)      994 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/utils/workspace_path.py
+-rw-r--r--   0 zu         (501) staff       (20)      833 2023-06-15 14:48:05.000000 phidata-2.0.0.dev5/phidata/utils/yaml_io.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.910653 phidata-2.0.0.dev5/phidata/workflow/
+-rw-r--r--   0 zu         (501) staff       (20)      109 2022-04-15 05:02:36.000000 phidata-2.0.0.dev5/phidata/workflow/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1855 2022-04-18 19:05:50.000000 phidata-2.0.0.dev5/phidata/workflow/decorator.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.910783 phidata-2.0.0.dev5/phidata/workflow/dev/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-02-28 02:08:34.000000 phidata-2.0.0.dev5/phidata/workflow/dev/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    42342 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/workflow/workflow.py
+-rw-r--r--   0 zu         (501) staff       (20)     1105 2022-04-25 21:05:27.000000 phidata-2.0.0.dev5/phidata/workflow/workflow_relatives.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.911134 phidata-2.0.0.dev5/phidata/workspace/
+-rw-r--r--   0 zu         (501) staff       (20)      110 2023-06-15 14:48:05.000000 phidata-2.0.0.dev5/phidata/workspace/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    11316 2023-07-07 23:39:27.000000 phidata-2.0.0.dev5/phidata/workspace/config.py
+-rw-r--r--   0 zu         (501) staff       (20)     8781 2023-07-06 09:54:23.000000 phidata-2.0.0.dev5/phidata/workspace/settings.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.850489 phidata-2.0.0.dev5/phidata.egg-info/
+-rw-r--r--   0 zu         (501) staff       (20)     3126 2023-07-18 13:46:12.000000 phidata-2.0.0.dev5/phidata.egg-info/PKG-INFO
+-rw-r--r--   0 zu         (501) staff       (20)    18749 2023-07-18 13:46:12.000000 phidata-2.0.0.dev5/phidata.egg-info/SOURCES.txt
+-rw-r--r--   0 zu         (501) staff       (20)        1 2023-07-18 13:46:12.000000 phidata-2.0.0.dev5/phidata.egg-info/dependency_links.txt
+-rw-r--r--   0 zu         (501) staff       (20)       51 2023-07-18 13:46:12.000000 phidata-2.0.0.dev5/phidata.egg-info/entry_points.txt
+-rw-r--r--   0 zu         (501) staff       (20)      179 2023-07-18 13:46:12.000000 phidata-2.0.0.dev5/phidata.egg-info/requires.txt
+-rw-r--r--   0 zu         (501) staff       (20)       12 2023-07-18 13:46:12.000000 phidata-2.0.0.dev5/phidata.egg-info/top_level.txt
+-rw-r--r--   0 zu         (501) staff       (20)     1629 2023-07-18 13:44:43.000000 phidata-2.0.0.dev5/pyproject.toml
+-rw-r--r--   0 zu         (501) staff       (20)       38 2023-07-18 13:46:12.911705 phidata-2.0.0.dev5/setup.cfg
+-rw-r--r--   0 zu         (501) staff       (20)       98 2022-04-14 17:46:27.000000 phidata-2.0.0.dev5/setup.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 13:46:12.911265 phidata-2.0.0.dev5/tests/
+-rw-r--r--   0 zu         (501) staff       (20)       40 2022-11-02 01:40:20.000000 phidata-2.0.0.dev5/tests/test_placeholder.py
```

### Comparing `phidata-2.0.0.dev4/LICENSE` & `phidata-2.0.0.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/PKG-INFO` & `phidata-2.0.0.dev5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phidata
-Version: 2.0.0.dev4
+Version: 2.0.0.dev5
 Summary: A toolkit for building applications using OSS
 Author-email: Ashpreet Bedi <ashpreet@phidata.com>
 Project-URL: homepage, https://phidata.com
 Project-URL: documentation, https://docs.phidata.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: phidata Version: 2.0.0.dev4 Summary: A toolkit for
+Metadata-Version: 2.1 Name: phidata Version: 2.0.0.dev5 Summary: A toolkit for
 building applications using OSS Author-email: Ashpreet Bedi
 phidata.com> Project-URL: homepage, https://phidata.com Project-URL:
 documentation, https://docs.phidata.com Requires-Python: >=3.7 Description-
 Content-Type: text/markdown Provides-Extra: dev Provides-Extra: aws License-
 File: LICENSE
                              ****** phidata ******
                       Run open source tools using python
```

### Comparing `phidata-2.0.0.dev4/README.md` & `phidata-2.0.0.dev5/README.md`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/api/client.py` & `phidata-2.0.0.dev5/phi/api/client.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/api/helpers.py` & `phidata-2.0.0.dev5/phi/api/helpers.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/api/routes.py` & `phidata-2.0.0.dev5/phi/api/routes.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/api/user.py` & `phidata-2.0.0.dev5/phi/api/user.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/api/workspace.py` & `phidata-2.0.0.dev5/phi/api/workspace.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/aws/api_client.py` & `phidata-2.0.0.dev5/phi/aws/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/aws/app/base.py` & `phidata-2.0.0.dev5/phi/aws/app/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/aws/app/fastapi/fastapi.py` & `phidata-2.0.0.dev5/phi/aws/app/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/aws/app/jupyter/jupyter.py` & `phidata-2.0.0.dev5/phi/aws/app/jupyter/jupyter.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/aws/app/qdrant/qdrant.py` & `phidata-2.0.0.dev5/phi/aws/app/qdrant/qdrant.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/aws/app/streamlit/streamlit.py` & `phidata-2.0.0.dev5/phi/aws/app/streamlit/streamlit.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/aws/resource/acm/certificate.py` & `phidata-2.0.0.dev5/phi/aws/resource/acm/certificate.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/aws/resource/base.py` & `phidata-2.0.0.dev5/phi/aws/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/aws/resource/cloudformation/stack.py` & `phidata-2.0.0.dev5/phi/aws/resource/cloudformation/stack.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/aws/resource/ec2/security_group.py` & `phidata-2.0.0.dev5/phi/aws/resource/ec2/security_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/aws/resource/ec2/subnet.py` & `phidata-2.0.0.dev5/phi/aws/resource/ec2/subnet.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/aws/resource/ec2/volume.py` & `phidata-2.0.0.dev5/phi/aws/resource/ec2/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/aws/resource/ecs/cluster.py` & `phidata-2.0.0.dev5/phi/aws/resource/ecs/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/aws/resource/ecs/container.py` & `phidata-2.0.0.dev5/phi/aws/resource/ecs/container.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/aws/resource/ecs/service.py` & `phidata-2.0.0.dev5/phi/aws/resource/ecs/service.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/aws/resource/ecs/task_definition.py` & `phidata-2.0.0.dev5/phi/aws/resource/ecs/task_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/aws/resource/ecs/volume.py` & `phidata-2.0.0.dev5/phi/aws/resource/ecs/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/aws/resource/eks/addon.py` & `phidata-2.0.0.dev5/phi/aws/resource/eks/addon.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/aws/resource/eks/cluster.py` & `phidata-2.0.0.dev5/phi/aws/resource/eks/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/aws/resource/eks/fargate_profile.py` & `phidata-2.0.0.dev5/phi/aws/resource/eks/fargate_profile.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/aws/resource/eks/kubeconfig.py` & `phidata-2.0.0.dev5/phi/aws/resource/eks/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/aws/resource/eks/node_group.py` & `phidata-2.0.0.dev5/phi/aws/resource/eks/node_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/aws/resource/elasticache/cluster.py` & `phidata-2.0.0.dev5/phi/aws/resource/elasticache/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/aws/resource/elasticache/subnet_group.py` & `phidata-2.0.0.dev5/phi/aws/resource/elasticache/subnet_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/aws/resource/elb/listener.py` & `phidata-2.0.0.dev5/phi/aws/resource/elb/listener.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/aws/resource/elb/load_balancer.py` & `phidata-2.0.0.dev5/phi/aws/resource/elb/load_balancer.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/aws/resource/elb/target_group.py` & `phidata-2.0.0.dev5/phi/aws/resource/elb/target_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/aws/resource/emr/cluster.py` & `phidata-2.0.0.dev5/phi/aws/resource/emr/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/aws/resource/glue/crawler.py` & `phidata-2.0.0.dev5/phi/aws/resource/glue/crawler.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/aws/resource/group.py` & `phidata-2.0.0.dev5/phi/aws/resource/group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/aws/resource/iam/policy.py` & `phidata-2.0.0.dev5/phi/aws/resource/iam/policy.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/aws/resource/iam/role.py` & `phidata-2.0.0.dev5/phi/aws/resource/iam/role.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/aws/resource/rds/db_cluster.py` & `phidata-2.0.0.dev5/phi/aws/resource/rds/db_cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/aws/resource/rds/db_instance.py` & `phidata-2.0.0.dev5/phi/aws/resource/rds/db_instance.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/aws/resource/rds/db_subnet_group.py` & `phidata-2.0.0.dev5/phi/aws/resource/rds/db_subnet_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/aws/resource/s3/bucket.py` & `phidata-2.0.0.dev5/phi/aws/resource/s3/bucket.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/aws/resource/secret/manager.py` & `phidata-2.0.0.dev5/phi/aws/resource/secret/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/aws/resource/secret/reader.py` & `phidata-2.0.0.dev5/phi/aws/resource/secret/reader.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/aws/resource/types.py` & `phidata-2.0.0.dev5/phi/aws/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/base.py` & `phidata-2.0.0.dev5/phi/base.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pathlib import Path
 from typing import Optional, List, Any, Dict
 
-from pydantic import BaseModel, ConfigDict, Field, field_validator
+from pydantic import BaseModel, ConfigDict
 
 from phi.workspace.settings import WorkspaceSettings
 
 
 class PhiBase(BaseModel):
     name: Optional[str] = None
     group: Optional[str] = None
@@ -17,15 +17,15 @@
     skip_read: bool = False
     skip_update: bool = False
     skip_delete: bool = False
     recreate_on_update: bool = False
     # Skip create if resource with the same name is active
     use_cache: bool = True
     # Force create/update/delete implementation
-    force: Optional[bool] = Field(None, validate_default=True)
+    force: Optional[bool] = None
 
     # -*- Debug Mode
     debug_mode: bool = False
 
     # -*- Resource Environment
     # Add env variables to resource where applicable
     env_vars: Optional[Dict[str, Any]] = None
@@ -62,36 +62,14 @@
     cached_secret_file_data: Optional[Dict[str, Any]] = None
 
     model_config = ConfigDict(arbitrary_types_allowed=True)
 
     def get_group_name(self) -> Optional[str]:
         return self.group or self.name
 
-    @field_validator("force", mode="before")
-    def update_force(cls, force):
-        if force:
-            return True
-
-        from os import getenv
-
-        phi_cli_force = getenv("PHI_CLI_FORCE", False)
-        if phi_cli_force:
-            return True
-        return False
-
-    # @model_validator(mode="before")
-    # def update_force(cls, data):
-    #     from os import getenv
-    #
-    #     phi_cli_force = getenv("PHI_CLI_FORCE", False)
-    #     if phi_cli_force:
-    #         data["force"] = True
-    #         logger.info("Setting force to True using PHI_CLI_FORCE")
-    #     return data
-
     @property
     def workspace_root(self) -> Optional[Path]:
         return self.workspace_settings.ws_root if self.workspace_settings is not None else None
 
     @property
     def workspace_name(self) -> Optional[str]:
         return self.workspace_settings.ws_name if self.workspace_settings is not None else None
```

### Comparing `phidata-2.0.0.dev4/phi/cli/auth_server.py` & `phidata-2.0.0.dev5/phi/cli/auth_server.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/cli/config.py` & `phidata-2.0.0.dev5/phi/cli/config.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/cli/console.py` & `phidata-2.0.0.dev5/phi/cli/console.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/cli/credentials.py` & `phidata-2.0.0.dev5/phi/cli/credentials.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/cli/entrypoint.py` & `phidata-2.0.0.dev5/phi/cli/entrypoint.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/cli/operator.py` & `phidata-2.0.0.dev5/phi/cli/operator.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/cli/settings.py` & `phidata-2.0.0.dev5/phi/cli/settings.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/cli/ws/ws_cli.py` & `phidata-2.0.0.dev5/phi/cli/ws/ws_cli.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/constants.py` & `phidata-2.0.0.dev5/phi/constants.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/docker/api_client.py` & `phidata-2.0.0.dev5/phi/docker/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/docker/app/base.py` & `phidata-2.0.0.dev5/phi/docker/app/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/docker/app/django/django.py` & `phidata-2.0.0.dev5/phi/docker/app/django/django.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/docker/app/fastapi/fastapi.py` & `phidata-2.0.0.dev5/phi/docker/app/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/docker/app/jupyter/jupyter.py` & `phidata-2.0.0.dev5/phi/docker/app/jupyter/jupyter.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/docker/app/postgres/postgres.py` & `phidata-2.0.0.dev5/phi/docker/app/postgres/postgres.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/docker/app/qdrant/qdrant.py` & `phidata-2.0.0.dev5/phi/docker/app/qdrant/qdrant.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/docker/app/streamlit/streamlit.py` & `phidata-2.0.0.dev5/phi/docker/app/streamlit/streamlit.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/docker/resource/base.py` & `phidata-2.0.0.dev5/phi/docker/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/docker/resource/container.py` & `phidata-2.0.0.dev5/phi/docker/resource/container.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/docker/resource/group.py` & `phidata-2.0.0.dev5/phi/docker/resource/group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/docker/resource/image.py` & `phidata-2.0.0.dev5/phi/docker/resource/image.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/docker/resource/network.py` & `phidata-2.0.0.dev5/phi/docker/resource/network.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/docker/resource/types.py` & `phidata-2.0.0.dev5/phi/docker/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/docker/resource/volume.py` & `phidata-2.0.0.dev5/phi/docker/resource/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/document/reader/pdf.py` & `phidata-2.0.0.dev5/phi/document/reader/pdf.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,54 +1,65 @@
 from pathlib import Path
 from typing import List, Optional
 
 from phi.document.base import Document
-from phi.document.reader.base import ReaderBase
+from phi.document.reader.base import Reader
 from phi.utils.log import logger
 
 
-class PdfReader(ReaderBase):
+class PDFReader(Reader):
     """Reader for PDF files"""
 
-    path: Path
+    def read(self, path: Path) -> List[Document]:
+        if not path:
+            raise ValueError("No path provided")
+
+        if not path.exists():
+            raise FileNotFoundError(f"Could not find PDF: {path}")
 
-    def _read(self) -> Optional[List[Document]]:
         try:
-            from pypdf import PdfReader  # noqa: F401
+            from pypdf import PdfReader as DocumentReader  # noqa: F401
         except ImportError:
-            raise ImportError("Please install pypdf to load PDF files")
+            raise ImportError("`pypdf` not installed")
 
         try:
-            self.reader = PdfReader(self.path)
-            return [
+            logger.info(f"Reading: {path}")
+            doc_reader = DocumentReader(path)
+            doc_name = path.name.split(".")[0]
+            documents = [
                 Document(
-                    content=page.extract_text(),
-                    source=str(self.path),
+                    name=doc_name,
                     meta_data={"page": page_number + 1},
+                    content=page.extract_text(),
                 )
-                for page_number, page in enumerate(self.reader.pages)
+                for page_number, page in enumerate(doc_reader.pages)
             ]
-        except Exception as e:
-            logger.warning(f"Could not read {self.path}: {e}")
-            return None
+            if self.chunk:
+                chunked_documents = []
+                for document in documents:
+                    chunked_documents.extend(self.chunk_document(document))
+                return chunked_documents
+            return documents
+        except Exception:
+            raise
 
 
 def read_pdfs_from_dir(dir: Path) -> List[Document]:
     """Read data from a PDF and return a list of Documents"""
 
     logger.info(f"Reading PDFs in: {dir}")
     pdfs_to_read: List[Path] = []
     for pdf in dir.glob("*.pdf"):
         pdfs_to_read.append(pdf)
     logger.info(f"Found {len(pdfs_to_read)} PDFs to read")
 
+    reader = PDFReader()
     parsed_pdfs: List[Document] = []
     for pdf in pdfs_to_read:
-        reader = PdfReader(path=pdf)
         # Parse the PDF document
-        documents: Optional[List[Document]] = reader.read()
+        documents: Optional[List[Document]] = reader.read(path=pdf)
         if documents is not None:
             # Add the parsed documents to the list
             parsed_pdfs.extend(documents)
         logger.info(f"Parsed: {str(pdf)}")
 
     return parsed_pdfs
```

### Comparing `phidata-2.0.0.dev4/phi/infra/app/base.py` & `phidata-2.0.0.dev5/phi/infra/app/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/infra/app/context.py` & `phidata-2.0.0.dev5/phi/infra/app/context.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/infra/app/db_app.py` & `phidata-2.0.0.dev5/phi/infra/app/db_app.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/infra/resource/base.py` & `phidata-2.0.0.dev5/phi/infra/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/infra/resource/group.py` & `phidata-2.0.0.dev5/phi/infra/resource/group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/schemas/user.py` & `phidata-2.0.0.dev5/phi/schemas/user.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/schemas/workspace.py` & `phidata-2.0.0.dev5/phi/schemas/workspace.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/utils/common.py` & `phidata-2.0.0.dev5/phi/utils/common.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/utils/defaults.py` & `phidata-2.0.0.dev5/phi/utils/defaults.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/utils/filesystem.py` & `phidata-2.0.0.dev5/phi/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/utils/git.py` & `phidata-2.0.0.dev5/phi/utils/git.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/utils/json_io.py` & `phidata-2.0.0.dev5/phi/utils/json_io.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/utils/load_env.py` & `phidata-2.0.0.dev5/phi/utils/load_env.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/utils/log.py` & `phidata-2.0.0.dev5/phi/utils/log.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/utils/pickle.py` & `phidata-2.0.0.dev5/phi/utils/pickle.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/utils/py_io.py` & `phidata-2.0.0.dev5/phi/utils/py_io.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/utils/pyproject.py` & `phidata-2.0.0.dev5/phi/utils/pyproject.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/utils/resource_filter.py` & `phidata-2.0.0.dev5/phi/utils/resource_filter.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/utils/yaml_io.py` & `phidata-2.0.0.dev5/phi/utils/yaml_io.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/workspace/config.py` & `phidata-2.0.0.dev5/phi/workspace/config.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/workspace/helpers.py` & `phidata-2.0.0.dev5/phi/workspace/helpers.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/workspace/operator.py` & `phidata-2.0.0.dev5/phi/workspace/operator.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phi/workspace/settings.py` & `phidata-2.0.0.dev5/phi/workspace/settings.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/airflow/operators/empty.py` & `phidata-2.0.0.dev5/phidata/airflow/operators/empty.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/airflow/airflow_base.py` & `phidata-2.0.0.dev5/phidata/app/airflow/airflow_base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/airflow/airflow_flower.py` & `phidata-2.0.0.dev5/phidata/app/airflow/airflow_flower.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/airflow/airflow_manager.py` & `phidata-2.0.0.dev5/phidata/app/airflow/airflow_manager.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/airflow/airflow_scheduler.py` & `phidata-2.0.0.dev5/phidata/app/airflow/airflow_scheduler.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/airflow/airflow_webserver.py` & `phidata-2.0.0.dev5/phidata/app/airflow/airflow_webserver.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/airflow/airflow_worker.py` & `phidata-2.0.0.dev5/phidata/app/airflow/airflow_worker.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/alertmanager/alertmanager.py` & `phidata-2.0.0.dev5/phidata/app/alertmanager/alertmanager.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/amundsen/frontend.py` & `phidata-2.0.0.dev5/phidata/app/amundsen/frontend.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/amundsen/metadata.py` & `phidata-2.0.0.dev5/phidata/app/amundsen/metadata.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/amundsen/search.py` & `phidata-2.0.0.dev5/phidata/app/amundsen/search.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/assistant/assistant.py` & `phidata-2.0.0.dev5/phidata/app/assistant/assistant.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/aws_app.py` & `phidata-2.0.0.dev5/phidata/app/aws_app.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/base_app.py` & `phidata-2.0.0.dev5/phidata/app/base_app.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/cadvisor/cadvisor.py` & `phidata-2.0.0.dev5/phidata/app/cadvisor/cadvisor.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/databox/databox.py` & `phidata-2.0.0.dev5/phidata/app/databox/databox.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/db/base_db.py` & `phidata-2.0.0.dev5/phidata/app/db/base_db.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/django/django_app.py` & `phidata-2.0.0.dev5/phidata/app/django/django_app.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/django/django_backup.py` & `phidata-2.0.0.dev5/phidata/app/django/django_backup.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/docker_app.py` & `phidata-2.0.0.dev5/phidata/app/docker_app.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/elastic/elastic_app.py` & `phidata-2.0.0.dev5/phidata/app/elastic/elastic_app.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/elasticsearch/elasticsearch.py` & `phidata-2.0.0.dev5/phidata/app/elasticsearch/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/fastapi/fastapi_server.py` & `phidata-2.0.0.dev5/phidata/app/fastapi/fastapi_server.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/grafana/grafana.py` & `phidata-2.0.0.dev5/phidata/app/grafana/grafana.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/group.py` & `phidata-2.0.0.dev5/phidata/app/group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/jupyter/jupyter.py` & `phidata-2.0.0.dev5/phidata/app/jupyter/jupyter.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/jupyter/jupyter_hub.py` & `phidata-2.0.0.dev5/phidata/app/jupyter/jupyter_hub.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/jupyter/jupyter_lab.py` & `phidata-2.0.0.dev5/phidata/app/jupyter/jupyter_lab.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/k8s/app.py` & `phidata-2.0.0.dev5/phidata/app/k8s/app.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/k8s/dir.py` & `phidata-2.0.0.dev5/phidata/app/k8s/dir.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/k8s/url.py` & `phidata-2.0.0.dev5/phidata/app/k8s/url.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/k8s_app.py` & `phidata-2.0.0.dev5/phidata/app/k8s_app.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/mysql/mysql_db.py` & `phidata-2.0.0.dev5/phidata/app/mysql/mysql_db.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/neo4j/neo4j.py` & `phidata-2.0.0.dev5/phidata/app/neo4j/neo4j.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/nodeexporter/nodeexporter.py` & `phidata-2.0.0.dev5/phidata/app/nodeexporter/nodeexporter.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/phidata_app.py` & `phidata-2.0.0.dev5/phidata/app/phidata_app.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/postgres/postgres_db.py` & `phidata-2.0.0.dev5/phidata/app/postgres/postgres_db.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/prometheus/prometheus.py` & `phidata-2.0.0.dev5/phidata/app/prometheus/prometheus.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/qdrant/qdrant.py` & `phidata-2.0.0.dev5/phidata/app/qdrant/qdrant.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/redis/redis.py` & `phidata-2.0.0.dev5/phidata/app/redis/redis.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/redis/stack.py` & `phidata-2.0.0.dev5/phidata/app/redis/stack.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/server/api_server.py` & `phidata-2.0.0.dev5/phidata/app/server/api_server.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/server/server_base.py` & `phidata-2.0.0.dev5/phidata/app/server/server_base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/spark/spark_base.py` & `phidata-2.0.0.dev5/phidata/app/spark/spark_base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/spark/spark_driver.py` & `phidata-2.0.0.dev5/phidata/app/spark/spark_driver.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/spark/spark_worker.py` & `phidata-2.0.0.dev5/phidata/app/spark/spark_worker.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/streamlit/streamlit_app.py` & `phidata-2.0.0.dev5/phidata/app/streamlit/streamlit_app.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/superset/superset_base.py` & `phidata-2.0.0.dev5/phidata/app/superset/superset_base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/superset/superset_init.py` & `phidata-2.0.0.dev5/phidata/app/superset/superset_init.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/superset/superset_webserver.py` & `phidata-2.0.0.dev5/phidata/app/superset/superset_webserver.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/superset/superset_worker.py` & `phidata-2.0.0.dev5/phidata/app/superset/superset_worker.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/superset/superset_worker_beat.py` & `phidata-2.0.0.dev5/phidata/app/superset/superset_worker_beat.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/traefik/crds.py` & `phidata-2.0.0.dev5/phidata/app/traefik/crds.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/traefik/ingress_route.py` & `phidata-2.0.0.dev5/phidata/app/traefik/ingress_route.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/app/traefik/router.py` & `phidata-2.0.0.dev5/phidata/app/traefik/router.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/asset/aws/aws_asset.py` & `phidata-2.0.0.dev5/phidata/asset/aws/aws_asset.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/asset/data_asset.py` & `phidata-2.0.0.dev5/phidata/asset/data_asset.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/asset/local/file.py` & `phidata-2.0.0.dev5/phidata/asset/local/file.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/asset/local/local_asset.py` & `phidata-2.0.0.dev5/phidata/asset/local/local_asset.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/aws/api_client.py` & `phidata-2.0.0.dev5/phidata/aws/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/aws/athena/query.py` & `phidata-2.0.0.dev5/phidata/aws/athena/query.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/aws/config.py` & `phidata-2.0.0.dev5/phidata/aws/config.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/aws/create/iam/eks_admin_role.py` & `phidata-2.0.0.dev5/phidata/aws/create/iam/eks_admin_role.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/aws/create/iam/role.py` & `phidata-2.0.0.dev5/phidata/aws/create/iam/role.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/aws/driver.py` & `phidata-2.0.0.dev5/phidata/aws/driver.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/aws/enums/manager_status.py` & `phidata-2.0.0.dev5/phidata/aws/enums/manager_status.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/aws/manager.py` & `phidata-2.0.0.dev5/phidata/aws/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/aws/resource/acm/certificate.py` & `phidata-2.0.0.dev5/phidata/aws/resource/acm/certificate.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/aws/resource/athena/query.py` & `phidata-2.0.0.dev5/phidata/aws/resource/athena/query.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/aws/resource/base.py` & `phidata-2.0.0.dev5/phidata/aws/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/aws/resource/cloudformation/stack.py` & `phidata-2.0.0.dev5/phidata/aws/resource/cloudformation/stack.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/aws/resource/ec2/security_group.py` & `phidata-2.0.0.dev5/phidata/aws/resource/ec2/security_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/aws/resource/ec2/subnet.py` & `phidata-2.0.0.dev5/phidata/aws/resource/ec2/subnet.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/aws/resource/ec2/volume.py` & `phidata-2.0.0.dev5/phidata/aws/resource/ec2/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/aws/resource/ecs/cluster.py` & `phidata-2.0.0.dev5/phidata/aws/resource/ecs/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/aws/resource/ecs/container.py` & `phidata-2.0.0.dev5/phidata/aws/resource/ecs/container.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/aws/resource/ecs/service.py` & `phidata-2.0.0.dev5/phidata/aws/resource/ecs/service.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/aws/resource/ecs/task_definition.py` & `phidata-2.0.0.dev5/phidata/aws/resource/ecs/task_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/aws/resource/ecs/volume.py` & `phidata-2.0.0.dev5/phidata/aws/resource/ecs/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/aws/resource/eks/addon.py` & `phidata-2.0.0.dev5/phidata/aws/resource/eks/addon.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/aws/resource/eks/cluster.py` & `phidata-2.0.0.dev5/phidata/aws/resource/eks/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/aws/resource/eks/fargate_profile.py` & `phidata-2.0.0.dev5/phidata/aws/resource/eks/fargate_profile.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/aws/resource/eks/kubeconfig.py` & `phidata-2.0.0.dev5/phidata/aws/resource/eks/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/aws/resource/eks/node_group.py` & `phidata-2.0.0.dev5/phidata/aws/resource/eks/node_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/aws/resource/elasticache/cluster.py` & `phidata-2.0.0.dev5/phidata/aws/resource/elasticache/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/aws/resource/elasticache/subnet_group.py` & `phidata-2.0.0.dev5/phidata/aws/resource/elasticache/subnet_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/aws/resource/elb/listener.py` & `phidata-2.0.0.dev5/phidata/aws/resource/elb/listener.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/aws/resource/elb/load_balancer.py` & `phidata-2.0.0.dev5/phidata/aws/resource/elb/load_balancer.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/aws/resource/elb/target_group.py` & `phidata-2.0.0.dev5/phidata/aws/resource/elb/target_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/aws/resource/emr/cluster.py` & `phidata-2.0.0.dev5/phidata/aws/resource/emr/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/aws/resource/glue/crawler.py` & `phidata-2.0.0.dev5/phidata/aws/resource/glue/crawler.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/aws/resource/group.py` & `phidata-2.0.0.dev5/phidata/aws/resource/group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/aws/resource/iam/group.py` & `phidata-2.0.0.dev5/phidata/aws/resource/iam/group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/aws/resource/iam/policy.py` & `phidata-2.0.0.dev5/phidata/aws/resource/iam/policy.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/aws/resource/iam/role.py` & `phidata-2.0.0.dev5/phidata/aws/resource/iam/role.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/aws/resource/rds/db_cluster.py` & `phidata-2.0.0.dev5/phidata/aws/resource/rds/db_cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/aws/resource/rds/db_instance.py` & `phidata-2.0.0.dev5/phidata/aws/resource/rds/db_instance.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/aws/resource/rds/db_subnet_group.py` & `phidata-2.0.0.dev5/phidata/aws/resource/rds/db_subnet_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/aws/resource/s3/bucket.py` & `phidata-2.0.0.dev5/phidata/aws/resource/s3/bucket.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/aws/resource/secret/manager.py` & `phidata-2.0.0.dev5/phidata/aws/resource/secret/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/aws/resource/secret/reader.py` & `phidata-2.0.0.dev5/phidata/aws/resource/secret/reader.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/aws/resource/types.py` & `phidata-2.0.0.dev5/phidata/aws/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/aws/resource/utils.py` & `phidata-2.0.0.dev5/phidata/aws/resource/utils.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/aws/s3/csv_dataset.py` & `phidata-2.0.0.dev5/phidata/aws/s3/csv_dataset.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/aws/s3/dataset.py` & `phidata-2.0.0.dev5/phidata/aws/s3/dataset.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/aws/s3/dataset_base.py` & `phidata-2.0.0.dev5/phidata/aws/s3/dataset_base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/aws/s3/object.py` & `phidata-2.0.0.dev5/phidata/aws/s3/object.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/aws/worker.py` & `phidata-2.0.0.dev5/phidata/aws/worker.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/base.py` & `phidata-2.0.0.dev5/phidata/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/checks/check.py` & `phidata-2.0.0.dev5/phidata/checks/check.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/checks/not_empty.py` & `phidata-2.0.0.dev5/phidata/checks/not_empty.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/constants.py` & `phidata-2.0.0.dev5/phidata/constants.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/decorators/timer.py` & `phidata-2.0.0.dev5/phidata/decorators/timer.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/decorators/validate_env.py` & `phidata-2.0.0.dev5/phidata/decorators/validate_env.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/docker/api_client.py` & `phidata-2.0.0.dev5/phidata/docker/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/docker/args.py` & `phidata-2.0.0.dev5/phidata/docker/args.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/docker/config.py` & `phidata-2.0.0.dev5/phidata/docker/config.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/docker/enums.py` & `phidata-2.0.0.dev5/phidata/docker/enums.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/docker/manager.py` & `phidata-2.0.0.dev5/phidata/docker/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/docker/resource/base.py` & `phidata-2.0.0.dev5/phidata/docker/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/docker/resource/container.py` & `phidata-2.0.0.dev5/phidata/docker/resource/container.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/docker/resource/group.py` & `phidata-2.0.0.dev5/phidata/docker/resource/group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/docker/resource/image.py` & `phidata-2.0.0.dev5/phidata/docker/resource/image.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/docker/resource/network.py` & `phidata-2.0.0.dev5/phidata/docker/resource/network.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/docker/resource/types.py` & `phidata-2.0.0.dev5/phidata/docker/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/docker/resource/utils.py` & `phidata-2.0.0.dev5/phidata/docker/resource/utils.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/docker/resource/volume.py` & `phidata-2.0.0.dev5/phidata/docker/resource/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/docker/utils/container.py` & `phidata-2.0.0.dev5/phidata/docker/utils/container.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/docker/worker.py` & `phidata-2.0.0.dev5/phidata/docker/worker.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/infra/args.py` & `phidata-2.0.0.dev5/phidata/infra/args.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/infra/config.py` & `phidata-2.0.0.dev5/phidata/infra/config.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/infra/resource.py` & `phidata-2.0.0.dev5/phidata/infra/resource.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/api_client.py` & `phidata-2.0.0.dev5/phidata/k8s/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/args.py` & `phidata-2.0.0.dev5/phidata/k8s/args.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/config.py` & `phidata-2.0.0.dev5/phidata/k8s/config.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py` & `phidata-2.0.0.dev5/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py` & `phidata-2.0.0.dev5/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/create/apps/v1/deployment.py` & `phidata-2.0.0.dev5/phidata/k8s/create/apps/v1/deployment.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/create/common/port.py` & `phidata-2.0.0.dev5/phidata/k8s/create/common/port.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/create/core/v1/config_map.py` & `phidata-2.0.0.dev5/phidata/k8s/create/core/v1/config_map.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/create/core/v1/container.py` & `phidata-2.0.0.dev5/phidata/k8s/create/core/v1/container.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/create/core/v1/namespace.py` & `phidata-2.0.0.dev5/phidata/k8s/create/core/v1/namespace.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/create/core/v1/persistent_volume.py` & `phidata-2.0.0.dev5/phidata/k8s/create/core/v1/persistent_volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/create/core/v1/persistent_volume_claim.py` & `phidata-2.0.0.dev5/phidata/k8s/create/core/v1/persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/create/core/v1/secret.py` & `phidata-2.0.0.dev5/phidata/k8s/create/core/v1/secret.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/create/core/v1/service.py` & `phidata-2.0.0.dev5/phidata/k8s/create/core/v1/service.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/create/core/v1/service_account.py` & `phidata-2.0.0.dev5/phidata/k8s/create/core/v1/service_account.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/create/core/v1/volume.py` & `phidata-2.0.0.dev5/phidata/k8s/create/core/v1/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/create/crb/eks_admin_crb.py` & `phidata-2.0.0.dev5/phidata/k8s/create/crb/eks_admin_crb.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/create/group.py` & `phidata-2.0.0.dev5/phidata/k8s/create/group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/create/kubeconfig.py` & `phidata-2.0.0.dev5/phidata/k8s/create/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/create/networking_k8s_io/v1/ingress.py` & `phidata-2.0.0.dev5/phidata/k8s/create/networking_k8s_io/v1/ingress.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py` & `phidata-2.0.0.dev5/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py` & `phidata-2.0.0.dev5/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/create/storage_k8s_io/v1/storage_class.py` & `phidata-2.0.0.dev5/phidata/k8s/create/storage_k8s_io/v1/storage_class.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/enums/api_version.py` & `phidata-2.0.0.dev5/phidata/k8s/enums/api_version.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/enums/kind.py` & `phidata-2.0.0.dev5/phidata/k8s/enums/kind.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/enums/manager_status.py` & `phidata-2.0.0.dev5/phidata/k8s/enums/manager_status.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/enums/pv.py` & `phidata-2.0.0.dev5/phidata/k8s/enums/pv.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/manager.py` & `phidata-2.0.0.dev5/phidata/k8s/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py` & `phidata-2.0.0.dev5/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py` & `phidata-2.0.0.dev5/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/resource/apps/v1/deployment.py` & `phidata-2.0.0.dev5/phidata/k8s/resource/apps/v1/deployment.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/resource/apps/v1/deployment_strategy.py` & `phidata-2.0.0.dev5/phidata/k8s/resource/apps/v1/deployment_strategy.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/resource/base.py` & `phidata-2.0.0.dev5/phidata/k8s/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/resource/core/v1/config_map.py` & `phidata-2.0.0.dev5/phidata/k8s/resource/core/v1/config_map.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/resource/core/v1/container.py` & `phidata-2.0.0.dev5/phidata/k8s/resource/core/v1/container.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/resource/core/v1/local_object_reference.py` & `phidata-2.0.0.dev5/phidata/k8s/resource/core/v1/local_object_reference.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/resource/core/v1/namespace.py` & `phidata-2.0.0.dev5/phidata/k8s/resource/core/v1/namespace.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/resource/core/v1/node_selector.py` & `phidata-2.0.0.dev5/phidata/k8s/resource/core/v1/node_selector.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/resource/core/v1/object_reference.py` & `phidata-2.0.0.dev5/phidata/k8s/resource/core/v1/object_reference.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/resource/core/v1/persistent_volume.py` & `phidata-2.0.0.dev5/phidata/k8s/resource/core/v1/persistent_volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/resource/core/v1/persistent_volume_claim.py` & `phidata-2.0.0.dev5/phidata/k8s/resource/core/v1/persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/resource/core/v1/pod.py` & `phidata-2.0.0.dev5/phidata/k8s/resource/core/v1/pod.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/resource/core/v1/pod_spec.py` & `phidata-2.0.0.dev5/phidata/k8s/resource/core/v1/pod_spec.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/resource/core/v1/pod_template_spec.py` & `phidata-2.0.0.dev5/phidata/k8s/resource/core/v1/pod_template_spec.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/resource/core/v1/resource_requirements.py` & `phidata-2.0.0.dev5/phidata/k8s/resource/core/v1/resource_requirements.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/resource/core/v1/secret.py` & `phidata-2.0.0.dev5/phidata/k8s/resource/core/v1/secret.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/resource/core/v1/service.py` & `phidata-2.0.0.dev5/phidata/k8s/resource/core/v1/service.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/resource/core/v1/service_account.py` & `phidata-2.0.0.dev5/phidata/k8s/resource/core/v1/service_account.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/resource/core/v1/toleration.py` & `phidata-2.0.0.dev5/phidata/k8s/resource/core/v1/toleration.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/resource/core/v1/topology_spread_constraints.py` & `phidata-2.0.0.dev5/phidata/k8s/resource/core/v1/topology_spread_constraints.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/resource/core/v1/volume.py` & `phidata-2.0.0.dev5/phidata/k8s/resource/core/v1/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/resource/core/v1/volume_node_affinity.py` & `phidata-2.0.0.dev5/phidata/k8s/resource/core/v1/volume_node_affinity.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/resource/core/v1/volume_source.py` & `phidata-2.0.0.dev5/phidata/k8s/resource/core/v1/volume_source.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/resource/group.py` & `phidata-2.0.0.dev5/phidata/k8s/resource/group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/resource/kubeconfig.py` & `phidata-2.0.0.dev5/phidata/k8s/resource/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/resource/meta/v1/label_selector.py` & `phidata-2.0.0.dev5/phidata/k8s/resource/meta/v1/label_selector.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/resource/meta/v1/object_meta.py` & `phidata-2.0.0.dev5/phidata/k8s/resource/meta/v1/object_meta.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/resource/networking_k8s_io/v1/ingress.py` & `phidata-2.0.0.dev5/phidata/k8s/resource/networking_k8s_io/v1/ingress.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py` & `phidata-2.0.0.dev5/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py` & `phidata-2.0.0.dev5/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py` & `phidata-2.0.0.dev5/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/resource/types.py` & `phidata-2.0.0.dev5/phidata/k8s/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/resource/utils.py` & `phidata-2.0.0.dev5/phidata/k8s/resource/utils.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/utils/pod.py` & `phidata-2.0.0.dev5/phidata/k8s/utils/pod.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/k8s/worker.py` & `phidata-2.0.0.dev5/phidata/k8s/worker.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/llm/duckdb/agent.py` & `phidata-2.0.0.dev5/phidata/llm/duckdb/agent.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/llm/duckdb/chain.py` & `phidata-2.0.0.dev5/phidata/llm/duckdb/chain.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/llm/duckdb/connection.py` & `phidata-2.0.0.dev5/phidata/llm/duckdb/connection.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/llm/duckdb/loader.py` & `phidata-2.0.0.dev5/phidata/llm/duckdb/loader.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/llm/duckdb/query.py` & `phidata-2.0.0.dev5/phidata/llm/duckdb/query.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/llm/duckdb/tool.py` & `phidata-2.0.0.dev5/phidata/llm/duckdb/tool.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/product/data_product.py` & `phidata-2.0.0.dev5/phidata/product/data_product.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/table/local/csv.py` & `phidata-2.0.0.dev5/phidata/table/local/csv.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/table/local/local_table.py` & `phidata-2.0.0.dev5/phidata/table/local/local_table.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/table/local/parquet.py` & `phidata-2.0.0.dev5/phidata/table/local/parquet.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/table/s3/csv.py` & `phidata-2.0.0.dev5/phidata/table/s3/csv.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/table/s3/parquet.py` & `phidata-2.0.0.dev5/phidata/table/s3/parquet.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/table/s3/s3_table.py` & `phidata-2.0.0.dev5/phidata/table/s3/s3_table.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/table/sql/postgres.py` & `phidata-2.0.0.dev5/phidata/table/sql/postgres.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/table/sql/sql_table.py` & `phidata-2.0.0.dev5/phidata/table/sql/sql_table.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/task/aws/athena/run_query.py` & `phidata-2.0.0.dev5/phidata/task/aws/athena/run_query.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/task/aws/emr/create_cluster.py` & `phidata-2.0.0.dev5/phidata/task/aws/emr/create_cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/task/aws/emr/delete_cluster.py` & `phidata-2.0.0.dev5/phidata/task/aws/emr/delete_cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/task/aws/glue/start_crawler.py` & `phidata-2.0.0.dev5/phidata/task/aws/glue/start_crawler.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/task/decorator.py` & `phidata-2.0.0.dev5/phidata/task/decorator.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/task/download/s3/to_file.py` & `phidata-2.0.0.dev5/phidata/task/download/s3/to_file.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/task/download/url/to_file.py` & `phidata-2.0.0.dev5/phidata/task/download/url/to_file.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/task/download/url/to_s3.py` & `phidata-2.0.0.dev5/phidata/task/download/url/to_s3.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/task/download/url/to_sql.py` & `phidata-2.0.0.dev5/phidata/task/download/url/to_sql.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/task/plot/sql/query.py` & `phidata-2.0.0.dev5/phidata/task/plot/sql/query.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/task/python_task.py` & `phidata-2.0.0.dev5/phidata/task/python_task.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/task/run/sql/query.py` & `phidata-2.0.0.dev5/phidata/task/run/sql/query.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/task/task.py` & `phidata-2.0.0.dev5/phidata/task/task.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/task/task_relatives.py` & `phidata-2.0.0.dev5/phidata/task/task_relatives.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/task/upload/file/to_s3.py` & `phidata-2.0.0.dev5/phidata/task/upload/file/to_s3.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/task/upload/file/to_sql.py` & `phidata-2.0.0.dev5/phidata/task/upload/file/to_sql.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/types/airflow.py` & `phidata-2.0.0.dev5/phidata/types/airflow.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/types/context.py` & `phidata-2.0.0.dev5/phidata/types/context.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/types/phidata_runtime.py` & `phidata-2.0.0.dev5/phidata/types/phidata_runtime.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/utils/cli_console.py` & `phidata-2.0.0.dev5/phidata/utils/cli_console.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/utils/common.py` & `phidata-2.0.0.dev5/phidata/utils/common.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/utils/compare.py` & `phidata-2.0.0.dev5/phidata/utils/compare.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/utils/context.py` & `phidata-2.0.0.dev5/phidata/utils/context.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/utils/dttm.py` & `phidata-2.0.0.dev5/phidata/utils/dttm.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/utils/enums.py` & `phidata-2.0.0.dev5/phidata/utils/enums.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/utils/env_file.py` & `phidata-2.0.0.dev5/phidata/utils/env_file.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/utils/env_var.py` & `phidata-2.0.0.dev5/phidata/utils/env_var.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/utils/filesystem.py` & `phidata-2.0.0.dev5/phidata/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/utils/get_python_objects_from_module.py` & `phidata-2.0.0.dev5/phidata/utils/get_python_objects_from_module.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/utils/json_io.py` & `phidata-2.0.0.dev5/phidata/utils/json_io.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/utils/k8s.py` & `phidata-2.0.0.dev5/phidata/utils/k8s.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/utils/log.py` & `phidata-2.0.0.dev5/phidata/utils/log.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/utils/print_table.py` & `phidata-2.0.0.dev5/phidata/utils/print_table.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/utils/workspace_path.py` & `phidata-2.0.0.dev5/phidata/utils/workspace_path.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/utils/yaml_io.py` & `phidata-2.0.0.dev5/phidata/utils/yaml_io.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/workflow/decorator.py` & `phidata-2.0.0.dev5/phidata/workflow/decorator.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/workflow/workflow.py` & `phidata-2.0.0.dev5/phidata/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/workflow/workflow_relatives.py` & `phidata-2.0.0.dev5/phidata/workflow/workflow_relatives.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/workspace/config.py` & `phidata-2.0.0.dev5/phidata/workspace/config.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata/workspace/settings.py` & `phidata-2.0.0.dev5/phidata/workspace/settings.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev4/phidata.egg-info/PKG-INFO` & `phidata-2.0.0.dev5/phidata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phidata
-Version: 2.0.0.dev4
+Version: 2.0.0.dev5
 Summary: A toolkit for building applications using OSS
 Author-email: Ashpreet Bedi <ashpreet@phidata.com>
 Project-URL: homepage, https://phidata.com
 Project-URL: documentation, https://docs.phidata.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: phidata Version: 2.0.0.dev4 Summary: A toolkit for
+Metadata-Version: 2.1 Name: phidata Version: 2.0.0.dev5 Summary: A toolkit for
 building applications using OSS Author-email: Ashpreet Bedi
 phidata.com> Project-URL: homepage, https://phidata.com Project-URL:
 documentation, https://docs.phidata.com Requires-Python: >=3.7 Description-
 Content-Type: text/markdown Provides-Extra: dev Provides-Extra: aws License-
 File: LICENSE
                              ****** phidata ******
                       Run open source tools using python
```

### Comparing `phidata-2.0.0.dev4/phidata.egg-info/SOURCES.txt` & `phidata-2.0.0.dev5/phidata.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -109,30 +109,39 @@
 phi/docker/resource/types.py
 phi/docker/resource/volume.py
 phi/document/__init__.py
 phi/document/base.py
 phi/document/reader/__init__.py
 phi/document/reader/base.py
 phi/document/reader/pdf.py
-phi/document/table/__init__.py
-phi/document/table/base.py
+phi/embedder/__init__.py
+phi/embedder/base.py
+phi/embedder/openai.py
 phi/infra/__init__.py
 phi/infra/enums.py
 phi/infra/app/__init__.py
 phi/infra/app/base.py
 phi/infra/app/context.py
 phi/infra/app/db_app.py
 phi/infra/resource/__init__.py
 phi/infra/resource/base.py
 phi/infra/resource/group.py
 phi/k8s/__init__.py
 phi/llm/__init__.py
+phi/llm/base.py
+phi/llm/openai.py
 phi/llm/conversation/__init__.py
-phi/llm/conversation/db.py
+phi/llm/conversation/conversation.py
 phi/llm/conversation/schemas.py
+phi/llm/conversation/storage/__init__.py
+phi/llm/conversation/storage/base.py
+phi/llm/conversation/storage/postgres.py
+phi/llm/knowledge/__init__.py
+phi/llm/knowledge/base.py
+phi/llm/knowledge/pdf.py
 phi/schemas/__init__.py
 phi/schemas/response.py
 phi/schemas/user.py
 phi/schemas/workspace.py
 phi/table/__init__.py
 phi/table/sql/__init__.py
 phi/table/sql/base.py
@@ -147,15 +156,17 @@
 phi/utils/log.py
 phi/utils/pickle.py
 phi/utils/py_io.py
 phi/utils/pyproject.py
 phi/utils/resource_filter.py
 phi/utils/yaml_io.py
 phi/vectordb/__init__.py
+phi/vectordb/base.py
 phi/vectordb/pgvector/__init__.py
+phi/vectordb/pgvector/pgvector.py
 phi/workspace/__init__.py
 phi/workspace/config.py
 phi/workspace/enums.py
 phi/workspace/helpers.py
 phi/workspace/operator.py
 phi/workspace/settings.py
 phidata/__init__.py
```

### Comparing `phidata-2.0.0.dev4/pyproject.toml` & `phidata-2.0.0.dev5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "phidata"
-version = "2.0.0.dev4"
+version = "2.0.0.dev5"
 description = "A toolkit for building applications using OSS"
 requires-python = ">=3.7"
 readme = "README.md"
 authors = [
   {name = "Ashpreet Bedi", email = "ashpreet@phidata.com"}
 ]
```

