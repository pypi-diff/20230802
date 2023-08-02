# Comparing `tmp/alqrrelu_package-0.1.0.tar.gz` & `tmp/alqrrelu_package-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alqrrelu_package-0.1.0.tar", max compression
+gzip compressed data, was "alqrrelu_package-0.2.0.tar", max compression
```

## Comparing `alqrrelu_package-0.1.0.tar` & `alqrrelu_package-0.2.0.tar`

### file list

```diff
@@ -1,4 +1,6 @@
--rw-r--r--   0        0        0        0 2023-08-02 02:39:01.151423 alqrrelu_package-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-08-02 02:39:01.151317 alqrrelu_package-0.1.0/alqrrelu_package/__init__.py
--rw-r--r--   0        0        0      324 2023-08-02 02:55:10.139466 alqrrelu_package-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      450 1970-01-01 00:00:00.000000 alqrrelu_package-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-02 02:39:01.151423 alqrrelu_package-0.2.0/README.md
+-rw-r--r--   0        0        0     6148 2023-08-02 03:42:24.498734 alqrrelu_package-0.2.0/alqrrelu_package/.DS_Store
+-rw-r--r--   0        0        0        0 2023-08-02 02:39:01.151317 alqrrelu_package-0.2.0/alqrrelu_package/__init__.py
+-rw-r--r--   0        0        0      618 2023-08-02 02:46:59.737002 alqrrelu_package-0.2.0/alqrrelu_package/alqrrelu.py
+-rw-r--r--   0        0        0      324 2023-08-02 03:46:39.201378 alqrrelu_package-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      450 1970-01-01 00:00:00.000000 alqrrelu_package-0.2.0/PKG-INFO
```

