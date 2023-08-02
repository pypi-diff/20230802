# Comparing `tmp/pyIFPNI-0.0.3.tar.gz` & `tmp/pyIFPNI-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyIFPNI-0.0.3.tar", last modified: Wed Aug  2 02:28:19 2023, max compression
+gzip compressed data, was "pyIFPNI-0.0.4.tar", last modified: Wed Aug  2 04:19:07 2023, max compression
```

## Comparing `pyIFPNI-0.0.3.tar` & `pyIFPNI-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 02:28:19.628083 pyIFPNI-0.0.3/
--rw-rw-rw-   0        0        0     1086 2023-08-01 04:06:37.000000 pyIFPNI-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      470 2023-08-02 02:28:19.610543 pyIFPNI-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       53 2023-08-01 04:07:30.000000 pyIFPNI-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 02:28:19.610543 pyIFPNI-0.0.3/pyIFPNI.egg-info/
--rw-rw-rw-   0        0        0      470 2023-08-02 02:28:19.000000 pyIFPNI-0.0.3/pyIFPNI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      189 2023-08-02 02:28:19.000000 pyIFPNI-0.0.3/pyIFPNI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 02:28:19.000000 pyIFPNI-0.0.3/pyIFPNI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-08-02 02:28:19.000000 pyIFPNI-0.0.3/pyIFPNI.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-02 02:28:19.610543 pyIFPNI-0.0.3/pyifpni/
--rw-rw-rw-   0        0        0        2 2023-08-02 02:06:16.000000 pyIFPNI-0.0.3/pyifpni/__init__.py
--rw-rw-rw-   0        0        0    25401 2023-08-02 02:17:04.000000 pyIFPNI-0.0.3/pyifpni/pyifpni.py
--rw-rw-rw-   0        0        0       42 2023-08-02 02:28:19.628083 pyIFPNI-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      649 2023-08-02 02:27:49.000000 pyIFPNI-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 04:19:07.475621 pyIFPNI-0.0.4/
+-rw-rw-rw-   0        0        0     1086 2023-08-01 04:06:37.000000 pyIFPNI-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      470 2023-08-02 04:19:07.473621 pyIFPNI-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       53 2023-08-01 04:07:30.000000 pyIFPNI-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 04:19:07.471468 pyIFPNI-0.0.4/pyIFPNI.egg-info/
+-rw-rw-rw-   0        0        0      470 2023-08-02 04:19:07.000000 pyIFPNI-0.0.4/pyIFPNI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      189 2023-08-02 04:19:07.000000 pyIFPNI-0.0.4/pyIFPNI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 04:19:07.000000 pyIFPNI-0.0.4/pyIFPNI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-08-02 04:19:07.000000 pyIFPNI-0.0.4/pyIFPNI.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-02 04:19:07.472585 pyIFPNI-0.0.4/pyifpni/
+-rw-rw-rw-   0        0        0        2 2023-08-02 02:06:16.000000 pyIFPNI-0.0.4/pyifpni/__init__.py
+-rw-rw-rw-   0        0        0    25580 2023-08-02 04:15:34.000000 pyIFPNI-0.0.4/pyifpni/pyifpni.py
+-rw-rw-rw-   0        0        0       42 2023-08-02 04:19:07.475621 pyIFPNI-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      649 2023-08-02 04:16:03.000000 pyIFPNI-0.0.4/setup.py
```

### Comparing `pyIFPNI-0.0.3/LICENSE` & `pyIFPNI-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyIFPNI-0.0.3/pyifpni/pyifpni.py` & `pyIFPNI-0.0.4/pyifpni/pyifpni.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,14 +108,15 @@
                             "Xinjiang": 121
                             }
         self.headers = {
             "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) "
                           "Chrome/115.0.0.0 Safari/537.36 Edg/115.0.1901.183"}
         self.result = []
         self.df = None
+        self.name = ""
 
     def set_form(self, name, first_symbols=False, order=None, orderDirection=None, author=None, original_spelling=None,
                  yearFrom=None, yearTo=None, rank_list=None, paleoregion_list=None, journal=None, abbreviation=None):
         """
         :param name: request; str
         :param first_symbols: optional; bool
         :param order: optional; one of ["name", "yearFrom", "title", "titleOrig", "titleAbbr", "lastName"]
@@ -261,17 +262,18 @@
         :param rank_list: optional, list
         :return: url, str
         """
         url = self.execute_URL(lists="supragenus", name=name, first_symbols=first_symbols, order=order,
                                orderDirection=orderDirection,
                                author=author, original_spelling=original_spelling, yearFrom=yearFrom, yearTo=yearTo,
                                rank_list=rank_list)
-        self.execute(url, name, save_to_csv)
+        self.name = name
+        self.execute(url, name)
 
-    def execute(self, url, name, save_to_csv):
+    def execute(self, url, name):
         self.result.clear()
         res = self.requests3(url)
         soup = BeautifulSoup(res.text, 'html.parser')
         total_count_num = soup.find("div", class_="list-group").find("h4").text.split(' ')[-1]
         total_page_num = math.ceil(int(total_count_num) / 10)
         print(f"{name}: There is/are {total_count_num} results found by {self.lists} search in {total_page_num} pages.")
         for page in range(1, total_page_num + 1):
@@ -298,86 +300,96 @@
                     try:
                         tem_item[column_label] = column_value.text.strip()
                         tem_item[column_label + ' href'] = self.url_base + column_value.find('a')['href']
                     except:
                         tem_item[column_label] = column_value.text.strip()
 
                 self.result.append(tem_item)
+
+    def save_to(self, save_to_csv):
         for i in self.result:
             self.df = pd.concat([self.df, pd.DataFrame.from_dict(i, orient="index").T], ignore_index=True)
         if save_to_csv:
             if save_to_csv.endswith(".csv"):
                 self.df.to_csv(save_to_csv)
             else:
                 self.df.to_csv(f"{save_to_csv}.csv")
         else:
-            self.df.to_csv(f"{name}.csv")
+            self.df.to_csv(f"{self.name}.csv")
 
     def genus(self, name, first_symbols=False, order=None, orderDirection=None, author=None, original_spelling=None,
               yearFrom=None, yearTo=None, rank_list=None, save_to_csv=None):
         url = self.execute_URL(lists="genus", name=name, first_symbols=first_symbols, order=order,
                                orderDirection=orderDirection,
                                author=author, original_spelling=original_spelling, yearFrom=yearFrom, yearTo=yearTo,
                                rank_list=rank_list)
-        self.execute(url, name, save_to_csv)
+        self.name = name
+        self.execute(url, name)
 
     def infragenus(self, name, first_symbols=False, order=None, orderDirection=None, author=None,
                    original_spelling=None,
                    yearFrom=None, yearTo=None, rank_list=None, save_to_csv=None):
         url = self.execute_URL(lists="infragenus", name=name, first_symbols=first_symbols, order=order,
                                orderDirection=orderDirection,
                                author=author, original_spelling=original_spelling, yearFrom=yearFrom, yearTo=yearTo,
                                rank_list=rank_list)
-        self.execute(url, name, save_to_csv)
+        self.name = name
+        self.execute(url, name)
 
     def species(self, name, first_symbols=False, order=None, orderDirection=None, author=None, original_spelling=None,
                 yearFrom=None, yearTo=None, rank_list=None, paleoregion_list=None, save_to_csv=None):
         url = self.execute_URL(lists="species", name=name, first_symbols=first_symbols, order=order,
                                orderDirection=orderDirection,
                                author=author, original_spelling=original_spelling, yearFrom=yearFrom, yearTo=yearTo,
                                rank_list=rank_list,
                                paleoregion_list=paleoregion_list)
-        self.execute(url, name, save_to_csv)
+        self.name = name
+        self.execute(url, name)
 
     def infraspecies(self, name, first_symbols=False, order=None, orderDirection=None, author=None,
                      original_spelling=None,
                      yearFrom=None, yearTo=None, rank_list=None, paleoregion_list=None, save_to_csv=None):
         url = self.execute_URL(lists="infraspecies", name=name, first_symbols=first_symbols, order=order,
                                orderDirection=orderDirection,
                                author=author, original_spelling=original_spelling, yearFrom=yearFrom, yearTo=yearTo,
                                rank_list=rank_list,
                                paleoregion_list=paleoregion_list)
-        self.execute(url, name, save_to_csv)
+        self.name = name
+        self.execute(url, name)
 
     def publication(self, title, first_symbols=False, order=None, orderDirection=None, author=None,
                     original_spelling=None,
                     yearFrom=None, yearTo=None, journal=None, save_to_csv=None):
         url = self.execute_URL(lists="publication", name=title, first_symbols=first_symbols, order=order,
                                orderDirection=orderDirection, author=author, original_spelling=original_spelling,
                                yearFrom=yearFrom, yearTo=yearTo, journal=journal)
-        self.execute(url, title, save_to_csv)
+        self.name = title
+        self.execute(url, title)
 
     def book(self, title, first_symbols=False, order=None, orderDirection=None, original_spelling=None,
              abbreviation=None, save_to_csv=None):
         url = self.execute_URL(lists="book", name=title, first_symbols=first_symbols, order=order,
                                orderDirection=orderDirection, original_spelling=original_spelling,
                                abbreviation=abbreviation)
-        self.execute(url, title, save_to_csv)
+        self.name = title
+        self.execute(url, title)
 
     def journal(self, title, first_symbols=False, order=None, orderDirection=None, original_spelling=None,
                 yearFrom=None, yearTo=None, save_to_csv=None):
         url = self.execute_URL(lists="journal", name=title, first_symbols=first_symbols, order=order,
                                orderDirection=orderDirection, original_spelling=original_spelling,
                                yearFrom=yearFrom, yearTo=yearTo)
-        self.execute(url, title, save_to_csv)
+        self.name = title
+        self.execute(url, title)
 
     def author(self, lastName, first_symbols=False, order=None, orderDirection=None, save_to_csv=None):
         url = self.execute_URL(lists="author", name=lastName, first_symbols=first_symbols, order=order,
                                orderDirection=orderDirection)
-        self.execute(url, lastName, save_to_csv)
+        self.name = lastName
+        self.execute(url, lastName)
 
     def requests3(self, url):
         for i in range(3):
             try:
                 res = requests.get(url, headers=self.headers)
                 return res
             except:
```

### Comparing `pyIFPNI-0.0.3/setup.py` & `pyIFPNI-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyIFPNI",
-    version="0.0.3",
+    version="0.0.4",
     author="Bailong Zhao",
     author_email="bailongzhao@163.com",
     description="A package accessing to IFPNI",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/WDragon101/pyIFPNI",
     packages=setuptools.find_packages(),
```

