# Comparing `tmp/trlc-1.1.5.tar.gz` & `tmp/trlc-1.1.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trlc-1.1.5.tar", last modified: Mon Jun 12 13:03:47 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

