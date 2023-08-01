# Comparing `tmp/topohub-0.1.tar.gz` & `tmp/topohub-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "topohub-0.1.tar", last modified: Tue Aug  1 23:02:10 2023, max compression
+gzip compressed data, was "topohub-0.2.tar", last modified: Tue Aug  1 23:39:54 2023, max compression
```

## Comparing `topohub-0.1.tar` & `topohub-0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 jurkiew   (1000) jurkiew   (1000)        0 2023-08-01 23:02:10.996045 topohub-0.1/
--rw-rw-r--   0 jurkiew   (1000) jurkiew   (1000)     1073 2023-07-28 21:06:53.000000 topohub-0.1/LICENSE
--rw-rw-r--   0 jurkiew   (1000) jurkiew   (1000)      972 2023-08-01 23:02:10.996045 topohub-0.1/PKG-INFO
--rw-rw-r--   0 jurkiew   (1000) jurkiew   (1000)        0 2023-07-28 21:07:06.000000 topohub-0.1/README.md
--rw-rw-r--   0 jurkiew   (1000) jurkiew   (1000)       38 2023-08-01 23:02:10.996045 topohub-0.1/setup.cfg
--rw-rw-r--   0 jurkiew   (1000) jurkiew   (1000)     1294 2023-08-01 23:02:03.000000 topohub-0.1/setup.py
-drwxrwxr-x   0 jurkiew   (1000) jurkiew   (1000)        0 2023-08-01 23:02:10.996045 topohub-0.1/topohub/
--rw-rw-r--   0 jurkiew   (1000) jurkiew   (1000)       20 2023-08-01 22:44:17.000000 topohub-0.1/topohub/__init__.py
--rw-rw-r--   0 jurkiew   (1000) jurkiew   (1000)    15688 2023-07-31 01:45:17.000000 topohub-0.1/topohub/generate.py
--rw-rw-r--   0 jurkiew   (1000) jurkiew   (1000)    18307 2023-07-31 01:43:47.000000 topohub-0.1/topohub/graph.py
--rw-rw-r--   0 jurkiew   (1000) jurkiew   (1000)     2985 2020-12-28 01:40:52.000000 topohub-0.1/topohub/mininet.py
-drwxrwxr-x   0 jurkiew   (1000) jurkiew   (1000)        0 2023-08-01 23:02:10.996045 topohub-0.1/topohub.egg-info/
--rw-rw-r--   0 jurkiew   (1000) jurkiew   (1000)      972 2023-08-01 23:02:10.000000 topohub-0.1/topohub.egg-info/PKG-INFO
--rw-rw-r--   0 jurkiew   (1000) jurkiew   (1000)      226 2023-08-01 23:02:10.000000 topohub-0.1/topohub.egg-info/SOURCES.txt
--rw-rw-r--   0 jurkiew   (1000) jurkiew   (1000)        1 2023-08-01 23:02:10.000000 topohub-0.1/topohub.egg-info/dependency_links.txt
--rw-rw-r--   0 jurkiew   (1000) jurkiew   (1000)        8 2023-08-01 23:02:10.000000 topohub-0.1/topohub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:39:54.020014 topohub-0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-01 23:39:44.000000 topohub-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-08-01 23:39:54.020014 topohub-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 23:39:44.000000 topohub-0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 23:39:54.020014 topohub-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-08-01 23:39:44.000000 topohub-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:39:54.020014 topohub-0.2/topohub/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-01 23:39:44.000000 topohub-0.2/topohub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15730 2023-08-01 23:39:44.000000 topohub-0.2/topohub/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18321 2023-08-01 23:39:44.000000 topohub-0.2/topohub/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-08-01 23:39:44.000000 topohub-0.2/topohub/mininet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:39:54.020014 topohub-0.2/topohub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-08-01 23:39:54.000000 topohub-0.2/topohub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-08-01 23:39:54.000000 topohub-0.2/topohub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 23:39:54.000000 topohub-0.2/topohub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-01 23:39:54.000000 topohub-0.2/topohub.egg-info/top_level.txt
```

### Comparing `topohub-0.1/LICENSE` & `topohub-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `topohub-0.1/PKG-INFO` & `topohub-0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 Metadata-Version: 2.1
 Name: topohub
-Version: 0.1
+Version: 0.2
 Summary: A repository of reference Gabriel graph and real-world topologies for networking research
 Home-page: https://github.com/piotrjurkiewicz/topohub
 Author: Piotr Jurkiewicz
 Author-email: piotr.jerzy.jurkiewicz@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Topic :: Internet
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: System :: Networking
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Telecommunications Industry
 Description-Content-Type: text/markdown
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `topohub-0.1/setup.py` & `topohub-0.2/setup.py`

 * *Files identical despite different names*

### Comparing `topohub-0.1/topohub/generate.py` & `topohub-0.2/topohub/generate.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 import os
 import random
 import sys
 import time
 
 import networkx as nx
 
-# from . import graph
-import graph
+import topohub.graph
 
 json.encoder.c_make_encoder = None
 MAX_GABRIEL_NODES = 4096
 
 class RoundingFloat(float):
     __repr__ = staticmethod(lambda x: format(x, '.2f'))
 
@@ -24,29 +23,29 @@
     @classmethod
     def generate_topo(cls, *args):
         return {}
 
     @classmethod
     def save_topo(cls, *args, **kwargs):
         g = nx.node_link_graph(cls.generate_topo(*args))
-        graph.calculate_utilization(g)
+        topohub.graph.calculate_utilization(g)
         if 'filename' in kwargs:
             filename = kwargs['filename']
         else:
             filename = f'mininet/topo_lib/{g.name}'
         os.makedirs(filename.rpartition('/')[0], exist_ok=True)
         json.dump(nx.node_link_data(g), open(f'{filename}.json', 'w'), indent=kwargs.get('indent', 0))
         ps = None
         if kwargs.get('with_plot'):
-            graph.save_topo_graph_svg(g, filename, cls.scaling)
+            topohub.graph.save_topo_graph_svg(g, filename, cls.scaling)
         if kwargs.get('with_path_stats'):
-            ps = graph.path_stats(g)
-            graph.path_stats_print(ps, filename)
+            ps = topohub.graph.path_stats(g)
+            topohub.graph.path_stats_print(ps, filename)
         if kwargs.get('with_topo_stats'):
-            ts = graph.topo_stats(g, ps)
+            ts = topohub.graph.topo_stats(g, ps)
             # graph.topo_stats_print(ts, g.graph['name'], filename)
             g.graph['stats'] = ts
         json.encoder.float = RoundingFloat
         json.dump(nx.node_link_data(g), open(f'{filename}.json', 'w'), indent=kwargs.get('indent', 0), default=lambda x: format(x, '.2f'))
         json.encoder.float = float
 
 class SNDLibGenerator(TopoGenerator):
@@ -92,15 +91,15 @@
                 nodes.append({'id': node, 'pos': (float(lon), float(lat))})
 
             if mode == 'links':
                 if line.startswith(")"):
                     mode = None
                     continue
                 node0, node1 = line.split()[2:4]
-                distance = graph.haversine(pos[node0], pos[node1])
+                distance = topohub.graph.haversine(pos[node0], pos[node1])
                 links.append({'source': node0, 'target': node1, 'distance': distance})
 
             if mode == 'demands':
                 if line.startswith(")"):
                     mode = None
                     continue
                 node0, node1 = line.split()[2:4]
@@ -164,15 +163,15 @@
                     lon = line.split()[-1]
                 elif line.startswith("    Latitude "):
                     lat = line.split()[-1]
 
             if mode == 'edge':
                 if line.startswith("  ]"):
                     try:
-                        distance = graph.haversine(pos[node0], pos[node1])
+                        distance = topohub.graph.haversine(pos[node0], pos[node1])
                         links.append({'source': node_id_to_name[node0], 'target': node_id_to_name[node1], 'distance': distance})
                     except KeyError:
                         pass
                     mode = None
                 elif line.startswith("    source "):
                     node0 = line.split()[-1]
                 elif line.startswith("    target "):
```

### Comparing `topohub-0.1/topohub/graph.py` & `topohub-0.2/topohub/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -268,15 +268,15 @@
         scale = 1000 / max(max0 - min0, max1 - min1)
         for n in pos:
             pos[n] = pos[n][0] * scale, (max1 - pos[n][1]) * scale
         max0, max1, min0, min1 = minmax(pos)
 
     with open(filename + '.svg', 'w') as f:
         f.write(f'<svg width="{max0 - min0 + 90:.2f}" height="{max1 - min1 + 90:.2f}" viewBox="{min0 - 45:.2f} {min1 - 45:.2f} {max0 - min0 + 90:.2f} {max1 - min1 + 90:.2f}" xmlns="http://www.w3.org/2000/svg">\n')
-        f.write('<style>path {stroke-width: 6; stroke: grey; fill: none;} circle {stroke: none; fill: lightblue;} text {font-size: 16; font-family: sans-serif; fill: black; text-anchor:middle;}</style>\n')
+        f.write('<style>path {fill: none; stroke: grey; stroke-width: 6;} circle {fill: lightblue; stroke: none;} text {fill: black; stroke: none; font-size: 16; font-family: sans-serif; text-anchor:middle;}</style>\n')
 
         for e in g.edges:
             x0, y0 = pos[e[0]]
             x1, y1 = pos[e[1]]
             f.write(f'<path d="M{x0:.2f},{y0:.2f},{x1:.2f},{y1:.2f}"/>\n')
 
         for n, (x, y) in pos.items():
```

### Comparing `topohub-0.1/topohub/mininet.py` & `topohub-0.2/topohub/mininet.py`

 * *Files identical despite different names*

### Comparing `topohub-0.1/topohub.egg-info/PKG-INFO` & `topohub-0.2/topohub.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 Metadata-Version: 2.1
 Name: topohub
-Version: 0.1
+Version: 0.2
 Summary: A repository of reference Gabriel graph and real-world topologies for networking research
 Home-page: https://github.com/piotrjurkiewicz/topohub
 Author: Piotr Jurkiewicz
 Author-email: piotr.jerzy.jurkiewicz@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Topic :: Internet
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: System :: Networking
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Telecommunications Industry
 Description-Content-Type: text/markdown
 License-File: LICENSE
-
-UNKNOWN
-
```

