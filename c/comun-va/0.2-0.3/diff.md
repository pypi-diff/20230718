# Comparing `tmp/comun_va-0.2.tar.gz` & `tmp/comun_va-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comun_va-0.2.tar", last modified: Mon Jul 17 12:45:36 2023, max compression
+gzip compressed data, was "comun_va-0.3.tar", last modified: Mon Jul 17 13:07:17 2023, max compression
```

## Comparing `comun_va-0.2.tar` & `comun_va-0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 12:45:36.350635 comun_va-0.2/
--rw-rw-rw-   0        0        0       53 2023-07-17 12:45:36.349331 comun_va-0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-17 12:45:36.347873 comun_va-0.2/comun_va.egg-info/
--rw-rw-rw-   0        0        0       53 2023-07-17 12:45:36.000000 comun_va-0.2/comun_va.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      179 2023-07-17 12:45:36.000000 comun_va-0.2/comun_va.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 12:45:36.000000 comun_va-0.2/comun_va.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-07-17 12:45:36.000000 comun_va-0.2/comun_va.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-17 12:45:36.000000 comun_va-0.2/comun_va.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4510 2023-07-17 12:40:44.000000 comun_va-0.2/comun_va.py
--rw-rw-rw-   0        0        0       42 2023-07-17 12:45:36.350635 comun_va-0.2/setup.cfg
--rw-rw-rw-   0        0        0      192 2023-07-17 12:45:20.000000 comun_va-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 13:07:17.123624 comun_va-0.3/
+-rw-rw-rw-   0        0        0       53 2023-07-17 13:07:17.123624 comun_va-0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-17 13:07:17.122613 comun_va-0.3/comun_va.egg-info/
+-rw-rw-rw-   0        0        0       53 2023-07-17 13:07:17.000000 comun_va-0.3/comun_va.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      179 2023-07-17 13:07:17.000000 comun_va-0.3/comun_va.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 13:07:17.000000 comun_va-0.3/comun_va.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-07-17 13:07:17.000000 comun_va-0.3/comun_va.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-17 13:07:17.000000 comun_va-0.3/comun_va.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4515 2023-07-17 13:04:26.000000 comun_va-0.3/comun_va.py
+-rw-rw-rw-   0        0        0       42 2023-07-17 13:07:17.124626 comun_va-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      192 2023-07-17 13:07:07.000000 comun_va-0.3/setup.py
```

### Comparing `comun_va-0.2/comun_va.py` & `comun_va-0.3/comun_va.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
                         self.prediction,
                         self.img_name,
                         self.error)
         mssql.ejecutar(query, query_values)
         mssql.cerrar_conexion()
 
 
-def get_image_from_ip_camera(camera_url):
+def get_image_from_ip_camera(camera_url: str):
     """
     Function that connect to an IP camera and return a frame
     :param camera_url: need to be the RTSP URL
     :return: given frame from OpenCV when you read a video capture
     """
     try:
         cap = cv2.VideoCapture(camera_url)  # IP Camera
```

