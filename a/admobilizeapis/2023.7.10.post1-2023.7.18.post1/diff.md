# Comparing `tmp/admobilizeapis-2023.7.10.post1.tar.gz` & `tmp/admobilizeapis-2023.7.18.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/admobilizeapis-2023.7.10.post1.tar", last modified: Mon Jul 10 14:53:50 2023, max compression
+gzip compressed data, was "dist/admobilizeapis-2023.7.18.post1.tar", last modified: Tue Jul 18 02:43:27 2023, max compression
```

## Comparing `admobilizeapis-2023.7.10.post1.tar` & `admobilizeapis-2023.7.18.post1.tar`

### file list

```diff
@@ -1,182 +1,182 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/
--rw-r--r--   0 root         (0) root         (0)       56 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/google/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/google/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/google/longrunning/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/google/longrunning/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8090 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/google/longrunning/operations_pb2.py
--rw-r--r--   0 root         (0) root         (0)    10932 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/google/longrunning/operations_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/wifi/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/wifi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/wifi/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/wifi/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/wifi/v1/wifi_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2457 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/wifi/v1/wifi_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/datagateway/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/datagateway/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/datagateway/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/datagateway/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8861 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/datagateway/v1alpha1/datagateway_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     8708 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/datagateway/v1alpha1/datagateway_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/iam/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/iam/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/iam/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/iam/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/iam/v1alpha1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    25837 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/iam/v1alpha1/iam_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4250 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/iam/v1alpha1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    35932 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/iam/v1alpha1/iam_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/notification/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/notification/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/notification/v1beta1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/notification/v1beta1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/notification/v1beta1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     6645 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/notification/v1beta1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    10396 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/notification/v1beta1/notification_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    14597 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/notification/v1beta1/notification_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/vision/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/vision/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/vision/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/vision/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/vision/v1/model_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2515 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/vision/v1/vision_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2912 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/vision/v1/vision_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/vision/v1/vision_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     4194 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/vision/v1/model_pb2.py
--rw-r--r--   0 root         (0) root         (0)    26810 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/vision/v1/vision_pb2.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/mlmodel/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/mlmodel/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/mlmodel/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)     6478 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/mlmodel/v1alpha1/mlmodel_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/mlmodel/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5542 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/mlmodel/v1alpha1/mlmodel_service_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/salestool/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/salestool/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/salestool/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/salestool/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4784 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/salestool/v1alpha1/salestool_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     5528 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/salestool/v1alpha1/salestool_service_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    15461 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    39106 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1/device_manager_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    28693 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1/device_manager_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha2/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha2/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha2/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    10609 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha2/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    28083 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha2/device_manager_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    18992 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha2/device_manager_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v2/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v2/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v2/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    20392 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v2/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    99455 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v2/device_manager_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    76701 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v2/device_manager_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha3/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha3/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha3/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    13543 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha3/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    41623 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha3/device_manager_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    29786 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha3/device_manager_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     9576 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    14877 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha1/device_manager_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    15271 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha1/device_manager_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/admprovider/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/admprovider/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/admprovider/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/admprovider/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/admprovider/v1alpha1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     6954 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/admprovider/v1alpha1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    22477 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/admprovider/v1alpha1/admprovider_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     8758 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/admprovider/v1alpha1/admprovider_service_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/malos/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/malos/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/malos/v1/
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/malos/v1/driver_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/malos/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4590 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/malos/v1/driver_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6136 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/malos/v1/maloseye_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/malos/v1/maloseye_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/query/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/query/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/query/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/query/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/query/v1alpha1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    15710 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/query/v1alpha1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    32988 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/query/v1alpha1/query_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    29571 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/query/v1alpha1/query_service_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/ayuda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/ayuda/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/ayuda/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/ayuda/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/ayuda/v1alpha1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    15801 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/ayuda/v1alpha1/ayuda_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    21203 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/ayuda/v1alpha1/ayuda_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3157 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/ayuda/v1alpha1/resources_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/signagelive/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/signagelive/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/signagelive/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/signagelive/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18378 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/signagelive/v1alpha1/signagelive_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/signagelive/v1alpha1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    24106 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/signagelive/v1alpha1/signagelive_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3240 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/signagelive/v1alpha1/resources_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/common/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/common/job_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/common/admobilize_types_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     4485 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/common/entity_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2623 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/common/admobilize_types_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2897 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/common/job_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/common/entity_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/billing/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/billing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/billing/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/billing/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2506 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/billing/v1alpha1/billing_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/billing/v1alpha1/billing_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/brightauthor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/brightauthor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/brightauthor/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)    22301 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/brightauthor/v1alpha1/brightauthor_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/brightauthor/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/brightauthor/v1alpha1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3246 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/brightauthor/v1alpha1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    16652 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/brightauthor/v1alpha1/brightauthor_service_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/cmsintegrations/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/cmsintegrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/cmsintegrations/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/cmsintegrations/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/cmsintegrations/v1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    29481 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/cmsintegrations/v1/cmsintegrations_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    10026 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/cmsintegrations/v1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    24348 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/cmsintegrations/v1/cmsintegrations_service_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/broadsign/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/broadsign/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/broadsign/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/broadsign/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21841 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/broadsign/v1alpha1/broadsign_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/broadsign/v1alpha1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3174 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/broadsign/v1alpha1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    16356 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/admobilize/proto/broadsign/v1alpha1/broadsign_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)      849 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilizeapis.egg-info/
--rw-r--r--   0 root         (0) root         (0)       76 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilizeapis.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilizeapis.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)     6814 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilizeapis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      849 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilizeapis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilizeapis.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/admobilizeapis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1201 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/README.md
--rw-r--r--   0 root         (0) root         (0)     1293 2023-07-10 14:53:49.000000 admobilizeapis-2023.7.10.post1/setup.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 14:53:50.000000 admobilizeapis-2023.7.10.post1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:43:27.000000 admobilizeapis-2023.7.18.post1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:43:27.000000 admobilizeapis-2023.7.18.post1/admobilize/
+-rw-r--r--   0 root         (0) root         (0)       56 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:43:27.000000 admobilizeapis-2023.7.18.post1/admobilize/google/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/google/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:43:27.000000 admobilizeapis-2023.7.18.post1/admobilize/google/longrunning/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/google/longrunning/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8090 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/google/longrunning/operations_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    10932 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/google/longrunning/operations_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:43:27.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:43:27.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/wifi/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/wifi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:43:27.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/wifi/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/wifi/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/wifi/v1/wifi_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2457 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/wifi/v1/wifi_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:43:27.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/datagateway/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/datagateway/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:43:27.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/datagateway/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/datagateway/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8861 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/datagateway/v1alpha1/datagateway_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     8708 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/datagateway/v1alpha1/datagateway_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:43:27.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/iam/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/iam/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:43:27.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/iam/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/iam/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/iam/v1alpha1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    25837 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/iam/v1alpha1/iam_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4250 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/iam/v1alpha1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    35932 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/iam/v1alpha1/iam_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:43:27.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/notification/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/notification/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:43:27.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/notification/v1beta1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/notification/v1beta1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/notification/v1beta1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     6645 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/notification/v1beta1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    10396 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/notification/v1beta1/notification_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    14597 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/notification/v1beta1/notification_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:43:27.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/vision/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/vision/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:43:27.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/vision/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/vision/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/vision/v1/model_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2515 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/vision/v1/vision_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2912 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/vision/v1/vision_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/vision/v1/vision_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     4194 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/vision/v1/model_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    26810 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/vision/v1/vision_pb2.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:43:27.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/mlmodel/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/mlmodel/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:43:27.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/mlmodel/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)     6478 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/mlmodel/v1alpha1/mlmodel_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/mlmodel/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5542 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/mlmodel/v1alpha1/mlmodel_service_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:43:27.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/salestool/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/salestool/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:43:27.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/salestool/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/salestool/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4784 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/salestool/v1alpha1/salestool_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     5528 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/salestool/v1alpha1/salestool_service_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:43:27.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/devicemanagement/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/devicemanagement/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:43:27.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/devicemanagement/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/devicemanagement/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/devicemanagement/v1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    15461 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/devicemanagement/v1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    39106 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/devicemanagement/v1/device_manager_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    28693 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/devicemanagement/v1/device_manager_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:43:27.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/devicemanagement/v1alpha2/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/devicemanagement/v1alpha2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/devicemanagement/v1alpha2/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    10609 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/devicemanagement/v1alpha2/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    28083 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/devicemanagement/v1alpha2/device_manager_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    18992 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/devicemanagement/v1alpha2/device_manager_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:43:27.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/devicemanagement/v2/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/devicemanagement/v2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/devicemanagement/v2/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    20392 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/devicemanagement/v2/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    99455 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/devicemanagement/v2/device_manager_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    76701 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/devicemanagement/v2/device_manager_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:43:27.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/devicemanagement/v1alpha3/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/devicemanagement/v1alpha3/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/devicemanagement/v1alpha3/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    13543 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/devicemanagement/v1alpha3/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    41623 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/devicemanagement/v1alpha3/device_manager_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    29786 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/devicemanagement/v1alpha3/device_manager_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:43:27.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/devicemanagement/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/devicemanagement/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/devicemanagement/v1alpha1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     9576 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/devicemanagement/v1alpha1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    14877 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/devicemanagement/v1alpha1/device_manager_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    15271 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/devicemanagement/v1alpha1/device_manager_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:43:27.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/admprovider/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/admprovider/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:43:27.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/admprovider/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/admprovider/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/admprovider/v1alpha1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     6954 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/admprovider/v1alpha1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    22477 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/admprovider/v1alpha1/admprovider_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     8758 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/admprovider/v1alpha1/admprovider_service_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:43:27.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/malos/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/malos/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:43:27.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/malos/v1/
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/malos/v1/driver_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/malos/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4590 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/malos/v1/driver_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6136 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/malos/v1/maloseye_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/malos/v1/maloseye_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:43:27.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/query/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/query/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:43:27.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/query/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/query/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/query/v1alpha1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    17400 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/query/v1alpha1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    36631 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/query/v1alpha1/query_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    31808 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/query/v1alpha1/query_service_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:43:27.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/ayuda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/ayuda/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:43:27.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/ayuda/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/ayuda/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/ayuda/v1alpha1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    15801 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/ayuda/v1alpha1/ayuda_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    21203 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/ayuda/v1alpha1/ayuda_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3157 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/ayuda/v1alpha1/resources_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:43:27.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/signagelive/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/signagelive/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:43:27.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/signagelive/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/signagelive/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18378 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/signagelive/v1alpha1/signagelive_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/signagelive/v1alpha1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    24106 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/signagelive/v1alpha1/signagelive_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3240 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/signagelive/v1alpha1/resources_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:43:27.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/common/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/common/job_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/common/admobilize_types_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     4485 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/common/entity_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2623 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/common/admobilize_types_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2897 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/common/job_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/common/entity_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:43:27.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/billing/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/billing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:43:27.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/billing/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/billing/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2506 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/billing/v1alpha1/billing_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/billing/v1alpha1/billing_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:43:27.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/brightauthor/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/brightauthor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:43:27.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/brightauthor/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)    22301 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/brightauthor/v1alpha1/brightauthor_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/brightauthor/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/brightauthor/v1alpha1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3246 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/brightauthor/v1alpha1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    16652 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/brightauthor/v1alpha1/brightauthor_service_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:43:27.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/cmsintegrations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/cmsintegrations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:43:27.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/cmsintegrations/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/cmsintegrations/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/cmsintegrations/v1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    29481 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/cmsintegrations/v1/cmsintegrations_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    10026 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/cmsintegrations/v1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    24348 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/cmsintegrations/v1/cmsintegrations_service_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:43:27.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/broadsign/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/broadsign/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:43:27.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/broadsign/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/broadsign/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21841 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/broadsign/v1alpha1/broadsign_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/broadsign/v1alpha1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3174 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/broadsign/v1alpha1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    16356 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilize/proto/broadsign/v1alpha1/broadsign_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      849 2023-07-18 02:43:27.000000 admobilizeapis-2023.7.18.post1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:43:27.000000 admobilizeapis-2023.7.18.post1/admobilizeapis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       76 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilizeapis.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilizeapis.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)     6814 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilizeapis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      849 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilizeapis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilizeapis.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/admobilizeapis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1201 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/README.md
+-rw-r--r--   0 root         (0) root         (0)     1293 2023-07-18 02:43:26.000000 admobilizeapis-2023.7.18.post1/setup.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 02:43:27.000000 admobilizeapis-2023.7.18.post1/setup.cfg
```

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/google/longrunning/operations_pb2.py` & `admobilizeapis-2023.7.18.post1/admobilize/google/longrunning/operations_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/google/longrunning/operations_pb2_grpc.py` & `admobilizeapis-2023.7.18.post1/admobilize/google/longrunning/operations_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/wifi/v1/wifi_pb2.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/wifi/v1/wifi_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/datagateway/v1alpha1/datagateway_service_pb2.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/datagateway/v1alpha1/datagateway_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/datagateway/v1alpha1/datagateway_service_pb2_grpc.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/datagateway/v1alpha1/datagateway_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/iam/v1alpha1/iam_service_pb2.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/iam/v1alpha1/iam_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/iam/v1alpha1/resources_pb2.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/iam/v1alpha1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/iam/v1alpha1/iam_service_pb2_grpc.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/iam/v1alpha1/iam_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/notification/v1beta1/resources_pb2.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/notification/v1beta1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/notification/v1beta1/notification_service_pb2.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/notification/v1beta1/notification_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/notification/v1beta1/notification_service_pb2_grpc.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/notification/v1beta1/notification_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/vision/v1/vision_service_pb2.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/vision/v1/vision_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/vision/v1/vision_service_pb2_grpc.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/vision/v1/vision_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/vision/v1/model_pb2.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/vision/v1/model_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/vision/v1/vision_pb2.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/vision/v1/vision_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/mlmodel/v1alpha1/mlmodel_service_pb2_grpc.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/mlmodel/v1alpha1/mlmodel_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/mlmodel/v1alpha1/mlmodel_service_pb2.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/mlmodel/v1alpha1/mlmodel_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/salestool/v1alpha1/salestool_service_pb2_grpc.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/salestool/v1alpha1/salestool_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/salestool/v1alpha1/salestool_service_pb2.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/salestool/v1alpha1/salestool_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1/resources_pb2.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/devicemanagement/v1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1/device_manager_pb2_grpc.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/devicemanagement/v1/device_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1/device_manager_pb2.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/devicemanagement/v1/device_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha2/resources_pb2.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/devicemanagement/v1alpha2/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha2/device_manager_pb2_grpc.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/devicemanagement/v1alpha2/device_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha2/device_manager_pb2.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/devicemanagement/v1alpha2/device_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v2/resources_pb2.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/devicemanagement/v2/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v2/device_manager_pb2_grpc.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/devicemanagement/v2/device_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v2/device_manager_pb2.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/devicemanagement/v2/device_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha3/resources_pb2.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/devicemanagement/v1alpha3/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha3/device_manager_pb2_grpc.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/devicemanagement/v1alpha3/device_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha3/device_manager_pb2.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/devicemanagement/v1alpha3/device_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha1/resources_pb2.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/devicemanagement/v1alpha1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha1/device_manager_pb2_grpc.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/devicemanagement/v1alpha1/device_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/devicemanagement/v1alpha1/device_manager_pb2.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/devicemanagement/v1alpha1/device_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/admprovider/v1alpha1/resources_pb2.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/admprovider/v1alpha1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/admprovider/v1alpha1/admprovider_service_pb2_grpc.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/admprovider/v1alpha1/admprovider_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/admprovider/v1alpha1/admprovider_service_pb2.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/admprovider/v1alpha1/admprovider_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/malos/v1/driver_pb2.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/malos/v1/driver_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/malos/v1/maloseye_pb2.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/malos/v1/maloseye_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/query/v1alpha1/resources_pb2.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/query/v1alpha1/resources_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.protobuf import field_mask_pb2 as google_dot_protobuf_dot_field__mask__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)admobilize/query/v1alpha1/resources.proto\x12\x19\x61\x64mobilize.query.v1alpha1\x1a\x1cgoogle/api/annotations.proto\x1a google/protobuf/field_mask.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1cgoogle/protobuf/struct.proto\"B\n\x07Project\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\x12\n\ncreated_at\x18\x02 \x01(\t\x12\x12\n\nupdated_at\x18\x03 \x01(\t\"2\n\x0bHeatmapData\x12\t\n\x01x\x18\x01 \x01(\r\x12\t\n\x01y\x18\x02 \x01(\r\x12\r\n\x05value\x18\x03 \x01(\x02\"?\n\x07Heatmap\x12\x34\n\x04\x64\x61ta\x18\x01 \x03(\x0b\x32&.admobilize.query.v1alpha1.HeatmapData\"\x80\x01\n\x06Metric\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05\x66ield\x18\x02 \x01(\t\x12\x11\n\toperation\x18\x03 \x01(\t\x12\x0e\n\x06\x66ilter\x18\x04 \x03(\t\x12\r\n\x05order\x18\x05 \x01(\t\x12\x19\n\x11\x63onversion_factor\x18\x06 \x01(\x01\x12\x0c\n\x04\x63\x61st\x18\x07 \x01(\t\"@\n\x0f\x41ggregateResult\x12\x0e\n\x06metric\x18\x01 \x01(\t\x12\x11\n\toperation\x18\x02 \x01(\t\x12\n\n\x02\x61s\x18\x03 \x01(\t\"\xbb\x01\n\x0fQueryFromResult\x12\x0e\n\x06select\x18\x01 \x03(\t\x12\x0b\n\x03sum\x18\x02 \x03(\t\x12\x0b\n\x03\x61vg\x18\x03 \x03(\t\x12\x0f\n\x07groupBy\x18\x04 \x03(\t\x12\x43\n\x07orderBy\x18\x05 \x03(\x0b\x32\x32.admobilize.query.v1alpha1.QueryFromResult.OrderBy\x1a(\n\x07OrderBy\x12\x0e\n\x06\x63olumn\x18\x01 \x01(\t\x12\r\n\x05order\x18\x02 \x01(\t\"4\n\rEncoderParams\x12\x0f\n\x07metrics\x18\x01 \x03(\t\x12\x12\n\ndimensions\x18\x02 \x03(\t\"?\n\x07\x44\x61taset\x12\r\n\x05label\x18\x01 \x01(\t\x12%\n\x05value\x18\x02 \x01(\x0b\x32\x16.google.protobuf.Value\")\n\x0bSchemaField\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\"\x80\x01\n\nClassifier\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\toperation\x18\x02 \x01(\t\x12\r\n\x05\x66ield\x18\x03 \x01(\t\x12\x42\n\nconditions\x18\x04 \x03(\x0b\x32..admobilize.query.v1alpha1.ClassifierCondition\"+\n\nOrderField\x12\x0e\n\x06\x63olumn\x18\x01 \x01(\t\x12\r\n\x05order\x18\x02 \x01(\t\"M\n\x13\x43lassifierCondition\x12\x0c\n\x04when\x18\x01 \x01(\t\x12\r\n\x05start\x18\x02 \x01(\x02\x12\x0b\n\x03\x65nd\x18\x03 \x01(\x02\x12\x0c\n\x04then\x18\x04 \x01(\t\"5\n\x06Status\x12\x13\n\x0bstatus_code\x18\x01 \x01(\t\x12\x16\n\x0estatus_message\x18\x02 \x01(\t\"3\n\tDeviceMap\x12\x11\n\tdevice_id\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65vice_name\x18\x02 \x01(\t\"\xc0\x01\n\x03Job\x12\x0e\n\x06job_id\x18\x01 \x01(\t\x12\x35\n\x06status\x18\x02 \x01(\x0e\x32%.admobilize.query.v1alpha1.Job.Status\x12\x0e\n\x06\x64\x65tail\x18\x03 \x01(\t\x12\x16\n\x0estatus_message\x18\x04 \x01(\t\x12\x11\n\tself_link\x18\x05 \x01(\t\"7\n\x06Status\x12\x0b\n\x07PENDING\x10\x00\x12\x0b\n\x07RUNNING\x10\x01\x12\x08\n\x04\x44ONE\x10\x03\x12\t\n\x05\x45RROR\x10\x04\"\xc9\x04\n\x06Report\x12\n\n\x02id\x18\x01 \x01(\t\x12\x13\n\x0b\x61\x64vertisers\x18\x02 \x03(\t\x12.\n\ncreated_on\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x14\n\x0c\x64\x61ys_to_send\x18\x04 \x03(\t\x12\x12\n\ndevice_ids\x18\x05 \x03(\t\x12\r\n\x05\x65mail\x18\x06 \x03(\t\x12\x0e\n\x06\x66ields\x18\x07 \x03(\t\x12\x0e\n\x06\x66ormat\x18\x08 \x01(\t\x12\x11\n\tfrequency\x18\t \x01(\t\x12\x10\n\x08interval\x18\n \x01(\t\x12-\n\tlast_sent\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x17\n\x0flast_report_url\x18\x0c \x01(\t\x12\r\n\x05media\x18\r \x03(\t\x12\x0c\n\x04name\x18\x0e \x01(\t\x12\x12\n\nproject_id\x18\x0f \x01(\t\x12.\n\nstart_date\x18\x10 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_date\x18\x15 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x19\n\x11\x66ilter_by_weekday\x18\x16 \x03(\r\x12?\n\x0e\x66ilter_by_time\x18\x17 \x01(\x0b\x32\'.admobilize.query.v1alpha1.FilterByTime\x12\x0e\n\x06status\x18\x11 \x01(\t\x12\r\n\x05table\x18\x12 \x01(\t\x12\x10\n\x08timezone\x18\x13 \x01(\t\x12\x0c\n\x04type\x18\x14 \x01(\t\"*\n\x0c\x46ilterByTime\x12\r\n\x05start\x18\x01 \x01(\t\x12\x0b\n\x03\x65nd\x18\x02 \x01(\t\")\n\x08\x46ilterBy\x12\x0e\n\x06\x63olumn\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"(\n\x0c\x43MSDimension\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\n\n\x02\x61s\x18\x02 \x01(\t\"~\n\rCMSDescriptor\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\x15\n\rplaylog_table\x18\x03 \x01(\t\x12\x39\n\x07\x63olumns\x18\x04 \x01(\x0b\x32(.admobilize.query.v1alpha1.CMSColumnsMap\"V\n\rCMSColumnsMap\x12\x13\n\x0b\x61\x64vertisers\x18\x01 \x01(\t\x12\r\n\x05sites\x18\x02 \x01(\t\x12\x0e\n\x06medias\x18\x03 \x01(\t\x12\x11\n\ttimestamp\x18\x04 \x01(\tB\x93\x01\n\x1d\x63om.admobilize.query.v1alpha1B\nQueryProtoP\x01Z@bitbucket.org/admobilize/admobilizeapis-go/pkg/queryapi/v1alpha1\xa2\x02\x05\x41\x44MQY\xaa\x02\x19\x41\x64Mobilize.Query.V1Alpha1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)admobilize/query/v1alpha1/resources.proto\x12\x19\x61\x64mobilize.query.v1alpha1\x1a\x1cgoogle/api/annotations.proto\x1a google/protobuf/field_mask.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1cgoogle/protobuf/struct.proto\"B\n\x07Project\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\x12\n\ncreated_at\x18\x02 \x01(\t\x12\x12\n\nupdated_at\x18\x03 \x01(\t\"2\n\x0bHeatmapData\x12\t\n\x01x\x18\x01 \x01(\r\x12\t\n\x01y\x18\x02 \x01(\r\x12\r\n\x05value\x18\x03 \x01(\x02\"?\n\x07Heatmap\x12\x34\n\x04\x64\x61ta\x18\x01 \x03(\x0b\x32&.admobilize.query.v1alpha1.HeatmapData\"\x80\x01\n\x06Metric\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05\x66ield\x18\x02 \x01(\t\x12\x11\n\toperation\x18\x03 \x01(\t\x12\x0e\n\x06\x66ilter\x18\x04 \x03(\t\x12\r\n\x05order\x18\x05 \x01(\t\x12\x19\n\x11\x63onversion_factor\x18\x06 \x01(\x01\x12\x0c\n\x04\x63\x61st\x18\x07 \x01(\t\"@\n\x0f\x41ggregateResult\x12\x0e\n\x06metric\x18\x01 \x01(\t\x12\x11\n\toperation\x18\x02 \x01(\t\x12\n\n\x02\x61s\x18\x03 \x01(\t\"\xbb\x01\n\x0fQueryFromResult\x12\x0e\n\x06select\x18\x01 \x03(\t\x12\x0b\n\x03sum\x18\x02 \x03(\t\x12\x0b\n\x03\x61vg\x18\x03 \x03(\t\x12\x0f\n\x07groupBy\x18\x04 \x03(\t\x12\x43\n\x07orderBy\x18\x05 \x03(\x0b\x32\x32.admobilize.query.v1alpha1.QueryFromResult.OrderBy\x1a(\n\x07OrderBy\x12\x0e\n\x06\x63olumn\x18\x01 \x01(\t\x12\r\n\x05order\x18\x02 \x01(\t\"4\n\rEncoderParams\x12\x0f\n\x07metrics\x18\x01 \x03(\t\x12\x12\n\ndimensions\x18\x02 \x03(\t\"?\n\x07\x44\x61taset\x12\r\n\x05label\x18\x01 \x01(\t\x12%\n\x05value\x18\x02 \x01(\x0b\x32\x16.google.protobuf.Value\")\n\x0bSchemaField\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\"\x80\x01\n\nClassifier\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\toperation\x18\x02 \x01(\t\x12\r\n\x05\x66ield\x18\x03 \x01(\t\x12\x42\n\nconditions\x18\x04 \x03(\x0b\x32..admobilize.query.v1alpha1.ClassifierCondition\"+\n\nOrderField\x12\x0e\n\x06\x63olumn\x18\x01 \x01(\t\x12\r\n\x05order\x18\x02 \x01(\t\"M\n\x13\x43lassifierCondition\x12\x0c\n\x04when\x18\x01 \x01(\t\x12\r\n\x05start\x18\x02 \x01(\x02\x12\x0b\n\x03\x65nd\x18\x03 \x01(\x02\x12\x0c\n\x04then\x18\x04 \x01(\t\"5\n\x06Status\x12\x13\n\x0bstatus_code\x18\x01 \x01(\t\x12\x16\n\x0estatus_message\x18\x02 \x01(\t\"3\n\tDeviceMap\x12\x11\n\tdevice_id\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65vice_name\x18\x02 \x01(\t\"\xc0\x01\n\x03Job\x12\x0e\n\x06job_id\x18\x01 \x01(\t\x12\x35\n\x06status\x18\x02 \x01(\x0e\x32%.admobilize.query.v1alpha1.Job.Status\x12\x0e\n\x06\x64\x65tail\x18\x03 \x01(\t\x12\x16\n\x0estatus_message\x18\x04 \x01(\t\x12\x11\n\tself_link\x18\x05 \x01(\t\"7\n\x06Status\x12\x0b\n\x07PENDING\x10\x00\x12\x0b\n\x07RUNNING\x10\x01\x12\x08\n\x04\x44ONE\x10\x03\x12\t\n\x05\x45RROR\x10\x04\"\xc9\x04\n\x06Report\x12\n\n\x02id\x18\x01 \x01(\t\x12\x13\n\x0b\x61\x64vertisers\x18\x02 \x03(\t\x12.\n\ncreated_on\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x14\n\x0c\x64\x61ys_to_send\x18\x04 \x03(\t\x12\x12\n\ndevice_ids\x18\x05 \x03(\t\x12\r\n\x05\x65mail\x18\x06 \x03(\t\x12\x0e\n\x06\x66ields\x18\x07 \x03(\t\x12\x0e\n\x06\x66ormat\x18\x08 \x01(\t\x12\x11\n\tfrequency\x18\t \x01(\t\x12\x10\n\x08interval\x18\n \x01(\t\x12-\n\tlast_sent\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x17\n\x0flast_report_url\x18\x0c \x01(\t\x12\r\n\x05media\x18\r \x03(\t\x12\x0c\n\x04name\x18\x0e \x01(\t\x12\x12\n\nproject_id\x18\x0f \x01(\t\x12.\n\nstart_date\x18\x10 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_date\x18\x15 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x19\n\x11\x66ilter_by_weekday\x18\x16 \x03(\r\x12?\n\x0e\x66ilter_by_time\x18\x17 \x01(\x0b\x32\'.admobilize.query.v1alpha1.FilterByTime\x12\x0e\n\x06status\x18\x11 \x01(\t\x12\r\n\x05table\x18\x12 \x01(\t\x12\x10\n\x08timezone\x18\x13 \x01(\t\x12\x0c\n\x04type\x18\x14 \x01(\t\"*\n\x0c\x46ilterByTime\x12\r\n\x05start\x18\x01 \x01(\t\x12\x0b\n\x03\x65nd\x18\x02 \x01(\t\")\n\x08\x46ilterBy\x12\x0e\n\x06\x63olumn\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"(\n\x0c\x43MSDimension\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\n\n\x02\x61s\x18\x02 \x01(\t\"~\n\rCMSDescriptor\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\x15\n\rplaylog_table\x18\x03 \x01(\t\x12\x39\n\x07\x63olumns\x18\x04 \x01(\x0b\x32(.admobilize.query.v1alpha1.CMSColumnsMap\"V\n\rCMSColumnsMap\x12\x13\n\x0b\x61\x64vertisers\x18\x01 \x01(\t\x12\r\n\x05sites\x18\x02 \x01(\t\x12\x0e\n\x06medias\x18\x03 \x01(\t\x12\x11\n\ttimestamp\x18\x04 \x01(\t\"P\n\tDashboard\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x35\n\x04rows\x18\x02 \x03(\x0b\x32\'.admobilize.query.v1alpha1.DashboardRow\"K\n\x0c\x44\x61shboardRow\x12;\n\x07widgets\x18\x01 \x03(\x0b\x32*.admobilize.query.v1alpha1.DashboardWidget\"*\n\x0f\x44\x61shboardWidget\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0b\n\x03url\x18\x02 \x01(\tB\x93\x01\n\x1d\x63om.admobilize.query.v1alpha1B\nQueryProtoP\x01Z@bitbucket.org/admobilize/admobilizeapis-go/pkg/queryapi/v1alpha1\xa2\x02\x05\x41\x44MQY\xaa\x02\x19\x41\x64Mobilize.Query.V1Alpha1b\x06proto3')
 
 
 
 _PROJECT = DESCRIPTOR.message_types_by_name['Project']
 _HEATMAPDATA = DESCRIPTOR.message_types_by_name['HeatmapData']
 _HEATMAP = DESCRIPTOR.message_types_by_name['Heatmap']
 _METRIC = DESCRIPTOR.message_types_by_name['Metric']
@@ -40,14 +40,17 @@
 _JOB = DESCRIPTOR.message_types_by_name['Job']
 _REPORT = DESCRIPTOR.message_types_by_name['Report']
 _FILTERBYTIME = DESCRIPTOR.message_types_by_name['FilterByTime']
 _FILTERBY = DESCRIPTOR.message_types_by_name['FilterBy']
 _CMSDIMENSION = DESCRIPTOR.message_types_by_name['CMSDimension']
 _CMSDESCRIPTOR = DESCRIPTOR.message_types_by_name['CMSDescriptor']
 _CMSCOLUMNSMAP = DESCRIPTOR.message_types_by_name['CMSColumnsMap']
+_DASHBOARD = DESCRIPTOR.message_types_by_name['Dashboard']
+_DASHBOARDROW = DESCRIPTOR.message_types_by_name['DashboardRow']
+_DASHBOARDWIDGET = DESCRIPTOR.message_types_by_name['DashboardWidget']
 _JOB_STATUS = _JOB.enum_types_by_name['Status']
 Project = _reflection.GeneratedProtocolMessageType('Project', (_message.Message,), {
   'DESCRIPTOR' : _PROJECT,
   '__module__' : 'admobilize.query.v1alpha1.resources_pb2'
   # @@protoc_insertion_point(class_scope:admobilize.query.v1alpha1.Project)
   })
 _sym_db.RegisterMessage(Project)
@@ -196,14 +199,35 @@
 CMSColumnsMap = _reflection.GeneratedProtocolMessageType('CMSColumnsMap', (_message.Message,), {
   'DESCRIPTOR' : _CMSCOLUMNSMAP,
   '__module__' : 'admobilize.query.v1alpha1.resources_pb2'
   # @@protoc_insertion_point(class_scope:admobilize.query.v1alpha1.CMSColumnsMap)
   })
 _sym_db.RegisterMessage(CMSColumnsMap)
 
+Dashboard = _reflection.GeneratedProtocolMessageType('Dashboard', (_message.Message,), {
+  'DESCRIPTOR' : _DASHBOARD,
+  '__module__' : 'admobilize.query.v1alpha1.resources_pb2'
+  # @@protoc_insertion_point(class_scope:admobilize.query.v1alpha1.Dashboard)
+  })
+_sym_db.RegisterMessage(Dashboard)
+
+DashboardRow = _reflection.GeneratedProtocolMessageType('DashboardRow', (_message.Message,), {
+  'DESCRIPTOR' : _DASHBOARDROW,
+  '__module__' : 'admobilize.query.v1alpha1.resources_pb2'
+  # @@protoc_insertion_point(class_scope:admobilize.query.v1alpha1.DashboardRow)
+  })
+_sym_db.RegisterMessage(DashboardRow)
+
+DashboardWidget = _reflection.GeneratedProtocolMessageType('DashboardWidget', (_message.Message,), {
+  'DESCRIPTOR' : _DASHBOARDWIDGET,
+  '__module__' : 'admobilize.query.v1alpha1.resources_pb2'
+  # @@protoc_insertion_point(class_scope:admobilize.query.v1alpha1.DashboardWidget)
+  })
+_sym_db.RegisterMessage(DashboardWidget)
+
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\035com.admobilize.query.v1alpha1B\nQueryProtoP\001Z@bitbucket.org/admobilize/admobilizeapis-go/pkg/queryapi/v1alpha1\242\002\005ADMQY\252\002\031AdMobilize.Query.V1Alpha1'
   _PROJECT._serialized_start=199
   _PROJECT._serialized_end=265
   _HEATMAPDATA._serialized_start=267
@@ -246,8 +270,14 @@
   _FILTERBY._serialized_end=2164
   _CMSDIMENSION._serialized_start=2166
   _CMSDIMENSION._serialized_end=2206
   _CMSDESCRIPTOR._serialized_start=2208
   _CMSDESCRIPTOR._serialized_end=2334
   _CMSCOLUMNSMAP._serialized_start=2336
   _CMSCOLUMNSMAP._serialized_end=2422
+  _DASHBOARD._serialized_start=2424
+  _DASHBOARD._serialized_end=2504
+  _DASHBOARDROW._serialized_start=2506
+  _DASHBOARDROW._serialized_end=2581
+  _DASHBOARDWIDGET._serialized_start=2583
+  _DASHBOARDWIDGET._serialized_end=2625
 # @@protoc_insertion_point(module_scope)
```

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/query/v1alpha1/query_service_pb2_grpc.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/query/v1alpha1/query_service_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
 from admobilize.proto.query.v1alpha1 import query_service_pb2 as admobilize_dot_query_dot_v1alpha1_dot_query__service__pb2
 from admobilize.proto.query.v1alpha1 import resources_pb2 as admobilize_dot_query_dot_v1alpha1_dot_resources__pb2
+from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 
 
 class QueryServiceStub(object):
     """Wrapper over BigQuery to abstract and isolate the infrastructure internal
     organization.
     """
 
@@ -33,14 +34,24 @@
                 response_deserializer=admobilize_dot_query_dot_v1alpha1_dot_query__service__pb2.ListTablesResponse.FromString,
                 )
         self.GetTableSchema = channel.unary_unary(
                 '/admobilize.query.v1alpha1.QueryService/GetTableSchema',
                 request_serializer=admobilize_dot_query_dot_v1alpha1_dot_query__service__pb2.GetTableSchemaRequest.SerializeToString,
                 response_deserializer=admobilize_dot_query_dot_v1alpha1_dot_query__service__pb2.GetTableSchemaResponse.FromString,
                 )
+        self.ListDashboards = channel.unary_unary(
+                '/admobilize.query.v1alpha1.QueryService/ListDashboards',
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                response_deserializer=admobilize_dot_query_dot_v1alpha1_dot_query__service__pb2.ListDashboardResponse.FromString,
+                )
+        self.GetDashboard = channel.unary_unary(
+                '/admobilize.query.v1alpha1.QueryService/GetDashboard',
+                request_serializer=admobilize_dot_query_dot_v1alpha1_dot_query__service__pb2.GetDashboardRequest.SerializeToString,
+                response_deserializer=admobilize_dot_query_dot_v1alpha1_dot_resources__pb2.Dashboard.FromString,
+                )
         self.GetReport = channel.unary_unary(
                 '/admobilize.query.v1alpha1.QueryService/GetReport',
                 request_serializer=admobilize_dot_query_dot_v1alpha1_dot_query__service__pb2.GetReportRequest.SerializeToString,
                 response_deserializer=admobilize_dot_query_dot_v1alpha1_dot_query__service__pb2.GetReportResponse.FromString,
                 )
         self.CreateReport = channel.unary_unary(
                 '/admobilize.query.v1alpha1.QueryService/CreateReport',
@@ -137,16 +148,31 @@
         """List table schema. <br/>
         Required permissions: `queryapi.datasets.getTableSchema`
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def ListDashboards(self, request, context):
+        """DASHBOARD API METHODS
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def GetDashboard(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def GetReport(self, request, context):
-        """Execute query and returns a report file. <br/>
+        """REPORTS API METHODS
+
+        Execute query and returns a report file. <br/>
         Required permissions: `queryapi.datasets.getTableReport`
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def CreateReport(self, request, context):
@@ -265,14 +291,24 @@
                     response_serializer=admobilize_dot_query_dot_v1alpha1_dot_query__service__pb2.ListTablesResponse.SerializeToString,
             ),
             'GetTableSchema': grpc.unary_unary_rpc_method_handler(
                     servicer.GetTableSchema,
                     request_deserializer=admobilize_dot_query_dot_v1alpha1_dot_query__service__pb2.GetTableSchemaRequest.FromString,
                     response_serializer=admobilize_dot_query_dot_v1alpha1_dot_query__service__pb2.GetTableSchemaResponse.SerializeToString,
             ),
+            'ListDashboards': grpc.unary_unary_rpc_method_handler(
+                    servicer.ListDashboards,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    response_serializer=admobilize_dot_query_dot_v1alpha1_dot_query__service__pb2.ListDashboardResponse.SerializeToString,
+            ),
+            'GetDashboard': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetDashboard,
+                    request_deserializer=admobilize_dot_query_dot_v1alpha1_dot_query__service__pb2.GetDashboardRequest.FromString,
+                    response_serializer=admobilize_dot_query_dot_v1alpha1_dot_resources__pb2.Dashboard.SerializeToString,
+            ),
             'GetReport': grpc.unary_unary_rpc_method_handler(
                     servicer.GetReport,
                     request_deserializer=admobilize_dot_query_dot_v1alpha1_dot_query__service__pb2.GetReportRequest.FromString,
                     response_serializer=admobilize_dot_query_dot_v1alpha1_dot_query__service__pb2.GetReportResponse.SerializeToString,
             ),
             'CreateReport': grpc.unary_unary_rpc_method_handler(
                     servicer.CreateReport,
@@ -411,14 +447,48 @@
         return grpc.experimental.unary_unary(request, target, '/admobilize.query.v1alpha1.QueryService/GetTableSchema',
             admobilize_dot_query_dot_v1alpha1_dot_query__service__pb2.GetTableSchemaRequest.SerializeToString,
             admobilize_dot_query_dot_v1alpha1_dot_query__service__pb2.GetTableSchemaResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def ListDashboards(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/admobilize.query.v1alpha1.QueryService/ListDashboards',
+            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            admobilize_dot_query_dot_v1alpha1_dot_query__service__pb2.ListDashboardResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetDashboard(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/admobilize.query.v1alpha1.QueryService/GetDashboard',
+            admobilize_dot_query_dot_v1alpha1_dot_query__service__pb2.GetDashboardRequest.SerializeToString,
+            admobilize_dot_query_dot_v1alpha1_dot_resources__pb2.Dashboard.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def GetReport(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/query/v1alpha1/query_service_pb2.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/query/v1alpha1/query_service_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,18 +12,19 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.protobuf import field_mask_pb2 as google_dot_protobuf_dot_field__mask__pb2
+from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from admobilize.proto.query.v1alpha1 import resources_pb2 as admobilize_dot_query_dot_v1alpha1_dot_resources__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n-admobilize/query/v1alpha1/query_service.proto\x12\x19\x61\x64mobilize.query.v1alpha1\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a google/protobuf/field_mask.proto\x1a)admobilize/query/v1alpha1/resources.proto\".\n\x1b\x43reateProjectDatasetRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\"\xdc\x07\n\x0cQueryRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\x32\n\x07metrics\x18\x03 \x03(\x0b\x32!.admobilize.query.v1alpha1.Metric\x12\x12\n\ndimensions\x18\x04 \x03(\t\x12\r\n\x05\x65poch\x18\x05 \x01(\t\x12\x16\n\x0ehas_comparison\x18\x06 \x01(\x08\x12\x44\n\x10\x61ggregate_result\x18\x0b \x01(\x0b\x32*.admobilize.query.v1alpha1.AggregateResult\x12\x45\n\x11query_from_result\x18( \x01(\x0b\x32*.admobilize.query.v1alpha1.QueryFromResult\x12:\n\x0b\x63lassifiers\x18\x0c \x03(\x0b\x32%.admobilize.query.v1alpha1.Classifier\x12\x0f\n\x07timeout\x18\t \x01(\r\x12\r\n\x05limit\x18\n \x01(\r\x12\x1a\n\x12\x64imensions_encoder\x18\r \x01(\x08\x12@\n\x0e\x65ncoder_params\x18* \x01(\x0b\x32(.admobilize.query.v1alpha1.EncoderParams\x12\x37\n\x08order_by\x18\x0f \x03(\x0b\x32%.admobilize.query.v1alpha1.OrderField\x12\x16\n\x0e\x66ilter_by_hour\x18\x10 \x03(\r\x12\x19\n\x11\x66ilter_by_weekday\x18\x11 \x03(\r\x12?\n\x0e\x66ilter_by_time\x18\x12 \x01(\x0b\x32\'.admobilize.query.v1alpha1.FilterByTime\x12\x36\n\x0b\x63ms_metrics\x18\x13 \x03(\x0b\x32!.admobilize.query.v1alpha1.Metric\x12>\n\rcms_dimension\x18\x14 \x01(\x0b\x32\'.admobilize.query.v1alpha1.CMSDimension\x12@\n\x0e\x63ms_descriptor\x18\x1e \x01(\x0b\x32(.admobilize.query.v1alpha1.CMSDescriptor\x12.\n\nstart_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08timezone\x18\x0e \x01(\t\x12\x0c\n\x03wid\x18\xe6\x07 \x01(\t\x12\x11\n\x08previous\x18\xe7\x07 \x01(\x08\"R\n\rQueryResponse\x12\x34\n\x08\x64\x61tasets\x18\x01 \x03(\x0b\x32\".admobilize.query.v1alpha1.Dataset\x12\x0b\n\x03tid\x18\x02 \x01(\t\"$\n\x11ListTablesRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\"$\n\x12ListTablesResponse\x12\x0e\n\x06tables\x18\x01 \x03(\t\"7\n\x15GetTableSchemaRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\"\x91\x01\n\x16GetTableSchemaResponse\x12\x36\n\x06schema\x18\x01 \x03(\x0b\x32&.admobilize.query.v1alpha1.SchemaField\x12\x10\n\x08num_rows\x18\x02 \x01(\x04\x12\x11\n\tnum_bytes\x18\x03 \x01(\x03\x12\x1a\n\x12last_modified_time\x18\x04 \x01(\x06\"\xba\x03\n\x10GetReportRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\r\n\x05\x65poch\x18\x03 \x01(\t\x12\x10\n\x08timezone\x18\t \x01(\t\x12\r\n\x05\x65mail\x18\x04 \x01(\t\x12\x0c\n\x04type\x18\x05 \x01(\t\x12\x0e\n\x06\x66ormat\x18\n \x01(\t\x12\x12\n\nspeed_unit\x18\x0b \x01(\t\x12\x19\n\x11\x66ilter_by_weekday\x18\x0c \x03(\r\x12?\n\x0e\x66ilter_by_time\x18\r \x01(\x0b\x32\'.admobilize.query.v1alpha1.FilterByTime\x12\x0e\n\x06\x66ields\x18\x0e \x03(\t\x12.\n\nstart_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x35\n\x07\x64\x65vices\x18\x08 \x03(\x0b\x32$.admobilize.query.v1alpha1.DeviceMap\x12\x13\n\x0b\x61\x64vertisers\x18\x0f \x03(\t\x12\x0e\n\x06medias\x18\x10 \x03(\t\"Z\n\x11GetReportResponse\x12\x31\n\x06status\x18\x01 \x01(\x0b\x32!.admobilize.query.v1alpha1.Status\x12\x12\n\nreport_url\x18\x02 \x01(\t\"\xdf\x01\n\x10\x43reateJobRequest\x12.\n\nstart_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\nproject_id\x18\x03 \x01(\t\x12\x12\n\nproduct_id\x18\x04 \x01(\t\x12\x10\n\x08timezone\x18\x07 \x01(\t\x12\x12\n\nspeed_unit\x18\x08 \x01(\t\x12\x12\n\ndevice_ids\x18\x05 \x03(\t\x12\x0b\n\x03\x63ms\x18\x06 \x01(\t\"G\n\rGetJobRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12*\n\x06\x66ields\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.FieldMask\"I\n\x14GetJobResultRequests\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x12\n\npage_token\x18\x03 \x01(\t\"2\n\x14\x45xportResultsRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0e\n\x06\x66ormat\x18\x02 \x01(\t\"j\n\x15GetDatapointsResponse\x12\x0e\n\x06job_id\x18\x01 \x01(\t\x12\x14\n\x0cjob_complete\x18\x02 \x01(\x08\x12\x17\n\x0fnext_page_token\x18\x03 \x01(\t\x12\x12\n\ndatapoints\x18\x04 \x01(\t\"K\n\x15\x45xportResultsResponse\x12\x0e\n\x06job_id\x18\x01 \x01(\t\x12\x14\n\x0cjob_complete\x18\x02 \x01(\x08\x12\x0c\n\x04urls\x18\x03 \x03(\t\"\xca\x03\n\x13GetTableDataRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\x0e\n\x06layout\x18\x03 \x01(\t\x12\x13\n\x0bmax_results\x18\x04 \x01(\r\x12\x12\n\npage_token\x18\x05 \x01(\t\x12\r\n\x05\x65poch\x18\x06 \x01(\t\x12\x35\n\x07\x64\x65vices\x18\x07 \x03(\x0b\x32$.admobilize.query.v1alpha1.DeviceMap\x12\x19\n\x11\x66ilter_by_weekday\x18\x08 \x03(\r\x12?\n\x0e\x66ilter_by_time\x18\t \x01(\x0b\x32\'.admobilize.query.v1alpha1.FilterByTime\x12\x10\n\x08group_by\x18\n \x03(\t\x12\x36\n\tfilter_by\x18\x0b \x01(\x0b\x32#.admobilize.query.v1alpha1.FilterBy\x12.\n\nstart_time\x18\x61 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x62 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08timezone\x18\x63 \x01(\t\"T\n\x14GetTableDataResponse\x12\x12\n\npage_token\x18\x02 \x01(\t\x12(\n\x04rows\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.ListValue\"4\n\x12ListReportsRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\"I\n\x13ListReportsResponse\x12\x32\n\x07reports\x18\x01 \x03(\x0b\x32!.admobilize.query.v1alpha1.Report\"\xb3\x03\n\x13\x43reateReportRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\x10\n\x08interval\x18\x03 \x01(\t\x12\x10\n\x08timezone\x18\t \x01(\t\x12\r\n\x05\x65mail\x18\x04 \x01(\t\x12\x0c\n\x04type\x18\x05 \x01(\t\x12\x0e\n\x06\x66ormat\x18\n \x01(\t\x12\x12\n\nspeed_unit\x18\x0b \x01(\t\x12\x11\n\tfrequency\x18\x0c \x01(\t\x12\x14\n\x0c\x64\x61ys_to_send\x18\r \x03(\t\x12\x19\n\x11\x66ilter_by_weekday\x18\x0e \x03(\r\x12?\n\x0e\x66ilter_by_time\x18\x0f \x01(\x0b\x32\'.admobilize.query.v1alpha1.FilterByTime\x12.\n\nstart_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07\x64\x65vices\x18\x08 \x03(\t\x12\x13\n\x0b\x61\x64vertisers\x18\x10 \x03(\t\x12\x0e\n\x06medias\x18\x11 \x03(\t\"\xdc\x02\n\x13UpdateReportRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\x0e\n\x06report\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x0c \x01(\t\x12\x10\n\x08interval\x18\x03 \x01(\t\x12\x10\n\x08timezone\x18\x04 \x01(\t\x12\r\n\x05\x65mail\x18\x05 \x03(\t\x12\x0c\n\x04type\x18\x06 \x01(\t\x12\x0e\n\x06\x66ormat\x18\x07 \x01(\t\x12\x12\n\nspeed_unit\x18\x08 \x01(\t\x12\x11\n\tfrequency\x18\t \x01(\t\x12\x14\n\x0c\x64\x61ys_to_send\x18\n \x03(\t\x12\x19\n\x11\x66ilter_by_weekday\x18\r \x03(\r\x12?\n\x0e\x66ilter_by_time\x18\x0e \x01(\x0b\x32\'.admobilize.query.v1alpha1.FilterByTime\x12,\n\x08\x65nd_time\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"D\n\x12PauseReportRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\x0e\n\x06report\x18\x03 \x01(\t\"F\n\x14RestartReportRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\x0e\n\x06report\x18\x03 \x01(\t\"E\n\x13\x43\x61ncelReportRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\x0e\n\x06report\x18\x03 \x01(\t\"\x97\x01\n\x17GetDeviceHeatmapRequest\x12\x0e\n\x06\x64\x65vice\x18\x01 \x01(\t\x12.\n\nstart_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06\x66ilter\x18\x04 \x01(\t2\xb3\x15\n\x0cQueryService\x12\x91\x01\n\x14\x43reateProjectDataset\x12\x36.admobilize.query.v1alpha1.CreateProjectDatasetRequest\x1a\".admobilize.query.v1alpha1.Project\"\x1d\x82\xd3\xe4\x93\x02\x17\"\x12/v1alpha1/projects:\x01*\x12\x9c\x01\n\x05Query\x12\'.admobilize.query.v1alpha1.QueryRequest\x1a(.admobilize.query.v1alpha1.QueryResponse\"@\x82\xd3\xe4\x93\x02:\"5/v1alpha1/projects/{project=*}/tables/{table=*}/query:\x01*\x12\x98\x01\n\nListTables\x12,.admobilize.query.v1alpha1.ListTablesRequest\x1a-.admobilize.query.v1alpha1.ListTablesResponse\"-\x82\xd3\xe4\x93\x02\'\x12%/v1alpha1/projects/{project=*}/tables\x12\xae\x01\n\x0eGetTableSchema\x12\x30.admobilize.query.v1alpha1.GetTableSchemaRequest\x1a\x31.admobilize.query.v1alpha1.GetTableSchemaResponse\"7\x82\xd3\xe4\x93\x02\x31\x12//v1alpha1/projects/{project=*}/tables/{table=*}\x12\xa9\x01\n\tGetReport\x12+.admobilize.query.v1alpha1.GetReportRequest\x1a,.admobilize.query.v1alpha1.GetReportResponse\"A\x82\xd3\xe4\x93\x02;\"6/v1alpha1/projects/{project=*}/tables/{table=*}/report:\x01*\x12\xa5\x01\n\x0c\x43reateReport\x12..admobilize.query.v1alpha1.CreateReportRequest\x1a!.admobilize.query.v1alpha1.Report\"B\x82\xd3\xe4\x93\x02<\"7/v1alpha1/projects/{project=*}/tables/{table=*}/reports:\x01*\x12\x9f\x01\n\x0cUpdateReport\x12..admobilize.query.v1alpha1.UpdateReportRequest\x1a!.admobilize.query.v1alpha1.Report\"<\x82\xd3\xe4\x93\x02\x36\x1a\x31/v1alpha1/projects/{project=*}/reports/{report=*}:\x01*\x12\x9c\x01\n\x0bListReports\x12-.admobilize.query.v1alpha1.ListReportsRequest\x1a..admobilize.query.v1alpha1.ListReportsResponse\".\x82\xd3\xe4\x93\x02(\x12&/v1alpha1/projects/{project=*}/reports\x12\xb4\x01\n\x0bPauseReport\x12-.admobilize.query.v1alpha1.PauseReportRequest\x1a!.admobilize.query.v1alpha1.Report\"S\x82\xd3\xe4\x93\x02M\"H/v1alpha1/projects/{project=*}/tables/{table=*}/reports/{report=*}:pause:\x01*\x12\xba\x01\n\rRestartReport\x12/.admobilize.query.v1alpha1.RestartReportRequest\x1a!.admobilize.query.v1alpha1.Report\"U\x82\xd3\xe4\x93\x02O\"J/v1alpha1/projects/{project=*}/tables/{table=*}/reports/{report=*}:restart:\x01*\x12\xb0\x01\n\x0c\x43\x61ncelReport\x12..admobilize.query.v1alpha1.CancelReportRequest\x1a!.admobilize.query.v1alpha1.Report\"M\x82\xd3\xe4\x93\x02G*B/v1alpha1/projects/{project=*}/tables/{table=*}/reports/{report=*}:\x01*\x12\xb0\x01\n\x0cGetTableData\x12..admobilize.query.v1alpha1.GetTableDataRequest\x1a/.admobilize.query.v1alpha1.GetTableDataResponse\"?\x82\xd3\xe4\x93\x02\x39\"4/v1alpha1/projects/{project=*}/tables/{table=*}/data:\x01*\x12\x98\x01\n\x10GetDeviceHeatmap\x12\x32.admobilize.query.v1alpha1.GetDeviceHeatmapRequest\x1a\".admobilize.query.v1alpha1.Heatmap\",\x82\xd3\xe4\x93\x02&\x12$/vialpha1/devices/{device=*}/heatmap\x12p\n\tCreateJob\x12+.admobilize.query.v1alpha1.CreateJobRequest\x1a\x1e.admobilize.query.v1alpha1.Job\"\x16\x82\xd3\xe4\x93\x02\x10\"\x0e/v1alpha1/jobs\x12q\n\x06GetJob\x12(.admobilize.query.v1alpha1.GetJobRequest\x1a\x1e.admobilize.query.v1alpha1.Job\"\x1d\x82\xd3\xe4\x93\x02\x17\x12\x15/v1alpha1/{id=jobs/*}\x12\x99\x01\n\rGetJobResults\x12/.admobilize.query.v1alpha1.GetJobResultRequests\x1a\x30.admobilize.query.v1alpha1.GetDatapointsResponse\"%\x82\xd3\xe4\x93\x02\x1f\x12\x1d/v1alpha1/{id=jobs/*}/results\x12\x98\x01\n\rExportResults\x12/.admobilize.query.v1alpha1.ExportResultsRequest\x1a\x30.admobilize.query.v1alpha1.ExportResultsResponse\"$\x82\xd3\xe4\x93\x02\x1e\x12\x1c/v1alpha1/{id=jobs/*}/exportB\x9c\x01\n\x1d\x63om.admobilize.query.v1alpha1B\x13QueryResourcesProtoP\x01Z@bitbucket.org/admobilize/admobilizeapis-go/pkg/queryapi/v1alpha1\xa2\x02\x05\x41\x44MQY\xaa\x02\x19\x41\x64Mobilize.Query.V1Alpha1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n-admobilize/query/v1alpha1/query_service.proto\x12\x19\x61\x64mobilize.query.v1alpha1\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a google/protobuf/field_mask.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a)admobilize/query/v1alpha1/resources.proto\".\n\x1b\x43reateProjectDatasetRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\"\xdc\x07\n\x0cQueryRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\x32\n\x07metrics\x18\x03 \x03(\x0b\x32!.admobilize.query.v1alpha1.Metric\x12\x12\n\ndimensions\x18\x04 \x03(\t\x12\r\n\x05\x65poch\x18\x05 \x01(\t\x12\x16\n\x0ehas_comparison\x18\x06 \x01(\x08\x12\x44\n\x10\x61ggregate_result\x18\x0b \x01(\x0b\x32*.admobilize.query.v1alpha1.AggregateResult\x12\x45\n\x11query_from_result\x18( \x01(\x0b\x32*.admobilize.query.v1alpha1.QueryFromResult\x12:\n\x0b\x63lassifiers\x18\x0c \x03(\x0b\x32%.admobilize.query.v1alpha1.Classifier\x12\x0f\n\x07timeout\x18\t \x01(\r\x12\r\n\x05limit\x18\n \x01(\r\x12\x1a\n\x12\x64imensions_encoder\x18\r \x01(\x08\x12@\n\x0e\x65ncoder_params\x18* \x01(\x0b\x32(.admobilize.query.v1alpha1.EncoderParams\x12\x37\n\x08order_by\x18\x0f \x03(\x0b\x32%.admobilize.query.v1alpha1.OrderField\x12\x16\n\x0e\x66ilter_by_hour\x18\x10 \x03(\r\x12\x19\n\x11\x66ilter_by_weekday\x18\x11 \x03(\r\x12?\n\x0e\x66ilter_by_time\x18\x12 \x01(\x0b\x32\'.admobilize.query.v1alpha1.FilterByTime\x12\x36\n\x0b\x63ms_metrics\x18\x13 \x03(\x0b\x32!.admobilize.query.v1alpha1.Metric\x12>\n\rcms_dimension\x18\x14 \x01(\x0b\x32\'.admobilize.query.v1alpha1.CMSDimension\x12@\n\x0e\x63ms_descriptor\x18\x1e \x01(\x0b\x32(.admobilize.query.v1alpha1.CMSDescriptor\x12.\n\nstart_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08timezone\x18\x0e \x01(\t\x12\x0c\n\x03wid\x18\xe6\x07 \x01(\t\x12\x11\n\x08previous\x18\xe7\x07 \x01(\x08\"R\n\rQueryResponse\x12\x34\n\x08\x64\x61tasets\x18\x01 \x03(\x0b\x32\".admobilize.query.v1alpha1.Dataset\x12\x0b\n\x03tid\x18\x02 \x01(\t\"$\n\x11ListTablesRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\"$\n\x12ListTablesResponse\x12\x0e\n\x06tables\x18\x01 \x03(\t\"7\n\x15GetTableSchemaRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\"\x91\x01\n\x16GetTableSchemaResponse\x12\x36\n\x06schema\x18\x01 \x03(\x0b\x32&.admobilize.query.v1alpha1.SchemaField\x12\x10\n\x08num_rows\x18\x02 \x01(\x04\x12\x11\n\tnum_bytes\x18\x03 \x01(\x03\x12\x1a\n\x12last_modified_time\x18\x04 \x01(\x06\"\xba\x03\n\x10GetReportRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\r\n\x05\x65poch\x18\x03 \x01(\t\x12\x10\n\x08timezone\x18\t \x01(\t\x12\r\n\x05\x65mail\x18\x04 \x01(\t\x12\x0c\n\x04type\x18\x05 \x01(\t\x12\x0e\n\x06\x66ormat\x18\n \x01(\t\x12\x12\n\nspeed_unit\x18\x0b \x01(\t\x12\x19\n\x11\x66ilter_by_weekday\x18\x0c \x03(\r\x12?\n\x0e\x66ilter_by_time\x18\r \x01(\x0b\x32\'.admobilize.query.v1alpha1.FilterByTime\x12\x0e\n\x06\x66ields\x18\x0e \x03(\t\x12.\n\nstart_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x35\n\x07\x64\x65vices\x18\x08 \x03(\x0b\x32$.admobilize.query.v1alpha1.DeviceMap\x12\x13\n\x0b\x61\x64vertisers\x18\x0f \x03(\t\x12\x0e\n\x06medias\x18\x10 \x03(\t\"Z\n\x11GetReportResponse\x12\x31\n\x06status\x18\x01 \x01(\x0b\x32!.admobilize.query.v1alpha1.Status\x12\x12\n\nreport_url\x18\x02 \x01(\t\"\xdf\x01\n\x10\x43reateJobRequest\x12.\n\nstart_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\nproject_id\x18\x03 \x01(\t\x12\x12\n\nproduct_id\x18\x04 \x01(\t\x12\x10\n\x08timezone\x18\x07 \x01(\t\x12\x12\n\nspeed_unit\x18\x08 \x01(\t\x12\x12\n\ndevice_ids\x18\x05 \x03(\t\x12\x0b\n\x03\x63ms\x18\x06 \x01(\t\"G\n\rGetJobRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12*\n\x06\x66ields\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.FieldMask\"I\n\x14GetJobResultRequests\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x12\n\npage_token\x18\x03 \x01(\t\"2\n\x14\x45xportResultsRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0e\n\x06\x66ormat\x18\x02 \x01(\t\"j\n\x15GetDatapointsResponse\x12\x0e\n\x06job_id\x18\x01 \x01(\t\x12\x14\n\x0cjob_complete\x18\x02 \x01(\x08\x12\x17\n\x0fnext_page_token\x18\x03 \x01(\t\x12\x12\n\ndatapoints\x18\x04 \x01(\t\"K\n\x15\x45xportResultsResponse\x12\x0e\n\x06job_id\x18\x01 \x01(\t\x12\x14\n\x0cjob_complete\x18\x02 \x01(\x08\x12\x0c\n\x04urls\x18\x03 \x03(\t\"\xca\x03\n\x13GetTableDataRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\x0e\n\x06layout\x18\x03 \x01(\t\x12\x13\n\x0bmax_results\x18\x04 \x01(\r\x12\x12\n\npage_token\x18\x05 \x01(\t\x12\r\n\x05\x65poch\x18\x06 \x01(\t\x12\x35\n\x07\x64\x65vices\x18\x07 \x03(\x0b\x32$.admobilize.query.v1alpha1.DeviceMap\x12\x19\n\x11\x66ilter_by_weekday\x18\x08 \x03(\r\x12?\n\x0e\x66ilter_by_time\x18\t \x01(\x0b\x32\'.admobilize.query.v1alpha1.FilterByTime\x12\x10\n\x08group_by\x18\n \x03(\t\x12\x36\n\tfilter_by\x18\x0b \x01(\x0b\x32#.admobilize.query.v1alpha1.FilterBy\x12.\n\nstart_time\x18\x61 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x62 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08timezone\x18\x63 \x01(\t\"T\n\x14GetTableDataResponse\x12\x12\n\npage_token\x18\x02 \x01(\t\x12(\n\x04rows\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.ListValue\"4\n\x12ListReportsRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\"I\n\x13ListReportsResponse\x12\x32\n\x07reports\x18\x01 \x03(\x0b\x32!.admobilize.query.v1alpha1.Report\"\xb3\x03\n\x13\x43reateReportRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\x10\n\x08interval\x18\x03 \x01(\t\x12\x10\n\x08timezone\x18\t \x01(\t\x12\r\n\x05\x65mail\x18\x04 \x01(\t\x12\x0c\n\x04type\x18\x05 \x01(\t\x12\x0e\n\x06\x66ormat\x18\n \x01(\t\x12\x12\n\nspeed_unit\x18\x0b \x01(\t\x12\x11\n\tfrequency\x18\x0c \x01(\t\x12\x14\n\x0c\x64\x61ys_to_send\x18\r \x03(\t\x12\x19\n\x11\x66ilter_by_weekday\x18\x0e \x03(\r\x12?\n\x0e\x66ilter_by_time\x18\x0f \x01(\x0b\x32\'.admobilize.query.v1alpha1.FilterByTime\x12.\n\nstart_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07\x64\x65vices\x18\x08 \x03(\t\x12\x13\n\x0b\x61\x64vertisers\x18\x10 \x03(\t\x12\x0e\n\x06medias\x18\x11 \x03(\t\"\xdc\x02\n\x13UpdateReportRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\x0e\n\x06report\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x0c \x01(\t\x12\x10\n\x08interval\x18\x03 \x01(\t\x12\x10\n\x08timezone\x18\x04 \x01(\t\x12\r\n\x05\x65mail\x18\x05 \x03(\t\x12\x0c\n\x04type\x18\x06 \x01(\t\x12\x0e\n\x06\x66ormat\x18\x07 \x01(\t\x12\x12\n\nspeed_unit\x18\x08 \x01(\t\x12\x11\n\tfrequency\x18\t \x01(\t\x12\x14\n\x0c\x64\x61ys_to_send\x18\n \x03(\t\x12\x19\n\x11\x66ilter_by_weekday\x18\r \x03(\r\x12?\n\x0e\x66ilter_by_time\x18\x0e \x01(\x0b\x32\'.admobilize.query.v1alpha1.FilterByTime\x12,\n\x08\x65nd_time\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"D\n\x12PauseReportRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\x0e\n\x06report\x18\x03 \x01(\t\"F\n\x14RestartReportRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\x0e\n\x06report\x18\x03 \x01(\t\"E\n\x13\x43\x61ncelReportRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\x0e\n\x06report\x18\x03 \x01(\t\"\xb7\x01\n\x17GetDeviceHeatmapRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\x0e\n\x06\x64\x65vice\x18\x03 \x01(\t\x12.\n\nstart_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06\x66ilter\x18\x06 \x01(\t\"Q\n\x15ListDashboardResponse\x12\x38\n\ndashboards\x18\x01 \x03(\x0b\x32$.admobilize.query.v1alpha1.Dashboard\"(\n\x13GetDashboardRequest\x12\x11\n\tdashboard\x18\x01 \x01(\t2\xe6\x17\n\x0cQueryService\x12\x91\x01\n\x14\x43reateProjectDataset\x12\x36.admobilize.query.v1alpha1.CreateProjectDatasetRequest\x1a\".admobilize.query.v1alpha1.Project\"\x1d\x82\xd3\xe4\x93\x02\x17\"\x12/v1alpha1/projects:\x01*\x12\x9c\x01\n\x05Query\x12\'.admobilize.query.v1alpha1.QueryRequest\x1a(.admobilize.query.v1alpha1.QueryResponse\"@\x82\xd3\xe4\x93\x02:\"5/v1alpha1/projects/{project=*}/tables/{table=*}/query:\x01*\x12\x98\x01\n\nListTables\x12,.admobilize.query.v1alpha1.ListTablesRequest\x1a-.admobilize.query.v1alpha1.ListTablesResponse\"-\x82\xd3\xe4\x93\x02\'\x12%/v1alpha1/projects/{project=*}/tables\x12\xae\x01\n\x0eGetTableSchema\x12\x30.admobilize.query.v1alpha1.GetTableSchemaRequest\x1a\x31.admobilize.query.v1alpha1.GetTableSchemaResponse\"7\x82\xd3\xe4\x93\x02\x31\x12//v1alpha1/projects/{project=*}/tables/{table=*}\x12x\n\x0eListDashboards\x12\x16.google.protobuf.Empty\x1a\x30.admobilize.query.v1alpha1.ListDashboardResponse\"\x1c\x82\xd3\xe4\x93\x02\x16\x12\x14/v1alpha1/dashboards\x12\x90\x01\n\x0cGetDashboard\x12..admobilize.query.v1alpha1.GetDashboardRequest\x1a$.admobilize.query.v1alpha1.Dashboard\"*\x82\xd3\xe4\x93\x02$\x12\"/v1alpha1/dashboards/{dashboard=*}\x12\xa9\x01\n\tGetReport\x12+.admobilize.query.v1alpha1.GetReportRequest\x1a,.admobilize.query.v1alpha1.GetReportResponse\"A\x82\xd3\xe4\x93\x02;\"6/v1alpha1/projects/{project=*}/tables/{table=*}/report:\x01*\x12\xa5\x01\n\x0c\x43reateReport\x12..admobilize.query.v1alpha1.CreateReportRequest\x1a!.admobilize.query.v1alpha1.Report\"B\x82\xd3\xe4\x93\x02<\"7/v1alpha1/projects/{project=*}/tables/{table=*}/reports:\x01*\x12\x9f\x01\n\x0cUpdateReport\x12..admobilize.query.v1alpha1.UpdateReportRequest\x1a!.admobilize.query.v1alpha1.Report\"<\x82\xd3\xe4\x93\x02\x36\x1a\x31/v1alpha1/projects/{project=*}/reports/{report=*}:\x01*\x12\x9c\x01\n\x0bListReports\x12-.admobilize.query.v1alpha1.ListReportsRequest\x1a..admobilize.query.v1alpha1.ListReportsResponse\".\x82\xd3\xe4\x93\x02(\x12&/v1alpha1/projects/{project=*}/reports\x12\xb4\x01\n\x0bPauseReport\x12-.admobilize.query.v1alpha1.PauseReportRequest\x1a!.admobilize.query.v1alpha1.Report\"S\x82\xd3\xe4\x93\x02M\"H/v1alpha1/projects/{project=*}/tables/{table=*}/reports/{report=*}:pause:\x01*\x12\xba\x01\n\rRestartReport\x12/.admobilize.query.v1alpha1.RestartReportRequest\x1a!.admobilize.query.v1alpha1.Report\"U\x82\xd3\xe4\x93\x02O\"J/v1alpha1/projects/{project=*}/tables/{table=*}/reports/{report=*}:restart:\x01*\x12\xb0\x01\n\x0c\x43\x61ncelReport\x12..admobilize.query.v1alpha1.CancelReportRequest\x1a!.admobilize.query.v1alpha1.Report\"M\x82\xd3\xe4\x93\x02G*B/v1alpha1/projects/{project=*}/tables/{table=*}/reports/{report=*}:\x01*\x12\xb0\x01\n\x0cGetTableData\x12..admobilize.query.v1alpha1.GetTableDataRequest\x1a/.admobilize.query.v1alpha1.GetTableDataResponse\"?\x82\xd3\xe4\x93\x02\x39\"4/v1alpha1/projects/{project=*}/tables/{table=*}/data:\x01*\x12\xbe\x01\n\x10GetDeviceHeatmap\x12\x32.admobilize.query.v1alpha1.GetDeviceHeatmapRequest\x1a\".admobilize.query.v1alpha1.Heatmap\"R\x82\xd3\xe4\x93\x02L\x12Jv1alpha1/projects/{project=*}/tables/{table=*}/devices/{device=*}/heatmap}\x12p\n\tCreateJob\x12+.admobilize.query.v1alpha1.CreateJobRequest\x1a\x1e.admobilize.query.v1alpha1.Job\"\x16\x82\xd3\xe4\x93\x02\x10\"\x0e/v1alpha1/jobs\x12q\n\x06GetJob\x12(.admobilize.query.v1alpha1.GetJobRequest\x1a\x1e.admobilize.query.v1alpha1.Job\"\x1d\x82\xd3\xe4\x93\x02\x17\x12\x15/v1alpha1/{id=jobs/*}\x12\x99\x01\n\rGetJobResults\x12/.admobilize.query.v1alpha1.GetJobResultRequests\x1a\x30.admobilize.query.v1alpha1.GetDatapointsResponse\"%\x82\xd3\xe4\x93\x02\x1f\x12\x1d/v1alpha1/{id=jobs/*}/results\x12\x98\x01\n\rExportResults\x12/.admobilize.query.v1alpha1.ExportResultsRequest\x1a\x30.admobilize.query.v1alpha1.ExportResultsResponse\"$\x82\xd3\xe4\x93\x02\x1e\x12\x1c/v1alpha1/{id=jobs/*}/exportB\x9c\x01\n\x1d\x63om.admobilize.query.v1alpha1B\x13QueryResourcesProtoP\x01Z@bitbucket.org/admobilize/admobilizeapis-go/pkg/queryapi/v1alpha1\xa2\x02\x05\x41\x44MQY\xaa\x02\x19\x41\x64Mobilize.Query.V1Alpha1b\x06proto3')
 
 
 
 _CREATEPROJECTDATASETREQUEST = DESCRIPTOR.message_types_by_name['CreateProjectDatasetRequest']
 _QUERYREQUEST = DESCRIPTOR.message_types_by_name['QueryRequest']
 _QUERYRESPONSE = DESCRIPTOR.message_types_by_name['QueryResponse']
 _LISTTABLESREQUEST = DESCRIPTOR.message_types_by_name['ListTablesRequest']
@@ -44,14 +45,16 @@
 _LISTREPORTSRESPONSE = DESCRIPTOR.message_types_by_name['ListReportsResponse']
 _CREATEREPORTREQUEST = DESCRIPTOR.message_types_by_name['CreateReportRequest']
 _UPDATEREPORTREQUEST = DESCRIPTOR.message_types_by_name['UpdateReportRequest']
 _PAUSEREPORTREQUEST = DESCRIPTOR.message_types_by_name['PauseReportRequest']
 _RESTARTREPORTREQUEST = DESCRIPTOR.message_types_by_name['RestartReportRequest']
 _CANCELREPORTREQUEST = DESCRIPTOR.message_types_by_name['CancelReportRequest']
 _GETDEVICEHEATMAPREQUEST = DESCRIPTOR.message_types_by_name['GetDeviceHeatmapRequest']
+_LISTDASHBOARDRESPONSE = DESCRIPTOR.message_types_by_name['ListDashboardResponse']
+_GETDASHBOARDREQUEST = DESCRIPTOR.message_types_by_name['GetDashboardRequest']
 CreateProjectDatasetRequest = _reflection.GeneratedProtocolMessageType('CreateProjectDatasetRequest', (_message.Message,), {
   'DESCRIPTOR' : _CREATEPROJECTDATASETREQUEST,
   '__module__' : 'admobilize.query.v1alpha1.query_service_pb2'
   # @@protoc_insertion_point(class_scope:admobilize.query.v1alpha1.CreateProjectDatasetRequest)
   })
 _sym_db.RegisterMessage(CreateProjectDatasetRequest)
 
@@ -219,27 +222,45 @@
 GetDeviceHeatmapRequest = _reflection.GeneratedProtocolMessageType('GetDeviceHeatmapRequest', (_message.Message,), {
   'DESCRIPTOR' : _GETDEVICEHEATMAPREQUEST,
   '__module__' : 'admobilize.query.v1alpha1.query_service_pb2'
   # @@protoc_insertion_point(class_scope:admobilize.query.v1alpha1.GetDeviceHeatmapRequest)
   })
 _sym_db.RegisterMessage(GetDeviceHeatmapRequest)
 
+ListDashboardResponse = _reflection.GeneratedProtocolMessageType('ListDashboardResponse', (_message.Message,), {
+  'DESCRIPTOR' : _LISTDASHBOARDRESPONSE,
+  '__module__' : 'admobilize.query.v1alpha1.query_service_pb2'
+  # @@protoc_insertion_point(class_scope:admobilize.query.v1alpha1.ListDashboardResponse)
+  })
+_sym_db.RegisterMessage(ListDashboardResponse)
+
+GetDashboardRequest = _reflection.GeneratedProtocolMessageType('GetDashboardRequest', (_message.Message,), {
+  'DESCRIPTOR' : _GETDASHBOARDREQUEST,
+  '__module__' : 'admobilize.query.v1alpha1.query_service_pb2'
+  # @@protoc_insertion_point(class_scope:admobilize.query.v1alpha1.GetDashboardRequest)
+  })
+_sym_db.RegisterMessage(GetDashboardRequest)
+
 _QUERYSERVICE = DESCRIPTOR.services_by_name['QueryService']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\035com.admobilize.query.v1alpha1B\023QueryResourcesProtoP\001Z@bitbucket.org/admobilize/admobilizeapis-go/pkg/queryapi/v1alpha1\242\002\005ADMQY\252\002\031AdMobilize.Query.V1Alpha1'
   _QUERYSERVICE.methods_by_name['CreateProjectDataset']._options = None
   _QUERYSERVICE.methods_by_name['CreateProjectDataset']._serialized_options = b'\202\323\344\223\002\027\"\022/v1alpha1/projects:\001*'
   _QUERYSERVICE.methods_by_name['Query']._options = None
   _QUERYSERVICE.methods_by_name['Query']._serialized_options = b'\202\323\344\223\002:\"5/v1alpha1/projects/{project=*}/tables/{table=*}/query:\001*'
   _QUERYSERVICE.methods_by_name['ListTables']._options = None
   _QUERYSERVICE.methods_by_name['ListTables']._serialized_options = b'\202\323\344\223\002\'\022%/v1alpha1/projects/{project=*}/tables'
   _QUERYSERVICE.methods_by_name['GetTableSchema']._options = None
   _QUERYSERVICE.methods_by_name['GetTableSchema']._serialized_options = b'\202\323\344\223\0021\022//v1alpha1/projects/{project=*}/tables/{table=*}'
+  _QUERYSERVICE.methods_by_name['ListDashboards']._options = None
+  _QUERYSERVICE.methods_by_name['ListDashboards']._serialized_options = b'\202\323\344\223\002\026\022\024/v1alpha1/dashboards'
+  _QUERYSERVICE.methods_by_name['GetDashboard']._options = None
+  _QUERYSERVICE.methods_by_name['GetDashboard']._serialized_options = b'\202\323\344\223\002$\022\"/v1alpha1/dashboards/{dashboard=*}'
   _QUERYSERVICE.methods_by_name['GetReport']._options = None
   _QUERYSERVICE.methods_by_name['GetReport']._serialized_options = b'\202\323\344\223\002;\"6/v1alpha1/projects/{project=*}/tables/{table=*}/report:\001*'
   _QUERYSERVICE.methods_by_name['CreateReport']._options = None
   _QUERYSERVICE.methods_by_name['CreateReport']._serialized_options = b'\202\323\344\223\002<\"7/v1alpha1/projects/{project=*}/tables/{table=*}/reports:\001*'
   _QUERYSERVICE.methods_by_name['UpdateReport']._options = None
   _QUERYSERVICE.methods_by_name['UpdateReport']._serialized_options = b'\202\323\344\223\0026\0321/v1alpha1/projects/{project=*}/reports/{report=*}:\001*'
   _QUERYSERVICE.methods_by_name['ListReports']._options = None
@@ -249,69 +270,73 @@
   _QUERYSERVICE.methods_by_name['RestartReport']._options = None
   _QUERYSERVICE.methods_by_name['RestartReport']._serialized_options = b'\202\323\344\223\002O\"J/v1alpha1/projects/{project=*}/tables/{table=*}/reports/{report=*}:restart:\001*'
   _QUERYSERVICE.methods_by_name['CancelReport']._options = None
   _QUERYSERVICE.methods_by_name['CancelReport']._serialized_options = b'\202\323\344\223\002G*B/v1alpha1/projects/{project=*}/tables/{table=*}/reports/{report=*}:\001*'
   _QUERYSERVICE.methods_by_name['GetTableData']._options = None
   _QUERYSERVICE.methods_by_name['GetTableData']._serialized_options = b'\202\323\344\223\0029\"4/v1alpha1/projects/{project=*}/tables/{table=*}/data:\001*'
   _QUERYSERVICE.methods_by_name['GetDeviceHeatmap']._options = None
-  _QUERYSERVICE.methods_by_name['GetDeviceHeatmap']._serialized_options = b'\202\323\344\223\002&\022$/vialpha1/devices/{device=*}/heatmap'
+  _QUERYSERVICE.methods_by_name['GetDeviceHeatmap']._serialized_options = b'\202\323\344\223\002L\022Jv1alpha1/projects/{project=*}/tables/{table=*}/devices/{device=*}/heatmap}'
   _QUERYSERVICE.methods_by_name['CreateJob']._options = None
   _QUERYSERVICE.methods_by_name['CreateJob']._serialized_options = b'\202\323\344\223\002\020\"\016/v1alpha1/jobs'
   _QUERYSERVICE.methods_by_name['GetJob']._options = None
   _QUERYSERVICE.methods_by_name['GetJob']._serialized_options = b'\202\323\344\223\002\027\022\025/v1alpha1/{id=jobs/*}'
   _QUERYSERVICE.methods_by_name['GetJobResults']._options = None
   _QUERYSERVICE.methods_by_name['GetJobResults']._serialized_options = b'\202\323\344\223\002\037\022\035/v1alpha1/{id=jobs/*}/results'
   _QUERYSERVICE.methods_by_name['ExportResults']._options = None
   _QUERYSERVICE.methods_by_name['ExportResults']._serialized_options = b'\202\323\344\223\002\036\022\034/v1alpha1/{id=jobs/*}/export'
-  _CREATEPROJECTDATASETREQUEST._serialized_start=246
-  _CREATEPROJECTDATASETREQUEST._serialized_end=292
-  _QUERYREQUEST._serialized_start=295
-  _QUERYREQUEST._serialized_end=1283
-  _QUERYRESPONSE._serialized_start=1285
-  _QUERYRESPONSE._serialized_end=1367
-  _LISTTABLESREQUEST._serialized_start=1369
-  _LISTTABLESREQUEST._serialized_end=1405
-  _LISTTABLESRESPONSE._serialized_start=1407
-  _LISTTABLESRESPONSE._serialized_end=1443
-  _GETTABLESCHEMAREQUEST._serialized_start=1445
-  _GETTABLESCHEMAREQUEST._serialized_end=1500
-  _GETTABLESCHEMARESPONSE._serialized_start=1503
-  _GETTABLESCHEMARESPONSE._serialized_end=1648
-  _GETREPORTREQUEST._serialized_start=1651
-  _GETREPORTREQUEST._serialized_end=2093
-  _GETREPORTRESPONSE._serialized_start=2095
-  _GETREPORTRESPONSE._serialized_end=2185
-  _CREATEJOBREQUEST._serialized_start=2188
-  _CREATEJOBREQUEST._serialized_end=2411
-  _GETJOBREQUEST._serialized_start=2413
-  _GETJOBREQUEST._serialized_end=2484
-  _GETJOBRESULTREQUESTS._serialized_start=2486
-  _GETJOBRESULTREQUESTS._serialized_end=2559
-  _EXPORTRESULTSREQUEST._serialized_start=2561
-  _EXPORTRESULTSREQUEST._serialized_end=2611
-  _GETDATAPOINTSRESPONSE._serialized_start=2613
-  _GETDATAPOINTSRESPONSE._serialized_end=2719
-  _EXPORTRESULTSRESPONSE._serialized_start=2721
-  _EXPORTRESULTSRESPONSE._serialized_end=2796
-  _GETTABLEDATAREQUEST._serialized_start=2799
-  _GETTABLEDATAREQUEST._serialized_end=3257
-  _GETTABLEDATARESPONSE._serialized_start=3259
-  _GETTABLEDATARESPONSE._serialized_end=3343
-  _LISTREPORTSREQUEST._serialized_start=3345
-  _LISTREPORTSREQUEST._serialized_end=3397
-  _LISTREPORTSRESPONSE._serialized_start=3399
-  _LISTREPORTSRESPONSE._serialized_end=3472
-  _CREATEREPORTREQUEST._serialized_start=3475
-  _CREATEREPORTREQUEST._serialized_end=3910
-  _UPDATEREPORTREQUEST._serialized_start=3913
-  _UPDATEREPORTREQUEST._serialized_end=4261
-  _PAUSEREPORTREQUEST._serialized_start=4263
-  _PAUSEREPORTREQUEST._serialized_end=4331
-  _RESTARTREPORTREQUEST._serialized_start=4333
-  _RESTARTREPORTREQUEST._serialized_end=4403
-  _CANCELREPORTREQUEST._serialized_start=4405
-  _CANCELREPORTREQUEST._serialized_end=4474
-  _GETDEVICEHEATMAPREQUEST._serialized_start=4477
-  _GETDEVICEHEATMAPREQUEST._serialized_end=4628
-  _QUERYSERVICE._serialized_start=4631
-  _QUERYSERVICE._serialized_end=7370
+  _CREATEPROJECTDATASETREQUEST._serialized_start=275
+  _CREATEPROJECTDATASETREQUEST._serialized_end=321
+  _QUERYREQUEST._serialized_start=324
+  _QUERYREQUEST._serialized_end=1312
+  _QUERYRESPONSE._serialized_start=1314
+  _QUERYRESPONSE._serialized_end=1396
+  _LISTTABLESREQUEST._serialized_start=1398
+  _LISTTABLESREQUEST._serialized_end=1434
+  _LISTTABLESRESPONSE._serialized_start=1436
+  _LISTTABLESRESPONSE._serialized_end=1472
+  _GETTABLESCHEMAREQUEST._serialized_start=1474
+  _GETTABLESCHEMAREQUEST._serialized_end=1529
+  _GETTABLESCHEMARESPONSE._serialized_start=1532
+  _GETTABLESCHEMARESPONSE._serialized_end=1677
+  _GETREPORTREQUEST._serialized_start=1680
+  _GETREPORTREQUEST._serialized_end=2122
+  _GETREPORTRESPONSE._serialized_start=2124
+  _GETREPORTRESPONSE._serialized_end=2214
+  _CREATEJOBREQUEST._serialized_start=2217
+  _CREATEJOBREQUEST._serialized_end=2440
+  _GETJOBREQUEST._serialized_start=2442
+  _GETJOBREQUEST._serialized_end=2513
+  _GETJOBRESULTREQUESTS._serialized_start=2515
+  _GETJOBRESULTREQUESTS._serialized_end=2588
+  _EXPORTRESULTSREQUEST._serialized_start=2590
+  _EXPORTRESULTSREQUEST._serialized_end=2640
+  _GETDATAPOINTSRESPONSE._serialized_start=2642
+  _GETDATAPOINTSRESPONSE._serialized_end=2748
+  _EXPORTRESULTSRESPONSE._serialized_start=2750
+  _EXPORTRESULTSRESPONSE._serialized_end=2825
+  _GETTABLEDATAREQUEST._serialized_start=2828
+  _GETTABLEDATAREQUEST._serialized_end=3286
+  _GETTABLEDATARESPONSE._serialized_start=3288
+  _GETTABLEDATARESPONSE._serialized_end=3372
+  _LISTREPORTSREQUEST._serialized_start=3374
+  _LISTREPORTSREQUEST._serialized_end=3426
+  _LISTREPORTSRESPONSE._serialized_start=3428
+  _LISTREPORTSRESPONSE._serialized_end=3501
+  _CREATEREPORTREQUEST._serialized_start=3504
+  _CREATEREPORTREQUEST._serialized_end=3939
+  _UPDATEREPORTREQUEST._serialized_start=3942
+  _UPDATEREPORTREQUEST._serialized_end=4290
+  _PAUSEREPORTREQUEST._serialized_start=4292
+  _PAUSEREPORTREQUEST._serialized_end=4360
+  _RESTARTREPORTREQUEST._serialized_start=4362
+  _RESTARTREPORTREQUEST._serialized_end=4432
+  _CANCELREPORTREQUEST._serialized_start=4434
+  _CANCELREPORTREQUEST._serialized_end=4503
+  _GETDEVICEHEATMAPREQUEST._serialized_start=4506
+  _GETDEVICEHEATMAPREQUEST._serialized_end=4689
+  _LISTDASHBOARDRESPONSE._serialized_start=4691
+  _LISTDASHBOARDRESPONSE._serialized_end=4772
+  _GETDASHBOARDREQUEST._serialized_start=4774
+  _GETDASHBOARDREQUEST._serialized_end=4814
+  _QUERYSERVICE._serialized_start=4817
+  _QUERYSERVICE._serialized_end=7863
 # @@protoc_insertion_point(module_scope)
```

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/ayuda/v1alpha1/ayuda_service_pb2.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/ayuda/v1alpha1/ayuda_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/ayuda/v1alpha1/ayuda_service_pb2_grpc.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/ayuda/v1alpha1/ayuda_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/ayuda/v1alpha1/resources_pb2.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/ayuda/v1alpha1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/signagelive/v1alpha1/signagelive_service_pb2.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/signagelive/v1alpha1/signagelive_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/signagelive/v1alpha1/signagelive_service_pb2_grpc.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/signagelive/v1alpha1/signagelive_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/signagelive/v1alpha1/resources_pb2.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/signagelive/v1alpha1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/common/entity_pb2.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/common/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/common/admobilize_types_pb2.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/common/admobilize_types_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/common/job_pb2.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/common/job_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/billing/v1alpha1/billing_pb2.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/billing/v1alpha1/billing_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/brightauthor/v1alpha1/brightauthor_service_pb2_grpc.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/brightauthor/v1alpha1/brightauthor_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/brightauthor/v1alpha1/resources_pb2.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/brightauthor/v1alpha1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/brightauthor/v1alpha1/brightauthor_service_pb2.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/brightauthor/v1alpha1/brightauthor_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/cmsintegrations/v1/cmsintegrations_service_pb2_grpc.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/cmsintegrations/v1/cmsintegrations_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/cmsintegrations/v1/resources_pb2.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/cmsintegrations/v1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/cmsintegrations/v1/cmsintegrations_service_pb2.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/cmsintegrations/v1/cmsintegrations_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/broadsign/v1alpha1/broadsign_service_pb2_grpc.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/broadsign/v1alpha1/broadsign_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/broadsign/v1alpha1/resources_pb2.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/broadsign/v1alpha1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilize/proto/broadsign/v1alpha1/broadsign_service_pb2.py` & `admobilizeapis-2023.7.18.post1/admobilize/proto/broadsign/v1alpha1/broadsign_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/PKG-INFO` & `admobilizeapis-2023.7.18.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: admobilizeapis
-Version: 2023.7.10.post1
+Version: 2023.7.18.post1
 Summary: Protobufs used in AdMobilize Ecosystem
 Home-page: https://www.bitbucket.org/admobilize/admobilizeapis
 Author: AdMobilize Team
 Author-email: devel@admobilize.com
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `admobilizeapis-2023.7.10.post1/admobilizeapis.egg-info/SOURCES.txt` & `admobilizeapis-2023.7.18.post1/admobilizeapis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/admobilizeapis.egg-info/PKG-INFO` & `admobilizeapis-2023.7.18.post1/admobilizeapis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: admobilizeapis
-Version: 2023.7.10.post1
+Version: 2023.7.18.post1
 Summary: Protobufs used in AdMobilize Ecosystem
 Home-page: https://www.bitbucket.org/admobilize/admobilizeapis
 Author: AdMobilize Team
 Author-email: devel@admobilize.com
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `admobilizeapis-2023.7.10.post1/README.md` & `admobilizeapis-2023.7.18.post1/README.md`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.10.post1/setup.py` & `admobilizeapis-2023.7.18.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 install_requires = ["google-api-core >= 1.6.0, < 2.0.0dev", "protobuf >= 3.6.0, < 4.0"]
 
 extras_require = {"grpc": ["grpcio>=1.2.0"]}
 
 setup(
     name="admobilizeapis",
-    version='2023.07.10r1',
+    version='2023.07.18r1',
     author="AdMobilize Team",
     author_email="devel@admobilize.com",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Programming Language :: Python",
```

