# Comparing `tmp/clirail-1.7.2.tar.gz` & `tmp/clirail-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clirail-1.7.2.tar", last modified: Wed Aug  2 12:04:20 2023, max compression
+gzip compressed data, was "clirail-1.7.3.tar", last modified: Wed Aug  2 12:26:24 2023, max compression
```

## Comparing `clirail-1.7.2.tar` & `clirail-1.7.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 ruben     (1000) ruben     (1000)        0 2023-08-02 12:04:20.581967 clirail-1.7.2/
--rw-r--r--   0 ruben     (1000) ruben     (1000)      125 2020-05-17 12:57:44.000000 clirail-1.7.2/.editorconfig
--rw-r--r--   0 ruben     (1000) ruben     (1000)     1210 2022-11-28 12:17:34.000000 clirail-1.7.2/.gitignore
--rw-r--r--   0 ruben     (1000) ruben     (1000)       79 2022-09-06 11:40:21.000000 clirail-1.7.2/.ycm_extra_conf.py
--rw-r--r--   0 ruben     (1000) ruben     (1000)     1337 2023-08-02 12:04:15.000000 clirail-1.7.2/CHANGELOG.md
--rw-r--r--   0 ruben     (1000) ruben     (1000)    35149 2017-09-30 07:16:26.000000 clirail-1.7.2/LICENSE
--rw-r--r--   0 ruben     (1000) ruben     (1000)     3364 2023-08-02 12:04:20.581967 clirail-1.7.2/PKG-INFO
--rw-r--r--   0 ruben     (1000) ruben     (1000)     2401 2020-05-18 11:54:33.000000 clirail-1.7.2/README.md
-drwxr-xr-x   0 ruben     (1000) ruben     (1000)        0 2023-08-02 12:04:20.581967 clirail-1.7.2/bin/
--rwxr-xr-x   0 ruben     (1000) ruben     (1000)       93 2020-05-17 14:15:03.000000 clirail-1.7.2/bin/clirail
-drwxr-xr-x   0 ruben     (1000) ruben     (1000)        0 2023-08-02 12:04:20.581967 clirail-1.7.2/clirail/
--rw-r--r--   0 ruben     (1000) ruben     (1000)        0 2020-05-17 12:54:56.000000 clirail-1.7.2/clirail/__init__.py
--rw-r--r--   0 ruben     (1000) ruben     (1000)     6436 2020-06-29 12:46:07.000000 clirail-1.7.2/clirail/clirail_main.py
--rw-r--r--   0 ruben     (1000) ruben     (1000)       72 2023-08-02 12:02:18.000000 clirail-1.7.2/clirail/config.py
--rw-r--r--   0 ruben     (1000) ruben     (1000)    26154 2020-05-17 12:47:07.000000 clirail-1.7.2/clirail/data.py
--rw-r--r--   0 ruben     (1000) ruben     (1000)     5276 2021-07-17 10:46:03.000000 clirail-1.7.2/clirail/messages.py
--rw-r--r--   0 ruben     (1000) ruben     (1000)     8927 2023-08-02 12:02:15.000000 clirail-1.7.2/clirail/printing.py
--rw-r--r--   0 ruben     (1000) ruben     (1000)     3763 2019-09-15 17:54:29.000000 clirail-1.7.2/clirail/xdg.py
-drwxr-xr-x   0 ruben     (1000) ruben     (1000)        0 2023-08-02 12:04:20.581967 clirail-1.7.2/clirail.egg-info/
--rw-r--r--   0 ruben     (1000) ruben     (1000)     3364 2023-08-02 12:04:20.000000 clirail-1.7.2/clirail.egg-info/PKG-INFO
--rw-r--r--   0 ruben     (1000) ruben     (1000)      481 2023-08-02 12:04:20.000000 clirail-1.7.2/clirail.egg-info/SOURCES.txt
--rw-r--r--   0 ruben     (1000) ruben     (1000)        1 2023-08-02 12:04:20.000000 clirail-1.7.2/clirail.egg-info/dependency_links.txt
--rw-r--r--   0 ruben     (1000) ruben     (1000)       25 2023-08-02 12:04:20.000000 clirail-1.7.2/clirail.egg-info/requires.txt
--rw-r--r--   0 ruben     (1000) ruben     (1000)        8 2023-08-02 12:04:20.000000 clirail-1.7.2/clirail.egg-info/top_level.txt
--rw-r--r--   0 ruben     (1000) ruben     (1000)     1561 2020-05-17 14:20:05.000000 clirail-1.7.2/requirements.txt
--rw-r--r--   0 ruben     (1000) ruben     (1000)       38 2023-08-02 12:04:20.581967 clirail-1.7.2/setup.cfg
--rwxr-xr-x   0 ruben     (1000) ruben     (1000)     1206 2023-08-02 12:04:15.000000 clirail-1.7.2/setup.py
-drwxr-xr-x   0 ruben     (1000) ruben     (1000)        0 2023-08-02 12:04:20.581967 clirail-1.7.2/tools/
--rwxr-xr-x   0 ruben     (1000) ruben     (1000)      208 2020-05-17 14:32:40.000000 clirail-1.7.2/tools/clean.sh
--rwxr-xr-x   0 ruben     (1000) ruben     (1000)      224 2020-05-17 15:05:56.000000 clirail-1.7.2/tools/create_venv.sh
--rwxr-xr-x   0 ruben     (1000) ruben     (1000)     1128 2022-11-28 12:35:56.000000 clirail-1.7.2/tools/release.sh
--rwxr-xr-x   0 ruben     (1000) ruben     (1000)      458 2020-05-17 14:20:02.000000 clirail-1.7.2/tools/update_requirements.sh
+drwxr-xr-x   0 ruben     (1000) ruben     (1000)        0 2023-08-02 12:26:24.675732 clirail-1.7.3/
+-rw-r--r--   0 ruben     (1000) ruben     (1000)      125 2020-05-17 12:57:44.000000 clirail-1.7.3/.editorconfig
+-rw-r--r--   0 ruben     (1000) ruben     (1000)     1210 2022-11-28 12:17:34.000000 clirail-1.7.3/.gitignore
+-rw-r--r--   0 ruben     (1000) ruben     (1000)       79 2022-09-06 11:40:21.000000 clirail-1.7.3/.ycm_extra_conf.py
+-rw-r--r--   0 ruben     (1000) ruben     (1000)     1574 2023-08-02 12:26:20.000000 clirail-1.7.3/CHANGELOG.md
+-rw-r--r--   0 ruben     (1000) ruben     (1000)    35149 2017-09-30 07:16:26.000000 clirail-1.7.3/LICENSE
+-rw-r--r--   0 ruben     (1000) ruben     (1000)     3364 2023-08-02 12:26:24.675732 clirail-1.7.3/PKG-INFO
+-rw-r--r--   0 ruben     (1000) ruben     (1000)     2401 2020-05-18 11:54:33.000000 clirail-1.7.3/README.md
+drwxr-xr-x   0 ruben     (1000) ruben     (1000)        0 2023-08-02 12:26:24.675732 clirail-1.7.3/bin/
+-rwxr-xr-x   0 ruben     (1000) ruben     (1000)       93 2020-05-17 14:15:03.000000 clirail-1.7.3/bin/clirail
+drwxr-xr-x   0 ruben     (1000) ruben     (1000)        0 2023-08-02 12:26:24.675732 clirail-1.7.3/clirail/
+-rw-r--r--   0 ruben     (1000) ruben     (1000)        0 2020-05-17 12:54:56.000000 clirail-1.7.3/clirail/__init__.py
+-rw-r--r--   0 ruben     (1000) ruben     (1000)     6533 2023-08-02 12:21:15.000000 clirail-1.7.3/clirail/clirail_main.py
+-rw-r--r--   0 ruben     (1000) ruben     (1000)       72 2023-08-02 12:02:18.000000 clirail-1.7.3/clirail/config.py
+-rw-r--r--   0 ruben     (1000) ruben     (1000)    26154 2020-05-17 12:47:07.000000 clirail-1.7.3/clirail/data.py
+-rw-r--r--   0 ruben     (1000) ruben     (1000)     5276 2021-07-17 10:46:03.000000 clirail-1.7.3/clirail/messages.py
+-rw-r--r--   0 ruben     (1000) ruben     (1000)     9090 2023-08-02 12:16:27.000000 clirail-1.7.3/clirail/printing.py
+-rw-r--r--   0 ruben     (1000) ruben     (1000)     3763 2019-09-15 17:54:29.000000 clirail-1.7.3/clirail/xdg.py
+drwxr-xr-x   0 ruben     (1000) ruben     (1000)        0 2023-08-02 12:26:24.675732 clirail-1.7.3/clirail.egg-info/
+-rw-r--r--   0 ruben     (1000) ruben     (1000)     3364 2023-08-02 12:26:24.000000 clirail-1.7.3/clirail.egg-info/PKG-INFO
+-rw-r--r--   0 ruben     (1000) ruben     (1000)      481 2023-08-02 12:26:24.000000 clirail-1.7.3/clirail.egg-info/SOURCES.txt
+-rw-r--r--   0 ruben     (1000) ruben     (1000)        1 2023-08-02 12:26:24.000000 clirail-1.7.3/clirail.egg-info/dependency_links.txt
+-rw-r--r--   0 ruben     (1000) ruben     (1000)       25 2023-08-02 12:26:24.000000 clirail-1.7.3/clirail.egg-info/requires.txt
+-rw-r--r--   0 ruben     (1000) ruben     (1000)        8 2023-08-02 12:26:24.000000 clirail-1.7.3/clirail.egg-info/top_level.txt
+-rw-r--r--   0 ruben     (1000) ruben     (1000)     1561 2020-05-17 14:20:05.000000 clirail-1.7.3/requirements.txt
+-rw-r--r--   0 ruben     (1000) ruben     (1000)       38 2023-08-02 12:26:24.675732 clirail-1.7.3/setup.cfg
+-rwxr-xr-x   0 ruben     (1000) ruben     (1000)     1206 2023-08-02 12:26:20.000000 clirail-1.7.3/setup.py
+drwxr-xr-x   0 ruben     (1000) ruben     (1000)        0 2023-08-02 12:26:24.675732 clirail-1.7.3/tools/
+-rwxr-xr-x   0 ruben     (1000) ruben     (1000)      208 2020-05-17 14:32:40.000000 clirail-1.7.3/tools/clean.sh
+-rwxr-xr-x   0 ruben     (1000) ruben     (1000)      224 2020-05-17 15:05:56.000000 clirail-1.7.3/tools/create_venv.sh
+-rwxr-xr-x   0 ruben     (1000) ruben     (1000)     1128 2022-11-28 12:35:56.000000 clirail-1.7.3/tools/release.sh
+-rwxr-xr-x   0 ruben     (1000) ruben     (1000)      458 2020-05-17 14:20:02.000000 clirail-1.7.3/tools/update_requirements.sh
```

### Comparing `clirail-1.7.2/.gitignore` & `clirail-1.7.3/.gitignore`

 * *Files identical despite different names*

### Comparing `clirail-1.7.2/CHANGELOG.md` & `clirail-1.7.3/CHANGELOG.md`

 * *Files 18% similar despite different names*

```diff
@@ -9,14 +9,25 @@
 ### Added
 ### Changed
 ### Deprecated
 ### Removed
 ### Fixed
 ### Security
 
+## [1.7.3] - 2023-08-02
+### Added
+### Changed
+- Make train type detection more robust against future train types
+- Add better error handling when iRail could not respond to our request
+
+### Deprecated
+### Removed
+### Fixed
+### Security
+
 ## [1.7.2] - 2023-08-02
 ### Added
 - Ignore the alert about coastal express
 - Recognize the T (tourist train) and EXP (coastal express) train types
 
 ### Changed
 ### Deprecated
```

### Comparing `clirail-1.7.2/LICENSE` & `clirail-1.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `clirail-1.7.2/PKG-INFO` & `clirail-1.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clirail
-Version: 1.7.2
+Version: 1.7.3
 Summary: Command line application for the iRail API
 Home-page: https://framagit.org/Midgard/clirail
 Author: Midgard
 Project-URL: Source, https://framagit.org/Midgard/clirail
 Project-URL: Change log, https://framagit.org/Midgard/clirail/-/blob/master/CHANGELOG.md
 Project-URL: Bug tracker, https://framagit.org/Midgard/clirail/-/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clirail-1.7.2/README.md` & `clirail-1.7.3/README.md`

 * *Files identical despite different names*

### Comparing `clirail-1.7.2/clirail/clirail_main.py` & `clirail-1.7.3/clirail/clirail_main.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 	except FileNotFoundError:
 		print(t("public_log"), file=sys.stderr)
 		_ = input()
 		print(t("downloading_stations"))
 		print("")
 		stations_file.parent.mkdir(exist_ok=True, parents=True)
 		req = requests.get(stations_url, params={"format": "json", "lang": LANG})
+		req.raise_for_status()
 		stations = req.json()
 
 		with open(str(stations_file), mode="w") as file:
 			json.dump(stations, file)
 
 		return stations["station"]
 
@@ -96,14 +97,15 @@
 		("id" if station_is_id else "station"): station,
 		"alerts": alerts,
 		"arrdep": "departure" if departure else "arrival",
 		"date": date, "time": time
 	}
 
 	req = requests.get(LIVEBOARD_URL, params=params)
+	req.raise_for_status()
 	return req.json()
 
 
 def get_connections(fro, to, moment=None, alerts=False):
 	date, time = irail_date(moment)
 
 	params = {
@@ -112,24 +114,26 @@
 
 		"from": fro, "to": to,
 		"alerts": alerts,
 		"date": date, "time": time
 	}
 
 	req = requests.get(CONNECTIONS_URL, params=params)
+	req.raise_for_status()
 	return req.json()
 
 
 def get_disturbances():
 	params = {
 		"lang": LANG,
 		"format": "json"
 	}
 
 	req = requests.get(DISTURBANCES_URL, params=params)
+	req.raise_for_status()
 	return req.json()
 
 
 # FIXME split into get_summary and print_summary
 def show_summary():
 	now = datetime.now()
 	hour_ago = now - timedelta(hours=1)
```

### Comparing `clirail-1.7.2/clirail/data.py` & `clirail-1.7.3/clirail/data.py`

 * *Files identical despite different names*

### Comparing `clirail-1.7.2/clirail/messages.py` & `clirail-1.7.3/clirail/messages.py`

 * *Files identical despite different names*

### Comparing `clirail-1.7.2/clirail/printing.py` & `clirail-1.7.3/clirail/printing.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,48 +4,51 @@
 
 from datetime import datetime, date
 from .messages import t
 import re
 from itertools import chain
 
 
-icons = [
-	("BUS",  "🚌"), # bus, typically to replace train in case of railroad works
-	("EUR",  "🚄"), # Eurostar
-	("ICE",  "🚄"), # ICE, German high-speed train
-	("THA",  "🚄"), # Thalys
-	("TGV",  "🚄"), # TGV, French high-speed train
-	("IC",   "🚅"), # intercity train
-	("ICT",  "🚅"), # tourist intercity train
-	("T",    "🚅"), # tourist train
-	("EXP",  "🚅"), # coastal express train
-	("P",    "🚅"), # peak train
-	("TRN",  "🚅"), # just a train
-	("EXT",  "🚅"), # replacement train or something
-	("S",    "🚂"), # sprinter train
-	("L",    "🚂"), # local train
-	("WALK", "🚶"), # walking
-	("",     "🚀")  # unknown, go by rocket
-]
+icons = {
+	"BUS":  "🚌", # bus, typically to replace train in case of railroad works
+	"EUR":  "🚄", # Eurostar
+	"ICE":  "🚄", # ICE, German high-speed train
+	"THA":  "🚄", # Thalys
+	"TGV":  "🚄", # TGV, French high-speed train
+	"IC":   "🚅", # intercity train
+	"T":    "🚅", # tourist train
+	"ICT":  "🚅", # tourist intercity train (actually same as T)
+	"EXP":  "🚅", # coastal express train (actually same as T, again)
+	"P":    "🚅", # rush hour train
+	"TRN":  "🚅", # unspecified train
+	"EXT":  "🚅", # extra train (ad-hoc replacement train in case of problems with another train)
+	"EC":   "🚅", # EuroCity
+	"S":    "🚂", # sprinter (suburban) train
+	"L":    "🚂", # local train
+	"WALK": "🚶", # walking
+	"":     "🚀"  # unknown, go by rocket
+}
 
 IGNORED_ALERTS = {
 	"Mondmaskerplicht", "Port du masque obligatoire", "Face mask mandatory", "Maskenpflicht",
 	"Kust-Express", "Côte-Express", "Côte-Express."
 }
 
 
 def without_colours(s):
 	return re.sub(r"\x1b\[[^m]*m", "", s)
 
 
 def icon_from_ref(ref):
-	for prefix, icon in icons:
-		if ref.startswith(prefix):
-			return icon
-	assert False
+	m = re.match(r"([A-Za-z]+)([0-9].+)?", ref)
+	if not m:
+		return icons[""]
+	prefix = m.group(1)
+
+	return icons.get(prefix) or icons[""]
 
 
 def format_duration(seconds, hm=t("hm_duration_fmt"), m=t("m_duration_fmt")):
 	minutes = int(seconds) // 60
 	if minutes < 60:
 		return m.format(minutes)
 	return hm.format(minutes // 60, minutes % 60)
```

### Comparing `clirail-1.7.2/clirail/xdg.py` & `clirail-1.7.3/clirail/xdg.py`

 * *Files identical despite different names*

### Comparing `clirail-1.7.2/clirail.egg-info/PKG-INFO` & `clirail-1.7.3/clirail.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clirail
-Version: 1.7.2
+Version: 1.7.3
 Summary: Command line application for the iRail API
 Home-page: https://framagit.org/Midgard/clirail
 Author: Midgard
 Project-URL: Source, https://framagit.org/Midgard/clirail
 Project-URL: Change log, https://framagit.org/Midgard/clirail/-/blob/master/CHANGELOG.md
 Project-URL: Bug tracker, https://framagit.org/Midgard/clirail/-/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clirail-1.7.2/requirements.txt` & `clirail-1.7.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `clirail-1.7.2/setup.py` & `clirail-1.7.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 
 setuptools.setup(
 	name="clirail",
-	version="1.7.2",
+	version="1.7.3",
 	author="Midgard",
 	author_email=None,
 	description="Command line application for the iRail API",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	scripts=["bin/clirail"],
```

### Comparing `clirail-1.7.2/tools/release.sh` & `clirail-1.7.3/tools/release.sh`

 * *Files identical despite different names*

