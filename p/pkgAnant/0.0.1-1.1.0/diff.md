# Comparing `tmp/pkgAnant-0.0.1.tar.gz` & `tmp/pkgAnant-1.1.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkgAnant-0.0.1.tar", last modified: Fri Jul 14 12:44:14 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

