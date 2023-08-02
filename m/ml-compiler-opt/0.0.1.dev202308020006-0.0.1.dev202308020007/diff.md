# Comparing `tmp/ml-compiler-opt-0.0.1.dev202308020006.tar.gz` & `tmp/ml_compiler_opt-0.0.1.dev202308020007-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-compiler-opt-0.0.1.dev202308020006.tar", last modified: Wed Aug  2 00:06:56 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

