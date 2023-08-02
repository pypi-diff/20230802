# Comparing `tmp/clirail-1.7.1.tar.gz` & `tmp/clirail-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clirail-1.7.1.tar", last modified: Mon Nov 28 12:28:08 2022, max compression
+gzip compressed data, was "clirail-1.7.2.tar", last modified: Wed Aug  2 12:04:20 2023, max compression
```

## Comparing `clirail-1.7.1.tar` & `clirail-1.7.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 ruben     (1000) ruben     (1000)        0 2022-11-28 12:28:08.064460 clirail-1.7.1/
--rw-r--r--   0 ruben     (1000) ruben     (1000)      125 2020-05-17 12:57:44.000000 clirail-1.7.1/.editorconfig
--rw-r--r--   0 ruben     (1000) ruben     (1000)     1210 2022-11-28 12:17:34.000000 clirail-1.7.1/.gitignore
--rw-r--r--   0 ruben     (1000) ruben     (1000)       79 2022-09-06 11:40:21.000000 clirail-1.7.1/.ycm_extra_conf.py
--rw-r--r--   0 ruben     (1000) ruben     (1000)     1300 2022-11-28 12:27:53.000000 clirail-1.7.1/CHANGELOG.md
--rw-r--r--   0 ruben     (1000) ruben     (1000)    35149 2017-09-30 07:16:26.000000 clirail-1.7.1/LICENSE
--rw-r--r--   0 ruben     (1000) ruben     (1000)     3364 2022-11-28 12:28:08.064460 clirail-1.7.1/PKG-INFO
--rw-r--r--   0 ruben     (1000) ruben     (1000)     2401 2020-05-18 11:54:33.000000 clirail-1.7.1/README.md
-drwxr-xr-x   0 ruben     (1000) ruben     (1000)        0 2022-11-28 12:28:08.054460 clirail-1.7.1/bin/
--rwxr-xr-x   0 ruben     (1000) ruben     (1000)       93 2020-05-17 14:15:03.000000 clirail-1.7.1/bin/clirail
-drwxr-xr-x   0 ruben     (1000) ruben     (1000)        0 2022-11-28 12:28:08.054460 clirail-1.7.1/clirail/
--rw-r--r--   0 ruben     (1000) ruben     (1000)        0 2020-05-17 12:54:56.000000 clirail-1.7.1/clirail/__init__.py
--rw-r--r--   0 ruben     (1000) ruben     (1000)     6436 2020-06-29 12:46:07.000000 clirail-1.7.1/clirail/clirail_main.py
--rw-r--r--   0 ruben     (1000) ruben     (1000)       72 2022-05-08 20:59:46.000000 clirail-1.7.1/clirail/config.py
--rw-r--r--   0 ruben     (1000) ruben     (1000)    26154 2020-05-17 12:47:07.000000 clirail-1.7.1/clirail/data.py
--rw-r--r--   0 ruben     (1000) ruben     (1000)     5276 2021-07-17 10:46:03.000000 clirail-1.7.1/clirail/messages.py
--rw-r--r--   0 ruben     (1000) ruben     (1000)     8800 2022-09-18 12:41:27.000000 clirail-1.7.1/clirail/printing.py
--rw-r--r--   0 ruben     (1000) ruben     (1000)     3763 2019-09-15 17:54:29.000000 clirail-1.7.1/clirail/xdg.py
-drwxr-xr-x   0 ruben     (1000) ruben     (1000)        0 2022-11-28 12:28:08.064460 clirail-1.7.1/clirail.egg-info/
--rw-r--r--   0 ruben     (1000) ruben     (1000)     3364 2022-11-28 12:28:07.000000 clirail-1.7.1/clirail.egg-info/PKG-INFO
--rw-r--r--   0 ruben     (1000) ruben     (1000)      481 2022-11-28 12:28:07.000000 clirail-1.7.1/clirail.egg-info/SOURCES.txt
--rw-r--r--   0 ruben     (1000) ruben     (1000)        1 2022-11-28 12:28:07.000000 clirail-1.7.1/clirail.egg-info/dependency_links.txt
--rw-r--r--   0 ruben     (1000) ruben     (1000)       25 2022-11-28 12:28:07.000000 clirail-1.7.1/clirail.egg-info/requires.txt
--rw-r--r--   0 ruben     (1000) ruben     (1000)        8 2022-11-28 12:28:07.000000 clirail-1.7.1/clirail.egg-info/top_level.txt
--rw-r--r--   0 ruben     (1000) ruben     (1000)     1561 2020-05-17 14:20:05.000000 clirail-1.7.1/requirements.txt
--rw-r--r--   0 ruben     (1000) ruben     (1000)       38 2022-11-28 12:28:08.064460 clirail-1.7.1/setup.cfg
--rwxr-xr-x   0 ruben     (1000) ruben     (1000)     1206 2022-11-28 12:27:52.000000 clirail-1.7.1/setup.py
-drwxr-xr-x   0 ruben     (1000) ruben     (1000)        0 2022-11-28 12:28:08.064460 clirail-1.7.1/tools/
--rwxr-xr-x   0 ruben     (1000) ruben     (1000)      208 2020-05-17 14:32:40.000000 clirail-1.7.1/tools/clean.sh
--rwxr-xr-x   0 ruben     (1000) ruben     (1000)      224 2020-05-17 15:05:56.000000 clirail-1.7.1/tools/create_venv.sh
--rwxr-xr-x   0 ruben     (1000) ruben     (1000)     1050 2022-05-08 21:03:20.000000 clirail-1.7.1/tools/release.sh
--rwxr-xr-x   0 ruben     (1000) ruben     (1000)      458 2020-05-17 14:20:02.000000 clirail-1.7.1/tools/update_requirements.sh
+drwxr-xr-x   0 ruben     (1000) ruben     (1000)        0 2023-08-02 12:04:20.581967 clirail-1.7.2/
+-rw-r--r--   0 ruben     (1000) ruben     (1000)      125 2020-05-17 12:57:44.000000 clirail-1.7.2/.editorconfig
+-rw-r--r--   0 ruben     (1000) ruben     (1000)     1210 2022-11-28 12:17:34.000000 clirail-1.7.2/.gitignore
+-rw-r--r--   0 ruben     (1000) ruben     (1000)       79 2022-09-06 11:40:21.000000 clirail-1.7.2/.ycm_extra_conf.py
+-rw-r--r--   0 ruben     (1000) ruben     (1000)     1337 2023-08-02 12:04:15.000000 clirail-1.7.2/CHANGELOG.md
+-rw-r--r--   0 ruben     (1000) ruben     (1000)    35149 2017-09-30 07:16:26.000000 clirail-1.7.2/LICENSE
+-rw-r--r--   0 ruben     (1000) ruben     (1000)     3364 2023-08-02 12:04:20.581967 clirail-1.7.2/PKG-INFO
+-rw-r--r--   0 ruben     (1000) ruben     (1000)     2401 2020-05-18 11:54:33.000000 clirail-1.7.2/README.md
+drwxr-xr-x   0 ruben     (1000) ruben     (1000)        0 2023-08-02 12:04:20.581967 clirail-1.7.2/bin/
+-rwxr-xr-x   0 ruben     (1000) ruben     (1000)       93 2020-05-17 14:15:03.000000 clirail-1.7.2/bin/clirail
+drwxr-xr-x   0 ruben     (1000) ruben     (1000)        0 2023-08-02 12:04:20.581967 clirail-1.7.2/clirail/
+-rw-r--r--   0 ruben     (1000) ruben     (1000)        0 2020-05-17 12:54:56.000000 clirail-1.7.2/clirail/__init__.py
+-rw-r--r--   0 ruben     (1000) ruben     (1000)     6436 2020-06-29 12:46:07.000000 clirail-1.7.2/clirail/clirail_main.py
+-rw-r--r--   0 ruben     (1000) ruben     (1000)       72 2023-08-02 12:02:18.000000 clirail-1.7.2/clirail/config.py
+-rw-r--r--   0 ruben     (1000) ruben     (1000)    26154 2020-05-17 12:47:07.000000 clirail-1.7.2/clirail/data.py
+-rw-r--r--   0 ruben     (1000) ruben     (1000)     5276 2021-07-17 10:46:03.000000 clirail-1.7.2/clirail/messages.py
+-rw-r--r--   0 ruben     (1000) ruben     (1000)     8927 2023-08-02 12:02:15.000000 clirail-1.7.2/clirail/printing.py
+-rw-r--r--   0 ruben     (1000) ruben     (1000)     3763 2019-09-15 17:54:29.000000 clirail-1.7.2/clirail/xdg.py
+drwxr-xr-x   0 ruben     (1000) ruben     (1000)        0 2023-08-02 12:04:20.581967 clirail-1.7.2/clirail.egg-info/
+-rw-r--r--   0 ruben     (1000) ruben     (1000)     3364 2023-08-02 12:04:20.000000 clirail-1.7.2/clirail.egg-info/PKG-INFO
+-rw-r--r--   0 ruben     (1000) ruben     (1000)      481 2023-08-02 12:04:20.000000 clirail-1.7.2/clirail.egg-info/SOURCES.txt
+-rw-r--r--   0 ruben     (1000) ruben     (1000)        1 2023-08-02 12:04:20.000000 clirail-1.7.2/clirail.egg-info/dependency_links.txt
+-rw-r--r--   0 ruben     (1000) ruben     (1000)       25 2023-08-02 12:04:20.000000 clirail-1.7.2/clirail.egg-info/requires.txt
+-rw-r--r--   0 ruben     (1000) ruben     (1000)        8 2023-08-02 12:04:20.000000 clirail-1.7.2/clirail.egg-info/top_level.txt
+-rw-r--r--   0 ruben     (1000) ruben     (1000)     1561 2020-05-17 14:20:05.000000 clirail-1.7.2/requirements.txt
+-rw-r--r--   0 ruben     (1000) ruben     (1000)       38 2023-08-02 12:04:20.581967 clirail-1.7.2/setup.cfg
+-rwxr-xr-x   0 ruben     (1000) ruben     (1000)     1206 2023-08-02 12:04:15.000000 clirail-1.7.2/setup.py
+drwxr-xr-x   0 ruben     (1000) ruben     (1000)        0 2023-08-02 12:04:20.581967 clirail-1.7.2/tools/
+-rwxr-xr-x   0 ruben     (1000) ruben     (1000)      208 2020-05-17 14:32:40.000000 clirail-1.7.2/tools/clean.sh
+-rwxr-xr-x   0 ruben     (1000) ruben     (1000)      224 2020-05-17 15:05:56.000000 clirail-1.7.2/tools/create_venv.sh
+-rwxr-xr-x   0 ruben     (1000) ruben     (1000)     1128 2022-11-28 12:35:56.000000 clirail-1.7.2/tools/release.sh
+-rwxr-xr-x   0 ruben     (1000) ruben     (1000)      458 2020-05-17 14:20:02.000000 clirail-1.7.2/tools/update_requirements.sh
```

### Comparing `clirail-1.7.1/.gitignore` & `clirail-1.7.2/.gitignore`

 * *Files identical despite different names*

### Comparing `clirail-1.7.1/CHANGELOG.md` & `clirail-1.7.2/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,50 +2,47 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).
 Since this is not a library, this project does not adhere to
 [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
-
-## [1.7.1] - 2022-11-28
 ### Added
 ### Changed
 ### Deprecated
 ### Removed
 ### Fixed
-- Add main script so source builds work (it had been accidentally gitignored)
 ### Security
 
-## [1.7] - 2022-05-08
+## [1.7.2] - 2023-08-02
 ### Added
+- Ignore the alert about coastal express
+- Recognize the T (tourist train) and EXP (coastal express) train types
+
 ### Changed
-- Update message to ignore about face masks
 ### Deprecated
 ### Removed
 ### Fixed
 ### Security
 
+## [1.7.1] - 2022-11-28
+### Fixed
+- Add main script so source builds work (it had been accidentally gitignored)
+
+## [1.7] - 2022-05-08
+### Changed
+- Update message to ignore about face masks
+
 ## [1.6] - 2021-07-17
 ### Added
 - Show date in results when not today
-### Changed
-### Deprecated
-### Removed
-### Fixed
-### Security
 
 ## [1.5] - 2021-07-06
 ### Added
 - Ignore the alert about masks being compulsory
-### Changed
-### Deprecated
-### Removed
-### Fixed
-### Security
 
 ## [1.4] - 2020-10-31
 ### Added
 - Emoji for Eurostar
 
 ## [1.3] - 2020-06-29
 ### Added
```

### Comparing `clirail-1.7.1/LICENSE` & `clirail-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `clirail-1.7.1/PKG-INFO` & `clirail-1.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clirail
-Version: 1.7.1
+Version: 1.7.2
 Summary: Command line application for the iRail API
 Home-page: https://framagit.org/Midgard/clirail
 Author: Midgard
 Project-URL: Source, https://framagit.org/Midgard/clirail
 Project-URL: Change log, https://framagit.org/Midgard/clirail/-/blob/master/CHANGELOG.md
 Project-URL: Bug tracker, https://framagit.org/Midgard/clirail/-/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clirail-1.7.1/README.md` & `clirail-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `clirail-1.7.1/clirail/clirail_main.py` & `clirail-1.7.2/clirail/clirail_main.py`

 * *Files identical despite different names*

### Comparing `clirail-1.7.1/clirail/data.py` & `clirail-1.7.2/clirail/data.py`

 * *Files identical despite different names*

### Comparing `clirail-1.7.1/clirail/messages.py` & `clirail-1.7.2/clirail/messages.py`

 * *Files identical despite different names*

### Comparing `clirail-1.7.1/clirail/printing.py` & `clirail-1.7.2/clirail/printing.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,28 +12,28 @@
 	("BUS",  "🚌"), # bus, typically to replace train in case of railroad works
 	("EUR",  "🚄"), # Eurostar
 	("ICE",  "🚄"), # ICE, German high-speed train
 	("THA",  "🚄"), # Thalys
 	("TGV",  "🚄"), # TGV, French high-speed train
 	("IC",   "🚅"), # intercity train
 	("ICT",  "🚅"), # tourist intercity train
+	("T",    "🚅"), # tourist train
+	("EXP",  "🚅"), # coastal express train
 	("P",    "🚅"), # peak train
 	("TRN",  "🚅"), # just a train
 	("EXT",  "🚅"), # replacement train or something
 	("S",    "🚂"), # sprinter train
 	("L",    "🚂"), # local train
 	("WALK", "🚶"), # walking
 	("",     "🚀")  # unknown, go by rocket
 ]
 
 IGNORED_ALERTS = {
-	"Mondmaskerplicht",
-	"Port du masque obligatoire",
-	"Face mask mandatory",
-	"Maskenpflicht"
+	"Mondmaskerplicht", "Port du masque obligatoire", "Face mask mandatory", "Maskenpflicht",
+	"Kust-Express", "Côte-Express", "Côte-Express."
 }
 
 
 def without_colours(s):
 	return re.sub(r"\x1b\[[^m]*m", "", s)
```

### Comparing `clirail-1.7.1/clirail/xdg.py` & `clirail-1.7.2/clirail/xdg.py`

 * *Files identical despite different names*

### Comparing `clirail-1.7.1/clirail.egg-info/PKG-INFO` & `clirail-1.7.2/clirail.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clirail
-Version: 1.7.1
+Version: 1.7.2
 Summary: Command line application for the iRail API
 Home-page: https://framagit.org/Midgard/clirail
 Author: Midgard
 Project-URL: Source, https://framagit.org/Midgard/clirail
 Project-URL: Change log, https://framagit.org/Midgard/clirail/-/blob/master/CHANGELOG.md
 Project-URL: Bug tracker, https://framagit.org/Midgard/clirail/-/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clirail-1.7.1/requirements.txt` & `clirail-1.7.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `clirail-1.7.1/setup.py` & `clirail-1.7.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 
 setuptools.setup(
 	name="clirail",
-	version="1.7.1",
+	version="1.7.2",
 	author="Midgard",
 	author_email=None,
 	description="Command line application for the iRail API",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	scripts=["bin/clirail"],
```

### Comparing `clirail-1.7.1/tools/release.sh` & `clirail-1.7.2/tools/release.sh`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 prev_version="$(./setup.py --version)"
 echo "$prev_version"
 read -p "Enter new version: v" version
 
 tagid=v"$version"
 if [ "$version" != "$prev_version" ]; then
 	sed -i 's/version=".*"/version="'"$version"'"/' setup.py
-	sed -i 's/## \[Unreleased\]/&\n\n## ['"$version"'] - '"$(date --utc +%Y-%m-%d)"'/' CHANGELOG.md
+	sed -i 's/## \[Unreleased\]/&\n### Added\n### Changed\n### Deprecated\n### Removed\n### Fixed\n### Security\n\n## ['"$version"'] - '"$(date --utc +%Y-%m-%d)"'/' CHANGELOG.md
 	echo; echo "Inspect CHANGELOG..."
 	${EDITOR:-nano} CHANGELOG.md
 	git add setup.py CHANGELOG.md
 	git commit -m "Bump version to $version"
 
 	echo "Creating git tag $tagid"
 	git tag -s -m "Version $version" "$tagid"
```

