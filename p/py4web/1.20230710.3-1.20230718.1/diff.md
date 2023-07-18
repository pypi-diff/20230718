# Comparing `tmp/py4web-1.20230710.3.tar.gz` & `tmp/py4web-1.20230718.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py4web-1.20230710.3.tar", last modified: Tue Jul 11 04:13:33 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

