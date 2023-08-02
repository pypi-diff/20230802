# Comparing `tmp/duffy-3.3.7.tar.gz` & `tmp/duffy-3.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duffy-3.3.7.tar", max compression
+gzip compressed data, was "duffy-3.3.8.tar", max compression
```

## Comparing `duffy-3.3.7.tar` & `duffy-3.3.8.tar`

### file list

```diff
@@ -1,64 +1,65 @@
--rw-r--r--   0        0        0     1062 2022-04-01 09:18:05.729280 duffy-3.3.7/LICENSE
--rw-r--r--   0        0        0     2614 2022-03-17 11:36:00.362316 duffy-3.3.7/README.md
--rw-r--r--   0        0        0        0 2021-11-04 19:37:25.052374 duffy-3.3.7/duffy/__init__.py
--rw-r--r--   0        0        0     3797 2023-06-13 10:45:34.117491 duffy-3.3.7/duffy/admin.py
--rw-r--r--   0        0        0      763 2023-06-13 10:45:34.117491 duffy-3.3.7/duffy/api_models/__init__.py
--rw-r--r--   0        0        0      438 2022-05-05 09:39:16.752260 duffy-3.3.7/duffy/api_models/common.py
--rw-r--r--   0        0        0      901 2023-06-13 10:45:34.117491 duffy-3.3.7/duffy/api_models/node.py
--rw-r--r--   0        0        0      785 2023-06-13 10:45:34.117491 duffy-3.3.7/duffy/api_models/pool.py
--rw-r--r--   0        0        0     1276 2023-06-13 10:45:34.117491 duffy-3.3.7/duffy/api_models/session.py
--rw-r--r--   0        0        0     2168 2023-06-13 10:45:34.117491 duffy-3.3.7/duffy/api_models/tenant.py
--rw-r--r--   0        0        0        0 2021-11-04 19:37:25.053374 duffy-3.3.7/duffy/app/__init__.py
--rw-r--r--   0        0        0     1478 2021-12-23 11:53:40.419878 duffy-3.3.7/duffy/app/auth.py
--rw-r--r--   0        0        0        0 2021-12-09 12:35:44.361777 duffy-3.3.7/duffy/app/controllers/__init__.py
--rw-r--r--   0        0        0     2393 2023-06-13 10:45:34.117491 duffy-3.3.7/duffy/app/controllers/node.py
--rw-r--r--   0        0        0     2003 2023-06-13 10:45:34.117491 duffy-3.3.7/duffy/app/controllers/pool.py
--rw-r--r--   0        0        0    13631 2023-06-13 10:45:34.117491 duffy-3.3.7/duffy/app/controllers/session.py
--rw-r--r--   0        0        0     5820 2023-06-13 10:45:34.117491 duffy-3.3.7/duffy/app/controllers/tenant.py
--rw-r--r--   0        0        0      438 2023-06-13 10:45:34.117491 duffy-3.3.7/duffy/app/database.py
--rw-r--r--   0        0        0     1763 2023-06-13 10:45:34.118491 duffy-3.3.7/duffy/app/main.py
--rw-r--r--   0        0        0     1301 2023-06-13 10:45:34.118491 duffy-3.3.7/duffy/app/util.py
--rw-r--r--   0        0        0    22150 2023-06-13 10:45:34.118491 duffy-3.3.7/duffy/cli.py
--rw-r--r--   0        0        0       96 2023-06-13 10:45:34.118491 duffy-3.3.7/duffy/client/__init__.py
--rw-r--r--   0        0        0     4287 2023-06-13 10:45:34.118491 duffy-3.3.7/duffy/client/formatter.py
--rw-r--r--   0        0        0     4201 2023-06-13 10:45:34.118491 duffy-3.3.7/duffy/client/main.py
--rw-r--r--   0        0        0       71 2023-06-13 10:45:34.118491 duffy-3.3.7/duffy/configuration/__init__.py
--rw-r--r--   0        0        0     1736 2023-06-13 10:45:34.118491 duffy-3.3.7/duffy/configuration/main.py
--rw-r--r--   0        0        0     4804 2023-06-13 10:45:34.118491 duffy-3.3.7/duffy/configuration/validation.py
--rw-r--r--   0        0        0     2675 2023-06-13 10:45:34.118491 duffy-3.3.7/duffy/database/__init__.py
--rw-r--r--   0        0        0     1840 2022-02-14 16:30:16.414977 duffy-3.3.7/duffy/database/migrations/env.py
--rw-r--r--   0        0        0     2512 2023-06-13 10:45:34.118491 duffy-3.3.7/duffy/database/migrations/main.py
--rw-r--r--   0        0        0      530 2022-02-23 17:54:04.381223 duffy-3.3.7/duffy/database/migrations/script.py.mako
--rw-r--r--   0        0        0        0 2021-11-23 15:11:13.761517 duffy-3.3.7/duffy/database/migrations/versions/.empty
--rw-r--r--   0        0        0      611 2023-06-13 10:45:34.118491 duffy-3.3.7/duffy/database/migrations/versions/ce2e575cb800_add_tenant_session_lifetimes.py
--rw-r--r--   0        0        0      134 2022-01-31 09:33:13.840537 duffy-3.3.7/duffy/database/model/__init__.py
--rw-r--r--   0        0        0     3032 2023-04-17 12:35:31.798781 duffy-3.3.7/duffy/database/model/node.py
--rw-r--r--   0        0        0     1082 2022-03-14 11:18:18.016981 duffy-3.3.7/duffy/database/model/session.py
--rw-r--r--   0        0        0     2845 2023-06-13 10:45:34.119491 duffy-3.3.7/duffy/database/model/tenant.py
--rw-r--r--   0        0        0     3811 2023-06-13 10:45:34.119491 duffy-3.3.7/duffy/database/setup.py
--rw-r--r--   0        0        0      281 2022-02-14 16:30:16.414977 duffy-3.3.7/duffy/database/types.py
--rw-r--r--   0        0        0     4590 2023-06-13 10:45:34.119491 duffy-3.3.7/duffy/database/util.py
--rw-r--r--   0        0        0      358 2021-11-24 14:21:28.066307 duffy-3.3.7/duffy/exceptions.py
--rw-r--r--   0        0        0        0 2022-02-07 13:59:09.420061 duffy-3.3.7/duffy/legacy/__init__.py
--rw-r--r--   0        0        0       99 2022-02-07 13:59:09.420061 duffy-3.3.7/duffy/legacy/api_models.py
--rw-r--r--   0        0        0      949 2022-02-07 13:59:09.420061 duffy-3.3.7/duffy/legacy/auth.py
--rw-r--r--   0        0        0     8273 2023-06-13 10:45:34.119491 duffy-3.3.7/duffy/legacy/main.py
--rw-r--r--   0        0        0     3163 2023-06-13 10:45:34.119491 duffy-3.3.7/duffy/misc.py
--rw-r--r--   0        0        0        0 2023-06-13 10:45:34.119491 duffy-3.3.7/duffy/nodes/__init__.py
--rw-r--r--   0        0        0     2862 2023-06-13 10:45:34.119491 duffy-3.3.7/duffy/nodes/context.py
--rw-r--r--   0        0        0      102 2023-06-13 10:45:34.119491 duffy-3.3.7/duffy/nodes/mechanisms/__init__.py
--rw-r--r--   0        0        0     4076 2023-06-13 10:45:34.119491 duffy-3.3.7/duffy/nodes/mechanisms/ansible.py
--rw-r--r--   0        0        0     1210 2023-06-13 10:45:34.119491 duffy-3.3.7/duffy/nodes/mechanisms/main.py
--rw-r--r--   0        0        0     3855 2023-06-13 10:45:34.119491 duffy-3.3.7/duffy/nodes/pools.py
--rw-r--r--   0        0        0     2175 2022-05-03 12:14:31.685232 duffy-3.3.7/duffy/shell.py
--rw-r--r--   0        0        0      293 2022-03-14 11:18:18.016981 duffy-3.3.7/duffy/tasks/__init__.py
--rw-r--r--   0        0        0      171 2022-02-14 16:30:16.414977 duffy-3.3.7/duffy/tasks/base.py
--rw-r--r--   0        0        0     7168 2023-06-13 10:45:34.119491 duffy-3.3.7/duffy/tasks/deprovision.py
--rw-r--r--   0        0        0     1221 2022-03-15 09:19:01.122691 duffy-3.3.7/duffy/tasks/expire.py
--rw-r--r--   0        0        0      417 2022-03-15 09:19:01.122691 duffy-3.3.7/duffy/tasks/locking.py
--rw-r--r--   0        0        0     1326 2023-06-13 10:45:34.119491 duffy-3.3.7/duffy/tasks/main.py
--rw-r--r--   0        0        0    11136 2023-06-13 10:45:34.120491 duffy-3.3.7/duffy/tasks/provision.py
--rw-r--r--   0        0        0     7004 2023-06-13 10:45:34.120491 duffy-3.3.7/duffy/util.py
--rw-r--r--   0        0        0       72 2023-06-13 10:45:34.120491 duffy-3.3.7/duffy/version.py
--rw-r--r--   0        0        0     4296 2023-06-26 11:04:46.069607 duffy-3.3.7/pyproject.toml
--rw-r--r--   0        0        0     5714 1970-01-01 00:00:00.000000 duffy-3.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-27 11:04:28.772486 duffy-3.3.8/LICENSE
+-rw-r--r--   0        0        0     2614 2023-07-27 11:06:43.284214 duffy-3.3.8/README.md
+-rw-r--r--   0        0        0        0 2021-11-04 19:37:25.052374 duffy-3.3.8/duffy/__init__.py
+-rw-r--r--   0        0        0     3797 2023-07-27 11:04:28.774486 duffy-3.3.8/duffy/admin.py
+-rw-r--r--   0        0        0      763 2023-07-27 11:04:28.774486 duffy-3.3.8/duffy/api_models/__init__.py
+-rw-r--r--   0        0        0      438 2023-07-27 11:04:28.774486 duffy-3.3.8/duffy/api_models/common.py
+-rw-r--r--   0        0        0      901 2023-07-27 11:04:28.774486 duffy-3.3.8/duffy/api_models/node.py
+-rw-r--r--   0        0        0      785 2023-07-27 11:04:28.774486 duffy-3.3.8/duffy/api_models/pool.py
+-rw-r--r--   0        0        0     1276 2023-07-27 11:04:28.774486 duffy-3.3.8/duffy/api_models/session.py
+-rw-r--r--   0        0        0     2168 2023-07-27 11:04:28.775486 duffy-3.3.8/duffy/api_models/tenant.py
+-rw-r--r--   0        0        0        0 2021-11-04 19:37:25.053374 duffy-3.3.8/duffy/app/__init__.py
+-rw-r--r--   0        0        0     1478 2021-12-23 11:53:40.419878 duffy-3.3.8/duffy/app/auth.py
+-rw-r--r--   0        0        0        0 2021-12-09 12:35:44.361777 duffy-3.3.8/duffy/app/controllers/__init__.py
+-rw-r--r--   0        0        0     2393 2023-07-27 11:04:28.775486 duffy-3.3.8/duffy/app/controllers/node.py
+-rw-r--r--   0        0        0     2003 2023-07-27 11:04:28.775486 duffy-3.3.8/duffy/app/controllers/pool.py
+-rw-r--r--   0        0        0    13953 2023-07-31 09:03:52.298005 duffy-3.3.8/duffy/app/controllers/session.py
+-rw-r--r--   0        0        0     5820 2023-07-27 11:04:28.775486 duffy-3.3.8/duffy/app/controllers/tenant.py
+-rw-r--r--   0        0        0      438 2023-07-27 11:04:28.775486 duffy-3.3.8/duffy/app/database.py
+-rw-r--r--   0        0        0     1763 2023-07-27 11:04:28.775486 duffy-3.3.8/duffy/app/main.py
+-rw-r--r--   0        0        0     1301 2023-07-27 11:04:28.775486 duffy-3.3.8/duffy/app/util.py
+-rw-r--r--   0        0        0    22150 2023-07-27 11:04:28.775486 duffy-3.3.8/duffy/cli.py
+-rw-r--r--   0        0        0       96 2023-07-27 11:04:28.775486 duffy-3.3.8/duffy/client/__init__.py
+-rw-r--r--   0        0        0     4287 2023-07-27 11:04:28.775486 duffy-3.3.8/duffy/client/formatter.py
+-rw-r--r--   0        0        0     4201 2023-07-27 11:04:28.775486 duffy-3.3.8/duffy/client/main.py
+-rw-r--r--   0        0        0       71 2023-07-27 11:04:28.775486 duffy-3.3.8/duffy/configuration/__init__.py
+-rw-r--r--   0        0        0     1736 2023-07-27 11:04:28.775486 duffy-3.3.8/duffy/configuration/main.py
+-rw-r--r--   0        0        0     4804 2023-07-31 09:06:49.009911 duffy-3.3.8/duffy/configuration/validation.py
+-rw-r--r--   0        0        0     2675 2023-07-27 11:04:28.776486 duffy-3.3.8/duffy/database/__init__.py
+-rw-r--r--   0        0        0     1840 2022-02-14 16:30:16.414977 duffy-3.3.8/duffy/database/migrations/env.py
+-rw-r--r--   0        0        0     2512 2023-07-27 11:04:28.776486 duffy-3.3.8/duffy/database/migrations/main.py
+-rw-r--r--   0        0        0      530 2022-02-23 17:54:04.381223 duffy-3.3.8/duffy/database/migrations/script.py.mako
+-rw-r--r--   0        0        0        0 2021-11-23 15:11:13.761517 duffy-3.3.8/duffy/database/migrations/versions/.empty
+-rw-r--r--   0        0        0     1963 2023-07-27 14:56:03.011019 duffy-3.3.8/duffy/database/migrations/versions/36cf064c0481_ignore_failed_nodes_in_unique_indexes.py
+-rw-r--r--   0        0        0      611 2023-07-27 11:04:28.776486 duffy-3.3.8/duffy/database/migrations/versions/ce2e575cb800_add_tenant_session_lifetimes.py
+-rw-r--r--   0        0        0      134 2022-01-31 09:33:13.840537 duffy-3.3.8/duffy/database/model/__init__.py
+-rw-r--r--   0        0        0     3049 2023-07-27 14:56:03.011019 duffy-3.3.8/duffy/database/model/node.py
+-rw-r--r--   0        0        0     1082 2022-03-14 11:18:18.016981 duffy-3.3.8/duffy/database/model/session.py
+-rw-r--r--   0        0        0     2845 2023-07-27 11:04:28.776486 duffy-3.3.8/duffy/database/model/tenant.py
+-rw-r--r--   0        0        0     3811 2023-07-27 11:04:20.438441 duffy-3.3.8/duffy/database/setup.py
+-rw-r--r--   0        0        0      281 2022-02-14 16:30:16.414977 duffy-3.3.8/duffy/database/types.py
+-rw-r--r--   0        0        0     4590 2023-07-27 11:04:28.776486 duffy-3.3.8/duffy/database/util.py
+-rw-r--r--   0        0        0      358 2021-11-24 14:21:28.066307 duffy-3.3.8/duffy/exceptions.py
+-rw-r--r--   0        0        0        0 2022-02-07 13:59:09.420061 duffy-3.3.8/duffy/legacy/__init__.py
+-rw-r--r--   0        0        0       99 2022-02-07 13:59:09.420061 duffy-3.3.8/duffy/legacy/api_models.py
+-rw-r--r--   0        0        0      949 2022-02-07 13:59:09.420061 duffy-3.3.8/duffy/legacy/auth.py
+-rw-r--r--   0        0        0     8273 2023-07-27 11:04:28.776486 duffy-3.3.8/duffy/legacy/main.py
+-rw-r--r--   0        0        0     3163 2023-07-31 09:06:49.010911 duffy-3.3.8/duffy/misc.py
+-rw-r--r--   0        0        0        0 2023-07-27 11:04:28.776486 duffy-3.3.8/duffy/nodes/__init__.py
+-rw-r--r--   0        0        0     2862 2023-07-27 11:04:28.776486 duffy-3.3.8/duffy/nodes/context.py
+-rw-r--r--   0        0        0      102 2023-07-27 11:04:28.776486 duffy-3.3.8/duffy/nodes/mechanisms/__init__.py
+-rw-r--r--   0        0        0     4076 2023-07-27 11:04:28.776486 duffy-3.3.8/duffy/nodes/mechanisms/ansible.py
+-rw-r--r--   0        0        0     1210 2023-07-27 11:04:28.776486 duffy-3.3.8/duffy/nodes/mechanisms/main.py
+-rw-r--r--   0        0        0     3855 2023-07-27 11:04:28.777486 duffy-3.3.8/duffy/nodes/pools.py
+-rw-r--r--   0        0        0     2175 2023-07-27 11:04:28.777486 duffy-3.3.8/duffy/shell.py
+-rw-r--r--   0        0        0      293 2022-03-14 11:18:18.016981 duffy-3.3.8/duffy/tasks/__init__.py
+-rw-r--r--   0        0        0      171 2022-02-14 16:30:16.414977 duffy-3.3.8/duffy/tasks/base.py
+-rw-r--r--   0        0        0     7168 2023-07-27 11:04:28.777486 duffy-3.3.8/duffy/tasks/deprovision.py
+-rw-r--r--   0        0        0     1221 2022-03-15 09:19:01.122691 duffy-3.3.8/duffy/tasks/expire.py
+-rw-r--r--   0        0        0      417 2022-03-15 09:19:01.122691 duffy-3.3.8/duffy/tasks/locking.py
+-rw-r--r--   0        0        0     1326 2023-07-27 11:04:28.777486 duffy-3.3.8/duffy/tasks/main.py
+-rw-r--r--   0        0        0    11136 2023-07-27 11:04:28.777486 duffy-3.3.8/duffy/tasks/provision.py
+-rw-r--r--   0        0        0     7004 2023-07-27 11:04:28.777486 duffy-3.3.8/duffy/util.py
+-rw-r--r--   0        0        0       72 2023-07-27 11:04:28.777486 duffy-3.3.8/duffy/version.py
+-rw-r--r--   0        0        0     4843 2023-08-02 10:48:51.871772 duffy-3.3.8/pyproject.toml
+-rw-r--r--   0        0        0     5745 1970-01-01 00:00:00.000000 duffy-3.3.8/PKG-INFO
```

### Comparing `duffy-3.3.7/LICENSE` & `duffy-3.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `duffy-3.3.7/README.md` & `duffy-3.3.8/README.md`

 * *Files identical despite different names*

### Comparing `duffy-3.3.7/duffy/admin.py` & `duffy-3.3.8/duffy/admin.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.7/duffy/api_models/__init__.py` & `duffy-3.3.8/duffy/api_models/__init__.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.7/duffy/api_models/node.py` & `duffy-3.3.8/duffy/api_models/node.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.7/duffy/api_models/pool.py` & `duffy-3.3.8/duffy/api_models/pool.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.7/duffy/api_models/session.py` & `duffy-3.3.8/duffy/api_models/session.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.7/duffy/api_models/tenant.py` & `duffy-3.3.8/duffy/api_models/tenant.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.7/duffy/app/auth.py` & `duffy-3.3.8/duffy/app/auth.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.7/duffy/app/controllers/node.py` & `duffy-3.3.8/duffy/app/controllers/node.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.7/duffy/app/controllers/pool.py` & `duffy-3.3.8/duffy/app/controllers/pool.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.7/duffy/app/controllers/session.py` & `duffy-3.3.8/duffy/app/controllers/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -261,14 +261,18 @@
             headers={"Retry-After": "0"},
         )
 
     # None not in contextualized_ipaddrs -> carry on
     async with SerializationErrorRetryContext() as retry:
         async for attempt in retry.attempts:
             for node in nodes_in_transaction:
+                # reload the node object to be on the safe side
+                node = (
+                    await db_async_session.execute(select(Node).filter_by(id=node.id))
+                ).scalar_one()
                 node.state = NodeState.deployed
 
             # Meh. Reload the session instance to ensure all related objects are present in the
             # session.
             await db_async_session.flush()
 
             session = (
@@ -281,14 +285,18 @@
                     )
                 )
             ).scalar_one()
 
             try:
                 await db_async_session.commit()
             except IntegrityError as exc:  # pragma: no cover
+                if attempt < retry.no_attempts:
+                    # re-raise to retry
+                    raise
+
                 raise HTTPException(HTTP_422_UNPROCESSABLE_ENTITY, str(exc))
 
     # Tell backend worker to fill up pools from which nodes were taken.
     fill_pools.delay(pool_names=list(pools_to_fill_up)).forget()
 
     return {"action": "post", "session": session}
```

### Comparing `duffy-3.3.7/duffy/app/controllers/tenant.py` & `duffy-3.3.8/duffy/app/controllers/tenant.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.7/duffy/app/main.py` & `duffy-3.3.8/duffy/app/main.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.7/duffy/app/util.py` & `duffy-3.3.8/duffy/app/util.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.7/duffy/cli.py` & `duffy-3.3.8/duffy/cli.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.7/duffy/client/formatter.py` & `duffy-3.3.8/duffy/client/formatter.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.7/duffy/client/main.py` & `duffy-3.3.8/duffy/client/main.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.7/duffy/configuration/main.py` & `duffy-3.3.8/duffy/configuration/main.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.7/duffy/configuration/validation.py` & `duffy-3.3.8/duffy/configuration/validation.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.7/duffy/database/__init__.py` & `duffy-3.3.8/duffy/database/__init__.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.7/duffy/database/migrations/env.py` & `duffy-3.3.8/duffy/database/migrations/env.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.7/duffy/database/migrations/main.py` & `duffy-3.3.8/duffy/database/migrations/main.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.7/duffy/database/migrations/script.py.mako` & `duffy-3.3.8/duffy/database/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `duffy-3.3.7/duffy/database/migrations/versions/ce2e575cb800_add_tenant_session_lifetimes.py` & `duffy-3.3.8/duffy/database/migrations/versions/ce2e575cb800_add_tenant_session_lifetimes.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.7/duffy/database/model/node.py` & `duffy-3.3.8/duffy/database/model/node.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,36 +6,37 @@
 
 from ...api_models import SessionNodeModel
 from .. import Base
 from ..types import NodeState
 from ..util import CreatableMixin, RetirableMixin
 from .session import Session
 
+INDEX_UNIQUENESS_CLAUSE = and_(
+    Column("retired_at") == None,  # noqa: E711
+    Column("state") != "provisioning",
+    Column("state") != "failed",
+)
 
-class Node(Base, CreatableMixin, RetirableMixin):
-    index_uniqueness_clause = and_(
-        Column("retired_at") == None,  # noqa: E711
-        Column("state") != "provisioning",
-    )
 
+class Node(Base, CreatableMixin, RetirableMixin):
     __tablename__ = "nodes"
     __table_args__ = (
         Index(
             "active_hostname_index",
             "hostname",
             unique=True,
-            sqlite_where=index_uniqueness_clause,
-            postgresql_where=index_uniqueness_clause,
+            sqlite_where=INDEX_UNIQUENESS_CLAUSE,
+            postgresql_where=INDEX_UNIQUENESS_CLAUSE,
         ),
         Index(
             "active_ipaddr_index",
             "ipaddr",
             unique=True,
-            sqlite_where=index_uniqueness_clause,
-            postgresql_where=index_uniqueness_clause,
+            sqlite_where=INDEX_UNIQUENESS_CLAUSE,
+            postgresql_where=INDEX_UNIQUENESS_CLAUSE,
         ),
     )
 
     id = Column(Integer, primary_key=True, nullable=False)
     hostname = Column(Text, nullable=True)
     ipaddr = Column(Text, nullable=True)
     state = Column(
```

### Comparing `duffy-3.3.7/duffy/database/model/session.py` & `duffy-3.3.8/duffy/database/model/session.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.7/duffy/database/model/tenant.py` & `duffy-3.3.8/duffy/database/model/tenant.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.7/duffy/database/setup.py` & `duffy-3.3.8/duffy/database/setup.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.7/duffy/database/util.py` & `duffy-3.3.8/duffy/database/util.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.7/duffy/legacy/auth.py` & `duffy-3.3.8/duffy/legacy/auth.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.7/duffy/legacy/main.py` & `duffy-3.3.8/duffy/legacy/main.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.7/duffy/misc.py` & `duffy-3.3.8/duffy/misc.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.7/duffy/nodes/context.py` & `duffy-3.3.8/duffy/nodes/context.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.7/duffy/nodes/mechanisms/ansible.py` & `duffy-3.3.8/duffy/nodes/mechanisms/ansible.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.7/duffy/nodes/mechanisms/main.py` & `duffy-3.3.8/duffy/nodes/mechanisms/main.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.7/duffy/nodes/pools.py` & `duffy-3.3.8/duffy/nodes/pools.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.7/duffy/shell.py` & `duffy-3.3.8/duffy/shell.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.7/duffy/tasks/deprovision.py` & `duffy-3.3.8/duffy/tasks/deprovision.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.7/duffy/tasks/expire.py` & `duffy-3.3.8/duffy/tasks/expire.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.7/duffy/tasks/main.py` & `duffy-3.3.8/duffy/tasks/main.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.7/duffy/tasks/provision.py` & `duffy-3.3.8/duffy/tasks/provision.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.7/duffy/util.py` & `duffy-3.3.8/duffy/util.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.7/pyproject.toml` & `duffy-3.3.8/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "duffy"
-version = "3.3.7"
+version = "3.3.8"
 description = "CentOS CI provisioner"
 authors = ["Nils Philippsen <nils@redhat.com>", "Vipul Siddharth <siddharthvipul1@gmail.com>", "Akashdeep Dhar <akashdeep@redhat.com>", "Ben Capper <bcapper@redhat.com>"]
 license = "MIT"
 maintainers = ["Nils Philippsen <nils@redhat.com>", "Vipul Siddharth <siddharthvipul1@gmail.com>", "Akashdeep Dhar <akashdeep@redhat.com>", "Ben Capper <bcapper@redhat.com>"]
 readme = "README.md"
 homepage = "https://github.com/CentOS/duffy"
 repository = "https://github.com/CentOS/duffy"
@@ -37,47 +37,47 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 click = "^8.0.3"
 PyYAML = "^6"
 SQLAlchemy = {version = "^2.0.5", extras=["asyncio"], optional = true}
 alembic = {version = "^1.7.5", optional = true}
 bcrypt = {version = "^3.2 || ^4", optional = true}
-fastapi = {version = ">=0.70, <2", optional = true}
-uvicorn = {version = ">=0.15, <2", optional = true}
+fastapi = {version = "^0.70 || ^0.71 || ^0.72 || ^0.73 || ^0.74 || ^0.75 || ^0.76 || ^0.77 || ^0.78 || ^0.79 || ^0.80 || ^0.81 || ^0.82 || ^0.83 || ^0.84 || ^0.85 || ^0.86 || ^0.87 || ^0.88 || ^0.89 || ^0.90 || ^0.91 || ^0.92 || ^0.93 || ^0.94 || ^0.95 || ^0.96 || ^0.97 || ^0.98 || ^0.99 || ^0.100.0", optional = true}
+uvicorn = {version = "^0.15 || ^0.16 || ^0.17 || ^0.18 || ^0.19 || ^0.20 || ^0.21 || ^0.22 || ^0.23.0", optional = true}
 Jinja2 = {version = "^3.0.3", optional = true}
 ansible-runner = {version = "^2.1.1", optional = true}
-asyncpg = {version = ">=0.25, <2", optional = true}
+asyncpg = {version = "^0.25 || ^0.26 || ^0.27 || ^0.28", optional = true}
 celery = {version = "^5.2.1", extras = ["redis"], optional = true}
-httpx = {version = ">=0.18.2, <2", optional = true}
-ipython = {version = ">=7.29", optional = true}
-jmespath = {version = ">=0.10, <2", optional = true}
+httpx = {version = "^0.18.2 || ^0.19 || ^0.20 || ^0.21 || ^0.22 || ^0.23 || ^0.24", optional = true}
+ipython = {version = "^7.29 || ^8", optional = true}
+jmespath = {version = ">=0.10,<1 || ^1", optional = true}
 pottery = {version = "^3", optional = true}
 psycopg2 = {version = "^2.9.2", optional = true}
 aiodns = {version = "^3.0.0", optional = true}
-pydantic = ">=1.6.2"
-aiosqlite = {version = ">=0.17.0, <2", optional = true}
-pyxdg = ">=0.27, <2"
+pydantic = "^1.6.2"
+aiosqlite = {version = "^0.17 || ^0.18 || ^0.19", optional = true}
+pyxdg = "^0.27 || ^0.28"
 
 [tool.poetry.dev-dependencies]
 Jinja2 = "^3.0.3"
 ansible = "^5.2 || ^6 || ^7.0.0 || ^8.0.0"
 ansible-core = "^2.12.1"
 ansible-runner = "^2.1.1"
-black = ">=21.9b0"
-flake8 = ">=3.9.2"
-httpx = ">=0.18.2, <2"
+black = "^21.9b0 || ^22 || ^23"
+flake8 = "^3.9.2 || ^4 || ^5 || ^6.0.0"
+httpx = "^0.18.2 || ^0.19 || ^0.20 || ^0.21 || ^0.22 || ^0.23 || ^0.24"
 isort = "^5.9.3"
-jmespath = ">=0.10, <2"
+jmespath = "^0.10 || ^1"
 poetry = "^1.2.0"
 pottery = "^3"
 pytest = ">=6.2.5"
-pytest-asyncio = ">=0.17, <2"
-pytest-black = ">=0.3.12, <2"
+pytest-asyncio = "^0.17 || ^0.18 || ^0.19 || ^0.20 || ^0.21"
+pytest-black = "^0.3.12"
 pytest-cov = "^3 || ^4"
-pytest-isort = ">=2"
+pytest-isort = "^2 || ^3"
 tox = "^3.24.4 || ^4.0.0"
 psycopg = "^3.0.16"
 pytest-postgresql = "^4.1.1 || ^5.0.0"
 coverage-conditional-plugin = "^0.8.0 || ^0.9.0"
 
 [tool.poetry.extras]
 # the `serve` command
```

### Comparing `duffy-3.3.7/PKG-INFO` & `duffy-3.3.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duffy
-Version: 3.3.7
+Version: 3.3.8
 Summary: CentOS CI provisioner
 Home-page: https://github.com/CentOS/duffy
 License: MIT
 Keywords: baremetal,ci,vm,opennebula,centos
 Author: Nils Philippsen
 Author-email: nils@redhat.com
 Maintainer: Nils Philippsen
@@ -40,30 +40,30 @@
 Provides-Extra: postgresql
 Provides-Extra: sqlite
 Provides-Extra: tasks
 Requires-Dist: Jinja2 (>=3.0.3,<4.0.0) ; extra == "app" or extra == "tasks" or extra == "legacy"
 Requires-Dist: PyYAML (>=6,<7)
 Requires-Dist: SQLAlchemy[asyncio] (>=2.0.5,<3.0.0) ; extra == "app" or extra == "admin" or extra == "database" or extra == "dev-shell"
 Requires-Dist: aiodns (>=3.0.0,<4.0.0) ; extra == "app" or extra == "tasks"
-Requires-Dist: aiosqlite (>=0.17.0,<2) ; extra == "sqlite"
+Requires-Dist: aiosqlite (>=0.17,<0.20) ; extra == "sqlite"
 Requires-Dist: alembic (>=1.7.5,<2.0.0) ; extra == "app" or extra == "database" or extra == "dev-shell"
 Requires-Dist: ansible-runner (>=2.1.1,<3.0.0) ; extra == "app" or extra == "tasks"
-Requires-Dist: asyncpg (>=0.25,<2) ; extra == "postgresql"
+Requires-Dist: asyncpg (>=0.25,<0.29) ; extra == "postgresql"
 Requires-Dist: bcrypt (>=3.2,<5) ; extra == "app" or extra == "admin" or extra == "database" or extra == "dev-shell"
 Requires-Dist: celery[redis] (>=5.2.1,<6.0.0) ; extra == "app" or extra == "tasks"
 Requires-Dist: click (>=8.0.3,<9.0.0)
-Requires-Dist: fastapi (>=0.70,<2) ; extra == "app" or extra == "admin"
-Requires-Dist: httpx (>=0.18.2,<2) ; extra == "legacy" or extra == "client"
-Requires-Dist: ipython (>=7.29) ; extra == "dev-shell"
+Requires-Dist: fastapi (>=0.70,<0.101.0) ; extra == "app" or extra == "admin"
+Requires-Dist: httpx (>=0.18.2,<0.25) ; extra == "legacy" or extra == "client"
+Requires-Dist: ipython (>=7.29,<9) ; extra == "dev-shell"
 Requires-Dist: jmespath (>=0.10,<2) ; extra == "app" or extra == "tasks"
 Requires-Dist: pottery (>=3,<4) ; extra == "app" or extra == "tasks"
 Requires-Dist: psycopg2 (>=2.9.2,<3.0.0) ; extra == "postgresql"
-Requires-Dist: pydantic (>=1.6.2)
-Requires-Dist: pyxdg (>=0.27,<2)
-Requires-Dist: uvicorn (>=0.15,<2) ; extra == "app"
+Requires-Dist: pydantic (>=1.6.2,<2.0.0)
+Requires-Dist: pyxdg (>=0.27,<0.29)
+Requires-Dist: uvicorn (>=0.15,<0.24.0) ; extra == "app"
 Project-URL: Documentation, https://github.com/CentOS/duffy/wiki
 Project-URL: Repository, https://github.com/CentOS/duffy
 Description-Content-Type: text/markdown
 
 ## Info
 Community Platform Engineering team (of Red Hat) is working on revamping this project and thus, have cleaned this repository by
 * marking other branches stale
```

