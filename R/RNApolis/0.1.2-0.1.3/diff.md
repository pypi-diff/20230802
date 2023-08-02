# Comparing `tmp/RNApolis-0.1.2.tar.gz` & `tmp/RNApolis-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RNApolis-0.1.2.tar", last modified: Wed Aug  2 13:45:08 2023, max compression
+gzip compressed data, was "RNApolis-0.1.3.tar", last modified: Wed Aug  2 14:31:34 2023, max compression
```

## Comparing `RNApolis-0.1.2.tar` & `RNApolis-0.1.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 tzok      (1000) tzok      (1000)        0 2023-08-02 13:45:08.094932 RNApolis-0.1.2/
--rw-r--r--   0 tzok      (1000) tzok      (1000)     1066 2023-04-04 15:11:51.000000 RNApolis-0.1.2/LICENSE
--rw-r--r--   0 tzok      (1000) tzok      (1000)      992 2023-08-02 13:45:08.094932 RNApolis-0.1.2/PKG-INFO
--rw-r--r--   0 tzok      (1000) tzok      (1000)      264 2023-04-04 15:11:51.000000 RNApolis-0.1.2/README.md
--rw-r--r--   0 tzok      (1000) tzok      (1000)       86 2023-04-04 15:11:51.000000 RNApolis-0.1.2/pyproject.toml
--rw-r--r--   0 tzok      (1000) tzok      (1000)       38 2023-08-02 13:45:08.094932 RNApolis-0.1.2/setup.cfg
--rw-r--r--   0 tzok      (1000) tzok      (1000)     1368 2023-08-02 13:44:49.000000 RNApolis-0.1.2/setup.py
-drwxr-xr-x   0 tzok      (1000) tzok      (1000)        0 2023-08-02 13:45:08.094932 RNApolis-0.1.2/src/
-drwxr-xr-x   0 tzok      (1000) tzok      (1000)        0 2023-08-02 13:45:08.094932 RNApolis-0.1.2/src/RNApolis.egg-info/
--rw-r--r--   0 tzok      (1000) tzok      (1000)      992 2023-08-02 13:45:08.000000 RNApolis-0.1.2/src/RNApolis.egg-info/PKG-INFO
--rw-r--r--   0 tzok      (1000) tzok      (1000)      656 2023-08-02 13:45:08.000000 RNApolis-0.1.2/src/RNApolis.egg-info/SOURCES.txt
--rw-r--r--   0 tzok      (1000) tzok      (1000)        1 2023-08-02 13:45:08.000000 RNApolis-0.1.2/src/RNApolis.egg-info/dependency_links.txt
--rw-r--r--   0 tzok      (1000) tzok      (1000)      220 2023-08-02 13:45:08.000000 RNApolis-0.1.2/src/RNApolis.egg-info/entry_points.txt
--rw-r--r--   0 tzok      (1000) tzok      (1000)       42 2023-08-02 13:45:08.000000 RNApolis-0.1.2/src/RNApolis.egg-info/requires.txt
--rw-r--r--   0 tzok      (1000) tzok      (1000)        9 2023-08-02 13:45:08.000000 RNApolis-0.1.2/src/RNApolis.egg-info/top_level.txt
-drwxr-xr-x   0 tzok      (1000) tzok      (1000)        0 2023-08-02 13:45:08.094932 RNApolis-0.1.2/src/rnapolis/
--rw-r--r--   0 tzok      (1000) tzok      (1000)    20766 2023-04-18 11:45:44.000000 RNApolis-0.1.2/src/rnapolis/annotator.py
--rw-r--r--   0 tzok      (1000) tzok      (1000)     8514 2023-04-04 15:11:51.000000 RNApolis-0.1.2/src/rnapolis/clashfinder.py
--rw-r--r--   0 tzok      (1000) tzok      (1000)    24612 2023-08-02 13:43:35.000000 RNApolis-0.1.2/src/rnapolis/common.py
--rwxr-xr-x   0 tzok      (1000) tzok      (1000)     1683 2023-04-04 15:11:51.000000 RNApolis-0.1.2/src/rnapolis/metareader.py
--rwxr-xr-x   0 tzok      (1000) tzok      (1000)      961 2023-05-18 12:12:42.000000 RNApolis-0.1.2/src/rnapolis/motif_extractor.py
--rw-r--r--   0 tzok      (1000) tzok      (1000)    11905 2023-04-04 15:11:51.000000 RNApolis-0.1.2/src/rnapolis/parser.py
--rw-r--r--   0 tzok      (1000) tzok      (1000)    18293 2023-04-18 11:45:44.000000 RNApolis-0.1.2/src/rnapolis/tertiary.py
--rwxr-xr-x   0 tzok      (1000) tzok      (1000)     1817 2023-04-04 15:11:51.000000 RNApolis-0.1.2/src/rnapolis/transformer.py
--rw-r--r--   0 tzok      (1000) tzok      (1000)      543 2023-04-04 15:11:51.000000 RNApolis-0.1.2/src/rnapolis/util.py
-drwxr-xr-x   0 tzok      (1000) tzok      (1000)        0 2023-08-02 13:45:08.094932 RNApolis-0.1.2/tests/
--rw-r--r--   0 tzok      (1000) tzok      (1000)     1509 2023-04-04 15:11:51.000000 RNApolis-0.1.2/tests/test_annotator.py
--rw-r--r--   0 tzok      (1000) tzok      (1000)     2639 2023-04-04 15:16:07.000000 RNApolis-0.1.2/tests/test_bugfixes.py
--rw-r--r--   0 tzok      (1000) tzok      (1000)     3635 2023-04-04 15:16:07.000000 RNApolis-0.1.2/tests/test_common.py
--rw-r--r--   0 tzok      (1000) tzok      (1000)     1145 2023-04-04 15:11:51.000000 RNApolis-0.1.2/tests/test_metareader.py
--rw-r--r--   0 tzok      (1000) tzok      (1000)      383 2023-04-04 15:11:51.000000 RNApolis-0.1.2/tests/test_parser.py
--rw-r--r--   0 tzok      (1000) tzok      (1000)    15655 2023-04-04 15:16:07.000000 RNApolis-0.1.2/tests/test_quadruplexes.py
--rw-r--r--   0 tzok      (1000) tzok      (1000)      445 2023-04-04 15:11:51.000000 RNApolis-0.1.2/tests/test_tertiary.py
+drwxr-xr-x   0 tzok      (1000) tzok      (1000)        0 2023-08-02 14:31:34.631976 RNApolis-0.1.3/
+-rw-r--r--   0 tzok      (1000) tzok      (1000)     1066 2023-04-04 15:11:51.000000 RNApolis-0.1.3/LICENSE
+-rw-r--r--   0 tzok      (1000) tzok      (1000)      992 2023-08-02 14:31:34.631976 RNApolis-0.1.3/PKG-INFO
+-rw-r--r--   0 tzok      (1000) tzok      (1000)      264 2023-04-04 15:11:51.000000 RNApolis-0.1.3/README.md
+-rw-r--r--   0 tzok      (1000) tzok      (1000)       86 2023-04-04 15:11:51.000000 RNApolis-0.1.3/pyproject.toml
+-rw-r--r--   0 tzok      (1000) tzok      (1000)       38 2023-08-02 14:31:34.631976 RNApolis-0.1.3/setup.cfg
+-rw-r--r--   0 tzok      (1000) tzok      (1000)     1368 2023-08-02 14:31:19.000000 RNApolis-0.1.3/setup.py
+drwxr-xr-x   0 tzok      (1000) tzok      (1000)        0 2023-08-02 14:31:34.631976 RNApolis-0.1.3/src/
+drwxr-xr-x   0 tzok      (1000) tzok      (1000)        0 2023-08-02 14:31:34.631976 RNApolis-0.1.3/src/RNApolis.egg-info/
+-rw-r--r--   0 tzok      (1000) tzok      (1000)      992 2023-08-02 14:31:34.000000 RNApolis-0.1.3/src/RNApolis.egg-info/PKG-INFO
+-rw-r--r--   0 tzok      (1000) tzok      (1000)      656 2023-08-02 14:31:34.000000 RNApolis-0.1.3/src/RNApolis.egg-info/SOURCES.txt
+-rw-r--r--   0 tzok      (1000) tzok      (1000)        1 2023-08-02 14:31:34.000000 RNApolis-0.1.3/src/RNApolis.egg-info/dependency_links.txt
+-rw-r--r--   0 tzok      (1000) tzok      (1000)      220 2023-08-02 14:31:34.000000 RNApolis-0.1.3/src/RNApolis.egg-info/entry_points.txt
+-rw-r--r--   0 tzok      (1000) tzok      (1000)       42 2023-08-02 14:31:34.000000 RNApolis-0.1.3/src/RNApolis.egg-info/requires.txt
+-rw-r--r--   0 tzok      (1000) tzok      (1000)        9 2023-08-02 14:31:34.000000 RNApolis-0.1.3/src/RNApolis.egg-info/top_level.txt
+drwxr-xr-x   0 tzok      (1000) tzok      (1000)        0 2023-08-02 14:31:34.631976 RNApolis-0.1.3/src/rnapolis/
+-rw-r--r--   0 tzok      (1000) tzok      (1000)    20766 2023-04-18 11:45:44.000000 RNApolis-0.1.3/src/rnapolis/annotator.py
+-rw-r--r--   0 tzok      (1000) tzok      (1000)     8514 2023-04-04 15:11:51.000000 RNApolis-0.1.3/src/rnapolis/clashfinder.py
+-rw-r--r--   0 tzok      (1000) tzok      (1000)    24620 2023-08-02 14:31:19.000000 RNApolis-0.1.3/src/rnapolis/common.py
+-rwxr-xr-x   0 tzok      (1000) tzok      (1000)     1683 2023-04-04 15:11:51.000000 RNApolis-0.1.3/src/rnapolis/metareader.py
+-rwxr-xr-x   0 tzok      (1000) tzok      (1000)      958 2023-08-02 14:31:19.000000 RNApolis-0.1.3/src/rnapolis/motif_extractor.py
+-rw-r--r--   0 tzok      (1000) tzok      (1000)    11905 2023-04-04 15:11:51.000000 RNApolis-0.1.3/src/rnapolis/parser.py
+-rw-r--r--   0 tzok      (1000) tzok      (1000)    18253 2023-08-02 14:31:19.000000 RNApolis-0.1.3/src/rnapolis/tertiary.py
+-rwxr-xr-x   0 tzok      (1000) tzok      (1000)     1817 2023-04-04 15:11:51.000000 RNApolis-0.1.3/src/rnapolis/transformer.py
+-rw-r--r--   0 tzok      (1000) tzok      (1000)      543 2023-04-04 15:11:51.000000 RNApolis-0.1.3/src/rnapolis/util.py
+drwxr-xr-x   0 tzok      (1000) tzok      (1000)        0 2023-08-02 14:31:34.631976 RNApolis-0.1.3/tests/
+-rw-r--r--   0 tzok      (1000) tzok      (1000)     1509 2023-04-04 15:11:51.000000 RNApolis-0.1.3/tests/test_annotator.py
+-rw-r--r--   0 tzok      (1000) tzok      (1000)     2639 2023-04-04 15:16:07.000000 RNApolis-0.1.3/tests/test_bugfixes.py
+-rw-r--r--   0 tzok      (1000) tzok      (1000)     3632 2023-08-02 14:31:19.000000 RNApolis-0.1.3/tests/test_common.py
+-rw-r--r--   0 tzok      (1000) tzok      (1000)     1145 2023-04-04 15:11:51.000000 RNApolis-0.1.3/tests/test_metareader.py
+-rw-r--r--   0 tzok      (1000) tzok      (1000)      383 2023-04-04 15:11:51.000000 RNApolis-0.1.3/tests/test_parser.py
+-rw-r--r--   0 tzok      (1000) tzok      (1000)    15655 2023-04-04 15:16:07.000000 RNApolis-0.1.3/tests/test_quadruplexes.py
+-rw-r--r--   0 tzok      (1000) tzok      (1000)      445 2023-04-04 15:11:51.000000 RNApolis-0.1.3/tests/test_tertiary.py
```

### Comparing `RNApolis-0.1.2/LICENSE` & `RNApolis-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `RNApolis-0.1.2/PKG-INFO` & `RNApolis-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RNApolis
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python library containing RNA-related bioinformatics functions and classes
 Home-page: https://github.com/tzok/rnapolis-py
 Author: Tomasz Zok
 Author-email: tomasz.zok@cs.put.poznan.pl
 Project-URL: Bug Tracker, https://github.com/tzok/rnapolis-py/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `RNApolis-0.1.2/setup.py` & `RNApolis-0.1.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="RNApolis",
-    version="0.1.2",
+    version="0.1.3",
     packages=["rnapolis"],
     package_dir={"": "src"},
     author="Tomasz Zok",
     author_email="tomasz.zok@cs.put.poznan.pl",
     description="A Python library containing RNA-related bioinformatics functions and classes",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `RNApolis-0.1.2/src/RNApolis.egg-info/PKG-INFO` & `RNApolis-0.1.3/src/RNApolis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RNApolis
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python library containing RNA-related bioinformatics functions and classes
 Home-page: https://github.com/tzok/rnapolis-py
 Author: Tomasz Zok
 Author-email: tomasz.zok@cs.put.poznan.pl
 Project-URL: Bug Tracker, https://github.com/tzok/rnapolis-py/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `RNApolis-0.1.2/src/RNApolis.egg-info/SOURCES.txt` & `RNApolis-0.1.3/src/RNApolis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RNApolis-0.1.2/src/rnapolis/annotator.py` & `RNApolis-0.1.3/src/rnapolis/annotator.py`

 * *Files identical despite different names*

### Comparing `RNApolis-0.1.2/src/rnapolis/clashfinder.py` & `RNApolis-0.1.3/src/rnapolis/clashfinder.py`

 * *Files identical despite different names*

### Comparing `RNApolis-0.1.2/src/rnapolis/common.py` & `RNApolis-0.1.3/src/rnapolis/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -445,15 +445,18 @@
 class BpSeq:
     entries: List[Entry]
 
     @staticmethod
     def from_string(bpseq_str: str):
         entries = []
         for line in bpseq_str.splitlines():
-            fields = line.strip().split()
+            line = line.strip()
+            if len(line) == 0:
+                continue
+            fields = line.split()
             if len(fields) != 3:
                 logging.warning("Failed to find 3 columns in BpSeq line: {}", line)
                 continue
             entry = Entry(int(fields[0]), fields[1], int(fields[2]))
             entries.append(entry)
         return BpSeq(entries)
 
@@ -531,15 +534,15 @@
 
         stems, single_strands, hairpins, loops = [], [], [], []
         stopset = set()
 
         # stems
         for stem_entries in self.__stems_entries:
             stem = Stem.from_bpseq_entries(
-                stem_entries, self.entries, self.to_dot_bracket.structure
+                stem_entries, self.entries, self.dot_bracket.structure
             )
             stems.append(stem)
             stopset.add(stem.strand5p.first - 1)
             stopset.add(stem.strand5p.last - 1)
             stopset.add(stem.strand3p.first - 1)
             stopset.add(stem.strand3p.last - 1)
 
@@ -548,46 +551,44 @@
 
         # 5' single strand
         if stops[0] > 0:
             single_strands.append(
                 SingleStrand(
                     Strand.from_bpseq_entries(
                         self.entries[: stops[0] + 1],
-                        self.to_dot_bracket.structure,
+                        self.dot_bracket.structure,
                     ),
                     True,
                     False,
                 )
             )
 
         # single strands
         for i in range(1, len(stops)):
             candidate = self.entries[stops[i - 1] : stops[i] + 1]
             if all([entry.pair == 0 for entry in candidate[1:-1]]):
                 if candidate[0].pair == candidate[-1].index_:
                     hairpins.append(
                         Hairpin(
                             Strand.from_bpseq_entries(
-                                candidate, self.to_dot_bracket.structure
+                                candidate, self.dot_bracket.structure
                             )
                         )
                     )
                 else:
                     loop_candidates.append(
-                        Strand.from_bpseq_entries(
-                            candidate, self.to_dot_bracket.structure
-                        )
+                        Strand.from_bpseq_entries(candidate, self.dot_bracket.structure)
                     )
 
         # 3' single strand
         if stops[-1] < len(self.entries) - 1:
             single_strands.append(
                 SingleStrand(
                     Strand.from_bpseq_entries(
-                        self.entries[stops[-1] :], self.to_dot_bracket.structure
+                        self.entries[stops[-1] :], self.dot_bracket.structure
                     ),
                     False,
                     True,
                 )
             )
 
         graph = defaultdict(set)
@@ -634,15 +635,15 @@
     def __regions(self) -> List[Tuple[int, int, int]]:
         return [
             (stem_entries[0].index_, stem_entries[0].pair, len(stem_entries))
             for stem_entries in self.__stems_entries
         ]
 
     @cached_property
-    def to_dot_bracket(self):
+    def dot_bracket(self):
         pulp.LpSolverDefault.msg = False
         return self.convert_to_dot_bracket(pulp.LpSolverDefault)
 
     def convert_to_dot_bracket(self, solver: pulp.LpSolver):
         # if PuLP solvers are not installed, use FCFS
         if len(pulp.listSolvers(onlyAvailable=True)) == 0:
             return self.fcfs()
```

### Comparing `RNApolis-0.1.2/src/rnapolis/metareader.py` & `RNApolis-0.1.3/src/rnapolis/metareader.py`

 * *Files identical despite different names*

### Comparing `RNApolis-0.1.2/src/rnapolis/motif_extractor.py` & `RNApolis-0.1.3/src/rnapolis/motif_extractor.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         bpseq = BpSeq.from_dotbracket(DotBracket.from_file(args.dbn))
     elif args.bpseq:
         bpseq = BpSeq.from_file(args.bpseq)
     else:
         parser.print_help()
         return
 
-    print(f"Full dot-bracket:\n{bpseq.to_dot_bracket}")
+    print(f"Full dot-bracket:\n{bpseq.dot_bracket}")
     stems, single_strands, hairpins, loops = bpseq.elements
 
     for element in itertools.chain(stems, single_strands, hairpins, loops):
         print(element)
 
 
 if __name__ == "__main__":
```

### Comparing `RNApolis-0.1.2/src/rnapolis/parser.py` & `RNApolis-0.1.3/src/rnapolis/parser.py`

 * *Files identical despite different names*

### Comparing `RNApolis-0.1.2/src/rnapolis/tertiary.py` & `RNApolis-0.1.3/src/rnapolis/tertiary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from functools import total_ordering
 import itertools
 import logging
 import math
 import string
 from collections import defaultdict
 from dataclasses import dataclass, field
 from functools import cached_property, total_ordering
@@ -546,15 +545,15 @@
             result.append(f">strand_{chain}")
             result.append(sequence)
             result.append(dbns[i])
             i += len(sequence)
         return "\n".join(result)
 
     def __generate_dot_bracket_per_strand(self, bpseq: BpSeq) -> List[str]:
-        dbn = bpseq.to_dot_bracket.structure
+        dbn = bpseq.dot_bracket.structure
         i = 0
         result = []
 
         for _, sequence in self.strands_sequences:
             result.append("".join(dbn[i : i + len(sequence)]))
             i += len(sequence)
         return result
```

### Comparing `RNApolis-0.1.2/src/rnapolis/transformer.py` & `RNApolis-0.1.3/src/rnapolis/transformer.py`

 * *Files identical despite different names*

### Comparing `RNApolis-0.1.2/src/rnapolis/util.py` & `RNApolis-0.1.3/src/rnapolis/util.py`

 * *Files identical despite different names*

### Comparing `RNApolis-0.1.2/tests/test_annotator.py` & `RNApolis-0.1.3/tests/test_annotator.py`

 * *Files identical despite different names*

### Comparing `RNApolis-0.1.2/tests/test_bugfixes.py` & `RNApolis-0.1.3/tests/test_bugfixes.py`

 * *Files identical despite different names*

### Comparing `RNApolis-0.1.2/tests/test_common.py` & `RNApolis-0.1.3/tests/test_common.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
     assert len(single_strands) == 1
     assert len(hairpins) == 1
     assert len(loops) == 2
 
 
 def test_pseudoknot_order_assignment():
     bpseq = BpSeq.from_file("tests/6EK0-L5-L8.bpseq")
-    dot_bracket = bpseq.to_dot_bracket
+    dot_bracket = bpseq.dot_bracket
 
     counter = Counter(dot_bracket.structure)
     assert counter["."] == 1185
     assert counter["("] == 1298
     assert counter["["] == 44
     assert counter["{"] == 17
     assert counter["<"] == 7
```

### Comparing `RNApolis-0.1.2/tests/test_metareader.py` & `RNApolis-0.1.3/tests/test_metareader.py`

 * *Files identical despite different names*

### Comparing `RNApolis-0.1.2/tests/test_quadruplexes.py` & `RNApolis-0.1.3/tests/test_quadruplexes.py`

 * *Files identical despite different names*

