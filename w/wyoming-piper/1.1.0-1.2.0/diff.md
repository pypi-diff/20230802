# Comparing `tmp/wyoming_piper-1.1.0.tar.gz` & `tmp/wyoming_piper-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wyoming_piper-1.1.0.tar", last modified: Mon Jul 17 16:10:40 2023, max compression
+gzip compressed data, was "wyoming_piper-1.2.0.tar", last modified: Tue Aug  1 21:59:03 2023, max compression
```

## Comparing `wyoming_piper-1.1.0.tar` & `wyoming_piper-1.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-17 16:10:40.025092 wyoming_piper-1.1.0/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       59 2023-07-13 15:51:03.000000 wyoming_piper-1.1.0/MANIFEST.in
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      666 2023-07-17 16:10:40.025092 wyoming_piper-1.1.0/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       15 2023-07-17 15:12:29.000000 wyoming_piper-1.1.0/requirements.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       38 2023-07-17 16:10:40.025092 wyoming_piper-1.1.0/setup.cfg
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1392 2023-07-17 15:12:32.000000 wyoming_piper-1.1.0/setup.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-17 16:10:40.025092 wyoming_piper-1.1.0/wyoming_piper/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       32 2023-04-21 15:28:34.000000 wyoming_piper-1.1.0/wyoming_piper/__init__.py
--rwxr-xr-x   0 hansenm   (1000) hansenm   (1000)     4773 2023-07-17 16:01:40.000000 wyoming_piper-1.1.0/wyoming_piper/__main__.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1015 2023-04-21 15:28:34.000000 wyoming_piper-1.1.0/wyoming_piper/const.py
--rwxr-xr-x   0 hansenm   (1000) hansenm   (1000)     3866 2023-07-13 14:58:56.000000 wyoming_piper-1.1.0/wyoming_piper/download.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1107 2023-05-10 19:58:23.000000 wyoming_piper-1.1.0/wyoming_piper/file_hash.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4603 2023-07-17 15:31:35.000000 wyoming_piper-1.1.0/wyoming_piper/handler.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5707 2023-07-17 15:27:00.000000 wyoming_piper-1.1.0/wyoming_piper/process.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)   116115 2023-07-13 15:29:35.000000 wyoming_piper-1.1.0/wyoming_piper/voices.json
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-17 16:10:40.025092 wyoming_piper-1.1.0/wyoming_piper.egg-info/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      666 2023-07-17 16:10:40.000000 wyoming_piper-1.1.0/wyoming_piper.egg-info/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      425 2023-07-17 16:10:40.000000 wyoming_piper-1.1.0/wyoming_piper.egg-info/SOURCES.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-07-17 16:10:40.000000 wyoming_piper-1.1.0/wyoming_piper.egg-info/dependency_links.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       15 2023-07-17 16:10:40.000000 wyoming_piper-1.1.0/wyoming_piper.egg-info/requires.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       14 2023-07-17 16:10:40.000000 wyoming_piper-1.1.0/wyoming_piper.egg-info/top_level.txt
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-08-01 21:59:03.072263 wyoming_piper-1.2.0/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       59 2023-07-17 16:41:50.000000 wyoming_piper-1.2.0/MANIFEST.in
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      666 2023-08-01 21:59:03.072263 wyoming_piper-1.2.0/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       15 2023-07-17 16:41:50.000000 wyoming_piper-1.2.0/requirements.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       38 2023-08-01 21:59:03.072263 wyoming_piper-1.2.0/setup.cfg
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1392 2023-08-01 21:23:47.000000 wyoming_piper-1.2.0/setup.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-08-01 21:59:03.072263 wyoming_piper-1.2.0/wyoming_piper/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       32 2023-04-21 15:28:34.000000 wyoming_piper-1.2.0/wyoming_piper/__init__.py
+-rwxr-xr-x   0 hansenm   (1000) hansenm   (1000)     4773 2023-07-17 16:41:50.000000 wyoming_piper-1.2.0/wyoming_piper/__main__.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1015 2023-04-21 15:28:34.000000 wyoming_piper-1.2.0/wyoming_piper/const.py
+-rwxr-xr-x   0 hansenm   (1000) hansenm   (1000)     3866 2023-07-17 16:41:50.000000 wyoming_piper-1.2.0/wyoming_piper/download.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1107 2023-05-10 19:58:23.000000 wyoming_piper-1.2.0/wyoming_piper/file_hash.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4603 2023-07-17 16:41:50.000000 wyoming_piper-1.2.0/wyoming_piper/handler.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5835 2023-08-01 21:58:49.000000 wyoming_piper-1.2.0/wyoming_piper/process.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)   123793 2023-08-01 21:52:01.000000 wyoming_piper-1.2.0/wyoming_piper/voices.json
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-08-01 21:59:03.072263 wyoming_piper-1.2.0/wyoming_piper.egg-info/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      666 2023-08-01 21:59:03.000000 wyoming_piper-1.2.0/wyoming_piper.egg-info/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      425 2023-08-01 21:59:03.000000 wyoming_piper-1.2.0/wyoming_piper.egg-info/SOURCES.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-08-01 21:59:03.000000 wyoming_piper-1.2.0/wyoming_piper.egg-info/dependency_links.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       15 2023-08-01 21:59:03.000000 wyoming_piper-1.2.0/wyoming_piper.egg-info/requires.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       14 2023-08-01 21:59:03.000000 wyoming_piper-1.2.0/wyoming_piper.egg-info/top_level.txt
```

### Comparing `wyoming_piper-1.1.0/PKG-INFO` & `wyoming_piper-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: wyoming_piper
-Version: 1.1.0
+Version: 1.2.0
 Summary: Wyoming Server for Piper
 Home-page: http://github.com/rhasspy/rhasspy3
 Author: Michael Hansen
 Author-email: mike@rhasspy.org
 License: MIT
 Description: UNKNOWN
 Keywords: rhasspy wyoming piper
```

### Comparing `wyoming_piper-1.1.0/setup.py` & `wyoming_piper-1.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 data_files = [module_dir / "voices.json"]
 
 # -----------------------------------------------------------------------------
 
 setup(
     name="wyoming_piper",
-    version="1.1.0",
+    version="1.2.0",
     description="Wyoming Server for Piper",
     url="http://github.com/rhasspy/rhasspy3",
     author="Michael Hansen",
     author_email="mike@rhasspy.org",
     license="MIT",
     packages=setuptools.find_packages(),
     package_data={
```

### Comparing `wyoming_piper-1.1.0/wyoming_piper/__main__.py` & `wyoming_piper-1.2.0/wyoming_piper/__main__.py`

 * *Files identical despite different names*

### Comparing `wyoming_piper-1.1.0/wyoming_piper/const.py` & `wyoming_piper-1.2.0/wyoming_piper/const.py`

 * *Files identical despite different names*

### Comparing `wyoming_piper-1.1.0/wyoming_piper/download.py` & `wyoming_piper-1.2.0/wyoming_piper/download.py`

 * *Files identical despite different names*

### Comparing `wyoming_piper-1.1.0/wyoming_piper/file_hash.py` & `wyoming_piper-1.2.0/wyoming_piper/file_hash.py`

 * *Files identical despite different names*

### Comparing `wyoming_piper-1.1.0/wyoming_piper/handler.py` & `wyoming_piper-1.2.0/wyoming_piper/handler.py`

 * *Files identical despite different names*

### Comparing `wyoming_piper-1.1.0/wyoming_piper/process.py` & `wyoming_piper-1.2.0/wyoming_piper/process.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,15 +79,18 @@
 
         # Resolve alias
         voice_info = self.voices_info.get(voice_name, {})
         voice_name = voice_info.get("key", voice_name)
         assert voice_name is not None
 
         piper_proc = self.processes.get(voice_name)
-        if piper_proc is None:
+        if (piper_proc is None) or (piper_proc.proc.returncode is not None):
+            # Remove if stopped
+            self.processes.pop(voice_name, None)
+
             # Start new Piper process
             if self.args.max_piper_procs > 0:
                 # Restrict number of running processes
                 while len(self.processes) >= self.args.max_piper_procs:
                     # Stop least recently used process
                     lru_proc_name, lru_proc = sorted(
                         self.processes.items(), key=lambda kv: kv[1].last_used
```

### Comparing `wyoming_piper-1.1.0/wyoming_piper/voices.json` & `wyoming_piper-1.2.0/wyoming_piper/voices.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9222222222222223%*

 * *Differences: {"'de_DE-thorsten_emotional-medium'": "OrderedDict([('key', 'de_DE-thorsten_emotional-medium'), "*

 * *                                      "('name', 'thorsten_emotional'), ('language', "*

 * *                                      "OrderedDict([('code', 'de_DE'), ('family', 'de'), "*

 * *                                      "('region', 'DE'), ('name_native', 'Deutsch'), "*

 * *                                      "('name_english', 'German'), ('country_english', "*

 * *                                      "'Germany')])), ('quali […]*

```diff
@@ -343,14 +343,53 @@
             "region": "DE"
         },
         "name": "thorsten",
         "num_speakers": 1,
         "quality": "medium",
         "speaker_id_map": {}
     },
+    "de_DE-thorsten_emotional-medium": {
+        "aliases": [],
+        "files": {
+            "de/de_DE/thorsten_emotional/medium/MODEL_CARD": {
+                "md5_digest": "91874c31e5b2e497ecda2ea8e6fda4a7",
+                "size_bytes": 302
+            },
+            "de/de_DE/thorsten_emotional/medium/de_DE-thorsten_emotional-medium.onnx": {
+                "md5_digest": "7cc67d24d9d0b34d7a4f6224d16236b9",
+                "size_bytes": 76745905
+            },
+            "de/de_DE/thorsten_emotional/medium/de_DE-thorsten_emotional-medium.onnx.json": {
+                "md5_digest": "1abac7e46522f774217c170da222f2a6",
+                "size_bytes": 5031
+            }
+        },
+        "key": "de_DE-thorsten_emotional-medium",
+        "language": {
+            "code": "de_DE",
+            "country_english": "Germany",
+            "family": "de",
+            "name_english": "German",
+            "name_native": "Deutsch",
+            "region": "DE"
+        },
+        "name": "thorsten_emotional",
+        "num_speakers": 8,
+        "quality": "medium",
+        "speaker_id_map": {
+            "amused": 0,
+            "angry": 1,
+            "disgusted": 2,
+            "drunk": 3,
+            "neutral": 4,
+            "sleepy": 5,
+            "surprised": 6,
+            "whisper": 7
+        }
+    },
     "el_GR-rapunzelina-low": {
         "aliases": [],
         "files": {
             "el/el_GR/rapunzelina/low/MODEL_CARD": {
                 "md5_digest": "c75270b41e7bf60dacd351753a483574",
                 "size_bytes": 303
             },
@@ -568,14 +607,49 @@
             "region": "GB"
         },
         "name": "northern_english_male",
         "num_speakers": 1,
         "quality": "medium",
         "speaker_id_map": {}
     },
+    "en_GB-semaine-medium": {
+        "aliases": [],
+        "files": {
+            "en/en_GB/semaine/medium/MODEL_CARD": {
+                "md5_digest": "340045a0ec470eaf3bec271ea746f946",
+                "size_bytes": 332
+            },
+            "en/en_GB/semaine/medium/en_GB-semaine-medium.onnx": {
+                "md5_digest": "3634c3b388165d3b698ea07ba3cac7d2",
+                "size_bytes": 76737711
+            },
+            "en/en_GB/semaine/medium/en_GB-semaine-medium.onnx.json": {
+                "md5_digest": "c30f92604f6ce3f378e7211440f13c8f",
+                "size_bytes": 5076
+            }
+        },
+        "key": "en_GB-semaine-medium",
+        "language": {
+            "code": "en_GB",
+            "country_english": "Great Britain",
+            "family": "en",
+            "name_english": "English",
+            "name_native": "English",
+            "region": "GB"
+        },
+        "name": "semaine",
+        "num_speakers": 4,
+        "quality": "medium",
+        "speaker_id_map": {
+            "obadiah": 2,
+            "poppy": 3,
+            "prudence": 0,
+            "spike": 1
+        }
+    },
     "en_GB-southern_english_female-low": {
         "aliases": [
             "en-gb-southern_english_female-low"
         ],
         "files": {
             "en/en_GB/southern_english_female/low/MODEL_CARD": {
                 "md5_digest": "77ac998c8b37842ef98594567f141629",
@@ -2534,14 +2608,47 @@
             "region": "FR"
         },
         "name": "siwis",
         "num_speakers": 1,
         "quality": "medium",
         "speaker_id_map": {}
     },
+    "fr_FR-upmc-medium": {
+        "aliases": [],
+        "files": {
+            "fr/fr_FR/upmc/medium/MODEL_CARD": {
+                "md5_digest": "9a49df5c79d89290ac626ebe08f05830",
+                "size_bytes": 316
+            },
+            "fr/fr_FR/upmc/medium/fr_FR-upmc-medium.onnx": {
+                "md5_digest": "6837ede9408c7e1b39fa4a126af9e865",
+                "size_bytes": 76733615
+            },
+            "fr/fr_FR/upmc/medium/fr_FR-upmc-medium.onnx.json": {
+                "md5_digest": "574571ae93aba72dbd159582981037da",
+                "size_bytes": 4996
+            }
+        },
+        "key": "fr_FR-upmc-medium",
+        "language": {
+            "code": "fr_FR",
+            "country_english": "France",
+            "family": "fr",
+            "name_english": "French",
+            "name_native": "Fran\u00e7ais",
+            "region": "FR"
+        },
+        "name": "upmc",
+        "num_speakers": 2,
+        "quality": "medium",
+        "speaker_id_map": {
+            "jessica": 0,
+            "pierre": 1
+        }
+    },
     "is_IS-bui-medium": {
         "aliases": [
             "is-bui-medium"
         ],
         "files": {
             "is/is_IS/bui/medium/MODEL_CARD": {
                 "md5_digest": "a055aad199d8cc58e52913ff2af461d8",
@@ -2827,14 +2934,44 @@
             "region": "KZ"
         },
         "name": "raya",
         "num_speakers": 1,
         "quality": "x_low",
         "speaker_id_map": {}
     },
+    "lb_LU-marylux-medium": {
+        "aliases": [],
+        "files": {
+            "lb/lb_LU/marylux/medium/MODEL_CARD": {
+                "md5_digest": "1eeb3d600789cdd8b3f23866023d8543",
+                "size_bytes": 330
+            },
+            "lb/lb_LU/marylux/medium/lb_LU-marylux-medium.onnx": {
+                "md5_digest": "966856e665a46cee45cb0cd2c475f8d5",
+                "size_bytes": 63201294
+            },
+            "lb/lb_LU/marylux/medium/lb_LU-marylux-medium.onnx.json": {
+                "md5_digest": "aea98b0e4fecaa0b3b7adc2048561095",
+                "size_bytes": 4979
+            }
+        },
+        "key": "lb_LU-marylux-medium",
+        "language": {
+            "code": "lb_LU",
+            "country_english": "Luxembourg",
+            "family": "lb",
+            "name_english": "Luxembourgish",
+            "name_native": "L\u00ebtzebuergesch",
+            "region": "LU"
+        },
+        "name": "marylux",
+        "num_speakers": 1,
+        "quality": "medium",
+        "speaker_id_map": {}
+    },
     "ne_NP-google-medium": {
         "aliases": [
             "ne-google-medium"
         ],
         "files": {
             "ne/ne_NP/google/medium/MODEL_CARD": {
                 "md5_digest": "afe022ba061870d0c9fe085fe9a9f31f",
@@ -3305,14 +3442,44 @@
             "region": "BR"
         },
         "name": "faber",
         "num_speakers": 1,
         "quality": "medium",
         "speaker_id_map": {}
     },
+    "ro_RO-mihai-medium": {
+        "aliases": [],
+        "files": {
+            "ro/ro_RO/mihai/medium/MODEL_CARD": {
+                "md5_digest": "4075864685b207c9a98bf1af237a1502",
+                "size_bytes": 277
+            },
+            "ro/ro_RO/mihai/medium/ro_RO-mihai-medium.onnx": {
+                "md5_digest": "45f4253916c93d3d05ad3fe1b07ea4f3",
+                "size_bytes": 63201294
+            },
+            "ro/ro_RO/mihai/medium/ro_RO-mihai-medium.onnx.json": {
+                "md5_digest": "f820f8ba65a8646c68792be581b85144",
+                "size_bytes": 4877
+            }
+        },
+        "key": "ro_RO-mihai-medium",
+        "language": {
+            "code": "ro_RO",
+            "country_english": "Romania",
+            "family": "ro",
+            "name_english": "Romanian",
+            "name_native": "Rom\u00e2n\u0103",
+            "region": "RO"
+        },
+        "name": "mihai",
+        "num_speakers": 1,
+        "quality": "medium",
+        "speaker_id_map": {}
+    },
     "ru_RU-denis-medium": {
         "aliases": [],
         "files": {
             "ru/ru_RU/denis/medium/MODEL_CARD": {
                 "md5_digest": "6fe09e0e097e4538809cc420653974e4",
                 "size_bytes": 275
             },
@@ -3427,14 +3594,47 @@
             "region": "RU"
         },
         "name": "ruslan",
         "num_speakers": 1,
         "quality": "medium",
         "speaker_id_map": {}
     },
+    "sr_RS-serbski_institut-medium": {
+        "aliases": [],
+        "files": {
+            "sr/sr_RS/serbski_institut/medium/MODEL_CARD": {
+                "md5_digest": "407a5b8ebef4877405de2e89eb806633",
+                "size_bytes": 343
+            },
+            "sr/sr_RS/serbski_institut/medium/sr_RS-serbski_institut-medium.onnx": {
+                "md5_digest": "02c6e27ac7b4dfa84272df89edca9feb",
+                "size_bytes": 76733615
+            },
+            "sr/sr_RS/serbski_institut/medium/sr_RS-serbski_institut-medium.onnx.json": {
+                "md5_digest": "dacee7595352af9b4d78bb42237bd759",
+                "size_bytes": 4999
+            }
+        },
+        "key": "sr_RS-serbski_institut-medium",
+        "language": {
+            "code": "sr_RS",
+            "country_english": "Serbia",
+            "family": "sr",
+            "name_english": "Serbian",
+            "name_native": "srpski",
+            "region": "RS"
+        },
+        "name": "serbski_institut",
+        "num_speakers": 2,
+        "quality": "medium",
+        "speaker_id_map": {
+            "dsb": 0,
+            "hsb": 1
+        }
+    },
     "sv_SE-nst-medium": {
         "aliases": [],
         "files": {
             "sv/sv_SE/nst/medium/MODEL_CARD": {
                 "md5_digest": "4a7cdb8f218a909b2b5e81d1903628da",
                 "size_bytes": 306
             },
@@ -3487,14 +3687,44 @@
             "region": "CD"
         },
         "name": "lanfrica",
         "num_speakers": 1,
         "quality": "medium",
         "speaker_id_map": {}
     },
+    "tr_TR-dfki-medium": {
+        "aliases": [],
+        "files": {
+            "tr/tr_TR/dfki/medium/MODEL_CARD": {
+                "md5_digest": "870d6bc19719328699449cb7b4dd56cf",
+                "size_bytes": 319
+            },
+            "tr/tr_TR/dfki/medium/tr_TR-dfki-medium.onnx": {
+                "md5_digest": "f51287b350a042dd8d67b2b215145e5a",
+                "size_bytes": 63201294
+            },
+            "tr/tr_TR/dfki/medium/tr_TR-dfki-medium.onnx.json": {
+                "md5_digest": "683c97d5bf7588abb4d7b9ff556c9466",
+                "size_bytes": 4960
+            }
+        },
+        "key": "tr_TR-dfki-medium",
+        "language": {
+            "code": "tr_TR",
+            "country_english": "Turkey",
+            "family": "tr",
+            "name_english": "Turkish",
+            "name_native": "T\u00fcrk\u00e7e",
+            "region": "TR"
+        },
+        "name": "dfki",
+        "num_speakers": 1,
+        "quality": "medium",
+        "speaker_id_map": {}
+    },
     "uk_UA-lada-x_low": {
         "aliases": [
             "uk-lada-x-low"
         ],
         "files": {
             "uk/uk_UA/lada/x_low/MODEL_CARD": {
                 "md5_digest": "8de03ca7a0aee2a1c088638ec18fdb87",
```

### Comparing `wyoming_piper-1.1.0/wyoming_piper.egg-info/PKG-INFO` & `wyoming_piper-1.2.0/wyoming_piper.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: wyoming-piper
-Version: 1.1.0
+Version: 1.2.0
 Summary: Wyoming Server for Piper
 Home-page: http://github.com/rhasspy/rhasspy3
 Author: Michael Hansen
 Author-email: mike@rhasspy.org
 License: MIT
 Description: UNKNOWN
 Keywords: rhasspy wyoming piper
```

