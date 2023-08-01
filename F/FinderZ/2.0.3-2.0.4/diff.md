# Comparing `tmp/finderz-2.0.3.tar.gz` & `tmp/finderz-2.0.4.tar.gz`

## Comparing `finderz-2.0.3.tar` & `finderz-2.0.4.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 finderz-2.0.3/.DS_Store
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 finderz-2.0.3/.readthedocs.yaml
--rw-r--r--   0        0        0     9965 2020-02-02 00:00:00.000000 finderz-2.0.3/docs/code structure.rst
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 finderz-2.0.3/docs/conf.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 finderz-2.0.3/docs/credits.rst
--rw-r--r--   0        0        0    28295 2020-02-02 00:00:00.000000 finderz-2.0.3/docs/function use.rst
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 finderz-2.0.3/docs/index.rst
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 finderz-2.0.3/docs/installation.rst
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 finderz-2.0.3/docs/updatev2.rst
--rw-r--r--   0        0        0   478505 2020-02-02 00:00:00.000000 finderz-2.0.3/docs/img/logo-color.jpg
--rw-r--r--   0        0        0   478505 2020-02-02 00:00:00.000000 finderz-2.0.3/logo/logo-color.jpg
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 finderz-2.0.3/old/src/.DS_Store
--rw-r--r--   0        0        0     9710 2020-02-02 00:00:00.000000 finderz-2.0.3/old/src/FinderZ/FinderZLib.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 finderz-2.0.3/old/src/FinderZ/__init__.py
--rw-r--r--   0        0        0    48940 2020-02-02 00:00:00.000000 finderz-2.0.3/src/FinderZ/FinderZV2.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 finderz-2.0.3/src/FinderZ/__init__.py
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 finderz-2.0.3/tests/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 finderz-2.0.3/tests/updates/.DS_Store
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 finderz-2.0.3/tests/updates/V2 Changelog.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 finderz-2.0.3/tests/updates/bash.sh
--rw-r--r--   0        0        0    15152 2020-02-02 00:00:00.000000 finderz-2.0.3/tests/updates/parentFunctions.py
--rw-r--r--   0        0        0     3478 2020-02-02 00:00:00.000000 finderz-2.0.3/tests/updates/update.py
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 finderz-2.0.3/LICENSE
--rw-r--r--   0        0        0     4330 2020-02-02 00:00:00.000000 finderz-2.0.3/README.md
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 finderz-2.0.3/pyproject.toml
--rw-r--r--   0        0        0     5110 2020-02-02 00:00:00.000000 finderz-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 finderz-2.0.4/.DS_Store
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 finderz-2.0.4/.readthedocs.yaml
+-rw-r--r--   0        0        0    10265 2020-02-02 00:00:00.000000 finderz-2.0.4/docs/code structure.rst
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 finderz-2.0.4/docs/conf.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 finderz-2.0.4/docs/credits.rst
+-rw-r--r--   0        0        0    28707 2020-02-02 00:00:00.000000 finderz-2.0.4/docs/function use.rst
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 finderz-2.0.4/docs/index.rst
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 finderz-2.0.4/docs/installation.rst
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 finderz-2.0.4/docs/updatev2.rst
+-rw-r--r--   0        0        0   478505 2020-02-02 00:00:00.000000 finderz-2.0.4/docs/img/logo-color.jpg
+-rw-r--r--   0        0        0   478505 2020-02-02 00:00:00.000000 finderz-2.0.4/logo/logo-color.jpg
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 finderz-2.0.4/old/src/.DS_Store
+-rw-r--r--   0        0        0     9710 2020-02-02 00:00:00.000000 finderz-2.0.4/old/src/FinderZ/FinderZLib.py
+-rw-r--r--   0        0        0    48940 2020-02-02 00:00:00.000000 finderz-2.0.4/old/src/FinderZ/FinderZV2.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 finderz-2.0.4/old/src/FinderZ/__init__.py
+-rw-r--r--   0        0        0    49539 2020-02-02 00:00:00.000000 finderz-2.0.4/src/FinderZ/FinderZV2.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 finderz-2.0.4/src/FinderZ/__init__.py
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 finderz-2.0.4/tests/.DS_Store
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 finderz-2.0.4/tests/updates/.DS_Store
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 finderz-2.0.4/tests/updates/V2 Changelog.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 finderz-2.0.4/tests/updates/bash.sh
+-rw-r--r--   0        0        0    15152 2020-02-02 00:00:00.000000 finderz-2.0.4/tests/updates/parentFunctions.py
+-rw-r--r--   0        0        0     3478 2020-02-02 00:00:00.000000 finderz-2.0.4/tests/updates/update.py
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 finderz-2.0.4/LICENSE
+-rw-r--r--   0        0        0     5589 2020-02-02 00:00:00.000000 finderz-2.0.4/README.md
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 finderz-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0     6369 2020-02-02 00:00:00.000000 finderz-2.0.4/PKG-INFO
```

### Comparing `finderz-2.0.3/.DS_Store` & `finderz-2.0.4/.DS_Store`

 * *Files identical despite different names*

### Comparing `finderz-2.0.3/docs/code structure.rst` & `finderz-2.0.4/docs/code structure.rst`

 * *Files 0% similar despite different names*

```diff
@@ -76,14 +76,18 @@
 The ``getTotalInfo`` Function:
 ------------------------------
 
 This function works by intancing two variables, one for file lines, and another for files. Its purpose is to rescurisvely go through every file in a directory and scan the amount of lines it has. It then returns that amount, and also can return the total amount of files that it iterated through.
 
 Thanks to the os.walk() function, recusrive actions are very easy to do, which what makes this possible along with many other recursive actions within other functions.
 
+The ``compareFiles`` Function:
+------------------------------
+
+This function works by iterating through an enumeration of two lists (one containing the contents of a file, and the other list containing the contents of another file). It gathers the difference in each line (if there is a difference).
 
 The **fileOperands** class
 ==========================
 
 The **fileOperands** class is the main class that contains many useful functions for various file operations. In V2, so many new things are added and fixed. Go check out the :doc:`updatev2` for more information on the V2 update of FinderZ!
 
 * findFiles
```

### Comparing `finderz-2.0.3/docs/conf.py` & `finderz-2.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `finderz-2.0.3/docs/function use.rst` & `finderz-2.0.4/docs/function use.rst`

 * *Files 0% similar despite different names*

```diff
@@ -232,14 +232,25 @@
     lines, files = GatherInfo.getTotalInfo('pattern', 'string', returnFileAmount = True, extensionFilters = ['.py'], recursive = True) #Replace pattern with a valid regex pattern.
     print(lines, files)
 
 The above code takes in .py (python files) only, as we have added .py in the file extension filter list. **Keep in mind, you can add as many extensionFilters as you want** which is why it is in the form of a list.
 
 The recursive option is set to true, so it will scan every (Python) file recursively in each directory, and files are returned with the returnFileAmount parameter set to True.
 
+``compareFiles``
+----------------
+
+This function can used in order to compare two files and what differences they have in their contents.
+
+.. code-block:: python
+
+    diff_lines = GatherInfo.compareFiles('/path/to/file', '/path/to/file2', comparison_output_file = '/path/to/comparison_file')
+
+The comparison file is a file to write to when the whole comparison process is done. This is completely optional.
+
 **fileOperands** Usage
 ======================
 
 The **fileOperands** class contains the biggest functions in the library. These functions are special functions which can be of use fo many users.
 
 ``findFiles``
 -------------
@@ -467,14 +478,15 @@
 
     The **Synchronize** class really only has one function that the user uses in order to use the synchronization properly. Although it is only one function, it is very complex (not to use, but rather how it works). Because of this, only the ``synchronize`` function will be explained here.
 
 ``synchronize``
 ---------------
 
 **IMPORTANT NOTE**
+
 .. note::
 
     Before using these functions, do keep in mind: It is highly dangerous to rename a directory or file as the last thing to do if you did other actions before (such as add files/dirs). This could lead to data loss! You should synchronize every time you add, remove, etc. something. 
 
 The ``synchronize`` function is a very complex function that the user can however use with ease. The main purpose of this function is to take in two directories, and synchronize them and their files.
 
 First, lets take a look at the features:
@@ -503,17 +515,18 @@
 The importantFilesFlag is a character that you as the user can use to mark certain files as important. This is explained under the features right above.
 
 For example, if the importantFilesFlag is left to a default (which is an underscore), an important file would look like this:::
 
     _importantFile.txt
 
 **IMPORTANT NOTE**
+
 .. note::
 
-    Concerning the sync backup folder, it is totally recommended that you use it. PLEASE NOTE: IF YOU RUN THE SYNCHRONIZATION FOR THE FIRST TIME, RUN THE FIRST TIME WITH THE SYNCBACKUPFOLDER SET TO TRUE. This is to prevent initial data loss! As stated before, I am not responsible for any data lost. Initially, to learn how this works, use the backup folder to prevent data loss! You an disable it by putting the parameter to False, if you really need to.
+    Concerning the sync backup folder, it is totally recommended that you use it. PLEASE NOTE: IF YOU RUN THE SYNCHRONIZATION FOR THE FIRST TIME, RUN THE FIRST TIME WITH THE SYNCBACKUPFOLDER SET TO TRUE. This is to prevent initial data loss! As stated before, I am not responsible for any data lost. Initially, to learn how this works, use the backup folder to prevent data loss! You can disable it by putting the parameter to False, if you really need to.
 
     PLEASE KEEP IN MIND: If you have dir1 and dir2, and you have a folder in dir1 but dir2 is empty (or viceversa), and then, renaming dir2 is the last thing you do, you could risk data loss, as the function will think you want to delete the folder from dir1 (because dir2 was the last one modified)
 
 
 The sync backup folder will always be marked with the important files flag so that it isn't accidentally removed. If the importantFilesFlag is left to its default value of an underscore, the sync backup folder would look like this:::
 
     _syncBackups
@@ -567,17 +580,17 @@
 The ``backgroundBackup`` function is basically the same thing as ``backup``, but it actually goes in the background. It has an extra optional (default = 8) refreshInterval parameter, which defines the interval (in seconds) for each backup.
 
 You can leave this in the background running and it will backup every time the refreshInterval strikes again.
 
 
 .. note::
 
-    It is reccomended that you use logs in order to prevent data loss. Logs help you (and me) figure out what went wrong or what you can do to retreive the file back/ what happened during a specific process.
+    It is recommended that you use logs in order to prevent data loss. Logs help you (and me) figure out what went wrong or what you can do to retreive the file back/ what happened during a specific process.
 
 
 **callBash** Usage
 ==================
 
 ``runFile``
 -----------
 
-This function can simply be used to run a shell script. It takes in one required parameter, the path to the shell script, and has an optional parameter to edit the permissions of the file to avoid executable issues.
+This function can simply be used to run a shell script. It takes in one required parameter, the path to the shell script, and has an optional parameter to edit the permissions of the file to avoid executable issues.
```

### Comparing `finderz-2.0.3/docs/index.rst` & `finderz-2.0.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `finderz-2.0.3/docs/updatev2.rst` & `finderz-2.0.4/docs/updatev2.rst`

 * *Files identical despite different names*

### Comparing `finderz-2.0.3/docs/img/logo-color.jpg` & `finderz-2.0.4/docs/img/logo-color.jpg`

 * *Files identical despite different names*

### Comparing `finderz-2.0.3/logo/logo-color.jpg` & `finderz-2.0.4/logo/logo-color.jpg`

 * *Files identical despite different names*

### Comparing `finderz-2.0.3/old/src/.DS_Store` & `finderz-2.0.4/old/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `finderz-2.0.3/old/src/FinderZ/FinderZLib.py` & `finderz-2.0.4/old/src/FinderZ/FinderZLib.py`

 * *Files identical despite different names*

### Comparing `finderz-2.0.3/src/FinderZ/FinderZV2.py` & `finderz-2.0.4/old/src/FinderZ/FinderZV2.py`

 * *Files identical despite different names*

### Comparing `finderz-2.0.3/tests/.DS_Store` & `finderz-2.0.4/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `finderz-2.0.3/tests/updates/.DS_Store` & `finderz-2.0.4/tests/updates/.DS_Store`

 * *Files identical despite different names*

### Comparing `finderz-2.0.3/tests/updates/V2 Changelog.txt` & `finderz-2.0.4/tests/updates/V2 Changelog.txt`

 * *Files identical despite different names*

### Comparing `finderz-2.0.3/tests/updates/parentFunctions.py` & `finderz-2.0.4/tests/updates/parentFunctions.py`

 * *Files identical despite different names*

### Comparing `finderz-2.0.3/tests/updates/update.py` & `finderz-2.0.4/tests/updates/update.py`

 * *Files identical despite different names*

### Comparing `finderz-2.0.3/LICENSE` & `finderz-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `finderz-2.0.3/README.md` & `finderz-2.0.4/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -15,50 +15,65 @@
 	
 </p>
 <p align = "center">
 	<img src="https://static.pepy.tech/badge/finderz"
 		height="23">
 </p>
 
-## **IMPORTANT: ** 
+## IMPORTANT: 
 **V2 is finally out! To check out the details, go to the readthedocs documentation under the update v2 section!**
-**LINK TO READ THE DOCS: [Documentation](https://finderz.readthedocs.io/en/latest/index.html)** 
-**IF YOU WANT TO USE THE SYNCHRONIZATION AND BACKUP CLASSeS, MAKE SURE TO THOROUGHLY READ THE [DOCUMENTATION](https://finderz.readthedocs.io/en/latest/index.html) IN ORDER TO PREVENT DATA LOSS**
+**Documentation: [FinderZ](https://finderz.readthedocs.io/en/latest/index.html)** 
 
+**If you want to use the Synchronization and Backup classes, please read the documentation linked above in order to prevent data loss**
+
+**AND: Huge thank you to [@RichardDally](https://github.com/RichardDally) , [@mikudae](https://github.com/mikudae) , [@kyzsuukii](https://github.com/kyzsuukii) , and [@fablau](github.com/fablau) for starring FinderZ.**
 ## **Written in python, this library provides you with different file operation commands as well as info gathering commands on directories as well as files.** 
 ____________________________________________________________________________
 ## **CHANGELOG: V2.0.0**
 
 To check out the details of V2, go to the [documentation](https://finderz.readthedocs.io/en/latest/index.html). This is a big update with many new things!
 
 
+**Minor Fix Version 2.0.4:**
+- Fixed bug where removing more than one file at a time gave an existence error. Sorry for that!
+- Fixed bug where removing a folder that contained folder with the same name as the sync backup folder would result in an infinite loop of backup folders being created.
+- Minimized logging by making file updating hash-dependent. Now, updating files is marked as a critical (C) action in the log.
+- Removed unnecessary printing in some functions.
+- Added a file comparison function in GatherInfo
+- Currently, after having tested FinderZ on Android, permission errors may occasionally occur. This is likely due to read/write permissions assigned to a specific file.
+
+**Minor Fix Version 2.0.3:**
+- Fixed bug in Backup class that gave an existence error. Sorry about that!
+- I have noticed some accidental printing in some functions (such as findFiles, that prints a boolean at the start). This does not currently affect anything, but just prints out occasional, unnecessary output. This will be fixed very soon.
+- Thank you for 16K Downloads!
+
 ## **Usage**
 Installation:
 ```
 pip3 install FinderZ
 ```
 Importing:
 ```
 import FinderZ
 ```
 
 ## **Features**
-- Consists of three classes: GatherInfo, fileOperands, Synchronize, Backup, and callBash.
+- Consists of five classes: GatherInfo, fileOperands, Synchronize, Backup, and callBash.
 - Advanced file operations, already built for you (including many options to choose from!) 
-- Supports regex operations for some functions, as well as specific filters and multiple other choices to choose from. Options such as exact search or something even just containing a keyword, or even having the option to choose to seaerch recursively, are all included.
-- Includes full-featured, reliable synchronization and backup classes.
+- Supports regex operations for some functions, as well as specific filters and multiple other choices to choose from. Options such as exact search or something even just containing a keyword, or even having the option to choose to search recursively, are all included.
+- Includes full-featured, reliable synchronization and backup classes (beta). Both include optional and detailed logging.
 - Full set of info gathering tools under the GatherInfo class.
 - Full-featured documentation to guide you through each function in detail. 
 - In case of functionality restrictions, callBash is a function that calls a bash script in order to expand functionality at its peak.
 - Easy to use.
 - You no longer have to take your time in making those file management algorithms that take a while to complete.
 - Fast and efficient, includes a plethora of other features. 
 ____________________________________________________________________________
 ## **Why?**
-- FinderZ is a way to easily expand on the file system of many operating system. It supports, MacOS, Windows, Linux, and Android.
+- FinderZ is a way to easily expand on the file system of many operating systems. It supports, MacOS, Windows, Linux, and Android.
 - Who wouldn't want a tool to manage their files easily in their python scripts? This will save time!
 ____________________________________________________________________________
 ## **How?**
 - FinderZ is composed of many iterating techniques and parametric options. Based on these options, the core of each function deals with a user's choice of what to do or what not to do.
 - More info under the documentation!
 ____________________________________________________________________________
 ## **User notice**
@@ -72,8 +87,8 @@
 - [Time module](https://docs.python.org/3/library/time.html)
 - [Hashlib module](https://docs.python.org/3/library/hashlib.html)
 - [re](https://docs.python.org/3/library/re.html)
 - [Subprocess module](https://docs.python.org/3/library/subprocess.html)
 
 ____________________________________________________________________________
 ## **Make sure to leave a star!**
-- If you like this project, leaving a star is what motivates me in doing more. Thank you, and I hope this is useful to all.
+- If you like this project, leaving a star is what motivates me in doing more. Thank you, and I hope this is useful to all.
```

### Comparing `finderz-2.0.3/pyproject.toml` & `finderz-2.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "FinderZ"
-version = "2.0.3"
+version = "2.0.4"
 authors = [
 	{ name="PatzEdi", email="patzedigithub@gmail.com" },
 ]
 description = "A library that extends file management functionality in Python with many useful features in order to save your time and make life easier!"
 readme = "README.md"
 license = "GPL-3.0-or-later"
 keywords = ["files", "filemanagement", "library", "development"]
```

### Comparing `finderz-2.0.3/PKG-INFO` & `finderz-2.0.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FinderZ
-Version: 2.0.3
+Version: 2.0.4
 Summary: A library that extends file management functionality in Python with many useful features in order to save your time and make life easier!
 Project-URL: Homepage, https://github.com/PatzEdi
 Project-URL: Repository, https://github.com/PatzEdi/FinderZ
 Project-URL: Bug Tracker, https://github.com/PatzEdi/FinderZ/issues
 Author-email: PatzEdi <patzedigithub@gmail.com>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE
@@ -32,50 +32,65 @@
 	
 </p>
 <p align = "center">
 	<img src="https://static.pepy.tech/badge/finderz"
 		height="23">
 </p>
 
-## **IMPORTANT: ** 
+## IMPORTANT: 
 **V2 is finally out! To check out the details, go to the readthedocs documentation under the update v2 section!**
-**LINK TO READ THE DOCS: [Documentation](https://finderz.readthedocs.io/en/latest/index.html)** 
-**IF YOU WANT TO USE THE SYNCHRONIZATION AND BACKUP CLASSeS, MAKE SURE TO THOROUGHLY READ THE [DOCUMENTATION](https://finderz.readthedocs.io/en/latest/index.html) IN ORDER TO PREVENT DATA LOSS**
+**Documentation: [FinderZ](https://finderz.readthedocs.io/en/latest/index.html)** 
 
+**If you want to use the Synchronization and Backup classes, please read the documentation linked above in order to prevent data loss**
+
+**AND: Huge thank you to [@RichardDally](https://github.com/RichardDally) , [@mikudae](https://github.com/mikudae) , [@kyzsuukii](https://github.com/kyzsuukii) , and [@fablau](github.com/fablau) for starring FinderZ.**
 ## **Written in python, this library provides you with different file operation commands as well as info gathering commands on directories as well as files.** 
 ____________________________________________________________________________
 ## **CHANGELOG: V2.0.0**
 
 To check out the details of V2, go to the [documentation](https://finderz.readthedocs.io/en/latest/index.html). This is a big update with many new things!
 
 
+**Minor Fix Version 2.0.4:**
+- Fixed bug where removing more than one file at a time gave an existence error. Sorry for that!
+- Fixed bug where removing a folder that contained folder with the same name as the sync backup folder would result in an infinite loop of backup folders being created.
+- Minimized logging by making file updating hash-dependent. Now, updating files is marked as a critical (C) action in the log.
+- Removed unnecessary printing in some functions.
+- Added a file comparison function in GatherInfo
+- Currently, after having tested FinderZ on Android, permission errors may occasionally occur. This is likely due to read/write permissions assigned to a specific file.
+
+**Minor Fix Version 2.0.3:**
+- Fixed bug in Backup class that gave an existence error. Sorry about that!
+- I have noticed some accidental printing in some functions (such as findFiles, that prints a boolean at the start). This does not currently affect anything, but just prints out occasional, unnecessary output. This will be fixed very soon.
+- Thank you for 16K Downloads!
+
 ## **Usage**
 Installation:
 ```
 pip3 install FinderZ
 ```
 Importing:
 ```
 import FinderZ
 ```
 
 ## **Features**
-- Consists of three classes: GatherInfo, fileOperands, Synchronize, Backup, and callBash.
+- Consists of five classes: GatherInfo, fileOperands, Synchronize, Backup, and callBash.
 - Advanced file operations, already built for you (including many options to choose from!) 
-- Supports regex operations for some functions, as well as specific filters and multiple other choices to choose from. Options such as exact search or something even just containing a keyword, or even having the option to choose to seaerch recursively, are all included.
-- Includes full-featured, reliable synchronization and backup classes.
+- Supports regex operations for some functions, as well as specific filters and multiple other choices to choose from. Options such as exact search or something even just containing a keyword, or even having the option to choose to search recursively, are all included.
+- Includes full-featured, reliable synchronization and backup classes (beta). Both include optional and detailed logging.
 - Full set of info gathering tools under the GatherInfo class.
 - Full-featured documentation to guide you through each function in detail. 
 - In case of functionality restrictions, callBash is a function that calls a bash script in order to expand functionality at its peak.
 - Easy to use.
 - You no longer have to take your time in making those file management algorithms that take a while to complete.
 - Fast and efficient, includes a plethora of other features. 
 ____________________________________________________________________________
 ## **Why?**
-- FinderZ is a way to easily expand on the file system of many operating system. It supports, MacOS, Windows, Linux, and Android.
+- FinderZ is a way to easily expand on the file system of many operating systems. It supports, MacOS, Windows, Linux, and Android.
 - Who wouldn't want a tool to manage their files easily in their python scripts? This will save time!
 ____________________________________________________________________________
 ## **How?**
 - FinderZ is composed of many iterating techniques and parametric options. Based on these options, the core of each function deals with a user's choice of what to do or what not to do.
 - More info under the documentation!
 ____________________________________________________________________________
 ## **User notice**
@@ -89,8 +104,8 @@
 - [Time module](https://docs.python.org/3/library/time.html)
 - [Hashlib module](https://docs.python.org/3/library/hashlib.html)
 - [re](https://docs.python.org/3/library/re.html)
 - [Subprocess module](https://docs.python.org/3/library/subprocess.html)
 
 ____________________________________________________________________________
 ## **Make sure to leave a star!**
-- If you like this project, leaving a star is what motivates me in doing more. Thank you, and I hope this is useful to all.
+- If you like this project, leaving a star is what motivates me in doing more. Thank you, and I hope this is useful to all.
```

