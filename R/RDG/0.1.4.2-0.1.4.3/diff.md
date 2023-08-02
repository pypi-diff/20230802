# Comparing `tmp/RDG-0.1.4.2.tar.gz` & `tmp/RDG-0.1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/RDG-0.1.4.2.tar", last modified: Wed Aug  2 09:38:25 2023, max compression
+gzip compressed data, was "dist/RDG-0.1.4.3.tar", last modified: Wed Aug  2 10:18:43 2023, max compression
```

## Comparing `RDG-0.1.4.2.tar` & `RDG-0.1.4.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-08-02 09:38:25.541573 RDG-0.1.4.2/
--rw-rw-r--   0 jack      (1000) jack      (1000)     1903 2021-12-06 12:38:15.000000 RDG-0.1.4.2/.gitignore
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-08-02 09:38:25.537573 RDG-0.1.4.2/.vscode/
--rw-rw-r--   0 jack      (1000) jack      (1000)       44 2022-01-17 13:41:16.000000 RDG-0.1.4.2/.vscode/settings.json
--rw-rw-r--   0 jack      (1000) jack      (1000)     1069 2021-11-30 13:45:44.000000 RDG-0.1.4.2/LICENSE
--rw-rw-r--   0 jack      (1000) jack      (1000)      179 2023-08-02 09:38:25.541573 RDG-0.1.4.2/PKG-INFO
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-08-02 09:38:25.537573 RDG-0.1.4.2/RDG/
--rw-rw-r--   0 jack      (1000) jack      (1000)    79290 2023-04-19 11:14:02.000000 RDG-0.1.4.2/RDG/RDG.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     3280 2023-02-23 17:46:03.000000 RDG-0.1.4.2/RDG/RDG_to_file.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      105 2023-02-23 18:52:36.000000 RDG-0.1.4.2/RDG/__init__.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     4056 2023-02-23 19:37:31.000000 RDG-0.1.4.2/RDG/build_RDG_from_sequence.py
--rw-rw-r--   0 jack      (1000) jack      (1000)    12515 2023-02-22 09:32:19.000000 RDG-0.1.4.2/RDG/dynamic_build.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     8400 2023-07-12 14:42:43.000000 RDG-0.1.4.2/RDG/plot_RDG.py
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-08-02 09:38:25.537573 RDG-0.1.4.2/RDG.egg-info/
--rw-rw-r--   0 jack      (1000) jack      (1000)      179 2023-08-02 09:38:25.000000 RDG-0.1.4.2/RDG.egg-info/PKG-INFO
--rw-rw-r--   0 jack      (1000) jack      (1000)      739 2023-08-02 09:38:25.000000 RDG-0.1.4.2/RDG.egg-info/SOURCES.txt
--rw-rw-r--   0 jack      (1000) jack      (1000)        1 2023-08-02 09:38:25.000000 RDG-0.1.4.2/RDG.egg-info/dependency_links.txt
--rw-rw-r--   0 jack      (1000) jack      (1000)       10 2023-08-02 09:38:25.000000 RDG-0.1.4.2/RDG.egg-info/top_level.txt
--rw-rw-r--   0 jack      (1000) jack      (1000)     3446 2022-10-03 10:20:00.000000 RDG-0.1.4.2/README.md
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-08-02 09:38:25.541573 RDG-0.1.4.2/images/
--rw-rw-r--   0 jack      (1000) jack      (1000)    86784 2022-02-16 10:51:06.000000 RDG-0.1.4.2/images/Impact_of_point_mutationspng
--rw-rw-r--   0 jack      (1000) jack      (1000)    16077 2022-02-16 10:52:18.000000 RDG-0.1.4.2/images/ORF_plot.png
--rw-rw-r--   0 jack      (1000) jack      (1000)    70987 2022-02-16 10:48:41.000000 RDG-0.1.4.2/images/Other_biological_info
--rw-rw-r--   0 jack      (1000) jack      (1000)    38683 2022-02-16 10:50:40.000000 RDG-0.1.4.2/images/Proportion_of_peptides.png
--rw-rw-r--   0 jack      (1000) jack      (1000)    64995 2022-02-16 10:50:16.000000 RDG-0.1.4.2/images/RDG.png
--rw-rw-r--   0 jack      (1000) jack      (1000)        1 2022-02-16 10:55:59.000000 RDG-0.1.4.2/images/README.md
--rw-rw-r--   0 jack      (1000) jack      (1000)    23419 2022-02-16 10:51:54.000000 RDG-0.1.4.2/images/current_representation.png
--rw-rw-r--   0 jack      (1000) jack      (1000)       38 2023-08-02 09:38:25.541573 RDG-0.1.4.2/setup.cfg
--rw-rw-r--   0 jack      (1000) jack      (1000)      123 2023-08-02 09:38:23.000000 RDG-0.1.4.2/setup.py
--rw-rw-r--   0 jack      (1000) jack      (1000)    67696 2023-02-23 19:38:15.000000 RDG-0.1.4.2/test.nwk
--rw-r--r--   0 jack      (1000) jack      (1000)    20480 2023-02-22 14:29:35.000000 RDG-0.1.4.2/test.rdg
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-08-02 09:38:25.541573 RDG-0.1.4.2/tests/
--rw-rw-r--   0 jack      (1000) jack      (1000)        0 2023-02-22 14:20:03.000000 RDG-0.1.4.2/tests/__init__.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     3885 2023-02-23 13:10:53.000000 RDG-0.1.4.2/tests/test_add_features.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      744 2023-02-21 14:15:19.000000 RDG-0.1.4.2/tests/test_add_remove_edge.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      439 2023-02-21 14:15:19.000000 RDG-0.1.4.2/tests/test_basics.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      681 2023-02-21 14:15:19.000000 RDG-0.1.4.2/tests/test_edgeObj.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     3867 2023-02-23 13:12:38.000000 RDG-0.1.4.2/tests/test_get.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     1921 2023-02-21 14:15:19.000000 RDG-0.1.4.2/tests/test_load_graph.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      826 2023-04-19 11:47:35.000000 RDG-0.1.4.2/tests/test_newick.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     1265 2023-02-22 11:05:16.000000 RDG-0.1.4.2/tests/test_nodeObj.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      828 2023-02-22 17:10:38.000000 RDG-0.1.4.2/tests/test_read_write.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     1448 2023-02-21 14:15:19.000000 RDG-0.1.4.2/tests/test_update_edge.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-08-02 10:18:43.966894 RDG-0.1.4.3/
+-rw-rw-r--   0 jack      (1000) jack      (1000)     1903 2021-12-06 12:38:15.000000 RDG-0.1.4.3/.gitignore
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-08-02 10:18:43.958894 RDG-0.1.4.3/.vscode/
+-rw-rw-r--   0 jack      (1000) jack      (1000)       44 2022-01-17 13:41:16.000000 RDG-0.1.4.3/.vscode/settings.json
+-rw-rw-r--   0 jack      (1000) jack      (1000)     1069 2021-11-30 13:45:44.000000 RDG-0.1.4.3/LICENSE
+-rw-rw-r--   0 jack      (1000) jack      (1000)       71 2023-08-02 10:18:43.962894 RDG-0.1.4.3/PKG-INFO
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-08-02 10:18:43.962894 RDG-0.1.4.3/RDG/
+-rw-rw-r--   0 jack      (1000) jack      (1000)    79173 2023-08-02 10:16:09.000000 RDG-0.1.4.3/RDG/RDG.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     3241 2023-08-02 10:16:30.000000 RDG-0.1.4.3/RDG/RDG_to_file.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      105 2023-02-23 18:52:36.000000 RDG-0.1.4.3/RDG/__init__.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     4056 2023-02-23 19:37:31.000000 RDG-0.1.4.3/RDG/build_RDG_from_sequence.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)    12006 2023-08-02 10:18:01.000000 RDG-0.1.4.3/RDG/dynamic_build.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     8400 2023-07-12 14:42:43.000000 RDG-0.1.4.3/RDG/plot_RDG.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-08-02 10:18:43.962894 RDG-0.1.4.3/RDG.egg-info/
+-rw-rw-r--   0 jack      (1000) jack      (1000)       71 2023-08-02 10:18:43.000000 RDG-0.1.4.3/RDG.egg-info/PKG-INFO
+-rw-rw-r--   0 jack      (1000) jack      (1000)      739 2023-08-02 10:18:43.000000 RDG-0.1.4.3/RDG.egg-info/SOURCES.txt
+-rw-rw-r--   0 jack      (1000) jack      (1000)        1 2023-08-02 10:18:43.000000 RDG-0.1.4.3/RDG.egg-info/dependency_links.txt
+-rw-rw-r--   0 jack      (1000) jack      (1000)       10 2023-08-02 10:18:43.000000 RDG-0.1.4.3/RDG.egg-info/top_level.txt
+-rw-rw-r--   0 jack      (1000) jack      (1000)     3446 2022-10-03 10:20:00.000000 RDG-0.1.4.3/README.md
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-08-02 10:18:43.962894 RDG-0.1.4.3/images/
+-rw-rw-r--   0 jack      (1000) jack      (1000)    86784 2022-02-16 10:51:06.000000 RDG-0.1.4.3/images/Impact_of_point_mutationspng
+-rw-rw-r--   0 jack      (1000) jack      (1000)    16077 2022-02-16 10:52:18.000000 RDG-0.1.4.3/images/ORF_plot.png
+-rw-rw-r--   0 jack      (1000) jack      (1000)    70987 2022-02-16 10:48:41.000000 RDG-0.1.4.3/images/Other_biological_info
+-rw-rw-r--   0 jack      (1000) jack      (1000)    38683 2022-02-16 10:50:40.000000 RDG-0.1.4.3/images/Proportion_of_peptides.png
+-rw-rw-r--   0 jack      (1000) jack      (1000)    64995 2022-02-16 10:50:16.000000 RDG-0.1.4.3/images/RDG.png
+-rw-rw-r--   0 jack      (1000) jack      (1000)        1 2022-02-16 10:55:59.000000 RDG-0.1.4.3/images/README.md
+-rw-rw-r--   0 jack      (1000) jack      (1000)    23419 2022-02-16 10:51:54.000000 RDG-0.1.4.3/images/current_representation.png
+-rw-rw-r--   0 jack      (1000) jack      (1000)       38 2023-08-02 10:18:43.966894 RDG-0.1.4.3/setup.cfg
+-rw-rw-r--   0 jack      (1000) jack      (1000)      123 2023-08-02 10:18:40.000000 RDG-0.1.4.3/setup.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)    67696 2023-02-23 19:38:15.000000 RDG-0.1.4.3/test.nwk
+-rw-r--r--   0 jack      (1000) jack      (1000)    20480 2023-02-22 14:29:35.000000 RDG-0.1.4.3/test.rdg
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-08-02 10:18:43.962894 RDG-0.1.4.3/tests/
+-rw-rw-r--   0 jack      (1000) jack      (1000)        0 2023-02-22 14:20:03.000000 RDG-0.1.4.3/tests/__init__.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     3885 2023-02-23 13:10:53.000000 RDG-0.1.4.3/tests/test_add_features.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      744 2023-02-21 14:15:19.000000 RDG-0.1.4.3/tests/test_add_remove_edge.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      439 2023-02-21 14:15:19.000000 RDG-0.1.4.3/tests/test_basics.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      681 2023-02-21 14:15:19.000000 RDG-0.1.4.3/tests/test_edgeObj.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     3867 2023-02-23 13:12:38.000000 RDG-0.1.4.3/tests/test_get.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     1921 2023-02-21 14:15:19.000000 RDG-0.1.4.3/tests/test_load_graph.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      826 2023-04-19 11:47:35.000000 RDG-0.1.4.3/tests/test_newick.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     1265 2023-02-22 11:05:16.000000 RDG-0.1.4.3/tests/test_nodeObj.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      828 2023-02-22 17:10:38.000000 RDG-0.1.4.3/tests/test_read_write.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     1448 2023-02-21 14:15:19.000000 RDG-0.1.4.3/tests/test_update_edge.py
```

### Comparing `RDG-0.1.4.2/.gitignore` & `RDG-0.1.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `RDG-0.1.4.2/LICENSE` & `RDG-0.1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `RDG-0.1.4.2/RDG/RDG.py` & `RDG-0.1.4.3/RDG/RDG.py`

 * *Files 0% similar despite different names*

```diff
@@ -2318,15 +2318,14 @@
                 raise ValueError("Graph has more than one startpoint")
             node = startpoints[0]
             root = node
 
         # Base case: If the current node is an endpoint, return its label and branch length
         if node in self.get_endpoints():
             path_to_root = self.root_to_node_of_acyclic_node_path(node)
-            print(path_to_root)
             branch_lengths = [self.nodes[i].node_start for i in path_to_root][:-1]
             branch_length = self.nodes[node].node_start - sum(branch_lengths)
             return f"{node}:{branch_length}"
 
         # Recursive case: Build the Newick string for the children of the current node
         children = self.nodes[node].output_nodes
 
@@ -2341,15 +2340,14 @@
         newick = f"({','.join(child_newick_strings)}){node}"
 
         # Calculate branch length based on the difference in 'position' values
         if root != node:
             path_to_root = self.root_to_node_of_acyclic_node_path(node)
             branch_lengths = [self.nodes[i].node_start for i in path_to_root]
             branch_length = branch_lengths[-1] - branch_lengths[-2]
-            print(node,  self.nodes[node].node_start, branch_length, branch_lengths)
             newick += f":{branch_length}"
 
         # If the current node is the root, append the final semicolon
         if node == root:
             newick += ";"
 
         return newick
```

### Comparing `RDG-0.1.4.2/RDG/RDG_to_file.py` & `RDG-0.1.4.3/RDG/RDG_to_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,14 @@
         The locus of the graph to load
 
     cache_file : str
         The name of the file to load from (should end in .sqlite)
     '''
     try:
         with SqliteDict(cache_file) as mydict:
-            print(list(mydict.keys()))
             graph_dict = mydict[
                 locus
             ]  # No need to use commit(), since we are only loading data!
     except Exception as ex:
         raise Exception("Error during loading data:", ex)
 
     dg = RDG()
```

### Comparing `RDG-0.1.4.2/RDG/build_RDG_from_sequence.py` & `RDG-0.1.4.3/RDG/build_RDG_from_sequence.py`

 * *Files identical despite different names*

### Comparing `RDG-0.1.4.2/RDG/dynamic_build.py` & `RDG-0.1.4.3/RDG/dynamic_build.py`

 * *Files 5% similar despite different names*

```diff
@@ -191,15 +191,14 @@
                 graph.nodes[readthrough_key].node_start,
                 next_stop_codon_position,
             ),
         )
         graph.add_edge(coding, readthrough_key, new_stop_node.key)
 
         graph.nodes[readthrough_key].node_type = "stop"
-        print(graph.nodes[readthrough_key].output_nodes)
 
         terminal_node_key = graph.get_new_node_key()
         three_prime_terminal_key = graph.nodes[readthrough_key].output_nodes[0]
 
         new_3_prime_edge = graph.get_new_edge_key()
         three_prime = Edge(
             key=new_3_prime_edge,
@@ -217,22 +216,15 @@
             key=terminal_node_key,
             node_type="3_prime",
             position=graph.nodes[three_prime_terminal_key].node_start,
         )
         graph.add_node(terminal_node)
         graph.add_edge(three_prime, new_stop_node.key, terminal_node_key)
 
-        print("out node: ", graph.nodes[terminal_node_key].output_nodes)
-        print("In node: ", graph.nodes[terminal_node_key].input_nodes)
-        print("In edge: ", graph.nodes[terminal_node_key].input_edges)
-        print(graph.edges[graph.nodes[terminal_node_key].input_edges[0]].from_node)
-
-        for n in graph.nodes.keys():
-            if 7 in graph.nodes[n].output_nodes:
-                print("7 is in: ", n, graph.nodes[n].output_nodes)
+
         # terminal_node_key2 = graph.get_new_node_key()
 
         # terminal_node2 = Node(
         #     key=terminal_node_key2,
         #     node_type="3_prime",
         #     position=graph.nodes[three_prime_terminal_key].node_start,
         #     edges_in=[new_3_prime_edge],
```

### Comparing `RDG-0.1.4.2/RDG/plot_RDG.py` & `RDG-0.1.4.3/RDG/plot_RDG.py`

 * *Files identical despite different names*

### Comparing `RDG-0.1.4.2/RDG.egg-info/SOURCES.txt` & `RDG-0.1.4.3/RDG.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RDG-0.1.4.2/README.md` & `RDG-0.1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `RDG-0.1.4.2/images/Impact_of_point_mutationspng` & `RDG-0.1.4.3/images/Impact_of_point_mutationspng`

 * *Files identical despite different names*

### Comparing `RDG-0.1.4.2/images/ORF_plot.png` & `RDG-0.1.4.3/images/ORF_plot.png`

 * *Files identical despite different names*

### Comparing `RDG-0.1.4.2/images/Other_biological_info` & `RDG-0.1.4.3/images/Other_biological_info`

 * *Files identical despite different names*

### Comparing `RDG-0.1.4.2/images/Proportion_of_peptides.png` & `RDG-0.1.4.3/images/Proportion_of_peptides.png`

 * *Files identical despite different names*

### Comparing `RDG-0.1.4.2/images/RDG.png` & `RDG-0.1.4.3/images/RDG.png`

 * *Files identical despite different names*

### Comparing `RDG-0.1.4.2/images/current_representation.png` & `RDG-0.1.4.3/images/current_representation.png`

 * *Files identical despite different names*

### Comparing `RDG-0.1.4.2/test.nwk` & `RDG-0.1.4.3/test.nwk`

 * *Files identical despite different names*

### Comparing `RDG-0.1.4.2/test.rdg` & `RDG-0.1.4.3/test.rdg`

 * *Files identical despite different names*

### Comparing `RDG-0.1.4.2/tests/test_add_features.py` & `RDG-0.1.4.3/tests/test_add_features.py`

 * *Files identical despite different names*

### Comparing `RDG-0.1.4.2/tests/test_add_remove_edge.py` & `RDG-0.1.4.3/tests/test_add_remove_edge.py`

 * *Files identical despite different names*

### Comparing `RDG-0.1.4.2/tests/test_edgeObj.py` & `RDG-0.1.4.3/tests/test_edgeObj.py`

 * *Files identical despite different names*

### Comparing `RDG-0.1.4.2/tests/test_get.py` & `RDG-0.1.4.3/tests/test_get.py`

 * *Files identical despite different names*

### Comparing `RDG-0.1.4.2/tests/test_load_graph.py` & `RDG-0.1.4.3/tests/test_load_graph.py`

 * *Files identical despite different names*

### Comparing `RDG-0.1.4.2/tests/test_newick.py` & `RDG-0.1.4.3/tests/test_newick.py`

 * *Files identical despite different names*

### Comparing `RDG-0.1.4.2/tests/test_nodeObj.py` & `RDG-0.1.4.3/tests/test_nodeObj.py`

 * *Files identical despite different names*

### Comparing `RDG-0.1.4.2/tests/test_read_write.py` & `RDG-0.1.4.3/tests/test_read_write.py`

 * *Files identical despite different names*

### Comparing `RDG-0.1.4.2/tests/test_update_edge.py` & `RDG-0.1.4.3/tests/test_update_edge.py`

 * *Files identical despite different names*

