# Comparing `tmp/PythonPackageUpdateChecker-1.0.13.tar.gz` & `tmp/PythonPackageUpdateChecker-1.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PythonPackageUpdateChecker-1.0.13.tar", last modified: Wed Aug  2 17:59:13 2023, max compression
+gzip compressed data, was "PythonPackageUpdateChecker-1.0.14.tar", last modified: Wed Aug  2 20:14:25 2023, max compression
```

## Comparing `PythonPackageUpdateChecker-1.0.13.tar` & `PythonPackageUpdateChecker-1.0.14.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:59:13.653543 PythonPackageUpdateChecker-1.0.13/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-02 17:59:04.000000 PythonPackageUpdateChecker-1.0.13/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-08-02 17:59:13.653543 PythonPackageUpdateChecker-1.0.13/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:59:13.653543 PythonPackageUpdateChecker-1.0.13/PythonPackageUpdateChecker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-08-02 17:59:13.000000 PythonPackageUpdateChecker-1.0.13/PythonPackageUpdateChecker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-02 17:59:13.000000 PythonPackageUpdateChecker-1.0.13/PythonPackageUpdateChecker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 17:59:13.000000 PythonPackageUpdateChecker-1.0.13/PythonPackageUpdateChecker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-02 17:59:13.000000 PythonPackageUpdateChecker-1.0.13/PythonPackageUpdateChecker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 17:59:13.000000 PythonPackageUpdateChecker-1.0.13/PythonPackageUpdateChecker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 17:59:13.000000 PythonPackageUpdateChecker-1.0.13/PythonPackageUpdateChecker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-08-02 17:59:04.000000 PythonPackageUpdateChecker-1.0.13/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 17:59:13.653543 PythonPackageUpdateChecker-1.0.13/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-08-02 17:59:04.000000 PythonPackageUpdateChecker-1.0.13/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 20:14:25.523270 PythonPackageUpdateChecker-1.0.14/
+-rw-rw-rw-   0        0        0     1071 2023-08-02 15:12:46.000000 PythonPackageUpdateChecker-1.0.14/LICENSE.txt
+-rw-rw-rw-   0        0        0     2604 2023-08-02 20:14:25.523270 PythonPackageUpdateChecker-1.0.14/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-02 20:14:25.522298 PythonPackageUpdateChecker-1.0.14/PythonPackageUpdateChecker.egg-info/
+-rw-rw-rw-   0        0        0     2604 2023-08-02 20:14:25.000000 PythonPackageUpdateChecker-1.0.14/PythonPackageUpdateChecker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2023-08-02 20:14:25.000000 PythonPackageUpdateChecker-1.0.14/PythonPackageUpdateChecker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 20:14:25.000000 PythonPackageUpdateChecker-1.0.14/PythonPackageUpdateChecker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-08-02 20:14:25.000000 PythonPackageUpdateChecker-1.0.14/PythonPackageUpdateChecker.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       32 2023-08-02 20:14:25.000000 PythonPackageUpdateChecker-1.0.14/PythonPackageUpdateChecker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 20:14:25.000000 PythonPackageUpdateChecker-1.0.14/PythonPackageUpdateChecker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1482 2023-08-02 15:12:46.000000 PythonPackageUpdateChecker-1.0.14/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-02 20:14:25.524268 PythonPackageUpdateChecker-1.0.14/setup.cfg
+-rw-rw-rw-   0        0        0     1717 2023-08-02 19:50:18.000000 PythonPackageUpdateChecker-1.0.14/setup.py
```

### Comparing `PythonPackageUpdateChecker-1.0.13/LICENSE.txt` & `PythonPackageUpdateChecker-1.0.14/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PythonPackageUpdateChecker-1.0.13/PKG-INFO` & `PythonPackageUpdateChecker-1.0.14/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,81 +1,78 @@
-Metadata-Version: 2.1
-Name: PythonPackageUpdateChecker
-Version: 1.0.13
-Summary: A utility to automatically check for updates of installed Python packages and update them to the latest versions.
-Author: Andrii Bohachev
-Author-email: andriybogachev@gmail.com
-License: MIT
-Project-URL: Source, https://github.com/andriybogachev/PythonPackageUpdateChecker
-Project-URL: Bug Reports, https://github.com/andriybogachev/PythonPackageUpdateChecker/issues
-Keywords: python package update checker utility async aiohttp
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-# PythonPackageUpdateChecker
-
-PythonPackageUpdateChecker is a utility that allows to automatically check for updates of installed Python packages and update them to the latest versions.
-
-It uses asynchronous requests to PyPI to fetch information about newest versions of packages, compares them to locally installed ones and executes pip commands to update packages if needed.
-
-Progress of update is displayed using tqdm library and overall execution time is measured.
-
-## Usage
-
-To use PythonPackageUpdateChecker, simply run the python script. It will:
-
-- Get local Python packages and versions
-- Fetch latest versions from PyPI asynchronously 
-- Determine which packages need update
-- Display list of outdated packages
-- Update required packages with pip
-- Show progress bars during update
-- Play sound on finish
-- Print total execution time
-
-## Requirements
-
-The following libraries are required:
-
-- pkg_resources
-- subprocess
-- asyncio
-- time
-- aiohttp
-- tqdm
-- winsound
-
-Python 3.6 or later is required.
-
-## License
-
-This project is licensed under the MIT license. See the LICENSE file for details.
-
-## Author
-
-Andrii Bohachev
-
-Email: andriybogachev@gmail.com
-
-Social profiles:
-- https://www.facebook.com/andriybogachev
-- https://github.com/andriybogachev/  
-- https://t.me/starf1re
-<<<<<<< HEAD
-- https://www.linkedin.com/in/andriibohachev/
-=======
-- https://www.linkedin.com/in/andriibohachev/
->>>>>>> 94b7e7e9cd40abf4a8244ba90cfba4359424c9cb
-"# PythonPackageUpdateChecker" 
-"# PythonPackageUpdateChecker" 
-"# PythonPackageUpdateChecker" 
-"# PythonPackageUpdateChecker" 
+Metadata-Version: 2.1
+Name: PythonPackageUpdateChecker
+Version: 1.0.14
+Summary: A utility to automatically check for updates of installed Python packages and update them to the latest versions.
+Author: Andrii Bohachev
+Author-email: andriybogachev@gmail.com
+License: MIT
+Project-URL: Source, https://github.com/andriybogachev/PythonPackageUpdateChecker
+Project-URL: Bug Reports, https://github.com/andriybogachev/PythonPackageUpdateChecker/issues
+Keywords: python package update checker utility async aiohttp
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# PythonPackageUpdateChecker
+
+PythonPackageUpdateChecker is a utility that allows to automatically check for updates of installed Python packages and update them to the latest versions.
+
+It uses asynchronous requests to PyPI to fetch information about newest versions of packages, compares them to locally installed ones and executes pip commands to update packages if needed.
+
+Progress of update is displayed using tqdm library and overall execution time is measured.
+
+## Usage
+
+To use PythonPackageUpdateChecker, simply run the python script. It will:
+
+- Get local Python packages and versions
+- Fetch latest versions from PyPI asynchronously 
+- Determine which packages need update
+- Display list of outdated packages
+- Update required packages with pip
+- Show progress bars during update
+- Play sound on finish
+- Print total execution time
+
+## Requirements
+
+The following libraries are required:
+
+- pkg_resources
+- subprocess
+- asyncio
+- time
+- aiohttp
+- tqdm
+- winsound
+
+Python 3.6 or later is required.
+
+## License
+
+This project is licensed under the MIT license. See the LICENSE file for details.
+
+## Author
+
+Andrii Bohachev
+
+Email: andriybogachev@gmail.com
+
+Social profiles:
+- https://www.facebook.com/andriybogachev
+- https://github.com/andriybogachev/  
+- https://t.me/starf1re
+<<<<<<< HEAD
+- https://www.linkedin.com/in/andriibohachev/
+=======
+- https://www.linkedin.com/in/andriibohachev/
+>>>>>>> 94b7e7e9cd40abf4a8244ba90cfba4359424c9cb
+"# PythonPackageUpdateChecker"
```

### Comparing `PythonPackageUpdateChecker-1.0.13/PythonPackageUpdateChecker.egg-info/PKG-INFO` & `PythonPackageUpdateChecker-1.0.14/PythonPackageUpdateChecker.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,81 +1,78 @@
-Metadata-Version: 2.1
-Name: PythonPackageUpdateChecker
-Version: 1.0.13
-Summary: A utility to automatically check for updates of installed Python packages and update them to the latest versions.
-Author: Andrii Bohachev
-Author-email: andriybogachev@gmail.com
-License: MIT
-Project-URL: Source, https://github.com/andriybogachev/PythonPackageUpdateChecker
-Project-URL: Bug Reports, https://github.com/andriybogachev/PythonPackageUpdateChecker/issues
-Keywords: python package update checker utility async aiohttp
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-# PythonPackageUpdateChecker
-
-PythonPackageUpdateChecker is a utility that allows to automatically check for updates of installed Python packages and update them to the latest versions.
-
-It uses asynchronous requests to PyPI to fetch information about newest versions of packages, compares them to locally installed ones and executes pip commands to update packages if needed.
-
-Progress of update is displayed using tqdm library and overall execution time is measured.
-
-## Usage
-
-To use PythonPackageUpdateChecker, simply run the python script. It will:
-
-- Get local Python packages and versions
-- Fetch latest versions from PyPI asynchronously 
-- Determine which packages need update
-- Display list of outdated packages
-- Update required packages with pip
-- Show progress bars during update
-- Play sound on finish
-- Print total execution time
-
-## Requirements
-
-The following libraries are required:
-
-- pkg_resources
-- subprocess
-- asyncio
-- time
-- aiohttp
-- tqdm
-- winsound
-
-Python 3.6 or later is required.
-
-## License
-
-This project is licensed under the MIT license. See the LICENSE file for details.
-
-## Author
-
-Andrii Bohachev
-
-Email: andriybogachev@gmail.com
-
-Social profiles:
-- https://www.facebook.com/andriybogachev
-- https://github.com/andriybogachev/  
-- https://t.me/starf1re
-<<<<<<< HEAD
-- https://www.linkedin.com/in/andriibohachev/
-=======
-- https://www.linkedin.com/in/andriibohachev/
->>>>>>> 94b7e7e9cd40abf4a8244ba90cfba4359424c9cb
-"# PythonPackageUpdateChecker" 
-"# PythonPackageUpdateChecker" 
-"# PythonPackageUpdateChecker" 
-"# PythonPackageUpdateChecker" 
+Metadata-Version: 2.1
+Name: PythonPackageUpdateChecker
+Version: 1.0.14
+Summary: A utility to automatically check for updates of installed Python packages and update them to the latest versions.
+Author: Andrii Bohachev
+Author-email: andriybogachev@gmail.com
+License: MIT
+Project-URL: Source, https://github.com/andriybogachev/PythonPackageUpdateChecker
+Project-URL: Bug Reports, https://github.com/andriybogachev/PythonPackageUpdateChecker/issues
+Keywords: python package update checker utility async aiohttp
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# PythonPackageUpdateChecker
+
+PythonPackageUpdateChecker is a utility that allows to automatically check for updates of installed Python packages and update them to the latest versions.
+
+It uses asynchronous requests to PyPI to fetch information about newest versions of packages, compares them to locally installed ones and executes pip commands to update packages if needed.
+
+Progress of update is displayed using tqdm library and overall execution time is measured.
+
+## Usage
+
+To use PythonPackageUpdateChecker, simply run the python script. It will:
+
+- Get local Python packages and versions
+- Fetch latest versions from PyPI asynchronously 
+- Determine which packages need update
+- Display list of outdated packages
+- Update required packages with pip
+- Show progress bars during update
+- Play sound on finish
+- Print total execution time
+
+## Requirements
+
+The following libraries are required:
+
+- pkg_resources
+- subprocess
+- asyncio
+- time
+- aiohttp
+- tqdm
+- winsound
+
+Python 3.6 or later is required.
+
+## License
+
+This project is licensed under the MIT license. See the LICENSE file for details.
+
+## Author
+
+Andrii Bohachev
+
+Email: andriybogachev@gmail.com
+
+Social profiles:
+- https://www.facebook.com/andriybogachev
+- https://github.com/andriybogachev/  
+- https://t.me/starf1re
+<<<<<<< HEAD
+- https://www.linkedin.com/in/andriibohachev/
+=======
+- https://www.linkedin.com/in/andriibohachev/
+>>>>>>> 94b7e7e9cd40abf4a8244ba90cfba4359424c9cb
+"# PythonPackageUpdateChecker"
```

### Comparing `PythonPackageUpdateChecker-1.0.13/README.md` & `PythonPackageUpdateChecker-1.0.14/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -49,10 +49,7 @@
 - https://t.me/starf1re
 <<<<<<< HEAD
 - https://www.linkedin.com/in/andriibohachev/
 =======
 - https://www.linkedin.com/in/andriibohachev/
 >>>>>>> 94b7e7e9cd40abf4a8244ba90cfba4359424c9cb
 "# PythonPackageUpdateChecker" 
-"# PythonPackageUpdateChecker" 
-"# PythonPackageUpdateChecker" 
-"# PythonPackageUpdateChecker"
```

### Comparing `PythonPackageUpdateChecker-1.0.13/setup.py` & `PythonPackageUpdateChecker-1.0.14/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 
 # Зчитуємо вміст файлу README.md
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="PythonPackageUpdateChecker",
-    version="1.0.13",
+    version="1.0.14",
     description="A utility to automatically check for updates of installed Python packages and update them to the latest versions.",
     long_description=long_description,
     # Вказуємо тип контенту для README.md
     long_description_content_type="text/markdown",
     author="Andrii Bohachev",
     author_email="andriybogachev@gmail.com",
     packages=find_packages(),
     install_requires=["setuptools", "aiohttp", "tqdm", "asyncio"],
     entry_points={
         "console_scripts": [
-            "pythonpackageupdatechecker = PythonPackageUpdateChecker.__main__"
+            "pythonpackageupdatechecker = PythonPackageUpdateChecker.__main__:main"
         ]
     },
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
```

