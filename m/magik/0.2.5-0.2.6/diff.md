# Comparing `tmp/magik-0.2.5.tar.gz` & `tmp/magik-0.2.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magik-0.2.5.tar", last modified: Mon Jul 31 09:38:43 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

