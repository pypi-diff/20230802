# Comparing `tmp/FindMyIP-1.1.1.tar.gz` & `tmp/FindMyIP-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FindMyIP-1.1.1.tar", last modified: Tue May 11 09:15:36 2021, max compression
+gzip compressed data, was "FindMyIP-1.2.0.tar", last modified: Wed Aug  2 13:55:16 2023, max compression
```

## Comparing `FindMyIP-1.1.1.tar` & `FindMyIP-1.2.0.tar`

### file list

```diff
@@ -1,12 +1,11 @@
-drwxrwxrwx   0        0        0        0 2021-05-11 09:15:36.065703 FindMyIP-1.1.1/
-drwxrwxrwx   0        0        0        0 2021-05-11 09:15:36.065703 FindMyIP-1.1.1/FindMyIP.egg-info/
--rw-rw-rw-   0        0        0     1729 2021-05-11 09:15:35.000000 FindMyIP-1.1.1/FindMyIP.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      170 2021-05-11 09:15:35.000000 FindMyIP-1.1.1/FindMyIP.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-05-11 09:15:35.000000 FindMyIP-1.1.1/FindMyIP.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2021-05-11 09:15:35.000000 FindMyIP-1.1.1/FindMyIP.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      909 2021-05-11 07:22:05.000000 FindMyIP-1.1.1/FindMyIP.py
--rw-rw-rw-   0        0        0     1729 2021-05-11 09:15:36.065703 FindMyIP-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      956 2021-05-11 09:13:43.000000 FindMyIP-1.1.1/README.md
--rw-rw-rw-   0        0        0       75 2021-05-11 09:14:25.000000 FindMyIP-1.1.1/__init__.py
--rw-rw-rw-   0        0        0       42 2021-05-11 09:15:36.065703 FindMyIP-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      731 2021-05-11 09:14:12.000000 FindMyIP-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 13:55:16.513903 FindMyIP-1.2.0/
+drwxrwxrwx   0        0        0        0 2023-08-02 13:55:16.498255 FindMyIP-1.2.0/FindMyIP.egg-info/
+-rw-rw-rw-   0        0        0     3051 2023-08-02 13:55:16.000000 FindMyIP-1.2.0/FindMyIP.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      168 2023-08-02 13:55:16.000000 FindMyIP-1.2.0/FindMyIP.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 13:55:16.000000 FindMyIP-1.2.0/FindMyIP.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-08-02 13:55:16.000000 FindMyIP-1.2.0/FindMyIP.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1526 2023-08-02 13:19:57.000000 FindMyIP-1.2.0/FindMyIP.py
+-rw-rw-rw-   0        0        0     3051 2023-08-02 13:55:16.513903 FindMyIP-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2682 2023-08-02 13:21:03.000000 FindMyIP-1.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-02 13:55:16.513903 FindMyIP-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      728 2023-08-02 13:55:08.000000 FindMyIP-1.2.0/setup.py
```

### Comparing `FindMyIP-1.1.1/setup.py` & `FindMyIP-1.2.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="FindMyIP",
-    packages=["."],
-    version="1.1.1",
-    description="Find your IP address (both internal(local) and external) or check your connection status.",
+    version="1.2.0",
+    scripts=["FindMyIP.py"],
+    description="Find your IP address (both internal and external) or check your connection state.",
     long_description=README,
     long_description_content_type="text/markdown",
-    url="https://github.com/Mehran-Seifalinia/Find-Your-IP",
+    url="https://github.com/Mehran-Seifalinia/FindMyIP",
     author="Mehran Seifalinia",
     author_email="mehran.seifalinia@gmail.com",
     classifiers=[
         "Programming Language :: Python :: 3",
     ],
 )
```

