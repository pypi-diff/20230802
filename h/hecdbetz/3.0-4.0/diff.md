# Comparing `tmp/hecdbetz-3.0.tar.gz` & `tmp/hecdbetz-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hecdbetz-3.0.tar", last modified: Wed Aug  2 08:49:54 2023, max compression
+gzip compressed data, was "dist/hecdbetz-4.0.tar", last modified: Wed Aug  2 09:24:54 2023, max compression
```

## Comparing `hecdbetz-3.0.tar` & `hecdbetz-4.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 zhangmingwei  (1000) zhangmingwei  (1000)        0 2023-08-02 08:49:54.000000 hecdbetz-3.0/
--rwxrw-r--   0 zhangmingwei  (1000) zhangmingwei  (1000)      582 2023-08-02 07:23:55.000000 hecdbetz-3.0/LICENSE
--rw-rw-r--   0 zhangmingwei  (1000) zhangmingwei  (1000)       84 2023-08-02 08:49:54.000000 hecdbetz-3.0/PKG-INFO
--rw-rw-r--   0 zhangmingwei  (1000) zhangmingwei  (1000)       21 2023-08-02 06:06:04.000000 hecdbetz-3.0/README.md
-drwxrwxr-x   0 zhangmingwei  (1000) zhangmingwei  (1000)        0 2023-08-02 08:49:54.000000 hecdbetz-3.0/hecdbetz/
--rw-rw-r--   0 zhangmingwei  (1000) zhangmingwei  (1000)       21 2023-08-02 06:45:08.000000 hecdbetz-3.0/hecdbetz/__init__.py
--rw-rw-r--   0 zhangmingwei  (1000) zhangmingwei  (1000)       33 2023-08-02 06:44:58.000000 hecdbetz-3.0/hecdbetz/add_num.py
--rw-rw-r--   0 zhangmingwei  (1000) zhangmingwei  (1000)      683 2023-08-02 06:13:22.000000 hecdbetz-3.0/hecdbetz/calculate.py
-drwxrwxr-x   0 zhangmingwei  (1000) zhangmingwei  (1000)        0 2023-08-02 08:49:54.000000 hecdbetz-3.0/hecdbetz.egg-info/
--rw-rw-r--   0 zhangmingwei  (1000) zhangmingwei  (1000)       84 2023-08-02 08:49:53.000000 hecdbetz-3.0/hecdbetz.egg-info/PKG-INFO
--rw-rw-r--   0 zhangmingwei  (1000) zhangmingwei  (1000)      252 2023-08-02 08:49:53.000000 hecdbetz-3.0/hecdbetz.egg-info/SOURCES.txt
--rw-rw-r--   0 zhangmingwei  (1000) zhangmingwei  (1000)        1 2023-08-02 08:49:53.000000 hecdbetz-3.0/hecdbetz.egg-info/dependency_links.txt
--rw-rw-r--   0 zhangmingwei  (1000) zhangmingwei  (1000)       53 2023-08-02 08:49:53.000000 hecdbetz-3.0/hecdbetz.egg-info/entry_points.txt
--rw-rw-r--   0 zhangmingwei  (1000) zhangmingwei  (1000)        9 2023-08-02 08:49:53.000000 hecdbetz-3.0/hecdbetz.egg-info/top_level.txt
--rw-rw-r--   0 zhangmingwei  (1000) zhangmingwei  (1000)       38 2023-08-02 08:49:54.000000 hecdbetz-3.0/setup.cfg
--rwxrw-rw-   0 zhangmingwei  (1000) zhangmingwei  (1000)      345 2023-08-02 08:49:38.000000 hecdbetz-3.0/setup.py
+drwxrwxr-x   0 zhangmingwei  (1000) zhangmingwei  (1000)        0 2023-08-02 09:24:54.000000 hecdbetz-4.0/
+-rwxrw-r--   0 zhangmingwei  (1000) zhangmingwei  (1000)      582 2023-08-02 07:23:55.000000 hecdbetz-4.0/LICENSE
+-rw-rw-r--   0 zhangmingwei  (1000) zhangmingwei  (1000)       84 2023-08-02 09:24:54.000000 hecdbetz-4.0/PKG-INFO
+-rw-rw-r--   0 zhangmingwei  (1000) zhangmingwei  (1000)       21 2023-08-02 06:06:04.000000 hecdbetz-4.0/README.md
+drwxrwxr-x   0 zhangmingwei  (1000) zhangmingwei  (1000)        0 2023-08-02 09:24:54.000000 hecdbetz-4.0/hecdbetz/
+-rw-rw-r--   0 zhangmingwei  (1000) zhangmingwei  (1000)       21 2023-08-02 06:45:08.000000 hecdbetz-4.0/hecdbetz/__init__.py
+-rw-rw-r--   0 zhangmingwei  (1000) zhangmingwei  (1000)       33 2023-08-02 06:44:58.000000 hecdbetz-4.0/hecdbetz/add_num.py
+-rwxrw-rw-   0 zhangmingwei  (1000) zhangmingwei  (1000)      713 2023-08-02 09:23:26.000000 hecdbetz-4.0/hecdbetz/calculate.py
+drwxrwxr-x   0 zhangmingwei  (1000) zhangmingwei  (1000)        0 2023-08-02 09:24:54.000000 hecdbetz-4.0/hecdbetz.egg-info/
+-rw-rw-r--   0 zhangmingwei  (1000) zhangmingwei  (1000)       84 2023-08-02 09:24:52.000000 hecdbetz-4.0/hecdbetz.egg-info/PKG-INFO
+-rw-rw-r--   0 zhangmingwei  (1000) zhangmingwei  (1000)      252 2023-08-02 09:24:52.000000 hecdbetz-4.0/hecdbetz.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhangmingwei  (1000) zhangmingwei  (1000)        1 2023-08-02 09:24:52.000000 hecdbetz-4.0/hecdbetz.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhangmingwei  (1000) zhangmingwei  (1000)       53 2023-08-02 09:24:52.000000 hecdbetz-4.0/hecdbetz.egg-info/entry_points.txt
+-rw-rw-r--   0 zhangmingwei  (1000) zhangmingwei  (1000)        9 2023-08-02 09:24:52.000000 hecdbetz-4.0/hecdbetz.egg-info/top_level.txt
+-rw-rw-r--   0 zhangmingwei  (1000) zhangmingwei  (1000)       38 2023-08-02 09:24:54.000000 hecdbetz-4.0/setup.cfg
+-rwxrw-rw-   0 zhangmingwei  (1000) zhangmingwei  (1000)      345 2023-08-02 09:24:23.000000 hecdbetz-4.0/setup.py
```

### Comparing `hecdbetz-3.0/LICENSE` & `hecdbetz-4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hecdbetz-3.0/hecdbetz/calculate.py` & `hecdbetz-4.0/hecdbetz/calculate.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,15 +11,20 @@
         result = num1 / num2
     else:
         print("Invalid operation")
         return
 
     print(f"The result of {operation} is: {result}")
 
-if __name__ == "__main__":
+def main():
     if len(sys.argv) != 4:
         print("Usage: python calculator.py <operation> <num1> <num2>")
     else:
         operation = sys.argv[1]
         num1 = float(sys.argv[2])
         num2 = float(sys.argv[3])
-        calculate(operation, num1, num2)
+        calculate(operation, num1, num2)
+
+
+if __name__ == "__main__":
+    main()
+
```

