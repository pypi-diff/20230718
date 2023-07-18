# Comparing `tmp/pyexifwrangle-0.1.2.tar.gz` & `tmp/pyexifwrangle-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyexifwrangle-0.1.2.tar", last modified: Thu Jul 13 15:40:02 2023, max compression
+gzip compressed data, was "dist/pyexifwrangle-0.1.3.tar", last modified: Tue Jul 18 15:04:52 2023, max compression
```

## Comparing `pyexifwrangle-0.1.2.tar` & `pyexifwrangle-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 stephanie   (501) staff       (20)        0 2023-07-13 15:40:02.000000 pyexifwrangle-0.1.2/
--rw-r--r--   0 stephanie   (501) staff       (20)     5328 2023-07-13 15:40:02.000000 pyexifwrangle-0.1.2/PKG-INFO
--rw-r--r--   0 stephanie   (501) staff       (20)     3898 2023-07-13 15:33:15.000000 pyexifwrangle-0.1.2/README.md
-drwxr-xr-x   0 stephanie   (501) staff       (20)        0 2023-07-13 15:40:02.000000 pyexifwrangle-0.1.2/pyexifwrangle/
--rw-r--r--   0 stephanie   (501) staff       (20)      132 2023-07-13 15:36:05.000000 pyexifwrangle-0.1.2/pyexifwrangle/__init__.py
--rw-r--r--   0 stephanie   (501) staff       (20)     2690 2023-07-12 18:15:44.000000 pyexifwrangle-0.1.2/pyexifwrangle/wrangle.py
-drwxr-xr-x   0 stephanie   (501) staff       (20)        0 2023-07-13 15:40:02.000000 pyexifwrangle-0.1.2/pyexifwrangle.egg-info/
--rw-r--r--   0 stephanie   (501) staff       (20)     5328 2023-07-13 15:40:01.000000 pyexifwrangle-0.1.2/pyexifwrangle.egg-info/PKG-INFO
--rw-r--r--   0 stephanie   (501) staff       (20)      253 2023-07-13 15:40:02.000000 pyexifwrangle-0.1.2/pyexifwrangle.egg-info/SOURCES.txt
--rw-r--r--   0 stephanie   (501) staff       (20)        1 2023-07-13 15:40:01.000000 pyexifwrangle-0.1.2/pyexifwrangle.egg-info/dependency_links.txt
--rw-r--r--   0 stephanie   (501) staff       (20)       38 2023-07-13 15:40:01.000000 pyexifwrangle-0.1.2/pyexifwrangle.egg-info/requires.txt
--rw-r--r--   0 stephanie   (501) staff       (20)       14 2023-07-13 15:40:01.000000 pyexifwrangle-0.1.2/pyexifwrangle.egg-info/top_level.txt
--rw-r--r--   0 stephanie   (501) staff       (20)       38 2023-07-13 15:40:02.000000 pyexifwrangle-0.1.2/setup.cfg
--rw-r--r--   0 stephanie   (501) staff       (20)     1167 2023-07-13 15:34:41.000000 pyexifwrangle-0.1.2/setup.py
+drwxr-xr-x   0 stephanie   (501) staff       (20)        0 2023-07-18 15:04:52.000000 pyexifwrangle-0.1.3/
+-rw-r--r--   0 stephanie   (501) staff       (20)     5328 2023-07-18 15:04:52.000000 pyexifwrangle-0.1.3/PKG-INFO
+-rw-r--r--   0 stephanie   (501) staff       (20)     3898 2023-07-13 15:33:15.000000 pyexifwrangle-0.1.3/README.md
+drwxr-xr-x   0 stephanie   (501) staff       (20)        0 2023-07-18 15:04:52.000000 pyexifwrangle-0.1.3/pyexifwrangle/
+-rw-r--r--   0 stephanie   (501) staff       (20)      132 2023-07-18 15:03:29.000000 pyexifwrangle-0.1.3/pyexifwrangle/__init__.py
+-rw-r--r--   0 stephanie   (501) staff       (20)     4112 2023-07-18 14:48:49.000000 pyexifwrangle-0.1.3/pyexifwrangle/wrangle.py
+drwxr-xr-x   0 stephanie   (501) staff       (20)        0 2023-07-18 15:04:52.000000 pyexifwrangle-0.1.3/pyexifwrangle.egg-info/
+-rw-r--r--   0 stephanie   (501) staff       (20)     5328 2023-07-18 15:04:52.000000 pyexifwrangle-0.1.3/pyexifwrangle.egg-info/PKG-INFO
+-rw-r--r--   0 stephanie   (501) staff       (20)      253 2023-07-18 15:04:52.000000 pyexifwrangle-0.1.3/pyexifwrangle.egg-info/SOURCES.txt
+-rw-r--r--   0 stephanie   (501) staff       (20)        1 2023-07-18 15:04:52.000000 pyexifwrangle-0.1.3/pyexifwrangle.egg-info/dependency_links.txt
+-rw-r--r--   0 stephanie   (501) staff       (20)       38 2023-07-18 15:04:52.000000 pyexifwrangle-0.1.3/pyexifwrangle.egg-info/requires.txt
+-rw-r--r--   0 stephanie   (501) staff       (20)       14 2023-07-18 15:04:52.000000 pyexifwrangle-0.1.3/pyexifwrangle.egg-info/top_level.txt
+-rw-r--r--   0 stephanie   (501) staff       (20)       38 2023-07-18 15:04:52.000000 pyexifwrangle-0.1.3/setup.cfg
+-rw-r--r--   0 stephanie   (501) staff       (20)     1167 2023-07-13 15:34:41.000000 pyexifwrangle-0.1.3/setup.py
```

### Comparing `pyexifwrangle-0.1.2/PKG-INFO` & `pyexifwrangle-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyexifwrangle
-Version: 0.1.2
+Version: 0.1.3
 Summary: A helper package for wrangling image EXIF data
 Home-page: https://github.com/stephaniereinders/pyexifwrangle
 Author: Stephanie Reinders
 Author-email: reinders.stephanie@gmail.com
 License: MIT
 Description: # Wrangle EXIF Data in Python
```

### Comparing `pyexifwrangle-0.1.2/README.md` & `pyexifwrangle-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pyexifwrangle-0.1.2/pyexifwrangle/wrangle.py` & `pyexifwrangle-0.1.3/pyexifwrangle/wrangle.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 def count_images_by_columns(df, columns, sort=None):
     """
     Group images by column(s) and count images
 
     Args:
         df (DataFrame): Data frame of EXIF data
         columns (list): List of columns to group by
+        sort (list): Optional list of columns for sorting returned data frame
 
     Returns:
         DataFrame
     """
 
     # group and count
     df = df.groupby(columns).size().reset_index()
@@ -37,15 +38,24 @@
     if sort is not None:
         df = df.sort_values(by=sort).reset_index(drop=True)
 
     return df
 
 
 def get_column(df, column):
-    """Extract column from data frame as list"""
+    """
+    Extract column from data frame as list
+
+    Args:
+        df (DataFrame): Data frame of EXIF data
+        column (str): Name of column to extract
+
+    Returns:
+        List
+    """
     return df[column].to_list()
 
 
 def filename2columns(df, filename_col, columns):
     """
     Split the filename column into individual columns.
 
@@ -69,16 +79,49 @@
     for i in range(1, len(columns)+1):
         column = columns.pop()
         df.insert(0, column, df[filename_col].str.split(os.path.sep).str[-i])
 
     return df
 
 
+def find_images(df, filter_dict, return_columns=None):
+    """
+    Use Pandas to filter the EXIF data frame for column(s) and column value(s) specified in filter_dict.
+
+    Args:
+        df (DataFrame): Data frame of EXIF data
+        filter_dict (dict): Dictionary of column and column value pair(s). Example filter_dict={'phone':
+        's21_1', 'Aperture': 2.2}
+        return_columns (list): Optional list of columns to return if you don't want the entire data frame
+
+    Returns:
+        DataFrame
+    """
+    for k, v in filter_dict.items():
+        df = df.query("`{0}` == @v".format(k)).reset_index(drop=True)
+
+    if return_columns is not None:
+        df = df[return_columns]
+
+    return df
+
+
 def read_exif(path, filename_col, encoding='utf-8'):
-    # read csv
+    """
+    Load EXIF data from a csv file as a Pandas data frame and drop any images whose name starts with '.'
+
+    Args:
+        path (str): Absolute or relative file path and file name of the csv file containing EXIF data extracted using
+        Phil Harvey's EXIFTool
+        filename_col (str): The name of the column in the EXIF data that contains the images' filenames
+        encoding (str): The encoding for Pandas to use when loading the csv file of EXIF data
+
+    Returns:
+        DataFrame
+    """
     df = pd.read_csv(path, encoding=encoding)
 
     # drop file names that start with '.'
     files = get_column(df=df, column=filename_col)
     images = pd.Series([s.split('/')[-1].strip() for s in files])
     df = df[~images.str.startswith('.')]
```

### Comparing `pyexifwrangle-0.1.2/pyexifwrangle.egg-info/PKG-INFO` & `pyexifwrangle-0.1.3/pyexifwrangle.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyexifwrangle
-Version: 0.1.2
+Version: 0.1.3
 Summary: A helper package for wrangling image EXIF data
 Home-page: https://github.com/stephaniereinders/pyexifwrangle
 Author: Stephanie Reinders
 Author-email: reinders.stephanie@gmail.com
 License: MIT
 Description: # Wrangle EXIF Data in Python
```

### Comparing `pyexifwrangle-0.1.2/setup.py` & `pyexifwrangle-0.1.3/setup.py`

 * *Files identical despite different names*

