# Comparing `tmp/PythonPackageUpdateChecker-1.0.11.tar.gz` & `tmp/PythonPackageUpdateChecker-1.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PythonPackageUpdateChecker-1.0.11.tar", last modified: Wed Aug  2 04:24:29 2023, max compression
+gzip compressed data, was "PythonPackageUpdateChecker-1.0.12.tar", last modified: Wed Aug  2 17:14:50 2023, max compression
```

## Comparing `PythonPackageUpdateChecker-1.0.11.tar` & `PythonPackageUpdateChecker-1.0.12.tar`

### file list

```diff
@@ -1,16 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 04:24:29.969285 PythonPackageUpdateChecker-1.0.11/
--rw-rw-rw-   0        0        0     1091 2023-07-31 14:52:03.000000 PythonPackageUpdateChecker-1.0.11/LICENSE.txt
--rw-rw-rw-   0        0        0     2451 2023-08-02 04:24:29.969285 PythonPackageUpdateChecker-1.0.11/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-02 04:24:29.949845 PythonPackageUpdateChecker-1.0.11/PythonPackageUpdateChecker/
--rw-rw-rw-   0        0        0        0 2023-08-02 04:17:52.000000 PythonPackageUpdateChecker-1.0.11/PythonPackageUpdateChecker/__init__.py
--rw-rw-rw-   0        0        0     5976 2023-08-02 04:19:38.000000 PythonPackageUpdateChecker-1.0.11/PythonPackageUpdateChecker/__main__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 04:24:29.968287 PythonPackageUpdateChecker-1.0.11/PythonPackageUpdateChecker.egg-info/
--rw-rw-rw-   0        0        0     2451 2023-08-02 04:24:29.000000 PythonPackageUpdateChecker-1.0.11/PythonPackageUpdateChecker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      410 2023-08-02 04:24:29.000000 PythonPackageUpdateChecker-1.0.11/PythonPackageUpdateChecker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 04:24:29.000000 PythonPackageUpdateChecker-1.0.11/PythonPackageUpdateChecker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       83 2023-08-02 04:24:29.000000 PythonPackageUpdateChecker-1.0.11/PythonPackageUpdateChecker.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       32 2023-08-02 04:24:29.000000 PythonPackageUpdateChecker-1.0.11/PythonPackageUpdateChecker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-08-02 04:24:29.000000 PythonPackageUpdateChecker-1.0.11/PythonPackageUpdateChecker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1382 2023-07-31 14:52:04.000000 PythonPackageUpdateChecker-1.0.11/README.md
--rw-rw-rw-   0        0        0       42 2023-08-02 04:24:29.969285 PythonPackageUpdateChecker-1.0.11/setup.cfg
--rw-rw-rw-   0        0        0     1754 2023-08-02 04:24:04.000000 PythonPackageUpdateChecker-1.0.11/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:14:50.563303 PythonPackageUpdateChecker-1.0.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-02 17:14:29.000000 PythonPackageUpdateChecker-1.0.12/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-08-02 17:14:50.563303 PythonPackageUpdateChecker-1.0.12/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:14:50.563303 PythonPackageUpdateChecker-1.0.12/PythonPackageUpdateChecker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-08-02 17:14:50.000000 PythonPackageUpdateChecker-1.0.12/PythonPackageUpdateChecker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-02 17:14:50.000000 PythonPackageUpdateChecker-1.0.12/PythonPackageUpdateChecker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 17:14:50.000000 PythonPackageUpdateChecker-1.0.12/PythonPackageUpdateChecker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-02 17:14:50.000000 PythonPackageUpdateChecker-1.0.12/PythonPackageUpdateChecker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 17:14:50.000000 PythonPackageUpdateChecker-1.0.12/PythonPackageUpdateChecker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 17:14:50.000000 PythonPackageUpdateChecker-1.0.12/PythonPackageUpdateChecker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-08-02 17:14:29.000000 PythonPackageUpdateChecker-1.0.12/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 17:14:50.563303 PythonPackageUpdateChecker-1.0.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-08-02 17:14:29.000000 PythonPackageUpdateChecker-1.0.12/setup.py
```

### Comparing `PythonPackageUpdateChecker-1.0.11/PKG-INFO` & `PythonPackageUpdateChecker-1.0.12/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,73 +1,79 @@
-Metadata-Version: 2.1
-Name: PythonPackageUpdateChecker
-Version: 1.0.11
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
-- https://www.linkedin.com/in/andriibohachev/
+Metadata-Version: 2.1
+Name: PythonPackageUpdateChecker
+Version: 1.0.12
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
+"# PythonPackageUpdateChecker"
```

### Comparing `PythonPackageUpdateChecker-1.0.11/PythonPackageUpdateChecker.egg-info/PKG-INFO` & `PythonPackageUpdateChecker-1.0.12/PythonPackageUpdateChecker.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,73 +1,79 @@
-Metadata-Version: 2.1
-Name: PythonPackageUpdateChecker
-Version: 1.0.11
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
-- https://www.linkedin.com/in/andriibohachev/
+Metadata-Version: 2.1
+Name: PythonPackageUpdateChecker
+Version: 1.0.12
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
+"# PythonPackageUpdateChecker"
```

### Comparing `PythonPackageUpdateChecker-1.0.11/README.md` & `PythonPackageUpdateChecker-1.0.12/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,50 +1,56 @@
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
-- https://www.linkedin.com/in/andriibohachev/
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
+"# PythonPackageUpdateChecker"
```

### Comparing `PythonPackageUpdateChecker-1.0.11/setup.py` & `PythonPackageUpdateChecker-1.0.12/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-from setuptools import setup, find_packages
-
-# Зчитуємо вміст файлу README.md
-with open("README.md", "r", encoding="utf-8") as f:
-    long_description = f.read()
-
-setup(
-    name="PythonPackageUpdateChecker",
-    version="1.0.11",
-    description="A utility to automatically check for updates of installed Python packages and update them to the latest versions.",
-    long_description=long_description,
-    # Вказуємо тип контенту для README.md
-    long_description_content_type="text/markdown",
-    author="Andrii Bohachev",
-    author_email="andriybogachev@gmail.com",
-    packages=find_packages(),
-    install_requires=["setuptools", "aiohttp", "tqdm", "asyncio"],
-    entry_points={
-        "console_scripts": [
-            "pythonpackageupdatechecker = PythonPackageUpdateChecker:__main__"
-        ]
-    },
-    classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        "Intended Audience :: Developers",
-        "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Operating System :: OS Independent",
-    ],
-    # exclude_package_data={"": ["subprocess", "winsound", "pkg_resources"]},
-    python_requires=">=3.6",
-    keywords="python package update checker utility async aiohttp",
-    project_urls={
-        "Source": "https://github.com/andriybogachev/PythonPackageUpdateChecker",
-        "Bug Reports": "https://github.com/andriybogachev/PythonPackageUpdateChecker/issues",
-    },
-    license="MIT",
-)
+from setuptools import setup, find_packages
+
+# Зчитуємо вміст файлу README.md
+with open("README.md", "r", encoding="utf-8") as f:
+    long_description = f.read()
+
+setup(
+    name="PythonPackageUpdateChecker",
+    version="1.0.12",
+    description="A utility to automatically check for updates of installed Python packages and update them to the latest versions.",
+    long_description=long_description,
+    # Вказуємо тип контенту для README.md
+    long_description_content_type="text/markdown",
+    author="Andrii Bohachev",
+    author_email="andriybogachev@gmail.com",
+    packages=find_packages(),
+    install_requires=["setuptools", "aiohttp", "tqdm", "asyncio"],
+    entry_points={
+        "console_scripts": [
+            "pythonpackageupdatechecker = PythonPackageUpdateChecker.__main__"
+        ]
+    },
+    classifiers=[
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Operating System :: OS Independent",
+    ],
+    # exclude_package_data={"": ["subprocess", "winsound", "pkg_resources"]},
+    python_requires=">=3.6",
+    keywords="python package update checker utility async aiohttp",
+    project_urls={
+        "Source": "https://github.com/andriybogachev/PythonPackageUpdateChecker",
+        "Bug Reports": "https://github.com/andriybogachev/PythonPackageUpdateChecker/issues",
+    },
+    license="MIT",
+)
```

