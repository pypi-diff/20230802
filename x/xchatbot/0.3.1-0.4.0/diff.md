# Comparing `tmp/xchatbot-0.3.1.tar.gz` & `tmp/xchatbot-0.4.0-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/xchatbot-0.3.1.tar", last modified: Sun Apr 26 13:56:13 2020, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

