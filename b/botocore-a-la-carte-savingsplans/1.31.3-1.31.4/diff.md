# Comparing `tmp/botocore-a-la-carte-savingsplans-1.31.3.tar.gz` & `tmp/botocore_a_la_carte_savingsplans-1.31.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-savingsplans-1.31.3.tar", last modified: Fri Jul 14 01:46:42 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

