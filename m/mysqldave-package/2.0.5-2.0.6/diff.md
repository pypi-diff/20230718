# Comparing `tmp/mysqldave_package-2.0.5.tar.gz` & `tmp/mysqldave_package-2.0.6.tar.gz`

## Comparing `mysqldave_package-2.0.5.tar` & `mysqldave_package-2.0.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 mysqldave_package-2.0.5/Admin Query SQL.md
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 mysqldave_package-2.0.5/Admin Statitics SQL.md
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 mysqldave_package-2.0.5/Cancel Queries.md
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 mysqldave_package-2.0.5/DB Analysis Queries.md
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 mysqldave_package-2.0.5/MySQL_basics.sql
--rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 mysqldave_package-2.0.5/QuickStart.md
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 mysqldave_package-2.0.5/Restore.md
--rwxr-xr-x   0        0        0      538 2020-02-02 00:00:00.000000 mysqldave_package-2.0.5/export_to_csv.bat
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 mysqldave_package-2.0.5/methods.md
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 mysqldave_package-2.0.5/src/mysqldave_package/.schemawiz_config2
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mysqldave_package-2.0.5/src/mysqldave_package/__init__.py
--rw-r--r--   0        0        0    14927 2020-02-02 00:00:00.000000 mysqldave_package-2.0.5/src/mysqldave_package/mysqldave.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 mysqldave_package-2.0.5/src/mysqldave_package/restored_sample.ddl
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 mysqldave_package-2.0.5/src/mysqldave_package/sample.csv
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 mysqldave_package-2.0.5/src/mysqldave_package/testcase1.csv
--rw-r--r--   0        0        0    54404 2020-02-02 00:00:00.000000 mysqldave_package-2.0.5/src/mysqldave_package/this.tsv
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 mysqldave_package-2.0.5/tests/.schemawiz_config2
--rwxr-xr-x   0        0        0      316 2020-02-02 00:00:00.000000 mysqldave_package-2.0.5/tests/backup.bat
--rwxr-xr-x   0        0        0      300 2020-02-02 00:00:00.000000 mysqldave_package-2.0.5/tests/restore.bat
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 mysqldave_package-2.0.5/tests/sample7.csv
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 mysqldave_package-2.0.5/tests/sample8.csv
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 mysqldave_package-2.0.5/tests/test_query_lock.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 mysqldave_package-2.0.5/tests/tester.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 mysqldave_package-2.0.5/tests/thistbl.csv
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 mysqldave_package-2.0.5/tests/z.new_sample7.ddl
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 mysqldave_package-2.0.5/tests/z.new_sample8.ddl
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 mysqldave_package-2.0.5/tests/z.new_thistbl.ddl
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 mysqldave_package-2.0.5/tests/z.restored_1sample7.ddl
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 mysqldave_package-2.0.5/tests/z.restored_sample7.ddl
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 mysqldave_package-2.0.5/tests/z.restored_sample8.ddl
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 mysqldave_package-2.0.5/tests/z.restored_thistbl.ddl
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 mysqldave_package-2.0.5/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 mysqldave_package-2.0.5/LICENSE
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 mysqldave_package-2.0.5/README.md
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 mysqldave_package-2.0.5/pyproject.toml
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 mysqldave_package-2.0.5/PKG-INFO
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 mysqldave_package-2.0.6/Admin Query SQL.md
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 mysqldave_package-2.0.6/Admin Statitics SQL.md
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 mysqldave_package-2.0.6/Cancel Queries.md
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 mysqldave_package-2.0.6/DB Analysis Queries.md
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 mysqldave_package-2.0.6/MySQL_basics.sql
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 mysqldave_package-2.0.6/QuickStart.md
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 mysqldave_package-2.0.6/Restore.md
+-rwxr-xr-x   0        0        0      538 2020-02-02 00:00:00.000000 mysqldave_package-2.0.6/export_to_csv.bat
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 mysqldave_package-2.0.6/methods.md
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 mysqldave_package-2.0.6/src/mysqldave_package/.schemawiz_config2
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mysqldave_package-2.0.6/src/mysqldave_package/__init__.py
+-rw-r--r--   0        0        0    14966 2020-02-02 00:00:00.000000 mysqldave_package-2.0.6/src/mysqldave_package/mysqldave.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 mysqldave_package-2.0.6/src/mysqldave_package/restored_sample.ddl
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 mysqldave_package-2.0.6/src/mysqldave_package/sample.csv
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 mysqldave_package-2.0.6/src/mysqldave_package/testcase1.csv
+-rw-r--r--   0        0        0    54404 2020-02-02 00:00:00.000000 mysqldave_package-2.0.6/src/mysqldave_package/this.tsv
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 mysqldave_package-2.0.6/tests/.schemawiz_config2
+-rwxr-xr-x   0        0        0      316 2020-02-02 00:00:00.000000 mysqldave_package-2.0.6/tests/backup.bat
+-rwxr-xr-x   0        0        0      300 2020-02-02 00:00:00.000000 mysqldave_package-2.0.6/tests/restore.bat
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 mysqldave_package-2.0.6/tests/sample7.csv
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 mysqldave_package-2.0.6/tests/sample8.csv
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 mysqldave_package-2.0.6/tests/test_query_lock.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 mysqldave_package-2.0.6/tests/tester.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 mysqldave_package-2.0.6/tests/thistbl.csv
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 mysqldave_package-2.0.6/tests/z.new_sample7.ddl
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 mysqldave_package-2.0.6/tests/z.new_sample8.ddl
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 mysqldave_package-2.0.6/tests/z.new_thistbl.ddl
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 mysqldave_package-2.0.6/tests/z.restored_1sample7.ddl
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 mysqldave_package-2.0.6/tests/z.restored_sample7.ddl
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 mysqldave_package-2.0.6/tests/z.restored_sample8.ddl
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 mysqldave_package-2.0.6/tests/z.restored_thistbl.ddl
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 mysqldave_package-2.0.6/.gitignore
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 mysqldave_package-2.0.6/LICENSE
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 mysqldave_package-2.0.6/README.md
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 mysqldave_package-2.0.6/pyproject.toml
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 mysqldave_package-2.0.6/PKG-INFO
```

### Comparing `mysqldave_package-2.0.5/Admin Statitics SQL.md` & `mysqldave_package-2.0.6/Admin Statitics SQL.md`

 * *Files identical despite different names*

### Comparing `mysqldave_package-2.0.5/DB Analysis Queries.md` & `mysqldave_package-2.0.6/DB Analysis Queries.md`

 * *Files identical despite different names*

### Comparing `mysqldave_package-2.0.5/QuickStart.md` & `mysqldave_package-2.0.6/QuickStart.md`

 * *Files identical despite different names*

### Comparing `mysqldave_package-2.0.5/export_to_csv.bat` & `mysqldave_package-2.0.6/export_to_csv.bat`

 * *Files identical despite different names*

### Comparing `mysqldave_package-2.0.5/methods.md` & `mysqldave_package-2.0.6/methods.md`

 * *Files identical despite different names*

### Comparing `mysqldave_package-2.0.5/src/mysqldave_package/mysqldave.py` & `mysqldave_package-2.0.6/src/mysqldave_package/mysqldave.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 def main():
 	mydb = mysql_db('this connection')
 	mydb.connect()
 	print(mydb.dbstr())
 
 
-	mydb.export_table_to_csv('this.tsv','information_schema.tables',',')
+	#mydb.export_table_to_csv('this.tsv','information_schema.tables',',')
 
 	#csvfilename = 'testcase1.csv'
 	#tblname = 'testcase1'
 	#mydb.load_csv_to_table(csvfilename,tblname,True,',')
 
 	mydb.close()
 
@@ -459,14 +459,15 @@
 		if self.db_conn_dets.DB_USERPWD == 'no-password-supplied':
 			self.ask_for_database_details()
 			connects_entered = True
 
 		try:
 			self.dbconn = mysql.connector.connect(
 					host=self.db_conn_dets.DB_HOST,
+					port=self.db_conn_dets.DB_PORT,
 					user=self.db_conn_dets.DB_USERNAME,
 					passwd=self.db_conn_dets.DB_USERPWD,
 					database=self.db_conn_dets.DB_NAME,
 					autocommit=True
 			)
 			self.cur = self.dbconn.cursor()
```

### Comparing `mysqldave_package-2.0.5/src/mysqldave_package/restored_sample.ddl` & `mysqldave_package-2.0.6/src/mysqldave_package/restored_sample.ddl`

 * *Files identical despite different names*

### Comparing `mysqldave_package-2.0.5/src/mysqldave_package/this.tsv` & `mysqldave_package-2.0.6/src/mysqldave_package/this.tsv`

 * *Files identical despite different names*

### Comparing `mysqldave_package-2.0.5/LICENSE` & `mysqldave_package-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mysqldave_package-2.0.5/pyproject.toml` & `mysqldave_package-2.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling","mysql.connector","garbledave_package"]
 
 build-backend = "hatchling.build"
 
 [project]
 name = "mysqldave_package"
-version = "2.0.5"
+version = "2.0.6"
 dependencies = [
   'mysql-connector-python >= 8.0.32',
   'garbledave_package >= 1.0.0'
 ]
 authors = [
   { name="Dave Skura", email="dskura@gmail.com" },
 ]
```

### Comparing `mysqldave_package-2.0.5/PKG-INFO` & `mysqldave_package-2.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqldave_package
-Version: 2.0.5
+Version: 2.0.6
 Summary: A wrapper for simplified Postgres usage using mysql.connector.
 Project-URL: Homepage, https://github.com/daveskura/mysqldave
 Project-URL: Author Linkedin, https://www.linkedin.com/in/2166883
 Author-email: Dave Skura <dskura@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

