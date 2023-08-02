# Comparing `tmp/pyIFPNI-0.0.4.tar.gz` & `tmp/pyIFPNI-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyIFPNI-0.0.4.tar", last modified: Wed Aug  2 04:19:07 2023, max compression
+gzip compressed data, was "pyIFPNI-0.0.5.tar", last modified: Wed Aug  2 04:27:20 2023, max compression
```

## Comparing `pyIFPNI-0.0.4.tar` & `pyIFPNI-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 04:19:07.475621 pyIFPNI-0.0.4/
--rw-rw-rw-   0        0        0     1086 2023-08-01 04:06:37.000000 pyIFPNI-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      470 2023-08-02 04:19:07.473621 pyIFPNI-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       53 2023-08-01 04:07:30.000000 pyIFPNI-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 04:19:07.471468 pyIFPNI-0.0.4/pyIFPNI.egg-info/
--rw-rw-rw-   0        0        0      470 2023-08-02 04:19:07.000000 pyIFPNI-0.0.4/pyIFPNI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      189 2023-08-02 04:19:07.000000 pyIFPNI-0.0.4/pyIFPNI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 04:19:07.000000 pyIFPNI-0.0.4/pyIFPNI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-08-02 04:19:07.000000 pyIFPNI-0.0.4/pyIFPNI.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-02 04:19:07.472585 pyIFPNI-0.0.4/pyifpni/
--rw-rw-rw-   0        0        0        2 2023-08-02 02:06:16.000000 pyIFPNI-0.0.4/pyifpni/__init__.py
--rw-rw-rw-   0        0        0    25580 2023-08-02 04:15:34.000000 pyIFPNI-0.0.4/pyifpni/pyifpni.py
--rw-rw-rw-   0        0        0       42 2023-08-02 04:19:07.475621 pyIFPNI-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      649 2023-08-02 04:16:03.000000 pyIFPNI-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 04:27:20.175356 pyIFPNI-0.0.5/
+-rw-rw-rw-   0        0        0     1086 2023-08-01 04:06:37.000000 pyIFPNI-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      470 2023-08-02 04:27:20.175356 pyIFPNI-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       53 2023-08-01 04:07:30.000000 pyIFPNI-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 04:27:20.173349 pyIFPNI-0.0.5/pyIFPNI.egg-info/
+-rw-rw-rw-   0        0        0      470 2023-08-02 04:27:20.000000 pyIFPNI-0.0.5/pyIFPNI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      189 2023-08-02 04:27:20.000000 pyIFPNI-0.0.5/pyIFPNI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 04:27:20.000000 pyIFPNI-0.0.5/pyIFPNI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-08-02 04:27:20.000000 pyIFPNI-0.0.5/pyIFPNI.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-02 04:27:20.174358 pyIFPNI-0.0.5/pyifpni/
+-rw-rw-rw-   0        0        0        2 2023-08-02 02:06:16.000000 pyIFPNI-0.0.5/pyifpni/__init__.py
+-rw-rw-rw-   0        0        0    25584 2023-08-02 04:27:09.000000 pyIFPNI-0.0.5/pyifpni/pyifpni.py
+-rw-rw-rw-   0        0        0       42 2023-08-02 04:27:20.175356 pyIFPNI-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      649 2023-08-02 04:27:09.000000 pyIFPNI-0.0.5/setup.py
```

### Comparing `pyIFPNI-0.0.4/LICENSE` & `pyIFPNI-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyIFPNI-0.0.4/pyifpni/pyifpni.py` & `pyIFPNI-0.0.5/pyifpni/pyifpni.py`

 * *Files 0% similar despite different names*

```diff
@@ -300,18 +300,18 @@
                     try:
                         tem_item[column_label] = column_value.text.strip()
                         tem_item[column_label + ' href'] = self.url_base + column_value.find('a')['href']
                     except:
                         tem_item[column_label] = column_value.text.strip()
 
                 self.result.append(tem_item)
-
-    def save_to(self, save_to_csv):
         for i in self.result:
             self.df = pd.concat([self.df, pd.DataFrame.from_dict(i, orient="index").T], ignore_index=True)
+
+    def save_to_csv(self, save_to_csv):
         if save_to_csv:
             if save_to_csv.endswith(".csv"):
                 self.df.to_csv(save_to_csv)
             else:
                 self.df.to_csv(f"{save_to_csv}.csv")
         else:
             self.df.to_csv(f"{self.name}.csv")
```

### Comparing `pyIFPNI-0.0.4/setup.py` & `pyIFPNI-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyIFPNI",
-    version="0.0.4",
+    version="0.0.5",
     author="Bailong Zhao",
     author_email="bailongzhao@163.com",
     description="A package accessing to IFPNI",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/WDragon101/pyIFPNI",
     packages=setuptools.find_packages(),
```

