# Comparing `tmp/py40kie-0.2.1.tar.gz` & `tmp/py40kie-0.2.2.tar.gz`

## Comparing `py40kie-0.2.1.tar` & `py40kie-0.2.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 py40kie-0.2.1/.github/workflows/publish-to-test-pypi.yml
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 py40kie-0.2.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py40kie-0.2.1/src/__init__.py
--rw-r--r--   0        0        0    11081 2020-02-02 00:00:00.000000 py40kie-0.2.1/src/py40kie.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 py40kie-0.2.1/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 py40kie-0.2.1/LICENSE
--rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 py40kie-0.2.1/README.md
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 py40kie-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4515 2020-02-02 00:00:00.000000 py40kie-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 py40kie-0.2.2/.github/workflows/publish-to-test-pypi.yml
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 py40kie-0.2.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py40kie-0.2.2/src/__init__.py
+-rw-r--r--   0        0        0    11081 2020-02-02 00:00:00.000000 py40kie-0.2.2/src/py40kie.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 py40kie-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 py40kie-0.2.2/LICENSE
+-rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 py40kie-0.2.2/README.md
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 py40kie-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 py40kie-0.2.2/PKG-INFO
```

### Comparing `py40kie-0.2.1/.github/workflows/publish-to-test-pypi.yml` & `py40kie-0.2.2/.github/workflows/publish-to-test-pypi.yml`

 * *Files identical despite different names*

### Comparing `py40kie-0.2.1/.github/workflows/python-publish.yml` & `py40kie-0.2.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `py40kie-0.2.1/src/py40kie.py` & `py40kie-0.2.2/src/py40kie.py`

 * *Files identical despite different names*

### Comparing `py40kie-0.2.1/.gitignore` & `py40kie-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `py40kie-0.2.1/LICENSE` & `py40kie-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py40kie-0.2.1/README.md` & `py40kie-0.2.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -10,24 +10,30 @@
   ```
 - Run py40kie using command line:  
   ```
   py40kie [-h] [-i EXTRA_INDEXES [EXTRA_INDEXES ...]] [-o OUTPUT_PDF] [-b] [-a] [-d] [-s] [-e] [-w] [-na] [-nd]
                [-ns] [-ne] [-nw] [-r RULE_PAGES [RULE_PAGES ...]] [-v]
                index_pdf pages [pages ...]
   ```
-  ### Examples  
+## Army List builder instructions
+- Create army list with [Google Sheet army list builder](https://drive.google.com/drive/folders/1_d0pSPt2FGUSlCSWsAF0c2JmgkWIa4DW)  
+- Run the generated py40kie command  
+## Examples  
   ```
   py40kie "Tyranids Index.pdf" 9 21 25 27 -o "my army list"  
   ```
   ```
   py40kie "Tyranids Index.pdf" "hive tyrant" "tyranid warriors with ranged bio-weapons" 25 "hOrMaGaUnTs" -o "./my lists/my army list"
   ```
   ```
   py40kie "Space Wolves Index.pdf" 7 1-23 "Blood Claws" 1-53 "terminator squad" "2-culexus assassin" 2-7 3-1 -o "Best Army List Ever.pdf" -i "Space Marines Index.pdf" "Agents of Imperium Index.pdf" "Imperial Armour Astartes.pdf"
   ```
+  ```
+  py40kie "Blood Angels Index.pdf" "Commander Dante" "Sanguinary Guard" "Lieutenant in Phobos Armour" "Death Company Marines" "Astraeus" "Culexus Assassin" "Knight Gallant" -o "super competitive list.pdf"  -i "Astartes Index.pdf" "Imperial Armour Astartes.pdf" "Agents of the Imperium Index.pdf" "Imperial Knights Index.pdf"
+  ```
   
   # Arguments
   #### Postional arguments
     - The "index.pdf" file to extract cards from  
     - Space separated list of cards to extract. Can be page numbers or **exact** unit titles. Army rules, detachment rules, stratagems, enhancements and unit wargear are included automatically  
   #### Optional arguments:  
     - -o: The file to save the extracted pdf to. Folder path can be included
@@ -42,16 +48,17 @@
     - -v: Optional flag to override page extraction. Will extract only the page numbers specified from the main index  
 
 # Contributions  
 ## Future features  
 Any suggested features would be appreciated  
  - [x] Allied units from other Indexes/Imperial Armour/Legends  
  - [x] Extract Adeptus Astartes army rule page for Space Marine lists  
- - [x] Create runnable command from [Google Sheet army builder lists](https://www.reddit.com/r/WarhammerCompetitive/comments/14br6rw/10e_40k_list_builder_spreadsheets/)  
-       Copy the cells in the yellow box from here to your own sheet: https://docs.google.com/spreadsheets/d/1A1lDqmL0f_iH9OIUQWL_v83_leyhm3t0rhyC20UfrPA  
+ - [x] Create runnable command from [Google Sheet army builder lists](https://drive.google.com/drive/folders/1_d0pSPt2FGUSlCSWsAF0c2JmgkWIa4DW)  
+       [Example Sheet](https://docs.google.com/spreadsheets/d/1A1lDqmL0f_iH9OIUQWL_v83_leyhm3t0rhyC20UfrPA)  
+       Original creator [u/Swelt](https://www.reddit.com/r/WarhammerCompetitive/comments/14br6rw/10e_40k_list_builder_spreadsheets)  
  - [ ] Extract extra rule pages. e.g. Deathwatch Armoury  
  - [ ] Handle exceptions gracefully  
  - [ ] Webapp version?...  
 
 
 ## Issues  
 py40kie was not tested on all indexes. If there is any problem extracting cards please submit an issue https://github.com/Dragons-Ire/40k-index-pdf-extractor/issues/new
```

### Comparing `py40kie-0.2.1/pyproject.toml` & `py40kie-0.2.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "py40kie"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   { name="Chris Austin", email="dragons.ire.oce@gmail.com" },
 ]
 description = "Command line Python program to extract army rules and unit cards from 10th edition Warhammer 40k indexes to create army list specific pdfs with reduced file size."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `py40kie-0.2.1/PKG-INFO` & `py40kie-0.2.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py40kie
-Version: 0.2.1
+Version: 0.2.2
 Summary: Command line Python program to extract army rules and unit cards from 10th edition Warhammer 40k indexes to create army list specific pdfs with reduced file size.
 Project-URL: Homepage, https://github.com/Dragons-Ire/40k-index-pdf-extractor
 Project-URL: Bug Tracker, https://github.com/Dragons-Ire/40k-index-pdf-extractor/issues
 Author-email: Chris Austin <dragons.ire.oce@gmail.com>
 License-File: LICENSE
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
@@ -31,24 +31,30 @@
   ```
 - Run py40kie using command line:  
   ```
   py40kie [-h] [-i EXTRA_INDEXES [EXTRA_INDEXES ...]] [-o OUTPUT_PDF] [-b] [-a] [-d] [-s] [-e] [-w] [-na] [-nd]
                [-ns] [-ne] [-nw] [-r RULE_PAGES [RULE_PAGES ...]] [-v]
                index_pdf pages [pages ...]
   ```
-  ### Examples  
+## Army List builder instructions
+- Create army list with [Google Sheet army list builder](https://drive.google.com/drive/folders/1_d0pSPt2FGUSlCSWsAF0c2JmgkWIa4DW)  
+- Run the generated py40kie command  
+## Examples  
   ```
   py40kie "Tyranids Index.pdf" 9 21 25 27 -o "my army list"  
   ```
   ```
   py40kie "Tyranids Index.pdf" "hive tyrant" "tyranid warriors with ranged bio-weapons" 25 "hOrMaGaUnTs" -o "./my lists/my army list"
   ```
   ```
   py40kie "Space Wolves Index.pdf" 7 1-23 "Blood Claws" 1-53 "terminator squad" "2-culexus assassin" 2-7 3-1 -o "Best Army List Ever.pdf" -i "Space Marines Index.pdf" "Agents of Imperium Index.pdf" "Imperial Armour Astartes.pdf"
   ```
+  ```
+  py40kie "Blood Angels Index.pdf" "Commander Dante" "Sanguinary Guard" "Lieutenant in Phobos Armour" "Death Company Marines" "Astraeus" "Culexus Assassin" "Knight Gallant" -o "super competitive list.pdf"  -i "Astartes Index.pdf" "Imperial Armour Astartes.pdf" "Agents of the Imperium Index.pdf" "Imperial Knights Index.pdf"
+  ```
   
   # Arguments
   #### Postional arguments
     - The "index.pdf" file to extract cards from  
     - Space separated list of cards to extract. Can be page numbers or **exact** unit titles. Army rules, detachment rules, stratagems, enhancements and unit wargear are included automatically  
   #### Optional arguments:  
     - -o: The file to save the extracted pdf to. Folder path can be included
@@ -63,16 +69,17 @@
     - -v: Optional flag to override page extraction. Will extract only the page numbers specified from the main index  
 
 # Contributions  
 ## Future features  
 Any suggested features would be appreciated  
  - [x] Allied units from other Indexes/Imperial Armour/Legends  
  - [x] Extract Adeptus Astartes army rule page for Space Marine lists  
- - [x] Create runnable command from [Google Sheet army builder lists](https://www.reddit.com/r/WarhammerCompetitive/comments/14br6rw/10e_40k_list_builder_spreadsheets/)  
-       Copy the cells in the yellow box from here to your own sheet: https://docs.google.com/spreadsheets/d/1A1lDqmL0f_iH9OIUQWL_v83_leyhm3t0rhyC20UfrPA  
+ - [x] Create runnable command from [Google Sheet army builder lists](https://drive.google.com/drive/folders/1_d0pSPt2FGUSlCSWsAF0c2JmgkWIa4DW)  
+       [Example Sheet](https://docs.google.com/spreadsheets/d/1A1lDqmL0f_iH9OIUQWL_v83_leyhm3t0rhyC20UfrPA)  
+       Original creator [u/Swelt](https://www.reddit.com/r/WarhammerCompetitive/comments/14br6rw/10e_40k_list_builder_spreadsheets)  
  - [ ] Extract extra rule pages. e.g. Deathwatch Armoury  
  - [ ] Handle exceptions gracefully  
  - [ ] Webapp version?...  
 
 
 ## Issues  
 py40kie was not tested on all indexes. If there is any problem extracting cards please submit an issue https://github.com/Dragons-Ire/40k-index-pdf-extractor/issues/new
```

