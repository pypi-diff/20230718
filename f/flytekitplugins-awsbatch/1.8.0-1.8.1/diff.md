# Comparing `tmp/flytekitplugins-awsbatch-1.8.0.tar.gz` & `tmp/flytekitplugins_awsbatch-1.8.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-awsbatch-1.8.0.tar", last modified: Tue Jul 11 22:07:12 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

