# Comparing `tmp/python-univer-1.3.8.tar.gz` & `tmp/python-univer-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-univer-1.3.8.tar", last modified: Thu Jan 19 04:21:08 2023, max compression
+gzip compressed data, was "python-univer-1.3.9.tar", last modified: Tue Jul 18 16:12:43 2023, max compression
```

## Comparing `python-univer-1.3.8.tar` & `python-univer-1.3.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 user      (1000) user      (1001)        0 2023-01-19 04:21:08.423333 python-univer-1.3.8/
--rw-r--r--   0 user      (1000) user      (1001)        0 2022-09-03 09:22:45.000000 python-univer-1.3.8/LICENSE
--rw-r--r--   0 user      (1000) user      (1001)     1269 2023-01-19 04:21:08.420000 python-univer-1.3.8/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1001)      706 2022-09-03 09:22:45.000000 python-univer-1.3.8/README.md
-drwxr-xr-x   0 user      (1000) user      (1001)        0 2023-01-19 04:21:08.416666 python-univer-1.3.8/python_univer.egg-info/
--rw-r--r--   0 user      (1000) user      (1001)     1269 2023-01-19 04:21:08.000000 python-univer-1.3.8/python_univer.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1001)      732 2023-01-19 04:21:08.000000 python-univer-1.3.8/python_univer.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1001)        1 2023-01-19 04:21:08.000000 python-univer-1.3.8/python_univer.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1001)       18 2023-01-19 04:21:08.000000 python-univer-1.3.8/python_univer.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1001)       10 2023-01-19 04:21:08.000000 python-univer-1.3.8/python_univer.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1001)       38 2023-01-19 04:21:08.423333 python-univer-1.3.8/setup.cfg
--rw-r--r--   0 user      (1000) user      (1001)      891 2023-01-19 04:13:58.000000 python-univer-1.3.8/setup.py
-drwxr-xr-x   0 user      (1000) user      (1001)        0 2023-01-19 04:21:08.420000 python-univer-1.3.8/univer_db/
--rw-r--r--   0 user      (1000) user      (1001)        0 2022-09-03 09:22:45.000000 python-univer-1.3.8/univer_db/__init__.py
--rw-r--r--   0 user      (1000) user      (1001)      472 2023-01-12 11:42:13.000000 python-univer-1.3.8/univer_db/config.py
-drwxr-xr-x   0 user      (1000) user      (1001)        0 2023-01-19 04:21:08.420000 python-univer-1.3.8/univer_db/models/
--rw-r--r--   0 user      (1000) user      (1001)      225 2023-01-12 11:42:13.000000 python-univer-1.3.8/univer_db/models/__init__.py
--rw-r--r--   0 user      (1000) user      (1001)     9291 2023-01-12 11:42:13.000000 python-univer-1.3.8/univer_db/models/base.py
--rw-r--r--   0 user      (1000) user      (1001)     8231 2022-09-03 09:22:45.000000 python-univer-1.3.8/univer_db/models/dormitories.py
--rw-r--r--   0 user      (1000) user      (1001)     1873 2023-01-12 16:07:27.000000 python-univer-1.3.8/univer_db/models/geo.py
--rw-r--r--   0 user      (1000) user      (1001)      951 2022-09-03 09:22:45.000000 python-univer-1.3.8/univer_db/models/grades.py
--rw-r--r--   0 user      (1000) user      (1001)        0 2022-09-03 09:22:45.000000 python-univer-1.3.8/univer_db/models/groups.py
--rw-r--r--   0 user      (1000) user      (1001)    33958 2023-01-19 04:13:44.000000 python-univer-1.3.8/univer_db/models/models.py
--rw-r--r--   0 user      (1000) user      (1001)     9202 2022-09-03 09:22:45.000000 python-univer-1.3.8/univer_db/models/orders.py
--rw-r--r--   0 user      (1000) user      (1001)    22021 2022-09-03 09:22:45.000000 python-univer-1.3.8/univer_db/models/roles.py
--rw-r--r--   0 user      (1000) user      (1001)     4182 2022-09-03 09:22:45.000000 python-univer-1.3.8/univer_db/models/schedule.py
--rw-r--r--   0 user      (1000) user      (1001)     3558 2022-09-03 09:22:45.000000 python-univer-1.3.8/univer_db/models/sheets.py
--rw-r--r--   0 user      (1000) user      (1001)     5047 2022-09-03 09:22:45.000000 python-univer-1.3.8/univer_db/models/structures.py
--rw-r--r--   0 user      (1000) user      (1001)      769 2023-01-12 11:42:13.000000 python-univer-1.3.8/univer_db/orm.py
-drwxr-xr-x   0 user      (1000) user      (1001)        0 2023-01-19 04:21:08.420000 python-univer-1.3.8/univer_db/tests/
--rw-r--r--   0 user      (1000) user      (1001)      264 2022-09-03 09:22:45.000000 python-univer-1.3.8/univer_db/tests/__init__.py
--rw-r--r--   0 user      (1000) user      (1001)      569 2023-01-12 16:11:14.000000 python-univer-1.3.8/univer_db/tests/geo.py
--rw-r--r--   0 user      (1000) user      (1001)     2635 2023-01-19 04:19:06.000000 python-univer-1.3.8/univer_db/tests/models.py
--rw-r--r--   0 user      (1000) user      (1001)     1136 2022-09-03 09:22:45.000000 python-univer-1.3.8/univer_db/tests/roles.py
--rw-r--r--   0 user      (1000) user      (1001)      624 2022-09-03 09:22:45.000000 python-univer-1.3.8/univer_db/tests/structures.py
+drwxr-xr-x   0 user      (1000) user      (1001)        0 2023-07-18 16:12:43.860000 python-univer-1.3.9/
+-rw-r--r--   0 user      (1000) user      (1001)        0 2023-07-18 16:09:38.000000 python-univer-1.3.9/LICENSE
+-rw-r--r--   0 user      (1000) user      (1001)     1233 2023-07-18 16:12:43.860000 python-univer-1.3.9/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1001)      706 2023-07-18 16:09:38.000000 python-univer-1.3.9/README.md
+drwxr-xr-x   0 user      (1000) user      (1001)        0 2023-07-18 16:12:43.860000 python-univer-1.3.9/python_univer.egg-info/
+-rw-r--r--   0 user      (1000) user      (1001)     1233 2023-07-18 16:12:43.000000 python-univer-1.3.9/python_univer.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1001)      732 2023-07-18 16:12:43.000000 python-univer-1.3.9/python_univer.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1001)        1 2023-07-18 16:12:43.000000 python-univer-1.3.9/python_univer.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1001)       18 2023-07-18 16:12:43.000000 python-univer-1.3.9/python_univer.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1001)       10 2023-07-18 16:12:43.000000 python-univer-1.3.9/python_univer.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1001)       38 2023-07-18 16:12:43.860000 python-univer-1.3.9/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1001)      891 2023-07-18 16:11:45.000000 python-univer-1.3.9/setup.py
+drwxr-xr-x   0 user      (1000) user      (1001)        0 2023-07-18 16:12:43.860000 python-univer-1.3.9/univer_db/
+-rw-r--r--   0 user      (1000) user      (1001)        0 2023-07-18 16:09:38.000000 python-univer-1.3.9/univer_db/__init__.py
+-rw-r--r--   0 user      (1000) user      (1001)      472 2023-07-18 16:09:38.000000 python-univer-1.3.9/univer_db/config.py
+drwxr-xr-x   0 user      (1000) user      (1001)        0 2023-07-18 16:12:43.860000 python-univer-1.3.9/univer_db/models/
+-rw-r--r--   0 user      (1000) user      (1001)      225 2023-07-18 16:09:38.000000 python-univer-1.3.9/univer_db/models/__init__.py
+-rw-r--r--   0 user      (1000) user      (1001)     9291 2023-07-18 16:09:38.000000 python-univer-1.3.9/univer_db/models/base.py
+-rw-r--r--   0 user      (1000) user      (1001)     8231 2023-07-18 16:09:38.000000 python-univer-1.3.9/univer_db/models/dormitories.py
+-rw-r--r--   0 user      (1000) user      (1001)     1873 2023-07-18 16:09:38.000000 python-univer-1.3.9/univer_db/models/geo.py
+-rw-r--r--   0 user      (1000) user      (1001)      951 2023-07-18 16:09:38.000000 python-univer-1.3.9/univer_db/models/grades.py
+-rw-r--r--   0 user      (1000) user      (1001)        0 2023-07-18 16:09:38.000000 python-univer-1.3.9/univer_db/models/groups.py
+-rw-r--r--   0 user      (1000) user      (1001)    33958 2023-07-18 16:09:38.000000 python-univer-1.3.9/univer_db/models/models.py
+-rw-r--r--   0 user      (1000) user      (1001)     9202 2023-07-18 16:09:38.000000 python-univer-1.3.9/univer_db/models/orders.py
+-rw-r--r--   0 user      (1000) user      (1001)    22087 2023-07-18 16:11:15.000000 python-univer-1.3.9/univer_db/models/roles.py
+-rw-r--r--   0 user      (1000) user      (1001)     4182 2023-07-18 16:09:38.000000 python-univer-1.3.9/univer_db/models/schedule.py
+-rw-r--r--   0 user      (1000) user      (1001)     3558 2023-07-18 16:09:38.000000 python-univer-1.3.9/univer_db/models/sheets.py
+-rw-r--r--   0 user      (1000) user      (1001)     5047 2023-07-18 16:09:38.000000 python-univer-1.3.9/univer_db/models/structures.py
+-rw-r--r--   0 user      (1000) user      (1001)      769 2023-07-18 16:09:38.000000 python-univer-1.3.9/univer_db/orm.py
+drwxr-xr-x   0 user      (1000) user      (1001)        0 2023-07-18 16:12:43.860000 python-univer-1.3.9/univer_db/tests/
+-rw-r--r--   0 user      (1000) user      (1001)      264 2023-07-18 16:09:38.000000 python-univer-1.3.9/univer_db/tests/__init__.py
+-rw-r--r--   0 user      (1000) user      (1001)      569 2023-07-18 16:09:38.000000 python-univer-1.3.9/univer_db/tests/geo.py
+-rw-r--r--   0 user      (1000) user      (1001)     2635 2023-07-18 16:09:38.000000 python-univer-1.3.9/univer_db/tests/models.py
+-rw-r--r--   0 user      (1000) user      (1001)     1136 2023-07-18 16:09:38.000000 python-univer-1.3.9/univer_db/tests/roles.py
+-rw-r--r--   0 user      (1000) user      (1001)      624 2023-07-18 16:09:38.000000 python-univer-1.3.9/univer_db/tests/structures.py
```

### Comparing `python-univer-1.3.8/PKG-INFO` & `python-univer-1.3.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: python-univer
-Version: 1.3.8
+Version: 1.3.9
 Summary: Данная библиотека содержить SqlAlchemy ORM для системы Univer
 Home-page: https://github.com/yessenovuniversity/python_univer
 Author: Nauryzbek Aitbayev
 Author-email: nauryzbek.aitbayev@yu.edu.kz
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -42,8 +40,7 @@
 session = Session()
 
 students = session.query(Student).filter(Student.course == 2, Student.status == 1)
 
 for student in students:
     print(student)
 ```
-
```

### Comparing `python-univer-1.3.8/README.md` & `python-univer-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `python-univer-1.3.8/python_univer.egg-info/PKG-INFO` & `python-univer-1.3.9/python_univer.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: python-univer
-Version: 1.3.8
+Version: 1.3.9
 Summary: Данная библиотека содержить SqlAlchemy ORM для системы Univer
 Home-page: https://github.com/yessenovuniversity/python_univer
 Author: Nauryzbek Aitbayev
 Author-email: nauryzbek.aitbayev@yu.edu.kz
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -42,8 +40,7 @@
 session = Session()
 
 students = session.query(Student).filter(Student.course == 2, Student.status == 1)
 
 for student in students:
     print(student)
 ```
-
```

### Comparing `python-univer-1.3.8/python_univer.egg-info/SOURCES.txt` & `python-univer-1.3.9/python_univer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-univer-1.3.8/setup.py` & `python-univer-1.3.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="python-univer",
-    version="1.3.8",
+    version="1.3.9",
     author="Nauryzbek Aitbayev",
     author_email="nauryzbek.aitbayev@yu.edu.kz",
     description="Данная библиотека содержить SqlAlchemy ORM для системы Univer",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/yessenovuniversity/python_univer",
     packages=setuptools.find_packages(),
```

### Comparing `python-univer-1.3.8/univer_db/models/base.py` & `python-univer-1.3.9/univer_db/models/base.py`

 * *Files identical despite different names*

### Comparing `python-univer-1.3.8/univer_db/models/dormitories.py` & `python-univer-1.3.9/univer_db/models/dormitories.py`

 * *Files identical despite different names*

### Comparing `python-univer-1.3.8/univer_db/models/geo.py` & `python-univer-1.3.9/univer_db/models/geo.py`

 * *Files identical despite different names*

### Comparing `python-univer-1.3.8/univer_db/models/grades.py` & `python-univer-1.3.9/univer_db/models/grades.py`

 * *Files identical despite different names*

### Comparing `python-univer-1.3.8/univer_db/models/models.py` & `python-univer-1.3.9/univer_db/models/models.py`

 * *Files identical despite different names*

### Comparing `python-univer-1.3.8/univer_db/models/orders.py` & `python-univer-1.3.9/univer_db/models/orders.py`

 * *Files identical despite different names*

### Comparing `python-univer-1.3.8/univer_db/models/roles.py` & `python-univer-1.3.9/univer_db/models/roles.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,17 +138,17 @@
     enrollment_type = relationship('EnrollmentType')
 
     # Район
     district_id = Column(ForeignKey('univer_district.district_id'))
     district = relationship('District')
 
     # ФИО студента
-    last_name = Column('students_sname', String(100))
-    first_name = Column('students_name', String(100))
-    middle_name = Column('students_father_name', String(100))
+    last_name = Column('students_sname', String(100, collation='utf8-bin'))
+    first_name = Column('students_name', String(100, collation='utf8-bin'))
+    middle_name = Column('students_father_name', String(100, collation='utf8-bin'))
 
     # Дата рождения
     birth_date = Column('students_birth_date', DateTime)
 
     # Электронная почта
     email = Column('students_email', String(25))
```

### Comparing `python-univer-1.3.8/univer_db/models/schedule.py` & `python-univer-1.3.9/univer_db/models/schedule.py`

 * *Files identical despite different names*

### Comparing `python-univer-1.3.8/univer_db/models/sheets.py` & `python-univer-1.3.9/univer_db/models/sheets.py`

 * *Files identical despite different names*

### Comparing `python-univer-1.3.8/univer_db/models/structures.py` & `python-univer-1.3.9/univer_db/models/structures.py`

 * *Files identical despite different names*

### Comparing `python-univer-1.3.8/univer_db/orm.py` & `python-univer-1.3.9/univer_db/orm.py`

 * *Files identical despite different names*

### Comparing `python-univer-1.3.8/univer_db/tests/geo.py` & `python-univer-1.3.9/univer_db/tests/geo.py`

 * *Files identical despite different names*

### Comparing `python-univer-1.3.8/univer_db/tests/models.py` & `python-univer-1.3.9/univer_db/tests/models.py`

 * *Files identical despite different names*

### Comparing `python-univer-1.3.8/univer_db/tests/roles.py` & `python-univer-1.3.9/univer_db/tests/roles.py`

 * *Files identical despite different names*

### Comparing `python-univer-1.3.8/univer_db/tests/structures.py` & `python-univer-1.3.9/univer_db/tests/structures.py`

 * *Files identical despite different names*

