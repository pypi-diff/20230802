# Comparing `tmp/i2cssh-0.1.3.tar.gz` & `tmp/i2cssh-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "i2cssh-0.1.3.tar", last modified: Wed Aug  2 13:41:13 2023, max compression
+gzip compressed data, was "i2cssh-0.1.4.tar", last modified: Wed Aug  2 15:56:36 2023, max compression
```

## Comparing `i2cssh-0.1.3.tar` & `i2cssh-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-02 13:41:13.444801 i2cssh-0.1.3/
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)     1057 2019-08-06 15:05:32.000000 i2cssh-0.1.3/LICENSE.txt
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)       13 2023-08-02 12:46:30.000000 i2cssh-0.1.3/MANIFEST.in
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)      711 2023-08-02 13:41:13.444156 i2cssh-0.1.3/PKG-INFO
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)    13819 2023-07-31 18:43:06.000000 i2cssh-0.1.3/README.md
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)       38 2023-08-02 13:41:13.445097 i2cssh-0.1.3/setup.cfg
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)     1067 2023-08-02 13:38:22.000000 i2cssh-0.1.3/setup.py
-drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-02 13:41:13.423007 i2cssh-0.1.3/src/
-drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-02 13:41:13.435063 i2cssh-0.1.3/src/i2cssh/
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)        0 2023-07-31 13:52:02.000000 i2cssh-0.1.3/src/i2cssh/__init__.py
--rwxr-xr-x   0 wouter.de.bie   (501) staff       (20)    24141 2023-08-02 13:00:29.000000 i2cssh-0.1.3/src/i2cssh/lib.py
--rwxr-xr-x   0 wouter.de.bie   (501) staff       (20)      132 2023-08-02 12:43:08.000000 i2cssh-0.1.3/src/i2cssh/main.py
-drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-02 13:41:13.442199 i2cssh-0.1.3/src/i2cssh/tests/
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)        0 2023-07-31 13:44:05.000000 i2cssh-0.1.3/src/i2cssh/tests/__init__.py
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)    23978 2023-08-02 09:50:11.000000 i2cssh-0.1.3/src/i2cssh/tests/test_i2cssh.py
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)       34 2023-08-02 13:39:20.000000 i2cssh-0.1.3/src/i2cssh/version.py
-drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-02 13:41:13.440528 i2cssh-0.1.3/src/i2cssh.egg-info/
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)      711 2023-08-02 13:41:13.000000 i2cssh-0.1.3/src/i2cssh.egg-info/PKG-INFO
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)      391 2023-08-02 13:41:13.000000 i2cssh-0.1.3/src/i2cssh.egg-info/SOURCES.txt
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)        1 2023-08-02 13:41:13.000000 i2cssh-0.1.3/src/i2cssh.egg-info/dependency_links.txt
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)       37 2023-08-02 13:41:13.000000 i2cssh-0.1.3/src/i2cssh.egg-info/entry_points.txt
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)       65 2023-08-02 13:41:13.000000 i2cssh-0.1.3/src/i2cssh.egg-info/requires.txt
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)        7 2023-08-02 13:41:13.000000 i2cssh-0.1.3/src/i2cssh.egg-info/top_level.txt
+drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-02 15:56:36.379549 i2cssh-0.1.4/
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)     1057 2019-08-06 15:05:32.000000 i2cssh-0.1.4/LICENSE.txt
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)       13 2023-08-02 12:46:30.000000 i2cssh-0.1.4/MANIFEST.in
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)      711 2023-08-02 15:56:36.378903 i2cssh-0.1.4/PKG-INFO
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)    13819 2023-07-31 18:43:06.000000 i2cssh-0.1.4/README.md
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)       38 2023-08-02 15:56:36.379821 i2cssh-0.1.4/setup.cfg
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)     1067 2023-08-02 13:38:22.000000 i2cssh-0.1.4/setup.py
+drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-02 15:56:36.341690 i2cssh-0.1.4/src/
+drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-02 15:56:36.355706 i2cssh-0.1.4/src/i2cssh/
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)        0 2023-07-31 13:52:02.000000 i2cssh-0.1.4/src/i2cssh/__init__.py
+-rwxr-xr-x   0 wouter.de.bie   (501) staff       (20)    24522 2023-08-02 15:54:34.000000 i2cssh-0.1.4/src/i2cssh/lib.py
+-rwxr-xr-x   0 wouter.de.bie   (501) staff       (20)      132 2023-08-02 12:43:08.000000 i2cssh-0.1.4/src/i2cssh/main.py
+drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-02 15:56:36.377318 i2cssh-0.1.4/src/i2cssh/tests/
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)        0 2023-07-31 13:44:05.000000 i2cssh-0.1.4/src/i2cssh/tests/__init__.py
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)    28775 2023-08-02 15:52:34.000000 i2cssh-0.1.4/src/i2cssh/tests/test_i2cssh.py
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)       34 2023-08-02 15:55:18.000000 i2cssh-0.1.4/src/i2cssh/version.py
+drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-02 15:56:36.371754 i2cssh-0.1.4/src/i2cssh.egg-info/
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)      711 2023-08-02 15:56:36.000000 i2cssh-0.1.4/src/i2cssh.egg-info/PKG-INFO
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)      391 2023-08-02 15:56:36.000000 i2cssh-0.1.4/src/i2cssh.egg-info/SOURCES.txt
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)        1 2023-08-02 15:56:36.000000 i2cssh-0.1.4/src/i2cssh.egg-info/dependency_links.txt
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)       37 2023-08-02 15:56:36.000000 i2cssh-0.1.4/src/i2cssh.egg-info/entry_points.txt
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)       65 2023-08-02 15:56:36.000000 i2cssh-0.1.4/src/i2cssh.egg-info/requires.txt
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)        7 2023-08-02 15:56:36.000000 i2cssh-0.1.4/src/i2cssh.egg-info/top_level.txt
```

### Comparing `i2cssh-0.1.3/LICENSE.txt` & `i2cssh-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `i2cssh-0.1.3/PKG-INFO` & `i2cssh-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i2cssh
-Version: 0.1.3
+Version: 0.1.4
 Summary: csshX like ssh tool for iTerm2
 Home-page: http://github.com/wouterdebie/i2cssh
 Author: Wouter de Bie
 Author-email: wouter@evenflow.nl
 License: MIT
 Keywords: ssh,i2cssh,csshX
 Classifier: Operating System :: MacOS
```

### Comparing `i2cssh-0.1.3/README.md` & `i2cssh-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `i2cssh-0.1.3/setup.py` & `i2cssh-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `i2cssh-0.1.3/src/i2cssh/lib.py` & `i2cssh-0.1.4/src/i2cssh/lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,16 +143,16 @@
     type=int,
     help="Number of rows (columns will be calculated)",
 )
 @optgroup.option(
     "--direction",
     "-d",
     multiple=False,
-    default="column",
-    type=click.Choice(["column", "row"], case_sensitive=False),
+    default="default",
+    type=click.Choice(["column", "row", "default"], case_sensitive=False),
     help="Direction that new sessions are created (default: column)",
 )
 @click.argument(
     "hosts_or_cluster",
     nargs=-1,
 )
 def app(hosts_or_cluster, *_args, **cmdline_opts):
@@ -226,14 +226,20 @@
                 groups.append(get_hosts([m]))
         else:
             groups.append(get_hosts(cmdline_opts.get("machines").split(",")))
 
     if filename := cmdline_opts.get("file"):
         groups.append(get_hosts(get_host_strs_from_file(filename)))
 
+    # Direction is a special case, since it has a default value in the command line options.
+    # In case it's default on the command line, we can assume wasn't set on the command line
+    # and we can delete it from the command opts alltogether. This way we can still use the
+    if cmdline_opts.get("direction") == "default":
+        cmdline_opts.pop("direction")
+
     # Each host might have additional options based on cluster config
     # or login@host syntax. We need to merge those options with the
     # global options specified in the config file and on the command line.
     #
     # Precedence is: global config < cluster config < host config < command line,
     # so we need to apply the options in that order.
 
@@ -281,14 +287,15 @@
             "geometry": compute_geometry(
                 len(hosts), hosts[0].get("rows"), hosts[0].get("columns")
             ),
             "profile": hosts[0].get("profile", "Default"),
             "shell": hosts[0].get("shell", "bash"),
             "broadcast": hosts[0].get("broadcast"),
             "nobroadcast": hosts[0].get("nobroadcast"),
+            "direction": hosts[0].get("direction"),
         }
         for hosts in groups
     ]
 
     # Execute the SSH sessions
     iterm2.run_until_complete(exec_in_iterm(groups, cmdline_opts, global_opts))
 
@@ -307,76 +314,69 @@
         # have keyboard broadcasting enabled.
         broadcast_domains = []
 
         for i, group in enumerate(groups):
             profile_name = group.get("profile")
 
             # Set the shell to be used for the session. Rather than executing this in the
-            # default shell, we add it to a LocalWriteOnlyProfile that is passed in as
+            # default shell, we add it to a LocalWriteOnlyProfile (lwop) that is then passed in as
             # profile_customizations when creating tabs and panes.
             shell = f"/usr/bin/env {group.get('shell')} -l"
             lwop = create_lwop(shell)
 
-            # if this is the first host in the group and we want sessions in a separate window,
+            # If this is the first host in the group and we want sessions in a separate window,
             # we create a new window. In any other cases we just create a new tab for the group
             if i == 0 and not (
                 cmdline_opts.get("same_window") or global_opts.get("same_window")
             ):
                 window = await create_window(connection, window, profile_name, lwop)
             else:
                 await create_tab(window, profile_name, lwop)
 
-            # Set window to fullscreen if necessary
+            # Set window to full screen if necessary
             if (
                 i == 0
                 and (cmdline_opts.get("fullscreen") or global_opts.get("fullscreen"))
                 or group["geometry"].get("requires_fullscreen")
             ):
                 await set_fullscreen(window)
 
             cols = group["geometry"]["cols"]
             rows = group["geometry"]["rows"]
 
-            if (
-                cmdline_opts.get("direction") == "column"
-                or global_opts.get("direction") == "column"
-            ):
-                vertical = True
-                horizontal = False
-            else:
+            if group.get("direction", "") == "row":
                 vertical = False
                 horizontal = True
+            else:
+                vertical = True
+                horizontal = False
 
             # List to keep track of panes that are created
             panes = []
 
             # After creating the tab, the first pane is already there
             pane = window.current_tab.current_session
             panes.append(pane)
 
             # Split vertically cols-1 times from the last pane
             # This takes care of the first row
             for col in range(1, cols):
-                pane = await pane.async_split_pane(
-                    vertical, profile_customizations=lwop, profile=profile_name
-                )
+                pane = await split_pane(profile_name, lwop, vertical, pane)
                 panes.append(pane)
 
             # For subsequent rows, we first go back to the first
             # pane of the row above, then split horizontally
             for row in range(1, rows):
                 first_col_of_last_row = col_row_to_index(0, row - 1, cols)
                 pane: Session = panes[first_col_of_last_row]
 
                 # Then for each column we split horizontally and jump
                 # to the pane in the next column on the previous row
                 for col in range(cols):
-                    new_pane = await pane.async_split_pane(
-                        horizontal, profile_customizations=lwop, profile=profile_name
-                    )
+                    new_pane = await split_pane(profile_name, lwop, horizontal, pane)
                     panes.append(new_pane)
                     next_pane = col_row_to_index(col + 1, row - 1, cols)
                     pane = panes[next_pane]
 
             # Add panes for this group to a broadcast domain, if the first host specifies
             # broadcast as an option, UNLESS nobroadcast is set as well.
             if not group.get("nobroadcast") and group.get("broadcast"):
@@ -445,14 +445,21 @@
 
         # Enable broadcast input for all groups that require it
         await enable_broadcast(connection, broadcast_domains)
 
     return inner
 
 
+async def split_pane(profile_name, lwop, vertical, pane):
+    pane = await pane.async_split_pane(
+        vertical, profile_customizations=lwop, profile=profile_name
+    )
+    return pane
+
+
 def create_lwop(shell):
     lwop = LocalWriteOnlyProfile()
     lwop.set_use_custom_command("Yes")
     lwop.set_command(f"{shell}\n")
     return lwop
```

### Comparing `i2cssh-0.1.3/src/i2cssh/tests/test_i2cssh.py` & `i2cssh-0.1.4/src/i2cssh/tests/test_i2cssh.py`

 * *Files 14% similar despite different names*

```diff
@@ -670,7 +670,155 @@
             {"rows": 5, "cols": 4, "requires_fullscreen": False},
         )
 
         self.assertEqual(
             i2cssh.lib.compute_geometry(4, 10, None),
             {"rows": 10, "cols": 1, "requires_fullscreen": False},
         )
+
+    @patch("i2cssh.lib.split_pane")
+    def test_direction_default_cli(self, mock_split_pane: MagicMock, mec: MagicMock):
+        config = {
+            "clusters": {
+                "foo": {
+                    "hosts": ["foo1", "foo2", "foo3", "foo4"],
+                }
+            },
+        }
+        invoke(["-c", "foo"], config)
+        assert_options(mec, "")
+        self.assertEqual(mock_split_pane.call_count, 3)
+        mock_split_pane.assert_has_calls(
+            [
+                call("Default", ANY, True, ANY),
+                call("Default", ANY, False, ANY),
+                call("Default", ANY, False, ANY),
+            ]
+        )
+
+    @patch("i2cssh.lib.split_pane")
+    def test_direction_row_cli(self, mock_split_pane: MagicMock, mec: MagicMock):
+        config = {
+            "clusters": {
+                "foo": {
+                    "hosts": ["foo1", "foo2", "foo3", "foo4"],
+                }
+            },
+        }
+        invoke(["-c", "foo", "-d", "row"], config)
+        assert_options(mec, "")
+        self.assertEqual(mock_split_pane.call_count, 3)
+        mock_split_pane.assert_has_calls(
+            [
+                call("Default", ANY, False, ANY),
+                call("Default", ANY, True, ANY),
+                call("Default", ANY, True, ANY),
+            ]
+        )
+
+    @patch("i2cssh.lib.split_pane")
+    def test_direction_column_cli(self, mock_split_pane: MagicMock, mec: MagicMock):
+        config = {
+            "clusters": {
+                "foo": {
+                    "hosts": ["foo1", "foo2", "foo3", "foo4"],
+                }
+            },
+        }
+        invoke(["-c", "foo", "-d", "column"], config)
+        assert_options(mec, "")
+        self.assertEqual(mock_split_pane.call_count, 3)
+        mock_split_pane.assert_has_calls(
+            [
+                call("Default", ANY, True, ANY),
+                call("Default", ANY, False, ANY),
+                call("Default", ANY, False, ANY),
+            ]
+        )
+
+    @patch("i2cssh.lib.split_pane")
+    def test_direction_row_config_global(
+        self, mock_split_pane: MagicMock, mec: MagicMock
+    ):
+        config = {
+            "direction": "row",
+            "clusters": {
+                "foo": {
+                    "hosts": ["foo1", "foo2", "foo3", "foo4"],
+                },
+            },
+        }
+        invoke(["-c", "foo"], config)
+        assert_options(mec, "")
+        self.assertEqual(mock_split_pane.call_count, 3)
+        mock_split_pane.assert_has_calls(
+            [
+                call("Default", ANY, False, ANY),
+                call("Default", ANY, True, ANY),
+                call("Default", ANY, True, ANY),
+            ]
+        )
+
+    @patch("i2cssh.lib.split_pane")
+    def test_direction_column_config_global(
+        self, mock_split_pane: MagicMock, mec: MagicMock
+    ):
+        config = {
+            "direction": "column",
+            "clusters": {
+                "foo": {
+                    "hosts": ["foo1", "foo2", "foo3", "foo4"],
+                },
+            },
+        }
+        invoke(["-c", "foo"], config)
+        assert_options(mec, "")
+        self.assertEqual(mock_split_pane.call_count, 3)
+        mock_split_pane.assert_has_calls(
+            [
+                call("Default", ANY, True, ANY),
+                call("Default", ANY, False, ANY),
+                call("Default", ANY, False, ANY),
+            ]
+        )
+
+    @patch("i2cssh.lib.split_pane")
+    def test_direction_row_config(self, mock_split_pane: MagicMock, mec: MagicMock):
+        config = {
+            "clusters": {
+                "foo": {
+                    "direction": "row",
+                    "hosts": ["foo1", "foo2", "foo3", "foo4"],
+                },
+            },
+        }
+        invoke(["-c", "foo"], config)
+        assert_options(mec, "")
+        self.assertEqual(mock_split_pane.call_count, 3)
+        mock_split_pane.assert_has_calls(
+            [
+                call("Default", ANY, False, ANY),
+                call("Default", ANY, True, ANY),
+                call("Default", ANY, True, ANY),
+            ]
+        )
+
+    @patch("i2cssh.lib.split_pane")
+    def test_direction_column_config(self, mock_split_pane: MagicMock, mec: MagicMock):
+        config = {
+            "clusters": {
+                "foo": {
+                    "direction": "column",
+                    "hosts": ["foo1", "foo2", "foo3", "foo4"],
+                },
+            },
+        }
+        invoke(["-c", "foo"], config)
+        assert_options(mec, "")
+        self.assertEqual(mock_split_pane.call_count, 3)
+        mock_split_pane.assert_has_calls(
+            [
+                call("Default", ANY, True, ANY),
+                call("Default", ANY, False, ANY),
+                call("Default", ANY, False, ANY),
+            ]
+        )
```

### Comparing `i2cssh-0.1.3/src/i2cssh.egg-info/PKG-INFO` & `i2cssh-0.1.4/src/i2cssh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i2cssh
-Version: 0.1.3
+Version: 0.1.4
 Summary: csshX like ssh tool for iTerm2
 Home-page: http://github.com/wouterdebie/i2cssh
 Author: Wouter de Bie
 Author-email: wouter@evenflow.nl
 License: MIT
 Keywords: ssh,i2cssh,csshX
 Classifier: Operating System :: MacOS
```

