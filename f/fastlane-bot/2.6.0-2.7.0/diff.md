# Comparing `tmp/fastlane_bot-2.6.0.tar.gz` & `tmp/fastlane_bot-2.7.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastlane_bot-2.6.0.tar", last modified: Mon Jul 31 20:08:55 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

