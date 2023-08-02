# Comparing `tmp/slack-react-0.3.2.tar.gz` & `tmp/slack-react-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slack-react-0.3.2.tar", last modified: Thu Jul 27 07:47:01 2023, max compression
+gzip compressed data, was "slack-react-0.3.3.tar", last modified: Wed Aug  2 15:37:02 2023, max compression
```

## Comparing `slack-react-0.3.2.tar` & `slack-react-0.3.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 07:47:01.395688 slack-react-0.3.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 07:47:01.391687 slack-react-0.3.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-27 07:46:51.000000 slack-react-0.3.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 07:47:01.391687 slack-react-0.3.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-27 07:46:51.000000 slack-react-0.3.2/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-27 07:46:51.000000 slack-react-0.3.2/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-27 07:46:51.000000 slack-react-0.3.2/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-27 07:46:51.000000 slack-react-0.3.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-27 07:46:51.000000 slack-react-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    42415 2023-07-27 07:47:01.395688 slack-react-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-27 07:46:51.000000 slack-react-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-27 07:46:51.000000 slack-react-0.3.2/init.ipy
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-27 07:46:51.000000 slack-react-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 07:47:01.395688 slack-react-0.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 07:47:01.395688 slack-react-0.3.2/slack_react.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    42415 2023-07-27 07:47:01.000000 slack-react-0.3.2/slack_react.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-27 07:47:01.000000 slack-react-0.3.2/slack_react.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 07:47:01.000000 slack-react-0.3.2/slack_react.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-27 07:47:01.000000 slack-react-0.3.2/slack_react.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-27 07:47:01.000000 slack-react-0.3.2/slack_react.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-27 07:47:01.000000 slack-react-0.3.2/slack_react.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    11102 2023-07-27 07:46:51.000000 slack-react-0.3.2/slack_react.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:37:02.410113 slack-react-0.3.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:37:02.406113 slack-react-0.3.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-08-02 15:36:46.000000 slack-react-0.3.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:37:02.406113 slack-react-0.3.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-02 15:36:46.000000 slack-react-0.3.3/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-08-02 15:36:46.000000 slack-react-0.3.3/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-08-02 15:36:46.000000 slack-react-0.3.3/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-02 15:36:46.000000 slack-react-0.3.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-02 15:36:46.000000 slack-react-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    42415 2023-08-02 15:37:02.410113 slack-react-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-08-02 15:36:46.000000 slack-react-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-02 15:36:46.000000 slack-react-0.3.3/init.ipy
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-08-02 15:36:46.000000 slack-react-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 15:37:02.410113 slack-react-0.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:37:02.406113 slack-react-0.3.3/slack_react.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    42415 2023-08-02 15:37:02.000000 slack-react-0.3.3/slack_react.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-08-02 15:37:02.000000 slack-react-0.3.3/slack_react.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 15:37:02.000000 slack-react-0.3.3/slack_react.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-02 15:37:02.000000 slack-react-0.3.3/slack_react.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-02 15:37:02.000000 slack-react-0.3.3/slack_react.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-02 15:37:02.000000 slack-react-0.3.3/slack_react.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11376 2023-08-02 15:36:46.000000 slack-react-0.3.3/slack_react.py
```

### Comparing `slack-react-0.3.2/.github/workflows/pypi.yaml` & `slack-react-0.3.3/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `slack-react-0.3.2/.github/workflows/release.yaml` & `slack-react-0.3.3/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `slack-react-0.3.2/LICENSE` & `slack-react-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `slack-react-0.3.2/PKG-INFO` & `slack-react-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slack-react
-Version: 0.3.2
+Version: 0.3.3
 Summary: Add reactions that spell out messages to Slack messages
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `slack-react-0.3.2/README.md` & `slack-react-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `slack-react-0.3.2/pyproject.toml` & `slack-react-0.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,14 @@
   "Programming Language :: Python :: 3",
 ]
 dependencies = [
   "appdirs",
   "rich",
   "slack_sdk"
 ]
-version = "0.3.2"
+version = "0.3.3"
 
 [tool.black]
 line-length = 79
 
 [project.scripts]
 slack-react = "slack_react:main"
```

### Comparing `slack-react-0.3.2/slack_react.egg-info/PKG-INFO` & `slack-react-0.3.3/slack_react.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slack-react
-Version: 0.3.2
+Version: 0.3.3
 Summary: Add reactions that spell out messages to Slack messages
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `slack-react-0.3.2/slack_react.py` & `slack-react-0.3.3/slack_react.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,14 +272,16 @@
             return channel["id"]
 
 
 def find_matching_message(client, channel_id, regex):
     # get the history of the channel
     response = client.conversations_history(channel=channel_id)
 
+    # TODO Get messages from threads
+
     # the messages are in the 'messages' field of the response
     messages = response["messages"]
 
     # create a regex object
     pattern = re.compile(regex)
 
     # iterate over the messages in reverse order
@@ -339,28 +341,34 @@
 
     if not channel_id:
         LOGGER.error(f"Channel '{args.channel}' not found")
         return 1
 
     response = client.conversations_history(channel=channel_id)
 
+    target_message = None
     if args.message:
         message = find_matching_message(client, channel_id, args.message)
         if not message:
             LOGGER.error("Message not found")
             return 1
         ts = message["ts"]
+        target_message = message["text"]
     else:
         # Default to last message
-        ts = response.get("messages", [{"ts": None}])[0]["ts"]
+        message = response.get("messages", [{"ts": None}])[0]
+        target_message = message["text"]
+        ts = message["ts"]
 
     if not ts:
         LOGGER.error("No messages found")
         return 1
 
+    LOGGER.debug("Target message: %s", message)
+    LOGGER.info("Target message: %s", target_message)
     remove_reactions(client, channel_id, ts)
 
     if args.reaction and not args.remove:
         add_reactions(client, channel_id, ts, args.reaction)
 
     return 0
```

