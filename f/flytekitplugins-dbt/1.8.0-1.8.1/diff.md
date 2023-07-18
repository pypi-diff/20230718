# Comparing `tmp/flytekitplugins-dbt-1.8.0.tar.gz` & `tmp/flytekitplugins_dbt-1.8.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-dbt-1.8.0.tar", last modified: Tue Jul 11 22:07:15 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

