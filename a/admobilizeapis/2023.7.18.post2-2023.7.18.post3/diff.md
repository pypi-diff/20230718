# Comparing `tmp/admobilizeapis-2023.7.18.post2.tar.gz` & `tmp/admobilizeapis-2023.7.18.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/admobilizeapis-2023.7.18.post2.tar", last modified: Tue Jul 18 04:27:55 2023, max compression
+gzip compressed data, was "dist/admobilizeapis-2023.7.18.post3.tar", last modified: Tue Jul 18 05:10:36 2023, max compression
```

## Comparing `admobilizeapis-2023.7.18.post2.tar` & `admobilizeapis-2023.7.18.post3.tar`

### file list

```diff
@@ -1,182 +1,182 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/
--rw-r--r--   0 root         (0) root         (0)       56 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/google/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/google/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/google/longrunning/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/google/longrunning/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8090 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/google/longrunning/operations_pb2.py
--rw-r--r--   0 root         (0) root         (0)    10932 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/google/longrunning/operations_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/wifi/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/wifi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/wifi/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/wifi/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/wifi/v1/wifi_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2457 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/wifi/v1/wifi_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/datagateway/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/datagateway/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/datagateway/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/datagateway/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8861 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/datagateway/v1alpha1/datagateway_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     8708 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/datagateway/v1alpha1/datagateway_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/iam/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/iam/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/iam/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/iam/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/iam/v1alpha1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    25837 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/iam/v1alpha1/iam_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4250 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/iam/v1alpha1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    35932 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/iam/v1alpha1/iam_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/notification/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/notification/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/notification/v1beta1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/notification/v1beta1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/notification/v1beta1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     6645 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/notification/v1beta1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    10396 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/notification/v1beta1/notification_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    14597 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/notification/v1beta1/notification_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/vision/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/vision/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/vision/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/vision/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/vision/v1/model_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2515 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/vision/v1/vision_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2912 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/vision/v1/vision_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/vision/v1/vision_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     4194 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/vision/v1/model_pb2.py
--rw-r--r--   0 root         (0) root         (0)    26810 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/vision/v1/vision_pb2.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/mlmodel/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/mlmodel/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/mlmodel/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)     6478 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/mlmodel/v1alpha1/mlmodel_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/mlmodel/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5542 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/mlmodel/v1alpha1/mlmodel_service_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/salestool/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/salestool/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/salestool/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/salestool/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4784 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/salestool/v1alpha1/salestool_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     5528 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/salestool/v1alpha1/salestool_service_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/devicemanagement/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/devicemanagement/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/devicemanagement/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/devicemanagement/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/devicemanagement/v1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    15461 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/devicemanagement/v1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    39106 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/devicemanagement/v1/device_manager_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    28693 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/devicemanagement/v1/device_manager_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/devicemanagement/v1alpha2/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/devicemanagement/v1alpha2/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/devicemanagement/v1alpha2/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    10609 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/devicemanagement/v1alpha2/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    28083 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/devicemanagement/v1alpha2/device_manager_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    18992 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/devicemanagement/v1alpha2/device_manager_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/devicemanagement/v2/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/devicemanagement/v2/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/devicemanagement/v2/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    20392 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/devicemanagement/v2/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    99455 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/devicemanagement/v2/device_manager_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    76701 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/devicemanagement/v2/device_manager_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/devicemanagement/v1alpha3/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/devicemanagement/v1alpha3/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/devicemanagement/v1alpha3/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    13543 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/devicemanagement/v1alpha3/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    41623 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/devicemanagement/v1alpha3/device_manager_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    29786 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/devicemanagement/v1alpha3/device_manager_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/devicemanagement/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/devicemanagement/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/devicemanagement/v1alpha1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     9576 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/devicemanagement/v1alpha1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    14877 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/devicemanagement/v1alpha1/device_manager_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    15271 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/devicemanagement/v1alpha1/device_manager_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/admprovider/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/admprovider/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/admprovider/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/admprovider/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/admprovider/v1alpha1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     6954 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/admprovider/v1alpha1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    22477 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/admprovider/v1alpha1/admprovider_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     8758 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/admprovider/v1alpha1/admprovider_service_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/malos/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/malos/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/malos/v1/
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/malos/v1/driver_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/malos/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4590 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/malos/v1/driver_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6136 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/malos/v1/maloseye_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/malos/v1/maloseye_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/query/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/query/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/query/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/query/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/query/v1alpha1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    17400 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/query/v1alpha1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    36631 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/query/v1alpha1/query_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    31806 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/query/v1alpha1/query_service_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/ayuda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/ayuda/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/ayuda/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/ayuda/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/ayuda/v1alpha1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    15801 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/ayuda/v1alpha1/ayuda_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    21203 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/ayuda/v1alpha1/ayuda_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3157 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/ayuda/v1alpha1/resources_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/signagelive/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/signagelive/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/signagelive/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/signagelive/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18378 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/signagelive/v1alpha1/signagelive_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/signagelive/v1alpha1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    24106 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/signagelive/v1alpha1/signagelive_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3240 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/signagelive/v1alpha1/resources_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/common/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/common/job_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/common/admobilize_types_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     4485 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/common/entity_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2623 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/common/admobilize_types_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2897 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/common/job_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/common/entity_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/billing/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/billing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/billing/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/billing/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2506 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/billing/v1alpha1/billing_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/billing/v1alpha1/billing_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/brightauthor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/brightauthor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/brightauthor/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)    22301 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/brightauthor/v1alpha1/brightauthor_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/brightauthor/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/brightauthor/v1alpha1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3246 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/brightauthor/v1alpha1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    16652 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/brightauthor/v1alpha1/brightauthor_service_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/cmsintegrations/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/cmsintegrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/cmsintegrations/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/cmsintegrations/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/cmsintegrations/v1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    29481 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/cmsintegrations/v1/cmsintegrations_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    10026 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/cmsintegrations/v1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    24348 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/cmsintegrations/v1/cmsintegrations_service_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/broadsign/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/broadsign/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/broadsign/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/broadsign/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21841 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/broadsign/v1alpha1/broadsign_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/broadsign/v1alpha1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3174 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/broadsign/v1alpha1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    16356 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilize/proto/broadsign/v1alpha1/broadsign_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)      849 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilizeapis.egg-info/
--rw-r--r--   0 root         (0) root         (0)       76 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilizeapis.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilizeapis.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)     6814 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilizeapis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      849 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilizeapis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilizeapis.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/admobilizeapis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1201 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/README.md
--rw-r--r--   0 root         (0) root         (0)     1293 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/setup.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 04:27:55.000000 admobilizeapis-2023.7.18.post2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/admobilize/
+-rw-r--r--   0 root         (0) root         (0)       56 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/admobilize/google/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/google/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/admobilize/google/longrunning/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/google/longrunning/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8090 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/google/longrunning/operations_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    10932 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/google/longrunning/operations_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/wifi/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/wifi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/wifi/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/wifi/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/wifi/v1/wifi_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2457 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/wifi/v1/wifi_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/datagateway/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/datagateway/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/datagateway/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/datagateway/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8861 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/datagateway/v1alpha1/datagateway_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     8708 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/datagateway/v1alpha1/datagateway_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/iam/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/iam/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/iam/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/iam/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/iam/v1alpha1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    25837 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/iam/v1alpha1/iam_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4250 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/iam/v1alpha1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    35932 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/iam/v1alpha1/iam_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/notification/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/notification/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/notification/v1beta1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/notification/v1beta1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/notification/v1beta1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     6645 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/notification/v1beta1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    10396 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/notification/v1beta1/notification_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    14597 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/notification/v1beta1/notification_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/vision/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/vision/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/vision/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/vision/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/vision/v1/model_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2515 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/vision/v1/vision_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2912 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/vision/v1/vision_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/vision/v1/vision_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     4194 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/vision/v1/model_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    26810 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/vision/v1/vision_pb2.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/mlmodel/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/mlmodel/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/mlmodel/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)     6478 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/mlmodel/v1alpha1/mlmodel_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/mlmodel/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5542 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/mlmodel/v1alpha1/mlmodel_service_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/salestool/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/salestool/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/salestool/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/salestool/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4784 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/salestool/v1alpha1/salestool_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     5528 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/salestool/v1alpha1/salestool_service_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/devicemanagement/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/devicemanagement/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/devicemanagement/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/devicemanagement/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/devicemanagement/v1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    15461 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/devicemanagement/v1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    39106 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/devicemanagement/v1/device_manager_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    28693 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/devicemanagement/v1/device_manager_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/devicemanagement/v1alpha2/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/devicemanagement/v1alpha2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/devicemanagement/v1alpha2/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    10609 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/devicemanagement/v1alpha2/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    28083 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/devicemanagement/v1alpha2/device_manager_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    18992 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/devicemanagement/v1alpha2/device_manager_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/devicemanagement/v2/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/devicemanagement/v2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/devicemanagement/v2/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    20392 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/devicemanagement/v2/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    99455 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/devicemanagement/v2/device_manager_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    76701 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/devicemanagement/v2/device_manager_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/devicemanagement/v1alpha3/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/devicemanagement/v1alpha3/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/devicemanagement/v1alpha3/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    13543 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/devicemanagement/v1alpha3/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    41623 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/devicemanagement/v1alpha3/device_manager_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    29786 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/devicemanagement/v1alpha3/device_manager_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/devicemanagement/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/devicemanagement/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/devicemanagement/v1alpha1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     9576 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/devicemanagement/v1alpha1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    14877 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/devicemanagement/v1alpha1/device_manager_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    15271 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/devicemanagement/v1alpha1/device_manager_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/admprovider/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/admprovider/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/admprovider/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/admprovider/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/admprovider/v1alpha1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     6954 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/admprovider/v1alpha1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    22477 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/admprovider/v1alpha1/admprovider_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     8758 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/admprovider/v1alpha1/admprovider_service_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/malos/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/malos/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/malos/v1/
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/malos/v1/driver_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/malos/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4590 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/malos/v1/driver_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6136 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/malos/v1/maloseye_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/malos/v1/maloseye_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/query/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/query/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/query/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/query/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/query/v1alpha1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    17400 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/query/v1alpha1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    35006 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/query/v1alpha1/query_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    31327 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/query/v1alpha1/query_service_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/ayuda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/ayuda/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/ayuda/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/ayuda/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/ayuda/v1alpha1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    15801 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/ayuda/v1alpha1/ayuda_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    21203 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/ayuda/v1alpha1/ayuda_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3157 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/ayuda/v1alpha1/resources_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/signagelive/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/signagelive/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/signagelive/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/signagelive/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18378 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/signagelive/v1alpha1/signagelive_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/signagelive/v1alpha1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    24106 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/signagelive/v1alpha1/signagelive_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3240 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/signagelive/v1alpha1/resources_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/common/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/common/job_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/common/admobilize_types_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     4485 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/common/entity_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2623 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/common/admobilize_types_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2897 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/common/job_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/common/entity_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/billing/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/billing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/billing/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/billing/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2506 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/billing/v1alpha1/billing_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/billing/v1alpha1/billing_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/brightauthor/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/brightauthor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/brightauthor/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)    22301 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/brightauthor/v1alpha1/brightauthor_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/brightauthor/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/brightauthor/v1alpha1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3246 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/brightauthor/v1alpha1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    16652 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/brightauthor/v1alpha1/brightauthor_service_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/cmsintegrations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/cmsintegrations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/cmsintegrations/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/cmsintegrations/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/cmsintegrations/v1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    29481 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/cmsintegrations/v1/cmsintegrations_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    10026 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/cmsintegrations/v1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    24348 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/cmsintegrations/v1/cmsintegrations_service_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/broadsign/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/broadsign/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/broadsign/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/broadsign/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21841 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/broadsign/v1alpha1/broadsign_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/broadsign/v1alpha1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3174 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/broadsign/v1alpha1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    16356 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/admobilize/proto/broadsign/v1alpha1/broadsign_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      849 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/admobilizeapis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       76 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/admobilizeapis.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/admobilizeapis.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)     6814 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/admobilizeapis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      849 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/admobilizeapis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/admobilizeapis.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/admobilizeapis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1201 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/README.md
+-rw-r--r--   0 root         (0) root         (0)     1293 2023-07-18 05:10:35.000000 admobilizeapis-2023.7.18.post3/setup.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 05:10:36.000000 admobilizeapis-2023.7.18.post3/setup.cfg
```

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/google/longrunning/operations_pb2.py` & `admobilizeapis-2023.7.18.post3/admobilize/google/longrunning/operations_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/google/longrunning/operations_pb2_grpc.py` & `admobilizeapis-2023.7.18.post3/admobilize/google/longrunning/operations_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/wifi/v1/wifi_pb2.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/wifi/v1/wifi_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/datagateway/v1alpha1/datagateway_service_pb2.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/datagateway/v1alpha1/datagateway_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/datagateway/v1alpha1/datagateway_service_pb2_grpc.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/datagateway/v1alpha1/datagateway_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/iam/v1alpha1/iam_service_pb2.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/iam/v1alpha1/iam_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/iam/v1alpha1/resources_pb2.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/iam/v1alpha1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/iam/v1alpha1/iam_service_pb2_grpc.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/iam/v1alpha1/iam_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/notification/v1beta1/resources_pb2.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/notification/v1beta1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/notification/v1beta1/notification_service_pb2.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/notification/v1beta1/notification_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/notification/v1beta1/notification_service_pb2_grpc.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/notification/v1beta1/notification_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/vision/v1/vision_service_pb2.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/vision/v1/vision_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/vision/v1/vision_service_pb2_grpc.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/vision/v1/vision_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/vision/v1/model_pb2.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/vision/v1/model_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/vision/v1/vision_pb2.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/vision/v1/vision_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/mlmodel/v1alpha1/mlmodel_service_pb2_grpc.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/mlmodel/v1alpha1/mlmodel_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/mlmodel/v1alpha1/mlmodel_service_pb2.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/mlmodel/v1alpha1/mlmodel_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/salestool/v1alpha1/salestool_service_pb2_grpc.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/salestool/v1alpha1/salestool_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/salestool/v1alpha1/salestool_service_pb2.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/salestool/v1alpha1/salestool_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/devicemanagement/v1/resources_pb2.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/devicemanagement/v1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/devicemanagement/v1/device_manager_pb2_grpc.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/devicemanagement/v1/device_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/devicemanagement/v1/device_manager_pb2.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/devicemanagement/v1/device_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/devicemanagement/v1alpha2/resources_pb2.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/devicemanagement/v1alpha2/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/devicemanagement/v1alpha2/device_manager_pb2_grpc.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/devicemanagement/v1alpha2/device_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/devicemanagement/v1alpha2/device_manager_pb2.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/devicemanagement/v1alpha2/device_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/devicemanagement/v2/resources_pb2.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/devicemanagement/v2/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/devicemanagement/v2/device_manager_pb2_grpc.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/devicemanagement/v2/device_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/devicemanagement/v2/device_manager_pb2.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/devicemanagement/v2/device_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/devicemanagement/v1alpha3/resources_pb2.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/devicemanagement/v1alpha3/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/devicemanagement/v1alpha3/device_manager_pb2_grpc.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/devicemanagement/v1alpha3/device_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/devicemanagement/v1alpha3/device_manager_pb2.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/devicemanagement/v1alpha3/device_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/devicemanagement/v1alpha1/resources_pb2.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/devicemanagement/v1alpha1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/devicemanagement/v1alpha1/device_manager_pb2_grpc.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/devicemanagement/v1alpha1/device_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/devicemanagement/v1alpha1/device_manager_pb2.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/devicemanagement/v1alpha1/device_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/admprovider/v1alpha1/resources_pb2.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/admprovider/v1alpha1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/admprovider/v1alpha1/admprovider_service_pb2_grpc.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/admprovider/v1alpha1/admprovider_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/admprovider/v1alpha1/admprovider_service_pb2.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/admprovider/v1alpha1/admprovider_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/malos/v1/driver_pb2.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/malos/v1/driver_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/malos/v1/maloseye_pb2.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/malos/v1/maloseye_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/query/v1alpha1/resources_pb2.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/query/v1alpha1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/query/v1alpha1/query_service_pb2_grpc.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/query/v1alpha1/query_service_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,19 +84,14 @@
                 response_deserializer=admobilize_dot_query_dot_v1alpha1_dot_resources__pb2.Report.FromString,
                 )
         self.GetTableData = channel.unary_unary(
                 '/admobilize.query.v1alpha1.QueryService/GetTableData',
                 request_serializer=admobilize_dot_query_dot_v1alpha1_dot_query__service__pb2.GetTableDataRequest.SerializeToString,
                 response_deserializer=admobilize_dot_query_dot_v1alpha1_dot_query__service__pb2.GetTableDataResponse.FromString,
                 )
-        self.GetDeviceHeatmap = channel.unary_unary(
-                '/admobilize.query.v1alpha1.QueryService/GetDeviceHeatmap',
-                request_serializer=admobilize_dot_query_dot_v1alpha1_dot_query__service__pb2.GetDeviceHeatmapRequest.SerializeToString,
-                response_deserializer=admobilize_dot_query_dot_v1alpha1_dot_resources__pb2.Heatmap.FromString,
-                )
         self.CreateJob = channel.unary_unary(
                 '/admobilize.query.v1alpha1.QueryService/CreateJob',
                 request_serializer=admobilize_dot_query_dot_v1alpha1_dot_query__service__pb2.CreateJobRequest.SerializeToString,
                 response_deserializer=admobilize_dot_query_dot_v1alpha1_dot_resources__pb2.Job.FromString,
                 )
         self.GetJob = channel.unary_unary(
                 '/admobilize.query.v1alpha1.QueryService/GetJob',
@@ -227,22 +222,22 @@
         """Get raw table data  <br/>
         Required permissions: `queryapi.datasets.getTableData`
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetDeviceHeatmap(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
     def CreateJob(self, request, context):
-        """
+        """rpc GetDeviceHeatmap(GetDeviceHeatmapRequest) returns (Heatmap) {
+        option (google.api.http) = {
+        get: "v1alpha1/projects/{project=*}/tables/{table=*}/devices/{device=*}/heatmap"
+        };
+        }
+
+
         DATA API METHODS
 
         Starts a job do retrieve user datapoints. <br/>
         Required permissions: `queryapi.jobs.create`
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
@@ -341,19 +336,14 @@
                     response_serializer=admobilize_dot_query_dot_v1alpha1_dot_resources__pb2.Report.SerializeToString,
             ),
             'GetTableData': grpc.unary_unary_rpc_method_handler(
                     servicer.GetTableData,
                     request_deserializer=admobilize_dot_query_dot_v1alpha1_dot_query__service__pb2.GetTableDataRequest.FromString,
                     response_serializer=admobilize_dot_query_dot_v1alpha1_dot_query__service__pb2.GetTableDataResponse.SerializeToString,
             ),
-            'GetDeviceHeatmap': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetDeviceHeatmap,
-                    request_deserializer=admobilize_dot_query_dot_v1alpha1_dot_query__service__pb2.GetDeviceHeatmapRequest.FromString,
-                    response_serializer=admobilize_dot_query_dot_v1alpha1_dot_resources__pb2.Heatmap.SerializeToString,
-            ),
             'CreateJob': grpc.unary_unary_rpc_method_handler(
                     servicer.CreateJob,
                     request_deserializer=admobilize_dot_query_dot_v1alpha1_dot_query__service__pb2.CreateJobRequest.FromString,
                     response_serializer=admobilize_dot_query_dot_v1alpha1_dot_resources__pb2.Job.SerializeToString,
             ),
             'GetJob': grpc.unary_unary_rpc_method_handler(
                     servicer.GetJob,
@@ -617,31 +607,14 @@
         return grpc.experimental.unary_unary(request, target, '/admobilize.query.v1alpha1.QueryService/GetTableData',
             admobilize_dot_query_dot_v1alpha1_dot_query__service__pb2.GetTableDataRequest.SerializeToString,
             admobilize_dot_query_dot_v1alpha1_dot_query__service__pb2.GetTableDataResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def GetDeviceHeatmap(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/admobilize.query.v1alpha1.QueryService/GetDeviceHeatmap',
-            admobilize_dot_query_dot_v1alpha1_dot_query__service__pb2.GetDeviceHeatmapRequest.SerializeToString,
-            admobilize_dot_query_dot_v1alpha1_dot_resources__pb2.Heatmap.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
     def CreateJob(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/query/v1alpha1/query_service_pb2.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/query/v1alpha1/query_service_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.protobuf import field_mask_pb2 as google_dot_protobuf_dot_field__mask__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from admobilize.proto.query.v1alpha1 import resources_pb2 as admobilize_dot_query_dot_v1alpha1_dot_resources__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n-admobilize/query/v1alpha1/query_service.proto\x12\x19\x61\x64mobilize.query.v1alpha1\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a google/protobuf/field_mask.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a)admobilize/query/v1alpha1/resources.proto\".\n\x1b\x43reateProjectDatasetRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\"\xdc\x07\n\x0cQueryRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\x32\n\x07metrics\x18\x03 \x03(\x0b\x32!.admobilize.query.v1alpha1.Metric\x12\x12\n\ndimensions\x18\x04 \x03(\t\x12\r\n\x05\x65poch\x18\x05 \x01(\t\x12\x16\n\x0ehas_comparison\x18\x06 \x01(\x08\x12\x44\n\x10\x61ggregate_result\x18\x0b \x01(\x0b\x32*.admobilize.query.v1alpha1.AggregateResult\x12\x45\n\x11query_from_result\x18( \x01(\x0b\x32*.admobilize.query.v1alpha1.QueryFromResult\x12:\n\x0b\x63lassifiers\x18\x0c \x03(\x0b\x32%.admobilize.query.v1alpha1.Classifier\x12\x0f\n\x07timeout\x18\t \x01(\r\x12\r\n\x05limit\x18\n \x01(\r\x12\x1a\n\x12\x64imensions_encoder\x18\r \x01(\x08\x12@\n\x0e\x65ncoder_params\x18* \x01(\x0b\x32(.admobilize.query.v1alpha1.EncoderParams\x12\x37\n\x08order_by\x18\x0f \x03(\x0b\x32%.admobilize.query.v1alpha1.OrderField\x12\x16\n\x0e\x66ilter_by_hour\x18\x10 \x03(\r\x12\x19\n\x11\x66ilter_by_weekday\x18\x11 \x03(\r\x12?\n\x0e\x66ilter_by_time\x18\x12 \x01(\x0b\x32\'.admobilize.query.v1alpha1.FilterByTime\x12\x36\n\x0b\x63ms_metrics\x18\x13 \x03(\x0b\x32!.admobilize.query.v1alpha1.Metric\x12>\n\rcms_dimension\x18\x14 \x01(\x0b\x32\'.admobilize.query.v1alpha1.CMSDimension\x12@\n\x0e\x63ms_descriptor\x18\x1e \x01(\x0b\x32(.admobilize.query.v1alpha1.CMSDescriptor\x12.\n\nstart_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08timezone\x18\x0e \x01(\t\x12\x0c\n\x03wid\x18\xe6\x07 \x01(\t\x12\x11\n\x08previous\x18\xe7\x07 \x01(\x08\"R\n\rQueryResponse\x12\x34\n\x08\x64\x61tasets\x18\x01 \x03(\x0b\x32\".admobilize.query.v1alpha1.Dataset\x12\x0b\n\x03tid\x18\x02 \x01(\t\"$\n\x11ListTablesRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\"$\n\x12ListTablesResponse\x12\x0e\n\x06tables\x18\x01 \x03(\t\"7\n\x15GetTableSchemaRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\"\x91\x01\n\x16GetTableSchemaResponse\x12\x36\n\x06schema\x18\x01 \x03(\x0b\x32&.admobilize.query.v1alpha1.SchemaField\x12\x10\n\x08num_rows\x18\x02 \x01(\x04\x12\x11\n\tnum_bytes\x18\x03 \x01(\x03\x12\x1a\n\x12last_modified_time\x18\x04 \x01(\x06\"\xba\x03\n\x10GetReportRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\r\n\x05\x65poch\x18\x03 \x01(\t\x12\x10\n\x08timezone\x18\t \x01(\t\x12\r\n\x05\x65mail\x18\x04 \x01(\t\x12\x0c\n\x04type\x18\x05 \x01(\t\x12\x0e\n\x06\x66ormat\x18\n \x01(\t\x12\x12\n\nspeed_unit\x18\x0b \x01(\t\x12\x19\n\x11\x66ilter_by_weekday\x18\x0c \x03(\r\x12?\n\x0e\x66ilter_by_time\x18\r \x01(\x0b\x32\'.admobilize.query.v1alpha1.FilterByTime\x12\x0e\n\x06\x66ields\x18\x0e \x03(\t\x12.\n\nstart_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x35\n\x07\x64\x65vices\x18\x08 \x03(\x0b\x32$.admobilize.query.v1alpha1.DeviceMap\x12\x13\n\x0b\x61\x64vertisers\x18\x0f \x03(\t\x12\x0e\n\x06medias\x18\x10 \x03(\t\"Z\n\x11GetReportResponse\x12\x31\n\x06status\x18\x01 \x01(\x0b\x32!.admobilize.query.v1alpha1.Status\x12\x12\n\nreport_url\x18\x02 \x01(\t\"\xdf\x01\n\x10\x43reateJobRequest\x12.\n\nstart_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\nproject_id\x18\x03 \x01(\t\x12\x12\n\nproduct_id\x18\x04 \x01(\t\x12\x10\n\x08timezone\x18\x07 \x01(\t\x12\x12\n\nspeed_unit\x18\x08 \x01(\t\x12\x12\n\ndevice_ids\x18\x05 \x03(\t\x12\x0b\n\x03\x63ms\x18\x06 \x01(\t\"G\n\rGetJobRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12*\n\x06\x66ields\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.FieldMask\"I\n\x14GetJobResultRequests\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x12\n\npage_token\x18\x03 \x01(\t\"2\n\x14\x45xportResultsRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0e\n\x06\x66ormat\x18\x02 \x01(\t\"j\n\x15GetDatapointsResponse\x12\x0e\n\x06job_id\x18\x01 \x01(\t\x12\x14\n\x0cjob_complete\x18\x02 \x01(\x08\x12\x17\n\x0fnext_page_token\x18\x03 \x01(\t\x12\x12\n\ndatapoints\x18\x04 \x01(\t\"K\n\x15\x45xportResultsResponse\x12\x0e\n\x06job_id\x18\x01 \x01(\t\x12\x14\n\x0cjob_complete\x18\x02 \x01(\x08\x12\x0c\n\x04urls\x18\x03 \x03(\t\"\xca\x03\n\x13GetTableDataRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\x0e\n\x06layout\x18\x03 \x01(\t\x12\x13\n\x0bmax_results\x18\x04 \x01(\r\x12\x12\n\npage_token\x18\x05 \x01(\t\x12\r\n\x05\x65poch\x18\x06 \x01(\t\x12\x35\n\x07\x64\x65vices\x18\x07 \x03(\x0b\x32$.admobilize.query.v1alpha1.DeviceMap\x12\x19\n\x11\x66ilter_by_weekday\x18\x08 \x03(\r\x12?\n\x0e\x66ilter_by_time\x18\t \x01(\x0b\x32\'.admobilize.query.v1alpha1.FilterByTime\x12\x10\n\x08group_by\x18\n \x03(\t\x12\x36\n\tfilter_by\x18\x0b \x01(\x0b\x32#.admobilize.query.v1alpha1.FilterBy\x12.\n\nstart_time\x18\x61 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x62 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08timezone\x18\x63 \x01(\t\"T\n\x14GetTableDataResponse\x12\x12\n\npage_token\x18\x02 \x01(\t\x12(\n\x04rows\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.ListValue\"4\n\x12ListReportsRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\"I\n\x13ListReportsResponse\x12\x32\n\x07reports\x18\x01 \x03(\x0b\x32!.admobilize.query.v1alpha1.Report\"\xb3\x03\n\x13\x43reateReportRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\x10\n\x08interval\x18\x03 \x01(\t\x12\x10\n\x08timezone\x18\t \x01(\t\x12\r\n\x05\x65mail\x18\x04 \x01(\t\x12\x0c\n\x04type\x18\x05 \x01(\t\x12\x0e\n\x06\x66ormat\x18\n \x01(\t\x12\x12\n\nspeed_unit\x18\x0b \x01(\t\x12\x11\n\tfrequency\x18\x0c \x01(\t\x12\x14\n\x0c\x64\x61ys_to_send\x18\r \x03(\t\x12\x19\n\x11\x66ilter_by_weekday\x18\x0e \x03(\r\x12?\n\x0e\x66ilter_by_time\x18\x0f \x01(\x0b\x32\'.admobilize.query.v1alpha1.FilterByTime\x12.\n\nstart_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07\x64\x65vices\x18\x08 \x03(\t\x12\x13\n\x0b\x61\x64vertisers\x18\x10 \x03(\t\x12\x0e\n\x06medias\x18\x11 \x03(\t\"\xdc\x02\n\x13UpdateReportRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\x0e\n\x06report\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x0c \x01(\t\x12\x10\n\x08interval\x18\x03 \x01(\t\x12\x10\n\x08timezone\x18\x04 \x01(\t\x12\r\n\x05\x65mail\x18\x05 \x03(\t\x12\x0c\n\x04type\x18\x06 \x01(\t\x12\x0e\n\x06\x66ormat\x18\x07 \x01(\t\x12\x12\n\nspeed_unit\x18\x08 \x01(\t\x12\x11\n\tfrequency\x18\t \x01(\t\x12\x14\n\x0c\x64\x61ys_to_send\x18\n \x03(\t\x12\x19\n\x11\x66ilter_by_weekday\x18\r \x03(\r\x12?\n\x0e\x66ilter_by_time\x18\x0e \x01(\x0b\x32\'.admobilize.query.v1alpha1.FilterByTime\x12,\n\x08\x65nd_time\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"D\n\x12PauseReportRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\x0e\n\x06report\x18\x03 \x01(\t\"F\n\x14RestartReportRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\x0e\n\x06report\x18\x03 \x01(\t\"E\n\x13\x43\x61ncelReportRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\x0e\n\x06report\x18\x03 \x01(\t\"\xb7\x01\n\x17GetDeviceHeatmapRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\x0e\n\x06\x64\x65vice\x18\x03 \x01(\t\x12.\n\nstart_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06\x66ilter\x18\x06 \x01(\t\"Q\n\x15ListDashboardResponse\x12\x38\n\ndashboards\x18\x01 \x03(\x0b\x32$.admobilize.query.v1alpha1.Dashboard\"(\n\x13GetDashboardRequest\x12\x11\n\tdashboard\x18\x01 \x01(\t2\xe5\x17\n\x0cQueryService\x12\x91\x01\n\x14\x43reateProjectDataset\x12\x36.admobilize.query.v1alpha1.CreateProjectDatasetRequest\x1a\".admobilize.query.v1alpha1.Project\"\x1d\x82\xd3\xe4\x93\x02\x17\"\x12/v1alpha1/projects:\x01*\x12\x9c\x01\n\x05Query\x12\'.admobilize.query.v1alpha1.QueryRequest\x1a(.admobilize.query.v1alpha1.QueryResponse\"@\x82\xd3\xe4\x93\x02:\"5/v1alpha1/projects/{project=*}/tables/{table=*}/query:\x01*\x12\x98\x01\n\nListTables\x12,.admobilize.query.v1alpha1.ListTablesRequest\x1a-.admobilize.query.v1alpha1.ListTablesResponse\"-\x82\xd3\xe4\x93\x02\'\x12%/v1alpha1/projects/{project=*}/tables\x12\xae\x01\n\x0eGetTableSchema\x12\x30.admobilize.query.v1alpha1.GetTableSchemaRequest\x1a\x31.admobilize.query.v1alpha1.GetTableSchemaResponse\"7\x82\xd3\xe4\x93\x02\x31\x12//v1alpha1/projects/{project=*}/tables/{table=*}\x12x\n\x0eListDashboards\x12\x16.google.protobuf.Empty\x1a\x30.admobilize.query.v1alpha1.ListDashboardResponse\"\x1c\x82\xd3\xe4\x93\x02\x16\x12\x14/v1alpha1/dashboards\x12\x90\x01\n\x0cGetDashboard\x12..admobilize.query.v1alpha1.GetDashboardRequest\x1a$.admobilize.query.v1alpha1.Dashboard\"*\x82\xd3\xe4\x93\x02$\x12\"/v1alpha1/dashboards/{dashboard=*}\x12\xa9\x01\n\tGetReport\x12+.admobilize.query.v1alpha1.GetReportRequest\x1a,.admobilize.query.v1alpha1.GetReportResponse\"A\x82\xd3\xe4\x93\x02;\"6/v1alpha1/projects/{project=*}/tables/{table=*}/report:\x01*\x12\xa5\x01\n\x0c\x43reateReport\x12..admobilize.query.v1alpha1.CreateReportRequest\x1a!.admobilize.query.v1alpha1.Report\"B\x82\xd3\xe4\x93\x02<\"7/v1alpha1/projects/{project=*}/tables/{table=*}/reports:\x01*\x12\x9f\x01\n\x0cUpdateReport\x12..admobilize.query.v1alpha1.UpdateReportRequest\x1a!.admobilize.query.v1alpha1.Report\"<\x82\xd3\xe4\x93\x02\x36\x1a\x31/v1alpha1/projects/{project=*}/reports/{report=*}:\x01*\x12\x9c\x01\n\x0bListReports\x12-.admobilize.query.v1alpha1.ListReportsRequest\x1a..admobilize.query.v1alpha1.ListReportsResponse\".\x82\xd3\xe4\x93\x02(\x12&/v1alpha1/projects/{project=*}/reports\x12\xb4\x01\n\x0bPauseReport\x12-.admobilize.query.v1alpha1.PauseReportRequest\x1a!.admobilize.query.v1alpha1.Report\"S\x82\xd3\xe4\x93\x02M\"H/v1alpha1/projects/{project=*}/tables/{table=*}/reports/{report=*}:pause:\x01*\x12\xba\x01\n\rRestartReport\x12/.admobilize.query.v1alpha1.RestartReportRequest\x1a!.admobilize.query.v1alpha1.Report\"U\x82\xd3\xe4\x93\x02O\"J/v1alpha1/projects/{project=*}/tables/{table=*}/reports/{report=*}:restart:\x01*\x12\xb0\x01\n\x0c\x43\x61ncelReport\x12..admobilize.query.v1alpha1.CancelReportRequest\x1a!.admobilize.query.v1alpha1.Report\"M\x82\xd3\xe4\x93\x02G*B/v1alpha1/projects/{project=*}/tables/{table=*}/reports/{report=*}:\x01*\x12\xb0\x01\n\x0cGetTableData\x12..admobilize.query.v1alpha1.GetTableDataRequest\x1a/.admobilize.query.v1alpha1.GetTableDataResponse\"?\x82\xd3\xe4\x93\x02\x39\"4/v1alpha1/projects/{project=*}/tables/{table=*}/data:\x01*\x12\xbd\x01\n\x10GetDeviceHeatmap\x12\x32.admobilize.query.v1alpha1.GetDeviceHeatmapRequest\x1a\".admobilize.query.v1alpha1.Heatmap\"Q\x82\xd3\xe4\x93\x02K\x12Iv1alpha1/projects/{project=*}/tables/{table=*}/devices/{device=*}/heatmap\x12p\n\tCreateJob\x12+.admobilize.query.v1alpha1.CreateJobRequest\x1a\x1e.admobilize.query.v1alpha1.Job\"\x16\x82\xd3\xe4\x93\x02\x10\"\x0e/v1alpha1/jobs\x12q\n\x06GetJob\x12(.admobilize.query.v1alpha1.GetJobRequest\x1a\x1e.admobilize.query.v1alpha1.Job\"\x1d\x82\xd3\xe4\x93\x02\x17\x12\x15/v1alpha1/{id=jobs/*}\x12\x99\x01\n\rGetJobResults\x12/.admobilize.query.v1alpha1.GetJobResultRequests\x1a\x30.admobilize.query.v1alpha1.GetDatapointsResponse\"%\x82\xd3\xe4\x93\x02\x1f\x12\x1d/v1alpha1/{id=jobs/*}/results\x12\x98\x01\n\rExportResults\x12/.admobilize.query.v1alpha1.ExportResultsRequest\x1a\x30.admobilize.query.v1alpha1.ExportResultsResponse\"$\x82\xd3\xe4\x93\x02\x1e\x12\x1c/v1alpha1/{id=jobs/*}/exportB\x9c\x01\n\x1d\x63om.admobilize.query.v1alpha1B\x13QueryResourcesProtoP\x01Z@bitbucket.org/admobilize/admobilizeapis-go/pkg/queryapi/v1alpha1\xa2\x02\x05\x41\x44MQY\xaa\x02\x19\x41\x64Mobilize.Query.V1Alpha1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n-admobilize/query/v1alpha1/query_service.proto\x12\x19\x61\x64mobilize.query.v1alpha1\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a google/protobuf/field_mask.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a)admobilize/query/v1alpha1/resources.proto\".\n\x1b\x43reateProjectDatasetRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\"\xdc\x07\n\x0cQueryRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\x32\n\x07metrics\x18\x03 \x03(\x0b\x32!.admobilize.query.v1alpha1.Metric\x12\x12\n\ndimensions\x18\x04 \x03(\t\x12\r\n\x05\x65poch\x18\x05 \x01(\t\x12\x16\n\x0ehas_comparison\x18\x06 \x01(\x08\x12\x44\n\x10\x61ggregate_result\x18\x0b \x01(\x0b\x32*.admobilize.query.v1alpha1.AggregateResult\x12\x45\n\x11query_from_result\x18( \x01(\x0b\x32*.admobilize.query.v1alpha1.QueryFromResult\x12:\n\x0b\x63lassifiers\x18\x0c \x03(\x0b\x32%.admobilize.query.v1alpha1.Classifier\x12\x0f\n\x07timeout\x18\t \x01(\r\x12\r\n\x05limit\x18\n \x01(\r\x12\x1a\n\x12\x64imensions_encoder\x18\r \x01(\x08\x12@\n\x0e\x65ncoder_params\x18* \x01(\x0b\x32(.admobilize.query.v1alpha1.EncoderParams\x12\x37\n\x08order_by\x18\x0f \x03(\x0b\x32%.admobilize.query.v1alpha1.OrderField\x12\x16\n\x0e\x66ilter_by_hour\x18\x10 \x03(\r\x12\x19\n\x11\x66ilter_by_weekday\x18\x11 \x03(\r\x12?\n\x0e\x66ilter_by_time\x18\x12 \x01(\x0b\x32\'.admobilize.query.v1alpha1.FilterByTime\x12\x36\n\x0b\x63ms_metrics\x18\x13 \x03(\x0b\x32!.admobilize.query.v1alpha1.Metric\x12>\n\rcms_dimension\x18\x14 \x01(\x0b\x32\'.admobilize.query.v1alpha1.CMSDimension\x12@\n\x0e\x63ms_descriptor\x18\x1e \x01(\x0b\x32(.admobilize.query.v1alpha1.CMSDescriptor\x12.\n\nstart_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08timezone\x18\x0e \x01(\t\x12\x0c\n\x03wid\x18\xe6\x07 \x01(\t\x12\x11\n\x08previous\x18\xe7\x07 \x01(\x08\"R\n\rQueryResponse\x12\x34\n\x08\x64\x61tasets\x18\x01 \x03(\x0b\x32\".admobilize.query.v1alpha1.Dataset\x12\x0b\n\x03tid\x18\x02 \x01(\t\"$\n\x11ListTablesRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\"$\n\x12ListTablesResponse\x12\x0e\n\x06tables\x18\x01 \x03(\t\"7\n\x15GetTableSchemaRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\"\x91\x01\n\x16GetTableSchemaResponse\x12\x36\n\x06schema\x18\x01 \x03(\x0b\x32&.admobilize.query.v1alpha1.SchemaField\x12\x10\n\x08num_rows\x18\x02 \x01(\x04\x12\x11\n\tnum_bytes\x18\x03 \x01(\x03\x12\x1a\n\x12last_modified_time\x18\x04 \x01(\x06\"\xba\x03\n\x10GetReportRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\r\n\x05\x65poch\x18\x03 \x01(\t\x12\x10\n\x08timezone\x18\t \x01(\t\x12\r\n\x05\x65mail\x18\x04 \x01(\t\x12\x0c\n\x04type\x18\x05 \x01(\t\x12\x0e\n\x06\x66ormat\x18\n \x01(\t\x12\x12\n\nspeed_unit\x18\x0b \x01(\t\x12\x19\n\x11\x66ilter_by_weekday\x18\x0c \x03(\r\x12?\n\x0e\x66ilter_by_time\x18\r \x01(\x0b\x32\'.admobilize.query.v1alpha1.FilterByTime\x12\x0e\n\x06\x66ields\x18\x0e \x03(\t\x12.\n\nstart_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x35\n\x07\x64\x65vices\x18\x08 \x03(\x0b\x32$.admobilize.query.v1alpha1.DeviceMap\x12\x13\n\x0b\x61\x64vertisers\x18\x0f \x03(\t\x12\x0e\n\x06medias\x18\x10 \x03(\t\"Z\n\x11GetReportResponse\x12\x31\n\x06status\x18\x01 \x01(\x0b\x32!.admobilize.query.v1alpha1.Status\x12\x12\n\nreport_url\x18\x02 \x01(\t\"\xdf\x01\n\x10\x43reateJobRequest\x12.\n\nstart_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\nproject_id\x18\x03 \x01(\t\x12\x12\n\nproduct_id\x18\x04 \x01(\t\x12\x10\n\x08timezone\x18\x07 \x01(\t\x12\x12\n\nspeed_unit\x18\x08 \x01(\t\x12\x12\n\ndevice_ids\x18\x05 \x03(\t\x12\x0b\n\x03\x63ms\x18\x06 \x01(\t\"G\n\rGetJobRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12*\n\x06\x66ields\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.FieldMask\"I\n\x14GetJobResultRequests\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x12\n\npage_token\x18\x03 \x01(\t\"2\n\x14\x45xportResultsRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0e\n\x06\x66ormat\x18\x02 \x01(\t\"j\n\x15GetDatapointsResponse\x12\x0e\n\x06job_id\x18\x01 \x01(\t\x12\x14\n\x0cjob_complete\x18\x02 \x01(\x08\x12\x17\n\x0fnext_page_token\x18\x03 \x01(\t\x12\x12\n\ndatapoints\x18\x04 \x01(\t\"K\n\x15\x45xportResultsResponse\x12\x0e\n\x06job_id\x18\x01 \x01(\t\x12\x14\n\x0cjob_complete\x18\x02 \x01(\x08\x12\x0c\n\x04urls\x18\x03 \x03(\t\"\xca\x03\n\x13GetTableDataRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\x0e\n\x06layout\x18\x03 \x01(\t\x12\x13\n\x0bmax_results\x18\x04 \x01(\r\x12\x12\n\npage_token\x18\x05 \x01(\t\x12\r\n\x05\x65poch\x18\x06 \x01(\t\x12\x35\n\x07\x64\x65vices\x18\x07 \x03(\x0b\x32$.admobilize.query.v1alpha1.DeviceMap\x12\x19\n\x11\x66ilter_by_weekday\x18\x08 \x03(\r\x12?\n\x0e\x66ilter_by_time\x18\t \x01(\x0b\x32\'.admobilize.query.v1alpha1.FilterByTime\x12\x10\n\x08group_by\x18\n \x03(\t\x12\x36\n\tfilter_by\x18\x0b \x01(\x0b\x32#.admobilize.query.v1alpha1.FilterBy\x12.\n\nstart_time\x18\x61 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x62 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08timezone\x18\x63 \x01(\t\"T\n\x14GetTableDataResponse\x12\x12\n\npage_token\x18\x02 \x01(\t\x12(\n\x04rows\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.ListValue\"4\n\x12ListReportsRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\"I\n\x13ListReportsResponse\x12\x32\n\x07reports\x18\x01 \x03(\x0b\x32!.admobilize.query.v1alpha1.Report\"\xb3\x03\n\x13\x43reateReportRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\x10\n\x08interval\x18\x03 \x01(\t\x12\x10\n\x08timezone\x18\t \x01(\t\x12\r\n\x05\x65mail\x18\x04 \x01(\t\x12\x0c\n\x04type\x18\x05 \x01(\t\x12\x0e\n\x06\x66ormat\x18\n \x01(\t\x12\x12\n\nspeed_unit\x18\x0b \x01(\t\x12\x11\n\tfrequency\x18\x0c \x01(\t\x12\x14\n\x0c\x64\x61ys_to_send\x18\r \x03(\t\x12\x19\n\x11\x66ilter_by_weekday\x18\x0e \x03(\r\x12?\n\x0e\x66ilter_by_time\x18\x0f \x01(\x0b\x32\'.admobilize.query.v1alpha1.FilterByTime\x12.\n\nstart_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07\x64\x65vices\x18\x08 \x03(\t\x12\x13\n\x0b\x61\x64vertisers\x18\x10 \x03(\t\x12\x0e\n\x06medias\x18\x11 \x03(\t\"\xdc\x02\n\x13UpdateReportRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\x0e\n\x06report\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x0c \x01(\t\x12\x10\n\x08interval\x18\x03 \x01(\t\x12\x10\n\x08timezone\x18\x04 \x01(\t\x12\r\n\x05\x65mail\x18\x05 \x03(\t\x12\x0c\n\x04type\x18\x06 \x01(\t\x12\x0e\n\x06\x66ormat\x18\x07 \x01(\t\x12\x12\n\nspeed_unit\x18\x08 \x01(\t\x12\x11\n\tfrequency\x18\t \x01(\t\x12\x14\n\x0c\x64\x61ys_to_send\x18\n \x03(\t\x12\x19\n\x11\x66ilter_by_weekday\x18\r \x03(\r\x12?\n\x0e\x66ilter_by_time\x18\x0e \x01(\x0b\x32\'.admobilize.query.v1alpha1.FilterByTime\x12,\n\x08\x65nd_time\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"D\n\x12PauseReportRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\x0e\n\x06report\x18\x03 \x01(\t\"F\n\x14RestartReportRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\x0e\n\x06report\x18\x03 \x01(\t\"E\n\x13\x43\x61ncelReportRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\x0e\n\x06report\x18\x03 \x01(\t\"\xb7\x01\n\x17GetDeviceHeatmapRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\x0e\n\x06\x64\x65vice\x18\x03 \x01(\t\x12.\n\nstart_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06\x66ilter\x18\x06 \x01(\t\"Q\n\x15ListDashboardResponse\x12\x38\n\ndashboards\x18\x01 \x03(\x0b\x32$.admobilize.query.v1alpha1.Dashboard\"(\n\x13GetDashboardRequest\x12\x11\n\tdashboard\x18\x01 \x01(\t2\xa5\x16\n\x0cQueryService\x12\x91\x01\n\x14\x43reateProjectDataset\x12\x36.admobilize.query.v1alpha1.CreateProjectDatasetRequest\x1a\".admobilize.query.v1alpha1.Project\"\x1d\x82\xd3\xe4\x93\x02\x17\"\x12/v1alpha1/projects:\x01*\x12\x9c\x01\n\x05Query\x12\'.admobilize.query.v1alpha1.QueryRequest\x1a(.admobilize.query.v1alpha1.QueryResponse\"@\x82\xd3\xe4\x93\x02:\"5/v1alpha1/projects/{project=*}/tables/{table=*}/query:\x01*\x12\x98\x01\n\nListTables\x12,.admobilize.query.v1alpha1.ListTablesRequest\x1a-.admobilize.query.v1alpha1.ListTablesResponse\"-\x82\xd3\xe4\x93\x02\'\x12%/v1alpha1/projects/{project=*}/tables\x12\xae\x01\n\x0eGetTableSchema\x12\x30.admobilize.query.v1alpha1.GetTableSchemaRequest\x1a\x31.admobilize.query.v1alpha1.GetTableSchemaResponse\"7\x82\xd3\xe4\x93\x02\x31\x12//v1alpha1/projects/{project=*}/tables/{table=*}\x12x\n\x0eListDashboards\x12\x16.google.protobuf.Empty\x1a\x30.admobilize.query.v1alpha1.ListDashboardResponse\"\x1c\x82\xd3\xe4\x93\x02\x16\x12\x14/v1alpha1/dashboards\x12\x90\x01\n\x0cGetDashboard\x12..admobilize.query.v1alpha1.GetDashboardRequest\x1a$.admobilize.query.v1alpha1.Dashboard\"*\x82\xd3\xe4\x93\x02$\x12\"/v1alpha1/dashboards/{dashboard=*}\x12\xa9\x01\n\tGetReport\x12+.admobilize.query.v1alpha1.GetReportRequest\x1a,.admobilize.query.v1alpha1.GetReportResponse\"A\x82\xd3\xe4\x93\x02;\"6/v1alpha1/projects/{project=*}/tables/{table=*}/report:\x01*\x12\xa5\x01\n\x0c\x43reateReport\x12..admobilize.query.v1alpha1.CreateReportRequest\x1a!.admobilize.query.v1alpha1.Report\"B\x82\xd3\xe4\x93\x02<\"7/v1alpha1/projects/{project=*}/tables/{table=*}/reports:\x01*\x12\x9f\x01\n\x0cUpdateReport\x12..admobilize.query.v1alpha1.UpdateReportRequest\x1a!.admobilize.query.v1alpha1.Report\"<\x82\xd3\xe4\x93\x02\x36\x1a\x31/v1alpha1/projects/{project=*}/reports/{report=*}:\x01*\x12\x9c\x01\n\x0bListReports\x12-.admobilize.query.v1alpha1.ListReportsRequest\x1a..admobilize.query.v1alpha1.ListReportsResponse\".\x82\xd3\xe4\x93\x02(\x12&/v1alpha1/projects/{project=*}/reports\x12\xb4\x01\n\x0bPauseReport\x12-.admobilize.query.v1alpha1.PauseReportRequest\x1a!.admobilize.query.v1alpha1.Report\"S\x82\xd3\xe4\x93\x02M\"H/v1alpha1/projects/{project=*}/tables/{table=*}/reports/{report=*}:pause:\x01*\x12\xba\x01\n\rRestartReport\x12/.admobilize.query.v1alpha1.RestartReportRequest\x1a!.admobilize.query.v1alpha1.Report\"U\x82\xd3\xe4\x93\x02O\"J/v1alpha1/projects/{project=*}/tables/{table=*}/reports/{report=*}:restart:\x01*\x12\xb0\x01\n\x0c\x43\x61ncelReport\x12..admobilize.query.v1alpha1.CancelReportRequest\x1a!.admobilize.query.v1alpha1.Report\"M\x82\xd3\xe4\x93\x02G*B/v1alpha1/projects/{project=*}/tables/{table=*}/reports/{report=*}:\x01*\x12\xb0\x01\n\x0cGetTableData\x12..admobilize.query.v1alpha1.GetTableDataRequest\x1a/.admobilize.query.v1alpha1.GetTableDataResponse\"?\x82\xd3\xe4\x93\x02\x39\"4/v1alpha1/projects/{project=*}/tables/{table=*}/data:\x01*\x12p\n\tCreateJob\x12+.admobilize.query.v1alpha1.CreateJobRequest\x1a\x1e.admobilize.query.v1alpha1.Job\"\x16\x82\xd3\xe4\x93\x02\x10\"\x0e/v1alpha1/jobs\x12q\n\x06GetJob\x12(.admobilize.query.v1alpha1.GetJobRequest\x1a\x1e.admobilize.query.v1alpha1.Job\"\x1d\x82\xd3\xe4\x93\x02\x17\x12\x15/v1alpha1/{id=jobs/*}\x12\x99\x01\n\rGetJobResults\x12/.admobilize.query.v1alpha1.GetJobResultRequests\x1a\x30.admobilize.query.v1alpha1.GetDatapointsResponse\"%\x82\xd3\xe4\x93\x02\x1f\x12\x1d/v1alpha1/{id=jobs/*}/results\x12\x98\x01\n\rExportResults\x12/.admobilize.query.v1alpha1.ExportResultsRequest\x1a\x30.admobilize.query.v1alpha1.ExportResultsResponse\"$\x82\xd3\xe4\x93\x02\x1e\x12\x1c/v1alpha1/{id=jobs/*}/exportB\x9c\x01\n\x1d\x63om.admobilize.query.v1alpha1B\x13QueryResourcesProtoP\x01Z@bitbucket.org/admobilize/admobilizeapis-go/pkg/queryapi/v1alpha1\xa2\x02\x05\x41\x44MQY\xaa\x02\x19\x41\x64Mobilize.Query.V1Alpha1b\x06proto3')
 
 
 
 _CREATEPROJECTDATASETREQUEST = DESCRIPTOR.message_types_by_name['CreateProjectDatasetRequest']
 _QUERYREQUEST = DESCRIPTOR.message_types_by_name['QueryRequest']
 _QUERYRESPONSE = DESCRIPTOR.message_types_by_name['QueryResponse']
 _LISTTABLESREQUEST = DESCRIPTOR.message_types_by_name['ListTablesRequest']
@@ -269,16 +269,14 @@
   _QUERYSERVICE.methods_by_name['PauseReport']._serialized_options = b'\202\323\344\223\002M\"H/v1alpha1/projects/{project=*}/tables/{table=*}/reports/{report=*}:pause:\001*'
   _QUERYSERVICE.methods_by_name['RestartReport']._options = None
   _QUERYSERVICE.methods_by_name['RestartReport']._serialized_options = b'\202\323\344\223\002O\"J/v1alpha1/projects/{project=*}/tables/{table=*}/reports/{report=*}:restart:\001*'
   _QUERYSERVICE.methods_by_name['CancelReport']._options = None
   _QUERYSERVICE.methods_by_name['CancelReport']._serialized_options = b'\202\323\344\223\002G*B/v1alpha1/projects/{project=*}/tables/{table=*}/reports/{report=*}:\001*'
   _QUERYSERVICE.methods_by_name['GetTableData']._options = None
   _QUERYSERVICE.methods_by_name['GetTableData']._serialized_options = b'\202\323\344\223\0029\"4/v1alpha1/projects/{project=*}/tables/{table=*}/data:\001*'
-  _QUERYSERVICE.methods_by_name['GetDeviceHeatmap']._options = None
-  _QUERYSERVICE.methods_by_name['GetDeviceHeatmap']._serialized_options = b'\202\323\344\223\002K\022Iv1alpha1/projects/{project=*}/tables/{table=*}/devices/{device=*}/heatmap'
   _QUERYSERVICE.methods_by_name['CreateJob']._options = None
   _QUERYSERVICE.methods_by_name['CreateJob']._serialized_options = b'\202\323\344\223\002\020\"\016/v1alpha1/jobs'
   _QUERYSERVICE.methods_by_name['GetJob']._options = None
   _QUERYSERVICE.methods_by_name['GetJob']._serialized_options = b'\202\323\344\223\002\027\022\025/v1alpha1/{id=jobs/*}'
   _QUERYSERVICE.methods_by_name['GetJobResults']._options = None
   _QUERYSERVICE.methods_by_name['GetJobResults']._serialized_options = b'\202\323\344\223\002\037\022\035/v1alpha1/{id=jobs/*}/results'
   _QUERYSERVICE.methods_by_name['ExportResults']._options = None
@@ -334,9 +332,9 @@
   _GETDEVICEHEATMAPREQUEST._serialized_start=4506
   _GETDEVICEHEATMAPREQUEST._serialized_end=4689
   _LISTDASHBOARDRESPONSE._serialized_start=4691
   _LISTDASHBOARDRESPONSE._serialized_end=4772
   _GETDASHBOARDREQUEST._serialized_start=4774
   _GETDASHBOARDREQUEST._serialized_end=4814
   _QUERYSERVICE._serialized_start=4817
-  _QUERYSERVICE._serialized_end=7862
+  _QUERYSERVICE._serialized_end=7670
 # @@protoc_insertion_point(module_scope)
```

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/ayuda/v1alpha1/ayuda_service_pb2.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/ayuda/v1alpha1/ayuda_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/ayuda/v1alpha1/ayuda_service_pb2_grpc.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/ayuda/v1alpha1/ayuda_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/ayuda/v1alpha1/resources_pb2.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/ayuda/v1alpha1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/signagelive/v1alpha1/signagelive_service_pb2.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/signagelive/v1alpha1/signagelive_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/signagelive/v1alpha1/signagelive_service_pb2_grpc.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/signagelive/v1alpha1/signagelive_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/signagelive/v1alpha1/resources_pb2.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/signagelive/v1alpha1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/common/entity_pb2.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/common/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/common/admobilize_types_pb2.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/common/admobilize_types_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/common/job_pb2.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/common/job_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/billing/v1alpha1/billing_pb2.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/billing/v1alpha1/billing_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/brightauthor/v1alpha1/brightauthor_service_pb2_grpc.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/brightauthor/v1alpha1/brightauthor_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/brightauthor/v1alpha1/resources_pb2.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/brightauthor/v1alpha1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/brightauthor/v1alpha1/brightauthor_service_pb2.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/brightauthor/v1alpha1/brightauthor_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/cmsintegrations/v1/cmsintegrations_service_pb2_grpc.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/cmsintegrations/v1/cmsintegrations_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/cmsintegrations/v1/resources_pb2.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/cmsintegrations/v1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/cmsintegrations/v1/cmsintegrations_service_pb2.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/cmsintegrations/v1/cmsintegrations_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/broadsign/v1alpha1/broadsign_service_pb2_grpc.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/broadsign/v1alpha1/broadsign_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/broadsign/v1alpha1/resources_pb2.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/broadsign/v1alpha1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilize/proto/broadsign/v1alpha1/broadsign_service_pb2.py` & `admobilizeapis-2023.7.18.post3/admobilize/proto/broadsign/v1alpha1/broadsign_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/PKG-INFO` & `admobilizeapis-2023.7.18.post3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: admobilizeapis
-Version: 2023.7.18.post2
+Version: 2023.7.18.post3
 Summary: Protobufs used in AdMobilize Ecosystem
 Home-page: https://www.bitbucket.org/admobilize/admobilizeapis
 Author: AdMobilize Team
 Author-email: devel@admobilize.com
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `admobilizeapis-2023.7.18.post2/admobilizeapis.egg-info/SOURCES.txt` & `admobilizeapis-2023.7.18.post3/admobilizeapis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/admobilizeapis.egg-info/PKG-INFO` & `admobilizeapis-2023.7.18.post3/admobilizeapis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: admobilizeapis
-Version: 2023.7.18.post2
+Version: 2023.7.18.post3
 Summary: Protobufs used in AdMobilize Ecosystem
 Home-page: https://www.bitbucket.org/admobilize/admobilizeapis
 Author: AdMobilize Team
 Author-email: devel@admobilize.com
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `admobilizeapis-2023.7.18.post2/README.md` & `admobilizeapis-2023.7.18.post3/README.md`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.7.18.post2/setup.py` & `admobilizeapis-2023.7.18.post3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 install_requires = ["google-api-core >= 1.6.0, < 2.0.0dev", "protobuf >= 3.6.0, < 4.0"]
 
 extras_require = {"grpc": ["grpcio>=1.2.0"]}
 
 setup(
     name="admobilizeapis",
-    version='2023.07.18r2',
+    version='2023.07.18r3',
     author="AdMobilize Team",
     author_email="devel@admobilize.com",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Programming Language :: Python",
```

