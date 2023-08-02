# Comparing `tmp/elabapi-python-0.2.4.tar.gz` & `tmp/elabapi-python-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elabapi-python-0.2.4.tar", last modified: Tue May 16 23:42:57 2023, max compression
+gzip compressed data, was "elabapi-python-0.3.0.tar", last modified: Wed Aug  2 00:25:26 2023, max compression
```

## Comparing `elabapi-python-0.2.4.tar` & `elabapi-python-0.3.0.tar`

### file list

```diff
@@ -1,200 +1,220 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:42:57.198383 elabapi-python-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-16 23:42:57.198383 elabapi-python-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19244 2023-05-16 23:42:50.000000 elabapi-python-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:42:57.146383 elabapi-python-0.2.4/elabapi_python/
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-05-16 23:42:50.000000 elabapi-python-0.2.4/elabapi_python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:42:57.150383 elabapi-python-0.2.4/elabapi_python/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-16 23:42:50.000000 elabapi-python-0.2.4/elabapi_python/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/api/api_keys_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    23562 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/api/comments_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10023 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/api/config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14817 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/api/events_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    20788 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/api/experiments_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18664 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/api/experiments_templates_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10417 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/api/favorite_tags_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    17373 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/api/idps_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    20047 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/api/items_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    17478 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/api/items_types_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14876 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/api/links_to_experiments_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14628 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/api/links_to_items_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    16132 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/api/notifications_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    20141 2023-05-16 23:42:50.000000 elabapi-python-0.2.4/elabapi_python/api/status_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18459 2023-05-16 23:42:50.000000 elabapi-python-0.2.4/elabapi_python/api/steps_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    22933 2023-05-16 23:42:50.000000 elabapi-python-0.2.4/elabapi_python/api/tags_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    20990 2023-05-16 23:42:50.000000 elabapi-python-0.2.4/elabapi_python/api/team_tags_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    20313 2023-05-16 23:42:50.000000 elabapi-python-0.2.4/elabapi_python/api/teamgroups_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14137 2023-05-16 23:42:50.000000 elabapi-python-0.2.4/elabapi_python/api/teams_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    17653 2023-05-16 23:42:50.000000 elabapi-python-0.2.4/elabapi_python/api/todolist_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-05-16 23:42:50.000000 elabapi-python-0.2.4/elabapi_python/api/unfinished_steps_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    28747 2023-05-16 23:42:50.000000 elabapi-python-0.2.4/elabapi_python/api/uploads_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14991 2023-05-16 23:42:50.000000 elabapi-python-0.2.4/elabapi_python/api/users_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25079 2023-05-16 23:42:50.000000 elabapi-python-0.2.4/elabapi_python/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-05-16 23:42:50.000000 elabapi-python-0.2.4/elabapi_python/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:42:57.162383 elabapi-python-0.2.4/elabapi_python/models/
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-05-16 23:42:50.000000 elabapi-python-0.2.4/elabapi_python/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-05-16 23:42:48.000000 elabapi-python-0.2.4/elabapi_python/models/apikey.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-05-16 23:42:48.000000 elabapi-python-0.2.4/elabapi_python/models/apikeys_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-05-16 23:42:48.000000 elabapi-python-0.2.4/elabapi_python/models/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)    72934 2023-05-16 23:42:48.000000 elabapi-python-0.2.4/elabapi_python/models/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    32079 2023-05-16 23:42:48.000000 elabapi-python-0.2.4/elabapi_python/models/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     9929 2023-05-16 23:42:48.000000 elabapi-python-0.2.4/elabapi_python/models/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-05-16 23:42:48.000000 elabapi-python-0.2.4/elabapi_python/models/events_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-05-16 23:42:48.000000 elabapi-python-0.2.4/elabapi_python/models/events_id_body1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-05-16 23:42:48.000000 elabapi-python-0.2.4/elabapi_python/models/eventsid_delta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-16 23:42:48.000000 elabapi-python-0.2.4/elabapi_python/models/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12288 2023-05-16 23:42:48.000000 elabapi-python-0.2.4/elabapi_python/models/experiment_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-05-16 23:42:48.000000 elabapi-python-0.2.4/elabapi_python/models/experiments_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-05-16 23:42:48.000000 elabapi-python-0.2.4/elabapi_python/models/experiments_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-05-16 23:42:48.000000 elabapi-python-0.2.4/elabapi_python/models/experiments_links_subid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-16 23:42:48.000000 elabapi-python-0.2.4/elabapi_python/models/experiments_templates_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-05-16 23:42:48.000000 elabapi-python-0.2.4/elabapi_python/models/experiments_templates_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-05-16 23:42:48.000000 elabapi-python-0.2.4/elabapi_python/models/favtags_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-05-16 23:42:48.000000 elabapi-python-0.2.4/elabapi_python/models/id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-05-16 23:42:48.000000 elabapi-python-0.2.4/elabapi_python/models/id1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-05-16 23:42:48.000000 elabapi-python-0.2.4/elabapi_python/models/id2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-05-16 23:42:48.000000 elabapi-python-0.2.4/elabapi_python/models/id3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-16 23:42:48.000000 elabapi-python-0.2.4/elabapi_python/models/id_comments_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-05-16 23:42:48.000000 elabapi-python-0.2.4/elabapi_python/models/id_status_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/models/id_steps_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/models/id_tags_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/models/id_teamgroups_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/models/id_uploads_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    11027 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/models/idp.py
--rw-r--r--   0 runner    (1001) docker     (123)    12993 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/models/idps_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/models/idps_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/models/inline_response200.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/models/inline_response2001.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/models/inline_response2002.py
--rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/models/inline_response2003.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/models/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/models/items_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/models/items_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/models/items_links_subid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/models/items_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/models/items_types_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/models/link.py
--rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/models/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/models/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/models/step.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/models/steps_subid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/models/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/models/tags_subid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    14827 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/models/team.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/models/team_tags_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/models/team_tags_body1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/models/team_tags_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/models/teamgroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/models/teamgroup_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/models/teamgroups_subid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/models/teams_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/models/todoitem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/models/todolist_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/models/todolist_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/models/unfinished_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/models/unfinished_steps.py
--rw-r--r--   0 runner    (1001) docker     (123)    11700 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/models/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/models/uploads_subid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    10577 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/models/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/models/users_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/models/users_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/elabapi_python/models/users_teams.py
--rw-r--r--   0 runner    (1001) docker     (123)    13031 2023-05-16 23:42:50.000000 elabapi-python-0.2.4/elabapi_python/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:42:57.146383 elabapi-python-0.2.4/elabapi_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-16 23:42:57.000000 elabapi-python-0.2.4/elabapi_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-05-16 23:42:57.000000 elabapi-python-0.2.4/elabapi_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 23:42:57.000000 elabapi-python-0.2.4/elabapi_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-16 23:42:57.000000 elabapi-python-0.2.4/elabapi_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-16 23:42:57.000000 elabapi-python-0.2.4/elabapi_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 23:42:57.198383 elabapi-python-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-16 23:42:50.000000 elabapi-python-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:42:57.198383 elabapi-python-0.2.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 23:42:50.000000 elabapi-python-0.2.4/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_api_keys_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-16 23:42:48.000000 elabapi-python-0.2.4/test/test_apikey.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-16 23:42:48.000000 elabapi-python-0.2.4/test/test_apikeys_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-16 23:42:48.000000 elabapi-python-0.2.4/test/test_comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_comments_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-16 23:42:48.000000 elabapi-python-0.2.4/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-16 23:42:48.000000 elabapi-python-0.2.4/test/test_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-16 23:42:48.000000 elabapi-python-0.2.4/test/test_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_events_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-16 23:42:48.000000 elabapi-python-0.2.4/test/test_events_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-16 23:42:48.000000 elabapi-python-0.2.4/test/test_events_id_body1.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-16 23:42:48.000000 elabapi-python-0.2.4/test/test_eventsid_delta.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-16 23:42:48.000000 elabapi-python-0.2.4/test/test_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-16 23:42:48.000000 elabapi-python-0.2.4/test/test_experiment_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_experiments_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-16 23:42:48.000000 elabapi-python-0.2.4/test/test_experiments_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-16 23:42:48.000000 elabapi-python-0.2.4/test/test_experiments_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-16 23:42:48.000000 elabapi-python-0.2.4/test/test_experiments_links_subid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_experiments_templates_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-16 23:42:48.000000 elabapi-python-0.2.4/test/test_experiments_templates_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-16 23:42:48.000000 elabapi-python-0.2.4/test/test_experiments_templates_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_favorite_tags_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-16 23:42:48.000000 elabapi-python-0.2.4/test/test_favtags_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-16 23:42:48.000000 elabapi-python-0.2.4/test/test_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-16 23:42:48.000000 elabapi-python-0.2.4/test/test_id1.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-16 23:42:48.000000 elabapi-python-0.2.4/test/test_id2.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-16 23:42:48.000000 elabapi-python-0.2.4/test/test_id3.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-16 23:42:48.000000 elabapi-python-0.2.4/test/test_id_comments_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-16 23:42:48.000000 elabapi-python-0.2.4/test/test_id_status_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_id_steps_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_id_tags_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_id_teamgroups_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_id_uploads_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_idp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_idps_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_idps_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_idps_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_inline_response200.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_inline_response2001.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_inline_response2002.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_inline_response2003.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_items_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_items_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_items_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_items_links_subid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_items_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_items_types_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_items_types_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_links_to_experiments_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_links_to_items_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_notifications_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-16 23:42:50.000000 elabapi-python-0.2.4/test/test_status_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-16 23:42:50.000000 elabapi-python-0.2.4/test/test_steps_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_steps_subid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-16 23:42:50.000000 elabapi-python-0.2.4/test/test_tags_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_tags_subid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_team.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-16 23:42:50.000000 elabapi-python-0.2.4/test/test_team_tags_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_team_tags_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_team_tags_body1.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_team_tags_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_teamgroup.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_teamgroup_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-16 23:42:50.000000 elabapi-python-0.2.4/test/test_teamgroups_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_teamgroups_subid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-16 23:42:50.000000 elabapi-python-0.2.4/test/test_teams_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_teams_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_todoitem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-16 23:42:50.000000 elabapi-python-0.2.4/test/test_todolist_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_todolist_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_todolist_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_unfinished_step.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_unfinished_steps.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-16 23:42:50.000000 elabapi-python-0.2.4/test/test_unfinished_steps_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-16 23:42:50.000000 elabapi-python-0.2.4/test/test_uploads_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_uploads_subid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-16 23:42:50.000000 elabapi-python-0.2.4/test/test_users_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_users_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_users_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-16 23:42:49.000000 elabapi-python-0.2.4/test/test_users_teams.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:25:26.469799 elabapi-python-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-08-02 00:25:26.469799 elabapi-python-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20466 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:25:26.389795 elabapi-python-0.3.0/elabapi_python/
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/elabapi_python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:25:26.405796 elabapi-python-0.3.0/elabapi_python/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/elabapi_python/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/elabapi_python/api/api_keys_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23562 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/elabapi_python/api/comments_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10023 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/elabapi_python/api/config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14817 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/elabapi_python/api/events_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20865 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/elabapi_python/api/experiments_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18664 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/elabapi_python/api/experiments_templates_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10420 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/elabapi_python/api/favorite_tags_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17373 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/elabapi_python/api/idps_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/elabapi_python/api/info_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20124 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/elabapi_python/api/items_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17478 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/elabapi_python/api/items_types_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14876 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/elabapi_python/api/links_to_experiments_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14628 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/elabapi_python/api/links_to_items_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16132 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/elabapi_python/api/notifications_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18943 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/elabapi_python/api/revisions_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20141 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/elabapi_python/api/status_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18459 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/elabapi_python/api/steps_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22432 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/elabapi_python/api/tags_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20990 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/elabapi_python/api/team_tags_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20313 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/elabapi_python/api/teamgroups_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14137 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/elabapi_python/api/teams_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17653 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/elabapi_python/api/todolist_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/elabapi_python/api/unfinished_steps_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29006 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/elabapi_python/api/uploads_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15030 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/elabapi_python/api/users_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25079 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/elabapi_python/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/elabapi_python/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:25:26.433798 elabapi-python-0.3.0/elabapi_python/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/elabapi_python/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-08-02 00:25:14.000000 elabapi-python-0.3.0/elabapi_python/models/apikey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-08-02 00:25:14.000000 elabapi-python-0.3.0/elabapi_python/models/apikeys_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-08-02 00:25:14.000000 elabapi-python-0.3.0/elabapi_python/models/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73807 2023-08-02 00:25:14.000000 elabapi-python-0.3.0/elabapi_python/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30070 2023-08-02 00:25:14.000000 elabapi-python-0.3.0/elabapi_python/models/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9929 2023-08-02 00:25:14.000000 elabapi-python-0.3.0/elabapi_python/models/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-08-02 00:25:14.000000 elabapi-python-0.3.0/elabapi_python/models/events_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-08-02 00:25:14.000000 elabapi-python-0.3.0/elabapi_python/models/events_id_body1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-08-02 00:25:14.000000 elabapi-python-0.3.0/elabapi_python/models/eventsid_delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/elabapi_python/models/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12288 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/elabapi_python/models/experiment_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/elabapi_python/models/experiments_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/elabapi_python/models/experiments_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/elabapi_python/models/experiments_links_subid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/elabapi_python/models/experiments_templates_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/elabapi_python/models/experiments_templates_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/elabapi_python/models/favtags_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/elabapi_python/models/id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/elabapi_python/models/id1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/elabapi_python/models/id2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/elabapi_python/models/id3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/elabapi_python/models/id_comments_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/elabapi_python/models/id_revisions_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/elabapi_python/models/id_status_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/elabapi_python/models/id_steps_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/elabapi_python/models/id_tags_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/elabapi_python/models/id_teamgroups_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/elabapi_python/models/id_uploads_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11027 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/elabapi_python/models/idp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12993 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/elabapi_python/models/idps_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/elabapi_python/models/idps_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9919 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/elabapi_python/models/inline_response200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/elabapi_python/models/inline_response2001.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/elabapi_python/models/inline_response2002.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/elabapi_python/models/inline_response2003.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/elabapi_python/models/inline_response2004.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/elabapi_python/models/inline_response2005.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/elabapi_python/models/inline_response2006.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/elabapi_python/models/inline_response2007.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/elabapi_python/models/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/elabapi_python/models/items_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/elabapi_python/models/items_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/elabapi_python/models/items_links_subid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/elabapi_python/models/items_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/elabapi_python/models/items_types_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/elabapi_python/models/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7620 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/elabapi_python/models/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7456 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/elabapi_python/models/revision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/elabapi_python/models/revisions_subid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/elabapi_python/models/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/elabapi_python/models/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/elabapi_python/models/steps_subid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/elabapi_python/models/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/elabapi_python/models/tags_subid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14842 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/elabapi_python/models/team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/elabapi_python/models/team_tags_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/elabapi_python/models/team_tags_body1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/elabapi_python/models/team_tags_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/elabapi_python/models/teamgroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/elabapi_python/models/teamgroup_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/elabapi_python/models/teamgroups_subid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/elabapi_python/models/teams_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/elabapi_python/models/todoitem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/elabapi_python/models/todolist_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/elabapi_python/models/todolist_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/elabapi_python/models/unfinished_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/elabapi_python/models/unfinished_steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/elabapi_python/models/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/elabapi_python/models/uploads_subid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/elabapi_python/models/uploads_subid_body1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11246 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/elabapi_python/models/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8175 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/elabapi_python/models/users_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/elabapi_python/models/users_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/elabapi_python/models/users_teams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13031 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/elabapi_python/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:25:26.393796 elabapi-python-0.3.0/elabapi_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-08-02 00:25:26.000000 elabapi-python-0.3.0/elabapi_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-08-02 00:25:26.000000 elabapi-python-0.3.0/elabapi_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 00:25:26.000000 elabapi-python-0.3.0/elabapi_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-02 00:25:26.000000 elabapi-python-0.3.0/elabapi_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-02 00:25:26.000000 elabapi-python-0.3.0/elabapi_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 00:25:26.469799 elabapi-python-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:25:26.469799 elabapi-python-0.3.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/test/test_api_keys_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-08-02 00:25:14.000000 elabapi-python-0.3.0/test/test_apikey.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-08-02 00:25:14.000000 elabapi-python-0.3.0/test/test_apikeys_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-08-02 00:25:14.000000 elabapi-python-0.3.0/test/test_comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/test/test_comments_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-08-02 00:25:14.000000 elabapi-python-0.3.0/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/test/test_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-08-02 00:25:14.000000 elabapi-python-0.3.0/test/test_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-08-02 00:25:14.000000 elabapi-python-0.3.0/test/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/test/test_events_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-02 00:25:14.000000 elabapi-python-0.3.0/test/test_events_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-08-02 00:25:14.000000 elabapi-python-0.3.0/test/test_events_id_body1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-08-02 00:25:14.000000 elabapi-python-0.3.0/test/test_eventsid_delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/test/test_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/test/test_experiment_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/test/test_experiments_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/test/test_experiments_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/test/test_experiments_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/test/test_experiments_links_subid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/test/test_experiments_templates_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/test/test_experiments_templates_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/test/test_experiments_templates_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/test/test_favorite_tags_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/test/test_favtags_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/test/test_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/test/test_id1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/test/test_id2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/test/test_id3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/test/test_id_comments_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/test/test_id_revisions_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/test/test_id_status_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/test/test_id_steps_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/test/test_id_tags_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/test/test_id_teamgroups_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/test/test_id_uploads_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/test/test_idp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/test/test_idps_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/test/test_idps_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/test/test_idps_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/test/test_info_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/test/test_inline_response200.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/test/test_inline_response2001.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/test/test_inline_response2002.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/test/test_inline_response2003.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/test/test_inline_response2004.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/test/test_inline_response2005.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/test/test_inline_response2006.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/test/test_inline_response2007.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-08-02 00:25:15.000000 elabapi-python-0.3.0/test/test_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/test/test_items_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/test/test_items_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/test/test_items_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/test/test_items_links_subid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/test/test_items_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/test/test_items_types_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/test/test_items_types_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/test/test_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/test/test_links_to_experiments_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/test/test_links_to_items_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/test/test_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/test/test_notifications_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/test/test_revision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/test/test_revisions_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/test/test_revisions_subid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/test/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/test/test_status_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/test/test_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/test/test_steps_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/test/test_steps_subid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/test/test_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/test/test_tags_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/test/test_tags_subid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/test/test_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/test/test_team_tags_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/test/test_team_tags_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/test/test_team_tags_body1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/test/test_team_tags_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/test/test_teamgroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/test/test_teamgroup_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/test/test_teamgroups_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/test/test_teamgroups_subid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/test/test_teams_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/test/test_teams_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/test/test_todoitem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/test/test_todolist_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/test/test_todolist_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/test/test_todolist_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/test/test_unfinished_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/test/test_unfinished_steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/test/test_unfinished_steps_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/test/test_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/test/test_uploads_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/test/test_uploads_subid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/test/test_uploads_subid_body1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/test/test_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-08-02 00:25:17.000000 elabapi-python-0.3.0/test/test_users_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/test/test_users_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/test/test_users_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-08-02 00:25:16.000000 elabapi-python-0.3.0/test/test_users_teams.py
```

### Comparing `elabapi-python-0.2.4/README.md` & `elabapi-python-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # elabapi-python
 This document describes all available endpoints and methods for eLabFTW's API version 2. 
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
 - API version: 2.0.0
-- Package version: 0.2.4
+- Package version: 0.3.0
 - Build package: io.swagger.codegen.v3.generators.python.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
@@ -135,14 +135,15 @@
 *FavoriteTagsApi* | [**post_favtags**](docs/FavoriteTagsApi.md#post_favtags) | **POST** /favtags | Add a tag as favorite.
 *FavoriteTagsApi* | [**read_favtags**](docs/FavoriteTagsApi.md#read_favtags) | **GET** /favtags | Read all favorite tags for the user.
 *IdpsApi* | [**delete_idp**](docs/IdpsApi.md#delete_idp) | **DELETE** /idps/{id} | Delete an idp.
 *IdpsApi* | [**patch_idp**](docs/IdpsApi.md#patch_idp) | **PATCH** /idps/{id} | Actions on an idp.
 *IdpsApi* | [**post_idp**](docs/IdpsApi.md#post_idp) | **POST** /idps | Create an idp.
 *IdpsApi* | [**read_idp**](docs/IdpsApi.md#read_idp) | **GET** /idps/{id} | Read an idp.
 *IdpsApi* | [**read_idps**](docs/IdpsApi.md#read_idps) | **GET** /idps | Read all IDPs.
+*InfoApi* | [**get_info**](docs/InfoApi.md#get_info) | **GET** /info | Get information about the instance.
 *ItemsApi* | [**delete_item**](docs/ItemsApi.md#delete_item) | **DELETE** /items/{id} | Delete an item.
 *ItemsApi* | [**get_item**](docs/ItemsApi.md#get_item) | **GET** /items/{id} | Read an item
 *ItemsApi* | [**patch_item**](docs/ItemsApi.md#patch_item) | **PATCH** /items/{id} | Modify an item
 *ItemsApi* | [**post_item**](docs/ItemsApi.md#post_item) | **POST** /items | Create an item
 *ItemsApi* | [**read_items**](docs/ItemsApi.md#read_items) | **GET** /items | Read all items that are accessible
 *ItemsTypesApi* | [**delete_items_type**](docs/ItemsTypesApi.md#delete_items_type) | **DELETE** /items_types/{id} | Delete an item type.
 *ItemsTypesApi* | [**get_items_type**](docs/ItemsTypesApi.md#get_items_type) | **GET** /items_types/{id} | Read an items type
@@ -155,24 +156,28 @@
 *LinksToItemsApi* | [**delete_entitiy_items_link**](docs/LinksToItemsApi.md#delete_entitiy_items_link) | **DELETE** /{entity_type}/{id}/items_links/{subid} | Delete an item link.
 *LinksToItemsApi* | [**post_entity_items_links**](docs/LinksToItemsApi.md#post_entity_items_links) | **POST** /{entity_type}/{id}/items_links/{subid} | Create or import a link.
 *LinksToItemsApi* | [**read_entity_items_links**](docs/LinksToItemsApi.md#read_entity_items_links) | **GET** /{entity_type}/{id}/items_links | Read all items links of that entity.
 *NotificationsApi* | [**delete_notifications**](docs/NotificationsApi.md#delete_notifications) | **DELETE** /users/{id}/notifications | Delete all notifications of the user.
 *NotificationsApi* | [**patch_notification**](docs/NotificationsApi.md#patch_notification) | **PATCH** /users/{id}/notifications/{subid} | Actions on a notification. Only changing &#x60;is_ack&#x60; column is possible. 
 *NotificationsApi* | [**read_notification**](docs/NotificationsApi.md#read_notification) | **GET** /users/{id}/notifications/{subid} | Read a notification.
 *NotificationsApi* | [**read_notifications**](docs/NotificationsApi.md#read_notifications) | **GET** /users/{id}/notifications | Read notifications of a user.
+*RevisionsApi* | [**patch_entity_revision**](docs/RevisionsApi.md#patch_entity_revision) | **PATCH** /{entity_type}/{id}/revisions/{subid} | Restore a revision.
+*RevisionsApi* | [**post_entity_revisions**](docs/RevisionsApi.md#post_entity_revisions) | **POST** /{entity_type}/{id}/revisions | Create a revision.
+*RevisionsApi* | [**read_entity_revision**](docs/RevisionsApi.md#read_entity_revision) | **GET** /{entity_type}/{id}/revisions/{subid} | Read a revision of that entity.
+*RevisionsApi* | [**read_entity_revisions**](docs/RevisionsApi.md#read_entity_revisions) | **GET** /{entity_type}/{id}/revisions | Read all revisions of that entity.
 *StatusApi* | [**delete_status**](docs/StatusApi.md#delete_status) | **DELETE** /teams/{id}/status/{subid} | Delete a status.
 *StatusApi* | [**patch_status**](docs/StatusApi.md#patch_status) | **PATCH** /teams/{id}/status/{subid} | Modify a status.
 *StatusApi* | [**post_team_one_status**](docs/StatusApi.md#post_team_one_status) | **POST** /teams/{id}/status | Create a new status.
 *StatusApi* | [**read_team_one_status**](docs/StatusApi.md#read_team_one_status) | **GET** /teams/{id}/status/{subid} | Read a status.
 *StatusApi* | [**read_team_status**](docs/StatusApi.md#read_team_status) | **GET** /teams/{id}/status | Read status of a team.
 *StepsApi* | [**delete_step**](docs/StepsApi.md#delete_step) | **DELETE** /{entity_type}/{id}/steps/{subid} | Delete a step.
 *StepsApi* | [**patch_step**](docs/StepsApi.md#patch_step) | **PATCH** /{entity_type}/{id}/steps/{subid} | Actions on a step. 
 *StepsApi* | [**post_step**](docs/StepsApi.md#post_step) | **POST** /{entity_type}/{id}/steps | Create a step.
 *StepsApi* | [**read_steps**](docs/StepsApi.md#read_steps) | **GET** /{entity_type}/{id}/steps | Read all steps of that entity.
-*TagsApi* | [**delete_tag**](docs/TagsApi.md#delete_tag) | **DELETE** /{entity_type}/{id}/tags/{subid} | Delete all tags.
+*TagsApi* | [**delete_tag**](docs/TagsApi.md#delete_tag) | **DELETE** /{entity_type}/{id}/tags | Delete all tags.
 *TagsApi* | [**patch_tag**](docs/TagsApi.md#patch_tag) | **PATCH** /{entity_type}/{id}/tags/{subid} | Actions on a tag (like removing it from the entity). 
 *TagsApi* | [**post_tag**](docs/TagsApi.md#post_tag) | **POST** /{entity_type}/{id}/tags | Create a tag.
 *TagsApi* | [**read_tag**](docs/TagsApi.md#read_tag) | **GET** /{entity_type}/{id}/tags/{subid} | Read a tag.
 *TagsApi* | [**read_tags**](docs/TagsApi.md#read_tags) | **GET** /{entity_type}/{id}/tags | Read all tags of that entity.
 *TeamTagsApi* | [**delete_team_tag**](docs/TeamTagsApi.md#delete_team_tag) | **DELETE** /team_tags/{id} | Delete a tag.
 *TeamTagsApi* | [**patch_tags**](docs/TeamTagsApi.md#patch_tags) | **PATCH** /team_tags | Actions on tags. 
 *TeamTagsApi* | [**patch_team_tag**](docs/TeamTagsApi.md#patch_team_tag) | **PATCH** /team_tags/{id} | Actions on a tag. 
@@ -191,15 +196,15 @@
 *TodolistApi* | [**delete_todoitem**](docs/TodolistApi.md#delete_todoitem) | **DELETE** /todolist/{id} | Delete a todoitem.
 *TodolistApi* | [**patch_todoitem**](docs/TodolistApi.md#patch_todoitem) | **PATCH** /todolist/{id} | Actions on a todoitem. 
 *TodolistApi* | [**post_todolist**](docs/TodolistApi.md#post_todolist) | **POST** /todolist | Create a todo item
 *TodolistApi* | [**read_todoitem**](docs/TodolistApi.md#read_todoitem) | **GET** /todolist/{id} | Read a todo entry.
 *TodolistApi* | [**read_todolist**](docs/TodolistApi.md#read_todolist) | **GET** /todolist | Read all todoitems.
 *UnfinishedStepsApi* | [**read_unfinished_steps**](docs/UnfinishedStepsApi.md#read_unfinished_steps) | **GET** /unfinished_steps | Read all unfinished steps.
 *UploadsApi* | [**delete_upload**](docs/UploadsApi.md#delete_upload) | **DELETE** /{entity_type}/{id}/uploads/{subid} | Delete an upload.
-*UploadsApi* | [**patch_upload**](docs/UploadsApi.md#patch_upload) | **PATCH** /{entity_type}/{id}/uploads/{subid} | Actions on an upload. 
+*UploadsApi* | [**patch_upload**](docs/UploadsApi.md#patch_upload) | **PATCH** /{entity_type}/{id}/uploads/{subid} | Modify attributes such as \&quot;real_name\&quot;, \&quot;comment\&quot; or \&quot;state\&quot; of an upload. 
 *UploadsApi* | [**post_upload**](docs/UploadsApi.md#post_upload) | **POST** /{entity_type}/{id}/uploads | Create an upload.
 *UploadsApi* | [**post_upload_replace**](docs/UploadsApi.md#post_upload_replace) | **POST** /{entity_type}/{id}/uploads/{subid} | Replace an existing uploaded file. The existing file will be archived and the new one will be added.
 *UploadsApi* | [**read_upload**](docs/UploadsApi.md#read_upload) | **GET** /{entity_type}/{id}/uploads/{subid} | Read an upload.
 *UploadsApi* | [**read_uploads**](docs/UploadsApi.md#read_uploads) | **GET** /{entity_type}/{id}/uploads | Read attached files of that entity.
 *UsersApi* | [**patch_user**](docs/UsersApi.md#patch_user) | **PATCH** /users/{id} | Modify a user.
 *UsersApi* | [**post_user**](docs/UsersApi.md#post_user) | **POST** /users | Create a new user.
 *UsersApi* | [**read_user**](docs/UsersApi.md#read_user) | **GET** /users/{id} | Read information of a user.
@@ -225,34 +230,41 @@
  - [ExperimentsTemplatesIdBody](docs/ExperimentsTemplatesIdBody.md)
  - [FavtagsBody](docs/FavtagsBody.md)
  - [Id](docs/Id.md)
  - [Id1](docs/Id1.md)
  - [Id2](docs/Id2.md)
  - [Id3](docs/Id3.md)
  - [IdCommentsBody](docs/IdCommentsBody.md)
+ - [IdRevisionsBody](docs/IdRevisionsBody.md)
  - [IdStatusBody](docs/IdStatusBody.md)
  - [IdStepsBody](docs/IdStepsBody.md)
  - [IdTagsBody](docs/IdTagsBody.md)
  - [IdTeamgroupsBody](docs/IdTeamgroupsBody.md)
  - [IdUploadsBody](docs/IdUploadsBody.md)
  - [Idp](docs/Idp.md)
  - [IdpsBody](docs/IdpsBody.md)
  - [IdpsIdBody](docs/IdpsIdBody.md)
  - [InlineResponse200](docs/InlineResponse200.md)
  - [InlineResponse2001](docs/InlineResponse2001.md)
  - [InlineResponse2002](docs/InlineResponse2002.md)
  - [InlineResponse2003](docs/InlineResponse2003.md)
+ - [InlineResponse2004](docs/InlineResponse2004.md)
+ - [InlineResponse2005](docs/InlineResponse2005.md)
+ - [InlineResponse2006](docs/InlineResponse2006.md)
+ - [InlineResponse2007](docs/InlineResponse2007.md)
  - [Item](docs/Item.md)
  - [ItemsBody](docs/ItemsBody.md)
  - [ItemsIdBody](docs/ItemsIdBody.md)
  - [ItemsLinksSubidBody](docs/ItemsLinksSubidBody.md)
  - [ItemsType](docs/ItemsType.md)
  - [ItemsTypesBody](docs/ItemsTypesBody.md)
  - [Link](docs/Link.md)
  - [Notification](docs/Notification.md)
+ - [Revision](docs/Revision.md)
+ - [RevisionsSubidBody](docs/RevisionsSubidBody.md)
  - [Status](docs/Status.md)
  - [Step](docs/Step.md)
  - [StepsSubidBody](docs/StepsSubidBody.md)
  - [Tag](docs/Tag.md)
  - [TagsSubidBody](docs/TagsSubidBody.md)
  - [Team](docs/Team.md)
  - [TeamTagsBody](docs/TeamTagsBody.md)
@@ -265,14 +277,15 @@
  - [Todoitem](docs/Todoitem.md)
  - [TodolistBody](docs/TodolistBody.md)
  - [TodolistIdBody](docs/TodolistIdBody.md)
  - [UnfinishedStep](docs/UnfinishedStep.md)
  - [UnfinishedSteps](docs/UnfinishedSteps.md)
  - [Upload](docs/Upload.md)
  - [UploadsSubidBody](docs/UploadsSubidBody.md)
+ - [UploadsSubidBody1](docs/UploadsSubidBody1.md)
  - [Users](docs/Users.md)
  - [UsersBody](docs/UsersBody.md)
  - [UsersIdBody](docs/UsersIdBody.md)
  - [UsersTeams](docs/UsersTeams.md)
 
 ## Documentation For Authorization
```

### Comparing `elabapi-python-0.2.4/elabapi_python/__init__.py` & `elabapi-python-0.3.0/elabapi_python/models/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,51 +1,23 @@
 # coding: utf-8
 
 # flake8: noqa
-
 """
     eLabFTW REST API v2 Documentation
 
     This document describes all available endpoints and methods for eLabFTW's API version 2.   # noqa: E501
 
     OpenAPI spec version: 2.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
-# import apis into sdk package
-from elabapi_python.api.api_keys_api import ApiKeysApi
-from elabapi_python.api.comments_api import CommentsApi
-from elabapi_python.api.config_api import ConfigApi
-from elabapi_python.api.events_api import EventsApi
-from elabapi_python.api.experiments_api import ExperimentsApi
-from elabapi_python.api.experiments_templates_api import ExperimentsTemplatesApi
-from elabapi_python.api.favorite_tags_api import FavoriteTagsApi
-from elabapi_python.api.idps_api import IdpsApi
-from elabapi_python.api.items_api import ItemsApi
-from elabapi_python.api.items_types_api import ItemsTypesApi
-from elabapi_python.api.links_to_experiments_api import LinksToExperimentsApi
-from elabapi_python.api.links_to_items_api import LinksToItemsApi
-from elabapi_python.api.notifications_api import NotificationsApi
-from elabapi_python.api.status_api import StatusApi
-from elabapi_python.api.steps_api import StepsApi
-from elabapi_python.api.tags_api import TagsApi
-from elabapi_python.api.team_tags_api import TeamTagsApi
-from elabapi_python.api.teamgroups_api import TeamgroupsApi
-from elabapi_python.api.teams_api import TeamsApi
-from elabapi_python.api.todolist_api import TodolistApi
-from elabapi_python.api.unfinished_steps_api import UnfinishedStepsApi
-from elabapi_python.api.uploads_api import UploadsApi
-from elabapi_python.api.users_api import UsersApi
-# import ApiClient
-from elabapi_python.api_client import ApiClient
-from elabapi_python.configuration import Configuration
-# import models into sdk package
+# import models into model package
 from elabapi_python.models.apikey import Apikey
 from elabapi_python.models.apikeys_body import ApikeysBody
 from elabapi_python.models.comment import Comment
 from elabapi_python.models.config import Config
 from elabapi_python.models.entity import Entity
 from elabapi_python.models.event import Event
 from elabapi_python.models.events_id_body import EventsIdBody
@@ -60,34 +32,41 @@
 from elabapi_python.models.experiments_templates_id_body import ExperimentsTemplatesIdBody
 from elabapi_python.models.favtags_body import FavtagsBody
 from elabapi_python.models.id import Id
 from elabapi_python.models.id1 import Id1
 from elabapi_python.models.id2 import Id2
 from elabapi_python.models.id3 import Id3
 from elabapi_python.models.id_comments_body import IdCommentsBody
+from elabapi_python.models.id_revisions_body import IdRevisionsBody
 from elabapi_python.models.id_status_body import IdStatusBody
 from elabapi_python.models.id_steps_body import IdStepsBody
 from elabapi_python.models.id_tags_body import IdTagsBody
 from elabapi_python.models.id_teamgroups_body import IdTeamgroupsBody
 from elabapi_python.models.id_uploads_body import IdUploadsBody
 from elabapi_python.models.idp import Idp
 from elabapi_python.models.idps_body import IdpsBody
 from elabapi_python.models.idps_id_body import IdpsIdBody
 from elabapi_python.models.inline_response200 import InlineResponse200
 from elabapi_python.models.inline_response2001 import InlineResponse2001
 from elabapi_python.models.inline_response2002 import InlineResponse2002
 from elabapi_python.models.inline_response2003 import InlineResponse2003
+from elabapi_python.models.inline_response2004 import InlineResponse2004
+from elabapi_python.models.inline_response2005 import InlineResponse2005
+from elabapi_python.models.inline_response2006 import InlineResponse2006
+from elabapi_python.models.inline_response2007 import InlineResponse2007
 from elabapi_python.models.item import Item
 from elabapi_python.models.items_body import ItemsBody
 from elabapi_python.models.items_id_body import ItemsIdBody
 from elabapi_python.models.items_links_subid_body import ItemsLinksSubidBody
 from elabapi_python.models.items_type import ItemsType
 from elabapi_python.models.items_types_body import ItemsTypesBody
 from elabapi_python.models.link import Link
 from elabapi_python.models.notification import Notification
+from elabapi_python.models.revision import Revision
+from elabapi_python.models.revisions_subid_body import RevisionsSubidBody
 from elabapi_python.models.status import Status
 from elabapi_python.models.step import Step
 from elabapi_python.models.steps_subid_body import StepsSubidBody
 from elabapi_python.models.tag import Tag
 from elabapi_python.models.tags_subid_body import TagsSubidBody
 from elabapi_python.models.team import Team
 from elabapi_python.models.team_tags_body import TeamTagsBody
@@ -100,11 +79,12 @@
 from elabapi_python.models.todoitem import Todoitem
 from elabapi_python.models.todolist_body import TodolistBody
 from elabapi_python.models.todolist_id_body import TodolistIdBody
 from elabapi_python.models.unfinished_step import UnfinishedStep
 from elabapi_python.models.unfinished_steps import UnfinishedSteps
 from elabapi_python.models.upload import Upload
 from elabapi_python.models.uploads_subid_body import UploadsSubidBody
+from elabapi_python.models.uploads_subid_body1 import UploadsSubidBody1
 from elabapi_python.models.users import Users
 from elabapi_python.models.users_body import UsersBody
 from elabapi_python.models.users_id_body import UsersIdBody
 from elabapi_python.models.users_teams import UsersTeams
```

### Comparing `elabapi-python-0.2.4/elabapi_python/api/__init__.py` & `elabapi-python-0.3.0/elabapi_python/api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,19 +7,21 @@
 from elabapi_python.api.comments_api import CommentsApi
 from elabapi_python.api.config_api import ConfigApi
 from elabapi_python.api.events_api import EventsApi
 from elabapi_python.api.experiments_api import ExperimentsApi
 from elabapi_python.api.experiments_templates_api import ExperimentsTemplatesApi
 from elabapi_python.api.favorite_tags_api import FavoriteTagsApi
 from elabapi_python.api.idps_api import IdpsApi
+from elabapi_python.api.info_api import InfoApi
 from elabapi_python.api.items_api import ItemsApi
 from elabapi_python.api.items_types_api import ItemsTypesApi
 from elabapi_python.api.links_to_experiments_api import LinksToExperimentsApi
 from elabapi_python.api.links_to_items_api import LinksToItemsApi
 from elabapi_python.api.notifications_api import NotificationsApi
+from elabapi_python.api.revisions_api import RevisionsApi
 from elabapi_python.api.status_api import StatusApi
 from elabapi_python.api.steps_api import StepsApi
 from elabapi_python.api.tags_api import TagsApi
 from elabapi_python.api.team_tags_api import TeamTagsApi
 from elabapi_python.api.teamgroups_api import TeamgroupsApi
 from elabapi_python.api.teams_api import TeamsApi
 from elabapi_python.api.todolist_api import TodolistApi
```

### Comparing `elabapi-python-0.2.4/elabapi_python/api/api_keys_api.py` & `elabapi-python-0.3.0/elabapi_python/api/api_keys_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/api/comments_api.py` & `elabapi-python-0.3.0/elabapi_python/api/comments_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/api/config_api.py` & `elabapi-python-0.3.0/elabapi_python/api/config_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/api/events_api.py` & `elabapi-python-0.3.0/elabapi_python/api/events_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/api/experiments_api.py` & `elabapi-python-0.3.0/elabapi_python/api/experiments_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -423,15 +423,15 @@
         >>> result = thread.get()
 
         :param async_req bool
         :param str q: Search for a term in title, body or elabid. 
         :param str extended: Extended search (advanced query). 
         :param int related: Look only for entries linked to this item id. 
         :param int cat: The status id of the experiments. 
-        :param list tags: An array of tags for filtering results containing all of these tags. 
+        :param list[str] tags: An array of tags for filtering results containing all of these tags. 
         :param int limit: Limit the number of results. 
         :param int offset: Skip a number of results. Use with limit to work the pagination. 
         :param list[str] metakey: Key search in metadata. 
         :param list[str] metavalue: Value search in metadata. 
         :return: list[Experiment]
                  If the method is called asynchronously,
                  returns the request thread.
@@ -452,15 +452,15 @@
         >>> result = thread.get()
 
         :param async_req bool
         :param str q: Search for a term in title, body or elabid. 
         :param str extended: Extended search (advanced query). 
         :param int related: Look only for entries linked to this item id. 
         :param int cat: The status id of the experiments. 
-        :param list tags: An array of tags for filtering results containing all of these tags. 
+        :param list[str] tags: An array of tags for filtering results containing all of these tags. 
         :param int limit: Limit the number of results. 
         :param int offset: Skip a number of results. Use with limit to work the pagination. 
         :param list[str] metakey: Key search in metadata. 
         :param list[str] metavalue: Value search in metadata. 
         :return: list[Experiment]
                  If the method is called asynchronously,
                  returns the request thread.
@@ -492,15 +492,16 @@
         if 'extended' in params:
             query_params.append(('extended', params['extended']))  # noqa: E501
         if 'related' in params:
             query_params.append(('related', params['related']))  # noqa: E501
         if 'cat' in params:
             query_params.append(('cat', params['cat']))  # noqa: E501
         if 'tags' in params:
-            query_params.append(('tags', params['tags']))  # noqa: E501
+            query_params.append(('tags[]', params['tags']))  # noqa: E501
+            collection_formats['tags[]'] = 'multi'  # noqa: E501
         if 'limit' in params:
             query_params.append(('limit', params['limit']))  # noqa: E501
         if 'offset' in params:
             query_params.append(('offset', params['offset']))  # noqa: E501
         if 'metakey' in params:
             query_params.append(('metakey[]', params['metakey']))  # noqa: E501
             collection_formats['metakey[]'] = 'multi'  # noqa: E501
```

### Comparing `elabapi-python-0.2.4/elabapi_python/api/experiments_templates_api.py` & `elabapi-python-0.3.0/elabapi_python/api/experiments_templates_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/api/favorite_tags_api.py` & `elabapi-python-0.3.0/elabapi_python/api/favorite_tags_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -219,15 +219,15 @@
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.read_favtags(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :return: InlineResponse200
+        :return: InlineResponse2001
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.read_favtags_with_http_info(**kwargs)  # noqa: E501
         else:
@@ -239,15 +239,15 @@
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.read_favtags_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :return: InlineResponse200
+        :return: InlineResponse2001
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = []  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
@@ -287,14 +287,14 @@
             '/favtags', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='InlineResponse200',  # noqa: E501
+            response_type='InlineResponse2001',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
```

### Comparing `elabapi-python-0.2.4/elabapi_python/api/idps_api.py` & `elabapi-python-0.3.0/elabapi_python/api/idps_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/api/items_api.py` & `elabapi-python-0.3.0/elabapi_python/api/items_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -422,15 +422,15 @@
         >>> thread = api.read_items(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str q: Search for a term in title, body or elabid. 
         :param str extended: Extended search (advanced query). 
         :param int cat: The category id of the items. 
-        :param list tags: An array of tags for filtering results containing all of these tags. 
+        :param list[str] tags: An array of tags for filtering results containing all of these tags. 
         :param int limit: Limit the number of results. 
         :param int offset: Skip a number of results. Use with limit to work the pagination. 
         :param list[str] metakey: Key search in metadata. 
         :param list[str] metavalue: Value search in metadata. 
         :return: list[Item]
                  If the method is called asynchronously,
                  returns the request thread.
@@ -450,15 +450,15 @@
         >>> thread = api.read_items_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str q: Search for a term in title, body or elabid. 
         :param str extended: Extended search (advanced query). 
         :param int cat: The category id of the items. 
-        :param list tags: An array of tags for filtering results containing all of these tags. 
+        :param list[str] tags: An array of tags for filtering results containing all of these tags. 
         :param int limit: Limit the number of results. 
         :param int offset: Skip a number of results. Use with limit to work the pagination. 
         :param list[str] metakey: Key search in metadata. 
         :param list[str] metavalue: Value search in metadata. 
         :return: list[Item]
                  If the method is called asynchronously,
                  returns the request thread.
@@ -488,15 +488,16 @@
         if 'q' in params:
             query_params.append(('q', params['q']))  # noqa: E501
         if 'extended' in params:
             query_params.append(('extended', params['extended']))  # noqa: E501
         if 'cat' in params:
             query_params.append(('cat', params['cat']))  # noqa: E501
         if 'tags' in params:
-            query_params.append(('tags', params['tags']))  # noqa: E501
+            query_params.append(('tags[]', params['tags']))  # noqa: E501
+            collection_formats['tags[]'] = 'multi'  # noqa: E501
         if 'limit' in params:
             query_params.append(('limit', params['limit']))  # noqa: E501
         if 'offset' in params:
             query_params.append(('offset', params['offset']))  # noqa: E501
         if 'metakey' in params:
             query_params.append(('metakey[]', params['metakey']))  # noqa: E501
             collection_formats['metakey[]'] = 'multi'  # noqa: E501
```

### Comparing `elabapi-python-0.2.4/elabapi_python/api/items_types_api.py` & `elabapi-python-0.3.0/elabapi_python/api/items_types_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/api/links_to_experiments_api.py` & `elabapi-python-0.3.0/elabapi_python/api/links_to_experiments_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/api/links_to_items_api.py` & `elabapi-python-0.3.0/elabapi_python/api/links_to_items_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/api/notifications_api.py` & `elabapi-python-0.3.0/elabapi_python/api/notifications_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -335,15 +335,15 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.read_notifications(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param Id2 id: ID of the user or `me`. (required)
-        :return: InlineResponse2003
+        :return: InlineResponse2006
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.read_notifications_with_http_info(id, **kwargs)  # noqa: E501
         else:
@@ -356,15 +356,15 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.read_notifications_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param Id2 id: ID of the user or `me`. (required)
-        :return: InlineResponse2003
+        :return: InlineResponse2006
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['id']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
@@ -410,14 +410,14 @@
             '/users/{id}/notifications', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='InlineResponse2003',  # noqa: E501
+            response_type='InlineResponse2006',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
```

### Comparing `elabapi-python-0.2.4/elabapi_python/api/status_api.py` & `elabapi-python-0.3.0/elabapi_python/api/status_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/api/steps_api.py` & `elabapi-python-0.3.0/elabapi_python/api/steps_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/api/tags_api.py` & `elabapi-python-0.3.0/elabapi_python/api/tags_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,57 +28,55 @@
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def delete_tag(self, entity_type, id, subid, **kwargs):  # noqa: E501
+    def delete_tag(self, entity_type, id, **kwargs):  # noqa: E501
         """Delete all tags.  # noqa: E501
 
         All the tags from that entity get removed.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.delete_tag(entity_type, id, subid, async_req=True)
+        >>> thread = api.delete_tag(entity_type, id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str entity_type: Entity type (required)
         :param int id: ID of the entity (required)
-        :param int subid: ID of the tag (required)
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.delete_tag_with_http_info(entity_type, id, subid, **kwargs)  # noqa: E501
+            return self.delete_tag_with_http_info(entity_type, id, **kwargs)  # noqa: E501
         else:
-            (data) = self.delete_tag_with_http_info(entity_type, id, subid, **kwargs)  # noqa: E501
+            (data) = self.delete_tag_with_http_info(entity_type, id, **kwargs)  # noqa: E501
             return data
 
-    def delete_tag_with_http_info(self, entity_type, id, subid, **kwargs):  # noqa: E501
+    def delete_tag_with_http_info(self, entity_type, id, **kwargs):  # noqa: E501
         """Delete all tags.  # noqa: E501
 
         All the tags from that entity get removed.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.delete_tag_with_http_info(entity_type, id, subid, async_req=True)
+        >>> thread = api.delete_tag_with_http_info(entity_type, id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str entity_type: Entity type (required)
         :param int id: ID of the entity (required)
-        :param int subid: ID of the tag (required)
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['entity_type', 'id', 'subid']  # noqa: E501
+        all_params = ['entity_type', 'id']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
@@ -93,28 +91,22 @@
         if ('entity_type' not in params or
                 params['entity_type'] is None):
             raise ValueError("Missing the required parameter `entity_type` when calling `delete_tag`")  # noqa: E501
         # verify the required parameter 'id' is set
         if ('id' not in params or
                 params['id'] is None):
             raise ValueError("Missing the required parameter `id` when calling `delete_tag`")  # noqa: E501
-        # verify the required parameter 'subid' is set
-        if ('subid' not in params or
-                params['subid'] is None):
-            raise ValueError("Missing the required parameter `subid` when calling `delete_tag`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'entity_type' in params:
             path_params['entity_type'] = params['entity_type']  # noqa: E501
         if 'id' in params:
             path_params['id'] = params['id']  # noqa: E501
-        if 'subid' in params:
-            path_params['subid'] = params['subid']  # noqa: E501
 
         query_params = []
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
@@ -124,15 +116,15 @@
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['token']  # noqa: E501
 
         return self.api_client.call_api(
-            '/{entity_type}/{id}/tags/{subid}', 'DELETE',
+            '/{entity_type}/{id}/tags', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type=None,  # noqa: E501
```

### Comparing `elabapi-python-0.2.4/elabapi_python/api/team_tags_api.py` & `elabapi-python-0.3.0/elabapi_python/api/team_tags_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -414,15 +414,15 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.read_team_tag(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param int id: ID of the tag. (required)
-        :return: InlineResponse2001
+        :return: InlineResponse2003
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.read_team_tag_with_http_info(id, **kwargs)  # noqa: E501
         else:
@@ -435,15 +435,15 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.read_team_tag_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param int id: ID of the tag. (required)
-        :return: InlineResponse2001
+        :return: InlineResponse2003
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['id']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
@@ -489,15 +489,15 @@
             '/team_tags/{id}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='InlineResponse2001',  # noqa: E501
+            response_type='InlineResponse2003',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
@@ -506,15 +506,15 @@
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.read_team_tags(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :return: InlineResponse2001
+        :return: InlineResponse2002
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.read_team_tags_with_http_info(**kwargs)  # noqa: E501
         else:
@@ -526,15 +526,15 @@
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.read_team_tags_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :return: InlineResponse2001
+        :return: InlineResponse2002
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = []  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
@@ -574,14 +574,14 @@
             '/team_tags', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='InlineResponse2001',  # noqa: E501
+            response_type='InlineResponse2002',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
```

### Comparing `elabapi-python-0.2.4/elabapi_python/api/teamgroups_api.py` & `elabapi-python-0.3.0/elabapi_python/api/teamgroups_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -439,15 +439,15 @@
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.read_teamgroup(id, subid, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param int id: ID of the team. (required)
         :param int subid: ID of the teamgroup. (required)
-        :return: InlineResponse2002
+        :return: InlineResponse2004
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.read_teamgroup_with_http_info(id, subid, **kwargs)  # noqa: E501
         else:
@@ -461,15 +461,15 @@
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.read_teamgroup_with_http_info(id, subid, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param int id: ID of the team. (required)
         :param int subid: ID of the teamgroup. (required)
-        :return: InlineResponse2002
+        :return: InlineResponse2004
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['id', 'subid']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
@@ -521,14 +521,14 @@
             '/teams/{id}/teamgroups/{subid}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='InlineResponse2002',  # noqa: E501
+            response_type='InlineResponse2004',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
```

### Comparing `elabapi-python-0.2.4/elabapi_python/api/teams_api.py` & `elabapi-python-0.3.0/elabapi_python/api/teams_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/api/todolist_api.py` & `elabapi-python-0.3.0/elabapi_python/api/todolist_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/api/unfinished_steps_api.py` & `elabapi-python-0.3.0/elabapi_python/api/unfinished_steps_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/api/uploads_api.py` & `elabapi-python-0.3.0/elabapi_python/api/uploads_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,50 +140,50 @@
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def patch_upload(self, entity_type, id, subid, **kwargs):  # noqa: E501
-        """Actions on an upload.   # noqa: E501
+        """Modify attributes such as \"real_name\", \"comment\" or \"state\" of an upload.   # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.patch_upload(entity_type, id, subid, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str entity_type: Entity type (required)
         :param int id: ID of the entity (required)
         :param int subid: ID of the upload (required)
-        :param UploadsSubidBody body: Parameters for modifying an upload.
+        :param UploadsSubidBody1 body: Parameters for modifying an upload attributes.
         :return: Upload
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.patch_upload_with_http_info(entity_type, id, subid, **kwargs)  # noqa: E501
         else:
             (data) = self.patch_upload_with_http_info(entity_type, id, subid, **kwargs)  # noqa: E501
             return data
 
     def patch_upload_with_http_info(self, entity_type, id, subid, **kwargs):  # noqa: E501
-        """Actions on an upload.   # noqa: E501
+        """Modify attributes such as \"real_name\", \"comment\" or \"state\" of an upload.   # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.patch_upload_with_http_info(entity_type, id, subid, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str entity_type: Entity type (required)
         :param int id: ID of the entity (required)
         :param int subid: ID of the upload (required)
-        :param UploadsSubidBody body: Parameters for modifying an upload.
+        :param UploadsSubidBody1 body: Parameters for modifying an upload attributes.
         :return: Upload
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['entity_type', 'id', 'subid', 'body']  # noqa: E501
         all_params.append('async_req')
@@ -377,15 +377,16 @@
         >>> thread = api.post_upload_replace(entity_type, id, subid, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str entity_type: Entity type (required)
         :param int id: ID of the entity (required)
         :param int subid: ID of the upload (required)
-        :param Object body: Parameters for replacing an upload.
+        :param str file:
+        :param str comment:
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.post_upload_replace_with_http_info(entity_type, id, subid, **kwargs)  # noqa: E501
@@ -401,21 +402,22 @@
         >>> thread = api.post_upload_replace_with_http_info(entity_type, id, subid, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str entity_type: Entity type (required)
         :param int id: ID of the entity (required)
         :param int subid: ID of the upload (required)
-        :param Object body: Parameters for replacing an upload.
+        :param str file:
+        :param str comment:
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['entity_type', 'id', 'subid', 'body']  # noqa: E501
+        all_params = ['entity_type', 'id', 'subid', 'file', 'comment']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
@@ -451,21 +453,23 @@
 
         query_params = []
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
+        if 'file' in params:
+            local_var_files['file'] = params['file']  # noqa: E501
+        if 'comment' in params:
+            form_params.append(('comment', params['comment']))  # noqa: E501
 
         body_params = None
-        if 'body' in params:
-            body_params = params['body']
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
-            ['application/octet-stream'])  # noqa: E501
+            ['multipart/form-data'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['token']  # noqa: E501
 
         return self.api_client.call_api(
             '/{entity_type}/{id}/uploads/{subid}', 'POST',
             path_params,
```

### Comparing `elabapi-python-0.2.4/elabapi_python/api/users_api.py` & `elabapi-python-0.3.0/elabapi_python/api/users_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -327,15 +327,15 @@
         If Sysadmin all users will be shown. If Admin only the users from the team. Normal users will be shown an error.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.read_users(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :return: list[Users]
+        :return: list[InlineResponse2005]
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.read_users_with_http_info(**kwargs)  # noqa: E501
         else:
@@ -348,15 +348,15 @@
         If Sysadmin all users will be shown. If Admin only the users from the team. Normal users will be shown an error.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.read_users_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :return: list[Users]
+        :return: list[InlineResponse2005]
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = []  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
@@ -396,14 +396,14 @@
             '/users', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='list[Users]',  # noqa: E501
+            response_type='list[InlineResponse2005]',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
```

### Comparing `elabapi-python-0.2.4/elabapi_python/api_client.py` & `elabapi-python-0.3.0/elabapi_python/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         self.pool = ThreadPool()
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'Swagger-Codegen/0.2.4/python'
+        self.user_agent = 'Swagger-Codegen/0.3.0/python'
 
     def __del__(self):
         self.pool.close()
         self.pool.join()
 
     @property
     def user_agent(self):
```

### Comparing `elabapi-python-0.2.4/elabapi_python/configuration.py` & `elabapi-python-0.3.0/elabapi_python/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,9 +243,9 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 2.0.0\n"\
-               "SDK Package Version: 0.2.4".\
+               "SDK Package Version: 0.3.0".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `elabapi-python-0.2.4/elabapi_python/models/apikey.py` & `elabapi-python-0.3.0/elabapi_python/models/apikey.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'id': 'int',
         'name': 'str',
-        'created_at': 'str',
+        'created_at': 'datetime',
         'hash': 'str',
         'can_write': 'int'
     }
 
     attribute_map = {
         'id': 'id',
         'name': 'name',
@@ -106,25 +106,25 @@
 
     @property
     def created_at(self):
         """Gets the created_at of this Apikey.  # noqa: E501
 
 
         :return: The created_at of this Apikey.  # noqa: E501
-        :rtype: str
+        :rtype: datetime
         """
         return self._created_at
 
     @created_at.setter
     def created_at(self, created_at):
         """Sets the created_at of this Apikey.
 
 
         :param created_at: The created_at of this Apikey.  # noqa: E501
-        :type: str
+        :type: datetime
         """
 
         self._created_at = created_at
 
     @property
     def hash(self):
         """Gets the hash of this Apikey.  # noqa: E501
```

### Comparing `elabapi-python-0.2.4/elabapi_python/models/apikeys_body.py` & `elabapi-python-0.3.0/elabapi_python/models/apikeys_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/models/comment.py` & `elabapi-python-0.3.0/elabapi_python/models/comment.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,19 +25,19 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'id': 'int',
-        'created_at': 'str',
+        'created_at': 'datetime',
         'item_id': 'int',
         'comment': 'str',
         'userid': 'int',
-        'modified_at': 'str',
+        'modified_at': 'datetime',
         'fullname': 'str',
         'firstname': 'str',
         'lastname': 'str',
         'orcid': 'str'
     }
 
     attribute_map = {
@@ -110,25 +110,25 @@
 
     @property
     def created_at(self):
         """Gets the created_at of this Comment.  # noqa: E501
 
 
         :return: The created_at of this Comment.  # noqa: E501
-        :rtype: str
+        :rtype: datetime
         """
         return self._created_at
 
     @created_at.setter
     def created_at(self, created_at):
         """Sets the created_at of this Comment.
 
 
         :param created_at: The created_at of this Comment.  # noqa: E501
-        :type: str
+        :type: datetime
         """
 
         self._created_at = created_at
 
     @property
     def item_id(self):
         """Gets the item_id of this Comment.  # noqa: E501
@@ -194,25 +194,25 @@
 
     @property
     def modified_at(self):
         """Gets the modified_at of this Comment.  # noqa: E501
 
 
         :return: The modified_at of this Comment.  # noqa: E501
-        :rtype: str
+        :rtype: datetime
         """
         return self._modified_at
 
     @modified_at.setter
     def modified_at(self, modified_at):
         """Sets the modified_at of this Comment.
 
 
         :param modified_at: The modified_at of this Comment.  # noqa: E501
-        :type: str
+        :type: datetime
         """
 
         self._modified_at = modified_at
 
     @property
     def fullname(self):
         """Gets the fullname of this Comment.  # noqa: E501
```

### Comparing `elabapi-python-0.2.4/elabapi_python/models/config.py` & `elabapi-python-0.3.0/elabapi_python/models/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
         'admins_create_users_remote_dir': 'str',
         'admin_validate': 'str',
         'announcement': 'str',
         'anon_users': 'str',
         'autologout_time': 'str',
         'blox_anon': 'str',
         'blox_enabled': 'str',
+        'cookie_validity_time': 'int',
         'debug': 'str',
         'deletable_xp': 'str',
         'email_domain': 'str',
         'extauth_email': 'str',
         'extauth_firstname': 'str',
         'extauth_lastname': 'str',
         'extauth_remote_user': 'str',
@@ -128,14 +129,15 @@
         'admins_create_users_remote_dir': 'admins_create_users_remote_dir',
         'admin_validate': 'admin_validate',
         'announcement': 'announcement',
         'anon_users': 'anon_users',
         'autologout_time': 'autologout_time',
         'blox_anon': 'blox_anon',
         'blox_enabled': 'blox_enabled',
+        'cookie_validity_time': 'cookie_validity_time',
         'debug': 'debug',
         'deletable_xp': 'deletable_xp',
         'email_domain': 'email_domain',
         'extauth_email': 'extauth_email',
         'extauth_firstname': 'extauth_firstname',
         'extauth_lastname': 'extauth_lastname',
         'extauth_remote_user': 'extauth_remote_user',
@@ -215,24 +217,25 @@
         'ts_limit': 'ts_limit',
         'ts_login': 'ts_login',
         'ts_password': 'ts_password',
         'ts_url': 'ts_url',
         'uploads_storage': 'uploads_storage'
     }
 
-    def __init__(self, admins_create_users=None, admins_create_users_remote_dir=None, admin_validate=None, announcement=None, anon_users=None, autologout_time=None, blox_anon=None, blox_enabled=None, debug=None, deletable_xp=None, email_domain=None, extauth_email=None, extauth_firstname=None, extauth_lastname=None, extauth_remote_user=None, extauth_teams=None, lang=None, ldap_base_dn=None, ldap_search_attr=None, ldap_email=None, ldap_firstname=None, ldap_host=None, ldap_lastname=None, ldap_password=None, ldap_port=None, ldap_team=None, ldap_toggle=None, ldap_use_tls=None, ldap_username=None, local_login=None, local_register=None, login_announcement=None, login_tries=None, logout_url=None, mail_from=None, max_revisions=None, min_days_revisions=None, min_delta_revisions=None, open_science=None, open_team=None, privacy_policy=None, proxy=None, remote_dir_config=None, remote_dir_service=None, s3_bucket_name=None, s3_endpoint=None, s3_path_prefix=None, s3_region=None, s3_verify_cert=None, saml_acs_binding=None, saml_allowrepeatattributename=None, saml_authnrequestssigned=None, saml_baseurl=None, saml_debug=None, saml_entityid=None, saml_logoutrequestsigned=None, saml_logoutresponsesigned=None, saml_lowercaseurlencoding=None, saml_nameidencrypted=None, saml_nameidformat=None, saml_privatekey=None, saml_relaxdestinationvalidation=None, saml_signmetadata=None, saml_slo_binding=None, saml_strict=None, saml_sync_teams=None, saml_team_create=None, saml_team_default=None, saml_toggle=None, saml_user_default=None, saml_wantassertionsencrypted=None, saml_wantassertionssigned=None, saml_wantmessagessigned=None, saml_wantnameid=None, saml_wantnameidencrypted=None, saml_wantxmlvalidation=None, saml_x509=None, saml_x509_new=None, schema=None, smtp_address=None, smtp_encryption=None, smtp_password=None, smtp_port=None, smtp_username=None, support_url=None, ts_authority=None, ts_cert=None, ts_hash=None, ts_limit=None, ts_login=None, ts_password=None, ts_url=None, uploads_storage=None):  # noqa: E501
+    def __init__(self, admins_create_users=None, admins_create_users_remote_dir=None, admin_validate=None, announcement=None, anon_users=None, autologout_time=None, blox_anon=None, blox_enabled=None, cookie_validity_time=None, debug=None, deletable_xp=None, email_domain=None, extauth_email=None, extauth_firstname=None, extauth_lastname=None, extauth_remote_user=None, extauth_teams=None, lang=None, ldap_base_dn=None, ldap_search_attr=None, ldap_email=None, ldap_firstname=None, ldap_host=None, ldap_lastname=None, ldap_password=None, ldap_port=None, ldap_team=None, ldap_toggle=None, ldap_use_tls=None, ldap_username=None, local_login=None, local_register=None, login_announcement=None, login_tries=None, logout_url=None, mail_from=None, max_revisions=None, min_days_revisions=None, min_delta_revisions=None, open_science=None, open_team=None, privacy_policy=None, proxy=None, remote_dir_config=None, remote_dir_service=None, s3_bucket_name=None, s3_endpoint=None, s3_path_prefix=None, s3_region=None, s3_verify_cert=None, saml_acs_binding=None, saml_allowrepeatattributename=None, saml_authnrequestssigned=None, saml_baseurl=None, saml_debug=None, saml_entityid=None, saml_logoutrequestsigned=None, saml_logoutresponsesigned=None, saml_lowercaseurlencoding=None, saml_nameidencrypted=None, saml_nameidformat=None, saml_privatekey=None, saml_relaxdestinationvalidation=None, saml_signmetadata=None, saml_slo_binding=None, saml_strict=None, saml_sync_teams=None, saml_team_create=None, saml_team_default=None, saml_toggle=None, saml_user_default=None, saml_wantassertionsencrypted=None, saml_wantassertionssigned=None, saml_wantmessagessigned=None, saml_wantnameid=None, saml_wantnameidencrypted=None, saml_wantxmlvalidation=None, saml_x509=None, saml_x509_new=None, schema=None, smtp_address=None, smtp_encryption=None, smtp_password=None, smtp_port=None, smtp_username=None, support_url=None, ts_authority=None, ts_cert=None, ts_hash=None, ts_limit=None, ts_login=None, ts_password=None, ts_url=None, uploads_storage=None):  # noqa: E501
         """Config - a model defined in Swagger"""  # noqa: E501
         self._admins_create_users = None
         self._admins_create_users_remote_dir = None
         self._admin_validate = None
         self._announcement = None
         self._anon_users = None
         self._autologout_time = None
         self._blox_anon = None
         self._blox_enabled = None
+        self._cookie_validity_time = None
         self._debug = None
         self._deletable_xp = None
         self._email_domain = None
         self._extauth_email = None
         self._extauth_firstname = None
         self._extauth_lastname = None
         self._extauth_remote_user = None
@@ -327,14 +330,16 @@
             self.anon_users = anon_users
         if autologout_time is not None:
             self.autologout_time = autologout_time
         if blox_anon is not None:
             self.blox_anon = blox_anon
         if blox_enabled is not None:
             self.blox_enabled = blox_enabled
+        if cookie_validity_time is not None:
+            self.cookie_validity_time = cookie_validity_time
         if debug is not None:
             self.debug = debug
         if deletable_xp is not None:
             self.deletable_xp = deletable_xp
         if email_domain is not None:
             self.email_domain = email_domain
         if extauth_email is not None:
@@ -667,14 +672,35 @@
         :param blox_enabled: The blox_enabled of this Config.  # noqa: E501
         :type: str
         """
 
         self._blox_enabled = blox_enabled
 
     @property
+    def cookie_validity_time(self):
+        """Gets the cookie_validity_time of this Config.  # noqa: E501
+
+
+        :return: The cookie_validity_time of this Config.  # noqa: E501
+        :rtype: int
+        """
+        return self._cookie_validity_time
+
+    @cookie_validity_time.setter
+    def cookie_validity_time(self, cookie_validity_time):
+        """Sets the cookie_validity_time of this Config.
+
+
+        :param cookie_validity_time: The cookie_validity_time of this Config.  # noqa: E501
+        :type: int
+        """
+
+        self._cookie_validity_time = cookie_validity_time
+
+    @property
     def debug(self):
         """Gets the debug of this Config.  # noqa: E501
 
 
         :return: The debug of this Config.  # noqa: E501
         :rtype: str
         """
```

### Comparing `elabapi-python-0.2.4/elabapi_python/models/entity.py` & `elabapi-python-0.3.0/elabapi_python/models/entity.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,33 +33,30 @@
         'canread': 'str',
         'canwrite': 'str',
         'category': 'str',
         'category_id': 'int',
         'color': 'str',
         'comments': 'list[Comment]',
         'content_type': 'int',
-        'created_at': 'str',
+        'created_at': 'datetime',
         '_date': 'str',
         'elabid': 'str',
-        'events_id': 'str',
-        'events_item_id': 'str',
         'firstname': 'str',
         'fullname': 'str',
         'has_attachement': 'int',
         'has_comment': 'int',
         'id': 'int',
-        'is_bound': 'str',
         'lastchangeby': 'int',
         'lastname': 'str',
         'links': 'list[Link]',
         'locked': 'int',
         'lockedby': 'int',
         'lockedwhen': 'str',
         'metadata': 'str',
-        'modified_at': 'str',
+        'modified_at': 'datetime',
         'next_step': 'str',
         'orcid': 'str',
         'page': 'str',
         'rating': 'int',
         'recent_comment': 'str',
         'sharelink': 'str',
         'state': 'int',
@@ -85,22 +82,19 @@
         'category_id': 'category_id',
         'color': 'color',
         'comments': 'comments',
         'content_type': 'content_type',
         'created_at': 'created_at',
         '_date': 'date',
         'elabid': 'elabid',
-        'events_id': 'events_id',
-        'events_item_id': 'events_item_id',
         'firstname': 'firstname',
         'fullname': 'fullname',
         'has_attachement': 'has_attachement',
         'has_comment': 'has_comment',
         'id': 'id',
-        'is_bound': 'is_bound',
         'lastchangeby': 'lastchangeby',
         'lastname': 'lastname',
         'links': 'links',
         'locked': 'locked',
         'lockedby': 'lockedby',
         'lockedwhen': 'lockedwhen',
         'metadata': 'metadata',
@@ -121,36 +115,33 @@
         'title': 'title',
         'type': 'type',
         'up_item_id': 'up_item_id',
         'uploads': 'uploads',
         'userid': 'userid'
     }
 
-    def __init__(self, body=None, body_html=None, canread=None, canwrite=None, category=None, category_id=None, color=None, comments=None, content_type=None, created_at=None, _date=None, elabid=None, events_id=None, events_item_id=None, firstname=None, fullname=None, has_attachement=None, has_comment=None, id=None, is_bound=None, lastchangeby=None, lastname=None, links=None, locked=None, lockedby=None, lockedwhen=None, metadata=None, modified_at=None, next_step=None, orcid=None, page=None, rating=None, recent_comment=None, sharelink=None, state=None, steps=None, tags=None, tags_id=None, timestamped=None, timestampedby=None, timestamped_at=None, title=None, type=None, up_item_id=None, uploads=None, userid=None):  # noqa: E501
+    def __init__(self, body=None, body_html=None, canread=None, canwrite=None, category=None, category_id=None, color=None, comments=None, content_type=None, created_at=None, _date=None, elabid=None, firstname=None, fullname=None, has_attachement=None, has_comment=None, id=None, lastchangeby=None, lastname=None, links=None, locked=None, lockedby=None, lockedwhen=None, metadata=None, modified_at=None, next_step=None, orcid=None, page=None, rating=None, recent_comment=None, sharelink=None, state=None, steps=None, tags=None, tags_id=None, timestamped=None, timestampedby=None, timestamped_at=None, title=None, type=None, up_item_id=None, uploads=None, userid=None):  # noqa: E501
         """Entity - a model defined in Swagger"""  # noqa: E501
         self._body = None
         self._body_html = None
         self._canread = None
         self._canwrite = None
         self._category = None
         self._category_id = None
         self._color = None
         self._comments = None
         self._content_type = None
         self._created_at = None
         self.__date = None
         self._elabid = None
-        self._events_id = None
-        self._events_item_id = None
         self._firstname = None
         self._fullname = None
         self._has_attachement = None
         self._has_comment = None
         self._id = None
-        self._is_bound = None
         self._lastchangeby = None
         self._lastname = None
         self._links = None
         self._locked = None
         self._lockedby = None
         self._lockedwhen = None
         self._metadata = None
@@ -194,30 +185,24 @@
             self.content_type = content_type
         if created_at is not None:
             self.created_at = created_at
         if _date is not None:
             self._date = _date
         if elabid is not None:
             self.elabid = elabid
-        if events_id is not None:
-            self.events_id = events_id
-        if events_item_id is not None:
-            self.events_item_id = events_item_id
         if firstname is not None:
             self.firstname = firstname
         if fullname is not None:
             self.fullname = fullname
         if has_attachement is not None:
             self.has_attachement = has_attachement
         if has_comment is not None:
             self.has_comment = has_comment
         if id is not None:
             self.id = id
-        if is_bound is not None:
-            self.is_bound = is_bound
         if lastchangeby is not None:
             self.lastchangeby = lastchangeby
         if lastname is not None:
             self.lastname = lastname
         if links is not None:
             self.links = links
         if locked is not None:
@@ -460,25 +445,25 @@
 
     @property
     def created_at(self):
         """Gets the created_at of this Entity.  # noqa: E501
 
 
         :return: The created_at of this Entity.  # noqa: E501
-        :rtype: str
+        :rtype: datetime
         """
         return self._created_at
 
     @created_at.setter
     def created_at(self, created_at):
         """Sets the created_at of this Entity.
 
 
         :param created_at: The created_at of this Entity.  # noqa: E501
-        :type: str
+        :type: datetime
         """
 
         self._created_at = created_at
 
     @property
     def _date(self):
         """Gets the _date of this Entity.  # noqa: E501
@@ -518,56 +503,14 @@
         :param elabid: The elabid of this Entity.  # noqa: E501
         :type: str
         """
 
         self._elabid = elabid
 
     @property
-    def events_id(self):
-        """Gets the events_id of this Entity.  # noqa: E501
-
-
-        :return: The events_id of this Entity.  # noqa: E501
-        :rtype: str
-        """
-        return self._events_id
-
-    @events_id.setter
-    def events_id(self, events_id):
-        """Sets the events_id of this Entity.
-
-
-        :param events_id: The events_id of this Entity.  # noqa: E501
-        :type: str
-        """
-
-        self._events_id = events_id
-
-    @property
-    def events_item_id(self):
-        """Gets the events_item_id of this Entity.  # noqa: E501
-
-
-        :return: The events_item_id of this Entity.  # noqa: E501
-        :rtype: str
-        """
-        return self._events_item_id
-
-    @events_item_id.setter
-    def events_item_id(self, events_item_id):
-        """Sets the events_item_id of this Entity.
-
-
-        :param events_item_id: The events_item_id of this Entity.  # noqa: E501
-        :type: str
-        """
-
-        self._events_item_id = events_item_id
-
-    @property
     def firstname(self):
         """Gets the firstname of this Entity.  # noqa: E501
 
 
         :return: The firstname of this Entity.  # noqa: E501
         :rtype: str
         """
@@ -665,35 +608,14 @@
         :param id: The id of this Entity.  # noqa: E501
         :type: int
         """
 
         self._id = id
 
     @property
-    def is_bound(self):
-        """Gets the is_bound of this Entity.  # noqa: E501
-
-
-        :return: The is_bound of this Entity.  # noqa: E501
-        :rtype: str
-        """
-        return self._is_bound
-
-    @is_bound.setter
-    def is_bound(self, is_bound):
-        """Sets the is_bound of this Entity.
-
-
-        :param is_bound: The is_bound of this Entity.  # noqa: E501
-        :type: str
-        """
-
-        self._is_bound = is_bound
-
-    @property
     def lastchangeby(self):
         """Gets the lastchangeby of this Entity.  # noqa: E501
 
 
         :return: The lastchangeby of this Entity.  # noqa: E501
         :rtype: int
         """
@@ -838,25 +760,25 @@
 
     @property
     def modified_at(self):
         """Gets the modified_at of this Entity.  # noqa: E501
 
 
         :return: The modified_at of this Entity.  # noqa: E501
-        :rtype: str
+        :rtype: datetime
         """
         return self._modified_at
 
     @modified_at.setter
     def modified_at(self, modified_at):
         """Sets the modified_at of this Entity.
 
 
         :param modified_at: The modified_at of this Entity.  # noqa: E501
-        :type: str
+        :type: datetime
         """
 
         self._modified_at = modified_at
 
     @property
     def next_step(self):
         """Gets the next_step of this Entity.  # noqa: E501
```

### Comparing `elabapi-python-0.2.4/elabapi_python/models/event.py` & `elabapi-python-0.3.0/elabapi_python/models/event.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/models/events_id_body.py` & `elabapi-python-0.3.0/elabapi_python/models/events_id_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/models/events_id_body1.py` & `elabapi-python-0.3.0/elabapi_python/models/events_id_body1.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/models/eventsid_delta.py` & `elabapi-python-0.3.0/elabapi_python/models/eventsid_delta.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/models/experiment.py` & `elabapi-python-0.3.0/elabapi_python/models/experiment.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/models/experiment_template.py` & `elabapi-python-0.3.0/elabapi_python/models/experiment_template.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/models/experiments_body.py` & `elabapi-python-0.3.0/elabapi_python/models/experiments_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/models/experiments_id_body.py` & `elabapi-python-0.3.0/elabapi_python/models/experiments_id_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/models/experiments_links_subid_body.py` & `elabapi-python-0.3.0/elabapi_python/models/experiments_links_subid_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/models/experiments_templates_body.py` & `elabapi-python-0.3.0/elabapi_python/models/experiments_templates_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/models/experiments_templates_id_body.py` & `elabapi-python-0.3.0/elabapi_python/models/experiments_templates_id_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/models/favtags_body.py` & `elabapi-python-0.3.0/elabapi_python/models/favtags_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/models/id.py` & `elabapi-python-0.3.0/elabapi_python/models/id.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/models/id1.py` & `elabapi-python-0.3.0/elabapi_python/models/id1.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/models/id2.py` & `elabapi-python-0.3.0/elabapi_python/models/id2.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/models/id3.py` & `elabapi-python-0.3.0/elabapi_python/models/id3.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/models/id_comments_body.py` & `elabapi-python-0.3.0/elabapi_python/models/id_comments_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/models/id_status_body.py` & `elabapi-python-0.3.0/elabapi_python/models/id_status_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/models/id_steps_body.py` & `elabapi-python-0.3.0/elabapi_python/models/id_steps_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/models/id_tags_body.py` & `elabapi-python-0.3.0/elabapi_python/models/id_tags_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/models/id_teamgroups_body.py` & `elabapi-python-0.3.0/elabapi_python/models/id_teamgroups_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/models/id_uploads_body.py` & `elabapi-python-0.3.0/elabapi_python/models/id_uploads_body.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,16 +38,15 @@
     }
 
     def __init__(self, file=None, comment=None):  # noqa: E501
         """IdUploadsBody - a model defined in Swagger"""  # noqa: E501
         self._file = None
         self._comment = None
         self.discriminator = None
-        if file is not None:
-            self.file = file
+        self.file = file
         if comment is not None:
             self.comment = comment
 
     @property
     def file(self):
         """Gets the file of this IdUploadsBody.  # noqa: E501
 
@@ -63,14 +62,16 @@
         """Sets the file of this IdUploadsBody.
 
         The file to upload.  # noqa: E501
 
         :param file: The file of this IdUploadsBody.  # noqa: E501
         :type: str
         """
+        if file is None:
+            raise ValueError("Invalid value for `file`, must not be `None`")  # noqa: E501
 
         self._file = file
 
     @property
     def comment(self):
         """Gets the comment of this IdUploadsBody.  # noqa: E501
```

### Comparing `elabapi-python-0.2.4/elabapi_python/models/idp.py` & `elabapi-python-0.3.0/elabapi_python/models/idp.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/models/idps_body.py` & `elabapi-python-0.3.0/elabapi_python/models/idps_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/models/idps_id_body.py` & `elabapi-python-0.3.0/elabapi_python/models/idps_id_body.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,20 +57,14 @@
 
 
         :param action: The action of this IdpsIdBody.  # noqa: E501
         :type: str
         """
         if action is None:
             raise ValueError("Invalid value for `action`, must not be `None`")  # noqa: E501
-        allowed_values = ["update"]  # noqa: E501
-        if action not in allowed_values:
-            raise ValueError(
-                "Invalid value for `action` ({0}), must be one of {1}"  # noqa: E501
-                .format(action, allowed_values)
-            )
 
         self._action = action
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `elabapi-python-0.2.4/elabapi_python/models/inline_response200.py` & `elabapi-python-0.3.0/elabapi_python/models/inline_response2001.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class InlineResponse200(object):
+class InlineResponse2001(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -36,84 +36,84 @@
     attribute_map = {
         'users_id': 'users_id',
         'tags_id': 'tags_id',
         'tag': 'tag'
     }
 
     def __init__(self, users_id=None, tags_id=None, tag=None):  # noqa: E501
-        """InlineResponse200 - a model defined in Swagger"""  # noqa: E501
+        """InlineResponse2001 - a model defined in Swagger"""  # noqa: E501
         self._users_id = None
         self._tags_id = None
         self._tag = None
         self.discriminator = None
         if users_id is not None:
             self.users_id = users_id
         if tags_id is not None:
             self.tags_id = tags_id
         if tag is not None:
             self.tag = tag
 
     @property
     def users_id(self):
-        """Gets the users_id of this InlineResponse200.  # noqa: E501
+        """Gets the users_id of this InlineResponse2001.  # noqa: E501
 
 
-        :return: The users_id of this InlineResponse200.  # noqa: E501
+        :return: The users_id of this InlineResponse2001.  # noqa: E501
         :rtype: int
         """
         return self._users_id
 
     @users_id.setter
     def users_id(self, users_id):
-        """Sets the users_id of this InlineResponse200.
+        """Sets the users_id of this InlineResponse2001.
 
 
-        :param users_id: The users_id of this InlineResponse200.  # noqa: E501
+        :param users_id: The users_id of this InlineResponse2001.  # noqa: E501
         :type: int
         """
 
         self._users_id = users_id
 
     @property
     def tags_id(self):
-        """Gets the tags_id of this InlineResponse200.  # noqa: E501
+        """Gets the tags_id of this InlineResponse2001.  # noqa: E501
 
 
-        :return: The tags_id of this InlineResponse200.  # noqa: E501
+        :return: The tags_id of this InlineResponse2001.  # noqa: E501
         :rtype: int
         """
         return self._tags_id
 
     @tags_id.setter
     def tags_id(self, tags_id):
-        """Sets the tags_id of this InlineResponse200.
+        """Sets the tags_id of this InlineResponse2001.
 
 
-        :param tags_id: The tags_id of this InlineResponse200.  # noqa: E501
+        :param tags_id: The tags_id of this InlineResponse2001.  # noqa: E501
         :type: int
         """
 
         self._tags_id = tags_id
 
     @property
     def tag(self):
-        """Gets the tag of this InlineResponse200.  # noqa: E501
+        """Gets the tag of this InlineResponse2001.  # noqa: E501
 
 
-        :return: The tag of this InlineResponse200.  # noqa: E501
+        :return: The tag of this InlineResponse2001.  # noqa: E501
         :rtype: str
         """
         return self._tag
 
     @tag.setter
     def tag(self, tag):
-        """Sets the tag of this InlineResponse200.
+        """Sets the tag of this InlineResponse2001.
 
 
-        :param tag: The tag of this InlineResponse200.  # noqa: E501
+        :param tag: The tag of this InlineResponse2001.  # noqa: E501
         :type: str
         """
 
         self._tag = tag
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -132,15 +132,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(InlineResponse200, dict):
+        if issubclass(InlineResponse2001, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -148,15 +148,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, InlineResponse200):
+        if not isinstance(other, InlineResponse2001):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `elabapi-python-0.2.4/elabapi_python/models/inline_response2001.py` & `elabapi-python-0.3.0/elabapi_python/models/inline_response2003.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class InlineResponse2001(object):
+class InlineResponse2003(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -34,60 +34,60 @@
 
     attribute_map = {
         'tag': 'tag',
         'id': 'id'
     }
 
     def __init__(self, tag=None, id=None):  # noqa: E501
-        """InlineResponse2001 - a model defined in Swagger"""  # noqa: E501
+        """InlineResponse2003 - a model defined in Swagger"""  # noqa: E501
         self._tag = None
         self._id = None
         self.discriminator = None
         if tag is not None:
             self.tag = tag
         if id is not None:
             self.id = id
 
     @property
     def tag(self):
-        """Gets the tag of this InlineResponse2001.  # noqa: E501
+        """Gets the tag of this InlineResponse2003.  # noqa: E501
 
 
-        :return: The tag of this InlineResponse2001.  # noqa: E501
+        :return: The tag of this InlineResponse2003.  # noqa: E501
         :rtype: str
         """
         return self._tag
 
     @tag.setter
     def tag(self, tag):
-        """Sets the tag of this InlineResponse2001.
+        """Sets the tag of this InlineResponse2003.
 
 
-        :param tag: The tag of this InlineResponse2001.  # noqa: E501
+        :param tag: The tag of this InlineResponse2003.  # noqa: E501
         :type: str
         """
 
         self._tag = tag
 
     @property
     def id(self):
-        """Gets the id of this InlineResponse2001.  # noqa: E501
+        """Gets the id of this InlineResponse2003.  # noqa: E501
 
 
-        :return: The id of this InlineResponse2001.  # noqa: E501
+        :return: The id of this InlineResponse2003.  # noqa: E501
         :rtype: int
         """
         return self._id
 
     @id.setter
     def id(self, id):
-        """Sets the id of this InlineResponse2001.
+        """Sets the id of this InlineResponse2003.
 
 
-        :param id: The id of this InlineResponse2001.  # noqa: E501
+        :param id: The id of this InlineResponse2003.  # noqa: E501
         :type: int
         """
 
         self._id = id
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -106,15 +106,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(InlineResponse2001, dict):
+        if issubclass(InlineResponse2003, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -122,15 +122,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, InlineResponse2001):
+        if not isinstance(other, InlineResponse2003):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `elabapi-python-0.2.4/elabapi_python/models/inline_response2002.py` & `elabapi-python-0.3.0/elabapi_python/models/inline_response2004.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class InlineResponse2002(object):
+class InlineResponse2004(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -36,84 +36,84 @@
     attribute_map = {
         'id': 'id',
         'name': 'name',
         'team': 'team'
     }
 
     def __init__(self, id=None, name=None, team=None):  # noqa: E501
-        """InlineResponse2002 - a model defined in Swagger"""  # noqa: E501
+        """InlineResponse2004 - a model defined in Swagger"""  # noqa: E501
         self._id = None
         self._name = None
         self._team = None
         self.discriminator = None
         if id is not None:
             self.id = id
         if name is not None:
             self.name = name
         if team is not None:
             self.team = team
 
     @property
     def id(self):
-        """Gets the id of this InlineResponse2002.  # noqa: E501
+        """Gets the id of this InlineResponse2004.  # noqa: E501
 
 
-        :return: The id of this InlineResponse2002.  # noqa: E501
+        :return: The id of this InlineResponse2004.  # noqa: E501
         :rtype: int
         """
         return self._id
 
     @id.setter
     def id(self, id):
-        """Sets the id of this InlineResponse2002.
+        """Sets the id of this InlineResponse2004.
 
 
-        :param id: The id of this InlineResponse2002.  # noqa: E501
+        :param id: The id of this InlineResponse2004.  # noqa: E501
         :type: int
         """
 
         self._id = id
 
     @property
     def name(self):
-        """Gets the name of this InlineResponse2002.  # noqa: E501
+        """Gets the name of this InlineResponse2004.  # noqa: E501
 
 
-        :return: The name of this InlineResponse2002.  # noqa: E501
+        :return: The name of this InlineResponse2004.  # noqa: E501
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
-        """Sets the name of this InlineResponse2002.
+        """Sets the name of this InlineResponse2004.
 
 
-        :param name: The name of this InlineResponse2002.  # noqa: E501
+        :param name: The name of this InlineResponse2004.  # noqa: E501
         :type: str
         """
 
         self._name = name
 
     @property
     def team(self):
-        """Gets the team of this InlineResponse2002.  # noqa: E501
+        """Gets the team of this InlineResponse2004.  # noqa: E501
 
 
-        :return: The team of this InlineResponse2002.  # noqa: E501
+        :return: The team of this InlineResponse2004.  # noqa: E501
         :rtype: int
         """
         return self._team
 
     @team.setter
     def team(self, team):
-        """Sets the team of this InlineResponse2002.
+        """Sets the team of this InlineResponse2004.
 
 
-        :param team: The team of this InlineResponse2002.  # noqa: E501
+        :param team: The team of this InlineResponse2004.  # noqa: E501
         :type: int
         """
 
         self._team = team
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -132,15 +132,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(InlineResponse2002, dict):
+        if issubclass(InlineResponse2004, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -148,15 +148,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, InlineResponse2002):
+        if not isinstance(other, InlineResponse2004):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `elabapi-python-0.2.4/elabapi_python/models/inline_response2003.py` & `elabapi-python-0.3.0/elabapi_python/models/inline_response2006.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class InlineResponse2003(object):
+class InlineResponse2006(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -28,29 +28,29 @@
                             and the value is json key in definition.
     """
     swagger_types = {
         'id': 'int',
         'category': 'int',
         'body': 'object',
         'is_ack': 'int',
-        'created_at': 'str',
+        'created_at': 'datetime',
         'userid': 'int'
     }
 
     attribute_map = {
         'id': 'id',
         'category': 'category',
         'body': 'body',
         'is_ack': 'is_ack',
         'created_at': 'created_at',
         'userid': 'userid'
     }
 
     def __init__(self, id=None, category=None, body=None, is_ack=None, created_at=None, userid=None):  # noqa: E501
-        """InlineResponse2003 - a model defined in Swagger"""  # noqa: E501
+        """InlineResponse2006 - a model defined in Swagger"""  # noqa: E501
         self._id = None
         self._category = None
         self._body = None
         self._is_ack = None
         self._created_at = None
         self._userid = None
         self.discriminator = None
@@ -65,133 +65,133 @@
         if created_at is not None:
             self.created_at = created_at
         if userid is not None:
             self.userid = userid
 
     @property
     def id(self):
-        """Gets the id of this InlineResponse2003.  # noqa: E501
+        """Gets the id of this InlineResponse2006.  # noqa: E501
 
 
-        :return: The id of this InlineResponse2003.  # noqa: E501
+        :return: The id of this InlineResponse2006.  # noqa: E501
         :rtype: int
         """
         return self._id
 
     @id.setter
     def id(self, id):
-        """Sets the id of this InlineResponse2003.
+        """Sets the id of this InlineResponse2006.
 
 
-        :param id: The id of this InlineResponse2003.  # noqa: E501
+        :param id: The id of this InlineResponse2006.  # noqa: E501
         :type: int
         """
 
         self._id = id
 
     @property
     def category(self):
-        """Gets the category of this InlineResponse2003.  # noqa: E501
+        """Gets the category of this InlineResponse2006.  # noqa: E501
 
 
-        :return: The category of this InlineResponse2003.  # noqa: E501
+        :return: The category of this InlineResponse2006.  # noqa: E501
         :rtype: int
         """
         return self._category
 
     @category.setter
     def category(self, category):
-        """Sets the category of this InlineResponse2003.
+        """Sets the category of this InlineResponse2006.
 
 
-        :param category: The category of this InlineResponse2003.  # noqa: E501
+        :param category: The category of this InlineResponse2006.  # noqa: E501
         :type: int
         """
 
         self._category = category
 
     @property
     def body(self):
-        """Gets the body of this InlineResponse2003.  # noqa: E501
+        """Gets the body of this InlineResponse2006.  # noqa: E501
 
 
-        :return: The body of this InlineResponse2003.  # noqa: E501
+        :return: The body of this InlineResponse2006.  # noqa: E501
         :rtype: object
         """
         return self._body
 
     @body.setter
     def body(self, body):
-        """Sets the body of this InlineResponse2003.
+        """Sets the body of this InlineResponse2006.
 
 
-        :param body: The body of this InlineResponse2003.  # noqa: E501
+        :param body: The body of this InlineResponse2006.  # noqa: E501
         :type: object
         """
 
         self._body = body
 
     @property
     def is_ack(self):
-        """Gets the is_ack of this InlineResponse2003.  # noqa: E501
+        """Gets the is_ack of this InlineResponse2006.  # noqa: E501
 
 
-        :return: The is_ack of this InlineResponse2003.  # noqa: E501
+        :return: The is_ack of this InlineResponse2006.  # noqa: E501
         :rtype: int
         """
         return self._is_ack
 
     @is_ack.setter
     def is_ack(self, is_ack):
-        """Sets the is_ack of this InlineResponse2003.
+        """Sets the is_ack of this InlineResponse2006.
 
 
-        :param is_ack: The is_ack of this InlineResponse2003.  # noqa: E501
+        :param is_ack: The is_ack of this InlineResponse2006.  # noqa: E501
         :type: int
         """
 
         self._is_ack = is_ack
 
     @property
     def created_at(self):
-        """Gets the created_at of this InlineResponse2003.  # noqa: E501
+        """Gets the created_at of this InlineResponse2006.  # noqa: E501
 
 
-        :return: The created_at of this InlineResponse2003.  # noqa: E501
-        :rtype: str
+        :return: The created_at of this InlineResponse2006.  # noqa: E501
+        :rtype: datetime
         """
         return self._created_at
 
     @created_at.setter
     def created_at(self, created_at):
-        """Sets the created_at of this InlineResponse2003.
+        """Sets the created_at of this InlineResponse2006.
 
 
-        :param created_at: The created_at of this InlineResponse2003.  # noqa: E501
-        :type: str
+        :param created_at: The created_at of this InlineResponse2006.  # noqa: E501
+        :type: datetime
         """
 
         self._created_at = created_at
 
     @property
     def userid(self):
-        """Gets the userid of this InlineResponse2003.  # noqa: E501
+        """Gets the userid of this InlineResponse2006.  # noqa: E501
 
 
-        :return: The userid of this InlineResponse2003.  # noqa: E501
+        :return: The userid of this InlineResponse2006.  # noqa: E501
         :rtype: int
         """
         return self._userid
 
     @userid.setter
     def userid(self, userid):
-        """Sets the userid of this InlineResponse2003.
+        """Sets the userid of this InlineResponse2006.
 
 
-        :param userid: The userid of this InlineResponse2003.  # noqa: E501
+        :param userid: The userid of this InlineResponse2006.  # noqa: E501
         :type: int
         """
 
         self._userid = userid
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -210,15 +210,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(InlineResponse2003, dict):
+        if issubclass(InlineResponse2006, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -226,15 +226,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, InlineResponse2003):
+        if not isinstance(other, InlineResponse2006):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `elabapi-python-0.2.4/elabapi_python/models/item.py` & `elabapi-python-0.3.0/elabapi_python/models/teamgroups_subid_body.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,42 +10,36 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from elabapi_python.models.entity import Entity  # noqa: F401,E501
 
-class Item(Entity):
+class TeamgroupsSubidBody(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
-    if hasattr(Entity, "swagger_types"):
-        swagger_types.update(Entity.swagger_types)
 
     attribute_map = {
     }
-    if hasattr(Entity, "attribute_map"):
-        attribute_map.update(Entity.attribute_map)
 
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """Item - a model defined in Swagger"""  # noqa: E501
+    def __init__(self):  # noqa: E501
+        """TeamgroupsSubidBody - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
-        Entity.__init__(self, *args, **kwargs)
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -60,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(Item, dict):
+        if issubclass(TeamgroupsSubidBody, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -76,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Item):
+        if not isinstance(other, TeamgroupsSubidBody):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `elabapi-python-0.2.4/elabapi_python/models/items_body.py` & `elabapi-python-0.3.0/elabapi_python/models/items_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/models/items_id_body.py` & `elabapi-python-0.3.0/elabapi_python/models/items_id_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/models/items_links_subid_body.py` & `elabapi-python-0.3.0/elabapi_python/models/items_links_subid_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/models/items_type.py` & `elabapi-python-0.3.0/elabapi_python/models/items_type.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,51 +27,46 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'category_id': 'int',
         'category': 'str',
         'color': 'str',
-        'bookable': 'int',
         'body': 'str',
         'ordering': 'int',
         'canread': 'str',
         'canwrite': 'str'
     }
 
     attribute_map = {
         'category_id': 'category_id',
         'category': 'category',
         'color': 'color',
-        'bookable': 'bookable',
         'body': 'body',
         'ordering': 'ordering',
         'canread': 'canread',
         'canwrite': 'canwrite'
     }
 
-    def __init__(self, category_id=None, category=None, color=None, bookable=None, body=None, ordering=None, canread=None, canwrite=None):  # noqa: E501
+    def __init__(self, category_id=None, category=None, color=None, body=None, ordering=None, canread=None, canwrite=None):  # noqa: E501
         """ItemsType - a model defined in Swagger"""  # noqa: E501
         self._category_id = None
         self._category = None
         self._color = None
-        self._bookable = None
         self._body = None
         self._ordering = None
         self._canread = None
         self._canwrite = None
         self.discriminator = None
         if category_id is not None:
             self.category_id = category_id
         if category is not None:
             self.category = category
         if color is not None:
             self.color = color
-        if bookable is not None:
-            self.bookable = bookable
         if body is not None:
             self.body = body
         if ordering is not None:
             self.ordering = ordering
         if canread is not None:
             self.canread = canread
         if canwrite is not None:
@@ -137,35 +132,14 @@
         :param color: The color of this ItemsType.  # noqa: E501
         :type: str
         """
 
         self._color = color
 
     @property
-    def bookable(self):
-        """Gets the bookable of this ItemsType.  # noqa: E501
-
-
-        :return: The bookable of this ItemsType.  # noqa: E501
-        :rtype: int
-        """
-        return self._bookable
-
-    @bookable.setter
-    def bookable(self, bookable):
-        """Sets the bookable of this ItemsType.
-
-
-        :param bookable: The bookable of this ItemsType.  # noqa: E501
-        :type: int
-        """
-
-        self._bookable = bookable
-
-    @property
     def body(self):
         """Gets the body of this ItemsType.  # noqa: E501
 
 
         :return: The body of this ItemsType.  # noqa: E501
         :rtype: str
         """
```

### Comparing `elabapi-python-0.2.4/elabapi_python/models/items_types_body.py` & `elabapi-python-0.3.0/elabapi_python/models/items_types_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/models/link.py` & `elabapi-python-0.3.0/elabapi_python/models/link.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,46 +28,46 @@
                             and the value is json key in definition.
     """
     swagger_types = {
         'itemid': 'int',
         'title': 'str',
         'elabid': 'str',
         'category': 'str',
-        'bookable': 'int',
+        'is_bookable': 'int',
         'color': 'str'
     }
 
     attribute_map = {
         'itemid': 'itemid',
         'title': 'title',
         'elabid': 'elabid',
         'category': 'category',
-        'bookable': 'bookable',
+        'is_bookable': 'is_bookable',
         'color': 'color'
     }
 
-    def __init__(self, itemid=None, title=None, elabid=None, category=None, bookable=None, color=None):  # noqa: E501
+    def __init__(self, itemid=None, title=None, elabid=None, category=None, is_bookable=None, color=None):  # noqa: E501
         """Link - a model defined in Swagger"""  # noqa: E501
         self._itemid = None
         self._title = None
         self._elabid = None
         self._category = None
-        self._bookable = None
+        self._is_bookable = None
         self._color = None
         self.discriminator = None
         if itemid is not None:
             self.itemid = itemid
         if title is not None:
             self.title = title
         if elabid is not None:
             self.elabid = elabid
         if category is not None:
             self.category = category
-        if bookable is not None:
-            self.bookable = bookable
+        if is_bookable is not None:
+            self.is_bookable = is_bookable
         if color is not None:
             self.color = color
 
     @property
     def itemid(self):
         """Gets the itemid of this Link.  # noqa: E501
 
@@ -148,33 +148,33 @@
         :param category: The category of this Link.  # noqa: E501
         :type: str
         """
 
         self._category = category
 
     @property
-    def bookable(self):
-        """Gets the bookable of this Link.  # noqa: E501
+    def is_bookable(self):
+        """Gets the is_bookable of this Link.  # noqa: E501
 
 
-        :return: The bookable of this Link.  # noqa: E501
+        :return: The is_bookable of this Link.  # noqa: E501
         :rtype: int
         """
-        return self._bookable
+        return self._is_bookable
 
-    @bookable.setter
-    def bookable(self, bookable):
-        """Sets the bookable of this Link.
+    @is_bookable.setter
+    def is_bookable(self, is_bookable):
+        """Sets the is_bookable of this Link.
 
 
-        :param bookable: The bookable of this Link.  # noqa: E501
+        :param is_bookable: The is_bookable of this Link.  # noqa: E501
         :type: int
         """
 
-        self._bookable = bookable
+        self._is_bookable = is_bookable
 
     @property
     def color(self):
         """Gets the color of this Link.  # noqa: E501
 
 
         :return: The color of this Link.  # noqa: E501
```

### Comparing `elabapi-python-0.2.4/elabapi_python/models/notification.py` & `elabapi-python-0.3.0/elabapi_python/models/notification.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'id': 'int',
         'category': 'int',
         'is_ack': 'int',
-        'created_at': 'str',
+        'created_at': 'datetime',
         'userid': 'int',
         'send_email': 'int',
         'email_sent_at': 'str',
         'body': 'str'
     }
 
     attribute_map = {
@@ -142,25 +142,25 @@
 
     @property
     def created_at(self):
         """Gets the created_at of this Notification.  # noqa: E501
 
 
         :return: The created_at of this Notification.  # noqa: E501
-        :rtype: str
+        :rtype: datetime
         """
         return self._created_at
 
     @created_at.setter
     def created_at(self, created_at):
         """Sets the created_at of this Notification.
 
 
         :param created_at: The created_at of this Notification.  # noqa: E501
-        :type: str
+        :type: datetime
         """
 
         self._created_at = created_at
 
     @property
     def userid(self):
         """Gets the userid of this Notification.  # noqa: E501
```

### Comparing `elabapi-python-0.2.4/elabapi_python/models/status.py` & `elabapi-python-0.3.0/elabapi_python/models/status.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/models/step.py` & `elabapi-python-0.3.0/elabapi_python/models/step.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/models/steps_subid_body.py` & `elabapi-python-0.3.0/elabapi_python/models/steps_subid_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/models/tag.py` & `elabapi-python-0.3.0/elabapi_python/models/tag.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/models/tags_subid_body.py` & `elabapi-python-0.3.0/elabapi_python/models/tags_subid_body.py`

 * *Files 7% similar despite different names*

```diff
@@ -57,20 +57,14 @@
 
 
         :param action: The action of this TagsSubidBody.  # noqa: E501
         :type: str
         """
         if action is None:
             raise ValueError("Invalid value for `action`, must not be `None`")  # noqa: E501
-        allowed_values = ["unreference"]  # noqa: E501
-        if action not in allowed_values:
-            raise ValueError(
-                "Invalid value for `action` ({0}), must be one of {1}"  # noqa: E501
-                .format(action, allowed_values)
-            )
 
         self._action = action
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `elabapi-python-0.2.4/elabapi_python/models/team.py` & `elabapi-python-0.3.0/elabapi_python/models/team.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         'common_template_md': 'str',
         'deletable_xp': 'int',
         'deletable_item': 'int',
         'user_create_tag': 'int',
         'force_exp_tpl': 'int',
         'link_name': 'str',
         'link_href': 'str',
-        'created_at': 'str',
+        'created_at': 'datetime',
         'orgid': 'str',
         'public_db': 'int',
         'force_canread': 'str',
         'force_canwrite': 'str',
         'do_force_canread': 'int',
         'do_force_canwrite': 'int',
         'visible': 'int'
@@ -339,25 +339,25 @@
 
     @property
     def created_at(self):
         """Gets the created_at of this Team.  # noqa: E501
 
 
         :return: The created_at of this Team.  # noqa: E501
-        :rtype: str
+        :rtype: datetime
         """
         return self._created_at
 
     @created_at.setter
     def created_at(self, created_at):
         """Sets the created_at of this Team.
 
 
         :param created_at: The created_at of this Team.  # noqa: E501
-        :type: str
+        :type: datetime
         """
 
         self._created_at = created_at
 
     @property
     def orgid(self):
         """Gets the orgid of this Team.  # noqa: E501
```

### Comparing `elabapi-python-0.2.4/elabapi_python/models/team_tags_body.py` & `elabapi-python-0.3.0/elabapi_python/models/team_tags_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/models/team_tags_body1.py` & `elabapi-python-0.3.0/elabapi_python/models/team_tags_body1.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,20 +56,14 @@
     def action(self, action):
         """Sets the action of this TeamTagsBody1.
 
 
         :param action: The action of this TeamTagsBody1.  # noqa: E501
         :type: str
         """
-        allowed_values = ["deduplicate"]  # noqa: E501
-        if action not in allowed_values:
-            raise ValueError(
-                "Invalid value for `action` ({0}), must be one of {1}"  # noqa: E501
-                .format(action, allowed_values)
-            )
 
         self._action = action
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `elabapi-python-0.2.4/elabapi_python/models/team_tags_id_body.py` & `elabapi-python-0.3.0/elabapi_python/models/team_tags_id_body.py`

 * *Files 11% similar despite different names*

```diff
@@ -61,20 +61,14 @@
     def action(self, action):
         """Sets the action of this TeamTagsIdBody.
 
 
         :param action: The action of this TeamTagsIdBody.  # noqa: E501
         :type: str
         """
-        allowed_values = ["updatetag"]  # noqa: E501
-        if action not in allowed_values:
-            raise ValueError(
-                "Invalid value for `action` ({0}), must be one of {1}"  # noqa: E501
-                .format(action, allowed_values)
-            )
 
         self._action = action
 
     @property
     def tag(self):
         """Gets the tag of this TeamTagsIdBody.  # noqa: E501
```

### Comparing `elabapi-python-0.2.4/elabapi_python/models/teamgroup.py` & `elabapi-python-0.3.0/elabapi_python/models/teamgroup.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/models/teamgroup_users.py` & `elabapi-python-0.3.0/elabapi_python/models/teamgroup_users.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/models/teamgroups_subid_body.py` & `elabapi-python-0.3.0/elabapi_python/models/users_id_body.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class TeamgroupsSubidBody(object):
+class UsersIdBody(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -30,15 +30,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """TeamgroupsSubidBody - a model defined in Swagger"""  # noqa: E501
+        """UsersIdBody - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(TeamgroupsSubidBody, dict):
+        if issubclass(UsersIdBody, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TeamgroupsSubidBody):
+        if not isinstance(other, UsersIdBody):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `elabapi-python-0.2.4/elabapi_python/models/teams_body.py` & `elabapi-python-0.3.0/elabapi_python/models/teams_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/models/todoitem.py` & `elabapi-python-0.3.0/elabapi_python/models/todoitem.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/models/todolist_body.py` & `elabapi-python-0.3.0/elabapi_python/models/todolist_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/models/todolist_id_body.py` & `elabapi-python-0.3.0/elabapi_python/models/todolist_id_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/models/unfinished_step.py` & `elabapi-python-0.3.0/elabapi_python/models/unfinished_step.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/models/unfinished_steps.py` & `elabapi-python-0.3.0/elabapi_python/models/unfinished_steps.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/models/upload.py` & `elabapi-python-0.3.0/elabapi_python/models/upload.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         'id': 'int',
         'real_name': 'str',
         'long_name': 'str',
         'comment': 'str',
         'item_id': 'int',
         'userid': 'str',
         'type': 'str',
-        'created_at': 'str',
+        'created_at': 'datetime',
         'hash': 'str',
         'hash_algorithm': 'str',
         'storage': 'int',
         'filesize': 'int',
         'state': 'int',
         'immutable': 'int',
         'fullname': 'str'
@@ -261,25 +261,25 @@
 
     @property
     def created_at(self):
         """Gets the created_at of this Upload.  # noqa: E501
 
 
         :return: The created_at of this Upload.  # noqa: E501
-        :rtype: str
+        :rtype: datetime
         """
         return self._created_at
 
     @created_at.setter
     def created_at(self, created_at):
         """Sets the created_at of this Upload.
 
 
         :param created_at: The created_at of this Upload.  # noqa: E501
-        :type: str
+        :type: datetime
         """
 
         self._created_at = created_at
 
     @property
     def hash(self):
         """Gets the hash of this Upload.  # noqa: E501
```

### Comparing `elabapi-python-0.2.4/elabapi_python/models/uploads_subid_body.py` & `elabapi-python-0.3.0/elabapi_python/models/id_revisions_body.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,68 +11,62 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class UploadsSubidBody(object):
+class IdRevisionsBody(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'action': 'str'
+        'body': 'str'
     }
 
     attribute_map = {
-        'action': 'action'
+        'body': 'body'
     }
 
-    def __init__(self, action=None):  # noqa: E501
-        """UploadsSubidBody - a model defined in Swagger"""  # noqa: E501
-        self._action = None
+    def __init__(self, body=None):  # noqa: E501
+        """IdRevisionsBody - a model defined in Swagger"""  # noqa: E501
+        self._body = None
         self.discriminator = None
-        self.action = action
+        self.body = body
 
     @property
-    def action(self):
-        """Gets the action of this UploadsSubidBody.  # noqa: E501
+    def body(self):
+        """Gets the body of this IdRevisionsBody.  # noqa: E501
 
 
-        :return: The action of this UploadsSubidBody.  # noqa: E501
+        :return: The body of this IdRevisionsBody.  # noqa: E501
         :rtype: str
         """
-        return self._action
+        return self._body
 
-    @action.setter
-    def action(self, action):
-        """Sets the action of this UploadsSubidBody.
+    @body.setter
+    def body(self, body):
+        """Sets the body of this IdRevisionsBody.
 
 
-        :param action: The action of this UploadsSubidBody.  # noqa: E501
+        :param body: The body of this IdRevisionsBody.  # noqa: E501
         :type: str
         """
-        if action is None:
-            raise ValueError("Invalid value for `action`, must not be `None`")  # noqa: E501
-        allowed_values = ["update"]  # noqa: E501
-        if action not in allowed_values:
-            raise ValueError(
-                "Invalid value for `action` ({0}), must be one of {1}"  # noqa: E501
-                .format(action, allowed_values)
-            )
+        if body is None:
+            raise ValueError("Invalid value for `body`, must not be `None`")  # noqa: E501
 
-        self._action = action
+        self._body = body
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -87,15 +81,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(UploadsSubidBody, dict):
+        if issubclass(IdRevisionsBody, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -103,15 +97,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, UploadsSubidBody):
+        if not isinstance(other, IdRevisionsBody):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `elabapi-python-0.2.4/elabapi_python/models/users.py` & `elabapi-python-0.3.0/elabapi_python/models/users.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,14 +36,15 @@
         'archived': 'int',
         'last_login': 'str',
         'fullname': 'str',
         'orcid': 'str',
         'orgid': 'str',
         'auth_service': 'int',
         'is_sysadmin': 'int',
+        'entrypoint': 'int',
         'teams': 'list[UsersTeams]'
     }
 
     attribute_map = {
         'userid': 'userid',
         'firstname': 'firstname',
         'lastname': 'lastname',
@@ -52,31 +53,33 @@
         'archived': 'archived',
         'last_login': 'last_login',
         'fullname': 'fullname',
         'orcid': 'orcid',
         'orgid': 'orgid',
         'auth_service': 'auth_service',
         'is_sysadmin': 'is_sysadmin',
+        'entrypoint': 'entrypoint',
         'teams': 'teams'
     }
 
-    def __init__(self, userid=None, firstname=None, lastname=None, email=None, validated=None, archived=None, last_login=None, fullname=None, orcid=None, orgid=None, auth_service=None, is_sysadmin=None, teams=None):  # noqa: E501
+    def __init__(self, userid=None, firstname=None, lastname=None, email=None, validated=None, archived=None, last_login=None, fullname=None, orcid=None, orgid=None, auth_service=None, is_sysadmin=None, entrypoint=None, teams=None):  # noqa: E501
         """Users - a model defined in Swagger"""  # noqa: E501
         self._userid = None
         self._firstname = None
         self._lastname = None
         self._email = None
         self._validated = None
         self._archived = None
         self._last_login = None
         self._fullname = None
         self._orcid = None
         self._orgid = None
         self._auth_service = None
         self._is_sysadmin = None
+        self._entrypoint = None
         self._teams = None
         self.discriminator = None
         if userid is not None:
             self.userid = userid
         if firstname is not None:
             self.firstname = firstname
         if lastname is not None:
@@ -95,14 +98,16 @@
             self.orcid = orcid
         if orgid is not None:
             self.orgid = orgid
         if auth_service is not None:
             self.auth_service = auth_service
         if is_sysadmin is not None:
             self.is_sysadmin = is_sysadmin
+        if entrypoint is not None:
+            self.entrypoint = entrypoint
         if teams is not None:
             self.teams = teams
 
     @property
     def userid(self):
         """Gets the userid of this Users.  # noqa: E501
 
@@ -351,14 +356,35 @@
         :param is_sysadmin: The is_sysadmin of this Users.  # noqa: E501
         :type: int
         """
 
         self._is_sysadmin = is_sysadmin
 
     @property
+    def entrypoint(self):
+        """Gets the entrypoint of this Users.  # noqa: E501
+
+
+        :return: The entrypoint of this Users.  # noqa: E501
+        :rtype: int
+        """
+        return self._entrypoint
+
+    @entrypoint.setter
+    def entrypoint(self, entrypoint):
+        """Sets the entrypoint of this Users.
+
+
+        :param entrypoint: The entrypoint of this Users.  # noqa: E501
+        :type: int
+        """
+
+        self._entrypoint = entrypoint
+
+    @property
     def teams(self):
         """Gets the teams of this Users.  # noqa: E501
 
 
         :return: The teams of this Users.  # noqa: E501
         :rtype: list[UsersTeams]
         """
```

### Comparing `elabapi-python-0.2.4/elabapi_python/models/users_body.py` & `elabapi-python-0.3.0/elabapi_python/models/users_body.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,44 +29,49 @@
     """
     swagger_types = {
         'firstname': 'str',
         'lastname': 'str',
         'email': 'str',
         'team': 'int',
         'valid_until': 'str',
-        'orgid': 'str'
+        'orgid': 'str',
+        'usergroup': 'int'
     }
 
     attribute_map = {
         'firstname': 'firstname',
         'lastname': 'lastname',
         'email': 'email',
         'team': 'team',
         'valid_until': 'valid_until',
-        'orgid': 'orgid'
+        'orgid': 'orgid',
+        'usergroup': 'usergroup'
     }
 
-    def __init__(self, firstname=None, lastname=None, email=None, team=None, valid_until=None, orgid=None):  # noqa: E501
+    def __init__(self, firstname=None, lastname=None, email=None, team=None, valid_until=None, orgid=None, usergroup=None):  # noqa: E501
         """UsersBody - a model defined in Swagger"""  # noqa: E501
         self._firstname = None
         self._lastname = None
         self._email = None
         self._team = None
         self._valid_until = None
         self._orgid = None
+        self._usergroup = None
         self.discriminator = None
         self.firstname = firstname
         self.lastname = lastname
         self.email = email
         if team is not None:
             self.team = team
         if valid_until is not None:
             self.valid_until = valid_until
         if orgid is not None:
             self.orgid = orgid
+        if usergroup is not None:
+            self.usergroup = usergroup
 
     @property
     def firstname(self):
         """Gets the firstname of this UsersBody.  # noqa: E501
 
         User's first name.  # noqa: E501
 
@@ -204,14 +209,43 @@
 
         :param orgid: The orgid of this UsersBody.  # noqa: E501
         :type: str
         """
 
         self._orgid = orgid
 
+    @property
+    def usergroup(self):
+        """Gets the usergroup of this UsersBody.  # noqa: E501
+
+        Which permissions level the user will get? `1` is Sysadmin, `2` is Admin, `4` is user (default)  # noqa: E501
+
+        :return: The usergroup of this UsersBody.  # noqa: E501
+        :rtype: int
+        """
+        return self._usergroup
+
+    @usergroup.setter
+    def usergroup(self, usergroup):
+        """Sets the usergroup of this UsersBody.
+
+        Which permissions level the user will get? `1` is Sysadmin, `2` is Admin, `4` is user (default)  # noqa: E501
+
+        :param usergroup: The usergroup of this UsersBody.  # noqa: E501
+        :type: int
+        """
+        allowed_values = [1, 2, 4]  # noqa: E501
+        if usergroup not in allowed_values:
+            raise ValueError(
+                "Invalid value for `usergroup` ({0}), must be one of {1}"  # noqa: E501
+                .format(usergroup, allowed_values)
+            )
+
+        self._usergroup = usergroup
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `elabapi-python-0.2.4/elabapi_python/models/users_id_body.py` & `elabapi-python-0.3.0/elabapi_python/models/revisions_subid_body.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,35 +11,63 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class UsersIdBody(object):
+class RevisionsSubidBody(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
+        'action': 'str'
     }
 
     attribute_map = {
+        'action': 'action'
     }
 
-    def __init__(self):  # noqa: E501
-        """UsersIdBody - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, action=None):  # noqa: E501
+        """RevisionsSubidBody - a model defined in Swagger"""  # noqa: E501
+        self._action = None
         self.discriminator = None
+        if action is not None:
+            self.action = action
+
+    @property
+    def action(self):
+        """Gets the action of this RevisionsSubidBody.  # noqa: E501
+
+        The `replace` action will restore the revision body to the entity.   # noqa: E501
+
+        :return: The action of this RevisionsSubidBody.  # noqa: E501
+        :rtype: str
+        """
+        return self._action
+
+    @action.setter
+    def action(self, action):
+        """Sets the action of this RevisionsSubidBody.
+
+        The `replace` action will restore the revision body to the entity.   # noqa: E501
+
+        :param action: The action of this RevisionsSubidBody.  # noqa: E501
+        :type: str
+        """
+
+        self._action = action
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -54,15 +82,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(UsersIdBody, dict):
+        if issubclass(RevisionsSubidBody, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +98,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, UsersIdBody):
+        if not isinstance(other, RevisionsSubidBody):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `elabapi-python-0.2.4/elabapi_python/models/users_teams.py` & `elabapi-python-0.3.0/elabapi_python/models/users_teams.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python/rest.py` & `elabapi-python-0.3.0/elabapi_python/rest.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/elabapi_python.egg-info/SOURCES.txt` & `elabapi-python-0.3.0/elabapi_python.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -14,19 +14,21 @@
 elabapi_python/api/comments_api.py
 elabapi_python/api/config_api.py
 elabapi_python/api/events_api.py
 elabapi_python/api/experiments_api.py
 elabapi_python/api/experiments_templates_api.py
 elabapi_python/api/favorite_tags_api.py
 elabapi_python/api/idps_api.py
+elabapi_python/api/info_api.py
 elabapi_python/api/items_api.py
 elabapi_python/api/items_types_api.py
 elabapi_python/api/links_to_experiments_api.py
 elabapi_python/api/links_to_items_api.py
 elabapi_python/api/notifications_api.py
+elabapi_python/api/revisions_api.py
 elabapi_python/api/status_api.py
 elabapi_python/api/steps_api.py
 elabapi_python/api/tags_api.py
 elabapi_python/api/team_tags_api.py
 elabapi_python/api/teamgroups_api.py
 elabapi_python/api/teams_api.py
 elabapi_python/api/todolist_api.py
@@ -52,34 +54,41 @@
 elabapi_python/models/experiments_templates_id_body.py
 elabapi_python/models/favtags_body.py
 elabapi_python/models/id.py
 elabapi_python/models/id1.py
 elabapi_python/models/id2.py
 elabapi_python/models/id3.py
 elabapi_python/models/id_comments_body.py
+elabapi_python/models/id_revisions_body.py
 elabapi_python/models/id_status_body.py
 elabapi_python/models/id_steps_body.py
 elabapi_python/models/id_tags_body.py
 elabapi_python/models/id_teamgroups_body.py
 elabapi_python/models/id_uploads_body.py
 elabapi_python/models/idp.py
 elabapi_python/models/idps_body.py
 elabapi_python/models/idps_id_body.py
 elabapi_python/models/inline_response200.py
 elabapi_python/models/inline_response2001.py
 elabapi_python/models/inline_response2002.py
 elabapi_python/models/inline_response2003.py
+elabapi_python/models/inline_response2004.py
+elabapi_python/models/inline_response2005.py
+elabapi_python/models/inline_response2006.py
+elabapi_python/models/inline_response2007.py
 elabapi_python/models/item.py
 elabapi_python/models/items_body.py
 elabapi_python/models/items_id_body.py
 elabapi_python/models/items_links_subid_body.py
 elabapi_python/models/items_type.py
 elabapi_python/models/items_types_body.py
 elabapi_python/models/link.py
 elabapi_python/models/notification.py
+elabapi_python/models/revision.py
+elabapi_python/models/revisions_subid_body.py
 elabapi_python/models/status.py
 elabapi_python/models/step.py
 elabapi_python/models/steps_subid_body.py
 elabapi_python/models/tag.py
 elabapi_python/models/tags_subid_body.py
 elabapi_python/models/team.py
 elabapi_python/models/team_tags_body.py
@@ -92,14 +101,15 @@
 elabapi_python/models/todoitem.py
 elabapi_python/models/todolist_body.py
 elabapi_python/models/todolist_id_body.py
 elabapi_python/models/unfinished_step.py
 elabapi_python/models/unfinished_steps.py
 elabapi_python/models/upload.py
 elabapi_python/models/uploads_subid_body.py
+elabapi_python/models/uploads_subid_body1.py
 elabapi_python/models/users.py
 elabapi_python/models/users_body.py
 elabapi_python/models/users_id_body.py
 elabapi_python/models/users_teams.py
 test/__init__.py
 test/test_api_keys_api.py
 test/test_apikey.py
@@ -126,40 +136,49 @@
 test/test_favorite_tags_api.py
 test/test_favtags_body.py
 test/test_id.py
 test/test_id1.py
 test/test_id2.py
 test/test_id3.py
 test/test_id_comments_body.py
+test/test_id_revisions_body.py
 test/test_id_status_body.py
 test/test_id_steps_body.py
 test/test_id_tags_body.py
 test/test_id_teamgroups_body.py
 test/test_id_uploads_body.py
 test/test_idp.py
 test/test_idps_api.py
 test/test_idps_body.py
 test/test_idps_id_body.py
+test/test_info_api.py
 test/test_inline_response200.py
 test/test_inline_response2001.py
 test/test_inline_response2002.py
 test/test_inline_response2003.py
+test/test_inline_response2004.py
+test/test_inline_response2005.py
+test/test_inline_response2006.py
+test/test_inline_response2007.py
 test/test_item.py
 test/test_items_api.py
 test/test_items_body.py
 test/test_items_id_body.py
 test/test_items_links_subid_body.py
 test/test_items_type.py
 test/test_items_types_api.py
 test/test_items_types_body.py
 test/test_link.py
 test/test_links_to_experiments_api.py
 test/test_links_to_items_api.py
 test/test_notification.py
 test/test_notifications_api.py
+test/test_revision.py
+test/test_revisions_api.py
+test/test_revisions_subid_body.py
 test/test_status.py
 test/test_status_api.py
 test/test_step.py
 test/test_steps_api.py
 test/test_steps_subid_body.py
 test/test_tag.py
 test/test_tags_api.py
@@ -181,12 +200,13 @@
 test/test_todolist_id_body.py
 test/test_unfinished_step.py
 test/test_unfinished_steps.py
 test/test_unfinished_steps_api.py
 test/test_upload.py
 test/test_uploads_api.py
 test/test_uploads_subid_body.py
+test/test_uploads_subid_body1.py
 test/test_users.py
 test/test_users_api.py
 test/test_users_body.py
 test/test_users_id_body.py
 test/test_users_teams.py
```

### Comparing `elabapi-python-0.2.4/setup.py` & `elabapi-python-0.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "elabapi-python"
-VERSION = "0.2.4"
+VERSION = "0.3.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `elabapi-python-0.2.4/test/test_api_keys_api.py` & `elabapi-python-0.3.0/test/test_api_keys_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_apikey.py` & `elabapi-python-0.3.0/test/test_apikey.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_apikeys_body.py` & `elabapi-python-0.3.0/test/test_apikeys_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_comment.py` & `elabapi-python-0.3.0/test/test_comment.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_comments_api.py` & `elabapi-python-0.3.0/test/test_comments_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_config.py` & `elabapi-python-0.3.0/test/test_config.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_config_api.py` & `elabapi-python-0.3.0/test/test_config_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_entity.py` & `elabapi-python-0.3.0/test/test_entity.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_event.py` & `elabapi-python-0.3.0/test/test_event.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_events_api.py` & `elabapi-python-0.3.0/test/test_events_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_events_id_body.py` & `elabapi-python-0.3.0/test/test_events_id_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_events_id_body1.py` & `elabapi-python-0.3.0/test/test_events_id_body1.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_eventsid_delta.py` & `elabapi-python-0.3.0/test/test_eventsid_delta.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_experiment.py` & `elabapi-python-0.3.0/test/test_experiment.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_experiment_template.py` & `elabapi-python-0.3.0/test/test_experiment_template.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_experiments_api.py` & `elabapi-python-0.3.0/test/test_experiments_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_experiments_body.py` & `elabapi-python-0.3.0/test/test_experiments_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_experiments_id_body.py` & `elabapi-python-0.3.0/test/test_experiments_id_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_experiments_links_subid_body.py` & `elabapi-python-0.3.0/test/test_experiments_links_subid_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_experiments_templates_api.py` & `elabapi-python-0.3.0/test/test_experiments_templates_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_experiments_templates_body.py` & `elabapi-python-0.3.0/test/test_experiments_templates_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_experiments_templates_id_body.py` & `elabapi-python-0.3.0/test/test_experiments_templates_id_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_favorite_tags_api.py` & `elabapi-python-0.3.0/test/test_favorite_tags_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_favtags_body.py` & `elabapi-python-0.3.0/test/test_favtags_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_id.py` & `elabapi-python-0.3.0/test/test_id.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_id1.py` & `elabapi-python-0.3.0/test/test_id1.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_id2.py` & `elabapi-python-0.3.0/test/test_id2.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_id3.py` & `elabapi-python-0.3.0/test/test_id3.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_id_comments_body.py` & `elabapi-python-0.3.0/test/test_id_comments_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_id_status_body.py` & `elabapi-python-0.3.0/test/test_id_status_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_id_steps_body.py` & `elabapi-python-0.3.0/test/test_id_steps_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_id_tags_body.py` & `elabapi-python-0.3.0/test/test_id_tags_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_id_teamgroups_body.py` & `elabapi-python-0.3.0/test/test_id_teamgroups_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_id_uploads_body.py` & `elabapi-python-0.3.0/test/test_id_uploads_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_idp.py` & `elabapi-python-0.3.0/test/test_idp.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_idps_api.py` & `elabapi-python-0.3.0/test/test_idps_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_idps_body.py` & `elabapi-python-0.3.0/test/test_idps_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_idps_id_body.py` & `elabapi-python-0.3.0/test/test_idps_id_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_inline_response200.py` & `elabapi-python-0.3.0/test/test_inline_response200.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_inline_response2001.py` & `elabapi-python-0.3.0/test/test_inline_response2001.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_inline_response2002.py` & `elabapi-python-0.3.0/test/test_inline_response2002.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_inline_response2003.py` & `elabapi-python-0.3.0/test/test_inline_response2003.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_item.py` & `elabapi-python-0.3.0/test/test_item.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_items_api.py` & `elabapi-python-0.3.0/test/test_items_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_items_body.py` & `elabapi-python-0.3.0/test/test_items_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_items_id_body.py` & `elabapi-python-0.3.0/test/test_items_id_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_items_links_subid_body.py` & `elabapi-python-0.3.0/test/test_items_links_subid_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_items_type.py` & `elabapi-python-0.3.0/test/test_items_type.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_items_types_api.py` & `elabapi-python-0.3.0/test/test_items_types_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_items_types_body.py` & `elabapi-python-0.3.0/test/test_items_types_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_link.py` & `elabapi-python-0.3.0/test/test_link.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_links_to_experiments_api.py` & `elabapi-python-0.3.0/test/test_links_to_experiments_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_links_to_items_api.py` & `elabapi-python-0.3.0/test/test_links_to_items_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_notification.py` & `elabapi-python-0.3.0/test/test_notification.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_notifications_api.py` & `elabapi-python-0.3.0/test/test_notifications_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_status.py` & `elabapi-python-0.3.0/test/test_status.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_status_api.py` & `elabapi-python-0.3.0/test/test_status_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_step.py` & `elabapi-python-0.3.0/test/test_step.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_steps_api.py` & `elabapi-python-0.3.0/test/test_steps_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_steps_subid_body.py` & `elabapi-python-0.3.0/test/test_steps_subid_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_tag.py` & `elabapi-python-0.3.0/test/test_tag.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_tags_api.py` & `elabapi-python-0.3.0/test/test_tags_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_tags_subid_body.py` & `elabapi-python-0.3.0/test/test_tags_subid_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_team.py` & `elabapi-python-0.3.0/test/test_team.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_team_tags_api.py` & `elabapi-python-0.3.0/test/test_team_tags_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_team_tags_body.py` & `elabapi-python-0.3.0/test/test_team_tags_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_team_tags_body1.py` & `elabapi-python-0.3.0/test/test_team_tags_body1.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_team_tags_id_body.py` & `elabapi-python-0.3.0/test/test_team_tags_id_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_teamgroup.py` & `elabapi-python-0.3.0/test/test_teamgroup.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_teamgroup_users.py` & `elabapi-python-0.3.0/test/test_teamgroup_users.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_teamgroups_api.py` & `elabapi-python-0.3.0/test/test_teamgroups_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_teamgroups_subid_body.py` & `elabapi-python-0.3.0/test/test_teamgroups_subid_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_teams_api.py` & `elabapi-python-0.3.0/test/test_teams_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_teams_body.py` & `elabapi-python-0.3.0/test/test_teams_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_todoitem.py` & `elabapi-python-0.3.0/test/test_todoitem.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_todolist_api.py` & `elabapi-python-0.3.0/test/test_todolist_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_todolist_body.py` & `elabapi-python-0.3.0/test/test_todolist_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_todolist_id_body.py` & `elabapi-python-0.3.0/test/test_todolist_id_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_unfinished_step.py` & `elabapi-python-0.3.0/test/test_unfinished_step.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_unfinished_steps.py` & `elabapi-python-0.3.0/test/test_unfinished_steps.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_unfinished_steps_api.py` & `elabapi-python-0.3.0/test/test_unfinished_steps_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_upload.py` & `elabapi-python-0.3.0/test/test_upload.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_uploads_api.py` & `elabapi-python-0.3.0/test/test_uploads_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         Delete an upload.  # noqa: E501
         """
         pass
 
     def test_patch_upload(self):
         """Test case for patch_upload
 
-        Actions on an upload.   # noqa: E501
+        Modify attributes such as \"real_name\", \"comment\" or \"state\" of an upload.   # noqa: E501
         """
         pass
 
     def test_post_upload(self):
         """Test case for post_upload
 
         Create an upload.  # noqa: E501
```

### Comparing `elabapi-python-0.2.4/test/test_uploads_subid_body.py` & `elabapi-python-0.3.0/test/test_uploads_subid_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_users.py` & `elabapi-python-0.3.0/test/test_users.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_users_api.py` & `elabapi-python-0.3.0/test/test_users_api.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_users_body.py` & `elabapi-python-0.3.0/test/test_users_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_users_id_body.py` & `elabapi-python-0.3.0/test/test_users_id_body.py`

 * *Files identical despite different names*

### Comparing `elabapi-python-0.2.4/test/test_users_teams.py` & `elabapi-python-0.3.0/test/test_users_teams.py`

 * *Files identical despite different names*

