# Comparing `tmp/alchql-3.3.1.28931664.tar.gz` & `tmp/alchql-3.3.1.28931672-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alchql-3.3.1.28931664.tar", last modified: Tue Jul 18 18:11:25 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

