# Comparing `tmp/spl_widgets-1.7.5.tar.gz` & `tmp/spl_widgets-1.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spl_widgets-1.7.5.tar", last modified: Fri Jul 28 18:55:43 2023, max compression
+gzip compressed data, was "spl_widgets-1.7.6.tar", last modified: Tue Aug  1 22:08:00 2023, max compression
```

## Comparing `spl_widgets-1.7.5.tar` & `spl_widgets-1.7.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-28 18:55:43.345169 spl_widgets-1.7.5/
--rw-r--r--   0 colin      (501) staff       (20)     1073 2021-11-03 16:44:37.000000 spl_widgets-1.7.5/LICENSE
--rw-r--r--   0 colin      (501) staff       (20)      411 2023-07-28 18:55:43.345029 spl_widgets-1.7.5/PKG-INFO
--rw-r--r--   0 colin      (501) staff       (20)     2101 2022-06-26 15:02:40.000000 spl_widgets-1.7.5/README.md
--rw-r--r--   0 colin      (501) staff       (20)      103 2021-11-03 16:36:22.000000 spl_widgets-1.7.5/pyproject.toml
--rw-r--r--   0 colin      (501) staff       (20)       38 2023-07-28 18:55:43.345208 spl_widgets-1.7.5/setup.cfg
--rw-r--r--   0 colin      (501) staff       (20)     1240 2023-07-28 18:54:56.000000 spl_widgets-1.7.5/setup.py
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-28 18:55:43.330898 spl_widgets-1.7.5/src/
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-28 18:55:43.334104 spl_widgets-1.7.5/src/spl_widgets/
--rw-r--r--   0 colin      (501) staff       (20)      279 2022-06-26 16:32:08.000000 spl_widgets-1.7.5/src/spl_widgets/__init__.py
--rw-r--r--   0 colin      (501) staff       (20)        0 2022-06-26 14:59:05.000000 spl_widgets-1.7.5/src/spl_widgets/__main__.py
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-28 18:55:43.335874 spl_widgets-1.7.5/src/spl_widgets/autoscorer/
--rw-r--r--   0 colin      (501) staff       (20)    15383 2023-07-27 21:36:42.000000 spl_widgets-1.7.5/src/spl_widgets/autoscorer/autoscore.py
--rw-r--r--   0 colin      (501) staff       (20)    18830 2023-07-27 18:42:32.000000 spl_widgets-1.7.5/src/spl_widgets/autoscorer/autoscorer_gui.py
--rw-r--r--   0 colin      (501) staff       (20)     5361 2023-07-28 18:55:30.000000 spl_widgets-1.7.5/src/spl_widgets/autoscorer/tokenize_to_ipa.py
--rw-r--r--   0 colin      (501) staff       (20)     3722 2023-05-26 16:24:48.000000 spl_widgets-1.7.5/src/spl_widgets/batch_tune.py
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-28 18:55:43.342174 spl_widgets-1.7.5/src/spl_widgets/data/
--rw-r--r--   0 colin      (501) staff       (20)  9670656 2023-05-26 16:25:12.000000 spl_widgets-1.7.5/src/spl_widgets/data/cmudict.sqlite
--rw-r--r--   0 colin      (501) staff       (20)       73 2023-07-26 16:35:15.000000 spl_widgets-1.7.5/src/spl_widgets/data/help_text.json
--rwxr-xr-x   0 colin      (501) staff       (20)     5378 2022-10-21 13:14:40.000000 spl_widgets-1.7.5/src/spl_widgets/gorilla_clean.py
--rw-r--r--   0 colin      (501) staff       (20)     2483 2022-12-17 21:45:28.000000 spl_widgets-1.7.5/src/spl_widgets/jukemake.py
--rw-r--r--   0 colin      (501) staff       (20)     4166 2023-05-25 22:28:36.000000 spl_widgets-1.7.5/src/spl_widgets/misc_util.py
--rwxr-xr-x   0 colin      (501) staff       (20)     3598 2023-04-14 19:27:21.000000 spl_widgets-1.7.5/src/spl_widgets/stk_swx.py
--rw-r--r--   0 colin      (501) staff       (20)     3614 2023-04-23 14:58:27.000000 spl_widgets-1.7.5/src/spl_widgets/tune_freq.py
--rw-r--r--   0 colin      (501) staff       (20)    17694 2023-05-26 16:20:21.000000 spl_widgets-1.7.5/src/spl_widgets/tuner.py
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-28 18:55:43.344797 spl_widgets-1.7.5/src/spl_widgets/util/
--rw-r--r--   0 colin      (501) staff       (20)     1169 2023-07-10 17:51:43.000000 spl_widgets-1.7.5/src/spl_widgets/util/color_util.py
--rw-r--r--   0 colin      (501) staff       (20)     5635 2023-07-26 16:35:15.000000 spl_widgets-1.7.5/src/spl_widgets/util/gui_util.py
--rw-r--r--   0 colin      (501) staff       (20)     3642 2023-05-26 16:25:13.000000 spl_widgets-1.7.5/src/spl_widgets/util/sqlite_db.py
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-28 18:55:43.335057 spl_widgets-1.7.5/src/spl_widgets.egg-info/
--rw-r--r--   0 colin      (501) staff       (20)      411 2023-07-28 18:55:43.000000 spl_widgets-1.7.5/src/spl_widgets.egg-info/PKG-INFO
--rw-r--r--   0 colin      (501) staff       (20)      839 2023-07-28 18:55:43.000000 spl_widgets-1.7.5/src/spl_widgets.egg-info/SOURCES.txt
--rw-r--r--   0 colin      (501) staff       (20)        1 2023-07-28 18:55:43.000000 spl_widgets-1.7.5/src/spl_widgets.egg-info/dependency_links.txt
--rw-r--r--   0 colin      (501) staff       (20)      265 2023-07-28 18:55:43.000000 spl_widgets-1.7.5/src/spl_widgets.egg-info/entry_points.txt
--rw-r--r--   0 colin      (501) staff       (20)       43 2023-07-28 18:55:43.000000 spl_widgets-1.7.5/src/spl_widgets.egg-info/requires.txt
--rw-r--r--   0 colin      (501) staff       (20)       12 2023-07-28 18:55:43.000000 spl_widgets-1.7.5/src/spl_widgets.egg-info/top_level.txt
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-08-01 22:08:00.934139 spl_widgets-1.7.6/
+-rw-r--r--   0 colin      (501) staff       (20)     1073 2021-11-03 16:44:37.000000 spl_widgets-1.7.6/LICENSE
+-rw-r--r--   0 colin      (501) staff       (20)      411 2023-08-01 22:08:00.934006 spl_widgets-1.7.6/PKG-INFO
+-rw-r--r--   0 colin      (501) staff       (20)     2101 2022-06-26 15:02:40.000000 spl_widgets-1.7.6/README.md
+-rw-r--r--   0 colin      (501) staff       (20)      103 2021-11-03 16:36:22.000000 spl_widgets-1.7.6/pyproject.toml
+-rw-r--r--   0 colin      (501) staff       (20)       38 2023-08-01 22:08:00.934177 spl_widgets-1.7.6/setup.cfg
+-rw-r--r--   0 colin      (501) staff       (20)     1240 2023-08-01 22:07:48.000000 spl_widgets-1.7.6/setup.py
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-08-01 22:08:00.923301 spl_widgets-1.7.6/src/
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-08-01 22:08:00.925360 spl_widgets-1.7.6/src/spl_widgets/
+-rw-r--r--   0 colin      (501) staff       (20)      279 2022-06-26 16:32:08.000000 spl_widgets-1.7.6/src/spl_widgets/__init__.py
+-rw-r--r--   0 colin      (501) staff       (20)        0 2022-06-26 14:59:05.000000 spl_widgets-1.7.6/src/spl_widgets/__main__.py
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-08-01 22:08:00.926826 spl_widgets-1.7.6/src/spl_widgets/autoscorer/
+-rw-r--r--   0 colin      (501) staff       (20)    15499 2023-08-01 22:06:41.000000 spl_widgets-1.7.6/src/spl_widgets/autoscorer/autoscore.py
+-rw-r--r--   0 colin      (501) staff       (20)    18830 2023-08-01 22:03:45.000000 spl_widgets-1.7.6/src/spl_widgets/autoscorer/autoscorer_gui.py
+-rw-r--r--   0 colin      (501) staff       (20)     5369 2023-07-28 19:15:27.000000 spl_widgets-1.7.6/src/spl_widgets/autoscorer/tokenize_to_ipa.py
+-rw-r--r--   0 colin      (501) staff       (20)     3722 2023-05-26 16:24:48.000000 spl_widgets-1.7.6/src/spl_widgets/batch_tune.py
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-08-01 22:08:00.933422 spl_widgets-1.7.6/src/spl_widgets/data/
+-rw-r--r--   0 colin      (501) staff       (20)  9670656 2023-05-26 16:25:12.000000 spl_widgets-1.7.6/src/spl_widgets/data/cmudict.sqlite
+-rw-r--r--   0 colin      (501) staff       (20)       73 2023-07-26 16:35:15.000000 spl_widgets-1.7.6/src/spl_widgets/data/help_text.json
+-rwxr-xr-x   0 colin      (501) staff       (20)     5378 2022-10-21 13:14:40.000000 spl_widgets-1.7.6/src/spl_widgets/gorilla_clean.py
+-rw-r--r--   0 colin      (501) staff       (20)     2483 2022-12-17 21:45:28.000000 spl_widgets-1.7.6/src/spl_widgets/jukemake.py
+-rw-r--r--   0 colin      (501) staff       (20)     4166 2023-05-25 22:28:36.000000 spl_widgets-1.7.6/src/spl_widgets/misc_util.py
+-rwxr-xr-x   0 colin      (501) staff       (20)     3598 2023-04-14 19:27:21.000000 spl_widgets-1.7.6/src/spl_widgets/stk_swx.py
+-rw-r--r--   0 colin      (501) staff       (20)     3614 2023-04-23 14:58:27.000000 spl_widgets-1.7.6/src/spl_widgets/tune_freq.py
+-rw-r--r--   0 colin      (501) staff       (20)    17694 2023-05-26 16:20:21.000000 spl_widgets-1.7.6/src/spl_widgets/tuner.py
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-08-01 22:08:00.933835 spl_widgets-1.7.6/src/spl_widgets/util/
+-rw-r--r--   0 colin      (501) staff       (20)     1169 2023-07-10 17:51:43.000000 spl_widgets-1.7.6/src/spl_widgets/util/color_util.py
+-rw-r--r--   0 colin      (501) staff       (20)     5635 2023-07-26 16:35:15.000000 spl_widgets-1.7.6/src/spl_widgets/util/gui_util.py
+-rw-r--r--   0 colin      (501) staff       (20)     3642 2023-05-26 16:25:13.000000 spl_widgets-1.7.6/src/spl_widgets/util/sqlite_db.py
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-08-01 22:08:00.926384 spl_widgets-1.7.6/src/spl_widgets.egg-info/
+-rw-r--r--   0 colin      (501) staff       (20)      411 2023-08-01 22:08:00.000000 spl_widgets-1.7.6/src/spl_widgets.egg-info/PKG-INFO
+-rw-r--r--   0 colin      (501) staff       (20)      839 2023-08-01 22:08:00.000000 spl_widgets-1.7.6/src/spl_widgets.egg-info/SOURCES.txt
+-rw-r--r--   0 colin      (501) staff       (20)        1 2023-08-01 22:08:00.000000 spl_widgets-1.7.6/src/spl_widgets.egg-info/dependency_links.txt
+-rw-r--r--   0 colin      (501) staff       (20)      265 2023-08-01 22:08:00.000000 spl_widgets-1.7.6/src/spl_widgets.egg-info/entry_points.txt
+-rw-r--r--   0 colin      (501) staff       (20)       43 2023-08-01 22:08:00.000000 spl_widgets-1.7.6/src/spl_widgets.egg-info/requires.txt
+-rw-r--r--   0 colin      (501) staff       (20)       12 2023-08-01 22:08:00.000000 spl_widgets-1.7.6/src/spl_widgets.egg-info/top_level.txt
```

### Comparing `spl_widgets-1.7.5/LICENSE` & `spl_widgets-1.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.5/README.md` & `spl_widgets-1.7.6/README.md`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.5/setup.py` & `spl_widgets-1.7.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 # with open("README.md", "r", encoding="utf-8") as fh:
 #     long_description = fh.read()
 
 setuptools.setup(
     name="spl_widgets",
-    version="1.7.5",
+    version="1.7.6",
     author="Colin Simon-Fellowes",
     author_email="colin.tsf@gmail.com",
     description="Widgets for the Barnard Speech Perception Laboratory",
     # long_description=long_description,
     # long_description_content_type="text/markdown",
     url="https://github.com/clntsf/spl_widgets",
     classifiers=[
```

### Comparing `spl_widgets-1.7.5/src/spl_widgets/autoscorer/autoscore.py` & `spl_widgets-1.7.6/src/spl_widgets/autoscorer/autoscore.py`

 * *Files 1% similar despite different names*

```diff
@@ -377,14 +377,17 @@
     outpath = Path(out_dir, f"{out_fn}.xlsx")
     wb.save(outpath)
 
     dfs = {}
 
     with pd.ExcelWriter(Path(out_dir, f"{out_fn}_PER_SEGMENT.xlsx"), engine="openpyxl") as writer:
         for (i, (sentence,scores)) in enumerate(user_sentence_phoneme_scores.items()):
+            avg = lambda l: round(sum(l)/len(l), 2)
+            scores["AVG"] = [*map(avg, zip(*scores.values()))]
+
             tokens = [*filter(str.isalpha, sentence_ipas[i])]
             df = pd.DataFrame(scores, index=tokens).T
         
             df.to_excel(writer, sheet_name=sentence[:31])
     
 if __name__ == "__main__":
     main()
```

### Comparing `spl_widgets-1.7.5/src/spl_widgets/autoscorer/autoscorer_gui.py` & `spl_widgets-1.7.6/src/spl_widgets/autoscorer/autoscorer_gui.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.5/src/spl_widgets/autoscorer/tokenize_to_ipa.py` & `spl_widgets-1.7.6/src/spl_widgets/autoscorer/tokenize_to_ipa.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,10 +163,10 @@
     arpa_words = to_arpabet(sentence, keep_punct)
     return arpa_to_ipa(arpa_words)
 
 # breaks up an idealized IPA string into tokens (might not be perfect, but it's definitely
 # mostly good, and worst case we just switch to passing them as a lists of tokens)
 def tokenize_ipa(ipa_str: str) -> list[str]:
     tokens = sorted(phonemes.values(), key=len, reverse=True)   # prioritize finding diphthongs
-    token_re = rf"({'|'.join(tokens)}|\s|.)"
+    token_re = rf"({'|'.join(tokens)}|\s|\*[\w\']*)"
 
     return re.findall(token_re, ipa_str)
```

### Comparing `spl_widgets-1.7.5/src/spl_widgets/batch_tune.py` & `spl_widgets-1.7.6/src/spl_widgets/batch_tune.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.5/src/spl_widgets/data/cmudict.sqlite` & `spl_widgets-1.7.6/src/spl_widgets/data/cmudict.sqlite`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.5/src/spl_widgets/gorilla_clean.py` & `spl_widgets-1.7.6/src/spl_widgets/gorilla_clean.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.5/src/spl_widgets/jukemake.py` & `spl_widgets-1.7.6/src/spl_widgets/jukemake.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.5/src/spl_widgets/misc_util.py` & `spl_widgets-1.7.6/src/spl_widgets/misc_util.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.5/src/spl_widgets/stk_swx.py` & `spl_widgets-1.7.6/src/spl_widgets/stk_swx.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.5/src/spl_widgets/tune_freq.py` & `spl_widgets-1.7.6/src/spl_widgets/tune_freq.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.5/src/spl_widgets/tuner.py` & `spl_widgets-1.7.6/src/spl_widgets/tuner.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.5/src/spl_widgets/util/color_util.py` & `spl_widgets-1.7.6/src/spl_widgets/util/color_util.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.5/src/spl_widgets/util/gui_util.py` & `spl_widgets-1.7.6/src/spl_widgets/util/gui_util.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.5/src/spl_widgets/util/sqlite_db.py` & `spl_widgets-1.7.6/src/spl_widgets/util/sqlite_db.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.5/src/spl_widgets.egg-info/SOURCES.txt` & `spl_widgets-1.7.6/src/spl_widgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

