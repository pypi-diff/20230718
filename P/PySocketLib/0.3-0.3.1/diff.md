# Comparing `tmp/PySocketLib-0.3.tar.gz` & `tmp/PySocketLib-0.3.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySocketLib-0.3.tar", last modified: Mon Jul 17 11:18:43 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

