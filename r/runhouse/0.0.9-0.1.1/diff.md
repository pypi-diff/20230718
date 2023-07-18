# Comparing `tmp/runhouse-0.0.9.tar.gz` & `tmp/runhouse-0.1.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runhouse-0.0.9.tar", last modified: Tue Jul 18 20:49:09 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

