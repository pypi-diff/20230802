# Comparing `tmp/simpleWebBrowsing-0.2.0.tar.gz` & `tmp/simpleWebBrowsing-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpleWebBrowsing-0.2.0.tar", last modified: Wed Feb 15 21:08:22 2023, max compression
+gzip compressed data, was "simpleWebBrowsing-0.3.0.tar", last modified: Tue Aug  1 22:32:25 2023, max compression
```

## Comparing `simpleWebBrowsing-0.2.0.tar` & `simpleWebBrowsing-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-02-15 21:08:22.842574 simpleWebBrowsing-0.2.0/
--rw-rw-rw-   0        0        0      547 2023-02-15 21:08:22.842574 simpleWebBrowsing-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-02-15 21:08:22.842574 simpleWebBrowsing-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      993 2023-02-15 21:08:07.000000 simpleWebBrowsing-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-15 21:08:22.826616 simpleWebBrowsing-0.2.0/simpleWebBrowsing/
--rw-rw-rw-   0        0        0        0 2023-02-15 18:46:32.000000 simpleWebBrowsing-0.2.0/simpleWebBrowsing/__init__.py
--rw-rw-rw-   0        0        0     3292 2023-02-01 21:36:09.000000 simpleWebBrowsing-0.2.0/simpleWebBrowsing/chromeConfig.py
-drwxrwxrwx   0        0        0        0 2023-02-15 21:08:22.838585 simpleWebBrowsing-0.2.0/simpleWebBrowsing/seleniumNew/
--rw-rw-rw-   0        0        0        0 2023-02-15 18:46:32.000000 simpleWebBrowsing-0.2.0/simpleWebBrowsing/seleniumNew/__init__.py
--rw-rw-rw-   0        0        0     1840 2023-02-01 18:59:12.000000 simpleWebBrowsing-0.2.0/simpleWebBrowsing/seleniumNew/chromeNav.py
--rw-rw-rw-   0        0        0     8581 2023-02-15 21:03:43.000000 simpleWebBrowsing-0.2.0/simpleWebBrowsing/seleniumNew/elementsNav.py
-drwxrwxrwx   0        0        0        0 2023-02-15 21:08:22.841585 simpleWebBrowsing-0.2.0/simpleWebBrowsing/seleniumOld/
--rw-rw-rw-   0        0        0        0 2023-02-15 18:46:32.000000 simpleWebBrowsing-0.2.0/simpleWebBrowsing/seleniumOld/__init__.py
--rw-rw-rw-   0        0        0     1831 2023-02-15 19:21:21.000000 simpleWebBrowsing-0.2.0/simpleWebBrowsing/seleniumOld/chromeNav.py
--rw-rw-rw-   0        0        0     8552 2023-02-15 21:03:34.000000 simpleWebBrowsing-0.2.0/simpleWebBrowsing/seleniumOld/elementsNav.py
-drwxrwxrwx   0        0        0        0 2023-02-15 21:08:22.835592 simpleWebBrowsing-0.2.0/simpleWebBrowsing.egg-info/
--rw-rw-rw-   0        0        0      547 2023-02-15 21:08:22.000000 simpleWebBrowsing-0.2.0/simpleWebBrowsing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      536 2023-02-15 21:08:22.000000 simpleWebBrowsing-0.2.0/simpleWebBrowsing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-15 21:08:22.000000 simpleWebBrowsing-0.2.0/simpleWebBrowsing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-02-15 21:08:22.000000 simpleWebBrowsing-0.2.0/simpleWebBrowsing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-02-15 21:08:22.000000 simpleWebBrowsing-0.2.0/simpleWebBrowsing.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 22:32:25.923362 simpleWebBrowsing-0.3.0/
+-rw-rw-rw-   0        0        0      547 2023-08-01 22:32:25.922364 simpleWebBrowsing-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-08-01 22:32:25.923362 simpleWebBrowsing-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      993 2023-08-01 22:31:29.000000 simpleWebBrowsing-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 22:32:25.868509 simpleWebBrowsing-0.3.0/simpleWebBrowsing/
+-rw-rw-rw-   0        0        0        0 2023-02-15 18:46:32.000000 simpleWebBrowsing-0.3.0/simpleWebBrowsing/__init__.py
+-rw-rw-rw-   0        0        0     5000 2023-08-01 22:31:34.000000 simpleWebBrowsing-0.3.0/simpleWebBrowsing/chromeConfig.py
+drwxrwxrwx   0        0        0        0 2023-08-01 22:32:25.903415 simpleWebBrowsing-0.3.0/simpleWebBrowsing/seleniumNew/
+-rw-rw-rw-   0        0        0        0 2023-02-15 18:46:32.000000 simpleWebBrowsing-0.3.0/simpleWebBrowsing/seleniumNew/__init__.py
+-rw-rw-rw-   0        0        0     1840 2023-02-01 18:59:12.000000 simpleWebBrowsing-0.3.0/simpleWebBrowsing/seleniumNew/chromeNav.py
+-rw-rw-rw-   0        0        0     8581 2023-02-15 21:03:43.000000 simpleWebBrowsing-0.3.0/simpleWebBrowsing/seleniumNew/elementsNav.py
+drwxrwxrwx   0        0        0        0 2023-08-01 22:32:25.921367 simpleWebBrowsing-0.3.0/simpleWebBrowsing/seleniumOld/
+-rw-rw-rw-   0        0        0        0 2023-02-15 18:46:32.000000 simpleWebBrowsing-0.3.0/simpleWebBrowsing/seleniumOld/__init__.py
+-rw-rw-rw-   0        0        0     1831 2023-02-15 19:21:21.000000 simpleWebBrowsing-0.3.0/simpleWebBrowsing/seleniumOld/chromeNav.py
+-rw-rw-rw-   0        0        0     8552 2023-02-15 21:03:34.000000 simpleWebBrowsing-0.3.0/simpleWebBrowsing/seleniumOld/elementsNav.py
+drwxrwxrwx   0        0        0        0 2023-08-01 22:32:25.885463 simpleWebBrowsing-0.3.0/simpleWebBrowsing.egg-info/
+-rw-rw-rw-   0        0        0      547 2023-08-01 22:32:25.000000 simpleWebBrowsing-0.3.0/simpleWebBrowsing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      536 2023-08-01 22:32:25.000000 simpleWebBrowsing-0.3.0/simpleWebBrowsing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 22:32:25.000000 simpleWebBrowsing-0.3.0/simpleWebBrowsing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-08-01 22:32:25.000000 simpleWebBrowsing-0.3.0/simpleWebBrowsing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-08-01 22:32:25.000000 simpleWebBrowsing-0.3.0/simpleWebBrowsing.egg-info/top_level.txt
```

### Comparing `simpleWebBrowsing-0.2.0/PKG-INFO` & `simpleWebBrowsing-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpleWebBrowsing
-Version: 0.2.0
+Version: 0.3.0
 Summary: Pacote Facilitador Para Manipulação Web
 Author: Marco Rocha
 Author-email: <marco.rocha2@outlook.com>
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `simpleWebBrowsing-0.2.0/setup.py` & `simpleWebBrowsing-0.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.2.0' 
+VERSION = '0.3.0' 
 DESCRIPTION = 'Pacote Facilitador Para Manipulação Web'
 LONG_DESCRIPTION = 'Pacote Facilitador Para Manipulação Web'
 
 # Setting up
 setup(
        # 'name' deve corresponder ao nome da pasta 'verysimplemodule'
         name="simpleWebBrowsing",
```

### Comparing `simpleWebBrowsing-0.2.0/simpleWebBrowsing/chromeConfig.py` & `simpleWebBrowsing-0.3.0/simpleWebBrowsing/chromeConfig.py`

 * *Files 23% similar despite different names*

```diff
@@ -62,14 +62,56 @@
         options.add_experimental_option('prefs', download)
         options.add_argument("user-data-dir=C:\\Users\\" + user + "\\AppData\\Local\\Google\\Chrome\\User Data\\" + diretorioUserChrome)
         options.add_argument("--start-maximized")
 
         driver = webdriver.Chrome(service=Service(ChromeDriverManager().install()), chrome_options=options)
     
         return driver
+    
+    def setupChromeNew(download_directory, process_name, chromedriver_automatico, chromedriver_directory):
+        print('[Chrome] Realizando a configuração do driver no chrome!')
+        print('')
+
+        user = getpass.getuser()
+        chrome_user_data_dir = f"C:\\Users\\{user}\\AppData\\Local\\Google\\Chrome\\User Data\\{process_name}"
+
+        download = {'download.default_directory' : download_directory}
+
+        options = webdriver.ChromeOptions()
+        options.add_experimental_option('excludeSwitches', ['enable-logging'])
+        options.add_experimental_option('prefs', download)
+        options.add_argument("--disable-notifications")
+        options.add_argument("--disable-infobars")
+        options.add_argument("--disable-popup-blocking")
+        options.add_argument(f"user-data-dir={chrome_user_data_dir}")
+        options.add_argument("--start-maximized")
+
+        if chromedriver_automatico == "N":
+            chrome_drive = chromedriver_directory + "\\chromedriver.exe"
+            driver = webdriver.Chrome(executable_path=chrome_drive, options=options)
+        else:
+            driver = webdriver.Chrome(service=Service(ChromeDriverManager().install()), chrome_options=options)
+    
+        return driver
+    
+    def closeChromeNew(driver, process_name):
+        user = getpass.getuser()
+        chrome_user_data_dir = f"C:\\Users\\{user}\\AppData\\Local\\Google\\Chrome\\User Data\\{process_name}"
+
+        print('')
+        print('[Chrome] Encerrando o navegador Web')
+        print('')
+
+        driver.close()
+        driver.quit()
+
+        try:
+            os.remove(chrome_user_data_dir)
+        except:
+            pass
 
     def closeChrome(driver):
         print('')
         print('[Chrome] Encerrando o navegador Web')
         print('')
 
         driver.close()
```

### Comparing `simpleWebBrowsing-0.2.0/simpleWebBrowsing/seleniumNew/chromeNav.py` & `simpleWebBrowsing-0.3.0/simpleWebBrowsing/seleniumNew/chromeNav.py`

 * *Files identical despite different names*

### Comparing `simpleWebBrowsing-0.2.0/simpleWebBrowsing/seleniumNew/elementsNav.py` & `simpleWebBrowsing-0.3.0/simpleWebBrowsing/seleniumNew/elementsNav.py`

 * *Files identical despite different names*

### Comparing `simpleWebBrowsing-0.2.0/simpleWebBrowsing/seleniumOld/chromeNav.py` & `simpleWebBrowsing-0.3.0/simpleWebBrowsing/seleniumOld/chromeNav.py`

 * *Files identical despite different names*

### Comparing `simpleWebBrowsing-0.2.0/simpleWebBrowsing/seleniumOld/elementsNav.py` & `simpleWebBrowsing-0.3.0/simpleWebBrowsing/seleniumOld/elementsNav.py`

 * *Files identical despite different names*

### Comparing `simpleWebBrowsing-0.2.0/simpleWebBrowsing.egg-info/PKG-INFO` & `simpleWebBrowsing-0.3.0/simpleWebBrowsing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpleWebBrowsing
-Version: 0.2.0
+Version: 0.3.0
 Summary: Pacote Facilitador Para Manipulação Web
 Author: Marco Rocha
 Author-email: <marco.rocha2@outlook.com>
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `simpleWebBrowsing-0.2.0/simpleWebBrowsing.egg-info/SOURCES.txt` & `simpleWebBrowsing-0.3.0/simpleWebBrowsing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

