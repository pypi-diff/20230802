# Comparing `tmp/flet_runtime-0.9.0.dev1623.tar.gz` & `tmp/flet_runtime-0.9.0.dev1630-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_runtime-0.9.0.dev1623.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

