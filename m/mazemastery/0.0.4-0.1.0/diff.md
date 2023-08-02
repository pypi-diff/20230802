# Comparing `tmp/mazemastery-0.0.4.tar.gz` & `tmp/mazemastery-0.1.0.tar.gz`

## Comparing `mazemastery-0.0.4.tar` & `mazemastery-0.1.0.tar`

### file list

```diff
@@ -1,42 +1,43 @@
--rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/__init__.py
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/api.py
--rw-r--r--   0        0        0     6828 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/debug_menu.py
--rw-r--r--   0        0        0     6302 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/maze.py
--rw-r--r--   0        0        0    35221 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/renderer.py
--rw-r--r--   0        0        0     3478 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/state.py
--rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/styles.py
--rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/cloud_e.png
--rw-r--r--   0        0        0     4986 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/cloud_n.png
--rw-r--r--   0        0        0     5366 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/cloud_ne.png
--rw-r--r--   0        0        0     5459 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/cloud_ne_inner_corner.png
--rw-r--r--   0        0        0     5120 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/cloud_ne_inner_corner_e.png
--rw-r--r--   0        0        0     5113 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/cloud_ne_inner_corner_n.png
--rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/cloud_nw.png
--rw-r--r--   0        0        0     5450 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/cloud_nw_inner_corner.png
--rw-r--r--   0        0        0     5188 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/cloud_nw_inner_corner_e.png
--rw-r--r--   0        0        0     4867 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/cloud_nw_inner_corner_n.png
--rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/cloud_nw_inner_corner_w.png
--rw-r--r--   0        0        0     4915 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/cloud_s.png
--rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/cloud_s_seam.png
--rw-r--r--   0        0        0     5352 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/cloud_se.png
--rw-r--r--   0        0        0     5037 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/cloud_se_inner_corner.png
--rw-r--r--   0        0        0     4950 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/cloud_se_inner_corner_e.png
--rw-r--r--   0        0        0     4900 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/cloud_se_inner_corner_s.png
--rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/cloud_se_spec.png
--rw-r--r--   0        0        0     5332 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/cloud_sw.png
--rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/cloud_sw_inner_corner.png
--rw-r--r--   0        0        0     4933 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/cloud_sw_inner_corner_s.png
--rw-r--r--   0        0        0     4966 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/cloud_sw_inner_corner_w.png
--rw-r--r--   0        0        0     5005 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/cloud_sw_spec.png
--rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/cloud_w.png
--rw-r--r--   0        0        0     7759 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/minotaur.png
--rw-r--r--   0        0        0    11075 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/warrior_down.png
--rw-r--r--   0        0        0    11600 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/warrior_left.png
--rw-r--r--   0        0        0    11852 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/warrior_right.png
--rw-r--r--   0        0        0    10990 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/warrior_up.png
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 mazemastery-0.0.4/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 mazemastery-0.0.4/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mazemastery-0.0.4/README.md
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 mazemastery-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 mazemastery-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 mazemastery-0.1.0/requirements.txt
+-rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 mazemastery-0.1.0/src/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mazemastery-0.1.0/src/mazemastery/__init__.py
+-rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 mazemastery-0.1.0/src/mazemastery/api.py
+-rw-r--r--   0        0        0     6701 2020-02-02 00:00:00.000000 mazemastery-0.1.0/src/mazemastery/debug_menu.py
+-rw-r--r--   0        0        0     6302 2020-02-02 00:00:00.000000 mazemastery-0.1.0/src/mazemastery/maze.py
+-rw-r--r--   0        0        0    35221 2020-02-02 00:00:00.000000 mazemastery-0.1.0/src/mazemastery/renderer.py
+-rw-r--r--   0        0        0     3478 2020-02-02 00:00:00.000000 mazemastery-0.1.0/src/mazemastery/state.py
+-rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 mazemastery-0.1.0/src/mazemastery/styles.py
+-rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 mazemastery-0.1.0/src/mazemastery/sprites/cloud_e.png
+-rw-r--r--   0        0        0     4986 2020-02-02 00:00:00.000000 mazemastery-0.1.0/src/mazemastery/sprites/cloud_n.png
+-rw-r--r--   0        0        0     5366 2020-02-02 00:00:00.000000 mazemastery-0.1.0/src/mazemastery/sprites/cloud_ne.png
+-rw-r--r--   0        0        0     5459 2020-02-02 00:00:00.000000 mazemastery-0.1.0/src/mazemastery/sprites/cloud_ne_inner_corner.png
+-rw-r--r--   0        0        0     5120 2020-02-02 00:00:00.000000 mazemastery-0.1.0/src/mazemastery/sprites/cloud_ne_inner_corner_e.png
+-rw-r--r--   0        0        0     5113 2020-02-02 00:00:00.000000 mazemastery-0.1.0/src/mazemastery/sprites/cloud_ne_inner_corner_n.png
+-rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 mazemastery-0.1.0/src/mazemastery/sprites/cloud_nw.png
+-rw-r--r--   0        0        0     5450 2020-02-02 00:00:00.000000 mazemastery-0.1.0/src/mazemastery/sprites/cloud_nw_inner_corner.png
+-rw-r--r--   0        0        0     5188 2020-02-02 00:00:00.000000 mazemastery-0.1.0/src/mazemastery/sprites/cloud_nw_inner_corner_e.png
+-rw-r--r--   0        0        0     4867 2020-02-02 00:00:00.000000 mazemastery-0.1.0/src/mazemastery/sprites/cloud_nw_inner_corner_n.png
+-rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 mazemastery-0.1.0/src/mazemastery/sprites/cloud_nw_inner_corner_w.png
+-rw-r--r--   0        0        0     4915 2020-02-02 00:00:00.000000 mazemastery-0.1.0/src/mazemastery/sprites/cloud_s.png
+-rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 mazemastery-0.1.0/src/mazemastery/sprites/cloud_s_seam.png
+-rw-r--r--   0        0        0     5352 2020-02-02 00:00:00.000000 mazemastery-0.1.0/src/mazemastery/sprites/cloud_se.png
+-rw-r--r--   0        0        0     5037 2020-02-02 00:00:00.000000 mazemastery-0.1.0/src/mazemastery/sprites/cloud_se_inner_corner.png
+-rw-r--r--   0        0        0     4950 2020-02-02 00:00:00.000000 mazemastery-0.1.0/src/mazemastery/sprites/cloud_se_inner_corner_e.png
+-rw-r--r--   0        0        0     4900 2020-02-02 00:00:00.000000 mazemastery-0.1.0/src/mazemastery/sprites/cloud_se_inner_corner_s.png
+-rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 mazemastery-0.1.0/src/mazemastery/sprites/cloud_se_spec.png
+-rw-r--r--   0        0        0     5332 2020-02-02 00:00:00.000000 mazemastery-0.1.0/src/mazemastery/sprites/cloud_sw.png
+-rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 mazemastery-0.1.0/src/mazemastery/sprites/cloud_sw_inner_corner.png
+-rw-r--r--   0        0        0     4933 2020-02-02 00:00:00.000000 mazemastery-0.1.0/src/mazemastery/sprites/cloud_sw_inner_corner_s.png
+-rw-r--r--   0        0        0     4966 2020-02-02 00:00:00.000000 mazemastery-0.1.0/src/mazemastery/sprites/cloud_sw_inner_corner_w.png
+-rw-r--r--   0        0        0     5005 2020-02-02 00:00:00.000000 mazemastery-0.1.0/src/mazemastery/sprites/cloud_sw_spec.png
+-rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 mazemastery-0.1.0/src/mazemastery/sprites/cloud_w.png
+-rw-r--r--   0        0        0     7759 2020-02-02 00:00:00.000000 mazemastery-0.1.0/src/mazemastery/sprites/minotaur.png
+-rw-r--r--   0        0        0    11075 2020-02-02 00:00:00.000000 mazemastery-0.1.0/src/mazemastery/sprites/warrior_down.png
+-rw-r--r--   0        0        0    11600 2020-02-02 00:00:00.000000 mazemastery-0.1.0/src/mazemastery/sprites/warrior_left.png
+-rw-r--r--   0        0        0    11852 2020-02-02 00:00:00.000000 mazemastery-0.1.0/src/mazemastery/sprites/warrior_right.png
+-rw-r--r--   0        0        0    10990 2020-02-02 00:00:00.000000 mazemastery-0.1.0/src/mazemastery/sprites/warrior_up.png
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 mazemastery-0.1.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 mazemastery-0.1.0/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mazemastery-0.1.0/README.md
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 mazemastery-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 mazemastery-0.1.0/PKG-INFO
```

### Comparing `mazemastery-0.0.4/src/mazemastery/api.py` & `mazemastery-0.1.0/src/mazemastery/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
 
 def set_pos(new_pos):
     state = State()
     if state.dead:
         return
     if new_pos not in state.maze[state.pos]:
-
         # We don't subtract a life on level 1
         if state.level != 1:
             state.lives -= 1
         new_pos = state.pos
     old_pos = state.pos
     state.pos = new_pos
     if state.lives == 0:
@@ -62,44 +61,39 @@
 
 
 def has_minotaur(cell):
     state = State()
     return cell == state.minotaur_coords
 
 
-def found_minotaur():
+def stop():
     state = State()
     state.found = True
 
 
-def was_found():
+def is_searching():
     state = State()
-    return state.found
+    return not state.found
+
 
 def is_neighbor(pos, neighbor):
     state = State()
     return neighbor in state.maze[pos]
 
-def push(pos):
-    state = State()
-    state.stack.append(pos)
-
-def pop():
-    state = State()
-    popped = state.stack.pop()
-    return popped
 
 def are_neighbors(pos1, pos2):
     state = State()
     return pos2 in state.maze[pos1]
 
+
 def get_neighbors(pos):
     state = State()
     return state.maze[pos]
 
+
 def run(level, solve, rows=10, cols=10, cell_size=50, delay=1000, seed=None):
     random.seed(seed)
     if level == 1:
         maze = create_corridor(cols)
         minotaur_coords = (0, cols - 1)
     elif level == 2:
         maze = create_corridor(cols)
```

### Comparing `mazemastery-0.0.4/src/mazemastery/debug_menu.py` & `mazemastery-0.1.0/src/mazemastery/debug_menu.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,33 +14,31 @@
                 command=self.handle_put_red_gem_button,
             ),
             "put_blue_gem": tk.Button(
                 renderer.root,
                 text="put_blue_gem(pos)",
                 command=self.handle_put_blue_gem_button,
             ),
-            "push": tk.Button(renderer.root, text="push(pos)"),
-            "pop": tk.Button(renderer.root, text="pop()"),
-            "found_minotaur": tk.Button(renderer.root, text="found_minotaur()"),
+            "found_minotaur": tk.Button(renderer.root, text="stop()"),
         }
 
         # These buttons are used to navigate the maze in debug mode
         self.nav_buttons = {
             "up": tk.Button(renderer.root, text="↑", command=lambda: self.handle_nav_button((-1, 0))),
             "left": tk.Button(renderer.root, text="←", command=lambda: self.handle_nav_button((0, -1))),
             "right": tk.Button(renderer.root, text="→", command=lambda: self.handle_nav_button((0, 1))),
             "down": tk.Button(renderer.root, text="↓", command=lambda: self.handle_nav_button((1, 0))),
-            "info": tk.Button(renderer.root, text="move", state=tk.DISABLED),
+            "info": tk.Button(renderer.root, text="set_pos", state=tk.DISABLED),
         }
 
         # These labels are used to display the current state of the maze
         self.state_labels = {
             "has_red_gem": tk.Label(renderer.root, text="has_red_gem(pos)"),
             "has_blue_gem": tk.Label(renderer.root, text="has_blue_gem(pos)"),
-            "was_found": tk.Label(renderer.root, text="was_found()"),
+            "was_found": tk.Label(renderer.root, text="is_searching()"),
         }
         self.max_button_width = max(
             [len(button["text"]) for button in self.api_buttons.values()]
             + [len(label["text"]) for label in self.state_labels.values()]
         )
 
         # Pressing this button transfers the user into debug mode.
```

### Comparing `mazemastery-0.0.4/src/mazemastery/maze.py` & `mazemastery-0.1.0/src/mazemastery/maze.py`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.4/src/mazemastery/renderer.py` & `mazemastery-0.1.0/src/mazemastery/renderer.py`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.4/src/mazemastery/state.py` & `mazemastery-0.1.0/src/mazemastery/state.py`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.4/src/mazemastery/styles.py` & `mazemastery-0.1.0/src/mazemastery/styles.py`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.4/src/mazemastery/sprites/cloud_e.png` & `mazemastery-0.1.0/src/mazemastery/sprites/cloud_e.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.4/src/mazemastery/sprites/cloud_n.png` & `mazemastery-0.1.0/src/mazemastery/sprites/cloud_n.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.4/src/mazemastery/sprites/cloud_ne.png` & `mazemastery-0.1.0/src/mazemastery/sprites/cloud_ne.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.4/src/mazemastery/sprites/cloud_ne_inner_corner.png` & `mazemastery-0.1.0/src/mazemastery/sprites/cloud_ne_inner_corner.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.4/src/mazemastery/sprites/cloud_ne_inner_corner_e.png` & `mazemastery-0.1.0/src/mazemastery/sprites/cloud_ne_inner_corner_e.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.4/src/mazemastery/sprites/cloud_ne_inner_corner_n.png` & `mazemastery-0.1.0/src/mazemastery/sprites/cloud_ne_inner_corner_n.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.4/src/mazemastery/sprites/cloud_nw.png` & `mazemastery-0.1.0/src/mazemastery/sprites/cloud_nw.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.4/src/mazemastery/sprites/cloud_nw_inner_corner.png` & `mazemastery-0.1.0/src/mazemastery/sprites/cloud_nw_inner_corner.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.4/src/mazemastery/sprites/cloud_nw_inner_corner_e.png` & `mazemastery-0.1.0/src/mazemastery/sprites/cloud_nw_inner_corner_e.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.4/src/mazemastery/sprites/cloud_nw_inner_corner_n.png` & `mazemastery-0.1.0/src/mazemastery/sprites/cloud_nw_inner_corner_n.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.4/src/mazemastery/sprites/cloud_nw_inner_corner_w.png` & `mazemastery-0.1.0/src/mazemastery/sprites/cloud_nw_inner_corner_w.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.4/src/mazemastery/sprites/cloud_s.png` & `mazemastery-0.1.0/src/mazemastery/sprites/cloud_s.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.4/src/mazemastery/sprites/cloud_s_seam.png` & `mazemastery-0.1.0/src/mazemastery/sprites/cloud_s_seam.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.4/src/mazemastery/sprites/cloud_se.png` & `mazemastery-0.1.0/src/mazemastery/sprites/cloud_se.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.4/src/mazemastery/sprites/cloud_se_inner_corner.png` & `mazemastery-0.1.0/src/mazemastery/sprites/cloud_se_inner_corner.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.4/src/mazemastery/sprites/cloud_se_inner_corner_e.png` & `mazemastery-0.1.0/src/mazemastery/sprites/cloud_se_inner_corner_e.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.4/src/mazemastery/sprites/cloud_se_inner_corner_s.png` & `mazemastery-0.1.0/src/mazemastery/sprites/cloud_se_inner_corner_s.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.4/src/mazemastery/sprites/cloud_se_spec.png` & `mazemastery-0.1.0/src/mazemastery/sprites/cloud_se_spec.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.4/src/mazemastery/sprites/cloud_sw.png` & `mazemastery-0.1.0/src/mazemastery/sprites/cloud_sw.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.4/src/mazemastery/sprites/cloud_sw_inner_corner.png` & `mazemastery-0.1.0/src/mazemastery/sprites/cloud_sw_inner_corner.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.4/src/mazemastery/sprites/cloud_sw_inner_corner_s.png` & `mazemastery-0.1.0/src/mazemastery/sprites/cloud_sw_inner_corner_s.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.4/src/mazemastery/sprites/cloud_sw_inner_corner_w.png` & `mazemastery-0.1.0/src/mazemastery/sprites/cloud_sw_inner_corner_w.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.4/src/mazemastery/sprites/cloud_sw_spec.png` & `mazemastery-0.1.0/src/mazemastery/sprites/cloud_sw_spec.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.4/src/mazemastery/sprites/cloud_w.png` & `mazemastery-0.1.0/src/mazemastery/sprites/cloud_w.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.4/src/mazemastery/sprites/minotaur.png` & `mazemastery-0.1.0/src/mazemastery/sprites/minotaur.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.4/src/mazemastery/sprites/warrior_down.png` & `mazemastery-0.1.0/src/mazemastery/sprites/warrior_down.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.4/src/mazemastery/sprites/warrior_left.png` & `mazemastery-0.1.0/src/mazemastery/sprites/warrior_left.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.4/src/mazemastery/sprites/warrior_right.png` & `mazemastery-0.1.0/src/mazemastery/sprites/warrior_right.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.4/src/mazemastery/sprites/warrior_up.png` & `mazemastery-0.1.0/src/mazemastery/sprites/warrior_up.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.4/LICENSE` & `mazemastery-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.4/pyproject.toml` & `mazemastery-0.1.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 [build-system]
 requires= ["hatchling", "Pillow"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mazemastery"
-version = "0.0.4"
+version = "0.1.0"
 description = "MazeMastery is a Python framework for teaching maze traversal to high school students. It helps students develop abstraction skills by providing a didactic tool. They can test their algorithms against randomized test cases of increasing complexity. The framework facilitates learning analysis and conceptual challenges. MazeMastery is an open-source project for scientists and educators."
 authors = [
     {name="Raphaël Baur", email="rabaur@ethz.ch"},
     {name="Jens Hartmann", email="s4jehart@uni-trier.de"},
     {name="Jaqueline Staub", email="staub@uni-trier.de"},
-    {name="Martin Löhnertz", email="loehnert@uni-trier.de"},
 ]
 dependencies = [
     "Pillow",
 ]
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `mazemastery-0.0.4/PKG-INFO` & `mazemastery-0.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: mazemastery
-Version: 0.0.4
+Version: 0.1.0
 Summary: MazeMastery is a Python framework for teaching maze traversal to high school students. It helps students develop abstraction skills by providing a didactic tool. They can test their algorithms against randomized test cases of increasing complexity. The framework facilitates learning analysis and conceptual challenges. MazeMastery is an open-source project for scientists and educators.
 Project-URL: Homepage, https://github.com/rabaur/MazeMastery
-Author-email: Raphaël Baur <rabaur@ethz.ch>, Jens Hartmann <s4jehart@uni-trier.de>, Jaqueline Staub <staub@uni-trier.de>, Martin Löhnertz <loehnert@uni-trier.de>
+Author-email: Raphaël Baur <rabaur@ethz.ch>, Jens Hartmann <s4jehart@uni-trier.de>, Jaqueline Staub <staub@uni-trier.de>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: pillow
```

