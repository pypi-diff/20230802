# Comparing `tmp/pyIFPNI-0.0.2.tar.gz` & `tmp/pyIFPNI-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyIFPNI-0.0.2.tar", last modified: Tue Aug  1 07:56:18 2023, max compression
+gzip compressed data, was "pyIFPNI-0.0.3.tar", last modified: Wed Aug  2 02:28:19 2023, max compression
```

## Comparing `pyIFPNI-0.0.2.tar` & `pyIFPNI-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 07:56:18.774368 pyIFPNI-0.0.2/
--rw-rw-rw-   0        0        0     1086 2023-08-01 04:06:37.000000 pyIFPNI-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      470 2023-08-01 07:56:18.773369 pyIFPNI-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       53 2023-08-01 04:07:30.000000 pyIFPNI-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 07:56:18.771369 pyIFPNI-0.0.2/pyIFPNI.egg-info/
--rw-rw-rw-   0        0        0      470 2023-08-01 07:56:18.000000 pyIFPNI-0.0.2/pyIFPNI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      189 2023-08-01 07:56:18.000000 pyIFPNI-0.0.2/pyIFPNI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 07:56:18.000000 pyIFPNI-0.0.2/pyIFPNI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-08-01 07:56:18.000000 pyIFPNI-0.0.2/pyIFPNI.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-01 07:56:18.772370 pyIFPNI-0.0.2/pyifpni/
--rw-rw-rw-   0        0        0       47 2023-08-01 07:52:23.000000 pyIFPNI-0.0.2/pyifpni/__init__.py
--rw-rw-rw-   0        0        0    25248 2023-08-01 07:51:09.000000 pyIFPNI-0.0.2/pyifpni/pyifpni.py
--rw-rw-rw-   0        0        0       42 2023-08-01 07:56:18.774368 pyIFPNI-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      649 2023-08-01 07:52:34.000000 pyIFPNI-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 02:28:19.628083 pyIFPNI-0.0.3/
+-rw-rw-rw-   0        0        0     1086 2023-08-01 04:06:37.000000 pyIFPNI-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      470 2023-08-02 02:28:19.610543 pyIFPNI-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       53 2023-08-01 04:07:30.000000 pyIFPNI-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 02:28:19.610543 pyIFPNI-0.0.3/pyIFPNI.egg-info/
+-rw-rw-rw-   0        0        0      470 2023-08-02 02:28:19.000000 pyIFPNI-0.0.3/pyIFPNI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      189 2023-08-02 02:28:19.000000 pyIFPNI-0.0.3/pyIFPNI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 02:28:19.000000 pyIFPNI-0.0.3/pyIFPNI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-08-02 02:28:19.000000 pyIFPNI-0.0.3/pyIFPNI.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-02 02:28:19.610543 pyIFPNI-0.0.3/pyifpni/
+-rw-rw-rw-   0        0        0        2 2023-08-02 02:06:16.000000 pyIFPNI-0.0.3/pyifpni/__init__.py
+-rw-rw-rw-   0        0        0    25401 2023-08-02 02:17:04.000000 pyIFPNI-0.0.3/pyifpni/pyifpni.py
+-rw-rw-rw-   0        0        0       42 2023-08-02 02:28:19.628083 pyIFPNI-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      649 2023-08-02 02:27:49.000000 pyIFPNI-0.0.3/setup.py
```

### Comparing `pyIFPNI-0.0.2/LICENSE` & `pyIFPNI-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyIFPNI-0.0.2/pyifpni/pyifpni.py` & `pyIFPNI-0.0.3/pyifpni/pyifpni.py`

 * *Files 1% similar despite different names*

```diff
@@ -285,15 +285,16 @@
                 tem_item = {}
                 try:
                     tem_item["href"] = self.url_base + item.find("h1").find("a")["href"]
                 except:
                     pass
                 info_res = self.requests3(tem_item["href"])
                 info_soup = BeautifulSoup(info_res.text, 'html.parser')
-                tem_item["IDNAME"] = info_soup.find('div', class_="panel-heading").find_all("span")[-1].text
+                head = info_soup.find("span", class_="input-group-addon label label-info")
+                tem_item[head.text] = head.find_next("span").text
                 dl = info_soup.find("dl", class_="dl-horizontal")
                 for i in dl.find_all("dt"):
                     column_label = i.text.strip()
                     column_value = i.find_next("dd")
                     try:
                         tem_item[column_label] = column_value.text.strip()
                         tem_item[column_label + ' href'] = self.url_base + column_value.find('a')['href']
@@ -379,13 +380,14 @@
             try:
                 res = requests.get(url, headers=self.headers)
                 return res
             except:
                 time.sleep(5)
 
 
-if __name__ == "__main__":
+'''if __name__ == "__main__":
     pyifpni = IFPNI()
-    # pyifpni.supragenus("Orchidaceae", save_to_csv="orchiaceae")
-    # pyifpni.genus("mahonia")
-    # pyifpni.species("achlys")
+    pyifpni.supragenus("Orchidaceae", save_to_csv="orchiaceae")
+    pyifpni.genus("mahonia")
+    pyifpni.species("achlys")
     pyifpni.species("mahonia", save_to_csv="mahonia speices")
+    pyifpni.supragenus("Berberidaceae", first_symbols=True, save_to_csv="Berberidaceae first symbols")'''
```

### Comparing `pyIFPNI-0.0.2/setup.py` & `pyIFPNI-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyIFPNI",
-    version="0.0.2",
+    version="0.0.3",
     author="Bailong Zhao",
     author_email="bailongzhao@163.com",
     description="A package accessing to IFPNI",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/WDragon101/pyIFPNI",
     packages=setuptools.find_packages(),
```

