# Comparing `tmp/decryptogame-1.0.2.tar.gz` & `tmp/decryptogame-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decryptogame-1.0.2.tar", last modified: Mon Jul 31 04:31:47 2023, max compression
+gzip compressed data, was "decryptogame-1.0.3.tar", last modified: Wed Aug  2 00:47:54 2023, max compression
```

## Comparing `decryptogame-1.0.2.tar` & `decryptogame-1.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 jadenrodriguez   (501) staff       (20)        0 2023-07-31 04:31:47.717971 decryptogame-1.0.2/
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)    35149 2023-06-02 04:55:47.000000 decryptogame-1.0.2/LICENSE
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)     1431 2023-07-31 04:31:47.716452 decryptogame-1.0.2/PKG-INFO
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)      836 2023-07-31 04:29:08.000000 decryptogame-1.0.2/README.md
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)      773 2023-07-31 04:30:17.000000 decryptogame-1.0.2/pyproject.toml
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)       38 2023-07-31 04:31:47.719583 decryptogame-1.0.2/setup.cfg
-drwxr-xr-x   0 jadenrodriguez   (501) staff       (20)        0 2023-07-31 04:31:47.643967 decryptogame-1.0.2/src/
-drwxr-xr-x   0 jadenrodriguez   (501) staff       (20)        0 2023-07-31 04:31:47.664270 decryptogame-1.0.2/src/decryptogame/
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)      965 2023-07-31 00:17:58.000000 decryptogame-1.0.2/src/decryptogame/__init__.py
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)     2502 2023-07-30 23:48:46.000000 decryptogame-1.0.2/src/decryptogame/components.py
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)     7193 2023-07-29 07:49:55.000000 decryptogame-1.0.2/src/decryptogame/end_criteria.py
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)     6833 2023-07-30 20:42:07.000000 decryptogame-1.0.2/src/decryptogame/game.py
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)     3627 2023-07-29 07:56:45.000000 decryptogame-1.0.2/src/decryptogame/generators.py
-drwxr-xr-x   0 jadenrodriguez   (501) staff       (20)        0 2023-07-31 04:31:47.674232 decryptogame-1.0.2/src/decryptogame/official_words/
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)     4745 2023-07-29 06:33:23.000000 decryptogame-1.0.2/src/decryptogame/official_words/english.py
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)     3726 2023-07-30 21:52:49.000000 decryptogame-1.0.2/src/decryptogame/play.py
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)     8570 2023-07-31 00:12:46.000000 decryptogame-1.0.2/src/decryptogame/teams.py
-drwxr-xr-x   0 jadenrodriguez   (501) staff       (20)        0 2023-07-31 04:31:47.673641 decryptogame-1.0.2/src/decryptogame.egg-info/
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)     1431 2023-07-31 04:31:47.000000 decryptogame-1.0.2/src/decryptogame.egg-info/PKG-INFO
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)      504 2023-07-31 04:31:47.000000 decryptogame-1.0.2/src/decryptogame.egg-info/SOURCES.txt
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)        1 2023-07-31 04:31:47.000000 decryptogame-1.0.2/src/decryptogame.egg-info/dependency_links.txt
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)       13 2023-07-31 04:31:47.000000 decryptogame-1.0.2/src/decryptogame.egg-info/top_level.txt
-drwxr-xr-x   0 jadenrodriguez   (501) staff       (20)        0 2023-07-31 04:31:47.679570 decryptogame-1.0.2/tests/
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)     1468 2023-07-29 05:55:47.000000 decryptogame-1.0.2/tests/test_components.py
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)     3926 2023-07-30 20:48:01.000000 decryptogame-1.0.2/tests/test_game.py
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)      943 2023-07-29 07:15:17.000000 decryptogame-1.0.2/tests/test_generators.py
+drwxr-xr-x   0 jadenrodriguez   (501) staff       (20)        0 2023-08-02 00:47:54.417050 decryptogame-1.0.3/
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)    35149 2023-06-02 04:55:47.000000 decryptogame-1.0.3/LICENSE
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)     1431 2023-08-02 00:47:54.415370 decryptogame-1.0.3/PKG-INFO
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)      836 2023-07-31 04:29:08.000000 decryptogame-1.0.3/README.md
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)      773 2023-08-02 00:37:58.000000 decryptogame-1.0.3/pyproject.toml
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)       38 2023-08-02 00:47:54.417280 decryptogame-1.0.3/setup.cfg
+drwxr-xr-x   0 jadenrodriguez   (501) staff       (20)        0 2023-08-02 00:47:54.375169 decryptogame-1.0.3/src/
+drwxr-xr-x   0 jadenrodriguez   (501) staff       (20)        0 2023-08-02 00:47:54.398301 decryptogame-1.0.3/src/decryptogame/
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)      965 2023-07-31 00:17:58.000000 decryptogame-1.0.3/src/decryptogame/__init__.py
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)     2410 2023-08-02 00:42:06.000000 decryptogame-1.0.3/src/decryptogame/components.py
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)     7193 2023-07-29 07:49:55.000000 decryptogame-1.0.3/src/decryptogame/end_criteria.py
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)     6833 2023-07-30 20:42:07.000000 decryptogame-1.0.3/src/decryptogame/game.py
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)     3664 2023-08-02 00:43:08.000000 decryptogame-1.0.3/src/decryptogame/generators.py
+drwxr-xr-x   0 jadenrodriguez   (501) staff       (20)        0 2023-08-02 00:47:54.405909 decryptogame-1.0.3/src/decryptogame/official_words/
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)     4745 2023-07-29 06:33:23.000000 decryptogame-1.0.3/src/decryptogame/official_words/english.py
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)     3726 2023-07-30 21:52:49.000000 decryptogame-1.0.3/src/decryptogame/play.py
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)     8570 2023-07-31 00:12:46.000000 decryptogame-1.0.3/src/decryptogame/teams.py
+drwxr-xr-x   0 jadenrodriguez   (501) staff       (20)        0 2023-08-02 00:47:54.405306 decryptogame-1.0.3/src/decryptogame.egg-info/
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)     1431 2023-08-02 00:47:54.000000 decryptogame-1.0.3/src/decryptogame.egg-info/PKG-INFO
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)      504 2023-08-02 00:47:54.000000 decryptogame-1.0.3/src/decryptogame.egg-info/SOURCES.txt
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)        1 2023-08-02 00:47:54.000000 decryptogame-1.0.3/src/decryptogame.egg-info/dependency_links.txt
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)       13 2023-08-02 00:47:54.000000 decryptogame-1.0.3/src/decryptogame.egg-info/top_level.txt
+drwxr-xr-x   0 jadenrodriguez   (501) staff       (20)        0 2023-08-02 00:47:54.411067 decryptogame-1.0.3/tests/
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)     1468 2023-07-29 05:55:47.000000 decryptogame-1.0.3/tests/test_components.py
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)     3926 2023-07-30 20:48:01.000000 decryptogame-1.0.3/tests/test_game.py
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)      943 2023-07-29 07:15:17.000000 decryptogame-1.0.3/tests/test_generators.py
```

### Comparing `decryptogame-1.0.2/LICENSE` & `decryptogame-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `decryptogame-1.0.2/PKG-INFO` & `decryptogame-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decryptogame
-Version: 1.0.2
+Version: 1.0.3
 Summary: A non-official implementation of a Decrypto-style game for simulation and AI work.
 Author-email: Jaden Rodriguez <jadenrodriguez7@gmail.com>
 Project-URL: Homepage, https://github.com/YaBoiSkinnyP/decryptogame/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
```

### Comparing `decryptogame-1.0.2/README.md` & `decryptogame-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `decryptogame-1.0.2/pyproject.toml` & `decryptogame-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "decryptogame"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Jaden Rodriguez", email="jadenrodriguez7@gmail.com" },
 ]
 description = "A non-official implementation of a Decrypto-style game for simulation and AI work."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `decryptogame-1.0.2/src/decryptogame/__init__.py` & `decryptogame-1.0.3/src/decryptogame/__init__.py`

 * *Files identical despite different names*

### Comparing `decryptogame-1.0.2/src/decryptogame/components.py` & `decryptogame-1.0.3/src/decryptogame/components.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,22 +24,19 @@
             spec (str): Format specification.
 
         Returns:
             str: A formatted string representation of the TeamName.
         """
         return f"<{self.name}: {self.value}>"
     
-    def __format__(self, spec):
-        """Custom formmatting method for TeamName enumeration values.
-
-        Args:
-            spec (str): Format specification.
+    def __str__(self):
+        """Custom string method for TeamName enumeration values.
 
         Returns:
-            str: A formatted string representation of the TeamName.
+            str: The name of the team.
         """
         return str(self.name)
 
 @dataclasses.dataclass(kw_only=True)
 class GameData:
     """Class representing the game data. It's main use would be for strategizing or simulating plies.
 
@@ -48,15 +45,15 @@
         miscommunications (Sequence[int], optional): The miscommunication counts for each team. Defaults to [0, 0].
         interceptions (Sequence[int], optional): The interception counts for each team. Defaults to [0, 0].
     """
     rounds_played: int = 0
     miscommunications: Sequence[int] = dataclasses.field(default_factory=lambda: [0, 0])
     interceptions: Sequence[int] = dataclasses.field(default_factory=lambda: [0, 0])
 
-    def copy(self):
+    def copy(self) -> GameData:
         """Create a deep copy of the GameData object.
 
         Returns:
             GameData: A deep copy of the GameData object.
         """
         return deepcopy(self)
```

### Comparing `decryptogame-1.0.2/src/decryptogame/end_criteria.py` & `decryptogame-1.0.3/src/decryptogame/end_criteria.py`

 * *Files identical despite different names*

### Comparing `decryptogame-1.0.2/src/decryptogame/game.py` & `decryptogame-1.0.3/src/decryptogame/game.py`

 * *Files identical despite different names*

### Comparing `decryptogame-1.0.2/src/decryptogame/generators.py` & `decryptogame-1.0.3/src/decryptogame/generators.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         """Generate the next set of random codes for each team.
 
         Returns:
             tuple[Code, Code]: A tuple containing the randomly generated codes for each team.
         """
         return [self.random.choice(codes) for codes in self.team_codes]
 
-    def __iter__(self):
+    def __iter__(self) -> RandomCodes:
         """Return the generator as an iterable object.
 
         Returns:
             RandomCodes: The generator object itself.
         """
         return self
     
@@ -73,14 +73,14 @@
                 self.words.remove(keyword)
                 keywords.append(keyword)
             cards.append(tuple(keywords))
         for keywords in cards:
             self.words.extend(keywords)
         return cards
 
-    def __iter__(self):
+    def __iter__(self) -> RandomKeywordCards:
         """Return the generator as an iterable object.
 
         Returns:
             RandomKeywordCards: The generator object itself.
         """
         return self
```

### Comparing `decryptogame-1.0.2/src/decryptogame/official_words/english.py` & `decryptogame-1.0.3/src/decryptogame/official_words/english.py`

 * *Files identical despite different names*

### Comparing `decryptogame-1.0.2/src/decryptogame/play.py` & `decryptogame-1.0.3/src/decryptogame/play.py`

 * *Files identical despite different names*

### Comparing `decryptogame-1.0.2/src/decryptogame/teams.py` & `decryptogame-1.0.3/src/decryptogame/teams.py`

 * *Files identical despite different names*

### Comparing `decryptogame-1.0.2/src/decryptogame.egg-info/PKG-INFO` & `decryptogame-1.0.3/src/decryptogame.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decryptogame
-Version: 1.0.2
+Version: 1.0.3
 Summary: A non-official implementation of a Decrypto-style game for simulation and AI work.
 Author-email: Jaden Rodriguez <jadenrodriguez7@gmail.com>
 Project-URL: Homepage, https://github.com/YaBoiSkinnyP/decryptogame/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
```

### Comparing `decryptogame-1.0.2/tests/test_components.py` & `decryptogame-1.0.3/tests/test_components.py`

 * *Files identical despite different names*

### Comparing `decryptogame-1.0.2/tests/test_game.py` & `decryptogame-1.0.3/tests/test_game.py`

 * *Files identical despite different names*

### Comparing `decryptogame-1.0.2/tests/test_generators.py` & `decryptogame-1.0.3/tests/test_generators.py`

 * *Files identical despite different names*

