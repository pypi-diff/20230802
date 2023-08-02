# Comparing `tmp/i2cssh-0.0.9.tar.gz` & `tmp/i2cssh-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "i2cssh-0.0.9.tar", last modified: Thu Nov 17 18:22:49 2022, max compression
+gzip compressed data, was "i2cssh-0.1.0.tar", last modified: Wed Aug  2 12:27:12 2023, max compression
```

## Comparing `i2cssh-0.0.9.tar` & `i2cssh-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,22 @@
-drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2022-11-17 18:22:49.452806 i2cssh-0.0.9/
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)     1057 2019-08-06 15:05:32.000000 i2cssh-0.0.9/LICENSE.txt
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)      711 2022-11-17 18:22:49.452419 i2cssh-0.0.9/PKG-INFO
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)    11780 2022-11-17 18:22:11.000000 i2cssh-0.0.9/README.md
--rwxr-xr-x   0 wouter.de.bie   (501) staff       (20)    18722 2022-11-17 18:17:57.000000 i2cssh-0.0.9/i2cssh
-drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2022-11-17 18:22:49.451600 i2cssh-0.0.9/i2cssh.egg-info/
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)      711 2022-11-17 18:22:49.000000 i2cssh-0.0.9/i2cssh.egg-info/PKG-INFO
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)      197 2022-11-17 18:22:49.000000 i2cssh-0.0.9/i2cssh.egg-info/SOURCES.txt
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)        1 2022-11-17 18:22:49.000000 i2cssh-0.0.9/i2cssh.egg-info/dependency_links.txt
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)       63 2022-11-17 18:22:49.000000 i2cssh-0.0.9/i2cssh.egg-info/requires.txt
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)        7 2022-11-17 18:22:49.000000 i2cssh-0.0.9/i2cssh.egg-info/top_level.txt
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)       38 2022-11-17 18:22:49.453184 i2cssh-0.0.9/setup.cfg
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)     1019 2022-11-16 19:36:17.000000 i2cssh-0.0.9/setup.py
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)       34 2022-11-17 18:18:35.000000 i2cssh-0.0.9/version.py
+drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-02 12:27:12.493567 i2cssh-0.1.0/
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)     1057 2019-08-06 15:05:32.000000 i2cssh-0.1.0/LICENSE.txt
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)       32 2023-08-02 09:52:37.000000 i2cssh-0.1.0/MANIFEST.in
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)      711 2023-08-02 12:27:12.493083 i2cssh-0.1.0/PKG-INFO
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)    13819 2023-07-31 18:43:06.000000 i2cssh-0.1.0/README.md
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)       38 2023-08-02 12:27:12.493767 i2cssh-0.1.0/setup.cfg
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)     1024 2023-08-02 08:54:25.000000 i2cssh-0.1.0/setup.py
+drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-02 12:27:12.475193 i2cssh-0.1.0/src/
+drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-02 12:27:12.484842 i2cssh-0.1.0/src/i2cssh/
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)        0 2023-07-31 13:52:02.000000 i2cssh-0.1.0/src/i2cssh/__init__.py
+-rwxr-xr-x   0 wouter.de.bie   (501) staff       (20)    24134 2023-08-02 09:36:27.000000 i2cssh-0.1.0/src/i2cssh/lib.py
+-rwxr-xr-x   0 wouter.de.bie   (501) staff       (20)      125 2023-07-31 14:19:43.000000 i2cssh-0.1.0/src/i2cssh/main.py
+drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-02 12:27:12.491386 i2cssh-0.1.0/src/i2cssh/tests/
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)        0 2023-07-31 13:44:05.000000 i2cssh-0.1.0/src/i2cssh/tests/__init__.py
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)    23978 2023-08-02 09:50:11.000000 i2cssh-0.1.0/src/i2cssh/tests/test_i2cssh.py
+drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-02 12:27:12.489809 i2cssh-0.1.0/src/i2cssh.egg-info/
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)      711 2023-08-02 12:27:12.000000 i2cssh-0.1.0/src/i2cssh.egg-info/PKG-INFO
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)      343 2023-08-02 12:27:12.000000 i2cssh-0.1.0/src/i2cssh.egg-info/SOURCES.txt
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)        1 2023-08-02 12:27:12.000000 i2cssh-0.1.0/src/i2cssh.egg-info/dependency_links.txt
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)       65 2023-08-02 12:27:12.000000 i2cssh-0.1.0/src/i2cssh.egg-info/requires.txt
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)       11 2023-08-02 12:27:12.000000 i2cssh-0.1.0/src/i2cssh.egg-info/top_level.txt
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)       34 2023-08-02 09:53:53.000000 i2cssh-0.1.0/version.py
```

### Comparing `i2cssh-0.0.9/LICENSE.txt` & `i2cssh-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `i2cssh-0.0.9/PKG-INFO` & `i2cssh-0.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i2cssh
-Version: 0.0.9
+Version: 0.1.0
 Summary: csshX like ssh tool for iTerm2
 Home-page: http://github.com/wouterdebie/i2cssh
 Author: Wouter de Bie
 Author-email: wouter@evenflow.nl
 License: MIT
 Keywords: ssh,i2cssh,csshX
 Classifier: Operating System :: MacOS
```

### Comparing `i2cssh-0.0.9/README.md` & `i2cssh-0.1.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -54,14 +54,17 @@
                                       need to start with LC_)
         -r, --rank                    Send LC_RANK with the host number as
                                       environment variable
         -X, --extra TEXT              Additional ssh parameters (e.g.
                                       -Xi=myidentity.pem)
         -g, --gateway TEXT            Multihop SSH connection gateway string (e.g.
                                       username@gateway) - usually used with -A
+        -x, --custom-command TEXT     Custom command to run instead of SSH. Use
+                                      "{host}" to for host substitution (e.g.
+                                      "kubectl exec -it {host} -- /bin/bash")
     iTerm2 options:
         -F, --fullscreen              Make the window fullscreen
         -b, --broadcast               Start with broadcast input (DANGEROUS!)
         -nb, --nobroadcast            Disable broadcast input
         -p, --profile TEXT            iTerm2 profile name (default: Default)
         -s, --sleep INTEGER           Number of seconds to sleep between creating
                                       SSH sessions
@@ -119,48 +122,75 @@
 columns: <cols> # Amount of columns
 rows: <rows> # Amount of rows
 sleep: <secs> # Seconds to sleep between creating SSH sessions
 direction: (column/row) # Direction that new sessions are created (default: column)
 shell: <shell> # Shell to use (default: /bin/bash)
 
 environment: # Send the following enviroment variables
-  - LC_FOO: foo
-  - LC_BAR: bar
+  LC_FOO: foo
+  LC_BAR: bar
+
+extra:
+  i: myidentity.pem
+  p: 2222
 ```
 
 Note: rows and columns can't be used at the same time.
 
+Clusters can also include hosts from other clusters through a cluster specific optional parameter `include_from`:
+
+```yaml
+version: 2
+clusters:
+  cluster1:
+    hosts:
+      - host1
+      - host2
+  cluster2:
+    hosts:
+      - host3
+      - host4
+    include_from:
+      - cluster1
+```
+
+Note that only the hosts will be included, but no additional configuration options. Secondly, includes
+aren't transitive, so if `cluster1` includes `cluster2`, which in turn includes `cluster3`, only the
+hosts from `cluster2` will be included in `cluster1`.
+
 The following precedence is used:
 
 `global options from config` < `cluster options from config` < `command line flags`
 
 Make sure the config file is valid YAML (e.g. use spaces instead of tabs)
 
 ## Options
 
-| Option                        | Description                                                                                                                                                                                                                     |
-| ----------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| `-A, --forward-agent`         | Enable SSH agent forwarding                                                                                                                                                                                                     |
-| `-l, --login LOGIN`           | This option will override all logins passed in to i2cssh. This goes for global config, cluster config or username@host passed on the command line                                                                               |
-| `-e, --environment KEY=VAL`   | Allows for passing environment varables to the SSH session. This can be a comma-separated list: `-e LC_FOO=foo,LC_BAR=bar`                                                                                                      |
-| `-F, --fullscreen`            | Enable fullscreen on startup                                                                                                                                                                                                    |
-| `-C, --columns COLUMNS `      | Set the amount of columns. Can't be used in conjunction with -R                                                                                                                                                                 |
-| `-R, --rows ROWS `            | Set the amount of columns. Can't be used in conjunction with -C                                                                                                                                                                 |
-| `-b, --broadcast `            | Enable broadcast on startup. i2cssh will send cmd-shift-i to the window and press the OK button.                                                                                                                                |
-| `-nb, --nobroadcast `         | Disable broadcast. This setting can be used to disable any broadcast that was set in the config.                                                                                                                                |
-| `-p, --profile PROFILE`       | Use a specific iTerm profile.                                                                                                                                                                                                   |
-| `-f, --file FILE `            | Will read nodes from a file. These will be added to any hosts specified on the command line or in the config.                                                                                                                   |
-| `-c, --clusters clus1,clus2 ` | Connect to one or more clusters that are specified in the config                                                                                                                                                                |
-| `-r, --rank `                 | Send a LC_RANK environment variable different for each host (from 0 to n)                                                                                                                                                       |
-| `-m, --machines a,b,c `       | Connect to the machines a, b and c                                                                                                                                                                                              |
-| `-t, --tab-split `            | Split servers/clusters into tabs, grouping arguments. Tabs are created as follows: hosts after a -m option are put in one tab, each cluster is always in its own tab, all the arguments are in one tab.                         |
-| `-T, --tab-split-nogroup `    | Split servers/clusters into tabs, _not_ grouping arguments. Tabs are created as follows: hosts after a -m option are put in one tab, each cluster is always in its own tab, each argument is in its own tab.                    |
-| `-W, --same-window `          | Do not create new Window, but spawn new cluster tabs in current (last used) iterm window                                                                                                                                        |
-| `-s, --sleep SLEEP `          | Wait SLEEP seconds between starting each ssh session. This will take decimals as well (0.5 for half a second)                                                                                                                   |
-| `-X, --extra EXTRA `          | Set extra ssh parameters in the form `-Xk=v`. For example: `i2cssh -Xi=myidentity.pem` will result in `ssh -i myidentity.pem`, or `i2cssh -Xp=2222 -XL=8080:localhost:8080` will result in `ssh -p 2222 -L 8080:localhost:8080` |
+| Option                                    | Description                                                                                                                                                                                                                                         |
+| ----------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| <nobr>`-A, --forward-agent`</nobr>        | Enable SSH agent forwarding                                                                                                                                                                                                                         |
+| <nobr>`-l, --login LOGIN`</nobr>          | This option will override all logins passed in to i2cssh. This goes for global config, cluster config or username@host passed on the command line.                                                                                                  |
+| <nobr>`-e, --environment KEY=VAL`</nobr>  | Allows for passing environment varables to the SSH session. This can be a comma-separated list: `-e LC_FOO=foo,LC_BAR=bar`                                                                                                                          |
+| <nobr>`-F, --fullscreen`</nobr>           | Enable fullscreen on startup.                                                                                                                                                                                                                       |
+| <nobr>`-C, --columns COLUMNS`</nobr>      | Set the amount of columns. Can't be used in conjunction with `-R`.                                                                                                                                                                                  |
+| <nobr>`-R, --rows ROWS`</nobr>            | Set the amount of columns. Can't be used in conjunction with `-C`.                                                                                                                                                                                  |
+| <nobr>`-b, --broadcast`</nobr>            | Enable broadcast on startup.                                                                                                                                                                                                                        |
+| <nobr>`-nb, --nobroadcast`</nobr>         | Disable broadcast. This setting can be used to disable any broadcast that was set in the config.                                                                                                                                                    |
+| <nobr>`-p, --profile PROFILE`</nobr>      | Use a specific iTerm profile.                                                                                                                                                                                                                       |
+| <nobr>`-f, --file FILE`</nobr>            | Will read nodes from a file. These will be added to any hosts specified on the command line or in the config.                                                                                                                                       |
+| <nobr>`-c, --clusters clus1,clus2`</nobr> | Connect to one or more clusters that are specified in the config.                                                                                                                                                                                   |
+| <nobr>`-r, --rank`</nobr>                 | Send a LC_RANK environment variable different for each host (from 0 to n).                                                                                                                                                                          |
+| <nobr>`-m, --machines a,b,c`</nobr>       | Connect to the machines a, b and c                                                                                                                                                                                                                  |
+| <nobr>`-t, --tab-split`</nobr>            | Split servers/clusters into tabs, grouping arguments. Tabs are created as follows: hosts after a -m option are put in one tab, each cluster is always in its own tab, all the arguments are in one tab.                                             |
+| <nobr>`-T, --tab-split-nogroup`</nobr>    | Split servers/clusters into tabs, _not_ grouping arguments. Tabs are created as follows: hosts after a -m option are put in one tab, each cluster is always in its own tab, each argument is in its own tab.                                        |
+| <nobr>`-W, --same-window`</nobr>          | Do not create new Window, but spawn new cluster tabs in current (last used) iterm window.                                                                                                                                                           |
+| <nobr>`-s, --sleep SLEEP`</nobr>          | Wait SLEEP seconds between starting each ssh session. This will take decimals as well (0.5 for half a second)                                                                                                                                       |
+| <nobr>`-E, --exec`</nobr>                 | Run ssh using exec, rather than just the command in the shell. This causes the pane to close when ssh exits. Note that any errors or logs will disappear.                                                                                           |
+| <nobr>`-X, --extra EXTRA`</nobr>          | Set extra ssh parameters in the form `-Xk=v` <br><br>E.g: `i2cssh -Xi=myidentity.pem` will result in `ssh -i myidentity.pem`, or `i2cssh -Xp=2222 -XL=8080:localhost:8080` will result in `ssh -p 2222 -L 8080:localhost:8080`                      |
+| <nobr>`-x, --custom-command`</nobr>       | Use a custom command to connect to the hosts. This will override the default `ssh` command. Use `{host}` as a substitution for the actual host will be used. E.g. `-x "kubectl exec -it {host} -- /bin/bash"` to execute `kubectl` instead of `ssh` |
 
 ## TODO
 
 - Better release process (homebrew update after new release)
 - Proper handling of resizing and full screen when the window is too small for the amount of rows or columns.
 
 ## Contributing to i2cssh
```

### Comparing `i2cssh-0.0.9/i2cssh` & `i2cssh-0.1.0/src/i2cssh/lib.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,195 +1,349 @@
-#!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 import asyncio
+import copy
 import math
 import os
+import re
 import sys
 
 import click
 import iterm2
 import yaml
 from click_option_group import MutuallyExclusiveOptionGroup, optgroup
 from iterm2 import Session
 from iterm2.color import Color
 from iterm2.profile import LocalWriteOnlyProfile
 
 from version import version
 
 
 @click.command()
-@optgroup.group('General options')
-@optgroup.option('--clusters', '-c', 'cli_clusters', multiple=False, help='Comma-separated list of clusters specified in ~/.i2csshrc')
-@optgroup.option('--machines', '-m', multiple=False, help='Comma-separated list of hosts')
-@optgroup.option('--file', '-f', multiple=False, help='Cluster file (one hostname per line)')
-@optgroup.option('--tab-split', '-t', is_flag=True, default=False, help="Split servers/clusters into tabs and put all hosts specified on the command line in one tab")
-@optgroup.option('--tab-split-nogroup', '-T', is_flag=True, default=False, help="Split servers/clusters into tabs and put each host specified on the command line in a separate tab")
-@optgroup.option('--same-window', '-W', is_flag=True, default=False, help="Use existing window for spawning new tabs")
-@optgroup.option('--version', '-v', is_flag=True, default=False, help="Show version")
-@optgroup.group('SSH options')
-@optgroup.option('--forward-agent', '-A', multiple=False, is_flag=True, help='Enable SSH agent forwarding')
-@optgroup.option('--login', '-l', multiple=False, help='SSH user name')
-@optgroup.option('--environment', '-e', multiple=False, help='Send environment vars (comma-separated list, need to start with LC_)')
-@optgroup.option('--rank', '-r', is_flag=True, help='Send LC_RANK with the host number as environment variable')
-@optgroup.option('--extra', '-X', multiple=True, help='Additional ssh parameters (e.g. -Xi=myidentity.pem)')
-@optgroup.option('--gateway', '-g', multiple=False, help='Multihop SSH connection gateway string (e.g. username@gateway) - usually used with -A')
-@optgroup.group('iTerm2 options')
-@optgroup.option('--fullscreen', '-F', is_flag=True, help='Make the window fullscreen')
-@optgroup.option('--broadcast', '-b', is_flag=True, default=False, help='Start with broadcast input (DANGEROUS!)')
-@optgroup.option('--nobroadcast', '-nb', is_flag=True, default=False, help='Disable broadcast input')
-@optgroup.option('--profile', '-p', multiple=False, help='iTerm2 profile name (default: Default)')
-@optgroup.option('--sleep', '-s', multiple=False, type=int, help='Number of seconds to sleep between creating SSH sessions')
-@optgroup.option('--shell', '-S', multiple=False, help='Shell to use when spawning the SSH sessions (default: bash)')
-@optgroup.option('--direction', '-d', multiple=False, default="column", type=click.Choice(['column', 'row'], case_sensitive=False), help='Direction that new sessions are created (default: column)')
+@optgroup.group("General options")
+@optgroup.option(
+    "--clusters",
+    "-c",
+    "cli_clusters",
+    multiple=False,
+    help="Comma-separated list of clusters specified in ~/.i2csshrc",
+)
+@optgroup.option(
+    "--machines", "-m", multiple=False, help="Comma-separated list of hosts"
+)
+@optgroup.option(
+    "--file", "-f", multiple=False, help="Cluster file (one hostname per line)"
+)
+@optgroup.option(
+    "--tab-split",
+    "-t",
+    is_flag=True,
+    default=False,
+    help="Split servers/clusters into tabs and put all hosts specified on the command line in one tab",
+)
+@optgroup.option(
+    "--tab-split-nogroup",
+    "-T",
+    is_flag=True,
+    default=False,
+    help="Split servers/clusters into tabs and put each host specified on the command line in a separate tab",
+)
+@optgroup.option(
+    "--same-window",
+    "-W",
+    is_flag=True,
+    default=False,
+    help="Use existing window for spawning new tabs",
+)
+@optgroup.option("--version", "-v", is_flag=True, default=False, help="Show version")
+@optgroup.group("SSH options")
+@optgroup.option(
+    "--forward-agent",
+    "-A",
+    multiple=False,
+    is_flag=True,
+    help="Enable SSH agent forwarding",
+)
+@optgroup.option("--login", "-l", multiple=False, help="SSH user name")
+@optgroup.option(
+    "--environment",
+    "-e",
+    multiple=False,
+    help="Send environment vars (comma-separated list, need to start with LC_)",
+)
+@optgroup.option(
+    "--rank",
+    "-r",
+    is_flag=True,
+    help="Send LC_RANK with the host number as environment variable",
+)
+@optgroup.option(
+    "--extra",
+    "-X",
+    multiple=True,
+    help="Additional ssh parameters (e.g. -Xi=myidentity.pem)",
+)
+@optgroup.option(
+    "--gateway",
+    "-g",
+    multiple=False,
+    help="Multihop SSH connection gateway string (e.g. username@gateway) - usually used with -A",
+)
+@optgroup.option(
+    "--custom-command",
+    "-x",
+    multiple=False,
+    help='Custom command to run instead of SSH. Use "{host}" to for host substitution (e.g. "kubectl exec -it {host} -- /bin/bash")',
+)
+@optgroup.group("iTerm2 options")
+@optgroup.option("--fullscreen", "-F", is_flag=True, help="Make the window fullscreen")
+@optgroup.option(
+    "--broadcast",
+    "-b",
+    is_flag=True,
+    default=False,
+    help="Start with broadcast input (DANGEROUS!)",
+)
+@optgroup.option(
+    "--nobroadcast", "-nb", is_flag=True, default=False, help="Disable broadcast input"
+)
+@optgroup.option(
+    "--profile", "-p", multiple=False, help="iTerm2 profile name (default: Default)"
+)
+@optgroup.option(
+    "--sleep",
+    "-s",
+    multiple=False,
+    type=int,
+    help="Number of seconds to sleep between creating SSH sessions",
+)
+@optgroup.option(
+    "--shell",
+    "-S",
+    multiple=False,
+    help="Shell to use when spawning the SSH sessions (default: bash)",
+)
+@optgroup.option(
+    "--exec",
+    "-E",
+    is_flag=True,
+    default=False,
+    help="Use exec when spawning ssh. This will close the pane when ssh exits",
+)
 @optgroup.group("Layout", cls=MutuallyExclusiveOptionGroup)
-@optgroup.option('--columns', '-C', multiple=False, type=int, help='Number of columns (rows will be calculated)')
-@optgroup.option('--rows', '-R', multiple=False, type=int, help='Number of rows (columns will be calculated)')
-@click.argument('hosts_or_cluster', nargs=-1, )
-def i2cssh(hosts_or_cluster, *_args, **opts):
+@optgroup.option(
+    "--columns",
+    "-C",
+    multiple=False,
+    type=int,
+    help="Number of columns (rows will be calculated)",
+)
+@optgroup.option(
+    "--rows",
+    "-R",
+    multiple=False,
+    type=int,
+    help="Number of rows (columns will be calculated)",
+)
+@optgroup.option(
+    "--direction",
+    "-d",
+    multiple=False,
+    default="column",
+    type=click.Choice(["column", "row"], case_sensitive=False),
+    help="Direction that new sessions are created (default: column)",
+)
+@click.argument(
+    "hosts_or_cluster",
+    nargs=-1,
+)
+def app(hosts_or_cluster, *_args, **cmdline_opts):
     """HOSTS: [(login@host [login@host] | login@cluster)]"""
 
-    sanitize_options(opts)
+    sanitize_options(cmdline_opts)
 
-    if opts.get("version"):
+    if cmdline_opts.get("version"):
         print(version())
         sys.exit(0)
 
     # Keep track of valid command line options so we can filter out
     # additional options in the config file
-    valid_options = list(opts.keys())
+    valid_options = list(cmdline_opts.keys())
 
-    # Load config file and get valid options
+    # Load config file and get valid options. Since command line options take precedence, we
+    # override the config file options with the command line options.
     config = read_config()
     if config:
-        global_options_from_config = filter_valid_options(config, valid_options)
+        global_opts = filter_valid_options(config, valid_options)
+        # apply_opts(global_options_from_config, opts, valid_options)
+        # opts = global_options_from_config
 
     # Because we can split tabs based on cluster/hosts/arguments we first
     # create different groups inside the hosts list. If it turns out we
     # don't need to split tabs, we'll just have one group by flattening
     # the list.
 
-    # List where we eventually store the groups of hosts. Hosts will be
-    # dictionaries with all the options necessary to spawn the SSH session
+    # List where we initially store the groups of hosts. Later we'll use these to apply options from
+    # different configuration places (cluster, global, command line), creating config_groups.
+    # Hosts are dictionaries with all the options necessary to spawn the SSH session
     groups = []
 
     # If there's only one argument, we assume it's a cluster name (since there's
     # no need to use i2cssh for a single host) and we get hosts from the cluster
     # configuration. Otherwise we construct a list of hosts from the arguments.
     if len(hosts_or_cluster) == 1:
         # Single cluster, so we know there's only one list returned
         groups = get_clusters_from_cluster_names(
-            [hosts_or_cluster[0]], config, valid_options)
+            [hosts_or_cluster[0]], config, valid_options
+        )
     # More than one argument, so we assume it's a list of hosts
     elif len(hosts_or_cluster) > 1:
         hosts = get_hosts(hosts_or_cluster)
         # If tab_split is defined, hosts get separate tabs, otherwise we put all
         # hosts defined as arguments in one group
-        if opts.get("tab_split"):
+        if cmdline_opts.get("tab_split") or global_opts.get("tab_split"):
             groups.append(hosts)
         else:
             for hosts in hosts:
                 groups.append([hosts])
 
     # The command line option '-c' can also provide clusters, so we need to get the hosts
     # from those clusters as well.
-    if opts.get("cli_clusters"):
+    if cmdline_opts.get("cli_clusters"):
         clusters = get_clusters_from_cluster_names(
-            opts.get("cli_clusters").split(","), config, valid_options)
+            cmdline_opts.get("cli_clusters").split(","), config, valid_options
+        )
         for cluster in clusters:
             groups.append(cluster)
 
     # The command line option '-m' can also provide hosts, so we need to get the hosts
     # from those host strings as well
-    if opts.get("machines"):
-        groups.append(get_hosts(opts.get("machines").split(",")))
+    if cmdline_opts.get("machines"):
+        # If tab_split_nogroup is defined, each host gets its own tab, otherwise we put all
+        # hosts defined as arguments in one group
+        if cmdline_opts.get("tab_split_nogroup") or global_opts.get(
+            "tab_split_nogroup"
+        ):
+            for m in cmdline_opts.get("machines").split(","):
+                groups.append(get_hosts([m]))
+        else:
+            groups.append(get_hosts(cmdline_opts.get("machines").split(",")))
 
-    if filename := opts.get("file"):
+    if filename := cmdline_opts.get("file"):
         groups.append(get_hosts(get_host_strs_from_file(filename)))
 
     # Each host might have additional options based on cluster config
     # or login@host syntax. We need to merge those options with the
     # global options specified in the config file and on the command line.
     #
-    # Precedence is: command line > global config > cluster config
+    # Precedence is: global config < cluster config < host config < command line,
+    # so we need to apply the options in that order.
+
     for hosts in groups:
-        if config:
-            # Apply global options from config file
-            apply_opts(hosts, global_options_from_config, valid_options)
-        # Apply options from command line
-        apply_opts(hosts, opts, valid_options)
+        for host in hosts:
+            # Save login in order to apply it later
+            login = host.get("login")
+
+            if config:
+                apply_opts(host, global_opts, valid_options)
+
+            # Apply cluster options from config file
+            cluster_options = host["cluster_options"]
+            apply_opts(host, cluster_options, valid_options)
+            host.pop("cluster_options")
+
+            # Apply login from host config we saved it
+            if login:
+                host["login"] = login
+
+            # Apply options from command line
+            apply_opts(host, cmdline_opts, valid_options)
 
     # Flatten the list if we don't need to split tabs. We create a single
     # group though, so we can still use the same code to calculate geometry
     # in both cases
-    if not (opts.get("tab_split") or opts.get("tab_split_nogroup")):
+    if not (
+        cmdline_opts.get("tab_split")
+        or cmdline_opts.get("tab_split_nogroup")
+        or global_opts.get("tab_split")
+        or global_opts.get("tab_split_nogroup")
+    ):
         groups = [flatten(groups)]
 
     # Bail if we don't have any hosts
     if len(flatten(groups)) == 0:
         click.echo("No hosts found")
         sys.exit(1)
 
     # Attach a geometry and group options to each group. Here we take options the first host, since
     # we assume that all hosts in a group have the same group options. Also, we set a few defaults.
-    groups = [{
-        "hosts": hosts,
-        "geometry": compute_geometry(len(hosts), hosts[0].get("rows"), hosts[0].get("columns")),
-        "profile": hosts[0].get("profile", "Default"),
-        "shell": hosts[0].get("shell", "bash"),
-        "broadcast": hosts[0].get("broadcast"),
-        "nobroadcast": hosts[0].get("nobroadcast"),
-    } for hosts in groups]
+    groups = [
+        {
+            "hosts": hosts,
+            "geometry": compute_geometry(
+                len(hosts), hosts[0].get("rows"), hosts[0].get("columns")
+            ),
+            "profile": hosts[0].get("profile", "Default"),
+            "shell": hosts[0].get("shell", "bash"),
+            "broadcast": hosts[0].get("broadcast"),
+            "nobroadcast": hosts[0].get("nobroadcast"),
+        }
+        for hosts in groups
+    ]
 
     # Execute the SSH sessions
-    iterm2.run_until_complete(exec_in_iterm(groups, opts))
+    iterm2.run_until_complete(exec_in_iterm(groups, cmdline_opts, global_opts))
 
-def exec_in_iterm(groups, opts):
+
+def exec_in_iterm(groups, cmdline_opts, global_opts):
     """
     Execute the SSH sessions in iTerm2
     This function takes in groups of hosts and global options and returns an
     async function that will be executed by iTerm2
     """
+
     async def inner(connection):
-        # Setup iterm API connection
-        app = await iterm2.async_get_app(connection)
-        window = app.current_window
-
-        # Bail if we're not inside iterm
-        if window is None:
-            click.echo("No current window")
-            sys.exit(1)
+        window = await get_window(connection)
 
         # Keep track of broadcast domains. This is later used to tell iTerm2 which tabs need to
         # have keyboard broadcasting enabled.
         broadcast_domains = []
 
         for i, group in enumerate(groups):
             profile_name = group.get("profile")
 
-            # Same thing for the shell
-            shell = f"/usr/bin/env {group.get('shell')} -l "
-            lwop = LocalWriteOnlyProfile()
-            lwop.set_use_custom_command("Yes")
-            lwop.set_command(f'{shell}\n')
+            # Set the shell to be used for the session. Rather than executing this in the
+            # default shell, we add it to a LocalWriteOnlyProfile that is passed in as
+            # profile_customizations when creating tabs and panes.
+            shell = f"/usr/bin/env {group.get('shell')} -l"
+            lwop = create_lwop(shell)
 
             # if this is the first host in the group and we want sessions in a separate window,
             # we create a new window. In any other cases we just create a new tab for the group
-            if i == 0 and not opts.get("same_window"):
-                window = await window.async_create(connection, profile_name, profile_customizations=lwop)
+            if i == 0 and not (
+                cmdline_opts.get("same_window") or global_opts.get("same_window")
+            ):
+                window = await create_window(connection, window, profile_name, lwop)
             else:
-                await window.async_create_tab(profile_name, profile_customizations=lwop)
+                await create_tab(window, profile_name, lwop)
 
             # Set window to fullscreen if necessary
-            if i == 0 and opts.get("fullscreen") or group["geometry"].get("requires_fullscreen"):
-                await window.async_set_fullscreen(True)
+            if (
+                i == 0
+                and (cmdline_opts.get("fullscreen") or global_opts.get("fullscreen"))
+                or group["geometry"].get("requires_fullscreen")
+            ):
+                await set_fullscreen(window)
 
             cols = group["geometry"]["cols"]
             rows = group["geometry"]["rows"]
 
-            if opts.get("direction") == "column":
+            if (
+                cmdline_opts.get("direction") == "column"
+                or global_opts.get("direction") == "column"
+            ):
                 vertical = True
                 horizontal = False
             else:
                 vertical = False
                 horizontal = True
 
             # List to keep track of panes that are created
@@ -198,82 +352,159 @@
             # After creating the tab, the first pane is already there
             pane = window.current_tab.current_session
             panes.append(pane)
 
             # Split vertically cols-1 times from the last pane
             # This takes care of the first row
             for col in range(1, cols):
-                pane = await pane.async_split_pane(vertical, profile_customizations=lwop, profile=profile_name)
+                pane = await pane.async_split_pane(
+                    vertical, profile_customizations=lwop, profile=profile_name
+                )
                 panes.append(pane)
 
             # For subsequent rows, we first go back to the first
             # pane of the row above, then split horizontally
             for row in range(1, rows):
-                first_col_of_last_row = col_row_to_index(0, row-1, cols)
+                first_col_of_last_row = col_row_to_index(0, row - 1, cols)
                 pane: Session = panes[first_col_of_last_row]
 
                 # Then for each column we split horizontally and jump
                 # to the pane in the next column on the previous row
                 for col in range(cols):
-                    new_pane = await pane.async_split_pane(horizontal, profile_customizations=lwop, profile=profile_name)
+                    new_pane = await pane.async_split_pane(
+                        horizontal, profile_customizations=lwop, profile=profile_name
+                    )
                     panes.append(new_pane)
-                    next_pane = col_row_to_index(col+1, row-1, cols)
+                    next_pane = col_row_to_index(col + 1, row - 1, cols)
                     pane = panes[next_pane]
 
             # Add panes for this group to a broadcast domain, if the first host specifies
             # broadcast as an option, UNLESS nobroadcast is set as well.
             if not group.get("nobroadcast") and group.get("broadcast"):
                 broadcast_domains.append(panes)
 
             for p, pane in enumerate(panes):
                 # There might be more panes than hosts
                 if p < len(group["hosts"]):
-                    env_vars = {}
-                    send_env = ""
-
-                    # Rank is just an env var, so set it if we have it
-                    if opts.get("rank"):
-                        env_vars["LC_RANK"] = str(p)
-
-                    # Split other env vars by comma and put them in a dict
-                    if from_env := opts.get("environment"):
-                        env_vars.update(dict(s.split("=")
-                                        for s in from_env.split(",")))
-
-                    # If we have env vars, we export them and set them in the
-                    # ssh options
-                    if len(env_vars) > 0:
-                        (env_vars_str, send_env) = get_env_vars_str(env_vars)
-                        await pane.async_send_text(f"{env_vars_str}\n")
+                    host_opts = group["hosts"][p]
+                    host = get_host_str(host_opts)
 
-                    ssh_prefix = create_ssh_prefix(opts)
-                    host = get_host_str(group["hosts"][p])
-
-                    if s := opts.get("sleep"):
-                        await asyncio.sleep(s)
-
-                    await pane.async_send_text(f"unset HISTFILE && {ssh_prefix} {send_env} {host}\n")
+                    # If a custom command is specified, execute that and don't care about ssh at all
+                    custom_command = host_opts.get("custom_command")
+                    if custom_command:
+                        # substitute the host name in the custom command
+                        cmd = custom_command.replace("{host}", host).lstrip()
+                        await execute_command(pane, f"unset HISTFILE && {cmd}\n")
+                    else:
+                        env_vars = {}
+                        send_env = ""
+
+                        # Rank is just an env var, so set it if we have it
+                        if host_opts.get("rank"):
+                            env_vars["LC_RANK"] = str(p)
+
+                        # Split other env vars by comma and put them in a dict
+                        if from_env := host_opts.get("environment"):
+                            # if from_env is a dict, assign
+                            if isinstance(from_env, dict):
+                                env_vars = from_env
+                            else:
+                                env_vars.update(
+                                    dict(s.split("=") for s in from_env.split(","))
+                                )
+
+                        # If we have env vars, we export them and set them in the
+                        # ssh options
+                        if len(env_vars) > 0:
+                            (env_vars_str, send_env) = get_env_vars_str(env_vars)
+                            await execute_command(pane, f"{env_vars_str}\n")
+
+                        ssh_prefix = create_ssh_prefix(
+                            host_opts.get("forward_agent"),
+                            host_opts.get("extra"),
+                            host_opts.get("gateway"),
+                        )
+
+                        if host_opts.get("exec"):
+                            # Set ControlMaster=no as a workaround for
+                            # https://gitlab.com/gnachman/iterm2/-/issues/11032
+                            ssh_prefix = f"exec {ssh_prefix} -o ControlMaster=no"
+
+                        if s := host_opts.get("sleep"):
+                            await sleep(s)
+
+                        cmd = f"unset HISTFILE && {ssh_prefix} {send_env} {host}\n"
+                        cmd = re.sub(" +", " ", cmd)
+                        await execute_command(pane, cmd)
 
                 # If we run out of hosts, display an "Unused" pane
                 else:
-                    profile = await pane.async_get_profile()
-                    await pane.async_send_text(f"unset HISTFILE\n")
-                    await asyncio.sleep(0.3)
-                    await profile.async_set_foreground_color(Color.from_hex("#ff0000"))
-                    crs = "\n" * 100
-                    await pane.async_send_text(f"stty -isig -icanon -echo && echo -e '{crs}UNUSED' && cat > /dev/null\n")
+                    await create_unused_pane(pane)
 
             # Activate first pane
             await panes[0].async_activate()
 
         # Enable broadcast input for all groups that require it
         await enable_broadcast(connection, broadcast_domains)
 
     return inner
 
+
+def create_lwop(shell):
+    lwop = LocalWriteOnlyProfile()
+    lwop.set_use_custom_command("Yes")
+    lwop.set_command(f"{shell}\n")
+    return lwop
+
+
+async def sleep(s):
+    await asyncio.sleep(s)
+
+
+async def set_fullscreen(window):
+    await window.async_set_fullscreen(True)
+
+
+async def get_window(connection):
+    # Setup iterm API connection
+    app = await iterm2.async_get_app(connection)
+    window = app.current_window
+
+    # Bail if we're not inside iterm
+    if window is None:
+        click.echo("No current window")
+        sys.exit(1)
+    return window
+
+
+async def create_window(connection, window, profile_name, lwop):
+    return await window.async_create(
+        connection, profile_name, profile_customizations=lwop
+    )
+
+
+async def create_tab(window, profile_name, lwop):
+    await window.async_create_tab(profile_name, profile_customizations=lwop)
+
+
+async def execute_command(pane, cmd):
+    await pane.async_send_text(cmd)
+
+
+async def create_unused_pane(pane):
+    profile = await pane.async_get_profile()
+    await pane.async_send_text(f"unset HISTFILE\n")
+    await asyncio.sleep(0.3)
+    await profile.async_set_foreground_color(Color.from_hex("#ff0000"))
+    crs = "\n" * 100
+    await pane.async_send_text(
+        f"stty -isig -icanon -echo && echo -e '{crs}UNUSED' && cat > /dev/null\n"
+    )
+
+
 def get_host_strs_from_file(filename):
     """Gets a list of host strings from a file"""
     hosts = []
     with open(filename) as f:
         for line in f:
             hosts.append(line.strip())
     return hosts
@@ -286,22 +517,27 @@
     to False. Through command line options, booleans can only be set
     to True, while in the config file they can be set to True or False.
     """
     for opt in opts:
         if opts[opt] is False:
             opts[opt] = None
 
+
 async def enable_broadcast(connection, broadcast_domains):
     domains = []
     for panes in broadcast_domains:
         domain = iterm2.broadcast.BroadcastDomain()
         for session in panes:
             domain.add_session(session)
         domains.append(domain)
 
+    await set_broadcast_domains(connection, domains)
+
+
+async def set_broadcast_domains(connection, domains):
     await iterm2.async_set_broadcast_domains(connection, domains)
 
 
 def get_host_str(host):
     """Returns a string login@host if the login is known. Otherwise returns just the hostname"""
     if login := host.get("login"):
         return f"{login}@{host['hostname']}"
@@ -312,30 +548,34 @@
 def get_env_vars_str(env_vars):
     """Returns a string that exports the env vars and a string that sets them in the ssh options"""
     env_vars_str = " ".join([f"export {k}={v};" for k, v in env_vars.items()])
     send_env = "-o SendEnv=" + ",".join([k for k in env_vars.keys()])
     return (env_vars_str, send_env)
 
 
-def create_ssh_prefix(opts):
+def create_ssh_prefix(forward_agent, extra, gateway):
     """Returns a string that contains the ssh prefix, including the ssh options"""
     ssh_options = []
-    if opts.get("forward_agent"):
+    if forward_agent:
         ssh_options.append("-A")
 
-    if e := opts.get("extra"):
-        for extra in e:
-            if "=" in extra:
-                k, v = extra.split("=")
+    if extra:
+        if isinstance(extra, dict):
+            for k, v in extra.items():
                 ssh_options.append(f"-{k} {v}")
-            else:
-                ssh_options.append(f"-{extra}")
+        else:
+            for e in extra:
+                if "=" in e:
+                    k, v = e.split("=", 1)
+                    ssh_options.append(f"-{k} {v}")
+                else:
+                    ssh_options.append(f"-{e}")
 
-    if g := opts.get("gateway"):
-        ssh_options.append(f"-o ProxyCommand=\"ssh -W %h:%p {g}\"")
+    if gateway:
+        ssh_options.append(f'-o ProxyCommand="ssh -W %h:%p {gateway}"')
 
     return "ssh " + " ".join(ssh_options)
 
 
 def col_row_to_index(col, row, cols):
     """Calcualate the index of a pane based on row and column"""
     return row * cols + col
@@ -365,61 +605,71 @@
 
 
 def get_clusters_from_cluster_names(cluster_names, config, valid_options):
     """
     Get hosts from a list of cluster names. Note that this returns
     a list of lists of hosts; one list per cluster.
 
-    This function doesn't creates hosts from the cluster, but also applies
+    This function doesn't only create hosts from the cluster, but also applies
     the options from the cluster to the hosts.
     """
     clusters = []
     for cluster_name in cluster_names:
-        host_strings = config["clusters"][cluster_name]["hosts"]
+        host_strings = config["clusters"][cluster_name].get("hosts", [])
         cluster_options = filter_valid_options(
-            config["clusters"][cluster_name], valid_options)
+            config["clusters"][cluster_name], valid_options
+        )
+
+        # Include hosts from other clusters if specified. Note that
+        # the cluster options from the included cluster are ignored.
+        if other_clusters := config["clusters"][cluster_name].get("include_from"):
+            host_strings += flatten(
+                [config["clusters"][c]["hosts"] for c in other_clusters]
+            )
 
         hosts = host_strings_to_hosts(host_strings)
 
         # Override host options with cluster options
         for host in hosts:
-            apply_opts(host, cluster_options, valid_options)
+            host["cluster_options"] = cluster_options
 
         clusters.append(hosts)
     return clusters
 
+
 def host_strings_to_hosts(host_strings):
     """Get hosts from a list of hostname or login@hostname strings"""
     hosts = []
     for host_string in host_strings:
         (login, hostname) = parse_hostname(host_string)
-        host = {"hostname": hostname, "login": login}
+        host = {"hostname": hostname, "login": login, "cluster_options": {}}
         hosts.append(host)
     return hosts
 
-def apply_opts(opts, overrides, valid_options):
+
+def apply_opts(target, overrides, valid_options):
     """
     Apply options from the config file and command line.
     This function will recursively apply options to nested lists.
     """
-    if isinstance(opts, list):
-        for opt in opts:
-            apply_opts(opt, overrides, valid_options)
+    if isinstance(target, list):
+        for host in target:
+            apply_opts(host, overrides, valid_options)
     else:
         for key in valid_options:
-            if key in overrides and overrides[key] is not None:
-                opts[key] = overrides[key]
+            if key in overrides and overrides[key] not in (None, ()):
+                target[key] = overrides[key]
 
 
 def parse_hostname(hostname):
     """Parse a [login@]hostname and return a tuple of (login, host)"""
     login = None
     host = hostname
     if "@" in hostname:
-        login, host = hostname.split("@")
+        login, host = hostname.rsplit("@", 1)
     return login, host
 
 
 def filter_valid_options(options, valid_options):
     """
     Filter provided options to only include valid options
     Note that this function will only take top-level options and will
@@ -444,15 +694,7 @@
             except yaml.YAMLError as exc:
                 print(exc)
 
 
 def flatten(l):
     """Flatten a list of lists"""
     return [item for sublist in l for item in sublist]
-
-
-def main():
-    i2cssh(prog_name="i2cssh")
-
-
-if __name__ == '__main__':
-    main()
```

### Comparing `i2cssh-0.0.9/i2cssh.egg-info/PKG-INFO` & `i2cssh-0.1.0/src/i2cssh.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i2cssh
-Version: 0.0.9
+Version: 0.1.0
 Summary: csshX like ssh tool for iTerm2
 Home-page: http://github.com/wouterdebie/i2cssh
 Author: Wouter de Bie
 Author-email: wouter@evenflow.nl
 License: MIT
 Keywords: ssh,i2cssh,csshX
 Classifier: Operating System :: MacOS
```

### Comparing `i2cssh-0.0.9/setup.py` & `i2cssh-0.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
 from setuptools import setup
 from version import version
 
 
 setup(
-    name='i2cssh',
+    name="i2cssh",
     version=version(),
-    author=u'Wouter de Bie',
-    author_email='wouter@evenflow.nl',
-    description='csshX like ssh tool for iTerm2',
-    url='http://github.com/wouterdebie/i2cssh',
-    scripts=['i2cssh'],
-    license='MIT',
-    keywords='ssh i2cssh csshX'.split(),
+    author="Wouter de Bie",
+    author_email="wouter@evenflow.nl",
+    description="csshX like ssh tool for iTerm2",
+    url="http://github.com/wouterdebie/i2cssh",
+    scripts=["bin/i2cssh"],
+    license="MIT",
+    keywords="ssh i2cssh csshX".split(),
     classifiers=[
-        'Operating System :: MacOS',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-        'Programming Language :: Python :: 3.12',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python',
-        'Topic :: Terminals :: Terminal Emulators/X Terminals',
-        'Topic :: Utilities',
+        "Operating System :: MacOS",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python",
+        "Topic :: Terminals :: Terminal Emulators/X Terminals",
+        "Topic :: Utilities",
     ],
-    python_requires='>3.8',
+    python_requires=">3.8",
     install_requires=[
-        'click-option-group==0.5.3',
-        'click==8.1.3',
-        'iterm2==2.6',
-        'PyYAML==6.0',
+        "click-option-group==0.5.6",
+        "click==8.1.6",
+        "iterm2==2.6",
+        "PyYAML==6.0.1",
     ],
 )
```

