# Comparing `tmp/polyswarm-api-3.4.0.tar.gz` & `tmp/polyswarm-api-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyswarm-api-3.4.0.tar", last modified: Tue Jul 11 20:22:10 2023, max compression
+gzip compressed data, was "polyswarm-api-3.4.1.tar", last modified: Wed Aug  2 19:42:39 2023, max compression
```

## Comparing `polyswarm-api-3.4.0.tar` & `polyswarm-api-3.4.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 20:22:10.436744 polyswarm-api-3.4.0/
--rw-rw-rw-   0 root         (0) root         (0)     1064 2023-07-11 20:21:49.000000 polyswarm-api-3.4.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       25 2023-07-11 20:21:49.000000 polyswarm-api-3.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1616 2023-07-11 20:22:10.436744 polyswarm-api-3.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      951 2023-07-11 20:21:49.000000 polyswarm-api-3.4.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      266 2023-07-11 20:21:49.000000 polyswarm-api-3.4.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 20:22:10.436744 polyswarm-api-3.4.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1293 2023-07-11 20:21:49.000000 polyswarm-api-3.4.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 20:22:10.432744 polyswarm-api-3.4.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 20:22:10.436744 polyswarm-api-3.4.0/src/polyswarm_api/
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-07-11 20:21:49.000000 polyswarm-api-3.4.0/src/polyswarm_api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    35477 2023-07-11 20:21:49.000000 polyswarm-api-3.4.0/src/polyswarm_api/api.py
--rw-rw-rw-   0 root         (0) root         (0)    20066 2023-07-11 20:21:49.000000 polyswarm-api-3.4.0/src/polyswarm_api/core.py
--rw-rw-rw-   0 root         (0) root         (0)     1431 2023-07-11 20:21:49.000000 polyswarm-api-3.4.0/src/polyswarm_api/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    40300 2023-07-11 20:21:49.000000 polyswarm-api-3.4.0/src/polyswarm_api/resources.py
--rw-rw-rw-   0 root         (0) root         (0)      967 2023-07-11 20:21:49.000000 polyswarm-api-3.4.0/src/polyswarm_api/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 20:22:10.436744 polyswarm-api-3.4.0/src/polyswarm_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1616 2023-07-11 20:22:10.000000 polyswarm-api-3.4.0/src/polyswarm_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      433 2023-07-11 20:22:10.000000 polyswarm-api-3.4.0/src/polyswarm_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 20:22:10.000000 polyswarm-api-3.4.0/src/polyswarm_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       90 2023-07-11 20:22:10.000000 polyswarm-api-3.4.0/src/polyswarm_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-07-11 20:22:10.000000 polyswarm-api-3.4.0/src/polyswarm_api.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 19:42:39.588670 polyswarm-api-3.4.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1064 2023-08-02 19:42:12.000000 polyswarm-api-3.4.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-08-02 19:42:12.000000 polyswarm-api-3.4.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1616 2023-08-02 19:42:39.588670 polyswarm-api-3.4.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      951 2023-08-02 19:42:12.000000 polyswarm-api-3.4.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      266 2023-08-02 19:42:12.000000 polyswarm-api-3.4.1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-02 19:42:39.588670 polyswarm-api-3.4.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1293 2023-08-02 19:42:12.000000 polyswarm-api-3.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 19:42:39.584670 polyswarm-api-3.4.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 19:42:39.584670 polyswarm-api-3.4.1/src/polyswarm_api/
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-08-02 19:42:12.000000 polyswarm-api-3.4.1/src/polyswarm_api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    35841 2023-08-02 19:42:12.000000 polyswarm-api-3.4.1/src/polyswarm_api/api.py
+-rw-rw-rw-   0 root         (0) root         (0)    20066 2023-08-02 19:42:12.000000 polyswarm-api-3.4.1/src/polyswarm_api/core.py
+-rw-rw-rw-   0 root         (0) root         (0)     1431 2023-08-02 19:42:12.000000 polyswarm-api-3.4.1/src/polyswarm_api/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    40300 2023-08-02 19:42:12.000000 polyswarm-api-3.4.1/src/polyswarm_api/resources.py
+-rw-rw-rw-   0 root         (0) root         (0)      967 2023-08-02 19:42:12.000000 polyswarm-api-3.4.1/src/polyswarm_api/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 19:42:39.588670 polyswarm-api-3.4.1/src/polyswarm_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1616 2023-08-02 19:42:39.000000 polyswarm-api-3.4.1/src/polyswarm_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      433 2023-08-02 19:42:39.000000 polyswarm-api-3.4.1/src/polyswarm_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 19:42:39.000000 polyswarm-api-3.4.1/src/polyswarm_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2023-08-02 19:42:39.000000 polyswarm-api-3.4.1/src/polyswarm_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-08-02 19:42:39.000000 polyswarm-api-3.4.1/src/polyswarm_api.egg-info/top_level.txt
```

### Comparing `polyswarm-api-3.4.0/LICENSE` & `polyswarm-api-3.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `polyswarm-api-3.4.0/PKG-INFO` & `polyswarm-api-3.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyswarm-api
-Version: 3.4.0
+Version: 3.4.1
 Summary: Client library to simplify interacting with the PolySwarm consumer API
 Home-page: https://github.com/polyswarm/polyswarm-api
 Author: PolySwarm Developers
 Author-email: info@polyswarm.io
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `polyswarm-api-3.4.0/README.md` & `polyswarm-api-3.4.1/README.md`

 * *Files identical despite different names*

### Comparing `polyswarm-api-3.4.0/setup.py` & `polyswarm-api-3.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # The README.md will be used as the content for the PyPi package details page on the Python Package Index.
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 
 setup(
     name='polyswarm-api',
-    version='3.4.0',
+    version='3.4.1',
     description='Client library to simplify interacting with the PolySwarm consumer API',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='PolySwarm Developers',
     author_email='info@polyswarm.io',
     url='https://github.com/polyswarm/polyswarm-api',
     license='MIT',
```

### Comparing `polyswarm-api-3.4.0/src/polyswarm_api/api.py` & `polyswarm-api-3.4.1/src/polyswarm_api/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -345,62 +345,62 @@
         :param rule: YaraRuleset object or string containing YARA rules to install
         :param ruleset_name: Name of the ruleset.
         :return: The created Hunt resource
         """
         logger.info('Create historical hunt %s', rule)
         rule, rule_id = self._parse_rule(rule)
         return resources.HistoricalHunt.create(self, yara=rule.yara if rule else None, rule_id=rule_id,
-                                               ruleset_name=ruleset_name).result()
+                                               ruleset_name=ruleset_name, community=self.community).result()
 
     def historical_get(self, hunt=None):
         """
         Get a historical hunt.
 
         :param hunt: Hunt ID
         :return: The Hunt resource
         """
         logger.info('Get historical hunt %s', hunt)
-        return resources.HistoricalHunt.get(self, id=hunt).result()
+        return resources.HistoricalHunt.get(self, id=hunt, community=self.community).result()
 
     def historical_update(self, hunt):
         """
         Cancel a historical hunt
         :param hunt: The historical hunt id
         :return: The deleted HistoricalHunt resource
         """
         logger.info('Deleting historical hunt %s', hunt)
-        return resources.HistoricalHunt.update(self, id=hunt).result()
+        return resources.HistoricalHunt.update(self, id=hunt, community=self.community).result()
 
     def historical_delete(self, hunt):
         """
         Delete a historical hunts.
 
         :param hunt: Hunt ID
         :return: The deleted Hunt resource
         """
         logger.info('Delete historical hunt %s', hunt)
-        return resources.HistoricalHunt.delete(self, id=hunt).result()
+        return resources.HistoricalHunt.delete(self, id=hunt, community=self.community).result()
 
     def historical_list(self, since=None):
         """
         List all historical hunts
 
         :return: Generator of Hunt resources
         """
         logger.info('List historical hunts since: %s', since)
-        return resources.HistoricalHunt.list(self, since=since).result()
+        return resources.HistoricalHunt.list(self, since=since, community=self.community).result()
 
     def historical_result(self, result_id):
         """
         Get historical hunt result
 
         :param result_id: Historical result id
         :return: HistoricalHuntResult resource
         """
-        return resources.HistoricalHuntResult.get(self, id=result_id).result()
+        return resources.HistoricalHuntResult.get(self, id=result_id, community=self.community).result()
 
     def historical_results(self, hunt=None, rule_name=None, family=None,
                            polyscore_lower=None, polyscore_upper=None):
         """
         Get results from a historical hunt
 
         :param hunt: ID of the hunt (None if latest hunt results are desired)
@@ -408,86 +408,86 @@
         :param family: Filter hunt results based on the family name (exact match).
         :param polyscore_lower: Polyscore lower bound for the hunt results.
         :param polyscore_upper: Polyscore upper bound for the hunt results.
         :return: Generator of HuntResult resources
         """
         logger.info('List historical results for hunt: %s', hunt)
         return resources.HistoricalHuntResultList.get(
-            self, id=hunt, rule_name=rule_name, family=family,
+            self, id=hunt, rule_name=rule_name, family=family, community=self.community,
             polyscore_lower=polyscore_lower, polyscore_upper=polyscore_upper).result()
 
     def historical_results_delete(self, result_ids):
         """
         Delete historical scan results
 
         :param result_ids: Historical Hunt Result IDs
         :return: The deleted HuntResult resources
         """
         logger.info('Delete historical results: %s', result_ids)
-        return resources.HistoricalHuntResultList.delete(self, result_ids=result_ids).result()
+        return resources.HistoricalHuntResultList.delete(self, result_ids=result_ids, community=self.community).result()
 
     def historical_delete_list(self, historical_ids):
         """
         Delete a historical hunts.
 
         :param historical_ids: Historical Hunt IDs
         :return: The deleted Hunt resource
         """
         logger.info('Delete historical hunts %s', historical_ids)
-        return resources.HistoricalHuntList.delete(self, historical_ids=historical_ids).result()
+        return resources.HistoricalHuntList.delete(self, historical_ids=historical_ids, community=self.community).result()
 
     def ruleset_create(self, name, rules, description=None):
         """
         Create a Yara Ruleset from the provided rules with the given name in the polyswarm platform.
         :param name: Name of the ruleset
         :param rules: Yara rules as a string
         :param description: Description of the ruleset
         :return: A YaraRuleset resource
         """
         logger.info('Create ruleset %s: %s', name, rules)
-        rules = resources.YaraRuleset(dict(name=name, description=description, yara=rules), api=self)
+        rules = resources.YaraRuleset(dict(name=name, description=description, yara=rules, community=self.community), api=self)
         return resources.YaraRuleset.create(self, yara=rules.yara, name=rules.name, description=rules.description).result()
 
     def ruleset_get(self, ruleset_id=None):
         """
         Retrieve a YaraRuleset from the polyswarm platform by its Id.
         :param ruleset_id: Id of the ruleset
         :return: A YaraRuleset resource
         """
         logger.info('Get ruleset %s', ruleset_id)
-        return resources.YaraRuleset.get(self, id=ruleset_id).result()
+        return resources.YaraRuleset.get(self, id=ruleset_id, community=self.community).result()
 
     def ruleset_update(self, ruleset_id, name=None, rules=None, description=None):
         """
         Update an existing YaraRuleset in the polyswarm platform by its Id.
         :param ruleset_id: Id of the ruleset
         :param name: New name of the ruleset
         :param rules: New yara rules as a string
         :param description: New description of the ruleset
         :return: The updated YaraRuleset resource
         """
         logger.info('Update ruleset %s', ruleset_id)
-        return resources.YaraRuleset.update(self, id=ruleset_id, name=name, yara=rules, description=description).result()
+        return resources.YaraRuleset.update(self, id=ruleset_id, name=name, yara=rules, description=description, community=self.community).result()
 
     def ruleset_delete(self, ruleset_id):
         """
         Delete a YaraRuleset from the polyswarm platform by its Id.
         :param ruleset_id: Id of the ruleset
         :return: A YaraRuleset resource
         """
         logger.info('Delete ruleset %s', ruleset_id)
-        return resources.YaraRuleset.delete(self, id=ruleset_id).result()
+        return resources.YaraRuleset.delete(self, id=ruleset_id, community=self.community).result()
 
     def ruleset_list(self):
         """
         List all YaraRulesets for the current account.
         :return: A generator of YaraRuleset resources
         """
         logger.info('List rulesets')
-        return resources.YaraRuleset.list(self).result()
+        return resources.YaraRuleset.list(self, community=self.community).result()
 
     def tag_link_get(self, sha256):
         """
         Fetch the Tags and Families associated with the given sha256.
 
         :param sha256: The sha256 of the artifact.
         :return: A TagLink resource
```

### Comparing `polyswarm-api-3.4.0/src/polyswarm_api/core.py` & `polyswarm-api-3.4.1/src/polyswarm_api/core.py`

 * *Files identical despite different names*

### Comparing `polyswarm-api-3.4.0/src/polyswarm_api/exceptions.py` & `polyswarm-api-3.4.1/src/polyswarm_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `polyswarm-api-3.4.0/src/polyswarm_api/resources.py` & `polyswarm-api-3.4.1/src/polyswarm_api/resources.py`

 * *Files identical despite different names*

### Comparing `polyswarm-api-3.4.0/src/polyswarm_api/settings.py` & `polyswarm-api-3.4.1/src/polyswarm_api/settings.py`

 * *Files identical despite different names*

### Comparing `polyswarm-api-3.4.0/src/polyswarm_api.egg-info/PKG-INFO` & `polyswarm-api-3.4.1/src/polyswarm_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyswarm-api
-Version: 3.4.0
+Version: 3.4.1
 Summary: Client library to simplify interacting with the PolySwarm consumer API
 Home-page: https://github.com/polyswarm/polyswarm-api
 Author: PolySwarm Developers
 Author-email: info@polyswarm.io
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

