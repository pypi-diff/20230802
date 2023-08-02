# Comparing `tmp/RDG-0.1.4.1.tar.gz` & `tmp/RDG-0.1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/RDG-0.1.4.1.tar", last modified: Mon Oct  3 10:42:03 2022, max compression
+gzip compressed data, was "dist/RDG-0.1.4.2.tar", last modified: Wed Aug  2 09:38:25 2023, max compression
```

## Comparing `RDG-0.1.4.1.tar` & `RDG-0.1.4.2.tar`

### file list

```diff
@@ -1,37 +1,43 @@
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2022-10-03 10:42:03.048214 RDG-0.1.4.1/
--rw-rw-r--   0 jack      (1000) jack      (1000)     1903 2021-12-06 12:38:15.000000 RDG-0.1.4.1/.gitignore
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2022-10-03 10:42:03.044214 RDG-0.1.4.1/.vscode/
--rw-rw-r--   0 jack      (1000) jack      (1000)       44 2022-01-17 13:41:16.000000 RDG-0.1.4.1/.vscode/settings.json
--rw-rw-r--   0 jack      (1000) jack      (1000)     1069 2021-11-30 13:45:44.000000 RDG-0.1.4.1/LICENSE
--rw-rw-r--   0 jack      (1000) jack      (1000)      179 2022-10-03 10:42:03.048214 RDG-0.1.4.1/PKG-INFO
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2022-10-03 10:42:03.044214 RDG-0.1.4.1/RDG/
--rw-rw-r--   0 jack      (1000) jack      (1000)     2706 2022-10-03 09:16:54.000000 RDG-0.1.4.1/RDG/RDG_to_file.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      115 2021-12-08 15:58:49.000000 RDG-0.1.4.1/RDG/__init__.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     3571 2022-01-18 15:47:36.000000 RDG-0.1.4.1/RDG/build_RDG_from_sequence.py
--rw-rw-r--   0 jack      (1000) jack      (1000)    25965 2022-10-03 09:17:17.000000 RDG-0.1.4.1/RDG/decision_graph.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     4407 2022-10-03 10:41:48.000000 RDG-0.1.4.1/RDG/plot_RDG.py
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2022-10-03 10:42:03.044214 RDG-0.1.4.1/RDG.egg-info/
--rw-rw-r--   0 jack      (1000) jack      (1000)      179 2022-10-03 10:42:02.000000 RDG-0.1.4.1/RDG.egg-info/PKG-INFO
--rw-rw-r--   0 jack      (1000) jack      (1000)      639 2022-10-03 10:42:03.000000 RDG-0.1.4.1/RDG.egg-info/SOURCES.txt
--rw-rw-r--   0 jack      (1000) jack      (1000)        1 2022-10-03 10:42:02.000000 RDG-0.1.4.1/RDG.egg-info/dependency_links.txt
--rw-rw-r--   0 jack      (1000) jack      (1000)       10 2022-10-03 10:42:02.000000 RDG-0.1.4.1/RDG.egg-info/top_level.txt
--rw-rw-r--   0 jack      (1000) jack      (1000)     3446 2022-10-03 10:20:00.000000 RDG-0.1.4.1/README.md
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2022-10-03 10:42:03.044214 RDG-0.1.4.1/images/
--rw-rw-r--   0 jack      (1000) jack      (1000)    86784 2022-02-16 10:51:06.000000 RDG-0.1.4.1/images/Impact_of_point_mutationspng
--rw-rw-r--   0 jack      (1000) jack      (1000)    16077 2022-02-16 10:52:18.000000 RDG-0.1.4.1/images/ORF_plot.png
--rw-rw-r--   0 jack      (1000) jack      (1000)    70987 2022-02-16 10:48:41.000000 RDG-0.1.4.1/images/Other_biological_info
--rw-rw-r--   0 jack      (1000) jack      (1000)    38683 2022-02-16 10:50:40.000000 RDG-0.1.4.1/images/Proportion_of_peptides.png
--rw-rw-r--   0 jack      (1000) jack      (1000)    64995 2022-02-16 10:50:16.000000 RDG-0.1.4.1/images/RDG.png
--rw-rw-r--   0 jack      (1000) jack      (1000)        1 2022-02-16 10:55:59.000000 RDG-0.1.4.1/images/README.md
--rw-rw-r--   0 jack      (1000) jack      (1000)    23419 2022-02-16 10:51:54.000000 RDG-0.1.4.1/images/current_representation.png
--rw-rw-r--   0 jack      (1000) jack      (1000)       38 2022-10-03 10:42:03.048214 RDG-0.1.4.1/setup.cfg
--rw-rw-r--   0 jack      (1000) jack      (1000)      123 2022-10-03 10:41:55.000000 RDG-0.1.4.1/setup.py
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2022-10-03 10:42:03.048214 RDG-0.1.4.1/tests/
--rw-rw-r--   0 jack      (1000) jack      (1000)        0 2021-11-30 14:33:13.000000 RDG-0.1.4.1/tests/__init__.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      313 2021-12-06 12:35:53.000000 RDG-0.1.4.1/tests/test_basics.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      559 2021-12-03 11:52:30.000000 RDG-0.1.4.1/tests/test_get.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     2079 2021-12-08 13:32:54.000000 RDG-0.1.4.1/tests/test_inset_orf.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      297 2021-12-06 12:34:35.000000 RDG-0.1.4.1/tests/test_load_graph.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      361 2021-12-06 12:32:25.000000 RDG-0.1.4.1/tests/test_read_write.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      447 2021-12-02 11:35:55.000000 RDG-0.1.4.1/tests/test_remove_edge.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     1319 2021-12-08 13:33:27.000000 RDG-0.1.4.1/tests/test_update_edge.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-08-02 09:38:25.541573 RDG-0.1.4.2/
+-rw-rw-r--   0 jack      (1000) jack      (1000)     1903 2021-12-06 12:38:15.000000 RDG-0.1.4.2/.gitignore
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-08-02 09:38:25.537573 RDG-0.1.4.2/.vscode/
+-rw-rw-r--   0 jack      (1000) jack      (1000)       44 2022-01-17 13:41:16.000000 RDG-0.1.4.2/.vscode/settings.json
+-rw-rw-r--   0 jack      (1000) jack      (1000)     1069 2021-11-30 13:45:44.000000 RDG-0.1.4.2/LICENSE
+-rw-rw-r--   0 jack      (1000) jack      (1000)      179 2023-08-02 09:38:25.541573 RDG-0.1.4.2/PKG-INFO
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-08-02 09:38:25.537573 RDG-0.1.4.2/RDG/
+-rw-rw-r--   0 jack      (1000) jack      (1000)    79290 2023-04-19 11:14:02.000000 RDG-0.1.4.2/RDG/RDG.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     3280 2023-02-23 17:46:03.000000 RDG-0.1.4.2/RDG/RDG_to_file.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      105 2023-02-23 18:52:36.000000 RDG-0.1.4.2/RDG/__init__.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     4056 2023-02-23 19:37:31.000000 RDG-0.1.4.2/RDG/build_RDG_from_sequence.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)    12515 2023-02-22 09:32:19.000000 RDG-0.1.4.2/RDG/dynamic_build.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     8400 2023-07-12 14:42:43.000000 RDG-0.1.4.2/RDG/plot_RDG.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-08-02 09:38:25.537573 RDG-0.1.4.2/RDG.egg-info/
+-rw-rw-r--   0 jack      (1000) jack      (1000)      179 2023-08-02 09:38:25.000000 RDG-0.1.4.2/RDG.egg-info/PKG-INFO
+-rw-rw-r--   0 jack      (1000) jack      (1000)      739 2023-08-02 09:38:25.000000 RDG-0.1.4.2/RDG.egg-info/SOURCES.txt
+-rw-rw-r--   0 jack      (1000) jack      (1000)        1 2023-08-02 09:38:25.000000 RDG-0.1.4.2/RDG.egg-info/dependency_links.txt
+-rw-rw-r--   0 jack      (1000) jack      (1000)       10 2023-08-02 09:38:25.000000 RDG-0.1.4.2/RDG.egg-info/top_level.txt
+-rw-rw-r--   0 jack      (1000) jack      (1000)     3446 2022-10-03 10:20:00.000000 RDG-0.1.4.2/README.md
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-08-02 09:38:25.541573 RDG-0.1.4.2/images/
+-rw-rw-r--   0 jack      (1000) jack      (1000)    86784 2022-02-16 10:51:06.000000 RDG-0.1.4.2/images/Impact_of_point_mutationspng
+-rw-rw-r--   0 jack      (1000) jack      (1000)    16077 2022-02-16 10:52:18.000000 RDG-0.1.4.2/images/ORF_plot.png
+-rw-rw-r--   0 jack      (1000) jack      (1000)    70987 2022-02-16 10:48:41.000000 RDG-0.1.4.2/images/Other_biological_info
+-rw-rw-r--   0 jack      (1000) jack      (1000)    38683 2022-02-16 10:50:40.000000 RDG-0.1.4.2/images/Proportion_of_peptides.png
+-rw-rw-r--   0 jack      (1000) jack      (1000)    64995 2022-02-16 10:50:16.000000 RDG-0.1.4.2/images/RDG.png
+-rw-rw-r--   0 jack      (1000) jack      (1000)        1 2022-02-16 10:55:59.000000 RDG-0.1.4.2/images/README.md
+-rw-rw-r--   0 jack      (1000) jack      (1000)    23419 2022-02-16 10:51:54.000000 RDG-0.1.4.2/images/current_representation.png
+-rw-rw-r--   0 jack      (1000) jack      (1000)       38 2023-08-02 09:38:25.541573 RDG-0.1.4.2/setup.cfg
+-rw-rw-r--   0 jack      (1000) jack      (1000)      123 2023-08-02 09:38:23.000000 RDG-0.1.4.2/setup.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)    67696 2023-02-23 19:38:15.000000 RDG-0.1.4.2/test.nwk
+-rw-r--r--   0 jack      (1000) jack      (1000)    20480 2023-02-22 14:29:35.000000 RDG-0.1.4.2/test.rdg
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-08-02 09:38:25.541573 RDG-0.1.4.2/tests/
+-rw-rw-r--   0 jack      (1000) jack      (1000)        0 2023-02-22 14:20:03.000000 RDG-0.1.4.2/tests/__init__.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     3885 2023-02-23 13:10:53.000000 RDG-0.1.4.2/tests/test_add_features.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      744 2023-02-21 14:15:19.000000 RDG-0.1.4.2/tests/test_add_remove_edge.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      439 2023-02-21 14:15:19.000000 RDG-0.1.4.2/tests/test_basics.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      681 2023-02-21 14:15:19.000000 RDG-0.1.4.2/tests/test_edgeObj.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     3867 2023-02-23 13:12:38.000000 RDG-0.1.4.2/tests/test_get.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     1921 2023-02-21 14:15:19.000000 RDG-0.1.4.2/tests/test_load_graph.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      826 2023-04-19 11:47:35.000000 RDG-0.1.4.2/tests/test_newick.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     1265 2023-02-22 11:05:16.000000 RDG-0.1.4.2/tests/test_nodeObj.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      828 2023-02-22 17:10:38.000000 RDG-0.1.4.2/tests/test_read_write.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     1448 2023-02-21 14:15:19.000000 RDG-0.1.4.2/tests/test_update_edge.py
```

### Comparing `RDG-0.1.4.1/.gitignore` & `RDG-0.1.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `RDG-0.1.4.1/LICENSE` & `RDG-0.1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `RDG-0.1.4.1/RDG/RDG_to_file.py` & `RDG-0.1.4.2/RDG/RDG_to_file.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,93 +1,134 @@
 from RDG import RDG, Node, Edge
 from sqlitedict import SqliteDict
 
 
 def to_dict(obj):
-    output ={}
-    print(obj, type(obj), obj.__dict__.items())
+    '''
+    Recursively convert a class to a dictionary
+
+    Parameters
+    ----------
+    obj : class
+        The class to convert to a dictionary
+
+    Returns 
+    -------
+    output : dict
+    '''
+    output = {}
     for key, item in obj.__dict__.items():
         if isinstance(item, list):
             l = []
             for item in item:
-                if isinstance(item, int):
-                    l.append(item)
-                else:
-                    d = to_dict(item)
-                    l.append(d)
+                l.append(item)
+
             output[key] = l
         else:
             output[key] = item
 
     return output
 
 
 def save(graph, save_file):
+    '''
+    Save a graph to a file
 
-    transcript = graph.locus
-    graph_dict = {transcript:{}}
+    Parameters
+    ----------
+    graph : RDG
+
+    save_file : str
+        The name of the file to save to (should end in .sqlite)
+    '''
+    graph_dict = {graph.locus: {}}
     for attr, value in graph.__dict__.items():
-        if attr not in graph_dict[transcript]:
-            graph_dict[transcript][attr] = {}
+        if attr not in graph_dict[graph.locus]:
+            graph_dict[graph.locus][attr] = {}
 
         if isinstance(value, dict):
             for key in value:
-                graph_dict[transcript][attr][key] = to_dict(value[key])
+                graph_dict[graph.locus][attr][key] = to_dict(value[key])
         else:
-            graph_dict[transcript][attr] = value
+            graph_dict[graph.locus][attr] = value
 
-    try:  
+    try:
         with SqliteDict(save_file) as output_dict:
             for key in graph_dict:
                 output_dict[key] = graph_dict[key]
-                output_dict.commit() 
+                output_dict.commit()
+
+    except:
+        raise Exception("Error during storing data (Possibly unsupported):")
+    
+def newick_to_file(newick, save_file):
+    '''
+    Save a newick string to a file
+
+    Parameters
+    ----------
+    newick : str
+        The newick string to save
+
+    save_file : str
+        The name of the file to save to (should end in .sqlite)
+    '''
+    with open(save_file, 'w') as file:
+        file.write(newick)
+
+
 
-    except Exception as ex:
-        print("Error during storing data (Possibly unsupported):", ex)
 
 
-def load(locus, cache_file="test_output.sqlite"):
+def load(locus, cache_file="test_output.sqlite") -> RDG:
+    '''
+    Load a graph from a file
+
+    Parameters
+    ----------
+    locus : str
+        The locus of the graph to load
+
+    cache_file : str
+        The name of the file to load from (should end in .sqlite)
+    '''
     try:
         with SqliteDict(cache_file) as mydict:
-            graph_dict = mydict[locus] # No need to use commit(), since we are only loading data!
+            print(list(mydict.keys()))
+            graph_dict = mydict[
+                locus
+            ]  # No need to use commit(), since we are only loading data!
     except Exception as ex:
-        print("Error during loading data:", ex)
-    
+        raise Exception("Error during loading data:", ex)
+
     dg = RDG()
     nodes = {}
-    for key in graph_dict['nodes']:
-        nodes[key] = Node(key, 
-        graph_dict['nodes'][key]['node_type'], 
-        graph_dict['nodes'][key]['node_start'],
-        graph_dict['nodes'][key]['input_edges'],
-        graph_dict['nodes'][key]['output_edges'],
-        graph_dict['nodes'][key]['input_nodes'],
-        graph_dict['nodes'][key]['output_nodes'])
+    for key in graph_dict["nodes"]:
+        nodes[key] = Node(
+            key,
+            graph_dict["nodes"][key]["node_type"],
+            graph_dict["nodes"][key]["node_start"],
+            graph_dict["nodes"][key]["input_edges"],
+            graph_dict["nodes"][key]["output_edges"],
+            graph_dict["nodes"][key]["input_nodes"],
+            graph_dict["nodes"][key]["output_nodes"],
+        )
 
     edges = {}
 
-    for key in graph_dict['edges']:
-        edges[key] = Edge(key, 
-        graph_dict['edges'][key]['edge_type'], 
-        graph_dict['edges'][key]['from_node'],
-        graph_dict['edges'][key]['to_node'],
-        graph_dict['edges'][key]['coordinates'])
-
-    dg = dg.Load(locus_name=locus, locus_start=graph_dict['locus_start'], locus_stop=graph_dict['locus_stop'], nodes=nodes, edges=edges)
+    for key in graph_dict["edges"]:
+        edges[key] = Edge(
+            key,
+            graph_dict["edges"][key]["edge_type"],
+            graph_dict["edges"][key]["from_node"],
+            graph_dict["edges"][key]["to_node"],
+            graph_dict["edges"][key]["coordinates"],
+        )
+
+    dg = dg.Load(
+        locus_name=locus,
+        locus_start=graph_dict["locus_start"],
+        locus_stop=graph_dict["locus_stop"],
+        nodes=nodes,
+        edges=edges,
+    )
     return dg
-
-
-
-
-# if __name__ == "__main__":
-#     dg = RDG()
-#     dg.add_open_reading_frame(30, 90)
-#     dg.add_open_reading_frame(131, 171)
-#     dg.add_open_reading_frame(150,850)
-   
-#     # save(dg, 'test_output.sqlite')
-#     dg2 = load('', 'test_output.sqlite')
-
-#     a = dg.describe()
-#     print()
-#     b = dg2.describe()
-#     print(a == b)
```

### Comparing `RDG-0.1.4.1/RDG/build_RDG_from_sequence.py` & `RDG-0.1.4.2/RDG/build_RDG_from_sequence.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-from networkx.exception import AmbiguousSolution
-from RDG import RDG, Node, Edge, plot, save
-from pprint import pprint
+from RDG import RDG
 from progress.bar import Bar
-from time import time
+from plot_RDG import plot
 
+# from profilestats import profile
 
 
 # table = """TTT F      CTT L      ATT I      GTT V
 # TTC F      CTC L      ATC I      GTC V
 # TTA L      CTA L      ATA I      GTA V
 # TTG L      CTG L      ATG M      GTG V
 # TCT S      CCT P      ACT T      GCT A
@@ -21,84 +20,109 @@
 # TGT C      CGT R      AGT S      GGT G
 # TGC C      CGC R      AGC S      GGC G
 # TGA Stop   CGA R      AGA R      GGA G
 # TGG W      CGG R      AGG R      GGG G"""
 # table = dict(zip(table.split()[::2],table.split()[1::2]))
 
 
-def parse_sequence_into_translated_regions(sequence, starts=["ATG", "CTG", "GTG"], min_length=10, reinitiation=False):
-    '''
+def parse_sequence_into_translated_regions(
+    sequence, starts=["ATG", "CTG", "GTG"], min_length=10, reinitiation=False
+):
+    """
     take a nucleotide sequence and return a list of ORFs
-    '''
-    frames = {1:[], 2:[], 3:[]}
-    for i in range(len(sequence)+1):
+    """
+    frames = {1: [], 2: [], 3: []}
+    for i in range(len(sequence) + 1):
         try:
-            codon = sequence[i:i+3]
+            codon = sequence[i : i + 3]
             if len(codon) == 3:
                 frames[1].append(codon)
         except KeyError:
             continue
         try:
-            codon = sequence[i+1:i+4]
+            codon = sequence[i + 1 : i + 4]
             if len(codon) == 3:
                 frames[1].append(codon)
         except KeyError:
             continue
         try:
-            codon = sequence[i+2:i+5]
+            codon = sequence[i + 2 : i + 5]
             if len(codon) == 3:
                 frames[1].append(codon)
         except KeyError:
             continue
-    
-    stops = ["TAA","TAG","TGA"]
-    
 
-    orf_sequences = [] 
+    stops = ["TAA", "TAG", "TGA"]
+
+    orf_sequences = []
     for i in range(len(sequence)):
-        if sequence[i:i+3] in starts:
-            for j in range(i,len(sequence),3):
-                if sequence[j:j+3] in stops:
-                    orf = [sequence[k:k+3] for k in range(i,j+3,3)]
-                    if len(''.join(orf)) > min_length:
-                        orf_sequences.append(''.join(orf))
+        if sequence[i : i + 3] in starts:
+            for j in range(i, len(sequence), 3):
+                if sequence[j : j + 3] in stops:
+                    orf = [sequence[k : k + 3] for k in range(i, j + 3, 3)]
+                    if len("".join(orf)) > min_length:
+                        orf_sequences.append("".join(orf))
                     break
 
-    orfs = [] 
+    orfs = []
     counter = 1
     for orf in orf_sequences:
         start_codon_position = sequence.find(orf)
         stop_codon_position = sequence.find(orf) + len(orf)
         orfs.append((start_codon_position, stop_codon_position))
         counter += 1
     return orfs
 
 
-def build_graphs_from_fasta(file_path, min_lenth=100, start_codons=["ATG", "CTG", "GTG"], reinitiation=False, readthrough=False, upstream_limit=1):
-    file = open(file_path, 'r').readlines()
-    sequences = {} 
+def build_graphs_from_fasta(
+    file_path,
+    min_lenth=100,
+    start_codons=["ATG", "CTG", "GTG"],
+    reinitiation=False,
+    readthrough=False,
+    upstream_limit=1,
+):
+    file = open(file_path, "r").readlines()
+    sequences = {}
     for line in file:
-        if line[0] == '>':
+        if line[0] == ">":
             name = line.split(" ")[0][1:]
             sequences[name] = ""
-            
         else:
-            sequences[name] += line.strip('\n')
+            sequences[name] += line.strip("\n")
 
     graphs = []
     for sequence in sequences:
-        orfs = parse_sequence_into_translated_regions(sequences[sequence], starts=start_codons, min_length=min_lenth)
+        orfs = parse_sequence_into_translated_regions(
+            sequences[sequence], starts=start_codons, min_length=min_lenth
+        )
         dg = RDG(name=sequence, locus_stop=len(sequences[sequence]))
-        with Bar('building...') as bar:
+        with Bar("building...") as bar:
             for orf in sorted(orfs):
-                dg.add_open_reading_frame(orf[0], orf[1], reinitiation=reinitiation)
-
+                dg.add_open_reading_frame(
+                    orf[0],
+                    orf[1],
+                    reinitiation=reinitiation,
+                    upstream_limit=upstream_limit,
+                )
                 bar.next()
         graphs.append(dg)
     return graphs
 
+
 if __name__ == "__main__":
-    # graphs = build_graphs_from_fasta('/home/jack/projects/decision_graphs/data/PHPT1_transcript_sequence.fa', min_lenth=0)
-    graphs = build_graphs_from_fasta('/home/jack/projects/decision_graphs/data/test_fasta_multi_sequences.fa')
+    graphs = build_graphs_from_fasta(
+        "/home/jack/projects/decision_graphs/data/PHPT1_transcript_sequence.fa",
+        min_lenth=10,
+        reinitiation=False,
+        readthrough=False,
+        upstream_limit=100,
+    )
+    # graphs = build_graphs_from_fasta('/home/jack/projects/decision_graphs/data/test_fasta_multi_sequences.fa')
     for dg in graphs:
+        orfs = dg.get_orfs()
+        longest_orf = max(orfs, key=lambda x: x[1] - x[0])
+        print(longest_orf, longest_orf[0] % 3)
+        print(dg.describe())
+        with open('test.nwk', "w") as f:
+            f.write(dg.newick())
         plot(dg)
-
```

### Comparing `RDG-0.1.4.1/RDG.egg-info/SOURCES.txt` & `RDG-0.1.4.2/RDG.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 .gitignore
 LICENSE
 README.md
 setup.py
+test.nwk
+test.rdg
 .vscode/settings.json
+RDG/RDG.py
 RDG/RDG_to_file.py
 RDG/__init__.py
 RDG/build_RDG_from_sequence.py
-RDG/decision_graph.py
+RDG/dynamic_build.py
 RDG/plot_RDG.py
 RDG.egg-info/PKG-INFO
 RDG.egg-info/SOURCES.txt
 RDG.egg-info/dependency_links.txt
 RDG.egg-info/top_level.txt
 images/Impact_of_point_mutationspng
 images/ORF_plot.png
 images/Other_biological_info
 images/Proportion_of_peptides.png
 images/RDG.png
 images/README.md
 images/current_representation.png
 tests/__init__.py
+tests/test_add_features.py
+tests/test_add_remove_edge.py
 tests/test_basics.py
+tests/test_edgeObj.py
 tests/test_get.py
-tests/test_inset_orf.py
 tests/test_load_graph.py
+tests/test_newick.py
+tests/test_nodeObj.py
 tests/test_read_write.py
-tests/test_remove_edge.py
 tests/test_update_edge.py
```

### Comparing `RDG-0.1.4.1/README.md` & `RDG-0.1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `RDG-0.1.4.1/images/Impact_of_point_mutationspng` & `RDG-0.1.4.2/images/Impact_of_point_mutationspng`

 * *Files identical despite different names*

### Comparing `RDG-0.1.4.1/images/ORF_plot.png` & `RDG-0.1.4.2/images/ORF_plot.png`

 * *Files identical despite different names*

### Comparing `RDG-0.1.4.1/images/Other_biological_info` & `RDG-0.1.4.2/images/Other_biological_info`

 * *Files identical despite different names*

### Comparing `RDG-0.1.4.1/images/Proportion_of_peptides.png` & `RDG-0.1.4.2/images/Proportion_of_peptides.png`

 * *Files identical despite different names*

### Comparing `RDG-0.1.4.1/images/RDG.png` & `RDG-0.1.4.2/images/RDG.png`

 * *Files identical despite different names*

### Comparing `RDG-0.1.4.1/images/current_representation.png` & `RDG-0.1.4.2/images/current_representation.png`

 * *Files identical despite different names*

### Comparing `RDG-0.1.4.1/tests/test_update_edge.py` & `RDG-0.1.4.2/tests/test_update_edge.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,44 +4,61 @@
 def test_update_edge_input_to_new_to_node():
     g = RDG()
     g = RDG.load_example(g)
     node_key = g.get_new_node_key()
 
     start_codon_position = 15
     stop_codon_position = 25
-    start_node = Node(key=node_key, node_type="start_codon", coordinates=start_codon_position, edges_in=[], edges_out=[], nodes_in=[], nodes_out=[])
+    start_node = Node(
+        key=node_key,
+        node_type="start_codon",
+        coordinates=start_codon_position,
+        edges_in=[],
+        edges_out=[],
+        nodes_in=[],
+        nodes_out=[],
+    )
 
     node_key = node_key + 1
-    stop_node = Node(key=node_key, node_type="stop_codon", coordinates=stop_codon_position, edges_in=[], edges_out=[], nodes_in=[], nodes_out=[])
-    
-    g.update_edge(2, 1, 5, (1,1000))
+    stop_node = Node(
+        key=node_key,
+        node_type="stop_codon",
+        coordinates=stop_codon_position,
+        edges_in=[],
+        edges_out=[],
+        nodes_in=[],
+        nodes_out=[],
+    )
+
+    g.update_edge(2, 1, 5, (1, 1000))
     tf = 2 in g.edges
     assert 2 in g.nodes[5].input_edges
 
+
 def test_update_edge_input_to_old_to_node():
     g = RDG()
     g = RDG.load_example(g)
-    g.update_edge(2, 1, 5, (1,1000))
+    g.update_edge(2, 1, 5, (1, 1000))
     assert 2 not in g.nodes[2].input_edges
 
 
 def test_update_edge_input_to_new_from_node():
     g = RDG()
     g = RDG.load_example(g)
 
-    g.update_edge(2, 1, 5, (1,1000))
+    g.update_edge(2, 1, 5, (1, 1000))
     assert 2 in g.nodes[1].output_edges
 
 
 def test_update_edge_input_to_old_from_node():
     g = RDG()
     g = RDG.load_example(g)
-    g.update_edge(2, 1, 5, (1,1000))
+    g.update_edge(2, 1, 5, (1, 1000))
     assert 2 not in g.nodes[3].output_edges
 
 
 def test_update_edge_input_to_new_to_node():
     g = RDG()
     g = RDG.load_example(g)
 
-    g.update_edge(2, 1, 5, (1,1000))
-    assert 2 in g.nodes[1].output_edges
+    g.update_edge(2, 1, 5, (1, 1000))
+    assert 2 in g.nodes[1].output_edges
```

