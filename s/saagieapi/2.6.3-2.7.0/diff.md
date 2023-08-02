# Comparing `tmp/saagieapi-2.6.3.tar.gz` & `tmp/saagieapi-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saagieapi-2.6.3.tar", max compression
+gzip compressed data, was "saagieapi-2.7.0.tar", max compression
```

## Comparing `saagieapi-2.6.3.tar` & `saagieapi-2.7.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0    11357 2023-07-19 13:58:57.604474 saagieapi-2.6.3/LICENSE
--rw-r--r--   0        0        0     4612 2023-07-19 13:58:57.608474 saagieapi-2.6.3/README.md
--rw-r--r--   0        0        0     1562 2023-07-19 13:59:27.649365 saagieapi-2.6.3/pyproject.toml
--rw-r--r--   0        0        0      583 2023-07-19 13:58:57.612475 saagieapi-2.6.3/saagieapi/__init__.py
--rw-r--r--   0        0        0       43 2023-07-19 13:58:57.612475 saagieapi-2.6.3/saagieapi/apps/__init__.py
--rw-r--r--   0        0        0    33369 2023-07-19 13:58:57.612475 saagieapi-2.6.3/saagieapi/apps/apps.py
--rw-r--r--   0        0        0     7591 2023-07-19 13:58:57.612475 saagieapi-2.6.3/saagieapi/apps/gql_queries.py
--rw-r--r--   0        0        0       83 2023-07-19 13:58:57.612475 saagieapi-2.6.3/saagieapi/docker_credentials/__init__.py
--rw-r--r--   0        0        0     8465 2023-07-19 13:58:57.612475 saagieapi-2.6.3/saagieapi/docker_credentials/docker_credentials.py
--rw-r--r--   0        0        0     1657 2023-07-19 13:58:57.612475 saagieapi-2.6.3/saagieapi/docker_credentials/gql_queries.py
--rw-r--r--   0        0        0       53 2023-07-19 13:58:57.612475 saagieapi-2.6.3/saagieapi/env_vars/__init__.py
--rw-r--r--   0        0        0    27280 2023-07-19 13:58:57.612475 saagieapi-2.6.3/saagieapi/env_vars/env_vars.py
--rw-r--r--   0        0        0     2671 2023-07-19 13:58:57.612475 saagieapi-2.6.3/saagieapi/env_vars/gql_queries.py
--rw-r--r--   0        0        0     4677 2023-07-19 13:58:57.612475 saagieapi-2.6.3/saagieapi/gql_queries.py
--rw-r--r--   0        0        0       49 2023-07-19 13:58:57.612475 saagieapi-2.6.3/saagieapi/groups/__init__.py
--rw-r--r--   0        0        0    14568 2023-07-19 13:58:57.612475 saagieapi-2.6.3/saagieapi/groups/groups.py
--rw-r--r--   0        0        0       43 2023-07-19 13:58:57.612475 saagieapi-2.6.3/saagieapi/jobs/__init__.py
--rw-r--r--   0        0        0     9510 2023-07-19 13:58:57.612475 saagieapi-2.6.3/saagieapi/jobs/gql_queries.py
--rw-r--r--   0        0        0    36602 2023-07-19 13:58:57.612475 saagieapi-2.6.3/saagieapi/jobs/jobs.py
--rw-r--r--   0        0        0      222 2023-07-19 13:58:57.612475 saagieapi-2.6.3/saagieapi/pipelines/__init__.py
--rw-r--r--   0        0        0     8853 2023-07-19 13:58:57.612475 saagieapi-2.6.3/saagieapi/pipelines/gql_queries.py
--rw-r--r--   0        0        0     3572 2023-07-19 13:58:57.612475 saagieapi-2.6.3/saagieapi/pipelines/graph_pipeline.py
--rw-r--r--   0        0        0    30113 2023-07-19 13:58:57.612475 saagieapi-2.6.3/saagieapi/pipelines/pipelines.py
--rw-r--r--   0        0        0       55 2023-07-19 13:58:57.612475 saagieapi-2.6.3/saagieapi/profiles/__init__.py
--rw-r--r--   0        0        0     4954 2023-07-19 13:58:57.612475 saagieapi-2.6.3/saagieapi/profiles/profiles.py
--rw-r--r--   0        0        0       55 2023-07-19 13:58:57.612475 saagieapi-2.6.3/saagieapi/projects/__init__.py
--rw-r--r--   0        0        0     2962 2023-07-19 13:58:57.612475 saagieapi-2.6.3/saagieapi/projects/gql_queries.py
--rw-r--r--   0        0        0    24508 2023-07-19 13:58:57.612475 saagieapi-2.6.3/saagieapi/projects/projects.py
--rw-r--r--   0        0        0       67 2023-07-19 13:58:57.612475 saagieapi-2.6.3/saagieapi/repositories/__init__.py
--rw-r--r--   0        0        0     8443 2023-07-19 13:58:57.612475 saagieapi-2.6.3/saagieapi/repositories/gql_queries.py
--rw-r--r--   0        0        0    10534 2023-07-19 13:58:57.612475 saagieapi-2.6.3/saagieapi/repositories/repositories.py
--rw-r--r--   0        0        0    19545 2023-07-19 13:58:57.612475 saagieapi-2.6.3/saagieapi/saagie_api.py
--rw-r--r--   0        0        0       55 2023-07-19 13:58:57.612475 saagieapi-2.6.3/saagieapi/storages/__init__.py
--rw-r--r--   0        0        0     1384 2023-07-19 13:58:57.612475 saagieapi-2.6.3/saagieapi/storages/gql_queries.py
--rw-r--r--   0        0        0     6561 2023-07-19 13:58:57.612475 saagieapi-2.6.3/saagieapi/storages/storages.py
--rw-r--r--   0        0        0       46 2023-07-19 13:58:57.612475 saagieapi-2.6.3/saagieapi/users/__init__.py
--rw-r--r--   0        0        0    10981 2023-07-19 13:58:57.612475 saagieapi-2.6.3/saagieapi/users/users.py
--rw-r--r--   0        0        0        0 2023-07-19 13:58:57.612475 saagieapi-2.6.3/saagieapi/utils/__init__.py
--rw-r--r--   0        0        0     1725 2023-07-19 13:58:57.612475 saagieapi-2.6.3/saagieapi/utils/bearer_auth.py
--rw-r--r--   0        0        0     3969 2023-07-19 13:58:57.612475 saagieapi-2.6.3/saagieapi/utils/folder_functions.py
--rw-r--r--   0        0        0     3113 2023-07-19 13:58:57.612475 saagieapi-2.6.3/saagieapi/utils/gql_client.py
--rw-r--r--   0        0        0     2336 2023-07-19 13:58:57.612475 saagieapi-2.6.3/saagieapi/utils/request_client.py
--rw-r--r--   0        0        0       54 2023-07-19 13:58:57.612475 saagieapi-2.6.3/saagieapi/utils/rich_console.py
--rw-r--r--   0        0        0     5561 1970-01-01 00:00:00.000000 saagieapi-2.6.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-02 07:55:45.052198 saagieapi-2.7.0/LICENSE
+-rw-r--r--   0        0        0     4669 2023-08-02 07:55:45.052198 saagieapi-2.7.0/README.md
+-rw-r--r--   0        0        0     1563 2023-08-02 07:56:22.106799 saagieapi-2.7.0/pyproject.toml
+-rw-r--r--   0        0        0      583 2023-08-02 07:55:45.056198 saagieapi-2.7.0/saagieapi/__init__.py
+-rw-r--r--   0        0        0       43 2023-08-02 07:55:45.056198 saagieapi-2.7.0/saagieapi/apps/__init__.py
+-rw-r--r--   0        0        0    35677 2023-08-02 07:55:45.056198 saagieapi-2.7.0/saagieapi/apps/apps.py
+-rw-r--r--   0        0        0    10408 2023-08-02 07:55:45.056198 saagieapi-2.7.0/saagieapi/apps/gql_queries.py
+-rw-r--r--   0        0        0       83 2023-08-02 07:55:45.056198 saagieapi-2.7.0/saagieapi/docker_credentials/__init__.py
+-rw-r--r--   0        0        0     8465 2023-08-02 07:55:45.056198 saagieapi-2.7.0/saagieapi/docker_credentials/docker_credentials.py
+-rw-r--r--   0        0        0     1657 2023-08-02 07:55:45.056198 saagieapi-2.7.0/saagieapi/docker_credentials/gql_queries.py
+-rw-r--r--   0        0        0       53 2023-08-02 07:55:45.056198 saagieapi-2.7.0/saagieapi/env_vars/__init__.py
+-rw-r--r--   0        0        0    27280 2023-08-02 07:55:45.056198 saagieapi-2.7.0/saagieapi/env_vars/env_vars.py
+-rw-r--r--   0        0        0     2671 2023-08-02 07:55:45.056198 saagieapi-2.7.0/saagieapi/env_vars/gql_queries.py
+-rw-r--r--   0        0        0     4677 2023-08-02 07:55:45.056198 saagieapi-2.7.0/saagieapi/gql_queries.py
+-rw-r--r--   0        0        0       49 2023-08-02 07:55:45.056198 saagieapi-2.7.0/saagieapi/groups/__init__.py
+-rw-r--r--   0        0        0    14568 2023-08-02 07:55:45.056198 saagieapi-2.7.0/saagieapi/groups/groups.py
+-rw-r--r--   0        0        0       43 2023-08-02 07:55:45.056198 saagieapi-2.7.0/saagieapi/jobs/__init__.py
+-rw-r--r--   0        0        0    10981 2023-08-02 07:55:45.056198 saagieapi-2.7.0/saagieapi/jobs/gql_queries.py
+-rw-r--r--   0        0        0    40608 2023-08-02 07:55:45.056198 saagieapi-2.7.0/saagieapi/jobs/jobs.py
+-rw-r--r--   0        0        0      222 2023-08-02 07:55:45.056198 saagieapi-2.7.0/saagieapi/pipelines/__init__.py
+-rw-r--r--   0        0        0     8853 2023-08-02 07:55:45.060198 saagieapi-2.7.0/saagieapi/pipelines/gql_queries.py
+-rw-r--r--   0        0        0     3495 2023-08-02 07:55:45.060198 saagieapi-2.7.0/saagieapi/pipelines/graph_pipeline.py
+-rw-r--r--   0        0        0    30113 2023-08-02 07:55:45.060198 saagieapi-2.7.0/saagieapi/pipelines/pipelines.py
+-rw-r--r--   0        0        0       55 2023-08-02 07:55:45.060198 saagieapi-2.7.0/saagieapi/profiles/__init__.py
+-rw-r--r--   0        0        0     4954 2023-08-02 07:55:45.060198 saagieapi-2.7.0/saagieapi/profiles/profiles.py
+-rw-r--r--   0        0        0       55 2023-08-02 07:55:45.060198 saagieapi-2.7.0/saagieapi/projects/__init__.py
+-rw-r--r--   0        0        0     2962 2023-08-02 07:55:45.060198 saagieapi-2.7.0/saagieapi/projects/gql_queries.py
+-rw-r--r--   0        0        0    24508 2023-08-02 07:55:45.060198 saagieapi-2.7.0/saagieapi/projects/projects.py
+-rw-r--r--   0        0        0       67 2023-08-02 07:55:45.060198 saagieapi-2.7.0/saagieapi/repositories/__init__.py
+-rw-r--r--   0        0        0     8443 2023-08-02 07:55:45.060198 saagieapi-2.7.0/saagieapi/repositories/gql_queries.py
+-rw-r--r--   0        0        0    10534 2023-08-02 07:55:45.060198 saagieapi-2.7.0/saagieapi/repositories/repositories.py
+-rw-r--r--   0        0        0    19545 2023-08-02 07:55:45.060198 saagieapi-2.7.0/saagieapi/saagie_api.py
+-rw-r--r--   0        0        0       55 2023-08-02 07:55:45.060198 saagieapi-2.7.0/saagieapi/storages/__init__.py
+-rw-r--r--   0        0        0     1384 2023-08-02 07:55:45.060198 saagieapi-2.7.0/saagieapi/storages/gql_queries.py
+-rw-r--r--   0        0        0     6561 2023-08-02 07:55:45.060198 saagieapi-2.7.0/saagieapi/storages/storages.py
+-rw-r--r--   0        0        0       46 2023-08-02 07:55:45.060198 saagieapi-2.7.0/saagieapi/users/__init__.py
+-rw-r--r--   0        0        0    10981 2023-08-02 07:55:45.060198 saagieapi-2.7.0/saagieapi/users/users.py
+-rw-r--r--   0        0        0        0 2023-08-02 07:55:45.060198 saagieapi-2.7.0/saagieapi/utils/__init__.py
+-rw-r--r--   0        0        0     1725 2023-08-02 07:55:45.060198 saagieapi-2.7.0/saagieapi/utils/bearer_auth.py
+-rw-r--r--   0        0        0     3969 2023-08-02 07:55:45.060198 saagieapi-2.7.0/saagieapi/utils/folder_functions.py
+-rw-r--r--   0        0        0     3113 2023-08-02 07:55:45.060198 saagieapi-2.7.0/saagieapi/utils/gql_client.py
+-rw-r--r--   0        0        0     2336 2023-08-02 07:55:45.060198 saagieapi-2.7.0/saagieapi/utils/request_client.py
+-rw-r--r--   0        0        0       54 2023-08-02 07:55:45.060198 saagieapi-2.7.0/saagieapi/utils/rich_console.py
+-rw-r--r--   0        0        0     5610 1970-01-01 00:00:00.000000 saagieapi-2.7.0/PKG-INFO
```

### Comparing `saagieapi-2.6.3/LICENSE` & `saagieapi-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `saagieapi-2.6.3/README.md` & `saagieapi-2.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 
 | **Saagie platform version** | **saagie-api release** |
 |-----------------------------|------------------------|
 | < 2.2.0                     | < 0.6.0                |
 | >= 2.2.0                    | >= 0.6.0               |
 | >= 2023.01                  | >= 2.4.0               |
 | >= 2023.02                  | >= 2.6.0               |
+| >= 2023.03                  | >= 2.7.0               |
 
 ## Usage
 
 All the implemented features are documented in the [Wiki](https://github.com/saagie/api-saagie/wiki)
 
 Here's a full example of how to use the API:
```

### Comparing `saagieapi-2.6.3/pyproject.toml` & `saagieapi-2.7.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "saagieapi"
-version = "2.6.3"
+version = "2.7.0"
 description = "Python API to interact with Saagie"
 authors = ["Saagie"]
 license = "GLWTPL"
 readme = "README.md"
 repository = "https://github.com/saagie/api-saagie"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 requests = "^2.27.0"
 gql = "^3.0.0"
-pytz = "^2021.1"
+pytz = ">=2021.1"
 croniter = "^1.0.1"
 requests_toolbelt = "^0.9.1"
 deprecation = "^2.1.0"
 rich = "^12.3.0"
 
 [tool.poetry.dev-dependencies]
 python-semantic-release = "7.28.1"
```

### Comparing `saagieapi-2.6.3/saagieapi/__init__.py` & `saagieapi-2.7.0/saagieapi/__init__.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.6.3/saagieapi/apps/apps.py` & `saagieapi-2.7.0/saagieapi/apps/apps.py`

 * *Files 4% similar despite different names*

```diff
@@ -890,7 +890,82 @@
         """
         project_id = self.saagie_api.projects.get_id(project_name)
         apps = self.saagie_api.apps.list_for_project_minimal(project_id)["project"]["apps"]
         app = list(filter(lambda j: j["name"] == app_name, apps))
         if app:
             return app[0]["id"]
         raise NameError(f"❌ App {app_name} does not exist.")
+
+    def get_stats(self, history_id, version_number, start_time):
+        """Get stats of the app
+
+        Parameters
+        ----------
+        history_id : str
+            UUID of your app history
+        version_number : str
+            Number of the version to get the stats
+        start_time : str
+            Date since to get the stats (format : "%Y-%m-%dT%H:%M:%S.%fZ")
+
+        Returns
+        -------
+        dict
+            Dict of app's stats
+        """
+        params = {
+            "appHistoryId": history_id,
+            "versionNumber": version_number,
+            "startTime": start_time,
+        }
+
+        return self.saagie_api.client.execute(query=gql(GQL_STATS_APP), variable_values=params)
+
+    def get_history_statuses(self, history_id, version_number, start_time):
+        """Get statuses history of the app
+
+        Parameters
+        ----------
+        history_id : str
+            UUID of your app history
+        version_number : str
+            Number of the version to get the statuses history
+        start_time : str
+            Date since to get the statuses history (format : "%Y-%m-%dT%H:%M:%S.%fZ")
+
+        Returns
+        -------
+        dict
+            Dict of app's statuses history
+        """
+        params = {
+            "appHistoryId": history_id,
+            "versionNumber": version_number,
+            "startTime": start_time,
+        }
+
+        return self.saagie_api.client.execute(query=gql(GQL_HISTORY_APP_STATUS), variable_values=params)
+
+    def count_history_statuses(self, history_id, version_number, start_time):
+        """Get count of statues history of the app
+
+        Parameters
+        ----------
+        history_id : str
+            UUID of your app history
+        version_number : str
+            Number of the version to get the count of statuses history
+        start_time : str
+            Date since to get the count of statuses history (format : "%Y-%m-%dT%H:%M:%S.%fZ")
+
+        Returns
+        -------
+        dict
+            count of statuses history
+        """
+        params = {
+            "appHistoryId": history_id,
+            "versionNumber": version_number,
+            "startTime": start_time,
+        }
+
+        return self.saagie_api.client.execute(query=gql(GQL_COUNT_HISTORY_APP_STATUS), variable_values=params)
```

### Comparing `saagieapi-2.6.3/saagieapi/docker_credentials/docker_credentials.py` & `saagieapi-2.7.0/saagieapi/docker_credentials/docker_credentials.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.6.3/saagieapi/docker_credentials/gql_queries.py` & `saagieapi-2.7.0/saagieapi/docker_credentials/gql_queries.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.6.3/saagieapi/env_vars/env_vars.py` & `saagieapi-2.7.0/saagieapi/env_vars/env_vars.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.6.3/saagieapi/env_vars/gql_queries.py` & `saagieapi-2.7.0/saagieapi/env_vars/gql_queries.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.6.3/saagieapi/gql_queries.py` & `saagieapi-2.7.0/saagieapi/gql_queries.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.6.3/saagieapi/groups/groups.py` & `saagieapi-2.7.0/saagieapi/groups/groups.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.6.3/saagieapi/jobs/gql_queries.py` & `saagieapi-2.7.0/saagieapi/jobs/gql_queries.py`

 * *Files 20% similar despite different names*

```diff
@@ -54,14 +54,18 @@
             }
             extraTechnology{
                 language
                 version
             }
             isCurrent
             isMajor
+            deletableState {
+                deletable
+                reasons
+            }
         }
         category
         technology {
             id
         }
         isScheduled
         cronScheduling
@@ -85,14 +89,15 @@
                 limit
             }
             memory{
                 request
                 limit
             }
         }
+        originalJobId
     }
 }
 """
 
 GQL_GET_JOB_INSTANCE = """
 query jobInstanceQuery($jobInstanceId: UUID!){
     jobInstance(id: $jobInstanceId){
@@ -342,14 +347,18 @@
             }
             extraTechnology{
                 language
                 version
             }
             isCurrent
             isMajor
+            deletableState {
+                deletable
+                reasons
+            }
         }
         category
         technology {
             id
         }
         isScheduled
         cronScheduling
@@ -370,15 +379,15 @@
                 limit
             }
             memory{
                 request
                 limit
             }
         }
-        
+        originalJobId
     }
 }
 """
 
 GQL_DELETE_JOB = """
 mutation deleteJobMutation($jobId: UUID!){
     deleteJob(jobId: $jobId)
@@ -392,7 +401,57 @@
         versions {      
             number      
             isCurrent      
         }    
     }
 }
 """
+
+GQL_DELETE_JOB_INSTANCE = """
+mutation deleteJobInstances($jobId: UUID!, $jobInstancesId: [UUID!]) {
+    deleteJobInstances(jobId: $jobId, jobInstanceIds: $jobInstancesId){
+        id
+        success
+    }
+}
+"""
+
+GQL_DELETE_JOB_INSTANCES_BY_SELECTOR = """
+mutation deleteJobInstancesBySelector($jobId: UUID!, 
+                                    $selector: JobInstanceSelector!, 
+                                    $minusInstancesId: [UUID!], 
+                                    $moreInstancesId: [UUID!]) {
+    deleteJobInstancesBySelector(
+        jobId: $jobId, 
+        selector: $selector,
+        minusJobInstanceIds: $minusInstancesId,
+        moreJobInstanceIds: $moreInstancesId
+    )
+}
+"""
+
+GQL_DELETE_JOB_VERSION = """
+mutation deleteJobVersion($jobId: UUID!, $jobVersionsNumber: [Int!]!) {
+    deleteJobVersions(jobId: $jobId, jobVersionNumbers: $jobVersionsNumber) {
+        number
+        success
+    }
+}
+"""
+
+GQL_DUPLICATE_JOB = """
+mutation duplicateJob($jobId: UUID!) {
+    duplicateJob(originalJobId: $jobId) {
+        id
+        name
+    }
+}
+"""
+
+GQL_COUNT_INSTANCES_BY_SELECTOR = """
+query countJobInstancesBySelector($jobId: UUID!) {
+    countJobInstancesBySelector(jobId: $jobId) {
+        selector
+        count
+    }
+}
+"""
```

### Comparing `saagieapi-2.6.3/saagieapi/jobs/jobs.py` & `saagieapi-2.7.0/saagieapi/jobs/jobs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1009,7 +1009,120 @@
             logging.info("✅ Job [%s] successfully imported", job_name)
         except Exception as exception:
             result = False
             logging.warning("❌ Job [%s] has not been successfully imported", job_name)
             logging.error("Something went wrong %s", exception)
 
         return result
+
+    def delete_instances(self, job_id, job_instances_id):
+        """Delete given job's instances
+        NB: You can only delete an instance not associated to a pipeline instance
+        Also you can only delete instances if they aren't processing by the orchestrator
+
+        Parameters
+        ----------
+        job_id : str
+            UUID of your job (see README on how to find it)
+        job_instances_id : [str]
+            List of UUID of instances to delete (see README on how to find it)
+
+        Returns
+        -------
+        dict
+            Dict of deleted instances
+
+        """
+        params = {"jobId": job_id, "jobInstancesId": job_instances_id}
+        result = self.saagie_api.client.execute(query=gql(GQL_DELETE_JOB_INSTANCE), variable_values=params)
+        logging.info("✅ Instances of job [%s] successfully deleted", job_id)
+        return result
+
+    def delete_instances_by_selector(
+        self, job_id, selector, exclude_instances_id: List = None, include_instances_id: List = None
+    ):
+        """Delete given job's instances by selector
+        NB: You can only delete an instance not associated to a pipeline instance.
+        Also you can only delete instances if they aren't processing by the orchestrator
+
+        Parameters
+        ----------
+        job_id : str
+            UUID of your job (see README on how to find it)
+        selector : str
+            Name of status to select in this list : ALL, SUCCEEDED, FAILED, STOPPED, UNKNOWN
+        exclude_instances_id : [str]
+            List of UUID of instances of your job to exclude from the deletion
+        include_instances_id: [str]
+            List of UUID of instances of your job to include from the deletion
+
+        Returns
+        -------
+        int
+            Return the number of instances deleted
+
+        """
+        params = {
+            "jobId": job_id,
+            "selector": selector,
+            "minusInstancesId": [] if exclude_instances_id is None else exclude_instances_id,
+            "moreInstancesId": [] if include_instances_id is None else include_instances_id,
+        }
+        result = self.saagie_api.client.execute(query=gql(GQL_DELETE_JOB_INSTANCES_BY_SELECTOR), variable_values=params)
+        logging.info("✅ Instances of job [%s] successfully deleted", job_id)
+        return result
+
+    def delete_versions(self, job_id, versions):
+        """Delete given job's versions
+        NB: You can only delete a version not associated to a pipeline instance
+
+        Parameters
+        ----------
+        job_id : str
+            UUID of your job (see README on how to find it)
+        versions : [str]
+            List of version numbers to delete
+
+        Returns
+        -------
+        dict
+            Dict of deleted versions
+
+        """
+        params = {"jobId": job_id, "jobVersionsNumber": versions}
+        result = self.saagie_api.client.execute(query=gql(GQL_DELETE_JOB_VERSION), variable_values=params)
+        logging.info("✅ Versions of job [%s] successfully deleted", job_id)
+        return result
+
+    def duplicate(self, job_id):
+        """Duplicate a given job
+
+        Parameters
+        ----------
+        job_id : str
+            UUID of your job (see README on how to find it)
+
+        Returns
+        -------
+        dict
+            Dict of duplicate job
+        """
+        result = self.saagie_api.client.execute(query=gql(GQL_DUPLICATE_JOB), variable_values={"jobId": job_id})
+        logging.info("✅ Job [%s] successfully duplicated", job_id)
+        return result
+
+    def count_instances_by_status(self, job_id):
+        """Count job instances by status
+
+        Parameters
+        ----------
+        job_id : str
+            UUID of your job (see README on how to find it)
+
+        Returns
+        -------
+        dict
+            Dict of job instances number by status
+        """
+        return self.saagie_api.client.execute(
+            query=gql(GQL_COUNT_INSTANCES_BY_SELECTOR), variable_values={"jobId": job_id}
+        )
```

### Comparing `saagieapi-2.6.3/saagieapi/pipelines/gql_queries.py` & `saagieapi-2.7.0/saagieapi/pipelines/gql_queries.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.6.3/saagieapi/pipelines/graph_pipeline.py` & `saagieapi-2.7.0/saagieapi/pipelines/graph_pipeline.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import uuid
 from typing import List
 
-import gql
-
 
 class Node:
     def __init__(self) -> None:
         self.uid = uuid.uuid4()
 
 
 class JobNode(Node):
@@ -31,24 +29,24 @@
     def add_failure_node(self, node: Node):
         self.next_nodes_failure.append(node)
 
 
 class ConditionStatusNode(ConditionNode):
     def __init__(self) -> None:
         super().__init__()
-        self.conditionValue: str = ""
+        self.condition_value: str = ""
 
     def put_all_success(self):
-        self.conditionValue = "AllSuccess"
+        self.condition_value = "AllSuccess"
 
     def put_all_success_or_skipped(self):
-        self.conditionValue = "AllSuccessOrSkipped"
+        self.condition_value = "AllSuccessOrSkipped"
 
     def put_at_least_one_success(self):
-        self.conditionValue = "AtLeastOneSuccess"
+        self.condition_value = "AtLeastOneSuccess"
 
 
 class ConditionExpressionNode(ConditionNode):
     def __init__(self) -> None:
         super().__init__()
         self.expression: str = ""
 
@@ -73,24 +71,23 @@
             if isinstance(node, JobNode):
                 dict_job = {"id": str(node.uid), "nextNodes": [str(nn.uid) for nn in node.next_nodes], "job": {}}
                 dict_job["job"]["id"] = node.job_id
                 self.list_job_nodes.append(dict_job)
                 if node.next_nodes:
                     for nex in node.next_nodes:
                         self.fill_nodes_lists(nex)
-            # elif isinstance(node, ConditionNode):
-            elif isinstance(node, ConditionStatusNode) or isinstance(node, ConditionExpressionNode):
+            elif isinstance(node, (ConditionStatusNode, ConditionExpressionNode)):
                 dict_condition = {
                     "id": str(node.uid),
                     "nextNodesSuccess": [str(nn.uid) for nn in node.next_nodes_success],
                     "nextNodesFailure": [str(nn.uid) for nn in node.next_nodes_failure],
                 }
                 if isinstance(node, ConditionStatusNode):
                     # "condition": {"status": {"value" : "AtLeastOneSuccess"}}
-                    dict_condition["condition"] = {"status": {"value": node.conditionValue}}
+                    dict_condition["condition"] = {"status": {"value": node.condition_value}}
 
                 if isinstance(node, ConditionExpressionNode):
                     # "condition": {"custom": {"value" : "1 + 1 == 2"}}
                     dict_condition["condition"] = {"custom": {"expression": node.expression}}
 
                 self.list_conditions_nodes.append(dict_condition)
                 if node.next_nodes_success:
```

### Comparing `saagieapi-2.6.3/saagieapi/pipelines/pipelines.py` & `saagieapi-2.7.0/saagieapi/pipelines/pipelines.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.6.3/saagieapi/profiles/profiles.py` & `saagieapi-2.7.0/saagieapi/profiles/profiles.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.6.3/saagieapi/projects/gql_queries.py` & `saagieapi-2.7.0/saagieapi/projects/gql_queries.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.6.3/saagieapi/projects/projects.py` & `saagieapi-2.7.0/saagieapi/projects/projects.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.6.3/saagieapi/repositories/gql_queries.py` & `saagieapi-2.7.0/saagieapi/repositories/gql_queries.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.6.3/saagieapi/repositories/repositories.py` & `saagieapi-2.7.0/saagieapi/repositories/repositories.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.6.3/saagieapi/saagie_api.py` & `saagieapi-2.7.0/saagieapi/saagie_api.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.6.3/saagieapi/storages/gql_queries.py` & `saagieapi-2.7.0/saagieapi/storages/gql_queries.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.6.3/saagieapi/storages/storages.py` & `saagieapi-2.7.0/saagieapi/storages/storages.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.6.3/saagieapi/users/users.py` & `saagieapi-2.7.0/saagieapi/users/users.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.6.3/saagieapi/utils/bearer_auth.py` & `saagieapi-2.7.0/saagieapi/utils/bearer_auth.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.6.3/saagieapi/utils/folder_functions.py` & `saagieapi-2.7.0/saagieapi/utils/folder_functions.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.6.3/saagieapi/utils/gql_client.py` & `saagieapi-2.7.0/saagieapi/utils/gql_client.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.6.3/saagieapi/utils/request_client.py` & `saagieapi-2.7.0/saagieapi/utils/request_client.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.6.3/PKG-INFO` & `saagieapi-2.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saagieapi
-Version: 2.6.3
+Version: 2.7.0
 Summary: Python API to interact with Saagie
 Home-page: https://github.com/saagie/api-saagie
 License: GLWTPL
 Author: Saagie
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: croniter (>=1.0.1,<2.0.0)
 Requires-Dist: deprecation (>=2.1.0,<3.0.0)
 Requires-Dist: gql (>=3.0.0,<4.0.0)
-Requires-Dist: pytz (>=2021.1,<2022.0)
+Requires-Dist: pytz (>=2021.1)
 Requires-Dist: requests (>=2.27.0,<3.0.0)
 Requires-Dist: requests_toolbelt (>=0.9.1,<0.10.0)
 Requires-Dist: rich (>=12.3.0,<13.0.0)
 Project-URL: Repository, https://github.com/saagie/api-saagie
 Description-Content-Type: text/markdown
 
 ![Saagie api logo](https://github.com/saagie/api-saagie/blob/master/.github/banner.png?raw=true)
@@ -60,14 +60,15 @@
 
 | **Saagie platform version** | **saagie-api release** |
 |-----------------------------|------------------------|
 | < 2.2.0                     | < 0.6.0                |
 | >= 2.2.0                    | >= 0.6.0               |
 | >= 2023.01                  | >= 2.4.0               |
 | >= 2023.02                  | >= 2.6.0               |
+| >= 2023.03                  | >= 2.7.0               |
 
 ## Usage
 
 All the implemented features are documented in the [Wiki](https://github.com/saagie/api-saagie/wiki)
 
 Here's a full example of how to use the API:
```

