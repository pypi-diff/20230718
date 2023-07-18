# Comparing `tmp/mesh_database_client-1.0.tar.gz` & `tmp/mesh_database_client-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mesh_database_client-1.0.tar", last modified: Sun Feb 12 00:57:56 2023, max compression
+gzip compressed data, was "dist\mesh_database_client-1.1.tar", last modified: Tue Jul 18 06:24:18 2023, max compression
```

## Comparing `mesh_database_client-1.0.tar` & `mesh_database_client-1.1.tar`

### file list

```diff
@@ -1,14 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-02-12 00:57:56.848877 mesh_database_client-1.0/
--rw-rw-rw-   0        0        0      553 2023-02-12 00:57:56.849876 mesh_database_client-1.0/PKG-INFO
--rw-rw-rw-   0        0        0      146 2023-02-12 00:23:57.000000 mesh_database_client-1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-02-12 00:57:56.831879 mesh_database_client-1.0/mesh_database_client/
--rw-rw-rw-   0        0        0       36 2023-01-30 04:48:44.000000 mesh_database_client-1.0/mesh_database_client/__init__.py
--rw-rw-rw-   0        0        0     6545 2023-02-12 00:56:24.000000 mesh_database_client-1.0/mesh_database_client/database.py
-drwxrwxrwx   0        0        0        0 2023-02-12 00:57:56.847876 mesh_database_client-1.0/mesh_database_client.egg-info/
--rw-rw-rw-   0        0        0      553 2023-02-12 00:57:56.000000 mesh_database_client-1.0/mesh_database_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      313 2023-02-12 00:57:56.000000 mesh_database_client-1.0/mesh_database_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-12 00:57:56.000000 mesh_database_client-1.0/mesh_database_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2023-02-12 00:57:56.000000 mesh_database_client-1.0/mesh_database_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-02-12 00:57:56.000000 mesh_database_client-1.0/mesh_database_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-02-12 00:57:56.850875 mesh_database_client-1.0/setup.cfg
--rw-rw-rw-   0        0        0      719 2023-02-12 00:33:41.000000 mesh_database_client-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 06:24:18.477008 mesh_database_client-1.1/
+-rw-rw-rw-   0        0        0      263 2023-07-18 06:24:18.477008 mesh_database_client-1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-18 06:24:18.458008 mesh_database_client-1.1/mesh_database_client/
+-rw-rw-rw-   0        0        0       36 2023-02-14 05:09:50.000000 mesh_database_client-1.1/mesh_database_client/__init__.py
+-rw-rw-rw-   0        0        0     7958 2023-07-18 04:56:31.000000 mesh_database_client-1.1/mesh_database_client/database.py
+drwxrwxrwx   0        0        0        0 2023-07-18 06:24:18.475008 mesh_database_client-1.1/mesh_database_client.egg-info/
+-rw-rw-rw-   0        0        0      263 2023-07-18 06:24:18.000000 mesh_database_client-1.1/mesh_database_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2023-07-18 06:24:18.000000 mesh_database_client-1.1/mesh_database_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 06:24:18.000000 mesh_database_client-1.1/mesh_database_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-07-18 06:24:18.000000 mesh_database_client-1.1/mesh_database_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 06:24:18.478008 mesh_database_client-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      345 2023-07-18 06:11:45.000000 mesh_database_client-1.1/setup.py
```

### Comparing `mesh_database_client-1.0/mesh_database_client/database.py` & `mesh_database_client-1.1/mesh_database_client/database.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 from google.oauth2 import service_account
 import pandas as pd
 import os
 import googlemaps
 from dotenv import load_dotenv
 from numpy import sqrt
 
-class DatabaseClient:
+load_dotenv()
 
-    def __init__(self, spreadsheet_id = None):
+class DatabaseClient:
 
-        load_dotenv()
+    def __init__(self, spreadsheet_id = None, include_active = False):
 
         self.spreadsheet_id = spreadsheet_id
         if self.spreadsheet_id is None:
             self.spreadsheet_id = os.environ.get("SPREADSHEET_ID")
 
         SCOPES = ['https://www.googleapis.com/auth/spreadsheets.readonly']
         # created in Google Cloud admin
@@ -32,15 +32,19 @@
 
         # Call the Sheets API
         self.sheet = self.service.spreadsheets()
 
         self.signup_df = self.get_signup_df()
         self.links_df = self.get_links_df()
 
-        # self.gmaps = googlemaps.Client(key=os.environ.get("MAPS_API"))
+        if include_active:
+            self.active_node_df = self.get_active_node_df()
+            self.active_link_df = self.get_active_link_df()
+
+        self.gmaps = googlemaps.Client(key=os.environ.get("MAPS_API"))
 
     def _get_sheets_credentials_from_env(self):
         try:
             credentials_mapping = {
                 "type": "GOOGLE_SHEETS_TYPE",
                 "project_id": "GOOGLE_SHEETS_PROJECT_ID",
                 "private_key_id": "GOOGLE_SHEETS_PRIVATE_KEY_ID",
@@ -79,27 +83,63 @@
         # force columns to be specific type
         df['NN'] = (pd.to_numeric(df['NN'], errors="coerce").fillna(0).astype(int))
         df['ID'] = (pd.to_numeric(df['ID'], errors="coerce").fillna(0).astype(int))
 
         df['Latitude'] = pd.to_numeric(df['Latitude'], errors='coerce')
         df['Longitude'] = pd.to_numeric(df['Longitude'], errors='coerce')
 
+        df['installDate'] = pd.to_datetime(df['installDate'], errors='coerce')
+
         df.drop(df.tail(1).index,inplace=True)
          
         return df
 
 
     def get_links_df(self):
         df = self.get_range_as_df('Links!A:I')
 
         # force columns to be specific type
         df['to'] = (pd.to_numeric(df['to'], errors="coerce").fillna(0).astype(int))
         df['from'] = (pd.to_numeric(df['from'], errors="coerce").fillna(0).astype(int))
         
         return df
+    
+    def get_active_node_df(self):
+        df = self.signup_df.copy()
+        df = df.sort_values(by=['installDate'])
+        df = df[df['Status'].isin(['Installed', 'NN assigned'])]
+        df = df[df['NN'] != 0]
+        df = df.drop_duplicates(subset='NN', keep='first')
+
+        return df
+    
+    def get_active_link_df(self):
+        df = self.links_df.copy()
+
+        columns_list = list(df.columns)
+        columns_list[6] = 'to_nn'
+        columns_list[7] = 'from_nn'
+
+        df.columns = columns_list
+
+        df['to'] = df['to_nn']
+        df['from'] = df['from_nn']
+        
+        df['to'] = pd.to_numeric(df['to'], errors='coerce').fillna(0).astype(int)
+        df['from'] = pd.to_numeric(df['from'], errors='coerce').fillna(0).astype(int)
+
+        df = df[~df['status'].isin(['dead', 'planned'])]
+
+        df = df[(df['to'] != 0) & (df['from'] != 0)]
+
+        # enure only active nodes are in links df
+        nns = self.active_node_df["NN"]
+        df = df[df["from"].isin(nns) & df["to"].isin(nns)]
+
+        return df
 
     def name_to_nn(self, name):
         signup_df = self.signup_df
         name_df = signup_df[signup_df['Name'].str.contains(name, case=False)]
         
         if name_df.empty:
             return None
@@ -182,13 +222,16 @@
         for index, row in nn_rows.iterrows():
             if row['Status'] == 'Installed':
                 return input_number
 
         return None
 
     def nn_to_location(self, nn):
-        row = self.signup_df[self.signup_df['NN'] == nn].iloc[0]
+        df = self.active_node_df
+        row = df[df['NN'] == nn].iloc[0]
         return {'Latitude': row.Latitude, 'Longitude': row.Longitude}
 
 
 if __name__ == '__main__':
-    database_client = DatabaseClient()
+    database_client = DatabaseClient(include_active=True)
+    name = database_client.name_to_nn("test")
+    print(name)
```

